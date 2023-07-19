# Comparing `tmp/dopt_blocks_python_client-0.0.0.tar.gz` & `tmp/dopt_blocks_python_client-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dopt_blocks_python_client-0.0.0.tar", max compression
+gzip compressed data, was "dopt_blocks_python_client-1.0.0.tar", max compression
```

## Comparing `dopt_blocks_python_client-0.0.0.tar` & `dopt_blocks_python_client-1.0.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0        0 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/README.md
--rw-r--r--   0        0        0      384 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     2498 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/__init__.py
--rw-r--r--   0        0        0      989 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/client.py
--rw-r--r--   0        0        0      348 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/core/__init__.py
--rw-r--r--   0        0        0      426 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      156 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/environment.py
--rw-r--r--   0        0        0      352 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/errors/__init__.py
--rw-r--r--   0        0        0      248 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/errors/bad_request_error.py
--rw-r--r--   0        0        0      252 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/errors/internal_server_error.py
--rw-r--r--   0        0        0      246 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/errors/not_found_error.py
--rw-r--r--   0        0        0      250 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/errors/unauthorized_error.py
--rw-r--r--   0        0        0        0 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/py.typed
--rw-r--r--   0        0        0      124 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/resources/blocks/__init__.py
--rw-r--r--   0        0        0     7421 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/resources/blocks/client.py
--rw-r--r--   0        0        0       65 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/resources/flows/__init__.py
--rw-r--r--   0        0        0     7823 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/resources/flows/client.py
--rw-r--r--   0        0        0     3392 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/types/__init__.py
--rw-r--r--   0        0        0      888 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/types/bad_request_error_response_body.py
--rw-r--r--   0        0        0      676 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/types/bad_request_error_response_body_code.py
--rw-r--r--   0        0        0      996 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/types/block_transition_query_string.py
--rw-r--r--   0        0        0      745 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/types/block_transition_request_body.py
--rw-r--r--   0        0        0      761 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/types/block_transition_request_params.py
--rw-r--r--   0        0        0      957 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/types/flow_intent_query_string.py
--rw-r--r--   0        0        0      740 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/types/flow_intent_request_body.py
--rw-r--r--   0        0        0      875 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/types/flow_intent_request_params.py
--rw-r--r--   0        0        0      830 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/types/flow_intent_request_params_intent.py
--rw-r--r--   0        0        0      870 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/types/get_block_query_string.py
--rw-r--r--   0        0        0      754 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/types/get_block_request_params.py
--rw-r--r--   0        0        0     1322 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/types/get_block_response.py
--rw-r--r--   0        0        0      495 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/types/get_block_response_fields_item.py
--rw-r--r--   0        0        0      928 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/types/get_block_response_fields_item_get_block_response_fields_item.py
--rw-r--r--   0        0        0      793 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/types/get_block_response_state.py
--rw-r--r--   0        0        0     1148 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/types/get_block_response_type.py
--rw-r--r--   0        0        0     1044 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/types/get_flow_query_string.py
--rw-r--r--   0        0        0      753 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/types/get_flow_request_params.py
--rw-r--r--   0        0        0     1120 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/types/get_flow_response.py
--rw-r--r--   0        0        0     1418 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/types/get_flow_response_blocks_item.py
--rw-r--r--   0        0        0      616 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/types/get_flow_response_blocks_item_fields_item.py
--rw-r--r--   0        0        0      946 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/types/get_flow_response_blocks_item_fields_item_get_flow_response_blocks_item_fields_item.py
--rw-r--r--   0        0        0      802 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/types/get_flow_response_blocks_item_state.py
--rw-r--r--   0        0        0     1211 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/types/get_flow_response_blocks_item_type.py
--rw-r--r--   0        0        0      795 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/types/get_flow_response_state.py
--rw-r--r--   0        0        0      780 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/types/health_check_response_body.py
--rw-r--r--   0        0        0      780 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/types/intent_request_intent.py
--rw-r--r--   0        0        0      854 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/types/internal_server_error_response_body.py
--rw-r--r--   0        0        0      842 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/types/not_found_error_response_body.py
--rw-r--r--   0        0        0      847 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/types/timeout_error_response_body.py
--rw-r--r--   0        0        0      849 2023-07-18 21:55:46.729035 dopt_blocks_python_client-0.0.0/src/dopt/types/unauthorized_error_response_body.py
--rw-r--r--   0        0        0      522 1970-01-01 00:00:00.000000 dopt_blocks_python_client-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1956 2023-07-19 00:14:14.936643 dopt_blocks_python_client-1.0.0/README.md
+-rw-r--r--   0        0        0      384 2023-07-19 00:14:14.936643 dopt_blocks_python_client-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2498 2023-07-19 00:14:14.936643 dopt_blocks_python_client-1.0.0/src/dopt/__init__.py
+-rw-r--r--   0        0        0      989 2023-07-19 00:14:14.936643 dopt_blocks_python_client-1.0.0/src/dopt/client.py
+-rw-r--r--   0        0        0      348 2023-07-19 00:14:14.936643 dopt_blocks_python_client-1.0.0/src/dopt/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-07-19 00:14:14.936643 dopt_blocks_python_client-1.0.0/src/dopt/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-07-19 00:14:14.936643 dopt_blocks_python_client-1.0.0/src/dopt/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-07-19 00:14:14.936643 dopt_blocks_python_client-1.0.0/src/dopt/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-07-19 00:14:14.936643 dopt_blocks_python_client-1.0.0/src/dopt/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      156 2023-07-19 00:14:14.936643 dopt_blocks_python_client-1.0.0/src/dopt/environment.py
+-rw-r--r--   0        0        0      352 2023-07-19 00:14:14.936643 dopt_blocks_python_client-1.0.0/src/dopt/errors/__init__.py
+-rw-r--r--   0        0        0      248 2023-07-19 00:14:14.936643 dopt_blocks_python_client-1.0.0/src/dopt/errors/bad_request_error.py
+-rw-r--r--   0        0        0      252 2023-07-19 00:14:14.936643 dopt_blocks_python_client-1.0.0/src/dopt/errors/internal_server_error.py
+-rw-r--r--   0        0        0      246 2023-07-19 00:14:14.936643 dopt_blocks_python_client-1.0.0/src/dopt/errors/not_found_error.py
+-rw-r--r--   0        0        0      250 2023-07-19 00:14:14.936643 dopt_blocks_python_client-1.0.0/src/dopt/errors/unauthorized_error.py
+-rw-r--r--   0        0        0        0 2023-07-19 00:14:14.936643 dopt_blocks_python_client-1.0.0/src/dopt/py.typed
+-rw-r--r--   0        0        0      124 2023-07-19 00:14:14.936643 dopt_blocks_python_client-1.0.0/src/dopt/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-07-19 00:14:14.936643 dopt_blocks_python_client-1.0.0/src/dopt/resources/blocks/__init__.py
+-rw-r--r--   0        0        0     7421 2023-07-19 00:14:14.936643 dopt_blocks_python_client-1.0.0/src/dopt/resources/blocks/client.py
+-rw-r--r--   0        0        0       65 2023-07-19 00:14:14.936643 dopt_blocks_python_client-1.0.0/src/dopt/resources/flows/__init__.py
+-rw-r--r--   0        0        0     7823 2023-07-19 00:14:14.936643 dopt_blocks_python_client-1.0.0/src/dopt/resources/flows/client.py
+-rw-r--r--   0        0        0     3392 2023-07-19 00:14:14.936643 dopt_blocks_python_client-1.0.0/src/dopt/types/__init__.py
+-rw-r--r--   0        0        0      888 2023-07-19 00:14:14.936643 dopt_blocks_python_client-1.0.0/src/dopt/types/bad_request_error_response_body.py
+-rw-r--r--   0        0        0      676 2023-07-19 00:14:14.936643 dopt_blocks_python_client-1.0.0/src/dopt/types/bad_request_error_response_body_code.py
+-rw-r--r--   0        0        0      996 2023-07-19 00:14:14.936643 dopt_blocks_python_client-1.0.0/src/dopt/types/block_transition_query_string.py
+-rw-r--r--   0        0        0      745 2023-07-19 00:14:14.936643 dopt_blocks_python_client-1.0.0/src/dopt/types/block_transition_request_body.py
+-rw-r--r--   0        0        0      761 2023-07-19 00:14:14.936643 dopt_blocks_python_client-1.0.0/src/dopt/types/block_transition_request_params.py
+-rw-r--r--   0        0        0      957 2023-07-19 00:14:14.936643 dopt_blocks_python_client-1.0.0/src/dopt/types/flow_intent_query_string.py
+-rw-r--r--   0        0        0      740 2023-07-19 00:14:14.936643 dopt_blocks_python_client-1.0.0/src/dopt/types/flow_intent_request_body.py
+-rw-r--r--   0        0        0      875 2023-07-19 00:14:14.936643 dopt_blocks_python_client-1.0.0/src/dopt/types/flow_intent_request_params.py
+-rw-r--r--   0        0        0      830 2023-07-19 00:14:14.936643 dopt_blocks_python_client-1.0.0/src/dopt/types/flow_intent_request_params_intent.py
+-rw-r--r--   0        0        0      870 2023-07-19 00:14:14.936643 dopt_blocks_python_client-1.0.0/src/dopt/types/get_block_query_string.py
+-rw-r--r--   0        0        0      754 2023-07-19 00:14:14.936643 dopt_blocks_python_client-1.0.0/src/dopt/types/get_block_request_params.py
+-rw-r--r--   0        0        0     1322 2023-07-19 00:14:14.936643 dopt_blocks_python_client-1.0.0/src/dopt/types/get_block_response.py
+-rw-r--r--   0        0        0      495 2023-07-19 00:14:14.936643 dopt_blocks_python_client-1.0.0/src/dopt/types/get_block_response_fields_item.py
+-rw-r--r--   0        0        0      928 2023-07-19 00:14:14.936643 dopt_blocks_python_client-1.0.0/src/dopt/types/get_block_response_fields_item_get_block_response_fields_item.py
+-rw-r--r--   0        0        0      793 2023-07-19 00:14:14.940642 dopt_blocks_python_client-1.0.0/src/dopt/types/get_block_response_state.py
+-rw-r--r--   0        0        0     1148 2023-07-19 00:14:14.940642 dopt_blocks_python_client-1.0.0/src/dopt/types/get_block_response_type.py
+-rw-r--r--   0        0        0     1044 2023-07-19 00:14:14.940642 dopt_blocks_python_client-1.0.0/src/dopt/types/get_flow_query_string.py
+-rw-r--r--   0        0        0      753 2023-07-19 00:14:14.940642 dopt_blocks_python_client-1.0.0/src/dopt/types/get_flow_request_params.py
+-rw-r--r--   0        0        0     1120 2023-07-19 00:14:14.940642 dopt_blocks_python_client-1.0.0/src/dopt/types/get_flow_response.py
+-rw-r--r--   0        0        0     1418 2023-07-19 00:14:14.940642 dopt_blocks_python_client-1.0.0/src/dopt/types/get_flow_response_blocks_item.py
+-rw-r--r--   0        0        0      616 2023-07-19 00:14:14.940642 dopt_blocks_python_client-1.0.0/src/dopt/types/get_flow_response_blocks_item_fields_item.py
+-rw-r--r--   0        0        0      946 2023-07-19 00:14:14.940642 dopt_blocks_python_client-1.0.0/src/dopt/types/get_flow_response_blocks_item_fields_item_get_flow_response_blocks_item_fields_item.py
+-rw-r--r--   0        0        0      802 2023-07-19 00:14:14.940642 dopt_blocks_python_client-1.0.0/src/dopt/types/get_flow_response_blocks_item_state.py
+-rw-r--r--   0        0        0     1211 2023-07-19 00:14:14.940642 dopt_blocks_python_client-1.0.0/src/dopt/types/get_flow_response_blocks_item_type.py
+-rw-r--r--   0        0        0      795 2023-07-19 00:14:14.940642 dopt_blocks_python_client-1.0.0/src/dopt/types/get_flow_response_state.py
+-rw-r--r--   0        0        0      780 2023-07-19 00:14:14.940642 dopt_blocks_python_client-1.0.0/src/dopt/types/health_check_response_body.py
+-rw-r--r--   0        0        0      780 2023-07-19 00:14:14.940642 dopt_blocks_python_client-1.0.0/src/dopt/types/intent_request_intent.py
+-rw-r--r--   0        0        0      854 2023-07-19 00:14:14.940642 dopt_blocks_python_client-1.0.0/src/dopt/types/internal_server_error_response_body.py
+-rw-r--r--   0        0        0      842 2023-07-19 00:14:14.940642 dopt_blocks_python_client-1.0.0/src/dopt/types/not_found_error_response_body.py
+-rw-r--r--   0        0        0      847 2023-07-19 00:14:14.940642 dopt_blocks_python_client-1.0.0/src/dopt/types/timeout_error_response_body.py
+-rw-r--r--   0        0        0      849 2023-07-19 00:14:14.940642 dopt_blocks_python_client-1.0.0/src/dopt/types/unauthorized_error_response_body.py
+-rw-r--r--   0        0        0     2478 1970-01-01 00:00:00.000000 dopt_blocks_python_client-1.0.0/PKG-INFO
```

### Comparing `dopt_blocks_python_client-0.0.0/src/dopt/__init__.py` & `dopt_blocks_python_client-1.0.0/src/dopt/__init__.py`

 * *Files identical despite different names*

### Comparing `dopt_blocks_python_client-0.0.0/src/dopt/client.py` & `dopt_blocks_python_client-1.0.0/src/dopt/client.py`

 * *Files identical despite different names*

### Comparing `dopt_blocks_python_client-0.0.0/src/dopt/core/datetime_utils.py` & `dopt_blocks_python_client-1.0.0/src/dopt/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `dopt_blocks_python_client-0.0.0/src/dopt/core/jsonable_encoder.py` & `dopt_blocks_python_client-1.0.0/src/dopt/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `dopt_blocks_python_client-0.0.0/src/dopt/resources/blocks/client.py` & `dopt_blocks_python_client-1.0.0/src/dopt/resources/blocks/client.py`

 * *Files identical despite different names*

### Comparing `dopt_blocks_python_client-0.0.0/src/dopt/resources/flows/client.py` & `dopt_blocks_python_client-1.0.0/src/dopt/resources/flows/client.py`

 * *Files identical despite different names*

### Comparing `dopt_blocks_python_client-0.0.0/src/dopt/types/__init__.py` & `dopt_blocks_python_client-1.0.0/src/dopt/types/__init__.py`

 * *Files identical despite different names*

### Comparing `dopt_blocks_python_client-0.0.0/src/dopt/types/bad_request_error_response_body.py` & `dopt_blocks_python_client-1.0.0/src/dopt/types/bad_request_error_response_body.py`

 * *Files identical despite different names*

### Comparing `dopt_blocks_python_client-0.0.0/src/dopt/types/bad_request_error_response_body_code.py` & `dopt_blocks_python_client-1.0.0/src/dopt/types/bad_request_error_response_body_code.py`

 * *Files identical despite different names*

### Comparing `dopt_blocks_python_client-0.0.0/src/dopt/types/block_transition_query_string.py` & `dopt_blocks_python_client-1.0.0/src/dopt/types/block_transition_query_string.py`

 * *Files identical despite different names*

### Comparing `dopt_blocks_python_client-0.0.0/src/dopt/types/block_transition_request_body.py` & `dopt_blocks_python_client-1.0.0/src/dopt/types/block_transition_request_body.py`

 * *Files identical despite different names*

### Comparing `dopt_blocks_python_client-0.0.0/src/dopt/types/block_transition_request_params.py` & `dopt_blocks_python_client-1.0.0/src/dopt/types/block_transition_request_params.py`

 * *Files identical despite different names*

### Comparing `dopt_blocks_python_client-0.0.0/src/dopt/types/flow_intent_query_string.py` & `dopt_blocks_python_client-1.0.0/src/dopt/types/flow_intent_query_string.py`

 * *Files identical despite different names*

### Comparing `dopt_blocks_python_client-0.0.0/src/dopt/types/flow_intent_request_body.py` & `dopt_blocks_python_client-1.0.0/src/dopt/types/flow_intent_request_body.py`

 * *Files identical despite different names*

### Comparing `dopt_blocks_python_client-0.0.0/src/dopt/types/flow_intent_request_params.py` & `dopt_blocks_python_client-1.0.0/src/dopt/types/flow_intent_request_params.py`

 * *Files identical despite different names*

### Comparing `dopt_blocks_python_client-0.0.0/src/dopt/types/flow_intent_request_params_intent.py` & `dopt_blocks_python_client-1.0.0/src/dopt/types/flow_intent_request_params_intent.py`

 * *Files identical despite different names*

### Comparing `dopt_blocks_python_client-0.0.0/src/dopt/types/get_block_query_string.py` & `dopt_blocks_python_client-1.0.0/src/dopt/types/get_block_query_string.py`

 * *Files identical despite different names*

### Comparing `dopt_blocks_python_client-0.0.0/src/dopt/types/get_block_request_params.py` & `dopt_blocks_python_client-1.0.0/src/dopt/types/get_block_request_params.py`

 * *Files identical despite different names*

### Comparing `dopt_blocks_python_client-0.0.0/src/dopt/types/get_block_response.py` & `dopt_blocks_python_client-1.0.0/src/dopt/types/get_block_response.py`

 * *Files identical despite different names*

### Comparing `dopt_blocks_python_client-0.0.0/src/dopt/types/get_block_response_fields_item_get_block_response_fields_item.py` & `dopt_blocks_python_client-1.0.0/src/dopt/types/get_block_response_fields_item_get_block_response_fields_item.py`

 * *Files identical despite different names*

### Comparing `dopt_blocks_python_client-0.0.0/src/dopt/types/get_block_response_state.py` & `dopt_blocks_python_client-1.0.0/src/dopt/types/get_block_response_state.py`

 * *Files identical despite different names*

### Comparing `dopt_blocks_python_client-0.0.0/src/dopt/types/get_block_response_type.py` & `dopt_blocks_python_client-1.0.0/src/dopt/types/get_block_response_type.py`

 * *Files identical despite different names*

### Comparing `dopt_blocks_python_client-0.0.0/src/dopt/types/get_flow_query_string.py` & `dopt_blocks_python_client-1.0.0/src/dopt/types/get_flow_query_string.py`

 * *Files identical despite different names*

### Comparing `dopt_blocks_python_client-0.0.0/src/dopt/types/get_flow_request_params.py` & `dopt_blocks_python_client-1.0.0/src/dopt/types/get_flow_request_params.py`

 * *Files identical despite different names*

### Comparing `dopt_blocks_python_client-0.0.0/src/dopt/types/get_flow_response.py` & `dopt_blocks_python_client-1.0.0/src/dopt/types/get_flow_response.py`

 * *Files identical despite different names*

### Comparing `dopt_blocks_python_client-0.0.0/src/dopt/types/get_flow_response_blocks_item.py` & `dopt_blocks_python_client-1.0.0/src/dopt/types/get_flow_response_blocks_item.py`

 * *Files identical despite different names*

### Comparing `dopt_blocks_python_client-0.0.0/src/dopt/types/get_flow_response_blocks_item_fields_item.py` & `dopt_blocks_python_client-1.0.0/src/dopt/types/get_flow_response_blocks_item_fields_item.py`

 * *Files identical despite different names*

### Comparing `dopt_blocks_python_client-0.0.0/src/dopt/types/get_flow_response_blocks_item_fields_item_get_flow_response_blocks_item_fields_item.py` & `dopt_blocks_python_client-1.0.0/src/dopt/types/get_flow_response_blocks_item_fields_item_get_flow_response_blocks_item_fields_item.py`

 * *Files identical despite different names*

### Comparing `dopt_blocks_python_client-0.0.0/src/dopt/types/get_flow_response_blocks_item_state.py` & `dopt_blocks_python_client-1.0.0/src/dopt/types/get_flow_response_blocks_item_state.py`

 * *Files identical despite different names*

### Comparing `dopt_blocks_python_client-0.0.0/src/dopt/types/get_flow_response_blocks_item_type.py` & `dopt_blocks_python_client-1.0.0/src/dopt/types/get_flow_response_blocks_item_type.py`

 * *Files identical despite different names*

### Comparing `dopt_blocks_python_client-0.0.0/src/dopt/types/get_flow_response_state.py` & `dopt_blocks_python_client-1.0.0/src/dopt/types/get_flow_response_state.py`

 * *Files identical despite different names*

### Comparing `dopt_blocks_python_client-0.0.0/src/dopt/types/health_check_response_body.py` & `dopt_blocks_python_client-1.0.0/src/dopt/types/health_check_response_body.py`

 * *Files identical despite different names*

### Comparing `dopt_blocks_python_client-0.0.0/src/dopt/types/intent_request_intent.py` & `dopt_blocks_python_client-1.0.0/src/dopt/types/intent_request_intent.py`

 * *Files identical despite different names*

### Comparing `dopt_blocks_python_client-0.0.0/src/dopt/types/internal_server_error_response_body.py` & `dopt_blocks_python_client-1.0.0/src/dopt/types/internal_server_error_response_body.py`

 * *Files identical despite different names*

### Comparing `dopt_blocks_python_client-0.0.0/src/dopt/types/not_found_error_response_body.py` & `dopt_blocks_python_client-1.0.0/src/dopt/types/not_found_error_response_body.py`

 * *Files identical despite different names*

### Comparing `dopt_blocks_python_client-0.0.0/src/dopt/types/timeout_error_response_body.py` & `dopt_blocks_python_client-1.0.0/src/dopt/types/timeout_error_response_body.py`

 * *Files identical despite different names*

### Comparing `dopt_blocks_python_client-0.0.0/src/dopt/types/unauthorized_error_response_body.py` & `dopt_blocks_python_client-1.0.0/src/dopt/types/unauthorized_error_response_body.py`

 * *Files identical despite different names*

