# Comparing `tmp/dvv-0.0.1.tar.gz` & `tmp/dvv-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvv-0.0.1.tar", max compression
+gzip compressed data, was "dvv-0.0.3.tar", max compression
```

## Comparing `dvv-0.0.1.tar` & `dvv-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-07-17 19:09:10.564827 dvv-0.0.1/LICENSE
--rw-r--r--   0        0        0      594 2023-07-17 22:07:32.960639 dvv-0.0.1/README.md
--rw-r--r--   0        0        0      109 2023-07-17 23:12:54.237805 dvv-0.0.1/dvv/__init__.py
--rw-r--r--   0        0        0        0 2023-07-17 19:34:03.101809 dvv-0.0.1/dvv/algorithm/__init__.py
--rw-r--r--   0        0        0      361 2023-07-17 19:37:18.773721 dvv-0.0.1/dvv/algorithm/mwcs.py
--rw-r--r--   0        0        0        0 2023-07-17 19:30:17.886704 dvv-0.0.1/dvv/coda_kernel/__init__.py
--rw-r--r--   0        0        0        0 2023-07-17 19:31:32.582874 dvv-0.0.1/dvv/surf_kernel/__init__.py
--rw-r--r--   0        0        0        0 2023-07-17 21:30:21.038608 dvv-0.0.1/dvv/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-07-17 21:31:25.436599 dvv-0.0.1/dvv/tests/test_algorithm/__init__.py
--rw-r--r--   0        0        0      157 2023-07-17 21:30:52.422068 dvv-0.0.1/dvv/tests/test_algorithm/test_mwcs.py
--rw-r--r--   0        0        0        0 2023-07-17 21:31:42.135786 dvv-0.0.1/dvv/tests/test_coda_kernel/__init__.py
--rw-r--r--   0        0        0        0 2023-07-17 21:31:55.124452 dvv-0.0.1/dvv/tests/test_surf_kernel/__init__.py
--rw-r--r--   0        0        0     1501 2023-07-18 21:25:26.521182 dvv-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1478 1970-01-01 00:00:00.000000 dvv-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-18 22:16:50.242289 dvv-0.0.3/LICENSE
+-rw-r--r--   0        0        0      594 2023-07-18 22:16:50.242289 dvv-0.0.3/README.md
+-rw-r--r--   0        0        0      109 2023-07-18 22:16:50.242289 dvv-0.0.3/dvv/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-18 22:16:50.242289 dvv-0.0.3/dvv/algorithm/__init__.py
+-rw-r--r--   0        0        0      361 2023-07-18 22:16:50.242289 dvv-0.0.3/dvv/algorithm/mwcs.py
+-rw-r--r--   0        0        0        0 2023-07-18 22:16:50.242289 dvv-0.0.3/dvv/coda_kernel/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-18 22:16:50.242289 dvv-0.0.3/dvv/surf_kernel/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-18 22:16:50.242289 dvv-0.0.3/dvv/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-18 22:16:50.242289 dvv-0.0.3/dvv/tests/test_algorithm/__init__.py
+-rw-r--r--   0        0        0      157 2023-07-18 22:16:50.242289 dvv-0.0.3/dvv/tests/test_algorithm/test_mwcs.py
+-rw-r--r--   0        0        0        0 2023-07-18 22:16:50.242289 dvv-0.0.3/dvv/tests/test_coda_kernel/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-18 22:16:50.242289 dvv-0.0.3/dvv/tests/test_surf_kernel/__init__.py
+-rw-r--r--   0        0        0     1501 2023-07-18 22:16:50.246289 dvv-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1478 1970-01-01 00:00:00.000000 dvv-0.0.3/PKG-INFO
```

### Comparing `dvv-0.0.1/LICENSE` & `dvv-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dvv-0.0.1/README.md` & `dvv-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `dvv-0.0.1/pyproject.toml` & `dvv-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dvv"
-version = "0.0.1"
+version = "0.0.3"
 description = "Seismic dv/v analysis"
 authors = ["OUCyf <oucyinfu@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 include = ["pyproject.toml", "dvv/**/*.py"]
 classifiers = [
         "Development Status :: 2 - Pre-Alpha",
```

### Comparing `dvv-0.0.1/PKG-INFO` & `dvv-0.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvv
-Version: 0.0.1
+Version: 0.0.3
 Summary: Seismic dv/v analysis
 License: Apache-2.0
 Author: OUCyf
 Author-email: oucyinfu@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
```

