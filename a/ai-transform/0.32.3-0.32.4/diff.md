# Comparing `tmp/ai_transform-0.32.3.tar.gz` & `tmp/ai_transform-0.32.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_transform-0.32.3.tar", last modified: Fri Jul 14 02:11:48 2023, max compression
+gzip compressed data, was "ai_transform-0.32.4.tar", last modified: Wed Jul 19 10:08:56 2023, max compression
```

## Comparing `ai_transform-0.32.3.tar` & `ai_transform-0.32.4.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:48.861410 ai_transform-0.32.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-07-14 02:11:28.000000 ai_transform-0.32.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-14 02:11:48.861410 ai_transform-0.32.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-07-14 02:11:28.000000 ai_transform-0.32.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:48.857410 ai_transform-0.32.3/ai_transform/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:48.857410 ai_transform-0.32.3/ai_transform/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29597 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/api/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/api/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/api/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/api/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:48.857410 ai_transform-0.32.3/ai_transform/components/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/components/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:48.857410 ai_transform-0.32.3/ai_transform/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    15129 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/dataset/field.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:48.857410 ai_transform-0.32.3/ai_transform/engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14965 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/engine/abstract_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/engine/dense_output_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/engine/in_memory_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/engine/multipass_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/engine/small_batch_stable_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/engine/stable_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:48.857410 ai_transform-0.32.3/ai_transform/operator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/operator/abstract_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/operator/dense_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:48.861410 ai_transform-0.32.3/ai_transform/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/utils/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/utils/document_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/utils/encode_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/utils/example_documents.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/utils/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/utils/keyphrase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:48.861410 ai_transform-0.32.3/ai_transform/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/workflow/abstract_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/workflow/context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-14 02:11:28.000000 ai_transform-0.32.3/ai_transform/workflow/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:48.857410 ai_transform-0.32.3/ai_transform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-14 02:11:48.000000 ai_transform-0.32.3/ai_transform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-14 02:11:48.000000 ai_transform-0.32.3/ai_transform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 02:11:48.000000 ai_transform-0.32.3/ai_transform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-14 02:11:48.000000 ai_transform-0.32.3/ai_transform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-14 02:11:48.000000 ai_transform-0.32.3/ai_transform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-14 02:11:28.000000 ai_transform-0.32.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 02:11:48.861410 ai_transform-0.32.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-14 02:11:28.000000 ai_transform-0.32.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:48.861410 ai_transform-0.32.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    16411 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:48.861410 ai_transform-0.32.3/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:48.861410 ai_transform-0.32.3/tests/core/test_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/core/test_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/core/test_api/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/core/test_api/test_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/core/test_api/test_keyphrase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/core/test_api/test_wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:48.861410 ai_transform-0.32.3/tests/core/test_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/core/test_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/core/test_dataset/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/core/test_dataset/test_field.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/core/test_dataset/test_keyphrase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:48.861410 ai_transform-0.32.3/tests/core/test_engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/core/test_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/core/test_engine/test_dense_output_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/core/test_engine/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/core/test_engine/test_engine_playground.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/core/test_engine/test_multipass_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/core/test_engine/test_stable_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:48.861410 ai_transform-0.32.3/tests/core/test_operator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/core/test_operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/core/test_operator/test_abstract_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/core/test_operator/test_document_diff.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:48.861410 ai_transform-0.32.3/tests/core/test_workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/core/test_workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/core/test_workflow/test_context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/core/test_workflow/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-14 02:11:28.000000 ai_transform-0.32.3/tests/test_connection_retry.py
+drwxrwxrwx   0        0        0        0 2023-07-19 10:08:56.023969 ai_transform-0.32.4/
+-rw-rw-rw-   0        0        0    11547 2023-07-19 09:56:09.000000 ai_transform-0.32.4/LICENSE
+-rw-rw-rw-   0        0        0      282 2023-07-19 10:08:56.022969 ai_transform-0.32.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3466 2023-07-19 09:56:09.000000 ai_transform-0.32.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-19 10:08:55.959388 ai_transform-0.32.4/ai_transform/
+-rw-rw-rw-   0        0        0      779 2023-07-19 10:08:44.000000 ai_transform-0.32.4/ai_transform/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 10:08:55.977388 ai_transform-0.32.4/ai_transform/api/
+-rw-rw-rw-   0        0        0        0 2023-07-19 09:56:09.000000 ai_transform-0.32.4/ai_transform/api/__init__.py
+-rw-rw-rw-   0        0        0    30422 2023-07-19 09:56:09.000000 ai_transform-0.32.4/ai_transform/api/api.py
+-rw-rw-rw-   0        0        0     4910 2023-07-19 09:56:09.000000 ai_transform-0.32.4/ai_transform/api/client.py
+-rw-rw-rw-   0        0        0      347 2023-07-19 09:56:09.000000 ai_transform-0.32.4/ai_transform/api/endpoints.py
+-rw-rw-rw-   0        0        0      820 2023-07-19 09:56:09.000000 ai_transform-0.32.4/ai_transform/api/helpers.py
+-rw-rw-rw-   0        0        0     3100 2023-07-19 09:56:09.000000 ai_transform-0.32.4/ai_transform/api/wrappers.py
+drwxrwxrwx   0        0        0        0 2023-07-19 10:08:55.979388 ai_transform-0.32.4/ai_transform/components/
+-rw-rw-rw-   0        0        0       50 2023-07-19 09:56:09.000000 ai_transform-0.32.4/ai_transform/components/__init__.py
+-rw-rw-rw-   0        0        0    12383 2023-07-19 09:56:09.000000 ai_transform-0.32.4/ai_transform/components/components.py
+-rw-rw-rw-   0        0        0     3899 2023-07-19 09:56:09.000000 ai_transform-0.32.4/ai_transform/config.py
+-rw-rw-rw-   0        0        0      157 2023-07-19 09:56:09.000000 ai_transform-0.32.4/ai_transform/constants.py
+drwxrwxrwx   0        0        0        0 2023-07-19 10:08:55.981388 ai_transform-0.32.4/ai_transform/dataset/
+-rw-rw-rw-   0        0        0        0 2023-07-19 09:56:09.000000 ai_transform-0.32.4/ai_transform/dataset/__init__.py
+-rw-rw-rw-   0        0        0    11652 2023-07-19 09:56:09.000000 ai_transform-0.32.4/ai_transform/dataset/dataset.py
+-rw-rw-rw-   0        0        0    15535 2023-07-19 09:56:09.000000 ai_transform-0.32.4/ai_transform/dataset/field.py
+drwxrwxrwx   0        0        0        0 2023-07-19 10:08:55.987388 ai_transform-0.32.4/ai_transform/engine/
+-rw-rw-rw-   0        0        0        0 2023-07-19 09:56:09.000000 ai_transform-0.32.4/ai_transform/engine/__init__.py
+-rw-rw-rw-   0        0        0    15374 2023-07-19 09:56:09.000000 ai_transform-0.32.4/ai_transform/engine/abstract_engine.py
+-rw-rw-rw-   0        0        0     3720 2023-07-19 09:56:09.000000 ai_transform-0.32.4/ai_transform/engine/dense_output_engine.py
+-rw-rw-rw-   0        0        0     1410 2023-07-19 09:56:09.000000 ai_transform-0.32.4/ai_transform/engine/in_memory_engine.py
+-rw-rw-rw-   0        0        0     4619 2023-07-19 09:56:09.000000 ai_transform-0.32.4/ai_transform/engine/multipass_engine.py
+-rw-rw-rw-   0        0        0     3407 2023-07-19 09:56:09.000000 ai_transform-0.32.4/ai_transform/engine/small_batch_stable_engine.py
+-rw-rw-rw-   0        0        0     3738 2023-07-19 09:56:09.000000 ai_transform-0.32.4/ai_transform/engine/stable_engine.py
+-rw-rw-rw-   0        0        0      857 2023-07-19 09:56:09.000000 ai_transform-0.32.4/ai_transform/errors.py
+-rw-rw-rw-   0        0        0     1584 2023-07-19 09:56:09.000000 ai_transform-0.32.4/ai_transform/logger.py
+drwxrwxrwx   0        0        0        0 2023-07-19 10:08:55.989962 ai_transform-0.32.4/ai_transform/operator/
+-rw-rw-rw-   0        0        0        0 2023-07-19 09:56:09.000000 ai_transform-0.32.4/ai_transform/operator/__init__.py
+-rw-rw-rw-   0        0        0     7593 2023-07-19 09:56:09.000000 ai_transform-0.32.4/ai_transform/operator/abstract_operator.py
+-rw-rw-rw-   0        0        0     1093 2023-07-19 09:56:09.000000 ai_transform-0.32.4/ai_transform/operator/dense_operator.py
+-rw-rw-rw-   0        0        0      573 2023-07-19 09:56:09.000000 ai_transform-0.32.4/ai_transform/timer.py
+-rw-rw-rw-   0        0        0      600 2023-07-19 09:56:09.000000 ai_transform-0.32.4/ai_transform/types.py
+drwxrwxrwx   0        0        0        0 2023-07-19 10:08:55.995969 ai_transform-0.32.4/ai_transform/utils/
+-rw-rw-rw-   0        0        0      242 2023-07-19 09:56:09.000000 ai_transform-0.32.4/ai_transform/utils/__init__.py
+-rw-rw-rw-   0        0        0     8518 2023-07-19 09:56:09.000000 ai_transform-0.32.4/ai_transform/utils/document.py
+-rw-rw-rw-   0        0        0     6180 2023-07-19 09:56:09.000000 ai_transform-0.32.4/ai_transform/utils/document_list.py
+-rw-rw-rw-   0        0        0      145 2023-07-19 09:56:09.000000 ai_transform-0.32.4/ai_transform/utils/encode_parameters.py
+-rw-rw-rw-   0        0        0     3835 2023-07-19 09:56:09.000000 ai_transform-0.32.4/ai_transform/utils/example_documents.py
+-rw-rw-rw-   0        0        0     3358 2023-07-19 09:56:09.000000 ai_transform-0.32.4/ai_transform/utils/json_encoder.py
+-rw-rw-rw-   0        0        0      969 2023-07-19 09:56:09.000000 ai_transform-0.32.4/ai_transform/utils/keyphrase.py
+drwxrwxrwx   0        0        0        0 2023-07-19 10:08:55.999969 ai_transform-0.32.4/ai_transform/workflow/
+-rw-rw-rw-   0        0        0       80 2023-07-19 09:56:09.000000 ai_transform-0.32.4/ai_transform/workflow/__init__.py
+-rw-rw-rw-   0        0        0     3792 2023-07-19 09:56:09.000000 ai_transform-0.32.4/ai_transform/workflow/abstract_workflow.py
+-rw-rw-rw-   0        0        0     8266 2023-07-19 09:56:09.000000 ai_transform-0.32.4/ai_transform/workflow/context_manager.py
+-rw-rw-rw-   0        0        0     3126 2023-07-19 09:56:09.000000 ai_transform-0.32.4/ai_transform/workflow/helpers.py
+drwxrwxrwx   0        0        0        0 2023-07-19 10:08:55.972389 ai_transform-0.32.4/ai_transform.egg-info/
+-rw-rw-rw-   0        0        0      282 2023-07-19 10:08:55.000000 ai_transform-0.32.4/ai_transform.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2488 2023-07-19 10:08:55.000000 ai_transform-0.32.4/ai_transform.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 10:08:55.000000 ai_transform-0.32.4/ai_transform.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      360 2023-07-19 10:08:55.000000 ai_transform-0.32.4/ai_transform.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-19 10:08:55.000000 ai_transform-0.32.4/ai_transform.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      134 2023-07-19 09:56:09.000000 ai_transform-0.32.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-19 10:08:56.023969 ai_transform-0.32.4/setup.cfg
+-rw-rw-rw-   0        0        0     1053 2023-07-19 10:08:44.000000 ai_transform-0.32.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 10:08:56.002969 ai_transform-0.32.4/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-19 09:56:09.000000 ai_transform-0.32.4/tests/__init__.py
+-rw-rw-rw-   0        0        0      315 2023-07-19 09:56:09.000000 ai_transform-0.32.4/tests/components.py
+-rw-rw-rw-   0        0        0    16892 2023-07-19 09:56:09.000000 ai_transform-0.32.4/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2023-07-19 10:08:56.003970 ai_transform-0.32.4/tests/core/
+-rw-rw-rw-   0        0        0        0 2023-07-19 09:56:09.000000 ai_transform-0.32.4/tests/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 10:08:56.008969 ai_transform-0.32.4/tests/core/test_api/
+-rw-rw-rw-   0        0        0        0 2023-07-19 09:56:09.000000 ai_transform-0.32.4/tests/core/test_api/__init__.py
+-rw-rw-rw-   0        0        0     2188 2023-07-19 09:56:09.000000 ai_transform-0.32.4/tests/core/test_api/test_client.py
+-rw-rw-rw-   0        0        0     1166 2023-07-19 09:56:09.000000 ai_transform-0.32.4/tests/core/test_api/test_endpoints.py
+-rw-rw-rw-   0        0        0     1032 2023-07-19 09:56:09.000000 ai_transform-0.32.4/tests/core/test_api/test_keyphrase.py
+-rw-rw-rw-   0        0        0     5549 2023-07-19 09:56:09.000000 ai_transform-0.32.4/tests/core/test_api/test_wrappers.py
+drwxrwxrwx   0        0        0        0 2023-07-19 10:08:56.011969 ai_transform-0.32.4/tests/core/test_dataset/
+-rw-rw-rw-   0        0        0        0 2023-07-19 09:56:09.000000 ai_transform-0.32.4/tests/core/test_dataset/__init__.py
+-rw-rw-rw-   0        0        0     6090 2023-07-19 09:56:09.000000 ai_transform-0.32.4/tests/core/test_dataset/test_dataset.py
+-rw-rw-rw-   0        0        0     2191 2023-07-19 09:56:09.000000 ai_transform-0.32.4/tests/core/test_dataset/test_field.py
+-rw-rw-rw-   0        0        0      980 2023-07-19 09:56:09.000000 ai_transform-0.32.4/tests/core/test_dataset/test_keyphrase.py
+drwxrwxrwx   0        0        0        0 2023-07-19 10:08:56.016969 ai_transform-0.32.4/tests/core/test_engine/
+-rw-rw-rw-   0        0        0        0 2023-07-19 09:56:09.000000 ai_transform-0.32.4/tests/core/test_engine/__init__.py
+-rw-rw-rw-   0        0        0     2681 2023-07-19 09:56:09.000000 ai_transform-0.32.4/tests/core/test_engine/test_dense_output_engine.py
+-rw-rw-rw-   0        0        0     2029 2023-07-19 09:56:09.000000 ai_transform-0.32.4/tests/core/test_engine/test_engine.py
+-rw-rw-rw-   0        0        0      718 2023-07-19 09:56:09.000000 ai_transform-0.32.4/tests/core/test_engine/test_engine_playground.py
+-rw-rw-rw-   0        0        0     3405 2023-07-19 09:56:09.000000 ai_transform-0.32.4/tests/core/test_engine/test_multipass_engine.py
+-rw-rw-rw-   0        0        0     3525 2023-07-19 09:56:09.000000 ai_transform-0.32.4/tests/core/test_engine/test_stable_engine.py
+drwxrwxrwx   0        0        0        0 2023-07-19 10:08:56.019969 ai_transform-0.32.4/tests/core/test_operator/
+-rw-rw-rw-   0        0        0        0 2023-07-19 09:56:09.000000 ai_transform-0.32.4/tests/core/test_operator/__init__.py
+-rw-rw-rw-   0        0        0      647 2023-07-19 09:56:09.000000 ai_transform-0.32.4/tests/core/test_operator/test_abstract_operator.py
+-rw-rw-rw-   0        0        0     2206 2023-07-19 09:56:09.000000 ai_transform-0.32.4/tests/core/test_operator/test_document_diff.py
+drwxrwxrwx   0        0        0        0 2023-07-19 10:08:56.021969 ai_transform-0.32.4/tests/core/test_workflow/
+-rw-rw-rw-   0        0        0        0 2023-07-19 09:56:09.000000 ai_transform-0.32.4/tests/core/test_workflow/__init__.py
+-rw-rw-rw-   0        0        0     1201 2023-07-19 09:56:09.000000 ai_transform-0.32.4/tests/core/test_workflow/test_context_manager.py
+-rw-rw-rw-   0        0        0     3425 2023-07-19 09:56:09.000000 ai_transform-0.32.4/tests/core/test_workflow/test_workflow.py
+-rw-rw-rw-   0        0        0      476 2023-07-19 09:56:09.000000 ai_transform-0.32.4/tests/test_connection_retry.py
```

### Comparing `ai_transform-0.32.3/LICENSE` & `ai_transform-0.32.4/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright 2022 Onsearch Pty LTD
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright 2022 Onsearch Pty LTD
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `ai_transform-0.32.3/README.md` & `ai_transform-0.32.4/README.md`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,118 +1,118 @@
-# AI Transform
-
-Below is a hierarchy diagram for all the moving parts of a workflow.
-
-![hierarchy](hierarchy.png "Hierarchy")
-
-## 🛠️ Installation
-
-Fresh install
-
-```{bash}
-pip install ai-transform
-```
-
-to upgrade to the latest version
-
-```{bash}
-pip install --upgrade ai-transform
-```
-
-## 🏃Quickstart
-
-To get started, please refer to the example scripts in `scripts/`
-
-```python
-
-import random
-from ai_transform.api.client import Client
-from ai_transform.engine.stable_engine import StableEngine
-from ai_transform.workflow.helpers import decode_workflow_token
-from ai_transform.workflow import Workflow
-from ai_transform.operator.abstract_operator import AbstractOperator
-from ai_transform.utils.random import Document
-
-class RandomOperator(AbstractOperator):
-    def __init__(self, upper_bound: int=10):
-        self.upper_bound = upper_bound
-
-    def transform(self, documents):
-        for d in documents:
-            d['random_number'] = random.randint(0, self.upper_bound)
-
-
-client = Client()
-ds = client.Dataset("sample_dataset")
-operator = RandomOperator()
-
-engine = StableEngine(
-    dataset=ds,
-    operator=operator,
-    chunksize=10,
-    filters=[],
-)
-workflow = Workflow(engine)
-
-workflow.run()
-```
-
-## Workflow IDs and Job IDs
-
-Workflows have Workflow IDs such as sentiment  - for example:
-sentiment.py is called sentiment and this is how the frontend triggers it.
-Workflow Name is what we call the workflow like Extract Sentiment .
-Each instance of a workflow is a job and these have job_id so we can track their status.
-
-## Engine Selection
-
-### StableEngine
-
-This the safest and most basic way to write a workflow. This engine will pull `chunksize`
-number of documents, transform them according to the transform method in the respective operator
-and then insert them. If `chunksize=None`, the engine will attempt to pull the entire dataset
-transform the entire dataset in one go, and then reinsert all the documents at once. Batching is limited
-by the value provided to `chunksize`.
-
-### InMemoryEngine
-
-This Engine is intended to be used when operations are done on the whole dataset at once.
-The advantage this has over `StableEngine` with `chunksize=None` is that the pulling and
-pushing documents is done in batch, but the operation is done in bulk. With `StableEngine`,
-this would have involved extremely large API calls with larger datasets.
-
-### Polling
-
-Sometimes you will want to wait until the Relevance AI
-schema updates before proceeding to the next step. For more information - look at `workflow/helpers.py` file.
-
-```{python}
-
-poll_until_health_updates_with_input_field(
-    dataset=dataset,
-    input_field=...,
-    output_field=...,
-    minimum_coverage=0.95,
-    sleep_timer=10
-)
-```
-
-
-### How to release
-
-To cut a release, go to "Releases" and create a new version from `main` branch.
-
-### Architecture Decisions
-
-#### Pydantic
-
-There are a few reasons for the pydantic choice:
-- good strong validation
-- outputs nicely to OpenAPI which allows us to generate workflow docs automatically in future for Workflow APIs
-- used in FastAPI stack so workflows can also be FastAPI compatible in the future.
-
-### For Developers
-
-When developing with Workflows Core, we have the following philosophies:
-
-- Support for only 1 entrypoint where possible
-- Readable comments for anything that others might not understand
+# AI Transform
+
+Below is a hierarchy diagram for all the moving parts of a workflow.
+
+![hierarchy](hierarchy.png "Hierarchy")
+
+## 🛠️ Installation
+
+Fresh install
+
+```{bash}
+pip install ai-transform
+```
+
+to upgrade to the latest version
+
+```{bash}
+pip install --upgrade ai-transform
+```
+
+## 🏃Quickstart
+
+To get started, please refer to the example scripts in `scripts/`
+
+```python
+
+import random
+from ai_transform.api.client import Client
+from ai_transform.engine.stable_engine import StableEngine
+from ai_transform.workflow.helpers import decode_workflow_token
+from ai_transform.workflow import Workflow
+from ai_transform.operator.abstract_operator import AbstractOperator
+from ai_transform.utils.random import Document
+
+class RandomOperator(AbstractOperator):
+    def __init__(self, upper_bound: int=10):
+        self.upper_bound = upper_bound
+
+    def transform(self, documents):
+        for d in documents:
+            d['random_number'] = random.randint(0, self.upper_bound)
+
+
+client = Client()
+ds = client.Dataset("sample_dataset")
+operator = RandomOperator()
+
+engine = StableEngine(
+    dataset=ds,
+    operator=operator,
+    chunksize=10,
+    filters=[],
+)
+workflow = Workflow(engine)
+
+workflow.run()
+```
+
+## Workflow IDs and Job IDs
+
+Workflows have Workflow IDs such as sentiment  - for example:
+sentiment.py is called sentiment and this is how the frontend triggers it.
+Workflow Name is what we call the workflow like Extract Sentiment .
+Each instance of a workflow is a job and these have job_id so we can track their status.
+
+## Engine Selection
+
+### StableEngine
+
+This the safest and most basic way to write a workflow. This engine will pull `chunksize`
+number of documents, transform them according to the transform method in the respective operator
+and then insert them. If `chunksize=None`, the engine will attempt to pull the entire dataset
+transform the entire dataset in one go, and then reinsert all the documents at once. Batching is limited
+by the value provided to `chunksize`.
+
+### InMemoryEngine
+
+This Engine is intended to be used when operations are done on the whole dataset at once.
+The advantage this has over `StableEngine` with `chunksize=None` is that the pulling and
+pushing documents is done in batch, but the operation is done in bulk. With `StableEngine`,
+this would have involved extremely large API calls with larger datasets.
+
+### Polling
+
+Sometimes you will want to wait until the Relevance AI
+schema updates before proceeding to the next step. For more information - look at `workflow/helpers.py` file.
+
+```{python}
+
+poll_until_health_updates_with_input_field(
+    dataset=dataset,
+    input_field=...,
+    output_field=...,
+    minimum_coverage=0.95,
+    sleep_timer=10
+)
+```
+
+
+### How to release
+
+To cut a release, go to "Releases" and create a new version from `main` branch.
+
+### Architecture Decisions
+
+#### Pydantic
+
+There are a few reasons for the pydantic choice:
+- good strong validation
+- outputs nicely to OpenAPI which allows us to generate workflow docs automatically in future for Workflow APIs
+- used in FastAPI stack so workflows can also be FastAPI compatible in the future.
+
+### For Developers
+
+When developing with Workflows Core, we have the following philosophies:
+
+- Support for only 1 entrypoint where possible
+- Readable comments for anything that others might not understand
```

### Comparing `ai_transform-0.32.3/ai_transform/__init__.py` & `ai_transform-0.32.4/ai_transform/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-__version__ = "0.32.3"
-
-from ai_transform.timer import Timer
-
-_TIMER = Timer()
-_TIMER.start()
-
-
-def add_config_paths(verbose: bool = False):
-    # Support all config paths
-    # Add config paths
-    import sys
-    import os
-
-    # Append the current files.
-    sys.path.append(".")
-    script_path = os.environ.get("script_path", "")
-    efs_mount_path = os.environ.get("EFS_MOUNT_PATH")
-    workflows_version = os.environ.get("WORKFLOWS_VERSION")
-    path = script_path.replace("/main.py", "")
-    main_path = f"{efs_mount_path}/scripts/{workflows_version}/{path}"
-    if verbose:
-        print(main_path)
-    if os.path.exists(main_path):
-        sys.path.append(main_path)
-    if verbose:
-        print(f"paths: {sys.path}")
-
-
-add_config_paths()
+__version__ = "0.32.4"
+
+from ai_transform.timer import Timer
+
+_TIMER = Timer()
+_TIMER.start()
+
+
+def add_config_paths(verbose: bool = False):
+    # Support all config paths
+    # Add config paths
+    import sys
+    import os
+
+    # Append the current files.
+    sys.path.append(".")
+    script_path = os.environ.get("script_path", "")
+    efs_mount_path = os.environ.get("EFS_MOUNT_PATH")
+    workflows_version = os.environ.get("WORKFLOWS_VERSION")
+    path = script_path.replace("/main.py", "")
+    main_path = f"{efs_mount_path}/scripts/{workflows_version}/{path}"
+    if verbose:
+        print(main_path)
+    if os.path.exists(main_path):
+        sys.path.append(main_path)
+    if verbose:
+        print(f"paths: {sys.path}")
+
+
+add_config_paths()
```

### Comparing `ai_transform-0.32.3/ai_transform/api/api.py` & `ai_transform-0.32.4/ai_transform/api/api.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,825 +1,825 @@
-import os
-import time
-import uuid
-import logging
-import requests
-
-from requests.models import Response
-from functools import wraps
-
-from typing import Any, Dict, List, Optional, Literal, Callable
-
-from ai_transform.logger import format_logging_info
-from ai_transform.utils import document
-from ai_transform.types import Credentials, FieldTransformer, Filter, Schema
-from ai_transform.api.wrappers import request_wrapper
-
-from ai_transform import __version__
-from ai_transform.logger import ic
-
-
-LOG_REQUESTS = bool(os.getenv("LOG_REQUESTS"))
-if LOG_REQUESTS:
-    # Get the current Unix timestamp as a string
-    timestamp = str(int(time.time()))
-
-    logging.basicConfig(
-        level=logging.DEBUG,
-        format="%(asctime)s - %(levelname)s - %(message)s",
-        handlers=[logging.FileHandler(f"{timestamp}_request_logs.log")],
-    )
-
-
-def to_curl(request: requests.PreparedRequest):
-    command = "curl -X {method} '{url}'".format(method=request.method, url=request.url)
-
-    for header, value in request.headers.items():
-        if header.lower() == "authorization":
-            value = "MASKED"
-        command += " -H '{header}: {value}'".format(header=header, value=value)
-
-    if request.body:
-        command += " -d '{data}'".format(data=request.body)
-
-    return command
-
-
-def log_request(request: requests.PreparedRequest):
-    curl_command = to_curl(request)
-    logging.debug(curl_command)
-
-
-def log_response(response: requests.Response):
-    logging.debug("Response Headers: %s", response.headers)
-    logging.debug("Response Content: %s\n", response.text)
-
-
-def get_response(response: requests.Response) -> Dict[str, Any]:
-    # get a json response
-    # if errors - print what the response contains
-    if response.status_code == 200:
-        try:
-            return response.json()
-        except Exception as e:
-            ic(e)
-            ic(format_logging_info({"x-trace-id": response.headers["x-trace-id"]}))
-            raise e
-    else:
-        datum = {"error": response.content.decode("utf-8")}
-        if "x-trace-id" in response.headers:
-            datum["x-trace-id"] = response.headers["x-trace-id"]
-
-        try:
-            # Log this somewhere if it errors
-            ic(format_logging_info(datum))
-        except Exception as no_content_e:
-            # in case there's no content
-            ic(no_content_e)
-            # we still want to raise the right error for retrying
-            # continue to raise exception so that any retry logic still holds
-            raise no_content_e
-
-
-# We implement retry as a function for several reasons
-# first - we can get a
-def retry(num_of_retries: int = 3, timeout: int = 30, retry_func: Callable = None):
-    """
-    Allows the function to retry upon failure.
-    Args:
-        num_of_retries: The number of times the function should retry
-        timeout: The number of seconds to wait between each retry
-    """
-
-    def _retry(func):
-        @wraps(func)
-        def function_wrapper(*args, **kwargs):
-            return request_wrapper(
-                func,
-                args,
-                kwargs,
-                num_retries=num_of_retries,
-                timeout=timeout,
-                exponential_backoff=2,
-                retry_func=retry_func,
-            )
-
-        return function_wrapper
-
-    return _retry
-
-
-class API:
-    def __init__(self, credentials: Credentials, job_id: str = None, name: str = None) -> None:
-        self._credentials = credentials
-        self._base_url = f"https://api-{self.credentials.region}.stack.tryrelevance.com/latest"
-        self._headers = dict(
-            Authorization=f"{self.credentials.project}:{self.credentials.api_key}", ai_transform_version=__version__
-        )
-        if job_id is not None:
-            self.headers.update(ai_transform_job_id=job_id)
-        if name is not None:
-            self.headers.update(ai_transform_name=name)
-
-        self.session = requests.Session()
-
-    @property
-    def credentials(self) -> Credentials:
-        return self._credentials
-
-    @property
-    def base_url(self) -> str:
-        return self._base_url
-
-    @property
-    def headers(self) -> Dict[str, str]:
-        return self._headers
-
-    @retry()
-    def _request(self, method: Literal["GET", "POST"], suffix: str, *args, **kwargs) -> Response:
-        request = requests.Request(method=method, url=self.base_url + suffix, headers=self.headers, *args, **kwargs)
-        prepared_request = request.prepare()
-
-        if LOG_REQUESTS:
-            log_request(prepared_request)
-
-        response = self.session.send(prepared_request)
-
-        if LOG_REQUESTS:
-            log_response(response)
-
-        return response
-
-    def get(self, suffix: str, *args, **kwargs) -> Response:
-        return self._request(method="GET", suffix=suffix, *args, **kwargs)
-
-    def post(self, suffix: str, *args, **kwargs) -> Response:
-        return self._request(method="POST", suffix=suffix, *args, **kwargs)
-
-    def _list_datasets(self):
-        response = self.get(suffix="/datasets/list")
-        return get_response(response)
-
-    def _create_dataset(
-        self, dataset_id: str, schema: Optional[Schema] = None, upsert: bool = True, expire: bool = False
-    ) -> Any:
-        obj = dict(id=dataset_id, upsert=upsert, expire=expire)
-        if schema:
-            obj["schema"] = schema
-        response = self.post(suffix=f"/datasets/create", json=obj)
-        return get_response(response)
-
-    def _delete_dataset(self, dataset_id: str) -> Any:
-        response = self.post(suffix=f"/datasets/{dataset_id}/delete")
-        return get_response(response)
-
-    def _get_schema(self, dataset_id: str) -> Schema:
-        response = self.get(suffix=f"/datasets/{dataset_id}/schema")
-        return get_response(response)
-
-    def _bulk_insert(
-        self,
-        dataset_id: str,
-        documents: List[document.Document],
-        insert_date: bool = True,
-        overwrite: bool = True,
-        update_schema: bool = True,
-        wait_for_update: bool = True,
-        field_transformers: List[FieldTransformer] = None,
-        ingest_in_background: bool = False,
-    ) -> Any:
-        response = self.post(
-            suffix=f"/datasets/{dataset_id}/documents/bulk_insert",
-            json=dict(
-                documents=documents,
-                insert_date=insert_date,
-                overwrite=overwrite,
-                update_schema=update_schema,
-                field_transformers=[] if field_transformers is None else field_transformers,
-                ingest_in_background=ingest_in_background,
-                wait_for_update=wait_for_update,
-            ),
-        )
-        return get_response(response)
-
-    def _bulk_update(
-        self,
-        dataset_id: str,
-        documents: List[document.Document],
-        insert_date: bool = True,
-        ingest_in_background: bool = True,
-        update_schema: bool = True,
-    ) -> Any:
-        response = self.post(
-            suffix=f"/datasets/{dataset_id}/documents/bulk_update",
-            json=dict(
-                updates=documents,
-                insert_date=insert_date,
-                ingest_in_background=ingest_in_background,
-                update_schema=update_schema,
-            ),
-        )
-        return get_response(response)
-
-    def _get_where(
-        self,
-        dataset_id: str,
-        page_size: int,
-        filters: Optional[List[Filter]] = None,
-        sort: Optional[list] = None,
-        select_fields: Optional[List[str]] = None,
-        include_vector: bool = True,
-        random_state: int = 0,
-        is_random: bool = False,
-        after_id: Optional[List] = None,
-        worker_number: int = 0,
-    ):
-        response = self.post(
-            suffix=f"/datasets/{dataset_id}/documents/get_where",
-            json=dict(
-                select_fields=[] if select_fields is None else select_fields,
-                page_size=min(9999, page_size),
-                sort=[] if sort is None else sort,
-                include_vector=include_vector,
-                filters=[] if filters is None else filters,
-                random_state=random_state,
-                is_random=is_random,
-                after_id=[] if after_id is None else after_id,
-                worker_number=worker_number,
-            ),
-        )
-        return get_response(response)
-
-    def _delete_where(self, dataset_id: str, filters: Optional[List[Filter]] = None):
-        response = self.post(
-            suffix=f"/datasets/{dataset_id}/documents/delete_where",
-            json=dict(filters=[] if filters is None else filters),
-        )
-        return get_response(response)
-
-    def _update_dataset_metadata(self, dataset_id: str, metadata: Dict[str, Any]):
-        """
-        Edit and add metadata about a dataset. Notably description, data source, etc
-        """
-        response = self.post(
-            suffix=f"/datasets/{dataset_id}/metadata", json=dict(dataset_id=dataset_id, metadata=metadata)
-        )
-        return get_response(response)
-
-    def _get_metadata(self, dataset_id: str) -> Dict[str, Any]:
-        response = self.get(suffix=f"/datasets/{dataset_id}/metadata")
-        return get_response(response)
-
-    def _insert_centroids(
-        self, dataset_id: str, cluster_centers: List[document.Document], vector_fields: List[str], alias: str
-    ):
-        response = self.post(
-            suffix=f"/datasets/{dataset_id}/cluster/centroids/insert",
-            json=dict(dataset_id=dataset_id, cluster_centers=cluster_centers, vector_fields=vector_fields, alias=alias),
-        )
-        return get_response(response)
-
-    def _get_centroids(
-        self,
-        dataset_id: str,
-        vector_fields: List[str],
-        alias: str,
-        page_size: int = 5,
-        page: int = 1,
-        cluster_ids: Optional[List] = None,
-        include_vector: bool = False,
-    ):
-        response = self.post(
-            suffix=f"/datasets/{dataset_id}/cluster/centroids/documents",
-            json=dict(
-                cluster_ids=[] if cluster_ids is None else cluster_ids,
-                vector_fields=vector_fields,
-                alias=alias,
-                page_size=min(9999, page_size),
-                page=page,
-                include_vector=include_vector,
-            ),
-        )
-        return get_response(response)
-
-    def _set_workflow_status(
-        self,
-        job_id: str,
-        workflow_name: str,
-        additional_information: str = "",
-        metadata: Dict[str, Any] = None,
-        status: str = "inprogress",
-        send_email: bool = True,
-        worker_number: int = None,
-        output: Dict[str, Any] = None,
-        email: Dict[str, Any] = None,
-        user_errors: str = None,
-    ):
-        # add edge case for API
-        if job_id == "":
-            return
-        if status not in {"inprogress", "complete", "failed"}:
-            raise ValueError("state should be one of `['inprogress', 'complete', 'failed']`")
-        parameters = dict(
-            status=status,
-            workflow_name=workflow_name,
-            additional_information=additional_information,
-            send_email=send_email,
-        )
-        # metadata can't be an empty dictionary as it overwrites
-        if metadata is not None and metadata != {}:
-            parameters["metadata"] = metadata
-
-        if worker_number is not None:
-            parameters["worker_number"] = worker_number
-
-        if output:
-            parameters["output"] = output
-
-        if user_errors:
-            parameters["user_errors"] = user_errors
-
-        if email:
-            # adding some assertions here for better developer experience
-            assert isinstance(email, dict)
-            assert "secondary_cta" in email
-            assert "url" in email["secondary_cta"]
-            assert "text" in email["secondary_cta"]
-
-            parameters["email"] = email
-
-        ic(parameters)
-
-        response = self.post(suffix=f"/workflows/{job_id}/status", json=parameters)
-        return get_response(response)
-
-    def _set_field_children(
-        self,
-        dataset_id: str,
-        fieldchildren_id: str,
-        field: str,
-        field_children: List[str],
-        metadata: Optional[Dict[str, Any]] = None,
-    ):
-        """
-        fieldchildren_id: The name of the workflow or operation
-
-        field: the input field of the operation
-
-        field_children: a list of output fields, taken from the most nested level
-        i.e. ["_sentiment_.text_field.alias"]
-
-        metadata: extra parameters associated with operation
-        i.e. n_clusters, n_init, softmax_temperature, etc...
-        """
-        params = dict(
-            field=field,
-            field_children=field_children,
-            category=fieldchildren_id,
-            metadata={} if metadata is None else metadata,
-        )
-        ic(params)
-        response = self.post(suffix=f"/datasets/{dataset_id}/field_children/{str(uuid.uuid4())}/update", json=params)
-        return get_response(response)
-
-    def _delete_field_children(self, dataset_id: str, fieldchildren_id: str):
-        response = self.post(suffix=f"/datasets/{dataset_id}/field_children/{fieldchildren_id}/delete")
-        return get_response(response)
-
-    def _list_field_children(self, dataset_id: str, page: int = 1, page_size: int = 10000, sort=None):
-        parameters = {"page": page, "page_size": page_size}
-
-        if sort:
-            parameters["sort"] = sort
-
-        response = self.post(suffix=f"/datasets/{dataset_id}/field_children/list", json=parameters)
-        return get_response(response)
-
-    def _get_health(self, dataset_id: str):
-        response = self.get(suffix=f"/datasets/{dataset_id}/monitor/health")
-        return get_response(response)
-
-    def _get_workflow_status(self, job_id: str):
-        response = self.post(suffix=f"/workflows/{job_id}/get")
-        return get_response(response)
-
-    def _update_workflow_metadata(self, job_id: str, metadata: Dict[str, Any]):
-        response = self.post(suffix=f"/workflows/{job_id}/metadata", json=dict(metadata=metadata))
-        return get_response(response)
-
-    def _get_file_upload_urls(self, dataset_id: str, files: List[str]):
-        response = self.post(suffix=f"/datasets/{dataset_id}/get_file_upload_urls", json=dict(files=files))
-        return get_response(response)
-
-    def _get_temp_file_upload_url(self, ext: str = None):
-        """Use this for temporary file uploads.
-        returns: {'download_url': ..., 'upload_url': ...}
-        """
-        body = {}
-        if ext is not None:
-            body["extension"] = ext
-        response = self.post(suffix=f"/services/get_temporary_file_upload_url", json=body)
-        return get_response(response)
-
-    def _upload_temporary_media(self, presigned_url: str, media_content: bytes):
-        return requests.put(presigned_url, headers={"x-amz-tagging": "Expire=true"}, data=media_content)
-
-    def _upload_media(self, presigned_url: str, media_content: bytes):
-        # dont use get response since response cannot be json decoded
-        return requests.put(presigned_url, data=media_content)
-
-    def _trigger(
-        self,
-        dataset_id: str,
-        params: dict,
-        workflow_id: str,
-        notebook_path: str = None,
-        instance_type: str = None,
-        host_type: str = None,
-        version: str = "production_version",
-    ):
-        """
-        trigger a workflow
-        """
-
-        data = dict(params=params, dataset_id=dataset_id, workflow_id=workflow_id, version=version)
-        if notebook_path is not None:
-            data["notebook_path"] = notebook_path
-        if instance_type is not None:
-            data["instance_type"] = instance_type
-        if host_type is not None:
-            data["host_type"] = host_type
-        return self.post(suffix=f"/workflows/trigger", json=data).json()
-
-    def _trigger_polling_workflow(
-        self,
-        dataset_id: str,
-        input_field: str,
-        output_field: str,
-        job_id: str,
-        workflow_name: str,
-        # set 95% coverage in case of edge cases like workflow only working
-        # on certain proportion of dataset
-        minimum_coverage: float = 0.95,
-        max_time: float = 120,
-        sleep_timer: float = 10,
-        workflow_id="poll",
-        version="production_version",
-    ):
-        """
-        Trigger the polling workflow
-        """
-        return self._trigger(
-            dataset_id=dataset_id,
-            params=dict(
-                dataset_id=dataset_id,
-                input_field=input_field,
-                output_field=output_field,
-                minimum_coverage=minimum_coverage,
-                max_time=max_time,
-                sleep_timer=sleep_timer,
-                parent_job_id=job_id,
-                parent_job_name=workflow_name,
-            ),
-            workflow_id=workflow_id,
-            version=version,
-            notebook_path="",
-            instance_type="batch",
-            host_type="batch",
-        )
-
-    def _update_workflow_progress(
-        self,
-        workflow_id: str,
-        worker_number: int = 0,
-        step: str = "Workflow",
-        n_processed: int = 0,
-        n_total: int = 0,
-        n_processed_pricing: Optional[int] = None,  # optional parameter
-    ):
-        """
-        Tracks Workflow Progress
-        """
-        if worker_number is None:
-            worker_number = 0
-
-        if n_processed_pricing:
-            params["n_processed_pricing "] = n_processed_pricing
-
-        params = dict(worker_number=worker_number, step=step, n_processed=n_processed, n_total=n_total)
-
-        ic("adding progress...")
-        ic(params)
-
-        response = self.post(suffix=f"/workflows/{workflow_id}/progress", json=params)
-        return get_response(response)
-
-    def _update_workflow_pricing(
-        self,
-        workflow_id: str,
-        worker_number: int = 0,
-        step: str = "Workflow",
-        n_processed_pricing: Optional[int] = None,
-    ):
-        """
-        Pricing endpoint is really part of progress endpoint but this is being
-        abstracted away for now due to the fact that the pricing is actually
-        something outside of progress.
-        """
-        if worker_number is None:
-            worker_number = 0
-
-        params = dict(worker_number=worker_number, step=step, n_processed_pricing=n_processed_pricing)
-        ic("adding progress...")
-        ic(params)
-        response = self.post(suffix=f"/workflows/{workflow_id}/progress", json=params)
-        return get_response(response)
-
-    def _append_tags(self, dataset_id: str, field: str, tags_to_add: List[str], filters: List[Filter]):
-        response = self.post(
-            suffix=f"/datasets/{dataset_id}/tags/append",
-            json=dict(field=field, tags_to_add=tags_to_add, filters=filters),
-        )
-        return get_response(response)
-
-    def _delete_tags(self, dataset_id: str, field: str, tags_to_delete: List[str], filters: List[Filter]):
-        response = self.post(
-            suffix=f"/datasets/{dataset_id}/tags/delete",
-            json=dict(field=field, tags_to_delete=tags_to_delete, filters=filters),
-        )
-        return get_response(response)
-
-    def _merge_tags(self, dataset_id: str, field: str, tags_to_merge: Dict[str, str], filters: List[Filter]):
-        response = self.post(
-            suffix=f"/datasets/{dataset_id}/tags/merge",
-            json=dict(field=field, tags_to_merge=tags_to_merge, filters=filters),
-        )
-        return get_response(response)
-
-    def _bulk_update_keyphrase(self, dataset_id: str, field: str, alias: str, updates: List):
-        """
-        Update keyphrases
-        """
-        response = self.post(
-            suffix=f"/datasets/{dataset_id}/fields/{field}.{alias}/keyphrase/bulk_update", json=dict(updates=updates)
-        )
-        return get_response(response)
-
-    def _bulk_delete_keyphrase(self, dataset_id: str, field: str, alias: str, ids: List[str]):
-        """
-        Update keyphrases
-        """
-        response = self.post(
-            suffix=f"/datasets/{dataset_id}/fields/{field}.{alias}/keyphrase/bulk_delete", json=dict(ids=ids)
-        )
-        return get_response(response)
-
-    def _get_keyphrase(self, dataset_id: str, field: str, alias: str, keyphrase_id: str):
-        """
-        Get keyphrase
-        """
-        if isinstance(keyphrase_id, str) and keyphrase_id != "":
-            response = self.get(suffix=f"/datasets/{dataset_id}/fields/{field}.{alias}/keyphrase/{keyphrase_id}/get")
-            return get_response(response)
-
-    def _delete_keyphrase(self, dataset_id: str, field: str, keyphrase_id: str, alias: str):
-        """
-        Deleting Keyphrases
-        """
-        response = self.post(suffix=f"/datasets/{dataset_id}/fields/{field}.{alias}/keyphrase/{keyphrase_id}/delete")
-        return get_response(response)
-
-    def _update_keyphrase(
-        self,
-        dataset_id: str,
-        field: str,
-        keyphrase_id: str,
-        alias: str,
-        keyphrase: str,
-        frequency: int = 0,
-        ancestors: list = None,
-        parents: list = None,
-        metadata: dict = None,
-        keyphrase_score: float = 0,
-        level: int = 0,
-    ):
-        # missing update contents here?
-        """
-        Update keyphrases
-        """
-        params = {
-            "_id": keyphrase_id,
-            "text": keyphrase,
-            "frequency": frequency,
-            "keyphrase_score": keyphrase_score,
-            "level": level,
-        }
-        if ancestors is not None:
-            params["ancestors"] = ancestors
-        if parents is not None:
-            params["parents"] = parents
-        if metadata is not None:
-            params["metadata"] = metadata
-        response = self.post(
-            suffix=f"/datasets/{dataset_id}/fields/{field}.{alias}/keyphrase/{keyphrase_id}/update", json=params
-        )
-        return get_response(response)
-
-    def _list_keyphrase(
-        self, dataset_id: str, field: str, alias: str, page: int = 0, page_size: int = 100, sort: list = None
-    ):
-        """
-        List keyphrases
-        """
-        params = {"page": page, "page_size": min(9999, page_size)}
-        if sort is not None:
-            params["sort"] = sort
-        response = self.post(suffix=f"/datasets/{dataset_id}/fields/{field}.{alias}/keyphrase/list", json=params)
-        return get_response(response)
-
-    def _facets(
-        self,
-        dataset_id: str,
-        fields: List[str],
-        data_interval: str = "monthly",
-        page_size: int = 1000,
-        asc: bool = False,
-    ):
-        response = self.post(
-            suffix=f"/datasets/{dataset_id}/facets",
-            json=dict(fields=fields, data_interval=data_interval, page_size=min(9999, page_size), asc=asc),
-        )
-        return get_response(response)
-
-    def _upsert_dataset_settings(self, dataset_id: str, settings: Optional[Dict[str, Any]] = None):
-        response = self.post(
-            suffix=f"/datasets/{dataset_id}/settings", json=dict(settings={} if settings is None else settings)
-        )
-        return get_response(response)
-
-    def _get_dataset_settings(self, dataset_id: str):
-        response = self.get(suffix=f"/datasets/{dataset_id}/settings")
-        return get_response(response)
-
-    def _create_deployable(self, dataset_id: Optional[str] = None, config: Optional[Dict[str, Any]] = None):
-        response = self.post(
-            suffix="/deployables/create",
-            json=dict(dataset_id=dataset_id, configuration={} if config is None else config),
-        )
-        return get_response(response)
-
-    def _share_dashboard(self, deployable_id: str):
-        response = self.post(suffix=f"/deployablegroups/{deployable_id}/share")
-        return get_response(response)
-
-    def _unshare_dashboard(self, deployable_id: str):
-        response = self.post(suffix=f"/deployablegroups/{deployable_id}/private")
-        return get_response(response)
-
-    def _get_deployable(self, deployable_id: str):
-        response = self.get(suffix=f"/deployables/{deployable_id}/get")
-        return get_response(response)
-
-    def _delete_deployable(self, deployable_id: str):
-        response = self.post(suffix=f"/deployables/delete", json=dict(id=deployable_id))
-        return get_response(response)
-
-    def _list_deployables(self, page_size: int):
-        response = self.get(suffix="/deployables/list", params=dict(page_size=min(9999, page_size)))
-        return get_response(response)
-
-    def _label_openai(
-        self,
-        dataset_id: str,
-        vector_field: str,
-        field: str,
-        alias: str,
-        question_suffix: str,
-        accuracy: int = 4,
-        cluster_ids: list = None,
-        dont_save_summaries: bool = True,
-        filters: list = None,
-    ):
-        params = {
-            "vector_fields": [vector_field],
-            # legacy parameter
-            "centroid_vector_fields": [vector_field],
-            "alias": alias,
-            "dataset_id": dataset_id,
-            "cluster_ids": cluster_ids,
-            "dont_save_summaries": dont_save_summaries,
-            "questions": [
-                {
-                    "cluster_ids": cluster_ids,
-                    "config": {
-                        "accuracy": accuracy,
-                        "examples": [],
-                        "field": field,
-                        "question_suffix": question_suffix,
-                    },
-                }
-            ],
-        }
-        if filters is not None:
-            params["filters"] = filters
-        response = self.post(suffix=f"/datasets/{dataset_id}/cluster/centroids/labels/create", json=params)
-        return get_response(response)
-
-    def _aggregate(
-        self,
-        dataset_id: str,
-        page_size: str = 20,
-        page: str = 1,
-        asc: str = False,
-        aggregation_query: Dict[str, List[Dict[str, Any]]] = None,
-        dataset_ids: List[str] = None,
-        filters: List[Filter] = None,
-    ):
-        response = self.post(
-            suffix=f"/datasets/{dataset_id}/aggregate",
-            json=dict(
-                filters=[] if filters is None else filters,
-                aggregation_query=aggregation_query,
-                page_size=min(9999, page_size),
-                page=page,
-                asc=asc,
-                dataset_ids=[] if dataset_ids is None else dataset_ids,
-                dataset_id=dataset_id,
-            ),
-        )
-        return get_response(response)
-
-    def _list_closest_to_center(
-        self,
-        dataset_id: str,
-        vector_fields: List[str],
-        alias: str,
-        approx: int = 0,
-        sum_fields: bool = True,
-        page: int = 1,
-        similarity_metric: str = "cosine",
-        min_score: float = 0,
-        include_vector: bool = False,
-        include_count: bool = True,
-        include_relevance: bool = False,
-        page_size: int = 20,
-        cluster_properties_filter: Dict[str, Any] = None,
-        cluster_ids: List[str] = None,
-        filters: List[Filter] = None,
-        select_fields: List[str] = None,
-    ):
-        response = self.post(
-            suffix=f"/datasets/{dataset_id}/cluster/centroids/list_closest_to_center",
-            json=dict(
-                vector_fields=vector_fields,
-                alias=alias,
-                approx=approx,
-                sum_fields=sum_fields,
-                page=page,
-                similarity_metric=similarity_metric,
-                min_score=min_score,
-                include_vector=include_vector,
-                include_count=include_count,
-                include_relevance=include_relevance,
-                page_size=min(9999, page_size),
-                cluster_properties_filter=cluster_properties_filter if cluster_properties_filter is not None else {},
-                filters=filters if filters is not None else [],
-                cluster_ids=cluster_ids if cluster_ids is not None else [],
-                select_fields=select_fields if select_fields is not None else [],
-            ),
-        )
-        return get_response(response)
-
-    def _list_project_keys(self):
-        response = self.get(suffix="/projects/keys/list")
-        return get_response(response)
-
-    def _get_project_key(self, key: str, token: str):
-        response = self.post(suffix="/projects/keys/get", json=dict(key=key, token=token))
-        return get_response(response)
-
-    def _set_project_key(self, key: str, value: str):
-        response = self.post(suffix="/projects/keys/set", json=dict(key=key, value=value))
-        return get_response(response)
-
-    def _delete_project_key(self, key: str):
-        response = self.post(suffix="/projects/keys/delete", json=dict(key=key))
-        return get_response(response)
-
-    def _update_version_aliases(self, development_version: str, production_version: str):
-        response = self.post(
-            suffix="/workflows/types/version_aliases/update",
-            json={"aliases": {"development_version": development_version, "production_version": production_version}},
-        )
-        return get_response(response)
-
-    def _openai_completion(
-        self, workflows_admin_token: str, body: dict, suffix: str = "/admin/proxy/openai/v1/completions"
-    ):
-        response = self.post(suffix=suffix, json={"token": workflows_admin_token, "body": body})
-        return get_response(response)
-
-    def _proxy_openai(self, workflows_admin_token: str, endpoint: str, body: dict):
-        response = self.post(
-            suffix="/admin/proxy/openai" + endpoint, json={"token": workflows_admin_token, "body": body}
-        )
-        return get_response(response)
+import os
+import time
+import uuid
+import logging
+import requests
+
+from requests.models import Response
+from functools import wraps
+
+from typing import Any, Dict, List, Optional, Literal, Callable
+
+from ai_transform.logger import format_logging_info
+from ai_transform.utils import document
+from ai_transform.types import Credentials, FieldTransformer, Filter, Schema
+from ai_transform.api.wrappers import request_wrapper
+
+from ai_transform import __version__
+from ai_transform.logger import ic
+
+
+LOG_REQUESTS = bool(os.getenv("LOG_REQUESTS"))
+if LOG_REQUESTS:
+    # Get the current Unix timestamp as a string
+    timestamp = str(int(time.time()))
+
+    logging.basicConfig(
+        level=logging.DEBUG,
+        format="%(asctime)s - %(levelname)s - %(message)s",
+        handlers=[logging.FileHandler(f"{timestamp}_request_logs.log")],
+    )
+
+
+def to_curl(request: requests.PreparedRequest):
+    command = "curl -X {method} '{url}'".format(method=request.method, url=request.url)
+
+    for header, value in request.headers.items():
+        if header.lower() == "authorization":
+            value = "MASKED"
+        command += " -H '{header}: {value}'".format(header=header, value=value)
+
+    if request.body:
+        command += " -d '{data}'".format(data=request.body)
+
+    return command
+
+
+def log_request(request: requests.PreparedRequest):
+    curl_command = to_curl(request)
+    logging.debug(curl_command)
+
+
+def log_response(response: requests.Response):
+    logging.debug("Response Headers: %s", response.headers)
+    logging.debug("Response Content: %s\n", response.text)
+
+
+def get_response(response: requests.Response) -> Dict[str, Any]:
+    # get a json response
+    # if errors - print what the response contains
+    if response.status_code == 200:
+        try:
+            return response.json()
+        except Exception as e:
+            ic(e)
+            ic(format_logging_info({"x-trace-id": response.headers["x-trace-id"]}))
+            raise e
+    else:
+        datum = {"error": response.content.decode("utf-8")}
+        if "x-trace-id" in response.headers:
+            datum["x-trace-id"] = response.headers["x-trace-id"]
+
+        try:
+            # Log this somewhere if it errors
+            ic(format_logging_info(datum))
+        except Exception as no_content_e:
+            # in case there's no content
+            ic(no_content_e)
+            # we still want to raise the right error for retrying
+            # continue to raise exception so that any retry logic still holds
+            raise no_content_e
+
+
+# We implement retry as a function for several reasons
+# first - we can get a
+def retry(num_of_retries: int = 3, timeout: int = 30, retry_func: Callable = None):
+    """
+    Allows the function to retry upon failure.
+    Args:
+        num_of_retries: The number of times the function should retry
+        timeout: The number of seconds to wait between each retry
+    """
+
+    def _retry(func):
+        @wraps(func)
+        def function_wrapper(*args, **kwargs):
+            return request_wrapper(
+                func,
+                args,
+                kwargs,
+                num_retries=num_of_retries,
+                timeout=timeout,
+                exponential_backoff=2,
+                retry_func=retry_func,
+            )
+
+        return function_wrapper
+
+    return _retry
+
+
+class API:
+    def __init__(self, credentials: Credentials, job_id: str = None, name: str = None) -> None:
+        self._credentials = credentials
+        self._base_url = f"https://api-{self.credentials.region}.stack.tryrelevance.com/latest"
+        self._headers = dict(
+            Authorization=f"{self.credentials.project}:{self.credentials.api_key}", ai_transform_version=__version__
+        )
+        if job_id is not None:
+            self.headers.update(ai_transform_job_id=job_id)
+        if name is not None:
+            self.headers.update(ai_transform_name=name)
+
+        self.session = requests.Session()
+
+    @property
+    def credentials(self) -> Credentials:
+        return self._credentials
+
+    @property
+    def base_url(self) -> str:
+        return self._base_url
+
+    @property
+    def headers(self) -> Dict[str, str]:
+        return self._headers
+
+    @retry()
+    def _request(self, method: Literal["GET", "POST"], suffix: str, *args, **kwargs) -> Response:
+        request = requests.Request(method=method, url=self.base_url + suffix, headers=self.headers, *args, **kwargs)
+        prepared_request = request.prepare()
+
+        if LOG_REQUESTS:
+            log_request(prepared_request)
+
+        response = self.session.send(prepared_request)
+
+        if LOG_REQUESTS:
+            log_response(response)
+
+        return response
+
+    def get(self, suffix: str, *args, **kwargs) -> Response:
+        return self._request(method="GET", suffix=suffix, *args, **kwargs)
+
+    def post(self, suffix: str, *args, **kwargs) -> Response:
+        return self._request(method="POST", suffix=suffix, *args, **kwargs)
+
+    def _list_datasets(self):
+        response = self.get(suffix="/datasets/list")
+        return get_response(response)
+
+    def _create_dataset(
+        self, dataset_id: str, schema: Optional[Schema] = None, upsert: bool = True, expire: bool = False
+    ) -> Any:
+        obj = dict(id=dataset_id, upsert=upsert, expire=expire)
+        if schema:
+            obj["schema"] = schema
+        response = self.post(suffix=f"/datasets/create", json=obj)
+        return get_response(response)
+
+    def _delete_dataset(self, dataset_id: str) -> Any:
+        response = self.post(suffix=f"/datasets/{dataset_id}/delete")
+        return get_response(response)
+
+    def _get_schema(self, dataset_id: str) -> Schema:
+        response = self.get(suffix=f"/datasets/{dataset_id}/schema")
+        return get_response(response)
+
+    def _bulk_insert(
+        self,
+        dataset_id: str,
+        documents: List[document.Document],
+        insert_date: bool = True,
+        overwrite: bool = True,
+        update_schema: bool = True,
+        wait_for_update: bool = True,
+        field_transformers: List[FieldTransformer] = None,
+        ingest_in_background: bool = False,
+    ) -> Any:
+        response = self.post(
+            suffix=f"/datasets/{dataset_id}/documents/bulk_insert",
+            json=dict(
+                documents=documents,
+                insert_date=insert_date,
+                overwrite=overwrite,
+                update_schema=update_schema,
+                field_transformers=[] if field_transformers is None else field_transformers,
+                ingest_in_background=ingest_in_background,
+                wait_for_update=wait_for_update,
+            ),
+        )
+        return get_response(response)
+
+    def _bulk_update(
+        self,
+        dataset_id: str,
+        documents: List[document.Document],
+        insert_date: bool = True,
+        ingest_in_background: bool = True,
+        update_schema: bool = True,
+    ) -> Any:
+        response = self.post(
+            suffix=f"/datasets/{dataset_id}/documents/bulk_update",
+            json=dict(
+                updates=documents,
+                insert_date=insert_date,
+                ingest_in_background=ingest_in_background,
+                update_schema=update_schema,
+            ),
+        )
+        return get_response(response)
+
+    def _get_where(
+        self,
+        dataset_id: str,
+        page_size: int,
+        filters: Optional[List[Filter]] = None,
+        sort: Optional[list] = None,
+        select_fields: Optional[List[str]] = None,
+        include_vector: bool = True,
+        random_state: int = 0,
+        is_random: bool = False,
+        after_id: Optional[List] = None,
+        worker_number: int = 0,
+    ):
+        response = self.post(
+            suffix=f"/datasets/{dataset_id}/documents/get_where",
+            json=dict(
+                select_fields=[] if select_fields is None else select_fields,
+                page_size=min(9999, page_size),
+                sort=[] if sort is None else sort,
+                include_vector=include_vector,
+                filters=[] if filters is None else filters,
+                random_state=random_state,
+                is_random=is_random,
+                after_id=[] if after_id is None else after_id,
+                worker_number=worker_number,
+            ),
+        )
+        return get_response(response)
+
+    def _delete_where(self, dataset_id: str, filters: Optional[List[Filter]] = None):
+        response = self.post(
+            suffix=f"/datasets/{dataset_id}/documents/delete_where",
+            json=dict(filters=[] if filters is None else filters),
+        )
+        return get_response(response)
+
+    def _update_dataset_metadata(self, dataset_id: str, metadata: Dict[str, Any]):
+        """
+        Edit and add metadata about a dataset. Notably description, data source, etc
+        """
+        response = self.post(
+            suffix=f"/datasets/{dataset_id}/metadata", json=dict(dataset_id=dataset_id, metadata=metadata)
+        )
+        return get_response(response)
+
+    def _get_metadata(self, dataset_id: str) -> Dict[str, Any]:
+        response = self.get(suffix=f"/datasets/{dataset_id}/metadata")
+        return get_response(response)
+
+    def _insert_centroids(
+        self, dataset_id: str, cluster_centers: List[document.Document], vector_fields: List[str], alias: str
+    ):
+        response = self.post(
+            suffix=f"/datasets/{dataset_id}/cluster/centroids/insert",
+            json=dict(dataset_id=dataset_id, cluster_centers=cluster_centers, vector_fields=vector_fields, alias=alias),
+        )
+        return get_response(response)
+
+    def _get_centroids(
+        self,
+        dataset_id: str,
+        vector_fields: List[str],
+        alias: str,
+        page_size: int = 5,
+        page: int = 1,
+        cluster_ids: Optional[List] = None,
+        include_vector: bool = False,
+    ):
+        response = self.post(
+            suffix=f"/datasets/{dataset_id}/cluster/centroids/documents",
+            json=dict(
+                cluster_ids=[] if cluster_ids is None else cluster_ids,
+                vector_fields=vector_fields,
+                alias=alias,
+                page_size=min(9999, page_size),
+                page=page,
+                include_vector=include_vector,
+            ),
+        )
+        return get_response(response)
+
+    def _set_workflow_status(
+        self,
+        job_id: str,
+        workflow_name: str,
+        additional_information: str = "",
+        metadata: Dict[str, Any] = None,
+        status: str = "inprogress",
+        send_email: bool = True,
+        worker_number: int = None,
+        output: Dict[str, Any] = None,
+        email: Dict[str, Any] = None,
+        user_errors: str = None,
+    ):
+        # add edge case for API
+        if job_id == "":
+            return
+        if status not in {"inprogress", "complete", "failed"}:
+            raise ValueError("state should be one of `['inprogress', 'complete', 'failed']`")
+        parameters = dict(
+            status=status,
+            workflow_name=workflow_name,
+            additional_information=additional_information,
+            send_email=send_email,
+        )
+        # metadata can't be an empty dictionary as it overwrites
+        if metadata is not None and metadata != {}:
+            parameters["metadata"] = metadata
+
+        if worker_number is not None:
+            parameters["worker_number"] = worker_number
+
+        if output:
+            parameters["output"] = output
+
+        if user_errors:
+            parameters["user_errors"] = user_errors
+
+        if email:
+            # adding some assertions here for better developer experience
+            assert isinstance(email, dict)
+            assert "secondary_cta" in email
+            assert "url" in email["secondary_cta"]
+            assert "text" in email["secondary_cta"]
+
+            parameters["email"] = email
+
+        ic(parameters)
+
+        response = self.post(suffix=f"/workflows/{job_id}/status", json=parameters)
+        return get_response(response)
+
+    def _set_field_children(
+        self,
+        dataset_id: str,
+        fieldchildren_id: str,
+        field: str,
+        field_children: List[str],
+        metadata: Optional[Dict[str, Any]] = None,
+    ):
+        """
+        fieldchildren_id: The name of the workflow or operation
+
+        field: the input field of the operation
+
+        field_children: a list of output fields, taken from the most nested level
+        i.e. ["_sentiment_.text_field.alias"]
+
+        metadata: extra parameters associated with operation
+        i.e. n_clusters, n_init, softmax_temperature, etc...
+        """
+        params = dict(
+            field=field,
+            field_children=field_children,
+            category=fieldchildren_id,
+            metadata={} if metadata is None else metadata,
+        )
+        ic(params)
+        response = self.post(suffix=f"/datasets/{dataset_id}/field_children/{str(uuid.uuid4())}/update", json=params)
+        return get_response(response)
+
+    def _delete_field_children(self, dataset_id: str, fieldchildren_id: str):
+        response = self.post(suffix=f"/datasets/{dataset_id}/field_children/{fieldchildren_id}/delete")
+        return get_response(response)
+
+    def _list_field_children(self, dataset_id: str, page: int = 1, page_size: int = 10000, sort=None):
+        parameters = {"page": page, "page_size": page_size}
+
+        if sort:
+            parameters["sort"] = sort
+
+        response = self.post(suffix=f"/datasets/{dataset_id}/field_children/list", json=parameters)
+        return get_response(response)
+
+    def _get_health(self, dataset_id: str):
+        response = self.get(suffix=f"/datasets/{dataset_id}/monitor/health")
+        return get_response(response)
+
+    def _get_workflow_status(self, job_id: str):
+        response = self.post(suffix=f"/workflows/{job_id}/get")
+        return get_response(response)
+
+    def _update_workflow_metadata(self, job_id: str, metadata: Dict[str, Any]):
+        response = self.post(suffix=f"/workflows/{job_id}/metadata", json=dict(metadata=metadata))
+        return get_response(response)
+
+    def _get_file_upload_urls(self, dataset_id: str, files: List[str]):
+        response = self.post(suffix=f"/datasets/{dataset_id}/get_file_upload_urls", json=dict(files=files))
+        return get_response(response)
+
+    def _get_temp_file_upload_url(self, ext: str = None):
+        """Use this for temporary file uploads.
+        returns: {'download_url': ..., 'upload_url': ...}
+        """
+        body = {}
+        if ext is not None:
+            body["extension"] = ext
+        response = self.post(suffix=f"/services/get_temporary_file_upload_url", json=body)
+        return get_response(response)
+
+    def _upload_temporary_media(self, presigned_url: str, media_content: bytes):
+        return requests.put(presigned_url, headers={"x-amz-tagging": "Expire=true"}, data=media_content)
+
+    def _upload_media(self, presigned_url: str, media_content: bytes):
+        # dont use get response since response cannot be json decoded
+        return requests.put(presigned_url, data=media_content)
+
+    def _trigger(
+        self,
+        dataset_id: str,
+        params: dict,
+        workflow_id: str,
+        notebook_path: str = None,
+        instance_type: str = None,
+        host_type: str = None,
+        version: str = "production_version",
+    ):
+        """
+        trigger a workflow
+        """
+
+        data = dict(params=params, dataset_id=dataset_id, workflow_id=workflow_id, version=version)
+        if notebook_path is not None:
+            data["notebook_path"] = notebook_path
+        if instance_type is not None:
+            data["instance_type"] = instance_type
+        if host_type is not None:
+            data["host_type"] = host_type
+        return self.post(suffix=f"/workflows/trigger", json=data).json()
+
+    def _trigger_polling_workflow(
+        self,
+        dataset_id: str,
+        input_field: str,
+        output_field: str,
+        job_id: str,
+        workflow_name: str,
+        # set 95% coverage in case of edge cases like workflow only working
+        # on certain proportion of dataset
+        minimum_coverage: float = 0.95,
+        max_time: float = 120,
+        sleep_timer: float = 10,
+        workflow_id="poll",
+        version="production_version",
+    ):
+        """
+        Trigger the polling workflow
+        """
+        return self._trigger(
+            dataset_id=dataset_id,
+            params=dict(
+                dataset_id=dataset_id,
+                input_field=input_field,
+                output_field=output_field,
+                minimum_coverage=minimum_coverage,
+                max_time=max_time,
+                sleep_timer=sleep_timer,
+                parent_job_id=job_id,
+                parent_job_name=workflow_name,
+            ),
+            workflow_id=workflow_id,
+            version=version,
+            notebook_path="",
+            instance_type="batch",
+            host_type="batch",
+        )
+
+    def _update_workflow_progress(
+        self,
+        workflow_id: str,
+        worker_number: int = 0,
+        step: str = "Workflow",
+        n_processed: int = 0,
+        n_total: int = 0,
+        n_processed_pricing: Optional[int] = None,  # optional parameter
+    ):
+        """
+        Tracks Workflow Progress
+        """
+        if worker_number is None:
+            worker_number = 0
+
+        if n_processed_pricing:
+            params["n_processed_pricing "] = n_processed_pricing
+
+        params = dict(worker_number=worker_number, step=step, n_processed=n_processed, n_total=n_total)
+
+        ic("adding progress...")
+        ic(params)
+
+        response = self.post(suffix=f"/workflows/{workflow_id}/progress", json=params)
+        return get_response(response)
+
+    def _update_workflow_pricing(
+        self,
+        workflow_id: str,
+        worker_number: int = 0,
+        step: str = "Workflow",
+        n_processed_pricing: Optional[int] = None,
+    ):
+        """
+        Pricing endpoint is really part of progress endpoint but this is being
+        abstracted away for now due to the fact that the pricing is actually
+        something outside of progress.
+        """
+        if worker_number is None:
+            worker_number = 0
+
+        params = dict(worker_number=worker_number, step=step, n_processed_pricing=n_processed_pricing)
+        ic("adding progress...")
+        ic(params)
+        response = self.post(suffix=f"/workflows/{workflow_id}/progress", json=params)
+        return get_response(response)
+
+    def _append_tags(self, dataset_id: str, field: str, tags_to_add: List[str], filters: List[Filter]):
+        response = self.post(
+            suffix=f"/datasets/{dataset_id}/tags/append",
+            json=dict(field=field, tags_to_add=tags_to_add, filters=filters),
+        )
+        return get_response(response)
+
+    def _delete_tags(self, dataset_id: str, field: str, tags_to_delete: List[str], filters: List[Filter]):
+        response = self.post(
+            suffix=f"/datasets/{dataset_id}/tags/delete",
+            json=dict(field=field, tags_to_delete=tags_to_delete, filters=filters),
+        )
+        return get_response(response)
+
+    def _merge_tags(self, dataset_id: str, field: str, tags_to_merge: Dict[str, str], filters: List[Filter]):
+        response = self.post(
+            suffix=f"/datasets/{dataset_id}/tags/merge",
+            json=dict(field=field, tags_to_merge=tags_to_merge, filters=filters),
+        )
+        return get_response(response)
+
+    def _bulk_update_keyphrase(self, dataset_id: str, field: str, alias: str, updates: List):
+        """
+        Update keyphrases
+        """
+        response = self.post(
+            suffix=f"/datasets/{dataset_id}/fields/{field}.{alias}/keyphrase/bulk_update", json=dict(updates=updates)
+        )
+        return get_response(response)
+
+    def _bulk_delete_keyphrase(self, dataset_id: str, field: str, alias: str, ids: List[str]):
+        """
+        Update keyphrases
+        """
+        response = self.post(
+            suffix=f"/datasets/{dataset_id}/fields/{field}.{alias}/keyphrase/bulk_delete", json=dict(ids=ids)
+        )
+        return get_response(response)
+
+    def _get_keyphrase(self, dataset_id: str, field: str, alias: str, keyphrase_id: str):
+        """
+        Get keyphrase
+        """
+        if isinstance(keyphrase_id, str) and keyphrase_id != "":
+            response = self.get(suffix=f"/datasets/{dataset_id}/fields/{field}.{alias}/keyphrase/{keyphrase_id}/get")
+            return get_response(response)
+
+    def _delete_keyphrase(self, dataset_id: str, field: str, keyphrase_id: str, alias: str):
+        """
+        Deleting Keyphrases
+        """
+        response = self.post(suffix=f"/datasets/{dataset_id}/fields/{field}.{alias}/keyphrase/{keyphrase_id}/delete")
+        return get_response(response)
+
+    def _update_keyphrase(
+        self,
+        dataset_id: str,
+        field: str,
+        keyphrase_id: str,
+        alias: str,
+        keyphrase: str,
+        frequency: int = 0,
+        ancestors: list = None,
+        parents: list = None,
+        metadata: dict = None,
+        keyphrase_score: float = 0,
+        level: int = 0,
+    ):
+        # missing update contents here?
+        """
+        Update keyphrases
+        """
+        params = {
+            "_id": keyphrase_id,
+            "text": keyphrase,
+            "frequency": frequency,
+            "keyphrase_score": keyphrase_score,
+            "level": level,
+        }
+        if ancestors is not None:
+            params["ancestors"] = ancestors
+        if parents is not None:
+            params["parents"] = parents
+        if metadata is not None:
+            params["metadata"] = metadata
+        response = self.post(
+            suffix=f"/datasets/{dataset_id}/fields/{field}.{alias}/keyphrase/{keyphrase_id}/update", json=params
+        )
+        return get_response(response)
+
+    def _list_keyphrase(
+        self, dataset_id: str, field: str, alias: str, page: int = 0, page_size: int = 100, sort: list = None
+    ):
+        """
+        List keyphrases
+        """
+        params = {"page": page, "page_size": min(9999, page_size)}
+        if sort is not None:
+            params["sort"] = sort
+        response = self.post(suffix=f"/datasets/{dataset_id}/fields/{field}.{alias}/keyphrase/list", json=params)
+        return get_response(response)
+
+    def _facets(
+        self,
+        dataset_id: str,
+        fields: List[str],
+        data_interval: str = "monthly",
+        page_size: int = 1000,
+        asc: bool = False,
+    ):
+        response = self.post(
+            suffix=f"/datasets/{dataset_id}/facets",
+            json=dict(fields=fields, data_interval=data_interval, page_size=min(9999, page_size), asc=asc),
+        )
+        return get_response(response)
+
+    def _upsert_dataset_settings(self, dataset_id: str, settings: Optional[Dict[str, Any]] = None):
+        response = self.post(
+            suffix=f"/datasets/{dataset_id}/settings", json=dict(settings={} if settings is None else settings)
+        )
+        return get_response(response)
+
+    def _get_dataset_settings(self, dataset_id: str):
+        response = self.get(suffix=f"/datasets/{dataset_id}/settings")
+        return get_response(response)
+
+    def _create_deployable(self, dataset_id: Optional[str] = None, config: Optional[Dict[str, Any]] = None):
+        response = self.post(
+            suffix="/deployables/create",
+            json=dict(dataset_id=dataset_id, configuration={} if config is None else config),
+        )
+        return get_response(response)
+
+    def _share_dashboard(self, deployable_id: str):
+        response = self.post(suffix=f"/deployablegroups/{deployable_id}/share")
+        return get_response(response)
+
+    def _unshare_dashboard(self, deployable_id: str):
+        response = self.post(suffix=f"/deployablegroups/{deployable_id}/private")
+        return get_response(response)
+
+    def _get_deployable(self, deployable_id: str):
+        response = self.get(suffix=f"/deployables/{deployable_id}/get")
+        return get_response(response)
+
+    def _delete_deployable(self, deployable_id: str):
+        response = self.post(suffix=f"/deployables/delete", json=dict(id=deployable_id))
+        return get_response(response)
+
+    def _list_deployables(self, page_size: int):
+        response = self.get(suffix="/deployables/list", params=dict(page_size=min(9999, page_size)))
+        return get_response(response)
+
+    def _label_openai(
+        self,
+        dataset_id: str,
+        vector_field: str,
+        field: str,
+        alias: str,
+        question_suffix: str,
+        accuracy: int = 4,
+        cluster_ids: list = None,
+        dont_save_summaries: bool = True,
+        filters: list = None,
+    ):
+        params = {
+            "vector_fields": [vector_field],
+            # legacy parameter
+            "centroid_vector_fields": [vector_field],
+            "alias": alias,
+            "dataset_id": dataset_id,
+            "cluster_ids": cluster_ids,
+            "dont_save_summaries": dont_save_summaries,
+            "questions": [
+                {
+                    "cluster_ids": cluster_ids,
+                    "config": {
+                        "accuracy": accuracy,
+                        "examples": [],
+                        "field": field,
+                        "question_suffix": question_suffix,
+                    },
+                }
+            ],
+        }
+        if filters is not None:
+            params["filters"] = filters
+        response = self.post(suffix=f"/datasets/{dataset_id}/cluster/centroids/labels/create", json=params)
+        return get_response(response)
+
+    def _aggregate(
+        self,
+        dataset_id: str,
+        page_size: str = 20,
+        page: str = 1,
+        asc: str = False,
+        aggregation_query: Dict[str, List[Dict[str, Any]]] = None,
+        dataset_ids: List[str] = None,
+        filters: List[Filter] = None,
+    ):
+        response = self.post(
+            suffix=f"/datasets/{dataset_id}/aggregate",
+            json=dict(
+                filters=[] if filters is None else filters,
+                aggregation_query=aggregation_query,
+                page_size=min(9999, page_size),
+                page=page,
+                asc=asc,
+                dataset_ids=[] if dataset_ids is None else dataset_ids,
+                dataset_id=dataset_id,
+            ),
+        )
+        return get_response(response)
+
+    def _list_closest_to_center(
+        self,
+        dataset_id: str,
+        vector_fields: List[str],
+        alias: str,
+        approx: int = 0,
+        sum_fields: bool = True,
+        page: int = 1,
+        similarity_metric: str = "cosine",
+        min_score: float = 0,
+        include_vector: bool = False,
+        include_count: bool = True,
+        include_relevance: bool = False,
+        page_size: int = 20,
+        cluster_properties_filter: Dict[str, Any] = None,
+        cluster_ids: List[str] = None,
+        filters: List[Filter] = None,
+        select_fields: List[str] = None,
+    ):
+        response = self.post(
+            suffix=f"/datasets/{dataset_id}/cluster/centroids/list_closest_to_center",
+            json=dict(
+                vector_fields=vector_fields,
+                alias=alias,
+                approx=approx,
+                sum_fields=sum_fields,
+                page=page,
+                similarity_metric=similarity_metric,
+                min_score=min_score,
+                include_vector=include_vector,
+                include_count=include_count,
+                include_relevance=include_relevance,
+                page_size=min(9999, page_size),
+                cluster_properties_filter=cluster_properties_filter if cluster_properties_filter is not None else {},
+                filters=filters if filters is not None else [],
+                cluster_ids=cluster_ids if cluster_ids is not None else [],
+                select_fields=select_fields if select_fields is not None else [],
+            ),
+        )
+        return get_response(response)
+
+    def _list_project_keys(self):
+        response = self.get(suffix="/projects/keys/list")
+        return get_response(response)
+
+    def _get_project_key(self, key: str, token: str):
+        response = self.post(suffix="/projects/keys/get", json=dict(key=key, token=token))
+        return get_response(response)
+
+    def _set_project_key(self, key: str, value: str):
+        response = self.post(suffix="/projects/keys/set", json=dict(key=key, value=value))
+        return get_response(response)
+
+    def _delete_project_key(self, key: str):
+        response = self.post(suffix="/projects/keys/delete", json=dict(key=key))
+        return get_response(response)
+
+    def _update_version_aliases(self, development_version: str, production_version: str):
+        response = self.post(
+            suffix="/workflows/types/version_aliases/update",
+            json={"aliases": {"development_version": development_version, "production_version": production_version}},
+        )
+        return get_response(response)
+
+    def _openai_completion(
+        self, workflows_admin_token: str, body: dict, suffix: str = "/admin/proxy/openai/v1/completions"
+    ):
+        response = self.post(suffix=suffix, json={"token": workflows_admin_token, "body": body})
+        return get_response(response)
+
+    def _proxy_openai(self, workflows_admin_token: str, endpoint: str, body: dict):
+        response = self.post(
+            suffix="/admin/proxy/openai" + endpoint, json={"token": workflows_admin_token, "body": body}
+        )
+        return get_response(response)
```

### Comparing `ai_transform-0.32.3/ai_transform/api/client.py` & `ai_transform-0.32.4/ai_transform/api/client.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,135 +1,135 @@
-import os
-import warnings
-
-from typing import Optional, Dict, Any, Union
-
-from ai_transform.api.api import API
-from ai_transform.api.helpers import process_token
-from ai_transform.dataset.dataset import Dataset
-from ai_transform.types import Schema
-from ai_transform.errors import AuthException
-from ai_transform.constants import WELCOME_MESSAGE
-from ai_transform.workflow.context_manager import WorkflowContextManager
-from ai_transform.logger import ic
-
-
-class Client:
-    def __init__(self, token: str = None, authenticate: bool = True) -> None:
-        if token is None:
-            token = os.getenv("DEVELOPMENT_TOKEN")
-
-        self._credentials = process_token(token)
-        self._token = token
-        self._api = API(credentials=self.credentials)
-
-        if authenticate:
-            try:
-                self.list_datasets()["datasets"]
-            except:
-                raise AuthException
-            else:
-                print(WELCOME_MESSAGE.format(self.credentials.project))
-        else:
-            warnings.warn(
-                "You have opted to not authenticate on client instantiation. Your token may or may not be valid."
-            )
-
-    @property
-    def credentials(self):
-        return self._credentials
-
-    @property
-    def api(self) -> API:
-        return self._api
-
-    def list_datasets(self):
-        return self.api._list_datasets()
-
-    def create_dataset(
-        self, dataset_id: str, schema: Optional[Schema] = None, upsert: bool = True, expire: bool = False
-    ) -> None:
-        return self.api._create_dataset(
-            dataset_id=dataset_id, schema={} if schema is None else schema, upsert=upsert, expire=expire
-        )
-
-    def delete_dataset(self, dataset_id: str) -> None:
-        return self.api._delete_dataset(dataset_id=dataset_id)
-
-    def Dataset(self, dataset_id: str, expire: bool = False) -> Dataset:
-        self.create_dataset(dataset_id=dataset_id, expire=expire)
-        return Dataset(api=self.api, dataset_id=dataset_id)
-
-    def SimpleWorkflow(
-        self,
-        workflow_name: str,
-        job_id: str,
-        additional_information: str = "",
-        send_email: bool = True,
-        email: Dict[str, Any] = None,
-        metadata: Dict[str, Any] = None,
-        output: dict = None,
-    ) -> WorkflowContextManager:
-        return WorkflowContextManager(
-            credentials=self.credentials,
-            workflow_name=workflow_name,
-            job_id=job_id,
-            metadata=metadata,
-            additional_information=additional_information,
-            send_email=send_email,
-            email=email,
-            output=output,
-        )
-
-    def insert_temp_local_media(self, file_path_or_bytes: Union[str, bytes], ext: str = None):
-        """
-        Insert temporary local media.
-        """
-        if isinstance(file_path_or_bytes, str):
-            with open(file_path_or_bytes, "rb") as fn_byte:
-                media_content = bytes(fn_byte.read())
-            if ext is None:
-                _, ext = os.path.splitext(file_path_or_bytes)
-                ext = ext[1:] # remove leading `.`
-            
-        elif isinstance(file_path_or_bytes, bytes):
-            media_content = file_path_or_bytes
-            if ext is None:
-                raise ValueError("Must set file ext i.e. `csv` or `png`")
-
-        else:
-            raise ValueError("`file_path_or_bytes` must be one of type `str` or `bytes`")
-
-        data = self.api._get_temp_file_upload_url(ext)
-        upload_url = data["upload_url"]
-        download_url = data["download_url"]
-            
-        response = self.api._upload_temporary_media(presigned_url=upload_url, media_content=media_content)
-        ic(response.content)
-        return {"download_url": download_url}
-
-    def list_project_keys(self):
-        return self.api._list_project_keys()
-
-    def get_project_key(self, key: str, token: str):
-        return self.api._get_project_key(key=key, token=token)
-
-    def set_project_key(self, key: str, value: str):
-        return self.api._set_project_key(key=key, value=value)
-
-    def delete_project_key(self, key: str):
-        return self.api._delete_project_key(key=key)
-
-    def update_api_version(self, development_version: str, production_version: str):
-        return self.api._update_version_aliases(development_version, production_version)
-
-    def openai_completion(
-        self,
-        prompt: str,
-        model: str = "text-davinci-003",
-        workflows_admin_token: str = None,
-        max_tokens: int = 20,
-        temperature: float = 0.0,
-    ):
-        if workflows_admin_token is None:
-            workflows_admin_token = os.getenv("WORKFLOWS_ADMIN_TOKEN")
-        return self.api._openai_completion(workflows_admin_token, model, prompt, max_tokens, temperature)
+import os
+import warnings
+
+from typing import Optional, Dict, Any, Union
+
+from ai_transform.api.api import API
+from ai_transform.api.helpers import process_token
+from ai_transform.dataset.dataset import Dataset
+from ai_transform.types import Schema
+from ai_transform.errors import AuthException
+from ai_transform.constants import WELCOME_MESSAGE
+from ai_transform.workflow.context_manager import WorkflowContextManager
+from ai_transform.logger import ic
+
+
+class Client:
+    def __init__(self, token: str = None, authenticate: bool = True) -> None:
+        if token is None:
+            token = os.getenv("DEVELOPMENT_TOKEN")
+
+        self._credentials = process_token(token)
+        self._token = token
+        self._api = API(credentials=self.credentials)
+
+        if authenticate:
+            try:
+                self.list_datasets()["datasets"]
+            except:
+                raise AuthException
+            else:
+                print(WELCOME_MESSAGE.format(self.credentials.project))
+        else:
+            warnings.warn(
+                "You have opted to not authenticate on client instantiation. Your token may or may not be valid."
+            )
+
+    @property
+    def credentials(self):
+        return self._credentials
+
+    @property
+    def api(self) -> API:
+        return self._api
+
+    def list_datasets(self):
+        return self.api._list_datasets()
+
+    def create_dataset(
+        self, dataset_id: str, schema: Optional[Schema] = None, upsert: bool = True, expire: bool = False
+    ) -> None:
+        return self.api._create_dataset(
+            dataset_id=dataset_id, schema={} if schema is None else schema, upsert=upsert, expire=expire
+        )
+
+    def delete_dataset(self, dataset_id: str) -> None:
+        return self.api._delete_dataset(dataset_id=dataset_id)
+
+    def Dataset(self, dataset_id: str, expire: bool = False) -> Dataset:
+        self.create_dataset(dataset_id=dataset_id, expire=expire)
+        return Dataset(api=self.api, dataset_id=dataset_id)
+
+    def SimpleWorkflow(
+        self,
+        workflow_name: str,
+        job_id: str,
+        additional_information: str = "",
+        send_email: bool = True,
+        email: Dict[str, Any] = None,
+        metadata: Dict[str, Any] = None,
+        output: dict = None,
+    ) -> WorkflowContextManager:
+        return WorkflowContextManager(
+            credentials=self.credentials,
+            workflow_name=workflow_name,
+            job_id=job_id,
+            metadata=metadata,
+            additional_information=additional_information,
+            send_email=send_email,
+            email=email,
+            output=output,
+        )
+
+    def insert_temp_local_media(self, file_path_or_bytes: Union[str, bytes], ext: str = None):
+        """
+        Insert temporary local media.
+        """
+        if isinstance(file_path_or_bytes, str):
+            with open(file_path_or_bytes, "rb") as fn_byte:
+                media_content = bytes(fn_byte.read())
+            if ext is None:
+                _, ext = os.path.splitext(file_path_or_bytes)
+                ext = ext[1:] # remove leading `.`
+            
+        elif isinstance(file_path_or_bytes, bytes):
+            media_content = file_path_or_bytes
+            if ext is None:
+                raise ValueError("Must set file ext i.e. `csv` or `png`")
+
+        else:
+            raise ValueError("`file_path_or_bytes` must be one of type `str` or `bytes`")
+
+        data = self.api._get_temp_file_upload_url(ext)
+        upload_url = data["upload_url"]
+        download_url = data["download_url"]
+            
+        response = self.api._upload_temporary_media(presigned_url=upload_url, media_content=media_content)
+        ic(response.content)
+        return {"download_url": download_url}
+
+    def list_project_keys(self):
+        return self.api._list_project_keys()
+
+    def get_project_key(self, key: str, token: str):
+        return self.api._get_project_key(key=key, token=token)
+
+    def set_project_key(self, key: str, value: str):
+        return self.api._set_project_key(key=key, value=value)
+
+    def delete_project_key(self, key: str):
+        return self.api._delete_project_key(key=key)
+
+    def update_api_version(self, development_version: str, production_version: str):
+        return self.api._update_version_aliases(development_version, production_version)
+
+    def openai_completion(
+        self,
+        prompt: str,
+        model: str = "text-davinci-003",
+        workflows_admin_token: str = None,
+        max_tokens: int = 20,
+        temperature: float = 0.0,
+    ):
+        if workflows_admin_token is None:
+            workflows_admin_token = os.getenv("WORKFLOWS_ADMIN_TOKEN")
+        return self.api._openai_completion(workflows_admin_token, model, prompt, max_tokens, temperature)
```

### Comparing `ai_transform-0.32.3/ai_transform/api/helpers.py` & `ai_transform-0.32.4/ai_transform/api/helpers.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from ai_transform.types import Credentials
-
-
-def process_token(token: str) -> Credentials:
-    return Credentials(*token.split(":"))
-
-
-def requests_post_mock(url="", headers=None, json=None):
-    """
-    Use as follows to help the API team debug responses
-    import requests
-    response = requests_post_mock(
-        url=f"https://api-{region}.stack.tryrelevance.com/latest/workflows/types/bulk_update",
-        headers={"Authorization": auth},
-        json={
-            "updates": workflows[0:20],
-            "version": "vtest"
-        }
-    )
-    ic(response)
-    """
-    # TODO: Add get request etc.
-    if headers is None:
-        headers = {}
-    if json is None:
-        json = {}
-    return f"""
-import requests
-r = requests.post(url='{url}',headers={headers},json={json})
-  """
+from ai_transform.types import Credentials
+
+
+def process_token(token: str) -> Credentials:
+    return Credentials(*token.split(":"))
+
+
+def requests_post_mock(url="", headers=None, json=None):
+    """
+    Use as follows to help the API team debug responses
+    import requests
+    response = requests_post_mock(
+        url=f"https://api-{region}.stack.tryrelevance.com/latest/workflows/types/bulk_update",
+        headers={"Authorization": auth},
+        json={
+            "updates": workflows[0:20],
+            "version": "vtest"
+        }
+    )
+    ic(response)
+    """
+    # TODO: Add get request etc.
+    if headers is None:
+        headers = {}
+    if json is None:
+        json = {}
+    return f"""
+import requests
+r = requests.post(url='{url}',headers={headers},json={json})
+  """
```

### Comparing `ai_transform-0.32.3/ai_transform/config.py` & `ai_transform-0.32.4/ai_transform/config.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,111 +1,111 @@
-"""
-Config class
-"""
-import uuid
-import json
-import base64
-import argparse
-
-from typing import Optional, List
-from ai_transform.workflow.helpers import decode_workflow_token
-
-from pydantic import BaseModel, Field
-
-
-def generate_random_string():
-    return str(uuid.uuid4())
-
-
-class BaseConfig(BaseModel):
-    """
-    An example configuration for workflows so that we can modify the the schema.
-
-    .. code-block::
-
-        from ai_transform.config import BaseConfig
-
-        class SentimentConfig(BaseConfig):
-            text_field: str
-
-
-        result = SentimentConfig.to_schema()
-
-    """
-
-    authorizationToken: str = None
-    dataset_id: Optional[str] = None
-    job_id: Optional[str] = Field(default_factory=generate_random_string, description="the job ID")
-    total_workers: Optional[int] = Field(default=None, description="Total workers.")
-    send_email: Optional[bool] = Field(
-        default=True, description="If True, sends an email upon completion. Otherwise, False."
-    )
-    additional_information: Optional[str] = Field(default="", description="What to include in the e-mail.")
-    filters: Optional[list] = Field(default=[], description="Filters to apply.")
-    documents: Optional[list] = Field(default=None, description="You can submit documents and have it run immediately.")
-
-    @classmethod
-    def to_schema(self):
-        return self.schema_json()
-
-    def read_from_argparser(self, argparser: argparse.ArgumentParser):
-        # Enables behavior such
-        # reads in required attributes from argparser
-        for k in self.dict():
-            # gets the required attributes like 'text_field'
-            setattr(self, k, getattr(argparser, k))
-
-    @classmethod
-    def read_token(self, token: str):
-        # Enables behavior such
-        # reads in required attributes from argparser
-        config_dict = decode_workflow_token(token)
-        return self.parse_obj(config_dict)
-
-    @classmethod
-    def read_dict(self, data: dict):
-        # Read from data dictionary
-        for k in self.dict():
-            setattr(self, k, data.get(k))
-
-    def get(self, value, default=None):
-        """
-        For backwards compatibility with previous dictionary-input
-        configs
-        """
-        if hasattr(self, value):
-            return getattr(self, value)
-        else:
-            return default
-
-    def __getitem__(self, *args, **kwargs):
-        return self.get(*args, **kwargs)
-
-    def generate_token(self, *args, **kwargs):
-        # Generates a token for you anytime
-        config: dict = self.dict()
-        return base64.b64encode(json.dumps(config).encode()).decode()
-
-
-class BaseTransformConfig(BaseConfig):
-    """
-    Same as BaseConfig but a few more additional attributes.
-    This is suitable for basic transformations that go through
-    the same pulling, transforming and then pushing (e.g. sentiment or emotion workflows)
-    """
-
-    pull_chunksize: Optional[int] = Field(
-        default=1000, description="How many do you want to download and upload to the server."
-    )
-    transform_chunksize: Optional[int] = Field(default=20, description="How many do you want to transform each time?")
-    refresh: Optional[bool] = Field(default=False, description="If True, re-runs the workflow on the entire dataset.")
-    output_to_status: Optional[bool] = Field(
-        default=False, description="If True, it will output results to status object."
-    )
-    documents: Optional[List[object]] = Field(
-        default_factory=lambda: [], description="If passed in, documents will be used instead of dataset."
-    )
-    limit_documents: Optional[int] = Field(
-        default=None,
-        description="If passed in, the transform will be limited to the number of documents specified here",
-    )
-    webhook_url: str = None
+"""
+Config class
+"""
+import uuid
+import json
+import base64
+import argparse
+
+from typing import Optional, List
+from ai_transform.workflow.helpers import decode_workflow_token
+
+from pydantic import BaseModel, Field
+
+
+def generate_random_string():
+    return str(uuid.uuid4())
+
+
+class BaseConfig(BaseModel):
+    """
+    An example configuration for workflows so that we can modify the the schema.
+
+    .. code-block::
+
+        from ai_transform.config import BaseConfig
+
+        class SentimentConfig(BaseConfig):
+            text_field: str
+
+
+        result = SentimentConfig.to_schema()
+
+    """
+
+    authorizationToken: str = None
+    dataset_id: Optional[str] = None
+    job_id: Optional[str] = Field(default_factory=generate_random_string, description="the job ID")
+    total_workers: Optional[int] = Field(default=None, description="Total workers.")
+    send_email: Optional[bool] = Field(
+        default=True, description="If True, sends an email upon completion. Otherwise, False."
+    )
+    additional_information: Optional[str] = Field(default="", description="What to include in the e-mail.")
+    filters: Optional[list] = Field(default=[], description="Filters to apply.")
+    documents: Optional[list] = Field(default=None, description="You can submit documents and have it run immediately.")
+
+    @classmethod
+    def to_schema(self):
+        return self.schema_json()
+
+    def read_from_argparser(self, argparser: argparse.ArgumentParser):
+        # Enables behavior such
+        # reads in required attributes from argparser
+        for k in self.dict():
+            # gets the required attributes like 'text_field'
+            setattr(self, k, getattr(argparser, k))
+
+    @classmethod
+    def read_token(self, token: str):
+        # Enables behavior such
+        # reads in required attributes from argparser
+        config_dict = decode_workflow_token(token)
+        return self.parse_obj(config_dict)
+
+    @classmethod
+    def read_dict(self, data: dict):
+        # Read from data dictionary
+        for k in self.dict():
+            setattr(self, k, data.get(k))
+
+    def get(self, value, default=None):
+        """
+        For backwards compatibility with previous dictionary-input
+        configs
+        """
+        if hasattr(self, value):
+            return getattr(self, value)
+        else:
+            return default
+
+    def __getitem__(self, *args, **kwargs):
+        return self.get(*args, **kwargs)
+
+    def generate_token(self, *args, **kwargs):
+        # Generates a token for you anytime
+        config: dict = self.dict()
+        return base64.b64encode(json.dumps(config).encode()).decode()
+
+
+class BaseTransformConfig(BaseConfig):
+    """
+    Same as BaseConfig but a few more additional attributes.
+    This is suitable for basic transformations that go through
+    the same pulling, transforming and then pushing (e.g. sentiment or emotion workflows)
+    """
+
+    pull_chunksize: Optional[int] = Field(
+        default=1000, description="How many do you want to download and upload to the server."
+    )
+    transform_chunksize: Optional[int] = Field(default=20, description="How many do you want to transform each time?")
+    refresh: Optional[bool] = Field(default=False, description="If True, re-runs the workflow on the entire dataset.")
+    output_to_status: Optional[bool] = Field(
+        default=False, description="If True, it will output results to status object."
+    )
+    documents: Optional[List[object]] = Field(
+        default_factory=lambda: [], description="If passed in, documents will be used instead of dataset."
+    )
+    limit_documents: Optional[int] = Field(
+        default=None,
+        description="If passed in, the transform will be limited to the number of documents specified here",
+    )
+    webhook_url: str = None
```

### Comparing `ai_transform-0.32.3/ai_transform/dataset/field.py` & `ai_transform-0.32.4/ai_transform/dataset/field.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,406 +1,406 @@
-import uuid
-import numpy as np
-
-from typing import Dict, Any, List, Optional, Union
-
-from ai_transform.types import Filter
-from ai_transform.utils.document_list import DocumentList
-from ai_transform.utils.keyphrase import Keyphrase
-from dataclasses import asdict
-
-
-class Field:
-    def __init__(self, dataset, field: str):
-        from ai_transform.dataset.dataset import Dataset
-
-        self._dataset: Dataset = dataset
-        self._field = field
-        if field != "_id":
-            self._dtype = dataset.schema.get(field)
-        else:
-            self._dtype = None
-        self._filter_type = self._get_filter_type()
-
-    @property
-    def dataset(self):
-        return self._dataset
-
-    @property
-    def dataset_id(self):
-        return self._dataset.dataset_id
-
-    @property
-    def field(self):
-        return self._field
-
-    def list_field_parents(self) -> List[str]:
-        all_field_children = self.dataset.list_field_children()["results"]
-        field_parents = []
-        for relationship in all_field_children:
-            if self.field in relationship["field_children"]:
-                field_parents += [relationship["field"]]
-        return list(set(field_parents))
-
-    def list_field_children(self) -> List[str]:
-        all_field_children = self.dataset.list_field_children()["results"]
-        field_children = []
-        for relationship in all_field_children:
-            if relationship["field"] == self.field:
-                field_children += relationship["field_children"]
-        return list(set(field_children))
-
-    def add_field_children(
-        self,
-        field_children: List[str],
-        fieldchildren_id: str = None,
-        metadata: Dict[str, Any] = None,
-        recursive: bool = False,
-    ):
-        if fieldchildren_id is None:
-            fieldchildren_id = str(uuid.uuid4())
-        return self.dataset.set_field_children(
-            fieldchildren_id=fieldchildren_id,
-            field=self.field,
-            field_children=field_children,
-            recursive=recursive,
-            metadata=metadata,
-        )
-
-    def _get_filter_type(self) -> str:
-        if self._dtype == "numeric":
-            filter_type = "numeric"
-        elif self._dtype == "date":
-            filter_type = "date"
-        elif self._dtype is None:
-            filter_type = "ids"
-        else:
-            filter_type = "exact_match"
-        return filter_type
-
-    def __eq__(self, other: Union[str, float, int, bool, None], filter_type: Optional[str] = None) -> Filter:
-        if filter_type is None:
-            filter_type = self._filter_type
-        return [{"field": self._field, "filter_type": filter_type, "condition": "==", "condition_value": other}]
-
-    def __lt__(self, other: Union[str, float, int, bool, None], filter_type: Optional[str] = None) -> Filter:
-        if filter_type is None:
-            filter_type = self._filter_type
-        return [{"field": self._field, "filter_type": filter_type, "condition": "<", "condition_value": other}]
-
-    def __le__(self, other: Union[str, float, int, bool, None], filter_type: Optional[str] = None) -> Filter:
-        if filter_type is None:
-            filter_type = self._filter_type
-        return [{"field": self._field, "filter_type": filter_type, "condition": "<=", "condition_value": other}]
-
-    def __gt__(self, other: Union[str, float, int, bool, None], filter_type: Optional[str] = None) -> Filter:
-        if filter_type is None:
-            filter_type = self._filter_type
-        return [{"field": self._field, "filter_type": filter_type, "condition": ">", "condition_value": other}]
-
-    def __ge__(self, other: Union[str, float, int, bool, None], filter_type: Optional[str] = None) -> Filter:
-        if filter_type is None:
-            filter_type = self._filter_type
-        return [{"field": self._field, "filter_type": filter_type, "condition": ">=", "condition_value": other}]
-
-    def contains(self, other: str) -> Filter:
-        return [{"field": self._field, "filter_type": "contains", "condition": "==", "condition_value": other}]
-
-    def exists(self) -> Filter:
-        if "_chunk_" in self._field:
-            if self._field.endswith("_chunk_"):
-                parent_field = self._field
-            else:
-                parent_field = self._field.split(".")[0]
-
-            return [{"chunk": {"path": parent_field, "filters": [{"fieldExists": {"field": self._field}}]}}]
-        return [{"field": self._field, "filter_type": "exists", "condition": "==", "condition_value": " "}]
-
-    def not_exists(self) -> Filter:
-        return [{"field": self._field, "filter_type": "exists", "condition": "!=", "condition_value": " "}]
-
-    def insert_centroids(self, centroid_documents: DocumentList):
-        raise NotImplementedError(f"`insert_centroids` not available for non-vector fields")
-
-    def label_openai(
-        self,
-        field: str,
-        question_suffix: str,
-        accuracy: int = 4,
-        cluster_ids: list = None,
-        dont_save_summaries: bool = True,
-        filters: list = None,
-    ):
-        raise NotImplementedError(f"`label_openai` not available for non-vector fields")
-
-    def get_centroids(
-        self, page_size: int = 5, page: int = 1, cluster_ids: Optional[List] = None, include_vector: bool = False
-    ):
-        raise NotImplementedError(f"`get_centroids` not available for non-vector fields")
-
-    def get_all_centroids(self):
-        raise NotImplementedError(f"`get_all_centroids` not available for non-vector fields")
-
-    def create_centroid_documents(self):
-        raise NotImplementedError(f"`create_centroid_documents` not available for non-vector fields")
-
-    def list_closest_to_center(
-        self,
-        centroid_vector_fields: List[str],
-        cluster_field: str,
-        approx: int = 0,
-        sum_fields: bool = True,
-        page: int = 1,
-        similarity_metric: str = "cosine",
-        min_score: float = 0,
-        include_vector: bool = False,
-        include_count: bool = True,
-        include_relevance: bool = False,
-        page_size: int = 20,
-        cluster_properties_filter: Dict[str, Any] = None,
-        cluster_ids: List[str] = None,
-        filters: List[Filter] = None,
-        select_fields: List[str] = None,
-    ):
-        raise NotImplementedError("`list_closest_to_center` not available for non-vector fields")
-
-    def get_keyphrase(self, keyphrase_id: str):
-        raise NotImplementedError(f"`get_keyphrase` not available for non-keyphrase fields")
-
-    def update_keyphrase(
-        self,
-        keyphrase_id: str,
-        alias: str,
-        keyphrase: str,
-        frequency: int = 0,
-        ancestors: list = None,
-        parents: list = None,
-        metadata: dict = None,
-        keyphrase_score: float = 0,
-        level: int = 0,
-    ):
-        raise NotImplementedError(f"`update_keyphrase` not available for non-keyphrase fields")
-
-    def delete_keyphrase(self, keyphrase_id: str):
-        raise NotImplementedError(f"`delete_keyphrase` not available for non-keyphrase fields")
-
-    def bulk_update_keyphrases(self, updates: List[Union[Keyphrase, dict]]):
-        raise NotImplementedError(f"`bulk_update_keyphrases` not available for non-keyphrase fields")
-
-    def list_keyphrases(self, page_size: int = 100, page: int = 1, sort: list = None):
-        raise NotImplementedError(f"`list_keyphrases` not available for non-keyphrase fields")
-
-
-class ClusterField(Field):
-    def __init__(self, dataset, field: str):
-        super().__init__(dataset=dataset, field=field)
-        _, *middle_fields, alias = field.split(".")
-        self._cluster_field = ".".join(middle_fields)
-        self._cluster_alias = alias
-
-    def insert_centroids(self, centroid_documents: Union[List[Dict[str, Any]], DocumentList]):
-        if isinstance(centroid_documents, DocumentList):
-            centroid_documents = centroid_documents.to_json()
-        return self._dataset.api._insert_centroids(
-            dataset_id=self.dataset_id,
-            cluster_centers=centroid_documents,
-            vector_fields=[self._cluster_field],
-            alias=self._cluster_alias,
-        )
-
-    def get_centroids(
-        self, page_size: int = 5, page: int = 1, cluster_ids: Optional[List] = None, include_vector: bool = False
-    ):
-        return self._dataset.api._get_centroids(
-            dataset_id=self.dataset_id,
-            vector_fields=[self._cluster_field],
-            alias=self._cluster_alias,
-            page_size=page_size,
-            page=page,
-            cluster_ids=cluster_ids,
-            include_vector=include_vector,
-        )
-
-    def get_all_centroids(self, page_size: int = 5, cluster_ids: Optional[List] = None, include_vector: bool = False):
-        """
-        Get all centroids and returns as a dictionary for easy access
-        """
-        all_centroids = {"results": []}
-        page = 1
-        while True:
-            res = self._dataset.api._get_centroids(
-                dataset_id=self.dataset_id,
-                vector_fields=[self._cluster_field],
-                alias=self._cluster_alias,
-                page_size=page_size,
-                cluster_ids=cluster_ids,
-                include_vector=include_vector,
-                page=page,
-            )["results"]
-            if len(res) == 0:
-                break
-            else:
-                all_centroids["results"] += res
-                page += 1
-        return all_centroids
-
-    def label_openai(
-        self,
-        field: str,
-        question_suffix: str,
-        accuracy: int = 4,
-        cluster_ids: list = None,
-        dont_save_summaries: bool = True,
-        filters: list = None,
-    ):
-        return self._dataset.api._label_openai(
-            dataset_id=self.dataset_id,
-            vector_field=self._cluster_field,
-            field=field,
-            alias=self._cluster_alias,
-            question_suffix=question_suffix,
-            accuracy=accuracy,
-            cluster_ids=cluster_ids if cluster_ids is not None else [],
-            dont_save_summaries=dont_save_summaries,
-            filters=filters if filters is not None else [],
-        )
-
-    def create_centroid_documents(self):
-        documents = self._dataset.get_all_documents(select_fields=[self._cluster_field, self._field])
-        documents = documents["documents"]
-
-        vectors = np.array([document[self._cluster_field] for document in documents])
-
-        labels = [document[self._field] for document in documents]
-
-        label_map = {}
-        for label in labels:
-            if label not in label_map:
-                label_map[label] = len(label_map)
-
-        n_clusters = len(label_map)
-        centroid_documents = []
-
-        selected_vectors: np.ndarray
-        centroid_vector: np.ndarray
-
-        label_indices = np.array([label_map[label] for label in labels])
-
-        for index in range(n_clusters):
-            selected_vectors = vectors[label_indices == index]
-            centroid_vector = selected_vectors.mean(0)
-
-            centroid_document = {"_id": f"cluster_{index}", f"{self._cluster_field}": centroid_vector.tolist()}
-            centroid_documents.append(centroid_document)
-
-        return centroid_documents
-
-    def list_closest_to_center(
-        self,
-        centroid_vector_fields: List[str] = None,
-        cluster_field: str = None,
-        approx: int = 0,
-        sum_fields: bool = True,
-        page: int = 1,
-        similarity_metric: str = "cosine",
-        min_score: float = 0,
-        include_vector: bool = False,
-        include_count: bool = True,
-        include_relevance: bool = False,
-        page_size: int = 20,
-        cluster_properties_filter: Dict[str, Any] = None,
-        cluster_ids: List[str] = None,
-        filters: List[Filter] = None,
-        select_fields: List[str] = None,
-    ):
-        return self._dataset.api._list_closest_to_center(
-            dataset_id=self.dataset_id,
-            alias=self._cluster_alias,
-            vector_fields=self._cluster_field[0],
-            centroid_vector_fields=centroid_vector_fields,
-            cluster_field=cluster_field,
-            approx=approx,
-            sum_fields=sum_fields,
-            page=page,
-            similarity_metric=similarity_metric,
-            min_score=min_score,
-            include_vector=include_vector,
-            include_count=include_count,
-            include_relevance=include_relevance,
-            page_size=page_size,
-            cluster_properties_filter=cluster_properties_filter,
-            cluster_ids=cluster_ids,
-            filters=filters,
-            select_fields=select_fields,
-        )
-
-
-class KeyphraseField(Field):
-    def __init__(self, dataset, field: str):
-        super().__init__(dataset=dataset, field=field)
-        _, *middle_fields, alias = field.split(".")
-        self._keyphrase_field = ".".join(middle_fields)
-        self._keyphrase_alias = alias
-
-    def get_keyphrase(self, keyphrase_id: str):
-        return self._dataset.api._get_keyphrase(
-            dataset_id=self.dataset_id,
-            field=self._keyphrase_field,
-            alias=self._keyphrase_alias,
-            keyphrase_id=keyphrase_id,
-        )
-
-    def update_keyphrase(
-        self,
-        keyphrase_id: str,
-        keyphrase: Union[Keyphrase, str],
-        frequency: int = 0,
-        ancestors: list = None,
-        parents: list = None,
-        metadata: dict = None,
-        keyphrase_score: float = 0,
-        level: int = 0,
-    ):
-        if isinstance(update, Keyphrase):
-            update = asdict(update)
-        return self._dataset.api._update_keyphrase(
-            dataset_id=self._dataset._dataset_id,
-            field=self._keyphrase_field,
-            alias=self._keyphrase_alias,
-            keyphrase_id=keyphrase_id,
-            keyphrase=keyphrase,
-            frequency=frequency,
-            ancestors=ancestors,
-            parents=parents,
-            metadata=metadata,
-            keyphrase_score=keyphrase_score,
-            level=level,
-        )
-
-    def delete_keyphrase(self, keyphrase_id: str):
-        return self._dataset.api._delete_keyphrase(
-            dataset_id=self.dataset_id,
-            field=self._keyphrase_field,
-            alias=self._keyphrase_alias,
-            keyphrase_id=keyphrase_id,
-        )
-
-    def bulk_update_keyphrases(self, updates: List[Union[Keyphrase, dict]]):
-        updates_list = []
-        for update in updates:
-            if isinstance(update, Keyphrase):
-                updates_list.append(asdict(update))
-            elif isinstance(update, dict):
-                updates_list.append(update)
-        return self._dataset.api._bulk_update_keyphrase(
-            dataset_id=self.dataset_id, field=self._keyphrase_field, alias=self._keyphrase_alias, updates=updates_list
-        )
-
-    def list_keyphrases(self, page_size: int = 100, page: int = 1, sort: list = None):
-        return self._dataset.api._list_keyphrase(
-            dataset_id=self.dataset_id,
-            field=self._keyphrase_field,
-            alias=self._keyphrase_alias,
-            page_size=page_size,
-            page=page,
-            sort=[] if sort is None else sort,
-        )
+import uuid
+import numpy as np
+
+from typing import Dict, Any, List, Optional, Union
+
+from ai_transform.types import Filter
+from ai_transform.utils.document_list import DocumentList
+from ai_transform.utils.keyphrase import Keyphrase
+from dataclasses import asdict
+
+
+class Field:
+    def __init__(self, dataset, field: str):
+        from ai_transform.dataset.dataset import Dataset
+
+        self._dataset: Dataset = dataset
+        self._field = field
+        if field != "_id":
+            self._dtype = dataset.schema.get(field)
+        else:
+            self._dtype = None
+        self._filter_type = self._get_filter_type()
+
+    @property
+    def dataset(self):
+        return self._dataset
+
+    @property
+    def dataset_id(self):
+        return self._dataset.dataset_id
+
+    @property
+    def field(self):
+        return self._field
+
+    def list_field_parents(self) -> List[str]:
+        all_field_children = self.dataset.list_field_children()["results"]
+        field_parents = []
+        for relationship in all_field_children:
+            if self.field in relationship["field_children"]:
+                field_parents += [relationship["field"]]
+        return list(set(field_parents))
+
+    def list_field_children(self) -> List[str]:
+        all_field_children = self.dataset.list_field_children()["results"]
+        field_children = []
+        for relationship in all_field_children:
+            if relationship["field"] == self.field:
+                field_children += relationship["field_children"]
+        return list(set(field_children))
+
+    def add_field_children(
+        self,
+        field_children: List[str],
+        fieldchildren_id: str = None,
+        metadata: Dict[str, Any] = None,
+        recursive: bool = False,
+    ):
+        if fieldchildren_id is None:
+            fieldchildren_id = str(uuid.uuid4())
+        return self.dataset.set_field_children(
+            fieldchildren_id=fieldchildren_id,
+            field=self.field,
+            field_children=field_children,
+            recursive=recursive,
+            metadata=metadata,
+        )
+
+    def _get_filter_type(self) -> str:
+        if self._dtype == "numeric":
+            filter_type = "numeric"
+        elif self._dtype == "date":
+            filter_type = "date"
+        elif self._dtype is None:
+            filter_type = "ids"
+        else:
+            filter_type = "exact_match"
+        return filter_type
+
+    def __eq__(self, other: Union[str, float, int, bool, None], filter_type: Optional[str] = None) -> Filter:
+        if filter_type is None:
+            filter_type = self._filter_type
+        return [{"field": self._field, "filter_type": filter_type, "condition": "==", "condition_value": other}]
+
+    def __lt__(self, other: Union[str, float, int, bool, None], filter_type: Optional[str] = None) -> Filter:
+        if filter_type is None:
+            filter_type = self._filter_type
+        return [{"field": self._field, "filter_type": filter_type, "condition": "<", "condition_value": other}]
+
+    def __le__(self, other: Union[str, float, int, bool, None], filter_type: Optional[str] = None) -> Filter:
+        if filter_type is None:
+            filter_type = self._filter_type
+        return [{"field": self._field, "filter_type": filter_type, "condition": "<=", "condition_value": other}]
+
+    def __gt__(self, other: Union[str, float, int, bool, None], filter_type: Optional[str] = None) -> Filter:
+        if filter_type is None:
+            filter_type = self._filter_type
+        return [{"field": self._field, "filter_type": filter_type, "condition": ">", "condition_value": other}]
+
+    def __ge__(self, other: Union[str, float, int, bool, None], filter_type: Optional[str] = None) -> Filter:
+        if filter_type is None:
+            filter_type = self._filter_type
+        return [{"field": self._field, "filter_type": filter_type, "condition": ">=", "condition_value": other}]
+
+    def contains(self, other: str) -> Filter:
+        return [{"field": self._field, "filter_type": "contains", "condition": "==", "condition_value": other}]
+
+    def exists(self) -> Filter:
+        if "_chunk_" in self._field:
+            if self._field.endswith("_chunk_"):
+                parent_field = self._field
+            else:
+                parent_field = self._field.split(".")[0]
+
+            return [{"chunk": {"path": parent_field, "filters": [{"fieldExists": {"field": self._field}}]}}]
+        return [{"field": self._field, "filter_type": "exists", "condition": "==", "condition_value": " "}]
+
+    def not_exists(self) -> Filter:
+        return [{"field": self._field, "filter_type": "exists", "condition": "!=", "condition_value": " "}]
+
+    def insert_centroids(self, centroid_documents: DocumentList):
+        raise NotImplementedError(f"`insert_centroids` not available for non-vector fields")
+
+    def label_openai(
+        self,
+        field: str,
+        question_suffix: str,
+        accuracy: int = 4,
+        cluster_ids: list = None,
+        dont_save_summaries: bool = True,
+        filters: list = None,
+    ):
+        raise NotImplementedError(f"`label_openai` not available for non-vector fields")
+
+    def get_centroids(
+        self, page_size: int = 5, page: int = 1, cluster_ids: Optional[List] = None, include_vector: bool = False
+    ):
+        raise NotImplementedError(f"`get_centroids` not available for non-vector fields")
+
+    def get_all_centroids(self):
+        raise NotImplementedError(f"`get_all_centroids` not available for non-vector fields")
+
+    def create_centroid_documents(self):
+        raise NotImplementedError(f"`create_centroid_documents` not available for non-vector fields")
+
+    def list_closest_to_center(
+        self,
+        centroid_vector_fields: List[str],
+        cluster_field: str,
+        approx: int = 0,
+        sum_fields: bool = True,
+        page: int = 1,
+        similarity_metric: str = "cosine",
+        min_score: float = 0,
+        include_vector: bool = False,
+        include_count: bool = True,
+        include_relevance: bool = False,
+        page_size: int = 20,
+        cluster_properties_filter: Dict[str, Any] = None,
+        cluster_ids: List[str] = None,
+        filters: List[Filter] = None,
+        select_fields: List[str] = None,
+    ):
+        raise NotImplementedError("`list_closest_to_center` not available for non-vector fields")
+
+    def get_keyphrase(self, keyphrase_id: str):
+        raise NotImplementedError(f"`get_keyphrase` not available for non-keyphrase fields")
+
+    def update_keyphrase(
+        self,
+        keyphrase_id: str,
+        alias: str,
+        keyphrase: str,
+        frequency: int = 0,
+        ancestors: list = None,
+        parents: list = None,
+        metadata: dict = None,
+        keyphrase_score: float = 0,
+        level: int = 0,
+    ):
+        raise NotImplementedError(f"`update_keyphrase` not available for non-keyphrase fields")
+
+    def delete_keyphrase(self, keyphrase_id: str):
+        raise NotImplementedError(f"`delete_keyphrase` not available for non-keyphrase fields")
+
+    def bulk_update_keyphrases(self, updates: List[Union[Keyphrase, dict]]):
+        raise NotImplementedError(f"`bulk_update_keyphrases` not available for non-keyphrase fields")
+
+    def list_keyphrases(self, page_size: int = 100, page: int = 1, sort: list = None):
+        raise NotImplementedError(f"`list_keyphrases` not available for non-keyphrase fields")
+
+
+class ClusterField(Field):
+    def __init__(self, dataset, field: str):
+        super().__init__(dataset=dataset, field=field)
+        _, *middle_fields, alias = field.split(".")
+        self._cluster_field = ".".join(middle_fields)
+        self._cluster_alias = alias
+
+    def insert_centroids(self, centroid_documents: Union[List[Dict[str, Any]], DocumentList]):
+        if isinstance(centroid_documents, DocumentList):
+            centroid_documents = centroid_documents.to_json()
+        return self._dataset.api._insert_centroids(
+            dataset_id=self.dataset_id,
+            cluster_centers=centroid_documents,
+            vector_fields=[self._cluster_field],
+            alias=self._cluster_alias,
+        )
+
+    def get_centroids(
+        self, page_size: int = 5, page: int = 1, cluster_ids: Optional[List] = None, include_vector: bool = False
+    ):
+        return self._dataset.api._get_centroids(
+            dataset_id=self.dataset_id,
+            vector_fields=[self._cluster_field],
+            alias=self._cluster_alias,
+            page_size=page_size,
+            page=page,
+            cluster_ids=cluster_ids,
+            include_vector=include_vector,
+        )
+
+    def get_all_centroids(self, page_size: int = 5, cluster_ids: Optional[List] = None, include_vector: bool = False):
+        """
+        Get all centroids and returns as a dictionary for easy access
+        """
+        all_centroids = {"results": []}
+        page = 1
+        while True:
+            res = self._dataset.api._get_centroids(
+                dataset_id=self.dataset_id,
+                vector_fields=[self._cluster_field],
+                alias=self._cluster_alias,
+                page_size=page_size,
+                cluster_ids=cluster_ids,
+                include_vector=include_vector,
+                page=page,
+            )["results"]
+            if len(res) == 0:
+                break
+            else:
+                all_centroids["results"] += res
+                page += 1
+        return all_centroids
+
+    def label_openai(
+        self,
+        field: str,
+        question_suffix: str,
+        accuracy: int = 4,
+        cluster_ids: list = None,
+        dont_save_summaries: bool = True,
+        filters: list = None,
+    ):
+        return self._dataset.api._label_openai(
+            dataset_id=self.dataset_id,
+            vector_field=self._cluster_field,
+            field=field,
+            alias=self._cluster_alias,
+            question_suffix=question_suffix,
+            accuracy=accuracy,
+            cluster_ids=cluster_ids if cluster_ids is not None else [],
+            dont_save_summaries=dont_save_summaries,
+            filters=filters if filters is not None else [],
+        )
+
+    def create_centroid_documents(self):
+        documents = self._dataset.get_all_documents(select_fields=[self._cluster_field, self._field])
+        documents = documents["documents"]
+
+        vectors = np.array([document[self._cluster_field] for document in documents])
+
+        labels = [document[self._field] for document in documents]
+
+        label_map = {}
+        for label in labels:
+            if label not in label_map:
+                label_map[label] = len(label_map)
+
+        n_clusters = len(label_map)
+        centroid_documents = []
+
+        selected_vectors: np.ndarray
+        centroid_vector: np.ndarray
+
+        label_indices = np.array([label_map[label] for label in labels])
+
+        for index in range(n_clusters):
+            selected_vectors = vectors[label_indices == index]
+            centroid_vector = selected_vectors.mean(0)
+
+            centroid_document = {"_id": f"cluster_{index}", f"{self._cluster_field}": centroid_vector.tolist()}
+            centroid_documents.append(centroid_document)
+
+        return centroid_documents
+
+    def list_closest_to_center(
+        self,
+        centroid_vector_fields: List[str] = None,
+        cluster_field: str = None,
+        approx: int = 0,
+        sum_fields: bool = True,
+        page: int = 1,
+        similarity_metric: str = "cosine",
+        min_score: float = 0,
+        include_vector: bool = False,
+        include_count: bool = True,
+        include_relevance: bool = False,
+        page_size: int = 20,
+        cluster_properties_filter: Dict[str, Any] = None,
+        cluster_ids: List[str] = None,
+        filters: List[Filter] = None,
+        select_fields: List[str] = None,
+    ):
+        return self._dataset.api._list_closest_to_center(
+            dataset_id=self.dataset_id,
+            alias=self._cluster_alias,
+            vector_fields=self._cluster_field[0],
+            centroid_vector_fields=centroid_vector_fields,
+            cluster_field=cluster_field,
+            approx=approx,
+            sum_fields=sum_fields,
+            page=page,
+            similarity_metric=similarity_metric,
+            min_score=min_score,
+            include_vector=include_vector,
+            include_count=include_count,
+            include_relevance=include_relevance,
+            page_size=page_size,
+            cluster_properties_filter=cluster_properties_filter,
+            cluster_ids=cluster_ids,
+            filters=filters,
+            select_fields=select_fields,
+        )
+
+
+class KeyphraseField(Field):
+    def __init__(self, dataset, field: str):
+        super().__init__(dataset=dataset, field=field)
+        _, *middle_fields, alias = field.split(".")
+        self._keyphrase_field = ".".join(middle_fields)
+        self._keyphrase_alias = alias
+
+    def get_keyphrase(self, keyphrase_id: str):
+        return self._dataset.api._get_keyphrase(
+            dataset_id=self.dataset_id,
+            field=self._keyphrase_field,
+            alias=self._keyphrase_alias,
+            keyphrase_id=keyphrase_id,
+        )
+
+    def update_keyphrase(
+        self,
+        keyphrase_id: str,
+        keyphrase: Union[Keyphrase, str],
+        frequency: int = 0,
+        ancestors: list = None,
+        parents: list = None,
+        metadata: dict = None,
+        keyphrase_score: float = 0,
+        level: int = 0,
+    ):
+        if isinstance(update, Keyphrase):
+            update = asdict(update)
+        return self._dataset.api._update_keyphrase(
+            dataset_id=self._dataset._dataset_id,
+            field=self._keyphrase_field,
+            alias=self._keyphrase_alias,
+            keyphrase_id=keyphrase_id,
+            keyphrase=keyphrase,
+            frequency=frequency,
+            ancestors=ancestors,
+            parents=parents,
+            metadata=metadata,
+            keyphrase_score=keyphrase_score,
+            level=level,
+        )
+
+    def delete_keyphrase(self, keyphrase_id: str):
+        return self._dataset.api._delete_keyphrase(
+            dataset_id=self.dataset_id,
+            field=self._keyphrase_field,
+            alias=self._keyphrase_alias,
+            keyphrase_id=keyphrase_id,
+        )
+
+    def bulk_update_keyphrases(self, updates: List[Union[Keyphrase, dict]]):
+        updates_list = []
+        for update in updates:
+            if isinstance(update, Keyphrase):
+                updates_list.append(asdict(update))
+            elif isinstance(update, dict):
+                updates_list.append(update)
+        return self._dataset.api._bulk_update_keyphrase(
+            dataset_id=self.dataset_id, field=self._keyphrase_field, alias=self._keyphrase_alias, updates=updates_list
+        )
+
+    def list_keyphrases(self, page_size: int = 100, page: int = 1, sort: list = None):
+        return self._dataset.api._list_keyphrase(
+            dataset_id=self.dataset_id,
+            field=self._keyphrase_field,
+            alias=self._keyphrase_alias,
+            page_size=page_size,
+            page=page,
+            sort=[] if sort is None else sort,
+        )
```

### Comparing `ai_transform-0.32.3/ai_transform/engine/multipass_engine.py` & `ai_transform-0.32.4/ai_transform/engine/multipass_engine.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,114 +1,114 @@
-import logging
-
-from typing import Optional, Sequence, List
-
-from ai_transform.logger import format_logging_info, ic
-from ai_transform.dataset.dataset import Dataset
-from ai_transform.operator.abstract_operator import AbstractOperator
-from ai_transform.engine.abstract_engine import AbstractEngine
-from ai_transform.utils.document import Document
-from ai_transform.types import Filter
-
-
-class MultiPassEngine(AbstractEngine):
-    def __init__(
-        self,
-        dataset: Dataset = None,
-        operators: Sequence[AbstractOperator] = None,
-        filters: Optional[List[Filter]] = None,
-        select_fields: Optional[List[str]] = None,
-        pull_chunksize: Optional[int] = 3000,
-        refresh: bool = True,
-        after_id: Optional[List[str]] = None,
-        worker_number: int = None,
-        total_workers: int = None,
-        check_for_missing_fields: bool = True,
-        output_to_status: Optional[bool] = False,
-        documents: Optional[List[object]] = None,
-        limit_documents: Optional[int] = None,
-        transform_chunksize: int = 20,
-        show_progress_bar: bool = True,
-    ):
-        super().__init__(
-            dataset=dataset,
-            operators=operators,
-            filters=filters,
-            select_fields=select_fields,
-            pull_chunksize=pull_chunksize,
-            refresh=refresh,
-            after_id=after_id,
-            worker_number=worker_number,
-            total_workers=total_workers,
-            check_for_missing_fields=check_for_missing_fields,
-            output_to_status=output_to_status,
-            documents=documents,
-            limit_documents=limit_documents,
-        )
-
-        self._transform_chunksize = min(self.pull_chunksize, transform_chunksize)
-        self._show_progress_bar = show_progress_bar
-
-    def handle_upsert(self, batch_index: int, batch_to_insert: List[Document]):
-        """
-        This functions handles the reinsertion of new transformed data back
-        into the dataset. This could happen for two reasons:
-            1. For a regular workflow
-            2. For outputting to status
-        """
-        if self.output_to_status:
-            # Store in output documents
-            self.extend_output_documents([document.to_json() for document in batch_to_insert])
-        else:
-            # Store in dataset
-            # We want to make sure the schema updates
-            # on the first chunk upserting
-            if batch_index < self.MAX_SCHEMA_UPDATE_LIMITER:
-                ingest_in_background = False
-            else:
-                ingest_in_background = True
-
-            result = self.update_chunk(
-                batch_to_insert,
-                update_schema=batch_index < self.MAX_SCHEMA_UPDATE_LIMITER,
-                ingest_in_background=ingest_in_background,
-            )
-            ic(result)
-
-    def _operate(self, operator: AbstractOperator, mini_batch: List[Document]):
-        try:
-            # note: do not put an IF inside ths try-except-else loop - the if code will not work
-            transformed_batch = operator(mini_batch)
-        except Exception as e:
-            ic(e)
-            ic({"chunk_ids": self._get_chunks_ids(mini_batch)})
-        else:
-            # if there is no exception then this block will be executed
-            # we only update schema on the first chunk
-            # otherwise it breaks down how the backend handles
-            # schema updates
-            self._successful_documents += len(mini_batch)
-            return transformed_batch
-
-    def apply(self) -> None:
-        """
-        Returns the ratio of successful chunks / total chunks needed to iterate over the dataset
-        """
-        for operator_index, operator in enumerate(self.operators):
-            operator.pre_hooks(self._dataset)
-
-            iterator = self.get_iterator()
-
-            for batch_index, mega_batch in enumerate(
-                self.api_progress(iterator, pass_index=operator_index, n_passes=len(self.operators))
-            ):
-                batch_to_insert: List[Document] = []
-
-                for mini_batch in AbstractEngine.chunk_documents(self._transform_chunksize, mega_batch):
-                    transformed_batch = self._operate(operator, mini_batch)
-                    if transformed_batch is not None:
-                        batch_to_insert += transformed_batch
-
-                if batch_to_insert:
-                    self.handle_upsert(batch_index, batch_to_insert)
-
-            operator.post_hooks(self._dataset)
+import logging
+
+from typing import Optional, Sequence, List
+
+from ai_transform.logger import format_logging_info, ic
+from ai_transform.dataset.dataset import Dataset
+from ai_transform.operator.abstract_operator import AbstractOperator
+from ai_transform.engine.abstract_engine import AbstractEngine
+from ai_transform.utils.document import Document
+from ai_transform.types import Filter
+
+
+class MultiPassEngine(AbstractEngine):
+    def __init__(
+        self,
+        dataset: Dataset = None,
+        operators: Sequence[AbstractOperator] = None,
+        filters: Optional[List[Filter]] = None,
+        select_fields: Optional[List[str]] = None,
+        pull_chunksize: Optional[int] = 3000,
+        refresh: bool = True,
+        after_id: Optional[List[str]] = None,
+        worker_number: int = None,
+        total_workers: int = None,
+        check_for_missing_fields: bool = True,
+        output_to_status: Optional[bool] = False,
+        documents: Optional[List[object]] = None,
+        limit_documents: Optional[int] = None,
+        transform_chunksize: int = 20,
+        show_progress_bar: bool = True,
+    ):
+        super().__init__(
+            dataset=dataset,
+            operators=operators,
+            filters=filters,
+            select_fields=select_fields,
+            pull_chunksize=pull_chunksize,
+            refresh=refresh,
+            after_id=after_id,
+            worker_number=worker_number,
+            total_workers=total_workers,
+            check_for_missing_fields=check_for_missing_fields,
+            output_to_status=output_to_status,
+            documents=documents,
+            limit_documents=limit_documents,
+        )
+
+        self._transform_chunksize = min(self.pull_chunksize, transform_chunksize)
+        self._show_progress_bar = show_progress_bar
+
+    def handle_upsert(self, batch_index: int, batch_to_insert: List[Document]):
+        """
+        This functions handles the reinsertion of new transformed data back
+        into the dataset. This could happen for two reasons:
+            1. For a regular workflow
+            2. For outputting to status
+        """
+        if self.output_to_status:
+            # Store in output documents
+            self.extend_output_documents([document.to_json() for document in batch_to_insert])
+        else:
+            # Store in dataset
+            # We want to make sure the schema updates
+            # on the first chunk upserting
+            if batch_index < self.MAX_SCHEMA_UPDATE_LIMITER:
+                ingest_in_background = False
+            else:
+                ingest_in_background = True
+
+            result = self.update_chunk(
+                batch_to_insert,
+                update_schema=batch_index < self.MAX_SCHEMA_UPDATE_LIMITER,
+                ingest_in_background=ingest_in_background,
+            )
+            ic(result)
+
+    def _operate(self, operator: AbstractOperator, mini_batch: List[Document]):
+        try:
+            # note: do not put an IF inside ths try-except-else loop - the if code will not work
+            transformed_batch = operator(mini_batch)
+        except Exception as e:
+            ic(e)
+            ic({"chunk_ids": self._get_chunks_ids(mini_batch)})
+        else:
+            # if there is no exception then this block will be executed
+            # we only update schema on the first chunk
+            # otherwise it breaks down how the backend handles
+            # schema updates
+            self._successful_documents += len(mini_batch)
+            return transformed_batch
+
+    def apply(self) -> None:
+        """
+        Returns the ratio of successful chunks / total chunks needed to iterate over the dataset
+        """
+        for operator_index, operator in enumerate(self.operators):
+            operator.pre_hooks(self._dataset)
+
+            iterator = self.get_iterator()
+
+            for batch_index, mega_batch in enumerate(
+                self.api_progress(iterator, pass_index=operator_index, n_passes=len(self.operators))
+            ):
+                batch_to_insert: List[Document] = []
+
+                for mini_batch in AbstractEngine.chunk_documents(self._transform_chunksize, mega_batch):
+                    transformed_batch = self._operate(operator, mini_batch)
+                    if transformed_batch is not None:
+                        batch_to_insert += transformed_batch
+
+                if batch_to_insert:
+                    self.handle_upsert(batch_index, batch_to_insert)
+
+            operator.post_hooks(self._dataset)
```

### Comparing `ai_transform-0.32.3/ai_transform/engine/stable_engine.py` & `ai_transform-0.32.4/ai_transform/engine/stable_engine.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-"""
-    Stable Engine Pseudo-algorithm-
-        1. Downloads about 1000 documents.
-        2. Processes it in much smaller chunks.
-        3. Upserts all 1000 documents.
-        4. Repeat until dataset has finished looping
-
-    We download a large chunk and upsert large chunks to avoid hammering
-    our servers.
-
-"""
-import logging
-
-from typing import Optional, List
-
-from ai_transform.logger import ic, format_logging_info
-from ai_transform.dataset.dataset import Dataset
-from ai_transform.operator.abstract_operator import AbstractOperator
-from ai_transform.engine.abstract_engine import AbstractEngine
-from ai_transform.utils.document import Document
-from ai_transform.types import Filter
-
-
-class StableEngine(AbstractEngine):
-    def __init__(
-        self,
-        dataset: Dataset = None,
-        operator: AbstractOperator = None,
-        filters: Optional[List[Filter]] = None,
-        select_fields: Optional[List[str]] = None,
-        pull_chunksize: Optional[int] = 3000,
-        refresh: bool = True,
-        after_id: Optional[List[str]] = None,
-        worker_number: int = None,
-        total_workers: int = None,
-        check_for_missing_fields: bool = True,
-        output_to_status: Optional[bool] = False,
-        documents: Optional[List[object]] = None,
-        limit_documents: Optional[int] = None,
-        transform_chunksize: int = 20,
-        show_progress_bar: bool = True,
-    ):
-        super().__init__(
-            dataset=dataset,
-            operator=operator,
-            filters=filters,
-            select_fields=select_fields,
-            pull_chunksize=pull_chunksize,
-            refresh=refresh,
-            after_id=after_id,
-            worker_number=worker_number,
-            total_workers=total_workers,
-            check_for_missing_fields=check_for_missing_fields,
-            output_to_status=output_to_status,
-            documents=documents,
-            limit_documents=limit_documents,
-        )
-
-        self._transform_chunksize = min(self.pull_chunksize, transform_chunksize)
-        self._show_progress_bar = show_progress_bar
-
-    def handle_upsert(self, batch_index: int, batch_to_insert: List[Document]):
-        if self.output_to_status:
-            # Store in output documents
-            self.extend_output_documents([document.to_json() for document in batch_to_insert])
-        else:
-            # Store in dataset
-            # We want to make sure the schema updates
-            # on the first chunk upserting
-            if batch_index < self.MAX_SCHEMA_UPDATE_LIMITER:
-                ingest_in_background = False
-            else:
-                ingest_in_background = True
-
-            result = self.update_chunk(
-                batch_to_insert,
-                update_schema=batch_index < self.MAX_SCHEMA_UPDATE_LIMITER,
-                ingest_in_background=ingest_in_background,
-            )
-            ic(result)
-
-    def apply(self) -> None:
-        """
-        Returns the ratio of successful chunks / total chunks needed to iterate over the dataset
-        """
-        iterator = self.get_iterator()
-
-        self.operator.pre_hooks(self._dataset)
-        for batch_index, mega_batch in enumerate(self.api_progress(iterator)):
-            batch_to_insert: List[Document] = []
-
-            for mini_batch in AbstractEngine.chunk_documents(self._transform_chunksize, mega_batch):
-                transformed_batch = self._operate(mini_batch)
-                if transformed_batch is not None:
-                    batch_to_insert += transformed_batch
-
-            self.handle_upsert(batch_index, batch_to_insert)
-
-        self.operator.post_hooks(self._dataset)
+"""
+    Stable Engine Pseudo-algorithm-
+        1. Downloads about 1000 documents.
+        2. Processes it in much smaller chunks.
+        3. Upserts all 1000 documents.
+        4. Repeat until dataset has finished looping
+
+    We download a large chunk and upsert large chunks to avoid hammering
+    our servers.
+
+"""
+import logging
+
+from typing import Optional, List
+
+from ai_transform.logger import ic, format_logging_info
+from ai_transform.dataset.dataset import Dataset
+from ai_transform.operator.abstract_operator import AbstractOperator
+from ai_transform.engine.abstract_engine import AbstractEngine
+from ai_transform.utils.document import Document
+from ai_transform.types import Filter
+
+
+class StableEngine(AbstractEngine):
+    def __init__(
+        self,
+        dataset: Dataset = None,
+        operator: AbstractOperator = None,
+        filters: Optional[List[Filter]] = None,
+        select_fields: Optional[List[str]] = None,
+        pull_chunksize: Optional[int] = 3000,
+        refresh: bool = True,
+        after_id: Optional[List[str]] = None,
+        worker_number: int = None,
+        total_workers: int = None,
+        check_for_missing_fields: bool = True,
+        output_to_status: Optional[bool] = False,
+        documents: Optional[List[object]] = None,
+        limit_documents: Optional[int] = None,
+        transform_chunksize: int = 20,
+        show_progress_bar: bool = True,
+    ):
+        super().__init__(
+            dataset=dataset,
+            operator=operator,
+            filters=filters,
+            select_fields=select_fields,
+            pull_chunksize=pull_chunksize,
+            refresh=refresh,
+            after_id=after_id,
+            worker_number=worker_number,
+            total_workers=total_workers,
+            check_for_missing_fields=check_for_missing_fields,
+            output_to_status=output_to_status,
+            documents=documents,
+            limit_documents=limit_documents,
+        )
+
+        self._transform_chunksize = min(self.pull_chunksize, transform_chunksize)
+        self._show_progress_bar = show_progress_bar
+
+    def handle_upsert(self, batch_index: int, batch_to_insert: List[Document]):
+        if self.output_to_status:
+            # Store in output documents
+            self.extend_output_documents([document.to_json() for document in batch_to_insert])
+        else:
+            # Store in dataset
+            # We want to make sure the schema updates
+            # on the first chunk upserting
+            if batch_index < self.MAX_SCHEMA_UPDATE_LIMITER:
+                ingest_in_background = False
+            else:
+                ingest_in_background = True
+
+            result = self.update_chunk(
+                batch_to_insert,
+                update_schema=batch_index < self.MAX_SCHEMA_UPDATE_LIMITER,
+                ingest_in_background=ingest_in_background,
+            )
+            ic(result)
+
+    def apply(self) -> None:
+        """
+        Returns the ratio of successful chunks / total chunks needed to iterate over the dataset
+        """
+        iterator = self.get_iterator()
+
+        self.operator.pre_hooks(self._dataset)
+        for batch_index, mega_batch in enumerate(self.api_progress(iterator)):
+            batch_to_insert: List[Document] = []
+
+            for mini_batch in AbstractEngine.chunk_documents(self._transform_chunksize, mega_batch):
+                transformed_batch = self._operate(mini_batch)
+                if transformed_batch is not None:
+                    batch_to_insert += transformed_batch
+
+            self.handle_upsert(batch_index, batch_to_insert)
+
+        self.operator.post_hooks(self._dataset)
```

### Comparing `ai_transform-0.32.3/ai_transform/logger.py` & `ai_transform-0.32.4/ai_transform/logger.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-import pprint
-import logging
-import datetime
-from icecream import ic
-from typing import Dict, Any, List
-from ai_transform.utils.document import Document
-from ai_transform.utils.document_list import DocumentList
-
-
-def format_logging_info(info: Dict[str, Any], indent=4, width=80, depth=None, compact=True, sort_dicts=False):
-    return "\n" + pprint.pformat(info, indent=indent, width=width, depth=depth, compact=compact, sort_dicts=sort_dicts)
-
-
-class Logger:
-    def __init__(self):
-        self._logger = logging.getLogger("WORKFLOW")
-        logging.basicConfig(format="%(asctime)s %(levelname)s %(message)s", datefmt="%Y-%m-%d %H:%M:%S")
-        self._logger.setLevel(logging.DEBUG)
-
-    def __call__(self, info: Any, no_vectors: bool = True) -> None:
-        if isinstance(info, Document):
-            info_to_log = info.to_json()
-            if no_vectors:
-                info_to_log = {k: v for k, v in info.items() if "_vector_" not in k}
-
-        elif isinstance(info, DocumentList):
-            info_to_log = [document.to_json() for document in info]
-        elif isinstance(info, List):
-            if isinstance(info[0], Document):
-                info_to_log = [document.to_json() for document in info]
-
-        else:
-            info_to_log = info
-
-        self._logger.debug(format_logging_info(info_to_log))
-
-
-def time_format():
-    timestamp = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
-    return f"{timestamp} | "
-
-
-ic.configureOutput(prefix=time_format, includeContext=True)
-# Change all printing statements
+import pprint
+import logging
+import datetime
+from icecream import ic
+from typing import Dict, Any, List
+from ai_transform.utils.document import Document
+from ai_transform.utils.document_list import DocumentList
+
+
+def format_logging_info(info: Dict[str, Any], indent=4, width=80, depth=None, compact=True, sort_dicts=False):
+    return "\n" + pprint.pformat(info, indent=indent, width=width, depth=depth, compact=compact, sort_dicts=sort_dicts)
+
+
+class Logger:
+    def __init__(self):
+        self._logger = logging.getLogger("WORKFLOW")
+        logging.basicConfig(format="%(asctime)s %(levelname)s %(message)s", datefmt="%Y-%m-%d %H:%M:%S")
+        self._logger.setLevel(logging.DEBUG)
+
+    def __call__(self, info: Any, no_vectors: bool = True) -> None:
+        if isinstance(info, Document):
+            info_to_log = info.to_json()
+            if no_vectors:
+                info_to_log = {k: v for k, v in info.items() if "_vector_" not in k}
+
+        elif isinstance(info, DocumentList):
+            info_to_log = [document.to_json() for document in info]
+        elif isinstance(info, List):
+            if isinstance(info[0], Document):
+                info_to_log = [document.to_json() for document in info]
+
+        else:
+            info_to_log = info
+
+        self._logger.debug(format_logging_info(info_to_log))
+
+
+def time_format():
+    timestamp = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
+    return f"{timestamp} | "
+
+
+ic.configureOutput(prefix=time_format, includeContext=True)
+# Change all printing statements
```

### Comparing `ai_transform-0.32.3/ai_transform/operator/dense_operator.py` & `ai_transform-0.32.4/ai_transform/operator/dense_operator.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-import logging
-
-from abc import abstractmethod
-
-from typing import Dict, Sequence
-
-from ai_transform.operator.abstract_operator import AbstractOperator
-from ai_transform.utils.document import Document
-from ai_transform.utils.document_list import DocumentList
-
-logger = logging.getLogger(__file__)
-
-
-DatasetID = str
-DenseOperatorOutput = Dict[DatasetID, Sequence[Document]]
-
-
-BAD_OPERATOR_MESSAGE = (
-    "please ensure the output of the operator is a dict that is a mapping of dataset_ids to documents"
-)
-
-
-class DenseOperator(AbstractOperator):
-    def __call__(self, old_documents: DocumentList) -> DenseOperatorOutput:
-        datum = self.transform(old_documents)
-        if not isinstance(datum, dict):
-            raise ValueError(BAD_OPERATOR_MESSAGE)
-        for _, documents in datum.items():
-            if not isinstance(documents, Sequence):
-                raise ValueError(BAD_OPERATOR_MESSAGE)
-        return datum
-
-    @abstractmethod
-    def transform(self, documents: DocumentList) -> DenseOperatorOutput:
-        raise NotImplementedError
+import logging
+
+from abc import abstractmethod
+
+from typing import Dict, Sequence
+
+from ai_transform.operator.abstract_operator import AbstractOperator
+from ai_transform.utils.document import Document
+from ai_transform.utils.document_list import DocumentList
+
+logger = logging.getLogger(__file__)
+
+
+DatasetID = str
+DenseOperatorOutput = Dict[DatasetID, Sequence[Document]]
+
+
+BAD_OPERATOR_MESSAGE = (
+    "please ensure the output of the operator is a dict that is a mapping of dataset_ids to documents"
+)
+
+
+class DenseOperator(AbstractOperator):
+    def __call__(self, old_documents: DocumentList) -> DenseOperatorOutput:
+        datum = self.transform(old_documents)
+        if not isinstance(datum, dict):
+            raise ValueError(BAD_OPERATOR_MESSAGE)
+        for _, documents in datum.items():
+            if not isinstance(documents, Sequence):
+                raise ValueError(BAD_OPERATOR_MESSAGE)
+        return datum
+
+    @abstractmethod
+    def transform(self, documents: DocumentList) -> DenseOperatorOutput:
+        raise NotImplementedError
```

### Comparing `ai_transform-0.32.3/ai_transform/timer.py` & `ai_transform-0.32.4/ai_transform/timer.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import os
-import time
-
-
-class Timer:
-    def start(self) -> None:
-        if "_WORKFLOW_START_TIME" not in os.environ:
-            os.environ["_WORKFLOW_START_TIME"] = str(time.time())
-
-    def stop(self) -> float:
-        if "_WORKFLOW_FINISH_TIME" not in os.environ:
-            os.environ["_WORKFLOW_FINISH_TIME"] = str(time.time())
-
-            _WORKFLOW_START_TIME = float(os.getenv("_WORKFLOW_START_TIME"))
-            _WORKFLOW_FINISH_TIME = float(os.getenv("_WORKFLOW_FINISH_TIME"))
-
-            return _WORKFLOW_FINISH_TIME - _WORKFLOW_START_TIME
+import os
+import time
+
+
+class Timer:
+    def start(self) -> None:
+        if "_WORKFLOW_START_TIME" not in os.environ:
+            os.environ["_WORKFLOW_START_TIME"] = str(time.time())
+
+    def stop(self) -> float:
+        if "_WORKFLOW_FINISH_TIME" not in os.environ:
+            os.environ["_WORKFLOW_FINISH_TIME"] = str(time.time())
+
+            _WORKFLOW_START_TIME = float(os.getenv("_WORKFLOW_START_TIME"))
+            _WORKFLOW_FINISH_TIME = float(os.getenv("_WORKFLOW_FINISH_TIME"))
+
+            return _WORKFLOW_FINISH_TIME - _WORKFLOW_START_TIME
```

### Comparing `ai_transform-0.32.3/ai_transform/utils/document.py` & `ai_transform-0.32.4/ai_transform/utils/document.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,232 +1,232 @@
-import re
-import uuid
-import pprint
-
-from typing import Dict, Any
-from copy import deepcopy
-from typing import Any, Optional
-from collections import UserDict
-
-from ai_transform.utils.json_encoder import json_encoder
-
-
-class Document(UserDict):
-    def __repr__(self):
-        return pprint.pformat(self.to_json(), indent=4, width=40)
-
-    def __setitem__(self, key: Any, value: Any) -> None:
-        try:
-            fields = key.split(".")
-        except:
-            super().__setitem__(key, value)
-        else:
-            obj = self.data
-            for curr_field, next_field in zip(fields, fields[1:]):
-                if curr_field.isdigit():
-                    curr_field = int(curr_field)
-
-                if (isinstance(obj, dict) and (curr_field not in obj)) or (
-                    isinstance(obj, list) and (curr_field >= len(obj))
-                ):
-                    if next_field.isdigit():
-                        obj[curr_field] = [{}]
-                    else:
-                        if isinstance(curr_field, int):
-                            curr_field = min(len(obj) - 1, int(curr_field))
-                            if next_field not in obj[curr_field]:
-                                obj[curr_field] = {}
-                        else:
-                            obj[curr_field] = {}
-
-                try:
-                    obj = obj[curr_field]
-                except IndexError:
-                    obj = obj[0]
-                except KeyError:
-                    obj = obj[curr_field]
-
-            if fields[-1].isdigit():
-                field = min(len(obj) - 1, int(fields[-1]))
-            else:
-                field = fields[-1]
-            obj[field] = value
-
-    def __getitem__(self, key: Any) -> Any:
-        try:
-            fields = key.split(".")
-        except:
-            return super().__getitem__(key)
-        else:
-            obj = self.data
-            for field in fields[:-1]:
-                if field.isdigit():
-                    field = int(field)
-
-                obj = obj[field]
-
-            if fields[-1].isdigit():
-                field = min(len(obj) - 1, int(fields[-1]))
-            else:
-                field = fields[-1]
-            return obj[field]
-
-    def __delitem__(self, key):
-        try:
-            fields = key.split(".")
-        except:
-            return super().__getitem__(key)
-        else:
-            obj = self.data
-            for field in fields[:-1]:
-                if field.isdigit():
-                    field = int(field)
-
-                obj = obj[field]
-
-            if fields[-1].isdigit():
-                field = min(len(obj) - 1, int(fields[-1]))
-            else:
-                field = fields[-1]
-            del obj[field]
-
-    def get(self, key: Any, default: Optional[Any] = None) -> Any:
-        try:
-            return self.__getitem__(key)
-        except:
-            return default
-
-    def set(self, key: Any, value: Any) -> None:
-        self.__setitem__(key, value)
-
-    def keys(self):
-        def get_keys(dictionary: Dict[str, Any], prefix=""):
-            keys = []
-            for key, value in dictionary.items():
-                current_key = prefix + "." + key if prefix else key
-                if isinstance(value, dict):
-                    keys.extend(get_keys(value, current_key))
-                elif isinstance(value, list):
-                    for i, item in enumerate(value):
-                        if isinstance(item, dict):
-                            keys.extend(get_keys(item, current_key + "." + str(i)))
-                    keys.append(current_key)
-                else:
-                    keys.append(current_key)
-            if prefix:
-                keys.append(prefix)
-            return keys
-
-        keys = set(get_keys(self.data))
-
-        keys_to_add = set()
-        for key in keys:
-            subkeys = key.split(".")
-            for i in range(1, len(subkeys)):
-                keys_to_add.add(".".join(subkeys[:i]))
-        keys.update(keys_to_add)
-
-        return list(sorted(keys))
-
-    def __contains__(self, key) -> bool:
-        return key in self.keys()
-
-    def to_json(self):
-        return json_encoder(deepcopy(self.data))
-
-    def list_chunks(self):
-        """
-        List the available chunks inside of the document.
-        """
-        # based on conversation with API team
-        return [k for k in self.keys() if k.endswith("_chunk_")]
-
-    def get_chunk(self, chunk_field: str, field: str = None, default: str = None):
-        return [document.get(field, default) for document in self.get(chunk_field, default=default)]
-
-    def _create_chunk_documents(self, field: str, values: list, generate_id: bool = False):
-        """
-        create chunk documents based on a given field and value.
-        """
-        from ai_transform.utils.document_list import DocumentList
-
-        if generate_id:
-            docs = [{"_id": uuid.uuid4().__str__(), field: values[i], "_order_": i} for i in range(len(values))]
-        else:
-            docs = [{field: values[i], "_order_": i} for i in range(len(values))]
-        return DocumentList(docs)
-
-    def _calculate_offset(self, text_to_find, string):
-        try:
-            result = [{"start": m.start(), "end": m.end()} for m in re.finditer(text_to_find, string)]
-        except Exception as e:
-            import traceback
-
-            traceback.print_exc()
-            # this is the error this exception aims to solve
-            #     for m in re.finditer(text_to_find, string)
-            #     return _compile(pattern, flags).finditer(string)
-            #     p = sre_compile.compile(pattern, flags)
-            #     p = sre_parse.parse(p, flags)
-            #     p = _parse_sub(source, state, flags & SRE_FLAG_VERBOSE, 0)
-            #     itemsappend(_parse(source, state, verbose, nested + 1,
-            #     raise source.error("nothing to repeat",
-            # re.error: nothing to repeat at position 0
-            # instead, we will use fuzzysearch
-            from fuzzysearch import find_near_matches
-
-            matches = find_near_matches(text_to_find, string, max_l_dist=2)
-            result = [{"start": m.start, "end": m.end} for m in matches]
-        return result
-
-    def set_chunk(self, chunk_field: str, field: str, values: list, generate_id: bool = False):
-        """
-        doc.list_chunks()
-        doc.get_chunk("value_chunk_", field="sentence") # returns a list of values
-        doc.set_chunk("value_chunk_", field="sentence", values=["hey", "test"])
-        """
-        # We use upsert behavior for now
-        from ai_transform.utils.document_list import DocumentList
-
-        new_chunk_docs = self._create_chunk_documents(field, values=values, generate_id=generate_id)
-        # Update on the old chunk docs
-        old_chunk_docs = DocumentList(self.get(chunk_field))
-        # Relying on immutable property
-        [d.update(new_chunk_docs[i]) for i, d in enumerate(old_chunk_docs.data)]
-
-    def split(
-        self,
-        split_operation: callable,
-        chunk_field: str,
-        field: str,
-        default: Any = None,
-        include_offsets: bool = True,
-        generate_id: bool = False,
-    ):
-        """
-        The split operation is as follows:
-
-        The split operation returns to us a list of possible values.
-        The chunk documents are then created automatically for you.
-        """
-        if default is None:
-            default = []
-        value = self.get(field, default)
-        split_values = split_operation(value)
-        chunk_documents = self._create_chunk_documents(field=field, values=split_values, generate_id=generate_id)
-
-        if include_offsets:
-            for i, d in enumerate(chunk_documents):
-                offsets = self._calculate_offset(d[field], value)
-                d["_offsets_"] = offsets
-
-        self.set(chunk_field, chunk_documents)
-
-    def operate_on_chunk(
-        self, operator_function: callable, chunk_field: str, field: str, output_field: str, default: Any = None
-    ):
-        """
-        Add an operate function.
-        """
-        values = self.get_chunk(chunk_field=chunk_field, field=field, default=default)
-        results = operator_function(values)
-        self.set_chunk(chunk_field=chunk_field, field=output_field, values=results)
+import re
+import uuid
+import pprint
+
+from typing import Dict, Any
+from copy import deepcopy
+from typing import Any, Optional
+from collections import UserDict
+
+from ai_transform.utils.json_encoder import json_encoder
+
+
+class Document(UserDict):
+    def __repr__(self):
+        return pprint.pformat(self.to_json(), indent=4, width=40)
+
+    def __setitem__(self, key: Any, value: Any) -> None:
+        try:
+            fields = key.split(".")
+        except:
+            super().__setitem__(key, value)
+        else:
+            obj = self.data
+            for curr_field, next_field in zip(fields, fields[1:]):
+                if curr_field.isdigit():
+                    curr_field = int(curr_field)
+
+                if (isinstance(obj, dict) and (curr_field not in obj)) or (
+                    isinstance(obj, list) and (curr_field >= len(obj))
+                ):
+                    if next_field.isdigit():
+                        obj[curr_field] = [{}]
+                    else:
+                        if isinstance(curr_field, int):
+                            curr_field = min(len(obj) - 1, int(curr_field))
+                            if next_field not in obj[curr_field]:
+                                obj[curr_field] = {}
+                        else:
+                            obj[curr_field] = {}
+
+                try:
+                    obj = obj[curr_field]
+                except IndexError:
+                    obj = obj[0]
+                except KeyError:
+                    obj = obj[curr_field]
+
+            if fields[-1].isdigit():
+                field = min(len(obj) - 1, int(fields[-1]))
+            else:
+                field = fields[-1]
+            obj[field] = value
+
+    def __getitem__(self, key: Any) -> Any:
+        try:
+            fields = key.split(".")
+        except:
+            return super().__getitem__(key)
+        else:
+            obj = self.data
+            for field in fields[:-1]:
+                if field.isdigit():
+                    field = int(field)
+
+                obj = obj[field]
+
+            if fields[-1].isdigit():
+                field = min(len(obj) - 1, int(fields[-1]))
+            else:
+                field = fields[-1]
+            return obj[field]
+
+    def __delitem__(self, key):
+        try:
+            fields = key.split(".")
+        except:
+            return super().__getitem__(key)
+        else:
+            obj = self.data
+            for field in fields[:-1]:
+                if field.isdigit():
+                    field = int(field)
+
+                obj = obj[field]
+
+            if fields[-1].isdigit():
+                field = min(len(obj) - 1, int(fields[-1]))
+            else:
+                field = fields[-1]
+            del obj[field]
+
+    def get(self, key: Any, default: Optional[Any] = None) -> Any:
+        try:
+            return self.__getitem__(key)
+        except:
+            return default
+
+    def set(self, key: Any, value: Any) -> None:
+        self.__setitem__(key, value)
+
+    def keys(self):
+        def get_keys(dictionary: Dict[str, Any], prefix=""):
+            keys = []
+            for key, value in dictionary.items():
+                current_key = prefix + "." + key if prefix else key
+                if isinstance(value, dict):
+                    keys.extend(get_keys(value, current_key))
+                elif isinstance(value, list):
+                    for i, item in enumerate(value):
+                        if isinstance(item, dict):
+                            keys.extend(get_keys(item, current_key + "." + str(i)))
+                    keys.append(current_key)
+                else:
+                    keys.append(current_key)
+            if prefix:
+                keys.append(prefix)
+            return keys
+
+        keys = set(get_keys(self.data))
+
+        keys_to_add = set()
+        for key in keys:
+            subkeys = key.split(".")
+            for i in range(1, len(subkeys)):
+                keys_to_add.add(".".join(subkeys[:i]))
+        keys.update(keys_to_add)
+
+        return list(sorted(keys))
+
+    def __contains__(self, key) -> bool:
+        return key in self.keys()
+
+    def to_json(self):
+        return json_encoder(deepcopy(self.data))
+
+    def list_chunks(self):
+        """
+        List the available chunks inside of the document.
+        """
+        # based on conversation with API team
+        return [k for k in self.keys() if k.endswith("_chunk_")]
+
+    def get_chunk(self, chunk_field: str, field: str = None, default: str = None):
+        return [document.get(field, default) for document in self.get(chunk_field, default=default)]
+
+    def _create_chunk_documents(self, field: str, values: list, generate_id: bool = False):
+        """
+        create chunk documents based on a given field and value.
+        """
+        from ai_transform.utils.document_list import DocumentList
+
+        if generate_id:
+            docs = [{"_id": uuid.uuid4().__str__(), field: values[i], "_order_": i} for i in range(len(values))]
+        else:
+            docs = [{field: values[i], "_order_": i} for i in range(len(values))]
+        return DocumentList(docs)
+
+    def _calculate_offset(self, text_to_find, string):
+        try:
+            result = [{"start": m.start(), "end": m.end()} for m in re.finditer(text_to_find, string)]
+        except Exception as e:
+            import traceback
+
+            traceback.print_exc()
+            # this is the error this exception aims to solve
+            #     for m in re.finditer(text_to_find, string)
+            #     return _compile(pattern, flags).finditer(string)
+            #     p = sre_compile.compile(pattern, flags)
+            #     p = sre_parse.parse(p, flags)
+            #     p = _parse_sub(source, state, flags & SRE_FLAG_VERBOSE, 0)
+            #     itemsappend(_parse(source, state, verbose, nested + 1,
+            #     raise source.error("nothing to repeat",
+            # re.error: nothing to repeat at position 0
+            # instead, we will use fuzzysearch
+            from fuzzysearch import find_near_matches
+
+            matches = find_near_matches(text_to_find, string, max_l_dist=2)
+            result = [{"start": m.start, "end": m.end} for m in matches]
+        return result
+
+    def set_chunk(self, chunk_field: str, field: str, values: list, generate_id: bool = False):
+        """
+        doc.list_chunks()
+        doc.get_chunk("value_chunk_", field="sentence") # returns a list of values
+        doc.set_chunk("value_chunk_", field="sentence", values=["hey", "test"])
+        """
+        # We use upsert behavior for now
+        from ai_transform.utils.document_list import DocumentList
+
+        new_chunk_docs = self._create_chunk_documents(field, values=values, generate_id=generate_id)
+        # Update on the old chunk docs
+        old_chunk_docs = DocumentList(self.get(chunk_field))
+        # Relying on immutable property
+        [d.update(new_chunk_docs[i]) for i, d in enumerate(old_chunk_docs.data)]
+
+    def split(
+        self,
+        split_operation: callable,
+        chunk_field: str,
+        field: str,
+        default: Any = None,
+        include_offsets: bool = True,
+        generate_id: bool = False,
+    ):
+        """
+        The split operation is as follows:
+
+        The split operation returns to us a list of possible values.
+        The chunk documents are then created automatically for you.
+        """
+        if default is None:
+            default = []
+        value = self.get(field, default)
+        split_values = split_operation(value)
+        chunk_documents = self._create_chunk_documents(field=field, values=split_values, generate_id=generate_id)
+
+        if include_offsets:
+            for i, d in enumerate(chunk_documents):
+                offsets = self._calculate_offset(d[field], value)
+                d["_offsets_"] = offsets
+
+        self.set(chunk_field, chunk_documents)
+
+    def operate_on_chunk(
+        self, operator_function: callable, chunk_field: str, field: str, output_field: str, default: Any = None
+    ):
+        """
+        Add an operate function.
+        """
+        values = self.get_chunk(chunk_field=chunk_field, field=field, default=default)
+        results = operator_function(values)
+        self.set_chunk(chunk_field=chunk_field, field=output_field, values=results)
```

### Comparing `ai_transform-0.32.3/ai_transform/utils/document_list.py` & `ai_transform-0.32.4/ai_transform/utils/document_list.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,159 +1,159 @@
-import pprint
-import warnings
-import itertools
-
-from collections import UserList
-from typing import Any, Dict, List, Union
-
-from ai_transform.utils.document import Document
-
-
-class DocumentList(UserList):
-    data: List[Document]
-
-    def __init__(self, initlist=None):
-        if initlist is not None:
-            for index, document in enumerate(initlist):
-                if not isinstance(document, Document):
-                    initlist[index] = Document(document)
-        super().__init__(initlist)
-
-    def __repr__(self):
-        return pprint.pformat(self.to_json(), indent=4, width=40)
-
-    def __getitem__(self, key: Union[str, int]) -> Document:
-        if isinstance(key, str):
-            return [document[key] for document in self.data]
-        elif isinstance(key, slice):
-            return self.__class__(self.data[key])
-        elif isinstance(key, int):
-            return self.data[key]
-
-    def __setitem__(self, key: Union[str, int], value: Union[Any, List[Any]]):
-        if isinstance(key, str):
-            if isinstance(value, list):
-                for document, value in zip(self.data, value):
-                    document[key] = value
-            else:
-                for document in self.data:
-                    document[key] = value
-        elif isinstance(key, int):
-            self.data[key] = value
-
-    def to_json(self):
-        return [document.to_json() for document in self.data]
-
-    def _flatten_list(self, list_of_lists):
-        flat_list = itertools.chain(*list_of_lists)
-        return list(flat_list)
-
-    def set_chunk_values(self, chunk_field: str, output_field: str, chunk_values: List[List[Any]], sortby: str = None):
-        if sortby is None:
-            if any("_order_" in key for key in self.data[0].keys()):
-                sortby = "_order_"
-
-        assert len(chunk_values) == len(
-            self.data
-        ), "The length of your values array should be the same as your documents"
-
-        for document, chunk_labels in zip(self.data, chunk_values):
-            if chunk_field not in document:
-                document[chunk_field] = []
-
-            chunk = document[chunk_field]
-
-            if chunk:
-                if sortby is not None:
-                    chunk = list(sorted(chunk, key=lambda x: x[sortby]))
-                assert len(chunk) == len(
-                    chunk_labels
-                ), "The length of your `chunk` array should be the same as your `chunk_values`"
-                for chunk_index in range(len(chunk_labels)):
-                    subchunk = Document(chunk[chunk_index])
-                    label = chunk_labels[chunk_index]
-                    subchunk[output_field] = label
-                    chunk[chunk_index] = subchunk.to_json()
-            else:
-                document[chunk_field] = chunk_labels
-
-    def set_chunks_from_flat(self, chunk_field: str, field: str, values: list):
-        """
-        Set chunks from a flat list.
-        Note that this is only possible if there is pre-existing
-        chunk documents.
-        """
-        # general logic for this is that we assume that the number of values equals
-        # to the number of chunk values
-        chunk_counter = 0
-        for i, doc in enumerate(self.data):
-            chunk_docs = []
-            for j, chunk_doc in enumerate(doc.get(chunk_field, [])):
-                # chunk_doc = Document(chunk_doc)
-                chunk_doc = Document(chunk_doc)
-                chunk_doc.set(field, values[chunk_counter])
-                chunk_docs.append(chunk_doc)
-                chunk_counter += 1
-            doc.set(chunk_field, chunk_docs)
-
-        if chunk_counter > len(values):
-            raise ValueError("Number of chunks do not match with number of values - check logic.")
-
-    def get_chunks_as_flat(self, chunk_field: str, field: str, default=None):
-        """
-        Set chunks from a flat list.
-        Note that this is only possible if there is pre-existing
-        chunk documents.
-        """
-        docs = DocumentList(self._flatten_list([d.get(chunk_field) for d in self.data]))
-        return [d.get(field, default=default) for d in docs.data]
-
-    def split_by_chunk(self, chunk_field: str, values: list):
-        """
-        Split a list of values based on the number of documents
-        within a specific chunk field
-        """
-        counter = 0
-        for d in self.data:
-            chunk_field_len = len(d.get(chunk_field, []))
-            yield values[counter : counter + chunk_field_len]
-            counter += len(d.get(chunk_field, []))
-
-    def remove_tag(self, field: str, value: str) -> None:
-        warnings.warn("This behaviour is experimental and is subject to change")
-
-        *tag_fields, remove_field = field.split(".")
-        tag_field = ".".join(tag_fields)
-
-        for document in self.data:
-            new_tags = []
-
-            old_tags = document.get(tag_field, [])
-            for tag_json in old_tags:
-                if tag_json.get(remove_field) != value:
-                    new_tags.append(tag_json)
-
-            document[tag_field] = new_tags
-
-    def append_tag(self, field: str, value: Union[Dict[str, Any], List[Dict[str, Any]]]) -> None:
-        warnings.warn("This behaviour is experimental and is subject to change")
-
-        if isinstance(value, list):
-            for document, tag in zip(self.data, value):
-                document[field].append(tag)
-        else:
-            for document in self.data:
-                document[field].append(value)
-
-    def sort_tags(self, field: str, reverse: bool = False) -> None:
-        warnings.warn("This behaviour is experimental and is subject to change")
-
-        *tag_fields, sort_field = field.split(".")
-        tag_field = ".".join(tag_fields)
-
-        for document in self.data:
-            tags = document.get(tag_field)
-
-            if tags is not None:
-                document[tag_field] = sorted(
-                    document[tag_field], key=lambda tag_json: tag_json[sort_field], reverse=reverse
-                )
+import pprint
+import warnings
+import itertools
+
+from collections import UserList
+from typing import Any, Dict, List, Union
+
+from ai_transform.utils.document import Document
+
+
+class DocumentList(UserList):
+    data: List[Document]
+
+    def __init__(self, initlist=None):
+        if initlist is not None:
+            for index, document in enumerate(initlist):
+                if not isinstance(document, Document):
+                    initlist[index] = Document(document)
+        super().__init__(initlist)
+
+    def __repr__(self):
+        return pprint.pformat(self.to_json(), indent=4, width=40)
+
+    def __getitem__(self, key: Union[str, int]) -> Document:
+        if isinstance(key, str):
+            return [document[key] for document in self.data]
+        elif isinstance(key, slice):
+            return self.__class__(self.data[key])
+        elif isinstance(key, int):
+            return self.data[key]
+
+    def __setitem__(self, key: Union[str, int], value: Union[Any, List[Any]]):
+        if isinstance(key, str):
+            if isinstance(value, list):
+                for document, value in zip(self.data, value):
+                    document[key] = value
+            else:
+                for document in self.data:
+                    document[key] = value
+        elif isinstance(key, int):
+            self.data[key] = value
+
+    def to_json(self):
+        return [document.to_json() for document in self.data]
+
+    def _flatten_list(self, list_of_lists):
+        flat_list = itertools.chain(*list_of_lists)
+        return list(flat_list)
+
+    def set_chunk_values(self, chunk_field: str, output_field: str, chunk_values: List[List[Any]], sortby: str = None):
+        if sortby is None:
+            if any("_order_" in key for key in self.data[0].keys()):
+                sortby = "_order_"
+
+        assert len(chunk_values) == len(
+            self.data
+        ), "The length of your values array should be the same as your documents"
+
+        for document, chunk_labels in zip(self.data, chunk_values):
+            if chunk_field not in document:
+                document[chunk_field] = []
+
+            chunk = document[chunk_field]
+
+            if chunk:
+                if sortby is not None:
+                    chunk = list(sorted(chunk, key=lambda x: x[sortby]))
+                assert len(chunk) == len(
+                    chunk_labels
+                ), "The length of your `chunk` array should be the same as your `chunk_values`"
+                for chunk_index in range(len(chunk_labels)):
+                    subchunk = Document(chunk[chunk_index])
+                    label = chunk_labels[chunk_index]
+                    subchunk[output_field] = label
+                    chunk[chunk_index] = subchunk.to_json()
+            else:
+                document[chunk_field] = chunk_labels
+
+    def set_chunks_from_flat(self, chunk_field: str, field: str, values: list):
+        """
+        Set chunks from a flat list.
+        Note that this is only possible if there is pre-existing
+        chunk documents.
+        """
+        # general logic for this is that we assume that the number of values equals
+        # to the number of chunk values
+        chunk_counter = 0
+        for i, doc in enumerate(self.data):
+            chunk_docs = []
+            for j, chunk_doc in enumerate(doc.get(chunk_field, [])):
+                # chunk_doc = Document(chunk_doc)
+                chunk_doc = Document(chunk_doc)
+                chunk_doc.set(field, values[chunk_counter])
+                chunk_docs.append(chunk_doc)
+                chunk_counter += 1
+            doc.set(chunk_field, chunk_docs)
+
+        if chunk_counter > len(values):
+            raise ValueError("Number of chunks do not match with number of values - check logic.")
+
+    def get_chunks_as_flat(self, chunk_field: str, field: str, default=None):
+        """
+        Set chunks from a flat list.
+        Note that this is only possible if there is pre-existing
+        chunk documents.
+        """
+        docs = DocumentList(self._flatten_list([d.get(chunk_field) for d in self.data]))
+        return [d.get(field, default=default) for d in docs.data]
+
+    def split_by_chunk(self, chunk_field: str, values: list):
+        """
+        Split a list of values based on the number of documents
+        within a specific chunk field
+        """
+        counter = 0
+        for d in self.data:
+            chunk_field_len = len(d.get(chunk_field, []))
+            yield values[counter : counter + chunk_field_len]
+            counter += len(d.get(chunk_field, []))
+
+    def remove_tag(self, field: str, value: str) -> None:
+        warnings.warn("This behaviour is experimental and is subject to change")
+
+        *tag_fields, remove_field = field.split(".")
+        tag_field = ".".join(tag_fields)
+
+        for document in self.data:
+            new_tags = []
+
+            old_tags = document.get(tag_field, [])
+            for tag_json in old_tags:
+                if tag_json.get(remove_field) != value:
+                    new_tags.append(tag_json)
+
+            document[tag_field] = new_tags
+
+    def append_tag(self, field: str, value: Union[Dict[str, Any], List[Dict[str, Any]]]) -> None:
+        warnings.warn("This behaviour is experimental and is subject to change")
+
+        if isinstance(value, list):
+            for document, tag in zip(self.data, value):
+                document[field].append(tag)
+        else:
+            for document in self.data:
+                document[field].append(value)
+
+    def sort_tags(self, field: str, reverse: bool = False) -> None:
+        warnings.warn("This behaviour is experimental and is subject to change")
+
+        *tag_fields, sort_field = field.split(".")
+        tag_field = ".".join(tag_fields)
+
+        for document in self.data:
+            tags = document.get(tag_field)
+
+            if tags is not None:
+                document[tag_field] = sorted(
+                    document[tag_field], key=lambda tag_json: tag_json[sort_field], reverse=reverse
+                )
```

### Comparing `ai_transform-0.32.3/ai_transform/utils/json_encoder.py` & `ai_transform-0.32.4/ai_transform/utils/json_encoder.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,118 +1,118 @@
-"""Json Encoder utility
-
-To invoke JSON encoder:
-
-```
-    from relevanceai import json_encoder
-```
-
-"""
-import math
-import datetime
-import dataclasses
-import collections
-import pandas as pd
-
-from ipaddress import IPv4Address, IPv4Interface, IPv4Network, IPv6Address, IPv6Interface, IPv6Network
-
-from enum import Enum
-from types import GeneratorType
-from uuid import UUID
-from collections import deque
-from pathlib import Path
-from pathlib import PurePath
-from types import GeneratorType
-from enum import Enum
-from typing import Any
-
-# Taken from pydanitc.json
-ENCODERS_BY_TYPE = {
-    bytes: lambda o: o.decode(),
-    datetime.date: lambda o: o.isoformat(),
-    datetime.datetime: lambda o: o.isoformat(),
-    datetime.time: lambda o: o.isoformat(),
-    datetime.timedelta: lambda td: td.total_seconds(),
-    Enum: lambda o: o.value,
-    frozenset: list,
-    deque: list,
-    GeneratorType: list,
-    IPv4Address: str,
-    IPv4Interface: str,
-    IPv4Network: str,
-    IPv6Address: str,
-    IPv6Interface: str,
-    IPv6Network: str,
-    Path: str,
-    set: list,
-    UUID: str,
-}
-
-
-def json_encoder(obj: Any, force_string: bool = False):
-    """Converts object so it is json serializable
-    If you want to add your own mapping,
-    customize it this way;
-
-    Parameters
-    ------------
-    obj: Any
-        The object to convert
-    force_string: bool
-        If True, forces the object to a string representation. Used mainly for
-        analytics tracking.
-
-    Example
-    --------
-
-    YOu can use our JSON encoder easily.
-    >>> documents = [{"value": np.nan}]
-    >>> client.json_encoder(documents)
-
-    If you want to use FastAPI's json encoder, do this:
-    >>> from fastapi import jsonable_encoder
-    >>> client.json_encoder = jsonable_encoder
-
-    """
-    from ai_transform.utils import DocumentList, Document
-
-    # Loop through iterators and convert
-    if isinstance(obj, (list, set, frozenset, GeneratorType, tuple, collections.deque)):
-        encoded_list = []
-        for item in obj:
-            encoded_list.append(json_encoder(item, force_string=force_string))
-        return encoded_list
-
-    # Loop through dictionaries and convert
-    if isinstance(obj, dict):
-        encoded_dict = {}
-        for key, value in obj.items():
-            encoded_key = json_encoder(key, force_string=force_string)
-            encoded_value = json_encoder(value, force_string=force_string)
-            encoded_dict[encoded_key] = encoded_value
-        return encoded_dict
-
-    # Custom conversions
-    if dataclasses.is_dataclass(obj):
-        return dataclasses.asdict(obj)
-    if isinstance(obj, Enum):
-        return obj.value
-    if isinstance(obj, PurePath):
-        return str(obj)
-    if isinstance(obj, (str, int, type(None))):
-        return obj
-    if isinstance(obj, float):
-        if math.isnan(obj):
-            return None
-        return obj
-    if isinstance(obj, (Document, DocumentList)):
-        return obj.to_json()
-    if type(obj) in ENCODERS_BY_TYPE:
-        return ENCODERS_BY_TYPE[type(obj)](obj)  # type: ignore
-
-    if force_string:
-        return repr(obj)
-
-    if isinstance(obj, pd.Timestamp):
-        return repr(obj)
-
-    raise ValueError(f"{obj} ({type(obj)}) cannot be converted to JSON format")
+"""Json Encoder utility
+
+To invoke JSON encoder:
+
+```
+    from relevanceai import json_encoder
+```
+
+"""
+import math
+import datetime
+import dataclasses
+import collections
+import pandas as pd
+
+from ipaddress import IPv4Address, IPv4Interface, IPv4Network, IPv6Address, IPv6Interface, IPv6Network
+
+from enum import Enum
+from types import GeneratorType
+from uuid import UUID
+from collections import deque
+from pathlib import Path
+from pathlib import PurePath
+from types import GeneratorType
+from enum import Enum
+from typing import Any
+
+# Taken from pydanitc.json
+ENCODERS_BY_TYPE = {
+    bytes: lambda o: o.decode(),
+    datetime.date: lambda o: o.isoformat(),
+    datetime.datetime: lambda o: o.isoformat(),
+    datetime.time: lambda o: o.isoformat(),
+    datetime.timedelta: lambda td: td.total_seconds(),
+    Enum: lambda o: o.value,
+    frozenset: list,
+    deque: list,
+    GeneratorType: list,
+    IPv4Address: str,
+    IPv4Interface: str,
+    IPv4Network: str,
+    IPv6Address: str,
+    IPv6Interface: str,
+    IPv6Network: str,
+    Path: str,
+    set: list,
+    UUID: str,
+}
+
+
+def json_encoder(obj: Any, force_string: bool = False):
+    """Converts object so it is json serializable
+    If you want to add your own mapping,
+    customize it this way;
+
+    Parameters
+    ------------
+    obj: Any
+        The object to convert
+    force_string: bool
+        If True, forces the object to a string representation. Used mainly for
+        analytics tracking.
+
+    Example
+    --------
+
+    YOu can use our JSON encoder easily.
+    >>> documents = [{"value": np.nan}]
+    >>> client.json_encoder(documents)
+
+    If you want to use FastAPI's json encoder, do this:
+    >>> from fastapi import jsonable_encoder
+    >>> client.json_encoder = jsonable_encoder
+
+    """
+    from ai_transform.utils import DocumentList, Document
+
+    # Loop through iterators and convert
+    if isinstance(obj, (list, set, frozenset, GeneratorType, tuple, collections.deque)):
+        encoded_list = []
+        for item in obj:
+            encoded_list.append(json_encoder(item, force_string=force_string))
+        return encoded_list
+
+    # Loop through dictionaries and convert
+    if isinstance(obj, dict):
+        encoded_dict = {}
+        for key, value in obj.items():
+            encoded_key = json_encoder(key, force_string=force_string)
+            encoded_value = json_encoder(value, force_string=force_string)
+            encoded_dict[encoded_key] = encoded_value
+        return encoded_dict
+
+    # Custom conversions
+    if dataclasses.is_dataclass(obj):
+        return dataclasses.asdict(obj)
+    if isinstance(obj, Enum):
+        return obj.value
+    if isinstance(obj, PurePath):
+        return str(obj)
+    if isinstance(obj, (str, int, type(None))):
+        return obj
+    if isinstance(obj, float):
+        if math.isnan(obj):
+            return None
+        return obj
+    if isinstance(obj, (Document, DocumentList)):
+        return obj.to_json()
+    if type(obj) in ENCODERS_BY_TYPE:
+        return ENCODERS_BY_TYPE[type(obj)](obj)  # type: ignore
+
+    if force_string:
+        return repr(obj)
+
+    if isinstance(obj, pd.Timestamp):
+        return repr(obj)
+
+    raise ValueError(f"{obj} ({type(obj)}) cannot be converted to JSON format")
```

### Comparing `ai_transform-0.32.3/ai_transform/utils/keyphrase.py` & `ai_transform-0.32.4/ai_transform/utils/keyphrase.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from typing import List, Dict
-from dataclasses import dataclass
-
-
-@dataclass
-class Keyphrase:
-    """
-    We use this class to enforce the format of a keyphrase and
-    make it easier to handle to CRUD operations on Keyphrase Field.
-
-    Member variables are:
-    _text: string, the keyphrase text
-    _id: string, the id of the keyphrase.
-    _ancestors: list of strings, the ancestors of the keyphrase in the taxnonomy.
-    _parents: list of strings, the parents of the keyphrase in the taxnonomy.
-    _level: integer, the level of the keyphrase.
-    _keyphrase_score: float, >=0, the score of the keyphrase.
-    _frequency: integer, the frequency of the keyphrase.
-    _metadata: dict, the metadata that is associated with the keyphrase.
-    """
-
-    text: str
-    _id: str
-    ancestors: List[str] = None
-    parents: List[str] = None
-    level: int = 0
-    keyphrase_score: float = 0.0
-    frequency: int = 0
-    metadata: Dict = None
+from typing import List, Dict
+from dataclasses import dataclass
+
+
+@dataclass
+class Keyphrase:
+    """
+    We use this class to enforce the format of a keyphrase and
+    make it easier to handle to CRUD operations on Keyphrase Field.
+
+    Member variables are:
+    _text: string, the keyphrase text
+    _id: string, the id of the keyphrase.
+    _ancestors: list of strings, the ancestors of the keyphrase in the taxnonomy.
+    _parents: list of strings, the parents of the keyphrase in the taxnonomy.
+    _level: integer, the level of the keyphrase.
+    _keyphrase_score: float, >=0, the score of the keyphrase.
+    _frequency: integer, the frequency of the keyphrase.
+    _metadata: dict, the metadata that is associated with the keyphrase.
+    """
+
+    text: str
+    _id: str
+    ancestors: List[str] = None
+    parents: List[str] = None
+    level: int = 0
+    keyphrase_score: float = 0.0
+    frequency: int = 0
+    metadata: Dict = None
```

### Comparing `ai_transform-0.32.3/ai_transform/workflow/abstract_workflow.py` & `ai_transform-0.32.4/ai_transform/workflow/abstract_workflow.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,133 +1,133 @@
-import uuid
-import logging
-import warnings
-
-from typing import Any, List, Dict, Optional
-
-from ai_transform.dataset.dataset import Dataset
-from ai_transform.engine.abstract_engine import AbstractEngine
-from ai_transform.workflow.context_manager import WorkflowContextManager
-from ai_transform.operator.abstract_operator import AbstractOperator
-from ai_transform.errors import UserFacingError
-
-logger = logging.getLogger(__name__)
-
-
-class Workflow:
-    def __init__(
-        self,
-        engine: AbstractEngine,
-        job_id: Optional[str] = None,
-        name: Optional[str] = "Workflow",
-        metadata: Optional[Dict[str, Any]] = None,
-        additional_information: str = "",
-        send_email: bool = True,
-        success_threshold: float = 0.8,
-        email: dict = None,
-        output: dict = None,
-        **kwargs,  # TODO: Update workflows, This for deprecated arguments
-    ):
-        if job_id is None:
-            job_id = str(uuid.uuid4())
-            warnings.warn(f"No job id supplied, using {job_id}")
-
-        self._name = name
-        self._engine = engine
-        self._job_id = job_id
-
-        self.engine.update_engine_props(job_id=job_id, workflow_name=name)
-
-        self._metadata = {} if metadata is None else metadata
-        self._additional_information = additional_information
-        self._send_email = send_email
-
-        self._success_threshold = success_threshold
-        self._email = email
-        self._output = output
-
-    @property
-    def success_threshold(self):
-        return self._success_threshold
-
-    @property
-    def name(self):
-        return self._name
-
-    @property
-    def engine(self) -> AbstractEngine:
-        return self._engine
-
-    @property
-    def dataset(self) -> Dataset:
-        return self.engine.dataset
-
-    @property
-    def api(self):
-        return self.dataset.api
-
-    @property
-    def job_id(self):
-        return self._job_id
-
-    @property
-    def metadata(self):
-        return self._metadata
-
-    @property
-    def additional_information(self):
-        return self._additional_information
-
-    @property
-    def send_email(self):
-        return self._send_email
-
-    @property
-    def email(self):
-        return self._email
-
-    @property
-    def operators(self) -> List[AbstractOperator]:
-        if isinstance(self.engine.operator, AbstractOperator):
-            return [self.engine.operator]
-        else:
-            return self.engine.operators
-
-    def run(self):
-        with WorkflowContextManager(
-            workflow_name=self.name,
-            job_id=self.job_id,
-            additional_information=self.additional_information,
-            send_email=self.send_email,
-            email=self.email,
-            success_threshold=self.success_threshold,
-            operators=self.operators,
-            metadata=self.metadata,
-            engine=self.engine,
-            dataset=self.dataset,
-            output=self._output,
-        ):
-            self.engine()
-
-    def get_status(self):
-        return self.api._get_workflow_status(self._job_id)
-
-    def update_metadata(self, metadata: Dict[str, Any]):
-        return self.api._update_workflow_metadata(self._job_id, metadata=metadata)
-
-    def raise_user_facing_error(self, message: str):
-        """
-        Usage:
-
-        workflow.raise_user_facing_error("Missing XYZ")
-        """
-        raise UserFacingError(
-            error_message=message,
-            client=self.engine.dataset,
-            job_id=self.job_id,
-            workflow_name=self.name,
-            additional_information=self.additional_information,
-            send_email=self.send_email,
-        )
-
-
-AbstractWorkflow = Workflow
+import uuid
+import logging
+import warnings
+
+from typing import Any, List, Dict, Optional
+
+from ai_transform.dataset.dataset import Dataset
+from ai_transform.engine.abstract_engine import AbstractEngine
+from ai_transform.workflow.context_manager import WorkflowContextManager
+from ai_transform.operator.abstract_operator import AbstractOperator
+from ai_transform.errors import UserFacingError
+
+logger = logging.getLogger(__name__)
+
+
+class Workflow:
+    def __init__(
+        self,
+        engine: AbstractEngine,
+        job_id: Optional[str] = None,
+        name: Optional[str] = "Workflow",
+        metadata: Optional[Dict[str, Any]] = None,
+        additional_information: str = "",
+        send_email: bool = True,
+        success_threshold: float = 0.8,
+        email: dict = None,
+        output: dict = None,
+        **kwargs,  # TODO: Update workflows, This for deprecated arguments
+    ):
+        if job_id is None:
+            job_id = str(uuid.uuid4())
+            warnings.warn(f"No job id supplied, using {job_id}")
+
+        self._name = name
+        self._engine = engine
+        self._job_id = job_id
+
+        self.engine.update_engine_props(job_id=job_id, workflow_name=name)
+
+        self._metadata = {} if metadata is None else metadata
+        self._additional_information = additional_information
+        self._send_email = send_email
+
+        self._success_threshold = success_threshold
+        self._email = email
+        self._output = output
+
+    @property
+    def success_threshold(self):
+        return self._success_threshold
+
+    @property
+    def name(self):
+        return self._name
+
+    @property
+    def engine(self) -> AbstractEngine:
+        return self._engine
+
+    @property
+    def dataset(self) -> Dataset:
+        return self.engine.dataset
+
+    @property
+    def api(self):
+        return self.dataset.api
+
+    @property
+    def job_id(self):
+        return self._job_id
+
+    @property
+    def metadata(self):
+        return self._metadata
+
+    @property
+    def additional_information(self):
+        return self._additional_information
+
+    @property
+    def send_email(self):
+        return self._send_email
+
+    @property
+    def email(self):
+        return self._email
+
+    @property
+    def operators(self) -> List[AbstractOperator]:
+        if isinstance(self.engine.operator, AbstractOperator):
+            return [self.engine.operator]
+        else:
+            return self.engine.operators
+
+    def run(self):
+        with WorkflowContextManager(
+            workflow_name=self.name,
+            job_id=self.job_id,
+            additional_information=self.additional_information,
+            send_email=self.send_email,
+            email=self.email,
+            success_threshold=self.success_threshold,
+            operators=self.operators,
+            metadata=self.metadata,
+            engine=self.engine,
+            dataset=self.dataset,
+            output=self._output,
+        ):
+            self.engine()
+
+    def get_status(self):
+        return self.api._get_workflow_status(self._job_id)
+
+    def update_metadata(self, metadata: Dict[str, Any]):
+        return self.api._update_workflow_metadata(self._job_id, metadata=metadata)
+
+    def raise_user_facing_error(self, message: str):
+        """
+        Usage:
+
+        workflow.raise_user_facing_error("Missing XYZ")
+        """
+        raise UserFacingError(
+            error_message=message,
+            client=self.engine.dataset,
+            job_id=self.job_id,
+            workflow_name=self.name,
+            additional_information=self.additional_information,
+            send_email=self.send_email,
+        )
+
+
+AbstractWorkflow = Workflow
```

### Comparing `ai_transform-0.32.3/ai_transform/workflow/helpers.py` & `ai_transform-0.32.4/ai_transform/workflow/helpers.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,109 +1,109 @@
-"""
-Base64 decoding for workflows
-"""
-import argparse
-import os
-import base64
-import json
-import time
-from ai_transform.dataset.dataset import Dataset
-from typing import Any, Mapping
-
-
-def decode_workflow_token(token: str) -> Mapping[str, Any]:
-    """
-    It takes a token, decodes it, and returns the decoded token
-
-    Parameters
-    ----------
-    token
-        The token that was generated by the workflow.
-
-    Returns
-    -------
-        A dictionary of the workflow configuration.
-
-    """
-    config = json.loads(base64.b64decode(token + "==="))
-    # Set workflow ID for tracking
-    os.environ["WORKFLOW_ID"] = config.get("job_id", "")
-    return config
-
-
-def read_token_from_script():
-    """
-    Reads in a token from script and returns a config as a
-    dictionary object.
-    """
-    parser = argparse.ArgumentParser()
-    parser.add_argument("token", help="The token used for the workflow config.")
-    args = parser.parse_args()
-    token = args.token
-    config = decode_workflow_token(token)
-    return config
-
-
-def safe_divide(x, y):
-    if y == 0:
-        return 0
-    else:
-        return x / y
-
-
-def calculate_health_proportion(health: dict):
-    """
-    Example health object looks like this:
-    {"exists": 300, "missing": 100}
-    """
-    return safe_divide(health["exists"], (health["exists"] + health["missing"]))
-
-
-def poll_until_health_updates(
-    dataset: Dataset, field: str, minimum_coverage: float = 0.95, sleep_timer: int = 10, max_time: int = 600
-):
-    """
-    Poll until the dataset has all required dataset.
-    """
-    health = dataset.health()
-    field_health = health[field]
-    proportion = calculate_health_proportion(field_health)
-    start_time = time.time()
-    while proportion <= minimum_coverage:
-        time.sleep(sleep_timer)
-        health = dataset.health()
-        field_health = health[field]
-        proportion = calculate_health_proportion(field_health)
-        current_time = time.time()
-        if (current_time - start_time) > max_time:
-            break
-    return
-
-
-def poll_until_health_updates_with_input_field(
-    dataset: Dataset,
-    input_field: str,
-    output_field: str,
-    minimum_coverage: float = 0.95,
-    sleep_timer: int = 10,
-    max_time: int = 600,
-):
-    """
-    Poll until the dataset has all required dataset.
-    Arguments:
-        dataset: Dataset object
-        input_field: the input field to poll on
-        outout_field: the output field,
-        minimum_coverage: the minimum amount of coverage
-            required based on the input field
-        sleep_timer:
-            the time in between each poll request
-    """
-    input_field_health = dataset.health()[input_field]
-    min_coverage = calculate_health_proportion(input_field_health) * minimum_coverage
-    return poll_until_health_updates(
-        dataset=dataset, field=output_field, minimum_coverage=min_coverage, sleep_timer=sleep_timer, max_time=max_time
-    )
-
-
-def encode_config(data: dict):
-    return base64.b64encode(json.dumps(data).encode()).decode()
+"""
+Base64 decoding for workflows
+"""
+import argparse
+import os
+import base64
+import json
+import time
+from ai_transform.dataset.dataset import Dataset
+from typing import Any, Mapping
+
+
+def decode_workflow_token(token: str) -> Mapping[str, Any]:
+    """
+    It takes a token, decodes it, and returns the decoded token
+
+    Parameters
+    ----------
+    token
+        The token that was generated by the workflow.
+
+    Returns
+    -------
+        A dictionary of the workflow configuration.
+
+    """
+    config = json.loads(base64.b64decode(token + "==="))
+    # Set workflow ID for tracking
+    os.environ["WORKFLOW_ID"] = config.get("job_id", "")
+    return config
+
+
+def read_token_from_script():
+    """
+    Reads in a token from script and returns a config as a
+    dictionary object.
+    """
+    parser = argparse.ArgumentParser()
+    parser.add_argument("token", help="The token used for the workflow config.")
+    args = parser.parse_args()
+    token = args.token
+    config = decode_workflow_token(token)
+    return config
+
+
+def safe_divide(x, y):
+    if y == 0:
+        return 0
+    else:
+        return x / y
+
+
+def calculate_health_proportion(health: dict):
+    """
+    Example health object looks like this:
+    {"exists": 300, "missing": 100}
+    """
+    return safe_divide(health["exists"], (health["exists"] + health["missing"]))
+
+
+def poll_until_health_updates(
+    dataset: Dataset, field: str, minimum_coverage: float = 0.95, sleep_timer: int = 10, max_time: int = 600
+):
+    """
+    Poll until the dataset has all required dataset.
+    """
+    health = dataset.health()
+    field_health = health[field]
+    proportion = calculate_health_proportion(field_health)
+    start_time = time.time()
+    while proportion <= minimum_coverage:
+        time.sleep(sleep_timer)
+        health = dataset.health()
+        field_health = health[field]
+        proportion = calculate_health_proportion(field_health)
+        current_time = time.time()
+        if (current_time - start_time) > max_time:
+            break
+    return
+
+
+def poll_until_health_updates_with_input_field(
+    dataset: Dataset,
+    input_field: str,
+    output_field: str,
+    minimum_coverage: float = 0.95,
+    sleep_timer: int = 10,
+    max_time: int = 600,
+):
+    """
+    Poll until the dataset has all required dataset.
+    Arguments:
+        dataset: Dataset object
+        input_field: the input field to poll on
+        outout_field: the output field,
+        minimum_coverage: the minimum amount of coverage
+            required based on the input field
+        sleep_timer:
+            the time in between each poll request
+    """
+    input_field_health = dataset.health()[input_field]
+    min_coverage = calculate_health_proportion(input_field_health) * minimum_coverage
+    return poll_until_health_updates(
+        dataset=dataset, field=output_field, minimum_coverage=min_coverage, sleep_timer=sleep_timer, max_time=max_time
+    )
+
+
+def encode_config(data: dict):
+    return base64.b64encode(json.dumps(data).encode()).decode()
```

### Comparing `ai_transform-0.32.3/ai_transform.egg-info/SOURCES.txt` & `ai_transform-0.32.4/ai_transform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.3/setup.py` & `ai_transform-0.32.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from setuptools import find_packages, setup
-
-from ai_transform import __version__
-
-requirements = ["tqdm>=4.49.0", "requests>=2.0.0", "pandas>=1.5.0", "pydantic>=1.10.2", "icecream==2.1.3"]
-
-ray_requirements = ["numpy>=1.19.0", "pyarrow==9.0.0", "ray==2.0.0"]
-
-core_test_requirements = ["pytest", "pytest-xdist", "pytest-cov", "sentence-splitter"]
-
-example_test_requirements = core_test_requirements + ["torch", "scikit-learn>=0.20.0", "transformers[torch]==4.18.0"]
-
-chunk_requirements = ["fuzzysearch==0.7.3"]
-
-setup(
-    name="ai_transform",
-    version=__version__,
-    url="https://tryrelevance.com/",
-    author="Relevance AI",
-    author_email="dev@tryrelevance.com",
-    packages=find_packages(),
-    setup_requires=["wheel"],
-    install_requires=requirements,
-    package_data={"": ["*.ini"]},
-    extras_require=dict(
-        core_tests=core_test_requirements,
-        example_tests=example_test_requirements,
-        ray=ray_requirements,
-        chunk=chunk_requirements,
-    ),
-)
+from setuptools import find_packages, setup
+
+from ai_transform import __version__
+
+requirements = ["tqdm>=4.49.0", "requests>=2.0.0", "pandas>=1.5.0", "pydantic>=1.10.2", "icecream==2.1.3", "typing-extensions==4.7.1"]
+
+ray_requirements = ["numpy>=1.19.0", "pyarrow==9.0.0", "ray==2.0.0"]
+
+core_test_requirements = ["pytest", "pytest-xdist", "pytest-cov", "sentence-splitter"]
+
+example_test_requirements = core_test_requirements + ["torch", "scikit-learn>=0.20.0", "transformers[torch]==4.18.0"]
+
+chunk_requirements = ["fuzzysearch==0.7.3"]
+
+setup(
+    name="ai_transform",
+    version=__version__,
+    url="https://tryrelevance.com/",
+    author="Relevance AI",
+    author_email="dev@tryrelevance.com",
+    packages=find_packages(),
+    setup_requires=["wheel"],
+    install_requires=requirements,
+    package_data={"": ["*.ini"]},
+    extras_require=dict(
+        core_tests=core_test_requirements,
+        example_tests=example_test_requirements,
+        ray=ray_requirements,
+        chunk=chunk_requirements,
+    ),
+)
```

### Comparing `ai_transform-0.32.3/tests/conftest.py` & `ai_transform-0.32.4/tests/conftest.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,481 +1,481 @@
-import os
-import json
-import uuid
-import time
-import base64
-import random
-import pytest
-import string
-
-from typing import List, Dict, Sequence
-
-from ai_transform.api.client import Client
-from ai_transform.api.helpers import process_token
-
-from ai_transform.dataset.dataset import Dataset
-
-from ai_transform.engine.stable_engine import StableEngine
-
-from ai_transform.operator.abstract_operator import AbstractOperator
-from ai_transform.operator.dense_operator import DenseOperator
-
-from ai_transform.utils.document import Document
-from ai_transform.utils.document_list import DocumentList
-from ai_transform.utils.example_documents import (
-    mock_documents,
-    static_documents,
-    tag_documents,
-    generate_random_vector,
-    incomplete_documents,
-)
-
-
-TEST_TOKEN = os.getenv("TEST_TOKEN")
-test_creds = process_token(TEST_TOKEN)
-
-
-@pytest.fixture(scope="session")
-def test_token() -> str:
-    return TEST_TOKEN
-
-
-@pytest.fixture(scope="session")
-def test_client(test_token: str) -> Client:
-    return Client(test_token)
-
-
-@pytest.fixture(scope="function")
-def test_dataset_id() -> str:
-    salt = "".join(random.choices(string.ascii_lowercase, k=10))
-    dataset_id = f"_sample_dataset_{salt}"
-    return dataset_id
-
-
-@pytest.fixture(scope="function")
-def empty_dataset(test_client: Client) -> Dataset:
-    salt = "".join(random.choices(string.ascii_lowercase, k=10))
-    dataset_id = f"_sample_dataset_{salt}"
-    dataset = test_client.Dataset(dataset_id, expire=False)
-    yield dataset
-    test_client.delete_dataset(dataset_id)
-
-
-@pytest.fixture(scope="class")
-def full_dataset(test_client: Client) -> Dataset:
-    salt = "".join(random.choices(string.ascii_lowercase, k=10))
-    dataset_id = f"_sample_dataset_{salt}"
-    dataset = test_client.Dataset(dataset_id, expire=True)
-    dataset.insert_documents(mock_documents(20))
-    yield dataset
-    test_client.delete_dataset(dataset_id)
-
-
-@pytest.fixture(scope="class")
-def partial_dataset(test_client: Client) -> Dataset:
-    salt = "".join(random.choices(string.ascii_lowercase, k=10))
-    dataset_id = f"_sample_dataset_{salt}"
-    dataset = test_client.Dataset(dataset_id, expire=True)
-    documents = mock_documents(1000)
-    fields = ["sample_1_label", "sample_2_label", "sample_3_label"]
-    for document in documents:
-        for field in random.sample(fields, k=random.randint(1, 3)):
-            document.pop(field)
-    dataset.insert_documents(documents)
-    yield dataset
-    test_client.delete_dataset(dataset_id)
-
-
-@pytest.fixture(scope="class")
-def simple_partial_dataset(test_client: Client) -> Dataset:
-    salt = "".join(random.choices(string.ascii_lowercase, k=10))
-    dataset_id = f"_sample_dataset_{salt}"
-    dataset = test_client.Dataset(dataset_id, expire=True)
-    documents = mock_documents(1000)
-    fields = ["sample_1_label"]
-    for document in documents:
-        if random.random() < 0.5:
-            document.pop(fields[0])
-    dataset.insert_documents(documents)
-    yield dataset
-    test_client.delete_dataset(dataset_id)
-
-
-@pytest.fixture(scope="class")
-def partial_dataset_with_outputs(test_client: Client) -> Dataset:
-    salt = "".join(random.choices(string.ascii_lowercase, k=10))
-    dataset_id = f"_sample_dataset_{salt}"
-    dataset = test_client.Dataset(dataset_id, expire=True)
-    documents = mock_documents(1000)
-    fields = ["sample_1_label", "sample_2_label", "sample_3_label"]
-    for document in documents:
-        for field in random.sample(fields, k=random.randint(1, 3)):
-            document.pop(field)
-    for document in documents:
-        for field in fields:
-            if document.get(field) and random.random() < 0.5:
-                document[field + "_output"] = document[field] + "_output"
-    dataset.insert_documents(documents)
-    yield dataset
-    test_client.delete_dataset(dataset_id)
-
-
-@pytest.fixture(scope="class")
-def mixed_dataset(test_client: Client) -> Dataset:
-    salt = "".join(random.choices(string.ascii_lowercase, k=10))
-    dataset_id = f"_sample_dataset_{salt}"
-    dataset = test_client.Dataset(dataset_id, expire=True)
-    documents = mock_documents(10)
-    stripped = mock_documents(10)
-    for document in stripped:
-        document.pop("_chunk_")
-    documents += stripped
-    dataset.insert_documents(documents)
-    yield dataset
-    test_client.delete_dataset(dataset_id)
-
-
-@pytest.fixture(scope="class")
-def static_dataset(test_client: Client) -> Dataset:
-    salt = "".join(random.choices(string.ascii_lowercase, k=10))
-    dataset_id = f"_sample_dataset_{salt}"
-    dataset = test_client.Dataset(dataset_id, expire=True)
-    dataset.insert_documents(static_documents(20))
-    yield dataset
-    test_client.delete_dataset(dataset_id)
-
-
-@pytest.fixture(scope="function")
-def dense_input_dataset1(test_client: Client) -> Dataset:
-    salt = "".join(random.choices(string.ascii_lowercase, k=10))
-    dataset_id = f"_sample_dataset_{salt}"
-    dataset = test_client.Dataset(dataset_id, expire=True)
-    dataset.insert_documents(static_documents(2))
-    yield dataset
-    test_client.delete_dataset(dataset_id)
-
-
-@pytest.fixture(scope="function")
-def dense_input_dataset2(test_client: Client) -> Dataset:
-    salt = "".join(random.choices(string.ascii_lowercase, k=10))
-    dataset_id = f"_sample_dataset_{salt}"
-    dataset = test_client.Dataset(dataset_id, expire=True)
-    dataset.insert_documents(mock_documents(100))
-    yield dataset
-    test_client.delete_dataset(dataset_id)
-
-
-@pytest.fixture(scope="function")
-def dense_output_dataset1(test_client: Client) -> Dataset:
-    salt = "".join(random.choices(string.ascii_lowercase, k=10))
-    dataset_id = f"_sample_dataset_{salt}"
-    dataset = test_client.Dataset(dataset_id, expire=True)
-    yield dataset
-    test_client.delete_dataset(dataset_id)
-
-
-@pytest.fixture(scope="function")
-def dense_output_dataset2(test_client: Client) -> Dataset:
-    salt = "".join(random.choices(string.ascii_lowercase, k=10))
-    dataset_id = f"_sample_dataset_{salt}"
-    dataset = test_client.Dataset(dataset_id, expire=True)
-    yield dataset
-    test_client.delete_dataset(dataset_id)
-
-
-@pytest.fixture(scope="function")
-def test_document() -> Document:
-    raw_dict = {"field1": {"field2": 1}, "field3": 3}
-    return Document(raw_dict)
-
-
-@pytest.fixture(scope="function")
-def test_documents() -> DocumentList:
-    return mock_documents()
-
-
-@pytest.fixture(scope="function")
-def test_tag_documents() -> DocumentList:
-    return tag_documents()
-
-
-@pytest.fixture(scope="function")
-def test_operator() -> AbstractOperator:
-    class ExampleOperator(AbstractOperator):
-        def transform(self, documents: DocumentList) -> DocumentList:
-            """
-            Main transform function
-            """
-            for document in documents:
-                if "new_field" not in document:
-                    document["new_field"] = 0
-
-                document["new_field"] += 3
-
-            return documents
-
-    return ExampleOperator()
-
-
-@pytest.fixture(scope="function")
-def test_partial_operator() -> AbstractOperator:
-    class PartialOperator(AbstractOperator):
-        def __init__(self, fields):
-            super().__init__(input_fields=fields, output_fields=[field + "_output" for field in fields])
-
-        def transform(self, documents: DocumentList) -> DocumentList:
-            """
-            Main transform function
-            """
-            for input_field, output_field in zip(self.input_fields, self.output_fields):
-                for document in documents:
-                    if document.get(input_field):
-                        document[output_field] = document[input_field] + "_output"
-
-            return documents
-
-    return PartialOperator
-
-
-@pytest.fixture(scope="function")
-def test_paid_operator() -> AbstractOperator:
-    class ExampleOperator(AbstractOperator):
-        def __init__(self):
-            super().__init__()
-
-        def transform(self, documents: DocumentList) -> DocumentList:
-            """
-            Main transform function
-            """
-            for document in documents:
-                if "new_field" not in document:
-                    document["new_field"] = 0
-
-                document["new_field"] += 3
-                self.n_processed_pricing += 1
-
-            return documents
-
-    return ExampleOperator()
-
-
-@pytest.fixture(scope="function")
-def test_dense_operator(dense_output_dataset1: Dataset, dense_output_dataset2: Dataset) -> DenseOperator:
-    class TestDenseOperator(DenseOperator):
-        def __init__(self, output_dataset_ids: Sequence[str]):
-            self.output_dataset_ids = output_dataset_ids
-            super().__init__()
-
-        def transform(self, documents: DocumentList) -> DocumentList:
-            """
-            Main transform function
-            """
-            for document in documents:
-                if "new_field" not in document:
-                    document["new_field"] = 0
-
-                document["new_field"] += 3
-
-            return {dataset_id: documents for dataset_id in self.output_dataset_ids}
-
-    output_dataset_ids = (dense_output_dataset1.dataset_id, dense_output_dataset2.dataset_id)
-    return TestDenseOperator(output_dataset_ids)
-
-
-@pytest.fixture(scope="function")
-def test_chunk_dense_operator(dense_output_dataset1: Dataset, dense_output_dataset2: Dataset) -> DenseOperator:
-    class TestDenseOperator(DenseOperator):
-        def __init__(self, output_dataset_ids: Sequence[str]):
-            self.output_dataset_ids = output_dataset_ids
-            self._chunk_field = "_chunk_"
-            self._text_field = "label"
-            self._alias = "default"
-            super().__init__()
-
-        def transform(self, documents: List[Document]) -> List[Document]:
-            outputs = []
-            for document in documents:
-                texts = document.get_chunk(chunk_field=self._chunk_field, field=self._text_field)
-                text_vectors = [generate_random_vector() for _ in range(len(texts))]
-
-                for sent_index, text_vector in enumerate(text_vectors):
-                    outputs.append(
-                        {
-                            "_id": document["_id"] + f":{sent_index}",
-                            f"{self._text_field}_{self._alias}_vector_": text_vector,
-                            "_order": sent_index,
-                        }
-                    )
-
-            return {dataset_id: documents for dataset_id in self.output_dataset_ids}
-
-    output_dataset_ids = (dense_output_dataset1.dataset_id, dense_output_dataset2.dataset_id)
-    return TestDenseOperator(output_dataset_ids)
-
-
-@pytest.fixture(scope="function")
-def test_engine(full_dataset: Dataset, test_operator: AbstractOperator) -> StableEngine:
-    return StableEngine(dataset=full_dataset, operator=test_operator)
-
-
-@pytest.fixture(scope="function")
-def test_paid_engine(full_dataset: Dataset, test_paid_operator: AbstractOperator) -> StableEngine:
-    return StableEngine(dataset=full_dataset, operator=test_paid_operator)
-
-
-@pytest.fixture(scope="function")
-def test_paid_engine_no_refresh(full_dataset: Dataset, test_paid_operator: AbstractOperator) -> StableEngine:
-    return StableEngine(dataset=full_dataset, operator=test_paid_operator, refresh=False)
-
-
-@pytest.fixture(scope="function")
-def test_sentiment_workflow_token(test_client: Client) -> str:
-    salt = "".join(random.choices(string.ascii_lowercase, k=10))
-    dataset_id = f"_sample_dataset_{salt}"
-    dataset = test_client.Dataset(dataset_id, expire=True)
-    dataset.insert_documents(incomplete_documents(20))
-    time.sleep(1)
-    job_id = str(uuid.uuid4())
-    config = dict(
-        job_id=job_id,
-        authorizationToken=test_client.credentials.token,
-        dataset_id=dataset_id,
-        text_field="sample_1_label",
-    )
-    config_string = json.dumps(config)
-    config_bytes = config_string.encode()
-    workflow_token = base64.b64encode(config_bytes).decode()
-    yield workflow_token
-    test_client.delete_dataset(dataset_id)
-
-
-@pytest.fixture(scope="function")
-def test_user_facing_error_workflow_token(test_client: Client) -> str:
-    salt = "".join(random.choices(string.ascii_lowercase, k=10))
-    dataset_id = f"_sample_dataset_{salt}"
-    dataset = test_client.Dataset(dataset_id, expire=True)
-    dataset.insert_documents(mock_documents(20))
-    time.sleep(1)
-    job_id = str(uuid.uuid4())
-    config = dict(
-        job_id=job_id,
-        dataset_id=dataset_id,
-        authorizationToken=test_client.credentials.token,
-        text_field="sample_1_description",
-    )
-    config_string = json.dumps(config)
-    config_bytes = config_string.encode()
-    workflow_token = base64.b64encode(config_bytes).decode()
-    yield workflow_token
-    test_client.delete_dataset(dataset_id)
-
-
-@pytest.fixture(scope="function")
-def test_sentiment_workflow_document_token(test_client: Client) -> str:
-    salt = "".join(random.choices(string.ascii_lowercase, k=10))
-    time.sleep(1)
-    job_id = str(uuid.uuid4())
-    config = dict(
-        job_id=job_id,
-        authorizationToken=test_client.credentials.token,
-        text_field="sample_1_label",
-        documents=mock_documents(10).to_json(),
-    )
-    config_string = json.dumps(config)
-    config_bytes = config_string.encode()
-    workflow_token = base64.b64encode(config_bytes).decode()
-    yield workflow_token
-
-
-@pytest.fixture(scope="function")
-def test_simple_workflow_token(test_client: Client) -> str:
-    salt = "".join(random.choices(string.ascii_lowercase, k=10))
-    dataset_id = f"_sample_dataset_{salt}"
-    dataset = test_client.Dataset(dataset_id, expire=True)
-    dataset.insert_documents(mock_documents(20))
-    time.sleep(1)
-    job_id = str(uuid.uuid4())
-    config = dict(
-        job_id=job_id, authorizationToken=test_client.credentials.token, dataset_id=dataset_id, send_email=True
-    )
-    config_string = json.dumps(config)
-    config_bytes = config_string.encode()
-    workflow_token = base64.b64encode(config_bytes).decode()
-    yield workflow_token
-    test_client.delete_dataset(dataset_id)
-
-
-@pytest.fixture(scope="function")
-def test_cluster_workflow_token(test_client: Client) -> str:
-    salt = "".join(random.choices(string.ascii_lowercase, k=10))
-    dataset_id = f"_sample_dataset_{salt}"
-    dataset = test_client.Dataset(dataset_id, expire=True)
-    dataset.insert_documents(incomplete_documents(20))
-    job_id = str(uuid.uuid4())
-    print(job_id)
-    config = dict(
-        job_id=job_id,
-        authorizationToken=test_client.credentials.token,
-        dataset_id=dataset_id,
-        vector_fields=["sample_1_vector_"],
-    )
-    config_string = json.dumps(config)
-    config_bytes = config_string.encode()
-    workflow_token = base64.b64encode(config_bytes).decode()
-    yield workflow_token
-    test_client.delete_dataset(dataset_id)
-
-
-@pytest.fixture(scope="function")
-def test_org_error_workflow_token(test_client: Client) -> str:
-    salt = "".join(random.choices(string.ascii_lowercase, k=10))
-    dataset_id = f"_sample_dataset_{salt}"
-    dataset = test_client.Dataset(dataset_id, expire=True)
-    dataset.insert_documents(incomplete_documents(20))
-    job_id = str(uuid.uuid4())
-    print(job_id)
-    config = dict(
-        job_id=job_id,
-        authorizationToken=test_client.credentials.token,
-        dataset_id=dataset_id,
-        vector_fields=["sample_1_vector_"],
-    )
-    config_string = json.dumps(config)
-    config_bytes = config_string.encode()
-    workflow_token = base64.b64encode(config_bytes).decode()
-    yield workflow_token
-    test_client.delete_dataset(dataset_id)
-
-
-@pytest.fixture()
-def test_keyphrases() -> List[Dict]:
-    return [
-        {
-            "text": "word",
-            "_id": "word",
-            "ancestors": [],
-            "parents": [],
-            "level": 1,
-            "keyphrase_score": 10,
-            "frequency": 3,
-            "metadata": {},
-        },
-        {
-            "text": "cat",
-            "_id": "cat",
-            "ancestors": ["word"],
-            "parents": ["word"],
-            "level": 0,
-            "keyphrase_score": 6.4,
-            "frequency": 7,
-            "metadata": {},
-        },
-    ]
-
-
-@pytest.fixture()
-def test_keyphrase_dataset(test_client: Client, test_dataset_id: str) -> Dataset:
-    docs = mock_documents(100)
-    dataset = test_client.Dataset((test_dataset_id), expire=True)
-    dataset.insert_documents(docs, ingest_in_background=False)
-    yield dataset
-    dataset.delete()
+import os
+import json
+import uuid
+import time
+import base64
+import random
+import pytest
+import string
+
+from typing import List, Dict, Sequence
+
+from ai_transform.api.client import Client
+from ai_transform.api.helpers import process_token
+
+from ai_transform.dataset.dataset import Dataset
+
+from ai_transform.engine.stable_engine import StableEngine
+
+from ai_transform.operator.abstract_operator import AbstractOperator
+from ai_transform.operator.dense_operator import DenseOperator
+
+from ai_transform.utils.document import Document
+from ai_transform.utils.document_list import DocumentList
+from ai_transform.utils.example_documents import (
+    mock_documents,
+    static_documents,
+    tag_documents,
+    generate_random_vector,
+    incomplete_documents,
+)
+
+
+TEST_TOKEN = os.getenv("TEST_TOKEN")
+test_creds = process_token(TEST_TOKEN)
+
+
+@pytest.fixture(scope="session")
+def test_token() -> str:
+    return TEST_TOKEN
+
+
+@pytest.fixture(scope="session")
+def test_client(test_token: str) -> Client:
+    return Client(test_token)
+
+
+@pytest.fixture(scope="function")
+def test_dataset_id() -> str:
+    salt = "".join(random.choices(string.ascii_lowercase, k=10))
+    dataset_id = f"_sample_dataset_{salt}"
+    return dataset_id
+
+
+@pytest.fixture(scope="function")
+def empty_dataset(test_client: Client) -> Dataset:
+    salt = "".join(random.choices(string.ascii_lowercase, k=10))
+    dataset_id = f"_sample_dataset_{salt}"
+    dataset = test_client.Dataset(dataset_id, expire=False)
+    yield dataset
+    test_client.delete_dataset(dataset_id)
+
+
+@pytest.fixture(scope="class")
+def full_dataset(test_client: Client) -> Dataset:
+    salt = "".join(random.choices(string.ascii_lowercase, k=10))
+    dataset_id = f"_sample_dataset_{salt}"
+    dataset = test_client.Dataset(dataset_id, expire=True)
+    dataset.insert_documents(mock_documents(20))
+    yield dataset
+    test_client.delete_dataset(dataset_id)
+
+
+@pytest.fixture(scope="class")
+def partial_dataset(test_client: Client) -> Dataset:
+    salt = "".join(random.choices(string.ascii_lowercase, k=10))
+    dataset_id = f"_sample_dataset_{salt}"
+    dataset = test_client.Dataset(dataset_id, expire=True)
+    documents = mock_documents(1000)
+    fields = ["sample_1_label", "sample_2_label", "sample_3_label"]
+    for document in documents:
+        for field in random.sample(fields, k=random.randint(1, 3)):
+            document.pop(field)
+    dataset.insert_documents(documents)
+    yield dataset
+    test_client.delete_dataset(dataset_id)
+
+
+@pytest.fixture(scope="class")
+def simple_partial_dataset(test_client: Client) -> Dataset:
+    salt = "".join(random.choices(string.ascii_lowercase, k=10))
+    dataset_id = f"_sample_dataset_{salt}"
+    dataset = test_client.Dataset(dataset_id, expire=True)
+    documents = mock_documents(1000)
+    fields = ["sample_1_label"]
+    for document in documents:
+        if random.random() < 0.5:
+            document.pop(fields[0])
+    dataset.insert_documents(documents)
+    yield dataset
+    test_client.delete_dataset(dataset_id)
+
+
+@pytest.fixture(scope="class")
+def partial_dataset_with_outputs(test_client: Client) -> Dataset:
+    salt = "".join(random.choices(string.ascii_lowercase, k=10))
+    dataset_id = f"_sample_dataset_{salt}"
+    dataset = test_client.Dataset(dataset_id, expire=True)
+    documents = mock_documents(1000)
+    fields = ["sample_1_label", "sample_2_label", "sample_3_label"]
+    for document in documents:
+        for field in random.sample(fields, k=random.randint(1, 3)):
+            document.pop(field)
+    for document in documents:
+        for field in fields:
+            if document.get(field) and random.random() < 0.5:
+                document[field + "_output"] = document[field] + "_output"
+    dataset.insert_documents(documents)
+    yield dataset
+    test_client.delete_dataset(dataset_id)
+
+
+@pytest.fixture(scope="class")
+def mixed_dataset(test_client: Client) -> Dataset:
+    salt = "".join(random.choices(string.ascii_lowercase, k=10))
+    dataset_id = f"_sample_dataset_{salt}"
+    dataset = test_client.Dataset(dataset_id, expire=True)
+    documents = mock_documents(10)
+    stripped = mock_documents(10)
+    for document in stripped:
+        document.pop("_chunk_")
+    documents += stripped
+    dataset.insert_documents(documents)
+    yield dataset
+    test_client.delete_dataset(dataset_id)
+
+
+@pytest.fixture(scope="class")
+def static_dataset(test_client: Client) -> Dataset:
+    salt = "".join(random.choices(string.ascii_lowercase, k=10))
+    dataset_id = f"_sample_dataset_{salt}"
+    dataset = test_client.Dataset(dataset_id, expire=True)
+    dataset.insert_documents(static_documents(20))
+    yield dataset
+    test_client.delete_dataset(dataset_id)
+
+
+@pytest.fixture(scope="function")
+def dense_input_dataset1(test_client: Client) -> Dataset:
+    salt = "".join(random.choices(string.ascii_lowercase, k=10))
+    dataset_id = f"_sample_dataset_{salt}"
+    dataset = test_client.Dataset(dataset_id, expire=True)
+    dataset.insert_documents(static_documents(2))
+    yield dataset
+    test_client.delete_dataset(dataset_id)
+
+
+@pytest.fixture(scope="function")
+def dense_input_dataset2(test_client: Client) -> Dataset:
+    salt = "".join(random.choices(string.ascii_lowercase, k=10))
+    dataset_id = f"_sample_dataset_{salt}"
+    dataset = test_client.Dataset(dataset_id, expire=True)
+    dataset.insert_documents(mock_documents(100))
+    yield dataset
+    test_client.delete_dataset(dataset_id)
+
+
+@pytest.fixture(scope="function")
+def dense_output_dataset1(test_client: Client) -> Dataset:
+    salt = "".join(random.choices(string.ascii_lowercase, k=10))
+    dataset_id = f"_sample_dataset_{salt}"
+    dataset = test_client.Dataset(dataset_id, expire=True)
+    yield dataset
+    test_client.delete_dataset(dataset_id)
+
+
+@pytest.fixture(scope="function")
+def dense_output_dataset2(test_client: Client) -> Dataset:
+    salt = "".join(random.choices(string.ascii_lowercase, k=10))
+    dataset_id = f"_sample_dataset_{salt}"
+    dataset = test_client.Dataset(dataset_id, expire=True)
+    yield dataset
+    test_client.delete_dataset(dataset_id)
+
+
+@pytest.fixture(scope="function")
+def test_document() -> Document:
+    raw_dict = {"field1": {"field2": 1}, "field3": 3}
+    return Document(raw_dict)
+
+
+@pytest.fixture(scope="function")
+def test_documents() -> DocumentList:
+    return mock_documents()
+
+
+@pytest.fixture(scope="function")
+def test_tag_documents() -> DocumentList:
+    return tag_documents()
+
+
+@pytest.fixture(scope="function")
+def test_operator() -> AbstractOperator:
+    class ExampleOperator(AbstractOperator):
+        def transform(self, documents: DocumentList) -> DocumentList:
+            """
+            Main transform function
+            """
+            for document in documents:
+                if "new_field" not in document:
+                    document["new_field"] = 0
+
+                document["new_field"] += 3
+
+            return documents
+
+    return ExampleOperator()
+
+
+@pytest.fixture(scope="function")
+def test_partial_operator() -> AbstractOperator:
+    class PartialOperator(AbstractOperator):
+        def __init__(self, fields):
+            super().__init__(input_fields=fields, output_fields=[field + "_output" for field in fields])
+
+        def transform(self, documents: DocumentList) -> DocumentList:
+            """
+            Main transform function
+            """
+            for input_field, output_field in zip(self.input_fields, self.output_fields):
+                for document in documents:
+                    if document.get(input_field):
+                        document[output_field] = document[input_field] + "_output"
+
+            return documents
+
+    return PartialOperator
+
+
+@pytest.fixture(scope="function")
+def test_paid_operator() -> AbstractOperator:
+    class ExampleOperator(AbstractOperator):
+        def __init__(self):
+            super().__init__()
+
+        def transform(self, documents: DocumentList) -> DocumentList:
+            """
+            Main transform function
+            """
+            for document in documents:
+                if "new_field" not in document:
+                    document["new_field"] = 0
+
+                document["new_field"] += 3
+                self.n_processed_pricing += 1
+
+            return documents
+
+    return ExampleOperator()
+
+
+@pytest.fixture(scope="function")
+def test_dense_operator(dense_output_dataset1: Dataset, dense_output_dataset2: Dataset) -> DenseOperator:
+    class TestDenseOperator(DenseOperator):
+        def __init__(self, output_dataset_ids: Sequence[str]):
+            self.output_dataset_ids = output_dataset_ids
+            super().__init__()
+
+        def transform(self, documents: DocumentList) -> DocumentList:
+            """
+            Main transform function
+            """
+            for document in documents:
+                if "new_field" not in document:
+                    document["new_field"] = 0
+
+                document["new_field"] += 3
+
+            return {dataset_id: documents for dataset_id in self.output_dataset_ids}
+
+    output_dataset_ids = (dense_output_dataset1.dataset_id, dense_output_dataset2.dataset_id)
+    return TestDenseOperator(output_dataset_ids)
+
+
+@pytest.fixture(scope="function")
+def test_chunk_dense_operator(dense_output_dataset1: Dataset, dense_output_dataset2: Dataset) -> DenseOperator:
+    class TestDenseOperator(DenseOperator):
+        def __init__(self, output_dataset_ids: Sequence[str]):
+            self.output_dataset_ids = output_dataset_ids
+            self._chunk_field = "_chunk_"
+            self._text_field = "label"
+            self._alias = "default"
+            super().__init__()
+
+        def transform(self, documents: List[Document]) -> List[Document]:
+            outputs = []
+            for document in documents:
+                texts = document.get_chunk(chunk_field=self._chunk_field, field=self._text_field)
+                text_vectors = [generate_random_vector() for _ in range(len(texts))]
+
+                for sent_index, text_vector in enumerate(text_vectors):
+                    outputs.append(
+                        {
+                            "_id": document["_id"] + f":{sent_index}",
+                            f"{self._text_field}_{self._alias}_vector_": text_vector,
+                            "_order": sent_index,
+                        }
+                    )
+
+            return {dataset_id: documents for dataset_id in self.output_dataset_ids}
+
+    output_dataset_ids = (dense_output_dataset1.dataset_id, dense_output_dataset2.dataset_id)
+    return TestDenseOperator(output_dataset_ids)
+
+
+@pytest.fixture(scope="function")
+def test_engine(full_dataset: Dataset, test_operator: AbstractOperator) -> StableEngine:
+    return StableEngine(dataset=full_dataset, operator=test_operator)
+
+
+@pytest.fixture(scope="function")
+def test_paid_engine(full_dataset: Dataset, test_paid_operator: AbstractOperator) -> StableEngine:
+    return StableEngine(dataset=full_dataset, operator=test_paid_operator)
+
+
+@pytest.fixture(scope="function")
+def test_paid_engine_no_refresh(full_dataset: Dataset, test_paid_operator: AbstractOperator) -> StableEngine:
+    return StableEngine(dataset=full_dataset, operator=test_paid_operator, refresh=False)
+
+
+@pytest.fixture(scope="function")
+def test_sentiment_workflow_token(test_client: Client) -> str:
+    salt = "".join(random.choices(string.ascii_lowercase, k=10))
+    dataset_id = f"_sample_dataset_{salt}"
+    dataset = test_client.Dataset(dataset_id, expire=True)
+    dataset.insert_documents(incomplete_documents(20))
+    time.sleep(1)
+    job_id = str(uuid.uuid4())
+    config = dict(
+        job_id=job_id,
+        authorizationToken=test_client.credentials.token,
+        dataset_id=dataset_id,
+        text_field="sample_1_label",
+    )
+    config_string = json.dumps(config)
+    config_bytes = config_string.encode()
+    workflow_token = base64.b64encode(config_bytes).decode()
+    yield workflow_token
+    test_client.delete_dataset(dataset_id)
+
+
+@pytest.fixture(scope="function")
+def test_user_facing_error_workflow_token(test_client: Client) -> str:
+    salt = "".join(random.choices(string.ascii_lowercase, k=10))
+    dataset_id = f"_sample_dataset_{salt}"
+    dataset = test_client.Dataset(dataset_id, expire=True)
+    dataset.insert_documents(mock_documents(20))
+    time.sleep(1)
+    job_id = str(uuid.uuid4())
+    config = dict(
+        job_id=job_id,
+        dataset_id=dataset_id,
+        authorizationToken=test_client.credentials.token,
+        text_field="sample_1_description",
+    )
+    config_string = json.dumps(config)
+    config_bytes = config_string.encode()
+    workflow_token = base64.b64encode(config_bytes).decode()
+    yield workflow_token
+    test_client.delete_dataset(dataset_id)
+
+
+@pytest.fixture(scope="function")
+def test_sentiment_workflow_document_token(test_client: Client) -> str:
+    salt = "".join(random.choices(string.ascii_lowercase, k=10))
+    time.sleep(1)
+    job_id = str(uuid.uuid4())
+    config = dict(
+        job_id=job_id,
+        authorizationToken=test_client.credentials.token,
+        text_field="sample_1_label",
+        documents=mock_documents(10).to_json(),
+    )
+    config_string = json.dumps(config)
+    config_bytes = config_string.encode()
+    workflow_token = base64.b64encode(config_bytes).decode()
+    yield workflow_token
+
+
+@pytest.fixture(scope="function")
+def test_simple_workflow_token(test_client: Client) -> str:
+    salt = "".join(random.choices(string.ascii_lowercase, k=10))
+    dataset_id = f"_sample_dataset_{salt}"
+    dataset = test_client.Dataset(dataset_id, expire=True)
+    dataset.insert_documents(mock_documents(20))
+    time.sleep(1)
+    job_id = str(uuid.uuid4())
+    config = dict(
+        job_id=job_id, authorizationToken=test_client.credentials.token, dataset_id=dataset_id, send_email=True
+    )
+    config_string = json.dumps(config)
+    config_bytes = config_string.encode()
+    workflow_token = base64.b64encode(config_bytes).decode()
+    yield workflow_token
+    test_client.delete_dataset(dataset_id)
+
+
+@pytest.fixture(scope="function")
+def test_cluster_workflow_token(test_client: Client) -> str:
+    salt = "".join(random.choices(string.ascii_lowercase, k=10))
+    dataset_id = f"_sample_dataset_{salt}"
+    dataset = test_client.Dataset(dataset_id, expire=True)
+    dataset.insert_documents(incomplete_documents(20))
+    job_id = str(uuid.uuid4())
+    print(job_id)
+    config = dict(
+        job_id=job_id,
+        authorizationToken=test_client.credentials.token,
+        dataset_id=dataset_id,
+        vector_fields=["sample_1_vector_"],
+    )
+    config_string = json.dumps(config)
+    config_bytes = config_string.encode()
+    workflow_token = base64.b64encode(config_bytes).decode()
+    yield workflow_token
+    test_client.delete_dataset(dataset_id)
+
+
+@pytest.fixture(scope="function")
+def test_org_error_workflow_token(test_client: Client) -> str:
+    salt = "".join(random.choices(string.ascii_lowercase, k=10))
+    dataset_id = f"_sample_dataset_{salt}"
+    dataset = test_client.Dataset(dataset_id, expire=True)
+    dataset.insert_documents(incomplete_documents(20))
+    job_id = str(uuid.uuid4())
+    print(job_id)
+    config = dict(
+        job_id=job_id,
+        authorizationToken=test_client.credentials.token,
+        dataset_id=dataset_id,
+        vector_fields=["sample_1_vector_"],
+    )
+    config_string = json.dumps(config)
+    config_bytes = config_string.encode()
+    workflow_token = base64.b64encode(config_bytes).decode()
+    yield workflow_token
+    test_client.delete_dataset(dataset_id)
+
+
+@pytest.fixture()
+def test_keyphrases() -> List[Dict]:
+    return [
+        {
+            "text": "word",
+            "_id": "word",
+            "ancestors": [],
+            "parents": [],
+            "level": 1,
+            "keyphrase_score": 10,
+            "frequency": 3,
+            "metadata": {},
+        },
+        {
+            "text": "cat",
+            "_id": "cat",
+            "ancestors": ["word"],
+            "parents": ["word"],
+            "level": 0,
+            "keyphrase_score": 6.4,
+            "frequency": 7,
+            "metadata": {},
+        },
+    ]
+
+
+@pytest.fixture()
+def test_keyphrase_dataset(test_client: Client, test_dataset_id: str) -> Dataset:
+    docs = mock_documents(100)
+    dataset = test_client.Dataset((test_dataset_id), expire=True)
+    dataset.insert_documents(docs, ingest_in_background=False)
+    yield dataset
+    dataset.delete()
```

### Comparing `ai_transform-0.32.3/tests/core/test_api/test_endpoints.py` & `ai_transform-0.32.4/tests/core/test_api/test_endpoints.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-import pytest
-import os
-from ai_transform.api.client import Client
-
-
-class TestEndpoints:
-    def test_generic_request(self, test_client: Client):
-        resp = test_client.api.post("/auth/users/list")
-        resp = test_client.api.get("/health")
-        assert resp.status_code == 200
-        assert resp.status_code == 200
-
-
-@pytest.mark.skip(reason="Don't hit openai")
-def test_proxy_openai(test_client: Client):
-    body = {
-        "model": f"gpt-3.5-turbo",
-        "messages": [
-            {"role": "system", "content": "You are a translator."},
-            {
-                "role": "assistant",
-                "content": """Example response:
-{"detected_language" : The detected language, "translated_text": The translated text}
-""",
-            },
-            {"role": "user", "content": "Example"},
-        ],
-        "temperature": 0,
-        "n": 1,
-        "presence_penalty": 0,
-        "frequency_penalty": 0,
-    }
-    response = test_client._api._proxy_openai(
-        workflows_admin_token=os.environ["WORKFLOW_ADMIN_TOKEN"], body=body, endpoint="/v1/chat/completions"
-    )
-    assert "choices" in response
+import pytest
+import os
+from ai_transform.api.client import Client
+
+
+class TestEndpoints:
+    def test_generic_request(self, test_client: Client):
+        resp = test_client.api.post("/auth/users/list")
+        resp = test_client.api.get("/health")
+        assert resp.status_code == 200
+        assert resp.status_code == 200
+
+
+@pytest.mark.skip(reason="Don't hit openai")
+def test_proxy_openai(test_client: Client):
+    body = {
+        "model": f"gpt-3.5-turbo",
+        "messages": [
+            {"role": "system", "content": "You are a translator."},
+            {
+                "role": "assistant",
+                "content": """Example response:
+{"detected_language" : The detected language, "translated_text": The translated text}
+""",
+            },
+            {"role": "user", "content": "Example"},
+        ],
+        "temperature": 0,
+        "n": 1,
+        "presence_penalty": 0,
+        "frequency_penalty": 0,
+    }
+    response = test_client._api._proxy_openai(
+        workflows_admin_token=os.environ["WORKFLOW_ADMIN_TOKEN"], body=body, endpoint="/v1/chat/completions"
+    )
+    assert "choices" in response
```

### Comparing `ai_transform-0.32.3/tests/core/test_api/test_keyphrase.py` & `ai_transform-0.32.4/tests/core/test_api/test_keyphrase.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-"""
-Test Keyphrase CRUD endpoints
-"""
-import uuid
-
-from ai_transform.utils import List
-from ai_transform.dataset.dataset import Dataset
-from ai_transform.api.client import Client
-from ai_transform.utils.keyphrase import Keyphrase
-
-
-# write a few tests
-class TestClient:
-    def test_upsert_keyphrases(
-        self, test_client: Client, test_keyphrase_dataset: Dataset, test_keyphrases: List[Keyphrase]
-    ):
-        # Test that upserting keyphrases is good
-        field = "sample_1_label"
-        alias = "default"
-        test_dataset_id = test_keyphrase_dataset.dataset_id
-
-        result = test_client.api._bulk_update_keyphrase(
-            dataset_id=test_dataset_id, field=field, alias=alias, updates=test_keyphrases
-        )
-        # Now that that we saw the actual dataset
-        result = test_client.api._get_keyphrase(test_dataset_id, field=field, alias=alias, keyphrase_id="word")
-        print(result)
-        assert result["text"] == "word" and result["keyphrase_score"] == 10, result
+"""
+Test Keyphrase CRUD endpoints
+"""
+import uuid
+
+from ai_transform.utils import List
+from ai_transform.dataset.dataset import Dataset
+from ai_transform.api.client import Client
+from ai_transform.utils.keyphrase import Keyphrase
+
+
+# write a few tests
+class TestClient:
+    def test_upsert_keyphrases(
+        self, test_client: Client, test_keyphrase_dataset: Dataset, test_keyphrases: List[Keyphrase]
+    ):
+        # Test that upserting keyphrases is good
+        field = "sample_1_label"
+        alias = "default"
+        test_dataset_id = test_keyphrase_dataset.dataset_id
+
+        result = test_client.api._bulk_update_keyphrase(
+            dataset_id=test_dataset_id, field=field, alias=alias, updates=test_keyphrases
+        )
+        # Now that that we saw the actual dataset
+        result = test_client.api._get_keyphrase(test_dataset_id, field=field, alias=alias, keyphrase_id="word")
+        print(result)
+        assert result["text"] == "word" and result["keyphrase_score"] == 10, result
```

### Comparing `ai_transform-0.32.3/tests/core/test_dataset/test_dataset.py` & `ai_transform-0.32.4/tests/core/test_dataset/test_dataset.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,145 +1,145 @@
-import pytest
-import random
-
-from ai_transform.dataset.dataset import Dataset
-from ai_transform.utils.example_documents import mock_documents
-
-
-class TestDataset1:
-    def test_insert(self, empty_dataset: Dataset):
-        documents = mock_documents(100)
-        result = empty_dataset.insert_documents(documents)
-        assert result["inserted"] == 100
-
-    def test_get_all(self, full_dataset: Dataset):
-        res = full_dataset.get_all_documents()
-        assert len(res["documents"]) == 20
-
-    def test_create_delete(self, empty_dataset: Dataset):
-        empty_dataset.delete()
-        empty_dataset.create()
-        assert True
-
-
-@pytest.mark.usefixtures("full_dataset")
-class TestDataset2:
-    def test_schema(self, full_dataset: Dataset):
-        documents = mock_documents(5)
-        keys = documents[0].keys()
-        keys = [".".join([sf for sf in nested_field.split(".") if not sf.isdigit()]) for nested_field in keys]
-        schema = full_dataset.schema
-        assert all([key in schema for key in keys if key not in ["_id"]])
-
-    def test_series(self, full_dataset: Dataset):
-        schema = full_dataset.schema
-        series = full_dataset[random.choice(list(schema.keys()))]
-        assert True
-
-    def test_update(self, full_dataset: Dataset):
-        old_documents = full_dataset.get_documents(20)["documents"]
-        for document in old_documents:
-            document["sample_1_value"] += 1
-        res = full_dataset.update_documents(old_documents)
-        assert not res["failed_documents"]
-
-    def test_metadata(self, full_dataset: Dataset):
-        metadata = full_dataset.get_metadata()["results"]
-        assert metadata == {}
-
-        new_metadata = {"_metadata_": 4}
-        full_dataset.insert_metadata(new_metadata)
-        metadata = full_dataset.get_metadata()["results"]
-        assert metadata == new_metadata
-
-        new_metadata = {"_metadata_": 4, "_metadata1_": 5}
-        full_dataset.update_metadata(new_metadata)
-        metadata = full_dataset.get_metadata()["results"]
-        assert "_metadata1_" in metadata
-        assert "_metadata_" in metadata
-
-
-@pytest.mark.usefixtures("static_dataset")
-class TestFilters:
-    def test_equals(self, static_dataset: Dataset):
-        filters = static_dataset["numeric_field"] == 5
-        res = static_dataset.get_documents(page_size=1, filters=filters)
-        documents = res["documents"]
-        assert res["count"] == 1
-        assert documents[0]["numeric_field"] == 5
-
-    def test_less_than(self, static_dataset: Dataset):
-        filters = static_dataset["numeric_field"] < 5
-        res = static_dataset.get_documents(page_size=20, filters=filters)
-        assert res["count"] == 5
-
-    def test_greater_than(self, static_dataset: Dataset):
-        filters = static_dataset["numeric_field"] > 5
-        res = static_dataset.get_documents(page_size=20, filters=filters)
-        assert res["count"] == 14
-
-    def test_less_than_equal_to(self, static_dataset: Dataset):
-        filters = static_dataset["numeric_field"] >= 5
-        res = static_dataset.get_documents(page_size=20, filters=filters)
-        assert res["count"] == 15
-
-    def test_greater_than_equal_to(self, static_dataset: Dataset):
-        filters = static_dataset["numeric_field"] <= 5
-        res = static_dataset.get_documents(page_size=20, filters=filters)
-        assert res["count"] == 6
-
-    def test_exists(self, static_dataset: Dataset):
-        filters = static_dataset["numeric_field"].exists()
-        res = static_dataset.get_documents(page_size=20, filters=filters)
-        assert res["count"] == 20
-
-    def test_not_exists(self, static_dataset: Dataset):
-        filters = static_dataset["numeric_field"].not_exists()
-        res = static_dataset.get_documents(page_size=20, filters=filters)
-        assert res["count"] == 0
-
-    def test_not_exists_for_field_dne(self, static_dataset: Dataset):
-        filters = static_dataset["this_field_does_not_exist"].not_exists()
-        res = static_dataset.get_documents(page_size=20, filters=filters)
-        assert res["count"] == 20
-
-    def test_contains(self, static_dataset: Dataset):
-        filters = static_dataset["text_field"].contains("3")
-        res = static_dataset.get_documents(page_size=20, filters=filters)
-        documents = res["documents"]
-        values = list(map(lambda document: document["text_field"], documents))
-        assert res["count"] == 2
-        assert all([value in values for value in {"3", "13"}])
-
-    def test_ids(self, static_dataset: Dataset):
-        res = static_dataset.get_documents(page_size=20)
-        documents = res["documents"]
-        _ids = list(map(lambda document: document["_id"], documents))
-        filters = static_dataset["_id"] == random.choice(_ids)
-        res = static_dataset.get_documents(page_size=20, filters=filters)
-        assert res["count"] == 1
-
-    @pytest.mark.xfail(reason="api bug")
-    def test_date(self, static_dataset: Dataset):
-        res = static_dataset.get_documents(page_size=20)
-        documents = res["documents"]
-        dates = list(map(lambda document: document["insert_date_"], documents))
-        filters = static_dataset["insert_date_"] == random.choice(dates)
-        res = static_dataset.get_documents(page_size=20, filters=filters)
-        assert res["count"] == 1
-
-
-class TestDatasetMedia:
-    def test_upload_medias(self, empty_dataset: Dataset):
-        urls = empty_dataset.insert_local_medias(["hierarchy.png", "hierarchy.png", "hierarchy.png"])
-        assert len(urls) == 3
-
-
-class TestChunkFilters:
-    def test_chunk_filters(self, mixed_dataset: Dataset):
-        filters = mixed_dataset["_chunk_.label"].exists()
-        filtered = mixed_dataset.get_documents(100, filters=filters)
-        assert filtered["count"] == 10
-
-        filters = mixed_dataset["_chunk_.label_chunkvector_"].exists()
-        filtered = mixed_dataset.get_documents(100, filters=filters)
-        assert filtered["count"] == 10
+import pytest
+import random
+
+from ai_transform.dataset.dataset import Dataset
+from ai_transform.utils.example_documents import mock_documents
+
+
+class TestDataset1:
+    def test_insert(self, empty_dataset: Dataset):
+        documents = mock_documents(100)
+        result = empty_dataset.insert_documents(documents)
+        assert result["inserted"] == 100
+
+    def test_get_all(self, full_dataset: Dataset):
+        res = full_dataset.get_all_documents()
+        assert len(res["documents"]) == 20
+
+    def test_create_delete(self, empty_dataset: Dataset):
+        empty_dataset.delete()
+        empty_dataset.create()
+        assert True
+
+
+@pytest.mark.usefixtures("full_dataset")
+class TestDataset2:
+    def test_schema(self, full_dataset: Dataset):
+        documents = mock_documents(5)
+        keys = documents[0].keys()
+        keys = [".".join([sf for sf in nested_field.split(".") if not sf.isdigit()]) for nested_field in keys]
+        schema = full_dataset.schema
+        assert all([key in schema for key in keys if key not in ["_id"]])
+
+    def test_series(self, full_dataset: Dataset):
+        schema = full_dataset.schema
+        series = full_dataset[random.choice(list(schema.keys()))]
+        assert True
+
+    def test_update(self, full_dataset: Dataset):
+        old_documents = full_dataset.get_documents(20)["documents"]
+        for document in old_documents:
+            document["sample_1_value"] += 1
+        res = full_dataset.update_documents(old_documents)
+        assert not res["failed_documents"]
+
+    def test_metadata(self, full_dataset: Dataset):
+        metadata = full_dataset.get_metadata()["results"]
+        assert metadata == {}
+
+        new_metadata = {"_metadata_": 4}
+        full_dataset.insert_metadata(new_metadata)
+        metadata = full_dataset.get_metadata()["results"]
+        assert metadata == new_metadata
+
+        new_metadata = {"_metadata_": 4, "_metadata1_": 5}
+        full_dataset.update_metadata(new_metadata)
+        metadata = full_dataset.get_metadata()["results"]
+        assert "_metadata1_" in metadata
+        assert "_metadata_" in metadata
+
+
+@pytest.mark.usefixtures("static_dataset")
+class TestFilters:
+    def test_equals(self, static_dataset: Dataset):
+        filters = static_dataset["numeric_field"] == 5
+        res = static_dataset.get_documents(page_size=1, filters=filters)
+        documents = res["documents"]
+        assert res["count"] == 1
+        assert documents[0]["numeric_field"] == 5
+
+    def test_less_than(self, static_dataset: Dataset):
+        filters = static_dataset["numeric_field"] < 5
+        res = static_dataset.get_documents(page_size=20, filters=filters)
+        assert res["count"] == 5
+
+    def test_greater_than(self, static_dataset: Dataset):
+        filters = static_dataset["numeric_field"] > 5
+        res = static_dataset.get_documents(page_size=20, filters=filters)
+        assert res["count"] == 14
+
+    def test_less_than_equal_to(self, static_dataset: Dataset):
+        filters = static_dataset["numeric_field"] >= 5
+        res = static_dataset.get_documents(page_size=20, filters=filters)
+        assert res["count"] == 15
+
+    def test_greater_than_equal_to(self, static_dataset: Dataset):
+        filters = static_dataset["numeric_field"] <= 5
+        res = static_dataset.get_documents(page_size=20, filters=filters)
+        assert res["count"] == 6
+
+    def test_exists(self, static_dataset: Dataset):
+        filters = static_dataset["numeric_field"].exists()
+        res = static_dataset.get_documents(page_size=20, filters=filters)
+        assert res["count"] == 20
+
+    def test_not_exists(self, static_dataset: Dataset):
+        filters = static_dataset["numeric_field"].not_exists()
+        res = static_dataset.get_documents(page_size=20, filters=filters)
+        assert res["count"] == 0
+
+    def test_not_exists_for_field_dne(self, static_dataset: Dataset):
+        filters = static_dataset["this_field_does_not_exist"].not_exists()
+        res = static_dataset.get_documents(page_size=20, filters=filters)
+        assert res["count"] == 20
+
+    def test_contains(self, static_dataset: Dataset):
+        filters = static_dataset["text_field"].contains("3")
+        res = static_dataset.get_documents(page_size=20, filters=filters)
+        documents = res["documents"]
+        values = list(map(lambda document: document["text_field"], documents))
+        assert res["count"] == 2
+        assert all([value in values for value in {"3", "13"}])
+
+    def test_ids(self, static_dataset: Dataset):
+        res = static_dataset.get_documents(page_size=20)
+        documents = res["documents"]
+        _ids = list(map(lambda document: document["_id"], documents))
+        filters = static_dataset["_id"] == random.choice(_ids)
+        res = static_dataset.get_documents(page_size=20, filters=filters)
+        assert res["count"] == 1
+
+    @pytest.mark.xfail(reason="api bug")
+    def test_date(self, static_dataset: Dataset):
+        res = static_dataset.get_documents(page_size=20)
+        documents = res["documents"]
+        dates = list(map(lambda document: document["insert_date_"], documents))
+        filters = static_dataset["insert_date_"] == random.choice(dates)
+        res = static_dataset.get_documents(page_size=20, filters=filters)
+        assert res["count"] == 1
+
+
+class TestDatasetMedia:
+    def test_upload_medias(self, empty_dataset: Dataset):
+        urls = empty_dataset.insert_local_medias(["hierarchy.png", "hierarchy.png", "hierarchy.png"])
+        assert len(urls) == 3
+
+
+class TestChunkFilters:
+    def test_chunk_filters(self, mixed_dataset: Dataset):
+        filters = mixed_dataset["_chunk_.label"].exists()
+        filtered = mixed_dataset.get_documents(100, filters=filters)
+        assert filtered["count"] == 10
+
+        filters = mixed_dataset["_chunk_.label_chunkvector_"].exists()
+        filtered = mixed_dataset.get_documents(100, filters=filters)
+        assert filtered["count"] == 10
```

### Comparing `ai_transform-0.32.3/tests/core/test_dataset/test_keyphrase.py` & `ai_transform-0.32.4/tests/core/test_dataset/test_keyphrase.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-import pytest
-
-from ai_transform.dataset.dataset import Dataset
-from ai_transform.utils.keyphrase import Keyphrase
-
-
-@pytest.mark.usefixtures("full_dataset")
-class TestKeyphraseCrud:
-    def test_crud(self, full_dataset: Dataset):
-        keyphrase_field = full_dataset["_keyphrase_.sample_1_label.default"]
-
-        keyphrase1 = Keyphrase(
-            text="cat", _id="cat", ancestors=[], parents=[], level=0, keyphrase_score=1.1, frequency=2, metadata={}
-        )
-        keyphrase2 = Keyphrase(
-            text="cat",
-            _id="dog",
-            ancestors=["cat"],
-            parents=["cat"],
-            level=1,
-            keyphrase_score=1.1,
-            frequency=1,
-            metadata={},
-        )
-        updates = [keyphrase1, keyphrase2]
-        response = keyphrase_field.bulk_update_keyphrases(updates=updates)
-
-        keyphrase = keyphrase_field.get_keyphrase(keyphrase_id="cat")
-        assert "cat" == keyphrase["text"]
+import pytest
+
+from ai_transform.dataset.dataset import Dataset
+from ai_transform.utils.keyphrase import Keyphrase
+
+
+@pytest.mark.usefixtures("full_dataset")
+class TestKeyphraseCrud:
+    def test_crud(self, full_dataset: Dataset):
+        keyphrase_field = full_dataset["_keyphrase_.sample_1_label.default"]
+
+        keyphrase1 = Keyphrase(
+            text="cat", _id="cat", ancestors=[], parents=[], level=0, keyphrase_score=1.1, frequency=2, metadata={}
+        )
+        keyphrase2 = Keyphrase(
+            text="cat",
+            _id="dog",
+            ancestors=["cat"],
+            parents=["cat"],
+            level=1,
+            keyphrase_score=1.1,
+            frequency=1,
+            metadata={},
+        )
+        updates = [keyphrase1, keyphrase2]
+        response = keyphrase_field.bulk_update_keyphrases(updates=updates)
+
+        keyphrase = keyphrase_field.get_keyphrase(keyphrase_id="cat")
+        assert "cat" == keyphrase["text"]
```

### Comparing `ai_transform-0.32.3/tests/core/test_engine/test_engine.py` & `ai_transform-0.32.4/tests/core/test_engine/test_engine.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-from typing import Any
-
-from ai_transform.api.client import Client
-from ai_transform.dataset.dataset import Dataset
-from ai_transform.operator.abstract_operator import AbstractOperator
-from ai_transform.engine.abstract_engine import AbstractEngine
-from ai_transform.engine.stable_engine import StableEngine
-
-from ai_transform.utils.example_documents import mock_documents
-
-
-class TestAbstractEngine:
-    def test_engine(self, full_dataset: Dataset, test_operator: AbstractOperator):
-        class ExampleEngine(AbstractEngine):
-            def apply(self) -> Any:
-                iterator = self.iterate()
-                for chunk in iterator:
-                    new_batch = self.operator(chunk)
-                    self.update_chunk(new_batch)
-
-                return
-
-        engine = ExampleEngine(full_dataset, test_operator)
-
-        assert isinstance(engine.operator, AbstractOperator)
-        assert len(ExampleEngine.__abstractmethods__) == 0
-
-    def test_engine_abstract(self, full_dataset: Dataset, test_operator: AbstractOperator):
-        class ExampleEngine(AbstractEngine):
-            pass
-
-        try:
-            engine = ExampleEngine(full_dataset, test_operator)
-        except:
-            assert True
-
-    def test_engine_select_fields(self, full_dataset: Dataset, test_operator: AbstractOperator):
-        class ExampleEngine(AbstractEngine):
-            def apply(self) -> Any:
-                return
-
-        engine = ExampleEngine(full_dataset, test_operator, select_fields=["_id", "_chunk_.label"])
-        assert "_chunk_" in engine._select_fields
-
-    def test_engine_select_fields(self, test_client: Client, test_dataset_id: str, test_operator: AbstractOperator):
-        engine = StableEngine(
-            test_client.Dataset(test_dataset_id), test_operator, transform_chunksize=2, documents=mock_documents(20)
-        )
-        engine()
-
-        assert len(engine.output_documents) == 20
-
-        test_client.delete_dataset(test_dataset_id)
+from typing import Any
+
+from ai_transform.api.client import Client
+from ai_transform.dataset.dataset import Dataset
+from ai_transform.operator.abstract_operator import AbstractOperator
+from ai_transform.engine.abstract_engine import AbstractEngine
+from ai_transform.engine.stable_engine import StableEngine
+
+from ai_transform.utils.example_documents import mock_documents
+
+
+class TestAbstractEngine:
+    def test_engine(self, full_dataset: Dataset, test_operator: AbstractOperator):
+        class ExampleEngine(AbstractEngine):
+            def apply(self) -> Any:
+                iterator = self.iterate()
+                for chunk in iterator:
+                    new_batch = self.operator(chunk)
+                    self.update_chunk(new_batch)
+
+                return
+
+        engine = ExampleEngine(full_dataset, test_operator)
+
+        assert isinstance(engine.operator, AbstractOperator)
+        assert len(ExampleEngine.__abstractmethods__) == 0
+
+    def test_engine_abstract(self, full_dataset: Dataset, test_operator: AbstractOperator):
+        class ExampleEngine(AbstractEngine):
+            pass
+
+        try:
+            engine = ExampleEngine(full_dataset, test_operator)
+        except:
+            assert True
+
+    def test_engine_select_fields(self, full_dataset: Dataset, test_operator: AbstractOperator):
+        class ExampleEngine(AbstractEngine):
+            def apply(self) -> Any:
+                return
+
+        engine = ExampleEngine(full_dataset, test_operator, select_fields=["_id", "_chunk_.label"])
+        assert "_chunk_" in engine._select_fields
+
+    def test_engine_select_fields(self, test_client: Client, test_dataset_id: str, test_operator: AbstractOperator):
+        engine = StableEngine(
+            test_client.Dataset(test_dataset_id), test_operator, transform_chunksize=2, documents=mock_documents(20)
+        )
+        engine()
+
+        assert len(engine.output_documents) == 20
+
+        test_client.delete_dataset(test_dataset_id)
```

### Comparing `ai_transform-0.32.3/tests/core/test_engine/test_stable_engine.py` & `ai_transform-0.32.4/tests/core/test_engine/test_stable_engine.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-import uuid
-
-from typing import Type
-
-from ai_transform.dataset.dataset import Dataset
-from ai_transform.engine.stable_engine import StableEngine
-from ai_transform.engine.small_batch_stable_engine import SmallBatchStableEngine
-
-from ai_transform.operator.abstract_operator import AbstractOperator
-from ai_transform.workflow.abstract_workflow import Workflow
-
-
-def _random_id():
-    return str(uuid.uuid4())
-
-
-class TestStableEngine:
-    def test_stable_engine(self, full_dataset: Dataset, test_operator: AbstractOperator):
-        engine = StableEngine(full_dataset, test_operator, worker_number=0)
-        workflow = Workflow(name=_random_id(), engine=engine, job_id=_random_id())
-        workflow.run()
-        assert engine.success_ratio == 1
-
-    def test_small_batch_stable_engine(self, full_dataset: Dataset, test_operator: AbstractOperator):
-        engine = SmallBatchStableEngine(full_dataset, test_operator)
-        workflow = Workflow(name=_random_id(), engine=engine, job_id=_random_id())
-        workflow.run()
-        assert engine.success_ratio == 1
-
-
-class TestStableEngineFilters:
-    _SELECTED_FIELDS = ["sample_1_label", "sample_2_label", "sample_3_label"]
-
-    def test_stable_engine_filters1(self, partial_dataset: Dataset, test_partial_operator: Type[AbstractOperator]):
-        prev_health = partial_dataset.health()
-        operator = test_partial_operator(self._SELECTED_FIELDS)
-
-        engine = StableEngine(partial_dataset, operator, select_fields=self._SELECTED_FIELDS)
-        workflow = Workflow(name=_random_id(), engine=engine, job_id=_random_id())
-        workflow.run()
-
-        post_health = partial_dataset.health()
-        for input_field, output_field in zip(operator.input_fields, operator.output_fields):
-            assert prev_health[input_field]["exists"] == post_health[output_field]["exists"]
-
-        assert engine.success_ratio == 1
-
-    def test_stable_engine_filters2(
-        self, partial_dataset_with_outputs: Dataset, test_partial_operator: Type[AbstractOperator]
-    ):
-        prev_health = partial_dataset_with_outputs.health()
-        operator = test_partial_operator(self._SELECTED_FIELDS)
-
-        engine = StableEngine(
-            partial_dataset_with_outputs, operator, select_fields=self._SELECTED_FIELDS, refresh=False
-        )
-        workflow = Workflow(name=_random_id(), engine=engine, job_id=_random_id())
-        workflow.run()
-
-        post_health = partial_dataset_with_outputs.health()
-        for input_field, output_field in zip(operator.input_fields, operator.output_fields):
-            assert prev_health[input_field]["exists"] == post_health[output_field]["exists"]
-
-        assert engine.success_ratio == 1
-
-    def test_stable_engine_filters3(
-        self, simple_partial_dataset: Dataset, test_partial_operator: Type[AbstractOperator]
-    ):
-        prev_health = simple_partial_dataset.health()
-        operator = test_partial_operator(["sample_1_label"])
-
-        engine = StableEngine(simple_partial_dataset, operator, select_fields=["sample_1_label"], refresh=False)
-        workflow = Workflow(name=_random_id(), engine=engine, job_id=_random_id())
-        workflow.run()
-
-        post_health = simple_partial_dataset.health()
-        for input_field, output_field in zip(operator.input_fields, operator.output_fields):
-            assert prev_health[input_field]["exists"] == post_health[output_field]["exists"]
-
-        assert engine.success_ratio == 1
+import uuid
+
+from typing import Type
+
+from ai_transform.dataset.dataset import Dataset
+from ai_transform.engine.stable_engine import StableEngine
+from ai_transform.engine.small_batch_stable_engine import SmallBatchStableEngine
+
+from ai_transform.operator.abstract_operator import AbstractOperator
+from ai_transform.workflow.abstract_workflow import Workflow
+
+
+def _random_id():
+    return str(uuid.uuid4())
+
+
+class TestStableEngine:
+    def test_stable_engine(self, full_dataset: Dataset, test_operator: AbstractOperator):
+        engine = StableEngine(full_dataset, test_operator, worker_number=0)
+        workflow = Workflow(name=_random_id(), engine=engine, job_id=_random_id())
+        workflow.run()
+        assert engine.success_ratio == 1
+
+    def test_small_batch_stable_engine(self, full_dataset: Dataset, test_operator: AbstractOperator):
+        engine = SmallBatchStableEngine(full_dataset, test_operator)
+        workflow = Workflow(name=_random_id(), engine=engine, job_id=_random_id())
+        workflow.run()
+        assert engine.success_ratio == 1
+
+
+class TestStableEngineFilters:
+    _SELECTED_FIELDS = ["sample_1_label", "sample_2_label", "sample_3_label"]
+
+    def test_stable_engine_filters1(self, partial_dataset: Dataset, test_partial_operator: Type[AbstractOperator]):
+        prev_health = partial_dataset.health()
+        operator = test_partial_operator(self._SELECTED_FIELDS)
+
+        engine = StableEngine(partial_dataset, operator, select_fields=self._SELECTED_FIELDS)
+        workflow = Workflow(name=_random_id(), engine=engine, job_id=_random_id())
+        workflow.run()
+
+        post_health = partial_dataset.health()
+        for input_field, output_field in zip(operator.input_fields, operator.output_fields):
+            assert prev_health[input_field]["exists"] == post_health[output_field]["exists"]
+
+        assert engine.success_ratio == 1
+
+    def test_stable_engine_filters2(
+        self, partial_dataset_with_outputs: Dataset, test_partial_operator: Type[AbstractOperator]
+    ):
+        prev_health = partial_dataset_with_outputs.health()
+        operator = test_partial_operator(self._SELECTED_FIELDS)
+
+        engine = StableEngine(
+            partial_dataset_with_outputs, operator, select_fields=self._SELECTED_FIELDS, refresh=False
+        )
+        workflow = Workflow(name=_random_id(), engine=engine, job_id=_random_id())
+        workflow.run()
+
+        post_health = partial_dataset_with_outputs.health()
+        for input_field, output_field in zip(operator.input_fields, operator.output_fields):
+            assert prev_health[input_field]["exists"] == post_health[output_field]["exists"]
+
+        assert engine.success_ratio == 1
+
+    def test_stable_engine_filters3(
+        self, simple_partial_dataset: Dataset, test_partial_operator: Type[AbstractOperator]
+    ):
+        prev_health = simple_partial_dataset.health()
+        operator = test_partial_operator(["sample_1_label"])
+
+        engine = StableEngine(simple_partial_dataset, operator, select_fields=["sample_1_label"], refresh=False)
+        workflow = Workflow(name=_random_id(), engine=engine, job_id=_random_id())
+        workflow.run()
+
+        post_health = simple_partial_dataset.health()
+        for input_field, output_field in zip(operator.input_fields, operator.output_fields):
+            assert prev_health[input_field]["exists"] == post_health[output_field]["exists"]
+
+        assert engine.success_ratio == 1
```

### Comparing `ai_transform-0.32.3/tests/core/test_operator/test_document_diff.py` & `ai_transform-0.32.4/tests/core/test_operator/test_document_diff.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-import json
-import random
-
-from copy import deepcopy
-from ai_transform.operator.abstract_operator import AbstractOperator
-from ai_transform.utils.document import Document
-from ai_transform.utils.example_documents import mock_documents, generate_random_label, generate_random_vector
-
-
-class TestDocumentDiff:
-    def test_diff1(self):
-        old_documents = mock_documents(3)
-        new_documents = deepcopy(old_documents)
-
-        expected_diff = []
-
-        for document in new_documents:
-            new_chunk = {"label": generate_random_label(), "label_chunkvector_": generate_random_vector()}
-            document["_chunk_"].append(new_chunk)
-            expected_diff.append({"_id": document["_id"], "_chunk_": document["_chunk_"]})
-
-        diff = AbstractOperator._postprocess(new_documents, old_documents).to_json()
-        diff = list(sorted(diff, key=lambda x: x["_id"]))
-        expected_diff = list(sorted(expected_diff, key=lambda x: x["_id"]))
-
-        assert json.dumps(diff, sort_keys=True) == json.dumps(expected_diff, sort_keys=True)
-
-    def test_update_diff(self):
-        old_documents = [Document({"label": "yes"}) for _ in range(5)]
-        new_documents = deepcopy(old_documents)
-        for document in new_documents:
-            document["label"] = "no"
-
-        diff = AbstractOperator._postprocess(new_documents, old_documents)
-        expected_diff = json.dumps({"label": "no"})
-
-        assert all(json.dumps(document.to_json()) == expected_diff for document in diff)
-
-    def test_no_diff(self):
-        documents = [Document({"value": 10})]
-        diff = AbstractOperator._postprocess(documents, documents)
-        assert not diff
-
-    def test_chunk_diff(self):
-        old_documents = [Document({"example_vector_": [random.random() for _ in range(5)]}) for _ in range(5)]
-        new_documents = deepcopy(old_documents)
-        for document in new_documents:
-            document["label"] = "yes"
-
-        diff = AbstractOperator._postprocess(new_documents, old_documents)
-        expected_diff = json.dumps({"label": "yes"})
-
-        assert all(json.dumps(document.to_json()) == expected_diff for document in diff)
+import json
+import random
+
+from copy import deepcopy
+from ai_transform.operator.abstract_operator import AbstractOperator
+from ai_transform.utils.document import Document
+from ai_transform.utils.example_documents import mock_documents, generate_random_label, generate_random_vector
+
+
+class TestDocumentDiff:
+    def test_diff1(self):
+        old_documents = mock_documents(3)
+        new_documents = deepcopy(old_documents)
+
+        expected_diff = []
+
+        for document in new_documents:
+            new_chunk = {"label": generate_random_label(), "label_chunkvector_": generate_random_vector()}
+            document["_chunk_"].append(new_chunk)
+            expected_diff.append({"_id": document["_id"], "_chunk_": document["_chunk_"]})
+
+        diff = AbstractOperator._postprocess(new_documents, old_documents).to_json()
+        diff = list(sorted(diff, key=lambda x: x["_id"]))
+        expected_diff = list(sorted(expected_diff, key=lambda x: x["_id"]))
+
+        assert json.dumps(diff, sort_keys=True) == json.dumps(expected_diff, sort_keys=True)
+
+    def test_update_diff(self):
+        old_documents = [Document({"label": "yes"}) for _ in range(5)]
+        new_documents = deepcopy(old_documents)
+        for document in new_documents:
+            document["label"] = "no"
+
+        diff = AbstractOperator._postprocess(new_documents, old_documents)
+        expected_diff = json.dumps({"label": "no"})
+
+        assert all(json.dumps(document.to_json()) == expected_diff for document in diff)
+
+    def test_no_diff(self):
+        documents = [Document({"value": 10})]
+        diff = AbstractOperator._postprocess(documents, documents)
+        assert not diff
+
+    def test_chunk_diff(self):
+        old_documents = [Document({"example_vector_": [random.random() for _ in range(5)]}) for _ in range(5)]
+        new_documents = deepcopy(old_documents)
+        for document in new_documents:
+            document["label"] = "yes"
+
+        diff = AbstractOperator._postprocess(new_documents, old_documents)
+        expected_diff = json.dumps({"label": "yes"})
+
+        assert all(json.dumps(document.to_json()) == expected_diff for document in diff)
```

### Comparing `ai_transform-0.32.3/tests/core/test_workflow/test_context_manager.py` & `ai_transform-0.32.4/tests/core/test_workflow/test_context_manager.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from ai_transform.dataset.dataset import Dataset
-
-
-class TestContextManager:
-    def test_field_children(self, full_dataset: Dataset):
-        parent_field = full_dataset["sample_1_vector_"]
-
-        parent_field.add_field_children(["_cluster_.sample_1_vector_.kmeans-1"])
-        parent_field.add_field_children(["_cluster_.sample_1_vector_.kmeans-2"])
-        parent_field.add_field_children(["_cluster_.sample_1_vector_.kmeans-3"])
-
-        child_field = full_dataset["_cluster_.sample_1_vector_.kmeans-3"]
-        child_field.add_field_children(["woah"], recursive=True)
-
-        grandchild_field = full_dataset["woah"]
-        grandchild_field.add_field_children(["woah's daughter"], recursive=True)
-
-        field_children = parent_field.list_field_children()
-
-        assert all(
-            [
-                field_child in field_children
-                for field_child in [
-                    "woah",
-                    "woah's daughter",
-                    "_cluster_.sample_1_vector_.kmeans-1",
-                    "_cluster_.sample_1_vector_.kmeans-2",
-                    "_cluster_.sample_1_vector_.kmeans-3",
-                ]
-            ]
-        )
+from ai_transform.dataset.dataset import Dataset
+
+
+class TestContextManager:
+    def test_field_children(self, full_dataset: Dataset):
+        parent_field = full_dataset["sample_1_vector_"]
+
+        parent_field.add_field_children(["_cluster_.sample_1_vector_.kmeans-1"])
+        parent_field.add_field_children(["_cluster_.sample_1_vector_.kmeans-2"])
+        parent_field.add_field_children(["_cluster_.sample_1_vector_.kmeans-3"])
+
+        child_field = full_dataset["_cluster_.sample_1_vector_.kmeans-3"]
+        child_field.add_field_children(["woah"], recursive=True)
+
+        grandchild_field = full_dataset["woah"]
+        grandchild_field.add_field_children(["woah's daughter"], recursive=True)
+
+        field_children = parent_field.list_field_children()
+
+        assert all(
+            [
+                field_child in field_children
+                for field_child in [
+                    "woah",
+                    "woah's daughter",
+                    "_cluster_.sample_1_vector_.kmeans-1",
+                    "_cluster_.sample_1_vector_.kmeans-2",
+                    "_cluster_.sample_1_vector_.kmeans-3",
+                ]
+            ]
+        )
```

### Comparing `ai_transform-0.32.3/tests/core/test_workflow/test_workflow.py` & `ai_transform-0.32.4/tests/core/test_workflow/test_workflow.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,79 +1,79 @@
-import time
-
-from pydantic import Field
-
-from ai_transform.api.client import Client
-from ai_transform.engine.abstract_engine import AbstractEngine
-from ai_transform.workflow.abstract_workflow import Workflow
-from ai_transform.config import BaseConfig
-
-
-class SimpleWorkflowConfig(BaseConfig):
-    input_field: str = Field("test_input_field", description="The field you want to are using to transform on")
-    output_field: str = Field("test_output_field", description="The output field")
-    minimum_coverage: float = Field(
-        0.95, description="The minimum amount of coverage of the output field relative to the input field."
-    )
-    max_time: float = Field(6000, description="THe maximum amount of time to allow for this to poll.")
-    sleep_timer: float = Field(10, description="How long to wait before each poll")
-    parent_job_id: str = Field(
-        None,
-        description="If supplied - it will update the status of the workflow as complete only once the workflow has complete.",
-    )
-    parent_job_name: str = Field(
-        None,
-        description="If supplied - it will update the status of the workflow as complete only once the workflow has complete.",
-    )
-
-
-class TestWorkflow:
-    def test_workflow(self, test_paid_engine: AbstractEngine):
-        workflow_name = "test_workflow"
-        workflow = Workflow(name=workflow_name, engine=test_paid_engine, job_id="test_job1")
-        res = workflow.run()
-        assert res is None
-
-        status = workflow.get_status()
-        assert status["steps"][workflow_name]["n_processed_pricing"] == 20
-
-    def test_workflow_no_refresh(self, test_paid_engine_no_refresh: AbstractEngine):
-        workflow_name = "test_workflow"
-        workflow = Workflow(name=workflow_name, engine=test_paid_engine_no_refresh, job_id="test_job2")
-        res = workflow.run()
-        assert res is None
-
-        status = workflow.get_status()
-        assert status["steps"][workflow_name]["n_processed_pricing"] == 20
-
-
-class TestSimpleWorkflow:
-    def test_simple_workflow_simple_case(self, test_client: Client, test_simple_workflow_token: str):
-        config = SimpleWorkflowConfig.read_token(test_simple_workflow_token)
-
-        x = 0
-        with test_client.SimpleWorkflow(
-            workflow_name="Simple Workflow",
-            job_id=config.job_id,
-            additional_information=config.additional_information,
-            send_email=config.send_email,
-        ):
-            x += 1
-        assert x == 1
-
-    def test_simple_workflow(self, test_client: Client):
-        simple_workflow_dataset = test_client.Dataset("test-simple-workflow-dataset", expire=True)
-        simple_workflow_dataset.insert_documents([{"_id": "0", "value": 0}])
-
-        workflow_name = "Simple Workflow"
-        time_sleep_value = 10
-
-        with test_client.SimpleWorkflow(workflow_name=workflow_name, job_id="test-simple-workflow") as workflow:
-            time.sleep(time_sleep_value)
-            simple_workflow_dataset.update_documents([{"_id": "0", "value": 1}], ingest_in_background=False)
-
-        status = workflow.get_status()
-        assert status["status"] == "complete"
-        assert status["steps"][workflow_name]["n_processed_pricing"] >= time_sleep_value
-
-        documents = simple_workflow_dataset.get_all_documents()["documents"]
-        assert documents[0]["value"] == 1
+import time
+
+from pydantic import Field
+
+from ai_transform.api.client import Client
+from ai_transform.engine.abstract_engine import AbstractEngine
+from ai_transform.workflow.abstract_workflow import Workflow
+from ai_transform.config import BaseConfig
+
+
+class SimpleWorkflowConfig(BaseConfig):
+    input_field: str = Field("test_input_field", description="The field you want to are using to transform on")
+    output_field: str = Field("test_output_field", description="The output field")
+    minimum_coverage: float = Field(
+        0.95, description="The minimum amount of coverage of the output field relative to the input field."
+    )
+    max_time: float = Field(6000, description="THe maximum amount of time to allow for this to poll.")
+    sleep_timer: float = Field(10, description="How long to wait before each poll")
+    parent_job_id: str = Field(
+        None,
+        description="If supplied - it will update the status of the workflow as complete only once the workflow has complete.",
+    )
+    parent_job_name: str = Field(
+        None,
+        description="If supplied - it will update the status of the workflow as complete only once the workflow has complete.",
+    )
+
+
+class TestWorkflow:
+    def test_workflow(self, test_paid_engine: AbstractEngine):
+        workflow_name = "test_workflow"
+        workflow = Workflow(name=workflow_name, engine=test_paid_engine, job_id="test_job1")
+        res = workflow.run()
+        assert res is None
+
+        status = workflow.get_status()
+        assert status["steps"][workflow_name]["n_processed_pricing"] == 20
+
+    def test_workflow_no_refresh(self, test_paid_engine_no_refresh: AbstractEngine):
+        workflow_name = "test_workflow"
+        workflow = Workflow(name=workflow_name, engine=test_paid_engine_no_refresh, job_id="test_job2")
+        res = workflow.run()
+        assert res is None
+
+        status = workflow.get_status()
+        assert status["steps"][workflow_name]["n_processed_pricing"] == 20
+
+
+class TestSimpleWorkflow:
+    def test_simple_workflow_simple_case(self, test_client: Client, test_simple_workflow_token: str):
+        config = SimpleWorkflowConfig.read_token(test_simple_workflow_token)
+
+        x = 0
+        with test_client.SimpleWorkflow(
+            workflow_name="Simple Workflow",
+            job_id=config.job_id,
+            additional_information=config.additional_information,
+            send_email=config.send_email,
+        ):
+            x += 1
+        assert x == 1
+
+    def test_simple_workflow(self, test_client: Client):
+        simple_workflow_dataset = test_client.Dataset("test-simple-workflow-dataset", expire=True)
+        simple_workflow_dataset.insert_documents([{"_id": "0", "value": 0}])
+
+        workflow_name = "Simple Workflow"
+        time_sleep_value = 10
+
+        with test_client.SimpleWorkflow(workflow_name=workflow_name, job_id="test-simple-workflow") as workflow:
+            time.sleep(time_sleep_value)
+            simple_workflow_dataset.update_documents([{"_id": "0", "value": 1}], ingest_in_background=False)
+
+        status = workflow.get_status()
+        assert status["status"] == "complete"
+        assert status["steps"][workflow_name]["n_processed_pricing"] >= time_sleep_value
+
+        documents = simple_workflow_dataset.get_all_documents()["documents"]
+        assert documents[0]["value"] == 1
```

