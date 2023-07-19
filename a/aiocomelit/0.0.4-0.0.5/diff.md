# Comparing `tmp/aiocomelit-0.0.4.tar.gz` & `tmp/aiocomelit-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiocomelit-0.0.4.tar", max compression
+gzip compressed data, was "aiocomelit-0.0.5.tar", max compression
```

## Comparing `aiocomelit-0.0.4.tar` & `aiocomelit-0.0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11346 2023-07-04 19:31:04.621003 aiocomelit-0.0.4/LICENSE
--rw-r--r--   0        0        0     3306 2023-07-04 19:31:04.721003 aiocomelit-0.0.4/README.md
--rw-r--r--   0        0        0     1940 2023-07-14 17:48:38.640530 aiocomelit-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      420 2023-07-14 17:48:38.640530 aiocomelit-0.0.4/src/aiocomelit/__init__.py
--rw-r--r--   0        0        0     9639 2023-07-14 17:43:51.602105 aiocomelit-0.0.4/src/aiocomelit/api.py
--rw-r--r--   0        0        0      428 2023-07-14 17:43:51.602105 aiocomelit-0.0.4/src/aiocomelit/const.py
--rw-r--r--   0        0        0      441 2023-07-05 21:05:53.271526 aiocomelit-0.0.4/src/aiocomelit/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-04 19:31:04.451003 aiocomelit-0.0.4/src/aiocomelit/py.typed
--rw-r--r--   0        0        0     4322 1970-01-01 00:00:00.000000 aiocomelit-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-07-04 19:31:04.621003 aiocomelit-0.0.5/LICENSE
+-rw-r--r--   0        0        0     3306 2023-07-04 19:31:04.721003 aiocomelit-0.0.5/README.md
+-rw-r--r--   0        0        0     1940 2023-07-19 13:08:35.709527 aiocomelit-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      420 2023-07-19 13:08:35.709527 aiocomelit-0.0.5/src/aiocomelit/__init__.py
+-rw-r--r--   0        0        0    10023 2023-07-19 12:57:26.968052 aiocomelit-0.0.5/src/aiocomelit/api.py
+-rw-r--r--   0        0        0      428 2023-07-14 17:43:51.602105 aiocomelit-0.0.5/src/aiocomelit/const.py
+-rw-r--r--   0        0        0      441 2023-07-05 21:05:53.271526 aiocomelit-0.0.5/src/aiocomelit/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-04 19:31:04.451003 aiocomelit-0.0.5/src/aiocomelit/py.typed
+-rw-r--r--   0        0        0     4322 1970-01-01 00:00:00.000000 aiocomelit-0.0.5/PKG-INFO
```

### Comparing `aiocomelit-0.0.4/LICENSE` & `aiocomelit-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aiocomelit-0.0.4/README.md` & `aiocomelit-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `aiocomelit-0.0.4/pyproject.toml` & `aiocomelit-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiocomelit"
-version = "0.0.4"
+version = "0.0.5"
 description = "Python library to control Comelit Simplehome"
 authors = ["Simone Chemelli <simone.chemelli@gmail.com>"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 repository = "https://github.com/chemelli74/aiocomelit"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
```

### Comparing `aiocomelit-0.0.4/src/aiocomelit/api.py` & `aiocomelit-0.0.5/src/aiocomelit/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,16 +68,16 @@
             "Accept-Language": "en-GB,en;q=0.5",
             "Origin": self.base_url,
             "Referer": f"{self.base_url}/",
         }
         jar = aiohttp.CookieJar(unsafe=True)
         self.session = aiohttp.ClientSession(cookie_jar=jar)
         self._unique_id: str | None = None
-        self._devices: list[ComelitSerialBridgeObject] = []
-        self._alarm: list[ComelitVedoObject] = []
+        self._devices: dict[str, dict[int, ComelitSerialBridgeObject]] = {}
+        self._alarm: dict[str, dict[int, ComelitVedoObject]] = {}
         self._alarm_logged: bool = False
 
     async def _get_devices(self, device_type: str) -> dict[str, Any]:
         """Get devices description."""
         timestamp = datetime.now().strftime("%s")
         url = f"{self.base_url}/user/icon_desc.json?type={device_type}&_={timestamp}"
         response = await self.session.get(
@@ -122,25 +122,26 @@
         """Enable required session cookie."""
         self.session.cookie_jar.update_cookies(
             SimpleCookie(f"domain={self.host}; name=sid; value=1;")
         )
 
     async def _do_alarm_login(self) -> bool:
         """Login into VEDO system via Comelit Serial Bridge."""
-        if self._alarm_logged:
-            return True
-
         payload = {"alm": self.alarm_pin}
         url = f"{self.base_url}/login.cgi"
         response = await self.session.post(
             url,
             data=payload,
             headers=self.headers,
             timeout=10,
         )
+        if "sid" not in response.cookies:
+            _LOGGER.debug('No "sid" cookie in VEDO login response for %s', self.host)
+            return False
+
         await self._set_cookie(response.cookies["sid"])
 
         return response.status == 200
 
     async def _get_alarm_desc(self) -> dict[str, Any]:
         """Get alarm description for VEDO system."""
         timestamp = datetime.now().strftime("%s")
@@ -199,70 +200,74 @@
         return await self._set_device_status(COVER, index, action)
 
     async def cover_status(self, index: int) -> int:
         """Get cover status."""
         await asyncio.sleep(SLEEP)
         return await self._get_device_status(COVER, index)
 
-    async def get_all_devices(self) -> list[ComelitSerialBridgeObject]:
+    async def get_all_devices(self) -> dict[str, dict[int, ComelitSerialBridgeObject]]:
         """Get all connected devices."""
 
         _LOGGER.debug("Getting all devices for host %s", self.host)
 
         for dev_type in (CLIMATE, COVER, LIGHT, OTHER):
             reply_json = await self._get_devices(dev_type)
             _LOGGER.debug(
                 "List of devices of type %s: %s",
                 dev_type,
                 reply_json,
             )
+            devices = {}
             for i in range(reply_json["num"]):
                 status = reply_json["status"][i]
                 dev_info = ComelitSerialBridgeObject(
                     index=i,
                     name=reply_json["desc"][i],
                     status=status,
                     human_status=await self._translate_device_status(dev_type, status),
                     type=dev_type,
                     val=reply_json["val"][i],
                     protected=reply_json["protected"][i],
                     zone=reply_json["env_desc"][reply_json["env"][i]],
                 )
-                self._devices.append(dev_info)
+                devices.update({i: dev_info})
+            self._devices.update({dev_type: devices})
 
         return self._devices
 
     async def alarm_login(self) -> bool:
         """Login to vedo alarm system."""
         _LOGGER.debug("Logging into %s (VEDO)", self.host)
         try:
             self._alarm_logged = await self._do_alarm_login()
         except (asyncio.exceptions.TimeoutError, aiohttp.ClientConnectorError) as exc:
             _LOGGER.warning("Connection error for %s", self.host)
             raise CannotConnect from exc
 
         if not self._alarm_logged:
+            _LOGGER.warning("Authentication failed for %s (VEDO)", self.host)
             raise CannotAuthenticate
 
         await asyncio.sleep(SLEEP)
         return True
 
-    async def get_alarm_config(self) -> list[ComelitVedoObject]:
+    async def get_alarm_config(self) -> dict[str, dict[int, ComelitVedoObject]]:
         """Get Comelit SimpleHome alarm configuration."""
 
         await self.alarm_login()
 
         reply_json_desc = await self._get_alarm_desc()
         _LOGGER.debug("Alarm description: %s", reply_json_desc)
         reply_json_stat = await self._get_alarm_stat()
         _LOGGER.debug("Alarm statistics: %s", reply_json_stat)
 
         if (reply_json_desc or reply_json_stat) is {}:
-            return []
+            return {}
 
+        alarms = {}
         for i in range(MAX_ZONES):
             if reply_json_desc["description"][i] == "":
                 continue
             vedo = ComelitVedoObject(
                 index=i,
                 name=reply_json_desc["description"][i],
                 p1=reply_json_desc["p1_pres"][i],
@@ -273,15 +278,16 @@
                 alarm=reply_json_stat["alarm"][i],
                 alarm_memory=reply_json_stat["alarm_memory"][i],
                 sabotage=reply_json_stat["sabotage"][i],
                 anomaly=reply_json_stat["anomaly"][i],
                 in_time=reply_json_stat["in_time"][i],
                 out_time=reply_json_stat["out_time"][i],
             )
-            self._alarm.append(vedo)
+            alarms.update({i: vedo})
+        self._alarm.update({"alarm": alarms})
 
         return self._alarm
 
     async def logout(self) -> None:
         """Comelit Simple Home Serial bridge logout."""
         self.session.cookie_jar.clear()
```

### Comparing `aiocomelit-0.0.4/PKG-INFO` & `aiocomelit-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiocomelit
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python library to control Comelit Simplehome
 Home-page: https://github.com/chemelli74/aiocomelit
 License: Apache Software License 2.0
 Author: Simone Chemelli
 Author-email: simone.chemelli@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aiocomelit Version: 0.0.4 Summary: Python library
+Metadata-Version: 2.1 Name: aiocomelit Version: 0.0.5 Summary: Python library
 to control Comelit Simplehome Home-page: https://github.com/chemelli74/
 aiocomelit License: Apache Software License 2.0 Author: Simone Chemelli Author-
 email: simone.chemelli@gmail.com Requires-Python: >=3.10,<4.0 Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License Classifier: Natural Language
 :: English Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```

