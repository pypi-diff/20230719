# Comparing `tmp/era_5g_interface-0.4.0.tar.gz` & `tmp/era_5g_interface-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "era_5g_interface-0.4.0.tar", last modified: Mon Jul 17 12:18:02 2023, max compression
+gzip compressed data, was "era_5g_interface-0.4.1.tar", last modified: Wed Jul 19 09:15:21 2023, max compression
```

## Comparing `era_5g_interface-0.4.0.tar` & `era_5g_interface-0.4.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 ikapinus  (1000) ikapinus  (1000)        0 2023-07-17 12:18:02.980758 era_5g_interface-0.4.0/
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)       12 2023-07-17 12:18:02.000000 era_5g_interface-0.4.0/MANIFEST.in
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)      427 2023-07-17 12:18:02.980758 era_5g_interface-0.4.0/PKG-INFO
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)      749 2023-07-17 12:18:02.000000 era_5g_interface-0.4.0/backend_shim.py
-drwxr-xr-x   0 ikapinus  (1000) ikapinus  (1000)        0 2023-07-17 12:18:02.980758 era_5g_interface-0.4.0/era_5g_interface/
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)        0 2023-07-17 12:18:02.000000 era_5g_interface-0.4.0/era_5g_interface/__init__.py
-drwxr-xr-x   0 ikapinus  (1000) ikapinus  (1000)        0 2023-07-17 12:18:02.980758 era_5g_interface-0.4.0/era_5g_interface/dataclasses/
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)        0 2023-07-17 12:18:02.000000 era_5g_interface-0.4.0/era_5g_interface/dataclasses/__init__.py
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)     1285 2023-07-17 12:18:02.000000 era_5g_interface-0.4.0/era_5g_interface/dataclasses/control_command.py
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)     1468 2023-07-17 12:18:02.000000 era_5g_interface-0.4.0/era_5g_interface/h264_decoder.py
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)     1699 2023-07-17 12:18:02.000000 era_5g_interface-0.4.0/era_5g_interface/h264_encoder.py
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)     4178 2023-07-17 12:18:02.000000 era_5g_interface-0.4.0/era_5g_interface/interface_helpers.py
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)        0 2023-07-17 12:18:02.000000 era_5g_interface-0.4.0/era_5g_interface/py.typed
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)     1470 2023-07-17 12:18:02.000000 era_5g_interface-0.4.0/era_5g_interface/task_handler.py
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)     2483 2023-07-17 12:18:02.000000 era_5g_interface-0.4.0/era_5g_interface/task_handler_internal_q.py
-drwxr-xr-x   0 ikapinus  (1000) ikapinus  (1000)        0 2023-07-17 12:18:02.980758 era_5g_interface-0.4.0/era_5g_interface/utils/
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)        0 2023-07-17 12:18:02.000000 era_5g_interface-0.4.0/era_5g_interface/utils/__init__.py
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)     5899 2023-07-17 12:18:02.000000 era_5g_interface-0.4.0/era_5g_interface/utils/rate_timer.py
-drwxr-xr-x   0 ikapinus  (1000) ikapinus  (1000)        0 2023-07-17 12:18:02.980758 era_5g_interface-0.4.0/era_5g_interface.egg-info/
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)      427 2023-07-17 12:18:02.000000 era_5g_interface-0.4.0/era_5g_interface.egg-info/PKG-INFO
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)      681 2023-07-17 12:18:02.000000 era_5g_interface-0.4.0/era_5g_interface.egg-info/SOURCES.txt
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)        1 2023-07-17 12:18:02.000000 era_5g_interface-0.4.0/era_5g_interface.egg-info/dependency_links.txt
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)        1 2023-07-17 12:18:02.000000 era_5g_interface-0.4.0/era_5g_interface.egg-info/namespace_packages.txt
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)       67 2023-07-17 12:18:02.000000 era_5g_interface-0.4.0/era_5g_interface.egg-info/requires.txt
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)       17 2023-07-17 12:18:02.000000 era_5g_interface-0.4.0/era_5g_interface.egg-info/top_level.txt
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)       38 2023-07-17 12:18:02.980758 era_5g_interface-0.4.0/setup.cfg
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)     1023 2023-07-17 12:18:02.000000 era_5g_interface-0.4.0/setup.py
+drwxr-xr-x   0 ikapinus  (1000) ikapinus  (1000)        0 2023-07-19 09:15:21.086159 era_5g_interface-0.4.1/
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)       12 2023-07-19 09:15:20.000000 era_5g_interface-0.4.1/MANIFEST.in
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)      421 2023-07-19 09:15:21.086159 era_5g_interface-0.4.1/PKG-INFO
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)      749 2023-07-19 09:15:20.000000 era_5g_interface-0.4.1/backend_shim.py
+drwxr-xr-x   0 ikapinus  (1000) ikapinus  (1000)        0 2023-07-19 09:15:21.086159 era_5g_interface-0.4.1/era_5g_interface/
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)        0 2023-07-19 09:15:20.000000 era_5g_interface-0.4.1/era_5g_interface/__init__.py
+drwxr-xr-x   0 ikapinus  (1000) ikapinus  (1000)        0 2023-07-19 09:15:21.086159 era_5g_interface-0.4.1/era_5g_interface/dataclasses/
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)        0 2023-07-19 09:15:20.000000 era_5g_interface-0.4.1/era_5g_interface/dataclasses/__init__.py
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)     1285 2023-07-19 09:15:20.000000 era_5g_interface-0.4.1/era_5g_interface/dataclasses/control_command.py
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)     1468 2023-07-19 09:15:20.000000 era_5g_interface-0.4.1/era_5g_interface/h264_decoder.py
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)     1699 2023-07-19 09:15:20.000000 era_5g_interface-0.4.1/era_5g_interface/h264_encoder.py
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)     4178 2023-07-19 09:15:20.000000 era_5g_interface-0.4.1/era_5g_interface/interface_helpers.py
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)        0 2023-07-19 09:15:20.000000 era_5g_interface-0.4.1/era_5g_interface/py.typed
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)     1470 2023-07-19 09:15:20.000000 era_5g_interface-0.4.1/era_5g_interface/task_handler.py
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)     2483 2023-07-19 09:15:20.000000 era_5g_interface-0.4.1/era_5g_interface/task_handler_internal_q.py
+drwxr-xr-x   0 ikapinus  (1000) ikapinus  (1000)        0 2023-07-19 09:15:21.086159 era_5g_interface-0.4.1/era_5g_interface/utils/
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)        0 2023-07-19 09:15:20.000000 era_5g_interface-0.4.1/era_5g_interface/utils/__init__.py
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)     5899 2023-07-19 09:15:20.000000 era_5g_interface-0.4.1/era_5g_interface/utils/rate_timer.py
+drwxr-xr-x   0 ikapinus  (1000) ikapinus  (1000)        0 2023-07-19 09:15:21.086159 era_5g_interface-0.4.1/era_5g_interface.egg-info/
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)      421 2023-07-19 09:15:21.000000 era_5g_interface-0.4.1/era_5g_interface.egg-info/PKG-INFO
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)      681 2023-07-19 09:15:21.000000 era_5g_interface-0.4.1/era_5g_interface.egg-info/SOURCES.txt
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)        1 2023-07-19 09:15:21.000000 era_5g_interface-0.4.1/era_5g_interface.egg-info/dependency_links.txt
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)        1 2023-07-19 09:15:21.000000 era_5g_interface-0.4.1/era_5g_interface.egg-info/namespace_packages.txt
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)       67 2023-07-19 09:15:21.000000 era_5g_interface-0.4.1/era_5g_interface.egg-info/requires.txt
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)       17 2023-07-19 09:15:21.000000 era_5g_interface-0.4.1/era_5g_interface.egg-info/top_level.txt
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)       38 2023-07-19 09:15:21.086159 era_5g_interface-0.4.1/setup.cfg
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)     1017 2023-07-19 09:15:20.000000 era_5g_interface-0.4.1/setup.py
```

### Comparing `era_5g_interface-0.4.0/backend_shim.py` & `era_5g_interface-0.4.1/backend_shim.py`

 * *Files identical despite different names*

### Comparing `era_5g_interface-0.4.0/era_5g_interface/dataclasses/control_command.py` & `era_5g_interface-0.4.1/era_5g_interface/dataclasses/control_command.py`

 * *Files identical despite different names*

### Comparing `era_5g_interface-0.4.0/era_5g_interface/h264_decoder.py` & `era_5g_interface-0.4.1/era_5g_interface/h264_decoder.py`

 * *Files identical despite different names*

### Comparing `era_5g_interface-0.4.0/era_5g_interface/h264_encoder.py` & `era_5g_interface-0.4.1/era_5g_interface/h264_encoder.py`

 * *Files identical despite different names*

### Comparing `era_5g_interface-0.4.0/era_5g_interface/interface_helpers.py` & `era_5g_interface-0.4.1/era_5g_interface/interface_helpers.py`

 * *Files identical despite different names*

### Comparing `era_5g_interface-0.4.0/era_5g_interface/task_handler.py` & `era_5g_interface-0.4.1/era_5g_interface/task_handler.py`

 * *Files identical despite different names*

### Comparing `era_5g_interface-0.4.0/era_5g_interface/task_handler_internal_q.py` & `era_5g_interface-0.4.1/era_5g_interface/task_handler_internal_q.py`

 * *Files identical despite different names*

### Comparing `era_5g_interface-0.4.0/era_5g_interface/utils/rate_timer.py` & `era_5g_interface-0.4.1/era_5g_interface/utils/rate_timer.py`

 * *Files identical despite different names*

### Comparing `era_5g_interface-0.4.0/era_5g_interface.egg-info/SOURCES.txt` & `era_5g_interface-0.4.1/era_5g_interface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `era_5g_interface-0.4.0/setup.py` & `era_5g_interface-0.4.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,10 +30,10 @@
         ),
     },
     'packages': (
         'era_5g_interface',
         'era_5g_interface.dataclasses',
         'era_5g_interface.utils',
     ),
-    'python_requires': '>=3.8,<3.11',
-    'version': '0.4.0',
+    'python_requires': '>=3.8',
+    'version': '0.4.1',
 })
```

