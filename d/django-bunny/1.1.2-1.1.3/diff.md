# Comparing `tmp/django_bunny-1.1.2.tar.gz` & `tmp/django_bunny-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_bunny-1.1.2.tar", max compression
+gzip compressed data, was "django_bunny-1.1.3.tar", max compression
```

## Comparing `django_bunny-1.1.2.tar` & `django_bunny-1.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-07-19 04:24:01.993156 django_bunny-1.1.2/django_bunny/__init__.py
--rw-r--r--   0        0        0     6880 2023-07-19 06:46:52.088652 django_bunny-1.1.2/django_bunny/storage.py
--rw-r--r--   0        0        0     1092 2023-07-19 04:24:01.993156 django_bunny-1.1.2/LICENSE
--rw-r--r--   0        0        0      855 2023-07-19 06:49:32.577959 django_bunny-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     2570 2023-07-19 06:49:08.934029 django_bunny-1.1.2/README.md
--rw-r--r--   0        0        0     3478 1970-01-01 00:00:00.000000 django_bunny-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-19 04:24:01.993156 django_bunny-1.1.3/django_bunny/__init__.py
+-rw-r--r--   0        0        0     6874 2023-07-19 06:51:00.185667 django_bunny-1.1.3/django_bunny/storage.py
+-rw-r--r--   0        0        0     1092 2023-07-19 04:24:01.993156 django_bunny-1.1.3/LICENSE
+-rw-r--r--   0        0        0      855 2023-07-19 06:51:31.735069 django_bunny-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2570 2023-07-19 06:49:08.934029 django_bunny-1.1.3/README.md
+-rw-r--r--   0        0        0     3478 1970-01-01 00:00:00.000000 django_bunny-1.1.3/PKG-INFO
```

### Comparing `django_bunny-1.1.2/django_bunny/storage.py` & `django_bunny-1.1.3/django_bunny/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         self.region = region
         self.hostname = hostname
 
         self.base_url += f"{username}/"
         self.headers = {"AccessKey": password, "Accept": "*/*"}
 
         try:
-            self.base_url += f"{kwargs['base_dir']}/" if "base_dir" in kwargs else settings.BUNNY_BASE_DIR
+            self.base_url += kwargs['base_dir'] if "base_dir" in kwargs else settings.BUNNY_BASE_DIR
         except:
             pass
 
     def _full_path(self, name) -> str:
         if name == "/":
             name = ""
         return self.base_url + name.replace("\\", "/")
```

### Comparing `django_bunny-1.1.2/LICENSE` & `django_bunny-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_bunny-1.1.2/pyproject.toml` & `django_bunny-1.1.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-bunny"
-version = "1.1.2"
+version = "1.1.3"
 description = "A django storage for bunny.net"
 authors = ["Neki <neki@nekidev.com>"]
 maintainers = ["Neki <neki@nekidev.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "django_bunny"}]
 homepage = "https://github.com/Nekidev/django-bunny/"
```

### Comparing `django_bunny-1.1.2/README.md` & `django_bunny-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `django_bunny-1.1.2/PKG-INFO` & `django_bunny-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-bunny
-Version: 1.1.2
+Version: 1.1.3
 Summary: A django storage for bunny.net
 Home-page: https://github.com/Nekidev/django-bunny/
 License: MIT
 Keywords: django,bunnycdn,django-storage
 Author: Neki
 Author-email: neki@nekidev.com
 Maintainer: Neki
```

