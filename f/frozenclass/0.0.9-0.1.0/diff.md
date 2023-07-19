# Comparing `tmp/frozenclass-0.0.9.tar.gz` & `tmp/frozenclass-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frozenclass-0.0.9.tar", last modified: Wed Apr 12 16:03:39 2023, max compression
+gzip compressed data, was "frozenclass-0.1.0.tar", last modified: Wed Jul 19 15:17:36 2023, max compression
```

## Comparing `frozenclass-0.0.9.tar` & `frozenclass-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 manjaro   (1000) manjaro   (1000)        0 2023-04-12 16:03:39.546409 frozenclass-0.0.9/
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)      677 2023-04-01 20:31:35.000000 frozenclass-0.0.9/LICENSE
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)     2826 2023-04-12 16:03:39.543075 frozenclass-0.0.9/PKG-INFO
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)     1920 2023-04-12 16:03:09.000000 frozenclass-0.0.9/README.md
-drwxr-xr-x   0 manjaro   (1000) manjaro   (1000)        0 2023-04-12 16:03:39.539742 frozenclass-0.0.9/frozenclass/
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)      151 2023-04-12 15:59:40.000000 frozenclass-0.0.9/frozenclass/__init__.py
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)     2365 2023-04-12 16:00:06.000000 frozenclass-0.0.9/frozenclass/auto_freeze.py
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)     4989 2023-04-12 15:17:00.000000 frozenclass-0.0.9/frozenclass/data_controller.py
-drwxr-xr-x   0 manjaro   (1000) manjaro   (1000)        0 2023-04-12 16:03:39.543075 frozenclass-0.0.9/frozenclass.egg-info/
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)     2826 2023-04-12 16:03:39.000000 frozenclass-0.0.9/frozenclass.egg-info/PKG-INFO
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)      364 2023-04-12 16:03:39.000000 frozenclass-0.0.9/frozenclass.egg-info/SOURCES.txt
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)        1 2023-04-12 16:03:39.000000 frozenclass-0.0.9/frozenclass.egg-info/dependency_links.txt
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)       12 2023-04-12 16:03:39.000000 frozenclass-0.0.9/frozenclass.egg-info/top_level.txt
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)     1011 2023-04-12 16:01:58.000000 frozenclass-0.0.9/pyproject.toml
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)       38 2023-04-12 16:03:39.546409 frozenclass-0.0.9/setup.cfg
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)     1406 2023-04-12 16:01:49.000000 frozenclass-0.0.9/setup.py
-drwxr-xr-x   0 manjaro   (1000) manjaro   (1000)        0 2023-04-12 16:03:39.543075 frozenclass-0.0.9/tests/
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)      900 2023-04-12 16:00:56.000000 frozenclass-0.0.9/tests/test_autosave.py
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)      860 2023-04-08 16:22:08.000000 frozenclass-0.0.9/tests/test_deep_save_load.py
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)     1461 2023-04-05 19:34:07.000000 frozenclass-0.0.9/tests/test_save_bases.py
--rw-r--r--   0 manjaro   (1000) manjaro   (1000)     1007 2023-04-05 19:34:07.000000 frozenclass-0.0.9/tests/test_save_load.py
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-07-19 15:17:36.966932 frozenclass-0.1.0/
+-rw-r--r--   0 q         (1000) q         (1000)      677 2023-07-18 20:15:53.000000 frozenclass-0.1.0/LICENSE
+-rw-r--r--   0 q         (1000) q         (1000)     8488 2023-07-19 15:17:36.966932 frozenclass-0.1.0/PKG-INFO
+-rw-r--r--   0 q         (1000) q         (1000)     7583 2023-07-18 20:15:53.000000 frozenclass-0.1.0/README.rst
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-07-19 15:17:36.963932 frozenclass-0.1.0/frozenclass/
+-rw-r--r--   0 q         (1000) q         (1000)      187 2023-07-19 15:12:57.000000 frozenclass-0.1.0/frozenclass/__init__.py
+-rw-r--r--   0 q         (1000) q         (1000)     2394 2023-07-19 15:12:57.000000 frozenclass-0.1.0/frozenclass/auto_freeze.py
+-rw-r--r--   0 q         (1000) q         (1000)     1598 2023-07-19 15:12:57.000000 frozenclass-0.1.0/frozenclass/cache.py
+-rw-r--r--   0 q         (1000) q         (1000)     5112 2023-07-19 15:12:57.000000 frozenclass-0.1.0/frozenclass/data_controller.py
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-07-19 15:17:36.964932 frozenclass-0.1.0/frozenclass.egg-info/
+-rw-r--r--   0 q         (1000) q         (1000)     8488 2023-07-19 15:17:36.000000 frozenclass-0.1.0/frozenclass.egg-info/PKG-INFO
+-rw-r--r--   0 q         (1000) q         (1000)      406 2023-07-19 15:17:36.000000 frozenclass-0.1.0/frozenclass.egg-info/SOURCES.txt
+-rw-r--r--   0 q         (1000) q         (1000)        1 2023-07-19 15:17:36.000000 frozenclass-0.1.0/frozenclass.egg-info/dependency_links.txt
+-rw-r--r--   0 q         (1000) q         (1000)       12 2023-07-19 15:17:36.000000 frozenclass-0.1.0/frozenclass.egg-info/top_level.txt
+-rw-r--r--   0 q         (1000) q         (1000)     1025 2023-07-19 15:14:03.000000 frozenclass-0.1.0/pyproject.toml
+-rw-r--r--   0 q         (1000) q         (1000)       38 2023-07-19 15:17:36.967932 frozenclass-0.1.0/setup.cfg
+-rw-r--r--   0 q         (1000) q         (1000)     1406 2023-07-19 15:15:10.000000 frozenclass-0.1.0/setup.py
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-07-19 15:17:36.966932 frozenclass-0.1.0/tests/
+-rw-r--r--   0 q         (1000) q         (1000)      900 2023-07-18 20:15:53.000000 frozenclass-0.1.0/tests/test_autosave.py
+-rw-r--r--   0 q         (1000) q         (1000)     2045 2023-07-19 15:12:57.000000 frozenclass-0.1.0/tests/test_cache.py
+-rw-r--r--   0 q         (1000) q         (1000)      860 2023-07-18 20:15:53.000000 frozenclass-0.1.0/tests/test_deep_save_load.py
+-rw-r--r--   0 q         (1000) q         (1000)     1461 2023-07-19 13:18:19.000000 frozenclass-0.1.0/tests/test_save_bases.py
+-rw-r--r--   0 q         (1000) q         (1000)     1007 2023-07-18 20:15:53.000000 frozenclass-0.1.0/tests/test_save_load.py
```

### Comparing `frozenclass-0.0.9/LICENSE` & `frozenclass-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `frozenclass-0.0.9/frozenclass/auto_freeze.py` & `frozenclass-0.1.0/frozenclass/auto_freeze.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from typing import Any
+from typing import Any, Callable
 
 from .data_controller import DataController
 from .exceptions import NoSave
 
 
-def AutoFreeze(saves_path: str = 'saves', mode: str = 'freeze'):
+def AutoFreeze(saves_path: str = 'saves', mode: str = 'freeze') -> Callable:
     """Automatically saves changes to variables made to the class
 
     Args:
         saves_path (str, optional): Path to save folder. Defaults to 'saves'.
         mode (str, optional): Save mode (as in DataController): 'freeze' or 'deep_freeze'. Defaults to 'freeze'.
     """
-    def wrapper_func(target_class: Any):
+    def wrapper_func(target_class: Any) -> Any:
         if '__name__' not in target_class.__dict__:
             raise AttributeError('Your class must contain a variable called __name__')
 
         setattr(target_class, '__controller', DataController(saves_path))
         setattr(target_class, '__is_init', False)
 
         setattr(target_class, '__staff_params', [
```

### Comparing `frozenclass-0.0.9/frozenclass/data_controller.py` & `frozenclass-0.1.0/frozenclass/data_controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,25 +65,27 @@
             Any: The instance of the class that was saved
         """
         list_dir = os.listdir(self._saves_path)
 
         for save_filename in list_dir:
             parser = DataParser(f"{self._saves_path}/{save_filename}", self)
             parsed_content = parser.parse_file_content()
-            if parsed_content["SavedModel"]["save_name"].lower() == save_name.lower():
+            if parsed_content and \
+                    parsed_content["SavedModel"]["save_name"].lower() == save_name.lower():
                 return parser.parse_file()
         raise NoSave("save_name")
 
     def load_saved_vars(self, save_name: str) -> Any:
         list_dir = os.listdir(self._saves_path)
 
         for save_filename in list_dir:
             parser = DataParser(f"{self._saves_path}/{save_filename}", self)
             parsed_content = parser.parse_file_content()
-            if parsed_content["SavedModel"]["save_name"].lower() == save_name.lower():
+            if parsed_content and \
+                    parsed_content["SavedModel"]["save_name"].lower() == save_name.lower():
                 return parser.parse_saved_args()
         raise NoSave("save_name")
 
     def dalete_save(self, save_name: str) -> None:
         """Need to delete save with this save name. Doesn't delete dependent saves.
 
         Args:
@@ -93,15 +95,16 @@
             NoSave: If there is no save with the given name
         """
         list_dir = os.listdir(self._saves_path)
 
         for save_filename in list_dir:
             parser = DataParser(f"{self._saves_path}/{save_filename}", self)
             parsed_content = parser.parse_file_content()
-            if parsed_content["SavedModel"]["save_name"] == save_name:
+            if parsed_content and \
+                    parsed_content["SavedModel"]["save_name"] == save_name:
                 platform_ = platform.system()
                 if platform_ == 'Linux':
                     os.system(f'rm -rf "{self._saves_path}/{save_filename}"')
                 elif platform_ == 'Windows':
                     os.system(f'del /f "{self._saves_path}/{save_filename}"')
                 return
         raise NoSave("save_name")
```

### Comparing `frozenclass-0.0.9/pyproject.toml` & `frozenclass-0.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "frozenclass"
-version = "0.0.9"
+version = "0.1.0"
 description = "Python module for convenient storage of classes in files."
 authors = ["GigantPro <gigantpro2000@gmail.com>"]
 license = "The GPLv3 License (GPLv3)"
-readme = "README.md"
+readme = "README.rst"
 
 [tool.poetry.dependencies]
 python = ">=3.7"
 
 [tool.poetry.group.dev.dependencies]
 setuptools = "^67.6.1"
 pylint = "^2.17.1"
@@ -45,9 +45,10 @@
     "C0207",
     "C2801",
     "C0206",
     "C0200",
     "E0401",
     "W1401",
     "W0212",
-    "C0103"
+    "C0103",
+    "E0211"
 ]
```

### Comparing `frozenclass-0.0.9/setup.py` & `frozenclass-0.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 :license: The GPLv3 License (GPLv3)
 :copyright: (c) 2023 Xiver organization
 """
 
 with open("pyproject.toml", encoding="utf-8") as file:
     VERSION = file.read().split("=")[2].split('"')[1]
 
-with open("README.md", encoding="utf-8") as f:
+with open("README.rst", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="frozenclass",
     version=VERSION,
     author="GigantPro",
     author_email="gigantpro2000@gmail.ru",
     description=("Python module for convenient storage of classes in files."),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/GigantPro/frozenclass",
-    download_url="https://github.com/Peopl3s/club-house-api/archive/main.zip",
+    download_url="https://github.com/GigantPro/frozenclass/archive/main.zip",
     license="The GPLv3 License (GPLv3)",
     packages=["frozenclass"],
     install_requires=[],
     classifiers=[
         "Operating System :: OS Independent",
         "Intended Audience :: End Users/Desktop",
         "Intended Audience :: Developers",
```

### Comparing `frozenclass-0.0.9/tests/test_autosave.py` & `frozenclass-0.1.0/tests/test_autosave.py`

 * *Files identical despite different names*

### Comparing `frozenclass-0.0.9/tests/test_deep_save_load.py` & `frozenclass-0.1.0/tests/test_deep_save_load.py`

 * *Files identical despite different names*

### Comparing `frozenclass-0.0.9/tests/test_save_bases.py` & `frozenclass-0.1.0/tests/test_save_bases.py`

 * *Files identical despite different names*

### Comparing `frozenclass-0.0.9/tests/test_save_load.py` & `frozenclass-0.1.0/tests/test_save_load.py`

 * *Files identical despite different names*

