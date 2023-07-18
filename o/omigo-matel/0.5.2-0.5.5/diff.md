# Comparing `tmp/omigo_matel-0.5.2.tar.gz` & `tmp/omigo_matel-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omigo_matel-0.5.2.tar", last modified: Thu May 25 19:18:25 2023, max compression
+gzip compressed data, was "omigo_matel-0.5.5.tar", last modified: Tue Jul 18 23:43:06 2023, max compression
```

## Comparing `omigo_matel-0.5.2.tar` & `omigo_matel-0.5.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:18:25.481094 omigo_matel-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-25 19:18:25.481094 omigo_matel-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:16:29.000000 omigo_matel-0.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-25 19:16:29.000000 omigo_matel-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-25 19:18:25.481094 omigo_matel-0.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:18:25.477094 omigo_matel-0.5.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:18:25.481094 omigo_matel-0.5.2/src/omigo_matel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:16:29.000000 omigo_matel-0.5.2/src/omigo_matel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:18:25.481094 omigo_matel-0.5.2/src/omigo_matel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-25 19:18:25.000000 omigo_matel-0.5.2/src/omigo_matel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-25 19:18:25.000000 omigo_matel-0.5.2/src/omigo_matel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 19:18:25.000000 omigo_matel-0.5.2/src/omigo_matel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-25 19:18:25.000000 omigo_matel-0.5.2/src/omigo_matel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-25 19:18:25.000000 omigo_matel-0.5.2/src/omigo_matel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:43:06.269063 omigo_matel-0.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-18 23:43:06.269063 omigo_matel-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 23:41:26.000000 omigo_matel-0.5.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-18 23:41:26.000000 omigo_matel-0.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-18 23:43:06.269063 omigo_matel-0.5.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:43:06.265062 omigo_matel-0.5.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:43:06.269063 omigo_matel-0.5.5/src/omigo_matel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 23:41:26.000000 omigo_matel-0.5.5/src/omigo_matel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:43:06.269063 omigo_matel-0.5.5/src/omigo_matel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-18 23:43:06.000000 omigo_matel-0.5.5/src/omigo_matel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-18 23:43:06.000000 omigo_matel-0.5.5/src/omigo_matel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 23:43:06.000000 omigo_matel-0.5.5/src/omigo_matel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-18 23:43:06.000000 omigo_matel-0.5.5/src/omigo_matel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-18 23:43:06.000000 omigo_matel-0.5.5/src/omigo_matel.egg-info/top_level.txt
```

### Comparing `omigo_matel-0.5.2/PKG-INFO` & `omigo_matel-0.5.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omigo_matel
-Version: 0.5.2
+Version: 0.5.5
 Summary: Data Analytics Library for Python
 Home-page: https://github.com/CrowdStrike/omigo-data-analytics
 Author: amit jaiswal
 Author-email: amit.jaiswal@gmail.com
 Project-URL: Bug Tracker, https://github.com/CrowdStrike/omigo-data-analytics/browse
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `omigo_matel-0.5.2/setup.cfg` & `omigo_matel-0.5.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = omigo_matel
-version = 0.5.2
+version = 0.5.5
 author = amit jaiswal
 author_email = amit.jaiswal@gmail.com
 description = Data Analytics Library for Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CrowdStrike/omigo-data-analytics
 project_urls =
```

### Comparing `omigo_matel-0.5.2/src/omigo_matel.egg-info/PKG-INFO` & `omigo_matel-0.5.5/src/omigo_matel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omigo-matel
-Version: 0.5.2
+Version: 0.5.5
 Summary: Data Analytics Library for Python
 Home-page: https://github.com/CrowdStrike/omigo-data-analytics
 Author: amit jaiswal
 Author-email: amit.jaiswal@gmail.com
 Project-URL: Bug Tracker, https://github.com/CrowdStrike/omigo-data-analytics/browse
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

