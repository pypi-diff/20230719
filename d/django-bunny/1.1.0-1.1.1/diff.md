# Comparing `tmp/django_bunny-1.1.0.tar.gz` & `tmp/django_bunny-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_bunny-1.1.0.tar", max compression
+gzip compressed data, was "django_bunny-1.1.1.tar", max compression
```

## Comparing `django_bunny-1.1.0.tar` & `django_bunny-1.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-07-19 04:24:01.993156 django_bunny-1.1.0/django_bunny/__init__.py
--rw-r--r--   0        0        0     6609 2023-07-19 04:31:27.674086 django_bunny-1.1.0/django_bunny/storage.py
--rw-r--r--   0        0        0     1092 2023-07-19 04:24:01.993156 django_bunny-1.1.0/LICENSE
--rw-r--r--   0        0        0      855 2023-07-19 04:32:15.873925 django_bunny-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     2243 2023-07-19 04:24:01.993156 django_bunny-1.1.0/README.md
--rw-r--r--   0        0        0     3159 1970-01-01 00:00:00.000000 django_bunny-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-19 04:24:01.993156 django_bunny-1.1.1/django_bunny/__init__.py
+-rw-r--r--   0        0        0     6704 2023-07-19 05:19:36.600052 django_bunny-1.1.1/django_bunny/storage.py
+-rw-r--r--   0        0        0     1092 2023-07-19 04:24:01.993156 django_bunny-1.1.1/LICENSE
+-rw-r--r--   0        0        0      855 2023-07-19 05:18:18.222820 django_bunny-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2243 2023-07-19 04:24:01.993156 django_bunny-1.1.1/README.md
+-rw-r--r--   0        0        0     3159 1970-01-01 00:00:00.000000 django_bunny-1.1.1/PKG-INFO
```

### Comparing `django_bunny-1.1.0/django_bunny/storage.py` & `django_bunny-1.1.1/django_bunny/storage.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,52 +92,52 @@
     def _full_path(self, name) -> str:
         if name == "/":
             name = ""
         return self.base_url + name.replace("\\", "/")
 
     def _save(self, name, content) -> str:
         r = requests.put(
-            self.base_url + name, data=content, headers=self.headers
+            self.base_url + name.replace("\\", "/"), data=content, headers=self.headers
         )
         return name
 
     def _open(self, name, mode="rb"):
-        r = requests.get(self.base_url + name, headers=self.headers)
+        r = requests.get(self.base_url + name.replace("\\", "/"), headers=self.headers)
         r.raise_for_status()
 
         return r.raw
 
     def delete(self, name) -> str:
         r = requests.delete(self.base_url + name, headers=self.headers)
 
         return name
 
     def exists(self, name) -> bool:
-        r = requests.head(self.base_url + name, headers=self.headers)
+        r = requests.head(self.base_url + name.replace("\\", "/"), headers=self.headers)
 
         if r.status_code == 404:
             return False
 
         r.raise_for_status()
 
         return True
 
     def url(self, name: str) -> str:
-        return self.hostname + name
+        return self.hostname + name.replace("\\", "/")
 
     def size(self, name: str) -> int:
         r = requests.head(self.url(name))
         r.raise_for_status()
 
         file_size = r.headers.get("Content-Length", 0)
 
         return int(file_size)
 
     def listdir(self, path) -> tuple:
-        r = requests.get(self.base_url + path, headers=self.headers)
+        r = requests.get(self.base_url + path.replace("\\", "/"), headers=self.headers)
         r.raise_for_status()
 
         objects = r.json()
 
         return (
             [item["ObjectName"] for item in objects if item["IsDirectory"]],
             [item["ObjectName"] for item in objects if not item["IsDirectory"]],
```

### Comparing `django_bunny-1.1.0/LICENSE` & `django_bunny-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_bunny-1.1.0/pyproject.toml` & `django_bunny-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-bunny"
-version = "1.1.0"
+version = "1.1.1"
 description = "A django storage for bunny.net"
 authors = ["Neki <neki@nekidev.com>"]
 maintainers = ["Neki <neki@nekidev.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "django_bunny"}]
 homepage = "https://github.com/Nekidev/django-bunny/"
```

### Comparing `django_bunny-1.1.0/README.md` & `django_bunny-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `django_bunny-1.1.0/PKG-INFO` & `django_bunny-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-bunny
-Version: 1.1.0
+Version: 1.1.1
 Summary: A django storage for bunny.net
 Home-page: https://github.com/Nekidev/django-bunny/
 License: MIT
 Keywords: django,bunnycdn,django-storage
 Author: Neki
 Author-email: neki@nekidev.com
 Maintainer: Neki
```

