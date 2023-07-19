# Comparing `tmp/idkwhttph-0.1.0.tar.gz` & `tmp/idkwhttph-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idkwhttph-0.1.0.tar", max compression
+gzip compressed data, was "idkwhttph-0.1.1.tar", max compression
```

## Comparing `idkwhttph-0.1.0.tar` & `idkwhttph-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    19493 2023-07-19 12:29:12.974649 idkwhttph-0.1.0/idkwhttph/__init__.py
--rw-r--r--   0        0        0    17691 2023-07-19 12:29:56.022607 idkwhttph-0.1.0/idkwhttph/replit_sync.py
--rw-r--r--   0        0        0      295 2023-07-19 12:28:14.234709 idkwhttph-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      492 2023-07-19 12:31:06.732015 idkwhttph-0.1.0/setup.py
--rw-r--r--   0        0        0      239 2023-07-19 12:31:06.732304 idkwhttph-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    19450 2023-07-19 12:57:29.753088 idkwhttph-0.1.1/idkwhttph/__init__.py
+-rw-r--r--   0        0        0    17691 2023-07-19 12:29:56.022607 idkwhttph-0.1.1/idkwhttph/replit_sync.py
+-rw-r--r--   0        0        0      295 2023-07-19 13:00:16.128912 idkwhttph-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      492 2023-07-19 13:00:30.437182 idkwhttph-0.1.1/setup.py
+-rw-r--r--   0        0        0      239 2023-07-19 13:00:30.437590 idkwhttph-0.1.1/PKG-INFO
```

### Comparing `idkwhttph-0.1.0/idkwhttph/__init__.py` & `idkwhttph-0.1.1/idkwhttph/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-__version__ = '0.1.0'
+__version__ = '0.1.1'
 #Imports
 
-from colorama import Fore as F, Style as S
 from getkey import getkey, keys
 from replit import clear
 from replit import db
 from time import sleep
 import cursor
 import json
 import shutil;
```

### Comparing `idkwhttph-0.1.0/idkwhttph/replit_sync.py` & `idkwhttph-0.1.1/idkwhttph/replit_sync.py`

 * *Files identical despite different names*

