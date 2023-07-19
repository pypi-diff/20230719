# Comparing `tmp/htscf-0.0.4.tar.gz` & `tmp/htscf-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htscf-0.0.4.tar", last modified: Wed Jul 19 07:43:11 2023, max compression
+gzip compressed data, was "htscf-0.0.5.tar", last modified: Wed Jul 19 07:55:22 2023, max compression
```

## Comparing `htscf-0.0.4.tar` & `htscf-0.0.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 07:43:10.999829 htscf-0.0.4/
--rw-rw-rw-   0        0        0     1084 2022-03-29 00:57:11.000000 htscf-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      209 2023-07-18 13:34:36.000000 htscf-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      825 2023-07-19 07:43:11.000827 htscf-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      336 2022-08-09 08:26:17.000000 htscf-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-19 07:43:10.894019 htscf-0.0.4/htscf/
--rw-rw-rw-   0        0        0        0 2023-07-18 13:34:36.000000 htscf-0.0.4/htscf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-19 07:43:10.956534 htscf-0.0.4/htscf/cli/
--rw-rw-rw-   0        0        0        0 2022-03-17 08:58:49.000000 htscf-0.0.4/htscf/cli/__init__.py
--rw-rw-rw-   0        0        0     1299 2023-07-18 13:34:36.000000 htscf-0.0.4/htscf/cli/bdc.py
--rw-rw-rw-   0        0        0     1182 2022-03-31 08:13:37.000000 htscf-0.0.4/htscf/cli/login.py
--rw-rw-rw-   0        0        0     1085 2022-03-31 08:05:58.000000 htscf-0.0.4/htscf/cli/logout.py
--rw-rw-rw-   0        0        0     1438 2023-07-18 12:36:26.000000 htscf-0.0.4/htscf/cli/main.py
-drwxrwxrwx   0        0        0        0 2023-07-19 07:43:10.960520 htscf-0.0.4/htscf/core/
--rw-rw-rw-   0        0        0        0 2021-10-09 11:42:50.000000 htscf-0.0.4/htscf/core/__init__.py
--rw-rw-rw-   0        0        0      802 2023-07-18 11:50:59.000000 htscf-0.0.4/htscf/core/createStep.py
--rw-rw-rw-   0        0        0     2796 2023-07-19 07:42:39.000000 htscf-0.0.4/htscf/core/flow.py
-drwxrwxrwx   0        0        0        0 2023-07-19 07:43:10.968877 htscf-0.0.4/htscf/io/
--rw-rw-rw-   0        0        0        0 2021-10-09 11:42:50.000000 htscf-0.0.4/htscf/io/__init__.py
--rw-rw-rw-   0        0        0     4919 2023-07-18 13:37:43.000000 htscf-0.0.4/htscf/io/vaspIO.py
-drwxrwxrwx   0        0        0        0 2023-07-19 07:43:10.975888 htscf-0.0.4/htscf/test/
--rw-rw-rw-   0        0        0        0 2023-07-18 13:07:06.000000 htscf-0.0.4/htscf/test/__init__.py
--rw-rw-rw-   0        0        0      175 2023-07-18 13:07:53.000000 htscf-0.0.4/htscf/test/test.py
-drwxrwxrwx   0        0        0        0 2023-07-19 07:43:10.998832 htscf-0.0.4/htscf/utils/
--rw-rw-rw-   0        0        0        0 2021-10-09 11:42:50.000000 htscf-0.0.4/htscf/utils/__init__.py
--rw-rw-rw-   0        0        0     1956 2023-07-18 13:04:20.000000 htscf-0.0.4/htscf/utils/qsub.py
--rw-rw-rw-   0        0        0     2740 2023-07-18 13:06:01.000000 htscf-0.0.4/htscf/utils/tools.py
-drwxrwxrwx   0        0        0        0 2023-07-19 07:43:10.921779 htscf-0.0.4/htscf.egg-info/
--rw-rw-rw-   0        0        0      825 2023-07-19 07:43:10.000000 htscf-0.0.4/htscf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      595 2023-07-19 07:43:10.000000 htscf-0.0.4/htscf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 07:43:10.000000 htscf-0.0.4/htscf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-07-19 07:43:10.000000 htscf-0.0.4/htscf.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-07-18 13:18:21.000000 htscf-0.0.4/htscf.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       63 2023-07-19 07:43:10.000000 htscf-0.0.4/htscf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-19 07:43:10.000000 htscf-0.0.4/htscf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       80 2022-03-09 04:15:13.000000 htscf-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0      669 2023-07-19 07:43:11.001824 htscf-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      197 2023-07-18 13:08:10.000000 htscf-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 07:55:22.191654 htscf-0.0.5/
+-rw-rw-rw-   0        0        0     1084 2022-03-29 00:57:11.000000 htscf-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      209 2023-07-18 13:34:36.000000 htscf-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      825 2023-07-19 07:55:22.191654 htscf-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      336 2022-08-09 08:26:17.000000 htscf-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-19 07:55:22.151378 htscf-0.0.5/htscf/
+-rw-rw-rw-   0        0        0        0 2023-07-18 13:34:36.000000 htscf-0.0.5/htscf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 07:55:22.180820 htscf-0.0.5/htscf/cli/
+-rw-rw-rw-   0        0        0        0 2022-03-17 08:58:49.000000 htscf-0.0.5/htscf/cli/__init__.py
+-rw-rw-rw-   0        0        0     1299 2023-07-18 13:34:36.000000 htscf-0.0.5/htscf/cli/bdc.py
+-rw-rw-rw-   0        0        0     1182 2022-03-31 08:13:37.000000 htscf-0.0.5/htscf/cli/login.py
+-rw-rw-rw-   0        0        0     1085 2022-03-31 08:05:58.000000 htscf-0.0.5/htscf/cli/logout.py
+-rw-rw-rw-   0        0        0     1438 2023-07-18 12:36:26.000000 htscf-0.0.5/htscf/cli/main.py
+drwxrwxrwx   0        0        0        0 2023-07-19 07:55:22.183875 htscf-0.0.5/htscf/core/
+-rw-rw-rw-   0        0        0        0 2021-10-09 11:42:50.000000 htscf-0.0.5/htscf/core/__init__.py
+-rw-rw-rw-   0        0        0      802 2023-07-18 11:50:59.000000 htscf-0.0.5/htscf/core/createStep.py
+-rw-rw-rw-   0        0        0     2796 2023-07-19 07:42:39.000000 htscf-0.0.5/htscf/core/flow.py
+drwxrwxrwx   0        0        0        0 2023-07-19 07:55:22.185872 htscf-0.0.5/htscf/io/
+-rw-rw-rw-   0        0        0        0 2021-10-09 11:42:50.000000 htscf-0.0.5/htscf/io/__init__.py
+-rw-rw-rw-   0        0        0     4919 2023-07-18 13:37:43.000000 htscf-0.0.5/htscf/io/vaspIO.py
+drwxrwxrwx   0        0        0        0 2023-07-19 07:55:22.187664 htscf-0.0.5/htscf/test/
+-rw-rw-rw-   0        0        0        0 2023-07-18 13:07:06.000000 htscf-0.0.5/htscf/test/__init__.py
+-rw-rw-rw-   0        0        0      175 2023-07-18 13:07:53.000000 htscf-0.0.5/htscf/test/test.py
+drwxrwxrwx   0        0        0        0 2023-07-19 07:55:22.190657 htscf-0.0.5/htscf/utils/
+-rw-rw-rw-   0        0        0        0 2021-10-09 11:42:50.000000 htscf-0.0.5/htscf/utils/__init__.py
+-rw-rw-rw-   0        0        0     1956 2023-07-18 13:04:20.000000 htscf-0.0.5/htscf/utils/qsub.py
+-rw-rw-rw-   0        0        0     2740 2023-07-18 13:06:01.000000 htscf-0.0.5/htscf/utils/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-19 07:55:22.175215 htscf-0.0.5/htscf.egg-info/
+-rw-rw-rw-   0        0        0      825 2023-07-19 07:55:22.000000 htscf-0.0.5/htscf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      595 2023-07-19 07:55:22.000000 htscf-0.0.5/htscf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 07:55:22.000000 htscf-0.0.5/htscf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-07-19 07:55:22.000000 htscf-0.0.5/htscf.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-07-18 13:18:21.000000 htscf-0.0.5/htscf.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       63 2023-07-19 07:55:22.000000 htscf-0.0.5/htscf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-19 07:55:22.000000 htscf-0.0.5/htscf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       80 2022-03-09 04:15:13.000000 htscf-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0      669 2023-07-19 07:55:22.192679 htscf-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      197 2023-07-18 13:08:10.000000 htscf-0.0.5/setup.py
```

### Comparing `htscf-0.0.4/LICENSE` & `htscf-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `htscf-0.0.4/PKG-INFO` & `htscf-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htscf
-Version: 0.0.4
+Version: 0.0.5
 Summary: High-throughput computing flow
 Home-page: http://zhcloud.top
 Author: Hao Zhao
 Author-email: 601095001@qq.com
 License: OSI Approved :: MIT License
 Platform: Linux/Windows
 Classifier: Programming Language :: Python :: 3
```

### Comparing `htscf-0.0.4/htscf/cli/bdc.py` & `htscf-0.0.5/htscf/cli/bdc.py`

 * *Files identical despite different names*

### Comparing `htscf-0.0.4/htscf/cli/login.py` & `htscf-0.0.5/htscf/cli/login.py`

 * *Files identical despite different names*

### Comparing `htscf-0.0.4/htscf/cli/logout.py` & `htscf-0.0.5/htscf/cli/logout.py`

 * *Files identical despite different names*

### Comparing `htscf-0.0.4/htscf/cli/main.py` & `htscf-0.0.5/htscf/cli/main.py`

 * *Files identical despite different names*

### Comparing `htscf-0.0.4/htscf/core/createStep.py` & `htscf-0.0.5/htscf/core/createStep.py`

 * *Files identical despite different names*

### Comparing `htscf-0.0.4/htscf/core/flow.py` & `htscf-0.0.5/htscf/core/flow.py`

 * *Files identical despite different names*

### Comparing `htscf-0.0.4/htscf/io/vaspIO.py` & `htscf-0.0.5/htscf/io/vaspIO.py`

 * *Files identical despite different names*

### Comparing `htscf-0.0.4/htscf/utils/qsub.py` & `htscf-0.0.5/htscf/utils/qsub.py`

 * *Files identical despite different names*

### Comparing `htscf-0.0.4/htscf/utils/tools.py` & `htscf-0.0.5/htscf/utils/tools.py`

 * *Files identical despite different names*

### Comparing `htscf-0.0.4/htscf.egg-info/PKG-INFO` & `htscf-0.0.5/htscf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htscf
-Version: 0.0.4
+Version: 0.0.5
 Summary: High-throughput computing flow
 Home-page: http://zhcloud.top
 Author: Hao Zhao
 Author-email: 601095001@qq.com
 License: OSI Approved :: MIT License
 Platform: Linux/Windows
 Classifier: Programming Language :: Python :: 3
```

### Comparing `htscf-0.0.4/htscf.egg-info/SOURCES.txt` & `htscf-0.0.5/htscf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `htscf-0.0.4/setup.cfg` & `htscf-0.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2068 7473 6366 0d0a 7665 7273 696f   = htscf..versio
-00000020: 6e20 3d20 302e 302e 340d 0a64 6573 6372  n = 0.0.4..descr
+00000020: 6e20 3d20 302e 302e 350d 0a64 6573 6372  n = 0.0.5..descr
 00000030: 6970 7469 6f6e 203d 2048 6967 682d 7468  iption = High-th
 00000040: 726f 7567 6870 7574 2063 6f6d 7075 7469  roughput computi
 00000050: 6e67 2066 6c6f 770d 0a6c 6f6e 675f 6465  ng flow..long_de
 00000060: 7363 7269 7074 696f 6e20 3d20 6669 6c65  scription = file
 00000070: 3a20 5245 4144 4d45 2e6d 640d 0a6c 6f6e  : README.md..lon
 00000080: 675f 6465 7363 7269 7074 696f 6e5f 636f  g_description_co
 00000090: 6e74 656e 745f 7479 7065 203d 2074 6578  ntent_type = tex
```

