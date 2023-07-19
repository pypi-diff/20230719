# Comparing `tmp/iamlistening-1.1.4.tar.gz` & `tmp/iamlistening-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamlistening-1.1.4.tar", max compression
+gzip compressed data, was "iamlistening-1.1.5.tar", max compression
```

## Comparing `iamlistening-1.1.4.tar` & `iamlistening-1.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-07-19 06:59:54.740383 iamlistening-1.1.4/LICENSE
--rw-r--r--   0        0        0     2910 2023-07-19 06:59:54.744383 iamlistening-1.1.4/README.md
--rw-r--r--   0        0        0       99 2023-07-19 06:59:55.496390 iamlistening-1.1.4/iamlistening/__init__.py
--rw-r--r--   0        0        0      661 2023-07-19 06:59:54.744383 iamlistening-1.1.4/iamlistening/config.py
--rw-r--r--   0        0        0     1490 2023-07-19 06:59:54.744383 iamlistening-1.1.4/iamlistening/default_settings.toml
--rw-r--r--   0        0        0     4307 2023-07-19 06:59:54.744383 iamlistening-1.1.4/iamlistening/main.py
--rw-r--r--   0        0        0     3093 2023-07-19 06:59:55.496390 iamlistening-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     3837 1970-01-01 00:00:00.000000 iamlistening-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-19 13:21:07.821226 iamlistening-1.1.5/LICENSE
+-rw-r--r--   0        0        0     2910 2023-07-19 13:21:07.821226 iamlistening-1.1.5/README.md
+-rw-r--r--   0        0        0       99 2023-07-19 13:21:09.377240 iamlistening-1.1.5/iamlistening/__init__.py
+-rw-r--r--   0        0        0      661 2023-07-19 13:21:07.821226 iamlistening-1.1.5/iamlistening/config.py
+-rw-r--r--   0        0        0     1490 2023-07-19 13:21:07.821226 iamlistening-1.1.5/iamlistening/default_settings.toml
+-rw-r--r--   0        0        0     4307 2023-07-19 13:21:07.821226 iamlistening-1.1.5/iamlistening/main.py
+-rw-r--r--   0        0        0     3094 2023-07-19 13:21:09.369239 iamlistening-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3837 1970-01-01 00:00:00.000000 iamlistening-1.1.5/PKG-INFO
```

### Comparing `iamlistening-1.1.4/LICENSE` & `iamlistening-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `iamlistening-1.1.4/README.md` & `iamlistening-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `iamlistening-1.1.4/iamlistening/config.py` & `iamlistening-1.1.5/iamlistening/config.py`

 * *Files identical despite different names*

### Comparing `iamlistening-1.1.4/iamlistening/default_settings.toml` & `iamlistening-1.1.5/iamlistening/default_settings.toml`

 * *Files identical despite different names*

### Comparing `iamlistening-1.1.4/iamlistening/main.py` & `iamlistening-1.1.5/iamlistening/main.py`

 * *Files identical despite different names*

### Comparing `iamlistening-1.1.4/pyproject.toml` & `iamlistening-1.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "iamlistening"
-version = "1.1.4"
+version = "1.1.5"
 description = "A python package to interact with messaging platform."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["discord", "telegram", "bot","messaging","matrix"]
 packages = [
     {include = "iamlistening"}
@@ -23,15 +23,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.10"
 dynaconf = "^3.1.12"
 telethon= "^1.28.5"
 py-cord= "^2.4.1"
 simplematrixbotlib= "^2.9.0"
-
+ 
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^8.0.1"
 ruff = "^0.0.278"
 
 [tool.ruff]
 select = [
```

### Comparing `iamlistening-1.1.4/PKG-INFO` & `iamlistening-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iamlistening
-Version: 1.1.4
+Version: 1.1.5
 Summary: A python package to interact with messaging platform.
 License: MIT
 Keywords: discord,telegram,bot,messaging,matrix
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iamlistening Version: 1.1.4 Summary: A python
+Metadata-Version: 2.1 Name: iamlistening Version: 1.1.5 Summary: A python
 package to interact with messaging platform. License: MIT Keywords:
 discord,telegram,bot,messaging,matrix Author: mraniki Author-email:
 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: dynaconf
 (>=3.1.12,<4.0.0) Requires-Dist: py-cord (>=2.4.1,<3.0.0) Requires-Dist:
```

