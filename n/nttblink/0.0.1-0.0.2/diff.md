# Comparing `tmp/nttblink-0.0.1.tar.gz` & `tmp/nttblink-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nttblink-0.0.1.tar", last modified: Tue Jul 18 16:35:32 2023, max compression
+gzip compressed data, was "nttblink-0.0.2.tar", last modified: Tue Jul 18 17:20:56 2023, max compression
```

## Comparing `nttblink-0.0.1.tar` & `nttblink-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 austin     (501) staff       (20)        0 2023-07-18 16:35:32.110170 nttblink-0.0.1/
--rw-r--r--   0 austin     (501) staff       (20)     4303 2023-07-18 16:35:32.109906 nttblink-0.0.1/PKG-INFO
--rw-r--r--   0 austin     (501) staff       (20)     3793 2023-07-18 16:23:55.000000 nttblink-0.0.1/README.md
-drwxr-xr-x   0 austin     (501) staff       (20)        0 2023-07-18 16:35:32.108198 nttblink-0.0.1/nttblink/
--rw-r--r--   0 austin     (501) staff       (20)       47 2023-07-18 16:01:00.000000 nttblink-0.0.1/nttblink/__init__.py
--rw-r--r--   0 austin     (501) staff       (20)     4761 2023-07-18 16:01:00.000000 nttblink-0.0.1/nttblink/nttblink.py
--rw-r--r--   0 austin     (501) staff       (20)      495 2023-07-18 16:01:00.000000 nttblink-0.0.1/nttblink/setup.py
-drwxr-xr-x   0 austin     (501) staff       (20)        0 2023-07-18 16:35:32.109573 nttblink-0.0.1/nttblink.egg-info/
--rw-r--r--   0 austin     (501) staff       (20)     4303 2023-07-18 16:35:32.000000 nttblink-0.0.1/nttblink.egg-info/PKG-INFO
--rw-r--r--   0 austin     (501) staff       (20)      212 2023-07-18 16:35:32.000000 nttblink-0.0.1/nttblink.egg-info/SOURCES.txt
--rw-r--r--   0 austin     (501) staff       (20)        1 2023-07-18 16:35:32.000000 nttblink-0.0.1/nttblink.egg-info/dependency_links.txt
--rw-r--r--   0 austin     (501) staff       (20)        9 2023-07-18 16:35:32.000000 nttblink-0.0.1/nttblink.egg-info/top_level.txt
--rw-r--r--   0 austin     (501) staff       (20)      604 2023-07-18 16:30:11.000000 nttblink-0.0.1/pyproject.toml
--rw-r--r--   0 austin     (501) staff       (20)       38 2023-07-18 16:35:32.110254 nttblink-0.0.1/setup.cfg
+drwxr-xr-x   0 austin     (501) staff       (20)        0 2023-07-18 17:20:56.021572 nttblink-0.0.2/
+-rw-r--r--   0 austin     (501) staff       (20)     4303 2023-07-18 17:20:56.021427 nttblink-0.0.2/PKG-INFO
+-rw-r--r--   0 austin     (501) staff       (20)     3793 2023-07-18 16:23:55.000000 nttblink-0.0.2/README.md
+drwxr-xr-x   0 austin     (501) staff       (20)        0 2023-07-18 17:20:56.020496 nttblink-0.0.2/nttblink/
+-rw-r--r--   0 austin     (501) staff       (20)       47 2023-07-18 16:01:00.000000 nttblink-0.0.2/nttblink/__init__.py
+-rw-r--r--   0 austin     (501) staff       (20)     4761 2023-07-18 16:01:00.000000 nttblink-0.0.2/nttblink/nttblink.py
+-rw-r--r--   0 austin     (501) staff       (20)      488 2023-07-18 17:18:54.000000 nttblink-0.0.2/nttblink/setup.py
+drwxr-xr-x   0 austin     (501) staff       (20)        0 2023-07-18 17:20:56.021224 nttblink-0.0.2/nttblink.egg-info/
+-rw-r--r--   0 austin     (501) staff       (20)     4303 2023-07-18 17:20:56.000000 nttblink-0.0.2/nttblink.egg-info/PKG-INFO
+-rw-r--r--   0 austin     (501) staff       (20)      212 2023-07-18 17:20:56.000000 nttblink-0.0.2/nttblink.egg-info/SOURCES.txt
+-rw-r--r--   0 austin     (501) staff       (20)        1 2023-07-18 17:20:56.000000 nttblink-0.0.2/nttblink.egg-info/dependency_links.txt
+-rw-r--r--   0 austin     (501) staff       (20)        9 2023-07-18 17:20:56.000000 nttblink-0.0.2/nttblink.egg-info/top_level.txt
+-rw-r--r--   0 austin     (501) staff       (20)      604 2023-07-18 17:17:41.000000 nttblink-0.0.2/pyproject.toml
+-rw-r--r--   0 austin     (501) staff       (20)       38 2023-07-18 17:20:56.021619 nttblink-0.0.2/setup.cfg
```

### Comparing `nttblink-0.0.1/PKG-INFO` & `nttblink-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nttblink
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small nttblink connector package
 Author-email: Austin Arlint <austin.arlint@global.ntt>
 Project-URL: Homepage, https://github.com/NTT-AM-DDD/python-nttblink
 Project-URL: Bug Tracker, https://github.com/NTT-AM-DDD/python-nttblink/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nttblink-0.0.1/README.md` & `nttblink-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `nttblink-0.0.1/nttblink/nttblink.py` & `nttblink-0.0.2/nttblink/nttblink.py`

 * *Files identical despite different names*

### Comparing `nttblink-0.0.1/nttblink.egg-info/PKG-INFO` & `nttblink-0.0.2/nttblink.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nttblink
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small nttblink connector package
 Author-email: Austin Arlint <austin.arlint@global.ntt>
 Project-URL: Homepage, https://github.com/NTT-AM-DDD/python-nttblink
 Project-URL: Bug Tracker, https://github.com/NTT-AM-DDD/python-nttblink/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nttblink-0.0.1/pyproject.toml` & `nttblink-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nttblink"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Austin Arlint", email="austin.arlint@global.ntt" },
 ]
 description = "A small nttblink connector package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

