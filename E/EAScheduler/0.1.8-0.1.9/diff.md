# Comparing `tmp/EAScheduler-0.1.8.tar.gz` & `tmp/EAScheduler-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EAScheduler-0.1.8.tar", last modified: Wed Dec 14 09:35:48 2022, max compression
+gzip compressed data, was "EAScheduler-0.1.9.tar", last modified: Wed Jul 19 09:51:07 2023, max compression
```

## Comparing `EAScheduler-0.1.8.tar` & `EAScheduler-0.1.9.tar`

### file list

```diff
@@ -1,41 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 09:35:48.352433 EAScheduler-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2022-12-14 09:35:38.000000 EAScheduler-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       80 2022-12-14 09:35:38.000000 EAScheduler-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2022-12-14 09:35:48.352433 EAScheduler-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       81 2022-12-14 09:35:38.000000 EAScheduler-0.1.8/requirements_setup.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-14 09:35:48.352433 EAScheduler-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2022-12-14 09:35:38.000000 EAScheduler-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 09:35:48.344433 EAScheduler-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 09:35:48.348433 EAScheduler-0.1.8/src/EAScheduler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2022-12-14 09:35:48.000000 EAScheduler-0.1.8/src/EAScheduler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2022-12-14 09:35:48.000000 EAScheduler-0.1.8/src/EAScheduler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-14 09:35:48.000000 EAScheduler-0.1.8/src/EAScheduler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2022-12-14 09:35:48.000000 EAScheduler-0.1.8/src/EAScheduler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2022-12-14 09:35:48.000000 EAScheduler-0.1.8/src/EAScheduler.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 09:35:48.348433 EAScheduler-0.1.8/src/eascheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2022-12-14 09:35:38.000000 EAScheduler-0.1.8/src/eascheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2022-12-14 09:35:38.000000 EAScheduler-0.1.8/src/eascheduler/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2022-12-14 09:35:38.000000 EAScheduler-0.1.8/src/eascheduler/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2022-12-14 09:35:38.000000 EAScheduler-0.1.8/src/eascheduler/default.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 09:35:48.348433 EAScheduler-0.1.8/src/eascheduler/errors/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2022-12-14 09:35:38.000000 EAScheduler-0.1.8/src/eascheduler/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2022-12-14 09:35:38.000000 EAScheduler-0.1.8/src/eascheduler/errors/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2022-12-14 09:35:38.000000 EAScheduler-0.1.8/src/eascheduler/errors/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 09:35:48.348433 EAScheduler-0.1.8/src/eascheduler/executors/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2022-12-14 09:35:38.000000 EAScheduler-0.1.8/src/eascheduler/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2022-12-14 09:35:38.000000 EAScheduler-0.1.8/src/eascheduler/executors/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 09:35:48.348433 EAScheduler-0.1.8/src/eascheduler/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2022-12-14 09:35:38.000000 EAScheduler-0.1.8/src/eascheduler/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4028 2022-12-14 09:35:38.000000 EAScheduler-0.1.8/src/eascheduler/jobs/job_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7770 2022-12-14 09:35:38.000000 EAScheduler-0.1.8/src/eascheduler/jobs/job_base_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2022-12-14 09:35:38.000000 EAScheduler-0.1.8/src/eascheduler/jobs/job_countdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2022-12-14 09:35:38.000000 EAScheduler-0.1.8/src/eascheduler/jobs/job_day_of_week.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2022-12-14 09:35:38.000000 EAScheduler-0.1.8/src/eascheduler/jobs/job_one_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2022-12-14 09:35:38.000000 EAScheduler-0.1.8/src/eascheduler/jobs/job_reoccuring.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2022-12-14 09:35:38.000000 EAScheduler-0.1.8/src/eascheduler/jobs/job_sun.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 09:35:38.000000 EAScheduler-0.1.8/src/eascheduler/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6354 2022-12-14 09:35:38.000000 EAScheduler-0.1.8/src/eascheduler/scheduler_view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 09:35:48.352433 EAScheduler-0.1.8/src/eascheduler/schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2022-12-14 09:35:38.000000 EAScheduler-0.1.8/src/eascheduler/schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2022-12-14 09:35:38.000000 EAScheduler-0.1.8/src/eascheduler/schedulers/scheduler_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2022-12-14 09:35:38.000000 EAScheduler-0.1.8/src/eascheduler/schedulers/scheduler_asyncthread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:51:07.205216 EAScheduler-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-19 09:50:54.000000 EAScheduler-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-19 09:50:54.000000 EAScheduler-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-19 09:51:07.201216 EAScheduler-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-19 09:50:54.000000 EAScheduler-0.1.9/requirements_setup.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 09:51:07.205216 EAScheduler-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-19 09:50:54.000000 EAScheduler-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:51:07.197216 EAScheduler-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:51:07.197216 EAScheduler-0.1.9/src/EAScheduler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-19 09:51:07.000000 EAScheduler-0.1.9/src/EAScheduler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-19 09:51:07.000000 EAScheduler-0.1.9/src/EAScheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 09:51:07.000000 EAScheduler-0.1.9/src/EAScheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-19 09:51:07.000000 EAScheduler-0.1.9/src/EAScheduler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-19 09:51:07.000000 EAScheduler-0.1.9/src/EAScheduler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:51:07.201216 EAScheduler-0.1.9/src/eascheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-19 09:50:54.000000 EAScheduler-0.1.9/src/eascheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-19 09:50:54.000000 EAScheduler-0.1.9/src/eascheduler/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-19 09:50:54.000000 EAScheduler-0.1.9/src/eascheduler/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-19 09:50:54.000000 EAScheduler-0.1.9/src/eascheduler/default.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:51:07.201216 EAScheduler-0.1.9/src/eascheduler/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-19 09:50:54.000000 EAScheduler-0.1.9/src/eascheduler/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-19 09:50:54.000000 EAScheduler-0.1.9/src/eascheduler/errors/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-19 09:50:54.000000 EAScheduler-0.1.9/src/eascheduler/errors/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:51:07.201216 EAScheduler-0.1.9/src/eascheduler/executors/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-19 09:50:54.000000 EAScheduler-0.1.9/src/eascheduler/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-19 09:50:54.000000 EAScheduler-0.1.9/src/eascheduler/executors/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:51:07.201216 EAScheduler-0.1.9/src/eascheduler/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-19 09:50:54.000000 EAScheduler-0.1.9/src/eascheduler/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-07-19 09:50:54.000000 EAScheduler-0.1.9/src/eascheduler/jobs/job_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-07-19 09:50:54.000000 EAScheduler-0.1.9/src/eascheduler/jobs/job_base_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-07-19 09:50:54.000000 EAScheduler-0.1.9/src/eascheduler/jobs/job_countdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-07-19 09:50:54.000000 EAScheduler-0.1.9/src/eascheduler/jobs/job_day_of_week.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-19 09:50:54.000000 EAScheduler-0.1.9/src/eascheduler/jobs/job_one_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-19 09:50:54.000000 EAScheduler-0.1.9/src/eascheduler/jobs/job_reoccuring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-19 09:50:54.000000 EAScheduler-0.1.9/src/eascheduler/jobs/job_sun.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 09:50:54.000000 EAScheduler-0.1.9/src/eascheduler/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-07-19 09:50:54.000000 EAScheduler-0.1.9/src/eascheduler/scheduler_view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:51:07.201216 EAScheduler-0.1.9/src/eascheduler/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-19 09:50:54.000000 EAScheduler-0.1.9/src/eascheduler/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-07-19 09:50:54.000000 EAScheduler-0.1.9/src/eascheduler/schedulers/scheduler_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-19 09:50:54.000000 EAScheduler-0.1.9/src/eascheduler/schedulers/scheduler_asyncthread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:51:07.201216 EAScheduler-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-07-19 09:50:54.000000 EAScheduler-0.1.9/tests/test_time_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-07-19 09:50:54.000000 EAScheduler-0.1.9/tests/test_view.py
```

### Comparing `EAScheduler-0.1.8/LICENSE` & `EAScheduler-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `EAScheduler-0.1.8/PKG-INFO` & `EAScheduler-0.1.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EAScheduler
-Version: 0.1.8
+Version: 0.1.9
 Summary: Easy async scheduling with a nice interface
 Home-page: https://github.com/spacemanspiff2007/eascheduler
 Author: spaceman_spiff
 Project-URL: Documentation, https://eascheduler.readthedocs.io/
 Project-URL: GitHub, https://github.com/spacemanspiff2007/eascheduler
 Keywords: scheduler,asyncio
 Classifier: Development Status :: 4 - Beta
@@ -37,50 +37,54 @@
 Easy Async Scheduler (or EAScheduler) is a lightweight asyncio scheduler with a nice and easy to use interface.
 
 ## Documentation
 [The documentation can be found at here](https://eascheduler.readthedocs.io)
 
 ## Changelog
 
-#### 0.18 (14.12.2022)
-- Fix for OneTimeJOb incorrectly showing a remaining time after the execution
+#### 0.1.9 (2023-07-19)
+- Fix for days when the sun doesn't rise or set.
+  In that case the next date with a sunrise/sunset will be returned.
+ 
+#### 0.1.8 (2022-12-14)
+- Fix for OneTimeJob incorrectly showing a remaining time after the execution
 - Dependency update
 
-#### 0.1.7 (27.07.2022)
+#### 0.1.7 (2022-07-27)
 - Added py.typed
 
-#### 0.1.6 (27.07.2022)
+#### 0.1.6 (2022-07-27)
 - Removed Python 3.7 support
 - Fixed setup issues
 
-#### 0.1.5 (14.02.2022)
+#### 0.1.5 (2022-02-14)
 - Jobs have a remaining function
 - CountdownJob has a stop function
 
-#### 0.1.4 (01.06.2021)
+#### 0.1.4 (2021-06-01)
 - Added option to pause and resume the scheduler
 - Jobs don't have to be in the future any more
 - Sorted imports with isort
 
-#### 0.1.3 (06.05.2021)
+#### 0.1.3 (2021-05-06)
 - Fixed a bug where a negative offset/jitter could result in multiple executions
 
-#### 0.1.2 (06.05.2021)
+#### 0.1.2 (2021-05-06)
 - Fixed a bug where ``.every(None, ...)`` would result in an error
 
-#### 0.1.1 (02.05.2021)
+#### 0.1.1 (2021-05-02)
 - Implemented a much nicer API and fixed some bugs
 
-#### 0.1.0 (21.04.2021)
+#### 0.1.0 (2021-04-21)
 - Fixed a race condition
 - Added tests
 
-#### 0.0.9 (19.04.2021)
+#### 0.0.9 (2021-04-19)
 - Fixes for wrong timezone
 - Added tests
 
-#### 0.0.8 (17.04.2021)
+#### 0.0.8 (2021-04-17)
 - Fixes for SunJob, ReoccurringJob
 - Added tests
 
-#### 0.0.7 (15.04.2021)
+#### 0.0.7 (2021-04-15)
 - Fixes for Sunrise/Sunset
```

### Comparing `EAScheduler-0.1.8/setup.py` & `EAScheduler-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `EAScheduler-0.1.8/src/EAScheduler.egg-info/PKG-INFO` & `EAScheduler-0.1.9/src/EAScheduler.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EAScheduler
-Version: 0.1.8
+Version: 0.1.9
 Summary: Easy async scheduling with a nice interface
 Home-page: https://github.com/spacemanspiff2007/eascheduler
 Author: spaceman_spiff
 Project-URL: Documentation, https://eascheduler.readthedocs.io/
 Project-URL: GitHub, https://github.com/spacemanspiff2007/eascheduler
 Keywords: scheduler,asyncio
 Classifier: Development Status :: 4 - Beta
@@ -37,50 +37,54 @@
 Easy Async Scheduler (or EAScheduler) is a lightweight asyncio scheduler with a nice and easy to use interface.
 
 ## Documentation
 [The documentation can be found at here](https://eascheduler.readthedocs.io)
 
 ## Changelog
 
-#### 0.18 (14.12.2022)
-- Fix for OneTimeJOb incorrectly showing a remaining time after the execution
+#### 0.1.9 (2023-07-19)
+- Fix for days when the sun doesn't rise or set.
+  In that case the next date with a sunrise/sunset will be returned.
+ 
+#### 0.1.8 (2022-12-14)
+- Fix for OneTimeJob incorrectly showing a remaining time after the execution
 - Dependency update
 
-#### 0.1.7 (27.07.2022)
+#### 0.1.7 (2022-07-27)
 - Added py.typed
 
-#### 0.1.6 (27.07.2022)
+#### 0.1.6 (2022-07-27)
 - Removed Python 3.7 support
 - Fixed setup issues
 
-#### 0.1.5 (14.02.2022)
+#### 0.1.5 (2022-02-14)
 - Jobs have a remaining function
 - CountdownJob has a stop function
 
-#### 0.1.4 (01.06.2021)
+#### 0.1.4 (2021-06-01)
 - Added option to pause and resume the scheduler
 - Jobs don't have to be in the future any more
 - Sorted imports with isort
 
-#### 0.1.3 (06.05.2021)
+#### 0.1.3 (2021-05-06)
 - Fixed a bug where a negative offset/jitter could result in multiple executions
 
-#### 0.1.2 (06.05.2021)
+#### 0.1.2 (2021-05-06)
 - Fixed a bug where ``.every(None, ...)`` would result in an error
 
-#### 0.1.1 (02.05.2021)
+#### 0.1.1 (2021-05-02)
 - Implemented a much nicer API and fixed some bugs
 
-#### 0.1.0 (21.04.2021)
+#### 0.1.0 (2021-04-21)
 - Fixed a race condition
 - Added tests
 
-#### 0.0.9 (19.04.2021)
+#### 0.0.9 (2021-04-19)
 - Fixes for wrong timezone
 - Added tests
 
-#### 0.0.8 (17.04.2021)
+#### 0.0.8 (2021-04-17)
 - Fixes for SunJob, ReoccurringJob
 - Added tests
 
-#### 0.0.7 (15.04.2021)
+#### 0.0.7 (2021-04-15)
 - Fixes for Sunrise/Sunset
```

### Comparing `EAScheduler-0.1.8/src/EAScheduler.egg-info/SOURCES.txt` & `EAScheduler-0.1.9/src/EAScheduler.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -24,8 +24,10 @@
 src/eascheduler/jobs/job_countdown.py
 src/eascheduler/jobs/job_day_of_week.py
 src/eascheduler/jobs/job_one_time.py
 src/eascheduler/jobs/job_reoccuring.py
 src/eascheduler/jobs/job_sun.py
 src/eascheduler/schedulers/__init__.py
 src/eascheduler/schedulers/scheduler_async.py
-src/eascheduler/schedulers/scheduler_asyncthread.py
+src/eascheduler/schedulers/scheduler_asyncthread.py
+tests/test_time_conversions.py
+tests/test_view.py
```

### Comparing `EAScheduler-0.1.8/src/eascheduler/executors/executor.py` & `EAScheduler-0.1.9/src/eascheduler/executors/executor.py`

 * *Files identical despite different names*

### Comparing `EAScheduler-0.1.8/src/eascheduler/jobs/job_base.py` & `EAScheduler-0.1.9/src/eascheduler/jobs/job_base.py`

 * *Files identical despite different names*

### Comparing `EAScheduler-0.1.8/src/eascheduler/jobs/job_base_datetime.py` & `EAScheduler-0.1.9/src/eascheduler/jobs/job_base_datetime.py`

 * *Files identical despite different names*

### Comparing `EAScheduler-0.1.8/src/eascheduler/jobs/job_countdown.py` & `EAScheduler-0.1.9/src/eascheduler/jobs/job_countdown.py`

 * *Files identical despite different names*

### Comparing `EAScheduler-0.1.8/src/eascheduler/jobs/job_day_of_week.py` & `EAScheduler-0.1.9/src/eascheduler/jobs/job_day_of_week.py`

 * *Files identical despite different names*

### Comparing `EAScheduler-0.1.8/src/eascheduler/jobs/job_one_time.py` & `EAScheduler-0.1.9/src/eascheduler/jobs/job_one_time.py`

 * *Files identical despite different names*

### Comparing `EAScheduler-0.1.8/src/eascheduler/jobs/job_reoccuring.py` & `EAScheduler-0.1.9/src/eascheduler/jobs/job_reoccuring.py`

 * *Files identical despite different names*

### Comparing `EAScheduler-0.1.8/src/eascheduler/jobs/job_sun.py` & `EAScheduler-0.1.9/src/eascheduler/jobs/job_sun.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,16 +49,25 @@
 
     def _advance_time(self, utc_dt: DateTime) -> DateTime:
         return pd_instance(self._sun_func(OBSERVER, utc_dt.add(days=1).date(), tzinfo=UTC)).set(microsecond=0)
 
     def _schedule_next_run(self):
         dt_next = get_now(UTC)
         last_run = from_timestamp(self._last_run_base)
-        next_run = pd_instance(self._sun_func(OBSERVER, dt_next.date(), tzinfo=UTC)).set(microsecond=0)
+        next_run = None
 
+        # If we are very far north or very far south it's possible that we don't have a sunrise at all
+        # If that's the case we advance and schedule for the next date that actually has a sunrise
+        while next_run is None:
+            try:
+                next_run = self._sun_func(OBSERVER, dt_next.date(), tzinfo=UTC)
+            except ValueError:
+                dt_next += timedelta(days=1)
+
+        next_run = pd_instance(next_run).set(microsecond=0)
         while next_run <= get_now(UTC) or next_run <= last_run:
             next_run = self._advance_time(next_run)
 
         self._next_run_base = next_run.timestamp()
         self._apply_boundaries()
```

### Comparing `EAScheduler-0.1.8/src/eascheduler/scheduler_view.py` & `EAScheduler-0.1.9/src/eascheduler/scheduler_view.py`

 * *Files identical despite different names*

### Comparing `EAScheduler-0.1.8/src/eascheduler/schedulers/scheduler_async.py` & `EAScheduler-0.1.9/src/eascheduler/schedulers/scheduler_async.py`

 * *Files identical despite different names*

### Comparing `EAScheduler-0.1.8/src/eascheduler/schedulers/scheduler_asyncthread.py` & `EAScheduler-0.1.9/src/eascheduler/schedulers/scheduler_asyncthread.py`

 * *Files identical despite different names*

