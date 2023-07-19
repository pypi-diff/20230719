# Comparing `tmp/django-bunny-1.0.9.tar.gz` & `tmp/django_bunny-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-bunny-1.0.9.tar", max compression
+gzip compressed data, was "django_bunny-1.1.0.tar", max compression
```

## Comparing `django-bunny-1.0.9.tar` & `django_bunny-1.1.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0        0 2023-05-09 02:51:37.446276 django-bunny-1.0.9/django_bunny/__init__.py
--rw-r--r--   0        0        0     5966 2023-05-09 05:16:05.772029 django-bunny-1.0.9/django_bunny/storage.py
--rw-r--r--   0        0        0     1092 2023-05-09 01:04:30.492122 django-bunny-1.0.9/LICENSE
--rw-r--r--   0        0        0      855 2023-05-09 05:16:15.161025 django-bunny-1.0.9/pyproject.toml
--rw-r--r--   0        0        0     2243 2023-05-09 02:51:17.790012 django-bunny-1.0.9/README.md
--rw-r--r--   0        0        0     2966 1970-01-01 00:00:00.000000 django-bunny-1.0.9/setup.py
--rw-r--r--   0        0        0     3108 1970-01-01 00:00:00.000000 django-bunny-1.0.9/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-19 04:24:01.993156 django_bunny-1.1.0/django_bunny/__init__.py
+-rw-r--r--   0        0        0     6609 2023-07-19 04:31:27.674086 django_bunny-1.1.0/django_bunny/storage.py
+-rw-r--r--   0        0        0     1092 2023-07-19 04:24:01.993156 django_bunny-1.1.0/LICENSE
+-rw-r--r--   0        0        0      855 2023-07-19 04:32:15.873925 django_bunny-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2243 2023-07-19 04:24:01.993156 django_bunny-1.1.0/README.md
+-rw-r--r--   0        0        0     3159 1970-01-01 00:00:00.000000 django_bunny-1.1.0/PKG-INFO
```

### Comparing `django-bunny-1.0.9/django_bunny/storage.py` & `django_bunny-1.1.0/django_bunny/storage.py`

 * *Files 12% similar despite different names*

```diff
@@ -83,82 +83,88 @@
 
         self.username = username
         self.password = password
         self.region = region
         self.hostname = hostname
 
         self.base_url += f"{username}/"
-        self.headers = {"AccessKey": self.password}
+        self.headers = {"AccessKey": password}
 
     def _full_path(self, name) -> str:
         if name == "/":
             name = ""
         return self.base_url + name.replace("\\", "/")
 
     def _save(self, name, content) -> str:
         r = requests.put(
-            self._full_path(name), data=content, headers=self.headers
+            self.base_url + name, data=content, headers=self.headers
         )
         return name
 
     def _open(self, name, mode="rb"):
-        r = requests.get(self._full_path(name), headers=self.headers)
+        r = requests.get(self.base_url + name, headers=self.headers)
         r.raise_for_status()
 
         return r.raw
 
     def delete(self, name) -> str:
-        r = requests.delete(self._full_path(name), headers=self.headers)
+        r = requests.delete(self.base_url + name, headers=self.headers)
 
         return name
 
     def exists(self, name) -> bool:
-        r = requests.head(self._full_path(name), headers=self.headers)
+        r = requests.head(self.base_url + name, headers=self.headers)
 
         if r.status_code == 404:
             return False
 
         r.raise_for_status()
 
         return True
 
     def url(self, name: str) -> str:
-        return self._full_path(name)
+        return self.hostname + name
 
     def size(self, name: str) -> int:
-        r = requests.head(self._full_path(name))
+        r = requests.head(self.url(name))
         r.raise_for_status()
 
         file_size = r.headers.get("Content-Length", 0)
 
         return int(file_size)
 
     def listdir(self, path) -> tuple:
-        r = requests.get(self._full_path(name), headers=self.headers)
+        r = requests.get(self.base_url + path, headers=self.headers)
         r.raise_for_status()
 
         objects = r.json()
 
         return (
             [item["ObjectName"] for item in objects if item["IsDirectory"]],
             [item["ObjectName"] for item in objects if not item["IsDirectory"]],
         )
 
     def get_created_time(self, name) -> datetime.datetime:
         r = requests.get(
-            self.base_url + name.rsplit("/", 1)[0], headers=self.headers
+            self.base_url + name.replace("\\", "/").rsplit("/", 1)[0], headers=self.headers
         )
         r.raise_for_status()
 
         iso_date = None
 
         for item in r.json():
-            if item["ObjectName"] == name:
-                iso_date = item["DateCreated"]
-                break
+            try:
+                if item["ObjectName"] == name.rsplit("/", 1)[len(name.rsplit("/", 1) - 1)]:
+                    iso_date = item["DateCreated"]
+                    break
+            except:
+                # Error fetching creation date for this file. A
+                # NotImplementedError is raised as specified by the Django
+                # documentation.
+                raise NotImplementedError()
 
         if iso_date is None:
             raise ValueError(f"File '{name}' does not exist.")
 
         if settings.USE_TZ == True:
             parsed_date = parser.parse(iso_date)
             parsed_date.replace(tzinfo=datetime.timezone.utc)
@@ -168,24 +174,30 @@
             parsed_date.replace(tzinfo=datetime.timezone.utc)
             parsed_date.astimezone()
             parsed_date.replace(tzinfo=None)
             return parsed_date
 
     def get_modified_time(self, name) -> datetime.datetime:
         r = requests.get(
-            self.base_url + name.rsplit("/", 1)[0], headers=self.headers
+            self.base_url + name.replace("\\", "/").rsplit("/", 1)[0], headers=self.headers
         )
         r.raise_for_status()
 
         iso_date = None
 
         for item in r.json():
-            if item["ObjectName"] == name.rsplit("/", 1)[1]:
-                iso_date = item["LastChanged"]
-                break
+            try:
+                if item["ObjectName"] == name.rsplit("/", 1)[len(name.rsplit("/", 1) - 1)]:
+                    iso_date = item["LastChanged"]
+                    break
+            except:
+                # Error fetching last modification date for this file. A
+                # NotImplementedError is raised as specified by the Django
+                # documentation.
+                raise NotImplementedError()
 
         if iso_date is None:
             raise ValueError(f"File '{name}' does not exist.")
 
         if settings.USE_TZ == True:
             parsed_date = parser.parse(iso_date)
             parsed_date.replace(tzinfo=datetime.timezone.utc)
```

### Comparing `django-bunny-1.0.9/LICENSE` & `django_bunny-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-bunny-1.0.9/pyproject.toml` & `django_bunny-1.1.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-bunny"
-version = "1.0.9"
+version = "1.1.0"
 description = "A django storage for bunny.net"
 authors = ["Neki <neki@nekidev.com>"]
 maintainers = ["Neki <neki@nekidev.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "django_bunny"}]
 homepage = "https://github.com/Nekidev/django-bunny/"
```

### Comparing `django-bunny-1.0.9/README.md` & `django_bunny-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `django-bunny-1.0.9/setup.py` & `django_bunny-1.1.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,106 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: django-bunny
+Version: 1.1.0
+Summary: A django storage for bunny.net
+Home-page: https://github.com/Nekidev/django-bunny/
+License: MIT
+Keywords: django,bunnycdn,django-storage
+Author: Neki
+Author-email: neki@nekidev.com
+Maintainer: Neki
+Maintainer-email: neki@nekidev.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Django (>=3.0.0)
+Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
+Requires-Dist: requests (>=2.30.0,<3.0.0)
+Project-URL: Documentation, https://github.com/Nekidev/django-bunny/tree/main/README.md
+Project-URL: Repository, https://github.com/Nekidev/django-bunny/
+Description-Content-Type: text/markdown
+
+# django-bunny
+
+A bunny.net storage for Django. It was created as a replacement for [django-bunny-storage](https://github.com/willmeyers/django-bunny-storage).
+
+
+## Installation
+
+You can install the library using `pip`:
+
+```bash
+pip install django-bunny
+```
+
+
+## Configuration
+
+First, add `django_bunny` to your `INSTALLED_APPS`:
+
+```py
+INSTALLED_APPS = [
+    ...,
+    "django_bunny",
+    ...
+]
+```
+
+Now, create the following variables inside your `settings.py` file. These are required if you are using Django < `4.2`. Otherwise, you can use `OPTIONS` in the `STORAGES` setting.
+
+```py
+# These can be found in your storage's dashboard under `FTP & API Access`
+BUNNY_USERNAME = "my-storage-name"
+BUNNY_PASSWORD = "my-storage-password"
+
+# This is the storage region's code. E.g. Los Angeles is `la`, Singapore is
+# `sg`, etc. The default is `ny` (New York).
+BUNNY_REGION = "my-storage-region"
+
+# Optional. For example, `https://myzone.b-cdn.net/`. `MEDIA_URL` will be used
+# if this is not set.
+BUNNY_HOSTNAME = "my-pullzone-hostname"
+```
+
+Finally, depending on which version of Django you are using you'll need to create one of these variables:
+
+```py
+# Django < 4.2
+DEFAULT_FILE_STORAGE = 'django_bunny.storage.BunnyStorage'
+
+# Django >= 4.2. Set `BunnyStorage` where you want to use bunny.net's storage.
+{
+    "default": {
+        "BACKEND": "django_bunny.storage.BunnyStorage",
+
+        # Add this if you did not create the BUNNY_* settings before. They are
+        # the same as BUNNY_* variables.
+        "OPTIONS": {
+            "username": "my-storage-name",
+            "password": "my-storage-password",
+            
+            # Optional. Defaults to `ny`
+            "region": "my-storage-region",
+            
+            # Optional. `MEDIA_URL` will be used if it is not set
+            "hostname": "my-pullzone-hostname"
+        }
+    },
+}
+```
 
-packages = \
-['django_bunny']
+In Django >= 4.2 you can set different credentials for the different storages. This allows you to, for example, use a separate storage for static files.
 
-package_data = \
-{'': ['*']}
 
-install_requires = \
-['Django>=3.0.0', 'python-dateutil>=2.8.2,<3.0.0', 'requests>=2.30.0,<3.0.0']
-
-setup_kwargs = {
-    'name': 'django-bunny',
-    'version': '1.0.9',
-    'description': 'A django storage for bunny.net',
-    'long_description': '# django-bunny\n\nA bunny.net storage for Django. It was created as a replacement for [django-bunny-storage](https://github.com/willmeyers/django-bunny-storage).\n\n\n## Installation\n\nYou can install the library using `pip`:\n\n```bash\npip install django-bunny\n```\n\n\n## Configuration\n\nFirst, add `django_bunny` to your `INSTALLED_APPS`:\n\n```py\nINSTALLED_APPS = [\n    ...,\n    "django_bunny",\n    ...\n]\n```\n\nNow, create the following variables inside your `settings.py` file. These are required if you are using Django < `4.2`. Otherwise, you can use `OPTIONS` in the `STORAGES` setting.\n\n```py\n# These can be found in your storage\'s dashboard under `FTP & API Access`\nBUNNY_USERNAME = "my-storage-name"\nBUNNY_PASSWORD = "my-storage-password"\n\n# This is the storage region\'s code. E.g. Los Angeles is `la`, Singapore is\n# `sg`, etc. The default is `ny` (New York).\nBUNNY_REGION = "my-storage-region"\n\n# Optional. For example, `https://myzone.b-cdn.net/`. `MEDIA_URL` will be used\n# if this is not set.\nBUNNY_HOSTNAME = "my-pullzone-hostname"\n```\n\nFinally, depending on which version of Django you are using you\'ll need to create one of these variables:\n\n```py\n# Django < 4.2\nDEFAULT_FILE_STORAGE = \'django_bunny.storage.BunnyStorage\'\n\n# Django >= 4.2. Set `BunnyStorage` where you want to use bunny.net\'s storage.\n{\n    "default": {\n        "BACKEND": "django_bunny.storage.BunnyStorage",\n\n        # Add this if you did not create the BUNNY_* settings before. They are\n        # the same as BUNNY_* variables.\n        "OPTIONS": {\n            "username": "my-storage-name",\n            "password": "my-storage-password",\n            \n            # Optional. Defaults to `ny`\n            "region": "my-storage-region",\n            \n            # Optional. `MEDIA_URL` will be used if it is not set\n            "hostname": "my-pullzone-hostname"\n        }\n    },\n}\n```\n\nIn Django >= 4.2 you can set different credentials for the different storages. This allows you to, for example, use a separate storage for static files.\n\n\n## Using in templates\n\nIn templates, you can use `{{ instance.file.url }}` directly. For example:\n\n```html\n<img src="{{ instance.file.url }}" />\n```\n',
-    'author': 'Neki',
-    'author_email': 'neki@nekidev.com',
-    'maintainer': 'Neki',
-    'maintainer_email': 'neki@nekidev.com',
-    'url': 'https://github.com/Nekidev/django-bunny/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
+## Using in templates
+
+In templates, you can use `{{ instance.file.url }}` directly. For example:
 
+```html
+<img src="{{ instance.file.url }}" />
+```
 
-setup(**setup_kwargs)
```

