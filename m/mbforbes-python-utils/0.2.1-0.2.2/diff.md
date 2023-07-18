# Comparing `tmp/mbforbes_python_utils-0.2.1.tar.gz` & `tmp/mbforbes_python_utils-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbforbes_python_utils-0.2.1.tar", last modified: Tue Jul 18 19:31:23 2023, max compression
+gzip compressed data, was "mbforbes_python_utils-0.2.2.tar", last modified: Tue Jul 18 19:33:33 2023, max compression
```

## Comparing `mbforbes_python_utils-0.2.1.tar` & `mbforbes_python_utils-0.2.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-07-18 19:31:23.085018 mbforbes_python_utils-0.2.1/
--rw-r--r--   0 max        (501) staff       (20)     1071 2023-07-18 19:17:23.000000 mbforbes_python_utils-0.2.1/LICENSE.txt
--rw-r--r--   0 max        (501) staff       (20)     1156 2023-07-18 19:31:23.084900 mbforbes_python_utils-0.2.1/PKG-INFO
--rw-r--r--   0 max        (501) staff       (20)      861 2023-07-18 19:30:50.000000 mbforbes_python_utils-0.2.1/README.md
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-07-18 19:31:23.084744 mbforbes_python_utils-0.2.1/mbforbes_python_utils.egg-info/
--rw-r--r--   0 max        (501) staff       (20)     1156 2023-07-18 19:31:23.000000 mbforbes_python_utils-0.2.1/mbforbes_python_utils.egg-info/PKG-INFO
--rw-r--r--   0 max        (501) staff       (20)      235 2023-07-18 19:31:23.000000 mbforbes_python_utils-0.2.1/mbforbes_python_utils.egg-info/SOURCES.txt
--rw-r--r--   0 max        (501) staff       (20)        1 2023-07-18 19:31:23.000000 mbforbes_python_utils-0.2.1/mbforbes_python_utils.egg-info/dependency_links.txt
--rw-r--r--   0 max        (501) staff       (20)       22 2023-07-18 19:31:23.000000 mbforbes_python_utils-0.2.1/mbforbes_python_utils.egg-info/top_level.txt
--rw-r--r--   0 max        (501) staff       (20)     1340 2023-07-18 19:16:57.000000 mbforbes_python_utils-0.2.1/mbforbes_python_utils.py
--rw-r--r--   0 max        (501) staff       (20)       38 2023-07-18 19:31:23.085058 mbforbes_python_utils-0.2.1/setup.cfg
--rw-r--r--   0 max        (501) staff       (20)      425 2023-07-18 19:31:14.000000 mbforbes_python_utils-0.2.1/setup.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-07-18 19:33:33.561392 mbforbes_python_utils-0.2.2/
+-rw-r--r--   0 max        (501) staff       (20)     1071 2023-07-18 19:17:23.000000 mbforbes_python_utils-0.2.2/LICENSE.txt
+-rw-r--r--   0 max        (501) staff       (20)     1156 2023-07-18 19:33:33.561277 mbforbes_python_utils-0.2.2/PKG-INFO
+-rw-r--r--   0 max        (501) staff       (20)      861 2023-07-18 19:32:41.000000 mbforbes_python_utils-0.2.2/README.md
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-07-18 19:33:33.561124 mbforbes_python_utils-0.2.2/mbforbes_python_utils.egg-info/
+-rw-r--r--   0 max        (501) staff       (20)     1156 2023-07-18 19:33:33.000000 mbforbes_python_utils-0.2.2/mbforbes_python_utils.egg-info/PKG-INFO
+-rw-r--r--   0 max        (501) staff       (20)      235 2023-07-18 19:33:33.000000 mbforbes_python_utils-0.2.2/mbforbes_python_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 max        (501) staff       (20)        1 2023-07-18 19:33:33.000000 mbforbes_python_utils-0.2.2/mbforbes_python_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 max        (501) staff       (20)       22 2023-07-18 19:33:33.000000 mbforbes_python_utils-0.2.2/mbforbes_python_utils.egg-info/top_level.txt
+-rw-r--r--   0 max        (501) staff       (20)     1340 2023-07-18 19:16:57.000000 mbforbes_python_utils-0.2.2/mbforbes_python_utils.py
+-rw-r--r--   0 max        (501) staff       (20)       38 2023-07-18 19:33:33.561430 mbforbes_python_utils-0.2.2/setup.cfg
+-rw-r--r--   0 max        (501) staff       (20)      425 2023-07-18 19:33:30.000000 mbforbes_python_utils-0.2.2/setup.py
```

### Comparing `mbforbes_python_utils-0.2.1/LICENSE.txt` & `mbforbes_python_utils-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mbforbes_python_utils-0.2.1/PKG-INFO` & `mbforbes_python_utils-0.2.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbforbes_python_utils
-Version: 0.2.1
+Version: 0.2.2
 Summary: Some tiny python utils so I can be lazier.
 Home-page: https://github.com/mbforbes/python-utils
 Author: Maxwell Forbes
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -13,15 +13,15 @@
 
 So maybe I stop writing the same things over and over.
 
 ## Installation
 
 ```sh
 # Python 3 only (I'm using Python 3.7).
-pip install mbforbes_python_utils
+pip install mbforbes-python-utils
 ```
 
 ## Usage
 
 ```python
 from mbforbes_python_utils import read, write, flatten
```

### Comparing `mbforbes_python_utils-0.2.1/README.md` & `mbforbes_python_utils-0.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 So maybe I stop writing the same things over and over.
 
 ## Installation
 
 ```sh
 # Python 3 only (I'm using Python 3.7).
-pip install mbforbes_python_utils
+pip install mbforbes-python-utils
 ```
 
 ## Usage
 
 ```python
 from mbforbes_python_utils import read, write, flatten
```

### Comparing `mbforbes_python_utils-0.2.1/mbforbes_python_utils.egg-info/PKG-INFO` & `mbforbes_python_utils-0.2.2/mbforbes_python_utils.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbforbes-python-utils
-Version: 0.2.1
+Version: 0.2.2
 Summary: Some tiny python utils so I can be lazier.
 Home-page: https://github.com/mbforbes/python-utils
 Author: Maxwell Forbes
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -13,15 +13,15 @@
 
 So maybe I stop writing the same things over and over.
 
 ## Installation
 
 ```sh
 # Python 3 only (I'm using Python 3.7).
-pip install mbforbes_python_utils
+pip install mbforbes-python-utils
 ```
 
 ## Usage
 
 ```python
 from mbforbes_python_utils import read, write, flatten
```

### Comparing `mbforbes_python_utils-0.2.1/mbforbes_python_utils.py` & `mbforbes_python_utils-0.2.2/mbforbes_python_utils.py`

 * *Files identical despite different names*

