# Comparing `tmp/py3seed-0.1.8.tar.gz` & `tmp/py3seed-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3seed-0.1.8.tar", last modified: Tue Jul 18 07:52:50 2023, max compression
+gzip compressed data, was "py3seed-0.1.9.tar", last modified: Wed Jul 19 07:42:07 2023, max compression
```

## Comparing `py3seed-0.1.8.tar` & `py3seed-0.1.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-18 07:52:50.279227 py3seed-0.1.8/
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1072 2021-08-08 16:29:42.000000 py3seed-0.1.8/LICENSE
--rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-07-18 07:52:50.279456 py3seed-0.1.8/PKG-INFO
--rw-r--r--   0 weiminfeng   (501) staff       (20)      288 2021-08-11 03:57:41.000000 py3seed-0.1.8/README.md
--rw-r--r--   0 weiminfeng   (501) staff       (20)      104 2021-09-18 08:01:25.000000 py3seed-0.1.8/pyproject.toml
--rw-r--r--   0 weiminfeng   (501) staff       (20)      911 2023-07-18 07:52:50.281220 py3seed-0.1.8/setup.cfg
--rw-r--r--   0 weiminfeng   (501) staff       (20)      214 2023-07-06 08:35:28.000000 py3seed-0.1.8/setup.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-18 07:52:50.250388 py3seed-0.1.8/src/
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-18 07:52:50.266260 py3seed-0.1.8/src/py3seed/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      743 2023-07-10 07:31:29.000000 py3seed-0.1.8/src/py3seed/__init__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1624 2023-07-10 03:47:01.000000 py3seed-0.1.8/src/py3seed/__main__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)      992 2021-09-02 08:44:38.000000 py3seed-0.1.8/src/py3seed/admin.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     6458 2023-07-10 03:55:28.000000 py3seed-0.1.8/src/py3seed/cachesupport.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-18 07:52:50.273629 py3seed-0.1.8/src/py3seed/commands/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      151 2021-09-01 02:10:05.000000 py3seed-0.1.8/src/py3seed/commands/__init__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    20437 2023-07-17 08:12:35.000000 py3seed-0.1.8/src/py3seed/commands/gen.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)      732 2023-06-27 01:48:25.000000 py3seed-0.1.8/src/py3seed/error.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    11554 2023-07-10 03:49:24.000000 py3seed-0.1.8/src/py3seed/inflection.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1166 2022-05-06 11:35:05.000000 py3seed-0.1.8/src/py3seed/log.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    17725 2023-07-11 02:10:39.000000 py3seed-0.1.8/src/py3seed/merge3.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    57700 2023-07-18 01:28:13.000000 py3seed-0.1.8/src/py3seed/model.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14489 2023-07-10 03:55:58.000000 py3seed-0.1.8/src/py3seed/mongosupport.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14678 2023-07-18 07:52:08.000000 py3seed-0.1.8/src/py3seed/utils.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     7471 2023-07-10 03:54:22.000000 py3seed-0.1.8/src/py3seed/websupport.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-18 07:52:50.270811 py3seed-0.1.8/src/py3seed.egg-info/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-07-18 07:52:50.000000 py3seed-0.1.8/src/py3seed.egg-info/PKG-INFO
--rw-r--r--   0 weiminfeng   (501) staff       (20)      718 2023-07-18 07:52:50.000000 py3seed-0.1.8/src/py3seed.egg-info/SOURCES.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)        1 2023-07-18 07:52:50.000000 py3seed-0.1.8/src/py3seed.egg-info/dependency_links.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)      111 2023-07-18 07:52:50.000000 py3seed-0.1.8/src/py3seed.egg-info/entry_points.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)       48 2023-07-18 07:52:50.000000 py3seed-0.1.8/src/py3seed.egg-info/requires.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)        8 2023-07-18 07:52:50.000000 py3seed-0.1.8/src/py3seed.egg-info/top_level.txt
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-18 07:52:50.278638 py3seed-0.1.8/tests/
--rw-r--r--   0 weiminfeng   (501) staff       (20)     3216 2022-12-09 02:58:18.000000 py3seed-0.1.8/tests/test_cachesupport.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     6599 2023-07-18 07:07:02.000000 py3seed-0.1.8/tests/test_gen.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14977 2023-07-10 03:39:53.000000 py3seed-0.1.8/tests/test_merge3.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     5116 2023-07-05 06:36:00.000000 py3seed-0.1.8/tests/test_model.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     2083 2023-07-05 06:36:25.000000 py3seed-0.1.8/tests/test_mongosupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-19 07:42:07.906938 py3seed-0.1.9/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1072 2021-08-08 16:29:42.000000 py3seed-0.1.9/LICENSE
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-07-19 07:42:07.907084 py3seed-0.1.9/PKG-INFO
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      288 2021-08-11 03:57:41.000000 py3seed-0.1.9/README.md
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      104 2021-09-18 08:01:25.000000 py3seed-0.1.9/pyproject.toml
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      911 2023-07-19 07:42:07.907738 py3seed-0.1.9/setup.cfg
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      214 2023-07-06 08:35:28.000000 py3seed-0.1.9/setup.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-19 07:42:07.883900 py3seed-0.1.9/src/
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-19 07:42:07.898965 py3seed-0.1.9/src/py3seed/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      743 2023-07-10 07:31:29.000000 py3seed-0.1.9/src/py3seed/__init__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1624 2023-07-10 03:47:01.000000 py3seed-0.1.9/src/py3seed/__main__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      992 2021-09-02 08:44:38.000000 py3seed-0.1.9/src/py3seed/admin.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     6458 2023-07-10 03:55:28.000000 py3seed-0.1.9/src/py3seed/cachesupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-19 07:42:07.902297 py3seed-0.1.9/src/py3seed/commands/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      151 2021-09-01 02:10:05.000000 py3seed-0.1.9/src/py3seed/commands/__init__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    21148 2023-07-19 07:41:26.000000 py3seed-0.1.9/src/py3seed/commands/gen.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      732 2023-06-27 01:48:25.000000 py3seed-0.1.9/src/py3seed/error.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    11554 2023-07-10 03:49:24.000000 py3seed-0.1.9/src/py3seed/inflection.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1166 2022-05-06 11:35:05.000000 py3seed-0.1.9/src/py3seed/log.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    17725 2023-07-11 02:10:39.000000 py3seed-0.1.9/src/py3seed/merge3.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    57700 2023-07-18 01:28:13.000000 py3seed-0.1.9/src/py3seed/model.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14489 2023-07-10 03:55:58.000000 py3seed-0.1.9/src/py3seed/mongosupport.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14673 2023-07-19 03:29:37.000000 py3seed-0.1.9/src/py3seed/utils.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     7471 2023-07-10 03:54:22.000000 py3seed-0.1.9/src/py3seed/websupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-19 07:42:07.901363 py3seed-0.1.9/src/py3seed.egg-info/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-07-19 07:42:07.000000 py3seed-0.1.9/src/py3seed.egg-info/PKG-INFO
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      718 2023-07-19 07:42:07.000000 py3seed-0.1.9/src/py3seed.egg-info/SOURCES.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)        1 2023-07-19 07:42:07.000000 py3seed-0.1.9/src/py3seed.egg-info/dependency_links.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      111 2023-07-19 07:42:07.000000 py3seed-0.1.9/src/py3seed.egg-info/entry_points.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)       48 2023-07-19 07:42:07.000000 py3seed-0.1.9/src/py3seed.egg-info/requires.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)        8 2023-07-19 07:42:07.000000 py3seed-0.1.9/src/py3seed.egg-info/top_level.txt
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-19 07:42:07.906371 py3seed-0.1.9/tests/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     3216 2022-12-09 02:58:18.000000 py3seed-0.1.9/tests/test_cachesupport.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     6599 2023-07-18 07:07:02.000000 py3seed-0.1.9/tests/test_gen.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14977 2023-07-10 03:39:53.000000 py3seed-0.1.9/tests/test_merge3.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     5116 2023-07-05 06:36:00.000000 py3seed-0.1.9/tests/test_model.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     2083 2023-07-05 06:36:25.000000 py3seed-0.1.9/tests/test_mongosupport.py
```

### Comparing `py3seed-0.1.8/LICENSE` & `py3seed-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.8/PKG-INFO` & `py3seed-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3seed
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package that bootstraps your project by simple data models definition and auto api and user interface generation
 Home-page: https://github.com/okosioc/pyseed
 Author: Samuel Feng
 Author-email: okosioc@gmail.com
 Project-URL: Bug Tracker, https://github.com/okosioc/pyseed/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py3seed-0.1.8/setup.cfg` & `py3seed-0.1.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = py3seed
-version = 0.1.8
+version = 0.1.9
 author = Samuel Feng
 author_email = okosioc@gmail.com
 description = A package that bootstraps your project by simple data models definition and auto api and user interface generation
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/okosioc/pyseed
 project_urls =
```

### Comparing `py3seed-0.1.8/src/py3seed/__init__.py` & `py3seed-0.1.9/src/py3seed/__init__.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.8/src/py3seed/__main__.py` & `py3seed-0.1.9/src/py3seed/__main__.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.8/src/py3seed/admin.py` & `py3seed-0.1.9/src/py3seed/admin.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.8/src/py3seed/cachesupport.py` & `py3seed-0.1.9/src/py3seed/cachesupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.8/src/py3seed/commands/gen.py` & `py3seed-0.1.9/src/py3seed/commands/gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,33 +15,38 @@
 import os
 import re
 import shutil
 import sys
 from typing import List
 
 from flask import request
-from jinja2 import Environment, TemplateSyntaxError, FileSystemLoader
+from jinja2 import Environment, TemplateSyntaxError, FileSystemLoader, filters
 from werkzeug.urls import url_quote, url_encode
 
 from py3seed import registered_models, BaseModel, TemplateError, LayoutError
 from py3seed.utils import work_in, generate_names, get_layout_fields, parse_layout
 from py3seed.merge3 import Merge3
 
 logger = logging.getLogger('pyseed')
 
 
 def _prepare_jinja2_env():
     """ Prepare env for rendering jinja2 templates. """
     #
     # For more env setting, please refer to https://jinja.palletsprojects.com/en/3.0.x/api/#jinja2.Environment
-    #   trim_blocks=True, the first newline after a block is removed (block, not variable tag!)
-    #   lstrip_blocks=True, leading spaces and tabs are stripped from the start of a line to a block
-    #   keep_trailing_newline=True, Preserve the trailing newline when rendering templates.
+    # - trim_blocks=True, the first newline after a block is removed (block, not variable tag!)
+    # - lstrip_blocks=True, leading spaces and tabs are stripped from the start of a line to a block
+    # - keep_trailing_newline=True, Preserve the trailing newline when rendering templates
     #
-    env = Environment(trim_blocks=True, lstrip_blocks=True, keep_trailing_newline=True)
+    # trim_blocks=True and lstrip_blocks=True -> make sure lines of {% ... %} and {# ... #} will be removed completely in render result
+    # keep_trailing_newline=True -> keep trailing newline to so that you can use indent filter to include the macro with a tailing newline
+    #
+    # For extension, plrease refer to https://jinja.palletsprojects.com/en/3.0.x/extensions/#loopcontrols-extension
+    #
+    env = Environment(trim_blocks=True, lstrip_blocks=True, keep_trailing_newline=True, extensions=['jinja2.ext.loopcontrols'])
 
     def split(value, separator):
         """ Split a string. """
         return value.split(separator)
 
     def items(value):
         """ Return items of a dict. """
@@ -62,20 +67,29 @@
         """ Return file name from a path. """
         return os.path.basename(value)
 
     def urlquote(value, charset='utf-8'):
         """ Url Quote. """
         return url_quote(value, charset)
 
+    def right(s: str, width: int = 4):
+        """ Do indent, if content is not blank, add leading indent"""
+        s = filters.do_indent(s, width)
+        if not s:
+            s = " " * width + s
+        #
+        return s
+
     env.filters['split'] = split
     env.filters['items'] = items
     env.filters['keys'] = keys
     env.filters['quote'] = quote
     env.filters['basename'] = basename
     env.filters['urlquote'] = urlquote
+    env.filters['right'] = right
 
     def update_query(**new_values):
         """ Update query. """
         args = request.args.copy()
         for key, value in new_values.items():
             args[key] = value
         return url_encode(args)
```

### Comparing `py3seed-0.1.8/src/py3seed/error.py` & `py3seed-0.1.9/src/py3seed/error.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.8/src/py3seed/inflection.py` & `py3seed-0.1.9/src/py3seed/inflection.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.8/src/py3seed/log.py` & `py3seed-0.1.9/src/py3seed/log.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.8/src/py3seed/merge3.py` & `py3seed-0.1.9/src/py3seed/merge3.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.8/src/py3seed/model.py` & `py3seed-0.1.9/src/py3seed/model.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.8/src/py3seed/mongosupport.py` & `py3seed-0.1.9/src/py3seed/mongosupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.8/src/py3seed/utils.py` & `py3seed-0.1.9/src/py3seed/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
             {name: 0, rows:[...]},
         ]]
     }
     """
 
     def _parse_lines(level, _lines, _schema):
         """ Recursively parse lines. """
-        leading = '-' * ((level + 1) * 2)  # 2 spaces for each level
+        leading = '- ' * (level + 1)  # 2 spaces for each level
         # logger.debug('Parse lines:\n' + '\n'.join(_lines))
         _rows = []
         # Get the indexes of lines that has same indent with first line
         first_line = _lines[0]
         first_indent = len(first_line) - len(first_line.lstrip())
         indexes = []
         for index in range(len(_lines)):
```

### Comparing `py3seed-0.1.8/src/py3seed/websupport.py` & `py3seed-0.1.9/src/py3seed/websupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.8/src/py3seed.egg-info/PKG-INFO` & `py3seed-0.1.9/src/py3seed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3seed
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package that bootstraps your project by simple data models definition and auto api and user interface generation
 Home-page: https://github.com/okosioc/pyseed
 Author: Samuel Feng
 Author-email: okosioc@gmail.com
 Project-URL: Bug Tracker, https://github.com/okosioc/pyseed/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py3seed-0.1.8/src/py3seed.egg-info/SOURCES.txt` & `py3seed-0.1.9/src/py3seed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.8/tests/test_cachesupport.py` & `py3seed-0.1.9/tests/test_cachesupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.8/tests/test_gen.py` & `py3seed-0.1.9/tests/test_gen.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.8/tests/test_merge3.py` & `py3seed-0.1.9/tests/test_merge3.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.8/tests/test_model.py` & `py3seed-0.1.9/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.8/tests/test_mongosupport.py` & `py3seed-0.1.9/tests/test_mongosupport.py`

 * *Files identical despite different names*

