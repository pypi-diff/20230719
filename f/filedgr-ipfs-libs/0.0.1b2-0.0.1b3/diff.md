# Comparing `tmp/filedgr-ipfs-libs-0.0.1b2.tar.gz` & `tmp/filedgr-ipfs-libs-0.0.1b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/ericfalk/ws_filedgr/filedgr-python-lib-ipfs/dist/tmp3xv9fzvz/filedgr-ipfs-libs-0.0.1b2.tar", last modified: Mon Nov 14 13:48:52 2022, max compression
+gzip compressed data, was "filedgr-ipfs-libs-0.0.1b3.tar", last modified: Wed Jul 19 12:55:54 2023, max compression
```

## Comparing `filedgr-ipfs-libs-0.0.1b2.tar` & `filedgr-ipfs-libs-0.0.1b3.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 ericfalk   (501) staff       (20)        0 2022-11-14 13:48:52.992743 filedgr-ipfs-libs-0.0.1b2/
--rw-r--r--   0 ericfalk   (501) staff       (20)     1063 2022-06-18 17:54:13.000000 filedgr-ipfs-libs-0.0.1b2/LICENSE
--rw-r--r--   0 ericfalk   (501) staff       (20)      613 2022-11-14 13:48:52.992871 filedgr-ipfs-libs-0.0.1b2/PKG-INFO
--rw-r--r--   0 ericfalk   (501) staff       (20)       83 2022-11-12 18:36:02.000000 filedgr-ipfs-libs-0.0.1b2/README.md
--rw-r--r--   0 ericfalk   (501) staff       (20)     1428 2022-11-14 13:48:19.000000 filedgr-ipfs-libs-0.0.1b2/pyproject.toml
--rw-r--r--   0 ericfalk   (501) staff       (20)      142 2022-11-14 13:48:52.993299 filedgr-ipfs-libs-0.0.1b2/setup.cfg
-drwxr-xr-x   0 ericfalk   (501) staff       (20)        0 2022-11-14 13:48:52.987086 filedgr-ipfs-libs-0.0.1b2/src/
-drwxr-xr-x   0 ericfalk   (501) staff       (20)        0 2022-11-14 13:48:52.990393 filedgr-ipfs-libs-0.0.1b2/src/filedgr_ipfs_libs.egg-info/
--rw-r--r--   0 ericfalk   (501) staff       (20)      613 2022-11-14 13:48:52.000000 filedgr-ipfs-libs-0.0.1b2/src/filedgr_ipfs_libs.egg-info/PKG-INFO
--rw-r--r--   0 ericfalk   (501) staff       (20)      415 2022-11-14 13:48:52.000000 filedgr-ipfs-libs-0.0.1b2/src/filedgr_ipfs_libs.egg-info/SOURCES.txt
--rw-r--r--   0 ericfalk   (501) staff       (20)        1 2022-11-14 13:48:52.000000 filedgr-ipfs-libs-0.0.1b2/src/filedgr_ipfs_libs.egg-info/dependency_links.txt
--rw-r--r--   0 ericfalk   (501) staff       (20)      126 2022-11-14 13:48:52.000000 filedgr-ipfs-libs-0.0.1b2/src/filedgr_ipfs_libs.egg-info/requires.txt
--rw-r--r--   0 ericfalk   (501) staff       (20)       17 2022-11-14 13:48:52.000000 filedgr-ipfs-libs-0.0.1b2/src/filedgr_ipfs_libs.egg-info/top_level.txt
-drwxr-xr-x   0 ericfalk   (501) staff       (20)        0 2022-11-14 13:48:52.991351 filedgr-ipfs-libs-0.0.1b2/src/filedgr_lib_ipfs/
--rw-r--r--   0 ericfalk   (501) staff       (20)       28 2022-11-14 13:48:24.000000 filedgr-ipfs-libs-0.0.1b2/src/filedgr_lib_ipfs/__init__.py
--rw-r--r--   0 ericfalk   (501) staff       (20)     2432 2022-11-14 13:47:49.000000 filedgr-ipfs-libs-0.0.1b2/src/filedgr_lib_ipfs/ipfs_client.py
-drwxr-xr-x   0 ericfalk   (501) staff       (20)        0 2022-11-14 13:48:52.992172 filedgr-ipfs-libs-0.0.1b2/src/filedgr_lib_ipfs/my_io/
--rw-r--r--   0 ericfalk   (501) staff       (20)        0 2022-06-18 17:23:43.000000 filedgr-ipfs-libs-0.0.1b2/src/filedgr_lib_ipfs/my_io/__init__.py
--rw-r--r--   0 ericfalk   (501) staff       (20)      508 2022-06-18 17:40:10.000000 filedgr-ipfs-libs-0.0.1b2/src/filedgr_lib_ipfs/my_io/my_file_io.py
+drwxr-xr-x   0 ericfalk   (501) staff       (20)        0 2023-07-19 12:55:54.263532 filedgr-ipfs-libs-0.0.1b3/
+-rw-r--r--   0 ericfalk   (501) staff       (20)     1063 2022-06-18 17:54:13.000000 filedgr-ipfs-libs-0.0.1b3/LICENSE
+-rw-r--r--   0 ericfalk   (501) staff       (20)      613 2023-07-19 12:55:54.263688 filedgr-ipfs-libs-0.0.1b3/PKG-INFO
+-rw-r--r--   0 ericfalk   (501) staff       (20)       83 2022-11-12 18:36:02.000000 filedgr-ipfs-libs-0.0.1b3/README.md
+-rw-r--r--   0 ericfalk   (501) staff       (20)     1384 2023-07-19 12:52:57.000000 filedgr-ipfs-libs-0.0.1b3/pyproject.toml
+-rw-r--r--   0 ericfalk   (501) staff       (20)      142 2023-07-19 12:55:54.264534 filedgr-ipfs-libs-0.0.1b3/setup.cfg
+drwxr-xr-x   0 ericfalk   (501) staff       (20)        0 2023-07-19 12:55:54.256606 filedgr-ipfs-libs-0.0.1b3/src/
+drwxr-xr-x   0 ericfalk   (501) staff       (20)        0 2023-07-19 12:55:54.259995 filedgr-ipfs-libs-0.0.1b3/src/filedgr_ipfs_libs.egg-info/
+-rw-r--r--   0 ericfalk   (501) staff       (20)      613 2023-07-19 12:55:54.000000 filedgr-ipfs-libs-0.0.1b3/src/filedgr_ipfs_libs.egg-info/PKG-INFO
+-rw-r--r--   0 ericfalk   (501) staff       (20)      441 2023-07-19 12:55:54.000000 filedgr-ipfs-libs-0.0.1b3/src/filedgr_ipfs_libs.egg-info/SOURCES.txt
+-rw-r--r--   0 ericfalk   (501) staff       (20)        1 2023-07-19 12:55:54.000000 filedgr-ipfs-libs-0.0.1b3/src/filedgr_ipfs_libs.egg-info/dependency_links.txt
+-rw-r--r--   0 ericfalk   (501) staff       (20)       96 2023-07-19 12:55:54.000000 filedgr-ipfs-libs-0.0.1b3/src/filedgr_ipfs_libs.egg-info/requires.txt
+-rw-r--r--   0 ericfalk   (501) staff       (20)       17 2023-07-19 12:55:54.000000 filedgr-ipfs-libs-0.0.1b3/src/filedgr_ipfs_libs.egg-info/top_level.txt
+drwxr-xr-x   0 ericfalk   (501) staff       (20)        0 2023-07-19 12:55:54.260969 filedgr-ipfs-libs-0.0.1b3/src/filedgr_lib_ipfs/
+-rw-r--r--   0 ericfalk   (501) staff       (20)       28 2023-07-19 12:53:15.000000 filedgr-ipfs-libs-0.0.1b3/src/filedgr_lib_ipfs/__init__.py
+-rw-r--r--   0 ericfalk   (501) staff       (20)     2430 2023-07-18 20:52:09.000000 filedgr-ipfs-libs-0.0.1b3/src/filedgr_lib_ipfs/ipfs_client.py
+drwxr-xr-x   0 ericfalk   (501) staff       (20)        0 2023-07-19 12:55:54.262148 filedgr-ipfs-libs-0.0.1b3/src/filedgr_lib_ipfs/my_io/
+-rw-r--r--   0 ericfalk   (501) staff       (20)        0 2022-06-18 17:23:43.000000 filedgr-ipfs-libs-0.0.1b3/src/filedgr_lib_ipfs/my_io/__init__.py
+-rw-r--r--   0 ericfalk   (501) staff       (20)      508 2022-06-18 17:40:10.000000 filedgr-ipfs-libs-0.0.1b3/src/filedgr_lib_ipfs/my_io/my_file_io.py
+drwxr-xr-x   0 ericfalk   (501) staff       (20)        0 2023-07-19 12:55:54.262733 filedgr-ipfs-libs-0.0.1b3/tests/
+-rw-r--r--   0 ericfalk   (501) staff       (20)      992 2022-11-14 13:11:42.000000 filedgr-ipfs-libs-0.0.1b3/tests/test_ipfs_client.py
```

### Comparing `filedgr-ipfs-libs-0.0.1b2/LICENSE` & `filedgr-ipfs-libs-0.0.1b3/LICENSE`

 * *Files identical despite different names*

### Comparing `filedgr-ipfs-libs-0.0.1b2/PKG-INFO` & `filedgr-ipfs-libs-0.0.1b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filedgr-ipfs-libs
-Version: 0.0.1b2
+Version: 0.0.1b3
 Summary: Python libs to interact with the IPFS node
 Author-email: Filedgr <code@filedgr.com>
 Project-URL: repository, https://github.com/Filedgr/filedgr-python-lib-ipfs
 Keywords: filedgr,ipfs,lib
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `filedgr-ipfs-libs-0.0.1b2/pyproject.toml` & `filedgr-ipfs-libs-0.0.1b3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "filedgr-ipfs-libs"
-version = "0.0.1-beta.2"
+version = "0.0.1-beta.3"
 requires-python = ">=3.9"
 description = "Python libs to interact with the IPFS node"
 readme = "README.md"
 authors = [{ name = "Filedgr", email = "code@filedgr.com" }]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["filedgr", "ipfs", "lib"]
 dependencies = [
-    "aiohttp>=3.8.1",
-    "cchardet>=2.1.7",
-    "aiodns>=3.0.0",
-    "orjson==3.7.2"]
+    "aiohttp==3.8.2",
+    "aiodns==3.0.0"]
 
 [project.optional-dependencies]
 build = ["build", "twine"]
 dev = ["black", "bumpver", "isort", "mypy", "pytest", "flake8"]
 
 [project.urls]
 repository = "https://github.com/Filedgr/filedgr-python-lib-ipfs"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 exclude = ["tests*"]
 
 [tool.bumpver]
-current_version = "0.0.1-beta.2"
+current_version = "0.0.1-beta.3"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = false
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `filedgr-ipfs-libs-0.0.1b2/src/filedgr_ipfs_libs.egg-info/PKG-INFO` & `filedgr-ipfs-libs-0.0.1b3/src/filedgr_ipfs_libs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filedgr-ipfs-libs
-Version: 0.0.1b2
+Version: 0.0.1b3
 Summary: Python libs to interact with the IPFS node
 Author-email: Filedgr <code@filedgr.com>
 Project-URL: repository, https://github.com/Filedgr/filedgr-python-lib-ipfs
 Keywords: filedgr,ipfs,lib
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `filedgr-ipfs-libs-0.0.1b2/src/filedgr_lib_ipfs/ipfs_client.py` & `filedgr-ipfs-libs-0.0.1b3/src/filedgr_lib_ipfs/ipfs_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import os
-
 import aiohttp
-
 from filedgr_lib_ipfs.my_io.my_file_io import build_dir_tree
 
 
 class IpfsClient:
 
     def __init__(self, host: str, port: int, protocol: str = "http", **kwargs):
         if host is None and port is None and 'host' not in kwargs and 'port' not in kwargs:
```

