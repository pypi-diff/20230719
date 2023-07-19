# Comparing `tmp/edman_web-2023.7.19.tar.gz` & `tmp/edman_web-2023.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edman_web-2023.7.19.tar", last modified: Wed Jul 19 02:33:02 2023, max compression
+gzip compressed data, was "edman_web-2023.7.6.tar", last modified: Thu Jul  6 02:03:21 2023, max compression
```

## Comparing `edman_web-2023.7.19.tar` & `edman_web-2023.7.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-07-19 02:33:02.286961 edman_web-2023.7.19/
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1115 2023-03-29 09:20:48.000000 edman_web-2023.7.19/LICENSE.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2391 2023-07-19 02:33:02.286961 edman_web-2023.7.19/PKG-INFO
--rw-r--r--   0 ohno      (1000) ohno      (1000)      693 2023-07-19 02:31:04.000000 edman_web-2023.7.19/README.rst
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-07-19 02:33:02.276961 edman_web-2023.7.19/edman_web/
--rw-r--r--   0 ohno      (1000) ohno      (1000)       82 2023-05-24 06:10:37.000000 edman_web-2023.7.19/edman_web/__init__.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     8325 2023-07-06 02:00:09.000000 edman_web-2023.7.19/edman_web/file_manager.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)        0 2023-05-23 00:36:23.000000 edman_web-2023.7.19/edman_web/py.typed
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2643 2023-05-24 06:10:37.000000 edman_web-2023.7.19/edman_web/search_manager.py
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-07-19 02:33:02.286961 edman_web-2023.7.19/edman_web.egg-info/
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2391 2023-07-19 02:33:02.000000 edman_web-2023.7.19/edman_web.egg-info/PKG-INFO
--rw-r--r--   0 ohno      (1000) ohno      (1000)      636 2023-07-19 02:33:02.000000 edman_web-2023.7.19/edman_web.egg-info/SOURCES.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)        1 2023-07-19 02:33:02.000000 edman_web-2023.7.19/edman_web.egg-info/dependency_links.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)       63 2023-07-19 02:33:02.000000 edman_web-2023.7.19/edman_web.egg-info/requires.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)       32 2023-07-19 02:33:02.000000 edman_web-2023.7.19/edman_web.egg-info/top_level.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1007 2023-07-19 02:31:04.000000 edman_web-2023.7.19/pyproject.toml
--rw-r--r--   0 ohno      (1000) ohno      (1000)       38 2023-07-19 02:33:02.286961 edman_web-2023.7.19/setup.cfg
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-07-19 02:33:02.286961 edman_web-2023.7.19/tests/
--rw-r--r--   0 ohno      (1000) ohno      (1000)    15482 2023-07-06 02:00:09.000000 edman_web-2023.7.19/tests/test_file_manager.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     5151 2023-05-24 06:10:37.000000 edman_web-2023.7.19/tests/test_search_manager.py
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-07-19 02:33:02.276961 edman_web-2023.7.19/venv/
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-07-19 02:33:02.286961 edman_web-2023.7.19/venv/bin/
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1729 2023-04-07 00:43:44.000000 edman_web-2023.7.19/venv/bin/jp.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      636 2023-05-18 00:15:38.000000 edman_web-2023.7.19/venv/bin/rst2html.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      758 2023-05-18 00:15:38.000000 edman_web-2023.7.19/venv/bin/rst2html4.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1093 2023-05-18 00:15:38.000000 edman_web-2023.7.19/venv/bin/rst2html5.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      835 2023-05-18 00:15:38.000000 edman_web-2023.7.19/venv/bin/rst2latex.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      658 2023-05-18 00:15:38.000000 edman_web-2023.7.19/venv/bin/rst2man.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      824 2023-05-18 00:15:38.000000 edman_web-2023.7.19/venv/bin/rst2odt.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      630 2023-05-18 00:15:38.000000 edman_web-2023.7.19/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      643 2023-05-18 00:15:38.000000 edman_web-2023.7.19/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      679 2023-05-18 00:15:38.000000 edman_web-2023.7.19/venv/bin/rst2s5.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      915 2023-05-18 00:15:38.000000 edman_web-2023.7.19/venv/bin/rst2xetex.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      644 2023-05-18 00:15:38.000000 edman_web-2023.7.19/venv/bin/rst2xml.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      712 2023-05-18 00:15:38.000000 edman_web-2023.7.19/venv/bin/rstpep2html.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-07-06 02:03:21.041667 edman_web-2023.7.6/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1115 2023-03-29 09:20:48.000000 edman_web-2023.7.6/LICENSE.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2327 2023-07-06 02:03:21.041667 edman_web-2023.7.6/PKG-INFO
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      626 2023-03-30 03:11:16.000000 edman_web-2023.7.6/README.rst
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-07-06 02:03:21.041667 edman_web-2023.7.6/edman_web/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       82 2023-05-24 06:10:37.000000 edman_web-2023.7.6/edman_web/__init__.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     8325 2023-07-06 02:00:09.000000 edman_web-2023.7.6/edman_web/file_manager.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)        0 2023-05-23 00:36:23.000000 edman_web-2023.7.6/edman_web/py.typed
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2643 2023-05-24 06:10:37.000000 edman_web-2023.7.6/edman_web/search_manager.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-07-06 02:03:21.041667 edman_web-2023.7.6/edman_web.egg-info/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2327 2023-07-06 02:03:21.000000 edman_web-2023.7.6/edman_web.egg-info/PKG-INFO
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      636 2023-07-06 02:03:21.000000 edman_web-2023.7.6/edman_web.egg-info/SOURCES.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)        1 2023-07-06 02:03:21.000000 edman_web-2023.7.6/edman_web.egg-info/dependency_links.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       62 2023-07-06 02:03:21.000000 edman_web-2023.7.6/edman_web.egg-info/requires.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       32 2023-07-06 02:03:21.000000 edman_web-2023.7.6/edman_web.egg-info/top_level.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1005 2023-07-06 02:00:09.000000 edman_web-2023.7.6/pyproject.toml
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       38 2023-07-06 02:03:21.041667 edman_web-2023.7.6/setup.cfg
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-07-06 02:03:21.041667 edman_web-2023.7.6/tests/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    15482 2023-07-06 02:00:09.000000 edman_web-2023.7.6/tests/test_file_manager.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     5151 2023-05-24 06:10:37.000000 edman_web-2023.7.6/tests/test_search_manager.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-07-06 02:03:21.031667 edman_web-2023.7.6/venv/
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-07-06 02:03:21.041667 edman_web-2023.7.6/venv/bin/
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1729 2023-04-07 00:43:44.000000 edman_web-2023.7.6/venv/bin/jp.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      636 2023-05-18 00:15:38.000000 edman_web-2023.7.6/venv/bin/rst2html.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      758 2023-05-18 00:15:38.000000 edman_web-2023.7.6/venv/bin/rst2html4.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1093 2023-05-18 00:15:38.000000 edman_web-2023.7.6/venv/bin/rst2html5.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      835 2023-05-18 00:15:38.000000 edman_web-2023.7.6/venv/bin/rst2latex.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      658 2023-05-18 00:15:38.000000 edman_web-2023.7.6/venv/bin/rst2man.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      824 2023-05-18 00:15:38.000000 edman_web-2023.7.6/venv/bin/rst2odt.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      630 2023-05-18 00:15:38.000000 edman_web-2023.7.6/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      643 2023-05-18 00:15:38.000000 edman_web-2023.7.6/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      679 2023-05-18 00:15:38.000000 edman_web-2023.7.6/venv/bin/rst2s5.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      915 2023-05-18 00:15:38.000000 edman_web-2023.7.6/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      644 2023-05-18 00:15:38.000000 edman_web-2023.7.6/venv/bin/rst2xml.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      712 2023-05-18 00:15:38.000000 edman_web-2023.7.6/venv/bin/rstpep2html.py
```

### Comparing `edman_web-2023.7.19/LICENSE.txt` & `edman_web-2023.7.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edman_web-2023.7.19/PKG-INFO` & `edman_web-2023.7.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edman_web
-Version: 2023.7.19
+Version: 2023.7.6
 Summary: Sub-package of edman for web applications.
 Author-email: Masaki Ohno <masakio@post.kek.jp>
 License: MIT License
         
         Copyright (c) 2019-2023 KEK IMSS SBRC/PF, Masaki Ohno, Yusuke Yamada
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -52,18 +52,14 @@
 
  pip install edman_web
 
 Licence
 -------
 MIT
 
-PyPI Project
-------------
-https://pypi.org/project/edman_web/
-
 API Document
 ------------
 https://ryde.github.io/edman_web/
 
 Author
 ------
```

### Comparing `edman_web-2023.7.19/edman_web/file_manager.py` & `edman_web-2023.7.6/edman_web/file_manager.py`

 * *Files identical despite different names*

### Comparing `edman_web-2023.7.19/edman_web/search_manager.py` & `edman_web-2023.7.6/edman_web/search_manager.py`

 * *Files identical despite different names*

### Comparing `edman_web-2023.7.19/edman_web.egg-info/PKG-INFO` & `edman_web-2023.7.6/edman_web.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edman-web
-Version: 2023.7.19
+Version: 2023.7.6
 Summary: Sub-package of edman for web applications.
 Author-email: Masaki Ohno <masakio@post.kek.jp>
 License: MIT License
         
         Copyright (c) 2019-2023 KEK IMSS SBRC/PF, Masaki Ohno, Yusuke Yamada
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -52,18 +52,14 @@
 
  pip install edman_web
 
 Licence
 -------
 MIT
 
-PyPI Project
-------------
-https://pypi.org/project/edman_web/
-
 API Document
 ------------
 https://ryde.github.io/edman_web/
 
 Author
 ------
```

### Comparing `edman_web-2023.7.19/edman_web.egg-info/SOURCES.txt` & `edman_web-2023.7.6/edman_web.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edman_web-2023.7.19/pyproject.toml` & `edman_web-2023.7.6/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
     "Topic :: Database :: Front-Ends",
 ]
 dependencies = [
-    "pymongo~=4.4.1",
-    "edman~=2023.7.19",
+    "pymongo~=4.4.0",
+    "edman~=2023.7.4",
     "Werkzeug~=2.3.6",
     "Pillow~=10.0.0"
 ]
-version = "2023.7.19"
+version = "2023.7.6"
 
 [project.urls]
 "documentation" = "https://ryde.github.io/edman_web/"
 "repository" = "https://github.com/ryde/edman_web"
 
 [tool.setuptools.packages.find]
 exclude = ["tests"]
```

### Comparing `edman_web-2023.7.19/tests/test_file_manager.py` & `edman_web-2023.7.6/tests/test_file_manager.py`

 * *Files identical despite different names*

### Comparing `edman_web-2023.7.19/tests/test_search_manager.py` & `edman_web-2023.7.6/tests/test_search_manager.py`

 * *Files identical despite different names*

### Comparing `edman_web-2023.7.19/venv/bin/jp.py` & `edman_web-2023.7.6/venv/bin/jp.py`

 * *Files identical despite different names*

### Comparing `edman_web-2023.7.19/venv/bin/rst2html.py` & `edman_web-2023.7.6/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `edman_web-2023.7.19/venv/bin/rst2html4.py` & `edman_web-2023.7.6/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `edman_web-2023.7.19/venv/bin/rst2html5.py` & `edman_web-2023.7.6/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `edman_web-2023.7.19/venv/bin/rst2latex.py` & `edman_web-2023.7.6/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `edman_web-2023.7.19/venv/bin/rst2man.py` & `edman_web-2023.7.6/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `edman_web-2023.7.19/venv/bin/rst2odt.py` & `edman_web-2023.7.6/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `edman_web-2023.7.19/venv/bin/rst2odt_prepstyles.py` & `edman_web-2023.7.6/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `edman_web-2023.7.19/venv/bin/rst2pseudoxml.py` & `edman_web-2023.7.6/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `edman_web-2023.7.19/venv/bin/rst2s5.py` & `edman_web-2023.7.6/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `edman_web-2023.7.19/venv/bin/rst2xetex.py` & `edman_web-2023.7.6/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `edman_web-2023.7.19/venv/bin/rst2xml.py` & `edman_web-2023.7.6/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `edman_web-2023.7.19/venv/bin/rstpep2html.py` & `edman_web-2023.7.6/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

