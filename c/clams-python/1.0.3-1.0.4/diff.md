# Comparing `tmp/clams-python-1.0.3.tar.gz` & `tmp/clams-python-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clams-python-1.0.3.tar", last modified: Wed Jun 14 22:29:53 2023, max compression
+gzip compressed data, was "clams-python-1.0.4.tar", last modified: Wed Jul 19 05:31:23 2023, max compression
```

## Comparing `clams-python-1.0.3.tar` & `clams-python-1.0.4.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:29:53.870197 clams-python-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-06-14 22:29:22.000000 clams-python-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-14 22:29:22.000000 clams-python-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-14 22:29:53.870197 clams-python-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-14 22:29:22.000000 clams-python-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-14 22:29:23.000000 clams-python-1.0.3/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:29:53.866196 clams-python-1.0.3/clams/
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-14 22:29:22.000000 clams-python-1.0.3/clams/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:29:53.866196 clams-python-1.0.3/clams/app/
--rw-r--r--   0 runner    (1001) docker     (123)    11822 2023-06-14 22:29:22.000000 clams-python-1.0.3/clams/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:29:53.866196 clams-python-1.0.3/clams/appmetadata/
--rw-r--r--   0 runner    (1001) docker     (123)    16533 2023-06-14 22:29:22.000000 clams-python-1.0.3/clams/appmetadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:29:53.866196 clams-python-1.0.3/clams/develop/
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-06-14 22:29:22.000000 clams-python-1.0.3/clams/develop/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:29:53.862196 clams-python-1.0.3/clams/develop/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:29:53.866196 clams-python-1.0.3/clams/develop/templates/app/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-14 22:29:22.000000 clams-python-1.0.3/clams/develop/templates/app/.dockerignore.template
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-14 22:29:22.000000 clams-python-1.0.3/clams/develop/templates/app/.gitignore.template
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-14 22:29:22.000000 clams-python-1.0.3/clams/develop/templates/app/Containerfile.template
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-14 22:29:22.000000 clams-python-1.0.3/clams/develop/templates/app/LICENSE.template
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-06-14 22:29:22.000000 clams-python-1.0.3/clams/develop/templates/app/README.md.template
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-14 22:29:22.000000 clams-python-1.0.3/clams/develop/templates/app/app.py.template
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-06-14 22:29:22.000000 clams-python-1.0.3/clams/develop/templates/app/metadata.py.template
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-14 22:29:22.000000 clams-python-1.0.3/clams/develop/templates/app/requirements.txt.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:29:53.866196 clams-python-1.0.3/clams/develop/templates/gha/
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-06-14 22:29:22.000000 clams-python-1.0.3/clams/develop/templates/gha/README.md.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:29:53.866196 clams-python-1.0.3/clams/develop/templates/gha/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-14 22:29:22.000000 clams-python-1.0.3/clams/develop/templates/gha/workflows/issue-apps-project.yml.template
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-14 22:29:22.000000 clams-python-1.0.3/clams/develop/templates/gha/workflows/issue-assign.yml.template
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-14 22:29:22.000000 clams-python-1.0.3/clams/develop/templates/gha/workflows/issue-close.yml.template
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-14 22:29:22.000000 clams-python-1.0.3/clams/develop/templates/gha/workflows/publish.yml.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:29:53.866196 clams-python-1.0.3/clams/restify/
--rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-06-14 22:29:22.000000 clams-python-1.0.3/clams/restify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:29:53.866196 clams-python-1.0.3/clams/serve/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-14 22:29:22.000000 clams-python-1.0.3/clams/serve/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:29:53.866196 clams-python-1.0.3/clams/source/
--rw-r--r--   0 runner    (1001) docker     (123)     9939 2023-06-14 22:29:22.000000 clams-python-1.0.3/clams/source/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:29:53.866196 clams-python-1.0.3/clams/ver/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-14 22:29:53.000000 clams-python-1.0.3/clams/ver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:29:53.870197 clams-python-1.0.3/clams_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-14 22:29:53.000000 clams-python-1.0.3/clams_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-14 22:29:53.000000 clams-python-1.0.3/clams_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 22:29:53.000000 clams-python-1.0.3/clams_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-14 22:29:53.000000 clams-python-1.0.3/clams_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-14 22:29:53.000000 clams-python-1.0.3/clams_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-14 22:29:53.000000 clams-python-1.0.3/clams_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-14 22:29:22.000000 clams-python-1.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 22:29:53.870197 clams-python-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-14 22:29:22.000000 clams-python-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:29:53.870197 clams-python-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    17097 2023-06-14 22:29:22.000000 clams-python-1.0.3/tests/test_clamsapp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-14 22:29:22.000000 clams-python-1.0.3/tests/test_clamscli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:31:23.009792 clams-python-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-07-19 05:30:48.000000 clams-python-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-19 05:30:48.000000 clams-python-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-19 05:31:23.005792 clams-python-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-19 05:30:48.000000 clams-python-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-19 05:30:48.000000 clams-python-1.0.4/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:31:23.001792 clams-python-1.0.4/clams/
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-19 05:30:48.000000 clams-python-1.0.4/clams/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:31:23.001792 clams-python-1.0.4/clams/app/
+-rw-r--r--   0 runner    (1001) docker     (123)    12038 2023-07-19 05:30:48.000000 clams-python-1.0.4/clams/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:31:23.001792 clams-python-1.0.4/clams/appmetadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    16533 2023-07-19 05:30:48.000000 clams-python-1.0.4/clams/appmetadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:31:23.001792 clams-python-1.0.4/clams/develop/
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-07-19 05:30:48.000000 clams-python-1.0.4/clams/develop/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:31:22.997792 clams-python-1.0.4/clams/develop/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:31:23.001792 clams-python-1.0.4/clams/develop/templates/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-19 05:30:48.000000 clams-python-1.0.4/clams/develop/templates/app/.dockerignore.template
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-19 05:30:48.000000 clams-python-1.0.4/clams/develop/templates/app/.gitignore.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-19 05:30:48.000000 clams-python-1.0.4/clams/develop/templates/app/Containerfile.template
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-19 05:30:48.000000 clams-python-1.0.4/clams/develop/templates/app/LICENSE.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-07-19 05:30:48.000000 clams-python-1.0.4/clams/develop/templates/app/README.md.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-19 05:30:48.000000 clams-python-1.0.4/clams/develop/templates/app/app.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-19 05:30:48.000000 clams-python-1.0.4/clams/develop/templates/app/metadata.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-19 05:30:48.000000 clams-python-1.0.4/clams/develop/templates/app/requirements.txt.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:31:23.005792 clams-python-1.0.4/clams/develop/templates/gha/
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-19 05:30:48.000000 clams-python-1.0.4/clams/develop/templates/gha/for-clams-team.md.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:31:23.005792 clams-python-1.0.4/clams/develop/templates/gha/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-19 05:30:48.000000 clams-python-1.0.4/clams/develop/templates/gha/workflows/issue-apps-project.yml.template
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-19 05:30:48.000000 clams-python-1.0.4/clams/develop/templates/gha/workflows/issue-assign.yml.template
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-19 05:30:48.000000 clams-python-1.0.4/clams/develop/templates/gha/workflows/issue-close.yml.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-19 05:30:48.000000 clams-python-1.0.4/clams/develop/templates/gha/workflows/publish.yml.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:31:23.005792 clams-python-1.0.4/clams/restify/
+-rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-07-19 05:30:48.000000 clams-python-1.0.4/clams/restify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:31:23.005792 clams-python-1.0.4/clams/serve/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-19 05:30:48.000000 clams-python-1.0.4/clams/serve/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:31:23.005792 clams-python-1.0.4/clams/source/
+-rw-r--r--   0 runner    (1001) docker     (123)    11761 2023-07-19 05:30:48.000000 clams-python-1.0.4/clams/source/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:31:23.005792 clams-python-1.0.4/clams/ver/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-19 05:31:22.000000 clams-python-1.0.4/clams/ver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:31:23.005792 clams-python-1.0.4/clams_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-19 05:31:22.000000 clams-python-1.0.4/clams_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-19 05:31:22.000000 clams-python-1.0.4/clams_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 05:31:22.000000 clams-python-1.0.4/clams_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-19 05:31:22.000000 clams-python-1.0.4/clams_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-19 05:31:22.000000 clams-python-1.0.4/clams_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-19 05:31:22.000000 clams-python-1.0.4/clams_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-19 05:30:48.000000 clams-python-1.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 05:31:23.009792 clams-python-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-07-19 05:30:48.000000 clams-python-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:31:23.005792 clams-python-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17330 2023-07-19 05:30:48.000000 clams-python-1.0.4/tests/test_clamsapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-07-19 05:30:48.000000 clams-python-1.0.4/tests/test_clamscli.py
```

### Comparing `clams-python-1.0.3/LICENSE` & `clams-python-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.3/PKG-INFO` & `clams-python-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clams-python
-Version: 1.0.3
+Version: 1.0.4
 Summary: A collection of APIs to develop CLAMS app for python
 Home-page: https://clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Flask
 Classifier: Framework :: Pytest
```

### Comparing `clams-python-1.0.3/README.md` & `clams-python-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.3/clams/__init__.py` & `clams-python-1.0.4/clams/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.3/clams/app/__init__.py` & `clams-python-1.0.4/clams/app/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -145,14 +145,16 @@
         :param runtime_params: key-value pairs of runtime parameters
         :return: a copy of parameter map, with default values added
         :raises ValueError: when a value for a required parameter is not found in the input
         """
         conf = {}
         for parameter in self.metadata.parameters:
             if parameter.name in runtime_params:
+                if parameter.choices and runtime_params[parameter.name] not in parameter.choices:
+                    raise ValueError(f"Value for parameter \"{parameter.name}\" must be one of {parameter.choices}.")
                 conf[parameter.name] = runtime_params[parameter.name]
             elif parameter.default is not None:
                 conf[parameter.name] = parameter.default
             else:
                 raise ValueError(f"Cannot find configuration for a required parameter \"{parameter.name}\".")
         return conf
```

### Comparing `clams-python-1.0.3/clams/appmetadata/__init__.py` & `clams-python-1.0.4/clams/appmetadata/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.3/clams/develop/__init__.py` & `clams-python-1.0.4/clams/develop/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.3/clams/develop/templates/app/.gitignore.template` & `clams-python-1.0.4/clams/develop/templates/app/.gitignore.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.3/clams/develop/templates/app/Containerfile.template` & `clams-python-1.0.4/clams/develop/templates/app/Containerfile.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.3/clams/develop/templates/app/README.md.template` & `clams-python-1.0.4/clams/develop/templates/app/README.md.template`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 ---
 This skeleton code is a scaffolding for Python-based CLAMS app development. Specifically, it contains 
 
 1. `app.py` and `metadata.py` to write the app 
 1. `requirements.txt` to specify python dependencies
 1. `Containerfile` to containerize the app and specify system dependencies
-1. `.gitignore` and `.dorckrignore` files listing commonly ignored files
+1. `.gitignore` and `.dockerignore` files listing commonly ignored files
 1. an empty `LICENSE` file to replace with an actual license information of the app
 1. `CLAMS-generic-readme.md` file with basic instructions of app installation and execution
 1. This `README.md` file for additional information not specified in the generic readme file. 
 1. A number of GitHub Actions workflows for issue/bug-report management 
 1. A GHA workflow to publish app images upon any push of a git tag
    * **NOTE**: All GHA workflows included are designed to only work in repositories under `clamsproject` organization.
 
@@ -20,18 +20,18 @@
 
 Then use the following section to document any additional information specific to this app. If your app works significantly different from what's described in the generic readme file, be as specific as possible. 
 
 ---
 
 ## User instruction
 
-General user instruction for CLAMS apps is available at [CLAMS Apps documentation](https://apps.clams.ai/clamsapp/).
+General user instructions for CLAMS apps is available at [CLAMS Apps documentation](https://apps.clams.ai/clamsapp).
 
 Below is a list of additional information specific to this app.
 
 ### System requirments
 
 (Any system-level software required to run this app)
 
 ### Configurable runtime parameter
 
-(Parameters should be already well-described in the app metadata. But you can use this space to show examples, for instance.)
+(Parameters should be already well-described in the app metadata. But you can use this space to show examples, for instance.)
```

### Comparing `clams-python-1.0.3/clams/develop/templates/app/app.py.template` & `clams-python-1.0.4/clams/develop/templates/app/app.py.template`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,32 @@
+"""
+DELETE THIS MODULE STRING AND REPLACE IT WITH A DESCRIPTION OF YOUR APP.
+
+app.py Template
+
+The app.py script does several things:
+- import the necessary code
+- create a subclass of ClamsApp that defines the metadata and provides a method to run the wrapped NLP tool
+- provide a way to run the code as a RESTful Flask service 
+
+
+"""
+
 import argparse
 from typing import Union
 
-# mostly likely you'll need these modules/classes
+# Imports needed for Clams and MMIF.
+# Non-NLP Clams applications will require AnnotationTypes
+
 from clams import ClamsApp, Restifier
 from mmif import Mmif, View, Annotation, Document, AnnotationTypes, DocumentTypes
 
+# For an NLP tool we need to import the LAPPS vocabulary items
+from lapps.discriminators import Uri
+
 
 class $APP_CLASS_NAME(ClamsApp):
 
     def __init__(self):
         super().__init__()
 
     def _appmetadata(self):
@@ -24,21 +42,23 @@
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "--port", action="store", default="5000", help="set port to listen"
     )
     parser.add_argument("--production", action="store_true", help="run gunicorn server")
-    # more arguments as needed
+    # add more arguments as needed
     # parser.add_argument(more_arg...)
 
     parsed_args = parser.parse_args()
 
     # create the app instance
     app = $APP_CLASS_NAME()
 
     http_app = Restifier(app, port=int(parsed_args.port)
     )
+    # for running the application in production mode
     if parsed_args.production:
         http_app.serve_production()
+    # development mode
     else:
         http_app.run()
```

### Comparing `clams-python-1.0.3/clams/develop/templates/app/metadata.py.template` & `clams-python-1.0.4/clams/develop/templates/app/metadata.py.template`

 * *Files 14% similar despite different names*

```diff
@@ -23,24 +23,27 @@
     
     # first set up some basic information
     metadata = AppMetadata(
         name="$APP_NAME",
         description="",  # briefly describe what the purpose and features of the app
         app_license="",  # short name for a software license like MIT, Apache2, GPL, etc.
         identifier="$APP_IDENTIFIER",  # should be a single string without whitespaces. If you don't intent to publish this app to the CLAMS app-directory, please use a full IRI format. 
-        url="https://fakegithub.com/some/repository",  # a website where the source code and full documentation of the app is hosted, if you are on the CLAMS team, see ``.github/README.md`` file in this directory.
-        # use the following if this app is a wrapper of an existing computational analysis tool
+        url="https://fakegithub.com/some/repository",  # a website where the source code and full documentation of the app is hosted
+        # (if you are on the CLAMS team, this MUST be "https://github.com/clamsproject/app-$APP_IDENTIFIER"
+        # (see ``.github/README.md`` file in this directory for the reason)
+        analyzer_version='version_X', # use this IF THIS APP IS A WRAPPER of an existing computational analysis algorithm
         # (it is very important to pinpoint the primary analyzer version for reproducibility)
-        analyzer_version='version_X',
+        # (for example, when the app's implementation uses ``torch``, it doesn't make the app a "torch-wrapper")
+        # (but, when the app doesn't implementaion any additional algorithms/model/architecture, but simply use API's of existing, for exmaple, OCR software, it is a wrapper)
         # if the analyzer is a python app, and it's specified in the requirements.txt
         # this trick can also be useful (replace ANALYZER_NAME with the pypi dist name)
         analyzer_version=[l.strip().rsplit('==')[-1] for l in open('requirements.txt').readlines() if re.match(r'^ANALYZER_NAME==', l)][0],
         analyzer_license="",  # short name for a software license
     )
-    # and then add I/O specifications: an app must have at least one input and ont output
+    # and then add I/O specifications: an app must have at least one input and one output
     metadata.add_input(DocumentTypes.Document)
     metadata.add_output(AnnotationTypes.Thing, typeSpecificProperty='property-value')
     
     # (optional) and finally add runtime parameter specifications
     metadata.add_parameter(name='a_param', description='example parameter description',
                            type='boolean', default='false')
     # metadta.add_parameter(more...)
```

### Comparing `clams-python-1.0.3/clams/develop/templates/gha/README.md.template` & `clams-python-1.0.4/clams/develop/templates/gha/for-clams-team.md.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.3/clams/develop/templates/gha/workflows/publish.yml.template` & `clams-python-1.0.4/clams/develop/templates/gha/workflows/publish.yml.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.3/clams/restify/__init__.py` & `clams-python-1.0.4/clams/restify/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.3/clams/source/__init__.py` & `clams-python-1.0.4/clams/source/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import argparse
 import itertools
 import json
 import sys
 import textwrap
 from os import path
 from typing import Union, Generator, List, Optional, Iterable
+from urllib.parse import urlparse
 
 from mmif import Mmif, Document, DocumentTypes, __specver__
 from mmif.serialize.mmif import MmifMetadata
 
 __all__ = ['WorkflowSource']
 
 DOC_JSON = Union[str, dict]
@@ -166,15 +167,15 @@
         gets re-primed.
         """
         self.prime()
         while True:
             yield self.produce()
 
 
-def generate_source_mmif(documents, prefix=None, **ignored):
+def generate_source_mmif_from_file(documents, prefix=None, **ignored):
     from string import Template
     at_types = {
         'video': DocumentTypes.VideoDocument,
         'audio': DocumentTypes.AudioDocument,
         'text': DocumentTypes.TextDocument,
         'image': DocumentTypes.ImageDocument
     }
@@ -184,15 +185,14 @@
             "id": "${aid}",
             "mime": "${mime}",
             "location": "${location}" }
         }''')
     pl = WorkflowSource()
     if prefix and not path.isabs(prefix):
         raise ValueError(f"prefix must be an absolute path; given \"{prefix}\".")
-
     for doc_id, arg in enumerate(documents, start=1):
         arg = arg.strip()
         if len(arg) < 1:
             continue
         result = arg.split(':', maxsplit=1)
         if len(result) == 2 and result[0].split('/', maxsplit=1)[0] in at_types:
             mime, location = result
@@ -212,14 +212,53 @@
             mime=mime,
             location=location
         )
         pl.add_document(doc)
     return pl.produce().serialize(pretty=True)
 
 
+def generate_source_mmif_from_customscheme(documents, scheme, **ignored):
+    from string import Template
+    at_types = {
+        'video': DocumentTypes.VideoDocument,
+        'audio': DocumentTypes.AudioDocument,
+        'text': DocumentTypes.TextDocument,
+        'image': DocumentTypes.ImageDocument
+    }
+    template = Template('''{
+          "@type": "${at_type}",
+          "properties": {
+            "id": "${aid}",
+            "mime": "${mime}",
+            "location": "${location}" }
+        }''')
+    pl = WorkflowSource()
+    for doc_id, arg in enumerate(documents, start=1):
+        arg = arg.strip()
+        if len(arg) < 1:
+            continue
+        result = arg.split(':', maxsplit=1)
+        if len(result) == 2 and result[0].split('/', maxsplit=1)[0] in at_types:
+            mime, location = result
+        else:
+            raise ValueError(
+                f'Invalid MIME types, or no MIME type and/or path provided, in argument {doc_id-1} to source'
+            )
+        if urlparse(location).scheme == '':
+            location = scheme + '://' + location
+        doc = template.substitute(
+            at_type=str(at_types[mime.split('/', maxsplit=1)[0]]),
+            aid=f'd{doc_id}',
+            mime=mime,
+            location=location
+        )
+        pl.add_document(doc)
+    return pl.produce().serialize(pretty=True)
+
+
 def describe_argparser():
     """
     returns two strings: one-line description of the argparser, and addition material, 
     which will be shown in `clams --help` and `clams <subcmd> --help`, respectively.
     """
     oneliner = 'provides CLI to create a "source" MMIF json.'
     additional = textwrap.dedent("""
@@ -241,32 +280,44 @@
              "``@type`` and MIME type (if given), printed to the standard output. "
     )
     parser.add_argument(
         '-p', '--prefix',
         default=None,
         metavar='PATH',
         nargs='?',
-        help='An absolute path to use as prefix for document file paths. When prefix is set, document file paths MUST '
-             'be relative. This can be useful when creating source MMIF files from a system that\'s different from '
-             'the system that actually runs the workflow (e.g. in a container).'
+        help='An absolute path to use as prefix for file paths (ONLY WORKS with `file` scheme, ignored otherwise). If '
+             'prefix is set, document file paths MUST be relative. Useful when creating source MMIF files from a '
+             'system that\'s different from the system that actually runs the workflow (e.g. in a container).'
     )
     parser.add_argument(
         '-o', '--output',
         default=None,
         action='store',
         nargs='?',
         help='A name of a file to capture a generated MMIF json. When not given, MMIF is printed to stdout.'
     )
+    parser.add_argument(
+        '-s', '--scheme',
+        default='file',
+        action='store',
+        nargs='?',
+        help='A scheme to associate with the document location URI. When not given, the default scheme is `file`.'
+    )
     return parser
 
 
 def main(args):
     if args.output:
         out_f = open(args.output, 'w')
     else:
         out_f = sys.stdout
-    out_f.write(generate_source_mmif(**vars(args)))
+    if args.scheme == 'file':
+        mmif = generate_source_mmif_from_file(**vars(args))
+    else:
+        mmif = generate_source_mmif_from_customscheme(**vars(args))
+    out_f.write(mmif)
+    return mmif
 
 if __name__ == '__main__':
     parser = prep_argparser()
     args = parser.parse_args()
     main(args)
```

### Comparing `clams-python-1.0.3/clams_python.egg-info/PKG-INFO` & `clams-python-1.0.4/clams_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clams-python
-Version: 1.0.3
+Version: 1.0.4
 Summary: A collection of APIs to develop CLAMS app for python
 Home-page: https://clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Flask
 Classifier: Framework :: Pytest
```

### Comparing `clams-python-1.0.3/clams_python.egg-info/SOURCES.txt` & `clams-python-1.0.4/clams_python.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 clams/develop/templates/app/.gitignore.template
 clams/develop/templates/app/Containerfile.template
 clams/develop/templates/app/LICENSE.template
 clams/develop/templates/app/README.md.template
 clams/develop/templates/app/app.py.template
 clams/develop/templates/app/metadata.py.template
 clams/develop/templates/app/requirements.txt.template
-clams/develop/templates/gha/README.md.template
+clams/develop/templates/gha/for-clams-team.md.template
 clams/develop/templates/gha/workflows/issue-apps-project.yml.template
 clams/develop/templates/gha/workflows/issue-assign.yml.template
 clams/develop/templates/gha/workflows/issue-close.yml.template
 clams/develop/templates/gha/workflows/publish.yml.template
 clams/restify/__init__.py
 clams/serve/__init__.py
 clams/source/__init__.py
```

### Comparing `clams-python-1.0.3/setup.py` & `clams-python-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.3/tests/test_clamsapp.py` & `clams-python-1.0.4/tests/test_clamsapp.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,25 +220,28 @@
             self.assertEqual(f.size, (200, 71))
             
     def test_get_configuration(self):
         self.app.metadata.parameters = []
         self.app.metadata.add_parameter('param1', 'first_param', 'string')
         self.app.metadata.add_parameter('param2', 'second_param', 'string', default='second_default')
         self.app.metadata.add_parameter('param3', 'third_param', 'boolean', default='f')
-        self.app.metadata.add_parameter('param4', 'fourth_param', 'integer', default='1')
+        self.app.metadata.add_parameter('param4', 'fourth_param', 'integer', default='1', choices="1 2 3".split())
         conf = self.app.get_configuration(param1='okay', non_parameter='should be ignored')
         self.assertEqual(len(conf), 4)
         self.assertFalse('non_parameter' in conf)
         self.assertEqual(type(conf['param1']), str)
         self.assertEqual(type(conf['param2']), str)
         self.assertEqual(type(conf['param3']), bool)
         self.assertEqual(type(conf['param4']), int)
         with self.assertRaises(ValueError):
             # because param1 doesn't have a default value and thus a required param
             self.app.get_configuration(param2='okay')
+        with self.assertRaisesRegexp(ValueError, r'.+must be one of.+'):
+            # because param4 can't be 4, note that param1 is "required" 
+            self.app.get_configuration(param1='p1', param4=4)
             
     def test_error_handling(self):
         params = {'raise_error': True, 'pretty': True}
         in_mmif = Mmif(self.in_mmif)
         try: 
             out_mmif = self.app.annotate(in_mmif, **params)
         except Exception as e:
```

