# Comparing `tmp/eef-data-0.49.tar.gz` & `tmp/eef-data-0.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eef-data-0.49.tar", last modified: Tue Jul 18 23:39:30 2023, max compression
+gzip compressed data, was "eef-data-0.50.tar", last modified: Tue Jul 18 23:42:10 2023, max compression
```

## Comparing `eef-data-0.49.tar` & `eef-data-0.50.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-18 23:39:30.069791 eef-data-0.49/
--rw-rw-r--   0 linux     (1000) linux     (1000)     1073 2023-05-04 23:15:45.000000 eef-data-0.49/LICENSE
--rw-rw-r--   0 linux     (1000) linux     (1000)      299 2023-07-18 23:39:30.069791 eef-data-0.49/PKG-INFO
--rw-rw-r--   0 linux     (1000) linux     (1000)    64622 2023-07-18 23:21:55.000000 eef-data-0.49/README.md
-drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-18 23:39:30.065791 eef-data-0.49/eef_data.egg-info/
--rw-rw-r--   0 linux     (1000) linux     (1000)      299 2023-07-18 23:39:30.000000 eef-data-0.49/eef_data.egg-info/PKG-INFO
--rw-rw-r--   0 linux     (1000) linux     (1000)      328 2023-07-18 23:39:30.000000 eef-data-0.49/eef_data.egg-info/SOURCES.txt
--rw-rw-r--   0 linux     (1000) linux     (1000)        1 2023-07-18 23:39:30.000000 eef-data-0.49/eef_data.egg-info/dependency_links.txt
--rw-rw-r--   0 linux     (1000) linux     (1000)       47 2023-07-18 23:39:30.000000 eef-data-0.49/eef_data.egg-info/entry_points.txt
--rw-rw-r--   0 linux     (1000) linux     (1000)       78 2023-07-18 23:39:30.000000 eef-data-0.49/eef_data.egg-info/requires.txt
--rw-rw-r--   0 linux     (1000) linux     (1000)        8 2023-07-18 23:39:30.000000 eef-data-0.49/eef_data.egg-info/top_level.txt
-drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-18 23:39:30.065791 eef-data-0.49/eefdata/
--rw-rw-r--   0 linux     (1000) linux     (1000)        0 2023-03-17 12:41:41.000000 eef-data-0.49/eefdata/__init__.py
--rw-rw-r--   0 linux     (1000) linux     (1000)   165254 2023-07-18 23:16:25.000000 eef-data-0.49/eefdata/app.py
-drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-18 23:39:30.065791 eef-data-0.49/eefdata/src/
--rw-rw-r--   0 linux     (1000) linux     (1000)        0 2023-03-17 12:41:42.000000 eef-data-0.49/eefdata/src/__init__.py
--rw-rw-r--   0 linux     (1000) linux     (1000)   151479 2023-07-18 18:50:53.000000 eef-data-0.49/eefdata/src/attributeIDs.py
--rw-rw-r--   0 linux     (1000) linux     (1000)   263004 2023-07-18 23:21:18.000000 eef-data-0.49/eefdata/src/funcs.py
--rw-rw-r--   0 linux     (1000) linux     (1000)       38 2023-07-18 23:39:30.069791 eef-data-0.49/setup.cfg
--rw-rw-r--   0 linux     (1000) linux     (1000)      790 2023-07-18 23:36:15.000000 eef-data-0.49/setup.py
+drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-18 23:42:10.863881 eef-data-0.50/
+-rw-rw-r--   0 linux     (1000) linux     (1000)     1073 2023-05-04 23:15:45.000000 eef-data-0.50/LICENSE
+-rw-rw-r--   0 linux     (1000) linux     (1000)    62814 2023-07-18 23:42:10.863881 eef-data-0.50/PKG-INFO
+-rw-rw-r--   0 linux     (1000) linux     (1000)    64622 2023-07-18 23:21:55.000000 eef-data-0.50/README.md
+drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-18 23:42:10.863881 eef-data-0.50/eef_data.egg-info/
+-rw-rw-r--   0 linux     (1000) linux     (1000)    62814 2023-07-18 23:42:10.000000 eef-data-0.50/eef_data.egg-info/PKG-INFO
+-rw-rw-r--   0 linux     (1000) linux     (1000)      328 2023-07-18 23:42:10.000000 eef-data-0.50/eef_data.egg-info/SOURCES.txt
+-rw-rw-r--   0 linux     (1000) linux     (1000)        1 2023-07-18 23:42:10.000000 eef-data-0.50/eef_data.egg-info/dependency_links.txt
+-rw-rw-r--   0 linux     (1000) linux     (1000)       47 2023-07-18 23:42:10.000000 eef-data-0.50/eef_data.egg-info/entry_points.txt
+-rw-rw-r--   0 linux     (1000) linux     (1000)       78 2023-07-18 23:42:10.000000 eef-data-0.50/eef_data.egg-info/requires.txt
+-rw-rw-r--   0 linux     (1000) linux     (1000)        8 2023-07-18 23:42:10.000000 eef-data-0.50/eef_data.egg-info/top_level.txt
+drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-18 23:42:10.863881 eef-data-0.50/eefdata/
+-rw-rw-r--   0 linux     (1000) linux     (1000)        0 2023-03-17 12:41:41.000000 eef-data-0.50/eefdata/__init__.py
+-rw-rw-r--   0 linux     (1000) linux     (1000)   165254 2023-07-18 23:16:25.000000 eef-data-0.50/eefdata/app.py
+drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-18 23:42:10.863881 eef-data-0.50/eefdata/src/
+-rw-rw-r--   0 linux     (1000) linux     (1000)        0 2023-03-17 12:41:42.000000 eef-data-0.50/eefdata/src/__init__.py
+-rw-rw-r--   0 linux     (1000) linux     (1000)   151479 2023-07-18 18:50:53.000000 eef-data-0.50/eefdata/src/attributeIDs.py
+-rw-rw-r--   0 linux     (1000) linux     (1000)   263004 2023-07-18 23:21:18.000000 eef-data-0.50/eefdata/src/funcs.py
+-rw-rw-r--   0 linux     (1000) linux     (1000)       38 2023-07-18 23:42:10.863881 eef-data-0.50/setup.cfg
+-rw-rw-r--   0 linux     (1000) linux     (1000)      693 2023-07-18 23:40:53.000000 eef-data-0.50/setup.py
```

### Comparing `eef-data-0.49/LICENSE` & `eef-data-0.50/LICENSE`

 * *Files identical despite different names*

### Comparing `eef-data-0.49/README.md` & `eef-data-0.50/README.md`

 * *Files identical despite different names*

### Comparing `eef-data-0.49/eefdata/app.py` & `eef-data-0.50/eefdata/app.py`

 * *Files identical despite different names*

### Comparing `eef-data-0.49/eefdata/src/attributeIDs.py` & `eef-data-0.50/eefdata/src/attributeIDs.py`

 * *Files identical despite different names*

### Comparing `eef-data-0.49/eefdata/src/funcs.py` & `eef-data-0.50/eefdata/src/funcs.py`

 * *Files identical despite different names*

