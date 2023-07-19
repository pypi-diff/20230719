# Comparing `tmp/jwt_pydantic-0.0.6.tar.gz` & `tmp/jwt_pydantic-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jwt_pydantic-0.0.6.tar", last modified: Wed Jan 25 16:53:15 2023, max compression
+gzip compressed data, was "jwt_pydantic-0.0.7.tar", last modified: Wed Jul 19 10:43:33 2023, max compression
```

## Comparing `jwt_pydantic-0.0.6.tar` & `jwt_pydantic-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 16:53:15.800281 jwt_pydantic-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-01-25 16:52:59.000000 jwt_pydantic-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-01-25 16:53:15.800281 jwt_pydantic-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-01-25 16:52:59.000000 jwt_pydantic-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 16:53:15.800281 jwt_pydantic-0.0.6/jwt_pydantic/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-01-25 16:52:59.000000 jwt_pydantic-0.0.6/jwt_pydantic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-01-25 16:52:59.000000 jwt_pydantic-0.0.6/jwt_pydantic/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-01-25 16:52:59.000000 jwt_pydantic-0.0.6/jwt_pydantic/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 16:53:15.800281 jwt_pydantic-0.0.6/jwt_pydantic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-01-25 16:53:15.000000 jwt_pydantic-0.0.6/jwt_pydantic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-01-25 16:53:15.000000 jwt_pydantic-0.0.6/jwt_pydantic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-25 16:53:15.000000 jwt_pydantic-0.0.6/jwt_pydantic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-01-25 16:53:15.000000 jwt_pydantic-0.0.6/jwt_pydantic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-25 16:53:15.000000 jwt_pydantic-0.0.6/jwt_pydantic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-01-25 16:52:59.000000 jwt_pydantic-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-25 16:53:15.800281 jwt_pydantic-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:43:33.573270 jwt_pydantic-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-19 10:43:16.000000 jwt_pydantic-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-07-19 10:43:33.573270 jwt_pydantic-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-07-19 10:43:16.000000 jwt_pydantic-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:43:33.573270 jwt_pydantic-0.0.7/jwt_pydantic/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-19 10:43:16.000000 jwt_pydantic-0.0.7/jwt_pydantic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-07-19 10:43:16.000000 jwt_pydantic-0.0.7/jwt_pydantic/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-07-19 10:43:16.000000 jwt_pydantic-0.0.7/jwt_pydantic/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:43:33.573270 jwt_pydantic-0.0.7/jwt_pydantic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-07-19 10:43:33.000000 jwt_pydantic-0.0.7/jwt_pydantic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-19 10:43:33.000000 jwt_pydantic-0.0.7/jwt_pydantic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 10:43:33.000000 jwt_pydantic-0.0.7/jwt_pydantic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-19 10:43:33.000000 jwt_pydantic-0.0.7/jwt_pydantic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-19 10:43:33.000000 jwt_pydantic-0.0.7/jwt_pydantic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-19 10:43:16.000000 jwt_pydantic-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 10:43:33.573270 jwt_pydantic-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:43:33.573270 jwt_pydantic-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-19 10:43:16.000000 jwt_pydantic-0.0.7/tests/test_jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-19 10:43:16.000000 jwt_pydantic-0.0.7/tests/test_middleware.py
```

### Comparing `jwt_pydantic-0.0.6/LICENSE` & `jwt_pydantic-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `jwt_pydantic-0.0.6/PKG-INFO` & `jwt_pydantic-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jwt_pydantic
-Version: 0.0.6
+Version: 0.0.7
 Summary: Verify JWT claims using the powerful features of Pydantic.
 Author: Adam Powis
 License: The MIT License (MIT)
         
         Copyright (c) 2022 Adam Powis
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `jwt_pydantic-0.0.6/README.md` & `jwt_pydantic-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `jwt_pydantic-0.0.6/jwt_pydantic/main.py` & `jwt_pydantic-0.0.7/jwt_pydantic/main.py`

 * *Files identical despite different names*

### Comparing `jwt_pydantic-0.0.6/jwt_pydantic/middleware.py` & `jwt_pydantic-0.0.7/jwt_pydantic/middleware.py`

 * *Files identical despite different names*

### Comparing `jwt_pydantic-0.0.6/jwt_pydantic.egg-info/PKG-INFO` & `jwt_pydantic-0.0.7/jwt_pydantic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jwt-pydantic
-Version: 0.0.6
+Version: 0.0.7
 Summary: Verify JWT claims using the powerful features of Pydantic.
 Author: Adam Powis
 License: The MIT License (MIT)
         
         Copyright (c) 2022 Adam Powis
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `jwt_pydantic-0.0.6/pyproject.toml` & `jwt_pydantic-0.0.7/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [build-system]
+
 requires = ["setuptools >= 65.5.0","wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jwt_pydantic"
 description = "Verify JWT claims using the powerful features of Pydantic."
-version = "0.0.6"
+version = "0.0.7"
 authors = [{name = "Adam Powis"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License"]
 requires-python = ">=3.8.0"
 dependencies = [
     "httpx",
```

