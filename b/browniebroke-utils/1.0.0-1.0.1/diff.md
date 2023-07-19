# Comparing `tmp/browniebroke_utils-1.0.0.tar.gz` & `tmp/browniebroke_utils-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "browniebroke_utils-1.0.0.tar", max compression
+gzip compressed data, was "browniebroke_utils-1.0.1.tar", max compression
```

## Comparing `browniebroke_utils-1.0.0.tar` & `browniebroke_utils-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1068 2023-06-27 11:45:42.997304 browniebroke_utils-1.0.0/LICENSE
--rw-r--r--   0        0        0     4519 2023-06-27 11:45:42.997304 browniebroke_utils-1.0.0/README.md
--rw-r--r--   0        0        0     2194 2023-06-27 11:45:44.197297 browniebroke_utils-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-06-27 11:45:44.145297 browniebroke_utils-1.0.0/src/browniebroke_utils/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 11:45:42.997304 browniebroke_utils-1.0.0/src/browniebroke_utils/py.typed
--rw-r--r--   0        0        0     1106 2023-06-27 11:45:42.997304 browniebroke_utils-1.0.0/src/browniebroke_utils/setup_prettier.py
--rw-r--r--   0        0        0      343 2023-06-27 11:45:42.997304 browniebroke_utils-1.0.0/src/browniebroke_utils/setup_pywatchers.py
--rw-r--r--   0        0        0      264 2023-06-27 11:45:42.997304 browniebroke_utils-1.0.0/src/browniebroke_utils/templates/prettier/prettier.xml
--rw-r--r--   0        0        0      449 2023-06-27 11:45:42.997304 browniebroke_utils-1.0.0/src/browniebroke_utils/templates/prettier/to_add.xml
--rw-r--r--   0        0        0     2731 2023-06-27 11:45:42.997304 browniebroke_utils-1.0.0/src/browniebroke_utils/templates/pywatchers/watchers.xml
--rw-r--r--   0        0        0     5771 1970-01-01 00:00:00.000000 browniebroke_utils-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-19 11:30:19.634081 browniebroke_utils-1.0.1/LICENSE
+-rw-r--r--   0        0        0     4519 2023-07-19 11:30:19.634081 browniebroke_utils-1.0.1/README.md
+-rw-r--r--   0        0        0     2196 2023-07-19 11:30:20.446077 browniebroke_utils-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-19 11:30:19.634081 browniebroke_utils-1.0.1/src/browniebroke_utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-19 11:30:19.634081 browniebroke_utils-1.0.1/src/browniebroke_utils/py.typed
+-rw-r--r--   0        0        0     1106 2023-07-19 11:30:19.634081 browniebroke_utils-1.0.1/src/browniebroke_utils/setup_prettier.py
+-rw-r--r--   0        0        0      343 2023-07-19 11:30:19.634081 browniebroke_utils-1.0.1/src/browniebroke_utils/setup_pywatchers.py
+-rw-r--r--   0        0        0      264 2023-07-19 11:30:19.634081 browniebroke_utils-1.0.1/src/browniebroke_utils/templates/prettier/prettier.xml
+-rw-r--r--   0        0        0      449 2023-07-19 11:30:19.634081 browniebroke_utils-1.0.1/src/browniebroke_utils/templates/prettier/to_add.xml
+-rw-r--r--   0        0        0     2731 2023-07-19 11:30:19.634081 browniebroke_utils-1.0.1/src/browniebroke_utils/templates/pywatchers/watchers.xml
+-rw-r--r--   0        0        0     5771 1970-01-01 00:00:00.000000 browniebroke_utils-1.0.1/PKG-INFO
```

### Comparing `browniebroke_utils-1.0.0/LICENSE` & `browniebroke_utils-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `browniebroke_utils-1.0.0/README.md` & `browniebroke_utils-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `browniebroke_utils-1.0.0/pyproject.toml` & `browniebroke_utils-1.0.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "browniebroke-utils"
-version = "1.0.0"
+version = "1.0.1"
 description = "A collections of small scripts."
 authors = ["Bruno Alla <alla.brunoo@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/browniebroke/browniebroke-utils"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
@@ -34,15 +34,15 @@
 
 [tool.poetry.scripts]
 pych-prettier = "browniebroke_utils.setup_prettier:main"
 pych-pywatchers = "browniebroke_utils.setup_pywatchers:main"
 
 [tool.semantic_release]
 branch = "main"
-version_toml = "pyproject.toml:tool.poetry.version"
+version_toml = ["pyproject.toml:tool.poetry.version"]
 version_variable = "src/browniebroke_utils/__init__.py:__version__"
 build_command = "pip install poetry && poetry build"
 
 [tool.pytest.ini_options]
 addopts = "-v -Wdefault --cov=browniebroke_utils --cov-report=term-missing:skip-covered"
 pythonpath = ["src"]
```

### Comparing `browniebroke_utils-1.0.0/src/browniebroke_utils/setup_prettier.py` & `browniebroke_utils-1.0.1/src/browniebroke_utils/setup_prettier.py`

 * *Files identical despite different names*

### Comparing `browniebroke_utils-1.0.0/src/browniebroke_utils/templates/pywatchers/watchers.xml` & `browniebroke_utils-1.0.1/src/browniebroke_utils/templates/pywatchers/watchers.xml`

 * *Files identical despite different names*

### Comparing `browniebroke_utils-1.0.0/PKG-INFO` & `browniebroke_utils-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: browniebroke-utils
-Version: 1.0.0
+Version: 1.0.1
 Summary: A collections of small scripts.
 Home-page: https://github.com/browniebroke/browniebroke-utils
 License: MIT
 Author: Bruno Alla
 Author-email: alla.brunoo@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: browniebroke-utils Version: 1.0.0 Summary: A
+Metadata-Version: 2.1 Name: browniebroke-utils Version: 1.0.1 Summary: A
 collections of small scripts. Home-page: https://github.com/browniebroke/
 browniebroke-utils License: MIT Author: Bruno Alla Author-email:
 alla.brunoo@gmail.com Requires-Python: >=3.8,<4.0 Classifier: Development
 Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

