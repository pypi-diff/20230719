# Comparing `tmp/idkwhttph-0.1.2.tar.gz` & `tmp/idkwhttph-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idkwhttph-0.1.2.tar", max compression
+gzip compressed data, was "idkwhttph-0.2.0.tar", max compression
```

## Comparing `idkwhttph-0.1.2.tar` & `idkwhttph-0.2.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    37180 2023-07-19 13:09:24.076551 idkwhttph-0.1.2/idkwhttph/__init__.py
--rw-r--r--   0        0        0      295 2023-07-19 13:09:13.364557 idkwhttph-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      492 2023-07-19 13:10:17.714866 idkwhttph-0.1.2/setup.py
--rw-r--r--   0        0        0      239 2023-07-19 13:10:17.715195 idkwhttph-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    37164 2023-07-19 13:18:37.721847 idkwhttph-0.2.0/idkwhttph/__init__.py
+-rw-r--r--   0        0        0      295 2023-07-19 13:14:08.898209 idkwhttph-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      492 2023-07-19 13:38:48.477754 idkwhttph-0.2.0/setup.py
+-rw-r--r--   0        0        0      239 2023-07-19 13:38:48.478515 idkwhttph-0.2.0/PKG-INFO
```

### Comparing `idkwhttph-0.1.2/idkwhttph/__init__.py` & `idkwhttph-0.2.0/idkwhttph/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.1.2'
+__version__ = '0.2.0'
 #Imports
 
 from getkey import getkey, keys
 from replit import clear
 from replit import db
 from time import sleep
 import cursor
@@ -1032,15 +1032,14 @@
   
 # Real password
 list_2 = ['']
 list_3 = list_1
 
 
 def Sign_In() -> None:
-  cursor.hide()
   global list_1, list_2, list_3, username,menu,show_hide,alert,JLI,matches
   username = ['']
   list_1 = ['']
   list_2 = ['']
   list_3 = list_1
   alert = False
   show_hide = False
```

