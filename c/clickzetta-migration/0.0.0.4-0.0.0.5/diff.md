# Comparing `tmp/clickzetta-migration-0.0.0.4.tar.gz` & `tmp/clickzetta-migration-0.0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickzetta-migration-0.0.0.4.tar", last modified: Tue Jul 18 08:25:08 2023, max compression
+gzip compressed data, was "clickzetta-migration-0.0.0.5.tar", last modified: Wed Jul 19 08:16:51 2023, max compression
```

## Comparing `clickzetta-migration-0.0.0.4.tar` & `clickzetta-migration-0.0.0.5.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 08:25:08.023453 clickzetta-migration-0.0.0.4/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       34 2023-07-18 07:23:21.000000 clickzetta-migration-0.0.0.4/MANIFEST.in
--rw-r--r--   0 lihanmiao   (501) staff       (20)      259 2023-07-18 08:25:08.023327 clickzetta-migration-0.0.0.4/PKG-INFO
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 08:25:08.014314 clickzetta-migration-0.0.0.4/clickzetta_migration.egg-info/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      259 2023-07-18 08:25:07.000000 clickzetta-migration-0.0.0.4/clickzetta_migration.egg-info/PKG-INFO
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2086 2023-07-18 08:25:08.000000 clickzetta-migration-0.0.0.4/clickzetta_migration.egg-info/SOURCES.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-07-18 08:25:07.000000 clickzetta-migration-0.0.0.4/clickzetta_migration.egg-info/dependency_links.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)       58 2023-07-18 08:25:07.000000 clickzetta-migration-0.0.0.4/clickzetta_migration.egg-info/entry_points.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-07-18 08:25:07.000000 clickzetta-migration-0.0.0.4/clickzetta_migration.egg-info/not-zip-safe
--rw-r--r--   0 lihanmiao   (501) staff       (20)      111 2023-07-18 08:25:07.000000 clickzetta-migration-0.0.0.4/clickzetta_migration.egg-info/requires.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)       10 2023-07-18 08:25:07.000000 clickzetta-migration-0.0.0.4/clickzetta_migration.egg-info/top_level.txt
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 08:25:08.014810 clickzetta-migration-0.0.0.4/migration/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 02:52:59.000000 clickzetta-migration-0.0.0.4/migration/__init__.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 08:25:08.015421 clickzetta-migration-0.0.0.4/migration/base/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       90 2023-07-11 03:06:38.000000 clickzetta-migration-0.0.0.4/migration/base/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      532 2023-07-13 08:55:34.000000 clickzetta-migration-0.0.0.4/migration/base/exceptions.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      444 2023-07-07 03:37:28.000000 clickzetta-migration-0.0.0.4/migration/base/status.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 08:25:08.015850 clickzetta-migration-0.0.0.4/migration/connector/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 02:53:59.000000 clickzetta-migration-0.0.0.4/migration/connector/__init__.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 08:25:08.016042 clickzetta-migration-0.0.0.4/migration/connector/destination/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 12:17:46.000000 clickzetta-migration-0.0.0.4/migration/connector/destination/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1249 2023-07-12 09:39:55.000000 clickzetta-migration-0.0.0.4/migration/connector/destination/base.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 08:25:08.016380 clickzetta-migration-0.0.0.4/migration/connector/destination/clickzetta/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-29 06:42:41.000000 clickzetta-migration-0.0.0.4/migration/connector/destination/clickzetta/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     6137 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.4/migration/connector/destination/clickzetta/destination.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 08:25:08.016696 clickzetta-migration-0.0.0.4/migration/connector/destination/doris/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-07-11 15:28:35.000000 clickzetta-migration-0.0.0.4/migration/connector/destination/doris/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     6243 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.4/migration/connector/destination/doris/destination.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 08:25:08.017416 clickzetta-migration-0.0.0.4/migration/connector/source/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       72 2023-07-11 03:06:38.000000 clickzetta-migration-0.0.0.4/migration/connector/source/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1879 2023-07-12 03:16:08.000000 clickzetta-migration-0.0.0.4/migration/connector/source/base.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 08:25:08.018093 clickzetta-migration-0.0.0.4/migration/connector/source/clickzetta/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-07-12 02:11:46.000000 clickzetta-migration-0.0.0.4/migration/connector/source/clickzetta/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     7338 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.4/migration/connector/source/clickzetta/source.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 08:25:08.018375 clickzetta-migration-0.0.0.4/migration/connector/source/doris/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:15:41.000000 clickzetta-migration-0.0.0.4/migration/connector/source/doris/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     6298 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.4/migration/connector/source/doris/source.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      352 2023-07-11 07:29:24.000000 clickzetta-migration-0.0.0.4/migration/connector/source/enum.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 08:25:08.018643 clickzetta-migration-0.0.0.4/migration/connector/source/hive/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:15:22.000000 clickzetta-migration-0.0.0.4/migration/connector/source/hive/__init__.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 08:25:08.018716 clickzetta-migration-0.0.0.4/migration/connector/source/odps/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:15:30.000000 clickzetta-migration-0.0.0.4/migration/connector/source/odps/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    11861 2023-07-17 08:44:25.000000 clickzetta-migration-0.0.0.4/migration/migration.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 08:25:08.019343 clickzetta-migration-0.0.0.4/migration/scheduler/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      112 2023-07-11 04:22:08.000000 clickzetta-migration-0.0.0.4/migration/scheduler/__init__.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 08:25:08.019733 clickzetta-migration-0.0.0.4/migration/scheduler/data_transformer/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:21:25.000000 clickzetta-migration-0.0.0.4/migration/scheduler/data_transformer/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3630 2023-07-12 11:45:19.000000 clickzetta-migration-0.0.0.4/migration/scheduler/data_transformer/transformer.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 08:25:08.019999 clickzetta-migration-0.0.0.4/migration/scheduler/data_validation/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:22:21.000000 clickzetta-migration-0.0.0.4/migration/scheduler/data_validation/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2845 2023-07-11 13:22:48.000000 clickzetta-migration-0.0.0.4/migration/scheduler/data_validation/validation.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4619 2023-07-17 07:57:48.000000 clickzetta-migration-0.0.0.4/migration/scheduler/scheduler.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 08:25:08.020283 clickzetta-migration-0.0.0.4/migration/scheduler/schema_transformer/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:21:14.000000 clickzetta-migration-0.0.0.4/migration/scheduler/schema_transformer/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4197 2023-07-12 09:39:55.000000 clickzetta-migration-0.0.0.4/migration/scheduler/schema_transformer/transformer.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 08:25:08.021500 clickzetta-migration-0.0.0.4/migration/scheduler/task/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      249 2023-07-11 03:06:38.000000 clickzetta-migration-0.0.0.4/migration/scheduler/task/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1395 2023-07-17 07:55:15.000000 clickzetta-migration-0.0.0.4/migration/scheduler/task/base_task.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1717 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.4/migration/scheduler/task/data_task.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1339 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.4/migration/scheduler/task/schema_task.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3356 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.4/migration/scheduler/task/validation_task.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2685 2023-07-13 10:20:49.000000 clickzetta-migration-0.0.0.4/migration/scheduler/transformer.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 08:25:08.021902 clickzetta-migration-0.0.0.4/migration/scheduler/unify_transformer/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-07-10 03:55:07.000000 clickzetta-migration-0.0.0.4/migration/scheduler/unify_transformer/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3881 2023-07-11 13:22:48.000000 clickzetta-migration-0.0.0.4/migration/scheduler/unify_transformer/transformer.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 08:25:08.022183 clickzetta-migration-0.0.0.4/migration/test/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-28 07:15:40.000000 clickzetta-migration-0.0.0.4/migration/test/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2348 2023-07-13 12:19:13.000000 clickzetta-migration-0.0.0.4/migration/test/util_test.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 08:25:08.022969 clickzetta-migration-0.0.0.4/migration/util/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 02:54:06.000000 clickzetta-migration-0.0.0.4/migration/util/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     7638 2023-07-17 09:06:42.000000 clickzetta-migration-0.0.0.4/migration/util/migration_tasks_status.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1180 2023-07-12 10:01:25.000000 clickzetta-migration-0.0.0.4/migration/util/object_storage_util.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1534 2023-07-18 07:36:47.000000 clickzetta-migration-0.0.0.4/migration/util/script_util.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)       23 2023-07-18 08:25:03.000000 clickzetta-migration-0.0.0.4/migration/version.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-07-18 08:25:08.023493 clickzetta-migration-0.0.0.4/setup.cfg
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1455 2023-07-18 08:25:03.000000 clickzetta-migration-0.0.0.4/setup.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 08:16:51.670657 clickzetta-migration-0.0.0.5/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       34 2023-07-18 07:23:21.000000 clickzetta-migration-0.0.0.5/MANIFEST.in
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      259 2023-07-19 08:16:51.670534 clickzetta-migration-0.0.0.5/PKG-INFO
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 08:16:51.662298 clickzetta-migration-0.0.0.5/clickzetta_migration.egg-info/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      259 2023-07-19 08:16:51.000000 clickzetta-migration-0.0.0.5/clickzetta_migration.egg-info/PKG-INFO
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2086 2023-07-19 08:16:51.000000 clickzetta-migration-0.0.0.5/clickzetta_migration.egg-info/SOURCES.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-07-19 08:16:51.000000 clickzetta-migration-0.0.0.5/clickzetta_migration.egg-info/dependency_links.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       58 2023-07-19 08:16:51.000000 clickzetta-migration-0.0.0.5/clickzetta_migration.egg-info/entry_points.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-07-19 08:16:51.000000 clickzetta-migration-0.0.0.5/clickzetta_migration.egg-info/not-zip-safe
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      141 2023-07-19 08:16:51.000000 clickzetta-migration-0.0.0.5/clickzetta_migration.egg-info/requires.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       10 2023-07-19 08:16:51.000000 clickzetta-migration-0.0.0.5/clickzetta_migration.egg-info/top_level.txt
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 08:16:51.662670 clickzetta-migration-0.0.0.5/migration/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 02:52:59.000000 clickzetta-migration-0.0.0.5/migration/__init__.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 08:16:51.663288 clickzetta-migration-0.0.0.5/migration/base/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       90 2023-07-11 03:06:38.000000 clickzetta-migration-0.0.0.5/migration/base/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      532 2023-07-13 08:55:34.000000 clickzetta-migration-0.0.0.5/migration/base/exceptions.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      444 2023-07-07 03:37:28.000000 clickzetta-migration-0.0.0.5/migration/base/status.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 08:16:51.663712 clickzetta-migration-0.0.0.5/migration/connector/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 02:53:59.000000 clickzetta-migration-0.0.0.5/migration/connector/__init__.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 08:16:51.663891 clickzetta-migration-0.0.0.5/migration/connector/destination/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 12:17:46.000000 clickzetta-migration-0.0.0.5/migration/connector/destination/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1249 2023-07-12 09:39:55.000000 clickzetta-migration-0.0.0.5/migration/connector/destination/base.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 08:16:51.664198 clickzetta-migration-0.0.0.5/migration/connector/destination/clickzetta/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-29 06:42:41.000000 clickzetta-migration-0.0.0.5/migration/connector/destination/clickzetta/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     6137 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.5/migration/connector/destination/clickzetta/destination.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 08:16:51.664578 clickzetta-migration-0.0.0.5/migration/connector/destination/doris/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-07-11 15:28:35.000000 clickzetta-migration-0.0.0.5/migration/connector/destination/doris/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     6243 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.5/migration/connector/destination/doris/destination.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 08:16:51.665208 clickzetta-migration-0.0.0.5/migration/connector/source/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       72 2023-07-11 03:06:38.000000 clickzetta-migration-0.0.0.5/migration/connector/source/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1879 2023-07-12 03:16:08.000000 clickzetta-migration-0.0.0.5/migration/connector/source/base.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 08:16:51.665588 clickzetta-migration-0.0.0.5/migration/connector/source/clickzetta/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-07-12 02:11:46.000000 clickzetta-migration-0.0.0.5/migration/connector/source/clickzetta/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     7338 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.5/migration/connector/source/clickzetta/source.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 08:16:51.665890 clickzetta-migration-0.0.0.5/migration/connector/source/doris/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:15:41.000000 clickzetta-migration-0.0.0.5/migration/connector/source/doris/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     6298 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.5/migration/connector/source/doris/source.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      352 2023-07-11 07:29:24.000000 clickzetta-migration-0.0.0.5/migration/connector/source/enum.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 08:16:51.666091 clickzetta-migration-0.0.0.5/migration/connector/source/hive/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:15:22.000000 clickzetta-migration-0.0.0.5/migration/connector/source/hive/__init__.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 08:16:51.666163 clickzetta-migration-0.0.0.5/migration/connector/source/odps/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:15:30.000000 clickzetta-migration-0.0.0.5/migration/connector/source/odps/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    11946 2023-07-19 08:11:58.000000 clickzetta-migration-0.0.0.5/migration/migration.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 08:16:51.666892 clickzetta-migration-0.0.0.5/migration/scheduler/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      112 2023-07-11 04:22:08.000000 clickzetta-migration-0.0.0.5/migration/scheduler/__init__.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 08:16:51.667257 clickzetta-migration-0.0.0.5/migration/scheduler/data_transformer/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:21:25.000000 clickzetta-migration-0.0.0.5/migration/scheduler/data_transformer/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3630 2023-07-12 11:45:19.000000 clickzetta-migration-0.0.0.5/migration/scheduler/data_transformer/transformer.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 08:16:51.667542 clickzetta-migration-0.0.0.5/migration/scheduler/data_validation/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:22:21.000000 clickzetta-migration-0.0.0.5/migration/scheduler/data_validation/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2845 2023-07-11 13:22:48.000000 clickzetta-migration-0.0.0.5/migration/scheduler/data_validation/validation.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4619 2023-07-17 07:57:48.000000 clickzetta-migration-0.0.0.5/migration/scheduler/scheduler.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 08:16:51.667823 clickzetta-migration-0.0.0.5/migration/scheduler/schema_transformer/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:21:14.000000 clickzetta-migration-0.0.0.5/migration/scheduler/schema_transformer/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4197 2023-07-12 09:39:55.000000 clickzetta-migration-0.0.0.5/migration/scheduler/schema_transformer/transformer.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 08:16:51.668979 clickzetta-migration-0.0.0.5/migration/scheduler/task/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      249 2023-07-11 03:06:38.000000 clickzetta-migration-0.0.0.5/migration/scheduler/task/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1395 2023-07-17 07:55:15.000000 clickzetta-migration-0.0.0.5/migration/scheduler/task/base_task.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1717 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.5/migration/scheduler/task/data_task.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1339 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.5/migration/scheduler/task/schema_task.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3356 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.5/migration/scheduler/task/validation_task.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2685 2023-07-13 10:20:49.000000 clickzetta-migration-0.0.0.5/migration/scheduler/transformer.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 08:16:51.669252 clickzetta-migration-0.0.0.5/migration/scheduler/unify_transformer/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-07-10 03:55:07.000000 clickzetta-migration-0.0.0.5/migration/scheduler/unify_transformer/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3881 2023-07-11 13:22:48.000000 clickzetta-migration-0.0.0.5/migration/scheduler/unify_transformer/transformer.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 08:16:51.669518 clickzetta-migration-0.0.0.5/migration/test/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-28 07:15:40.000000 clickzetta-migration-0.0.0.5/migration/test/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2348 2023-07-13 12:19:13.000000 clickzetta-migration-0.0.0.5/migration/test/util_test.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 08:16:51.670170 clickzetta-migration-0.0.0.5/migration/util/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 02:54:06.000000 clickzetta-migration-0.0.0.5/migration/util/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     7705 2023-07-19 08:16:46.000000 clickzetta-migration-0.0.0.5/migration/util/migration_tasks_status.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1180 2023-07-12 10:01:25.000000 clickzetta-migration-0.0.0.5/migration/util/object_storage_util.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1534 2023-07-18 07:36:47.000000 clickzetta-migration-0.0.0.5/migration/util/script_util.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       23 2023-07-19 08:16:46.000000 clickzetta-migration-0.0.0.5/migration/version.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-07-19 08:16:51.670699 clickzetta-migration-0.0.0.5/setup.cfg
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1503 2023-07-19 07:42:07.000000 clickzetta-migration-0.0.0.5/setup.py
```

### Comparing `clickzetta-migration-0.0.0.4/clickzetta_migration.egg-info/SOURCES.txt` & `clickzetta-migration-0.0.0.5/clickzetta_migration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.4/migration/base/exceptions.py` & `clickzetta-migration-0.0.0.5/migration/base/exceptions.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.4/migration/connector/destination/base.py` & `clickzetta-migration-0.0.0.5/migration/connector/destination/base.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.4/migration/connector/destination/clickzetta/destination.py` & `clickzetta-migration-0.0.0.5/migration/connector/destination/clickzetta/destination.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.4/migration/connector/destination/doris/destination.py` & `clickzetta-migration-0.0.0.5/migration/connector/destination/doris/destination.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.4/migration/connector/source/base.py` & `clickzetta-migration-0.0.0.5/migration/connector/source/base.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.4/migration/connector/source/clickzetta/source.py` & `clickzetta-migration-0.0.0.5/migration/connector/source/clickzetta/source.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.4/migration/connector/source/doris/source.py` & `clickzetta-migration-0.0.0.5/migration/connector/source/doris/source.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.4/migration/migration.py` & `clickzetta-migration-0.0.0.5/migration/migration.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     with open(out_path, 'w') as f:
         for db in dbs:
             if db.startswith("__") or db.startswith("information_schema"):
                 continue
             tables = source.get_table_names(db)
             for table in tables:
                 f.write(f"{db}.{table}\n")
+    logger.info(f"Generating meta from source {source} to {out_path} successfully!")
 
 
 def schema(source: Source, destination: Destination, db_list: list, config_table_list: list, external_table_list: list,
            project_name: str, concurrency: int, quit_if_fail: bool):
     logger.info(f"Transforming schema from source {source} to destination {destination}")
     print(f"Transforming schema from source {source} to destination {destination}")
     SchemaTransformer(source, destination, project_name, db_list, config_table_list, external_table_list, concurrency,
```

### Comparing `clickzetta-migration-0.0.0.4/migration/scheduler/data_transformer/transformer.py` & `clickzetta-migration-0.0.0.5/migration/scheduler/data_transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.4/migration/scheduler/data_validation/validation.py` & `clickzetta-migration-0.0.0.5/migration/scheduler/data_validation/validation.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.4/migration/scheduler/scheduler.py` & `clickzetta-migration-0.0.0.5/migration/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.4/migration/scheduler/schema_transformer/transformer.py` & `clickzetta-migration-0.0.0.5/migration/scheduler/schema_transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.4/migration/scheduler/task/base_task.py` & `clickzetta-migration-0.0.0.5/migration/scheduler/task/base_task.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.4/migration/scheduler/task/data_task.py` & `clickzetta-migration-0.0.0.5/migration/scheduler/task/data_task.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.4/migration/scheduler/task/schema_task.py` & `clickzetta-migration-0.0.0.5/migration/scheduler/task/schema_task.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.4/migration/scheduler/task/validation_task.py` & `clickzetta-migration-0.0.0.5/migration/scheduler/task/validation_task.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.4/migration/scheduler/transformer.py` & `clickzetta-migration-0.0.0.5/migration/scheduler/transformer.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.4/migration/scheduler/unify_transformer/transformer.py` & `clickzetta-migration-0.0.0.5/migration/scheduler/unify_transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.4/migration/test/util_test.py` & `clickzetta-migration-0.0.0.5/migration/test/util_test.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.4/migration/util/migration_tasks_status.py` & `clickzetta-migration-0.0.0.5/migration/util/migration_tasks_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,18 @@
             prject_id STRING NOT NULL,
             task_status STRING NOT NULL,
             task_type STRING NOT NULL,
             task_start_time DATETIME NOT NULL,
             task_end_time DATETIME
         )
         UNIQUE KEY (id)
-        DISTRIBUTED BY HASH(id) BUCKETS 6;
+        DISTRIBUTED BY HASH(id) BUCKETS 6
+        PROPERTIES (
+            "replication_num" = "1"
+        );
         """
         destination.execute_sql(ddl)
         return f"{project_name}_{table_index}"
 
 
 def update_task_status(destination: Destination, task: Task):
     if destination.name.lower() == "clickzetta":
```

### Comparing `clickzetta-migration-0.0.0.4/migration/util/object_storage_util.py` & `clickzetta-migration-0.0.0.5/migration/util/object_storage_util.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.4/migration/util/script_util.py` & `clickzetta-migration-0.0.0.5/migration/util/script_util.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.4/setup.py` & `clickzetta-migration-0.0.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,20 +11,22 @@
 
 # Should be one of:
 # 'Development Status :: 3 - Alpha'
 # 'Development Status :: 4 - Beta'
 # 'Development Status :: 5 - Production/Stable'
 release_status = "Development Status :: 3 - Alpha"
 dependencies = [
-    'scheduler >= 0.8.4',
+    'schedule >= 1.2.0',
     'clickzetta-connector >= 0.8.29',
     'docopt >= 0.6.2',
     'pyyaml >= 6.0',
     'openpyxl >= 3.1.2',
     'tabulate >= 0.8.9',
+    'pymysql >= 1.0.2',
+    'sqlparse >= 0.4.1',
 ]
 extras = {
 
 }
 
 all_extras = []
```

