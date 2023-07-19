# Comparing `tmp/pipcoloringsliberyV1-1.0.0.tar.gz` & `tmp/pipcoloringsliberyV1-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipcoloringsliberyV1-1.0.0.tar", last modified: Wed Jul 19 02:48:02 2023, max compression
+gzip compressed data, was "pipcoloringsliberyV1-1.1.0.tar", last modified: Wed Jul 19 02:50:07 2023, max compression
```

## Comparing `pipcoloringsliberyV1-1.0.0.tar` & `pipcoloringsliberyV1-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 02:48:02.324639 pipcoloringsliberyV1-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      353 2023-07-19 02:48:02.324639 pipcoloringsliberyV1-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 02:48:02.320639 pipcoloringsliberyV1-1.0.0/pipcoloringsliberyV1/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-19 02:48:01.000000 pipcoloringsliberyV1-1.0.0/pipcoloringsliberyV1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 02:48:02.324639 pipcoloringsliberyV1-1.0.0/pipcoloringsliberyV1.egg-info/
--rw-r--r--   0 root         (0) root         (0)      353 2023-07-19 02:48:02.000000 pipcoloringsliberyV1-1.0.0/pipcoloringsliberyV1.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      217 2023-07-19 02:48:02.000000 pipcoloringsliberyV1-1.0.0/pipcoloringsliberyV1.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 02:48:02.000000 pipcoloringsliberyV1-1.0.0/pipcoloringsliberyV1.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-19 02:48:02.000000 pipcoloringsliberyV1-1.0.0/pipcoloringsliberyV1.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-19 02:48:02.324639 pipcoloringsliberyV1-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      566 2023-07-19 02:48:01.000000 pipcoloringsliberyV1-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 02:50:07.564244 pipcoloringsliberyV1-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      353 2023-07-19 02:50:07.560243 pipcoloringsliberyV1-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 02:50:07.560243 pipcoloringsliberyV1-1.1.0/pipcoloringsliberyV1/
+-rw-r--r--   0 root         (0) root         (0)    96773 2023-07-19 02:50:07.000000 pipcoloringsliberyV1-1.1.0/pipcoloringsliberyV1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 02:50:07.560243 pipcoloringsliberyV1-1.1.0/pipcoloringsliberyV1.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      353 2023-07-19 02:50:07.000000 pipcoloringsliberyV1-1.1.0/pipcoloringsliberyV1.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      217 2023-07-19 02:50:07.000000 pipcoloringsliberyV1-1.1.0/pipcoloringsliberyV1.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 02:50:07.000000 pipcoloringsliberyV1-1.1.0/pipcoloringsliberyV1.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-19 02:50:07.000000 pipcoloringsliberyV1-1.1.0/pipcoloringsliberyV1.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-19 02:50:07.564244 pipcoloringsliberyV1-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      566 2023-07-19 02:50:07.000000 pipcoloringsliberyV1-1.1.0/setup.py
```

### Comparing `pipcoloringsliberyV1-1.0.0/setup.py` & `pipcoloringsliberyV1-1.1.0/setup.py`

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
     name="pipcoloringsliberyV1",
     version=VERSION,
```

