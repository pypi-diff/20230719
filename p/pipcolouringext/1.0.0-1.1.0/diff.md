# Comparing `tmp/pipcolouringext-1.0.0.tar.gz` & `tmp/pipcolouringext-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipcolouringext-1.0.0.tar", last modified: Wed Jul 19 03:40:31 2023, max compression
+gzip compressed data, was "pipcolouringext-1.1.0.tar", last modified: Wed Jul 19 03:42:37 2023, max compression
```

## Comparing `pipcolouringext-1.0.0.tar` & `pipcolouringext-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:40:31.617759 pipcolouringext-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      348 2023-07-19 03:40:31.617759 pipcolouringext-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:40:31.617759 pipcolouringext-1.0.0/pipcolouringext/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-19 03:40:31.000000 pipcolouringext-1.0.0/pipcolouringext/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:40:31.617759 pipcolouringext-1.0.0/pipcolouringext.egg-info/
--rw-r--r--   0 root         (0) root         (0)      348 2023-07-19 03:40:31.000000 pipcolouringext-1.0.0/pipcolouringext.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      192 2023-07-19 03:40:31.000000 pipcolouringext-1.0.0/pipcolouringext.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 03:40:31.000000 pipcolouringext-1.0.0/pipcolouringext.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-07-19 03:40:31.000000 pipcolouringext-1.0.0/pipcolouringext.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-19 03:40:31.617759 pipcolouringext-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      561 2023-07-19 03:40:31.000000 pipcolouringext-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:42:37.309312 pipcolouringext-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      348 2023-07-19 03:42:37.309312 pipcolouringext-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:42:37.305312 pipcolouringext-1.1.0/pipcolouringext/
+-rw-r--r--   0 root         (0) root         (0)    96773 2023-07-19 03:42:36.000000 pipcolouringext-1.1.0/pipcolouringext/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 03:42:37.309312 pipcolouringext-1.1.0/pipcolouringext.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      348 2023-07-19 03:42:37.000000 pipcolouringext-1.1.0/pipcolouringext.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      192 2023-07-19 03:42:37.000000 pipcolouringext-1.1.0/pipcolouringext.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 03:42:37.000000 pipcolouringext-1.1.0/pipcolouringext.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-19 03:42:37.000000 pipcolouringext-1.1.0/pipcolouringext.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-19 03:42:37.309312 pipcolouringext-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      561 2023-07-19 03:42:36.000000 pipcolouringext-1.1.0/setup.py
```

### Comparing `pipcolouringext-1.0.0/setup.py` & `pipcolouringext-1.1.0/setup.py`

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
     name="pipcolouringext",
     version=VERSION,
```

