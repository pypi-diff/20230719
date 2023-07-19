# Comparing `tmp/kmemory-0.1.0.tar.gz` & `tmp/kmemory-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kmemory-0.1.0.tar", last modified: Fri Jul 14 18:01:21 2023, max compression
+gzip compressed data, was "kmemory-1.1.0.tar", last modified: Wed Jul 19 15:11:03 2023, max compression
```

## Comparing `kmemory-0.1.0.tar` & `kmemory-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-14 18:01:21.613690 kmemory-0.1.0/
--rw-r--r--   0 kali      (1000) kali      (1000)     1073 2023-07-14 17:58:32.000000 kmemory-0.1.0/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)      215 2023-07-14 18:01:21.613690 kmemory-0.1.0/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      224 2023-07-14 17:58:15.000000 kmemory-0.1.0/README.md
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-14 18:01:21.613690 kmemory-0.1.0/kmemory/
--rw-r--r--   0 kali      (1000) kali      (1000)        0 2023-07-14 17:45:39.000000 kmemory-0.1.0/kmemory/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)       52 2023-07-14 17:56:19.000000 kmemory-0.1.0/kmemory/kmemory.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-14 18:01:21.613690 kmemory-0.1.0/kmemory.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)      215 2023-07-14 18:01:21.000000 kmemory-0.1.0/kmemory.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      204 2023-07-14 18:01:21.000000 kmemory-0.1.0/kmemory.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-07-14 18:01:21.000000 kmemory-0.1.0/kmemory.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        8 2023-07-14 18:01:21.000000 kmemory-0.1.0/kmemory.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       86 2023-07-14 18:00:56.000000 kmemory-0.1.0/pyproject.toml
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-07-14 18:01:21.613690 kmemory-0.1.0/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)      270 2023-07-14 17:48:31.000000 kmemory-0.1.0/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-19 15:11:03.624978 kmemory-1.1.0/
+-rw-r--r--   0 kali      (1000) kali      (1000)     1073 2023-07-14 18:08:52.000000 kmemory-1.1.0/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)      215 2023-07-19 15:11:03.624978 kmemory-1.1.0/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      224 2023-07-14 18:08:52.000000 kmemory-1.1.0/README.md
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-19 15:11:03.624978 kmemory-1.1.0/kmemory/
+-rw-r--r--   0 kali      (1000) kali      (1000)      714 2023-07-19 15:10:54.000000 kmemory-1.1.0/kmemory/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)      507 2023-07-19 15:03:11.000000 kmemory-1.1.0/kmemory/kmemory.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-19 15:11:03.624978 kmemory-1.1.0/kmemory.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)      215 2023-07-19 15:11:03.000000 kmemory-1.1.0/kmemory.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      204 2023-07-19 15:11:03.000000 kmemory-1.1.0/kmemory.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-07-19 15:11:03.000000 kmemory-1.1.0/kmemory.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        8 2023-07-19 15:11:03.000000 kmemory-1.1.0/kmemory.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       86 2023-07-14 18:08:52.000000 kmemory-1.1.0/pyproject.toml
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-07-19 15:11:03.624978 kmemory-1.1.0/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)      271 2023-07-19 15:10:55.000000 kmemory-1.1.0/setup.py
```

### Comparing `kmemory-0.1.0/LICENSE` & `kmemory-1.1.0/LICENSE`

 * *Files identical despite different names*

