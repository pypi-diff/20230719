# Comparing `tmp/iamlistening-1.1.1.tar.gz` & `tmp/iamlistening-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamlistening-1.1.1.tar", max compression
+gzip compressed data, was "iamlistening-1.1.2.tar", max compression
```

## Comparing `iamlistening-1.1.1.tar` & `iamlistening-1.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-07-18 22:00:43.761457 iamlistening-1.1.1/LICENSE
--rw-r--r--   0        0        0     2910 2023-07-18 22:00:43.761457 iamlistening-1.1.1/README.md
--rw-r--r--   0        0        0       99 2023-07-18 22:00:44.801473 iamlistening-1.1.1/iamlistening/__init__.py
--rw-r--r--   0        0        0      661 2023-07-18 22:00:43.761457 iamlistening-1.1.1/iamlistening/config.py
--rw-r--r--   0        0        0     1490 2023-07-18 22:00:43.761457 iamlistening-1.1.1/iamlistening/default_settings.toml
--rw-r--r--   0        0        0     4307 2023-07-18 22:00:43.761457 iamlistening-1.1.1/iamlistening/main.py
--rw-r--r--   0        0        0     3075 2023-07-18 22:00:44.801473 iamlistening-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     3837 1970-01-01 00:00:00.000000 iamlistening-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-18 22:09:57.004128 iamlistening-1.1.2/LICENSE
+-rw-r--r--   0        0        0     2910 2023-07-18 22:09:57.004128 iamlistening-1.1.2/README.md
+-rw-r--r--   0        0        0       99 2023-07-18 22:09:57.784129 iamlistening-1.1.2/iamlistening/__init__.py
+-rw-r--r--   0        0        0      661 2023-07-18 22:09:57.004128 iamlistening-1.1.2/iamlistening/config.py
+-rw-r--r--   0        0        0     1490 2023-07-18 22:09:57.004128 iamlistening-1.1.2/iamlistening/default_settings.toml
+-rw-r--r--   0        0        0     4307 2023-07-18 22:09:57.004128 iamlistening-1.1.2/iamlistening/main.py
+-rw-r--r--   0        0        0     3075 2023-07-18 22:09:57.784129 iamlistening-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3837 1970-01-01 00:00:00.000000 iamlistening-1.1.2/PKG-INFO
```

### Comparing `iamlistening-1.1.1/LICENSE` & `iamlistening-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iamlistening-1.1.1/README.md` & `iamlistening-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `iamlistening-1.1.1/iamlistening/config.py` & `iamlistening-1.1.2/iamlistening/config.py`

 * *Files identical despite different names*

### Comparing `iamlistening-1.1.1/iamlistening/default_settings.toml` & `iamlistening-1.1.2/iamlistening/default_settings.toml`

 * *Files identical despite different names*

### Comparing `iamlistening-1.1.1/iamlistening/main.py` & `iamlistening-1.1.2/iamlistening/main.py`

 * *Files identical despite different names*

### Comparing `iamlistening-1.1.1/pyproject.toml` & `iamlistening-1.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "iamlistening"
-version = "1.1.1"
+version = "1.1.2"
 description = "A python package to interact with messaging platform."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["discord", "telegram", "bot","messaging","matrix"]
 packages = [
     {include = "iamlistening"}
```

### Comparing `iamlistening-1.1.1/PKG-INFO` & `iamlistening-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iamlistening
-Version: 1.1.1
+Version: 1.1.2
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
-Metadata-Version: 2.1 Name: iamlistening Version: 1.1.1 Summary: A python
+Metadata-Version: 2.1 Name: iamlistening Version: 1.1.2 Summary: A python
 package to interact with messaging platform. License: MIT Keywords:
 discord,telegram,bot,messaging,matrix Author: mraniki Author-email:
 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: dynaconf
 (>=3.1.12,<4.0.0) Requires-Dist: py-cord (>=2.4.1,<3.0.0) Requires-Dist:
```

