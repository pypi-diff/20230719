# Comparing `tmp/Navix-0.3.7.tar.gz` & `tmp/Navix-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Navix-0.3.7.tar", last modified: Thu Jul 13 10:30:55 2023, max compression
+gzip compressed data, was "Navix-0.3.8.tar", last modified: Wed Jul 19 07:24:11 2023, max compression
```

## Comparing `Navix-0.3.7.tar` & `Navix-0.3.8.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:30:55.388015 Navix-0.3.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:30:55.380015 Navix-0.3.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:30:55.380015 Navix-0.3.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-13 10:30:34.000000 Navix-0.3.7/.github/workflows/CD.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-13 10:30:34.000000 Navix-0.3.7/.github/workflows/CI.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-07-13 10:30:34.000000 Navix-0.3.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-13 10:30:34.000000 Navix-0.3.7/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-13 10:30:34.000000 Navix-0.3.7/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-07-13 10:30:34.000000 Navix-0.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-13 10:30:34.000000 Navix-0.3.7/NOTICE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:30:55.384015 Navix-0.3.7/Navix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18408 2023-07-13 10:30:55.000000 Navix-0.3.7/Navix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-13 10:30:55.000000 Navix-0.3.7/Navix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 10:30:55.000000 Navix-0.3.7/Navix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-13 10:30:55.000000 Navix-0.3.7/Navix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-13 10:30:55.000000 Navix-0.3.7/Navix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18408 2023-07-13 10:30:55.388015 Navix-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-07-13 10:30:34.000000 Navix-0.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:30:55.384015 Navix-0.3.7/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-13 10:30:34.000000 Navix-0.3.7/docs/design_notes.md
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-07-13 10:30:34.000000 Navix-0.3.7/docs/performance.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-13 10:30:34.000000 Navix-0.3.7/docs/performance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:30:55.384015 Navix-0.3.7/navix/
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-13 10:30:34.000000 Navix-0.3.7/navix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-13 10:30:34.000000 Navix-0.3.7/navix/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-07-13 10:30:34.000000 Navix-0.3.7/navix/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-13 10:30:34.000000 Navix-0.3.7/navix/components.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-13 10:30:34.000000 Navix-0.3.7/navix/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10020 2023-07-13 10:30:34.000000 Navix-0.3.7/navix/entities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:30:55.384015 Navix-0.3.7/navix/environments/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-13 10:30:34.000000 Navix-0.3.7/navix/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-07-13 10:30:34.000000 Navix-0.3.7/navix/environments/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-07-13 10:30:34.000000 Navix-0.3.7/navix/environments/keydoor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-13 10:30:34.000000 Navix-0.3.7/navix/environments/room.py
--rw-r--r--   0 runner    (1001) docker     (123)    12599 2023-07-13 10:30:34.000000 Navix-0.3.7/navix/graphics.py
--rw-r--r--   0 runner    (1001) docker     (123)     7733 2023-07-13 10:30:34.000000 Navix-0.3.7/navix/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-07-13 10:30:34.000000 Navix-0.3.7/navix/observations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-13 10:30:34.000000 Navix-0.3.7/navix/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-13 10:30:34.000000 Navix-0.3.7/navix/terminations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-07-13 10:30:34.000000 Navix-0.3.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-13 10:30:34.000000 Navix-0.3.7/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:30:55.384015 Navix-0.3.7/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      808 2023-07-13 10:30:34.000000 Navix-0.3.7/scripts/release.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 10:30:55.388015 Navix-0.3.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:30:55.388015 Navix-0.3.7/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:30:55.388015 Navix-0.3.7/tests/performance/
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-13 10:30:34.000000 Navix-0.3.7/tests/performance/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-13 10:30:34.000000 Navix-0.3.7/tests/performance/minigrid.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-13 10:30:34.000000 Navix-0.3.7/tests/performance/minigrid_report.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-13 10:30:34.000000 Navix-0.3.7/tests/performance/observations.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-13 10:30:34.000000 Navix-0.3.7/tests/performance/observations_keydoor_report.txt
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-13 10:30:34.000000 Navix-0.3.7/tests/performance/observations_room_report.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-13 10:30:34.000000 Navix-0.3.7/tests/performance/profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)    13636 2023-07-13 10:30:34.000000 Navix-0.3.7/tests/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-13 10:30:34.000000 Navix-0.3.7/tests/test_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-13 10:30:34.000000 Navix-0.3.7/tests/test_environments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-07-13 10:30:34.000000 Navix-0.3.7/tests/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-07-13 10:30:34.000000 Navix-0.3.7/tests/test_observations.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-13 10:30:34.000000 Navix-0.3.7/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-13 10:30:34.000000 Navix-0.3.7/tests/test_terminations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:24:11.024318 Navix-0.3.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:24:11.016318 Navix-0.3.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:24:11.020318 Navix-0.3.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-19 07:23:59.000000 Navix-0.3.8/.github/workflows/CD.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-19 07:23:59.000000 Navix-0.3.8/.github/workflows/CI.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-07-19 07:23:59.000000 Navix-0.3.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-19 07:23:59.000000 Navix-0.3.8/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-19 07:23:59.000000 Navix-0.3.8/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-07-19 07:23:59.000000 Navix-0.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-19 07:23:59.000000 Navix-0.3.8/NOTICE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:24:11.020318 Navix-0.3.8/Navix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18408 2023-07-19 07:24:10.000000 Navix-0.3.8/Navix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-19 07:24:11.000000 Navix-0.3.8/Navix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 07:24:10.000000 Navix-0.3.8/Navix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-19 07:24:10.000000 Navix-0.3.8/Navix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-19 07:24:10.000000 Navix-0.3.8/Navix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18408 2023-07-19 07:24:11.024318 Navix-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-07-19 07:23:59.000000 Navix-0.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:24:11.020318 Navix-0.3.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-19 07:23:59.000000 Navix-0.3.8/docs/design_notes.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-07-19 07:23:59.000000 Navix-0.3.8/docs/performance.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-19 07:23:59.000000 Navix-0.3.8/docs/performance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:24:11.024318 Navix-0.3.8/navix/
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-19 07:23:59.000000 Navix-0.3.8/navix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-19 07:23:59.000000 Navix-0.3.8/navix/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-07-19 07:23:59.000000 Navix-0.3.8/navix/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-19 07:23:59.000000 Navix-0.3.8/navix/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-19 07:23:59.000000 Navix-0.3.8/navix/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10042 2023-07-19 07:23:59.000000 Navix-0.3.8/navix/entities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:24:11.024318 Navix-0.3.8/navix/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-19 07:23:59.000000 Navix-0.3.8/navix/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-07-19 07:23:59.000000 Navix-0.3.8/navix/environments/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-07-19 07:23:59.000000 Navix-0.3.8/navix/environments/keydoor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-19 07:23:59.000000 Navix-0.3.8/navix/environments/room.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12599 2023-07-19 07:23:59.000000 Navix-0.3.8/navix/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7734 2023-07-19 07:23:59.000000 Navix-0.3.8/navix/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-07-19 07:23:59.000000 Navix-0.3.8/navix/observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-19 07:23:59.000000 Navix-0.3.8/navix/spaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-19 07:23:59.000000 Navix-0.3.8/navix/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-19 07:23:59.000000 Navix-0.3.8/navix/terminations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-07-19 07:23:59.000000 Navix-0.3.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-19 07:23:59.000000 Navix-0.3.8/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:24:11.024318 Navix-0.3.8/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      808 2023-07-19 07:23:59.000000 Navix-0.3.8/scripts/release.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 07:24:11.024318 Navix-0.3.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:24:11.024318 Navix-0.3.8/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:24:11.024318 Navix-0.3.8/tests/performance/
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-19 07:23:59.000000 Navix-0.3.8/tests/performance/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-19 07:23:59.000000 Navix-0.3.8/tests/performance/minigrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-19 07:23:59.000000 Navix-0.3.8/tests/performance/minigrid_report.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-19 07:23:59.000000 Navix-0.3.8/tests/performance/observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-19 07:23:59.000000 Navix-0.3.8/tests/performance/observations_keydoor_report.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-19 07:23:59.000000 Navix-0.3.8/tests/performance/observations_room_report.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-19 07:23:59.000000 Navix-0.3.8/tests/performance/profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13636 2023-07-19 07:23:59.000000 Navix-0.3.8/tests/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-19 07:23:59.000000 Navix-0.3.8/tests/test_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-07-19 07:23:59.000000 Navix-0.3.8/tests/test_environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-07-19 07:23:59.000000 Navix-0.3.8/tests/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-07-19 07:23:59.000000 Navix-0.3.8/tests/test_observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-19 07:23:59.000000 Navix-0.3.8/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-19 07:23:59.000000 Navix-0.3.8/tests/test_terminations.py
```

### Comparing `Navix-0.3.7/.github/workflows/CD.yml` & `Navix-0.3.8/.github/workflows/CD.yml`

 * *Files identical despite different names*

### Comparing `Navix-0.3.7/.github/workflows/CI.yml` & `Navix-0.3.8/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `Navix-0.3.7/.gitignore` & `Navix-0.3.8/.gitignore`

 * *Files identical despite different names*

### Comparing `Navix-0.3.7/COPYRIGHT` & `Navix-0.3.8/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `Navix-0.3.7/LICENSE` & `Navix-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `Navix-0.3.7/Navix.egg-info/PKG-INFO` & `Navix-0.3.8/Navix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Navix
-Version: 0.3.7
+Version: 0.3.8
 Summary: Accelerated gridworld navigation with JAX for deep reinforcement learning
 Author-email: Eduardo Pignatelli <edu.pignatelli@gmail.com>
 Maintainer-email: Eduardo Pignatelli <edu.pignatelli@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `Navix-0.3.7/Navix.egg-info/SOURCES.txt` & `Navix-0.3.8/Navix.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 navix/actions.py
 navix/components.py
 navix/config.py
 navix/entities.py
 navix/graphics.py
 navix/grid.py
 navix/observations.py
+navix/spaces.py
 navix/tasks.py
 navix/terminations.py
 navix/environments/__init__.py
 navix/environments/environment.py
 navix/environments/keydoor.py
 navix/environments/room.py
 scripts/release.sh
```

### Comparing `Navix-0.3.7/PKG-INFO` & `Navix-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Navix
-Version: 0.3.7
+Version: 0.3.8
 Summary: Accelerated gridworld navigation with JAX for deep reinforcement learning
 Author-email: Eduardo Pignatelli <edu.pignatelli@gmail.com>
 Maintainer-email: Eduardo Pignatelli <edu.pignatelli@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `Navix-0.3.7/README.md` & `Navix-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `Navix-0.3.7/docs/design_notes.md` & `Navix-0.3.8/docs/design_notes.md`

 * *Files identical despite different names*

### Comparing `Navix-0.3.7/docs/performance.ipynb` & `Navix-0.3.8/docs/performance.ipynb`

 * *Files identical despite different names*

### Comparing `Navix-0.3.7/docs/performance.py` & `Navix-0.3.8/docs/performance.py`

 * *Files identical despite different names*

### Comparing `Navix-0.3.7/navix/__init__.py` & `Navix-0.3.8/navix/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,8 +25,9 @@
     graphics,
     grid,
     observations,
     tasks,
     environments,
     terminations,
     config,
+    spaces,
 )
```

### Comparing `Navix-0.3.7/navix/_version.py` & `Navix-0.3.8/navix/_version.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,9 +14,9 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 
-__version__ = "0.3.7"
+__version__ = "0.3.8"
 __version_info__ = tuple(int(i) for i in __version__.split(".") if i.isdigit())
```

### Comparing `Navix-0.3.7/navix/actions.py` & `Navix-0.3.8/navix/actions.py`

 * *Files identical despite different names*

### Comparing `Navix-0.3.7/navix/components.py` & `Navix-0.3.8/navix/components.py`

 * *Files identical despite different names*

### Comparing `Navix-0.3.7/navix/entities.py` & `Navix-0.3.8/navix/entities.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,15 +237,17 @@
 
     @property
     def transparent(self) -> Array:
         return self.open
 
     @property
     def sprite(self) -> Array:
-        sprite = SPRITES_REGISTRY[Entities.DOOR.value][self.direction, jnp.asarray(self.open, dtype=jnp.int32)]
+        sprite = SPRITES_REGISTRY[Entities.DOOR.value][
+            self.direction, jnp.asarray(self.open, dtype=jnp.int32)
+        ]
         if sprite.ndim == 3:
             # batch it
             sprite = sprite[None]
         # ensure same batch size
         if sprite.shape[0] != self.position.shape[0]:
             sprite = jnp.broadcast_to(sprite, (*self.shape, *sprite.shape[1:]))
         return sprite
```

### Comparing `Navix-0.3.7/navix/environments/__init__.py` & `Navix-0.3.8/navix/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `Navix-0.3.7/navix/environments/environment.py` & `Navix-0.3.8/navix/environments/environment.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,28 +16,30 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 
 from __future__ import annotations
 
+import sys
 import abc
 from enum import IntEnum
 from typing import Any, Callable, Dict
 import jax
 import jax.numpy as jnp
 from jax.random import KeyArray
 from jax import Array
 from flax import struct
 
 
 from .. import tasks, terminations, observations
-from ..graphics import RenderingCache
+from ..graphics import RenderingCache, TILE_SIZE
 from ..entities import State
 from ..actions import ACTIONS
+from ..spaces import Space, Discrete, Continuous
 
 
 class StepType(IntEnum):
     TRANSITION = 0
     """discount > 0, episode continues"""
     TRUNCATION = 1
     """discount > 0, episode ends"""
@@ -73,14 +75,47 @@
     reward_fn: Callable[[State, Array, State], Array] = struct.field(
         pytree_node=False, default=tasks.navigation
     )
     termination_fn: Callable[[State, Array, State], Array] = struct.field(
         pytree_node=False, default=terminations.on_navigation_completion
     )
 
+    @property
+    def observation_space(self) -> Space:
+        if self.observation_fn == observations.none:
+            return Continuous(shape=())
+        elif self.observation_fn == observations.categorical:
+            return Discrete(sys.maxsize, shape=(self.height, self.width))
+        elif self.observation_fn == observations.categorical_first_person:
+            radius = observations.RADIUS
+            return Discrete(sys.maxsize, shape=(radius + 1, radius * 2 + 1))
+        elif self.observation_fn == observations.rgb:
+            return Discrete(
+                256,
+                shape=(self.height * TILE_SIZE, self.width * TILE_SIZE, 3),
+                dtype=jnp.uint8,
+            )
+        elif self.observation_fn == observations.rgb_first_person:
+            radius = observations.RADIUS
+            return Discrete(
+                256,
+                shape=(radius * TILE_SIZE * 2 + 1, radius * TILE_SIZE * 2 + 1, 3),
+                dtype=jnp.uint8,
+            )
+        else:
+            raise NotImplementedError(
+                "Unknown observation space for observation function {}".format(
+                    self.observation_fn
+                )
+            )
+
+    @property
+    def action_space(self) -> Space:
+        return Discrete(len(ACTIONS))
+
     @abc.abstractmethod
     def reset(self, key: KeyArray, cache: RenderingCache | None = None) -> Timestep:
         raise NotImplementedError()
 
     def _step(self, timestep: Timestep, action: Array, actions_set=ACTIONS) -> Timestep:
         # update agents
         state = jax.lax.switch(action, actions_set.values(), timestep.state)
```

### Comparing `Navix-0.3.7/navix/environments/keydoor.py` & `Navix-0.3.8/navix/environments/keydoor.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,20 @@
 from ..environments import Timestep
 from ..grid import mask_by_coordinates, room, random_positions, random_directions
 
 
 class KeyDoor(Environment):
     def reset(self, key: KeyArray, cache: Union[RenderingCache, None] = None) -> Timestep:  # type: ignore
         # check minimum height and width
-        assert self.height > 3, f"Room height must be greater than 3, got {self.height} instead"
-        assert self.width > 4, f"Room width must be greater than 5, got {self.width} instead"
+        assert (
+            self.height > 3
+        ), f"Room height must be greater than 3, got {self.height} instead"
+        assert (
+            self.width > 4
+        ), f"Room width must be greater than 5, got {self.width} instead"
 
         key, k1, k2, k3, k4 = jax.random.split(key, 5)
 
         grid = room(height=self.height, width=self.width)
 
         # door positions
         # col can be between 1 and height - 2
@@ -35,21 +39,27 @@
         )
 
         # wall positions
         wall_rows = jnp.arange(1, self.height - 1)
         wall_cols = jnp.asarray([door_col] * (self.height - 2))
         wall_pos = jnp.stack((wall_rows, wall_cols), axis=1)
         # remove wall where the door is
-        wall_pos = jnp.delete(wall_pos, door_row - 1, axis=0, assume_unique_indices=True)
+        wall_pos = jnp.delete(
+            wall_pos, door_row - 1, axis=0, assume_unique_indices=True
+        )
         walls = Wall(position=wall_pos)
 
         # get rooms
-        first_room_mask = mask_by_coordinates(grid, (jnp.asarray(self.height), door_col), jnp.less)
+        first_room_mask = mask_by_coordinates(
+            grid, (jnp.asarray(self.height), door_col), jnp.less
+        )
         first_room = jnp.where(first_room_mask, grid, -1)  # put walls where not mask
-        second_room_mask = mask_by_coordinates(grid, (jnp.asarray(0), door_col), jnp.greater)
+        second_room_mask = mask_by_coordinates(
+            grid, (jnp.asarray(0), door_col), jnp.greater
+        )
         second_room = jnp.where(second_room_mask, grid, -1)  # put walls where not mask
 
         # spawn player
         player_pos = random_positions(k1, first_room)
         player_dir = random_directions(k2)
         player = Player(
             position=player_pos, direction=player_dir, pocket=EMPTY_POCKET_ID
```

### Comparing `Navix-0.3.7/navix/environments/room.py` & `Navix-0.3.8/navix/environments/room.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,21 +15,20 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 
 from __future__ import annotations
-from typing import Callable, Union
+from typing import Union
 
 import jax
 import jax.numpy as jnp
 from jax.random import KeyArray
 
-
 from ..components import EMPTY_POCKET_ID
 from ..entities import Entities, Goal, Player, State
 from ..grid import random_positions, random_directions, room
 from ..graphics import RenderingCache
 from .environment import Environment, Timestep
```

### Comparing `Navix-0.3.7/navix/graphics.py` & `Navix-0.3.8/navix/graphics.py`

 * *Files identical despite different names*

### Comparing `Navix-0.3.7/navix/grid.py` & `Navix-0.3.8/navix/grid.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,15 @@
             lambda x: jnp.rot90(x, 2),  # 0 = flip, 1 = flip
             lambda x: jnp.rot90(x, 3),  # 0 = flip, 1 = transpose
             lambda x: x,
         ),
         cropped,
     )
 
-    cropped = rotated[:radius + 1]
+    cropped = rotated[: radius + 1]
     return jnp.asarray(cropped, dtype=grid.dtype)
 
 
 def view_cone(transparency_map: Array, origin: Array, radius: int) -> Array:
     # transparency_map is a boolean map of transparent (1) and opaque (0) tiles
 
     def fin_diff(array, _):
```

### Comparing `Navix-0.3.7/navix/observations.py` & `Navix-0.3.8/navix/observations.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,17 @@
 
 from . import graphics
 from .components import DISCARD_PILE_IDX
 from .entities import State
 from .grid import align, idx_from_coordinates, crop, view_cone
 
 
+RADIUS = 3
+
+
 def none(
     state: State,
 ) -> Array:
     return jnp.asarray(())
 
 
 def categorical(
@@ -48,32 +51,31 @@
     grid = state.grid.reshape(-1).at[indices].set(tags)
     # unflatten patches to reconstruct the grid
     return grid.reshape(shape)
 
 
 def categorical_first_person(
     state: State,
-    radius: int = 3,
 ) -> Array:
     # get transparency map
     transparency_map = jnp.where(state.grid == 0, 1, 0)
     positions = state.get_positions()
     transparent = state.get_transparency()
     transparency_map = transparency_map.at[tuple(positions.T)].set(~transparent)
 
     # apply view mask
     player = state.get_player()
-    view = view_cone(transparency_map, player.position, radius)
+    view = view_cone(transparency_map, player.position, RADIUS)
 
     # get categorical representation
     tags = state.get_tags()
     obs = state.grid.at[tuple(positions.T)].set(tags) * view
 
     # crop grid to agent's view
-    obs = crop(obs, player.position, player.direction, radius)
+    obs = crop(obs, player.position, player.direction, RADIUS)
 
     return obs
 
 
 def rgb(
     state: State,
 ) -> Array:
@@ -95,29 +97,28 @@
     )
     image = graphics.unflatten_patches(patches, image_size)
     return image
 
 
 def rgb_first_person(
     state: State,
-    radius: int = 3,
 ) -> Array:
     # calculate final image size
     image_size = (
         state.grid.shape[0] * graphics.TILE_SIZE,
         state.grid.shape[1] * graphics.TILE_SIZE,
     )
 
     # get agent's view
     transparency_map = jnp.where(state.grid == 0, 1, 0)
     positions = state.get_positions()
     transparent = state.get_transparency()
     transparency_map = transparency_map.at[tuple(positions.T)].set(~transparent)
     player = state.get_player()
-    view = view_cone(transparency_map, player.position, radius)
+    view = view_cone(transparency_map, player.position, RADIUS)
     view = jax.image.resize(view, image_size, method="nearest")
     view = jnp.tile(view[..., None], (1, 1, 3))
 
     # get sprites aligned to player's direction
     sprites = state.get_sprites()
     sprites = jax.vmap(lambda x: align(x, jnp.asarray(0), player.direction))(sprites)
 
@@ -127,14 +128,14 @@
 
     # remove discard pile
     patches = patches[:DISCARD_PILE_IDX]
     # rearrange the sprites in a grid
     patchwork = patches.reshape(*state.grid.shape, *patches.shape[1:])
 
     # crop grid to agent's view
-    patchwork = crop(patchwork, player.position, player.direction, radius)
+    patchwork = crop(patchwork, player.position, player.direction, RADIUS)
 
     # reconstruct image
     obs = jnp.swapaxes(patchwork, 1, 2)
     shape = obs.shape
     obs = obs.reshape(shape[0] * shape[1], shape[2] * shape[3], *shape[4:])
     return obs
```

### Comparing `Navix-0.3.7/navix/tasks.py` & `Navix-0.3.8/navix/tasks.py`

 * *Files identical despite different names*

### Comparing `Navix-0.3.7/navix/terminations.py` & `Navix-0.3.8/navix/terminations.py`

 * *Files identical despite different names*

### Comparing `Navix-0.3.7/pyproject.toml` & `Navix-0.3.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Navix-0.3.7/scripts/release.sh` & `Navix-0.3.8/scripts/release.sh`

 * *Files identical despite different names*

### Comparing `Navix-0.3.7/tests/performance/grid.py` & `Navix-0.3.8/tests/performance/grid.py`

 * *Files identical despite different names*

### Comparing `Navix-0.3.7/tests/performance/minigrid.py` & `Navix-0.3.8/tests/performance/minigrid.py`

 * *Files identical despite different names*

### Comparing `Navix-0.3.7/tests/performance/observations.py` & `Navix-0.3.8/tests/performance/observations.py`

 * *Files identical despite different names*

### Comparing `Navix-0.3.7/tests/performance/observations_keydoor_report.txt` & `Navix-0.3.8/tests/performance/observations_keydoor_report.txt`

 * *Files identical despite different names*

### Comparing `Navix-0.3.7/tests/performance/observations_room_report.txt` & `Navix-0.3.8/tests/performance/observations_room_report.txt`

 * *Files identical despite different names*

### Comparing `Navix-0.3.7/tests/performance/profiling.py` & `Navix-0.3.8/tests/performance/profiling.py`

 * *Files identical despite different names*

### Comparing `Navix-0.3.7/tests/test_actions.py` & `Navix-0.3.8/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `Navix-0.3.7/tests/test_entities.py` & `Navix-0.3.8/tests/test_entities.py`

 * *Files identical despite different names*

### Comparing `Navix-0.3.7/tests/test_environments.py` & `Navix-0.3.8/tests/test_environments.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -79,8 +79,8 @@
     return
 
 
 if __name__ == "__main__":
     # test_room()
     # jax.jit(test_room)()
     # test_keydoor()
-    test_keydoor2()
+    test_keydoor2()
```

### Comparing `Navix-0.3.7/tests/test_grid.py` & `Navix-0.3.8/tests/test_grid.py`

 * *Files identical despite different names*

### Comparing `Navix-0.3.7/tests/test_observations.py` & `Navix-0.3.8/tests/test_observations.py`

 * *Files identical despite different names*

### Comparing `Navix-0.3.7/tests/test_tasks.py` & `Navix-0.3.8/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `Navix-0.3.7/tests/test_terminations.py` & `Navix-0.3.8/tests/test_terminations.py`

 * *Files identical despite different names*

