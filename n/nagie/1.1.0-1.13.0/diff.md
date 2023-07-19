# Comparing `tmp/nagie-1.1.0.tar.gz` & `tmp/nagie-1.13.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nagie-1.1.0.tar", last modified: Wed Jul 19 13:35:58 2023, max compression
+gzip compressed data, was "nagie-1.13.0.tar", last modified: Wed Jul 19 13:40:45 2023, max compression
```

## Comparing `nagie-1.1.0.tar` & `nagie-1.13.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 13:35:58.746833 nagie-1.1.0/
--rw-rw-rw-   0        0        0      300 2023-07-19 13:35:58.745834 nagie-1.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-19 13:35:58.703834 nagie-1.1.0/nagie.egg-info/
--rw-rw-rw-   0        0        0      300 2023-07-19 13:35:56.000000 nagie-1.1.0/nagie.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      160 2023-07-19 13:35:57.000000 nagie-1.1.0/nagie.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 13:35:56.000000 nagie-1.1.0/nagie.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-19 13:35:56.000000 nagie-1.1.0/nagie.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-19 13:35:58.733833 nagie-1.1.0/nagogy/
--rw-rw-rw-   0        0        0       25 2023-03-26 12:23:21.000000 nagie-1.1.0/nagogy/__init__.py
--rw-rw-rw-   0        0        0      222 2023-07-19 13:32:10.000000 nagie-1.1.0/nagogy/nagogy.py
--rw-rw-rw-   0        0        0       42 2023-07-19 13:35:58.746833 nagie-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      864 2023-07-19 13:35:31.000000 nagie-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 13:40:45.379836 nagie-1.13.0/
+-rw-rw-rw-   0        0        0      301 2023-07-19 13:40:45.378836 nagie-1.13.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-19 13:40:45.375837 nagie-1.13.0/nagie.egg-info/
+-rw-rw-rw-   0        0        0      301 2023-07-19 13:40:45.000000 nagie-1.13.0/nagie.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      160 2023-07-19 13:40:45.000000 nagie-1.13.0/nagie.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 13:40:45.000000 nagie-1.13.0/nagie.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-19 13:40:45.000000 nagie-1.13.0/nagie.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-19 13:40:45.377836 nagie-1.13.0/nagogy/
+-rw-rw-rw-   0        0        0       25 2023-03-26 12:23:21.000000 nagie-1.13.0/nagogy/__init__.py
+-rw-rw-rw-   0        0        0      222 2023-07-19 13:32:10.000000 nagie-1.13.0/nagogy/nagogy.py
+-rw-rw-rw-   0        0        0       42 2023-07-19 13:40:45.379836 nagie-1.13.0/setup.cfg
+-rw-rw-rw-   0        0        0      865 2023-07-19 13:40:17.000000 nagie-1.13.0/setup.py
```

### Comparing `nagie-1.1.0/setup.py` & `nagie-1.13.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.1.0'
+VERSION = '1.13.0'
 DESCRIPTION = 'normal nagie'
 LONG_DESCRIPTION = 'nagogy fr'
 setup(
     name="nagie",
     version=VERSION,
     author="Dreamy",
     author_email="hotasfok@gmail.com",
```

