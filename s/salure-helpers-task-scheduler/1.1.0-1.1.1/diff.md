# Comparing `tmp/salure_helpers_task_scheduler-1.1.0.tar.gz` & `tmp/salure_helpers_task_scheduler-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/salure_helpers_task_scheduler-1.1.0.tar", last modified: Tue Jul 18 07:47:51 2023, max compression
+gzip compressed data, was "dist/salure_helpers_task_scheduler-1.1.1.tar", last modified: Wed Jul 19 12:31:24 2023, max compression
```

## Comparing `salure_helpers_task_scheduler-1.1.0.tar` & `salure_helpers_task_scheduler-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 07:47:51.000000 salure_helpers_task_scheduler-1.1.0/
--rw-r--r--   0 root         (0) root         (0)      269 2023-07-18 07:47:51.000000 salure_helpers_task_scheduler-1.1.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 07:47:51.000000 salure_helpers_task_scheduler-1.1.0/salure_helpers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 07:47:51.000000 salure_helpers_task_scheduler-1.1.0/salure_helpers/task_scheduler/
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-07-18 07:47:38.000000 salure_helpers_task_scheduler-1.1.0/salure_helpers/task_scheduler/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    39810 2023-07-18 07:47:38.000000 salure_helpers_task_scheduler-1.1.0/salure_helpers/task_scheduler/task_scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 07:47:51.000000 salure_helpers_task_scheduler-1.1.0/salure_helpers_task_scheduler.egg-info/
--rw-r--r--   0 root         (0) root         (0)      269 2023-07-18 07:47:51.000000 salure_helpers_task_scheduler-1.1.0/salure_helpers_task_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      414 2023-07-18 07:47:51.000000 salure_helpers_task_scheduler-1.1.0/salure_helpers_task_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 07:47:51.000000 salure_helpers_task_scheduler-1.1.0/salure_helpers_task_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 07:47:51.000000 salure_helpers_task_scheduler-1.1.0/salure_helpers_task_scheduler.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      151 2023-07-18 07:47:51.000000 salure_helpers_task_scheduler-1.1.0/salure_helpers_task_scheduler.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-18 07:47:51.000000 salure_helpers_task_scheduler-1.1.0/salure_helpers_task_scheduler.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 07:47:51.000000 salure_helpers_task_scheduler-1.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      614 2023-07-18 07:47:38.000000 salure_helpers_task_scheduler-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 12:31:24.000000 salure_helpers_task_scheduler-1.1.1/
+-rw-r--r--   0 root         (0) root         (0)      269 2023-07-19 12:31:24.000000 salure_helpers_task_scheduler-1.1.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 12:31:24.000000 salure_helpers_task_scheduler-1.1.1/salure_helpers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 12:31:24.000000 salure_helpers_task_scheduler-1.1.1/salure_helpers/task_scheduler/
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-07-19 12:31:07.000000 salure_helpers_task_scheduler-1.1.1/salure_helpers/task_scheduler/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    39810 2023-07-19 12:31:07.000000 salure_helpers_task_scheduler-1.1.1/salure_helpers/task_scheduler/task_scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 12:31:24.000000 salure_helpers_task_scheduler-1.1.1/salure_helpers_task_scheduler.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      269 2023-07-19 12:31:24.000000 salure_helpers_task_scheduler-1.1.1/salure_helpers_task_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      414 2023-07-19 12:31:24.000000 salure_helpers_task_scheduler-1.1.1/salure_helpers_task_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 12:31:24.000000 salure_helpers_task_scheduler-1.1.1/salure_helpers_task_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 12:31:24.000000 salure_helpers_task_scheduler-1.1.1/salure_helpers_task_scheduler.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      177 2023-07-19 12:31:24.000000 salure_helpers_task_scheduler-1.1.1/salure_helpers_task_scheduler.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-19 12:31:24.000000 salure_helpers_task_scheduler-1.1.1/salure_helpers_task_scheduler.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-19 12:31:24.000000 salure_helpers_task_scheduler-1.1.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      651 2023-07-19 12:31:07.000000 salure_helpers_task_scheduler-1.1.1/setup.py
```

### Comparing `salure_helpers_task_scheduler-1.1.0/salure_helpers/task_scheduler/task_scheduler.py` & `salure_helpers_task_scheduler-1.1.1/salure_helpers/task_scheduler/task_scheduler.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_task_scheduler-1.1.0/setup.py` & `salure_helpers_task_scheduler-1.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from setuptools import setup
 
 
 setup(
     name='salure_helpers_task_scheduler',
-    version='1.1.0',
+    version='1.1.1',
     description='Task Scheduler from Salure',
     long_description='Task Schedule from Salure',
     author='D&A Salure',
     author_email='support@salureconnnect.com',
     packages=["salure_helpers.task_scheduler"],
     license='Salure License',
     install_requires=[
         'salure-helpers-mysql>=1',
         'salure-helpers-salureconnect>=1',
         'salure-helpers-mandrill>=0',
         'salure-helpers-salure_functions>=0',
+        'salure-helpers-elastic>=0',
         'pandas>=1,<=1.35',
         'requests>=2,<=3'
     ],
     zip_safe=False,
 )
```

