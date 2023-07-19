# Comparing `tmp/py3seed-0.2.0.tar.gz` & `tmp/py3seed-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3seed-0.2.0.tar", last modified: Wed Jul 19 07:46:14 2023, max compression
+gzip compressed data, was "py3seed-0.2.1.tar", last modified: Wed Jul 19 07:50:45 2023, max compression
```

## Comparing `py3seed-0.2.0.tar` & `py3seed-0.2.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-19 07:46:14.220773 py3seed-0.2.0/
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1072 2021-08-08 16:29:42.000000 py3seed-0.2.0/LICENSE
--rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-07-19 07:46:14.220925 py3seed-0.2.0/PKG-INFO
--rw-r--r--   0 weiminfeng   (501) staff       (20)      288 2021-08-11 03:57:41.000000 py3seed-0.2.0/README.md
--rw-r--r--   0 weiminfeng   (501) staff       (20)      104 2021-09-18 08:01:25.000000 py3seed-0.2.0/pyproject.toml
--rw-r--r--   0 weiminfeng   (501) staff       (20)      911 2023-07-19 07:46:14.221608 py3seed-0.2.0/setup.cfg
--rw-r--r--   0 weiminfeng   (501) staff       (20)      214 2023-07-06 08:35:28.000000 py3seed-0.2.0/setup.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-19 07:46:14.193815 py3seed-0.2.0/src/
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-19 07:46:14.210085 py3seed-0.2.0/src/py3seed/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      743 2023-07-10 07:31:29.000000 py3seed-0.2.0/src/py3seed/__init__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1624 2023-07-10 03:47:01.000000 py3seed-0.2.0/src/py3seed/__main__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)      992 2021-09-02 08:44:38.000000 py3seed-0.2.0/src/py3seed/admin.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     6458 2023-07-10 03:55:28.000000 py3seed-0.2.0/src/py3seed/cachesupport.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-19 07:46:14.216092 py3seed-0.2.0/src/py3seed/commands/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      151 2021-09-01 02:10:05.000000 py3seed-0.2.0/src/py3seed/commands/__init__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    21160 2023-07-19 07:44:52.000000 py3seed-0.2.0/src/py3seed/commands/gen.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)      732 2023-06-27 01:48:25.000000 py3seed-0.2.0/src/py3seed/error.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    11554 2023-07-10 03:49:24.000000 py3seed-0.2.0/src/py3seed/inflection.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1166 2022-05-06 11:35:05.000000 py3seed-0.2.0/src/py3seed/log.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    17725 2023-07-11 02:10:39.000000 py3seed-0.2.0/src/py3seed/merge3.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    57700 2023-07-18 01:28:13.000000 py3seed-0.2.0/src/py3seed/model.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14489 2023-07-10 03:55:58.000000 py3seed-0.2.0/src/py3seed/mongosupport.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14673 2023-07-19 03:29:37.000000 py3seed-0.2.0/src/py3seed/utils.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     7471 2023-07-10 03:54:22.000000 py3seed-0.2.0/src/py3seed/websupport.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-19 07:46:14.214952 py3seed-0.2.0/src/py3seed.egg-info/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-07-19 07:46:14.000000 py3seed-0.2.0/src/py3seed.egg-info/PKG-INFO
--rw-r--r--   0 weiminfeng   (501) staff       (20)      718 2023-07-19 07:46:14.000000 py3seed-0.2.0/src/py3seed.egg-info/SOURCES.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)        1 2023-07-19 07:46:14.000000 py3seed-0.2.0/src/py3seed.egg-info/dependency_links.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)      111 2023-07-19 07:46:14.000000 py3seed-0.2.0/src/py3seed.egg-info/entry_points.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)       48 2023-07-19 07:46:14.000000 py3seed-0.2.0/src/py3seed.egg-info/requires.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)        8 2023-07-19 07:46:14.000000 py3seed-0.2.0/src/py3seed.egg-info/top_level.txt
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-19 07:46:14.220175 py3seed-0.2.0/tests/
--rw-r--r--   0 weiminfeng   (501) staff       (20)     3216 2022-12-09 02:58:18.000000 py3seed-0.2.0/tests/test_cachesupport.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     6599 2023-07-18 07:07:02.000000 py3seed-0.2.0/tests/test_gen.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14977 2023-07-10 03:39:53.000000 py3seed-0.2.0/tests/test_merge3.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     5116 2023-07-05 06:36:00.000000 py3seed-0.2.0/tests/test_model.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     2083 2023-07-05 06:36:25.000000 py3seed-0.2.0/tests/test_mongosupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-19 07:50:45.548194 py3seed-0.2.1/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1072 2021-08-08 16:29:42.000000 py3seed-0.2.1/LICENSE
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-07-19 07:50:45.548471 py3seed-0.2.1/PKG-INFO
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      288 2021-08-11 03:57:41.000000 py3seed-0.2.1/README.md
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      104 2021-09-18 08:01:25.000000 py3seed-0.2.1/pyproject.toml
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      911 2023-07-19 07:50:45.549167 py3seed-0.2.1/setup.cfg
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      214 2023-07-06 08:35:28.000000 py3seed-0.2.1/setup.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-19 07:50:45.535984 py3seed-0.2.1/src/
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-19 07:50:45.542012 py3seed-0.2.1/src/py3seed/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      743 2023-07-10 07:31:29.000000 py3seed-0.2.1/src/py3seed/__init__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1624 2023-07-10 03:47:01.000000 py3seed-0.2.1/src/py3seed/__main__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      992 2021-09-02 08:44:38.000000 py3seed-0.2.1/src/py3seed/admin.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     6458 2023-07-10 03:55:28.000000 py3seed-0.2.1/src/py3seed/cachesupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-19 07:50:45.545365 py3seed-0.2.1/src/py3seed/commands/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      151 2021-09-01 02:10:05.000000 py3seed-0.2.1/src/py3seed/commands/__init__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    21146 2023-07-19 07:50:14.000000 py3seed-0.2.1/src/py3seed/commands/gen.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      732 2023-06-27 01:48:25.000000 py3seed-0.2.1/src/py3seed/error.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    11554 2023-07-10 03:49:24.000000 py3seed-0.2.1/src/py3seed/inflection.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1166 2022-05-06 11:35:05.000000 py3seed-0.2.1/src/py3seed/log.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    17725 2023-07-11 02:10:39.000000 py3seed-0.2.1/src/py3seed/merge3.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    57700 2023-07-18 01:28:13.000000 py3seed-0.2.1/src/py3seed/model.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14489 2023-07-10 03:55:58.000000 py3seed-0.2.1/src/py3seed/mongosupport.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14673 2023-07-19 03:29:37.000000 py3seed-0.2.1/src/py3seed/utils.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     7471 2023-07-10 03:54:22.000000 py3seed-0.2.1/src/py3seed/websupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-19 07:50:45.544276 py3seed-0.2.1/src/py3seed.egg-info/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-07-19 07:50:45.000000 py3seed-0.2.1/src/py3seed.egg-info/PKG-INFO
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      718 2023-07-19 07:50:45.000000 py3seed-0.2.1/src/py3seed.egg-info/SOURCES.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)        1 2023-07-19 07:50:45.000000 py3seed-0.2.1/src/py3seed.egg-info/dependency_links.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      111 2023-07-19 07:50:45.000000 py3seed-0.2.1/src/py3seed.egg-info/entry_points.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)       48 2023-07-19 07:50:45.000000 py3seed-0.2.1/src/py3seed.egg-info/requires.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)        8 2023-07-19 07:50:45.000000 py3seed-0.2.1/src/py3seed.egg-info/top_level.txt
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-19 07:50:45.547804 py3seed-0.2.1/tests/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     3216 2022-12-09 02:58:18.000000 py3seed-0.2.1/tests/test_cachesupport.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     6599 2023-07-18 07:07:02.000000 py3seed-0.2.1/tests/test_gen.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14977 2023-07-10 03:39:53.000000 py3seed-0.2.1/tests/test_merge3.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     5116 2023-07-05 06:36:00.000000 py3seed-0.2.1/tests/test_model.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     2083 2023-07-05 06:36:25.000000 py3seed-0.2.1/tests/test_mongosupport.py
```

### Comparing `py3seed-0.2.0/LICENSE` & `py3seed-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.0/PKG-INFO` & `py3seed-0.2.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3seed
-Version: 0.2.0
+Version: 0.2.1
 Summary: A package that bootstraps your project by simple data models definition and auto api and user interface generation
 Home-page: https://github.com/okosioc/pyseed
 Author: Samuel Feng
 Author-email: okosioc@gmail.com
 Project-URL: Bug Tracker, https://github.com/okosioc/pyseed/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py3seed-0.2.0/setup.cfg` & `py3seed-0.2.1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = py3seed
-version = 0.2.0
+version = 0.2.1
 author = Samuel Feng
 author_email = okosioc@gmail.com
 description = A package that bootstraps your project by simple data models definition and auto api and user interface generation
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/okosioc/pyseed
 project_urls =
```

### Comparing `py3seed-0.2.0/src/py3seed/__init__.py` & `py3seed-0.2.1/src/py3seed/__init__.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.0/src/py3seed/__main__.py` & `py3seed-0.2.1/src/py3seed/__main__.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.0/src/py3seed/admin.py` & `py3seed-0.2.1/src/py3seed/admin.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.0/src/py3seed/cachesupport.py` & `py3seed-0.2.1/src/py3seed/cachesupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.0/src/py3seed/commands/gen.py` & `py3seed-0.2.1/src/py3seed/commands/gen.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,17 +68,17 @@
         return os.path.basename(value)
 
     def urlquote(value, charset='utf-8'):
         """ Url Quote. """
         return url_quote(value, charset)
 
     def right(s: str, width: int = 4):
-        """ Do indent, if content is not blank, add leading indent"""
-        s = filters.do_indent(s, width, first=True)
-        if not s:
+        """ Do indent, if content is not blank, add leading indent. """
+        s = filters.do_indent(s, width)
+        if s:
             s = " " * width + s
         #
         return s
 
     env.filters['split'] = split
     env.filters['items'] = items
     env.filters['keys'] = keys
```

### Comparing `py3seed-0.2.0/src/py3seed/error.py` & `py3seed-0.2.1/src/py3seed/error.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.0/src/py3seed/inflection.py` & `py3seed-0.2.1/src/py3seed/inflection.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.0/src/py3seed/log.py` & `py3seed-0.2.1/src/py3seed/log.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.0/src/py3seed/merge3.py` & `py3seed-0.2.1/src/py3seed/merge3.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.0/src/py3seed/model.py` & `py3seed-0.2.1/src/py3seed/model.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.0/src/py3seed/mongosupport.py` & `py3seed-0.2.1/src/py3seed/mongosupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.0/src/py3seed/utils.py` & `py3seed-0.2.1/src/py3seed/utils.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.0/src/py3seed/websupport.py` & `py3seed-0.2.1/src/py3seed/websupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.0/src/py3seed.egg-info/PKG-INFO` & `py3seed-0.2.1/src/py3seed.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3seed
-Version: 0.2.0
+Version: 0.2.1
 Summary: A package that bootstraps your project by simple data models definition and auto api and user interface generation
 Home-page: https://github.com/okosioc/pyseed
 Author: Samuel Feng
 Author-email: okosioc@gmail.com
 Project-URL: Bug Tracker, https://github.com/okosioc/pyseed/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py3seed-0.2.0/src/py3seed.egg-info/SOURCES.txt` & `py3seed-0.2.1/src/py3seed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.0/tests/test_cachesupport.py` & `py3seed-0.2.1/tests/test_cachesupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.0/tests/test_gen.py` & `py3seed-0.2.1/tests/test_gen.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.0/tests/test_merge3.py` & `py3seed-0.2.1/tests/test_merge3.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.0/tests/test_model.py` & `py3seed-0.2.1/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.0/tests/test_mongosupport.py` & `py3seed-0.2.1/tests/test_mongosupport.py`

 * *Files identical despite different names*

