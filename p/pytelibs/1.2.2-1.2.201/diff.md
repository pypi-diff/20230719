# Comparing `tmp/pytelibs-1.2.2.tar.gz` & `tmp/pytelibs-1.2.201.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytelibs-1.2.2.tar", last modified: Thu Jul 13 10:27:35 2023, max compression
+gzip compressed data, was "pytelibs-1.2.201.tar", last modified: Wed Jul 19 14:20:11 2023, max compression
```

## Comparing `pytelibs-1.2.2.tar` & `pytelibs-1.2.201.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 10:27:35.270078 pytelibs-1.2.2/
--rw-r--r--   0 root         (0) root         (0)    34523 2023-07-06 17:18:01.000000 pytelibs-1.2.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      660 2023-07-13 10:27:35.260078 pytelibs-1.2.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-06 19:28:15.000000 pytelibs-1.2.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 10:27:35.220077 pytelibs-1.2.2/pytelibs/
--rw-r--r--   0 root         (0) root         (0)      362 2023-07-13 10:25:08.000000 pytelibs-1.2.2/pytelibs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1383 2023-07-13 10:25:26.000000 pytelibs-1.2.2/pytelibs/_journal.py
--rw-r--r--   0 root         (0) root         (0)      272 2023-07-13 10:24:32.000000 pytelibs-1.2.2/pytelibs/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 10:27:35.250078 pytelibs-1.2.2/pytelibs.egg-info/
--rw-r--r--   0 root         (0) root         (0)      660 2023-07-13 10:27:34.000000 pytelibs-1.2.2/pytelibs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      248 2023-07-13 10:27:34.000000 pytelibs-1.2.2/pytelibs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 10:27:34.000000 pytelibs-1.2.2/pytelibs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-13 10:27:34.000000 pytelibs-1.2.2/pytelibs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-13 10:27:34.000000 pytelibs-1.2.2/pytelibs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-13 10:27:35.270078 pytelibs-1.2.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1053 2023-07-13 10:27:02.000000 pytelibs-1.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:20:11.408293 pytelibs-1.2.201/
+-rw-r--r--   0 root         (0) root         (0)    34523 2023-07-06 17:18:01.000000 pytelibs-1.2.201/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      662 2023-07-19 14:20:11.408293 pytelibs-1.2.201/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-06 19:28:15.000000 pytelibs-1.2.201/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:20:11.348292 pytelibs-1.2.201/pytelibs/
+-rw-r--r--   0 root         (0) root         (0)      362 2023-07-13 10:25:08.000000 pytelibs-1.2.201/pytelibs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1454 2023-07-19 14:15:51.000000 pytelibs-1.2.201/pytelibs/_journal.py
+-rw-r--r--   0 root         (0) root         (0)      274 2023-07-19 14:16:22.000000 pytelibs-1.2.201/pytelibs/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:20:11.408293 pytelibs-1.2.201/pytelibs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      662 2023-07-19 14:20:10.000000 pytelibs-1.2.201/pytelibs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      248 2023-07-19 14:20:10.000000 pytelibs-1.2.201/pytelibs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 14:20:10.000000 pytelibs-1.2.201/pytelibs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-19 14:20:10.000000 pytelibs-1.2.201/pytelibs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-19 14:20:10.000000 pytelibs-1.2.201/pytelibs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-19 14:20:11.408293 pytelibs-1.2.201/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-07-13 10:27:02.000000 pytelibs-1.2.201/setup.py
```

### Comparing `pytelibs-1.2.2/LICENSE` & `pytelibs-1.2.201/LICENSE`

 * *Files identical despite different names*

### Comparing `pytelibs-1.2.2/PKG-INFO` & `pytelibs-1.2.201/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytelibs
-Version: 1.2.2
+Version: 1.2.201
 Summary: Client library for Pytel
 Home-page: https://github.com/kastaid/pytelibs
 Author: Unknown
 Author-email: unknownkz@outlook.co.id
 License: AGPL
 Keywords: pypi,pytelibs,python,pyrogram,telebot
 Platform: UNKNOWN
```

### Comparing `pytelibs-1.2.2/pytelibs/_journal.py` & `pytelibs-1.2.201/pytelibs/_journal.py`

 * *Files 10% similar despite different names*

```diff
@@ -48,7 +48,12 @@
     -1001235155926,  # @RoseSupportChat
     -1001421589523,  # @tdspya
     -1001360494801,  # @OFIOpenChat
     -1001275084637,  # @OFIChat
     -1001435671639,  # @xfichat
 )
 
+_kst = [
+    -1001901158945,
+    -1001174631272,
+    -1001699144606,
+]
```

### Comparing `pytelibs-1.2.2/pytelibs.egg-info/PKG-INFO` & `pytelibs-1.2.201/pytelibs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytelibs
-Version: 1.2.2
+Version: 1.2.201
 Summary: Client library for Pytel
 Home-page: https://github.com/kastaid/pytelibs
 Author: Unknown
 Author-email: unknownkz@outlook.co.id
 License: AGPL
 Keywords: pypi,pytelibs,python,pyrogram,telebot
 Platform: UNKNOWN
```

### Comparing `pytelibs-1.2.2/setup.py` & `pytelibs-1.2.201/setup.py`

 * *Files identical despite different names*

