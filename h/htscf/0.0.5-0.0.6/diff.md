# Comparing `tmp/htscf-0.0.5.tar.gz` & `tmp/htscf-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htscf-0.0.5.tar", last modified: Wed Jul 19 07:55:22 2023, max compression
+gzip compressed data, was "htscf-0.0.6.tar", last modified: Wed Jul 19 08:05:00 2023, max compression
```

## Comparing `htscf-0.0.5.tar` & `htscf-0.0.6.tar`

### file list

```diff
@@ -1,38 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 07:55:22.191654 htscf-0.0.5/
--rw-rw-rw-   0        0        0     1084 2022-03-29 00:57:11.000000 htscf-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      209 2023-07-18 13:34:36.000000 htscf-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      825 2023-07-19 07:55:22.191654 htscf-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      336 2022-08-09 08:26:17.000000 htscf-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-19 07:55:22.151378 htscf-0.0.5/htscf/
--rw-rw-rw-   0        0        0        0 2023-07-18 13:34:36.000000 htscf-0.0.5/htscf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-19 07:55:22.180820 htscf-0.0.5/htscf/cli/
--rw-rw-rw-   0        0        0        0 2022-03-17 08:58:49.000000 htscf-0.0.5/htscf/cli/__init__.py
--rw-rw-rw-   0        0        0     1299 2023-07-18 13:34:36.000000 htscf-0.0.5/htscf/cli/bdc.py
--rw-rw-rw-   0        0        0     1182 2022-03-31 08:13:37.000000 htscf-0.0.5/htscf/cli/login.py
--rw-rw-rw-   0        0        0     1085 2022-03-31 08:05:58.000000 htscf-0.0.5/htscf/cli/logout.py
--rw-rw-rw-   0        0        0     1438 2023-07-18 12:36:26.000000 htscf-0.0.5/htscf/cli/main.py
-drwxrwxrwx   0        0        0        0 2023-07-19 07:55:22.183875 htscf-0.0.5/htscf/core/
--rw-rw-rw-   0        0        0        0 2021-10-09 11:42:50.000000 htscf-0.0.5/htscf/core/__init__.py
--rw-rw-rw-   0        0        0      802 2023-07-18 11:50:59.000000 htscf-0.0.5/htscf/core/createStep.py
--rw-rw-rw-   0        0        0     2796 2023-07-19 07:42:39.000000 htscf-0.0.5/htscf/core/flow.py
-drwxrwxrwx   0        0        0        0 2023-07-19 07:55:22.185872 htscf-0.0.5/htscf/io/
--rw-rw-rw-   0        0        0        0 2021-10-09 11:42:50.000000 htscf-0.0.5/htscf/io/__init__.py
--rw-rw-rw-   0        0        0     4919 2023-07-18 13:37:43.000000 htscf-0.0.5/htscf/io/vaspIO.py
-drwxrwxrwx   0        0        0        0 2023-07-19 07:55:22.187664 htscf-0.0.5/htscf/test/
--rw-rw-rw-   0        0        0        0 2023-07-18 13:07:06.000000 htscf-0.0.5/htscf/test/__init__.py
--rw-rw-rw-   0        0        0      175 2023-07-18 13:07:53.000000 htscf-0.0.5/htscf/test/test.py
-drwxrwxrwx   0        0        0        0 2023-07-19 07:55:22.190657 htscf-0.0.5/htscf/utils/
--rw-rw-rw-   0        0        0        0 2021-10-09 11:42:50.000000 htscf-0.0.5/htscf/utils/__init__.py
--rw-rw-rw-   0        0        0     1956 2023-07-18 13:04:20.000000 htscf-0.0.5/htscf/utils/qsub.py
--rw-rw-rw-   0        0        0     2740 2023-07-18 13:06:01.000000 htscf-0.0.5/htscf/utils/tools.py
-drwxrwxrwx   0        0        0        0 2023-07-19 07:55:22.175215 htscf-0.0.5/htscf.egg-info/
--rw-rw-rw-   0        0        0      825 2023-07-19 07:55:22.000000 htscf-0.0.5/htscf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      595 2023-07-19 07:55:22.000000 htscf-0.0.5/htscf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 07:55:22.000000 htscf-0.0.5/htscf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-07-19 07:55:22.000000 htscf-0.0.5/htscf.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-07-18 13:18:21.000000 htscf-0.0.5/htscf.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       63 2023-07-19 07:55:22.000000 htscf-0.0.5/htscf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-19 07:55:22.000000 htscf-0.0.5/htscf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       80 2022-03-09 04:15:13.000000 htscf-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0      669 2023-07-19 07:55:22.192679 htscf-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      197 2023-07-18 13:08:10.000000 htscf-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 08:05:00.317605 htscf-0.0.6/
+-rw-rw-rw-   0        0        0     1084 2022-03-29 00:57:11.000000 htscf-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      209 2023-07-18 13:34:36.000000 htscf-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      825 2023-07-19 08:05:00.317605 htscf-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      336 2022-08-09 08:26:17.000000 htscf-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-19 08:05:00.283000 htscf-0.0.6/htscf/
+-rw-rw-rw-   0        0        0        0 2023-07-18 13:34:36.000000 htscf-0.0.6/htscf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 08:05:00.305939 htscf-0.0.6/htscf/cli/
+-rw-rw-rw-   0        0        0        0 2022-03-17 08:58:49.000000 htscf-0.0.6/htscf/cli/__init__.py
+-rw-rw-rw-   0        0        0     1299 2023-07-18 13:34:36.000000 htscf-0.0.6/htscf/cli/bdc.py
+-rw-rw-rw-   0        0        0     1182 2022-03-31 08:13:37.000000 htscf-0.0.6/htscf/cli/login.py
+-rw-rw-rw-   0        0        0     1085 2022-03-31 08:05:58.000000 htscf-0.0.6/htscf/cli/logout.py
+-rw-rw-rw-   0        0        0     1438 2023-07-18 12:36:26.000000 htscf-0.0.6/htscf/cli/main.py
+drwxrwxrwx   0        0        0        0 2023-07-19 08:05:00.308930 htscf-0.0.6/htscf/core/
+-rw-rw-rw-   0        0        0        0 2021-10-09 11:42:50.000000 htscf-0.0.6/htscf/core/__init__.py
+-rw-rw-rw-   0        0        0      802 2023-07-18 11:50:59.000000 htscf-0.0.6/htscf/core/createStep.py
+-rw-rw-rw-   0        0        0     2796 2023-07-19 07:42:39.000000 htscf-0.0.6/htscf/core/flow.py
+drwxrwxrwx   0        0        0        0 2023-07-19 08:05:00.310433 htscf-0.0.6/htscf/db/
+-rw-rw-rw-   0        0        0        0 2023-07-18 06:33:00.000000 htscf-0.0.6/htscf/db/__init__.py
+-rw-rw-rw-   0        0        0      264 2023-07-18 06:38:01.000000 htscf-0.0.6/htscf/db/mongo.py
+drwxrwxrwx   0        0        0        0 2023-07-19 08:05:00.312427 htscf-0.0.6/htscf/io/
+-rw-rw-rw-   0        0        0        0 2021-10-09 11:42:50.000000 htscf-0.0.6/htscf/io/__init__.py
+-rw-rw-rw-   0        0        0     4919 2023-07-18 13:37:43.000000 htscf-0.0.6/htscf/io/vaspIO.py
+drwxrwxrwx   0        0        0        0 2023-07-19 08:05:00.314293 htscf-0.0.6/htscf/test/
+-rw-rw-rw-   0        0        0        0 2023-07-18 13:07:06.000000 htscf-0.0.6/htscf/test/__init__.py
+-rw-rw-rw-   0        0        0      175 2023-07-18 13:07:53.000000 htscf-0.0.6/htscf/test/test.py
+drwxrwxrwx   0        0        0        0 2023-07-19 08:05:00.316606 htscf-0.0.6/htscf/utils/
+-rw-rw-rw-   0        0        0        0 2021-10-09 11:42:50.000000 htscf-0.0.6/htscf/utils/__init__.py
+-rw-rw-rw-   0        0        0     1956 2023-07-18 13:04:20.000000 htscf-0.0.6/htscf/utils/qsub.py
+-rw-rw-rw-   0        0        0     2740 2023-07-18 13:06:01.000000 htscf-0.0.6/htscf/utils/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-19 08:05:00.299980 htscf-0.0.6/htscf.egg-info/
+-rw-rw-rw-   0        0        0      825 2023-07-19 08:05:00.000000 htscf-0.0.6/htscf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      634 2023-07-19 08:05:00.000000 htscf-0.0.6/htscf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 08:05:00.000000 htscf-0.0.6/htscf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-07-19 08:05:00.000000 htscf-0.0.6/htscf.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-07-18 13:18:21.000000 htscf-0.0.6/htscf.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       63 2023-07-19 08:05:00.000000 htscf-0.0.6/htscf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-19 08:05:00.000000 htscf-0.0.6/htscf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       80 2022-03-09 04:15:13.000000 htscf-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0      669 2023-07-19 08:05:00.319600 htscf-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      197 2023-07-18 13:08:10.000000 htscf-0.0.6/setup.py
```

### Comparing `htscf-0.0.5/LICENSE` & `htscf-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `htscf-0.0.5/PKG-INFO` & `htscf-0.0.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htscf
-Version: 0.0.5
+Version: 0.0.6
 Summary: High-throughput computing flow
 Home-page: http://zhcloud.top
 Author: Hao Zhao
 Author-email: 601095001@qq.com
 License: OSI Approved :: MIT License
 Platform: Linux/Windows
 Classifier: Programming Language :: Python :: 3
```

### Comparing `htscf-0.0.5/htscf/cli/bdc.py` & `htscf-0.0.6/htscf/cli/bdc.py`

 * *Files identical despite different names*

### Comparing `htscf-0.0.5/htscf/cli/login.py` & `htscf-0.0.6/htscf/cli/login.py`

 * *Files identical despite different names*

### Comparing `htscf-0.0.5/htscf/cli/logout.py` & `htscf-0.0.6/htscf/cli/logout.py`

 * *Files identical despite different names*

### Comparing `htscf-0.0.5/htscf/cli/main.py` & `htscf-0.0.6/htscf/cli/main.py`

 * *Files identical despite different names*

### Comparing `htscf-0.0.5/htscf/core/createStep.py` & `htscf-0.0.6/htscf/core/createStep.py`

 * *Files identical despite different names*

### Comparing `htscf-0.0.5/htscf/core/flow.py` & `htscf-0.0.6/htscf/core/flow.py`

 * *Files identical despite different names*

### Comparing `htscf-0.0.5/htscf/io/vaspIO.py` & `htscf-0.0.6/htscf/io/vaspIO.py`

 * *Files identical despite different names*

### Comparing `htscf-0.0.5/htscf/utils/qsub.py` & `htscf-0.0.6/htscf/utils/qsub.py`

 * *Files identical despite different names*

### Comparing `htscf-0.0.5/htscf/utils/tools.py` & `htscf-0.0.6/htscf/utils/tools.py`

 * *Files identical despite different names*

### Comparing `htscf-0.0.5/htscf.egg-info/PKG-INFO` & `htscf-0.0.6/htscf.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htscf
-Version: 0.0.5
+Version: 0.0.6
 Summary: High-throughput computing flow
 Home-page: http://zhcloud.top
 Author: Hao Zhao
 Author-email: 601095001@qq.com
 License: OSI Approved :: MIT License
 Platform: Linux/Windows
 Classifier: Programming Language :: Python :: 3
```

### Comparing `htscf-0.0.5/htscf.egg-info/SOURCES.txt` & `htscf-0.0.6/htscf.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 htscf/cli/bdc.py
 htscf/cli/login.py
 htscf/cli/logout.py
 htscf/cli/main.py
 htscf/core/__init__.py
 htscf/core/createStep.py
 htscf/core/flow.py
+htscf/db/__init__.py
+htscf/db/mongo.py
 htscf/io/__init__.py
 htscf/io/vaspIO.py
 htscf/test/__init__.py
 htscf/test/test.py
 htscf/utils/__init__.py
 htscf/utils/qsub.py
 htscf/utils/tools.py
```

### Comparing `htscf-0.0.5/setup.cfg` & `htscf-0.0.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2068 7473 6366 0d0a 7665 7273 696f   = htscf..versio
-00000020: 6e20 3d20 302e 302e 350d 0a64 6573 6372  n = 0.0.5..descr
+00000020: 6e20 3d20 302e 302e 360d 0a64 6573 6372  n = 0.0.6..descr
 00000030: 6970 7469 6f6e 203d 2048 6967 682d 7468  iption = High-th
 00000040: 726f 7567 6870 7574 2063 6f6d 7075 7469  roughput computi
 00000050: 6e67 2066 6c6f 770d 0a6c 6f6e 675f 6465  ng flow..long_de
 00000060: 7363 7269 7074 696f 6e20 3d20 6669 6c65  scription = file
 00000070: 3a20 5245 4144 4d45 2e6d 640d 0a6c 6f6e  : README.md..lon
 00000080: 675f 6465 7363 7269 7074 696f 6e5f 636f  g_description_co
 00000090: 6e74 656e 745f 7479 7065 203d 2074 6578  ntent_type = tex
```

