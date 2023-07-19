# Comparing `tmp/argil-0.0.4.tar.gz` & `tmp/argil-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argil-0.0.4.tar", last modified: Mon Jul 17 06:46:11 2023, max compression
+gzip compressed data, was "argil-0.0.5.tar", last modified: Wed Jul 19 05:28:09 2023, max compression
```

## Comparing `argil-0.0.4.tar` & `argil-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:46:11.401167 argil-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    34600 2023-07-17 06:45:59.000000 argil-0.0.4/LICENCE.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-17 06:45:59.000000 argil-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-17 06:46:11.401167 argil-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-17 06:45:59.000000 argil-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:46:11.401167 argil-0.0.4/argil/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-17 06:45:59.000000 argil-0.0.4/argil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-17 06:45:59.000000 argil-0.0.4/argil/config.json
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-17 06:45:59.000000 argil-0.0.4/argil/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-17 06:45:59.000000 argil-0.0.4/argil/workflowRuns.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-17 06:45:59.000000 argil-0.0.4/argil/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:46:11.401167 argil-0.0.4/argil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-17 06:46:11.000000 argil-0.0.4/argil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-17 06:46:11.000000 argil-0.0.4/argil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 06:46:11.000000 argil-0.0.4/argil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-17 06:46:11.000000 argil-0.0.4/argil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-17 06:46:11.000000 argil-0.0.4/argil.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 06:46:11.401167 argil-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-17 06:46:11.000000 argil-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:28:09.776034 argil-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    34600 2023-07-19 05:27:58.000000 argil-0.0.5/LICENCE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-07-19 05:28:09.772034 argil-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-19 05:27:58.000000 argil-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:28:09.772034 argil-0.0.5/argil/
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-19 05:27:58.000000 argil-0.0.5/argil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-07-19 05:27:58.000000 argil-0.0.5/argil/api_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-19 05:27:58.000000 argil-0.0.5/argil/argil_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-19 05:27:58.000000 argil-0.0.5/argil/argil_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:28:09.772034 argil-0.0.5/argil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-07-19 05:28:09.000000 argil-0.0.5/argil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-19 05:28:09.000000 argil-0.0.5/argil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 05:28:09.000000 argil-0.0.5/argil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-19 05:28:09.000000 argil-0.0.5/argil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-19 05:28:09.000000 argil-0.0.5/argil.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 05:28:09.776034 argil-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-19 05:28:09.000000 argil-0.0.5/setup.py
```

### Comparing `argil-0.0.4/LICENCE.md` & `argil-0.0.5/LICENCE.md`

 * *Files identical despite different names*

