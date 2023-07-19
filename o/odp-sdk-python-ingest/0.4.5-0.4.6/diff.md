# Comparing `tmp/odp_sdk_python_ingest-0.4.5.tar.gz` & `tmp/odp_sdk_python_ingest-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odp_sdk_python_ingest-0.4.5.tar", max compression
+gzip compressed data, was "odp_sdk_python_ingest-0.4.6.tar", max compression
```

## Comparing `odp_sdk_python_ingest-0.4.5.tar` & `odp_sdk_python_ingest-0.4.6.tar`

### file list

```diff
@@ -1,87 +1,87 @@
--rw-r--r--   0        0        0      842 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/README.md
--rw-r--r--   0        0        0        0 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/__init__.py
--rw-r--r--   0        0        0        0 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/auth/__init__.py
--rw-r--r--   0        0        0        0 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/auth/cdf/__init__.py
--rw-r--r--   0        0        0     3258 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/auth/cdf/cdf_token_handler.py
--rw-r--r--   0        0        0     1764 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/auth/cdf/federated_cognite_client.py
--rw-r--r--   0        0        0      163 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/auth/odp/__init__.py
--rw-r--r--   0        0        0     3064 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/auth/odp/interactive_login_token_handler.py
--rw-r--r--   0        0        0     1813 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/auth/odp/ropc_token_handler.py
--rw-r--r--   0        0        0     1358 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/auth/odp/token_handler.py
--rw-r--r--   0        0        0       49 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/auth/prefect/__init__.py
--rw-r--r--   0        0        0     3877 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/auth/prefect/prefect_b2c_client.py
--rw-r--r--   0        0        0        0 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/compute/__init__.py
--rw-r--r--   0        0        0        0 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/compute/blocks/__init__.py
--rw-r--r--   0        0        0     2374 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/compute/blocks/aad_client_credentials.py
--rw-r--r--   0        0        0     6042 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/compute/blocks/azure_storage.py
--rw-r--r--   0        0        0     2879 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/compute/blocks/cdf_storage.py
--rw-r--r--   0        0        0      579 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/compute/blocks/db_engine.py
--rw-r--r--   0        0        0      354 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/compute/blocks/odcat.py
--rw-r--r--   0        0        0     2378 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/compute/blocks/postgres.py
--rw-r--r--   0        0        0        0 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/compute/cli/__init__.py
--rw-r--r--   0        0        0      479 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/compute/cli/__main__.py
--rw-r--r--   0        0        0      435 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/compute/cli/authenticate.py
--rw-r--r--   0        0        0     2610 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/compute/cli/block.py
--rw-r--r--   0        0        0     5041 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/compute/cli/context.py
--rw-r--r--   0        0        0     7296 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/compute/cli/deploy.py
--rw-r--r--   0        0        0     2741 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/compute/cli/parameters.py
--rw-r--r--   0        0        0       43 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/compute/cli/params/__init__.py
--rw-r--r--   0        0        0      515 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/compute/cli/params/type_param_type.py
--rw-r--r--   0        0        0     3421 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/compute/cli/run.py
--rw-r--r--   0        0        0     1019 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/compute/cli/schema.py
--rw-r--r--   0        0        0        0 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/compute/config/__init__.py
--rw-r--r--   0        0        0      708 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/compute/config/cdf_config.py
--rw-r--r--   0        0        0      816 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/compute/config/dask_config.py
--rw-r--r--   0        0        0      125 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/compute/deploy/__init__.py
--rw-r--r--   0        0        0      216 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/compute/deploy/abstract_deployment_block.py
--rw-r--r--   0        0        0       40 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/compute/deploy/block/__init__.py
--rw-r--r--   0        0        0      501 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/compute/deploy/block/generic_block.py
--rw-r--r--   0        0        0     1591 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/compute/deploy/deployment_block_factory.py
--rw-r--r--   0        0        0      190 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/compute/deploy/runtime/__init__.py
--rw-r--r--   0        0        0      481 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/compute/deploy/runtime/abstract_runtime.py
--rw-r--r--   0        0        0     3463 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/compute/deploy/runtime/kubernetes.py
--rw-r--r--   0        0        0     4567 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/compute/deploy/runtime/kubernetes_dask.py
--rw-r--r--   0        0        0     1718 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/compute/deploy/runtime/kubernetes_tiered_resource.py
--rw-r--r--   0        0        0       88 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/compute/deploy/schedule/__init__.py
--rw-r--r--   0        0        0      417 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/compute/deploy/schedule/abstract_schedule.py
--rw-r--r--   0        0        0      471 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/compute/deploy/schedule/cron_schedule.py
--rw-r--r--   0        0        0     1030 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/compute/deploy/schedule/interval_schedule.py
--rw-r--r--   0        0        0       73 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/compute/deploy/storage/__init__.py
--rw-r--r--   0        0        0      938 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/compute/deploy/storage/abstract_storage.py
--rw-r--r--   0        0        0    10993 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/compute/deploy/storage/docker.py
--rw-r--r--   0        0        0        0 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/compute/deploy/storage/prefect_healthcheck.py
--rw-r--r--   0        0        0        0 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/compute/flow_state/__init__.py
--rw-r--r--   0        0        0     4679 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/compute/flow_state/stateful_value_impl.py
--rw-r--r--   0        0        0        0 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/compute/flow_state/store/__init__.py
--rw-r--r--   0        0        0     1060 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/compute/flow_state/store/watermark_file_store.py
--rw-r--r--   0        0        0      639 2023-05-25 11:48:05.335815 odp_sdk_python_ingest-0.4.5/odp/compute/flow_state/store/watermark_inmemory_store.py
--rw-r--r--   0        0        0      728 2023-05-25 11:48:05.339815 odp_sdk_python_ingest-0.4.5/odp/compute/flow_state/store/watermark_redis_store.py
--rw-r--r--   0        0        0     5488 2023-05-25 11:48:05.339815 odp_sdk_python_ingest-0.4.5/odp/compute/secrets.py
--rw-r--r--   0        0        0        0 2023-05-25 11:48:05.339815 odp_sdk_python_ingest-0.4.5/odp/compute/state_handlers/__init__.py
--rw-r--r--   0        0        0     2005 2023-05-25 11:48:05.339815 odp_sdk_python_ingest-0.4.5/odp/compute/state_handlers/metrics_pusher.py
--rw-r--r--   0        0        0        0 2023-05-25 11:48:05.339815 odp_sdk_python_ingest-0.4.5/odp/compute/tasks/__init__.py
--rw-r--r--   0        0        0        0 2023-05-25 11:48:05.339815 odp_sdk_python_ingest-0.4.5/odp/compute/tasks/cdf/__init__.py
--rw-r--r--   0        0        0     3217 2023-05-25 11:48:05.339815 odp_sdk_python_ingest-0.4.5/odp/compute/tasks/cdf/cdf_credentials.py
--rw-r--r--   0        0        0     1438 2023-05-25 11:48:05.339815 odp_sdk_python_ingest-0.4.5/odp/compute/tasks/concurrency_limit.py
--rw-r--r--   0        0        0      705 2023-05-25 11:48:05.339815 odp_sdk_python_ingest-0.4.5/odp/compute/tasks/measured_task.py
--rw-r--r--   0        0        0     1580 2023-05-25 11:48:05.339815 odp_sdk_python_ingest-0.4.5/odp/compute/tasks/tasks.py
--rw-r--r--   0        0        0        0 2023-05-25 11:48:05.339815 odp_sdk_python_ingest-0.4.5/odp/metrics/__init__.py
--rw-r--r--   0        0        0     4758 2023-05-25 11:48:05.339815 odp_sdk_python_ingest-0.4.5/odp/metrics/abstract_metrics.py
--rw-r--r--   0        0        0     2303 2023-05-25 11:48:05.339815 odp_sdk_python_ingest-0.4.5/odp/metrics/metric_client.py
--rw-r--r--   0        0        0        0 2023-05-25 11:48:05.339815 odp_sdk_python_ingest-0.4.5/odp/metrics/mock/__init__.py
--rw-r--r--   0        0        0     2523 2023-05-25 11:48:05.339815 odp_sdk_python_ingest-0.4.5/odp/metrics/mock/metric_client.py
--rw-r--r--   0        0        0     3271 2023-05-25 11:48:05.339815 odp_sdk_python_ingest-0.4.5/odp/metrics/mock/metrics.py
--rw-r--r--   0        0        0        0 2023-05-25 11:48:05.339815 odp_sdk_python_ingest-0.4.5/odp/metrics/prometheus/__init__.py
--rw-r--r--   0        0        0     2613 2023-05-25 11:48:05.339815 odp_sdk_python_ingest-0.4.5/odp/metrics/prometheus/metric_client.py
--rw-r--r--   0        0        0     3686 2023-05-25 11:48:05.339815 odp_sdk_python_ingest-0.4.5/odp/metrics/prometheus/metrics.py
--rw-r--r--   0        0        0        0 2023-05-25 11:48:05.339815 odp_sdk_python_ingest-0.4.5/odp/types/__init__.py
--rw-r--r--   0        0        0      361 2023-05-25 11:48:05.339815 odp_sdk_python_ingest-0.4.5/odp/types/file_info.py
--rw-r--r--   0        0        0      248 2023-05-25 11:48:05.339815 odp_sdk_python_ingest-0.4.5/odp/utils/__init__.py
--rw-r--r--   0        0        0     2887 2023-05-25 11:48:05.339815 odp_sdk_python_ingest-0.4.5/odp/utils/args.py
--rw-r--r--   0        0        0     1128 2023-05-25 11:48:05.339815 odp_sdk_python_ingest-0.4.5/odp/utils/deploy_helpers.py
--rw-r--r--   0        0        0     4913 2023-05-25 11:48:05.339815 odp_sdk_python_ingest-0.4.5/odp/utils/import_helpers.py
--rw-r--r--   0        0        0      607 2023-05-25 11:48:05.339815 odp_sdk_python_ingest-0.4.5/odp/utils/naming.py
--rw-r--r--   0        0        0     5715 2023-05-25 11:48:05.339815 odp_sdk_python_ingest-0.4.5/odp/utils/retry.py
--rw-r--r--   0        0        0      317 2023-05-25 11:48:05.339815 odp_sdk_python_ingest-0.4.5/odp/utils/timers.py
--rw-r--r--   0        0        0     1945 2023-05-25 11:49:25.651601 odp_sdk_python_ingest-0.4.5/pyproject.toml
--rw-r--r--   0        0        0     2544 1970-01-01 00:00:00.000000 odp_sdk_python_ingest-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0      842 2023-07-19 13:13:17.759530 odp_sdk_python_ingest-0.4.6/README.md
+-rw-r--r--   0        0        0        0 2023-07-19 13:13:17.759530 odp_sdk_python_ingest-0.4.6/odp/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-19 13:13:17.759530 odp_sdk_python_ingest-0.4.6/odp/auth/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-19 13:13:17.759530 odp_sdk_python_ingest-0.4.6/odp/auth/cdf/__init__.py
+-rw-r--r--   0        0        0     3258 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/auth/cdf/cdf_token_handler.py
+-rw-r--r--   0        0        0     1764 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/auth/cdf/federated_cognite_client.py
+-rw-r--r--   0        0        0      163 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/auth/odp/__init__.py
+-rw-r--r--   0        0        0     3306 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/auth/odp/interactive_login_token_handler.py
+-rw-r--r--   0        0        0     1813 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/auth/odp/ropc_token_handler.py
+-rw-r--r--   0        0        0     1358 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/auth/odp/token_handler.py
+-rw-r--r--   0        0        0       49 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/auth/prefect/__init__.py
+-rw-r--r--   0        0        0     3877 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/auth/prefect/prefect_b2c_client.py
+-rw-r--r--   0        0        0        0 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/blocks/__init__.py
+-rw-r--r--   0        0        0     2490 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/blocks/aad_client_credentials.py
+-rw-r--r--   0        0        0     6042 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/blocks/azure_storage.py
+-rw-r--r--   0        0        0     2879 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/blocks/cdf_storage.py
+-rw-r--r--   0        0        0      579 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/blocks/db_engine.py
+-rw-r--r--   0        0        0      354 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/blocks/odcat.py
+-rw-r--r--   0        0        0     2378 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/blocks/postgres.py
+-rw-r--r--   0        0        0        0 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/cli/__init__.py
+-rw-r--r--   0        0        0      479 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/cli/__main__.py
+-rw-r--r--   0        0        0      435 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/cli/authenticate.py
+-rw-r--r--   0        0        0     2610 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/cli/block.py
+-rw-r--r--   0        0        0     5041 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/cli/context.py
+-rw-r--r--   0        0        0     7296 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/cli/deploy.py
+-rw-r--r--   0        0        0     2741 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/cli/parameters.py
+-rw-r--r--   0        0        0       43 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/cli/params/__init__.py
+-rw-r--r--   0        0        0      515 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/cli/params/type_param_type.py
+-rw-r--r--   0        0        0     3421 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/cli/run.py
+-rw-r--r--   0        0        0     1019 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/cli/schema.py
+-rw-r--r--   0        0        0        0 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/config/__init__.py
+-rw-r--r--   0        0        0      708 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/config/cdf_config.py
+-rw-r--r--   0        0        0      816 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/config/dask_config.py
+-rw-r--r--   0        0        0      125 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/deploy/__init__.py
+-rw-r--r--   0        0        0      216 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/deploy/abstract_deployment_block.py
+-rw-r--r--   0        0        0       40 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/deploy/block/__init__.py
+-rw-r--r--   0        0        0      501 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/deploy/block/generic_block.py
+-rw-r--r--   0        0        0     1591 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/deploy/deployment_block_factory.py
+-rw-r--r--   0        0        0      190 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/deploy/runtime/__init__.py
+-rw-r--r--   0        0        0      481 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/deploy/runtime/abstract_runtime.py
+-rw-r--r--   0        0        0     3463 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/deploy/runtime/kubernetes.py
+-rw-r--r--   0        0        0     4567 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/deploy/runtime/kubernetes_dask.py
+-rw-r--r--   0        0        0     1718 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/deploy/runtime/kubernetes_tiered_resource.py
+-rw-r--r--   0        0        0       88 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/deploy/schedule/__init__.py
+-rw-r--r--   0        0        0      417 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/deploy/schedule/abstract_schedule.py
+-rw-r--r--   0        0        0      471 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/deploy/schedule/cron_schedule.py
+-rw-r--r--   0        0        0     1030 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/deploy/schedule/interval_schedule.py
+-rw-r--r--   0        0        0       73 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/deploy/storage/__init__.py
+-rw-r--r--   0        0        0      938 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/deploy/storage/abstract_storage.py
+-rw-r--r--   0        0        0    10993 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/deploy/storage/docker.py
+-rw-r--r--   0        0        0        0 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/deploy/storage/prefect_healthcheck.py
+-rw-r--r--   0        0        0        0 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/flow_state/__init__.py
+-rw-r--r--   0        0        0     4679 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/flow_state/stateful_value_impl.py
+-rw-r--r--   0        0        0        0 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/flow_state/store/__init__.py
+-rw-r--r--   0        0        0     1060 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/flow_state/store/watermark_file_store.py
+-rw-r--r--   0        0        0      639 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/flow_state/store/watermark_inmemory_store.py
+-rw-r--r--   0        0        0      728 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/flow_state/store/watermark_redis_store.py
+-rw-r--r--   0        0        0     5488 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/secrets.py
+-rw-r--r--   0        0        0        0 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/state_handlers/__init__.py
+-rw-r--r--   0        0        0     2005 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/state_handlers/metrics_pusher.py
+-rw-r--r--   0        0        0        0 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/tasks/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/tasks/cdf/__init__.py
+-rw-r--r--   0        0        0     3217 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/tasks/cdf/cdf_credentials.py
+-rw-r--r--   0        0        0     1438 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/tasks/concurrency_limit.py
+-rw-r--r--   0        0        0      705 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/tasks/measured_task.py
+-rw-r--r--   0        0        0     1580 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/compute/tasks/tasks.py
+-rw-r--r--   0        0        0        0 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/metrics/__init__.py
+-rw-r--r--   0        0        0     4758 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/metrics/abstract_metrics.py
+-rw-r--r--   0        0        0     2303 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/metrics/metric_client.py
+-rw-r--r--   0        0        0        0 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/metrics/mock/__init__.py
+-rw-r--r--   0        0        0     2523 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/metrics/mock/metric_client.py
+-rw-r--r--   0        0        0     3271 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/metrics/mock/metrics.py
+-rw-r--r--   0        0        0        0 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/metrics/prometheus/__init__.py
+-rw-r--r--   0        0        0     2613 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/metrics/prometheus/metric_client.py
+-rw-r--r--   0        0        0     3686 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/metrics/prometheus/metrics.py
+-rw-r--r--   0        0        0        0 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/types/__init__.py
+-rw-r--r--   0        0        0      361 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/types/file_info.py
+-rw-r--r--   0        0        0      248 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/utils/__init__.py
+-rw-r--r--   0        0        0     2887 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/utils/args.py
+-rw-r--r--   0        0        0     1128 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/utils/deploy_helpers.py
+-rw-r--r--   0        0        0     4913 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/utils/import_helpers.py
+-rw-r--r--   0        0        0      607 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/utils/naming.py
+-rw-r--r--   0        0        0     5715 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/utils/retry.py
+-rw-r--r--   0        0        0      317 2023-07-19 13:13:17.763530 odp_sdk_python_ingest-0.4.6/odp/utils/timers.py
+-rw-r--r--   0        0        0     1945 2023-07-19 13:14:33.248227 odp_sdk_python_ingest-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0     2544 1970-01-01 00:00:00.000000 odp_sdk_python_ingest-0.4.6/PKG-INFO
```

### Comparing `odp_sdk_python_ingest-0.4.5/README.md` & `odp_sdk_python_ingest-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.5/odp/auth/cdf/cdf_token_handler.py` & `odp_sdk_python_ingest-0.4.6/odp/auth/cdf/cdf_token_handler.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.5/odp/auth/cdf/federated_cognite_client.py` & `odp_sdk_python_ingest-0.4.6/odp/auth/cdf/federated_cognite_client.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.5/odp/auth/odp/interactive_login_token_handler.py` & `odp_sdk_python_ingest-0.4.6/odp/auth/odp/interactive_login_token_handler.py`

 * *Files 9% similar despite different names*

```diff
@@ -73,12 +73,18 @@
             token = self._app.acquire_token_interactive(
                 scopes=self._scopes,
             )
 
         if not token:
             raise RuntimeError("Failed to obtain user token")
 
-        claims = token["id_token_claims"]
-        exp = claims["exp"]
+        if "id_token_claims" in token:
+            claims = token["id_token_claims"]
+            exp = claims["exp"]
+            self._token = token["id_token"]
+        elif "access_token" in token:
+            exp = token["expires_in"]
+            self._token = token["access_token"]
+        else:
+            raise RuntimeError("Invalid user token")
 
-        self._token = token["id_token"]
         self._token_expiry = datetime.fromtimestamp(exp)
```

### Comparing `odp_sdk_python_ingest-0.4.5/odp/auth/odp/ropc_token_handler.py` & `odp_sdk_python_ingest-0.4.6/odp/auth/odp/ropc_token_handler.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.5/odp/auth/odp/token_handler.py` & `odp_sdk_python_ingest-0.4.6/odp/auth/odp/token_handler.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.5/odp/auth/prefect/prefect_b2c_client.py` & `odp_sdk_python_ingest-0.4.6/odp/auth/prefect/prefect_b2c_client.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.5/odp/compute/blocks/aad_client_credentials.py` & `odp_sdk_python_ingest-0.4.6/odp/compute/blocks/aad_client_credentials.py`

 * *Files 10% similar despite different names*

```diff
@@ -59,15 +59,18 @@
                 "client_secret": self.client_secret.get_secret_value(),
                 "scope": self.scope.get_secret_value(),
                 "grant_type": self.grant_type,
             },
         )
         response.raise_for_status()
         response_data = response.json()
-        self._expiry_time = response_data["expires_on"]
+        try:
+            self._expiry_time = response_data["expires_on"]
+        except KeyError:
+            self._expiry_time = time.time() + response_data["expires_in"]
         return response_data["access_token"]
 
     def _auth_callback(self, request: requests.PreparedRequest) -> requests.PreparedRequest:
         request.headers.update({"Authorization": f"Bearer {self.get_token()}"})
         return request
 
     @contextmanager
```

### Comparing `odp_sdk_python_ingest-0.4.5/odp/compute/blocks/azure_storage.py` & `odp_sdk_python_ingest-0.4.6/odp/compute/blocks/azure_storage.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.5/odp/compute/blocks/cdf_storage.py` & `odp_sdk_python_ingest-0.4.6/odp/compute/blocks/cdf_storage.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.5/odp/compute/blocks/db_engine.py` & `odp_sdk_python_ingest-0.4.6/odp/compute/blocks/db_engine.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.5/odp/compute/blocks/postgres.py` & `odp_sdk_python_ingest-0.4.6/odp/compute/blocks/postgres.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.5/odp/compute/cli/block.py` & `odp_sdk_python_ingest-0.4.6/odp/compute/cli/block.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.5/odp/compute/cli/context.py` & `odp_sdk_python_ingest-0.4.6/odp/compute/cli/context.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.5/odp/compute/cli/deploy.py` & `odp_sdk_python_ingest-0.4.6/odp/compute/cli/deploy.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.5/odp/compute/cli/parameters.py` & `odp_sdk_python_ingest-0.4.6/odp/compute/cli/parameters.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.5/odp/compute/cli/params/type_param_type.py` & `odp_sdk_python_ingest-0.4.6/odp/compute/cli/params/type_param_type.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.5/odp/compute/cli/run.py` & `odp_sdk_python_ingest-0.4.6/odp/compute/cli/run.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.5/odp/compute/cli/schema.py` & `odp_sdk_python_ingest-0.4.6/odp/compute/cli/schema.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.5/odp/compute/config/cdf_config.py` & `odp_sdk_python_ingest-0.4.6/odp/compute/config/cdf_config.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.5/odp/compute/config/dask_config.py` & `odp_sdk_python_ingest-0.4.6/odp/compute/config/dask_config.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.5/odp/compute/deploy/deployment_block_factory.py` & `odp_sdk_python_ingest-0.4.6/odp/compute/deploy/deployment_block_factory.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.5/odp/compute/deploy/runtime/kubernetes.py` & `odp_sdk_python_ingest-0.4.6/odp/compute/deploy/runtime/kubernetes.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.5/odp/compute/deploy/runtime/kubernetes_dask.py` & `odp_sdk_python_ingest-0.4.6/odp/compute/deploy/runtime/kubernetes_dask.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.5/odp/compute/deploy/runtime/kubernetes_tiered_resource.py` & `odp_sdk_python_ingest-0.4.6/odp/compute/deploy/runtime/kubernetes_tiered_resource.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.5/odp/compute/deploy/schedule/interval_schedule.py` & `odp_sdk_python_ingest-0.4.6/odp/compute/deploy/schedule/interval_schedule.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.5/odp/compute/deploy/storage/abstract_storage.py` & `odp_sdk_python_ingest-0.4.6/odp/compute/deploy/storage/abstract_storage.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.5/odp/compute/deploy/storage/docker.py` & `odp_sdk_python_ingest-0.4.6/odp/compute/deploy/storage/docker.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.5/odp/compute/flow_state/stateful_value_impl.py` & `odp_sdk_python_ingest-0.4.6/odp/compute/flow_state/stateful_value_impl.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.5/odp/compute/flow_state/store/watermark_file_store.py` & `odp_sdk_python_ingest-0.4.6/odp/compute/flow_state/store/watermark_file_store.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.5/odp/compute/flow_state/store/watermark_inmemory_store.py` & `odp_sdk_python_ingest-0.4.6/odp/compute/flow_state/store/watermark_inmemory_store.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.5/odp/compute/flow_state/store/watermark_redis_store.py` & `odp_sdk_python_ingest-0.4.6/odp/compute/flow_state/store/watermark_redis_store.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.5/odp/compute/secrets.py` & `odp_sdk_python_ingest-0.4.6/odp/compute/secrets.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.5/odp/compute/state_handlers/metrics_pusher.py` & `odp_sdk_python_ingest-0.4.6/odp/compute/state_handlers/metrics_pusher.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.5/odp/compute/tasks/cdf/cdf_credentials.py` & `odp_sdk_python_ingest-0.4.6/odp/compute/tasks/cdf/cdf_credentials.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.5/odp/compute/tasks/concurrency_limit.py` & `odp_sdk_python_ingest-0.4.6/odp/compute/tasks/concurrency_limit.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.5/odp/compute/tasks/measured_task.py` & `odp_sdk_python_ingest-0.4.6/odp/compute/tasks/measured_task.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.5/odp/compute/tasks/tasks.py` & `odp_sdk_python_ingest-0.4.6/odp/compute/tasks/tasks.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.5/odp/metrics/abstract_metrics.py` & `odp_sdk_python_ingest-0.4.6/odp/metrics/abstract_metrics.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.5/odp/metrics/metric_client.py` & `odp_sdk_python_ingest-0.4.6/odp/metrics/metric_client.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.5/odp/metrics/mock/metric_client.py` & `odp_sdk_python_ingest-0.4.6/odp/metrics/mock/metric_client.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.5/odp/metrics/mock/metrics.py` & `odp_sdk_python_ingest-0.4.6/odp/metrics/mock/metrics.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.5/odp/metrics/prometheus/metric_client.py` & `odp_sdk_python_ingest-0.4.6/odp/metrics/prometheus/metric_client.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.5/odp/metrics/prometheus/metrics.py` & `odp_sdk_python_ingest-0.4.6/odp/metrics/prometheus/metrics.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.5/odp/utils/args.py` & `odp_sdk_python_ingest-0.4.6/odp/utils/args.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.5/odp/utils/deploy_helpers.py` & `odp_sdk_python_ingest-0.4.6/odp/utils/deploy_helpers.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.5/odp/utils/import_helpers.py` & `odp_sdk_python_ingest-0.4.6/odp/utils/import_helpers.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.5/odp/utils/naming.py` & `odp_sdk_python_ingest-0.4.6/odp/utils/naming.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.5/odp/utils/retry.py` & `odp_sdk_python_ingest-0.4.6/odp/utils/retry.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.5/pyproject.toml` & `odp_sdk_python_ingest-0.4.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "odp-sdk-python-ingest"
-version = "0.4.5"
+version = "0.4.6"
 description = "ODP ingest SDK"
 authors = ["Thomas Li Fredriksen <thomas.fredriksen@oceandata.earth>"]
 readme = "README.md"
 packages = [
     {include="odp"}
 ]
```

### Comparing `odp_sdk_python_ingest-0.4.5/PKG-INFO` & `odp_sdk_python_ingest-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odp-sdk-python-ingest
-Version: 0.4.5
+Version: 0.4.6
 Summary: ODP ingest SDK
 Author: Thomas Li Fredriksen
 Author-email: thomas.fredriksen@oceandata.earth
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: odp-sdk-python-ingest Version: 0.4.5 Summary: ODP
+Metadata-Version: 2.1 Name: odp-sdk-python-ingest Version: 0.4.6 Summary: ODP
 ingest SDK Author: Thomas Li Fredriksen Author-email:
 thomas.fredriksen@oceandata.earth Requires-Python: >=3.10,<4.0 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-Dist:
 azure-common (>=1.1.28,<2.0.0) Requires-Dist: azure-identity (>=1.11.0,<2.0.0)
 Requires-Dist: azure-keyvault (>=4.2.0,<5.0.0) Requires-Dist: azure-keyvault-
 secrets (>=4.6.0,<5.0.0) Requires-Dist: azure-storage-blob (>=12.13.1,<13.0.0)
```

