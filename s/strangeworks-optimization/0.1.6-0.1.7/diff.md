# Comparing `tmp/strangeworks_optimization-0.1.6.tar.gz` & `tmp/strangeworks_optimization-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strangeworks_optimization-0.1.6.tar", max compression
+gzip compressed data, was "strangeworks_optimization-0.1.7.tar", max compression
```

## Comparing `strangeworks_optimization-0.1.6.tar` & `strangeworks_optimization-0.1.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      196 2023-07-17 21:42:14.320216 strangeworks_optimization-0.1.6/README.md
--rw-r--r--   0        0        0     1009 2023-07-17 21:42:27.824425 strangeworks_optimization-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      174 2023-07-17 21:42:14.320216 strangeworks_optimization-0.1.6/strangeworks_optimization/__init__.py
--rw-r--r--   0        0        0     4438 2023-07-17 21:42:14.320216 strangeworks_optimization-0.1.6/strangeworks_optimization/optimization.py
--rw-r--r--   0        0        0      907 1970-01-01 00:00:00.000000 strangeworks_optimization-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      196 2023-07-19 15:49:19.087108 strangeworks_optimization-0.1.7/README.md
+-rw-r--r--   0        0        0     1009 2023-07-19 15:49:35.175371 strangeworks_optimization-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      174 2023-07-19 15:49:19.087108 strangeworks_optimization-0.1.7/strangeworks_optimization/__init__.py
+-rw-r--r--   0        0        0     5827 2023-07-19 15:49:19.087108 strangeworks_optimization-0.1.7/strangeworks_optimization/optimization.py
+-rw-r--r--   0        0        0      907 1970-01-01 00:00:00.000000 strangeworks_optimization-0.1.7/PKG-INFO
```

### Comparing `strangeworks_optimization-0.1.6/pyproject.toml` & `strangeworks_optimization-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strangeworks-optimization"
-version = "0.1.6"
+version = "0.1.7"
 description = "This SDK extends the Strangeworks SDK to provide access to the Strangeworks Optimization API."
 authors = ["Strange Devs <hello@strangeworks.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 packages = [{include = "strangeworks_optimization"}]
```

### Comparing `strangeworks_optimization-0.1.6/PKG-INFO` & `strangeworks_optimization-0.1.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strangeworks-optimization
-Version: 0.1.6
+Version: 0.1.7
 Summary: This SDK extends the Strangeworks SDK to provide access to the Strangeworks Optimization API.
 License: Apache-2.0
 Author: Strange Devs
 Author-email: hello@strangeworks.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

