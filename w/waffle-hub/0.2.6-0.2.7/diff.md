# Comparing `tmp/waffle_hub-0.2.6.tar.gz` & `tmp/waffle_hub-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waffle_hub-0.2.6.tar", last modified: Mon Jul 17 01:46:18 2023, max compression
+gzip compressed data, was "waffle_hub-0.2.7.tar", last modified: Wed Jul 19 12:10:25 2023, max compression
```

## Comparing `waffle_hub-0.2.6.tar` & `waffle_hub-0.2.7.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-07-17 01:46:18.114918 waffle_hub-0.2.6/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    35149 2023-06-12 07:00:05.000000 waffle_hub-0.2.6/LICENSE
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      138 2023-06-12 07:00:05.000000 waffle_hub-0.2.6/MANIFEST.in
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     4422 2023-07-17 01:46:18.110918 waffle_hub-0.2.6/PKG-INFO
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     3341 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/README.md
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      386 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/requirements.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       38 2023-07-17 01:46:18.114918 waffle_hub-0.2.6/setup.cfg
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2935 2023-06-16 03:34:36.000000 waffle_hub-0.2.6/setup.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-07-17 01:46:18.106917 waffle_hub-0.2.6/tests/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     8844 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/tests/test_cli.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    18878 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/tests/test_dataset.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     4581 2023-06-24 03:11:53.000000 waffle_hub-0.2.6/tests/test_ddp.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    12717 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/tests/test_hub.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-07-17 01:46:18.106917 waffle_hub-0.2.6/waffle_hub/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2292 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/waffle_hub/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-07-17 01:46:18.110918 waffle_hub-0.2.6/waffle_hub/dataset/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       53 2023-06-12 07:00:05.000000 waffle_hub-0.2.6/waffle_hub/dataset/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-07-17 01:46:18.110918 waffle_hub-0.2.6/waffle_hub/dataset/adapter/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      419 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/waffle_hub/dataset/adapter/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     7146 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/waffle_hub/dataset/adapter/autocare_dlt.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     6516 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/waffle_hub/dataset/adapter/coco.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     9006 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/waffle_hub/dataset/adapter/transformers.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    14273 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/waffle_hub/dataset/adapter/yolo.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      633 2023-06-16 03:34:36.000000 waffle_hub-0.2.6/waffle_hub/dataset/cli.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    50432 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/waffle_hub/dataset/dataset.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-07-17 01:46:18.110918 waffle_hub-0.2.6/waffle_hub/experimental/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:00:05.000000 waffle_hub-0.2.6/waffle_hub/experimental/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-07-17 01:46:18.110918 waffle_hub-0.2.6/waffle_hub/experimental/auto_label/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:00:05.000000 waffle_hub-0.2.6/waffle_hub/experimental/auto_label/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     8261 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/waffle_hub/experimental/auto_label/grounding_dino.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2986 2023-06-12 07:00:05.000000 waffle_hub-0.2.6/waffle_hub/experimental/serve.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-07-17 01:46:18.110918 waffle_hub-0.2.6/waffle_hub/hub/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       39 2023-06-16 03:34:36.000000 waffle_hub-0.2.6/waffle_hub/hub/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-07-17 01:46:18.110918 waffle_hub-0.2.6/waffle_hub/hub/adapter/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:00:05.000000 waffle_hub-0.2.6/waffle_hub/hub/adapter/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-07-17 01:46:18.110918 waffle_hub-0.2.6/waffle_hub/hub/adapter/autocare_dlt/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       75 2023-06-12 07:00:05.000000 waffle_hub-0.2.6/waffle_hub/hub/adapter/autocare_dlt/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    10199 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/waffle_hub/hub/adapter/autocare_dlt/autocare_dlt_hub.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     4515 2023-06-24 03:11:53.000000 waffle_hub-0.2.6/waffle_hub/hub/adapter/autocare_dlt/config.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-07-17 01:46:18.110918 waffle_hub-0.2.6/waffle_hub/hub/adapter/autocare_dlt/configs/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      129 2023-06-12 07:00:05.000000 waffle_hub-0.2.6/waffle_hub/hub/adapter/autocare_dlt/configs/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1913 2023-06-12 07:00:05.000000 waffle_hub-0.2.6/waffle_hub/hub/adapter/autocare_dlt/configs/data_cfg.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     5446 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/waffle_hub/hub/adapter/autocare_dlt/configs/model_cfg.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-07-17 01:46:18.110918 waffle_hub-0.2.6/waffle_hub/hub/adapter/transformers/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       77 2023-06-12 07:51:09.000000 waffle_hub-0.2.6/waffle_hub/hub/adapter/transformers/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2220 2023-06-24 03:11:53.000000 waffle_hub-0.2.6/waffle_hub/hub/adapter/transformers/config.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     9156 2023-06-24 03:11:53.000000 waffle_hub-0.2.6/waffle_hub/hub/adapter/transformers/train_input_helper.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    10543 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/waffle_hub/hub/adapter/transformers/transformers_hub.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-07-17 01:46:18.110918 waffle_hub-0.2.6/waffle_hub/hub/adapter/ultralytics/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       74 2023-06-12 07:00:05.000000 waffle_hub-0.2.6/waffle_hub/hub/adapter/ultralytics/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     6999 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/waffle_hub/hub/adapter/ultralytics/config.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    13208 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      585 2023-06-16 03:34:36.000000 waffle_hub-0.2.6/waffle_hub/hub/cli.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    54492 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/waffle_hub/hub/hub.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-07-17 01:46:18.110918 waffle_hub-0.2.6/waffle_hub/hub/model/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:00:05.000000 waffle_hub-0.2.6/waffle_hub/hub/model/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    13900 2023-06-24 03:11:53.000000 waffle_hub-0.2.6/waffle_hub/hub/model/wrapper.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-07-17 01:46:18.110918 waffle_hub-0.2.6/waffle_hub/schema/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      345 2023-06-12 07:00:05.000000 waffle_hub-0.2.6/waffle_hub/schema/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1236 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/waffle_hub/schema/base_schema.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1731 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/waffle_hub/schema/configs.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      871 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/waffle_hub/schema/data.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      378 2023-06-12 07:51:09.000000 waffle_hub-0.2.6/waffle_hub/schema/evaluate.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-07-17 01:46:18.110918 waffle_hub-0.2.6/waffle_hub/schema/fields/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      138 2023-06-12 07:00:05.000000 waffle_hub-0.2.6/waffle_hub/schema/fields/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    17259 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/waffle_hub/schema/fields/annotation.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1722 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/waffle_hub/schema/fields/base_field.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     7283 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/waffle_hub/schema/fields/category.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     3137 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/waffle_hub/schema/fields/image.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      537 2023-06-24 03:11:53.000000 waffle_hub-0.2.6/waffle_hub/schema/result.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-07-17 01:46:18.110918 waffle_hub-0.2.6/waffle_hub/utils/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:00:05.000000 waffle_hub-0.2.6/waffle_hub/utils/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     3462 2023-06-16 03:34:37.000000 waffle_hub-0.2.6/waffle_hub/utils/base_cli.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     3694 2023-06-12 07:00:05.000000 waffle_hub-0.2.6/waffle_hub/utils/callback.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1686 2023-06-12 07:00:05.000000 waffle_hub-0.2.6/waffle_hub/utils/conversion.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     5752 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/waffle_hub/utils/data.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     4200 2023-06-12 07:51:09.000000 waffle_hub-0.2.6/waffle_hub/utils/draw.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     4420 2023-06-12 07:51:09.000000 waffle_hub-0.2.6/waffle_hub/utils/evaluate.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     6049 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/waffle_hub/utils/metric_logger.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      631 2023-06-12 07:51:09.000000 waffle_hub-0.2.6/waffle_hub/utils/process.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-07-17 01:46:18.110918 waffle_hub-0.2.6/waffle_hub.egg-info/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     4422 2023-07-17 01:46:18.000000 waffle_hub-0.2.6/waffle_hub.egg-info/PKG-INFO
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2276 2023-07-17 01:46:18.000000 waffle_hub-0.2.6/waffle_hub.egg-info/SOURCES.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        1 2023-07-17 01:46:18.000000 waffle_hub-0.2.6/waffle_hub.egg-info/dependency_links.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      224 2023-07-17 01:46:18.000000 waffle_hub-0.2.6/waffle_hub.egg-info/entry_points.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      308 2023-07-17 01:46:18.000000 waffle_hub-0.2.6/waffle_hub.egg-info/requires.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       11 2023-07-17 01:46:18.000000 waffle_hub-0.2.6/waffle_hub.egg-info/top_level.txt
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-19 12:10:25.482363 waffle_hub-0.2.7/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)    35149 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/LICENSE
+-rw-r--r--   0 lhj       (1001) lhj       (1001)      138 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/MANIFEST.in
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     4395 2023-07-19 12:10:25.482363 waffle_hub-0.2.7/PKG-INFO
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     3314 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/README.md
+-rw-r--r--   0 lhj       (1001) lhj       (1001)      386 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/requirements.txt
+-rw-r--r--   0 lhj       (1001) lhj       (1001)       38 2023-07-19 12:10:25.482363 waffle_hub-0.2.7/setup.cfg
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     2935 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/setup.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-19 12:10:25.482363 waffle_hub-0.2.7/tests/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     8814 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/tests/test_cli.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)    18878 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/tests/test_dataset.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     4581 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/tests/test_ddp.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)    12951 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/tests/test_hub.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-19 12:10:25.482363 waffle_hub-0.2.7/waffle_hub/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     2292 2023-07-19 12:09:36.000000 waffle_hub-0.2.7/waffle_hub/__init__.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-19 12:10:25.482363 waffle_hub-0.2.7/waffle_hub/dataset/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)       53 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/dataset/__init__.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-19 12:10:25.482363 waffle_hub-0.2.7/waffle_hub/dataset/adapter/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)      419 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/dataset/adapter/__init__.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     7146 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/dataset/adapter/autocare_dlt.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     6516 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/dataset/adapter/coco.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     9006 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/dataset/adapter/transformers.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)    14273 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/dataset/adapter/yolo.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)      633 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/dataset/cli.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)    50432 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/dataset/dataset.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-19 12:10:25.482363 waffle_hub-0.2.7/waffle_hub/experimental/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)        0 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/experimental/__init__.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-19 12:10:25.482363 waffle_hub-0.2.7/waffle_hub/experimental/auto_label/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)        0 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/experimental/auto_label/__init__.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     8261 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/experimental/auto_label/grounding_dino.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     2986 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/experimental/serve.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-19 12:10:25.482363 waffle_hub-0.2.7/waffle_hub/hub/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)       39 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/hub/__init__.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-19 12:10:25.482363 waffle_hub-0.2.7/waffle_hub/hub/adapter/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)        0 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/hub/adapter/__init__.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-19 12:10:25.482363 waffle_hub-0.2.7/waffle_hub/hub/adapter/autocare_dlt/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)       75 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/hub/adapter/autocare_dlt/__init__.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)    10199 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/hub/adapter/autocare_dlt/autocare_dlt_hub.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     4515 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/hub/adapter/autocare_dlt/config.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-19 12:10:25.482363 waffle_hub-0.2.7/waffle_hub/hub/adapter/autocare_dlt/configs/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)      129 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/hub/adapter/autocare_dlt/configs/__init__.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     1913 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/hub/adapter/autocare_dlt/configs/data_cfg.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     5446 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/hub/adapter/autocare_dlt/configs/model_cfg.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-19 12:10:25.482363 waffle_hub-0.2.7/waffle_hub/hub/adapter/transformers/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)       77 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/hub/adapter/transformers/__init__.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     2220 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/hub/adapter/transformers/config.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     9156 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/hub/adapter/transformers/train_input_helper.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)    10543 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/hub/adapter/transformers/transformers_hub.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-19 12:10:25.482363 waffle_hub-0.2.7/waffle_hub/hub/adapter/ultralytics/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)       74 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/hub/adapter/ultralytics/__init__.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     6999 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/hub/adapter/ultralytics/config.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)    13208 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)      585 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/hub/cli.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)    57365 2023-07-19 12:09:24.000000 waffle_hub-0.2.7/waffle_hub/hub/hub.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-19 12:10:25.482363 waffle_hub-0.2.7/waffle_hub/hub/model/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)        0 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/hub/model/__init__.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)    13900 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/hub/model/wrapper.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-19 12:10:25.482363 waffle_hub-0.2.7/waffle_hub/schema/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)      345 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/schema/__init__.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     1236 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/schema/base_schema.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     1745 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/schema/configs.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)      954 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/schema/data.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)      378 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/schema/evaluate.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-19 12:10:25.482363 waffle_hub-0.2.7/waffle_hub/schema/fields/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)      138 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/schema/fields/__init__.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)    17259 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/schema/fields/annotation.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     1722 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/schema/fields/base_field.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     7283 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/schema/fields/category.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     3137 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/schema/fields/image.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)      537 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/schema/result.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-19 12:10:25.482363 waffle_hub-0.2.7/waffle_hub/utils/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)        0 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/utils/__init__.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     3462 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/utils/base_cli.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     3694 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/utils/callback.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     1686 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/utils/conversion.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     8726 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/utils/data.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     4200 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/utils/draw.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     4420 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/utils/evaluate.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     6049 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/utils/metric_logger.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)      631 2023-07-19 11:29:39.000000 waffle_hub-0.2.7/waffle_hub/utils/process.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-19 12:10:25.482363 waffle_hub-0.2.7/waffle_hub.egg-info/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     4395 2023-07-19 12:10:25.000000 waffle_hub-0.2.7/waffle_hub.egg-info/PKG-INFO
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     2276 2023-07-19 12:10:25.000000 waffle_hub-0.2.7/waffle_hub.egg-info/SOURCES.txt
+-rw-r--r--   0 lhj       (1001) lhj       (1001)        1 2023-07-19 12:10:25.000000 waffle_hub-0.2.7/waffle_hub.egg-info/dependency_links.txt
+-rw-r--r--   0 lhj       (1001) lhj       (1001)      224 2023-07-19 12:10:25.000000 waffle_hub-0.2.7/waffle_hub.egg-info/entry_points.txt
+-rw-r--r--   0 lhj       (1001) lhj       (1001)      308 2023-07-19 12:10:25.000000 waffle_hub-0.2.7/waffle_hub.egg-info/requires.txt
+-rw-r--r--   0 lhj       (1001) lhj       (1001)       11 2023-07-19 12:10:25.000000 waffle_hub-0.2.7/waffle_hub.egg-info/top_level.txt
```

### Comparing `waffle_hub-0.2.6/LICENSE` & `waffle_hub-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.6/PKG-INFO` & `waffle_hub-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waffle_hub
-Version: 0.2.6
+Version: 0.2.7
 Summary: Waffle hub
 Home-page: https://github.com/snuailab/waffle_hub
 Author: SNUAILAB
 Author-email: huijae.lee@snuailab.ai
 License: GPL-3.0
 Project-URL: Bug Reports, https://github.com/snuailab/waffle_hub/issues
 Project-URL: Source, https://github.com/snuailab/waffle_hub
@@ -97,12 +97,12 @@
 ## CLI
 ```bash
 wd sample --name mnist_classification --task classification
 wd split --name mnist_classification --train-ratio 0.8 --val-ratio 0.1 --test-ratio 0.1
 wd export --name mnist_classification --data-type YOLO
 
 wh new --name my_classifier --task classification --model-type yolov8 --model-size n --categories [1,2]
-wh train --name my_classifier --dataset-path datasets/mnist_classification/exports/YOLO --epochs 30 --batch-size 64 --image-size 64 --device cpu
+wh train --name my_classifier --dataset mnist_classification --epochs 30 --batch-size 64 --image-size 64 --device cpu
 wh inference --name my_classifier --source datasets/mnist_classification/exports/YOLO --draw --device cpu
 ```
 
 See our [documentation](https://snuailab.github.io/waffle/) for more information!
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: waffle_hub Version: 0.2.6 Summary: Waffle hub Home-
+Metadata-Version: 2.1 Name: waffle_hub Version: 0.2.7 Summary: Waffle hub Home-
 page: https://github.com/snuailab/waffle_hub Author: SNUAILAB Author-email:
 huijae.lee@snuailab.ai License: GPL-3.0 Project-URL: Bug Reports, https://
 github.com/snuailab/waffle_hub/issues Project-URL: Source, https://github.com/
 snuailab/waffle_hub Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLO,Ultralytics,SNUAILAB Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
@@ -48,12 +48,11 @@
 dataset.get_category_names(), ) hub.train( dataset = dataset, epochs = 30,
 batch_size = 64, image_size=64, device="cpu" ) hub.inference
 ( source=export_dir, draw=True, device="cpu" ) ``` ## CLI ```bash wd sample --
 name mnist_classification --task classification wd split --name
 mnist_classification --train-ratio 0.8 --val-ratio 0.1 --test-ratio 0.1 wd
 export --name mnist_classification --data-type YOLO wh new --name my_classifier
 --task classification --model-type yolov8 --model-size n --categories [1,2] wh
-train --name my_classifier --dataset-path datasets/mnist_classification/
-exports/YOLO --epochs 30 --batch-size 64 --image-size 64 --device cpu wh
-inference --name my_classifier --source datasets/mnist_classification/exports/
-YOLO --draw --device cpu ``` See our [documentation](https://
-snuailab.github.io/waffle/) for more information!
+train --name my_classifier --dataset mnist_classification --epochs 30 --batch-
+size 64 --image-size 64 --device cpu wh inference --name my_classifier --source
+datasets/mnist_classification/exports/YOLO --draw --device cpu ``` See our
+[documentation](https://snuailab.github.io/waffle/) for more information!
```

### Comparing `waffle_hub-0.2.6/README.md` & `waffle_hub-0.2.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -71,12 +71,12 @@
 ## CLI
 ```bash
 wd sample --name mnist_classification --task classification
 wd split --name mnist_classification --train-ratio 0.8 --val-ratio 0.1 --test-ratio 0.1
 wd export --name mnist_classification --data-type YOLO
 
 wh new --name my_classifier --task classification --model-type yolov8 --model-size n --categories [1,2]
-wh train --name my_classifier --dataset-path datasets/mnist_classification/exports/YOLO --epochs 30 --batch-size 64 --image-size 64 --device cpu
+wh train --name my_classifier --dataset mnist_classification --epochs 30 --batch-size 64 --image-size 64 --device cpu
 wh inference --name my_classifier --source datasets/mnist_classification/exports/YOLO --draw --device cpu
 ```
 
 See our [documentation](https://snuailab.github.io/waffle/) for more information!
```

#### html2text {}

```diff
@@ -33,12 +33,11 @@
 dataset.get_category_names(), ) hub.train( dataset = dataset, epochs = 30,
 batch_size = 64, image_size=64, device="cpu" ) hub.inference
 ( source=export_dir, draw=True, device="cpu" ) ``` ## CLI ```bash wd sample --
 name mnist_classification --task classification wd split --name
 mnist_classification --train-ratio 0.8 --val-ratio 0.1 --test-ratio 0.1 wd
 export --name mnist_classification --data-type YOLO wh new --name my_classifier
 --task classification --model-type yolov8 --model-size n --categories [1,2] wh
-train --name my_classifier --dataset-path datasets/mnist_classification/
-exports/YOLO --epochs 30 --batch-size 64 --image-size 64 --device cpu wh
-inference --name my_classifier --source datasets/mnist_classification/exports/
-YOLO --draw --device cpu ``` See our [documentation](https://
-snuailab.github.io/waffle/) for more information!
+train --name my_classifier --dataset mnist_classification --epochs 30 --batch-
+size 64 --image-size 64 --device cpu wh inference --name my_classifier --source
+datasets/mnist_classification/exports/YOLO --draw --device cpu ``` See our
+[documentation](https://snuailab.github.io/waffle/) for more information!
```

### Comparing `waffle_hub-0.2.6/setup.py` & `waffle_hub-0.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.6/tests/test_cli.py` & `waffle_hub-0.2.7/tests/test_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,15 +260,15 @@
     assert (test_dir / "hubs" / "test" / "artifacts").exists()
 
 
 def test_hub_inference(test_dir: Path):
     cmd = f'python -m waffle_hub.hub.cli inference \
         --root-dir {test_dir / "hubs"} \
         --name test \
-        --source {test_dir / "datasets" / "mnist" / "exports" / "YOLO" / "test" / "images" } \
+        --source {test_dir / "datasets" / "from_coco" / "raw"} \
         --confidence-threshold 0.25 \
         --device cpu \
         --workers 0 \
     '
     ret = run_cli(cmd)
     assert ret.returncode == 0
     assert (test_dir / "hubs" / "test" / "inferences").exists()
```

### Comparing `waffle_hub-0.2.6/tests/test_dataset.py` & `waffle_hub-0.2.7/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.6/tests/test_ddp.py` & `waffle_hub-0.2.7/tests/test_ddp.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.6/tests/test_hub.py` & `waffle_hub-0.2.7/tests/test_hub.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,15 +148,17 @@
     _export(hub, half=False, hold=hold)
     # _export(hub, half=True, hold=hold)  # cpu cannot be half
     _feature_extraction(hub, image_size)
     _benchmark(hub, image_size)
     _util(hub)
 
 
-def test_ultralytics_segmentation(instance_segmentation_dataset: Dataset, tmpdir: Path):
+def test_ultralytics_segmentation(
+    instance_segmentation_dataset: Dataset, tmpdir: Path, test_video_path: Path
+):
     image_size = 32
     dataset = instance_segmentation_dataset
 
     # test hub
     name = "test_seg"
     hub = Hub.new(
         name=name,
@@ -171,17 +173,20 @@
     hub: Hub = Hub.from_model_config(
         name=name + "_from_model_config",
         model_config_file=tmpdir / name / Hub.MODEL_CONFIG_FILE,
         root_dir=tmpdir,
     )
 
     _total(hub, dataset, image_size)
+    _inference(hub, test_video_path, hold=False)
 
 
-def test_ultralytics_object_detection(object_detection_dataset: Dataset, tmpdir: Path):
+def test_ultralytics_object_detection(
+    object_detection_dataset: Dataset, tmpdir: Path, test_video_path: Path
+):
     image_size = 32
     dataset = object_detection_dataset
 
     # test hub
     name = "test_det"
     hub = Hub.new(
         name=name,
@@ -196,14 +201,15 @@
     hub: Hub = Hub.from_model_config(
         name=name + "_from_model_config",
         model_config_file=tmpdir / name / Hub.MODEL_CONFIG_FILE,
         root_dir=tmpdir,
     )
 
     _total(hub, dataset, image_size)
+    _inference(hub, test_video_path, hold=False)
 
 
 def test_ultralytics_object_detection_advance_params(
     object_detection_dataset: Dataset, tmpdir: Path
 ):
     image_size = 32
     dataset = object_detection_dataset
@@ -236,15 +242,17 @@
     _total(hub, dataset, image_size, str(tmpdir / "adv.json"))
     hub.delete_artifact()
 
     with pytest.raises(ValueError):
         _total(hub, dataset, image_size, {"box": 4, "dummy_adv_param": 2})
 
 
-def test_ultralytics_classification(classification_dataset: Dataset, tmpdir: Path):
+def test_ultralytics_classification(
+    classification_dataset: Dataset, tmpdir: Path, test_video_path: Path
+):
     image_size = 32
     dataset = classification_dataset
 
     # test hub
     name = "test_cls"
     hub = Hub.new(
         name=name,
@@ -259,14 +267,15 @@
     hub: Hub = Hub.from_model_config(
         name=name + "_from_model_config",
         model_config_file=tmpdir / name / Hub.MODEL_CONFIG_FILE,
         root_dir=tmpdir,
     )
 
     _total(hub, dataset, image_size)
+    _inference(hub, test_video_path, hold=False)
 
 
 def test_transformers_object_detection(object_detection_dataset: Dataset, tmpdir: Path):
     image_size = 32
     dataset = object_detection_dataset
 
     # test hub
```

### Comparing `waffle_hub-0.2.6/waffle_hub/__init__.py` & `waffle_hub-0.2.7/waffle_hub/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.6"
+__version__ = "0.2.7"
 
 import enum
 from collections import OrderedDict
 
 BACKEND_MAP = OrderedDict(
     {
         "ultralytics": {
```

### Comparing `waffle_hub-0.2.6/waffle_hub/dataset/adapter/autocare_dlt.py` & `waffle_hub-0.2.7/waffle_hub/dataset/adapter/autocare_dlt.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.6/waffle_hub/dataset/adapter/coco.py` & `waffle_hub-0.2.7/waffle_hub/dataset/adapter/coco.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.6/waffle_hub/dataset/adapter/transformers.py` & `waffle_hub-0.2.7/waffle_hub/dataset/adapter/transformers.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.6/waffle_hub/dataset/adapter/yolo.py` & `waffle_hub-0.2.7/waffle_hub/dataset/adapter/yolo.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.6/waffle_hub/dataset/cli.py` & `waffle_hub-0.2.7/waffle_hub/dataset/cli.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.6/waffle_hub/dataset/dataset.py` & `waffle_hub-0.2.7/waffle_hub/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.6/waffle_hub/experimental/auto_label/grounding_dino.py` & `waffle_hub-0.2.7/waffle_hub/experimental/auto_label/grounding_dino.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.6/waffle_hub/experimental/serve.py` & `waffle_hub-0.2.7/waffle_hub/experimental/serve.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.6/waffle_hub/hub/adapter/autocare_dlt/autocare_dlt_hub.py` & `waffle_hub-0.2.7/waffle_hub/hub/adapter/autocare_dlt/autocare_dlt_hub.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.6/waffle_hub/hub/adapter/autocare_dlt/config.py` & `waffle_hub-0.2.7/waffle_hub/hub/adapter/autocare_dlt/config.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.6/waffle_hub/hub/adapter/autocare_dlt/configs/data_cfg.py` & `waffle_hub-0.2.7/waffle_hub/hub/adapter/autocare_dlt/configs/data_cfg.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.6/waffle_hub/hub/adapter/autocare_dlt/configs/model_cfg.py` & `waffle_hub-0.2.7/waffle_hub/hub/adapter/autocare_dlt/configs/model_cfg.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.6/waffle_hub/hub/adapter/transformers/config.py` & `waffle_hub-0.2.7/waffle_hub/hub/adapter/transformers/config.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.6/waffle_hub/hub/adapter/transformers/train_input_helper.py` & `waffle_hub-0.2.7/waffle_hub/hub/adapter/transformers/train_input_helper.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.6/waffle_hub/hub/adapter/transformers/transformers_hub.py` & `waffle_hub-0.2.7/waffle_hub/hub/adapter/transformers/transformers_hub.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.6/waffle_hub/hub/adapter/ultralytics/config.py` & `waffle_hub-0.2.7/waffle_hub/hub/adapter/ultralytics/config.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.6/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py` & `waffle_hub-0.2.7/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.6/waffle_hub/hub/cli.py` & `waffle_hub-0.2.7/waffle_hub/hub/cli.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.6/waffle_hub/hub/hub.py` & `waffle_hub-0.2.7/waffle_hub/hub/hub.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,15 +45,20 @@
 )
 from waffle_hub.utils.callback import (
     EvaluateCallback,
     ExportCallback,
     InferenceCallback,
     TrainCallback,
 )
-from waffle_hub.utils.data import ImageDataset, LabeledDataset, get_image_transform
+from waffle_hub.utils.data import (
+    IMAGE_EXTS,
+    VIDEO_EXTS,
+    get_dataset_class,
+    get_image_transform,
+)
 from waffle_hub.utils.draw import draw_results
 from waffle_hub.utils.evaluate import evaluate_function
 from waffle_hub.utils.metric_logger import MetricLogger
 
 logger = logging.getLogger(__name__)
 
 
@@ -996,14 +1001,15 @@
         ## overwrite train config with default config
         for k, v in cfg.to_dict().items():
             if v is None:
                 field_value = getattr(
                     self.DEFAULT_PARAMS[self.task][self.model_type][self.model_size], k
                 )
                 setattr(cfg, k, field_value)
+        cfg.image_size = cfg.image_size if isinstance(cfg.image_size, list) else [cfg.image_size, cfg.image_size]
 
         ## overwrite train advance config
         if cfg.advance_params:
             if isinstance(cfg.advance_params, (str, PurePath)):
                 # check if it is yaml or json
                 if Path(cfg.advance_params).exists():
                     if Path(cfg.advance_params).suffix in [".yaml", ".yml"]:
@@ -1044,31 +1050,26 @@
         return result
 
     # Evaluation Hook
     def get_model(self):
         raise NotImplementedError
 
     def before_evaluate(self, cfg: EvaluateConfig):
-        # overwrite training config
-        train_config = self.get_train_config()
-        if cfg.image_size is None:
-            cfg.image_size = train_config.image_size
-        if cfg.letter_box is None:
-            cfg.letter_box = train_config.letter_box
+        pass
 
     def on_evaluate_start(self, cfg: EvaluateConfig):
         pass
 
     def evaluating(self, cfg: EvaluateConfig, callback: EvaluateCallback) -> str:
         device = cfg.device
 
         model = self.get_model().to(device)
 
         dataset = Dataset.load(cfg.dataset_name, cfg.dataset_root_dir)
-        dataloader = LabeledDataset(
+        dataloader = get_dataset_class("dataset")(
             dataset,
             cfg.image_size,
             letter_box=cfg.letter_box,
             set_name=cfg.set_name,
         ).get_dataloader(cfg.batch_size, cfg.workers)
 
         result_parser = get_parser(self.task)(**cfg.to_dict(), categories=self.categories)
@@ -1193,19 +1194,26 @@
                     name=dataset.parts[-1], root_dir=dataset.parents[0].absolute()
                 )
             elif dataset in Dataset.get_dataset_list(dataset_root_dir):
                 dataset = Dataset.load(name=dataset, root_dir=dataset_root_dir)
             else:
                 raise FileNotFoundError(f"Dataset {dataset} is not exist.")
 
+        # overwrite training config
+        train_config = self.get_train_config()
+        if image_size is None:
+            image_size = train_config.image_size
+        if letter_box is None:
+            letter_box = train_config.letter_box
+
         cfg = EvaluateConfig(
             dataset_name=dataset.name,
             set_name=set_name,
             batch_size=batch_size,
-            image_size=image_size,
+            image_size=image_size if isinstance(image_size, list) else [image_size, image_size],
             letter_box=letter_box,
             confidence_threshold=confidence_threshold,
             iou_threshold=iou_threshold,
             half=half,
             workers=workers,
             device="cpu" if device == "cpu" else f"cuda:{device}",
             draw=draw,
@@ -1223,59 +1231,84 @@
             callback.register_thread(thread)
             callback.start()
 
         return result
 
     # inference hooks
     def before_inference(self, cfg: InferenceConfig):
-        # overwrite training config
-        train_config = self.get_train_config()
-        if cfg.image_size is None:
-            cfg.image_size = train_config.image_size
-        if cfg.letter_box is None:
-            cfg.letter_box = train_config.letter_box
+        pass
 
     def on_inference_start(self, cfg: InferenceConfig):
         pass
 
     def inferencing(self, cfg: InferenceConfig, callback: InferenceCallback) -> str:
         device = cfg.device
-
         model = self.get_model().to(device)
-        dataloader = ImageDataset(
-            cfg.source, cfg.image_size, letter_box=cfg.letter_box
-        ).get_dataloader(cfg.batch_size, cfg.workers)
-
         result_parser = get_parser(self.task)(**cfg.to_dict(), categories=self.categories)
 
+        if cfg.source_type == "image":
+            dataset = get_dataset_class(cfg.source_type)(
+                cfg.source, cfg.image_size, letter_box=cfg.letter_box, recursive=cfg.recursive
+            )
+            dataloader = dataset.get_dataloader(cfg.batch_size, cfg.workers)
+        elif cfg.source_type == "video":
+            dataset = get_dataset_class(cfg.source_type)(
+                cfg.source, cfg.image_size, letter_box=cfg.letter_box
+            )
+            dataloader = dataset.get_dataloader(cfg.batch_size, cfg.workers)
+        else:
+            raise ValueError(f"Invalid source type: {cfg.source_type}")
+
+        if cfg.draw and cfg.source_type == "video":
+            writer = None
+
         results = []
         callback._total_steps = len(dataloader) + 1
         for i, (images, image_infos) in tqdm.tqdm(
             enumerate(dataloader, start=1), total=len(dataloader)
         ):
             result_batch = model(images.to(device))
             result_batch = result_parser(result_batch, image_infos)
             for result, image_info in zip(result_batch, image_infos):
-                image_path = image_info.image_path
 
-                relpath = Path(image_path).relative_to(cfg.source)
-                results.append({str(relpath): [res.to_dict() for res in result]})
+                results.append({str(image_info.image_rel_path): [res.to_dict() for res in result]})
 
                 if cfg.draw:
                     draw = draw_results(
-                        image_path,
+                        image_info.ori_image,
                         result,
                         names=[x["name"] for x in self.categories],
                     )
-                    draw_path = self.draw_dir / relpath.with_suffix(".png")
+                    draw_path = self.draw_dir / Path(image_info.image_rel_path).with_suffix(".png")
                     io.make_directory(draw_path.parent)
                     cv2.imwrite(str(draw_path), draw)
 
+                if cfg.draw and cfg.source_type == "video":
+                    if writer is None:
+                        h, w = draw.shape[:2]
+                        writer = cv2.VideoWriter(
+                            str(self.inference_dir / Path(cfg.source).with_suffix(".mp4").name),
+                            cv2.VideoWriter_fourcc(*"mp4v"),
+                            dataset.fps,
+                            (w, h),
+                        )
+                    writer.write(draw)
+
+                if cfg.show:
+                    cv2.imshow("result", draw)
+                    cv2.waitKey(0)
+
             callback.update(i)
 
+        if cfg.draw and cfg.source_type == "video":
+            writer.release()
+
+        if cfg.show:
+            cv2.destroyAllWindows()
+
         io.save_json(
             results,
             self.inference_file,
             create_directory=True,
         )
 
     def on_inference_end(self, cfg: InferenceConfig):
@@ -1284,41 +1317,43 @@
     def after_inference(self, cfg: InferenceConfig, result: EvaluateResult):
         result.predictions = self.get_inference_result()
         if cfg.draw:
             result.draw_dir = self.draw_dir
 
     def inference(
         self,
-        source: str,
+        source: Union[str, Dataset],
         recursive: bool = True,
         image_size: Union[int, list[int]] = None,
         letter_box: bool = None,
         batch_size: int = 4,
         confidence_threshold: float = 0.25,
         iou_threshold: float = 0.5,
         half: bool = False,
         workers: int = 2,
         device: str = "0",
         draw: bool = False,
+        show: bool = False,
         hold: bool = True,
     ) -> InferenceResult:
         """Start Inference
 
         Args:
-            source (str): source directory
+            source (str): image directory or image path or video path.
             recursive (bool, optional): recursive. Defaults to True.
             image_size (Union[int, list[int]], optional): image size. None for using training config. Defaults to None.
             letter_box (bool, optional): letter box. None for using training config. Defaults to None.
             batch_size (int, optional): batch size. Defaults to 4.
             confidence_threshold (float, optional): confidence threshold. Defaults to 0.25.
             iou_threshold (float, optional): iou threshold. Defaults to 0.5.
             half (bool, optional): half. Defaults to False.
             workers (int, optional): workers. Defaults to 2.
             device (str, optional): device. "cpu" or "gpu_id". Defaults to "0".
             draw (bool, optional): draw. Defaults to False.
+            show (bool, optional): show. Defaults to False.
             hold (bool, optional): hold. Defaults to True.
 
 
         Raises:
             FileNotFoundError: if can not detect appropriate dataset.
             e: something gone wrong with ultralytics
 
@@ -1359,26 +1394,61 @@
             except Exception as e:
                 if self.inference_dir.exists():
                     io.remove_directory(self.inference_dir)
                 callback.force_finish()
                 callback.set_failed()
                 raise e
 
+        # image_dir, image_path, video_path, dataset_name, dataset
+        if isinstance(source, (str, Path)):
+            if Path(source).exists():
+                source = Path(source)
+                if source.is_dir():
+                    source = source.absolute()
+                    source_type = "image"
+                elif source.suffix in IMAGE_EXTS:
+                    source = [source.absolute()]
+                    source_type = "image"
+                elif source.suffix in VIDEO_EXTS:
+                    source = str(source.absolute())
+                    source_type = "video"
+                else:
+                    raise ValueError(
+                        f"Invalid source: {source}\n"
+                        + "Please use image directory or image path or video path."
+                    )
+            else:
+                raise FileNotFoundError(f"Source {source} is not exist.")
+        else:
+            raise ValueError(
+                f"Invalid source: {source}\n"
+                + "Please use image directory or image path or video path."
+            )
+
+        # overwrite training config
+        train_config = self.get_train_config()
+        if image_size is None:
+            image_size = train_config.image_size
+        if letter_box is None:
+            letter_box = train_config.letter_box
+
         cfg = InferenceConfig(
             source=source,
+            source_type=source_type,
             batch_size=batch_size,
             recursive=recursive,
-            image_size=image_size,
+            image_size=image_size if isinstance(image_size, list) else [image_size, image_size],
             letter_box=letter_box,
             confidence_threshold=confidence_threshold,
             iou_threshold=iou_threshold,
             half=half,
             workers=workers,
             device="cpu" if device == "cpu" else f"cuda:{device}",
-            draw=draw,
+            draw=draw or show,
+            show=show,
         )
 
         callback = InferenceCallback(100)  # dummy step
         result = InferenceResult()
         result.callback = callback
 
         if hold:
@@ -1388,19 +1458,15 @@
             callback.register_thread(thread)
             callback.start()
 
         return result
 
     # Export Hook
     def before_export(self, cfg: ExportConfig):
-
-        # overwrite training config
-        train_config = self.get_train_config()
-        if cfg.image_size is None:
-            cfg.image_size = train_config.image_size
+        pass
 
     def on_export_start(self, cfg: ExportConfig):
         pass
 
     def exporting(self, cfg: ExportConfig, callback: ExportCallback) -> str:
         image_size = cfg.image_size
         image_size = [image_size, image_size] if isinstance(image_size, int) else image_size
@@ -1493,16 +1559,21 @@
             except Exception as e:
                 if self.onnx_file.exists():
                     io.remove_file(self.onnx_file)
                 callback.force_finish()
                 callback.set_failed()
                 raise e
 
+        # overwrite training config
+        train_config = self.get_train_config()
+        if image_size is None:
+            image_size = train_config.image_size
+
         cfg = ExportConfig(
-            image_size=image_size,
+            image_size=image_size if isinstance(image_size, list) else [image_size, image_size],
             batch_size=batch_size,
             opset_version=opset_version,
             half=half,
             device="cpu" if device == "cpu" else f"cuda:{device}",
         )
 
         callback = ExportCallback(1)
```

### Comparing `waffle_hub-0.2.6/waffle_hub/hub/model/wrapper.py` & `waffle_hub-0.2.7/waffle_hub/hub/model/wrapper.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.6/waffle_hub/schema/base_schema.py` & `waffle_hub-0.2.7/waffle_hub/schema/base_schema.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.6/waffle_hub/schema/configs.py` & `waffle_hub-0.2.7/waffle_hub/schema/configs.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 @dataclass
 class TrainConfig(BaseSchema):
     dataset_path: str = None
     epochs: int = None
     batch_size: int = None
-    image_size: Union[int, list[int]] = None
+    image_size: list[int] = None
     learning_rate: float = None
     letter_box: bool = None
     pretrained_model: str = None
     device: str = None
     workers: int = None
     seed: int = None
     advance_params: dict = None
@@ -32,38 +32,40 @@
 
 
 @dataclass
 class EvaluateConfig(BaseSchema):
     dataset_name: str = None
     set_name: str = None
     batch_size: int = None
-    image_size: Union[int, list[int]] = None
+    image_size: list[int] = None
     letter_box: bool = None
     confidence_threshold: float = None
     iou_threshold: float = None
     half: bool = None
     workers: int = None
     device: str = None
     draw: bool = None
     dataset_root_dir: str = None
 
 
 @dataclass
 class InferenceConfig(BaseSchema):
     source: str = None
+    source_type: str = None
     batch_size: int = None
     recursive: bool = None
-    image_size: Union[int, list[int]] = None
+    image_size: list[int] = None
     letter_box: bool = None
     confidence_threshold: float = None
     iou_threshold: float = None
     half: bool = None
     workers: int = None
     device: str = None
     draw: bool = None
+    show: bool = None
 
 
 @dataclass
 class ExportConfig(BaseSchema):
     image_size: Union[int, list[int]] = None
     batch_size: int = None
     input_name: list[str] = None
```

### Comparing `waffle_hub-0.2.6/waffle_hub/schema/data.py` & `waffle_hub-0.2.7/waffle_hub/schema/data.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from dataclasses import dataclass
 
+import numpy as np
 from waffle_utils.log import datetime_now
 
 from waffle_hub.schema.base_schema import BaseSchema
 from waffle_hub.schema.fields import Category
 
 
 @dataclass
@@ -31,8 +32,10 @@
         ImageInfo: ImageInfo
     """
 
     ori_shape: list[int]
     new_shape: list[int]
     input_shape: list[int]
     pad: list[int]
+    ori_image: np.ndarray = None
     image_path: str = None
+    image_rel_path: str = None
```

### Comparing `waffle_hub-0.2.6/waffle_hub/schema/fields/annotation.py` & `waffle_hub-0.2.7/waffle_hub/schema/fields/annotation.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.6/waffle_hub/schema/fields/base_field.py` & `waffle_hub-0.2.7/waffle_hub/schema/fields/base_field.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.6/waffle_hub/schema/fields/category.py` & `waffle_hub-0.2.7/waffle_hub/schema/fields/category.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.6/waffle_hub/schema/fields/image.py` & `waffle_hub-0.2.7/waffle_hub/schema/fields/image.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.6/waffle_hub/schema/result.py` & `waffle_hub-0.2.7/waffle_hub/schema/result.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.6/waffle_hub/utils/base_cli.py` & `waffle_hub-0.2.7/waffle_hub/utils/base_cli.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.6/waffle_hub/utils/callback.py` & `waffle_hub-0.2.7/waffle_hub/utils/callback.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.6/waffle_hub/utils/conversion.py` & `waffle_hub-0.2.7/waffle_hub/utils/conversion.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.6/waffle_hub/utils/data.py` & `waffle_hub-0.2.7/waffle_hub/utils/data.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,62 @@
+import warnings
 from pathlib import Path
 from typing import Union
 
 import cv2
 import numpy as np
 import torch
 from natsort import natsorted
 from torchvision import transforms as T
 from waffle_utils.file import io
 
 from waffle_hub.dataset import Dataset
 from waffle_hub.schema.data import ImageInfo
 from waffle_hub.schema.fields import Annotation, Category, Image
 
+IMAGE_EXTS = [".png", ".jpg", ".jpeg", ".bmp", ".tif", ".tiff"]
+VIDEO_EXTS = [".mp4", ".avi", ".mov", ".mkv"]
+
 
 def get_images(d, recursive: bool = True) -> list[str]:
     exp = "**/*" if recursive else "*"
     image_paths = []
-    for ext in ["png", "jpg", "jpeg", "bmp", "tif", "tiff"]:
-        image_paths += list(Path(d).glob(exp.lower() + "." + ext))
-        image_paths += list(Path(d).glob(exp.upper() + "." + ext))
+    for ext in IMAGE_EXTS:
+        image_paths += list(Path(d).glob(exp.lower() + ext))
+        image_paths += list(Path(d).glob(exp.upper() + ext))
     return natsorted(
         list(
             set(
                 map(
                     str,
                     image_paths,
                 )
             )
         )
     )
 
 
+def get_videos(d, recursive: bool = True) -> list[str]:
+    exp = "**/*" if recursive else "*"
+    video_paths = []
+    for ext in VIDEO_EXTS:
+        video_paths += list(Path(d).glob(exp.lower() + ext))
+        video_paths += list(Path(d).glob(exp.upper() + ext))
+    return natsorted(
+        list(
+            set(
+                map(
+                    str,
+                    video_paths,
+                )
+            )
+        )
+    )
+
+
 def resize_image(
     image: np.ndarray, image_size: list[int], letter_box: bool = False
 ) -> list[np.ndarray, ImageInfo]:
     """Resize Image.
 
     Args:
         image (np.ndarray): opencv image.
@@ -65,95 +87,139 @@
             h_ = H
 
             total_pad = h_ - w_
             left = total_pad // 2
             right = total_pad - left
             top, bottom = 0, 0
 
-        image = cv2.resize(image, (w_, h_), interpolation=cv2.INTER_CUBIC)
-        image = cv2.copyMakeBorder(image, top, bottom, left, right, None, value=(114, 114, 114))
+        resized_image = cv2.resize(image, (w_, h_), interpolation=cv2.INTER_CUBIC)
+        resized_image = cv2.copyMakeBorder(
+            resized_image, top, bottom, left, right, None, value=(114, 114, 114)
+        )
 
     else:
         w_, h_ = W, H
         left, top = 0, 0
-        image = cv2.resize(image, (w_, h_), interpolation=cv2.INTER_CUBIC)
+        resized_image = cv2.resize(image, (w_, h_), interpolation=cv2.INTER_CUBIC)
 
-    return image, ImageInfo(
+    return resized_image, ImageInfo(
+        ori_image=cv2.cvtColor(image, cv2.COLOR_BGR2RGB),
         ori_shape=(w, h),
         new_shape=(w_, h_),
         input_shape=(W, H),
         pad=(left, top),
     )
 
 
 def get_image_transform(image_size: Union[int, list[int]], letter_box: bool = False):
-
-    if isinstance(image_size, int):
-        image_size = [image_size, image_size]
-
     def transform(image: Union[np.ndarray, str]) -> tuple[torch.Tensor, ImageInfo]:
         if isinstance(image, str):
             image = cv2.imread(image)
-        image = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
+            image = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
         image, image_info = resize_image(image, image_size, letter_box)
         return T.ToTensor()(image), image_info
 
     return transform
 
 
-class ImageDataset:
+def get_dataset_class(dataset_type: str):
+    if dataset_type == "image":
+        return ImageDataset
+    elif dataset_type == "video":
+        return VideoDataset
+    elif dataset_type == "dataset":
+        return LabeledDataset
+    else:
+        raise ValueError(f"Unknown dataset type: {dataset_type}")
+
+
+class BaseDataset:
+    def __init__(
+        self,
+        image_size: Union[int, list[int]],
+        letter_box: bool = False,
+    ):
+        if isinstance(image_size, int):
+            image_size = [image_size, image_size]
+
+        if len(image_size) != 2:
+            raise ValueError("image_size must be a int or list of int with length 2(width, height).")
+
+        self.image_size = image_size
+        self.letter_box = letter_box
+
+        self.transform = get_image_transform(self.image_size, self.letter_box)
+
+    def __len__(self):
+        raise NotImplementedError
+
+    def __getitem__(self, idx):
+        raise NotImplementedError
+
+    def collate_fn(self, batch):
+        raise NotImplementedError
+
+    def get_dataloader(self, batch_size: int = 4, num_workers: int = 0):
+        return torch.utils.data.DataLoader(
+            self,
+            batch_size,
+            num_workers=num_workers,
+            collate_fn=self.collate_fn,
+            shuffle=False,
+            drop_last=False,
+        )
+
+
+class ImageDataset(BaseDataset):
     def __init__(
         self,
         image_dir: str,
         image_size: Union[int, list[int]],
         letter_box: bool = False,
         recursive: bool = True,
+        **kwargs,
     ):
+        super().__init__(image_size, letter_box)
+
         self.image_dir = image_dir
         if Path(self.image_dir).is_file():
             self.image_paths = [self.image_dir]
+            self.image_root_dir = Path(self.image_dir).parent
         else:
             self.image_paths = get_images(self.image_dir, recursive=recursive)
-
-        self.transform = get_image_transform(image_size, letter_box)
+            self.image_root_dir = Path(self.image_dir)
 
     def __len__(self):
         return len(self.image_paths)
 
     def __getitem__(self, idx):
         image_path = self.image_paths[idx]
 
-        image, image_info = self.transform(image_path)
+        image_tensor, image_info = self.transform(image_path)
         image_info.image_path = image_path
+        image_info.image_rel_path = str(Path(image_path).relative_to(self.image_root_dir))
 
-        return image, image_info
+        return image_tensor, image_info
 
     def collate_fn(self, batch):
         images, infos = list(zip(*batch))
         return torch.stack(images, dim=0), infos
 
-    def get_dataloader(self, batch_size: int = 4, num_workers: int = 0):
-        return torch.utils.data.DataLoader(
-            self,
-            batch_size,
-            num_workers=num_workers,
-            collate_fn=self.collate_fn,
-            shuffle=False,
-            drop_last=False,
-        )
-
 
-class LabeledDataset:
+class LabeledDataset(BaseDataset):
     def __init__(
         self,
         dataset: Dataset,
         image_size: Union[int, list[int]],
         letter_box: bool = False,
         set_name: str = None,
+        **kwargs,
     ):
+        super().__init__(image_size, letter_box)
+
         self.dataset = dataset
         self.image_dir = dataset.raw_image_dir
         self.set_name = set_name
 
         if self.set_name == "train":
             set_file = self.dataset.train_set_file
         elif self.set_name == "val":
@@ -166,35 +232,64 @@
         self.images: list[Image] = self.dataset.get_images(
             io.load_json(set_file) if set_file else None
         )
         self.image_to_annotations: dict[int, list[Annotation]] = {
             image.image_id: self.dataset.get_annotations(image.image_id) for image in self.images
         }
 
-        self.transform = get_image_transform(image_size, letter_box)
-
     def __len__(self):
         return len(self.images)
 
     def __getitem__(self, idx):
         image = self.images[idx]
         image_path = str(self.image_dir / image.file_name)
         annotations: list[Annotation] = self.image_to_annotations[image.image_id]
 
-        image, image_info = self.transform(image_path)
+        image_tensor, image_info = self.transform(image_path)
         image_info.image_path = image_path
+        image_info.image_rel_path = image.file_name
 
-        return image, image_info, annotations
+        return image_tensor, image_info, annotations
 
     def collate_fn(self, batch):
         images, infos, annotations = list(zip(*batch))
         return torch.stack(images, dim=0), infos, annotations
 
-    def get_dataloader(self, batch_size: int = 4, num_workers: int = 0):
-        return torch.utils.data.DataLoader(
-            self,
-            batch_size,
-            num_workers=num_workers,
-            collate_fn=self.collate_fn,
-            shuffle=False,
-            drop_last=False,
-        )
+
+class VideoDataset(BaseDataset):
+    def __init__(
+        self,
+        video_path: str,
+        image_size: Union[int, list[int]],
+        letter_box: bool = False,
+        **kwargs,
+    ):
+        super().__init__(image_size, letter_box)
+
+        self.video_path = video_path
+        self.cap = cv2.VideoCapture(self.video_path)
+        self.frame_count = int(self.cap.get(cv2.CAP_PROP_FRAME_COUNT))
+        self.fps = round(self.cap.get(cv2.CAP_PROP_FPS))
+
+    def __len__(self):
+        return self.frame_count
+
+    def __getitem__(self, idx):
+        # self.cap.set(cv2.CAP_PROP_POS_FRAMES, idx)
+        ret, frame = self.cap.read()
+        if not ret:
+            raise ValueError(f"Failed to read frame {idx} from video {self.video_path}.")
+        image_tensor, image_info = self.transform(frame)
+        image_info.image_rel_path = f"{idx}.png"
+
+        return image_tensor, image_info
+
+    def collate_fn(self, batch):
+        images, infos = list(zip(*batch))
+        return torch.stack(images, dim=0), infos
+
+    def get_dataloader(self, batch_size: int = 1, num_workers: int = 0):
+        if batch_size > 1:
+            warnings.warn("batch_size > 1 is not supported for video dataset.")
+        if num_workers > 0:
+            warnings.warn("num_workers > 0 is not supported for video dataset.")
+        return super().get_dataloader(batch_size=1, num_workers=0)
```

### Comparing `waffle_hub-0.2.6/waffle_hub/utils/draw.py` & `waffle_hub-0.2.7/waffle_hub/utils/draw.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.6/waffle_hub/utils/evaluate.py` & `waffle_hub-0.2.7/waffle_hub/utils/evaluate.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.6/waffle_hub/utils/metric_logger.py` & `waffle_hub-0.2.7/waffle_hub/utils/metric_logger.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.6/waffle_hub/utils/process.py` & `waffle_hub-0.2.7/waffle_hub/utils/process.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.6/waffle_hub.egg-info/PKG-INFO` & `waffle_hub-0.2.7/waffle_hub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waffle-hub
-Version: 0.2.6
+Version: 0.2.7
 Summary: Waffle hub
 Home-page: https://github.com/snuailab/waffle_hub
 Author: SNUAILAB
 Author-email: huijae.lee@snuailab.ai
 License: GPL-3.0
 Project-URL: Bug Reports, https://github.com/snuailab/waffle_hub/issues
 Project-URL: Source, https://github.com/snuailab/waffle_hub
@@ -97,12 +97,12 @@
 ## CLI
 ```bash
 wd sample --name mnist_classification --task classification
 wd split --name mnist_classification --train-ratio 0.8 --val-ratio 0.1 --test-ratio 0.1
 wd export --name mnist_classification --data-type YOLO
 
 wh new --name my_classifier --task classification --model-type yolov8 --model-size n --categories [1,2]
-wh train --name my_classifier --dataset-path datasets/mnist_classification/exports/YOLO --epochs 30 --batch-size 64 --image-size 64 --device cpu
+wh train --name my_classifier --dataset mnist_classification --epochs 30 --batch-size 64 --image-size 64 --device cpu
 wh inference --name my_classifier --source datasets/mnist_classification/exports/YOLO --draw --device cpu
 ```
 
 See our [documentation](https://snuailab.github.io/waffle/) for more information!
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: waffle-hub Version: 0.2.6 Summary: Waffle hub Home-
+Metadata-Version: 2.1 Name: waffle-hub Version: 0.2.7 Summary: Waffle hub Home-
 page: https://github.com/snuailab/waffle_hub Author: SNUAILAB Author-email:
 huijae.lee@snuailab.ai License: GPL-3.0 Project-URL: Bug Reports, https://
 github.com/snuailab/waffle_hub/issues Project-URL: Source, https://github.com/
 snuailab/waffle_hub Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLO,Ultralytics,SNUAILAB Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
@@ -48,12 +48,11 @@
 dataset.get_category_names(), ) hub.train( dataset = dataset, epochs = 30,
 batch_size = 64, image_size=64, device="cpu" ) hub.inference
 ( source=export_dir, draw=True, device="cpu" ) ``` ## CLI ```bash wd sample --
 name mnist_classification --task classification wd split --name
 mnist_classification --train-ratio 0.8 --val-ratio 0.1 --test-ratio 0.1 wd
 export --name mnist_classification --data-type YOLO wh new --name my_classifier
 --task classification --model-type yolov8 --model-size n --categories [1,2] wh
-train --name my_classifier --dataset-path datasets/mnist_classification/
-exports/YOLO --epochs 30 --batch-size 64 --image-size 64 --device cpu wh
-inference --name my_classifier --source datasets/mnist_classification/exports/
-YOLO --draw --device cpu ``` See our [documentation](https://
-snuailab.github.io/waffle/) for more information!
+train --name my_classifier --dataset mnist_classification --epochs 30 --batch-
+size 64 --image-size 64 --device cpu wh inference --name my_classifier --source
+datasets/mnist_classification/exports/YOLO --draw --device cpu ``` See our
+[documentation](https://snuailab.github.io/waffle/) for more information!
```

### Comparing `waffle_hub-0.2.6/waffle_hub.egg-info/SOURCES.txt` & `waffle_hub-0.2.7/waffle_hub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

