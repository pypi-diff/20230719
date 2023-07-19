# Comparing `tmp/contactapi-0.0.17.tar.gz` & `tmp/contactapi-0.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contactapi-0.0.17.tar", last modified: Wed Jul 19 10:20:56 2023, max compression
+gzip compressed data, was "contactapi-0.0.18.tar", last modified: Wed Jul 19 10:31:44 2023, max compression
```

## Comparing `contactapi-0.0.17.tar` & `contactapi-0.0.18.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:20:56.734940 contactapi-0.0.17/
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-19 10:20:56.734940 contactapi-0.0.17/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-19 10:20:45.000000 contactapi-0.0.17/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-19 10:20:45.000000 contactapi-0.0.17/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 10:20:56.734940 contactapi-0.0.17/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:20:56.734940 contactapi-0.0.17/src/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-19 10:20:45.000000 contactapi-0.0.17/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-19 10:20:45.000000 contactapi-0.0.17/src/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-19 10:20:45.000000 contactapi-0.0.17/src/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:20:56.734940 contactapi-0.0.17/src/contactapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-19 10:20:56.000000 contactapi-0.0.17/src/contactapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-19 10:20:56.000000 contactapi-0.0.17/src/contactapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 10:20:56.000000 contactapi-0.0.17/src/contactapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-19 10:20:56.000000 contactapi-0.0.17/src/contactapi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-19 10:20:56.000000 contactapi-0.0.17/src/contactapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-19 10:20:56.000000 contactapi-0.0.17/src/contactapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-19 10:20:45.000000 contactapi-0.0.17/src/crud.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-19 10:20:45.000000 contactapi-0.0.17/src/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-19 10:20:45.000000 contactapi-0.0.17/src/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-19 10:20:45.000000 contactapi-0.0.17/src/router.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-19 10:20:45.000000 contactapi-0.0.17/src/schemas.py
+drwxrwxr-x   0 yulai     (1000) yulai     (1000)        0 2023-07-19 10:31:44.046672 contactapi-0.0.18/
+-rw-rw-r--   0 yulai     (1000) yulai     (1000)      857 2023-07-19 10:31:44.046672 contactapi-0.0.18/PKG-INFO
+-rw-rw-r--   0 yulai     (1000) yulai     (1000)      681 2023-07-19 08:06:58.000000 contactapi-0.0.18/README.md
+-rw-rw-r--   0 yulai     (1000) yulai     (1000)      367 2023-07-19 10:31:18.000000 contactapi-0.0.18/pyproject.toml
+-rw-rw-r--   0 yulai     (1000) yulai     (1000)       38 2023-07-19 10:31:44.050673 contactapi-0.0.18/setup.cfg
+drwxrwxr-x   0 yulai     (1000) yulai     (1000)        0 2023-07-19 10:31:44.038672 contactapi-0.0.18/src/
+-rw-rw-r--   0 yulai     (1000) yulai     (1000)       21 2023-07-19 10:13:50.000000 contactapi-0.0.18/src/__init__.py
+-rw-rw-r--   0 yulai     (1000) yulai     (1000)      182 2023-07-19 10:04:10.000000 contactapi-0.0.18/src/__main__.py
+-rw-rw-r--   0 yulai     (1000) yulai     (1000)      745 2023-07-17 04:44:55.000000 contactapi-0.0.18/src/config.py
+drwxrwxr-x   0 yulai     (1000) yulai     (1000)        0 2023-07-19 10:31:44.046672 contactapi-0.0.18/src/contactapi.egg-info/
+-rw-rw-r--   0 yulai     (1000) yulai     (1000)      857 2023-07-19 10:31:43.000000 contactapi-0.0.18/src/contactapi.egg-info/PKG-INFO
+-rw-rw-r--   0 yulai     (1000) yulai     (1000)      367 2023-07-19 10:31:44.000000 contactapi-0.0.18/src/contactapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 yulai     (1000) yulai     (1000)        1 2023-07-19 10:31:43.000000 contactapi-0.0.18/src/contactapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 yulai     (1000) yulai     (1000)       48 2023-07-19 10:31:43.000000 contactapi-0.0.18/src/contactapi.egg-info/entry_points.txt
+-rw-rw-r--   0 yulai     (1000) yulai     (1000)       27 2023-07-19 10:31:43.000000 contactapi-0.0.18/src/contactapi.egg-info/requires.txt
+-rw-rw-r--   0 yulai     (1000) yulai     (1000)       57 2023-07-19 10:31:43.000000 contactapi-0.0.18/src/contactapi.egg-info/top_level.txt
+-rw-rw-r--   0 yulai     (1000) yulai     (1000)      941 2023-07-14 18:20:21.000000 contactapi-0.0.18/src/crud.py
+-rw-rw-r--   0 yulai     (1000) yulai     (1000)      285 2023-07-17 13:46:37.000000 contactapi-0.0.18/src/main.py
+-rw-rw-r--   0 yulai     (1000) yulai     (1000)      224 2023-07-19 10:11:32.000000 contactapi-0.0.18/src/models.py
+-rw-rw-r--   0 yulai     (1000) yulai     (1000)     1355 2023-07-19 10:10:37.000000 contactapi-0.0.18/src/router.py
+-rw-rw-r--   0 yulai     (1000) yulai     (1000)      306 2023-07-14 18:20:21.000000 contactapi-0.0.18/src/schemas.py
```

### Comparing `contactapi-0.0.17/PKG-INFO` & `contactapi-0.0.18/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: contactapi
-Version: 0.0.17
+Version: 0.0.18
 Summary: Just a demo project
-Keywords: flask,project
+Keywords: fastapi,project
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # fastapi
 
 # Runing API via podman
```

### Comparing `contactapi-0.0.17/README.md` & `contactapi-0.0.18/README.md`

 * *Files identical despite different names*

### Comparing `contactapi-0.0.17/src/config.py` & `contactapi-0.0.18/src/config.py`

 * *Files identical despite different names*

### Comparing `contactapi-0.0.17/src/contactapi.egg-info/PKG-INFO` & `contactapi-0.0.18/src/contactapi.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: contactapi
-Version: 0.0.17
+Version: 0.0.18
 Summary: Just a demo project
-Keywords: flask,project
+Keywords: fastapi,project
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # fastapi
 
 # Runing API via podman
```

### Comparing `contactapi-0.0.17/src/crud.py` & `contactapi-0.0.18/src/crud.py`

 * *Files identical despite different names*

### Comparing `contactapi-0.0.17/src/router.py` & `contactapi-0.0.18/src/router.py`

 * *Files identical despite different names*

