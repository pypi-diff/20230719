# Comparing `tmp/omigo_ext-0.5.3.tar.gz` & `tmp/omigo_ext-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omigo_ext-0.5.3.tar", last modified: Tue Jul 18 22:40:29 2023, max compression
+gzip compressed data, was "omigo_ext-0.5.4.tar", last modified: Tue Jul 18 23:33:09 2023, max compression
```

## Comparing `omigo_ext-0.5.3.tar` & `omigo_ext-0.5.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:40:29.459624 omigo_ext-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-18 22:40:29.459624 omigo_ext-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 22:39:56.000000 omigo_ext-0.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-18 22:39:56.000000 omigo_ext-0.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-18 22:40:29.459624 omigo_ext-0.5.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:40:29.455624 omigo_ext-0.5.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:40:29.459624 omigo_ext-0.5.3/src/omigo_ext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 22:39:56.000000 omigo_ext-0.5.3/src/omigo_ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-18 22:39:56.000000 omigo_ext-0.5.3/src/omigo_ext/etl_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-07-18 22:39:56.000000 omigo_ext-0.5.3/src/omigo_ext/geomap_viz.py
--rw-r--r--   0 runner    (1001) docker     (123)    16665 2023-07-18 22:39:56.000000 omigo_ext-0.5.3/src/omigo_ext/graph_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-07-18 22:39:56.000000 omigo_ext-0.5.3/src/omigo_ext/graphviz_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     8274 2023-07-18 22:39:56.000000 omigo_ext-0.5.3/src/omigo_ext/jira_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-18 22:39:56.000000 omigo_ext-0.5.3/src/omigo_ext/kafka_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-07-18 22:39:56.000000 omigo_ext-0.5.3/src/omigo_ext/multithread_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-07-18 22:39:56.000000 omigo_ext-0.5.3/src/omigo_ext/ws_ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:40:29.459624 omigo_ext-0.5.3/src/omigo_ext.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-18 22:40:29.000000 omigo_ext-0.5.3/src/omigo_ext.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-18 22:40:29.000000 omigo_ext-0.5.3/src/omigo_ext.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 22:40:29.000000 omigo_ext-0.5.3/src/omigo_ext.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-18 22:40:29.000000 omigo_ext-0.5.3/src/omigo_ext.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 22:40:29.000000 omigo_ext-0.5.3/src/omigo_ext.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:33:09.570848 omigo_ext-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-18 23:33:09.570848 omigo_ext-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 23:32:36.000000 omigo_ext-0.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-18 23:32:36.000000 omigo_ext-0.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-18 23:33:09.570848 omigo_ext-0.5.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:33:09.566847 omigo_ext-0.5.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:33:09.570848 omigo_ext-0.5.4/src/omigo_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 23:32:36.000000 omigo_ext-0.5.4/src/omigo_ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-18 23:32:36.000000 omigo_ext-0.5.4/src/omigo_ext/etl_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-07-18 23:32:36.000000 omigo_ext-0.5.4/src/omigo_ext/geomap_viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16665 2023-07-18 23:32:36.000000 omigo_ext-0.5.4/src/omigo_ext/graph_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-07-18 23:32:36.000000 omigo_ext-0.5.4/src/omigo_ext/graphviz_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8274 2023-07-18 23:32:36.000000 omigo_ext-0.5.4/src/omigo_ext/jira_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-18 23:32:36.000000 omigo_ext-0.5.4/src/omigo_ext/kafka_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-07-18 23:32:36.000000 omigo_ext-0.5.4/src/omigo_ext/multithread_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-07-18 23:32:36.000000 omigo_ext-0.5.4/src/omigo_ext/ws_ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:33:09.570848 omigo_ext-0.5.4/src/omigo_ext.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-18 23:33:09.000000 omigo_ext-0.5.4/src/omigo_ext.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-18 23:33:09.000000 omigo_ext-0.5.4/src/omigo_ext.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 23:33:09.000000 omigo_ext-0.5.4/src/omigo_ext.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-18 23:33:09.000000 omigo_ext-0.5.4/src/omigo_ext.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 23:33:09.000000 omigo_ext-0.5.4/src/omigo_ext.egg-info/top_level.txt
```

### Comparing `omigo_ext-0.5.3/setup.cfg` & `omigo_ext-0.5.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = omigo_ext
-version = 0.5.3
+version = 0.5.4
 author = amit jaiswal
 author_email = amit.jaiswal@gmail.com
 description = Extensions for omigo_core package
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CrowdStrike/omigo-data-analytics
 project_urls =
```

### Comparing `omigo_ext-0.5.3/src/omigo_ext/etl_ext.py` & `omigo_ext-0.5.4/src/omigo_ext/etl_ext.py`

 * *Files identical despite different names*

### Comparing `omigo_ext-0.5.3/src/omigo_ext/geomap_viz.py` & `omigo_ext-0.5.4/src/omigo_ext/geomap_viz.py`

 * *Files identical despite different names*

### Comparing `omigo_ext-0.5.3/src/omigo_ext/graph_ext.py` & `omigo_ext-0.5.4/src/omigo_ext/graph_ext.py`

 * *Files identical despite different names*

### Comparing `omigo_ext-0.5.3/src/omigo_ext/graphviz_ext.py` & `omigo_ext-0.5.4/src/omigo_ext/graphviz_ext.py`

 * *Files identical despite different names*

### Comparing `omigo_ext-0.5.3/src/omigo_ext/jira_ext.py` & `omigo_ext-0.5.4/src/omigo_ext/jira_ext.py`

 * *Files identical despite different names*

### Comparing `omigo_ext-0.5.3/src/omigo_ext/kafka_ext.py` & `omigo_ext-0.5.4/src/omigo_ext/kafka_ext.py`

 * *Files identical despite different names*

### Comparing `omigo_ext-0.5.3/src/omigo_ext/multithread_ext.py` & `omigo_ext-0.5.4/src/omigo_ext/multithread_ext.py`

 * *Files identical despite different names*

### Comparing `omigo_ext-0.5.3/src/omigo_ext/ws_ext.py` & `omigo_ext-0.5.4/src/omigo_ext/ws_ext.py`

 * *Files identical despite different names*

