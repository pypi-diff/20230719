# Comparing `tmp/ilsadvbisnvavojebaij-0.2.0.tar.gz` & `tmp/ilsadvbisnvavojebaij-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ilsadvbisnvavojebaij-0.2.0.tar", last modified: Sun Jul  2 08:25:56 2023, max compression
+gzip compressed data, was "ilsadvbisnvavojebaij-0.2.1.tar", last modified: Wed Jul 19 05:02:45 2023, max compression
```

## Comparing `ilsadvbisnvavojebaij-0.2.0.tar` & `ilsadvbisnvavojebaij-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:25:56.726603 ilsadvbisnvavojebaij-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-02 08:25:56.726603 ilsadvbisnvavojebaij-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 08:25:36.000000 ilsadvbisnvavojebaij-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-02 08:25:36.000000 ilsadvbisnvavojebaij-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-02 08:25:56.730603 ilsadvbisnvavojebaij-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:25:56.722603 ilsadvbisnvavojebaij-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:25:56.726603 ilsadvbisnvavojebaij-0.2.0/src/ilsadvbisnvavojebaij/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-02 08:25:36.000000 ilsadvbisnvavojebaij-0.2.0/src/ilsadvbisnvavojebaij/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:25:56.726603 ilsadvbisnvavojebaij-0.2.0/src/ilsadvbisnvavojebaij/math/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 08:25:36.000000 ilsadvbisnvavojebaij-0.2.0/src/ilsadvbisnvavojebaij/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-02 08:25:36.000000 ilsadvbisnvavojebaij-0.2.0/src/ilsadvbisnvavojebaij/math/scalars.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-02 08:25:36.000000 ilsadvbisnvavojebaij-0.2.0/src/ilsadvbisnvavojebaij/math/vectors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:25:56.726603 ilsadvbisnvavojebaij-0.2.0/src/ilsadvbisnvavojebaij/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 08:25:36.000000 ilsadvbisnvavojebaij-0.2.0/src/ilsadvbisnvavojebaij/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-02 08:25:36.000000 ilsadvbisnvavojebaij-0.2.0/src/ilsadvbisnvavojebaij/utils/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:25:56.726603 ilsadvbisnvavojebaij-0.2.0/src/ilsadvbisnvavojebaij.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-02 08:25:56.000000 ilsadvbisnvavojebaij-0.2.0/src/ilsadvbisnvavojebaij.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-02 08:25:56.000000 ilsadvbisnvavojebaij-0.2.0/src/ilsadvbisnvavojebaij.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 08:25:56.000000 ilsadvbisnvavojebaij-0.2.0/src/ilsadvbisnvavojebaij.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-02 08:25:56.000000 ilsadvbisnvavojebaij-0.2.0/src/ilsadvbisnvavojebaij.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-02 08:25:56.000000 ilsadvbisnvavojebaij-0.2.0/src/ilsadvbisnvavojebaij.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:02:45.131695 ilsadvbisnvavojebaij-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-19 05:02:45.131695 ilsadvbisnvavojebaij-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 05:02:28.000000 ilsadvbisnvavojebaij-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-19 05:02:28.000000 ilsadvbisnvavojebaij-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-19 05:02:45.131695 ilsadvbisnvavojebaij-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:02:45.127695 ilsadvbisnvavojebaij-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:02:45.127695 ilsadvbisnvavojebaij-0.2.1/src/ilsadvbisnvavojebaij/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-19 05:02:28.000000 ilsadvbisnvavojebaij-0.2.1/src/ilsadvbisnvavojebaij/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:02:45.127695 ilsadvbisnvavojebaij-0.2.1/src/ilsadvbisnvavojebaij/math/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 05:02:28.000000 ilsadvbisnvavojebaij-0.2.1/src/ilsadvbisnvavojebaij/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-19 05:02:28.000000 ilsadvbisnvavojebaij-0.2.1/src/ilsadvbisnvavojebaij/math/scalars.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-19 05:02:28.000000 ilsadvbisnvavojebaij-0.2.1/src/ilsadvbisnvavojebaij/math/vectors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:02:45.131695 ilsadvbisnvavojebaij-0.2.1/src/ilsadvbisnvavojebaij/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 05:02:28.000000 ilsadvbisnvavojebaij-0.2.1/src/ilsadvbisnvavojebaij/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-19 05:02:28.000000 ilsadvbisnvavojebaij-0.2.1/src/ilsadvbisnvavojebaij/utils/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:02:45.127695 ilsadvbisnvavojebaij-0.2.1/src/ilsadvbisnvavojebaij.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-19 05:02:45.000000 ilsadvbisnvavojebaij-0.2.1/src/ilsadvbisnvavojebaij.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-19 05:02:45.000000 ilsadvbisnvavojebaij-0.2.1/src/ilsadvbisnvavojebaij.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 05:02:45.000000 ilsadvbisnvavojebaij-0.2.1/src/ilsadvbisnvavojebaij.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-19 05:02:45.000000 ilsadvbisnvavojebaij-0.2.1/src/ilsadvbisnvavojebaij.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-19 05:02:45.000000 ilsadvbisnvavojebaij-0.2.1/src/ilsadvbisnvavojebaij.egg-info/top_level.txt
```

### Comparing `ilsadvbisnvavojebaij-0.2.0/PKG-INFO` & `ilsadvbisnvavojebaij-0.2.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ilsadvbisnvavojebaij
-Version: 0.2.0
+Version: 0.2.1
 Summary: A randome placeholder package for CI testing
 Author: Francisco Castillo
 Author-email: fjcastillocarrasco@gmail.com
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `ilsadvbisnvavojebaij-0.2.0/setup.cfg` & `ilsadvbisnvavojebaij-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ilsadvbisnvavojebaij-0.2.0/src/ilsadvbisnvavojebaij/math/vectors.py` & `ilsadvbisnvavojebaij-0.2.1/src/ilsadvbisnvavojebaij/math/vectors.py`

 * *Files identical despite different names*

### Comparing `ilsadvbisnvavojebaij-0.2.0/src/ilsadvbisnvavojebaij/utils/logging.py` & `ilsadvbisnvavojebaij-0.2.1/src/ilsadvbisnvavojebaij/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ilsadvbisnvavojebaij-0.2.0/src/ilsadvbisnvavojebaij.egg-info/PKG-INFO` & `ilsadvbisnvavojebaij-0.2.1/src/ilsadvbisnvavojebaij.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ilsadvbisnvavojebaij
-Version: 0.2.0
+Version: 0.2.1
 Summary: A randome placeholder package for CI testing
 Author: Francisco Castillo
 Author-email: fjcastillocarrasco@gmail.com
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `ilsadvbisnvavojebaij-0.2.0/src/ilsadvbisnvavojebaij.egg-info/SOURCES.txt` & `ilsadvbisnvavojebaij-0.2.1/src/ilsadvbisnvavojebaij.egg-info/SOURCES.txt`

 * *Files identical despite different names*

