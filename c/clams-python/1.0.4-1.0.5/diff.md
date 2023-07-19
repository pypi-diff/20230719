# Comparing `tmp/clams-python-1.0.4.tar.gz` & `tmp/clams-python-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clams-python-1.0.4.tar", last modified: Wed Jul 19 05:31:23 2023, max compression
+gzip compressed data, was "clams-python-1.0.5.tar", last modified: Wed Jul 19 07:41:45 2023, max compression
```

## Comparing `clams-python-1.0.4.tar` & `clams-python-1.0.5.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:31:23.009792 clams-python-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-07-19 05:30:48.000000 clams-python-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-19 05:30:48.000000 clams-python-1.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-19 05:31:23.005792 clams-python-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-19 05:30:48.000000 clams-python-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-19 05:30:48.000000 clams-python-1.0.4/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:31:23.001792 clams-python-1.0.4/clams/
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-19 05:30:48.000000 clams-python-1.0.4/clams/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:31:23.001792 clams-python-1.0.4/clams/app/
--rw-r--r--   0 runner    (1001) docker     (123)    12038 2023-07-19 05:30:48.000000 clams-python-1.0.4/clams/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:31:23.001792 clams-python-1.0.4/clams/appmetadata/
--rw-r--r--   0 runner    (1001) docker     (123)    16533 2023-07-19 05:30:48.000000 clams-python-1.0.4/clams/appmetadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:31:23.001792 clams-python-1.0.4/clams/develop/
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-07-19 05:30:48.000000 clams-python-1.0.4/clams/develop/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:31:22.997792 clams-python-1.0.4/clams/develop/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:31:23.001792 clams-python-1.0.4/clams/develop/templates/app/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-19 05:30:48.000000 clams-python-1.0.4/clams/develop/templates/app/.dockerignore.template
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-19 05:30:48.000000 clams-python-1.0.4/clams/develop/templates/app/.gitignore.template
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-19 05:30:48.000000 clams-python-1.0.4/clams/develop/templates/app/Containerfile.template
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-19 05:30:48.000000 clams-python-1.0.4/clams/develop/templates/app/LICENSE.template
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-07-19 05:30:48.000000 clams-python-1.0.4/clams/develop/templates/app/README.md.template
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-19 05:30:48.000000 clams-python-1.0.4/clams/develop/templates/app/app.py.template
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-19 05:30:48.000000 clams-python-1.0.4/clams/develop/templates/app/metadata.py.template
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-19 05:30:48.000000 clams-python-1.0.4/clams/develop/templates/app/requirements.txt.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:31:23.005792 clams-python-1.0.4/clams/develop/templates/gha/
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-19 05:30:48.000000 clams-python-1.0.4/clams/develop/templates/gha/for-clams-team.md.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:31:23.005792 clams-python-1.0.4/clams/develop/templates/gha/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-19 05:30:48.000000 clams-python-1.0.4/clams/develop/templates/gha/workflows/issue-apps-project.yml.template
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-19 05:30:48.000000 clams-python-1.0.4/clams/develop/templates/gha/workflows/issue-assign.yml.template
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-19 05:30:48.000000 clams-python-1.0.4/clams/develop/templates/gha/workflows/issue-close.yml.template
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-19 05:30:48.000000 clams-python-1.0.4/clams/develop/templates/gha/workflows/publish.yml.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:31:23.005792 clams-python-1.0.4/clams/restify/
--rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-07-19 05:30:48.000000 clams-python-1.0.4/clams/restify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:31:23.005792 clams-python-1.0.4/clams/serve/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-19 05:30:48.000000 clams-python-1.0.4/clams/serve/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:31:23.005792 clams-python-1.0.4/clams/source/
--rw-r--r--   0 runner    (1001) docker     (123)    11761 2023-07-19 05:30:48.000000 clams-python-1.0.4/clams/source/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:31:23.005792 clams-python-1.0.4/clams/ver/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-19 05:31:22.000000 clams-python-1.0.4/clams/ver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:31:23.005792 clams-python-1.0.4/clams_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-19 05:31:22.000000 clams-python-1.0.4/clams_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-19 05:31:22.000000 clams-python-1.0.4/clams_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 05:31:22.000000 clams-python-1.0.4/clams_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-19 05:31:22.000000 clams-python-1.0.4/clams_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-19 05:31:22.000000 clams-python-1.0.4/clams_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-19 05:31:22.000000 clams-python-1.0.4/clams_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-19 05:30:48.000000 clams-python-1.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 05:31:23.009792 clams-python-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-07-19 05:30:48.000000 clams-python-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:31:23.005792 clams-python-1.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    17330 2023-07-19 05:30:48.000000 clams-python-1.0.4/tests/test_clamsapp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-07-19 05:30:48.000000 clams-python-1.0.4/tests/test_clamscli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:41:45.561348 clams-python-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-07-19 07:41:09.000000 clams-python-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-19 07:41:09.000000 clams-python-1.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-19 07:41:45.561348 clams-python-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-19 07:41:09.000000 clams-python-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-19 07:41:10.000000 clams-python-1.0.5/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:41:45.557348 clams-python-1.0.5/clams/
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-19 07:41:09.000000 clams-python-1.0.5/clams/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:41:45.557348 clams-python-1.0.5/clams/app/
+-rw-r--r--   0 runner    (1001) docker     (123)    12038 2023-07-19 07:41:09.000000 clams-python-1.0.5/clams/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:41:45.557348 clams-python-1.0.5/clams/appmetadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    16533 2023-07-19 07:41:09.000000 clams-python-1.0.5/clams/appmetadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:41:45.557348 clams-python-1.0.5/clams/develop/
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-07-19 07:41:09.000000 clams-python-1.0.5/clams/develop/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:41:45.553348 clams-python-1.0.5/clams/develop/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:41:45.557348 clams-python-1.0.5/clams/develop/templates/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-19 07:41:09.000000 clams-python-1.0.5/clams/develop/templates/app/.dockerignore.template
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-19 07:41:09.000000 clams-python-1.0.5/clams/develop/templates/app/.gitignore.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-19 07:41:09.000000 clams-python-1.0.5/clams/develop/templates/app/Containerfile.template
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-19 07:41:09.000000 clams-python-1.0.5/clams/develop/templates/app/LICENSE.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-07-19 07:41:09.000000 clams-python-1.0.5/clams/develop/templates/app/README.md.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-19 07:41:09.000000 clams-python-1.0.5/clams/develop/templates/app/app.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-19 07:41:09.000000 clams-python-1.0.5/clams/develop/templates/app/metadata.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-19 07:41:09.000000 clams-python-1.0.5/clams/develop/templates/app/requirements.txt.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:41:45.557348 clams-python-1.0.5/clams/develop/templates/gha/
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-19 07:41:09.000000 clams-python-1.0.5/clams/develop/templates/gha/for-clams-team.md.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:41:45.557348 clams-python-1.0.5/clams/develop/templates/gha/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-19 07:41:09.000000 clams-python-1.0.5/clams/develop/templates/gha/workflows/issue-apps-project.yml.template
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-19 07:41:09.000000 clams-python-1.0.5/clams/develop/templates/gha/workflows/issue-assign.yml.template
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-19 07:41:09.000000 clams-python-1.0.5/clams/develop/templates/gha/workflows/issue-close.yml.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-19 07:41:09.000000 clams-python-1.0.5/clams/develop/templates/gha/workflows/publish.yml.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:41:45.557348 clams-python-1.0.5/clams/restify/
+-rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-07-19 07:41:09.000000 clams-python-1.0.5/clams/restify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:41:45.557348 clams-python-1.0.5/clams/serve/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-19 07:41:09.000000 clams-python-1.0.5/clams/serve/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:41:45.557348 clams-python-1.0.5/clams/source/
+-rw-r--r--   0 runner    (1001) docker     (123)    11761 2023-07-19 07:41:09.000000 clams-python-1.0.5/clams/source/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:41:45.561348 clams-python-1.0.5/clams/ver/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-19 07:41:45.000000 clams-python-1.0.5/clams/ver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:41:45.561348 clams-python-1.0.5/clams_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-19 07:41:45.000000 clams-python-1.0.5/clams_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-19 07:41:45.000000 clams-python-1.0.5/clams_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 07:41:45.000000 clams-python-1.0.5/clams_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-19 07:41:45.000000 clams-python-1.0.5/clams_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-19 07:41:45.000000 clams-python-1.0.5/clams_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-19 07:41:45.000000 clams-python-1.0.5/clams_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-19 07:41:09.000000 clams-python-1.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 07:41:45.561348 clams-python-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-07-19 07:41:09.000000 clams-python-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:41:45.561348 clams-python-1.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17330 2023-07-19 07:41:09.000000 clams-python-1.0.5/tests/test_clamsapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-07-19 07:41:09.000000 clams-python-1.0.5/tests/test_clamscli.py
```

### Comparing `clams-python-1.0.4/LICENSE` & `clams-python-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.4/PKG-INFO` & `clams-python-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clams-python
-Version: 1.0.4
+Version: 1.0.5
 Summary: A collection of APIs to develop CLAMS app for python
 Home-page: https://clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Flask
 Classifier: Framework :: Pytest
```

### Comparing `clams-python-1.0.4/README.md` & `clams-python-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.4/clams/__init__.py` & `clams-python-1.0.5/clams/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.4/clams/app/__init__.py` & `clams-python-1.0.5/clams/app/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.4/clams/appmetadata/__init__.py` & `clams-python-1.0.5/clams/appmetadata/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.4/clams/develop/__init__.py` & `clams-python-1.0.5/clams/develop/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.4/clams/develop/templates/app/.gitignore.template` & `clams-python-1.0.5/clams/develop/templates/app/.gitignore.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.4/clams/develop/templates/app/Containerfile.template` & `clams-python-1.0.5/clams/develop/templates/app/Containerfile.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.4/clams/develop/templates/app/README.md.template` & `clams-python-1.0.5/clams/develop/templates/app/README.md.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.4/clams/develop/templates/app/app.py.template` & `clams-python-1.0.5/clams/develop/templates/app/app.py.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.4/clams/develop/templates/app/metadata.py.template` & `clams-python-1.0.5/clams/develop/templates/app/metadata.py.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.4/clams/develop/templates/gha/for-clams-team.md.template` & `clams-python-1.0.5/clams/develop/templates/gha/for-clams-team.md.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.4/clams/develop/templates/gha/workflows/publish.yml.template` & `clams-python-1.0.5/clams/develop/templates/gha/workflows/publish.yml.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.4/clams/restify/__init__.py` & `clams-python-1.0.5/clams/restify/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.4/clams/source/__init__.py` & `clams-python-1.0.5/clams/source/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.4/clams_python.egg-info/PKG-INFO` & `clams-python-1.0.5/clams_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clams-python
-Version: 1.0.4
+Version: 1.0.5
 Summary: A collection of APIs to develop CLAMS app for python
 Home-page: https://clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Flask
 Classifier: Framework :: Pytest
```

### Comparing `clams-python-1.0.4/clams_python.egg-info/SOURCES.txt` & `clams-python-1.0.5/clams_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.4/setup.py` & `clams-python-1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.4/tests/test_clamsapp.py` & `clams-python-1.0.5/tests/test_clamsapp.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.4/tests/test_clamscli.py` & `clams-python-1.0.5/tests/test_clamscli.py`

 * *Files identical despite different names*

