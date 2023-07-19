# Comparing `tmp/ml-management-0.0.41.tar.gz` & `tmp/ml-management-0.0.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-management-0.0.41.tar", last modified: Fri Jul  7 06:26:59 2023, max compression
+gzip compressed data, was "ml-management-0.0.42.tar", last modified: Wed Jul 19 07:08:19 2023, max compression
```

## Comparing `ml-management-0.0.41.tar` & `ml-management-0.0.42.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-07-07 06:26:59.957116 ml-management-0.0.41/
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)       18 2023-07-05 09:14:25.000000 ml-management-0.0.41/MANIFEST.in
-drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-07-07 06:26:59.949116 ml-management-0.0.41/ML_management/
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        0 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/__init__.py
-drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-07-07 06:26:59.949116 ml-management-0.0.41/ML_management/collectors/
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      120 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/collectors/__init__.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     1092 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/collectors/collector_pattern.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      456 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/collectors/collector_pattern_to_methods_map.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     1318 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/collectors/collectors.py
-drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-07-07 06:26:59.949116 ml-management-0.0.41/ML_management/collectors/dummy/
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        0 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/collectors/dummy/__init__.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      463 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/collectors/dummy/dummy_collector.py
-drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-07-07 06:26:59.949116 ml-management-0.0.41/ML_management/collectors/s3/
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        0 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/collectors/s3/__init__.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     9711 2023-07-06 08:06:30.000000 ml-management-0.0.41/ML_management/collectors/s3/s3collector.py
-drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-07-07 06:26:59.949116 ml-management-0.0.41/ML_management/collectors/topic_markers/
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        0 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/collectors/topic_markers/__init__.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)   331440 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/collectors/topic_markers/api_schema.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     3167 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/collectors/topic_markers/topic_markers_collector.py
-drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-07-07 06:26:59.953116 ml-management-0.0.41/ML_management/dataset_loader_template/
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        0 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/dataset_loader_template/__init__.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     2407 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/dataset_loader_template/dataset_loader_pattern.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      457 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/dataset_loader_template/dataset_loader_pattern_to_methods_map.py
-drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-07-07 06:26:59.953116 ml-management-0.0.41/ML_management/executor_template/
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        0 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/executor_template/__init__.py
-drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-07-07 06:26:59.953116 ml-management-0.0.41/ML_management/executor_template/default_executors/
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        0 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/executor_template/default_executors/__init__.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      895 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/executor_template/default_executors/finetune_executor.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      843 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/executor_template/default_executors/test_executor.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      869 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/executor_template/default_executors/train_executor.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     4566 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/executor_template/executor_pattern.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      402 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/executor_template/executor_pattern_to_methods_map.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      334 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/executor_template/upload_model_mode.py
-drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-07-07 06:26:59.957116 ml-management-0.0.41/ML_management/mlmanagement/
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      737 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/mlmanagement/__init__.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     3392 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/mlmanagement/jsonschema_exceptions.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     5054 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/mlmanagement/jsonschema_inference.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)    14229 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/mlmanagement/mlmanagement.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)    10260 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/mlmanagement/mlmanager.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      201 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/mlmanagement/model_type.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     5001 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/mlmanagement/server_mlmanager_exceptions.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      316 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/mlmanagement/utils.py
-drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-07-07 06:26:59.957116 ml-management-0.0.41/ML_management/models/
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        0 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/models/__init__.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      949 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/models/model_type_to_methods_map.py
-drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-07-07 06:26:59.957116 ml-management-0.0.41/ML_management/models/patterns/
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        0 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/models/patterns/__init__.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     4202 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/models/patterns/model_pattern.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      561 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/models/patterns/retrainable_model.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      445 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/models/patterns/torch_model.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      457 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/models/patterns/trainable_model.py
-drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-07-07 06:26:59.957116 ml-management-0.0.41/ML_management/registry/
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        0 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/registry/__init__.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     2566 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/registry/exceptions.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     7556 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/registry/registry_manager.py
-drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-07-07 06:26:59.957116 ml-management-0.0.41/ML_management/tests/
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        0 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/tests/__init__.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     3361 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/tests/test_jsonschema_inference.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     9858 2023-07-05 16:21:11.000000 ml-management-0.0.41/ML_management/tests/test_s3_dataset.py
-drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-07-07 06:26:59.957116 ml-management-0.0.41/ML_management/uploader_data/
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        0 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/uploader_data/__init__.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     1914 2023-07-05 16:21:11.000000 ml-management-0.0.41/ML_management/uploader_data/s3_uploader.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     1430 2023-07-05 16:21:11.000000 ml-management-0.0.41/ML_management/uploader_data/utils.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      312 2023-07-07 06:26:59.957116 ml-management-0.0.41/PKG-INFO
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)       56 2023-07-05 09:14:25.000000 ml-management-0.0.41/README.md
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        6 2023-07-07 06:25:31.000000 ml-management-0.0.41/VERSION
-drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-07-07 06:26:59.957116 ml-management-0.0.41/ml_management.egg-info/
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      312 2023-07-07 06:26:59.000000 ml-management-0.0.41/ml_management.egg-info/PKG-INFO
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     2486 2023-07-07 06:26:59.000000 ml-management-0.0.41/ml_management.egg-info/SOURCES.txt
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        1 2023-07-07 06:26:59.000000 ml-management-0.0.41/ml_management.egg-info/dependency_links.txt
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      166 2023-07-07 06:26:59.000000 ml-management-0.0.41/ml_management.egg-info/requires.txt
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)       14 2023-07-07 06:26:59.000000 ml-management-0.0.41/ml_management.egg-info/top_level.txt
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)       38 2023-07-07 06:26:59.957116 ml-management-0.0.41/setup.cfg
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     1076 2023-07-05 16:21:11.000000 ml-management-0.0.41/setup.py
+drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-07-19 07:08:19.213818 ml-management-0.0.42/
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)       18 2023-06-05 10:13:00.000000 ml-management-0.0.42/MANIFEST.in
+drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-07-19 07:08:19.209818 ml-management-0.0.42/ML_management/
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/__init__.py
+drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-07-19 07:08:19.209818 ml-management-0.0.42/ML_management/collectors/
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      120 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/collectors/__init__.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     1092 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/collectors/collector_pattern.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      456 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/collectors/collector_pattern_to_methods_map.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     1318 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/collectors/collectors.py
+drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-07-19 07:08:19.209818 ml-management-0.0.42/ML_management/collectors/dummy/
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/collectors/dummy/__init__.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      463 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/collectors/dummy/dummy_collector.py
+drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-07-19 07:08:19.209818 ml-management-0.0.42/ML_management/collectors/s3/
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/collectors/s3/__init__.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     9711 2023-07-10 10:57:45.000000 ml-management-0.0.42/ML_management/collectors/s3/s3collector.py
+drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-07-19 07:08:19.209818 ml-management-0.0.42/ML_management/collectors/topic_markers/
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/collectors/topic_markers/__init__.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)   331440 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/collectors/topic_markers/api_schema.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     3167 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/collectors/topic_markers/topic_markers_collector.py
+drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-07-19 07:08:19.209818 ml-management-0.0.42/ML_management/dataset_loader_template/
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/dataset_loader_template/__init__.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     3651 2023-07-17 08:09:48.000000 ml-management-0.0.42/ML_management/dataset_loader_template/dataset_loader_pattern.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      457 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/dataset_loader_template/dataset_loader_pattern_to_methods_map.py
+drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-07-19 07:08:19.209818 ml-management-0.0.42/ML_management/executor_template/
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/executor_template/__init__.py
+drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-07-19 07:08:19.213818 ml-management-0.0.42/ML_management/executor_template/default_executors/
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/executor_template/default_executors/__init__.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      895 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/executor_template/default_executors/finetune_executor.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      843 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/executor_template/default_executors/test_executor.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      869 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/executor_template/default_executors/train_executor.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     5807 2023-07-17 08:09:48.000000 ml-management-0.0.42/ML_management/executor_template/executor_pattern.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      402 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/executor_template/executor_pattern_to_methods_map.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      334 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/executor_template/upload_model_mode.py
+drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-07-19 07:08:19.213818 ml-management-0.0.42/ML_management/mlmanagement/
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      737 2023-07-03 06:55:20.000000 ml-management-0.0.42/ML_management/mlmanagement/__init__.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     3392 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/mlmanagement/jsonschema_exceptions.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     5054 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/mlmanagement/jsonschema_inference.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)    14229 2023-07-17 08:09:48.000000 ml-management-0.0.42/ML_management/mlmanagement/mlmanagement.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)    10260 2023-07-17 08:09:48.000000 ml-management-0.0.42/ML_management/mlmanagement/mlmanager.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      201 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/mlmanagement/model_type.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     5001 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/mlmanagement/server_mlmanager_exceptions.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      316 2023-07-17 08:09:48.000000 ml-management-0.0.42/ML_management/mlmanagement/utils.py
+drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-07-19 07:08:19.213818 ml-management-0.0.42/ML_management/models/
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/models/__init__.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      949 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/models/model_type_to_methods_map.py
+drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-07-19 07:08:19.213818 ml-management-0.0.42/ML_management/models/patterns/
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/models/patterns/__init__.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     4202 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/models/patterns/model_pattern.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      561 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/models/patterns/retrainable_model.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      445 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/models/patterns/torch_model.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      457 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/models/patterns/trainable_model.py
+drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-07-19 07:08:19.213818 ml-management-0.0.42/ML_management/registry/
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/registry/__init__.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     2564 2023-07-10 10:57:45.000000 ml-management-0.0.42/ML_management/registry/exceptions.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     7556 2023-07-17 08:09:48.000000 ml-management-0.0.42/ML_management/registry/registry_manager.py
+drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-07-19 07:08:19.213818 ml-management-0.0.42/ML_management/tests/
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/tests/__init__.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     3361 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/tests/test_jsonschema_inference.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     9858 2023-07-10 10:57:45.000000 ml-management-0.0.42/ML_management/tests/test_s3_dataset.py
+drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-07-19 07:08:19.213818 ml-management-0.0.42/ML_management/uploader_data/
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-05 10:13:00.000000 ml-management-0.0.42/ML_management/uploader_data/__init__.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     1914 2023-07-10 10:57:45.000000 ml-management-0.0.42/ML_management/uploader_data/s3_uploader.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     1430 2023-07-10 10:57:45.000000 ml-management-0.0.42/ML_management/uploader_data/utils.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      367 2023-07-19 07:08:19.213818 ml-management-0.0.42/PKG-INFO
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)       56 2023-06-05 10:13:00.000000 ml-management-0.0.42/README.md
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        6 2023-07-19 07:07:33.000000 ml-management-0.0.42/VERSION
+drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-07-19 07:08:19.213818 ml-management-0.0.42/ml_management.egg-info/
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      367 2023-07-19 07:08:19.000000 ml-management-0.0.42/ml_management.egg-info/PKG-INFO
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     2486 2023-07-19 07:08:19.000000 ml-management-0.0.42/ml_management.egg-info/SOURCES.txt
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        1 2023-07-19 07:08:19.000000 ml-management-0.0.42/ml_management.egg-info/dependency_links.txt
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      166 2023-07-19 07:08:19.000000 ml-management-0.0.42/ml_management.egg-info/requires.txt
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)       14 2023-07-19 07:08:19.000000 ml-management-0.0.42/ml_management.egg-info/top_level.txt
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)       38 2023-07-19 07:08:19.213818 ml-management-0.0.42/setup.cfg
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     1076 2023-07-10 10:57:45.000000 ml-management-0.0.42/setup.py
```

### Comparing `ml-management-0.0.41/ML_management/collectors/collector_pattern.py` & `ml-management-0.0.42/ML_management/collectors/collector_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.41/ML_management/collectors/collectors.py` & `ml-management-0.0.42/ML_management/collectors/collectors.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.41/ML_management/collectors/s3/s3collector.py` & `ml-management-0.0.42/ML_management/collectors/s3/s3collector.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.41/ML_management/collectors/topic_markers/api_schema.py` & `ml-management-0.0.42/ML_management/collectors/topic_markers/api_schema.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.41/ML_management/collectors/topic_markers/topic_markers_collector.py` & `ml-management-0.0.42/ML_management/collectors/topic_markers/topic_markers_collector.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.41/ML_management/executor_template/default_executors/finetune_executor.py` & `ml-management-0.0.42/ML_management/executor_template/default_executors/finetune_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.41/ML_management/executor_template/default_executors/test_executor.py` & `ml-management-0.0.42/ML_management/executor_template/default_executors/test_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.41/ML_management/executor_template/default_executors/train_executor.py` & `ml-management-0.0.42/ML_management/executor_template/default_executors/train_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.41/ML_management/executor_template/executor_pattern.py` & `ml-management-0.0.42/ML_management/executor_template/executor_pattern.py`

 * *Files 24% similar despite different names*

```diff
@@ -61,31 +61,52 @@
                       In this case, the ``"my_file"`` artifact is downloaded from S3.
                       The ``"my_file2"`` artifact is downloaded from local path.
 
                       If ``None``, no artifacts are added to the model.
         """
         raise NotImplementedError
 
-    def upload_executor(self, pip_requirements=None, extra_pip_requirements=None, conda_env=None):
+    def upload_executor(self, pip_requirements=None, extra_pip_requirements=None, conda_env=None, artifacts: dict = None):
         """
         Upload wrapper to MLmanagement server.
 
         :param pip_requirements: {{ pip_requirements }}
+
         :param extra_pip_requirements: {{ extra_pip_requirements }}
         `pip_requirements` and 'extra_pip_requirements' must be either a string path to a pip requirements file on the
             local filesystem or an iterable of pip requirement strings.
+
         :param conda_env: {{ conda_env }}
         'conda_env' must be a dict specifying the conda environment for this model.
+
+        :param artifacts: A dictionary containing ``<name, artifact_uri>`` entries. Remote artifact URIs
+                          are resolved to absolute filesystem paths, producing a dictionary of
+                          ``<name, absolute_path>`` entries. ``python_model`` can reference these
+                          resolved entries as the ``artifacts`` property of the ``context`` parameter
+                          in :func:`PythonModel.load_context() <mlflow.pyfunc.PythonModel.load_context>`
+                          and :func:`PythonModel.predict() <mlflow.pyfunc.PythonModel.predict>`.
+                          For example, consider the following ``artifacts`` dictionary::
+
+                            {
+                                "my_file": "s3://my-bucket/path/to/my/file"
+                            }
+
+                          In this case, the ``"my_file"`` artifact is downloaded from S3. The
+                          ``python_model`` can then refer to ``"my_file"`` as an absolute filesystem
+                          path via ``context.artifacts["my_file"]``.
+
+                          If ``None``, no artifacts are added to the executor.
         """
         old_experiment_name = utils.active_experiment_name
         mlmanagement.set_experiment(EXPERIMENT_NAME_FOR_EXECUTOR)
         try:
             with mlmanagement.start_run(nested=True):
                 mlmanagement.log_model(
                     artifact_path="",
+                    artifacts=artifacts,
                     python_model=self,
                     registered_model_name=self.executor_name,
                     pip_requirements=pip_requirements,
                     extra_pip_requirements=extra_pip_requirements,
                     conda_env=conda_env,
                 )
         except Exception as err:
```

### Comparing `ml-management-0.0.41/ML_management/mlmanagement/__init__.py` & `ml-management-0.0.42/ML_management/mlmanagement/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.41/ML_management/mlmanagement/jsonschema_exceptions.py` & `ml-management-0.0.42/ML_management/mlmanagement/jsonschema_exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.41/ML_management/mlmanagement/jsonschema_inference.py` & `ml-management-0.0.42/ML_management/mlmanagement/jsonschema_inference.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.41/ML_management/mlmanagement/mlmanagement.py` & `ml-management-0.0.42/ML_management/mlmanagement/mlmanagement.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.41/ML_management/mlmanagement/mlmanager.py` & `ml-management-0.0.42/ML_management/mlmanagement/mlmanager.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.41/ML_management/mlmanagement/server_mlmanager_exceptions.py` & `ml-management-0.0.42/ML_management/mlmanagement/server_mlmanager_exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.41/ML_management/models/model_type_to_methods_map.py` & `ml-management-0.0.42/ML_management/models/model_type_to_methods_map.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.41/ML_management/models/patterns/model_pattern.py` & `ml-management-0.0.42/ML_management/models/patterns/model_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.41/ML_management/models/patterns/retrainable_model.py` & `ml-management-0.0.42/ML_management/models/patterns/retrainable_model.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.41/ML_management/registry/exceptions.py` & `ml-management-0.0.42/ML_management/registry/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Custom exception definition (necessary for RegistryManager)."""
 
 
 class VersionNotFound(Exception):
     """Define Version Not Found Exception."""
 
-    def __init__(self, model_name: str, version: str):
+    def __init__(self, model_name: str, version: int):
         self.model_name = model_name
         self.version = version
-        self.message = f'There is no version "{self.version}" for model "{self.model_name}"'
+        self.message = f'There is no version {self.version} for model "{self.model_name}"'
         super().__init__(self.message)
 
     def __reduce__(self):
         """Define reduce method to make exception picklable."""
         return (VersionNotFound, (self.model_name, self.version))
```

### Comparing `ml-management-0.0.41/ML_management/registry/registry_manager.py` & `ml-management-0.0.42/ML_management/registry/registry_manager.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.41/ML_management/tests/test_jsonschema_inference.py` & `ml-management-0.0.42/ML_management/tests/test_jsonschema_inference.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.41/ML_management/tests/test_s3_dataset.py` & `ml-management-0.0.42/ML_management/tests/test_s3_dataset.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.41/ML_management/uploader_data/s3_uploader.py` & `ml-management-0.0.42/ML_management/uploader_data/s3_uploader.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.41/ML_management/uploader_data/utils.py` & `ml-management-0.0.42/ML_management/uploader_data/utils.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.41/ml_management.egg-info/SOURCES.txt` & `ml-management-0.0.42/ml_management.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.41/setup.py` & `ml-management-0.0.42/setup.py`

 * *Files identical despite different names*

