# Comparing `tmp/htscf-0.0.2.tar.gz` & `tmp/htscf-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htscf-0.0.2.tar", last modified: Tue Jul 18 13:23:49 2023, max compression
+gzip compressed data, was "htscf-0.0.3.tar", last modified: Tue Jul 18 13:37:59 2023, max compression
```

## Comparing `htscf-0.0.2.tar` & `htscf-0.0.3.tar`

### file list

```diff
@@ -1,35 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 13:23:49.409767 htscf-0.0.2/
--rw-rw-rw-   0        0        0     1084 2022-03-29 00:57:11.000000 htscf-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      209 2022-08-07 16:57:01.000000 htscf-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      825 2023-07-18 13:23:49.409767 htscf-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      336 2022-08-09 08:26:17.000000 htscf-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 13:23:49.394832 htscf-0.0.2/htscf.egg-info/
--rw-rw-rw-   0        0        0      825 2023-07-18 13:23:49.000000 htscf-0.0.2/htscf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      555 2023-07-18 13:23:49.000000 htscf-0.0.2/htscf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 13:23:49.000000 htscf-0.0.2/htscf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-07-18 13:23:49.000000 htscf-0.0.2/htscf.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-07-18 13:18:21.000000 htscf-0.0.2/htscf.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       63 2023-07-18 13:23:49.000000 htscf-0.0.2/htscf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-18 13:23:49.000000 htscf-0.0.2/htscf.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-18 13:23:49.395805 htscf-0.0.2/htsct/
--rw-rw-rw-   0        0        0       36 2023-07-18 13:06:43.000000 htscf-0.0.2/htsct/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 13:23:49.401788 htscf-0.0.2/htsct/cli/
--rw-rw-rw-   0        0        0        0 2022-03-17 08:58:49.000000 htscf-0.0.2/htsct/cli/__init__.py
--rw-rw-rw-   0        0        0     1299 2023-07-18 12:34:47.000000 htscf-0.0.2/htsct/cli/bdc.py
--rw-rw-rw-   0        0        0     1182 2022-03-31 08:13:37.000000 htscf-0.0.2/htsct/cli/login.py
--rw-rw-rw-   0        0        0     1085 2022-03-31 08:05:58.000000 htscf-0.0.2/htsct/cli/logout.py
--rw-rw-rw-   0        0        0     1438 2023-07-18 12:36:26.000000 htscf-0.0.2/htsct/cli/main.py
-drwxrwxrwx   0        0        0        0 2023-07-18 13:23:49.403783 htscf-0.0.2/htsct/core/
--rw-rw-rw-   0        0        0        0 2021-10-09 11:42:50.000000 htscf-0.0.2/htsct/core/__init__.py
--rw-rw-rw-   0        0        0      802 2023-07-18 11:50:59.000000 htscf-0.0.2/htsct/core/createStep.py
--rw-rw-rw-   0        0        0     2649 2023-07-18 12:21:40.000000 htscf-0.0.2/htsct/core/flow.py
-drwxrwxrwx   0        0        0        0 2023-07-18 13:23:49.405777 htscf-0.0.2/htsct/test/
--rw-rw-rw-   0        0        0        0 2023-07-18 13:07:06.000000 htscf-0.0.2/htsct/test/__init__.py
--rw-rw-rw-   0        0        0      175 2023-07-18 13:07:53.000000 htscf-0.0.2/htsct/test/test.py
-drwxrwxrwx   0        0        0        0 2023-07-18 13:23:49.408769 htscf-0.0.2/htsct/utils/
--rw-rw-rw-   0        0        0        0 2021-10-09 11:42:50.000000 htscf-0.0.2/htsct/utils/__init__.py
--rw-rw-rw-   0        0        0     1956 2023-07-18 13:04:20.000000 htscf-0.0.2/htsct/utils/qsub.py
--rw-rw-rw-   0        0        0     2740 2023-07-18 13:06:01.000000 htscf-0.0.2/htsct/utils/tools.py
--rw-rw-rw-   0        0        0       80 2022-03-09 04:15:13.000000 htscf-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      669 2023-07-18 13:23:49.410764 htscf-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      197 2023-07-18 13:08:10.000000 htscf-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 13:37:59.051215 htscf-0.0.3/
+-rw-rw-rw-   0        0        0     1084 2022-03-29 00:57:11.000000 htscf-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      209 2023-07-18 13:34:36.000000 htscf-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      825 2023-07-18 13:37:59.051215 htscf-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      336 2022-08-09 08:26:17.000000 htscf-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 13:37:59.012345 htscf-0.0.3/htscf/
+-rw-rw-rw-   0        0        0        0 2023-07-18 13:34:36.000000 htscf-0.0.3/htscf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 13:37:59.039247 htscf-0.0.3/htscf/cli/
+-rw-rw-rw-   0        0        0        0 2022-03-17 08:58:49.000000 htscf-0.0.3/htscf/cli/__init__.py
+-rw-rw-rw-   0        0        0     1299 2023-07-18 13:34:36.000000 htscf-0.0.3/htscf/cli/bdc.py
+-rw-rw-rw-   0        0        0     1182 2022-03-31 08:13:37.000000 htscf-0.0.3/htscf/cli/login.py
+-rw-rw-rw-   0        0        0     1085 2022-03-31 08:05:58.000000 htscf-0.0.3/htscf/cli/logout.py
+-rw-rw-rw-   0        0        0     1438 2023-07-18 12:36:26.000000 htscf-0.0.3/htscf/cli/main.py
+drwxrwxrwx   0        0        0        0 2023-07-18 13:37:59.043236 htscf-0.0.3/htscf/core/
+-rw-rw-rw-   0        0        0        0 2021-10-09 11:42:50.000000 htscf-0.0.3/htscf/core/__init__.py
+-rw-rw-rw-   0        0        0      802 2023-07-18 11:50:59.000000 htscf-0.0.3/htscf/core/createStep.py
+-rw-rw-rw-   0        0        0     2649 2023-07-18 13:37:43.000000 htscf-0.0.3/htscf/core/flow.py
+drwxrwxrwx   0        0        0        0 2023-07-18 13:37:59.045231 htscf-0.0.3/htscf/io/
+-rw-rw-rw-   0        0        0        0 2021-10-09 11:42:50.000000 htscf-0.0.3/htscf/io/__init__.py
+-rw-rw-rw-   0        0        0     4919 2023-07-18 13:37:43.000000 htscf-0.0.3/htscf/io/vaspIO.py
+drwxrwxrwx   0        0        0        0 2023-07-18 13:37:59.047226 htscf-0.0.3/htscf/test/
+-rw-rw-rw-   0        0        0        0 2023-07-18 13:07:06.000000 htscf-0.0.3/htscf/test/__init__.py
+-rw-rw-rw-   0        0        0      175 2023-07-18 13:07:53.000000 htscf-0.0.3/htscf/test/test.py
+drwxrwxrwx   0        0        0        0 2023-07-18 13:37:59.050243 htscf-0.0.3/htscf/utils/
+-rw-rw-rw-   0        0        0        0 2021-10-09 11:42:50.000000 htscf-0.0.3/htscf/utils/__init__.py
+-rw-rw-rw-   0        0        0     1956 2023-07-18 13:04:20.000000 htscf-0.0.3/htscf/utils/qsub.py
+-rw-rw-rw-   0        0        0     2740 2023-07-18 13:06:01.000000 htscf-0.0.3/htscf/utils/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-18 13:37:59.034285 htscf-0.0.3/htscf.egg-info/
+-rw-rw-rw-   0        0        0      825 2023-07-18 13:37:58.000000 htscf-0.0.3/htscf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      595 2023-07-18 13:37:58.000000 htscf-0.0.3/htscf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 13:37:58.000000 htscf-0.0.3/htscf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-07-18 13:37:58.000000 htscf-0.0.3/htscf.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-07-18 13:18:21.000000 htscf-0.0.3/htscf.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       63 2023-07-18 13:37:58.000000 htscf-0.0.3/htscf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-18 13:37:58.000000 htscf-0.0.3/htscf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       80 2022-03-09 04:15:13.000000 htscf-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      669 2023-07-18 13:37:59.052212 htscf-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      197 2023-07-18 13:08:10.000000 htscf-0.0.3/setup.py
```

### Comparing `htscf-0.0.2/LICENSE` & `htscf-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `htscf-0.0.2/PKG-INFO` & `htscf-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htscf
-Version: 0.0.2
+Version: 0.0.3
 Summary: High-throughput computing flow
 Home-page: http://zhcloud.top
 Author: Hao Zhao
 Author-email: 601095001@qq.com
 License: OSI Approved :: MIT License
 Platform: Linux/Windows
 Classifier: Programming Language :: Python :: 3
```

### Comparing `htscf-0.0.2/htscf.egg-info/PKG-INFO` & `htscf-0.0.3/htscf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htscf
-Version: 0.0.2
+Version: 0.0.3
 Summary: High-throughput computing flow
 Home-page: http://zhcloud.top
 Author: Hao Zhao
 Author-email: 601095001@qq.com
 License: OSI Approved :: MIT License
 Platform: Linux/Windows
 Classifier: Programming Language :: Python :: 3
```

### Comparing `htscf-0.0.2/htscf.egg-info/SOURCES.txt` & `htscf-0.0.3/htscf.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
+htscf/__init__.py
 htscf.egg-info/PKG-INFO
 htscf.egg-info/SOURCES.txt
 htscf.egg-info/dependency_links.txt
 htscf.egg-info/entry_points.txt
 htscf.egg-info/not-zip-safe
 htscf.egg-info/requires.txt
 htscf.egg-info/top_level.txt
-htsct/__init__.py
-htsct/cli/__init__.py
-htsct/cli/bdc.py
-htsct/cli/login.py
-htsct/cli/logout.py
-htsct/cli/main.py
-htsct/core/__init__.py
-htsct/core/createStep.py
-htsct/core/flow.py
-htsct/test/__init__.py
-htsct/test/test.py
-htsct/utils/__init__.py
-htsct/utils/qsub.py
-htsct/utils/tools.py
+htscf/cli/__init__.py
+htscf/cli/bdc.py
+htscf/cli/login.py
+htscf/cli/logout.py
+htscf/cli/main.py
+htscf/core/__init__.py
+htscf/core/createStep.py
+htscf/core/flow.py
+htscf/io/__init__.py
+htscf/io/vaspIO.py
+htscf/test/__init__.py
+htscf/test/test.py
+htscf/utils/__init__.py
+htscf/utils/qsub.py
+htscf/utils/tools.py
```

### Comparing `htscf-0.0.2/htsct/cli/bdc.py` & `htscf-0.0.3/htscf/cli/bdc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from argparse import ArgumentParser
-from htsct.io.vaspIO import writeIncar
+from htscf.io.vaspIO import writeIncar
 from os import system
 
 
 class CLICommand:
     """bandDecomposedCharge
     """
```

### Comparing `htscf-0.0.2/htsct/cli/login.py` & `htscf-0.0.3/htscf/cli/login.py`

 * *Files identical despite different names*

### Comparing `htscf-0.0.2/htsct/cli/logout.py` & `htscf-0.0.3/htscf/cli/logout.py`

 * *Files identical despite different names*

### Comparing `htscf-0.0.2/htsct/cli/main.py` & `htscf-0.0.3/htscf/cli/main.py`

 * *Files identical despite different names*

### Comparing `htscf-0.0.2/htsct/core/createStep.py` & `htscf-0.0.3/htscf/core/createStep.py`

 * *Files identical despite different names*

### Comparing `htscf-0.0.2/htsct/core/flow.py` & `htscf-0.0.3/htscf/core/flow.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 from subprocess import Popen, PIPE
 from typing import Union
 from functools import reduce
-from htsct.db.mongo import connect
+from htscf.db.mongo import connect
 from uuid import uuid4
 from pathlib import Path
 from sys import platform
 
 
 def workflow(rootPath: Union[Path, str], stepIds: list[str], dbName, stepsCollectionName, stepLogCollectionName, host, port):
     """
```

### Comparing `htscf-0.0.2/htsct/utils/qsub.py` & `htscf-0.0.3/htscf/utils/qsub.py`

 * *Files identical despite different names*

### Comparing `htscf-0.0.2/htsct/utils/tools.py` & `htscf-0.0.3/htscf/utils/tools.py`

 * *Files identical despite different names*

### Comparing `htscf-0.0.2/setup.cfg` & `htscf-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2068 7473 6366 0d0a 7665 7273 696f   = htscf..versio
-00000020: 6e20 3d20 302e 302e 320d 0a64 6573 6372  n = 0.0.2..descr
+00000020: 6e20 3d20 302e 302e 330d 0a64 6573 6372  n = 0.0.3..descr
 00000030: 6970 7469 6f6e 203d 2048 6967 682d 7468  iption = High-th
 00000040: 726f 7567 6870 7574 2063 6f6d 7075 7469  roughput computi
 00000050: 6e67 2066 6c6f 770d 0a6c 6f6e 675f 6465  ng flow..long_de
 00000060: 7363 7269 7074 696f 6e20 3d20 6669 6c65  scription = file
 00000070: 3a20 5245 4144 4d45 2e6d 640d 0a6c 6f6e  : README.md..lon
 00000080: 675f 6465 7363 7269 7074 696f 6e5f 636f  g_description_co
 00000090: 6e74 656e 745f 7479 7065 203d 2074 6578  ntent_type = tex
```

