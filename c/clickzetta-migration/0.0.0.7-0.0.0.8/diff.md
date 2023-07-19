# Comparing `tmp/clickzetta-migration-0.0.0.7.tar.gz` & `tmp/clickzetta-migration-0.0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickzetta-migration-0.0.0.7.tar", last modified: Wed Jul 19 08:35:51 2023, max compression
+gzip compressed data, was "clickzetta-migration-0.0.0.8.tar", last modified: Wed Jul 19 10:53:38 2023, max compression
```

## Comparing `clickzetta-migration-0.0.0.7.tar` & `clickzetta-migration-0.0.0.8.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 08:35:51.756165 clickzetta-migration-0.0.0.7/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       34 2023-07-18 07:23:21.000000 clickzetta-migration-0.0.0.7/MANIFEST.in
--rw-r--r--   0 lihanmiao   (501) staff       (20)      259 2023-07-19 08:35:51.756019 clickzetta-migration-0.0.0.7/PKG-INFO
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 08:35:51.747306 clickzetta-migration-0.0.0.7/clickzetta_migration.egg-info/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      259 2023-07-19 08:35:51.000000 clickzetta-migration-0.0.0.7/clickzetta_migration.egg-info/PKG-INFO
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2086 2023-07-19 08:35:51.000000 clickzetta-migration-0.0.0.7/clickzetta_migration.egg-info/SOURCES.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-07-19 08:35:51.000000 clickzetta-migration-0.0.0.7/clickzetta_migration.egg-info/dependency_links.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)       58 2023-07-19 08:35:51.000000 clickzetta-migration-0.0.0.7/clickzetta_migration.egg-info/entry_points.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-07-19 08:35:51.000000 clickzetta-migration-0.0.0.7/clickzetta_migration.egg-info/not-zip-safe
--rw-r--r--   0 lihanmiao   (501) staff       (20)      141 2023-07-19 08:35:51.000000 clickzetta-migration-0.0.0.7/clickzetta_migration.egg-info/requires.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)       10 2023-07-19 08:35:51.000000 clickzetta-migration-0.0.0.7/clickzetta_migration.egg-info/top_level.txt
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 08:35:51.747999 clickzetta-migration-0.0.0.7/migration/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 02:52:59.000000 clickzetta-migration-0.0.0.7/migration/__init__.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 08:35:51.748681 clickzetta-migration-0.0.0.7/migration/base/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       90 2023-07-11 03:06:38.000000 clickzetta-migration-0.0.0.7/migration/base/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      532 2023-07-13 08:55:34.000000 clickzetta-migration-0.0.0.7/migration/base/exceptions.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      444 2023-07-07 03:37:28.000000 clickzetta-migration-0.0.0.7/migration/base/status.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 08:35:51.749070 clickzetta-migration-0.0.0.7/migration/connector/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 02:53:59.000000 clickzetta-migration-0.0.0.7/migration/connector/__init__.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 08:35:51.749238 clickzetta-migration-0.0.0.7/migration/connector/destination/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 12:17:46.000000 clickzetta-migration-0.0.0.7/migration/connector/destination/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1249 2023-07-12 09:39:55.000000 clickzetta-migration-0.0.0.7/migration/connector/destination/base.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 08:35:51.749565 clickzetta-migration-0.0.0.7/migration/connector/destination/clickzetta/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-29 06:42:41.000000 clickzetta-migration-0.0.0.7/migration/connector/destination/clickzetta/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     6137 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.7/migration/connector/destination/clickzetta/destination.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 08:35:51.750028 clickzetta-migration-0.0.0.7/migration/connector/destination/doris/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-07-11 15:28:35.000000 clickzetta-migration-0.0.0.7/migration/connector/destination/doris/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     6243 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.7/migration/connector/destination/doris/destination.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 08:35:51.750627 clickzetta-migration-0.0.0.7/migration/connector/source/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       72 2023-07-11 03:06:38.000000 clickzetta-migration-0.0.0.7/migration/connector/source/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1879 2023-07-12 03:16:08.000000 clickzetta-migration-0.0.0.7/migration/connector/source/base.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 08:35:51.750989 clickzetta-migration-0.0.0.7/migration/connector/source/clickzetta/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-07-12 02:11:46.000000 clickzetta-migration-0.0.0.7/migration/connector/source/clickzetta/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     7338 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.7/migration/connector/source/clickzetta/source.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 08:35:51.751274 clickzetta-migration-0.0.0.7/migration/connector/source/doris/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:15:41.000000 clickzetta-migration-0.0.0.7/migration/connector/source/doris/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     6298 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.7/migration/connector/source/doris/source.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      352 2023-07-11 07:29:24.000000 clickzetta-migration-0.0.0.7/migration/connector/source/enum.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 08:35:51.751569 clickzetta-migration-0.0.0.7/migration/connector/source/hive/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:15:22.000000 clickzetta-migration-0.0.0.7/migration/connector/source/hive/__init__.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 08:35:51.751638 clickzetta-migration-0.0.0.7/migration/connector/source/odps/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:15:30.000000 clickzetta-migration-0.0.0.7/migration/connector/source/odps/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    11946 2023-07-19 08:11:58.000000 clickzetta-migration-0.0.0.7/migration/migration.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 08:35:51.752230 clickzetta-migration-0.0.0.7/migration/scheduler/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      112 2023-07-11 04:22:08.000000 clickzetta-migration-0.0.0.7/migration/scheduler/__init__.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 08:35:51.752596 clickzetta-migration-0.0.0.7/migration/scheduler/data_transformer/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:21:25.000000 clickzetta-migration-0.0.0.7/migration/scheduler/data_transformer/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3630 2023-07-12 11:45:19.000000 clickzetta-migration-0.0.0.7/migration/scheduler/data_transformer/transformer.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 08:35:51.752867 clickzetta-migration-0.0.0.7/migration/scheduler/data_validation/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:22:21.000000 clickzetta-migration-0.0.0.7/migration/scheduler/data_validation/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2845 2023-07-11 13:22:48.000000 clickzetta-migration-0.0.0.7/migration/scheduler/data_validation/validation.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4619 2023-07-17 07:57:48.000000 clickzetta-migration-0.0.0.7/migration/scheduler/scheduler.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 08:35:51.753127 clickzetta-migration-0.0.0.7/migration/scheduler/schema_transformer/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:21:14.000000 clickzetta-migration-0.0.0.7/migration/scheduler/schema_transformer/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4197 2023-07-12 09:39:55.000000 clickzetta-migration-0.0.0.7/migration/scheduler/schema_transformer/transformer.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 08:35:51.754212 clickzetta-migration-0.0.0.7/migration/scheduler/task/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      249 2023-07-11 03:06:38.000000 clickzetta-migration-0.0.0.7/migration/scheduler/task/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1395 2023-07-17 07:55:15.000000 clickzetta-migration-0.0.0.7/migration/scheduler/task/base_task.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1717 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.7/migration/scheduler/task/data_task.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1339 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.7/migration/scheduler/task/schema_task.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3356 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.7/migration/scheduler/task/validation_task.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2685 2023-07-13 10:20:49.000000 clickzetta-migration-0.0.0.7/migration/scheduler/transformer.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 08:35:51.754620 clickzetta-migration-0.0.0.7/migration/scheduler/unify_transformer/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-07-10 03:55:07.000000 clickzetta-migration-0.0.0.7/migration/scheduler/unify_transformer/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3881 2023-07-11 13:22:48.000000 clickzetta-migration-0.0.0.7/migration/scheduler/unify_transformer/transformer.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 08:35:51.754884 clickzetta-migration-0.0.0.7/migration/test/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-28 07:15:40.000000 clickzetta-migration-0.0.0.7/migration/test/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2480 2023-07-19 08:31:48.000000 clickzetta-migration-0.0.0.7/migration/test/util_test.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 08:35:51.755696 clickzetta-migration-0.0.0.7/migration/util/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 02:54:06.000000 clickzetta-migration-0.0.0.7/migration/util/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     7705 2023-07-19 08:16:46.000000 clickzetta-migration-0.0.0.7/migration/util/migration_tasks_status.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1180 2023-07-12 10:01:25.000000 clickzetta-migration-0.0.0.7/migration/util/object_storage_util.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1787 2023-07-19 08:33:07.000000 clickzetta-migration-0.0.0.7/migration/util/script_util.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)       23 2023-07-19 08:35:49.000000 clickzetta-migration-0.0.0.7/migration/version.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-07-19 08:35:51.756213 clickzetta-migration-0.0.0.7/setup.cfg
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1503 2023-07-19 08:35:49.000000 clickzetta-migration-0.0.0.7/setup.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 10:53:38.016198 clickzetta-migration-0.0.0.8/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       34 2023-07-18 07:23:21.000000 clickzetta-migration-0.0.0.8/MANIFEST.in
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      259 2023-07-19 10:53:38.016077 clickzetta-migration-0.0.0.8/PKG-INFO
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 10:53:38.008955 clickzetta-migration-0.0.0.8/clickzetta_migration.egg-info/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      259 2023-07-19 10:53:37.000000 clickzetta-migration-0.0.0.8/clickzetta_migration.egg-info/PKG-INFO
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2086 2023-07-19 10:53:38.000000 clickzetta-migration-0.0.0.8/clickzetta_migration.egg-info/SOURCES.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-07-19 10:53:37.000000 clickzetta-migration-0.0.0.8/clickzetta_migration.egg-info/dependency_links.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       58 2023-07-19 10:53:37.000000 clickzetta-migration-0.0.0.8/clickzetta_migration.egg-info/entry_points.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-07-19 10:53:37.000000 clickzetta-migration-0.0.0.8/clickzetta_migration.egg-info/not-zip-safe
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      141 2023-07-19 10:53:37.000000 clickzetta-migration-0.0.0.8/clickzetta_migration.egg-info/requires.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       10 2023-07-19 10:53:37.000000 clickzetta-migration-0.0.0.8/clickzetta_migration.egg-info/top_level.txt
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 10:53:38.009313 clickzetta-migration-0.0.0.8/migration/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 02:52:59.000000 clickzetta-migration-0.0.0.8/migration/__init__.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 10:53:38.009832 clickzetta-migration-0.0.0.8/migration/base/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       90 2023-07-11 03:06:38.000000 clickzetta-migration-0.0.0.8/migration/base/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      532 2023-07-13 08:55:34.000000 clickzetta-migration-0.0.0.8/migration/base/exceptions.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      444 2023-07-07 03:37:28.000000 clickzetta-migration-0.0.0.8/migration/base/status.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 10:53:38.010027 clickzetta-migration-0.0.0.8/migration/connector/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 02:53:59.000000 clickzetta-migration-0.0.0.8/migration/connector/__init__.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 10:53:38.010160 clickzetta-migration-0.0.0.8/migration/connector/destination/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 12:17:46.000000 clickzetta-migration-0.0.0.8/migration/connector/destination/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1249 2023-07-12 09:39:55.000000 clickzetta-migration-0.0.0.8/migration/connector/destination/base.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 10:53:38.010433 clickzetta-migration-0.0.0.8/migration/connector/destination/clickzetta/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-29 06:42:41.000000 clickzetta-migration-0.0.0.8/migration/connector/destination/clickzetta/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     6137 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.8/migration/connector/destination/clickzetta/destination.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 10:53:38.010704 clickzetta-migration-0.0.0.8/migration/connector/destination/doris/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-07-11 15:28:35.000000 clickzetta-migration-0.0.0.8/migration/connector/destination/doris/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     6243 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.8/migration/connector/destination/doris/destination.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 10:53:38.011314 clickzetta-migration-0.0.0.8/migration/connector/source/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       72 2023-07-11 03:06:38.000000 clickzetta-migration-0.0.0.8/migration/connector/source/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1879 2023-07-12 03:16:08.000000 clickzetta-migration-0.0.0.8/migration/connector/source/base.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 10:53:38.011593 clickzetta-migration-0.0.0.8/migration/connector/source/clickzetta/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-07-12 02:11:46.000000 clickzetta-migration-0.0.0.8/migration/connector/source/clickzetta/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     7648 2023-07-19 10:52:37.000000 clickzetta-migration-0.0.0.8/migration/connector/source/clickzetta/source.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 10:53:38.011854 clickzetta-migration-0.0.0.8/migration/connector/source/doris/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:15:41.000000 clickzetta-migration-0.0.0.8/migration/connector/source/doris/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     6298 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.8/migration/connector/source/doris/source.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      352 2023-07-11 07:29:24.000000 clickzetta-migration-0.0.0.8/migration/connector/source/enum.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 10:53:38.012052 clickzetta-migration-0.0.0.8/migration/connector/source/hive/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:15:22.000000 clickzetta-migration-0.0.0.8/migration/connector/source/hive/__init__.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 10:53:38.012122 clickzetta-migration-0.0.0.8/migration/connector/source/odps/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:15:30.000000 clickzetta-migration-0.0.0.8/migration/connector/source/odps/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    11946 2023-07-19 08:11:58.000000 clickzetta-migration-0.0.0.8/migration/migration.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 10:53:38.012624 clickzetta-migration-0.0.0.8/migration/scheduler/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      112 2023-07-11 04:22:08.000000 clickzetta-migration-0.0.0.8/migration/scheduler/__init__.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 10:53:38.012998 clickzetta-migration-0.0.0.8/migration/scheduler/data_transformer/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:21:25.000000 clickzetta-migration-0.0.0.8/migration/scheduler/data_transformer/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3630 2023-07-12 11:45:19.000000 clickzetta-migration-0.0.0.8/migration/scheduler/data_transformer/transformer.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 10:53:38.013268 clickzetta-migration-0.0.0.8/migration/scheduler/data_validation/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:22:21.000000 clickzetta-migration-0.0.0.8/migration/scheduler/data_validation/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2841 2023-07-19 10:52:37.000000 clickzetta-migration-0.0.0.8/migration/scheduler/data_validation/validation.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4619 2023-07-17 07:57:48.000000 clickzetta-migration-0.0.0.8/migration/scheduler/scheduler.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 10:53:38.013498 clickzetta-migration-0.0.0.8/migration/scheduler/schema_transformer/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:21:14.000000 clickzetta-migration-0.0.0.8/migration/scheduler/schema_transformer/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4197 2023-07-12 09:39:55.000000 clickzetta-migration-0.0.0.8/migration/scheduler/schema_transformer/transformer.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 10:53:38.014518 clickzetta-migration-0.0.0.8/migration/scheduler/task/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      249 2023-07-11 03:06:38.000000 clickzetta-migration-0.0.0.8/migration/scheduler/task/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1395 2023-07-17 07:55:15.000000 clickzetta-migration-0.0.0.8/migration/scheduler/task/base_task.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1717 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.8/migration/scheduler/task/data_task.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1339 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.8/migration/scheduler/task/schema_task.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3356 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.8/migration/scheduler/task/validation_task.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2685 2023-07-13 10:20:49.000000 clickzetta-migration-0.0.0.8/migration/scheduler/transformer.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 10:53:38.014786 clickzetta-migration-0.0.0.8/migration/scheduler/unify_transformer/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-07-10 03:55:07.000000 clickzetta-migration-0.0.0.8/migration/scheduler/unify_transformer/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3881 2023-07-11 13:22:48.000000 clickzetta-migration-0.0.0.8/migration/scheduler/unify_transformer/transformer.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 10:53:38.015055 clickzetta-migration-0.0.0.8/migration/test/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-28 07:15:40.000000 clickzetta-migration-0.0.0.8/migration/test/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2480 2023-07-19 08:31:48.000000 clickzetta-migration-0.0.0.8/migration/test/util_test.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-19 10:53:38.015832 clickzetta-migration-0.0.0.8/migration/util/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 02:54:06.000000 clickzetta-migration-0.0.0.8/migration/util/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     7705 2023-07-19 08:16:46.000000 clickzetta-migration-0.0.0.8/migration/util/migration_tasks_status.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1180 2023-07-12 10:01:25.000000 clickzetta-migration-0.0.0.8/migration/util/object_storage_util.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1787 2023-07-19 08:33:07.000000 clickzetta-migration-0.0.0.8/migration/util/script_util.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       23 2023-07-19 10:53:36.000000 clickzetta-migration-0.0.0.8/migration/version.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-07-19 10:53:38.016238 clickzetta-migration-0.0.0.8/setup.cfg
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1503 2023-07-19 08:35:49.000000 clickzetta-migration-0.0.0.8/setup.py
```

### Comparing `clickzetta-migration-0.0.0.7/clickzetta_migration.egg-info/SOURCES.txt` & `clickzetta-migration-0.0.0.8/clickzetta_migration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.7/migration/base/exceptions.py` & `clickzetta-migration-0.0.0.8/migration/base/exceptions.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.7/migration/connector/destination/base.py` & `clickzetta-migration-0.0.0.8/migration/connector/destination/base.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.7/migration/connector/destination/clickzetta/destination.py` & `clickzetta-migration-0.0.0.8/migration/connector/destination/clickzetta/destination.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.7/migration/connector/destination/doris/destination.py` & `clickzetta-migration-0.0.0.8/migration/connector/destination/doris/destination.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.7/migration/connector/source/base.py` & `clickzetta-migration-0.0.0.8/migration/connector/source/base.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.7/migration/connector/source/clickzetta/source.py` & `clickzetta-migration-0.0.0.8/migration/connector/source/clickzetta/source.py`

 * *Files 5% similar despite different names*

```diff
@@ -145,12 +145,18 @@
             unload_sql += partition_sql[:-4]
         try:
             self.execute_sql(unload_sql)
         except BaseException as e:
             logger.error(f"Create temp view {temp_view_name} failed, error: {e}")
             self.execute_sql(f"drop materialized view if exists {temp_view_name}")
             raise f"Create temp view {temp_view_name} failed, error: {e}"
-        file_paths = script_utils.get_files_path(self.instance_id, self.workspace, temp_view_name.split('.')[0],
+        file_paths = set()
+        try:
+            file_paths = script_utils.get_files_path(self.instance_id, self.workspace, temp_view_name.split('.')[0],
                                                  temp_view_name.split('.')[1], meta_conf_path=self.meta_conf_path)
+        except BaseException as e:
+            logger.error(f"Get object storage files path failed, error: {e}")
+            self.execute_sql(f"drop materialized view if exists {temp_view_name}")
+            raise f"Get object storage files path failed, error: {e}"
         logger.info(f"Unload data from Clickzetta successfully")
         self.execute_sql(f"drop materialized view if exists {temp_view_name}")
         return file_paths
```

### Comparing `clickzetta-migration-0.0.0.7/migration/connector/source/doris/source.py` & `clickzetta-migration-0.0.0.8/migration/connector/source/doris/source.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.7/migration/migration.py` & `clickzetta-migration-0.0.0.8/migration/migration.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.7/migration/scheduler/data_transformer/transformer.py` & `clickzetta-migration-0.0.0.8/migration/scheduler/data_transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.7/migration/scheduler/data_validation/validation.py` & `clickzetta-migration-0.0.0.8/migration/scheduler/data_validation/validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 LEFT_BRACKET = '('
 
 
 class Validation(Transformer):
 
     def get_migration_tasks(self):
         transform_table_list = self.get_transform_table_list()
-        if transform_table_list.empty():
+        if not transform_table_list:
             logger.warning("No table to transform, please check your profile.yml")
             raise ProfileConfigError("No table to transform, please check your profile.yml")
         validation_tables = []
 
         if DOT_SPLITTER not in transform_table_list[0]:
             for db in transform_table_list:
                 tables = self.source.get_table_names(db)
```

### Comparing `clickzetta-migration-0.0.0.7/migration/scheduler/scheduler.py` & `clickzetta-migration-0.0.0.8/migration/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.7/migration/scheduler/schema_transformer/transformer.py` & `clickzetta-migration-0.0.0.8/migration/scheduler/schema_transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.7/migration/scheduler/task/base_task.py` & `clickzetta-migration-0.0.0.8/migration/scheduler/task/base_task.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.7/migration/scheduler/task/data_task.py` & `clickzetta-migration-0.0.0.8/migration/scheduler/task/data_task.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.7/migration/scheduler/task/schema_task.py` & `clickzetta-migration-0.0.0.8/migration/scheduler/task/schema_task.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.7/migration/scheduler/task/validation_task.py` & `clickzetta-migration-0.0.0.8/migration/scheduler/task/validation_task.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.7/migration/scheduler/transformer.py` & `clickzetta-migration-0.0.0.8/migration/scheduler/transformer.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.7/migration/scheduler/unify_transformer/transformer.py` & `clickzetta-migration-0.0.0.8/migration/scheduler/unify_transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.7/migration/test/util_test.py` & `clickzetta-migration-0.0.0.8/migration/test/util_test.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.7/migration/util/migration_tasks_status.py` & `clickzetta-migration-0.0.0.8/migration/util/migration_tasks_status.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.7/migration/util/object_storage_util.py` & `clickzetta-migration-0.0.0.8/migration/util/object_storage_util.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.7/migration/util/script_util.py` & `clickzetta-migration-0.0.0.8/migration/util/script_util.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.7/setup.py` & `clickzetta-migration-0.0.0.8/setup.py`

 * *Files identical despite different names*

