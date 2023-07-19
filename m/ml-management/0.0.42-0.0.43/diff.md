# Comparing `tmp/ml-management-0.0.42.tar.gz` & `tmp/ml-management-0.0.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-management-0.0.42.tar", last modified: Wed Jul 19 07:08:19 2023, max compression
+gzip compressed data, was "ml-management-0.0.43.tar", last modified: Wed Jul 19 10:30:58 2023, max compression
```

## Comparing `ml-management-0.0.42.tar` & `ml-management-0.0.43.tar`

### file list

```diff
@@ -1,74 +1,75 @@
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-07-19 07:08:19.213818 ml-management-0.0.42/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)       18 2023-06-05 10:13:00.000000 ml-management-0.0.42/MANIFEST.in
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-07-19 07:08:19.209818 ml-management-0.0.42/ML_management/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/__init__.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-07-19 07:08:19.209818 ml-management-0.0.42/ML_management/collectors/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      120 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/collectors/__init__.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     1092 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/collectors/collector_pattern.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      456 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/collectors/collector_pattern_to_methods_map.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     1318 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/collectors/collectors.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-07-19 07:08:19.209818 ml-management-0.0.42/ML_management/collectors/dummy/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/collectors/dummy/__init__.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      463 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/collectors/dummy/dummy_collector.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-07-19 07:08:19.209818 ml-management-0.0.42/ML_management/collectors/s3/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/collectors/s3/__init__.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     9711 2023-07-10 10:57:45.000000 ml-management-0.0.42/ML_management/collectors/s3/s3collector.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-07-19 07:08:19.209818 ml-management-0.0.42/ML_management/collectors/topic_markers/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/collectors/topic_markers/__init__.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)   331440 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/collectors/topic_markers/api_schema.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     3167 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/collectors/topic_markers/topic_markers_collector.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-07-19 07:08:19.209818 ml-management-0.0.42/ML_management/dataset_loader_template/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/dataset_loader_template/__init__.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     3651 2023-07-17 08:09:48.000000 ml-management-0.0.42/ML_management/dataset_loader_template/dataset_loader_pattern.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      457 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/dataset_loader_template/dataset_loader_pattern_to_methods_map.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-07-19 07:08:19.209818 ml-management-0.0.42/ML_management/executor_template/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/executor_template/__init__.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-07-19 07:08:19.213818 ml-management-0.0.42/ML_management/executor_template/default_executors/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/executor_template/default_executors/__init__.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      895 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/executor_template/default_executors/finetune_executor.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      843 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/executor_template/default_executors/test_executor.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      869 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/executor_template/default_executors/train_executor.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     5807 2023-07-17 08:09:48.000000 ml-management-0.0.42/ML_management/executor_template/executor_pattern.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      402 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/executor_template/executor_pattern_to_methods_map.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      334 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/executor_template/upload_model_mode.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-07-19 07:08:19.213818 ml-management-0.0.42/ML_management/mlmanagement/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      737 2023-07-03 06:55:20.000000 ml-management-0.0.42/ML_management/mlmanagement/__init__.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     3392 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/mlmanagement/jsonschema_exceptions.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     5054 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/mlmanagement/jsonschema_inference.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)    14229 2023-07-17 08:09:48.000000 ml-management-0.0.42/ML_management/mlmanagement/mlmanagement.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)    10260 2023-07-17 08:09:48.000000 ml-management-0.0.42/ML_management/mlmanagement/mlmanager.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      201 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/mlmanagement/model_type.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     5001 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/mlmanagement/server_mlmanager_exceptions.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      316 2023-07-17 08:09:48.000000 ml-management-0.0.42/ML_management/mlmanagement/utils.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-07-19 07:08:19.213818 ml-management-0.0.42/ML_management/models/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/models/__init__.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      949 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/models/model_type_to_methods_map.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-07-19 07:08:19.213818 ml-management-0.0.42/ML_management/models/patterns/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/models/patterns/__init__.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     4202 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/models/patterns/model_pattern.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      561 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/models/patterns/retrainable_model.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      445 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/models/patterns/torch_model.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      457 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/models/patterns/trainable_model.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-07-19 07:08:19.213818 ml-management-0.0.42/ML_management/registry/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/registry/__init__.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     2564 2023-07-10 10:57:45.000000 ml-management-0.0.42/ML_management/registry/exceptions.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     7556 2023-07-17 08:09:48.000000 ml-management-0.0.42/ML_management/registry/registry_manager.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-07-19 07:08:19.213818 ml-management-0.0.42/ML_management/tests/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/tests/__init__.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     3361 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/tests/test_jsonschema_inference.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     9858 2023-07-10 10:57:45.000000 ml-management-0.0.42/ML_management/tests/test_s3_dataset.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-07-19 07:08:19.213818 ml-management-0.0.42/ML_management/uploader_data/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/uploader_data/__init__.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     1914 2023-07-10 10:57:45.000000 ml-management-0.0.42/ML_management/uploader_data/s3_uploader.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     1430 2023-07-10 10:57:45.000000 ml-management-0.0.42/ML_management/uploader_data/utils.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      367 2023-07-19 07:08:19.213818 ml-management-0.0.42/PKG-INFO
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)       56 2023-06-05 10:13:00.000000 ml-management-0.0.42/README.md
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        6 2023-07-19 07:07:33.000000 ml-management-0.0.42/VERSION
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-07-19 07:08:19.213818 ml-management-0.0.42/ml_management.egg-info/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      367 2023-07-19 07:08:19.000000 ml-management-0.0.42/ml_management.egg-info/PKG-INFO
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     2486 2023-07-19 07:08:19.000000 ml-management-0.0.42/ml_management.egg-info/SOURCES.txt
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        1 2023-07-19 07:08:19.000000 ml-management-0.0.42/ml_management.egg-info/dependency_links.txt
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      166 2023-07-19 07:08:19.000000 ml-management-0.0.42/ml_management.egg-info/requires.txt
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)       14 2023-07-19 07:08:19.000000 ml-management-0.0.42/ml_management.egg-info/top_level.txt
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)       38 2023-07-19 07:08:19.213818 ml-management-0.0.42/setup.cfg
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     1076 2023-07-10 10:57:45.000000 ml-management-0.0.42/setup.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-19 10:30:58.550286 ml-management-0.0.43/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)       18 2023-06-29 11:52:32.000000 ml-management-0.0.43/MANIFEST.in
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-19 10:30:58.546286 ml-management-0.0.43/ML_management/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/__init__.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-19 10:30:58.546286 ml-management-0.0.43/ML_management/collectors/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      120 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/collectors/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     1092 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/collectors/collector_pattern.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      456 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/collectors/collector_pattern_to_methods_map.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     1318 2023-07-11 12:32:50.000000 ml-management-0.0.43/ML_management/collectors/collectors.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-19 10:30:58.546286 ml-management-0.0.43/ML_management/collectors/dummy/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/collectors/dummy/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      463 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/collectors/dummy/dummy_collector.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-19 10:30:58.546286 ml-management-0.0.43/ML_management/collectors/s3/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/collectors/s3/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     9711 2023-07-10 10:35:03.000000 ml-management-0.0.43/ML_management/collectors/s3/s3collector.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-19 10:30:58.550286 ml-management-0.0.43/ML_management/collectors/topic_markers/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/collectors/topic_markers/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)   331440 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/collectors/topic_markers/api_schema.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     3167 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/collectors/topic_markers/topic_markers_collector.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-19 10:30:58.550286 ml-management-0.0.43/ML_management/dataset_loader_template/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/dataset_loader_template/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     4373 2023-07-19 10:07:23.000000 ml-management-0.0.43/ML_management/dataset_loader_template/dataset_loader_pattern.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      457 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/dataset_loader_template/dataset_loader_pattern_to_methods_map.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-19 10:30:58.550286 ml-management-0.0.43/ML_management/executor_template/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/executor_template/__init__.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-19 10:30:58.550286 ml-management-0.0.43/ML_management/executor_template/default_executors/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/executor_template/default_executors/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      895 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/executor_template/default_executors/finetune_executor.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      843 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/executor_template/default_executors/test_executor.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      869 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/executor_template/default_executors/train_executor.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     6505 2023-07-19 10:07:23.000000 ml-management-0.0.43/ML_management/executor_template/executor_pattern.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      402 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/executor_template/executor_pattern_to_methods_map.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      334 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/executor_template/upload_model_mode.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-19 10:30:58.550286 ml-management-0.0.43/ML_management/mlmanagement/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      737 2023-07-04 13:14:56.000000 ml-management-0.0.43/ML_management/mlmanagement/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     3392 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/mlmanagement/jsonschema_exceptions.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     5054 2023-07-11 12:32:50.000000 ml-management-0.0.43/ML_management/mlmanagement/jsonschema_inference.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)    15292 2023-07-19 10:07:23.000000 ml-management-0.0.43/ML_management/mlmanagement/mlmanagement.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)    10500 2023-07-19 10:07:23.000000 ml-management-0.0.43/ML_management/mlmanagement/mlmanager.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      201 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/mlmanagement/model_type.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     2701 2023-07-19 10:07:23.000000 ml-management-0.0.43/ML_management/mlmanagement/module_finder.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     5001 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/mlmanagement/server_mlmanager_exceptions.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      316 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/mlmanagement/utils.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-19 10:30:58.550286 ml-management-0.0.43/ML_management/models/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/models/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      949 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/models/model_type_to_methods_map.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-19 10:30:58.550286 ml-management-0.0.43/ML_management/models/patterns/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/models/patterns/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     4865 2023-07-19 10:07:23.000000 ml-management-0.0.43/ML_management/models/patterns/model_pattern.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      561 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/models/patterns/retrainable_model.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      445 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/models/patterns/torch_model.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      457 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/models/patterns/trainable_model.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-19 10:30:58.550286 ml-management-0.0.43/ML_management/registry/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/registry/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     2564 2023-07-10 10:35:03.000000 ml-management-0.0.43/ML_management/registry/exceptions.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     7556 2023-07-11 12:32:50.000000 ml-management-0.0.43/ML_management/registry/registry_manager.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-19 10:30:58.550286 ml-management-0.0.43/ML_management/tests/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/tests/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     3361 2023-07-11 12:32:50.000000 ml-management-0.0.43/ML_management/tests/test_jsonschema_inference.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     9858 2023-07-11 12:32:50.000000 ml-management-0.0.43/ML_management/tests/test_s3_dataset.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-19 10:30:58.550286 ml-management-0.0.43/ML_management/uploader_data/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/uploader_data/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     1914 2023-07-10 10:35:03.000000 ml-management-0.0.43/ML_management/uploader_data/s3_uploader.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     1430 2023-07-10 10:35:03.000000 ml-management-0.0.43/ML_management/uploader_data/utils.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      367 2023-07-19 10:30:58.550286 ml-management-0.0.43/PKG-INFO
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)       56 2023-06-29 11:52:32.000000 ml-management-0.0.43/README.md
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        7 2023-07-19 10:28:54.000000 ml-management-0.0.43/VERSION
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-19 10:30:58.550286 ml-management-0.0.43/ml_management.egg-info/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      367 2023-07-19 10:30:58.000000 ml-management-0.0.43/ml_management.egg-info/PKG-INFO
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     2530 2023-07-19 10:30:58.000000 ml-management-0.0.43/ml_management.egg-info/SOURCES.txt
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        1 2023-07-19 10:30:58.000000 ml-management-0.0.43/ml_management.egg-info/dependency_links.txt
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      166 2023-07-19 10:30:58.000000 ml-management-0.0.43/ml_management.egg-info/requires.txt
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)       14 2023-07-19 10:30:58.000000 ml-management-0.0.43/ml_management.egg-info/top_level.txt
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)       38 2023-07-19 10:30:58.550286 ml-management-0.0.43/setup.cfg
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     1076 2023-07-10 10:35:03.000000 ml-management-0.0.43/setup.py
```

### Comparing `ml-management-0.0.42/ML_management/collectors/collector_pattern.py` & `ml-management-0.0.43/ML_management/collectors/collector_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.42/ML_management/collectors/collectors.py` & `ml-management-0.0.43/ML_management/collectors/collectors.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.42/ML_management/collectors/s3/s3collector.py` & `ml-management-0.0.43/ML_management/collectors/s3/s3collector.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.42/ML_management/collectors/topic_markers/api_schema.py` & `ml-management-0.0.43/ML_management/collectors/topic_markers/api_schema.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.42/ML_management/collectors/topic_markers/topic_markers_collector.py` & `ml-management-0.0.43/ML_management/collectors/topic_markers/topic_markers_collector.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.42/ML_management/executor_template/default_executors/finetune_executor.py` & `ml-management-0.0.43/ML_management/executor_template/default_executors/finetune_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.42/ML_management/executor_template/default_executors/test_executor.py` & `ml-management-0.0.43/ML_management/executor_template/default_executors/test_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.42/ML_management/executor_template/default_executors/train_executor.py` & `ml-management-0.0.43/ML_management/executor_template/default_executors/train_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.42/ML_management/executor_template/executor_pattern.py` & `ml-management-0.0.43/ML_management/executor_template/executor_pattern.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Executor template for custom executor."""
 from abc import ABC, abstractmethod
-from typing import List
+from typing import List, Optional
 
 from ML_management.executor_template.upload_model_mode import UploadModelMode
 from ML_management.mlmanagement import mlmanagement, utils
+from ML_management.mlmanagement.module_finder import ModuleFinder
 from ML_management.mlmanagement.utils import EXPERIMENT_NAME_FOR_EXECUTOR
 from ML_management.models.model_type_to_methods_map import ModelMethodName
 from mlflow.pyfunc import PythonModel
 
 
 class JobExecutorPattern(PythonModel, ABC):
     """Define custom job executor."""
@@ -61,15 +62,23 @@
                       In this case, the ``"my_file"`` artifact is downloaded from S3.
                       The ``"my_file2"`` artifact is downloaded from local path.
 
                       If ``None``, no artifacts are added to the model.
         """
         raise NotImplementedError
 
-    def upload_executor(self, pip_requirements=None, extra_pip_requirements=None, conda_env=None, artifacts: dict = None):
+    def upload_executor(
+        self,
+        pip_requirements=None,
+        extra_pip_requirements=None,
+        conda_env=None,
+        artifacts: Optional[dict] = None,
+        extra_modules_names: Optional[List[str]] = None,
+        used_modules_names: Optional[List[str]] = None,
+    ):
         """
         Upload wrapper to MLmanagement server.
 
         :param pip_requirements: {{ pip_requirements }}
 
         :param extra_pip_requirements: {{ extra_pip_requirements }}
         `pip_requirements` and 'extra_pip_requirements' must be either a string path to a pip requirements file on the
@@ -91,25 +100,33 @@
                             }
 
                           In this case, the ``"my_file"`` artifact is downloaded from S3. The
                           ``python_model`` can then refer to ``"my_file"`` as an absolute filesystem
                           path via ``context.artifacts["my_file"]``.
 
                           If ``None``, no artifacts are added to the executor.
+
+        :param extra_modules_names: names of modules that should be pickled by value
+            in addition to auto-detected modules.
+
+        :param used_modules_names: modules that should be pickled by value, disables the auto-detection of modules.
         """
         old_experiment_name = utils.active_experiment_name
         mlmanagement.set_experiment(EXPERIMENT_NAME_FOR_EXECUTOR)
         try:
             with mlmanagement.start_run(nested=True):
                 mlmanagement.log_model(
                     artifact_path="",
                     artifacts=artifacts,
                     python_model=self,
                     registered_model_name=self.executor_name,
                     pip_requirements=pip_requirements,
                     extra_pip_requirements=extra_pip_requirements,
                     conda_env=conda_env,
+                    extra_modules_names=extra_modules_names,
+                    used_modules_names=used_modules_names,
+                    root_module_name=ModuleFinder.get_my_caller_module_name(),
                 )
         except Exception as err:
             raise err
         finally:
             utils.active_experiment_name = old_experiment_name
```

### Comparing `ml-management-0.0.42/ML_management/mlmanagement/__init__.py` & `ml-management-0.0.43/ML_management/mlmanagement/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.42/ML_management/mlmanagement/jsonschema_exceptions.py` & `ml-management-0.0.43/ML_management/mlmanagement/jsonschema_exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.42/ML_management/mlmanagement/jsonschema_inference.py` & `ml-management-0.0.43/ML_management/mlmanagement/jsonschema_inference.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.42/ML_management/mlmanagement/mlmanagement.py` & `ml-management-0.0.43/ML_management/mlmanagement/mlmanagement.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,22 +4,25 @@
 ML_manager sends request to our server on /mlflow endpoint
 Server calls original mlflow function accordingly
 """
 import atexit
 import inspect
 import io
 import os
+import sys
 import tempfile
 import zipfile
 from typing import Any, Dict, List, Optional, Union
 
+import cloudpickle
 import numpy
 import pandas
 from ML_management.mlmanagement import utils
 from ML_management.mlmanagement.mlmanager import request_for_function
+from ML_management.mlmanagement.module_finder import ModuleFinder
 from ML_management.mlmanagement.utils import active_run_stack, is_server
 from mlflow.entities import Experiment, Run, RunStatus
 from mlflow.entities.model_registry import ModelVersion, RegisteredModel
 from mlflow.models import Model
 from mlflow.pyfunc import PyFuncModel
 from mlflow.store.entities import PagedList
 from mlflow.tracking.fluent import _RUN_ID_ENV_VAR
@@ -174,23 +177,44 @@
     await_registration_for=300,
     pip_requirements=None,
     extra_pip_requirements=None,
     metadata=None,
     source_model_name=None,
     source_model_version=None,
     upload_model_mode=None,
+    extra_modules_names=None,
+    used_modules_names=None,
+    root_module_name: str = "__main__",
 ):
     """
     Log a Pyfunc model with custom inference logic and optional data dependencies as an MLflow artifact.
 
     Current run is using.
     You cannot specify the parameters: loader_module, data_path and the parameters: python_model, artifacts together.
     """
+    if extra_modules_names and used_modules_names:
+        raise RuntimeError("Parameters 'extra_modules_names' and 'used_modules_names' cannot be used at the same time.")
     start_run_if_not_exist()
-    return request_for_function(inspect.currentframe(), ["pyfunc"])
+    if used_modules_names:
+        submodules = set(used_modules_names)
+        ModuleFinder.import_modules_by_name(submodules)
+    else:
+        submodules = ModuleFinder().find_root_submodules(root_name=root_module_name)
+        if extra_modules_names:
+            extra_set = set(extra_modules_names)
+            ModuleFinder.import_modules_by_name(extra_set)
+            submodules = submodules.union(extra_set)
+    try:
+        for module_name in submodules:
+            cloudpickle.register_pickle_by_value(sys.modules[module_name])
+        result = request_for_function(inspect.currentframe(), ["pyfunc"])
+        return result
+    finally:
+        for module_name in submodules:
+            cloudpickle.unregister_pickle_by_value(sys.modules[module_name])
 
 
 def log_metric(key: str, value: float, step: Optional[int] = None) -> None:
     """Log a metric under the current run. If no run is active, this method will create a new active run."""
     start_run_if_not_exist()
     return request_for_function(inspect.currentframe())
```

### Comparing `ml-management-0.0.42/ML_management/mlmanagement/mlmanager.py` & `ml-management-0.0.43/ML_management/mlmanagement/mlmanager.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,14 +45,21 @@
     Steps for log model:
     0) Infer jsonschema, raise if it is invalid
     1) open temporary directory
     2) Do mlflow.save_model() locally
     3) Pack it to zip file
     4) Send it to server to log model there.
     """
+    extra_imports_args = [
+        "submodules",
+        "module_name",
+        "used_modules_names",
+        "extra_modules_names",
+        "root_module_name",
+    ]
     delete_args_for_save_model_func = [
         "artifact_path",
         "registered_model_name",
         "await_registration_for",
         # now, extra arguments
         "upload_model_mode",
         "source_model_name",
@@ -61,14 +68,16 @@
     delete_args_for_log_func = [
         "python_model",
         "artifacts",
         "conda_env",
         "pip_requirements",
         "extra_pip_requirements",
     ]  # not need for log model on server
+    for delete_arg in extra_imports_args:
+        del kwargs[delete_arg]
     kwargs_for_save_model = kwargs.copy()
     for delete_arg in delete_args_for_save_model_func:
         del kwargs_for_save_model[delete_arg]
 
     python_model = kwargs_for_save_model["python_model"]
 
     # import some modules here because of circular import
```

### Comparing `ml-management-0.0.42/ML_management/mlmanagement/server_mlmanager_exceptions.py` & `ml-management-0.0.43/ML_management/mlmanagement/server_mlmanager_exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.42/ML_management/models/model_type_to_methods_map.py` & `ml-management-0.0.43/ML_management/models/model_type_to_methods_map.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.42/ML_management/models/patterns/model_pattern.py` & `ml-management-0.0.43/ML_management/models/patterns/model_pattern.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Define Abstract class for Model with necessary methods and methods to implement."""
 from abc import ABC, abstractmethod
+from typing import List, Optional
 
 from ML_management.mlmanagement import mlmanagement, utils
+from ML_management.mlmanagement.module_finder import ModuleFinder
 
 import mlflow
 
 
 class Model(mlflow.pyfunc.PythonModel, ABC):
     """Abstract class for model that Job will use."""
 
@@ -22,14 +24,16 @@
         self,
         registered_model_name: str,
         artifacts: dict = None,
         experiment_name: str = None,
         pip_requirements=None,
         extra_pip_requirements=None,
         conda_env=None,
+        extra_modules_names: Optional[List[str]] = None,
+        used_modules_names: Optional[List[str]] = None,
     ):
         """
         Upload wrapper to MLmanagement server.
 
         :param pyfunc_model_name: The run-relative artifact path to which to log the Python model.
         :param artifacts: A dictionary containing ``<name, artifact_uri>`` entries. Remote artifact URIs
                           are resolved to absolute filesystem paths, producing a dictionary of
@@ -55,14 +59,17 @@
         :param experiment_name: Name of experiment to which load the model
         :param pip_requirements: {{ pip_requirements }}
         :param extra_pip_requirements: {{ extra_pip_requirements }}
         `pip_requirements` and 'extra_pip_requirements' must be either a string path to a pip requirements file on the
             local filesystem or an iterable of pip requirement strings.
         :param conda_env: {{ conda_env }}
         'conda_env' must be a dict specifying the conda environment for this model.
+        :param extra_modules_names: names of modules that should be pickled by value
+            in addition to auto-detected modules.
+        :param used_modules_names: modules that should be pickled by value, disables the auto-detection of modules.
         """
         old_experiment_name = utils.active_experiment_name
         if experiment_name:
             mlmanagement.set_experiment(experiment_name)
         try:
             with mlmanagement.start_run(nested=True):
                 mlmanagement.log_model(
@@ -75,12 +82,15 @@
                     else None,  # set that after model download from mlflow
                     source_model_version=self.source_model_version
                     if hasattr(self, "source_model_version")
                     else None,  # set that after model download from mlflow
                     pip_requirements=pip_requirements,
                     extra_pip_requirements=extra_pip_requirements,
                     conda_env=conda_env,
+                    extra_modules_names=extra_modules_names,
+                    used_modules_names=used_modules_names,
+                    root_module_name=ModuleFinder.get_my_caller_module_name(),
                 )
         except Exception as err:
             raise err
         finally:
             utils.active_experiment_name = old_experiment_name
```

### Comparing `ml-management-0.0.42/ML_management/models/patterns/retrainable_model.py` & `ml-management-0.0.43/ML_management/models/patterns/retrainable_model.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.42/ML_management/registry/exceptions.py` & `ml-management-0.0.43/ML_management/registry/exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.42/ML_management/registry/registry_manager.py` & `ml-management-0.0.43/ML_management/registry/registry_manager.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.42/ML_management/tests/test_jsonschema_inference.py` & `ml-management-0.0.43/ML_management/tests/test_jsonschema_inference.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.42/ML_management/tests/test_s3_dataset.py` & `ml-management-0.0.43/ML_management/tests/test_s3_dataset.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.42/ML_management/uploader_data/s3_uploader.py` & `ml-management-0.0.43/ML_management/uploader_data/s3_uploader.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.42/ML_management/uploader_data/utils.py` & `ml-management-0.0.43/ML_management/uploader_data/utils.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.42/ml_management.egg-info/SOURCES.txt` & `ml-management-0.0.43/ml_management.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 ML_management/executor_template/default_executors/train_executor.py
 ML_management/mlmanagement/__init__.py
 ML_management/mlmanagement/jsonschema_exceptions.py
 ML_management/mlmanagement/jsonschema_inference.py
 ML_management/mlmanagement/mlmanagement.py
 ML_management/mlmanagement/mlmanager.py
 ML_management/mlmanagement/model_type.py
+ML_management/mlmanagement/module_finder.py
 ML_management/mlmanagement/server_mlmanager_exceptions.py
 ML_management/mlmanagement/utils.py
 ML_management/models/__init__.py
 ML_management/models/model_type_to_methods_map.py
 ML_management/models/patterns/__init__.py
 ML_management/models/patterns/model_pattern.py
 ML_management/models/patterns/retrainable_model.py
```

### Comparing `ml-management-0.0.42/setup.py` & `ml-management-0.0.43/setup.py`

 * *Files identical despite different names*

