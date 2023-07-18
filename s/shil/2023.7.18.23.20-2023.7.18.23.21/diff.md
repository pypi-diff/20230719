# Comparing `tmp/shil-2023.7.18.23.20.tar.gz` & `tmp/shil-2023.7.18.23.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shil-2023.7.18.23.20.tar", last modified: Tue Jul 18 23:20:44 2023, max compression
+gzip compressed data, was "shil-2023.7.18.23.21.tar", last modified: Tue Jul 18 23:21:54 2023, max compression
```

## Comparing `shil-2023.7.18.23.20.tar` & `shil-2023.7.18.23.21.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:20:44.023936 shil-2023.7.18.23.20/
--rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-07-18 23:20:44.023936 shil-2023.7.18.23.20/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-07-18 23:19:13.000000 shil-2023.7.18.23.20/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-18 23:20:44.023936 shil-2023.7.18.23.20/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-18 23:19:13.000000 shil-2023.7.18.23.20/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:20:44.019936 shil-2023.7.18.23.20/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:20:44.019936 shil-2023.7.18.23.20/src/shil/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-18 23:19:13.000000 shil-2023.7.18.23.20/src/shil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-18 23:19:13.000000 shil-2023.7.18.23.20/src/shil/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-18 23:20:39.000000 shil-2023.7.18.23.20/src/shil/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-18 23:19:13.000000 shil-2023.7.18.23.20/src/shil/bin.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-18 23:19:13.000000 shil-2023.7.18.23.20/src/shil/console.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:20:44.023936 shil-2023.7.18.23.20/src/shil/models/
--rw-r--r--   0 runner    (1001) docker     (123)     9259 2023-07-18 23:19:51.000000 shil-2023.7.18.23.20/src/shil/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-18 23:19:13.000000 shil-2023.7.18.23.20/src/shil/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:20:44.023936 shil-2023.7.18.23.20/src/shil/parser/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-18 23:19:13.000000 shil-2023.7.18.23.20/src/shil/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-07-18 23:19:13.000000 shil-2023.7.18.23.20/src/shil/parser/grammar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-07-18 23:19:13.000000 shil-2023.7.18.23.20/src/shil/parser/semantics.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-18 23:19:13.000000 shil-2023.7.18.23.20/src/shil/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:20:44.023936 shil-2023.7.18.23.20/src/shil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-07-18 23:20:44.000000 shil-2023.7.18.23.20/src/shil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-18 23:20:44.000000 shil-2023.7.18.23.20/src/shil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 23:20:44.000000 shil-2023.7.18.23.20/src/shil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 23:20:44.000000 shil-2023.7.18.23.20/src/shil.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-18 23:20:44.000000 shil-2023.7.18.23.20/src/shil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-18 23:20:44.000000 shil-2023.7.18.23.20/src/shil.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:21:54.120150 shil-2023.7.18.23.21/
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-07-18 23:21:54.120150 shil-2023.7.18.23.21/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-07-18 23:20:24.000000 shil-2023.7.18.23.21/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-18 23:21:54.120150 shil-2023.7.18.23.21/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-18 23:20:24.000000 shil-2023.7.18.23.21/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:21:54.108150 shil-2023.7.18.23.21/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:21:54.120150 shil-2023.7.18.23.21/src/shil/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-18 23:20:24.000000 shil-2023.7.18.23.21/src/shil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-18 23:20:24.000000 shil-2023.7.18.23.21/src/shil/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-18 23:21:50.000000 shil-2023.7.18.23.21/src/shil/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-18 23:20:24.000000 shil-2023.7.18.23.21/src/shil/bin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-18 23:20:24.000000 shil-2023.7.18.23.21/src/shil/console.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:21:54.120150 shil-2023.7.18.23.21/src/shil/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     9259 2023-07-18 23:21:01.000000 shil-2023.7.18.23.21/src/shil/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-18 23:20:24.000000 shil-2023.7.18.23.21/src/shil/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:21:54.120150 shil-2023.7.18.23.21/src/shil/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-18 23:20:24.000000 shil-2023.7.18.23.21/src/shil/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-07-18 23:20:24.000000 shil-2023.7.18.23.21/src/shil/parser/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-07-18 23:20:24.000000 shil-2023.7.18.23.21/src/shil/parser/semantics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-18 23:20:24.000000 shil-2023.7.18.23.21/src/shil/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:21:54.120150 shil-2023.7.18.23.21/src/shil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-07-18 23:21:54.000000 shil-2023.7.18.23.21/src/shil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-18 23:21:54.000000 shil-2023.7.18.23.21/src/shil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 23:21:54.000000 shil-2023.7.18.23.21/src/shil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 23:21:54.000000 shil-2023.7.18.23.21/src/shil.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-18 23:21:54.000000 shil-2023.7.18.23.21/src/shil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-18 23:21:54.000000 shil-2023.7.18.23.21/src/shil.egg-info/top_level.txt
```

### Comparing `shil-2023.7.18.23.20/PKG-INFO` & `shil-2023.7.18.23.21/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shil
-Version: 2023.7.18.23.20
+Version: 2023.7.18.23.21
 Summary: Shell helper utilities for python
 Home-page: https://github.com/elo-enterprises/shil/
 Author: elo
 License: MIT
 Project-URL: Documentation, https://github.com/elo-enterprises/shil/
 Project-URL: Source, https://github.com/elo-enterprises/shil/
 Project-URL: Download, https://github.com/elo-enterprises/shil/#files
@@ -27,15 +27,15 @@
     </td>
   </tr>
   <tr>
     <td width=15%><img src=img/icon.png style="width:150px"></td>
     <td>
       Shell-util library for python.  Includes helpers for subprocess invocation, shell-formatters / pretty-printers, and more.
       <br/><br/>
-      <a href=https://pypi.python.org/pypi/shil/><img src=""https://img.shields.io/pypi/l/shil.svg"></a>
+      <a href=https://pypi.python.org/pypi/shil/><img src="https://img.shields.io/pypi/l/shil.svg"></a>
       <a href="https://github.com/elo-enterprises/shil/actions/workflows/python-test.yml"><img src="https://github.com/elo-enterprises/shil/actions/workflows/python-test.yml/badge.svg"></a>
     </td>
   </tr>
 </table>
 
 ---------------------------------------------------------------------------------
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: shil Version: 2023.7.18.23.20 Summary: Shell helper
+Metadata-Version: 2.1 Name: shil Version: 2023.7.18.23.21 Summary: Shell helper
 utilities for python Home-page: https://github.com/elo-enterprises/shil/
 Author: elo License: MIT Project-URL: Documentation, https://github.com/elo-
 enterprises/shil/ Project-URL: Source, https://github.com/elo-enterprises/shil/
 Project-URL: Download, https://github.com/elo-enterprises/shil/#files Platform:
 any Classifier: Programming Language :: Python Requires-Python: >3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM Provides-
 Extra: dev Provides-Extra: testing Provides-Extra: lint Provides-Extra: publish
 shil    
                Shell-util library for python. Includes helpers for subprocess
                invocation, shell-formatters / pretty-printers, and more.
 [img/icon.png]
-               img.shields.io/pypi/l/shil.svg">
-                [https://github.com/elo-enterprises/shil/actions/workflows/
-               python-test.yml/badge.svg]
+               [https://img.shields.io/pypi/l/shil.svg] [https://github.com/
+               elo-enterprises/shil/actions/workflows/python-test.yml/
+               badge.svg]
 -------------------------------------------------------------------------------
 -- * [Overview](#overview) * [Features](#features) * [Installation]
 (#installation) * [Usage](#usage) * [OOP-style Dispatch](#oop-style-dispatch) *
 [Functional approach to dispatch](#functional-approach-to-dispatch) * [Loading
 data when command-output is JSON](#loading-data-when-command-output-is-json) *
 [Serialization with Pydantic](#serialization-with-pydantic) * [Caller
 determines logging](#caller-determines-logging) * [Rich-console Support](#rich-
```

### Comparing `shil-2023.7.18.23.20/README.md` & `shil-2023.7.18.23.21/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     </td>
   </tr>
   <tr>
     <td width=15%><img src=img/icon.png style="width:150px"></td>
     <td>
       Shell-util library for python.  Includes helpers for subprocess invocation, shell-formatters / pretty-printers, and more.
       <br/><br/>
-      <a href=https://pypi.python.org/pypi/shil/><img src=""https://img.shields.io/pypi/l/shil.svg"></a>
+      <a href=https://pypi.python.org/pypi/shil/><img src="https://img.shields.io/pypi/l/shil.svg"></a>
       <a href="https://github.com/elo-enterprises/shil/actions/workflows/python-test.yml"><img src="https://github.com/elo-enterprises/shil/actions/workflows/python-test.yml/badge.svg"></a>
     </td>
   </tr>
 </table>
 
 ---------------------------------------------------------------------------------
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 shil    
                Shell-util library for python. Includes helpers for subprocess
                invocation, shell-formatters / pretty-printers, and more.
 [img/icon.png]
-               img.shields.io/pypi/l/shil.svg">
-                [https://github.com/elo-enterprises/shil/actions/workflows/
-               python-test.yml/badge.svg]
+               [https://img.shields.io/pypi/l/shil.svg] [https://github.com/
+               elo-enterprises/shil/actions/workflows/python-test.yml/
+               badge.svg]
 -------------------------------------------------------------------------------
 -- * [Overview](#overview) * [Features](#features) * [Installation]
 (#installation) * [Usage](#usage) * [OOP-style Dispatch](#oop-style-dispatch) *
 [Functional approach to dispatch](#functional-approach-to-dispatch) * [Loading
 data when command-output is JSON](#loading-data-when-command-output-is-json) *
 [Serialization with Pydantic](#serialization-with-pydantic) * [Caller
 determines logging](#caller-determines-logging) * [Rich-console Support](#rich-
```

### Comparing `shil-2023.7.18.23.20/setup.cfg` & `shil-2023.7.18.23.21/setup.cfg`

 * *Files identical despite different names*

### Comparing `shil-2023.7.18.23.20/setup.py` & `shil-2023.7.18.23.21/setup.py`

 * *Files identical despite different names*

### Comparing `shil-2023.7.18.23.20/src/shil/__main__.py` & `shil-2023.7.18.23.21/src/shil/__main__.py`

 * *Files identical despite different names*

### Comparing `shil-2023.7.18.23.20/src/shil/models/__init__.py` & `shil-2023.7.18.23.21/src/shil/models/__init__.py`

 * *Files identical despite different names*

### Comparing `shil-2023.7.18.23.20/src/shil/parser/__init__.py` & `shil-2023.7.18.23.21/src/shil/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `shil-2023.7.18.23.20/src/shil/parser/grammar.py` & `shil-2023.7.18.23.21/src/shil/parser/grammar.py`

 * *Files identical despite different names*

### Comparing `shil-2023.7.18.23.20/src/shil/parser/semantics.py` & `shil-2023.7.18.23.21/src/shil/parser/semantics.py`

 * *Files identical despite different names*

### Comparing `shil-2023.7.18.23.20/src/shil/util.py` & `shil-2023.7.18.23.21/src/shil/util.py`

 * *Files identical despite different names*

### Comparing `shil-2023.7.18.23.20/src/shil.egg-info/PKG-INFO` & `shil-2023.7.18.23.21/src/shil.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shil
-Version: 2023.7.18.23.20
+Version: 2023.7.18.23.21
 Summary: Shell helper utilities for python
 Home-page: https://github.com/elo-enterprises/shil/
 Author: elo
 License: MIT
 Project-URL: Documentation, https://github.com/elo-enterprises/shil/
 Project-URL: Source, https://github.com/elo-enterprises/shil/
 Project-URL: Download, https://github.com/elo-enterprises/shil/#files
@@ -27,15 +27,15 @@
     </td>
   </tr>
   <tr>
     <td width=15%><img src=img/icon.png style="width:150px"></td>
     <td>
       Shell-util library for python.  Includes helpers for subprocess invocation, shell-formatters / pretty-printers, and more.
       <br/><br/>
-      <a href=https://pypi.python.org/pypi/shil/><img src=""https://img.shields.io/pypi/l/shil.svg"></a>
+      <a href=https://pypi.python.org/pypi/shil/><img src="https://img.shields.io/pypi/l/shil.svg"></a>
       <a href="https://github.com/elo-enterprises/shil/actions/workflows/python-test.yml"><img src="https://github.com/elo-enterprises/shil/actions/workflows/python-test.yml/badge.svg"></a>
     </td>
   </tr>
 </table>
 
 ---------------------------------------------------------------------------------
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: shil Version: 2023.7.18.23.20 Summary: Shell helper
+Metadata-Version: 2.1 Name: shil Version: 2023.7.18.23.21 Summary: Shell helper
 utilities for python Home-page: https://github.com/elo-enterprises/shil/
 Author: elo License: MIT Project-URL: Documentation, https://github.com/elo-
 enterprises/shil/ Project-URL: Source, https://github.com/elo-enterprises/shil/
 Project-URL: Download, https://github.com/elo-enterprises/shil/#files Platform:
 any Classifier: Programming Language :: Python Requires-Python: >3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM Provides-
 Extra: dev Provides-Extra: testing Provides-Extra: lint Provides-Extra: publish
 shil    
                Shell-util library for python. Includes helpers for subprocess
                invocation, shell-formatters / pretty-printers, and more.
 [img/icon.png]
-               img.shields.io/pypi/l/shil.svg">
-                [https://github.com/elo-enterprises/shil/actions/workflows/
-               python-test.yml/badge.svg]
+               [https://img.shields.io/pypi/l/shil.svg] [https://github.com/
+               elo-enterprises/shil/actions/workflows/python-test.yml/
+               badge.svg]
 -------------------------------------------------------------------------------
 -- * [Overview](#overview) * [Features](#features) * [Installation]
 (#installation) * [Usage](#usage) * [OOP-style Dispatch](#oop-style-dispatch) *
 [Functional approach to dispatch](#functional-approach-to-dispatch) * [Loading
 data when command-output is JSON](#loading-data-when-command-output-is-json) *
 [Serialization with Pydantic](#serialization-with-pydantic) * [Caller
 determines logging](#caller-determines-logging) * [Rich-console Support](#rich-
```

