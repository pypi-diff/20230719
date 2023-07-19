# Comparing `tmp/polyapi-5.7.0.4.tar.gz` & `tmp/polyapi-5.7.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyapi-5.7.0.4.tar", last modified: Thu Apr 20 09:00:46 2023, max compression
+gzip compressed data, was "polyapi-5.7.0.6.tar", last modified: Wed Jul 19 08:25:40 2023, max compression
```

## Comparing `polyapi-5.7.0.4.tar` & `polyapi-5.7.0.6.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 artem     (1000) artem     (1000)        0 2023-04-20 09:00:46.262089 polyapi-5.7.0.4/
--rw-r--r--   0 artem     (1000) artem     (1000)     1061 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/LICENSE.txt
--rw-r--r--   0 artem     (1000) artem     (1000)     1547 2023-04-20 09:00:46.262089 polyapi-5.7.0.4/PKG-INFO
--rw-r--r--   0 artem     (1000) artem     (1000)     1048 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/README.txt
-drwxr-xr-x   0 artem     (1000) artem     (1000)        0 2023-04-20 09:00:46.252089 polyapi-5.7.0.4/polyapi.egg-info/
--rw-r--r--   0 artem     (1000) artem     (1000)     1547 2023-04-20 09:00:46.000000 polyapi-5.7.0.4/polyapi.egg-info/PKG-INFO
--rw-r--r--   0 artem     (1000) artem     (1000)     1547 2023-04-20 09:00:46.000000 polyapi-5.7.0.4/polyapi.egg-info/SOURCES.txt
--rw-r--r--   0 artem     (1000) artem     (1000)        1 2023-04-20 09:00:46.000000 polyapi-5.7.0.4/polyapi.egg-info/dependency_links.txt
--rw-r--r--   0 artem     (1000) artem     (1000)       27 2023-04-20 09:00:46.000000 polyapi-5.7.0.4/polyapi.egg-info/requires.txt
--rw-r--r--   0 artem     (1000) artem     (1000)       11 2023-04-20 09:00:46.000000 polyapi-5.7.0.4/polyapi.egg-info/top_level.txt
-drwxr-xr-x   0 artem     (1000) artem     (1000)        0 2023-04-20 09:00:46.252089 polyapi-5.7.0.4/polymatica/
--rw-r--r--   0 artem     (1000) artem     (1000)      153 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/__init__.py
--rw-r--r--   0 artem     (1000) artem     (1000)     8939 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/authorization.py
--rw-r--r--   0 artem     (1000) artem     (1000)     3686 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/business_logic_doc.py
--rw-r--r--   0 artem     (1000) artem     (1000)   411436 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/business_scenarios.py
-drwxr-xr-x   0 artem     (1000) artem     (1000)        0 2023-04-20 09:00:46.252089 polyapi-5.7.0.4/polymatica/commands/
--rw-r--r--   0 artem     (1000) artem     (1000)      298 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/commands/__init__.py
--rw-r--r--   0 artem     (1000) artem     (1000)     4098 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/commands/base_command.py
--rw-r--r--   0 artem     (1000) artem     (1000)     3118 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/commands/olap_module.py
--rw-r--r--   0 artem     (1000) artem     (1000)     1884 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/commands/other_modules.py
-drwxr-xr-x   0 artem     (1000) artem     (1000)        0 2023-04-20 09:00:46.252089 polyapi-5.7.0.4/polymatica/common/
--rw-r--r--   0 artem     (1000) artem     (1000)      353 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/common/__init__.py
--rw-r--r--   0 artem     (1000) artem     (1000)     4821 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/common/consts.py
--rw-r--r--   0 artem     (1000) artem     (1000)    18721 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/common/helper_funcs.py
--rw-r--r--   0 artem     (1000) artem     (1000)    37161 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/error_handler.py
--rw-r--r--   0 artem     (1000) artem     (1000)     4765 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/exceptions.py
--rw-r--r--   0 artem     (1000) artem     (1000)    17499 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/executor.py
-drwxr-xr-x   0 artem     (1000) artem     (1000)        0 2023-04-20 09:00:46.252089 polyapi-5.7.0.4/polymatica/graph/
--rw-r--r--   0 artem     (1000) artem     (1000)      136 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/graph/__init__.py
--rw-r--r--   0 artem     (1000) artem     (1000)    21693 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/graph/base_graph.py
--rw-r--r--   0 artem     (1000) artem     (1000)    21384 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/graph/graph_interface.py
-drwxr-xr-x   0 artem     (1000) artem     (1000)        0 2023-04-20 09:00:46.262089 polyapi-5.7.0.4/polymatica/graph/types/
--rw-r--r--   0 artem     (1000) artem     (1000)      668 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/graph/types/__init__.py
--rw-r--r--   0 artem     (1000) artem     (1000)     2485 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/graph/types/areas.py
--rw-r--r--   0 artem     (1000) artem     (1000)     3631 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/graph/types/balls.py
--rw-r--r--   0 artem     (1000) artem     (1000)     2498 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/graph/types/chord.py
--rw-r--r--   0 artem     (1000) artem     (1000)     4067 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/graph/types/circles.py
--rw-r--r--   0 artem     (1000) artem     (1000)     3652 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/graph/types/circles_series.py
--rw-r--r--   0 artem     (1000) artem     (1000)     4641 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/graph/types/corridors.py
--rw-r--r--   0 artem     (1000) artem     (1000)     3132 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/graph/types/cumulative_areas.py
--rw-r--r--   0 artem     (1000) artem     (1000)     3518 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/graph/types/cumulative_cylinders.py
--rw-r--r--   0 artem     (1000) artem     (1000)     3603 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/graph/types/cylinders.py
--rw-r--r--   0 artem     (1000) artem     (1000)     8064 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/graph/types/graph.py
--rw-r--r--   0 artem     (1000) artem     (1000)     3278 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/graph/types/lines.py
--rw-r--r--   0 artem     (1000) artem     (1000)     3972 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/graph/types/pies.py
--rw-r--r--   0 artem     (1000) artem     (1000)     3966 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/graph/types/point.py
--rw-r--r--   0 artem     (1000) artem     (1000)     3897 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/graph/types/point_series.py
--rw-r--r--   0 artem     (1000) artem     (1000)     3579 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/graph/types/pools.py
--rw-r--r--   0 artem     (1000) artem     (1000)     3403 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/graph/types/pools_3d.py
--rw-r--r--   0 artem     (1000) artem     (1000)     2242 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/graph/types/radar.py
--rw-r--r--   0 artem     (1000) artem     (1000)     1903 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/graph/types/sankey.py
--rw-r--r--   0 artem     (1000) artem     (1000)     3605 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/graph/types/surface.py
--rw-r--r--   0 artem     (1000) artem     (1000)    20352 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/helper.py
-drwxr-xr-x   0 artem     (1000) artem     (1000)        0 2023-04-20 09:00:46.262089 polyapi-5.7.0.4/polymatica/versions/
--rw-r--r--   0 artem     (1000) artem     (1000)      260 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/versions/__init__.py
--rw-r--r--   0 artem     (1000) artem     (1000)    10603 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/versions/polymatica_57.py
--rw-r--r--   0 artem     (1000) artem     (1000)     1600 2023-04-20 08:52:18.000000 polyapi-5.7.0.4/polymatica/versions/versions_redirect.py
--rw-r--r--   0 artem     (1000) artem     (1000)       38 2023-04-20 09:00:46.262089 polyapi-5.7.0.4/setup.cfg
--rw-r--r--   0 artem     (1000) artem     (1000)      759 2023-04-20 08:57:01.000000 polyapi-5.7.0.4/setup.py
+drwxr-xr-x   0 artem     (1000) artem     (1000)        0 2023-07-19 08:25:40.078790 polyapi-5.7.0.6/
+-rw-r--r--   0 artem     (1000) artem     (1000)     1061 2023-07-19 08:24:44.000000 polyapi-5.7.0.6/LICENSE.txt
+-rw-r--r--   0 artem     (1000) artem     (1000)     1550 2023-07-19 08:25:40.078790 polyapi-5.7.0.6/PKG-INFO
+-rw-r--r--   0 artem     (1000) artem     (1000)     1042 2023-07-19 08:24:44.000000 polyapi-5.7.0.6/README.txt
+drwxr-xr-x   0 artem     (1000) artem     (1000)        0 2023-07-19 08:25:40.068790 polyapi-5.7.0.6/polyapi.egg-info/
+-rw-r--r--   0 artem     (1000) artem     (1000)     1550 2023-07-19 08:25:39.000000 polyapi-5.7.0.6/polyapi.egg-info/PKG-INFO
+-rw-r--r--   0 artem     (1000) artem     (1000)     1547 2023-07-19 08:25:40.000000 polyapi-5.7.0.6/polyapi.egg-info/SOURCES.txt
+-rw-r--r--   0 artem     (1000) artem     (1000)        1 2023-07-19 08:25:39.000000 polyapi-5.7.0.6/polyapi.egg-info/dependency_links.txt
+-rw-r--r--   0 artem     (1000) artem     (1000)       27 2023-07-19 08:25:39.000000 polyapi-5.7.0.6/polyapi.egg-info/requires.txt
+-rw-r--r--   0 artem     (1000) artem     (1000)       11 2023-07-19 08:25:39.000000 polyapi-5.7.0.6/polyapi.egg-info/top_level.txt
+drwxr-xr-x   0 artem     (1000) artem     (1000)        0 2023-07-19 08:25:40.078790 polyapi-5.7.0.6/polymatica/
+-rw-r--r--   0 artem     (1000) artem     (1000)      153 2023-07-19 08:24:44.000000 polyapi-5.7.0.6/polymatica/__init__.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     8939 2023-07-19 08:24:44.000000 polyapi-5.7.0.6/polymatica/authorization.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     3686 2023-07-19 08:24:44.000000 polyapi-5.7.0.6/polymatica/business_logic_doc.py
+-rw-r--r--   0 artem     (1000) artem     (1000)   419073 2023-07-19 08:24:44.000000 polyapi-5.7.0.6/polymatica/business_scenarios.py
+drwxr-xr-x   0 artem     (1000) artem     (1000)        0 2023-07-19 08:25:40.078790 polyapi-5.7.0.6/polymatica/commands/
+-rw-r--r--   0 artem     (1000) artem     (1000)      298 2023-07-19 08:24:44.000000 polyapi-5.7.0.6/polymatica/commands/__init__.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     4098 2023-07-19 08:24:44.000000 polyapi-5.7.0.6/polymatica/commands/base_command.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     3118 2023-07-19 08:24:44.000000 polyapi-5.7.0.6/polymatica/commands/olap_module.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     1884 2023-07-19 08:24:44.000000 polyapi-5.7.0.6/polymatica/commands/other_modules.py
+drwxr-xr-x   0 artem     (1000) artem     (1000)        0 2023-07-19 08:25:40.078790 polyapi-5.7.0.6/polymatica/common/
+-rw-r--r--   0 artem     (1000) artem     (1000)      353 2023-07-19 08:24:44.000000 polyapi-5.7.0.6/polymatica/common/__init__.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     4821 2023-07-19 08:24:44.000000 polyapi-5.7.0.6/polymatica/common/consts.py
+-rw-r--r--   0 artem     (1000) artem     (1000)    18721 2023-07-19 08:24:44.000000 polyapi-5.7.0.6/polymatica/common/helper_funcs.py
+-rw-r--r--   0 artem     (1000) artem     (1000)    37315 2023-07-19 08:24:44.000000 polyapi-5.7.0.6/polymatica/error_handler.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     4765 2023-07-19 08:24:44.000000 polyapi-5.7.0.6/polymatica/exceptions.py
+-rw-r--r--   0 artem     (1000) artem     (1000)    17499 2023-07-19 08:24:44.000000 polyapi-5.7.0.6/polymatica/executor.py
+drwxr-xr-x   0 artem     (1000) artem     (1000)        0 2023-07-19 08:25:40.078790 polyapi-5.7.0.6/polymatica/graph/
+-rw-r--r--   0 artem     (1000) artem     (1000)      136 2023-07-19 08:24:44.000000 polyapi-5.7.0.6/polymatica/graph/__init__.py
+-rw-r--r--   0 artem     (1000) artem     (1000)    21693 2023-07-19 08:24:44.000000 polyapi-5.7.0.6/polymatica/graph/base_graph.py
+-rw-r--r--   0 artem     (1000) artem     (1000)    21384 2023-07-19 08:24:44.000000 polyapi-5.7.0.6/polymatica/graph/graph_interface.py
+drwxr-xr-x   0 artem     (1000) artem     (1000)        0 2023-07-19 08:25:40.078790 polyapi-5.7.0.6/polymatica/graph/types/
+-rw-r--r--   0 artem     (1000) artem     (1000)      668 2023-07-19 08:24:44.000000 polyapi-5.7.0.6/polymatica/graph/types/__init__.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     2485 2023-07-19 08:24:44.000000 polyapi-5.7.0.6/polymatica/graph/types/areas.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     3631 2023-07-19 08:24:44.000000 polyapi-5.7.0.6/polymatica/graph/types/balls.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     2498 2023-07-19 08:24:44.000000 polyapi-5.7.0.6/polymatica/graph/types/chord.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     4067 2023-07-19 08:24:44.000000 polyapi-5.7.0.6/polymatica/graph/types/circles.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     3652 2023-07-19 08:24:44.000000 polyapi-5.7.0.6/polymatica/graph/types/circles_series.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     4641 2023-07-19 08:24:44.000000 polyapi-5.7.0.6/polymatica/graph/types/corridors.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     3132 2023-07-19 08:24:44.000000 polyapi-5.7.0.6/polymatica/graph/types/cumulative_areas.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     3518 2023-07-19 08:24:44.000000 polyapi-5.7.0.6/polymatica/graph/types/cumulative_cylinders.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     3603 2023-07-19 08:24:44.000000 polyapi-5.7.0.6/polymatica/graph/types/cylinders.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     8064 2023-07-19 08:24:44.000000 polyapi-5.7.0.6/polymatica/graph/types/graph.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     3278 2023-07-19 08:24:44.000000 polyapi-5.7.0.6/polymatica/graph/types/lines.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     3972 2023-07-19 08:24:44.000000 polyapi-5.7.0.6/polymatica/graph/types/pies.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     3966 2023-07-19 08:24:44.000000 polyapi-5.7.0.6/polymatica/graph/types/point.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     3897 2023-07-19 08:24:44.000000 polyapi-5.7.0.6/polymatica/graph/types/point_series.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     3579 2023-07-19 08:24:44.000000 polyapi-5.7.0.6/polymatica/graph/types/pools.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     3403 2023-07-19 08:24:44.000000 polyapi-5.7.0.6/polymatica/graph/types/pools_3d.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     2242 2023-07-19 08:24:44.000000 polyapi-5.7.0.6/polymatica/graph/types/radar.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     1903 2023-07-19 08:24:44.000000 polyapi-5.7.0.6/polymatica/graph/types/sankey.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     3605 2023-07-19 08:24:44.000000 polyapi-5.7.0.6/polymatica/graph/types/surface.py
+-rw-r--r--   0 artem     (1000) artem     (1000)    20352 2023-07-19 08:24:44.000000 polyapi-5.7.0.6/polymatica/helper.py
+drwxr-xr-x   0 artem     (1000) artem     (1000)        0 2023-07-19 08:25:40.078790 polyapi-5.7.0.6/polymatica/versions/
+-rw-r--r--   0 artem     (1000) artem     (1000)      260 2023-07-19 08:24:44.000000 polyapi-5.7.0.6/polymatica/versions/__init__.py
+-rw-r--r--   0 artem     (1000) artem     (1000)    10979 2023-07-19 08:24:44.000000 polyapi-5.7.0.6/polymatica/versions/polymatica_57.py
+-rw-r--r--   0 artem     (1000) artem     (1000)     1600 2023-07-19 08:24:44.000000 polyapi-5.7.0.6/polymatica/versions/versions_redirect.py
+-rw-r--r--   0 artem     (1000) artem     (1000)       38 2023-07-19 08:25:40.078790 polyapi-5.7.0.6/setup.cfg
+-rw-r--r--   0 artem     (1000) artem     (1000)      759 2023-07-19 08:24:44.000000 polyapi-5.7.0.6/setup.py
```

### Comparing `polyapi-5.7.0.4/LICENSE.txt` & `polyapi-5.7.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.4/PKG-INFO` & `polyapi-5.7.0.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyapi
-Version: 5.7.0.4
+Version: 5.7.0.6
 Summary: Wrapper for Polymatica API
 Home-page: https://www.polymatica.ru
 Author: Polymatica Rus LLC
 Author-email: development@polymatica.com
 License: MIT
 Keywords: polymatica
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,14 +12,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE.txt
 
 Библиотека предназначенна для работы с Polymatica API.
 
-Основным модулем бизнес-логики является файл business_scenarios.py, импортировать который можно с помощью команды ``from polyapi import business_scenarios as sc``.
+Основным модулем бизнес-логики является файл business_scenarios.py, импортировать который можно с помощью команды ``from polymatica import business_scenarios as sc``.
 
 Модуль предоставляет два класса для работы с Полиматикой - ``BusinessLogic`` и ``GetDataChunk``. Методы этих классов можно посмотреть при помощи стандартной функции ``dir()``.
 
 Аргументы функций и прочую docstring-документацию модуля и функций можно посмотреть при помощи стандартной функции ``help()``.
 
 Инициализация нового клиентского подключения: ``client = sc.BusinessLogic(login="your_login", password="your_password", url="polymatica_server_url", **args)``
```

### Comparing `polyapi-5.7.0.4/README.txt` & `polyapi-5.7.0.6/README.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Библиотека предназначенна для работы с Polymatica API.
-
-Основным модулем бизнес-логики является файл business_scenarios.py, импортировать который можно с помощью команды ``from polyapi import business_scenarios as sc``.
-
-Модуль предоставляет два класса для работы с Полиматикой - ``BusinessLogic`` и ``GetDataChunk``. Методы этих классов можно посмотреть при помощи стандартной функции ``dir()``.
-
-Аргументы функций и прочую docstring-документацию модуля и функций можно посмотреть при помощи стандартной функции ``help()``.
-
-Инициализация нового клиентского подключения: ``client = sc.BusinessLogic(login="your_login", password="your_password", url="polymatica_server_url", **args)``
+Библиотека предназначенна для работы с Polymatica API.
+
+Основным модулем бизнес-логики является файл business_scenarios.py, импортировать который можно с помощью команды ``from polymatica import business_scenarios as sc``.
+
+Модуль предоставляет два класса для работы с Полиматикой - ``BusinessLogic`` и ``GetDataChunk``. Методы этих классов можно посмотреть при помощи стандартной функции ``dir()``.
+
+Аргументы функций и прочую docstring-документацию модуля и функций можно посмотреть при помощи стандартной функции ``help()``.
+
+Инициализация нового клиентского подключения: ``client = sc.BusinessLogic(login="your_login", password="your_password", url="polymatica_server_url", **args)``
```

### Comparing `polyapi-5.7.0.4/polyapi.egg-info/PKG-INFO` & `polyapi-5.7.0.6/polyapi.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyapi
-Version: 5.7.0.4
+Version: 5.7.0.6
 Summary: Wrapper for Polymatica API
 Home-page: https://www.polymatica.ru
 Author: Polymatica Rus LLC
 Author-email: development@polymatica.com
 License: MIT
 Keywords: polymatica
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,14 +12,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE.txt
 
 Библиотека предназначенна для работы с Polymatica API.
 
-Основным модулем бизнес-логики является файл business_scenarios.py, импортировать который можно с помощью команды ``from polyapi import business_scenarios as sc``.
+Основным модулем бизнес-логики является файл business_scenarios.py, импортировать который можно с помощью команды ``from polymatica import business_scenarios as sc``.
 
 Модуль предоставляет два класса для работы с Полиматикой - ``BusinessLogic`` и ``GetDataChunk``. Методы этих классов можно посмотреть при помощи стандартной функции ``dir()``.
 
 Аргументы функций и прочую docstring-документацию модуля и функций можно посмотреть при помощи стандартной функции ``help()``.
 
 Инициализация нового клиентского подключения: ``client = sc.BusinessLogic(login="your_login", password="your_password", url="polymatica_server_url", **args)``
```

### Comparing `polyapi-5.7.0.4/polyapi.egg-info/SOURCES.txt` & `polyapi-5.7.0.6/polyapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.4/polymatica/authorization.py` & `polyapi-5.7.0.6/polymatica/authorization.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.4/polymatica/business_logic_doc.py` & `polyapi-5.7.0.6/polymatica/business_logic_doc.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.4/polymatica/business_scenarios.py` & `polyapi-5.7.0.6/polymatica/business_scenarios.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 """
 Модуль работы с бизнес-сценариями Полиматики.
 """
-
+import math
 # Default lib
 
 import os
 import re
 import time
 import ast
 import datetime
@@ -38,14 +38,16 @@
 
 # ----------------------------------------------------------------------------------------------------------------------
 
 # настройка логирования
 logger = logging.getLogger(__name__)
 logger.addHandler(NullHandler())
 
+UNITS_LOAD_DATA_CHUNK = 1000
+
 
 # ----------------------------------------------------------------------------------------------------------------------
 
 class BusinessLogic:
     """
     Базовый класс, описывающий бизнес-сценарии использования Полиматики.
     Используемые переменные класса:
@@ -1011,20 +1013,21 @@
         config_data = self.execute_manager_command(command_name='user_iface', state='get_configuration')
         configuration, datetime_field = self.h.parse_result(config_data, 'configuration'), 'datetime_format'
         if datetime_field not in configuration or not configuration[datetime_field]:
             return ISO_DATE_FORMAT
         return configuration[datetime_field]
 
     @timing
-    def put_dim_filter(self, dim_name: str, filter_name: Union[str, List, None] = None,
+    def put_dim_filter(self, dim_name: str = None, filter_name: Union[str, List, None] = None,
                        start_date: Union[int, str] = None, end_date: Union[int, str] = None,
-                       filter_field_format: Union[str, None] = None) -> Dict:
+                       filter_field_format: Union[str, None] = None, dim_id: str = None) -> Dict:
         """
         Установка фильтра по размерностям.
         :param dim_name: (str) Название размерности, по которой производится фильтрация.
+        :param dim_id: (str) ID размерности, по которой производится фильтрация.
         :param filter_name: (Union[str, List, None]) Название фильтра;
             может быть задано строкой (один фильтр) или списком (несколько фильтров);
             в случае, если нужно указать интервал дат, необходимо передать None.
         :params start_date, end_date: (Union[int, str]) Начальная и конечная дата фильтрации соответственно.
             Начальная и конечная дата фильтрации формируют по сути интервал дат.
             Несколько особенностей задания этих параметров:
                 1. Если используются месяцы, то необходимо использовать следующие значения (с учётом регистра):
@@ -1053,20 +1056,20 @@
             Если в актуальном случае этот параметр не указан, то будет получено системное значение из Полиматики.
             Параметр необходим для корректной фильтрации даты-времени.
         :return: (Dict) результат команды ("filter", "apply_data").
         """
         # заполнение списка dates_list в зависимости от содержания параметров filter_name, start_date, end_date
         try:
             dates_list = error_handler.checks(
-                self, self.func_name, filter_name, start_date, end_date, filter_field_format)
+                self, self.func_name, filter_name, start_date, end_date, filter_field_format, dim_name, dim_id)
         except Exception as e:
             return self._raise_exception(PolymaticaException, str(e))
 
         # получение id размерности
-        dim_id = self.get_dim_id(dim_name)
+        dim_id = dim_id or self.get_dim_id(dim_name)
 
         # Наложить фильтр на размерность (в неактивной области)
         # получение списка активных и неактивных фильтров
         result = self.h.get_filter_rows(dim_id)
         filters_list = self.h.parse_result(result=result, key="data")  # получить названия фильтров
         filters_values = self.h.parse_result(result=result, key="marks")  # получить список on/off [0,0,...,0]
 
@@ -1862,14 +1865,27 @@
         # проверка прав на сценарий (на все ли мультисферы, участвующие в сценарии, пользователь имеет права)
         self._check_scenario_cubes_permission(scenario_id)
 
         # запуск сценария в зависимости от версии Полиматики
         self.version_redirect.invoke_method('_run_scenario_impl', scenario_id=scenario_id, scenario_name=scenario_name)
 
     @timing
+    def run_scenario_on_layer(self, scenario_id: str, layer_id: str):
+        # проверка прав на сценарий (на все ли мультисферы, участвующие в сценарии, пользователь имеет права)
+        self._check_scenario_cubes_permission(scenario_id)
+
+        # запуск сценария в зависимости от версии Полиматики
+        self.version_redirect.invoke_method('_run_scenario_on_layer_impl', scenario_id=scenario_id, layer_id=layer_id)
+
+    def _run_scenario_on_layer_impl(self, scenario_id: str, layer_id: str):
+        self._raise_exception(PolymaticaException,
+                              "This method available only since 5.7 version, current version: {}".format(
+                                  self.polymatica_version))
+
+    @timing
     def run_scenario_by_id(self, sc_id: str) -> Dict:
         """
         Запустить сценарий по его идентификатору.
         Метод актуален только для версии Polymatica 5.6.
         При вызове на версии Polymatica 5.7 и выше будет сгенерирована ошибка.
         :param sc_id: (str) идентификатор запускаемого сценария.
         :return: (Dict) Результат команды ("script", "run").
@@ -1901,15 +1917,16 @@
 
         # если такого пользователя нет - генерируем ошибку
         return self._raise_exception(
             UserNotFoundError, 'User with login "{}" not found!'.format(user_name), with_traceback=False)
 
     @timing
     def run_scenario_by_user(self, scenario_name: str, user_name: str,
-                             user_password: str = None, units: int = 500, timeout: int = None) -> Tuple:
+                             user_password: str = None, units: int = UNITS_LOAD_DATA_CHUNK,
+                             timeout: int = None) -> Tuple:
         """
         Запустить сценарий от имени заданного пользователя и дождаться его загрузки. Если по каким-то причинам
         невозможно дождаться загрузки выбранного сценария (не отвечает сервер Полиматики или сервер вернул невалидный
         статус), то будет сгенерирована ошибка.
         :param scenario_name: (str) название сценария.
         :param user_name: (str) имя пользователя, под которым запускается сценарий.
         :param user_password: (str) пароль пользователя, под которым запускается сценарий;
@@ -2001,15 +2018,15 @@
                 if not column:
                     top_columns[i] = top_columns[i - 1]
             columns_result.insert(0, top_columns)
         return columns_result, top_dims_count, left_dims_count
 
     @timing
     def get_data_frame(self,
-                       units: int = 100,
+                       units: int = UNITS_LOAD_DATA_CHUNK,
                        show_all_columns: bool = False,
                        show_all_rows: bool = False
                        ) -> Tuple[pd.DataFrame, pd.DataFrame]:
         """
         Генератор, подгружающий мультисферу постранично (порциями строк).
         Подразумевается, что перед вызовом метода вся иерархия данных в мультисфере будет раскрыта,
         иначе будут возвращаться неполные данные.
@@ -2695,15 +2712,15 @@
             # обновляем общее число строк мультисферы и сохраняем идентификаторы всех слоёв
             if multisphere_module_id:
                 self.set_multisphere_module_id(multisphere_module_id)
                 self.layers_list = list(new_layers)
                 self.update_total_row()
             return result
 
-    def _convert_schedule_item(self, time_zones: dict, user_schedule: dict):
+    def _convert_schedule_item(self, time_zones: Dict, user_schedule: Dict):
         """
         Подготовка пользовательского планировщика.
         """
         if not user_schedule:
             return
 
         # установить значение периода для запроса
@@ -2716,16 +2733,16 @@
 
         # преобразование времени в UNIX time
         h_m = user_schedule["time"].split(":")
         d = datetime.datetime(1970, 1, 1, int(h_m[0]) + 3, int(h_m[1]), 0)
         user_schedule["time"] = int(time.mktime(d.timetuple()))
 
     @timing
-    def create_sphere(self, cube_name: str, source_name: str, file_type: str, update_params: dict,
-                      sql_params: dict = None, user_interval: str = "с текущего дня", filepath: str = str(),
+    def create_sphere(self, cube_name: str, source_name: str, file_type: str, update_params: Dict,
+                      sql_params: Dict = None, user_interval: str = "с текущего дня", filepath: str = str(),
                       separator: str = str(), increment_dim: str = str(), interval_dim: str = str(),
                       interval_borders: list = None, encoding: str = str(), delayed: bool = False) -> dict:
         """
         Создать новый куб.
         :param cube_name: (str) название создаваемого куба, должно состоять из 5 и более символов.
         :param source_name: (str) название источника данных,
             название не должно содержать пробелов, и длина должна быть больше 5 символов.
@@ -2988,15 +3005,15 @@
 
         # и, наконец, создаём сферу с нужными параметрами
         self.func_name = "create_sphere"
         return self.execute_manager_command(
             command_name="user_cube", state="save_ext_info_several_sources_request", **command_params)
 
     @timing
-    def update_cube(self, cube_name: str, update_params: dict, user_interval: str = "с текущего дня",
+    def update_cube(self, cube_name: str, update_params: Dict, user_interval: str = "с текущего дня",
                     delayed: bool = False, increment_dim: str = str(),
                     interval_dim: str = str(), interval_borders: list = None) -> dict:
         """
         Обновить существующий куб.
         :param cube_name: (str) название обновляемого куба.
         :param update_params: (dict) параметры обновления мультисферы; имеет структуру:
             {
@@ -3726,15 +3743,15 @@
         # склонировать права пользователя
         if clone_user:
             clone_user_permissions = {
                 k: v for data in users_data for k, v in data.items() if data["login"] == clone_user}
             user_permissions = {k: v for data in users_data for k, v in data.items() if data["login"] == user_name}
             requested_uuid = clone_user_permissions["uuid"]
             clone_user_permissions["login"], clone_user_permissions["uuid"] = user_permissions["login"], \
-                                                                              user_permissions["uuid"]
+                user_permissions["uuid"]
             user_permissions = clone_user_permissions
         # или предоставить все права
         else:
             user_permissions = {k: v for data in users_data for k, v in data.items() if data["login"] == user_name}
             user_permissions["roles"] = ALL_PERMISSIONS
             requested_uuid = user_permissions["uuid"]
         # cubes permissions for user
@@ -3975,15 +3992,16 @@
 
         # если режим отображения тоталов был изменён, то возвращаем исходный режим, и возвращаем результат
         if need_change_total_mode:
             self.change_total_mode()
         return result
 
     @timing
-    def load_sphere_chunk(self, units: int = 100, convert_type: bool = False, default_value: Any = None,
+    def load_sphere_chunk(self, units: int = UNITS_LOAD_DATA_CHUNK, convert_type: bool = False,
+                          default_value: Any = None,
                           convert_empty_values: bool = True) -> Dict:
         """
         Генератор, подгружающий мультисферу постранично (порциями строк).
         Особенности использования метода:
             1. В мультисфере не должно быть вынесенных вверх размерностей, иначе будет сгенерировано исключение.
             2. Для корректного получения данных необходимо,
                 чтобы перед вызовом метода были развёрнуты все узлы мультисферы.
@@ -4447,51 +4465,62 @@
             return active_layer_id
 
         # подразумеваем, что в сессии единственный дефолтный (начальный) слой - вернём его идентификатор
         # если же по каким-то причинам и его нет, то вернём пустую строку, т.к. никаких вариантов больше нет
         layers = self.get_layer_list()
         return layers[0][0] if layers else str()
 
+    @timing
+    def get_active_layer_name(self) -> str:
+        """
+        Возвращает название активного слоя.
+        :return: (str) название слоя.
+        """
+        return self.execute_manager_command(command_name="user_layer",
+                                            state="get_layer",
+                                            layer_id=self.get_active_layer_id()
+                                            )['queries'][0]['command']['layer']['name']
+
     def _get_modules_in_layer(self, layer_id: str, is_int_type: bool = True) -> List:
         """
         Возвращает список модулей на заданном слое.
         :param layer_id: идентификатор слоя, модули которого необходимо получить.
         :param is_int_type: флаг, показывающий, в каком виде выводить тип модуля:
             в числовом (500) или строковом ('Мультисфера'). Соответствующая мапа переводов хранится в CODE_NAME_MAP.
-        :return: (list) список вида [[module_id, module_name, module_type], [...], ...],
+        :return: (list) список вида [[module_id, module_name, module_type, cube_id], [...], ...],
             содержащий информацию о модулях в текущем слое.
         """
         # получаем список всех модулей, находящихся в текущем слое
         settings = self.execute_manager_command(command_name="user_layer", state="get_layer", layer_id=layer_id)
         layer_info = self.h.parse_result(result=settings, key="layer") or dict()
 
         # проходя по каждому модулю, извлекаем из него информацию
         result = []
         for module in layer_info.get('module_descs'):
-            module_id, base_module_type = module.get('uuid'), module.get('type_id')
+            module_id, base_module_type, cube_id = module.get('uuid'), module.get('type_id'), module.get('cube_id')
             module_type = base_module_type if is_int_type else CODE_NAME_MAP.get(base_module_type, base_module_type)
 
             # имя модуля в этих настройках не указано - подгружаем отдельно и формируем общий результат
             module_setting = self.execute_manager_command(
                 command_name="user_iface", state="load_settings", module_id=module_id)
             module_info = self.h.parse_result(result=module_setting, key="settings") or dict()
-            result.append([module_id, module_info.get('title', str()), module_type])
+            result.append([module_id, module_info.get('title', str()), module_type, cube_id])
         return result
 
     @timing
     def get_module_list(self) -> List:
         """
         Возвращает список модулей в активном слое текущей сессии.
         :return: (list) список вида [[module_id, module_name, module_type], [...], ...],
             содержащий информацию о модулях на активном слое.
         :call_example:
             1. Инициализируем класс: bl_test = sc.BusinessLogic(login="login", password="password", url="url")
             2. Вызов метода:
                 module_list = bl_test.get_module_list()
-                output: [["module_id", "module_name', "module_type"], [...], ...] - список модулей в активном слое
+                output: [["module_id", "module_name', "module_type", "cube_id"], [...], ...] - список модулей в активном слое
                     в текущей сессии.
         """
         # получаем идентификатор активного слоя
         active_layer_id = self.get_active_layer_id()
         if not active_layer_id:
             return self._raise_exception(PolymaticaException, 'Active layer not set!', with_traceback=False)
 
@@ -4607,15 +4636,15 @@
             if len(error_modules) == len(ms_ids):
                 return self._raise_exception(PolymaticaException, message, with_traceback=False)
             else:
                 logger.warning(message)
 
     @timing
     def graph_create(self, g_type: Union[int, str] = 1, settings: str = str(), grid: int = 3, labels: Dict = None,
-                     other: Dict = None, olap_module_id: str = str(), m_size: dict = None) -> str:
+                     other: Dict = None, olap_module_id: str = str(), m_size: Dict = None) -> str:
         """
         Создать график с заданными параметрами на основе активной или заданной мультисферы.
         Описание параметров:
 
         :param g_type: тип графика; можно задавать как целочисленное значение, так и строковое.
             Возможные значения (указаны целочисленные и строковые варианты):
                 [1, "lines"] - линии
@@ -4852,15 +4881,15 @@
             return self._raise_exception(GraphError, str(ex))
         self._set_graph_module_id(graph_module_id)
         self.func_name = 'graph_create'
         return graph_module_id
 
     @timing
     def graph_modify(self, g_type: Union[int, str] = 1, settings: str = str(), grid: int = 3, labels: Dict = None,
-                     other: Dict = None, graph_id: str = str(), m_size: dict = None) -> str:
+                     other: Dict = None, graph_id: str = str(), m_size: Dict = None) -> str:
         """
         Изменить уже существующий график по заданным параметрам.
         Описание параметров:
 
         :param g_type: тип графика; можно задавать как целочисленное значение, так и строковое.
             Возможные значения (указаны целочисленные и строковые варианты):
                 [1, "lines"] - линии
@@ -5565,15 +5594,15 @@
         except Exception as e:
             return self._raise_exception(ValueError, str(e))
 
         # получаем список сценариев и находим необходимый нам
         scripts_list = self.get_scripts_list()
         self.func_name = 'get_scenario_metadata'
         for script in scripts_list:
-            if script.get('uuid') == script_id:
+            if script.get('id') == script_id:
                 break
         else:
             return self._raise_exception(ValueError, 'Scenario with id "{}" not found!'.format(script_id))
 
         # получаем метаданные
         metadata_result = self.execute_manager_command(
             command_name='scripts', state='get_script_metadata', script_id=script_id)
@@ -5824,15 +5853,15 @@
         # суть метода: сначала меняем режим отображения тоталов, а затем меняем ещё раз
         # после второго вызова режим отображения вернётся в исходное значение, и мы сможем получить это самое значение
         self.change_total_mode()
         res = self.change_total_mode()
         return self.h.parse_result(res, 'show_inter_total')
 
     @timing
-    def request_to_api_v2(self, url: str, method: str, headers: dict, cookies=None, data=None, json: dict = None):
+    def request_to_api_v2(self, url: str, method: str, headers: Dict, cookies=None, data=None, json: Dict = None):
         if cookies is None:
             cookies = {'session': self.session_id}
 
         return requests.request(method=method, url=url, headers=headers, cookies=cookies, data=data, json=json)
 
     @timing
     def switch_session(self, new_owner_uuid: str) -> int:
@@ -5853,14 +5882,15 @@
         url = self.base_url + "api/v2/sessions/current"
         data = {"new_owner": new_owner_uuid}
         headers = {
             'Content-Type': 'application/json', 'Accept': '*/*',
         }
 
         response = self.request_to_api_v2(url=url, method="PATCH", headers=headers, json=data)
+        assert response.status_code == 204, "Response status code != 204"
 
         return response.status_code
 
 
 class GetDataChunk:
     """ Класс для получения данных чанками """
 
@@ -5900,14 +5930,16 @@
         # список имён активных размерностей
         self.dim_lst = []
 
         # получаем количество строк в мультисфере
         total_row, _ = self.sc.get_row_and_col_num(with_total_cols=False, with_total_rows=False)
         self.total_row = total_row
 
+        self.total_row_show_full = self.get_total_rows(True)
+
         # словарь типов размерностей Полиматики; т.к. все значения этого словаря уникальны, его можно "перевернуть"
         self.olap_types = self.sc.server_codes.get("olap", {}).get("olap_data_type", {})
         self.reversed_olap_types = {value: key for key, value in self.olap_types.items()}
 
         # список колонок в формате
         # {"id": <column id>, "data_type": <dimension/fact/fact_dimension>, "name": <column name>, "type": <column type>}
         self.columns = self._get_col_types()
@@ -5958,15 +5990,15 @@
 
     def _get_dim_type(self, olap_type: int) -> str:
         """
         Возвращает тип размерности.
         """
         return list(self.olap_types.keys())[list(self.olap_types.values()).index(olap_type)]
 
-    def _update_or_append_key(self, dict_container: dict, key: str):
+    def _update_or_append_key(self, dict_container: Dict, key: str):
         """
         Добавляет ключ в словарь, если его ещё там нет, иначе значение ключа увеличивает на 1.
         """
         if key not in dict_container:
             dict_container.update({key: 1})
         else:
             dict_container[key] += 1
@@ -6066,15 +6098,29 @@
             }
             columns.append(measure_data)
             exists_columns.add(measure_name)
             self.facts_qty += 1
 
         return columns
 
-    def load_sphere_chunk(self, units: int = 100, convert_type: bool = False,
+    def get_total_rows(self, show_full: bool = False) -> int:
+        response = self.sc.execute_olap_command(
+            command_name="view",
+            state="get_2",
+            from_row=0,
+            from_col=0,
+            num_row=1,
+            num_col=1,
+            show_inter_total=show_full,
+            show_horz_total=show_full,
+            show_vert_total=show_full,
+        )
+        return response['queries'][0]['command']['total_row']
+
+    def load_sphere_chunk(self, units: int = UNITS_LOAD_DATA_CHUNK, convert_type: bool = False,
                           default_value: Any = None, convert_empty_values: bool = True,
                           show_full: bool = False) -> Dict:
         """
         Генератор, подгружающий мультисферу постранично (порциями строк).
         Особенности использования метода:
             1. В мультисфере не должно быть вынесенных вверх размерностей, иначе будет сгенерировано исключение.
             2. Для корректного получения данных необходимо,
@@ -6132,15 +6178,19 @@
         # проверка на количество подгружаемых строк
         error_handler.checks(self.sc, 'load_sphere_chunk', units, convert_type, convert_empty_values)
 
         # если был передан параметр convert_type, то нужно инициализировать класс преобразования типов
         if convert_type:
             type_converter = TypeConverter(self.sc, default_value, convert_empty_values)
 
-        start, total_row = 0, self.total_row
+        self.total_row_show_full = self.get_total_rows(True)
+        headers_count = self.top_dims_qty + 1
+
+        rows_data = None
+        start, total_row = 0, self.total_row_show_full
         while total_row > 0:
             total_row -= units
 
             # получаем число вызываемых строк и столбцов
             # от костыля с версиями никуда не избавиться, т.к. приходится поддерживать багованную версию Полиматики 5.6
             exec_num_row, exec_num_col = units, self.total_cols
             if self.sc.polymatica_version == "5.6":
@@ -6155,29 +6205,152 @@
                 from_col=0,
                 num_row=exec_num_row,
                 num_col=exec_num_col,
                 show_inter_total=show_full,
                 show_horz_total=show_full,
                 show_vert_total=show_full,
             )
-            rows_data = self.h.parse_result(result=rows_result, key="data")
+            data_parsed = self.h.parse_result(result=rows_result, key="data")
 
             headers_count = self.top_dims_qty + 1
-            if not show_full:
-                rows_data = rows_data[headers_count:]
+            if rows_data is None and show_full:
+                rows_data = data_parsed
+            else:
+                rows_data = data_parsed[headers_count:]
 
             for idx, item in enumerate(rows_data):
                 if show_full and idx < headers_count:
                     yield dict(zip(range(len(item)), item))  # return header
                 else:
                     ms_data = type_converter.convert_data_types(self.column_types, item) if convert_type else item
                     yield dict(zip(self.column_names, ms_data))  # return converted data
 
             start += units
 
+    DICT_CELL_TYPES = {
+        1: "Пустая ячейка",
+        2: "Базовая размерность",
+        3: "Групповая размерность",
+        4: "Факты",
+        5: "Всего",
+    }
+
+    def load_sphere_chunk_v2(
+            self,
+            units: int = UNITS_LOAD_DATA_CHUNK,
+    ) -> Tuple[list, list, list, Callable, dict]:
+        """
+        Обновленный метод, возвращающий хедеры и функцию-генератор для выгрузки данных мультисферы по чанкам.
+        Данные выгружаются с типами. Формат ячейки с данными: {"value": <value (str)>, "type": <тип (int)>}.
+        :return: top dims list, left dims list, data header list[list], load_data_by_chunk function, extra info dict:
+            {
+                "data_cols_count": <количество колонок с данными>,
+                "data_rows_count": <количество строк с данными>,
+                "inter_total_hidden_dimensions": <скрытые подыитоги>,
+                "show_global_horz_total": <скрытые глобальные горизантальные итоги>,
+                "show_global_vert_total": <скрытые глобальные вертикальные итоги>,
+            }
+        """
+        assert units > 0, ValueError("units (size of chank) cannot be less 1")
+
+        # get dimensions
+        response = self.sc.execute_olap_command(
+            command_name="dimension",
+            state="list_rq",
+        )
+        dimensions: Dict[Dict] = {dim['id']: dim for dim in response['queries'][0]['command']['dimensions']}
+
+        # get facts
+        response = self.sc.execute_olap_command(
+            command_name="fact",
+            state="list_rq",
+        )
+        facts: Dict[Dict] = {dim['id']: dim for dim in response['queries'][0]['command']['facts']}
+
+        # load 1 row with 1 col to get valid total_col and total_row
+        response = self.sc.execute_olap_command(
+            command_name="view",
+            state="get",
+            from_row=0,
+            from_col=0,
+            num_row=1,
+            num_col=1,
+        )
+        command_data: Dict = response['queries'][0]['command']
+
+        data_cols_count = command_data['total_col']
+        data_rows_count = command_data['total_row']
+        inter_total_hidden_dimensions = command_data['inter_total_hidden_dimensions']
+        show_global_horz_total = command_data['show_global_horz_total']
+        show_global_vert_total = command_data['show_global_horz_total']
+
+        extra_info = {
+            "data_cols_count": data_cols_count,
+            "data_rows_count": data_rows_count,
+            "inter_total_hidden_dimensions": inter_total_hidden_dimensions,
+            "show_global_horz_total": show_global_horz_total,
+            "show_global_vert_total": show_global_vert_total,
+        }
+
+        # load all cols to create correct data headers
+        response = self.sc.execute_olap_command(
+            command_name="view",
+            state="get",
+            from_row=0,
+            from_col=0,
+            num_row=1,
+            num_col=data_cols_count,
+        )
+        command_data: Dict = response['queries'][0]['command']
+
+        top_dims = [dimensions[dim_id]['name'] for dim_id in command_data['top_dims']]
+        left_dims = [dimensions[dim_id]['name'] for dim_id in command_data['left_dims']]
+
+        data_header = []
+        for row in command_data['top']:
+            tmp_data_header_row = []
+            for cell in row:
+                if cell['type'] == 4:  # fact
+                    fact_id = cell['fact_id']
+                    cell['value'] = facts[fact_id]['name']
+                tmp_data_header_row += [{
+                    'value': cell.get('value', None),
+                    'type': cell.get('type')
+                }]
+            data_header += [tmp_data_header_row]
+
+        def load_data_by_chunk() -> Tuple[list, list]:
+            """
+            Function-generator for loading data from sphere by chunks.
+            :return: left columns list[list], data list[list]
+            """
+            idx_start_row = 0
+
+            while idx_start_row < data_rows_count:
+                idx_end_row = idx_start_row + units
+
+                response = self.sc.execute_olap_command(
+                    command_name="view",
+                    state="get",
+                    from_row=idx_start_row,
+                    from_col=0,
+                    num_row=units,
+                    num_col=data_cols_count,
+                )
+                command_data: Dict = response['queries'][0]['command']
+                left_data = [[{'value': cell.get('value', None), 'type': cell.get('type')} for cell in row]
+                              for row in command_data['left']]
+                data = command_data['data']
+
+                yield left_data, data
+
+                idx_start_row = idx_end_row
+
+        return top_dims, left_dims, data_header, load_data_by_chunk, extra_info
+
     @property
     def olap_module_info(self):
         """
         Получает дополнительную информацию по размерностям в обработанном формате.
         Подробнее в методе BusinessLogic.get_olap_module_info.
 
         :return: (Dict) текущая конфигурация OLAP--модуля;
```

### Comparing `polyapi-5.7.0.4/polymatica/commands/base_command.py` & `polyapi-5.7.0.6/polymatica/commands/base_command.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.4/polymatica/commands/olap_module.py` & `polyapi-5.7.0.6/polymatica/commands/olap_module.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.4/polymatica/commands/other_modules.py` & `polyapi-5.7.0.6/polymatica/commands/other_modules.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.4/polymatica/common/consts.py` & `polyapi-5.7.0.6/polymatica/common/consts.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.4/polymatica/common/helper_funcs.py` & `polyapi-5.7.0.6/polymatica/common/helper_funcs.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.4/polymatica/error_handler.py` & `polyapi-5.7.0.6/polymatica/error_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,21 +183,23 @@
             raise ValueError('Param "num_row" must be "int" type!')
         if not isinstance(filter_name, (str, list, set, tuple)):
             raise ValueError('Param "filter_name" must be one of following types: ["str", "list", "set", "tuple"]!')
         if not filter_name:
             raise ValueError('Param "filter_name" cannot be empty!')
         return [filter_name] if isinstance(filter_name, str) else filter_name
     elif func_name == "put_dim_filter":
-        filter_name, start_date, end_date, filter_field_format = args[0], args[1], args[2], args[3]
+        filter_name, start_date, end_date, filter_field_format, dim_name, dim_id = args[0], args[1], args[2], args[3], args[4], args[5]
         if (filter_name is None) and (start_date is None and end_date is None):
             raise ValueError("If you don't filter one value by param filter_name,"
                              " please assign value to args start_date AND end_date!")
         elif (filter_name is not None) and (start_date is not None and end_date is not None):
             raise ValueError("Please, fill in arg filter_name for filtering one value OR:\n"
                              "args start_date AND end_date for filtering date interval!")
+        if dim_name is None and dim_id is None:
+            raise ValueError("You should specify dim_name or dim_id")
 
         # список для заполнения данными
         dates_list = []
 
         # Заполнение списка dates_list в зависимости от содержания параметров filter_name, start_date, end_date
         # заполнить список для недельного интервала
         if (filter_name is None) and (start_date is not None and end_date is not None):
```

### Comparing `polyapi-5.7.0.4/polymatica/exceptions.py` & `polyapi-5.7.0.6/polymatica/exceptions.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.4/polymatica/executor.py` & `polyapi-5.7.0.6/polymatica/executor.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.4/polymatica/graph/base_graph.py` & `polyapi-5.7.0.6/polymatica/graph/base_graph.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.4/polymatica/graph/graph_interface.py` & `polyapi-5.7.0.6/polymatica/graph/graph_interface.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.4/polymatica/graph/types/__init__.py` & `polyapi-5.7.0.6/polymatica/graph/types/__init__.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.4/polymatica/graph/types/areas.py` & `polyapi-5.7.0.6/polymatica/graph/types/areas.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.4/polymatica/graph/types/balls.py` & `polyapi-5.7.0.6/polymatica/graph/types/balls.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.4/polymatica/graph/types/chord.py` & `polyapi-5.7.0.6/polymatica/graph/types/chord.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.4/polymatica/graph/types/circles.py` & `polyapi-5.7.0.6/polymatica/graph/types/circles.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.4/polymatica/graph/types/circles_series.py` & `polyapi-5.7.0.6/polymatica/graph/types/circles_series.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.4/polymatica/graph/types/corridors.py` & `polyapi-5.7.0.6/polymatica/graph/types/corridors.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.4/polymatica/graph/types/cumulative_areas.py` & `polyapi-5.7.0.6/polymatica/graph/types/cumulative_areas.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.4/polymatica/graph/types/cumulative_cylinders.py` & `polyapi-5.7.0.6/polymatica/graph/types/cumulative_cylinders.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.4/polymatica/graph/types/cylinders.py` & `polyapi-5.7.0.6/polymatica/graph/types/cylinders.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.4/polymatica/graph/types/graph.py` & `polyapi-5.7.0.6/polymatica/graph/types/graph.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.4/polymatica/graph/types/lines.py` & `polyapi-5.7.0.6/polymatica/graph/types/lines.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.4/polymatica/graph/types/pies.py` & `polyapi-5.7.0.6/polymatica/graph/types/pies.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.4/polymatica/graph/types/point.py` & `polyapi-5.7.0.6/polymatica/graph/types/point.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.4/polymatica/graph/types/point_series.py` & `polyapi-5.7.0.6/polymatica/graph/types/point_series.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.4/polymatica/graph/types/pools.py` & `polyapi-5.7.0.6/polymatica/graph/types/pools.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.4/polymatica/graph/types/pools_3d.py` & `polyapi-5.7.0.6/polymatica/graph/types/pools_3d.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.4/polymatica/graph/types/radar.py` & `polyapi-5.7.0.6/polymatica/graph/types/radar.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.4/polymatica/graph/types/sankey.py` & `polyapi-5.7.0.6/polymatica/graph/types/sankey.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.4/polymatica/graph/types/surface.py` & `polyapi-5.7.0.6/polymatica/graph/types/surface.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.4/polymatica/helper.py` & `polyapi-5.7.0.6/polymatica/helper.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.4/polymatica/versions/polymatica_57.py` & `polyapi-5.7.0.6/polymatica/versions/polymatica_57.py`

 * *Files 4% similar despite different names*

```diff
@@ -125,70 +125,48 @@
 
     def run_scenario_impl(self, **kwargs):
         """
         Запуск сценария.
         """
         scenario_id, scenario_name = kwargs.get('scenario_id'), kwargs.get('scenario_name')
 
-        # 1. Получаем информацию о запускаемом сценарии
-        script_data = self.base_bs.execute_manager_command(
-            command_name="scripts", state="get_script_description", script_id=scenario_id)
-        script_info = self.base_bs.h.parse_result(script_data, 'script')
-
-        # 2. Получаем идентификаторы существующих слоёв
+        # Получаем идентификаторы существующих слоёв
         exists_layers = self.base_bs._get_session_layers()
         exists_layer_ids = [layer.get('uuid') for layer in exists_layers]
 
-        # 3. Создаём новый слой, на котором будет запущен наш сценарий, и добавляем его в список существующих слоёв
+        # Создаём новый слой, на котором будет запущен наш сценарий, и добавляем его в список существующих слоёв
         new_layer_data = self.base_bs.execute_manager_command(command_name="user_layer", state="create_layer")
         layer_uuid = (self.base_bs.h.parse_result(new_layer_data, 'layer') or dict()).get("uuid")
         if not layer_uuid:
             return self._raise_exception(ScenarioError, 'New layer has been no created!')
         exists_layer_ids.append(layer_uuid)
 
-        # 4. Переименовываем слой - он будет называться также, как запускаемый сценарий
+        # Переименовываем слой - он будет называться также, как запускаемый сценарий
         self.base_bs.execute_manager_command(
             command_name="user_layer", state="rename_layer", layer_id=layer_uuid, name=scenario_name)
 
-        # 5. Запускаем и воспроизводим сценарий
-        self.base_bs.execute_manager_command(
-            command_name="scripts",
-            state="load_on_layer",
-            script_id=scenario_id,
-            runtime_id=layer_uuid,
-            on_load_action=0
-        )
-        self.base_bs.execute_manager_command(
-            command_name="scripts",
-            state="play_to_position",
-            script_id=scenario_id,
-            runtime_id=layer_uuid,
-            play_to_position=script_info.get('steps_count') - 1,
-            clear_workspace=True
-        )
-
-        # 6. Ожидание загрузки сценария
-        self._wait_scenario_loaded(layer_uuid)
+        # Запуск сценария на слое
+        self.run_scenario_on_layer_impl(layer_id=layer_uuid, scenario_id=scenario_id)
 
-        # 7. Сделать слой активным
+        # Сделать слой активным
         self.base_bs.execute_manager_command(command_name="user_layer", state="set_active_layer", layer_id=layer_uuid)
 
-        # 8. Инициализация слоя, содержащего сценарий
+        # Инициализация слоя, содержащего сценарий
         self.base_bs.execute_manager_command(command_name="user_layer", state="init_layer", layer_id=layer_uuid)
 
-        # 9. Сохранение интерфейсных настроек
+        # Сохранение интерфейсных настроек
         settings = {"wm_layers2": {"lids": exists_layer_ids, "active": layer_uuid}}
         self.base_bs.execute_manager_command(
             command_name="user_iface",
             state="save_settings",
             module_id=self.base_bs.authorization_uuid,
             settings=settings
         )
 
-        # 10. Сохранение переменных окружения
+        # Сохранение переменных окружения
         self.base_bs.layers_list = exists_layer_ids
         self.base_bs.active_layer_id = layer_uuid
         layer_settings = self.base_bs.execute_manager_command(
             command_name="user_layer", state="get_layer", layer_id=layer_uuid)
         module_descs = self.base_bs.h.parse_result(
             result=layer_settings, key="layer", nested_key="module_descs") or list()
         if not module_descs:
@@ -198,11 +176,46 @@
             for module in module_descs:
                 # берём первую по счёту мультисферу
                 if module.get('type_id') == MULTISPHERE_ID:
                     self.base_bs.set_multisphere_module_id(module.get('uuid', str()))
                     self.base_bs.cube_id = module.get('cube_id', str())
                     break
 
-        # 11. Обновление числа строк активной мультисферы
+        # Обновление числа строк активной мультисферы
         if self.base_bs.multisphere_module_id:
             self.base_bs.update_total_row()
         self.base_bs.func_name = 'run_scenario'
+
+    def run_scenario_on_layer_impl(self, **kwargs):
+        """
+        Запуск сценария на заданном слое
+        """
+
+        scenario_id, layer_id = kwargs.get('scenario_id'), kwargs.get('layer_id')
+
+        # Получаем информацию о запускаемом сценарии
+        script_data = self.base_bs.execute_manager_command(
+            command_name="scripts", state="get_script_description", script_id=scenario_id)
+        script_info = self.base_bs.h.parse_result(script_data, 'script')
+
+        self.base_bs.execute_manager_command(
+            command_name="scripts",
+            state="load_on_layer",
+            script_id=scenario_id,
+            runtime_id=layer_id,
+            on_load_action=0
+        )
+        self.base_bs.execute_manager_command(
+            command_name="scripts",
+            state="play_to_position",
+            script_id=scenario_id,
+            runtime_id=layer_id,
+            play_to_position=script_info.get('steps_count') - 1,
+            clear_workspace=True
+        )
+
+        self._wait_scenario_loaded(layer_id)
+
+        # сохраняем текущий слой как активный
+        self.base_bs.active_layer_id = layer_id
+
+        self.base_bs.func_name = 'run_scenario_on_layer'
```

### Comparing `polyapi-5.7.0.4/polymatica/versions/versions_redirect.py` & `polyapi-5.7.0.6/polymatica/versions/versions_redirect.py`

 * *Files identical despite different names*

### Comparing `polyapi-5.7.0.4/setup.py` & `polyapi-5.7.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: OS Independent',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='polyapi',
-    version='5.7.0.4',
+    version='5.7.0.6',
     description='Wrapper for Polymatica API',
     long_description=open('README.txt', encoding='utf-8').read(),
     url='https://www.polymatica.ru',
     author='Polymatica Rus LLC',
     author_email='development@polymatica.com',
     license='MIT',
     classifiers=classifiers,
```

