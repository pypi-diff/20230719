# Comparing `tmp/lino_react-23.7.2.tar.gz` & `tmp/lino_react-23.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lino_react-23.7.2.tar", last modified: Tue Jul 18 09:52:38 2023, max compression
+gzip compressed data, was "lino_react-23.7.3.tar", last modified: Tue Jul 18 09:59:57 2023, max compression
```

## Comparing `lino_react-23.7.2.tar` & `lino_react-23.7.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-18 09:52:38.892101 lino_react-23.7.2/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    34523 2021-04-12 19:37:56.000000 lino_react-23.7.2/COPYING
--rw-rw-rw-   0 luc       (1000) www-data    (33)      157 2020-04-27 23:26:14.000000 lino_react-23.7.2/MANIFEST.in
--rw-rw-r--   0 luc       (1000) www-data    (33)     1069 2023-07-18 09:52:38.892101 lino_react-23.7.2/PKG-INFO
--rw-rw-rw-   0 luc       (1000) www-data    (33)      178 2021-05-23 18:57:15.000000 lino_react-23.7.2/README.rst
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-18 09:52:38.888101 lino_react-23.7.2/lino_react/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      283 2021-05-23 18:57:15.000000 lino_react-23.7.2/lino_react/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-18 09:52:38.888101 lino_react-23.7.2/lino_react/react/
--rw-rw-r--   0 luc       (1000) www-data    (33)     4628 2023-06-13 10:30:58.000000 lino_react-23.7.2/lino_react/react/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-18 09:52:38.888101 lino_react-23.7.2/lino_react/react/__pycache__/
--rw-rw-r--   0 luc       (1000) www-data    (33)     3362 2023-06-23 05:20:50.000000 lino_react-23.7.2/lino_react/react/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 luc       (1000) www-data    (33)     4010 2023-07-05 02:47:39.000000 lino_react-23.7.2/lino_react/react/__pycache__/icons.cpython-310.pyc
--rw-rw-r--   0 luc       (1000) www-data    (33)      140 2023-06-23 05:20:51.000000 lino_react-23.7.2/lino_react/react/__pycache__/models.cpython-310.pyc
--rw-rw-r--   0 luc       (1000) www-data    (33)    18481 2023-07-18 09:49:19.000000 lino_react-23.7.2/lino_react/react/__pycache__/renderer.cpython-310.pyc
--rw-rw-r--   0 luc       (1000) www-data    (33)    20595 2023-06-23 08:10:05.000000 lino_react-23.7.2/lino_react/react/__pycache__/views.cpython-310.pyc
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-18 09:52:38.888101 lino_react-23.7.2/lino_react/react/config/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-18 09:52:38.888101 lino_react-23.7.2/lino_react/react/config/react/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2018-11-27 12:45:09.000000 lino_react-23.7.2/lino_react/react/config/react/linoweb.json
--rw-rw-r--   0 luc       (1000) www-data    (33)     1910 2023-06-11 12:10:21.000000 lino_react-23.7.2/lino_react/react/config/react/main.html
--rw-rw-r--   0 luc       (1000) www-data    (33)    16246 2022-11-30 04:23:52.000000 lino_react-23.7.2/lino_react/react/config/react/service-worker.js
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3952 2023-07-05 02:47:35.000000 lino_react-23.7.2/lino_react/react/icons.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       36 2018-11-22 22:23:05.000000 lino_react-23.7.2/lino_react/react/index.js
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2023-03-28 18:53:35.000000 lino_react-23.7.2/lino_react/react/models.py
--rw-rw-r--   0 luc       (1000) www-data    (33)    29449 2023-07-18 09:49:16.000000 lino_react-23.7.2/lino_react/react/renderer.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-18 09:52:38.888101 lino_react-23.7.2/lino_react/react/static/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-18 09:52:38.892101 lino_react-23.7.2/lino_react/react/static/media/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    10355 2021-05-17 15:54:58.000000 lino_react-23.7.2/lino_react/react/static/media/color.6441e63a.png
--rw-rw-rw-   0 luc       (1000) www-data    (33)    10355 2021-01-26 04:29:47.000000 lino_react-23.7.2/lino_react/react/static/media/color.c7a33805.png
--rw-rw-rw-   0 luc       (1000) www-data    (33)    13112 2020-09-29 17:55:04.000000 lino_react-23.7.2/lino_react/react/static/media/line.567f5738.gif
--rw-rw-rw-   0 luc       (1000) www-data    (33)    39748 2021-01-26 04:29:47.000000 lino_react-23.7.2/lino_react/react/static/media/primeicons.2d2afb27.eot
--rw-rw-rw-   0 luc       (1000) www-data    (33)    57384 2021-05-17 15:54:58.000000 lino_react-23.7.2/lino_react/react/static/media/primeicons.3a0d4a58.ttf
--rw-rw-rw-   0 luc       (1000) www-data    (33)    39648 2021-01-26 04:29:47.000000 lino_react-23.7.2/lino_react/react/static/media/primeicons.66ee0deb.woff
--rw-rw-rw-   0 luc       (1000) www-data    (33)   234640 2021-05-17 15:54:58.000000 lino_react-23.7.2/lino_react/react/static/media/primeicons.c55d94a2.svg
--rw-rw-rw-   0 luc       (1000) www-data    (33)    39572 2021-01-26 04:29:47.000000 lino_react-23.7.2/lino_react/react/static/media/primeicons.df0140f8.ttf
--rw-rw-rw-   0 luc       (1000) www-data    (33)    57560 2021-05-17 15:54:58.000000 lino_react-23.7.2/lino_react/react/static/media/primeicons.dfbfef2d.eot
--rw-rw-rw-   0 luc       (1000) www-data    (33)   163568 2021-01-26 04:29:47.000000 lino_react-23.7.2/lino_react/react/static/media/primeicons.e5e0e944.svg
--rw-rw-rw-   0 luc       (1000) www-data    (33)    57460 2021-05-17 15:54:58.000000 lino_react-23.7.2/lino_react/react/static/media/primeicons.e61f3495.woff
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-18 09:52:38.892101 lino_react-23.7.2/lino_react/react/static/react/
--rw-rw-r--   0 luc       (1000) www-data    (33)  1789571 2023-07-18 09:49:16.000000 lino_react-23.7.2/lino_react/react/static/react/main.js
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2437 2021-09-23 03:04:12.000000 lino_react-23.7.2/lino_react/react/static/react/main.js.LICENSE.txt
--rw-rw-r--   0 luc       (1000) www-data    (33)    28705 2023-03-24 10:38:37.000000 lino_react-23.7.2/lino_react/react/views.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     1431 2023-07-18 09:52:15.000000 lino_react-23.7.2/lino_react/setup_info.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-18 09:52:38.888101 lino_react-23.7.2/lino_react.egg-info/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1069 2023-07-18 09:52:38.000000 lino_react-23.7.2/lino_react.egg-info/PKG-INFO
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1522 2023-07-18 09:52:38.000000 lino_react-23.7.2/lino_react.egg-info/SOURCES.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2023-07-18 09:52:38.000000 lino_react-23.7.2/lino_react.egg-info/dependency_links.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2019-01-08 09:40:17.000000 lino_react-23.7.2/lino_react.egg-info/not-zip-safe
--rw-rw-rw-   0 luc       (1000) www-data    (33)        5 2023-07-18 09:52:38.000000 lino_react-23.7.2/lino_react.egg-info/requires.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)       11 2023-07-18 09:52:38.000000 lino_react-23.7.2/lino_react.egg-info/top_level.txt
--rw-rw-r--   0 luc       (1000) www-data    (33)       38 2023-07-18 09:52:38.892101 lino_react-23.7.2/setup.cfg
--rw-rw-rw-   0 luc       (1000) www-data    (33)      183 2021-04-06 11:15:38.000000 lino_react-23.7.2/setup.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      348 2021-05-23 18:57:15.000000 lino_react-23.7.2/tasks.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-18 09:59:57.667353 lino_react-23.7.3/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    34523 2021-04-12 19:37:56.000000 lino_react-23.7.3/COPYING
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      157 2020-04-27 23:26:14.000000 lino_react-23.7.3/MANIFEST.in
+-rw-rw-r--   0 luc       (1000) www-data    (33)     1069 2023-07-18 09:59:57.667353 lino_react-23.7.3/PKG-INFO
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      178 2021-05-23 18:57:15.000000 lino_react-23.7.3/README.rst
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-18 09:59:57.663352 lino_react-23.7.3/lino_react/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      283 2021-05-23 18:57:15.000000 lino_react-23.7.3/lino_react/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-18 09:59:57.663352 lino_react-23.7.3/lino_react/react/
+-rw-rw-r--   0 luc       (1000) www-data    (33)     4628 2023-06-13 10:30:58.000000 lino_react-23.7.3/lino_react/react/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-18 09:59:57.663352 lino_react-23.7.3/lino_react/react/__pycache__/
+-rw-rw-r--   0 luc       (1000) www-data    (33)     3362 2023-06-23 05:20:50.000000 lino_react-23.7.3/lino_react/react/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 luc       (1000) www-data    (33)     4010 2023-07-05 02:47:39.000000 lino_react-23.7.3/lino_react/react/__pycache__/icons.cpython-310.pyc
+-rw-rw-r--   0 luc       (1000) www-data    (33)      140 2023-06-23 05:20:51.000000 lino_react-23.7.3/lino_react/react/__pycache__/models.cpython-310.pyc
+-rw-rw-r--   0 luc       (1000) www-data    (33)    18481 2023-07-18 09:49:19.000000 lino_react-23.7.3/lino_react/react/__pycache__/renderer.cpython-310.pyc
+-rw-rw-r--   0 luc       (1000) www-data    (33)    20595 2023-06-23 08:10:05.000000 lino_react-23.7.3/lino_react/react/__pycache__/views.cpython-310.pyc
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-18 09:59:57.663352 lino_react-23.7.3/lino_react/react/config/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-18 09:59:57.663352 lino_react-23.7.3/lino_react/react/config/react/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2018-11-27 12:45:09.000000 lino_react-23.7.3/lino_react/react/config/react/linoweb.json
+-rw-rw-r--   0 luc       (1000) www-data    (33)     1910 2023-06-11 12:10:21.000000 lino_react-23.7.3/lino_react/react/config/react/main.html
+-rw-rw-r--   0 luc       (1000) www-data    (33)    16246 2022-11-30 04:23:52.000000 lino_react-23.7.3/lino_react/react/config/react/service-worker.js
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3952 2023-07-05 02:47:35.000000 lino_react-23.7.3/lino_react/react/icons.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       36 2018-11-22 22:23:05.000000 lino_react-23.7.3/lino_react/react/index.js
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2023-03-28 18:53:35.000000 lino_react-23.7.3/lino_react/react/models.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)    29449 2023-07-18 09:49:16.000000 lino_react-23.7.3/lino_react/react/renderer.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-18 09:59:57.663352 lino_react-23.7.3/lino_react/react/static/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-18 09:59:57.663352 lino_react-23.7.3/lino_react/react/static/media/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    10355 2021-05-17 15:54:58.000000 lino_react-23.7.3/lino_react/react/static/media/color.6441e63a.png
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    10355 2021-01-26 04:29:47.000000 lino_react-23.7.3/lino_react/react/static/media/color.c7a33805.png
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    13112 2020-09-29 17:55:04.000000 lino_react-23.7.3/lino_react/react/static/media/line.567f5738.gif
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    39748 2021-01-26 04:29:47.000000 lino_react-23.7.3/lino_react/react/static/media/primeicons.2d2afb27.eot
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    57384 2021-05-17 15:54:58.000000 lino_react-23.7.3/lino_react/react/static/media/primeicons.3a0d4a58.ttf
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    39648 2021-01-26 04:29:47.000000 lino_react-23.7.3/lino_react/react/static/media/primeicons.66ee0deb.woff
+-rw-rw-rw-   0 luc       (1000) www-data    (33)   234640 2021-05-17 15:54:58.000000 lino_react-23.7.3/lino_react/react/static/media/primeicons.c55d94a2.svg
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    39572 2021-01-26 04:29:47.000000 lino_react-23.7.3/lino_react/react/static/media/primeicons.df0140f8.ttf
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    57560 2021-05-17 15:54:58.000000 lino_react-23.7.3/lino_react/react/static/media/primeicons.dfbfef2d.eot
+-rw-rw-rw-   0 luc       (1000) www-data    (33)   163568 2021-01-26 04:29:47.000000 lino_react-23.7.3/lino_react/react/static/media/primeicons.e5e0e944.svg
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    57460 2021-05-17 15:54:58.000000 lino_react-23.7.3/lino_react/react/static/media/primeicons.e61f3495.woff
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-18 09:59:57.667353 lino_react-23.7.3/lino_react/react/static/react/
+-rw-rw-r--   0 luc       (1000) www-data    (33)  1788685 2023-07-18 09:58:49.000000 lino_react-23.7.3/lino_react/react/static/react/main.js
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2437 2021-09-23 03:04:12.000000 lino_react-23.7.3/lino_react/react/static/react/main.js.LICENSE.txt
+-rw-rw-r--   0 luc       (1000) www-data    (33)    28705 2023-03-24 10:38:37.000000 lino_react-23.7.3/lino_react/react/views.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     1431 2023-07-18 09:59:35.000000 lino_react-23.7.3/lino_react/setup_info.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-18 09:59:57.663352 lino_react-23.7.3/lino_react.egg-info/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1069 2023-07-18 09:59:57.000000 lino_react-23.7.3/lino_react.egg-info/PKG-INFO
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1522 2023-07-18 09:59:57.000000 lino_react-23.7.3/lino_react.egg-info/SOURCES.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2023-07-18 09:59:57.000000 lino_react-23.7.3/lino_react.egg-info/dependency_links.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2019-01-08 09:40:17.000000 lino_react-23.7.3/lino_react.egg-info/not-zip-safe
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        5 2023-07-18 09:59:57.000000 lino_react-23.7.3/lino_react.egg-info/requires.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       11 2023-07-18 09:59:57.000000 lino_react-23.7.3/lino_react.egg-info/top_level.txt
+-rw-rw-r--   0 luc       (1000) www-data    (33)       38 2023-07-18 09:59:57.667353 lino_react-23.7.3/setup.cfg
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      183 2021-04-06 11:15:38.000000 lino_react-23.7.3/setup.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      348 2021-05-23 18:57:15.000000 lino_react-23.7.3/tasks.py
```

### Comparing `lino_react-23.7.2/COPYING` & `lino_react-23.7.3/COPYING`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.2/PKG-INFO` & `lino_react-23.7.3/lino_react.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: lino_react
-Version: 23.7.2
+Name: lino-react
+Version: 23.7.3
 Summary: The React front end for Lino
 Home-page: https://gitlab.com/lino-framework/react
 Author: Rumma & Ko Ltd
 Author-email: info@lino-framework.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier:   Programming Language :: Python
```

### Comparing `lino_react-23.7.2/lino_react/react/__init__.py` & `lino_react-23.7.3/lino_react/react/__init__.py`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.2/lino_react/react/__pycache__/__init__.cpython-310.pyc` & `lino_react-23.7.3/lino_react/react/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.2/lino_react/react/__pycache__/icons.cpython-310.pyc` & `lino_react-23.7.3/lino_react/react/__pycache__/icons.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.2/lino_react/react/__pycache__/renderer.cpython-310.pyc` & `lino_react-23.7.3/lino_react/react/__pycache__/renderer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.2/lino_react/react/__pycache__/views.cpython-310.pyc` & `lino_react-23.7.3/lino_react/react/__pycache__/views.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.2/lino_react/react/config/react/main.html` & `lino_react-23.7.3/lino_react/react/config/react/main.html`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.2/lino_react/react/config/react/service-worker.js` & `lino_react-23.7.3/lino_react/react/config/react/service-worker.js`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.2/lino_react/react/icons.py` & `lino_react-23.7.3/lino_react/react/icons.py`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.2/lino_react/react/renderer.py` & `lino_react-23.7.3/lino_react/react/renderer.py`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.2/lino_react/react/static/media/color.6441e63a.png` & `lino_react-23.7.3/lino_react/react/static/media/color.6441e63a.png`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.2/lino_react/react/static/media/color.c7a33805.png` & `lino_react-23.7.3/lino_react/react/static/media/color.c7a33805.png`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.2/lino_react/react/static/media/line.567f5738.gif` & `lino_react-23.7.3/lino_react/react/static/media/line.567f5738.gif`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.2/lino_react/react/static/media/primeicons.2d2afb27.eot` & `lino_react-23.7.3/lino_react/react/static/media/primeicons.2d2afb27.eot`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.2/lino_react/react/static/media/primeicons.3a0d4a58.ttf` & `lino_react-23.7.3/lino_react/react/static/media/primeicons.3a0d4a58.ttf`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.2/lino_react/react/static/media/primeicons.66ee0deb.woff` & `lino_react-23.7.3/lino_react/react/static/media/primeicons.66ee0deb.woff`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.2/lino_react/react/static/media/primeicons.c55d94a2.svg` & `lino_react-23.7.3/lino_react/react/static/media/primeicons.c55d94a2.svg`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.2/lino_react/react/static/media/primeicons.df0140f8.ttf` & `lino_react-23.7.3/lino_react/react/static/media/primeicons.df0140f8.ttf`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.2/lino_react/react/static/media/primeicons.dfbfef2d.eot` & `lino_react-23.7.3/lino_react/react/static/media/primeicons.dfbfef2d.eot`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.2/lino_react/react/static/media/primeicons.e5e0e944.svg` & `lino_react-23.7.3/lino_react/react/static/media/primeicons.e5e0e944.svg`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.2/lino_react/react/static/media/primeicons.e61f3495.woff` & `lino_react-23.7.3/lino_react/react/static/media/primeicons.e61f3495.woff`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.2/lino_react/react/static/react/main.js` & `lino_react-23.7.3/lino_react/react/static/react/main.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -3075,15 +3075,15 @@
                     disabledFields: {}
                 };
                 const __WEBPACK_DEFAULT_EXPORT__ = LinoBbar
             },
             6149: (e, t, n) => {
                 "use strict";
                 n.d(t, {
-                    Z: () => Ye
+                    Z: () => Ge
                 });
                 var o = n(3379),
                     r = n.n(o),
                     i = n(5397);
                 r()(i.Z, {
                     insert: "head",
                     singleton: !1
@@ -5112,122 +5112,102 @@
                             var n = arguments[t];
                             for (var o in n) Object.prototype.hasOwnProperty.call(n, o) && (e[o] = n[o])
                         }
                         return e
                     }, Be.apply(this, arguments)
                 }
 
-                function Fe(e, t) {
-                    var n = Object.keys(e);
-                    if (Object.getOwnPropertySymbols) {
-                        var o = Object.getOwnPropertySymbols(e);
-                        t && (o = o.filter((function(t) {
-                            return Object.getOwnPropertyDescriptor(e, t).enumerable
-                        }))), n.push.apply(n, o)
-                    }
-                    return n
-                }
-
-                function ze(e, t, n) {
-                    return t in e ? Object.defineProperty(e, t, {
-                        value: n,
-                        enumerable: !0,
-                        configurable: !0,
-                        writable: !0
-                    }) : e[t] = n, e
-                }
-
-                function Ue(e, t, n, o, r, i, a) {
+                function Fe(e, t, n, o, r, i, a) {
                     try {
                         var l = e[i](a),
                             s = l.value
                     } catch (e) {
                         return void n(e)
                     }
                     l.done ? t(s) : Promise.resolve(s).then(o, r)
                 }
 
-                function Ke(e) {
+                function ze(e) {
                     return function() {
                         var t = this,
                             n = arguments;
                         return new Promise((function(o, r) {
                             var i = e.apply(t, n);
 
                             function a(e) {
-                                Ue(i, o, r, a, l, "next", e)
+                                Fe(i, o, r, a, l, "next", e)
                             }
 
                             function l(e) {
-                                Ue(i, o, r, a, l, "throw", e)
+                                Fe(i, o, r, a, l, "throw", e)
                             }
                             a(void 0)
                         }))
                     }
                 }
 
-                function We(e, t) {
+                function Ue(e, t) {
                     for (var n = 0; n < t.length; n++) {
                         var o = t[n];
                         o.enumerable = o.enumerable || !1, o.configurable = !0, "value" in o && (o.writable = !0), Object.defineProperty(e, o.key, o)
                     }
                 }
 
-                function He(e, t) {
-                    return He = Object.setPrototypeOf || function(e, t) {
+                function Ke(e, t) {
+                    return Ke = Object.setPrototypeOf || function(e, t) {
                         return e.__proto__ = t, e
-                    }, He(e, t)
+                    }, Ke(e, t)
                 }
 
-                function Ve(e, t) {
+                function We(e, t) {
                     if (t && ("object" === Ne(t) || "function" == typeof t)) return t;
                     if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
-                    return Ge(e)
+                    return He(e)
                 }
 
-                function Ge(e) {
+                function He(e) {
                     if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
                     return e
                 }
 
-                function Ze(e) {
-                    return Ze = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
+                function Ve(e) {
+                    return Ve = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
                         return e.__proto__ || Object.getPrototypeOf(e)
-                    }, Ze(e)
+                    }, Ve(e)
                 }
-                var Ye = function(e) {
+                var Ge = function(e) {
                     ! function(e, t) {
                         if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function");
                         Object.defineProperty(e, "prototype", {
                             value: Object.create(t && t.prototype, {
                                 constructor: {
                                     value: e,
                                     writable: !0,
                                     configurable: !0
                                 }
                             }),
                             writable: !1
-                        }), t && He(e, t)
+                        }), t && Ke(e, t)
                     }(d, e);
                     var t, n, o, r, i, p, u = (i = d, p = function() {
                         if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
                         if (Reflect.construct.sham) return !1;
                         if ("function" == typeof Proxy) return !0;
                         try {
                             return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
                         } catch (e) {
                             return !1
                         }
                     }(), function() {
-                        var e, t = Ze(i);
+                        var e, t = Ve(i);
                         if (p) {
-                            var n = Ze(this).constructor;
+                            var n = Ve(this).constructor;
                             e = Reflect.construct(t, arguments, n)
                         } else e = t.apply(this, arguments);
-                        return Ve(this, e)
+                        return We(this, e)
                     });
 
                     function d(e) {
                         var t;
                         ! function(e, t) {
                             if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
                         }(this, d), t = u.call(this, e);
@@ -5273,15 +5253,15 @@
                             })),
                             sortCol: void 0,
                             sortField: void 0,
                             sortFieldName: void 0,
                             sortOrder: 0,
                             title: "",
                             topRow: 0
-                        }, t.actionWrapper = t.actionWrapper.bind(Ge(t)), t.consumeServerResponse = t.consumeServerResponse.bind(Ge(t)), t.get_current_grid_config = t.get_current_grid_config.bind(Ge(t)), t.get_full_id = t.get_full_id.bind(Ge(t)), t.getData = t.getData.bind(Ge(t)), t.getOne = t.getOne.bind(Ge(t)), t.getUri = t.getUri.bind(Ge(t)), t.handleWindowChange = (0, x.Ds)(t.handleWindowChange.bind(Ge(t)), 50), t.messageInterceptor = t.messageInterceptor.bind(Ge(t)), t.registerScroll = t.registerScroll.bind(Ge(t)), t.multiRowView = t.multiRowView.bind(Ge(t)), t.onKeyDown = t.onKeyDown.bind(Ge(t)), t.onRowDoubleClick = t.onRowDoubleClick.bind(Ge(t)), t.onSort = t.onSort.bind(Ge(t)), t.refresh = t.refresh.bind(Ge(t)), t.quickFilter = (0, x.Ds)(t.quickFilter.bind(Ge(t)), 200), t.reload = t.reload.bind(Ge(t)), t.reset = t.reset.bind(Ge(t)), t.update_params_values = t.update_params_values.bind(Ge(t)), t
+                        }, t.actionWrapper = t.actionWrapper.bind(He(t)), t.consumeServerResponse = t.consumeServerResponse.bind(He(t)), t.get_current_grid_config = t.get_current_grid_config.bind(He(t)), t.get_full_id = t.get_full_id.bind(He(t)), t.getData = t.getData.bind(He(t)), t.getOne = t.getOne.bind(He(t)), t.getUri = t.getUri.bind(He(t)), t.handleWindowChange = (0, x.Ds)(t.handleWindowChange.bind(He(t)), 50), t.messageInterceptor = t.messageInterceptor.bind(He(t)), t.registerScroll = t.registerScroll.bind(He(t)), t.multiRowView = t.multiRowView.bind(He(t)), t.onKeyDown = t.onKeyDown.bind(He(t)), t.onRowDoubleClick = t.onRowDoubleClick.bind(He(t)), t.onSort = t.onSort.bind(He(t)), t.refresh = t.refresh.bind(He(t)), t.quickFilter = (0, x.Ds)(t.quickFilter.bind(He(t)), 200), t.reload = t.reload.bind(He(t)), t.reset = t.reset.bind(He(t)), t.update_params_values = t.update_params_values.bind(He(t)), t
                     }
                     return t = d, n = [{
                         key: "get_full_id",
                         value: function() {
                             return "".concat(this.props.packId, ".").concat(this.props.actorId)
                         }
                     }, {
@@ -5487,15 +5467,15 @@
                         key: "getUri",
                         value: function(e) {
                             var t = "api/".concat(this.props.packId, "/").concat(this.props.actorId);
                             return void 0 !== e && (t += "?".concat(g.stringify(e))), t
                         }
                     }, {
                         key: "getData",
-                        value: (r = Ke(y().mark((function e(t, n, o) {
+                        value: (r = ze(y().mark((function e(t, n, o) {
                             var r, i = this,
                                 a = arguments;
                             return y().wrap((function(e) {
                                 for (;;) switch (e.prev = e.next) {
                                     case 0:
                                         return (r = a.length > 3 && void 0 !== a[3] && a[3]) && Object.assign(this.data, {
                                             loading: !0,
@@ -5516,15 +5496,15 @@
                                 }
                             }), e, this)
                         }))), function(e, t, n) {
                             return r.apply(this, arguments)
                         })
                     }, {
                         key: "getOne",
-                        value: (o = Ke(y().mark((function e(t, n, o, r) {
+                        value: (o = ze(y().mark((function e(t, n, o, r) {
                             var i = this;
                             return y().wrap((function(e) {
                                 for (;;) switch (e.prev = e.next) {
                                     case 0:
                                         return e.next = 2, (0, b.he)("api/".concat(this.props.packId, "/").concat(this.props.actorId, "/").concat(t, "?").concat(g.stringify(n)), {
                                             signal: o
                                         }).then(window.App.handleAjaxResponse).then((function(e) {
@@ -5602,30 +5582,15 @@
                                 show_top_toolbar: !(0, x.tq)() && void 0 !== this.props.actorData.col,
                                 window_width: window.innerWidth
                             })
                         }
                     }, {
                         key: "update_params_values",
                         value: function(e, t, n) {
-                            (0, x.ku)(this.data.params_values, this.props.actorData.params_fields);
-                            var o = Object.assign({}, this.data.params_values, function(e) {
-                                    for (var t = 1; t < arguments.length; t++) {
-                                        var n = null != arguments[t] ? arguments[t] : {};
-                                        t % 2 ? Fe(Object(n), !0).forEach((function(t) {
-                                            ze(e, t, n[t])
-                                        })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Fe(Object(n)).forEach((function(t) {
-                                            Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
-                                        }))
-                                    }
-                                    return e
-                                }({}, e)),
-                                r = (0, x.ku)(o, this.props.actorData.params_fields);
-                            this.data.pv = r, Object.assign(this.data, {
-                                params_values: o
-                            }), this.reload()
+                            this.data.pv = (0, x.ku)(Object.assign(this.data.params_values, e), this.props.actorData.params_fields), this.reload()
                         }
                     }, {
                         key: "get_current_grid_config",
                         value: function(e) {
                             var t = this.props.actorData.col,
                                 n = [],
                                 o = [],
@@ -5646,15 +5611,15 @@
                                 return !i.includes(e.fields_index)
                             })).forEach((function(e) {
                                 n.push(e.name), e.width ? o.push(e.width) : o.push(15)
                             })), n.forEach((function(e) {
                                 r.push(t.filter((function(t) {
                                     return t.name === e
                                 }))[0].hidden)
-                            })), e[me.Td] = n, e[me.SX] = r, e[me.EO] = o, e[me.ks] = (0, x.ku)(this.data.params_values, this.props.actorData.params_fields), e
+                            })), e[me.Td] = n, e[me.SX] = r, e[me.EO] = o, e[me.ks] = this.data.pv, e
                         }
                     }, {
                         key: "render",
                         value: function() {
                             var e = this,
                                 t = "l-grid ";
                             if ("whitewall" === window.App.data.themeName && (t += "l-whitewall-body "), this.props.actorData.hide_if_empty && this.props.inDetail && 0 === this.data.rows.length) return null;
@@ -5807,22 +5772,22 @@
                                         showPVDialog: !1
                                     })
                                 }
                             }, this.props.actorData.params_layout && this.state.showPVDialog && a.createElement(Le, {
                                 parent: this
                             })))
                         }
-                    }], n && We(t.prototype, n), Object.defineProperty(t, "prototype", {
+                    }], n && Ue(t.prototype, n), Object.defineProperty(t, "prototype", {
                         writable: !1
                     }), d
                 }(a.Component);
-                Ye.propTypes = {
+                Ge.propTypes = {
                     inDetail: f().bool,
                     depth: f().number
-                }, Ye.defaultProps = {
+                }, Ge.defaultProps = {
                     inDetail: !1,
                     depth: 0
                 }
             },
             7573: (e, t, n) => {
                 "use strict";
                 n.d(t, {
```

### Comparing `lino_react-23.7.2/lino_react/react/static/react/main.js.LICENSE.txt` & `lino_react-23.7.3/lino_react/react/static/react/main.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.2/lino_react/react/views.py` & `lino_react-23.7.3/lino_react/react/views.py`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.2/lino_react/setup_info.py` & `lino_react-23.7.3/lino_react/setup_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: UTF-8 -*-
 # Copyright 2015-2023 Rumma & Ko Ltd
 # License: GNU Affero General Public License v3 (see file COPYING for details)
 
 SETUP_INFO = dict(
     name='lino_react',
-    version='23.7.2',
+    version='23.7.3',
     install_requires=['lino'],
     tests_require=[],
     test_suite='tests',
     description="The React front end for Lino",
     license_files=['COPYING'],
     include_package_data=False,
     zip_safe=False,
```

### Comparing `lino_react-23.7.2/lino_react.egg-info/PKG-INFO` & `lino_react-23.7.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: lino-react
-Version: 23.7.2
+Name: lino_react
+Version: 23.7.3
 Summary: The React front end for Lino
 Home-page: https://gitlab.com/lino-framework/react
 Author: Rumma & Ko Ltd
 Author-email: info@lino-framework.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier:   Programming Language :: Python
```

### Comparing `lino_react-23.7.2/lino_react.egg-info/SOURCES.txt` & `lino_react-23.7.3/lino_react.egg-info/SOURCES.txt`

 * *Files identical despite different names*

