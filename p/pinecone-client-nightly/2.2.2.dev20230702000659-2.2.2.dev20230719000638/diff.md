# Comparing `tmp/pinecone-client-nightly-2.2.2.dev20230702000659.tar.gz` & `tmp/pinecone-client-nightly-2.2.2.dev20230719000638.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinecone-client-nightly-2.2.2.dev20230702000659.tar", last modified: Sun Jul  2 00:07:13 2023, max compression
+gzip compressed data, was "pinecone-client-nightly-2.2.2.dev20230719000638.tar", last modified: Wed Jul 19 00:06:40 2023, max compression
```

## Comparing `pinecone-client-nightly-2.2.2.dev20230702000659.tar` & `pinecone-client-nightly-2.2.2.dev20230719000638.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 00:07:13.491162 pinecone-client-nightly-2.2.2.dev20230702000659/
--rw-r--r--   0 runner    (1001) docker     (123)    12723 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-02 00:07:13.491162 pinecone-client-nightly-2.2.2.dev20230702000659/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 00:07:13.483162 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/__environment__
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/__version__
--rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 00:07:13.483162 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/api_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/api_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 00:07:13.483162 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 00:07:13.483162 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/api/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43926 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/api/index_operations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    38121 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/api/vector_operations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    36997 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 00:07:13.487162 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17845 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 00:07:13.487162 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11635 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/approximated_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11698 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/collection_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    11707 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/create_collection_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    16268 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12916 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/delete_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11755 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/describe_index_stats_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12954 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/describe_index_stats_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11664 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/fetch_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12242 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/hnsw_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11441 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/index_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    13694 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/index_meta_database.py
--rw-r--r--   0 runner    (1001) docker     (123)    11641 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/index_meta_database_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    11786 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/index_meta_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    11571 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/namespace_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    11732 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/patch_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/protobuf_any.py
--rw-r--r--   0 runner    (1001) docker     (123)    12416 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/protobuf_null_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    15518 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/query_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12307 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/query_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    13273 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/query_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)    11770 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/rpc_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    13071 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/scored_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)    11760 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/single_query_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    11562 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/sparse_values.py
--rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11947 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/upsert_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11309 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/upsert_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12705 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/vector.py
--rw-r--r--   0 runner    (1001) docker     (123)    80289 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 00:07:13.487162 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/models/
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12819 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 00:07:13.487162 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/grpc/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37787 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/grpc/index_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 00:07:13.487162 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/grpc/protos/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/grpc/protos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34942 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/grpc/protos/vector_column_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9908 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/grpc/protos/vector_column_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    57479 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/grpc/protos/vector_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/grpc/protos/vector_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/grpc/retry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 00:07:13.491162 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/utils/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    30364 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     9465 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 00:07:13.491162 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone_client_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-02 00:07:13.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone_client_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-07-02 00:07:13.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone_client_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 00:07:13.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone_client_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-02 00:07:13.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone_client_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-02 00:07:13.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone_client_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-02 00:07:13.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pinecone_client_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/requirements-grpc.txt
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-02 00:07:13.491162 pinecone-client-nightly-2.2.2.dev20230702000659/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-02 00:06:59.000000 pinecone-client-nightly-2.2.2.dev20230702000659/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:06:40.401060 pinecone-client-nightly-2.2.2.dev20230719000638/
+-rw-r--r--   0 runner    (1001) docker     (123)    12723 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-19 00:06:40.401060 pinecone-client-nightly-2.2.2.dev20230719000638/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:06:40.393060 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/__environment__
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/__version__
+-rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:06:40.397060 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/api_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/api_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:06:40.397060 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:06:40.397060 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43926 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/api/index_operations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38121 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/api/vector_operations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36997 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:06:40.397060 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17845 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:06:40.397060 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11635 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/approximated_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11698 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/collection_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11707 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/create_collection_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16268 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12916 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/delete_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11755 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/describe_index_stats_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12954 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/describe_index_stats_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11664 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/fetch_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12242 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/hnsw_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11441 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/index_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13694 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/index_meta_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11641 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/index_meta_database_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11786 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/index_meta_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11571 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/namespace_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11732 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/patch_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/protobuf_any.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12416 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/protobuf_null_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15518 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/query_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12307 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/query_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13273 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/query_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11770 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/rpc_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13071 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/scored_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11760 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/single_query_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11562 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/sparse_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11947 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/upsert_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11309 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/upsert_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12705 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80289 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:06:40.397060 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12819 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:06:40.401060 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37787 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/grpc/index_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:06:40.401060 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/grpc/protos/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/grpc/protos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34942 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/grpc/protos/vector_column_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9908 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/grpc/protos/vector_column_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57479 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/grpc/protos/vector_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/grpc/protos/vector_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/grpc/retry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:06:40.401060 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/utils/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30363 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9465 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:06:40.401060 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone_client_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-19 00:06:40.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone_client_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-07-19 00:06:40.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone_client_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 00:06:40.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone_client_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-19 00:06:40.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone_client_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-19 00:06:40.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone_client_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-19 00:06:40.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pinecone_client_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/requirements-grpc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-19 00:06:40.401060 pinecone-client-nightly-2.2.2.dev20230719000638/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-19 00:06:38.000000 pinecone-client-nightly-2.2.2.dev20230719000638/setup.py
```

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/LICENSE.txt` & `pinecone-client-nightly-2.2.2.dev20230719000638/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/PKG-INFO` & `pinecone-client-nightly-2.2.2.dev20230719000638/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinecone-client-nightly
-Version: 2.2.2.dev20230702000659
+Version: 2.2.2.dev20230719000638
 Summary: Pinecone client and SDK
 Home-page: https://www.pinecone.io/
 Author: Pinecone Systems, Inc.
 Author-email: support@pinecone.io
 License: Proprietary License
 Project-URL: Homepage, https://www.pinecone.io
 Project-URL: Documentation, https://pinecone.io/docs
```

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/config.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/config.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/api_action.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/api_action.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/api_base.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/api_base.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/__init__.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/__init__.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/api/index_operations_api.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/api/index_operations_api.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/api/vector_operations_api.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/api/vector_operations_api.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/api_client.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/api_client.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/apis/__init__.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/configuration.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/configuration.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/exceptions.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/approximated_config.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/approximated_config.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/collection_meta.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/collection_meta.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/create_collection_request.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/create_collection_request.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/create_request.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/create_request.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/delete_request.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/delete_request.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/describe_index_stats_request.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/describe_index_stats_request.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/describe_index_stats_response.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/describe_index_stats_response.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/fetch_response.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/fetch_response.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/hnsw_config.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/hnsw_config.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/index_meta.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/index_meta.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/index_meta_database.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/index_meta_database.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/index_meta_database_status.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/index_meta_database_status.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/index_meta_status.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/index_meta_status.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/namespace_summary.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/namespace_summary.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/patch_request.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/patch_request.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/protobuf_any.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/protobuf_null_value.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/protobuf_null_value.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/query_request.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/query_request.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/query_response.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/query_response.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/query_vector.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/query_vector.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/rpc_status.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/rpc_status.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/scored_vector.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/scored_vector.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/single_query_results.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/single_query_results.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/sparse_values.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/sparse_values.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/update_request.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/update_request.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/upsert_request.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/upsert_request.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/upsert_response.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/upsert_response.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model/vector.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model/vector.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/model_utils.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/model_utils.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/models/__init__.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/client/rest.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/client/rest.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/grpc/index_grpc.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/grpc/index_grpc.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/grpc/protos/vector_column_service_pb2.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/grpc/protos/vector_column_service_pb2.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/grpc/protos/vector_column_service_pb2_grpc.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/grpc/protos/vector_column_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/grpc/protos/vector_service_pb2.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/grpc/protos/vector_service_pb2.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/grpc/protos/vector_service_pb2_grpc.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/grpc/protos/vector_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/grpc/retry.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/grpc/retry.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/utils/__init__.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/utils/constants.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/utils/constants.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/core/utils/error_handling.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/core/utils/error_handling.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/exceptions.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/exceptions.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/index.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/index.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
                                      values=[1.0, 2.0, 3.0],
                                      sparse_values=SparseValues(indices=[1, 2], values=[0.2, 0.4]))])
 
         Args:
             vectors (Union[List[Vector], List[Tuple]]): A list of vectors to upsert.
 
                      A vector can be represented by a 1) Vector object, a 2) tuple or 3) a dictionary
-                     1) if a tuple is used, it must be of the form (id, values, meatadata) or (id, values).
+                     1) if a tuple is used, it must be of the form (id, values, metadata) or (id, values).
                         where id is a string, vector is a list of floats, metadata is a dict,
                         and sparse_values is a dict of the form {'indices': List[int], 'values': List[float]}.
                         Examples: ('id1', [1.0, 2.0, 3.0], {'key': 'value'}, {'indices': [1, 2], 'values': [0.2, 0.4]}),
                                   ('id1', [1.0, 2.0, 3.0], None, {'indices': [1, 2], 'values': [0.2, 0.4]})
                                   ('id1', [1.0, 2.0, 3.0], {'key': 'value'}), ('id2', [1.0, 2.0, 3.0]),
 
                     2) if a Vector object is used, a Vector object must be of the form
```

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/info.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/info.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone/manage.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone/manage.py`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone_client_nightly.egg-info/PKG-INFO` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone_client_nightly.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinecone-client-nightly
-Version: 2.2.2.dev20230702000659
+Version: 2.2.2.dev20230719000638
 Summary: Pinecone client and SDK
 Home-page: https://www.pinecone.io/
 Author: Pinecone Systems, Inc.
 Author-email: support@pinecone.io
 License: Proprietary License
 Project-URL: Homepage, https://www.pinecone.io
 Project-URL: Documentation, https://pinecone.io/docs
```

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/pinecone_client_nightly.egg-info/SOURCES.txt` & `pinecone-client-nightly-2.2.2.dev20230719000638/pinecone_client_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pinecone-client-nightly-2.2.2.dev20230702000659/setup.py` & `pinecone-client-nightly-2.2.2.dev20230719000638/setup.py`

 * *Files identical despite different names*

