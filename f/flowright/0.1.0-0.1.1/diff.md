# Comparing `tmp/flowright-0.1.0.tar.gz` & `tmp/flowright-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowright-0.1.0.tar", max compression
+gzip compressed data, was "flowright-0.1.1.tar", max compression
```

## Comparing `flowright-0.1.0.tar` & `flowright-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      982 2023-06-27 01:13:08.109252 flowright-0.1.0/README.md
--rw-r--r--   0        0        0       66 2023-05-04 15:18:14.888426 flowright-0.1.0/flowright/__init__.py
--rw-r--r--   0        0        0    12421 2023-06-06 00:57:45.549641 flowright-0.1.0/flowright/client.py
--rw-r--r--   0        0        0     4853 2023-07-04 17:19:48.872140 flowright-0.1.0/flowright/commands.py
--rw-r--r--   0        0        0    11995 2023-06-01 15:35:35.253891 flowright-0.1.0/flowright/components.py
--rw-r--r--   0        0        0      647 2023-05-26 21:22:07.241233 flowright-0.1.0/flowright/config.py
--rw-r--r--   0        0        0     5241 2023-06-01 02:23:22.877147 flowright-0.1.0/flowright/customization.py
--rw-r--r--   0        0        0     1089 2023-06-03 02:36:45.186233 flowright-0.1.0/flowright/messages.py
--rw-r--r--   0        0        0     5999 2023-06-03 02:36:48.167192 flowright-0.1.0/flowright/res/client.html
--rw-r--r--   0        0        0     8976 2023-07-01 01:52:41.859892 flowright-0.1.0/flowright/server.py
--rw-r--r--   0        0        0      599 2023-07-01 02:14:01.805633 flowright-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1835 1970-01-01 00:00:00.000000 flowright-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      982 2023-06-27 01:13:08.109252 flowright-0.1.1/README.md
+-rw-r--r--   0        0        0       66 2023-05-04 15:18:14.888426 flowright-0.1.1/flowright/__init__.py
+-rw-r--r--   0        0        0    12421 2023-06-06 00:57:45.549641 flowright-0.1.1/flowright/client.py
+-rw-r--r--   0        0        0     4857 2023-07-18 23:07:46.105394 flowright-0.1.1/flowright/commands.py
+-rw-r--r--   0        0        0    11995 2023-06-01 15:35:35.253891 flowright-0.1.1/flowright/components.py
+-rw-r--r--   0        0        0      647 2023-05-26 21:22:07.241233 flowright-0.1.1/flowright/config.py
+-rw-r--r--   0        0        0     5241 2023-06-01 02:23:22.877147 flowright-0.1.1/flowright/customization.py
+-rw-r--r--   0        0        0     1089 2023-06-03 02:36:45.186233 flowright-0.1.1/flowright/messages.py
+-rw-r--r--   0        0        0     5999 2023-06-03 02:36:48.167192 flowright-0.1.1/flowright/res/client.html
+-rw-r--r--   0        0        0     8976 2023-07-01 01:52:41.859892 flowright-0.1.1/flowright/server.py
+-rw-r--r--   0        0        0      599 2023-07-18 23:07:53.087050 flowright-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1835 1970-01-01 00:00:00.000000 flowright-0.1.1/PKG-INFO
```

### Comparing `flowright-0.1.0/README.md` & `flowright-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `flowright-0.1.0/flowright/client.py` & `flowright-0.1.1/flowright/client.py`

 * *Files identical despite different names*

### Comparing `flowright-0.1.0/flowright/commands.py` & `flowright-0.1.1/flowright/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,15 +124,15 @@
     token = r.json()['current_client_jwt']
 
     pathlib.Path(flowright_data_location).mkdir(parents=True, exist_ok=True)
 
     with open(os.path.join(flowright_data_location, '.token'), 'w') as f:
         f.write(token)
 
-def run(app_dir: str, *, reload: bool = False, devreload: bool = False, uds: str | None = None) -> None:
+def serve(app_dir: str, *, reload: bool = False, devreload: bool = False, uds: str | None = None) -> None:
     env = os.environ
 
     # check path is valid
     if not os.path.exists(app_dir) or not os.path.isdir(app_dir):
         print(f'Invalid app directory: {app_dir}')
         exit(1)
 
@@ -154,9 +154,9 @@
 
 
 def run() -> None:
     fire.Fire({
         'login': login,
         'link': link,
         'upload': upload,
-        'run': run
+        'run': serve
     })
```

### Comparing `flowright-0.1.0/flowright/components.py` & `flowright-0.1.1/flowright/components.py`

 * *Files identical despite different names*

### Comparing `flowright-0.1.0/flowright/config.py` & `flowright-0.1.1/flowright/config.py`

 * *Files identical despite different names*

### Comparing `flowright-0.1.0/flowright/customization.py` & `flowright-0.1.1/flowright/customization.py`

 * *Files identical despite different names*

### Comparing `flowright-0.1.0/flowright/messages.py` & `flowright-0.1.1/flowright/messages.py`

 * *Files identical despite different names*

### Comparing `flowright-0.1.0/flowright/res/client.html` & `flowright-0.1.1/flowright/res/client.html`

 * *Files identical despite different names*

### Comparing `flowright-0.1.0/flowright/server.py` & `flowright-0.1.1/flowright/server.py`

 * *Files identical despite different names*

### Comparing `flowright-0.1.0/pyproject.toml` & `flowright-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flowright"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["ReeceJones <reece_jones@icloud.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 starlette = "^0.26.1"
```

### Comparing `flowright-0.1.0/PKG-INFO` & `flowright-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowright
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: ReeceJones
 Author-email: reece_jones@icloud.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

