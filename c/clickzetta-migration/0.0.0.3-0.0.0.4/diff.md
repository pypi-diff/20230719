# Comparing `tmp/clickzetta-migration-0.0.0.3.tar.gz` & `tmp/clickzetta-migration-0.0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickzetta-migration-0.0.0.3.tar", last modified: Tue Jul 18 07:37:10 2023, max compression
+gzip compressed data, was "clickzetta-migration-0.0.0.4.tar", last modified: Tue Jul 18 08:25:08 2023, max compression
```

## Comparing `clickzetta-migration-0.0.0.3.tar` & `clickzetta-migration-0.0.0.4.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 07:37:10.862268 clickzetta-migration-0.0.0.3/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       34 2023-07-18 07:23:21.000000 clickzetta-migration-0.0.0.3/MANIFEST.in
--rw-r--r--   0 lihanmiao   (501) staff       (20)      259 2023-07-18 07:37:10.862145 clickzetta-migration-0.0.0.3/PKG-INFO
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 07:37:10.854801 clickzetta-migration-0.0.0.3/clickzetta_migration.egg-info/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      259 2023-07-18 07:37:10.000000 clickzetta-migration-0.0.0.3/clickzetta_migration.egg-info/PKG-INFO
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2086 2023-07-18 07:37:10.000000 clickzetta-migration-0.0.0.3/clickzetta_migration.egg-info/SOURCES.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-07-18 07:37:10.000000 clickzetta-migration-0.0.0.3/clickzetta_migration.egg-info/dependency_links.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)       58 2023-07-18 07:37:10.000000 clickzetta-migration-0.0.0.3/clickzetta_migration.egg-info/entry_points.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-07-18 07:37:10.000000 clickzetta-migration-0.0.0.3/clickzetta_migration.egg-info/not-zip-safe
--rw-r--r--   0 lihanmiao   (501) staff       (20)      111 2023-07-18 07:37:10.000000 clickzetta-migration-0.0.0.3/clickzetta_migration.egg-info/requires.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)       10 2023-07-18 07:37:10.000000 clickzetta-migration-0.0.0.3/clickzetta_migration.egg-info/top_level.txt
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 07:37:10.855188 clickzetta-migration-0.0.0.3/migration/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 02:52:59.000000 clickzetta-migration-0.0.0.3/migration/__init__.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 07:37:10.855732 clickzetta-migration-0.0.0.3/migration/base/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       90 2023-07-11 03:06:38.000000 clickzetta-migration-0.0.0.3/migration/base/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      532 2023-07-13 08:55:34.000000 clickzetta-migration-0.0.0.3/migration/base/exceptions.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      444 2023-07-07 03:37:28.000000 clickzetta-migration-0.0.0.3/migration/base/status.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 07:37:10.855938 clickzetta-migration-0.0.0.3/migration/connector/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 02:53:59.000000 clickzetta-migration-0.0.0.3/migration/connector/__init__.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 07:37:10.856109 clickzetta-migration-0.0.0.3/migration/connector/destination/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 12:17:46.000000 clickzetta-migration-0.0.0.3/migration/connector/destination/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1249 2023-07-12 09:39:55.000000 clickzetta-migration-0.0.0.3/migration/connector/destination/base.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 07:37:10.856371 clickzetta-migration-0.0.0.3/migration/connector/destination/clickzetta/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-29 06:42:41.000000 clickzetta-migration-0.0.0.3/migration/connector/destination/clickzetta/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     6137 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.3/migration/connector/destination/clickzetta/destination.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 07:37:10.856660 clickzetta-migration-0.0.0.3/migration/connector/destination/doris/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-07-11 15:28:35.000000 clickzetta-migration-0.0.0.3/migration/connector/destination/doris/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     6243 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.3/migration/connector/destination/doris/destination.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 07:37:10.857276 clickzetta-migration-0.0.0.3/migration/connector/source/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       72 2023-07-11 03:06:38.000000 clickzetta-migration-0.0.0.3/migration/connector/source/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1879 2023-07-12 03:16:08.000000 clickzetta-migration-0.0.0.3/migration/connector/source/base.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 07:37:10.857559 clickzetta-migration-0.0.0.3/migration/connector/source/clickzetta/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-07-12 02:11:46.000000 clickzetta-migration-0.0.0.3/migration/connector/source/clickzetta/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     7338 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.3/migration/connector/source/clickzetta/source.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 07:37:10.857855 clickzetta-migration-0.0.0.3/migration/connector/source/doris/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:15:41.000000 clickzetta-migration-0.0.0.3/migration/connector/source/doris/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     6298 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.3/migration/connector/source/doris/source.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      352 2023-07-11 07:29:24.000000 clickzetta-migration-0.0.0.3/migration/connector/source/enum.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 07:37:10.858057 clickzetta-migration-0.0.0.3/migration/connector/source/hive/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:15:22.000000 clickzetta-migration-0.0.0.3/migration/connector/source/hive/__init__.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 07:37:10.858134 clickzetta-migration-0.0.0.3/migration/connector/source/odps/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:15:30.000000 clickzetta-migration-0.0.0.3/migration/connector/source/odps/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    11861 2023-07-17 08:44:25.000000 clickzetta-migration-0.0.0.3/migration/migration.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 07:37:10.858628 clickzetta-migration-0.0.0.3/migration/scheduler/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      112 2023-07-11 04:22:08.000000 clickzetta-migration-0.0.0.3/migration/scheduler/__init__.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 07:37:10.858915 clickzetta-migration-0.0.0.3/migration/scheduler/data_transformer/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:21:25.000000 clickzetta-migration-0.0.0.3/migration/scheduler/data_transformer/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3630 2023-07-12 11:45:19.000000 clickzetta-migration-0.0.0.3/migration/scheduler/data_transformer/transformer.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 07:37:10.859189 clickzetta-migration-0.0.0.3/migration/scheduler/data_validation/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:22:21.000000 clickzetta-migration-0.0.0.3/migration/scheduler/data_validation/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2845 2023-07-11 13:22:48.000000 clickzetta-migration-0.0.0.3/migration/scheduler/data_validation/validation.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4619 2023-07-17 07:57:48.000000 clickzetta-migration-0.0.0.3/migration/scheduler/scheduler.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 07:37:10.859472 clickzetta-migration-0.0.0.3/migration/scheduler/schema_transformer/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:21:14.000000 clickzetta-migration-0.0.0.3/migration/scheduler/schema_transformer/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4197 2023-07-12 09:39:55.000000 clickzetta-migration-0.0.0.3/migration/scheduler/schema_transformer/transformer.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 07:37:10.860559 clickzetta-migration-0.0.0.3/migration/scheduler/task/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      249 2023-07-11 03:06:38.000000 clickzetta-migration-0.0.0.3/migration/scheduler/task/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1395 2023-07-17 07:55:15.000000 clickzetta-migration-0.0.0.3/migration/scheduler/task/base_task.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1717 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.3/migration/scheduler/task/data_task.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1339 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.3/migration/scheduler/task/schema_task.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3356 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.3/migration/scheduler/task/validation_task.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2685 2023-07-13 10:20:49.000000 clickzetta-migration-0.0.0.3/migration/scheduler/transformer.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 07:37:10.860864 clickzetta-migration-0.0.0.3/migration/scheduler/unify_transformer/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-07-10 03:55:07.000000 clickzetta-migration-0.0.0.3/migration/scheduler/unify_transformer/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3881 2023-07-11 13:22:48.000000 clickzetta-migration-0.0.0.3/migration/scheduler/unify_transformer/transformer.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 07:37:10.861147 clickzetta-migration-0.0.0.3/migration/test/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-28 07:15:40.000000 clickzetta-migration-0.0.0.3/migration/test/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2348 2023-07-13 12:19:13.000000 clickzetta-migration-0.0.0.3/migration/test/util_test.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 07:37:10.861902 clickzetta-migration-0.0.0.3/migration/util/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 02:54:06.000000 clickzetta-migration-0.0.0.3/migration/util/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     7638 2023-07-17 09:06:42.000000 clickzetta-migration-0.0.0.3/migration/util/migration_tasks_status.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1180 2023-07-12 10:01:25.000000 clickzetta-migration-0.0.0.3/migration/util/object_storage_util.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1534 2023-07-18 07:36:47.000000 clickzetta-migration-0.0.0.3/migration/util/script_util.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)       23 2023-07-18 07:36:47.000000 clickzetta-migration-0.0.0.3/migration/version.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-07-18 07:37:10.862307 clickzetta-migration-0.0.0.3/setup.cfg
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1455 2023-07-18 07:36:47.000000 clickzetta-migration-0.0.0.3/setup.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 08:25:08.023453 clickzetta-migration-0.0.0.4/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       34 2023-07-18 07:23:21.000000 clickzetta-migration-0.0.0.4/MANIFEST.in
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      259 2023-07-18 08:25:08.023327 clickzetta-migration-0.0.0.4/PKG-INFO
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 08:25:08.014314 clickzetta-migration-0.0.0.4/clickzetta_migration.egg-info/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      259 2023-07-18 08:25:07.000000 clickzetta-migration-0.0.0.4/clickzetta_migration.egg-info/PKG-INFO
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2086 2023-07-18 08:25:08.000000 clickzetta-migration-0.0.0.4/clickzetta_migration.egg-info/SOURCES.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-07-18 08:25:07.000000 clickzetta-migration-0.0.0.4/clickzetta_migration.egg-info/dependency_links.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       58 2023-07-18 08:25:07.000000 clickzetta-migration-0.0.0.4/clickzetta_migration.egg-info/entry_points.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-07-18 08:25:07.000000 clickzetta-migration-0.0.0.4/clickzetta_migration.egg-info/not-zip-safe
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      111 2023-07-18 08:25:07.000000 clickzetta-migration-0.0.0.4/clickzetta_migration.egg-info/requires.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       10 2023-07-18 08:25:07.000000 clickzetta-migration-0.0.0.4/clickzetta_migration.egg-info/top_level.txt
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 08:25:08.014810 clickzetta-migration-0.0.0.4/migration/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 02:52:59.000000 clickzetta-migration-0.0.0.4/migration/__init__.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 08:25:08.015421 clickzetta-migration-0.0.0.4/migration/base/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       90 2023-07-11 03:06:38.000000 clickzetta-migration-0.0.0.4/migration/base/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      532 2023-07-13 08:55:34.000000 clickzetta-migration-0.0.0.4/migration/base/exceptions.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      444 2023-07-07 03:37:28.000000 clickzetta-migration-0.0.0.4/migration/base/status.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 08:25:08.015850 clickzetta-migration-0.0.0.4/migration/connector/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 02:53:59.000000 clickzetta-migration-0.0.0.4/migration/connector/__init__.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 08:25:08.016042 clickzetta-migration-0.0.0.4/migration/connector/destination/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 12:17:46.000000 clickzetta-migration-0.0.0.4/migration/connector/destination/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1249 2023-07-12 09:39:55.000000 clickzetta-migration-0.0.0.4/migration/connector/destination/base.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 08:25:08.016380 clickzetta-migration-0.0.0.4/migration/connector/destination/clickzetta/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-29 06:42:41.000000 clickzetta-migration-0.0.0.4/migration/connector/destination/clickzetta/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     6137 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.4/migration/connector/destination/clickzetta/destination.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 08:25:08.016696 clickzetta-migration-0.0.0.4/migration/connector/destination/doris/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-07-11 15:28:35.000000 clickzetta-migration-0.0.0.4/migration/connector/destination/doris/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     6243 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.4/migration/connector/destination/doris/destination.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 08:25:08.017416 clickzetta-migration-0.0.0.4/migration/connector/source/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       72 2023-07-11 03:06:38.000000 clickzetta-migration-0.0.0.4/migration/connector/source/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1879 2023-07-12 03:16:08.000000 clickzetta-migration-0.0.0.4/migration/connector/source/base.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 08:25:08.018093 clickzetta-migration-0.0.0.4/migration/connector/source/clickzetta/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-07-12 02:11:46.000000 clickzetta-migration-0.0.0.4/migration/connector/source/clickzetta/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     7338 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.4/migration/connector/source/clickzetta/source.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 08:25:08.018375 clickzetta-migration-0.0.0.4/migration/connector/source/doris/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:15:41.000000 clickzetta-migration-0.0.0.4/migration/connector/source/doris/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     6298 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.4/migration/connector/source/doris/source.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      352 2023-07-11 07:29:24.000000 clickzetta-migration-0.0.0.4/migration/connector/source/enum.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 08:25:08.018643 clickzetta-migration-0.0.0.4/migration/connector/source/hive/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:15:22.000000 clickzetta-migration-0.0.0.4/migration/connector/source/hive/__init__.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 08:25:08.018716 clickzetta-migration-0.0.0.4/migration/connector/source/odps/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:15:30.000000 clickzetta-migration-0.0.0.4/migration/connector/source/odps/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    11861 2023-07-17 08:44:25.000000 clickzetta-migration-0.0.0.4/migration/migration.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 08:25:08.019343 clickzetta-migration-0.0.0.4/migration/scheduler/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      112 2023-07-11 04:22:08.000000 clickzetta-migration-0.0.0.4/migration/scheduler/__init__.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 08:25:08.019733 clickzetta-migration-0.0.0.4/migration/scheduler/data_transformer/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:21:25.000000 clickzetta-migration-0.0.0.4/migration/scheduler/data_transformer/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3630 2023-07-12 11:45:19.000000 clickzetta-migration-0.0.0.4/migration/scheduler/data_transformer/transformer.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 08:25:08.019999 clickzetta-migration-0.0.0.4/migration/scheduler/data_validation/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:22:21.000000 clickzetta-migration-0.0.0.4/migration/scheduler/data_validation/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2845 2023-07-11 13:22:48.000000 clickzetta-migration-0.0.0.4/migration/scheduler/data_validation/validation.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4619 2023-07-17 07:57:48.000000 clickzetta-migration-0.0.0.4/migration/scheduler/scheduler.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 08:25:08.020283 clickzetta-migration-0.0.0.4/migration/scheduler/schema_transformer/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:21:14.000000 clickzetta-migration-0.0.0.4/migration/scheduler/schema_transformer/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4197 2023-07-12 09:39:55.000000 clickzetta-migration-0.0.0.4/migration/scheduler/schema_transformer/transformer.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 08:25:08.021500 clickzetta-migration-0.0.0.4/migration/scheduler/task/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      249 2023-07-11 03:06:38.000000 clickzetta-migration-0.0.0.4/migration/scheduler/task/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1395 2023-07-17 07:55:15.000000 clickzetta-migration-0.0.0.4/migration/scheduler/task/base_task.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1717 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.4/migration/scheduler/task/data_task.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1339 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.4/migration/scheduler/task/schema_task.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3356 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.4/migration/scheduler/task/validation_task.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2685 2023-07-13 10:20:49.000000 clickzetta-migration-0.0.0.4/migration/scheduler/transformer.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 08:25:08.021902 clickzetta-migration-0.0.0.4/migration/scheduler/unify_transformer/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-07-10 03:55:07.000000 clickzetta-migration-0.0.0.4/migration/scheduler/unify_transformer/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3881 2023-07-11 13:22:48.000000 clickzetta-migration-0.0.0.4/migration/scheduler/unify_transformer/transformer.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 08:25:08.022183 clickzetta-migration-0.0.0.4/migration/test/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-28 07:15:40.000000 clickzetta-migration-0.0.0.4/migration/test/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2348 2023-07-13 12:19:13.000000 clickzetta-migration-0.0.0.4/migration/test/util_test.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 08:25:08.022969 clickzetta-migration-0.0.0.4/migration/util/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 02:54:06.000000 clickzetta-migration-0.0.0.4/migration/util/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     7638 2023-07-17 09:06:42.000000 clickzetta-migration-0.0.0.4/migration/util/migration_tasks_status.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1180 2023-07-12 10:01:25.000000 clickzetta-migration-0.0.0.4/migration/util/object_storage_util.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1534 2023-07-18 07:36:47.000000 clickzetta-migration-0.0.0.4/migration/util/script_util.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       23 2023-07-18 08:25:03.000000 clickzetta-migration-0.0.0.4/migration/version.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-07-18 08:25:08.023493 clickzetta-migration-0.0.0.4/setup.cfg
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1455 2023-07-18 08:25:03.000000 clickzetta-migration-0.0.0.4/setup.py
```

### Comparing `clickzetta-migration-0.0.0.3/clickzetta_migration.egg-info/SOURCES.txt` & `clickzetta-migration-0.0.0.4/clickzetta_migration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.3/migration/base/exceptions.py` & `clickzetta-migration-0.0.0.4/migration/base/exceptions.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.3/migration/connector/destination/base.py` & `clickzetta-migration-0.0.0.4/migration/connector/destination/base.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.3/migration/connector/destination/clickzetta/destination.py` & `clickzetta-migration-0.0.0.4/migration/connector/destination/clickzetta/destination.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.3/migration/connector/destination/doris/destination.py` & `clickzetta-migration-0.0.0.4/migration/connector/destination/doris/destination.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.3/migration/connector/source/base.py` & `clickzetta-migration-0.0.0.4/migration/connector/source/base.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.3/migration/connector/source/clickzetta/source.py` & `clickzetta-migration-0.0.0.4/migration/connector/source/clickzetta/source.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.3/migration/connector/source/doris/source.py` & `clickzetta-migration-0.0.0.4/migration/connector/source/doris/source.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.3/migration/migration.py` & `clickzetta-migration-0.0.0.4/migration/migration.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.3/migration/scheduler/data_transformer/transformer.py` & `clickzetta-migration-0.0.0.4/migration/scheduler/data_transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.3/migration/scheduler/data_validation/validation.py` & `clickzetta-migration-0.0.0.4/migration/scheduler/data_validation/validation.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.3/migration/scheduler/scheduler.py` & `clickzetta-migration-0.0.0.4/migration/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.3/migration/scheduler/schema_transformer/transformer.py` & `clickzetta-migration-0.0.0.4/migration/scheduler/schema_transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.3/migration/scheduler/task/base_task.py` & `clickzetta-migration-0.0.0.4/migration/scheduler/task/base_task.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.3/migration/scheduler/task/data_task.py` & `clickzetta-migration-0.0.0.4/migration/scheduler/task/data_task.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.3/migration/scheduler/task/schema_task.py` & `clickzetta-migration-0.0.0.4/migration/scheduler/task/schema_task.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.3/migration/scheduler/task/validation_task.py` & `clickzetta-migration-0.0.0.4/migration/scheduler/task/validation_task.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.3/migration/scheduler/transformer.py` & `clickzetta-migration-0.0.0.4/migration/scheduler/transformer.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.3/migration/scheduler/unify_transformer/transformer.py` & `clickzetta-migration-0.0.0.4/migration/scheduler/unify_transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.3/migration/test/util_test.py` & `clickzetta-migration-0.0.0.4/migration/test/util_test.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.3/migration/util/migration_tasks_status.py` & `clickzetta-migration-0.0.0.4/migration/util/migration_tasks_status.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.3/migration/util/object_storage_util.py` & `clickzetta-migration-0.0.0.4/migration/util/object_storage_util.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.3/migration/util/script_util.py` & `clickzetta-migration-0.0.0.4/migration/util/script_util.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.3/setup.py` & `clickzetta-migration-0.0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,14 @@
     url='https://www.yunqi.tech/',
     author="mocun",
     author_email="hanmiao.li@clickzetta.com",
     platforms="Posix; MacOS X;",
     packages=packages,
     install_requires=dependencies,
     extras_require=extras,
-    python_requires=">=3.7",
+    python_requires=">=3.6",
     entry_points={
         'console_scripts': ['cz-migration=migration.migration:main'],
     },
     include_package_data=True,
     zip_safe=False,
 )
```

