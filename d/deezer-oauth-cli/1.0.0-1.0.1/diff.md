# Comparing `tmp/deezer_oauth_cli-1.0.0.tar.gz` & `tmp/deezer_oauth_cli-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deezer_oauth_cli-1.0.0.tar", max compression
+gzip compressed data, was "deezer_oauth_cli-1.0.1.tar", max compression
```

## Comparing `deezer_oauth_cli-1.0.0.tar` & `deezer_oauth_cli-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1068 2023-06-27 11:38:19.540667 deezer_oauth_cli-1.0.0/LICENSE
--rw-r--r--   0        0        0     5350 2023-06-27 11:38:19.540667 deezer_oauth_cli-1.0.0/README.md
--rw-r--r--   0        0        0     2253 2023-06-27 11:38:20.592685 deezer_oauth_cli-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-06-27 11:38:20.564685 deezer_oauth_cli-1.0.0/src/deezer_oauth/__init__.py
--rw-r--r--   0        0        0     1833 2023-06-27 11:38:19.540667 deezer_oauth_cli-1.0.0/src/deezer_oauth/client.py
--rw-r--r--   0        0        0      115 2023-06-27 11:38:19.540667 deezer_oauth_cli-1.0.0/src/deezer_oauth/constants.py
--rw-r--r--   0        0        0     1003 2023-06-27 11:38:19.544667 deezer_oauth_cli-1.0.0/src/deezer_oauth/files.py
--rw-r--r--   0        0        0     1043 2023-06-27 11:38:19.544667 deezer_oauth_cli-1.0.0/src/deezer_oauth/main.py
--rw-r--r--   0        0        0        0 2023-06-27 11:38:19.544667 deezer_oauth_cli-1.0.0/src/deezer_oauth/py.typed
--rw-r--r--   0        0        0     3238 2023-06-27 11:38:19.544667 deezer_oauth_cli-1.0.0/src/deezer_oauth/server.py
--rw-r--r--   0        0        0     6781 1970-01-01 00:00:00.000000 deezer_oauth_cli-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-19 12:48:53.273398 deezer_oauth_cli-1.0.1/LICENSE
+-rw-r--r--   0        0        0     5350 2023-07-19 12:48:53.273398 deezer_oauth_cli-1.0.1/README.md
+-rw-r--r--   0        0        0     2255 2023-07-19 12:48:54.173412 deezer_oauth_cli-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-19 12:48:53.277398 deezer_oauth_cli-1.0.1/src/deezer_oauth/__init__.py
+-rw-r--r--   0        0        0     1833 2023-07-19 12:48:53.277398 deezer_oauth_cli-1.0.1/src/deezer_oauth/client.py
+-rw-r--r--   0        0        0      115 2023-07-19 12:48:53.277398 deezer_oauth_cli-1.0.1/src/deezer_oauth/constants.py
+-rw-r--r--   0        0        0     1003 2023-07-19 12:48:53.277398 deezer_oauth_cli-1.0.1/src/deezer_oauth/files.py
+-rw-r--r--   0        0        0     1043 2023-07-19 12:48:53.277398 deezer_oauth_cli-1.0.1/src/deezer_oauth/main.py
+-rw-r--r--   0        0        0        0 2023-07-19 12:48:53.277398 deezer_oauth_cli-1.0.1/src/deezer_oauth/py.typed
+-rw-r--r--   0        0        0     3238 2023-07-19 12:48:53.277398 deezer_oauth_cli-1.0.1/src/deezer_oauth/server.py
+-rw-r--r--   0        0        0     6781 1970-01-01 00:00:00.000000 deezer_oauth_cli-1.0.1/PKG-INFO
```

### Comparing `deezer_oauth_cli-1.0.0/LICENSE` & `deezer_oauth_cli-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deezer_oauth_cli-1.0.0/README.md` & `deezer_oauth_cli-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `deezer_oauth_cli-1.0.0/pyproject.toml` & `deezer_oauth_cli-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deezer-oauth-cli"
-version = "1.0.0"
+version = "1.0.1"
 description = "A small CLI to quickly obtain an API token for Deezer API."
 authors = ["Bruno Alla <alla.brunoo@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/browniebroke/deezer-oauth-cli"
 documentation = "https://github.com/browniebroke/deezer-oauth-cli/blob/main/README.md"
 classifiers = [
@@ -38,15 +38,15 @@
 pytest = "^7.0"
 pytest-cov = "^4.0"
 pytest-mock = "^3.6"
 responses = "^0.23.0"
 
 [tool.semantic_release]
 branch = "main"
-version_toml = "pyproject.toml:tool.poetry.version"
+version_toml = ["pyproject.toml:tool.poetry.version"]
 version_variable = "src/deezer_oauth/__init__.py:__version__"
 build_command = "pip install poetry && poetry build"
 
 [tool.pytest.ini_options]
 addopts = "-v -Wdefault --cov=deezer_oauth --cov-report=term-missing:skip-covered"
 pythonpath = ["src"]
```

### Comparing `deezer_oauth_cli-1.0.0/src/deezer_oauth/client.py` & `deezer_oauth_cli-1.0.1/src/deezer_oauth/client.py`

 * *Files identical despite different names*

### Comparing `deezer_oauth_cli-1.0.0/src/deezer_oauth/files.py` & `deezer_oauth_cli-1.0.1/src/deezer_oauth/files.py`

 * *Files identical despite different names*

### Comparing `deezer_oauth_cli-1.0.0/src/deezer_oauth/main.py` & `deezer_oauth_cli-1.0.1/src/deezer_oauth/main.py`

 * *Files identical despite different names*

### Comparing `deezer_oauth_cli-1.0.0/src/deezer_oauth/server.py` & `deezer_oauth_cli-1.0.1/src/deezer_oauth/server.py`

 * *Files identical despite different names*

### Comparing `deezer_oauth_cli-1.0.0/PKG-INFO` & `deezer_oauth_cli-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deezer-oauth-cli
-Version: 1.0.0
+Version: 1.0.1
 Summary: A small CLI to quickly obtain an API token for Deezer API.
 Home-page: https://github.com/browniebroke/deezer-oauth-cli
 License: MIT
 Author: Bruno Alla
 Author-email: alla.brunoo@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: deezer-oauth-cli Version: 1.0.0 Summary: A small
+Metadata-Version: 2.1 Name: deezer-oauth-cli Version: 1.0.1 Summary: A small
 CLI to quickly obtain an API token for Deezer API. Home-page: https://
 github.com/browniebroke/deezer-oauth-cli License: MIT Author: Bruno Alla
 Author-email: alla.brunoo@gmail.com Requires-Python: >=3.8,<4.0 Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Natural Language
 :: English Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```

