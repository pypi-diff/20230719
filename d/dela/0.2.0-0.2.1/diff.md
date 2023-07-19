# Comparing `tmp/dela-0.2.0.tar.gz` & `tmp/dela-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dela-0.2.0.tar", max compression
+gzip compressed data, was "dela-0.2.1.tar", max compression
```

## Comparing `dela-0.2.0.tar` & `dela-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,13 @@
--rw-r--r--   0        0        0     2496 2023-07-19 11:15:50.660163 dela-0.2.0/README.md
--rw-r--r--   0        0        0      267 2023-07-19 11:15:50.660163 dela-0.2.0/dela/FileReader.py
--rw-r--r--   0        0        0     2153 2023-07-19 11:15:50.660163 dela-0.2.0/dela/ListCommand.py
--rw-r--r--   0        0        0      204 2023-07-19 11:15:50.660163 dela-0.2.0/dela/TagPresentation.py
--rw-r--r--   0        0        0     1893 2023-07-19 11:15:50.660163 dela-0.2.0/dela/TagsCommand.py
--rw-r--r--   0        0        0     1131 2023-07-19 11:15:50.660163 dela-0.2.0/dela/Todo.py
--rw-r--r--   0        0        0      677 2023-07-19 11:15:50.660163 dela-0.2.0/dela/TodoPresentation.py
--rw-r--r--   0        0        0     1439 2023-07-19 11:15:50.660163 dela-0.2.0/dela/TodoRepo.py
--rw-r--r--   0        0        0        0 2023-07-19 11:15:50.660163 dela-0.2.0/dela/__init__.py
--rw-r--r--   0        0        0     2953 2023-07-19 11:15:50.660163 dela-0.2.0/dela/__main__.py
--rw-r--r--   0        0        0      426 2023-07-19 11:15:50.660163 dela-0.2.0/dela/comparators.py
--rw-r--r--   0        0        0      754 2023-07-19 11:15:50.660163 dela-0.2.0/dela/filters.py
--rw-r--r--   0        0        0      187 2023-07-19 11:15:50.660163 dela-0.2.0/dela/logger.py
--rw-r--r--   0        0        0      367 2023-07-19 11:15:50.664162 dela-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3074 1970-01-01 00:00:00.000000 dela-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2496 2023-07-19 11:20:51.344739 dela-0.2.1/README.md
+-rw-r--r--   0        0        0      267 2023-07-19 11:20:51.344739 dela-0.2.1/dela/FileReader.py
+-rw-r--r--   0        0        0     2153 2023-07-19 11:20:51.344739 dela-0.2.1/dela/ListCommand.py
+-rw-r--r--   0        0        0     1131 2023-07-19 11:20:51.344739 dela-0.2.1/dela/Todo.py
+-rw-r--r--   0        0        0      677 2023-07-19 11:20:51.344739 dela-0.2.1/dela/TodoPresentation.py
+-rw-r--r--   0        0        0     1439 2023-07-19 11:20:51.344739 dela-0.2.1/dela/TodoRepo.py
+-rw-r--r--   0        0        0        0 2023-07-19 11:20:51.344739 dela-0.2.1/dela/__init__.py
+-rw-r--r--   0        0        0     2912 2023-07-19 11:20:51.344739 dela-0.2.1/dela/__main__.py
+-rw-r--r--   0        0        0      426 2023-07-19 11:20:51.344739 dela-0.2.1/dela/comparators.py
+-rw-r--r--   0        0        0      754 2023-07-19 11:20:51.344739 dela-0.2.1/dela/filters.py
+-rw-r--r--   0        0        0      187 2023-07-19 11:20:51.344739 dela-0.2.1/dela/logger.py
+-rw-r--r--   0        0        0      367 2023-07-19 11:20:51.348739 dela-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3074 1970-01-01 00:00:00.000000 dela-0.2.1/PKG-INFO
```

### Comparing `dela-0.2.0/README.md` & `dela-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `dela-0.2.0/dela/ListCommand.py` & `dela-0.2.1/dela/ListCommand.py`

 * *Files identical despite different names*

### Comparing `dela-0.2.0/dela/Todo.py` & `dela-0.2.1/dela/Todo.py`

 * *Files identical despite different names*

### Comparing `dela-0.2.0/dela/TodoPresentation.py` & `dela-0.2.1/dela/TodoPresentation.py`

 * *Files identical despite different names*

### Comparing `dela-0.2.0/dela/TodoRepo.py` & `dela-0.2.1/dela/TodoRepo.py`

 * *Files identical despite different names*

### Comparing `dela-0.2.0/dela/__main__.py` & `dela-0.2.1/dela/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #! /bin/python
 import pkg_resources
 from docopt import docopt
-from dela.TagsCommand import TagsCommand
 from dela.ListCommand import ListCommand
 from dela.logger import log
 
 doc = """dela
 
 CLI to list todos in markdown files, like Obsidian Vaults.
```

### Comparing `dela-0.2.0/dela/filters.py` & `dela-0.2.1/dela/filters.py`

 * *Files identical despite different names*

### Comparing `dela-0.2.0/PKG-INFO` & `dela-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dela
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 License: MIT
 Author: 'Anton Shuvalov'
 Author-email: anton@shuvalov.info
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

