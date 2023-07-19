# Comparing `tmp/mongoy-0.0.1.tar.gz` & `tmp/mongoy-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongoy-0.0.1.tar", last modified: Tue Jul 18 16:09:44 2023, max compression
+gzip compressed data, was "mongoy-0.1.0.tar", last modified: Tue Jul 18 17:31:19 2023, max compression
```

## Comparing `mongoy-0.0.1.tar` & `mongoy-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jarmanrandhawa   (501) staff       (20)        0 2023-07-18 16:09:44.846048 mongoy-0.0.1/
--rw-r--r--   0 jarmanrandhawa   (501) staff       (20)     1061 2023-07-18 15:58:12.000000 mongoy-0.0.1/LICENSE
--rw-r--r--   0 jarmanrandhawa   (501) staff       (20)      409 2023-07-18 16:09:44.845867 mongoy-0.0.1/PKG-INFO
--rw-r--r--   0 jarmanrandhawa   (501) staff       (20)       71 2023-07-18 15:56:36.000000 mongoy-0.0.1/README.md
-drwxr-xr-x   0 jarmanrandhawa   (501) staff       (20)        0 2023-07-18 16:09:44.843845 mongoy-0.0.1/mongoy/
-drwxr-xr-x   0 jarmanrandhawa   (501) staff       (20)        0 2023-07-18 16:09:44.845629 mongoy-0.0.1/mongoy/mongoy.egg-info/
--rw-r--r--   0 jarmanrandhawa   (501) staff       (20)      409 2023-07-18 16:09:44.000000 mongoy-0.0.1/mongoy/mongoy.egg-info/PKG-INFO
--rw-r--r--   0 jarmanrandhawa   (501) staff       (20)      210 2023-07-18 16:09:44.000000 mongoy-0.0.1/mongoy/mongoy.egg-info/SOURCES.txt
--rw-r--r--   0 jarmanrandhawa   (501) staff       (20)        1 2023-07-18 16:09:44.000000 mongoy-0.0.1/mongoy/mongoy.egg-info/dependency_links.txt
--rw-r--r--   0 jarmanrandhawa   (501) staff       (20)        8 2023-07-18 16:09:44.000000 mongoy-0.0.1/mongoy/mongoy.egg-info/requires.txt
--rw-r--r--   0 jarmanrandhawa   (501) staff       (20)        7 2023-07-18 16:09:44.000000 mongoy-0.0.1/mongoy/mongoy.egg-info/top_level.txt
--rw-r--r--   0 jarmanrandhawa   (501) staff       (20)       38 2023-07-18 16:09:44.846089 mongoy-0.0.1/setup.cfg
--rw-r--r--   0 jarmanrandhawa   (501) staff       (20)     1188 2023-07-18 16:08:15.000000 mongoy-0.0.1/setup.py
+drwxr-xr-x   0 jarmanrandhawa   (501) staff       (20)        0 2023-07-18 17:31:19.644498 mongoy-0.1.0/
+-rw-r--r--   0 jarmanrandhawa   (501) staff       (20)     1061 2023-07-18 15:58:12.000000 mongoy-0.1.0/LICENSE
+-rw-r--r--   0 jarmanrandhawa   (501) staff       (20)      409 2023-07-18 17:31:19.644364 mongoy-0.1.0/PKG-INFO
+-rw-r--r--   0 jarmanrandhawa   (501) staff       (20)       71 2023-07-18 15:56:36.000000 mongoy-0.1.0/README.md
+drwxr-xr-x   0 jarmanrandhawa   (501) staff       (20)        0 2023-07-18 17:31:19.642915 mongoy-0.1.0/mongoy/
+drwxr-xr-x   0 jarmanrandhawa   (501) staff       (20)        0 2023-07-18 17:31:19.644194 mongoy-0.1.0/mongoy/mongoy.egg-info/
+-rw-r--r--   0 jarmanrandhawa   (501) staff       (20)      409 2023-07-18 17:31:19.000000 mongoy-0.1.0/mongoy/mongoy.egg-info/PKG-INFO
+-rw-r--r--   0 jarmanrandhawa   (501) staff       (20)      210 2023-07-18 17:31:19.000000 mongoy-0.1.0/mongoy/mongoy.egg-info/SOURCES.txt
+-rw-r--r--   0 jarmanrandhawa   (501) staff       (20)        1 2023-07-18 17:31:19.000000 mongoy-0.1.0/mongoy/mongoy.egg-info/dependency_links.txt
+-rw-r--r--   0 jarmanrandhawa   (501) staff       (20)        8 2023-07-18 17:31:19.000000 mongoy-0.1.0/mongoy/mongoy.egg-info/requires.txt
+-rw-r--r--   0 jarmanrandhawa   (501) staff       (20)        7 2023-07-18 17:31:19.000000 mongoy-0.1.0/mongoy/mongoy.egg-info/top_level.txt
+-rw-r--r--   0 jarmanrandhawa   (501) staff       (20)       38 2023-07-18 17:31:19.644538 mongoy-0.1.0/setup.cfg
+-rw-r--r--   0 jarmanrandhawa   (501) staff       (20)     1188 2023-07-18 17:30:38.000000 mongoy-0.1.0/setup.py
```

### Comparing `mongoy-0.0.1/LICENSE` & `mongoy-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mongoy-0.0.1/setup.py` & `mongoy-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mongoy",                     # This is the name of the package
-    version="0.0.1",                        # The initial release version
+    version="0.1.0",                        # The initial release version
     author="pavittarx",                     # Full name of the author
     description="wrapper utility for mongodb",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
```

