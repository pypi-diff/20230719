# Comparing `tmp/dagster-hightouch-0.1.1.tar.gz` & `tmp/dagster-hightouch-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-hightouch-0.1.1.tar", last modified: Thu Jun 23 20:29:00 2022, max compression
+gzip compressed data, was "dagster-hightouch-0.1.5.tar", last modified: Wed Jul 19 15:00:23 2023, max compression
```

## Comparing `dagster-hightouch-0.1.1.tar` & `dagster-hightouch-0.1.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-23 20:29:00.155879 dagster-hightouch-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-06-23 20:28:52.000000 dagster-hightouch-0.1.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-23 20:29:00.155879 dagster-hightouch-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-23 20:29:00.155879 dagster-hightouch-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      879 2022-06-23 20:28:52.000000 dagster-hightouch-0.1.1/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)     3116 2022-06-23 20:28:52.000000 dagster-hightouch-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)    10174 2022-06-23 20:28:52.000000 dagster-hightouch-0.1.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-06-23 20:28:52.000000 dagster-hightouch-0.1.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      877 2022-06-23 20:29:00.155879 dagster-hightouch-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      426 2022-06-23 20:28:52.000000 dagster-hightouch-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-23 20:29:00.155879 dagster-hightouch-0.1.1/dagster_hightouch/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-23 20:28:52.000000 dagster-hightouch-0.1.1/dagster_hightouch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-06-23 20:28:59.000000 dagster-hightouch-0.1.1/dagster_hightouch/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     2951 2022-06-23 20:28:52.000000 dagster-hightouch-0.1.1/dagster_hightouch/ops.py
--rw-r--r--   0 runner    (1001) docker     (121)    10092 2022-06-23 20:28:52.000000 dagster-hightouch-0.1.1/dagster_hightouch/resources.py
--rw-r--r--   0 runner    (1001) docker     (121)     1292 2022-06-23 20:28:52.000000 dagster-hightouch-0.1.1/dagster_hightouch/types.py
--rw-r--r--   0 runner    (1001) docker     (121)     2352 2022-06-23 20:28:52.000000 dagster-hightouch-0.1.1/dagster_hightouch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-23 20:29:00.155879 dagster-hightouch-0.1.1/dagster_hightouch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      877 2022-06-23 20:28:59.000000 dagster-hightouch-0.1.1/dagster_hightouch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      482 2022-06-23 20:29:00.000000 dagster-hightouch-0.1.1/dagster_hightouch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-23 20:28:59.000000 dagster-hightouch-0.1.1/dagster_hightouch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-06-23 20:28:59.000000 dagster-hightouch-0.1.1/dagster_hightouch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-06-23 20:29:00.000000 dagster-hightouch-0.1.1/dagster_hightouch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      297 2022-06-23 20:28:52.000000 dagster-hightouch-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      562 2022-06-23 20:29:00.155879 dagster-hightouch-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:00:23.630497 dagster-hightouch-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-19 15:00:17.000000 dagster-hightouch-0.1.5/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:00:23.626497 dagster-hightouch-0.1.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:00:23.626497 dagster-hightouch-0.1.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-19 15:00:17.000000 dagster-hightouch-0.1.5/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-07-19 15:00:17.000000 dagster-hightouch-0.1.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-19 15:00:17.000000 dagster-hightouch-0.1.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-19 15:00:17.000000 dagster-hightouch-0.1.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-07-19 15:00:23.630497 dagster-hightouch-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-19 15:00:17.000000 dagster-hightouch-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:00:23.630497 dagster-hightouch-0.1.5/dagster_hightouch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:00:17.000000 dagster-hightouch-0.1.5/dagster_hightouch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-19 15:00:23.000000 dagster-hightouch-0.1.5/dagster_hightouch/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-19 15:00:17.000000 dagster-hightouch-0.1.5/dagster_hightouch/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10092 2023-07-19 15:00:17.000000 dagster-hightouch-0.1.5/dagster_hightouch/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-19 15:00:17.000000 dagster-hightouch-0.1.5/dagster_hightouch/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-19 15:00:17.000000 dagster-hightouch-0.1.5/dagster_hightouch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:00:23.630497 dagster-hightouch-0.1.5/dagster_hightouch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-07-19 15:00:23.000000 dagster-hightouch-0.1.5/dagster_hightouch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-19 15:00:23.000000 dagster-hightouch-0.1.5/dagster_hightouch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 15:00:23.000000 dagster-hightouch-0.1.5/dagster_hightouch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-19 15:00:23.000000 dagster-hightouch-0.1.5/dagster_hightouch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-19 15:00:23.000000 dagster-hightouch-0.1.5/dagster_hightouch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-19 15:00:17.000000 dagster-hightouch-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-19 15:00:23.630497 dagster-hightouch-0.1.5/setup.cfg
```

### Comparing `dagster-hightouch-0.1.1/.github/workflows/pypi-publish.yml` & `dagster-hightouch-0.1.5/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `dagster-hightouch-0.1.1/.gitignore` & `dagster-hightouch-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `dagster-hightouch-0.1.1/LICENSE.md` & `dagster-hightouch-0.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dagster-hightouch-0.1.1/dagster_hightouch/ops.py` & `dagster-hightouch-0.1.5/dagster_hightouch/ops.py`

 * *Files identical despite different names*

### Comparing `dagster-hightouch-0.1.1/dagster_hightouch/resources.py` & `dagster-hightouch-0.1.5/dagster_hightouch/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-hightouch-0.1.1/dagster_hightouch/types.py` & `dagster-hightouch-0.1.5/dagster_hightouch/types.py`

 * *Files identical despite different names*

### Comparing `dagster-hightouch-0.1.1/dagster_hightouch/utils.py` & `dagster-hightouch-0.1.5/dagster_hightouch/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-hightouch-0.1.1/setup.cfg` & `dagster-hightouch-0.1.5/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -11,14 +11,14 @@
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 packages = dagster_hightouch
 python_requires = >=3.8
 install_requires = 
-	dagster >= "0.14"
-	requests >= "2.0"
+	dagster>=0.14
+	requests>=2.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

