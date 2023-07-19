# Comparing `tmp/sunsynk-0.3.6.tar.gz` & `tmp/sunsynk-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sunsynk-0.3.6.tar", last modified: Fri May 19 13:27:21 2023, max compression
+gzip compressed data, was "sunsynk-0.3.7.tar", last modified: Wed Jul 19 12:53:30 2023, max compression
```

## Comparing `sunsynk-0.3.6.tar` & `sunsynk-0.3.7.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:27:21.837749 sunsynk-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-19 13:27:10.000000 sunsynk-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-19 13:27:10.000000 sunsynk-0.3.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-19 13:27:21.837749 sunsynk-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-19 13:27:10.000000 sunsynk-0.3.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-19 13:27:21.837749 sunsynk-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-19 13:27:10.000000 sunsynk-0.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:27:21.833749 sunsynk-0.3.6/sunsynk/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-19 13:27:10.000000 sunsynk-0.3.6/sunsynk/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11717 2023-05-19 13:27:10.000000 sunsynk-0.3.6/sunsynk/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12189 2023-05-19 13:27:10.000000 sunsynk-0.3.6/sunsynk/definitions3ph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-19 13:27:10.000000 sunsynk-0.3.6/sunsynk/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-19 13:27:10.000000 sunsynk-0.3.6/sunsynk/pysunsynk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8147 2023-05-19 13:27:10.000000 sunsynk-0.3.6/sunsynk/rwsensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-05-19 13:27:10.000000 sunsynk-0.3.6/sunsynk/sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-05-19 13:27:10.000000 sunsynk-0.3.6/sunsynk/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-19 13:27:10.000000 sunsynk-0.3.6/sunsynk/sunsynk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-19 13:27:10.000000 sunsynk-0.3.6/sunsynk/usunsynk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:27:21.833749 sunsynk-0.3.6/sunsynk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-19 13:27:21.000000 sunsynk-0.3.6/sunsynk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-19 13:27:21.000000 sunsynk-0.3.6/sunsynk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 13:27:21.000000 sunsynk-0.3.6/sunsynk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-19 13:27:21.000000 sunsynk-0.3.6/sunsynk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-19 13:27:21.000000 sunsynk-0.3.6/sunsynk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 13:27:21.000000 sunsynk-0.3.6/sunsynk.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:27:21.833749 sunsynk-0.3.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-19 13:27:10.000000 sunsynk-0.3.6/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:27:10.000000 sunsynk-0.3.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-19 13:27:10.000000 sunsynk-0.3.6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-05-19 13:27:10.000000 sunsynk-0.3.6/tests/hass-addon-sunsynk-dev.zip
--rw-r--r--   0 runner    (1001) docker     (123)    14052 2023-05-19 13:27:10.000000 sunsynk-0.3.6/tests/hass-addon-sunsynk.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:27:21.833749 sunsynk-0.3.6/tests/hass_addon_sunsynk_multi/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-19 13:27:10.000000 sunsynk-0.3.6/tests/hass_addon_sunsynk_multi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-19 13:27:10.000000 sunsynk-0.3.6/tests/hass_addon_sunsynk_multi/test_definitions3ph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-05-19 13:27:10.000000 sunsynk-0.3.6/tests/hass_addon_sunsynk_multi/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-19 13:27:10.000000 sunsynk-0.3.6/tests/hass_addon_sunsynk_multi/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-19 13:27:10.000000 sunsynk-0.3.6/tests/hass_addon_sunsynk_multi/test_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-19 13:27:10.000000 sunsynk-0.3.6/tests/hass_addon_sunsynk_multi/test_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:27:21.837749 sunsynk-0.3.6/tests/sunsynk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:27:10.000000 sunsynk-0.3.6/tests/sunsynk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-19 13:27:10.000000 sunsynk-0.3.6/tests/sunsynk/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-19 13:27:10.000000 sunsynk-0.3.6/tests/sunsynk/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-05-19 13:27:10.000000 sunsynk-0.3.6/tests/sunsynk/test_pysunsynk.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-19 13:27:10.000000 sunsynk-0.3.6/tests/sunsynk/test_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-05-19 13:27:10.000000 sunsynk-0.3.6/tests/sunsynk/test_rwsensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-05-19 13:27:10.000000 sunsynk-0.3.6/tests/sunsynk/test_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-19 13:27:10.000000 sunsynk-0.3.6/tests/sunsynk/test_sunsynk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-19 13:27:10.000000 sunsynk-0.3.6/tests/sunsynk/test_usunsynk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:53:30.366794 sunsynk-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-19 12:53:21.000000 sunsynk-0.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-19 12:53:21.000000 sunsynk-0.3.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-07-19 12:53:30.366794 sunsynk-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-07-19 12:53:21.000000 sunsynk-0.3.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-19 12:53:30.366794 sunsynk-0.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-19 12:53:21.000000 sunsynk-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:53:30.366794 sunsynk-0.3.7/sunsynk/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-19 12:53:21.000000 sunsynk-0.3.7/sunsynk/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11717 2023-07-19 12:53:21.000000 sunsynk-0.3.7/sunsynk/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12189 2023-07-19 12:53:21.000000 sunsynk-0.3.7/sunsynk/definitions3ph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-07-19 12:53:21.000000 sunsynk-0.3.7/sunsynk/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-07-19 12:53:21.000000 sunsynk-0.3.7/sunsynk/pysunsynk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8207 2023-07-19 12:53:21.000000 sunsynk-0.3.7/sunsynk/rwsensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-07-19 12:53:21.000000 sunsynk-0.3.7/sunsynk/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-19 12:53:21.000000 sunsynk-0.3.7/sunsynk/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-07-19 12:53:21.000000 sunsynk-0.3.7/sunsynk/sunsynk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-19 12:53:21.000000 sunsynk-0.3.7/sunsynk/usunsynk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:53:30.366794 sunsynk-0.3.7/sunsynk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-07-19 12:53:30.000000 sunsynk-0.3.7/sunsynk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-19 12:53:30.000000 sunsynk-0.3.7/sunsynk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 12:53:30.000000 sunsynk-0.3.7/sunsynk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-19 12:53:30.000000 sunsynk-0.3.7/sunsynk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-19 12:53:30.000000 sunsynk-0.3.7/sunsynk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 12:53:30.000000 sunsynk-0.3.7/sunsynk.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:53:30.366794 sunsynk-0.3.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-19 12:53:21.000000 sunsynk-0.3.7/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:53:21.000000 sunsynk-0.3.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-19 12:53:21.000000 sunsynk-0.3.7/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-07-19 12:53:21.000000 sunsynk-0.3.7/tests/hass-addon-sunsynk-dev.zip
+-rw-r--r--   0 runner    (1001) docker     (123)    14052 2023-07-19 12:53:21.000000 sunsynk-0.3.7/tests/hass-addon-sunsynk.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:53:30.366794 sunsynk-0.3.7/tests/hass_addon_sunsynk_multi/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-19 12:53:21.000000 sunsynk-0.3.7/tests/hass_addon_sunsynk_multi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-19 12:53:21.000000 sunsynk-0.3.7/tests/hass_addon_sunsynk_multi/test_definitions3ph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-07-19 12:53:21.000000 sunsynk-0.3.7/tests/hass_addon_sunsynk_multi/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-19 12:53:21.000000 sunsynk-0.3.7/tests/hass_addon_sunsynk_multi/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-19 12:53:21.000000 sunsynk-0.3.7/tests/hass_addon_sunsynk_multi/test_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-19 12:53:21.000000 sunsynk-0.3.7/tests/hass_addon_sunsynk_multi/test_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:53:30.366794 sunsynk-0.3.7/tests/sunsynk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:53:21.000000 sunsynk-0.3.7/tests/sunsynk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-19 12:53:21.000000 sunsynk-0.3.7/tests/sunsynk/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-19 12:53:21.000000 sunsynk-0.3.7/tests/sunsynk/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-07-19 12:53:21.000000 sunsynk-0.3.7/tests/sunsynk/test_pysunsynk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-19 12:53:21.000000 sunsynk-0.3.7/tests/sunsynk/test_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-07-19 12:53:21.000000 sunsynk-0.3.7/tests/sunsynk/test_rwsensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-07-19 12:53:21.000000 sunsynk-0.3.7/tests/sunsynk/test_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-07-19 12:53:21.000000 sunsynk-0.3.7/tests/sunsynk/test_sunsynk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-19 12:53:21.000000 sunsynk-0.3.7/tests/sunsynk/test_usunsynk.py
```

### Comparing `sunsynk-0.3.6/LICENSE` & `sunsynk-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.6/PKG-INFO` & `sunsynk-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sunsynk
-Version: 0.3.6
+Version: 0.3.7
 Summary: Library to interface Deye/Sunsynk Hybrid Inverters
 Home-page: https://kellerza.github.io/sunsynk/
 Author: Johann Kellerman
 Author-email: kellerza@gmail.com
 License: MIT
 Keywords: sunsynk,deye,inverter,modbus,asyncio
 Classifier: Development Status :: 4 - Beta
```

### Comparing `sunsynk-0.3.6/README.md` & `sunsynk-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.6/setup.cfg` & `sunsynk-0.3.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.6/sunsynk/definitions.py` & `sunsynk-0.3.7/sunsynk/definitions.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.6/sunsynk/definitions3ph.py` & `sunsynk-0.3.7/sunsynk/definitions3ph.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.6/sunsynk/helpers.py` & `sunsynk-0.3.7/sunsynk/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     except ValueError as err:
         _LOGGER.error(str(err))
     return 0
 
 
 def signed(val: Union[int, float]) -> Union[int, float]:
     """Convert 16-bit value to signed int."""
-    return val if val <= 0x7FFF else val - 0xFFFF
+    return val if val <= 0x7FFF else val - 0x10000
 
 
 def slug(name: str) -> str:
     """Create a slug."""
     return name.lower().replace(" ", "_").replace("-", "_")
```

### Comparing `sunsynk-0.3.6/sunsynk/pysunsynk.py` & `sunsynk-0.3.7/sunsynk/pysunsynk.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Sunsync Modbus interface."""
 import asyncio
 import logging
-from typing import Sequence
+from typing import Any, Sequence
 from urllib.parse import urlparse
 
 import attrs
 from pymodbus import version
 from pymodbus.client import (
     AsyncModbusSerialClient,
     AsyncModbusTcpClient,
     ModbusBaseClient,
 )
+from pymodbus.transaction import ModbusRtuFramer
 
 from sunsynk.sunsynk import Sunsynk
 
 _LOGGER = logging.getLogger(__name__)
 
 
 @attrs.define
@@ -24,16 +25,28 @@
     client: ModbusBaseClient = None  # type:ignore
 
     def _new_client(self) -> ModbusBaseClient:
         """Create a new client."""
         url = urlparse(f"{self.port}")
         if url.hostname:
             host, port = url.hostname, url.port or 502
-            _LOGGER.info("PyModbus %s TCP: %s:%s", version.short(), host, port)
-            return AsyncModbusTcpClient(host=host, port=port)
+
+            # Framer from the URL scheme
+            opt: dict[str, Any] = {}
+            if url.scheme == "serial-tcp":
+                opt = {"framer": ModbusRtuFramer}
+            elif url.scheme != "tcp":  # default ModbusSocketFramer
+                raise NotImplementedError(
+                    "Unknown scheme {url.scheme}: Only tcp and serial-tcp are supported"
+                )
+
+            _LOGGER.info(
+                "PyModbus %s %s: %s:%s", version.short(), url.scheme, host, port
+            )
+            return AsyncModbusTcpClient(host=host, port=port, **opt)
 
         _LOGGER.info("PyModbus %s Serial: %s", version.short(), self.port)
         return AsyncModbusSerialClient(
             port=self.port,
             baudrate=self.baudrate,
             # method="rtu",
             stopbits=1,
@@ -57,15 +70,15 @@
         try:
             res = await self.client.write_registers(  # type:ignore
                 address=address, values=[value], slave=self.server_id
             )
             if res.function_code < 0x80:  # test that we are not an error
                 return True
             _LOGGER.error("failed to write register %s=%s", address, value)
-        except asyncio.TimeoutError:
+        except (asyncio.TimeoutError, TimeoutError):
             _LOGGER.error("timeout writing register %s=%s", address, value)
         self.timeouts += 1
         return False
 
     async def read_holding_registers(self, start: int, length: int) -> Sequence[int]:
         """Read a holding register."""
         await self.connect()
```

### Comparing `sunsynk-0.3.6/sunsynk/rwsensors.py` & `sunsynk-0.3.7/sunsynk/rwsensors.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,16 @@
     def value_to_reg(self, value: ValType, resolve: ResolveType) -> RegType:
         """Get the reg value from a display value, or the current reg value if out of range."""
         fval = float(value)  # type:ignore
         minv = resolve_num(resolve, self.min, 0)
         maxv = resolve_num(resolve, self.max, 100)
         val = int(max(minv, min(maxv, fval / abs(self.factor))))
         if len(self.address) == 1:
+            if val < 0:
+                val = 0x10000 + val
             return self.reg(val)
         if len(self.address) == 2:
             return self.reg(val & 0xFFFF, int(val >> 16))
         raise NotImplementedError
 
 
 @attrs.define(slots=True, eq=False)
```

### Comparing `sunsynk-0.3.6/sunsynk/sensors.py` & `sunsynk-0.3.7/sunsynk/sensors.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.6/sunsynk/state.py` & `sunsynk-0.3.7/sunsynk/state.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.6/sunsynk/sunsynk.py` & `sunsynk-0.3.7/sunsynk/sunsynk.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.6/sunsynk/usunsynk.py` & `sunsynk-0.3.7/sunsynk/usunsynk.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.6/sunsynk.egg-info/PKG-INFO` & `sunsynk-0.3.7/sunsynk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sunsynk
-Version: 0.3.6
+Version: 0.3.7
 Summary: Library to interface Deye/Sunsynk Hybrid Inverters
 Home-page: https://kellerza.github.io/sunsynk/
 Author: Johann Kellerman
 Author-email: kellerza@gmail.com
 License: MIT
 Keywords: sunsynk,deye,inverter,modbus,asyncio
 Classifier: Development Status :: 4 - Beta
```

### Comparing `sunsynk-0.3.6/sunsynk.egg-info/SOURCES.txt` & `sunsynk-0.3.7/sunsynk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.6/tests/conftest.py` & `sunsynk-0.3.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.6/tests/hass-addon-sunsynk-dev.zip` & `sunsynk-0.3.7/tests/hass-addon-sunsynk-dev.zip`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.6/tests/hass-addon-sunsynk.zip` & `sunsynk-0.3.7/tests/hass-addon-sunsynk.zip`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.6/tests/hass_addon_sunsynk_multi/test_filter.py` & `sunsynk-0.3.7/tests/hass_addon_sunsynk_multi/test_filter.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.6/tests/hass_addon_sunsynk_multi/test_run.py` & `sunsynk-0.3.7/tests/hass_addon_sunsynk_multi/test_run.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.6/tests/hass_addon_sunsynk_multi/test_sensors.py` & `sunsynk-0.3.7/tests/hass_addon_sunsynk_multi/test_sensors.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.6/tests/hass_addon_sunsynk_multi/test_state.py` & `sunsynk-0.3.7/tests/hass_addon_sunsynk_multi/test_state.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.6/tests/sunsynk/test_helpers.py` & `sunsynk-0.3.7/tests/sunsynk/test_helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,22 +32,26 @@
     res1 = int_round(1.0)
     assert isinstance(res1, int)
     assert res1 == 1
 
 
 def test_signed() -> None:
     assert signed(0x7FFF) == 0x7FFF
-    assert signed(0xFFFF) == 0
+    assert signed(0xFFFF) == -1
+    assert signed(0) == 0
+    assert signed(32767) == 32767
+    assert signed(32768) == -32768
 
 
 def test_signeds() -> None:
     """Signed sensors have a -1 factor"""
     s = Sensor(1, "", "", factor=-1)
     assert s.reg_to_value((1,)) == 1
-    assert s.reg_to_value((0xFFFE,)) == -1
+    assert s.reg_to_value((0xFFFE,)) == -2
+    assert s.reg_to_value((0xFFBA,)) == -70
 
     s = Sensor(1, "", "", factor=1)
     assert s.reg_to_value((1,)) == 1
     assert s.reg_to_value((0xFFFE,)) == 0xFFFE
     assert s.reg_to_value((1, 1)) == 0x10001
```

### Comparing `sunsynk-0.3.6/tests/sunsynk/test_pysunsynk.py` & `sunsynk-0.3.7/tests/sunsynk/test_pysunsynk.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,38 @@
 """PyModbus."""
-from unittest.mock import AsyncMock, MagicMock, PropertyMock, patch
+import asyncio
+from unittest.mock import AsyncMock, MagicMock, PropertyMock, call, patch
 
 import pytest
 
-from sunsynk.pysunsynk import pySunsynk
+from sunsynk.pysunsynk import ModbusRtuFramer, pySunsynk
 from sunsynk.state import InverterState
 
 
 @pytest.mark.asyncio
 async def test_pyss():
     ss = pySunsynk()
     with pytest.raises(ConnectionError):
         await ss.connect()
 
+    ss.client = None
+    with pytest.raises(NotImplementedError):
+        ss.port = "xcp://localhost:10"
+        await ss.connect()
+
+    with patch("sunsynk.pysunsynk.AsyncModbusTcpClient") as client:
+        client.return_value = MagicMock()
+        ss.port = "serial-tcp://localhost:10"
+        assert client.call_args_list == []
+        await ss.connect()
+        assert client.call_args_list == [
+            call(host="localhost", port=10, framer=ModbusRtuFramer)
+        ]
+        assert ss.client is not None
+
 
 P_ASYNC_CONNECTED = "sunsynk.pysunsynk.AsyncModbusTcpClient.async_connected"
 P_CONNECT = "sunsynk.pysunsynk.AsyncModbusTcpClient.connect"
 P_READ_HR = "sunsynk.pysunsynk.AsyncModbusTcpClient.read_holding_registers"
 P_WRITE_REGS = "sunsynk.pysunsynk.AsyncModbusTcpClient.write_registers"
 
 
@@ -88,14 +104,15 @@
 @patch(P_CONNECT, new_callable=AsyncMock)
 @patch(P_WRITE_REGS, new_callable=AsyncMock)
 async def test_ss_tcp_write(
     write_registers: AsyncMock,
     _connect: AsyncMock,
     async_connect: PropertyMock,
     state: InverterState,
+    caplog,
 ):
     ss = pySunsynk(port="tcp://1.1.1.1")
     ss.state = state
 
     # Ensure we can write
     async_connect.return_value = 1
 
@@ -103,16 +120,26 @@
     write_registers.return_value = wrr = MagicMock()
     wrr.function_code = 0
     res = await ss.write_register(address=1, value=1)
     assert res is True
 
     # some error during read
     wrr.function_code = 0x100
+    assert "failed" not in caplog.text
+    res = await ss.write_register(address=1, value=1)
+    assert res is False
+    assert "failed" in caplog.text
+
+    # Timeout
+    write_registers.return_value = None
+    write_registers.side_effect = asyncio.TimeoutError
+    assert "timeout writing" not in caplog.text
     res = await ss.write_register(address=1, value=1)
     assert res is False
+    assert "timeout writing" in caplog.text
 
 
 @pytest.mark.asyncio
 @patch("sunsynk.pysunsynk.AsyncModbusSerialClient", async_connected=PropertyMock)
 async def test_ss_serial(serialc: MagicMock, state: InverterState):
     ss = pySunsynk(port="/dev/tty0")
     ss.state = state
```

### Comparing `sunsynk-0.3.6/tests/sunsynk/test_register.py` & `sunsynk-0.3.7/tests/sunsynk/test_register.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.6/tests/sunsynk/test_rwsensors.py` & `sunsynk-0.3.7/tests/sunsynk/test_rwsensors.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,14 +86,18 @@
     state.update({1: 500})
     assert state[s] == 500  # does not take min/max into account!
 
     assert s.value_to_reg(200, state.get) == (200,)
     assert s.value_to_reg(500, state.get) == (300,)
     assert s.value_to_reg(-1, state.get) == (1,)
 
+    # writing negative values (when allowed by min)
+    s.min = -10
+    assert s.value_to_reg(-1, state.get) == (65535,)
+
     s = NumberRWSensor(1, "s2", factor=0.01)
     state.track(s)
 
     state.update({1: 4850})
     assert state.registers[1] == 4850
     assert state[s] == 48.5
```

### Comparing `sunsynk-0.3.6/tests/sunsynk/test_sensors.py` & `sunsynk-0.3.7/tests/sunsynk/test_sensors.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.6/tests/sunsynk/test_sunsynk.py` & `sunsynk-0.3.7/tests/sunsynk/test_sunsynk.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.6/tests/sunsynk/test_usunsynk.py` & `sunsynk-0.3.7/tests/sunsynk/test_usunsynk.py`

 * *Files identical despite different names*

