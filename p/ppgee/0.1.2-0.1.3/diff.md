# Comparing `tmp/ppgee-0.1.2.tar.gz` & `tmp/ppgee-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ppgee-0.1.2.tar", max compression
+gzip compressed data, was "ppgee-0.1.3.tar", max compression
```

## Comparing `ppgee-0.1.2.tar` & `ppgee-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0       49 2022-10-04 06:09:48.466579 ppgee-0.1.2/ppgee/__init__.py
--rw-r--r--   0        0        0     1117 2022-10-04 06:08:21.872238 ppgee-0.1.2/ppgee/__main__.py
--rw-r--r--   0        0        0     2019 2022-10-04 06:01:48.907915 ppgee-0.1.2/ppgee/client.py
--rw-r--r--   0        0        0       99 2022-10-04 05:47:14.455055 ppgee-0.1.2/ppgee/errors.py
--rw-r--r--   0        0        0     1478 2022-10-04 01:09:26.833131 ppgee-0.1.2/ppgee/http.py
--rw-r--r--   0        0        0       37 2022-10-04 02:58:54.533973 ppgee-0.1.2/ppgee/pages/__init__.py
--rw-r--r--   0        0        0     1356 2022-10-04 03:25:25.570009 ppgee-0.1.2/ppgee/pages/frequency.py
--rw-r--r--   0        0        0     1191 2022-10-04 03:01:16.964666 ppgee-0.1.2/ppgee/parser.py
--rw-r--r--   0        0        0      412 2022-10-04 06:09:57.006021 ppgee-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      729 2022-10-04 06:10:05.980142 ppgee-0.1.2/setup.py
--rw-r--r--   0        0        0      325 2022-10-04 06:10:05.980358 ppgee-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       77 2023-07-19 05:31:14.682666 ppgee-0.1.3/ppgee/__init__.py
+-rw-r--r--   0        0        0     1206 2023-07-19 04:28:34.984494 ppgee-0.1.3/ppgee/__main__.py
+-rw-r--r--   0        0        0     2005 2023-07-19 05:30:13.889154 ppgee-0.1.3/ppgee/client.py
+-rw-r--r--   0        0        0       99 2023-07-19 04:04:24.485053 ppgee-0.1.3/ppgee/errors.py
+-rw-r--r--   0        0        0     1478 2023-07-19 04:04:24.485053 ppgee-0.1.3/ppgee/http.py
+-rw-r--r--   0        0        0       73 2023-07-19 05:26:14.954583 ppgee-0.1.3/ppgee/pages/__init__.py
+-rw-r--r--   0        0        0     1356 2023-07-19 04:04:24.488386 ppgee-0.1.3/ppgee/pages/frequency.py
+-rw-r--r--   0        0        0     1191 2023-07-19 04:04:24.488386 ppgee-0.1.3/ppgee/parser.py
+-rw-r--r--   0        0        0      412 2023-07-19 05:30:58.723497 ppgee-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      325 1970-01-01 00:00:00.000000 ppgee-0.1.3/PKG-INFO
```

### Comparing `ppgee-0.1.2/ppgee/__main__.py` & `ppgee-0.1.3/ppgee/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -30,12 +30,15 @@
                 eprint("Attendency not available yet.")
             await asyncio.sleep(1)
     except errors.InvalidCredentialsException:
         eprint("Invalid credentials.")
 
 
 def main():
-    asyncio.run(cli())
+    try:
+        asyncio.run(cli())
+    except KeyboardInterrupt:
+        print("Keyboard Interrupt. Exiting.")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ppgee-0.1.2/ppgee/client.py` & `ppgee-0.1.3/ppgee/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,24 +35,24 @@
             await self.session.close()
 
     async def __aenter__(self):
         await self.start()
         await self.login()
         return self
 
-    async def __aexit__(self, exc_type, exc, tb) -> None:
+    async def __aexit__(self, *_) -> None:
         if self.is_logged:
             await self.logoff()
         await self.close()
 
     async def login(self) -> None:
         logger.info("Logging in...")
         if self.user and self.password:
             resp = await self.http.login(self.user, self.password)
-            if "aindex" not in resp: # authentication failed
+            if "aindex" not in resp:  # authentication failed
                 await self.close()
                 raise errors.InvalidCredentialsException()
             self.is_logged = True
         else:
             logger.info("Logged in without credentials")
 
     @is_logged_check
```

### Comparing `ppgee-0.1.2/ppgee/http.py` & `ppgee-0.1.3/ppgee/http.py`

 * *Files identical despite different names*

### Comparing `ppgee-0.1.2/ppgee/pages/frequency.py` & `ppgee-0.1.3/ppgee/pages/frequency.py`

 * *Files identical despite different names*

### Comparing `ppgee-0.1.2/ppgee/parser.py` & `ppgee-0.1.3/ppgee/parser.py`

 * *Files identical despite different names*

