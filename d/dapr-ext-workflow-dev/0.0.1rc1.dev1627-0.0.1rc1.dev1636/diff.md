# Comparing `tmp/dapr-ext-workflow-dev-0.0.1rc1.dev1627.tar.gz` & `tmp/dapr-ext-workflow-dev-0.0.1rc1.dev1636.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dapr-ext-workflow-dev-0.0.1rc1.dev1627.tar", last modified: Fri Jul 14 18:52:10 2023, max compression
+gzip compressed data, was "dist/dapr-ext-workflow-dev-0.0.1rc1.dev1636.tar", last modified: Tue Jul 18 22:44:55 2023, max compression
```

## Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1627.tar` & `dapr-ext-workflow-dev-0.0.1rc1.dev1636.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:52:10.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1627/
--rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-07-14 18:51:50.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1627/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-14 18:52:10.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1627/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-14 18:51:50.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1627/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:52:10.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1627/dapr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:52:10.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1627/dapr/ext/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:52:10.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1627/dapr/ext/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-14 18:51:50.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1627/dapr/ext/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10443 2023-07-14 18:51:50.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1627/dapr/ext/workflow/dapr_workflow_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-07-14 18:51:50.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1627/dapr/ext/workflow/dapr_workflow_context.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-14 18:51:50.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1627/dapr/ext/workflow/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-14 18:51:50.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1627/dapr/ext/workflow/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-14 18:51:50.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1627/dapr/ext/workflow/workflow_activity_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-07-14 18:51:50.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1627/dapr/ext/workflow/workflow_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-14 18:51:50.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1627/dapr/ext/workflow/workflow_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-14 18:51:50.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1627/dapr/ext/workflow/workflow_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:52:10.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1627/dapr_ext_workflow_dev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-14 18:52:10.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1627/dapr_ext_workflow_dev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-14 18:52:10.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1627/dapr_ext_workflow_dev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 18:52:10.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1627/dapr_ext_workflow_dev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-14 18:52:10.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1627/dapr_ext_workflow_dev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-14 18:52:10.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1627/dapr_ext_workflow_dev.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-14 18:52:10.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1627/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-14 18:51:50.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1627/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:44:55.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1636/
+-rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-07-18 22:44:37.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1636/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-18 22:44:55.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1636/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-18 22:44:37.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1636/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:44:55.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1636/dapr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:44:55.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1636/dapr/ext/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:44:55.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1636/dapr/ext/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-18 22:44:37.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1636/dapr/ext/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10443 2023-07-18 22:44:37.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1636/dapr/ext/workflow/dapr_workflow_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-07-18 22:44:37.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1636/dapr/ext/workflow/dapr_workflow_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-18 22:44:37.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1636/dapr/ext/workflow/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-18 22:44:37.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1636/dapr/ext/workflow/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-18 22:44:37.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1636/dapr/ext/workflow/workflow_activity_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-07-18 22:44:37.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1636/dapr/ext/workflow/workflow_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-18 22:44:37.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1636/dapr/ext/workflow/workflow_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-18 22:44:37.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1636/dapr/ext/workflow/workflow_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:44:55.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1636/dapr_ext_workflow_dev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-18 22:44:55.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1636/dapr_ext_workflow_dev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-18 22:44:55.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1636/dapr_ext_workflow_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 22:44:55.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1636/dapr_ext_workflow_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-18 22:44:55.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1636/dapr_ext_workflow_dev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-18 22:44:55.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1636/dapr_ext_workflow_dev.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-18 22:44:55.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1636/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-18 22:44:37.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1636/setup.py
```

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1627/LICENSE` & `dapr-ext-workflow-dev-0.0.1rc1.dev1636/LICENSE`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1627/PKG-INFO` & `dapr-ext-workflow-dev-0.0.1rc1.dev1636/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: dapr-ext-workflow-dev
-Version: 0.0.1rc1.dev1627
+Version: 0.0.1rc1.dev1636
 Summary: The developmental release for Dapr Workflow Authoring.
 Home-page: https://dapr.io/
 Author: Dapr Authors
 Author-email: daprweb@microsoft.com
 License: Apache
 Project-URL: Documentation, https://github.com/dapr/docs
 Project-URL: Source, https://github.com/dapr/python-sdk
```

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1627/dapr/ext/workflow/__init__.py` & `dapr-ext-workflow-dev-0.0.1rc1.dev1636/dapr/ext/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1627/dapr/ext/workflow/dapr_workflow_client.py` & `dapr-ext-workflow-dev-0.0.1rc1.dev1636/dapr/ext/workflow/dapr_workflow_client.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1627/dapr/ext/workflow/dapr_workflow_context.py` & `dapr-ext-workflow-dev-0.0.1rc1.dev1636/dapr/ext/workflow/dapr_workflow_context.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1627/dapr/ext/workflow/util.py` & `dapr-ext-workflow-dev-0.0.1rc1.dev1636/dapr/ext/workflow/util.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1627/dapr/ext/workflow/version.py` & `dapr-ext-workflow-dev-0.0.1rc1.dev1636/dapr/ext/workflow/version.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1627/dapr/ext/workflow/workflow_activity_context.py` & `dapr-ext-workflow-dev-0.0.1rc1.dev1636/dapr/ext/workflow/workflow_activity_context.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1627/dapr/ext/workflow/workflow_context.py` & `dapr-ext-workflow-dev-0.0.1rc1.dev1636/dapr/ext/workflow/workflow_context.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1627/dapr/ext/workflow/workflow_runtime.py` & `dapr-ext-workflow-dev-0.0.1rc1.dev1636/dapr/ext/workflow/workflow_runtime.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1627/dapr/ext/workflow/workflow_state.py` & `dapr-ext-workflow-dev-0.0.1rc1.dev1636/dapr/ext/workflow/workflow_state.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1627/dapr_ext_workflow_dev.egg-info/PKG-INFO` & `dapr-ext-workflow-dev-0.0.1rc1.dev1636/dapr_ext_workflow_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: dapr-ext-workflow-dev
-Version: 0.0.1rc1.dev1627
+Version: 0.0.1rc1.dev1636
 Summary: The developmental release for Dapr Workflow Authoring.
 Home-page: https://dapr.io/
 Author: Dapr Authors
 Author-email: daprweb@microsoft.com
 License: Apache
 Project-URL: Documentation, https://github.com/dapr/docs
 Project-URL: Source, https://github.com/dapr/python-sdk
```

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1627/dapr_ext_workflow_dev.egg-info/SOURCES.txt` & `dapr-ext-workflow-dev-0.0.1rc1.dev1636/dapr_ext_workflow_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1627/setup.cfg` & `dapr-ext-workflow-dev-0.0.1rc1.dev1636/setup.cfg`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1627/setup.py` & `dapr-ext-workflow-dev-0.0.1rc1.dev1636/setup.py`

 * *Files identical despite different names*

