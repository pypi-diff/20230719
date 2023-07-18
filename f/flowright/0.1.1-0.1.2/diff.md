# Comparing `tmp/flowright-0.1.1.tar.gz` & `tmp/flowright-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowright-0.1.1.tar", max compression
+gzip compressed data, was "flowright-0.1.2.tar", max compression
```

## Comparing `flowright-0.1.1.tar` & `flowright-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      982 2023-06-27 01:13:08.109252 flowright-0.1.1/README.md
--rw-r--r--   0        0        0       66 2023-05-04 15:18:14.888426 flowright-0.1.1/flowright/__init__.py
--rw-r--r--   0        0        0    12421 2023-06-06 00:57:45.549641 flowright-0.1.1/flowright/client.py
--rw-r--r--   0        0        0     4857 2023-07-18 23:07:46.105394 flowright-0.1.1/flowright/commands.py
--rw-r--r--   0        0        0    11995 2023-06-01 15:35:35.253891 flowright-0.1.1/flowright/components.py
--rw-r--r--   0        0        0      647 2023-05-26 21:22:07.241233 flowright-0.1.1/flowright/config.py
--rw-r--r--   0        0        0     5241 2023-06-01 02:23:22.877147 flowright-0.1.1/flowright/customization.py
--rw-r--r--   0        0        0     1089 2023-06-03 02:36:45.186233 flowright-0.1.1/flowright/messages.py
--rw-r--r--   0        0        0     5999 2023-06-03 02:36:48.167192 flowright-0.1.1/flowright/res/client.html
--rw-r--r--   0        0        0     8976 2023-07-01 01:52:41.859892 flowright-0.1.1/flowright/server.py
--rw-r--r--   0        0        0      599 2023-07-18 23:07:53.087050 flowright-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1835 1970-01-01 00:00:00.000000 flowright-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      982 2023-06-27 01:13:08.109252 flowright-0.1.2/README.md
+-rw-r--r--   0        0        0       66 2023-05-04 15:18:14.888426 flowright-0.1.2/flowright/__init__.py
+-rw-r--r--   0        0        0    12421 2023-06-06 00:57:45.549641 flowright-0.1.2/flowright/client.py
+-rw-r--r--   0        0        0     4949 2023-07-18 23:33:10.000522 flowright-0.1.2/flowright/commands.py
+-rw-r--r--   0        0        0    11995 2023-06-01 15:35:35.253891 flowright-0.1.2/flowright/components.py
+-rw-r--r--   0        0        0      647 2023-05-26 21:22:07.241233 flowright-0.1.2/flowright/config.py
+-rw-r--r--   0        0        0     5241 2023-06-01 02:23:22.877147 flowright-0.1.2/flowright/customization.py
+-rw-r--r--   0        0        0     1089 2023-06-03 02:36:45.186233 flowright-0.1.2/flowright/messages.py
+-rw-r--r--   0        0        0     5999 2023-06-03 02:36:48.167192 flowright-0.1.2/flowright/res/client.html
+-rw-r--r--   0        0        0     8976 2023-07-01 01:52:41.859892 flowright-0.1.2/flowright/server.py
+-rw-r--r--   0        0        0      599 2023-07-18 23:37:33.376052 flowright-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1835 1970-01-01 00:00:00.000000 flowright-0.1.2/PKG-INFO
```

### Comparing `flowright-0.1.1/README.md` & `flowright-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `flowright-0.1.1/flowright/client.py` & `flowright-0.1.2/flowright/client.py`

 * *Files identical despite different names*

### Comparing `flowright-0.1.1/flowright/commands.py` & `flowright-0.1.2/flowright/commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import tempfile
 import base64
 
 from pydantic import BaseModel
 
 flowright_url = os.environ.get('FLOWRIGHT_URL', 'http://localhost:3000')
 flowright_api_url = os.environ.get('FLOWRIGHT_API_URL', 'http://localhost:8090')
+flowright_module_location = os.path.dirname(os.path.abspath(__file__))
 flowright_data_location = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'flowright_data')
 
 class PackageRequirement(BaseModel):
     name: str
     version: str
 
 def _get_live_packages() -> list[PackageRequirement]:
@@ -133,23 +134,23 @@
 
     # check path is valid
     if not os.path.exists(app_dir) or not os.path.isdir(app_dir):
         print(f'Invalid app directory: {app_dir}')
         exit(1)
 
     env['FLOWRIGHT_APP_DIR'] = os.path.abspath(app_dir)
-    args = ["uvicorn", "--app-dir", "flowright"]
+    args = ["uvicorn", "--app-dir", flowright_module_location]
     if devreload:
         args.extend(["--reload"])
     if reload:
         env['FLOWRIGHT_RELOAD'] = 'True'
     if uds is not None:
         args.extend(["--uds", uds])
 
-    args.extend(["server:app"])
+    args.extend(["server:app"]) # TODO
 
     try:
         subprocess.run(args, env=env)
     except KeyboardInterrupt:
         pass
```

### Comparing `flowright-0.1.1/flowright/components.py` & `flowright-0.1.2/flowright/components.py`

 * *Files identical despite different names*

### Comparing `flowright-0.1.1/flowright/config.py` & `flowright-0.1.2/flowright/config.py`

 * *Files identical despite different names*

### Comparing `flowright-0.1.1/flowright/customization.py` & `flowright-0.1.2/flowright/customization.py`

 * *Files identical despite different names*

### Comparing `flowright-0.1.1/flowright/messages.py` & `flowright-0.1.2/flowright/messages.py`

 * *Files identical despite different names*

### Comparing `flowright-0.1.1/flowright/res/client.html` & `flowright-0.1.2/flowright/res/client.html`

 * *Files identical despite different names*

### Comparing `flowright-0.1.1/flowright/server.py` & `flowright-0.1.2/flowright/server.py`

 * *Files identical despite different names*

### Comparing `flowright-0.1.1/pyproject.toml` & `flowright-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flowright"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["ReeceJones <reece_jones@icloud.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 starlette = "^0.26.1"
```

### Comparing `flowright-0.1.1/PKG-INFO` & `flowright-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowright
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: ReeceJones
 Author-email: reece_jones@icloud.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

