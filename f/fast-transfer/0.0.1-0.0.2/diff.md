# Comparing `tmp/fast-transfer-0.0.1.tar.gz` & `tmp/fast_transfer-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast-transfer-0.0.1.tar", last modified: Wed Jul 19 06:16:24 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `fast-transfer-0.0.1.tar` & `fast_transfer-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,9 @@
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-07-19 06:16:24.243320 fast-transfer-0.0.1/
--rw-r--r--   0 chen      (1000) chen      (1000)     1063 2023-07-19 03:04:47.000000 fast-transfer-0.0.1/LICENSE
--rw-r--r--   0 chen      (1000) chen      (1000)      760 2023-07-19 06:16:24.243320 fast-transfer-0.0.1/PKG-INFO
--rw-r--r--   0 chen      (1000) chen      (1000)      244 2023-07-19 06:06:24.000000 fast-transfer-0.0.1/README.md
--rw-r--r--   0 chen      (1000) chen      (1000)      589 2023-07-19 06:09:55.000000 fast-transfer-0.0.1/pyproject.toml
--rw-r--r--   0 chen      (1000) chen      (1000)       38 2023-07-19 06:16:24.243320 fast-transfer-0.0.1/setup.cfg
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-07-19 06:16:24.243320 fast-transfer-0.0.1/src/
--rw-r--r--   0 chen      (1000) chen      (1000)     2028 2023-07-19 06:02:39.000000 fast-transfer-0.0.1/src/app.py
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-07-19 06:16:24.243320 fast-transfer-0.0.1/src/fast_transfer.egg-info/
--rw-r--r--   0 chen      (1000) chen      (1000)      760 2023-07-19 06:16:24.000000 fast-transfer-0.0.1/src/fast_transfer.egg-info/PKG-INFO
--rw-r--r--   0 chen      (1000) chen      (1000)      207 2023-07-19 06:16:24.000000 fast-transfer-0.0.1/src/fast_transfer.egg-info/SOURCES.txt
--rw-r--r--   0 chen      (1000) chen      (1000)        1 2023-07-19 06:16:24.000000 fast-transfer-0.0.1/src/fast_transfer.egg-info/dependency_links.txt
--rw-r--r--   0 chen      (1000) chen      (1000)       27 2023-07-19 06:16:24.000000 fast-transfer-0.0.1/src/fast_transfer.egg-info/top_level.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fast_transfer-0.0.2/src/fast-transfer/__init__.py
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 fast_transfer-0.0.2/src/fast-transfer/app.py
+-rw-r--r--   0        0        0   207302 2020-02-02 00:00:00.000000 fast_transfer-0.0.2/src/fast-transfer/static/bulma.min.css
+-rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 fast_transfer-0.0.2/src/fast-transfer/templates/index.html
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 fast_transfer-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 fast_transfer-0.0.2/LICENSE
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 fast_transfer-0.0.2/README.md
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 fast_transfer-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 fast_transfer-0.0.2/PKG-INFO
```

### Comparing `fast-transfer-0.0.1/LICENSE` & `fast_transfer-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fast-transfer-0.0.1/PKG-INFO` & `fast_transfer-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: fast-transfer
-Version: 0.0.1
+Version: 0.0.2
 Summary: An easy and fast way to transfer files
-Author-email: ChanMo <chan.mo@outlook.com>
 Project-URL: Homepage, https://github.com/ChanMo/fast-transfer
 Project-URL: Bug Tracker, https://github.com/ChanMo/fast-transfer/issues
-Classifier: Programming Language :: Python :: 3
+Author-email: ChanMo <chan.mo@outlook.com>
+License-File: LICENSE
+Keywords: fast-transfer,http.server,share,transfer
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
+Requires-Dist: click
+Requires-Dist: flask
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # Fast Transfer
 
 An easy and fast way to transfer files between mulitple users.
 If you offten run the command `python -m http.server`, you will like it.
```

### Comparing `fast-transfer-0.0.1/pyproject.toml` & `fast_transfer-0.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 [project]
 name = "fast-transfer"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="ChanMo", email="chan.mo@outlook.com" },
 ]
+keywords = ["http.server", "transfer", "share", "fast-transfer"]
 description = "An easy and fast way to transfer files"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+  "click",
+  "flask"
+]
 
 [project.urls]
 "Homepage" = "https://github.com/ChanMo/fast-transfer"
 "Bug Tracker" = "https://github.com/ChanMo/fast-transfer/issues"
 
 [build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
+requires = ["hatchling"]
+build-backend = "hatchling.build"
```

### Comparing `fast-transfer-0.0.1/src/app.py` & `fast_transfer-0.0.2/src/fast-transfer/app.py`

 * *Files identical despite different names*

