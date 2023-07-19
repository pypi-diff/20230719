# Comparing `tmp/soda-core-denodo-3.0.45.tar.gz` & `tmp/soda-core-denodo-3.0.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda-core-denodo-3.0.45.tar", last modified: Wed Jul 12 09:26:46 2023, max compression
+gzip compressed data, was "soda-core-denodo-3.0.46.tar", last modified: Wed Jul 19 15:16:00 2023, max compression
```

## Comparing `soda-core-denodo-3.0.45.tar` & `soda-core-denodo-3.0.46.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 09:26:46.861708 soda-core-denodo-3.0.45/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-12 09:26:46.861708 soda-core-denodo-3.0.45/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-12 09:26:46.861708 soda-core-denodo-3.0.45/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      657 2023-07-12 09:26:19.000000 soda-core-denodo-3.0.45/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 09:26:46.861708 soda-core-denodo-3.0.45/soda/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 09:26:46.861708 soda-core-denodo-3.0.45/soda/data_sources/
--rw-r--r--   0 runner    (1001) docker     (122)     2479 2023-07-12 09:26:19.000000 soda-core-denodo-3.0.45/soda/data_sources/denodo_data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 09:26:46.861708 soda-core-denodo-3.0.45/soda_core_denodo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-12 09:26:46.000000 soda-core-denodo-3.0.45/soda_core_denodo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-07-12 09:26:46.000000 soda-core-denodo-3.0.45/soda_core_denodo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-12 09:26:46.000000 soda-core-denodo-3.0.45/soda_core_denodo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       45 2023-07-12 09:26:46.000000 soda-core-denodo-3.0.45/soda_core_denodo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-12 09:26:46.000000 soda-core-denodo-3.0.45/soda_core_denodo.egg-info/top_level.txt
+drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-19 15:16:00.432125 soda-core-denodo-3.0.46/
+-rw-r--r--   0 vijay      (501) staff       (20)       61 2023-07-19 15:16:00.431691 soda-core-denodo-3.0.46/PKG-INFO
+-rw-r--r--   0 vijay      (501) staff       (20)       38 2023-07-19 15:16:00.432259 soda-core-denodo-3.0.46/setup.cfg
+-rw-r--r--   0 vijay      (501) staff       (20)      657 2023-07-19 13:37:16.000000 soda-core-denodo-3.0.46/setup.py
+drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-19 15:16:00.426888 soda-core-denodo-3.0.46/soda/
+drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-19 15:16:00.428492 soda-core-denodo-3.0.46/soda/data_sources/
+-rw-r--r--   0 vijay      (501) staff       (20)     2479 2023-06-08 07:54:26.000000 soda-core-denodo-3.0.46/soda/data_sources/denodo_data_source.py
+drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-19 15:16:00.431185 soda-core-denodo-3.0.46/soda_core_denodo.egg-info/
+-rw-r--r--   0 vijay      (501) staff       (20)       61 2023-07-19 15:16:00.000000 soda-core-denodo-3.0.46/soda_core_denodo.egg-info/PKG-INFO
+-rw-r--r--   0 vijay      (501) staff       (20)      247 2023-07-19 15:16:00.000000 soda-core-denodo-3.0.46/soda_core_denodo.egg-info/SOURCES.txt
+-rw-r--r--   0 vijay      (501) staff       (20)        1 2023-07-19 15:16:00.000000 soda-core-denodo-3.0.46/soda_core_denodo.egg-info/dependency_links.txt
+-rw-r--r--   0 vijay      (501) staff       (20)       45 2023-07-19 15:16:00.000000 soda-core-denodo-3.0.46/soda_core_denodo.egg-info/requires.txt
+-rw-r--r--   0 vijay      (501) staff       (20)        5 2023-07-19 15:16:00.000000 soda-core-denodo-3.0.46/soda_core_denodo.egg-info/top_level.txt
```

### Comparing `soda-core-denodo-3.0.45/setup.py` & `soda-core-denodo-3.0.46/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 if sys.version_info < (3, 7):
     print("Error: Soda Core requires at least Python 3.7")
     print("Error: Please upgrade your Python version to 3.7 or later")
     sys.exit(1)
 
 package_name = "soda-core-denodo"
-package_version = "3.0.45"
+package_version = "3.0.46"
 # TODO Add proper description
 description = "Soda Core Denodo Package"
 
 requires = [f"soda-core=={package_version}", f"soda-core-postgres=={package_version}"]
 # TODO Fix the params
 setup(
     name=package_name,
```

### Comparing `soda-core-denodo-3.0.45/soda/data_sources/denodo_data_source.py` & `soda-core-denodo-3.0.46/soda/data_sources/denodo_data_source.py`

 * *Files identical despite different names*

