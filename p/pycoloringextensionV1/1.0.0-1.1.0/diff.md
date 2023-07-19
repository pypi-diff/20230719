# Comparing `tmp/pycoloringextensionV1-1.0.0.tar.gz` & `tmp/pycoloringextensionV1-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycoloringextensionV1-1.0.0.tar", last modified: Wed Jul 19 01:18:57 2023, max compression
+gzip compressed data, was "pycoloringextensionV1-1.1.0.tar", last modified: Wed Jul 19 01:21:02 2023, max compression
```

## Comparing `pycoloringextensionV1-1.0.0.tar` & `pycoloringextensionV1-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 01:18:57.454313 pycoloringextensionV1-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      354 2023-07-19 01:18:57.454313 pycoloringextensionV1-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 01:18:57.454313 pycoloringextensionV1-1.0.0/pycoloringextensionV1/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-19 01:18:57.000000 pycoloringextensionV1-1.0.0/pycoloringextensionV1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 01:18:57.454313 pycoloringextensionV1-1.0.0/pycoloringextensionV1.egg-info/
--rw-r--r--   0 root         (0) root         (0)      354 2023-07-19 01:18:57.000000 pycoloringextensionV1-1.0.0/pycoloringextensionV1.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      222 2023-07-19 01:18:57.000000 pycoloringextensionV1-1.0.0/pycoloringextensionV1.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 01:18:57.000000 pycoloringextensionV1-1.0.0/pycoloringextensionV1.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 01:18:57.000000 pycoloringextensionV1-1.0.0/pycoloringextensionV1.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-19 01:18:57.454313 pycoloringextensionV1-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      567 2023-07-19 01:18:57.000000 pycoloringextensionV1-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 01:21:02.765980 pycoloringextensionV1-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      354 2023-07-19 01:21:02.765980 pycoloringextensionV1-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 01:21:02.765980 pycoloringextensionV1-1.1.0/pycoloringextensionV1/
+-rw-r--r--   0 root         (0) root         (0)    96773 2023-07-19 01:21:02.000000 pycoloringextensionV1-1.1.0/pycoloringextensionV1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 01:21:02.765980 pycoloringextensionV1-1.1.0/pycoloringextensionV1.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      354 2023-07-19 01:21:02.000000 pycoloringextensionV1-1.1.0/pycoloringextensionV1.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      222 2023-07-19 01:21:02.000000 pycoloringextensionV1-1.1.0/pycoloringextensionV1.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 01:21:02.000000 pycoloringextensionV1-1.1.0/pycoloringextensionV1.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-19 01:21:02.000000 pycoloringextensionV1-1.1.0/pycoloringextensionV1.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-19 01:21:02.765980 pycoloringextensionV1-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      567 2023-07-19 01:21:02.000000 pycoloringextensionV1-1.1.0/setup.py
```

### Comparing `pycoloringextensionV1-1.0.0/setup.py` & `pycoloringextensionV1-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="pycoloringextensionV1",
     version=VERSION,
```

