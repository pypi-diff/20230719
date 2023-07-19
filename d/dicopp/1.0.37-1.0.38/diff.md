# Comparing `tmp/dicopp-1.0.37.tar.gz` & `tmp/dicopp-1.0.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicopp-1.0.37.tar", last modified: Sat Jul 15 08:32:10 2023, max compression
+gzip compressed data, was "dicopp-1.0.38.tar", last modified: Wed Jul 19 10:36:42 2023, max compression
```

## Comparing `dicopp-1.0.37.tar` & `dicopp-1.0.38.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 bc        (1000) bc        (1000)        0 2023-07-15 08:32:10.838813 dicopp-1.0.37/
--rw-rw-r--   0 bc        (1000) bc        (1000)       30 2023-05-12 11:46:51.000000 dicopp-1.0.37/MANIFEST.in
--rw-rw-r--   0 bc        (1000) bc        (1000)      387 2023-07-15 08:32:10.838813 dicopp-1.0.37/PKG-INFO
--rw-rw-r--   0 bc        (1000) bc        (1000)      894 2023-03-23 11:57:18.000000 dicopp-1.0.37/README.md
-drwxrwxr-x   0 bc        (1000) bc        (1000)        0 2023-07-15 08:32:10.834813 dicopp-1.0.37/dicopp/
--rw-rw-r--   0 bc        (1000) bc        (1000)     1252 2023-07-15 06:20:45.000000 dicopp-1.0.37/dicopp/base.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     1909 2022-01-31 07:04:25.000000 dicopp-1.0.37/dicopp/com.py
--rw-rw-r--   0 bc        (1000) bc        (1000)      359 2022-01-31 07:04:25.000000 dicopp-1.0.37/dicopp/con.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     1468 2022-07-07 04:32:27.000000 dicopp-1.0.37/dicopp/daem.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     1553 2022-01-31 07:04:25.000000 dicopp-1.0.37/dicopp/details.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     2640 2022-01-31 07:04:25.000000 dicopp-1.0.37/dicopp/dload.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     1429 2022-01-31 07:04:25.000000 dicopp-1.0.37/dicopp/extension.py
--rw-rw-r--   0 bc        (1000) bc        (1000)      688 2022-01-31 07:04:25.000000 dicopp-1.0.37/dicopp/first.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     1976 2022-01-31 07:04:25.000000 dicopp-1.0.37/dicopp/flist.py
--rw-rw-r--   0 bc        (1000) bc        (1000)    32953 2023-07-15 06:02:55.000000 dicopp-1.0.37/dicopp/hublist.xml.gz
--rw-rw-r--   0 bc        (1000) bc        (1000)     4579 2023-07-15 06:20:45.000000 dicopp-1.0.37/dicopp/hubs.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     1195 2022-01-31 07:04:25.000000 dicopp-1.0.37/dicopp/hubscon.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     1519 2022-01-31 07:04:25.000000 dicopp-1.0.37/dicopp/hubson.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     1436 2022-05-05 03:24:34.000000 dicopp-1.0.37/dicopp/layout.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     1323 2022-01-31 07:04:25.000000 dicopp-1.0.37/dicopp/limit.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     1028 2022-01-31 07:04:25.000000 dicopp-1.0.37/dicopp/log.py
--rw-rw-r--   0 bc        (1000) bc        (1000)      994 2022-05-07 04:49:33.000000 dicopp-1.0.37/dicopp/main.py
--rw-rw-r--   0 bc        (1000) bc        (1000)      895 2022-01-31 07:04:25.000000 dicopp-1.0.37/dicopp/nick.py
--rw-rw-r--   0 bc        (1000) bc        (1000)      205 2022-01-31 07:04:25.000000 dicopp-1.0.37/dicopp/overrides.py
--rw-rw-r--   0 bc        (1000) bc        (1000)      980 2022-01-31 07:04:25.000000 dicopp-1.0.37/dicopp/reqs.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     4641 2022-01-31 07:04:25.000000 dicopp-1.0.37/dicopp/search.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     1374 2022-01-31 07:04:25.000000 dicopp-1.0.37/dicopp/sets.py
--rw-rw-r--   0 bc        (1000) bc        (1000)      612 2022-01-31 07:04:25.000000 dicopp-1.0.37/dicopp/share.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     1503 2022-01-31 07:04:25.000000 dicopp-1.0.37/dicopp/stor2.py
--rw-rw-r--   0 bc        (1000) bc        (1000)      661 2022-01-31 07:04:25.000000 dicopp-1.0.37/dicopp/userinfo.py
--rw-rw-r--   0 bc        (1000) bc        (1000)     1514 2022-01-31 07:04:25.000000 dicopp-1.0.37/dicopp/users.py
--rw-rw-r--   0 bc        (1000) bc        (1000)      540 2022-01-31 07:04:25.000000 dicopp-1.0.37/dicopp/usersloc.py
-drwxrwxr-x   0 bc        (1000) bc        (1000)        0 2023-07-15 08:32:10.838813 dicopp-1.0.37/dicopp.egg-info/
--rw-rw-r--   0 bc        (1000) bc        (1000)      387 2023-07-15 08:32:10.000000 dicopp-1.0.37/dicopp.egg-info/PKG-INFO
--rw-rw-r--   0 bc        (1000) bc        (1000)      658 2023-07-15 08:32:10.000000 dicopp-1.0.37/dicopp.egg-info/SOURCES.txt
--rw-rw-r--   0 bc        (1000) bc        (1000)        1 2023-07-15 08:32:10.000000 dicopp-1.0.37/dicopp.egg-info/dependency_links.txt
--rw-rw-r--   0 bc        (1000) bc        (1000)       44 2023-07-15 08:32:10.000000 dicopp-1.0.37/dicopp.egg-info/entry_points.txt
--rw-rw-r--   0 bc        (1000) bc        (1000)       60 2023-07-15 08:32:10.000000 dicopp-1.0.37/dicopp.egg-info/requires.txt
--rw-rw-r--   0 bc        (1000) bc        (1000)        7 2023-07-15 08:32:10.000000 dicopp-1.0.37/dicopp.egg-info/top_level.txt
--rw-rw-r--   0 bc        (1000) bc        (1000)       38 2023-07-15 08:32:10.838813 dicopp-1.0.37/setup.cfg
--rw-rw-r--   0 bc        (1000) bc        (1000)      945 2023-07-15 06:20:45.000000 dicopp-1.0.37/setup.py
+drwxrwxr-x   0 bc        (1000) bc        (1000)        0 2023-07-19 10:36:42.260252 dicopp-1.0.38/
+-rw-rw-r--   0 bc        (1000) bc        (1000)       30 2023-05-12 11:46:51.000000 dicopp-1.0.38/MANIFEST.in
+-rw-rw-r--   0 bc        (1000) bc        (1000)      450 2023-07-19 10:36:42.260252 dicopp-1.0.38/PKG-INFO
+-rw-rw-r--   0 bc        (1000) bc        (1000)      894 2023-03-23 11:57:18.000000 dicopp-1.0.38/README.md
+drwxrwxr-x   0 bc        (1000) bc        (1000)        0 2023-07-19 10:36:42.252251 dicopp-1.0.38/dicopp/
+-rw-rw-r--   0 bc        (1000) bc        (1000)     1252 2023-07-15 06:20:45.000000 dicopp-1.0.38/dicopp/base.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     1909 2022-01-31 07:04:25.000000 dicopp-1.0.38/dicopp/com.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)      359 2022-01-31 07:04:25.000000 dicopp-1.0.38/dicopp/con.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     1468 2022-07-07 04:32:27.000000 dicopp-1.0.38/dicopp/daem.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     1553 2022-01-31 07:04:25.000000 dicopp-1.0.38/dicopp/details.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     2640 2022-01-31 07:04:25.000000 dicopp-1.0.38/dicopp/dload.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     1429 2022-01-31 07:04:25.000000 dicopp-1.0.38/dicopp/extension.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)      688 2022-01-31 07:04:25.000000 dicopp-1.0.38/dicopp/first.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     1976 2022-01-31 07:04:25.000000 dicopp-1.0.38/dicopp/flist.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)    32746 2023-07-19 05:51:22.000000 dicopp-1.0.38/dicopp/hublist.xml.gz
+-rw-rw-r--   0 bc        (1000) bc        (1000)     4579 2023-07-15 06:20:45.000000 dicopp-1.0.38/dicopp/hubs.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     1195 2022-01-31 07:04:25.000000 dicopp-1.0.38/dicopp/hubscon.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     1519 2022-01-31 07:04:25.000000 dicopp-1.0.38/dicopp/hubson.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     1436 2022-05-05 03:24:34.000000 dicopp-1.0.38/dicopp/layout.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     1323 2022-01-31 07:04:25.000000 dicopp-1.0.38/dicopp/limit.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     1028 2022-01-31 07:04:25.000000 dicopp-1.0.38/dicopp/log.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     1673 2023-07-19 06:08:25.000000 dicopp-1.0.38/dicopp/main.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)      895 2022-01-31 07:04:25.000000 dicopp-1.0.38/dicopp/nick.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)      205 2022-01-31 07:04:25.000000 dicopp-1.0.38/dicopp/overrides.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)      980 2022-01-31 07:04:25.000000 dicopp-1.0.38/dicopp/reqs.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     4641 2022-01-31 07:04:25.000000 dicopp-1.0.38/dicopp/search.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     1374 2022-01-31 07:04:25.000000 dicopp-1.0.38/dicopp/sets.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)      612 2022-01-31 07:04:25.000000 dicopp-1.0.38/dicopp/share.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     1503 2022-01-31 07:04:25.000000 dicopp-1.0.38/dicopp/stor2.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)      661 2022-01-31 07:04:25.000000 dicopp-1.0.38/dicopp/userinfo.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)     1514 2022-01-31 07:04:25.000000 dicopp-1.0.38/dicopp/users.py
+-rw-rw-r--   0 bc        (1000) bc        (1000)      540 2022-01-31 07:04:25.000000 dicopp-1.0.38/dicopp/usersloc.py
+drwxrwxr-x   0 bc        (1000) bc        (1000)        0 2023-07-19 10:36:42.256251 dicopp-1.0.38/dicopp.egg-info/
+-rw-rw-r--   0 bc        (1000) bc        (1000)      450 2023-07-19 10:36:42.000000 dicopp-1.0.38/dicopp.egg-info/PKG-INFO
+-rw-rw-r--   0 bc        (1000) bc        (1000)      658 2023-07-19 10:36:42.000000 dicopp-1.0.38/dicopp.egg-info/SOURCES.txt
+-rw-rw-r--   0 bc        (1000) bc        (1000)        1 2023-07-19 10:36:42.000000 dicopp-1.0.38/dicopp.egg-info/dependency_links.txt
+-rw-rw-r--   0 bc        (1000) bc        (1000)       44 2023-07-19 10:36:42.000000 dicopp-1.0.38/dicopp.egg-info/entry_points.txt
+-rw-rw-r--   0 bc        (1000) bc        (1000)       60 2023-07-19 10:36:42.000000 dicopp-1.0.38/dicopp.egg-info/requires.txt
+-rw-rw-r--   0 bc        (1000) bc        (1000)        7 2023-07-19 10:36:42.000000 dicopp-1.0.38/dicopp.egg-info/top_level.txt
+-rw-rw-r--   0 bc        (1000) bc        (1000)       38 2023-07-19 10:36:42.260252 dicopp-1.0.38/setup.cfg
+-rw-rw-r--   0 bc        (1000) bc        (1000)      945 2023-07-15 06:20:45.000000 dicopp-1.0.38/setup.py
```

### Comparing `dicopp-1.0.37/README.md` & `dicopp-1.0.38/README.md`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.37/dicopp/base.py` & `dicopp-1.0.38/dicopp/base.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.37/dicopp/com.py` & `dicopp-1.0.38/dicopp/com.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.37/dicopp/daem.py` & `dicopp-1.0.38/dicopp/daem.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.37/dicopp/details.py` & `dicopp-1.0.38/dicopp/details.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.37/dicopp/dload.py` & `dicopp-1.0.38/dicopp/dload.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.37/dicopp/extension.py` & `dicopp-1.0.38/dicopp/extension.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.37/dicopp/first.py` & `dicopp-1.0.38/dicopp/first.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.37/dicopp/flist.py` & `dicopp-1.0.38/dicopp/flist.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.37/dicopp/hubs.py` & `dicopp-1.0.38/dicopp/hubs.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.37/dicopp/hubscon.py` & `dicopp-1.0.38/dicopp/hubscon.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.37/dicopp/hubson.py` & `dicopp-1.0.38/dicopp/hubson.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.37/dicopp/layout.py` & `dicopp-1.0.38/dicopp/layout.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.37/dicopp/limit.py` & `dicopp-1.0.38/dicopp/limit.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.37/dicopp/log.py` & `dicopp-1.0.38/dicopp/log.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.37/dicopp/nick.py` & `dicopp-1.0.38/dicopp/nick.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.37/dicopp/reqs.py` & `dicopp-1.0.38/dicopp/reqs.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.37/dicopp/search.py` & `dicopp-1.0.38/dicopp/search.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.37/dicopp/sets.py` & `dicopp-1.0.38/dicopp/sets.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.37/dicopp/share.py` & `dicopp-1.0.38/dicopp/share.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.37/dicopp/stor2.py` & `dicopp-1.0.38/dicopp/stor2.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.37/dicopp/userinfo.py` & `dicopp-1.0.38/dicopp/userinfo.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.37/dicopp/users.py` & `dicopp-1.0.38/dicopp/users.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.37/dicopp/usersloc.py` & `dicopp-1.0.38/dicopp/usersloc.py`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.37/dicopp.egg-info/SOURCES.txt` & `dicopp-1.0.38/dicopp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dicopp-1.0.37/setup.py` & `dicopp-1.0.38/setup.py`

 * *Files identical despite different names*

