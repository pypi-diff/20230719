# Comparing `tmp/contactapi-0.0.16.tar.gz` & `tmp/contactapi-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contactapi-0.0.16.tar", last modified: Wed Jul 19 10:15:38 2023, max compression
+gzip compressed data, was "contactapi-0.0.17.tar", last modified: Wed Jul 19 10:20:56 2023, max compression
```

## Comparing `contactapi-0.0.16.tar` & `contactapi-0.0.17.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:15:38.501173 contactapi-0.0.16/
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-19 10:15:38.501173 contactapi-0.0.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-19 10:15:28.000000 contactapi-0.0.16/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-19 10:15:28.000000 contactapi-0.0.16/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 10:15:38.501173 contactapi-0.0.16/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:15:38.497173 contactapi-0.0.16/src/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-19 10:15:28.000000 contactapi-0.0.16/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-19 10:15:28.000000 contactapi-0.0.16/src/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-19 10:15:28.000000 contactapi-0.0.16/src/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:15:38.497173 contactapi-0.0.16/src/contactapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-19 10:15:38.000000 contactapi-0.0.16/src/contactapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-19 10:15:38.000000 contactapi-0.0.16/src/contactapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 10:15:38.000000 contactapi-0.0.16/src/contactapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-19 10:15:38.000000 contactapi-0.0.16/src/contactapi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-19 10:15:38.000000 contactapi-0.0.16/src/contactapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-19 10:15:38.000000 contactapi-0.0.16/src/contactapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-19 10:15:28.000000 contactapi-0.0.16/src/crud.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-19 10:15:28.000000 contactapi-0.0.16/src/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-19 10:15:28.000000 contactapi-0.0.16/src/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-19 10:15:28.000000 contactapi-0.0.16/src/router.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-19 10:15:28.000000 contactapi-0.0.16/src/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:20:56.734940 contactapi-0.0.17/
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-19 10:20:56.734940 contactapi-0.0.17/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-19 10:20:45.000000 contactapi-0.0.17/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-19 10:20:45.000000 contactapi-0.0.17/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 10:20:56.734940 contactapi-0.0.17/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:20:56.734940 contactapi-0.0.17/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-19 10:20:45.000000 contactapi-0.0.17/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-19 10:20:45.000000 contactapi-0.0.17/src/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-19 10:20:45.000000 contactapi-0.0.17/src/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:20:56.734940 contactapi-0.0.17/src/contactapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-19 10:20:56.000000 contactapi-0.0.17/src/contactapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-19 10:20:56.000000 contactapi-0.0.17/src/contactapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 10:20:56.000000 contactapi-0.0.17/src/contactapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-19 10:20:56.000000 contactapi-0.0.17/src/contactapi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-19 10:20:56.000000 contactapi-0.0.17/src/contactapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-19 10:20:56.000000 contactapi-0.0.17/src/contactapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-19 10:20:45.000000 contactapi-0.0.17/src/crud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-19 10:20:45.000000 contactapi-0.0.17/src/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-19 10:20:45.000000 contactapi-0.0.17/src/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-19 10:20:45.000000 contactapi-0.0.17/src/router.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-19 10:20:45.000000 contactapi-0.0.17/src/schemas.py
```

### Comparing `contactapi-0.0.16/PKG-INFO` & `contactapi-0.0.17/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contactapi
-Version: 0.0.16
+Version: 0.0.17
 Summary: Just a demo project
 Keywords: flask,project
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # fastapi
```

### Comparing `contactapi-0.0.16/README.md` & `contactapi-0.0.17/README.md`

 * *Files identical despite different names*

### Comparing `contactapi-0.0.16/src/config.py` & `contactapi-0.0.17/src/config.py`

 * *Files identical despite different names*

### Comparing `contactapi-0.0.16/src/contactapi.egg-info/PKG-INFO` & `contactapi-0.0.17/src/contactapi.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contactapi
-Version: 0.0.16
+Version: 0.0.17
 Summary: Just a demo project
 Keywords: flask,project
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # fastapi
```

### Comparing `contactapi-0.0.16/src/crud.py` & `contactapi-0.0.17/src/crud.py`

 * *Files identical despite different names*

### Comparing `contactapi-0.0.16/src/router.py` & `contactapi-0.0.17/src/router.py`

 * *Files identical despite different names*

