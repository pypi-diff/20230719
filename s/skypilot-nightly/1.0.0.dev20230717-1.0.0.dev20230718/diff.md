# Comparing `tmp/skypilot-nightly-1.0.0.dev20230717.tar.gz` & `tmp/skypilot-nightly-1.0.0.dev20230718.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skypilot-nightly-1.0.0.dev20230717.tar", last modified: Mon Jul 17 10:43:20 2023, max compression
+gzip compressed data, was "skypilot-nightly-1.0.0.dev20230718.tar", last modified: Tue Jul 18 10:40:58 2023, max compression
```

## Comparing `skypilot-nightly-1.0.0.dev20230717.tar` & `skypilot-nightly-1.0.0.dev20230718.tar`

### file list

```diff
@@ -1,228 +1,228 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.341377 skypilot-nightly-1.0.0.dev20230717/
--rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-07-17 10:43:20.341377 skypilot-nightly-1.0.0.dev20230717/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8543 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 10:43:20.341377 skypilot-nightly-1.0.0.dev20230717/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-07-17 10:43:10.000000 skypilot-nightly-1.0.0.dev20230717/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.317377 skypilot-nightly-1.0.0.dev20230717/sky/
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-17 10:43:10.000000 skypilot-nightly-1.0.0.dev20230717/sky/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.317377 skypilot-nightly-1.0.0.dev20230717/sky/adaptors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/adaptors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/adaptors/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/adaptors/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/adaptors/cloudflare.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/adaptors/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/adaptors/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/adaptors/ibm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/adaptors/oci.py
--rw-r--r--   0 runner    (1001) docker     (123)    15607 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.321377 skypilot-nightly-1.0.0.dev20230717/sky/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/backends/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)   112970 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/backends/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   200283 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/backends/cloud_vm_ray_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/backends/docker_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16448 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/backends/local_docker_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.321377 skypilot-nightly-1.0.0.dev20230717/sky/backends/monkey_patches/
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/backends/monkey_patches/monkey_patch_ray_up.py
--rw-r--r--   0 runner    (1001) docker     (123)    24422 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/backends/onprem_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/backends/wheel_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.321377 skypilot-nightly-1.0.0.dev20230717/sky/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8723 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/benchmark/benchmark_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    24638 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/benchmark/benchmark_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/check.py
--rw-r--r--   0 runner    (1001) docker     (123)   167453 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/cloud_stores.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.321377 skypilot-nightly-1.0.0.dev20230717/sky/clouds/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41057 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)    25762 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    26861 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    42681 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)    20117 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/ibm.py
--rw-r--r--   0 runner    (1001) docker     (123)    12001 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/lambda_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    24269 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/oci.py
--rw-r--r--   0 runner    (1001) docker     (123)    14878 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/scp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.321377 skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/
--rw-r--r--   0 runner    (1001) docker     (123)    12336 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/aws_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/azure_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    23188 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.325377 skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/data_fetchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/data_fetchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20092 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/data_fetchers/fetch_aws.py
--rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/data_fetchers/fetch_azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    18601 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    18969 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/gcp_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/ibm_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/lambda_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/oci_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/scp_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    40110 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/dag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.325377 skypilot-nightly-1.0.0.dev20230717/sky/data/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/data/data_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/data/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/data/mounting_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    89247 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/data/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/data/storage_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    41456 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)    26274 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/global_user_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    43765 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.325377 skypilot-nightly-1.0.0.dev20230717/sky/provision/
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/provision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.325377 skypilot-nightly-1.0.0.dev20230717/sky/provision/aws/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/provision/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/provision/aws/instance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.325377 skypilot-nightly-1.0.0.dev20230717/sky/provision/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/provision/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/provision/gcp/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/provision/gcp/instance_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    42860 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.325377 skypilot-nightly-1.0.0.dev20230717/sky/setup_files/
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/setup_files/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-07-17 10:43:10.000000 skypilot-nightly-1.0.0.dev20230717/sky/setup_files/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/sky_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.325377 skypilot-nightly-1.0.0.dev20230717/sky/skylet/
--rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/attempt_skylet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/autostop_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    32722 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/job_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    19585 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/log_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.313377 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.329377 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/aws/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.329377 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/aws/cloudwatch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/aws/cloudwatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32698 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    52192 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/aws/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    29406 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/aws/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/aws/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.329377 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/azure/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/azure/azure-config-template.json
--rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/azure/azure-vm-template.json
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/azure/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    17469 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/azure/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.329377 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34963 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/gcp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/gcp/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    26192 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/gcp/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    14292 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/gcp/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.329377 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/ibm/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/ibm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38280 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/ibm/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/ibm/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    34628 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/ibm/vpc_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.329377 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/lambda_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/lambda_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/lambda_cloud/lambda_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/lambda_cloud/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.329377 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/oci/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/oci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/oci/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    20136 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/oci/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    17048 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/oci/query_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/oci/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.333377 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/scp/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/scp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/scp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    22219 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/scp/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    15481 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/scp/scp_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.333377 skypilot-nightly-1.0.0.dev20230717/sky/skylet/ray_patches/
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/ray_patches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/ray_patches/autoscaler.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/ray_patches/cli.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/ray_patches/command_runner.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/ray_patches/job_head.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/ray_patches/log_monitor.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/ray_patches/resource_demand_scheduler.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/ray_patches/updater.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/ray_patches/worker.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/skylet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/subprocess_daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skypilot_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.333377 skypilot-nightly-1.0.0.dev20230717/sky/spot/
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/spot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/spot/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    25102 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/spot/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.333377 skypilot-nightly-1.0.0.dev20230717/sky/spot/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/spot/dashboard/dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.333377 skypilot-nightly-1.0.0.dev20230717/sky/spot/dashboard/static/
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/spot/dashboard/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.333377 skypilot-nightly-1.0.0.dev20230717/sky/spot/dashboard/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/spot/dashboard/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    21311 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/spot/recovery_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    22484 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/spot/spot_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    34333 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/spot/spot_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/status_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    38424 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.333377 skypilot-nightly-1.0.0.dev20230717/sky/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    11406 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/templates/aws-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/templates/azure-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)    11151 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/templates/gcp-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/templates/gcp-tpu-create.sh.j2
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/templates/gcp-tpu-delete.sh.j2
--rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/templates/ibm-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/templates/lambda-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/templates/local-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/templates/oci-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/templates/scp-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/templates/spot-controller.yaml.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.337377 skypilot-nightly-1.0.0.dev20230717/sky/usage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/usage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/usage/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    17294 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/usage/usage_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.337377 skypilot-nightly-1.0.0.dev20230717/sky/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/utils/accelerator_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.337377 skypilot-nightly-1.0.0.dev20230717/sky/utils/cli_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/utils/cli_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14891 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/utils/cli_utils/status_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14688 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/utils/command_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    12077 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/utils/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/utils/dag_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/utils/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/utils/env_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/utils/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/utils/subprocess_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/utils/timeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/utils/tpu_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/utils/ux_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/utils/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.337377 skypilot-nightly-1.0.0.dev20230717/skypilot_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-07-17 10:43:20.000000 skypilot-nightly-1.0.0.dev20230717/skypilot_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-07-17 10:43:20.000000 skypilot-nightly-1.0.0.dev20230717/skypilot_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 10:43:20.000000 skypilot-nightly-1.0.0.dev20230717/skypilot_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-17 10:43:20.000000 skypilot-nightly-1.0.0.dev20230717/skypilot_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-17 10:43:20.000000 skypilot-nightly-1.0.0.dev20230717/skypilot_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-17 10:43:20.000000 skypilot-nightly-1.0.0.dev20230717/skypilot_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.341377 skypilot-nightly-1.0.0.dev20230717/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/tests/test_global_user_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/tests/test_list_accelerators.py
--rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/tests/test_onprem.py
--rw-r--r--   0 runner    (1001) docker     (123)    22937 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/tests/test_optimizer_dryruns.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/tests/test_optimizer_random_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/tests/test_pycryptodome_version.py
--rw-r--r--   0 runner    (1001) docker     (123)   124066 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/tests/test_smoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/tests/test_spot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/tests/test_wheels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:40:58.749944 skypilot-nightly-1.0.0.dev20230718/
+-rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-07-18 10:40:58.749944 skypilot-nightly-1.0.0.dev20230718/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8543 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 10:40:58.749944 skypilot-nightly-1.0.0.dev20230718/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-07-18 10:40:50.000000 skypilot-nightly-1.0.0.dev20230718/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:40:58.729944 skypilot-nightly-1.0.0.dev20230718/sky/
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-18 10:40:50.000000 skypilot-nightly-1.0.0.dev20230718/sky/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:40:58.729944 skypilot-nightly-1.0.0.dev20230718/sky/adaptors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/adaptors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/adaptors/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/adaptors/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/adaptors/cloudflare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/adaptors/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/adaptors/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/adaptors/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/adaptors/oci.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15607 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:40:58.729944 skypilot-nightly-1.0.0.dev20230718/sky/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/backends/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)   112970 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/backends/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   200448 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/backends/cloud_vm_ray_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/backends/docker_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16448 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/backends/local_docker_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:40:58.729944 skypilot-nightly-1.0.0.dev20230718/sky/backends/monkey_patches/
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/backends/monkey_patches/monkey_patch_ray_up.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24422 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/backends/onprem_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/backends/wheel_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:40:58.729944 skypilot-nightly-1.0.0.dev20230718/sky/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8723 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/benchmark/benchmark_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24638 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/benchmark/benchmark_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)   167453 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/cloud_stores.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:40:58.733944 skypilot-nightly-1.0.0.dev20230718/sky/clouds/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/clouds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41057 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/clouds/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25762 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/clouds/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26861 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/clouds/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42863 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/clouds/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20117 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/clouds/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12001 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/clouds/lambda_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/clouds/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24269 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/clouds/oci.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14878 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/clouds/scp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:40:58.733944 skypilot-nightly-1.0.0.dev20230718/sky/clouds/service_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)    12350 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/clouds/service_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/clouds/service_catalog/aws_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/clouds/service_catalog/azure_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23188 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/clouds/service_catalog/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/clouds/service_catalog/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/clouds/service_catalog/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:40:58.733944 skypilot-nightly-1.0.0.dev20230718/sky/clouds/service_catalog/data_fetchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/clouds/service_catalog/data_fetchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20092 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/clouds/service_catalog/data_fetchers/fetch_aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/clouds/service_catalog/data_fetchers/fetch_azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18557 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19540 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/clouds/service_catalog/gcp_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/clouds/service_catalog/ibm_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/clouds/service_catalog/lambda_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/clouds/service_catalog/oci_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/clouds/service_catalog/scp_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40110 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/dag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:40:58.733944 skypilot-nightly-1.0.0.dev20230718/sky/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/data/data_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/data/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/data/mounting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89247 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/data/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/data/storage_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41456 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26274 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/global_user_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43765 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:40:58.733944 skypilot-nightly-1.0.0.dev20230718/sky/provision/
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/provision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:40:58.737944 skypilot-nightly-1.0.0.dev20230718/sky/provision/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/provision/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/provision/aws/instance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:40:58.737944 skypilot-nightly-1.0.0.dev20230718/sky/provision/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/provision/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/provision/gcp/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/provision/gcp/instance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42860 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:40:58.737944 skypilot-nightly-1.0.0.dev20230718/sky/setup_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/setup_files/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-07-18 10:40:50.000000 skypilot-nightly-1.0.0.dev20230718/sky/setup_files/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/sky_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:40:58.737944 skypilot-nightly-1.0.0.dev20230718/sky/skylet/
+-rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/attempt_skylet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/autostop_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32722 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/job_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19585 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/log_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:40:58.725944 skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:40:58.737944 skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:40:58.737944 skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/aws/cloudwatch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/aws/cloudwatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32698 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52192 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/aws/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29406 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/aws/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/aws/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:40:58.737944 skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/azure/azure-config-template.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/azure/azure-vm-template.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/azure/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17469 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/azure/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:40:58.741944 skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34963 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/gcp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/gcp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26192 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/gcp/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14292 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/gcp/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:40:58.741944 skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/ibm/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/ibm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38280 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/ibm/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/ibm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34628 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/ibm/vpc_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:40:58.741944 skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/lambda_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/lambda_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/lambda_cloud/lambda_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/lambda_cloud/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:40:58.741944 skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/oci/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/oci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/oci/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20136 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/oci/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17048 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/oci/query_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/oci/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:40:58.741944 skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/scp/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/scp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/scp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22219 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/scp/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15481 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/scp/scp_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:40:58.741944 skypilot-nightly-1.0.0.dev20230718/sky/skylet/ray_patches/
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/ray_patches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/ray_patches/autoscaler.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/ray_patches/cli.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/ray_patches/command_runner.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/ray_patches/job_head.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/ray_patches/log_monitor.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/ray_patches/resource_demand_scheduler.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/ray_patches/updater.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/ray_patches/worker.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/skylet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skylet/subprocess_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/skypilot_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:40:58.745944 skypilot-nightly-1.0.0.dev20230718/sky/spot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/spot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/spot/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25102 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/spot/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:40:58.745944 skypilot-nightly-1.0.0.dev20230718/sky/spot/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/spot/dashboard/dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:40:58.745944 skypilot-nightly-1.0.0.dev20230718/sky/spot/dashboard/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/spot/dashboard/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:40:58.745944 skypilot-nightly-1.0.0.dev20230718/sky/spot/dashboard/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/spot/dashboard/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    21311 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/spot/recovery_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22484 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/spot/spot_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34333 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/spot/spot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/status_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38424 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:40:58.745944 skypilot-nightly-1.0.0.dev20230718/sky/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    11406 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/templates/aws-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/templates/azure-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)    11151 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/templates/gcp-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/templates/gcp-tpu-create.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/templates/gcp-tpu-delete.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/templates/ibm-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/templates/lambda-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/templates/local-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/templates/oci-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/templates/scp-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/templates/spot-controller.yaml.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:40:58.745944 skypilot-nightly-1.0.0.dev20230718/sky/usage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/usage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/usage/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17294 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/usage/usage_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:40:58.745944 skypilot-nightly-1.0.0.dev20230718/sky/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/utils/accelerator_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:40:58.745944 skypilot-nightly-1.0.0.dev20230718/sky/utils/cli_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/utils/cli_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14891 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/utils/cli_utils/status_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14688 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/utils/command_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12077 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/utils/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/utils/dag_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/utils/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/utils/env_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/utils/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/utils/subprocess_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/utils/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/utils/tpu_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/utils/ux_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/sky/utils/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:40:58.749944 skypilot-nightly-1.0.0.dev20230718/skypilot_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-07-18 10:40:58.000000 skypilot-nightly-1.0.0.dev20230718/skypilot_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-07-18 10:40:58.000000 skypilot-nightly-1.0.0.dev20230718/skypilot_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 10:40:58.000000 skypilot-nightly-1.0.0.dev20230718/skypilot_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-18 10:40:58.000000 skypilot-nightly-1.0.0.dev20230718/skypilot_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-18 10:40:58.000000 skypilot-nightly-1.0.0.dev20230718/skypilot_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-18 10:40:58.000000 skypilot-nightly-1.0.0.dev20230718/skypilot_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:40:58.749944 skypilot-nightly-1.0.0.dev20230718/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/tests/test_global_user_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/tests/test_list_accelerators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/tests/test_onprem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22937 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/tests/test_optimizer_dryruns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/tests/test_optimizer_random_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/tests/test_pycryptodome_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124131 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/tests/test_smoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/tests/test_spot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-18 10:40:45.000000 skypilot-nightly-1.0.0.dev20230718/tests/test_wheels.py
```

### Comparing `skypilot-nightly-1.0.0.dev20230717/LICENSE` & `skypilot-nightly-1.0.0.dev20230718/LICENSE`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/MANIFEST.in` & `skypilot-nightly-1.0.0.dev20230718/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/PKG-INFO` & `skypilot-nightly-1.0.0.dev20230718/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skypilot-nightly
-Version: 1.0.0.dev20230717
+Version: 1.0.0.dev20230718
 Summary: SkyPilot: An intercloud broker for the clouds
 Author: SkyPilot Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/skypilot-org/skypilot
 Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: skypilot-nightly Version: 1.0.0.dev20230717
+Metadata-Version: 2.1 Name: skypilot-nightly Version: 1.0.0.dev20230718
 Summary: SkyPilot: An intercloud broker for the clouds Author: SkyPilot Team
 License: Apache 2.0 Project-URL: Homepage, https://github.com/skypilot-org/
 skypilot Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `skypilot-nightly-1.0.0.dev20230717/README.md` & `skypilot-nightly-1.0.0.dev20230718/README.md`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/pyproject.toml` & `skypilot-nightly-1.0.0.dev20230718/pyproject.toml`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/setup.py` & `skypilot-nightly-1.0.0.dev20230718/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,15 +108,19 @@
     # Adopted from ray's setup.py:
     # https://github.com/ray-project/ray/blob/86fab1764e618215d8131e8e5068f0d493c77023/python/setup.py#L326
     'protobuf >= 3.15.3, != 3.19.5',
     'psutil',
     'pulp',
     # Ray job has an issue with pydantic>2.0.0, due to API changes of pydantic. See
     # https://github.com/ray-project/ray/issues/36990
-    'pydantic<2.0'
+    'pydantic<2.0',
+    # Cython 3.0 release breaks PyYAML installed by aws-cli.
+    # https://github.com/yaml/pyyaml/issues/601
+    # https://github.com/aws/aws-cli/issues/8036
+    'pyyaml<=5.3.1'
 ]
 
 # NOTE: Change the templates/spot-controller.yaml.j2 file if any of the
 # following packages dependencies are changed.
 aws_dependencies = [
     # NOTE: this installs CLI V1. To use AWS SSO (e.g., `aws sso login`), users
     # should instead use CLI V2 which is not pip-installable. See
```

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/__init__.py` & `skypilot-nightly-1.0.0.dev20230718/sky/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """The SkyPilot package."""
 import os
 
 # Replaced with the current commit when building the wheels.
-__commit__ = '3a8ae21556069e9585bbe9fa0b8fd6641eaf8b00'
-__version__ = '1.0.0-dev20230717'
+__commit__ = 'a184687490b6c596dc7b76a0ba9fc4728012f58c'
+__version__ = '1.0.0-dev20230718'
 __root_dir__ = os.path.dirname(os.path.abspath(__file__))
 
 # Keep this order to avoid cyclic imports
 from sky import backends
 from sky import benchmark
 from sky import clouds
 from sky.clouds.service_catalog import list_accelerators
```

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/adaptors/aws.py` & `skypilot-nightly-1.0.0.dev20230718/sky/adaptors/aws.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/adaptors/azure.py` & `skypilot-nightly-1.0.0.dev20230718/sky/adaptors/azure.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/adaptors/cloudflare.py` & `skypilot-nightly-1.0.0.dev20230718/sky/adaptors/cloudflare.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/adaptors/docker.py` & `skypilot-nightly-1.0.0.dev20230718/sky/adaptors/docker.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/adaptors/gcp.py` & `skypilot-nightly-1.0.0.dev20230718/sky/adaptors/gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/adaptors/ibm.py` & `skypilot-nightly-1.0.0.dev20230718/sky/adaptors/ibm.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/adaptors/oci.py` & `skypilot-nightly-1.0.0.dev20230718/sky/adaptors/oci.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/authentication.py` & `skypilot-nightly-1.0.0.dev20230718/sky/authentication.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/backends/backend.py` & `skypilot-nightly-1.0.0.dev20230718/sky/backends/backend.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/backends/backend_utils.py` & `skypilot-nightly-1.0.0.dev20230718/sky/backends/backend_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/backends/cloud_vm_ray_backend.py` & `skypilot-nightly-1.0.0.dev20230718/sky/backends/cloud_vm_ray_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import pathlib
 import re
 import signal
 import subprocess
 import sys
 import tempfile
 import textwrap
+import threading
 import time
 import typing
 from typing import Dict, Iterable, List, Optional, Tuple, Union, Set
 
 import colorama
 import filelock
 
@@ -3258,16 +3259,17 @@
                                                follow=follow)
         if job_id is None and spot_job_id is None:
             logger.info(
                 'Job ID not provided. Streaming the logs of the latest job.')
 
         # With the stdin=subprocess.DEVNULL, the ctrl-c will not directly
         # kill the process, so we need to handle it manually here.
-        signal.signal(signal.SIGINT, backend_utils.interrupt_handler)
-        signal.signal(signal.SIGTSTP, backend_utils.stop_handler)
+        if threading.current_thread() is threading.main_thread():
+            signal.signal(signal.SIGINT, backend_utils.interrupt_handler)
+            signal.signal(signal.SIGTSTP, backend_utils.stop_handler)
         try:
             returncode = self.run_on_head(
                 handle,
                 code,
                 stream_logs=True,
                 process_stream=False,
                 # Allocate a pseudo-terminal to disable output buffering.
@@ -3292,16 +3294,17 @@
         if job_name is not None:
             code = spot_lib.SpotCodeGen.stream_logs_by_name(job_name, follow)
         else:
             code = spot_lib.SpotCodeGen.stream_logs_by_id(job_id, follow)
 
         # With the stdin=subprocess.DEVNULL, the ctrl-c will not directly
         # kill the process, so we need to handle it manually here.
-        signal.signal(signal.SIGINT, backend_utils.interrupt_handler)
-        signal.signal(signal.SIGTSTP, backend_utils.stop_handler)
+        if threading.current_thread() is threading.main_thread():
+            signal.signal(signal.SIGINT, backend_utils.interrupt_handler)
+            signal.signal(signal.SIGTSTP, backend_utils.stop_handler)
 
         # Refer to the notes in tail_logs.
         self.run_on_head(
             handle,
             code,
             stream_logs=True,
             process_stream=False,
```

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/backends/docker_utils.py` & `skypilot-nightly-1.0.0.dev20230718/sky/backends/docker_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/backends/local_docker_backend.py` & `skypilot-nightly-1.0.0.dev20230718/sky/backends/local_docker_backend.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/backends/monkey_patches/monkey_patch_ray_up.py` & `skypilot-nightly-1.0.0.dev20230718/sky/backends/monkey_patches/monkey_patch_ray_up.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/backends/onprem_utils.py` & `skypilot-nightly-1.0.0.dev20230718/sky/backends/onprem_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/backends/wheel_utils.py` & `skypilot-nightly-1.0.0.dev20230718/sky/backends/wheel_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/benchmark/benchmark_state.py` & `skypilot-nightly-1.0.0.dev20230718/sky/benchmark/benchmark_state.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/benchmark/benchmark_utils.py` & `skypilot-nightly-1.0.0.dev20230718/sky/benchmark/benchmark_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/check.py` & `skypilot-nightly-1.0.0.dev20230718/sky/check.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/cli.py` & `skypilot-nightly-1.0.0.dev20230718/sky/cli.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/cloud_stores.py` & `skypilot-nightly-1.0.0.dev20230718/sky/cloud_stores.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/clouds/__init__.py` & `skypilot-nightly-1.0.0.dev20230718/sky/clouds/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/clouds/aws.py` & `skypilot-nightly-1.0.0.dev20230718/sky/clouds/aws.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/clouds/azure.py` & `skypilot-nightly-1.0.0.dev20230718/sky/clouds/azure.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/clouds/cloud.py` & `skypilot-nightly-1.0.0.dev20230718/sky/clouds/cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/clouds/gcp.py` & `skypilot-nightly-1.0.0.dev20230718/sky/clouds/gcp.py`

 * *Files 0% similar despite different names*

```diff
@@ -354,26 +354,29 @@
                 resources_vars['tpu_vm'] = r.accelerator_args.get('tpu_vm')
                 resources_vars['runtime_version'] = r.accelerator_args[
                     'runtime_version']
                 resources_vars['tpu_name'] = r.accelerator_args.get('tpu_name')
             else:
                 # Convert to GCP names:
                 # https://cloud.google.com/compute/docs/gpus
-                if acc == 'A100-80GB':
-                    # A100-80GB has a different name pattern.
+                if acc in ('A100-80GB', 'L4'):
+                    # A100-80GB and L4 have a different name pattern.
                     resources_vars['gpu'] = 'nvidia-{}'.format(acc.lower())
                 else:
                     resources_vars['gpu'] = 'nvidia-tesla-{}'.format(
                         acc.lower())
                 resources_vars['gpu_count'] = acc_count
                 if acc == 'K80':
                     # Though the image is called cu113, it actually has later
                     # versions of CUDA as noted below.
                     # CUDA driver version 470.57.02, CUDA Library 11.4
                     image_id = 'skypilot:k80-debian-10'
+                elif acc == 'L4':
+                    # CUDA driver version 525.105.17, CUDA Library 11.8
+                    image_id = 'skypilot:cuda118-debian-11'
                 else:
                     # Though the image is called cu113, it actually has later
                     # versions of CUDA as noted below.
                     # CUDA driver version 510.47.03, CUDA Library 11.6
                     # Does not support torch==1.13.0 with cu117
                     image_id = 'skypilot:gpu-debian-10'
```

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/clouds/ibm.py` & `skypilot-nightly-1.0.0.dev20230718/sky/clouds/ibm.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/clouds/lambda_cloud.py` & `skypilot-nightly-1.0.0.dev20230718/sky/clouds/lambda_cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/clouds/local.py` & `skypilot-nightly-1.0.0.dev20230718/sky/clouds/local.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/clouds/oci.py` & `skypilot-nightly-1.0.0.dev20230718/sky/clouds/oci.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/clouds/scp.py` & `skypilot-nightly-1.0.0.dev20230718/sky/clouds/scp.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/__init__.py` & `skypilot-nightly-1.0.0.dev20230718/sky/clouds/service_catalog/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -278,14 +278,15 @@
     """Returns a list of commonly used GPU names."""
     return [
         'A10',
         'A10G',
         'A100',
         'A100-80GB',
         'K80',
+        'L4',
         'M60',
         'P100',
         'T4',
         'V100',
         'V100-32GB',
     ]
```

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/aws_catalog.py` & `skypilot-nightly-1.0.0.dev20230718/sky/clouds/service_catalog/aws_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/azure_catalog.py` & `skypilot-nightly-1.0.0.dev20230718/sky/clouds/service_catalog/azure_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/common.py` & `skypilot-nightly-1.0.0.dev20230718/sky/clouds/service_catalog/common.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/config.py` & `skypilot-nightly-1.0.0.dev20230718/sky/clouds/service_catalog/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/data_fetchers/fetch_aws.py` & `skypilot-nightly-1.0.0.dev20230718/sky/clouds/service_catalog/data_fetchers/fetch_aws.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/data_fetchers/fetch_azure.py` & `skypilot-nightly-1.0.0.dev20230718/sky/clouds/service_catalog/data_fetchers/fetch_azure.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py` & `skypilot-nightly-1.0.0.dev20230718/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,24 +55,24 @@
         textwrap.dedent("""\
  InstanceType,AcceleratorName,AcceleratorCount,vCPUs,MemoryGiB,GpuInfo,Price,SpotPrice,Region,AvailabilityZone
  n1-highmem-8,,,8.0,52.0,,0.473212,0.099624,us-central2,us-central2-b
  """)))
 
 # TODO(woosuk): Make this more robust.
 # Refer to: https://github.com/skypilot-org/skypilot/issues/1006
-# G2 series has L4 GPU, which is not supported by SkyPilot yet
-# Unsupported Series: 'f1', 'm2', 'g2'
+# Unsupported Series: 'f1', 'm2'
 SERIES_TO_DISCRIPTION = {
     'a2': 'A2 Instance',
     'c2': 'Compute optimized',
     'c2d': 'C2D AMD Instance',
     'c3': 'C3 Instance',
     'e2': 'E2 Instance',
     'f1': 'Micro Instance with burstable CPU',
     'g1': 'Small Instance with 1 VCPU',
+    'g2': 'G2 Instance',
     'm1': 'Memory-optimized Instance',
     # FIXME(woosuk): Support M2 series.
     'm3': 'M3 Memory-optimized Instance',
     'n1': 'N1 Predefined Instance',
     'n2': 'N2 Instance',
     'n2d': 'N2D AMD Instance',
     't2a': 'T2A Arm Instance',
```

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py` & `skypilot-nightly-1.0.0.dev20230718/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/gcp_catalog.py` & `skypilot-nightly-1.0.0.dev20230718/sky/clouds/service_catalog/gcp_catalog.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,29 +54,45 @@
 # This can be switched between n1 and n2.
 # n2 is not allowed for launching GPUs.
 _DEFAULT_HOST_VM_FAMILY = 'n1'
 _DEFAULT_GPU_MEMORY_CPU_RATIO = 4
 
 # TODO(zongheng): fix A100 info directly in catalog.
 # https://cloud.google.com/blog/products/compute/a2-vms-with-nvidia-a100-gpus-are-ga
-# count -> vm type
-_A100_INSTANCE_TYPE_DICTS = {
+
+# If A100 is used, host VM type must be A2; if L4 is used, VM type must be G2.
+# Conversely, A2 can only be used with A100, and G2 only with L4.
+# https://cloud.google.com/compute/docs/gpus
+# acc_type -> count -> vm types
+_ACC_INSTANCE_TYPE_DICTS = {
     'A100': {
-        1: 'a2-highgpu-1g',
-        2: 'a2-highgpu-2g',
-        4: 'a2-highgpu-4g',
-        8: 'a2-highgpu-8g',
-        16: 'a2-megagpu-16g',
+        1: ['a2-highgpu-1g'],
+        2: ['a2-highgpu-2g'],
+        4: ['a2-highgpu-4g'],
+        8: ['a2-highgpu-8g'],
+        16: ['a2-megagpu-16g'],
     },
     'A100-80GB': {
-        1: 'a2-ultragpu-1g',
-        2: 'a2-ultragpu-2g',
-        4: 'a2-ultragpu-4g',
-        8: 'a2-ultragpu-8g',
-    }
+        1: ['a2-ultragpu-1g'],
+        2: ['a2-ultragpu-2g'],
+        4: ['a2-ultragpu-4g'],
+        8: ['a2-ultragpu-8g'],
+    },
+    'L4': {
+        1: [
+            'g2-standard-4',
+            'g2-standard-8',
+            'g2-standard-12',
+            'g2-standard-16',
+            'g2-standard-32',
+        ],
+        2: ['g2-standard-24'],
+        4: ['g2-standard-48'],
+        8: ['g2-standard-96'],
+    },
 }
 
 # Number of CPU cores per GPU based on the AWS setting.
 # GCP A100 has its own instance type mapping.
 # Refer to sky/clouds/service_catalog/gcp_catalog.py
 _NUM_ACC_TO_NUM_CPU = {
     # Based on p2 on AWS.
@@ -227,21 +243,18 @@
     """
     (instance_list,
      fuzzy_candidate_list) = common.get_instance_type_for_accelerator_impl(
          _df, acc_name, acc_count, cpus, memory, use_spot, region, zone)
     if instance_list is None:
         return None, fuzzy_candidate_list
 
-    if acc_name in _A100_INSTANCE_TYPE_DICTS:
-        # If A100 is used, host VM type must be A2.
-        # https://cloud.google.com/compute/docs/gpus#a100-gpus
-
+    if acc_name in _ACC_INSTANCE_TYPE_DICTS:
         df = _df[_df['InstanceType'].notna()]
-        instance_type = _A100_INSTANCE_TYPE_DICTS[acc_name][acc_count]
-        df = df[df['InstanceType'] == instance_type]
+        instance_types = _ACC_INSTANCE_TYPE_DICTS[acc_name][acc_count]
+        df = df[df['InstanceType'].isin(instance_types)]
 
         # Check the cpus and memory specified by the user.
         instance_type = common.get_instance_type_for_cpus_mem_impl(
             df, cpus, memory)
         if instance_type is None:
             return None, []
         return [instance_type], []
@@ -341,53 +354,56 @@
                                             case_sensitive)
 
     # Remove GPUs that are unsupported by SkyPilot.
     new_results = {}
     for acc_name, acc_info in results.items():
         if (acc_name.startswith('tpu') or
                 acc_name in _NUM_ACC_TO_MAX_CPU_AND_MEMORY or
-                acc_name in _A100_INSTANCE_TYPE_DICTS):
-            new_results[acc_name] = acc_info
+                acc_name in _ACC_INSTANCE_TYPE_DICTS):
             new_results[acc_name] = acc_info
     results = new_results
 
-    a100_infos = results.get('A100', []) + results.get('A100-80GB', [])
-    if not a100_infos:
-        return results
-
     # Unlike other GPUs that can be attached to different sizes of N1 VMs,
-    # A100 GPUs can only be attached to fixed-size A2 VMs.
+    # A100 GPUs can only be attached to fixed-size A2 VMs,
+    # and L4 GPUs can only be attached to G2 VMs.
     # Thus, we can show their exact cost including the host VM prices.
+
+    acc_infos: List[common.InstanceTypeInfo] = sum(
+        [results.get(a, []) for a in _ACC_INSTANCE_TYPE_DICTS], [])
+    if not acc_infos:
+        return results
+
     new_infos = defaultdict(list)
-    for info in a100_infos:
-        assert pd.isna(info.instance_type) and pd.isna(info.memory), a100_infos
-        a100_host_vm_type = _A100_INSTANCE_TYPE_DICTS[info.accelerator_name][
+    for info in acc_infos:
+        assert pd.isna(info.instance_type) and pd.isna(info.memory), acc_infos
+        vm_types = _ACC_INSTANCE_TYPE_DICTS[info.accelerator_name][
             info.accelerator_count]
-        df = _df[_df['InstanceType'] == a100_host_vm_type]
-        cpu_count = df['vCPUs'].iloc[0]
-        memory = df['MemoryGiB'].iloc[0]
-        vm_price = common.get_hourly_cost_impl(_df,
-                                               a100_host_vm_type,
-                                               use_spot=False,
-                                               region=None,
-                                               zone=None)
-        vm_spot_price = common.get_hourly_cost_impl(_df,
-                                                    a100_host_vm_type,
-                                                    use_spot=True,
-                                                    region=None,
-                                                    zone=None)
-        new_infos[info.accelerator_name].append(
-            info._replace(
-                instance_type=a100_host_vm_type,
-                cpu_count=cpu_count,
-                memory=memory,
-                # total cost = VM instance + GPU.
-                price=info.price + vm_price,
-                spot_price=info.spot_price + vm_spot_price,
-            ))
+        for vm_type in vm_types:
+            df = _df[_df['InstanceType'] == vm_type]
+            cpu_count = df['vCPUs'].iloc[0]
+            memory = df['MemoryGiB'].iloc[0]
+            vm_price = common.get_hourly_cost_impl(_df,
+                                                   vm_type,
+                                                   use_spot=False,
+                                                   region=None,
+                                                   zone=None)
+            vm_spot_price = common.get_hourly_cost_impl(_df,
+                                                        vm_type,
+                                                        use_spot=True,
+                                                        region=None,
+                                                        zone=None)
+            new_infos[info.accelerator_name].append(
+                info._replace(
+                    instance_type=vm_type,
+                    cpu_count=cpu_count,
+                    memory=memory,
+                    # total cost = VM instance + GPU.
+                    price=info.price + vm_price,
+                    spot_price=info.spot_price + vm_spot_price,
+                ))
     results.update(new_infos)
     return results
 
 
 def get_region_zones_for_accelerators(
     accelerator: str,
     count: int,
@@ -407,22 +423,23 @@
     the accelerators can be attached to.
 
     Raises:
         exceptions.ResourcesMismatchError: If the accelerators cannot be
             attached to the host.
     """
     if accelerators is None:
-        if instance_type.startswith('a2-'):
-            # NOTE: While it is allowed to use A2 machines as CPU-only nodes,
-            # we exclude this case as it is uncommon and undesirable.
-            with ux_utils.print_exception_no_traceback():
-                raise exceptions.ResourcesMismatchError(
-                    'A2 instance types should be used with A100 GPUs. '
-                    'Either use other instance types or specify the '
-                    'accelerators as A100.')
+        for acc_name, val in _ACC_INSTANCE_TYPE_DICTS.items():
+            if instance_type in sum(val.values(), []):
+                # NOTE: While it is allowed to use A2/G2 VMs as CPU-only nodes,
+                # we exclude this case as it is uncommon and undesirable.
+                with ux_utils.print_exception_no_traceback():
+                    raise exceptions.ResourcesMismatchError(
+                        f'{instance_type} instance types should be used with '
+                        f'{acc_name} GPUs. Either use other instance types or '
+                        f'specify the accelerators as {acc_name}.')
         return
 
     acc = list(accelerators.items())
     assert len(acc) == 1, acc
     acc_name, acc_count = acc[0]
 
     # Check if the accelerator is supported by GCP.
@@ -437,47 +454,45 @@
             with ux_utils.print_exception_no_traceback():
                 raise exceptions.ResourcesMismatchError(
                     'TPU Nodes can be only used with N1 machines. '
                     'Please refer to: '
                     'https://cloud.google.com/compute/docs/general-purpose-machines#n1_machines')  # pylint: disable=line-too-long
         return
 
-    # Treat A100 as a special case.
-    if acc_name in _A100_INSTANCE_TYPE_DICTS:
-        a100_instance_type = _A100_INSTANCE_TYPE_DICTS[acc_name][acc_count]
-        if instance_type != a100_instance_type:
+    if acc_name in _ACC_INSTANCE_TYPE_DICTS:
+        matching_types = _ACC_INSTANCE_TYPE_DICTS[acc_name][acc_count]
+        if instance_type not in matching_types:
             with ux_utils.print_exception_no_traceback():
                 raise exceptions.ResourcesMismatchError(
-                    f'A100:{acc_count} cannot be attached to {instance_type}. '
-                    f'Use {a100_instance_type} instead. Please refer to '
-                    'https://cloud.google.com/compute/docs/gpus#a100-gpus')
+                    f'{acc_name} GPUs cannot be attached to {instance_type}. '
+                    f'Use one of {matching_types} instead. Please refer to '
+                    'https://cloud.google.com/compute/docs/gpus')
     elif not instance_type.startswith('n1-'):
         # Other GPUs must be attached to N1 machines.
         # Refer to: https://cloud.google.com/compute/docs/machine-types#gpus
         with ux_utils.print_exception_no_traceback():
             raise exceptions.ResourcesMismatchError(
                 f'{acc_name} GPUs cannot be attached to {instance_type}. '
                 'Use N1 instance types instead. Please refer to: '
                 'https://cloud.google.com/compute/docs/machine-types#gpus')
 
-    if acc_name in _A100_INSTANCE_TYPE_DICTS:
-        valid_counts = list(_A100_INSTANCE_TYPE_DICTS[acc_name].keys())
+    if acc_name in _ACC_INSTANCE_TYPE_DICTS:
+        valid_counts = list(_ACC_INSTANCE_TYPE_DICTS[acc_name].keys())
     else:
         assert acc_name in _NUM_ACC_TO_MAX_CPU_AND_MEMORY, acc_name
         valid_counts = list(_NUM_ACC_TO_MAX_CPU_AND_MEMORY[acc_name].keys())
     if acc_count not in valid_counts:
         with ux_utils.print_exception_no_traceback():
             raise exceptions.ResourcesMismatchError(
                 f'{acc_name}:{acc_count} is not launchable on GCP. '
                 f'The valid {acc_name} counts are {valid_counts}.')
 
     # Check maximum vCPUs and memory.
-    if acc_name in _A100_INSTANCE_TYPE_DICTS:
-        max_cpus, max_memory = get_vcpus_mem_from_instance_type(
-            a100_instance_type)
+    if acc_name in _ACC_INSTANCE_TYPE_DICTS:
+        max_cpus, max_memory = get_vcpus_mem_from_instance_type(instance_type)
     else:
         max_cpus, max_memory = _NUM_ACC_TO_MAX_CPU_AND_MEMORY[acc_name][
             acc_count]
         if acc_name == 'K80' and acc_count == 8:
             if zone in ['asia-east1-a', 'us-east1-d']:
                 max_memory = 416
         elif acc_name == 'P100' and acc_count == 4:
```

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/ibm_catalog.py` & `skypilot-nightly-1.0.0.dev20230718/sky/clouds/service_catalog/ibm_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/lambda_catalog.py` & `skypilot-nightly-1.0.0.dev20230718/sky/clouds/service_catalog/lambda_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/oci_catalog.py` & `skypilot-nightly-1.0.0.dev20230718/sky/clouds/service_catalog/oci_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/scp_catalog.py` & `skypilot-nightly-1.0.0.dev20230718/sky/clouds/service_catalog/scp_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/core.py` & `skypilot-nightly-1.0.0.dev20230718/sky/core.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/dag.py` & `skypilot-nightly-1.0.0.dev20230718/sky/dag.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/data/data_transfer.py` & `skypilot-nightly-1.0.0.dev20230718/sky/data/data_transfer.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/data/data_utils.py` & `skypilot-nightly-1.0.0.dev20230718/sky/data/data_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/data/mounting_utils.py` & `skypilot-nightly-1.0.0.dev20230718/sky/data/mounting_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/data/storage.py` & `skypilot-nightly-1.0.0.dev20230718/sky/data/storage.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/data/storage_utils.py` & `skypilot-nightly-1.0.0.dev20230718/sky/data/storage_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/exceptions.py` & `skypilot-nightly-1.0.0.dev20230718/sky/exceptions.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/execution.py` & `skypilot-nightly-1.0.0.dev20230718/sky/execution.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/global_user_state.py` & `skypilot-nightly-1.0.0.dev20230718/sky/global_user_state.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/optimizer.py` & `skypilot-nightly-1.0.0.dev20230718/sky/optimizer.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/provision/__init__.py` & `skypilot-nightly-1.0.0.dev20230718/sky/provision/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/provision/aws/instance.py` & `skypilot-nightly-1.0.0.dev20230718/sky/provision/aws/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/provision/gcp/instance.py` & `skypilot-nightly-1.0.0.dev20230718/sky/provision/gcp/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/provision/gcp/instance_utils.py` & `skypilot-nightly-1.0.0.dev20230718/sky/provision/gcp/instance_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/resources.py` & `skypilot-nightly-1.0.0.dev20230718/sky/resources.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/setup_files/MANIFEST.in` & `skypilot-nightly-1.0.0.dev20230718/sky/setup_files/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/setup_files/setup.py` & `skypilot-nightly-1.0.0.dev20230718/sky/setup_files/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,15 +108,19 @@
     # Adopted from ray's setup.py:
     # https://github.com/ray-project/ray/blob/86fab1764e618215d8131e8e5068f0d493c77023/python/setup.py#L326
     'protobuf >= 3.15.3, != 3.19.5',
     'psutil',
     'pulp',
     # Ray job has an issue with pydantic>2.0.0, due to API changes of pydantic. See
     # https://github.com/ray-project/ray/issues/36990
-    'pydantic<2.0'
+    'pydantic<2.0',
+    # Cython 3.0 release breaks PyYAML installed by aws-cli.
+    # https://github.com/yaml/pyyaml/issues/601
+    # https://github.com/aws/aws-cli/issues/8036
+    'pyyaml<=5.3.1'
 ]
 
 # NOTE: Change the templates/spot-controller.yaml.j2 file if any of the
 # following packages dependencies are changed.
 aws_dependencies = [
     # NOTE: this installs CLI V1. To use AWS SSO (e.g., `aws sso login`), users
     # should instead use CLI V2 which is not pip-installable. See
```

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/sky_logging.py` & `skypilot-nightly-1.0.0.dev20230718/sky/sky_logging.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/skylet/LICENSE` & `skypilot-nightly-1.0.0.dev20230718/sky/skylet/LICENSE`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/skylet/attempt_skylet.py` & `skypilot-nightly-1.0.0.dev20230718/sky/skylet/attempt_skylet.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/skylet/autostop_lib.py` & `skypilot-nightly-1.0.0.dev20230718/sky/skylet/autostop_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/skylet/configs.py` & `skypilot-nightly-1.0.0.dev20230718/sky/skylet/configs.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/skylet/constants.py` & `skypilot-nightly-1.0.0.dev20230718/sky/skylet/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/skylet/events.py` & `skypilot-nightly-1.0.0.dev20230718/sky/skylet/events.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/skylet/job_lib.py` & `skypilot-nightly-1.0.0.dev20230718/sky/skylet/job_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/skylet/log_lib.py` & `skypilot-nightly-1.0.0.dev20230718/sky/skylet/log_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py` & `skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/aws/config.py` & `skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/aws/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/aws/node_provider.py` & `skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/aws/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/aws/utils.py` & `skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/aws/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/azure/azure-config-template.json` & `skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/azure/azure-config-template.json`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/azure/azure-vm-template.json` & `skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/azure/azure-vm-template.json`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/azure/config.py` & `skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/azure/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/azure/node_provider.py` & `skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/azure/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/gcp/config.py` & `skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/gcp/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/gcp/constants.py` & `skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/gcp/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/gcp/node.py` & `skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/gcp/node.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/gcp/node_provider.py` & `skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/gcp/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/ibm/node_provider.py` & `skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/ibm/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/ibm/utils.py` & `skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/ibm/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/ibm/vpc_provider.py` & `skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/ibm/vpc_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/lambda_cloud/lambda_utils.py` & `skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/lambda_cloud/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/lambda_cloud/node_provider.py` & `skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/lambda_cloud/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/oci/config.py` & `skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/oci/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/oci/node_provider.py` & `skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/oci/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/oci/query_helper.py` & `skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/oci/query_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/scp/config.py` & `skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/scp/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/scp/node_provider.py` & `skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/scp/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/scp/scp_utils.py` & `skypilot-nightly-1.0.0.dev20230718/sky/skylet/providers/scp/scp_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/skylet/ray_patches/__init__.py` & `skypilot-nightly-1.0.0.dev20230718/sky/skylet/ray_patches/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/skylet/ray_patches/log_monitor.py.patch` & `skypilot-nightly-1.0.0.dev20230718/sky/skylet/ray_patches/log_monitor.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/skylet/ray_patches/resource_demand_scheduler.py.patch` & `skypilot-nightly-1.0.0.dev20230718/sky/skylet/ray_patches/resource_demand_scheduler.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/skylet/ray_patches/worker.py.patch` & `skypilot-nightly-1.0.0.dev20230718/sky/skylet/ray_patches/worker.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/skylet/skylet.py` & `skypilot-nightly-1.0.0.dev20230718/sky/skylet/skylet.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/skylet/subprocess_daemon.py` & `skypilot-nightly-1.0.0.dev20230718/sky/skylet/subprocess_daemon.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/skypilot_config.py` & `skypilot-nightly-1.0.0.dev20230718/sky/skypilot_config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/spot/__init__.py` & `skypilot-nightly-1.0.0.dev20230718/sky/spot/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/spot/constants.py` & `skypilot-nightly-1.0.0.dev20230718/sky/spot/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/spot/controller.py` & `skypilot-nightly-1.0.0.dev20230718/sky/spot/controller.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/spot/dashboard/dashboard.py` & `skypilot-nightly-1.0.0.dev20230718/sky/spot/dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/spot/dashboard/static/favicon.ico` & `skypilot-nightly-1.0.0.dev20230718/sky/spot/dashboard/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/spot/dashboard/templates/index.html` & `skypilot-nightly-1.0.0.dev20230718/sky/spot/dashboard/templates/index.html`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/spot/recovery_strategy.py` & `skypilot-nightly-1.0.0.dev20230718/sky/spot/recovery_strategy.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/spot/spot_state.py` & `skypilot-nightly-1.0.0.dev20230718/sky/spot/spot_state.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/spot/spot_utils.py` & `skypilot-nightly-1.0.0.dev20230718/sky/spot/spot_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/status_lib.py` & `skypilot-nightly-1.0.0.dev20230718/sky/status_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/task.py` & `skypilot-nightly-1.0.0.dev20230718/sky/task.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/templates/aws-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230718/sky/templates/aws-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/templates/azure-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230718/sky/templates/azure-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/templates/gcp-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230718/sky/templates/gcp-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/templates/ibm-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230718/sky/templates/ibm-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/templates/lambda-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230718/sky/templates/lambda-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/templates/local-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230718/sky/templates/local-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/templates/oci-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230718/sky/templates/oci-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/templates/scp-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230718/sky/templates/scp-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/templates/spot-controller.yaml.j2` & `skypilot-nightly-1.0.0.dev20230718/sky/templates/spot-controller.yaml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/usage/constants.py` & `skypilot-nightly-1.0.0.dev20230718/sky/usage/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/usage/usage_lib.py` & `skypilot-nightly-1.0.0.dev20230718/sky/usage/usage_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/utils/accelerator_registry.py` & `skypilot-nightly-1.0.0.dev20230718/sky/utils/accelerator_registry.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/utils/cli_utils/status_utils.py` & `skypilot-nightly-1.0.0.dev20230718/sky/utils/cli_utils/status_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/utils/command_runner.py` & `skypilot-nightly-1.0.0.dev20230718/sky/utils/command_runner.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/utils/common_utils.py` & `skypilot-nightly-1.0.0.dev20230718/sky/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/utils/dag_utils.py` & `skypilot-nightly-1.0.0.dev20230718/sky/utils/dag_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/utils/db_utils.py` & `skypilot-nightly-1.0.0.dev20230718/sky/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/utils/env_options.py` & `skypilot-nightly-1.0.0.dev20230718/sky/utils/env_options.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/utils/log_utils.py` & `skypilot-nightly-1.0.0.dev20230718/sky/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/utils/schemas.py` & `skypilot-nightly-1.0.0.dev20230718/sky/utils/schemas.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/utils/subprocess_utils.py` & `skypilot-nightly-1.0.0.dev20230718/sky/utils/subprocess_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/utils/timeline.py` & `skypilot-nightly-1.0.0.dev20230718/sky/utils/timeline.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/utils/tpu_utils.py` & `skypilot-nightly-1.0.0.dev20230718/sky/utils/tpu_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/utils/ux_utils.py` & `skypilot-nightly-1.0.0.dev20230718/sky/utils/ux_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/sky/utils/validator.py` & `skypilot-nightly-1.0.0.dev20230718/sky/utils/validator.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/skypilot_nightly.egg-info/PKG-INFO` & `skypilot-nightly-1.0.0.dev20230718/skypilot_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skypilot-nightly
-Version: 1.0.0.dev20230717
+Version: 1.0.0.dev20230718
 Summary: SkyPilot: An intercloud broker for the clouds
 Author: SkyPilot Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/skypilot-org/skypilot
 Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: skypilot-nightly Version: 1.0.0.dev20230717
+Metadata-Version: 2.1 Name: skypilot-nightly Version: 1.0.0.dev20230718
 Summary: SkyPilot: An intercloud broker for the clouds Author: SkyPilot Team
 License: Apache 2.0 Project-URL: Homepage, https://github.com/skypilot-org/
 skypilot Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `skypilot-nightly-1.0.0.dev20230717/skypilot_nightly.egg-info/SOURCES.txt` & `skypilot-nightly-1.0.0.dev20230718/skypilot_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/skypilot_nightly.egg-info/requires.txt` & `skypilot-nightly-1.0.0.dev20230718/skypilot_nightly.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 tabulate
 filelock>=3.6.0
 packaging
 protobuf!=3.19.5,>=3.15.3
 psutil
 pulp
 pydantic<2.0
+pyyaml<=5.3.1
 awscli
 boto3
 pycryptodome==3.12.0
 
 [:python_version < "3.10" and sys_platform != "darwin"]
 grpcio!=1.48.0,<=1.51.3,>=1.32.0
```

### Comparing `skypilot-nightly-1.0.0.dev20230717/tests/test_cli.py` & `skypilot-nightly-1.0.0.dev20230718/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/tests/test_config.py` & `skypilot-nightly-1.0.0.dev20230718/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/tests/test_jobs.py` & `skypilot-nightly-1.0.0.dev20230718/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/tests/test_list_accelerators.py` & `skypilot-nightly-1.0.0.dev20230718/tests/test_list_accelerators.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/tests/test_onprem.py` & `skypilot-nightly-1.0.0.dev20230718/tests/test_onprem.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/tests/test_optimizer_dryruns.py` & `skypilot-nightly-1.0.0.dev20230718/tests/test_optimizer_dryruns.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/tests/test_optimizer_random_dag.py` & `skypilot-nightly-1.0.0.dev20230718/tests/test_optimizer_random_dag.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/tests/test_smoke.py` & `skypilot-nightly-1.0.0.dev20230718/tests/test_smoke.py`

 * *Files 0% similar despite different names*

```diff
@@ -6887,869 +6887,873 @@
 0001ae60: 5b69 7465 6d20 696e 206f 7574 2066 6f72  [item in out for
 0001ae70: 2069 7465 6d20 696e 2073 746f 7261 6765   item in storage
 0001ae80: 5f6f 626a 5f6e 616d 655d 290a 0a20 2020  _obj_name])..   
 0001ae90: 2020 2020 2023 2052 756e 2073 6b79 2073       # Run sky s
 0001aea0: 746f 7261 6765 2064 656c 6574 6520 616c  torage delete al
 0001aeb0: 6c20 746f 2064 656c 6574 6520 616c 6c20  l to delete all 
 0001aec0: 7374 6f72 6167 6520 6f62 6a65 6374 730a  storage objects.
-0001aed0: 2020 2020 2020 2020 7375 6270 726f 6365          subproce
-0001aee0: 7373 2e63 6865 636b 5f6f 7574 7075 7428  ss.check_output(
-0001aef0: 5b27 736b 7927 2c20 2773 746f 7261 6765  ['sky', 'storage
-0001af00: 272c 2027 6465 6c65 7465 272c 2027 2d61  ', 'delete', '-a
-0001af10: 275d 290a 0a20 2020 2020 2020 2023 2052  '])..        # R
-0001af20: 756e 2073 6b79 2073 746f 7261 6765 206c  un sky storage l
-0001af30: 7320 746f 2063 6865 636b 2069 6620 616c  s to check if al
-0001af40: 6c20 7374 6f72 6167 6520 6f62 6a65 6374  l storage object
-0001af50: 7320 6669 6c74 6572 6564 2062 7920 7374  s filtered by st
-0001af60: 6f72 650a 2020 2020 2020 2020 2320 7479  ore.        # ty
-0001af70: 7065 2061 7265 2064 656c 6574 6564 0a20  pe are deleted. 
-0001af80: 2020 2020 2020 206f 7574 5f61 6c6c 203d         out_all =
-0001af90: 2073 7562 7072 6f63 6573 732e 6368 6563   subprocess.chec
-0001afa0: 6b5f 6f75 7470 7574 285b 2773 6b79 272c  k_output(['sky',
-0001afb0: 2027 7374 6f72 6167 6527 2c20 276c 7327   'storage', 'ls'
-0001afc0: 5d29 0a20 2020 2020 2020 206f 7574 203d  ]).        out =
-0001afd0: 205b 0a20 2020 2020 2020 2020 2020 2069   [.            i
-0001afe0: 7465 6d2e 7370 6c69 7428 295b 305d 0a20  tem.split()[0]. 
-0001aff0: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-0001b000: 7465 6d20 696e 206f 7574 5f61 6c6c 2e64  tem in out_all.d
-0001b010: 6563 6f64 6528 2775 7466 2d38 2729 2e73  ecode('utf-8').s
-0001b020: 706c 6974 6c69 6e65 7328 290a 2020 2020  plitlines().    
-0001b030: 2020 2020 2020 2020 6966 2073 746f 7265          if store
-0001b040: 5f74 7970 652e 7661 6c75 6520 696e 2069  _type.value in i
-0001b050: 7465 6d0a 2020 2020 2020 2020 5d0a 2020  tem.        ].  
-0001b060: 2020 2020 2020 6173 7365 7274 2061 6c6c        assert all
-0001b070: 285b 6974 656d 206e 6f74 2069 6e20 6f75  ([item not in ou
-0001b080: 7420 666f 7220 6974 656d 2069 6e20 7374  t for item in st
-0001b090: 6f72 6167 655f 6f62 6a5f 6e61 6d65 5d29  orage_obj_name])
-0001b0a0: 0a0a 2020 2020 4070 7974 6573 742e 6d61  ..    @pytest.ma
-0001b0b0: 726b 2e70 6172 616d 6574 7269 7a65 2827  rk.parametrize('
-0001b0c0: 7374 6f72 655f 7479 7065 272c 205b 0a20  store_type', [. 
-0001b0d0: 2020 2020 2020 2073 746f 7261 6765 5f6c         storage_l
-0001b0e0: 6962 2e53 746f 7265 5479 7065 2e53 332c  ib.StoreType.S3,
-0001b0f0: 2073 746f 7261 6765 5f6c 6962 2e53 746f   storage_lib.Sto
-0001b100: 7265 5479 7065 2e47 4353 2c0a 2020 2020  reType.GCS,.    
-0001b110: 2020 2020 7079 7465 7374 2e70 6172 616d      pytest.param
-0001b120: 2873 746f 7261 6765 5f6c 6962 2e53 746f  (storage_lib.Sto
-0001b130: 7265 5479 7065 2e52 322c 206d 6172 6b73  reType.R2, marks
-0001b140: 3d70 7974 6573 742e 6d61 726b 2e63 6c6f  =pytest.mark.clo
-0001b150: 7564 666c 6172 6529 0a20 2020 205d 290a  udflare).    ]).
-0001b160: 2020 2020 6465 6620 7465 7374 5f62 7563      def test_buc
-0001b170: 6b65 745f 6578 7465 726e 616c 5f64 656c  ket_external_del
-0001b180: 6574 696f 6e28 7365 6c66 2c20 746d 705f  etion(self, tmp_
-0001b190: 7363 7261 7463 685f 7374 6f72 6167 655f  scratch_storage_
-0001b1a0: 6f62 6a2c 0a20 2020 2020 2020 2020 2020  obj,.           
-0001b1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b1c0: 2020 2020 2020 2020 2020 2073 746f 7265             store
-0001b1d0: 5f74 7970 6529 3a0a 2020 2020 2020 2020  _type):.        
-0001b1e0: 2320 4372 6561 7465 7320 6120 6275 636b  # Creates a buck
-0001b1f0: 6574 2c20 6465 6c65 7465 7320 6974 2065  et, deletes it e
-0001b200: 7874 6572 6e61 6c6c 7920 7573 696e 6720  xternally using 
-0001b210: 636c 6f75 6420 636c 6920 636f 6d6d 616e  cloud cli comman
-0001b220: 6473 0a20 2020 2020 2020 2023 2061 6e64  ds.        # and
-0001b230: 2074 6865 6e20 7472 6965 7320 746f 2064   then tries to d
-0001b240: 656c 6574 6520 6974 2075 7369 6e67 2073  elete it using s
-0001b250: 6b79 2073 746f 7261 6765 2064 656c 6574  ky storage delet
-0001b260: 652e 0a20 2020 2020 2020 2074 6d70 5f73  e..        tmp_s
-0001b270: 6372 6174 6368 5f73 746f 7261 6765 5f6f  cratch_storage_o
-0001b280: 626a 2e61 6464 5f73 746f 7265 2873 746f  bj.add_store(sto
-0001b290: 7265 5f74 7970 6529 0a0a 2020 2020 2020  re_type)..      
-0001b2a0: 2020 2320 5275 6e20 736b 7920 7374 6f72    # Run sky stor
-0001b2b0: 6167 6520 6c73 2074 6f20 6368 6563 6b20  age ls to check 
-0001b2c0: 6966 2073 746f 7261 6765 206f 626a 6563  if storage objec
-0001b2d0: 7420 6578 6973 7473 2069 6e20 7468 6520  t exists in the 
-0001b2e0: 6f75 7470 7574 0a20 2020 2020 2020 206f  output.        o
-0001b2f0: 7574 203d 2073 7562 7072 6f63 6573 732e  ut = subprocess.
-0001b300: 6368 6563 6b5f 6f75 7470 7574 285b 2773  check_output(['s
-0001b310: 6b79 272c 2027 7374 6f72 6167 6527 2c20  ky', 'storage', 
-0001b320: 276c 7327 5d29 0a20 2020 2020 2020 2061  'ls']).        a
-0001b330: 7373 6572 7420 746d 705f 7363 7261 7463  ssert tmp_scratc
-0001b340: 685f 7374 6f72 6167 655f 6f62 6a2e 6e61  h_storage_obj.na
-0001b350: 6d65 2069 6e20 6f75 742e 6465 636f 6465  me in out.decode
-0001b360: 2827 7574 662d 3827 290a 0a20 2020 2020  ('utf-8')..     
-0001b370: 2020 2023 2044 656c 6574 6520 6275 636b     # Delete buck
-0001b380: 6574 2065 7874 6572 6e61 6c6c 790a 2020  et externally.  
-0001b390: 2020 2020 2020 636d 6420 3d20 7365 6c66        cmd = self
-0001b3a0: 2e63 6c69 5f64 656c 6574 655f 636d 6428  .cli_delete_cmd(
-0001b3b0: 7374 6f72 655f 7479 7065 2c20 746d 705f  store_type, tmp_
-0001b3c0: 7363 7261 7463 685f 7374 6f72 6167 655f  scratch_storage_
-0001b3d0: 6f62 6a2e 6e61 6d65 290a 2020 2020 2020  obj.name).      
-0001b3e0: 2020 7375 6270 726f 6365 7373 2e63 6865    subprocess.che
-0001b3f0: 636b 5f6f 7574 7075 7428 636d 642c 2073  ck_output(cmd, s
-0001b400: 6865 6c6c 3d54 7275 6529 0a0a 2020 2020  hell=True)..    
-0001b410: 2020 2020 2320 5275 6e20 736b 7920 7374      # Run sky st
-0001b420: 6f72 6167 6520 6465 6c65 7465 2074 6f20  orage delete to 
-0001b430: 6465 6c65 7465 2074 6865 2073 746f 7261  delete the stora
-0001b440: 6765 206f 626a 6563 740a 2020 2020 2020  ge object.      
-0001b450: 2020 6f75 7420 3d20 7375 6270 726f 6365    out = subproce
-0001b460: 7373 2e63 6865 636b 5f6f 7574 7075 7428  ss.check_output(
-0001b470: 0a20 2020 2020 2020 2020 2020 205b 2773  .            ['s
-0001b480: 6b79 272c 2027 7374 6f72 6167 6527 2c20  ky', 'storage', 
-0001b490: 2764 656c 6574 6527 2c20 746d 705f 7363  'delete', tmp_sc
-0001b4a0: 7261 7463 685f 7374 6f72 6167 655f 6f62  ratch_storage_ob
-0001b4b0: 6a2e 6e61 6d65 5d29 0a20 2020 2020 2020  j.name]).       
-0001b4c0: 2023 204d 616b 6520 7375 7265 2062 7563   # Make sure buc
-0001b4d0: 6b65 7420 7761 7320 6e6f 7420 6372 6561  ket was not crea
-0001b4e0: 7465 6420 6475 7269 6e67 2064 656c 6574  ted during delet
-0001b4f0: 696f 6e20 2873 6565 2069 7373 7565 2023  ion (see issue #
-0001b500: 3133 3232 290a 2020 2020 2020 2020 6173  1322).        as
-0001b510: 7365 7274 2027 6372 6561 7465 6427 206e  sert 'created' n
-0001b520: 6f74 2069 6e20 6f75 742e 6465 636f 6465  ot in out.decode
-0001b530: 2827 7574 662d 3827 292e 6c6f 7765 7228  ('utf-8').lower(
-0001b540: 290a 0a20 2020 2020 2020 2023 2052 756e  )..        # Run
-0001b550: 2073 6b79 2073 746f 7261 6765 206c 7320   sky storage ls 
-0001b560: 746f 2063 6865 636b 2069 6620 7374 6f72  to check if stor
-0001b570: 6167 6520 6f62 6a65 6374 2069 7320 6465  age object is de
-0001b580: 6c65 7465 640a 2020 2020 2020 2020 6f75  leted.        ou
-0001b590: 7420 3d20 7375 6270 726f 6365 7373 2e63  t = subprocess.c
-0001b5a0: 6865 636b 5f6f 7574 7075 7428 5b27 736b  heck_output(['sk
-0001b5b0: 7927 2c20 2773 746f 7261 6765 272c 2027  y', 'storage', '
-0001b5c0: 6c73 275d 290a 2020 2020 2020 2020 6173  ls']).        as
-0001b5d0: 7365 7274 2074 6d70 5f73 6372 6174 6368  sert tmp_scratch
-0001b5e0: 5f73 746f 7261 6765 5f6f 626a 2e6e 616d  _storage_obj.nam
-0001b5f0: 6520 6e6f 7420 696e 206f 7574 2e64 6563  e not in out.dec
-0001b600: 6f64 6528 2775 7466 2d38 2729 0a0a 2020  ode('utf-8')..  
-0001b610: 2020 4070 7974 6573 742e 6d61 726b 2e70    @pytest.mark.p
-0001b620: 6172 616d 6574 7269 7a65 2827 7374 6f72  arametrize('stor
-0001b630: 655f 7479 7065 272c 205b 0a20 2020 2020  e_type', [.     
-0001b640: 2020 2073 746f 7261 6765 5f6c 6962 2e53     storage_lib.S
-0001b650: 746f 7265 5479 7065 2e53 332c 2073 746f  toreType.S3, sto
-0001b660: 7261 6765 5f6c 6962 2e53 746f 7265 5479  rage_lib.StoreTy
-0001b670: 7065 2e47 4353 2c0a 2020 2020 2020 2020  pe.GCS,.        
-0001b680: 7079 7465 7374 2e70 6172 616d 2873 746f  pytest.param(sto
-0001b690: 7261 6765 5f6c 6962 2e53 746f 7265 5479  rage_lib.StoreTy
-0001b6a0: 7065 2e52 322c 206d 6172 6b73 3d70 7974  pe.R2, marks=pyt
-0001b6b0: 6573 742e 6d61 726b 2e63 6c6f 7564 666c  est.mark.cloudfl
-0001b6c0: 6172 6529 0a20 2020 205d 290a 2020 2020  are).    ]).    
-0001b6d0: 6465 6620 7465 7374 5f62 7563 6b65 745f  def test_bucket_
-0001b6e0: 6275 6c6b 5f64 656c 6574 696f 6e28 7365  bulk_deletion(se
-0001b6f0: 6c66 2c20 7374 6f72 655f 7479 7065 2c20  lf, store_type, 
-0001b700: 746d 705f 6275 6c6b 5f64 656c 5f73 746f  tmp_bulk_del_sto
-0001b710: 7261 6765 5f6f 626a 293a 0a20 2020 2020  rage_obj):.     
-0001b720: 2020 2023 2043 7265 6174 6573 2061 2074     # Creates a t
-0001b730: 656d 7020 666f 6c64 6572 2077 6974 6820  emp folder with 
-0001b740: 6f76 6572 2032 3536 2066 696c 6573 2061  over 256 files a
-0001b750: 6e64 2066 6f6c 6465 7273 2c20 7570 6c6f  nd folders, uplo
-0001b760: 6164 0a20 2020 2020 2020 2023 2066 696c  ad.        # fil
-0001b770: 6573 2061 6e64 2066 6f6c 6465 7273 2074  es and folders t
-0001b780: 6f20 6120 6e65 7720 6275 636b 6574 2c20  o a new bucket, 
-0001b790: 7468 656e 2064 656c 6574 6520 6275 636b  then delete buck
-0001b7a0: 6574 2e0a 2020 2020 2020 2020 746d 705f  et..        tmp_
-0001b7b0: 6275 6c6b 5f64 656c 5f73 746f 7261 6765  bulk_del_storage
-0001b7c0: 5f6f 626a 2e61 6464 5f73 746f 7265 2873  _obj.add_store(s
-0001b7d0: 746f 7265 5f74 7970 6529 0a0a 2020 2020  tore_type)..    
-0001b7e0: 2020 2020 7375 6270 726f 6365 7373 2e63      subprocess.c
-0001b7f0: 6865 636b 5f6f 7574 7075 7428 0a20 2020  heck_output(.   
-0001b800: 2020 2020 2020 2020 205b 2773 6b79 272c           ['sky',
-0001b810: 2027 7374 6f72 6167 6527 2c20 2764 656c   'storage', 'del
-0001b820: 6574 6527 2c20 746d 705f 6275 6c6b 5f64  ete', tmp_bulk_d
-0001b830: 656c 5f73 746f 7261 6765 5f6f 626a 2e6e  el_storage_obj.n
-0001b840: 616d 655d 290a 0a20 2020 2020 2020 206f  ame])..        o
-0001b850: 7574 7075 7420 3d20 7375 6270 726f 6365  utput = subproce
-0001b860: 7373 2e63 6865 636b 5f6f 7574 7075 7428  ss.check_output(
-0001b870: 5b27 736b 7927 2c20 2773 746f 7261 6765  ['sky', 'storage
-0001b880: 272c 2027 6c73 275d 290a 2020 2020 2020  ', 'ls']).      
-0001b890: 2020 6173 7365 7274 2074 6d70 5f62 756c    assert tmp_bul
-0001b8a0: 6b5f 6465 6c5f 7374 6f72 6167 655f 6f62  k_del_storage_ob
-0001b8b0: 6a2e 6e61 6d65 206e 6f74 2069 6e20 6f75  j.name not in ou
-0001b8c0: 7470 7574 2e64 6563 6f64 6528 2775 7466  tput.decode('utf
-0001b8d0: 2d38 2729 0a0a 2020 2020 4070 7974 6573  -8')..    @pytes
-0001b8e0: 742e 6d61 726b 2e70 6172 616d 6574 7269  t.mark.parametri
-0001b8f0: 7a65 280a 2020 2020 2020 2020 2774 6d70  ze(.        'tmp
-0001b900: 5f70 7562 6c69 635f 7374 6f72 6167 655f  _public_storage_
-0001b910: 6f62 6a2c 2073 746f 7265 5f74 7970 6527  obj, store_type'
-0001b920: 2c0a 2020 2020 2020 2020 5b28 2773 333a  ,.        [('s3:
-0001b930: 2f2f 7463 6761 2d32 2d6f 7065 6e27 2c20  //tcga-2-open', 
-0001b940: 7374 6f72 6167 655f 6c69 622e 5374 6f72  storage_lib.Stor
-0001b950: 6554 7970 652e 5333 292c 0a20 2020 2020  eType.S3),.     
-0001b960: 2020 2020 2827 7333 3a2f 2f64 6967 6974      ('s3://digit
-0001b970: 616c 636f 7270 6f72 6127 2c20 7374 6f72  alcorpora', stor
-0001b980: 6167 655f 6c69 622e 5374 6f72 6554 7970  age_lib.StoreTyp
-0001b990: 652e 5333 292c 0a20 2020 2020 2020 2020  e.S3),.         
-0001b9a0: 2827 6773 3a2f 2f67 6370 2d70 7562 6c69  ('gs://gcp-publi
-0001b9b0: 632d 6461 7461 2d73 656e 7469 6e65 6c2d  c-data-sentinel-
-0001b9c0: 3227 2c20 7374 6f72 6167 655f 6c69 622e  2', storage_lib.
-0001b9d0: 5374 6f72 6554 7970 652e 4743 5329 5d2c  StoreType.GCS)],
-0001b9e0: 0a20 2020 2020 2020 2069 6e64 6972 6563  .        indirec
-0001b9f0: 743d 5b27 746d 705f 7075 626c 6963 5f73  t=['tmp_public_s
-0001ba00: 746f 7261 6765 5f6f 626a 275d 290a 2020  torage_obj']).  
-0001ba10: 2020 6465 6620 7465 7374 5f70 7562 6c69    def test_publi
-0001ba20: 635f 6275 636b 6574 2873 656c 662c 2074  c_bucket(self, t
-0001ba30: 6d70 5f70 7562 6c69 635f 7374 6f72 6167  mp_public_storag
-0001ba40: 655f 6f62 6a2c 2073 746f 7265 5f74 7970  e_obj, store_typ
-0001ba50: 6529 3a0a 2020 2020 2020 2020 2320 4372  e):.        # Cr
-0001ba60: 6561 7465 7320 6120 6e65 7720 6275 636b  eates a new buck
-0001ba70: 6574 2077 6974 6820 6120 7075 626c 6963  et with a public
-0001ba80: 2073 6f75 7263 6520 616e 6420 7665 7269   source and veri
-0001ba90: 6669 6573 2074 6861 7420 6974 2069 7320  fies that it is 
-0001baa0: 6e6f 740a 2020 2020 2020 2020 2320 6164  not.        # ad
-0001bab0: 6465 6420 746f 2067 6c6f 6261 6c5f 7573  ded to global_us
-0001bac0: 6572 5f73 7461 7465 2e0a 2020 2020 2020  er_state..      
-0001bad0: 2020 746d 705f 7075 626c 6963 5f73 746f    tmp_public_sto
-0001bae0: 7261 6765 5f6f 626a 2e61 6464 5f73 746f  rage_obj.add_sto
-0001baf0: 7265 2873 746f 7265 5f74 7970 6529 0a0a  re(store_type)..
-0001bb00: 2020 2020 2020 2020 2320 5275 6e20 736b          # Run sk
-0001bb10: 7920 7374 6f72 6167 6520 6c73 2074 6f20  y storage ls to 
-0001bb20: 6368 6563 6b20 6966 2073 746f 7261 6765  check if storage
-0001bb30: 206f 626a 6563 7420 6578 6973 7473 2069   object exists i
-0001bb40: 6e20 7468 6520 6f75 7470 7574 0a20 2020  n the output.   
-0001bb50: 2020 2020 206f 7574 203d 2073 7562 7072       out = subpr
-0001bb60: 6f63 6573 732e 6368 6563 6b5f 6f75 7470  ocess.check_outp
-0001bb70: 7574 285b 2773 6b79 272c 2027 7374 6f72  ut(['sky', 'stor
-0001bb80: 6167 6527 2c20 276c 7327 5d29 0a20 2020  age', 'ls']).   
-0001bb90: 2020 2020 2061 7373 6572 7420 746d 705f       assert tmp_
-0001bba0: 7075 626c 6963 5f73 746f 7261 6765 5f6f  public_storage_o
-0001bbb0: 626a 2e6e 616d 6520 6e6f 7420 696e 206f  bj.name not in o
-0001bbc0: 7574 2e64 6563 6f64 6528 2775 7466 2d38  ut.decode('utf-8
-0001bbd0: 2729 0a0a 2020 2020 4070 7974 6573 742e  ')..    @pytest.
-0001bbe0: 6d61 726b 2e70 6172 616d 6574 7269 7a65  mark.parametrize
-0001bbf0: 2827 6e6f 6e65 7869 7374 5f62 7563 6b65  ('nonexist_bucke
-0001bc00: 745f 7572 6c27 2c20 5b0a 2020 2020 2020  t_url', [.      
-0001bc10: 2020 2773 333a 2f2f 7b72 616e 646f 6d5f    's3://{random_
-0001bc20: 6e61 6d65 7d27 2c20 2767 733a 2f2f 7b72  name}', 'gs://{r
-0001bc30: 616e 646f 6d5f 6e61 6d65 7d27 2c0a 2020  andom_name}',.  
-0001bc40: 2020 2020 2020 7079 7465 7374 2e70 6172        pytest.par
-0001bc50: 616d 2827 7232 3a2f 2f7b 7261 6e64 6f6d  am('r2://{random
-0001bc60: 5f6e 616d 657d 272c 206d 6172 6b73 3d70  _name}', marks=p
-0001bc70: 7974 6573 742e 6d61 726b 2e63 6c6f 7564  ytest.mark.cloud
-0001bc80: 666c 6172 6529 0a20 2020 205d 290a 2020  flare).    ]).  
-0001bc90: 2020 6465 6620 7465 7374 5f6e 6f6e 6578    def test_nonex
-0001bca0: 6973 7465 6e74 5f62 7563 6b65 7428 7365  istent_bucket(se
-0001bcb0: 6c66 2c20 6e6f 6e65 7869 7374 5f62 7563  lf, nonexist_buc
-0001bcc0: 6b65 745f 7572 6c29 3a0a 2020 2020 2020  ket_url):.      
-0001bcd0: 2020 2320 4174 7465 6d70 7473 2074 6f20    # Attempts to 
-0001bce0: 6372 6561 7465 2066 6574 6368 2061 2073  create fetch a s
-0001bcf0: 7472 6f61 6765 2077 6974 6820 6120 6e6f  troage with a no
-0001bd00: 6e2d 6578 6973 7465 6e74 2073 6f75 7263  n-existent sourc
-0001bd10: 652e 0a20 2020 2020 2020 2023 2047 656e  e..        # Gen
-0001bd20: 6572 6174 6520 6120 7261 6e64 6f6d 2062  erate a random b
-0001bd30: 7563 6b65 7420 6e61 6d65 2061 6e64 2076  ucket name and v
-0001bd40: 6572 6966 7920 6974 2064 6f65 736e 2774  erify it doesn't
-0001bd50: 2065 7869 7374 3a0a 2020 2020 2020 2020   exist:.        
-0001bd60: 7265 7472 795f 636f 756e 7420 3d20 300a  retry_count = 0.
-0001bd70: 2020 2020 2020 2020 7768 696c 6520 5472          while Tr
-0001bd80: 7565 3a0a 2020 2020 2020 2020 2020 2020  ue:.            
-0001bd90: 6e6f 6e65 7869 7374 5f62 7563 6b65 745f  nonexist_bucket_
-0001bda0: 6e61 6d65 203d 2073 7472 2875 7569 642e  name = str(uuid.
-0001bdb0: 7575 6964 3428 2929 0a20 2020 2020 2020  uuid4()).       
-0001bdc0: 2020 2020 2069 6620 6e6f 6e65 7869 7374       if nonexist
-0001bdd0: 5f62 7563 6b65 745f 7572 6c2e 7374 6172  _bucket_url.star
-0001bde0: 7473 7769 7468 2827 7333 2729 3a0a 2020  tswith('s3'):.  
-0001bdf0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-0001be00: 6d6d 616e 6420 3d20 6627 6177 7320 7333  mmand = f'aws s3
-0001be10: 6170 6920 6865 6164 2d62 7563 6b65 7420  api head-bucket 
-0001be20: 2d2d 6275 636b 6574 207b 6e6f 6e65 7869  --bucket {nonexi
-0001be30: 7374 5f62 7563 6b65 745f 6e61 6d65 7d27  st_bucket_name}'
-0001be40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001be50: 2065 7870 6563 7465 645f 6f75 7470 7574   expected_output
-0001be60: 203d 2027 3430 3427 0a20 2020 2020 2020   = '404'.       
-0001be70: 2020 2020 2065 6c69 6620 6e6f 6e65 7869       elif nonexi
-0001be80: 7374 5f62 7563 6b65 745f 7572 6c2e 7374  st_bucket_url.st
-0001be90: 6172 7473 7769 7468 2827 6773 2729 3a0a  artswith('gs'):.
-0001bea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001beb0: 636f 6d6d 616e 6420 3d20 6627 6773 7574  command = f'gsut
-0001bec0: 696c 206c 7320 7b6e 6f6e 6578 6973 745f  il ls {nonexist_
-0001bed0: 6275 636b 6574 5f75 726c 2e66 6f72 6d61  bucket_url.forma
-0001bee0: 7428 7261 6e64 6f6d 5f6e 616d 653d 6e6f  t(random_name=no
-0001bef0: 6e65 7869 7374 5f62 7563 6b65 745f 6e61  nexist_bucket_na
-0001bf00: 6d65 297d 270a 2020 2020 2020 2020 2020  me)}'.          
-0001bf10: 2020 2020 2020 6578 7065 6374 6564 5f6f        expected_o
-0001bf20: 7574 7075 7420 3d20 2742 7563 6b65 744e  utput = 'BucketN
-0001bf30: 6f74 466f 756e 6445 7863 6570 7469 6f6e  otFoundException
-0001bf40: 270a 2020 2020 2020 2020 2020 2020 656c  '.            el
-0001bf50: 6966 206e 6f6e 6578 6973 745f 6275 636b  if nonexist_buck
-0001bf60: 6574 5f75 726c 2e73 7461 7274 7377 6974  et_url.startswit
-0001bf70: 6828 2772 3227 293a 0a20 2020 2020 2020  h('r2'):.       
-0001bf80: 2020 2020 2020 2020 2065 6e64 706f 696e           endpoin
-0001bf90: 745f 7572 6c20 3d20 636c 6f75 6466 6c61  t_url = cloudfla
-0001bfa0: 7265 2e63 7265 6174 655f 656e 6470 6f69  re.create_endpoi
-0001bfb0: 6e74 2829 0a20 2020 2020 2020 2020 2020  nt().           
-0001bfc0: 2020 2020 2063 6f6d 6d61 6e64 203d 2066       command = f
-0001bfd0: 2741 5753 5f53 4841 5245 445f 4352 4544  'AWS_SHARED_CRED
-0001bfe0: 454e 5449 414c 535f 4649 4c45 3d7b 636c  ENTIALS_FILE={cl
-0001bff0: 6f75 6466 6c61 7265 2e52 325f 4352 4544  oudflare.R2_CRED
-0001c000: 454e 5449 414c 535f 5041 5448 7d20 6177  ENTIALS_PATH} aw
-0001c010: 7320 7333 6170 6920 6865 6164 2d62 7563  s s3api head-buc
-0001c020: 6b65 7420 2d2d 6275 636b 6574 207b 6e6f  ket --bucket {no
-0001c030: 6e65 7869 7374 5f62 7563 6b65 745f 6e61  nexist_bucket_na
-0001c040: 6d65 7d20 2d2d 656e 6470 6f69 6e74 207b  me} --endpoint {
-0001c050: 656e 6470 6f69 6e74 5f75 726c 7d20 2d2d  endpoint_url} --
-0001c060: 7072 6f66 696c 653d 7232 270a 2020 2020  profile=r2'.    
-0001c070: 2020 2020 2020 2020 2020 2020 6578 7065              expe
-0001c080: 6374 6564 5f6f 7574 7075 7420 3d20 2734  cted_output = '4
-0001c090: 3034 270a 2020 2020 2020 2020 2020 2020  04'.            
-0001c0a0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0001c0b0: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-0001c0c0: 6545 7272 6f72 2827 556e 7375 7070 6f72  eError('Unsuppor
-0001c0d0: 7465 6420 6275 636b 6574 2074 7970 6520  ted bucket type 
-0001c0e0: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
-0001c0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c100: 2020 2066 277b 6e6f 6e65 7869 7374 5f62     f'{nonexist_b
-0001c110: 7563 6b65 745f 7572 6c7d 2729 0a0a 2020  ucket_url}')..  
-0001c120: 2020 2020 2020 2020 2020 2320 4368 6563            # Chec
-0001c130: 6b20 6966 2062 7563 6b65 7420 6578 6973  k if bucket exis
-0001c140: 7473 2075 7369 6e67 2074 6865 2063 6c69  ts using the cli
-0001c150: 3a0a 2020 2020 2020 2020 2020 2020 7472  :.            tr
-0001c160: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
-0001c170: 2020 206f 7574 203d 2073 7562 7072 6f63     out = subproc
-0001c180: 6573 732e 6368 6563 6b5f 6f75 7470 7574  ess.check_output
-0001c190: 2863 6f6d 6d61 6e64 2c0a 2020 2020 2020  (command,.      
-0001c1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c1c0: 2020 2020 2020 2020 7374 6465 7272 3d73          stderr=s
-0001c1d0: 7562 7072 6f63 6573 732e 5354 444f 5554  ubprocess.STDOUT
-0001c1e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001aed0: 2020 2020 2020 2020 6465 6c65 7465 5f63          delete_c
+0001aee0: 6d64 203d 205b 2773 6b79 272c 2027 7374  md = ['sky', 'st
+0001aef0: 6f72 6167 6527 2c20 2764 656c 6574 6527  orage', 'delete'
+0001af00: 5d0a 2020 2020 2020 2020 6465 6c65 7465  ].        delete
+0001af10: 5f63 6d64 202b 3d20 7374 6f72 6167 655f  _cmd += storage_
+0001af20: 6f62 6a5f 6e61 6d65 0a20 2020 2020 2020  obj_name.       
+0001af30: 2073 7562 7072 6f63 6573 732e 6368 6563   subprocess.chec
+0001af40: 6b5f 6f75 7470 7574 2864 656c 6574 655f  k_output(delete_
+0001af50: 636d 6429 0a0a 2020 2020 2020 2020 2320  cmd)..        # 
+0001af60: 5275 6e20 736b 7920 7374 6f72 6167 6520  Run sky storage 
+0001af70: 6c73 2074 6f20 6368 6563 6b20 6966 2061  ls to check if a
+0001af80: 6c6c 2073 746f 7261 6765 206f 626a 6563  ll storage objec
+0001af90: 7473 2066 696c 7465 7265 6420 6279 2073  ts filtered by s
+0001afa0: 746f 7265 0a20 2020 2020 2020 2023 2074  tore.        # t
+0001afb0: 7970 6520 6172 6520 6465 6c65 7465 640a  ype are deleted.
+0001afc0: 2020 2020 2020 2020 6f75 745f 616c 6c20          out_all 
+0001afd0: 3d20 7375 6270 726f 6365 7373 2e63 6865  = subprocess.che
+0001afe0: 636b 5f6f 7574 7075 7428 5b27 736b 7927  ck_output(['sky'
+0001aff0: 2c20 2773 746f 7261 6765 272c 2027 6c73  , 'storage', 'ls
+0001b000: 275d 290a 2020 2020 2020 2020 6f75 7420  ']).        out 
+0001b010: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
+0001b020: 6974 656d 2e73 706c 6974 2829 5b30 5d0a  item.split()[0].
+0001b030: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0001b040: 6974 656d 2069 6e20 6f75 745f 616c 6c2e  item in out_all.
+0001b050: 6465 636f 6465 2827 7574 662d 3827 292e  decode('utf-8').
+0001b060: 7370 6c69 746c 696e 6573 2829 0a20 2020  splitlines().   
+0001b070: 2020 2020 2020 2020 2069 6620 7374 6f72           if stor
+0001b080: 655f 7479 7065 2e76 616c 7565 2069 6e20  e_type.value in 
+0001b090: 6974 656d 0a20 2020 2020 2020 205d 0a20  item.        ]. 
+0001b0a0: 2020 2020 2020 2061 7373 6572 7420 616c         assert al
+0001b0b0: 6c28 5b69 7465 6d20 6e6f 7420 696e 206f  l([item not in o
+0001b0c0: 7574 2066 6f72 2069 7465 6d20 696e 2073  ut for item in s
+0001b0d0: 746f 7261 6765 5f6f 626a 5f6e 616d 655d  torage_obj_name]
+0001b0e0: 290a 0a20 2020 2040 7079 7465 7374 2e6d  )..    @pytest.m
+0001b0f0: 6172 6b2e 7061 7261 6d65 7472 697a 6528  ark.parametrize(
+0001b100: 2773 746f 7265 5f74 7970 6527 2c20 5b0a  'store_type', [.
+0001b110: 2020 2020 2020 2020 7374 6f72 6167 655f          storage_
+0001b120: 6c69 622e 5374 6f72 6554 7970 652e 5333  lib.StoreType.S3
+0001b130: 2c20 7374 6f72 6167 655f 6c69 622e 5374  , storage_lib.St
+0001b140: 6f72 6554 7970 652e 4743 532c 0a20 2020  oreType.GCS,.   
+0001b150: 2020 2020 2070 7974 6573 742e 7061 7261       pytest.para
+0001b160: 6d28 7374 6f72 6167 655f 6c69 622e 5374  m(storage_lib.St
+0001b170: 6f72 6554 7970 652e 5232 2c20 6d61 726b  oreType.R2, mark
+0001b180: 733d 7079 7465 7374 2e6d 6172 6b2e 636c  s=pytest.mark.cl
+0001b190: 6f75 6466 6c61 7265 290a 2020 2020 5d29  oudflare).    ])
+0001b1a0: 0a20 2020 2064 6566 2074 6573 745f 6275  .    def test_bu
+0001b1b0: 636b 6574 5f65 7874 6572 6e61 6c5f 6465  cket_external_de
+0001b1c0: 6c65 7469 6f6e 2873 656c 662c 2074 6d70  letion(self, tmp
+0001b1d0: 5f73 6372 6174 6368 5f73 746f 7261 6765  _scratch_storage
+0001b1e0: 5f6f 626a 2c0a 2020 2020 2020 2020 2020  _obj,.          
+0001b1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b200: 2020 2020 2020 2020 2020 2020 7374 6f72              stor
+0001b210: 655f 7479 7065 293a 0a20 2020 2020 2020  e_type):.       
+0001b220: 2023 2043 7265 6174 6573 2061 2062 7563   # Creates a buc
+0001b230: 6b65 742c 2064 656c 6574 6573 2069 7420  ket, deletes it 
+0001b240: 6578 7465 726e 616c 6c79 2075 7369 6e67  externally using
+0001b250: 2063 6c6f 7564 2063 6c69 2063 6f6d 6d61   cloud cli comma
+0001b260: 6e64 730a 2020 2020 2020 2020 2320 616e  nds.        # an
+0001b270: 6420 7468 656e 2074 7269 6573 2074 6f20  d then tries to 
+0001b280: 6465 6c65 7465 2069 7420 7573 696e 6720  delete it using 
+0001b290: 736b 7920 7374 6f72 6167 6520 6465 6c65  sky storage dele
+0001b2a0: 7465 2e0a 2020 2020 2020 2020 746d 705f  te..        tmp_
+0001b2b0: 7363 7261 7463 685f 7374 6f72 6167 655f  scratch_storage_
+0001b2c0: 6f62 6a2e 6164 645f 7374 6f72 6528 7374  obj.add_store(st
+0001b2d0: 6f72 655f 7479 7065 290a 0a20 2020 2020  ore_type)..     
+0001b2e0: 2020 2023 2052 756e 2073 6b79 2073 746f     # Run sky sto
+0001b2f0: 7261 6765 206c 7320 746f 2063 6865 636b  rage ls to check
+0001b300: 2069 6620 7374 6f72 6167 6520 6f62 6a65   if storage obje
+0001b310: 6374 2065 7869 7374 7320 696e 2074 6865  ct exists in the
+0001b320: 206f 7574 7075 740a 2020 2020 2020 2020   output.        
+0001b330: 6f75 7420 3d20 7375 6270 726f 6365 7373  out = subprocess
+0001b340: 2e63 6865 636b 5f6f 7574 7075 7428 5b27  .check_output(['
+0001b350: 736b 7927 2c20 2773 746f 7261 6765 272c  sky', 'storage',
+0001b360: 2027 6c73 275d 290a 2020 2020 2020 2020   'ls']).        
+0001b370: 6173 7365 7274 2074 6d70 5f73 6372 6174  assert tmp_scrat
+0001b380: 6368 5f73 746f 7261 6765 5f6f 626a 2e6e  ch_storage_obj.n
+0001b390: 616d 6520 696e 206f 7574 2e64 6563 6f64  ame in out.decod
+0001b3a0: 6528 2775 7466 2d38 2729 0a0a 2020 2020  e('utf-8')..    
+0001b3b0: 2020 2020 2320 4465 6c65 7465 2062 7563      # Delete buc
+0001b3c0: 6b65 7420 6578 7465 726e 616c 6c79 0a20  ket externally. 
+0001b3d0: 2020 2020 2020 2063 6d64 203d 2073 656c         cmd = sel
+0001b3e0: 662e 636c 695f 6465 6c65 7465 5f63 6d64  f.cli_delete_cmd
+0001b3f0: 2873 746f 7265 5f74 7970 652c 2074 6d70  (store_type, tmp
+0001b400: 5f73 6372 6174 6368 5f73 746f 7261 6765  _scratch_storage
+0001b410: 5f6f 626a 2e6e 616d 6529 0a20 2020 2020  _obj.name).     
+0001b420: 2020 2073 7562 7072 6f63 6573 732e 6368     subprocess.ch
+0001b430: 6563 6b5f 6f75 7470 7574 2863 6d64 2c20  eck_output(cmd, 
+0001b440: 7368 656c 6c3d 5472 7565 290a 0a20 2020  shell=True)..   
+0001b450: 2020 2020 2023 2052 756e 2073 6b79 2073       # Run sky s
+0001b460: 746f 7261 6765 2064 656c 6574 6520 746f  torage delete to
+0001b470: 2064 656c 6574 6520 7468 6520 7374 6f72   delete the stor
+0001b480: 6167 6520 6f62 6a65 6374 0a20 2020 2020  age object.     
+0001b490: 2020 206f 7574 203d 2073 7562 7072 6f63     out = subproc
+0001b4a0: 6573 732e 6368 6563 6b5f 6f75 7470 7574  ess.check_output
+0001b4b0: 280a 2020 2020 2020 2020 2020 2020 5b27  (.            ['
+0001b4c0: 736b 7927 2c20 2773 746f 7261 6765 272c  sky', 'storage',
+0001b4d0: 2027 6465 6c65 7465 272c 2074 6d70 5f73   'delete', tmp_s
+0001b4e0: 6372 6174 6368 5f73 746f 7261 6765 5f6f  cratch_storage_o
+0001b4f0: 626a 2e6e 616d 655d 290a 2020 2020 2020  bj.name]).      
+0001b500: 2020 2320 4d61 6b65 2073 7572 6520 6275    # Make sure bu
+0001b510: 636b 6574 2077 6173 206e 6f74 2063 7265  cket was not cre
+0001b520: 6174 6564 2064 7572 696e 6720 6465 6c65  ated during dele
+0001b530: 7469 6f6e 2028 7365 6520 6973 7375 6520  tion (see issue 
+0001b540: 2331 3332 3229 0a20 2020 2020 2020 2061  #1322).        a
+0001b550: 7373 6572 7420 2763 7265 6174 6564 2720  ssert 'created' 
+0001b560: 6e6f 7420 696e 206f 7574 2e64 6563 6f64  not in out.decod
+0001b570: 6528 2775 7466 2d38 2729 2e6c 6f77 6572  e('utf-8').lower
+0001b580: 2829 0a0a 2020 2020 2020 2020 2320 5275  ()..        # Ru
+0001b590: 6e20 736b 7920 7374 6f72 6167 6520 6c73  n sky storage ls
+0001b5a0: 2074 6f20 6368 6563 6b20 6966 2073 746f   to check if sto
+0001b5b0: 7261 6765 206f 626a 6563 7420 6973 2064  rage object is d
+0001b5c0: 656c 6574 6564 0a20 2020 2020 2020 206f  eleted.        o
+0001b5d0: 7574 203d 2073 7562 7072 6f63 6573 732e  ut = subprocess.
+0001b5e0: 6368 6563 6b5f 6f75 7470 7574 285b 2773  check_output(['s
+0001b5f0: 6b79 272c 2027 7374 6f72 6167 6527 2c20  ky', 'storage', 
+0001b600: 276c 7327 5d29 0a20 2020 2020 2020 2061  'ls']).        a
+0001b610: 7373 6572 7420 746d 705f 7363 7261 7463  ssert tmp_scratc
+0001b620: 685f 7374 6f72 6167 655f 6f62 6a2e 6e61  h_storage_obj.na
+0001b630: 6d65 206e 6f74 2069 6e20 6f75 742e 6465  me not in out.de
+0001b640: 636f 6465 2827 7574 662d 3827 290a 0a20  code('utf-8').. 
+0001b650: 2020 2040 7079 7465 7374 2e6d 6172 6b2e     @pytest.mark.
+0001b660: 7061 7261 6d65 7472 697a 6528 2773 746f  parametrize('sto
+0001b670: 7265 5f74 7970 6527 2c20 5b0a 2020 2020  re_type', [.    
+0001b680: 2020 2020 7374 6f72 6167 655f 6c69 622e      storage_lib.
+0001b690: 5374 6f72 6554 7970 652e 5333 2c20 7374  StoreType.S3, st
+0001b6a0: 6f72 6167 655f 6c69 622e 5374 6f72 6554  orage_lib.StoreT
+0001b6b0: 7970 652e 4743 532c 0a20 2020 2020 2020  ype.GCS,.       
+0001b6c0: 2070 7974 6573 742e 7061 7261 6d28 7374   pytest.param(st
+0001b6d0: 6f72 6167 655f 6c69 622e 5374 6f72 6554  orage_lib.StoreT
+0001b6e0: 7970 652e 5232 2c20 6d61 726b 733d 7079  ype.R2, marks=py
+0001b6f0: 7465 7374 2e6d 6172 6b2e 636c 6f75 6466  test.mark.cloudf
+0001b700: 6c61 7265 290a 2020 2020 5d29 0a20 2020  lare).    ]).   
+0001b710: 2064 6566 2074 6573 745f 6275 636b 6574   def test_bucket
+0001b720: 5f62 756c 6b5f 6465 6c65 7469 6f6e 2873  _bulk_deletion(s
+0001b730: 656c 662c 2073 746f 7265 5f74 7970 652c  elf, store_type,
+0001b740: 2074 6d70 5f62 756c 6b5f 6465 6c5f 7374   tmp_bulk_del_st
+0001b750: 6f72 6167 655f 6f62 6a29 3a0a 2020 2020  orage_obj):.    
+0001b760: 2020 2020 2320 4372 6561 7465 7320 6120      # Creates a 
+0001b770: 7465 6d70 2066 6f6c 6465 7220 7769 7468  temp folder with
+0001b780: 206f 7665 7220 3235 3620 6669 6c65 7320   over 256 files 
+0001b790: 616e 6420 666f 6c64 6572 732c 2075 706c  and folders, upl
+0001b7a0: 6f61 640a 2020 2020 2020 2020 2320 6669  oad.        # fi
+0001b7b0: 6c65 7320 616e 6420 666f 6c64 6572 7320  les and folders 
+0001b7c0: 746f 2061 206e 6577 2062 7563 6b65 742c  to a new bucket,
+0001b7d0: 2074 6865 6e20 6465 6c65 7465 2062 7563   then delete buc
+0001b7e0: 6b65 742e 0a20 2020 2020 2020 2074 6d70  ket..        tmp
+0001b7f0: 5f62 756c 6b5f 6465 6c5f 7374 6f72 6167  _bulk_del_storag
+0001b800: 655f 6f62 6a2e 6164 645f 7374 6f72 6528  e_obj.add_store(
+0001b810: 7374 6f72 655f 7479 7065 290a 0a20 2020  store_type)..   
+0001b820: 2020 2020 2073 7562 7072 6f63 6573 732e       subprocess.
+0001b830: 6368 6563 6b5f 6f75 7470 7574 280a 2020  check_output(.  
+0001b840: 2020 2020 2020 2020 2020 5b27 736b 7927            ['sky'
+0001b850: 2c20 2773 746f 7261 6765 272c 2027 6465  , 'storage', 'de
+0001b860: 6c65 7465 272c 2074 6d70 5f62 756c 6b5f  lete', tmp_bulk_
+0001b870: 6465 6c5f 7374 6f72 6167 655f 6f62 6a2e  del_storage_obj.
+0001b880: 6e61 6d65 5d29 0a0a 2020 2020 2020 2020  name])..        
+0001b890: 6f75 7470 7574 203d 2073 7562 7072 6f63  output = subproc
+0001b8a0: 6573 732e 6368 6563 6b5f 6f75 7470 7574  ess.check_output
+0001b8b0: 285b 2773 6b79 272c 2027 7374 6f72 6167  (['sky', 'storag
+0001b8c0: 6527 2c20 276c 7327 5d29 0a20 2020 2020  e', 'ls']).     
+0001b8d0: 2020 2061 7373 6572 7420 746d 705f 6275     assert tmp_bu
+0001b8e0: 6c6b 5f64 656c 5f73 746f 7261 6765 5f6f  lk_del_storage_o
+0001b8f0: 626a 2e6e 616d 6520 6e6f 7420 696e 206f  bj.name not in o
+0001b900: 7574 7075 742e 6465 636f 6465 2827 7574  utput.decode('ut
+0001b910: 662d 3827 290a 0a20 2020 2040 7079 7465  f-8')..    @pyte
+0001b920: 7374 2e6d 6172 6b2e 7061 7261 6d65 7472  st.mark.parametr
+0001b930: 697a 6528 0a20 2020 2020 2020 2027 746d  ize(.        'tm
+0001b940: 705f 7075 626c 6963 5f73 746f 7261 6765  p_public_storage
+0001b950: 5f6f 626a 2c20 7374 6f72 655f 7479 7065  _obj, store_type
+0001b960: 272c 0a20 2020 2020 2020 205b 2827 7333  ',.        [('s3
+0001b970: 3a2f 2f74 6367 612d 322d 6f70 656e 272c  ://tcga-2-open',
+0001b980: 2073 746f 7261 6765 5f6c 6962 2e53 746f   storage_lib.Sto
+0001b990: 7265 5479 7065 2e53 3329 2c0a 2020 2020  reType.S3),.    
+0001b9a0: 2020 2020 2028 2773 333a 2f2f 6469 6769       ('s3://digi
+0001b9b0: 7461 6c63 6f72 706f 7261 272c 2073 746f  talcorpora', sto
+0001b9c0: 7261 6765 5f6c 6962 2e53 746f 7265 5479  rage_lib.StoreTy
+0001b9d0: 7065 2e53 3329 2c0a 2020 2020 2020 2020  pe.S3),.        
+0001b9e0: 2028 2767 733a 2f2f 6763 702d 7075 626c   ('gs://gcp-publ
+0001b9f0: 6963 2d64 6174 612d 7365 6e74 696e 656c  ic-data-sentinel
+0001ba00: 2d32 272c 2073 746f 7261 6765 5f6c 6962  -2', storage_lib
+0001ba10: 2e53 746f 7265 5479 7065 2e47 4353 295d  .StoreType.GCS)]
+0001ba20: 2c0a 2020 2020 2020 2020 696e 6469 7265  ,.        indire
+0001ba30: 6374 3d5b 2774 6d70 5f70 7562 6c69 635f  ct=['tmp_public_
+0001ba40: 7374 6f72 6167 655f 6f62 6a27 5d29 0a20  storage_obj']). 
+0001ba50: 2020 2064 6566 2074 6573 745f 7075 626c     def test_publ
+0001ba60: 6963 5f62 7563 6b65 7428 7365 6c66 2c20  ic_bucket(self, 
+0001ba70: 746d 705f 7075 626c 6963 5f73 746f 7261  tmp_public_stora
+0001ba80: 6765 5f6f 626a 2c20 7374 6f72 655f 7479  ge_obj, store_ty
+0001ba90: 7065 293a 0a20 2020 2020 2020 2023 2043  pe):.        # C
+0001baa0: 7265 6174 6573 2061 206e 6577 2062 7563  reates a new buc
+0001bab0: 6b65 7420 7769 7468 2061 2070 7562 6c69  ket with a publi
+0001bac0: 6320 736f 7572 6365 2061 6e64 2076 6572  c source and ver
+0001bad0: 6966 6965 7320 7468 6174 2069 7420 6973  ifies that it is
+0001bae0: 206e 6f74 0a20 2020 2020 2020 2023 2061   not.        # a
+0001baf0: 6464 6564 2074 6f20 676c 6f62 616c 5f75  dded to global_u
+0001bb00: 7365 725f 7374 6174 652e 0a20 2020 2020  ser_state..     
+0001bb10: 2020 2074 6d70 5f70 7562 6c69 635f 7374     tmp_public_st
+0001bb20: 6f72 6167 655f 6f62 6a2e 6164 645f 7374  orage_obj.add_st
+0001bb30: 6f72 6528 7374 6f72 655f 7479 7065 290a  ore(store_type).
+0001bb40: 0a20 2020 2020 2020 2023 2052 756e 2073  .        # Run s
+0001bb50: 6b79 2073 746f 7261 6765 206c 7320 746f  ky storage ls to
+0001bb60: 2063 6865 636b 2069 6620 7374 6f72 6167   check if storag
+0001bb70: 6520 6f62 6a65 6374 2065 7869 7374 7320  e object exists 
+0001bb80: 696e 2074 6865 206f 7574 7075 740a 2020  in the output.  
+0001bb90: 2020 2020 2020 6f75 7420 3d20 7375 6270        out = subp
+0001bba0: 726f 6365 7373 2e63 6865 636b 5f6f 7574  rocess.check_out
+0001bbb0: 7075 7428 5b27 736b 7927 2c20 2773 746f  put(['sky', 'sto
+0001bbc0: 7261 6765 272c 2027 6c73 275d 290a 2020  rage', 'ls']).  
+0001bbd0: 2020 2020 2020 6173 7365 7274 2074 6d70        assert tmp
+0001bbe0: 5f70 7562 6c69 635f 7374 6f72 6167 655f  _public_storage_
+0001bbf0: 6f62 6a2e 6e61 6d65 206e 6f74 2069 6e20  obj.name not in 
+0001bc00: 6f75 742e 6465 636f 6465 2827 7574 662d  out.decode('utf-
+0001bc10: 3827 290a 0a20 2020 2040 7079 7465 7374  8')..    @pytest
+0001bc20: 2e6d 6172 6b2e 7061 7261 6d65 7472 697a  .mark.parametriz
+0001bc30: 6528 276e 6f6e 6578 6973 745f 6275 636b  e('nonexist_buck
+0001bc40: 6574 5f75 726c 272c 205b 0a20 2020 2020  et_url', [.     
+0001bc50: 2020 2027 7333 3a2f 2f7b 7261 6e64 6f6d     's3://{random
+0001bc60: 5f6e 616d 657d 272c 2027 6773 3a2f 2f7b  _name}', 'gs://{
+0001bc70: 7261 6e64 6f6d 5f6e 616d 657d 272c 0a20  random_name}',. 
+0001bc80: 2020 2020 2020 2070 7974 6573 742e 7061         pytest.pa
+0001bc90: 7261 6d28 2772 323a 2f2f 7b72 616e 646f  ram('r2://{rando
+0001bca0: 6d5f 6e61 6d65 7d27 2c20 6d61 726b 733d  m_name}', marks=
+0001bcb0: 7079 7465 7374 2e6d 6172 6b2e 636c 6f75  pytest.mark.clou
+0001bcc0: 6466 6c61 7265 290a 2020 2020 5d29 0a20  dflare).    ]). 
+0001bcd0: 2020 2064 6566 2074 6573 745f 6e6f 6e65     def test_none
+0001bce0: 7869 7374 656e 745f 6275 636b 6574 2873  xistent_bucket(s
+0001bcf0: 656c 662c 206e 6f6e 6578 6973 745f 6275  elf, nonexist_bu
+0001bd00: 636b 6574 5f75 726c 293a 0a20 2020 2020  cket_url):.     
+0001bd10: 2020 2023 2041 7474 656d 7074 7320 746f     # Attempts to
+0001bd20: 2063 7265 6174 6520 6665 7463 6820 6120   create fetch a 
+0001bd30: 7374 726f 6167 6520 7769 7468 2061 206e  stroage with a n
+0001bd40: 6f6e 2d65 7869 7374 656e 7420 736f 7572  on-existent sour
+0001bd50: 6365 2e0a 2020 2020 2020 2020 2320 4765  ce..        # Ge
+0001bd60: 6e65 7261 7465 2061 2072 616e 646f 6d20  nerate a random 
+0001bd70: 6275 636b 6574 206e 616d 6520 616e 6420  bucket name and 
+0001bd80: 7665 7269 6679 2069 7420 646f 6573 6e27  verify it doesn'
+0001bd90: 7420 6578 6973 743a 0a20 2020 2020 2020  t exist:.       
+0001bda0: 2072 6574 7279 5f63 6f75 6e74 203d 2030   retry_count = 0
+0001bdb0: 0a20 2020 2020 2020 2077 6869 6c65 2054  .        while T
+0001bdc0: 7275 653a 0a20 2020 2020 2020 2020 2020  rue:.           
+0001bdd0: 206e 6f6e 6578 6973 745f 6275 636b 6574   nonexist_bucket
+0001bde0: 5f6e 616d 6520 3d20 7374 7228 7575 6964  _name = str(uuid
+0001bdf0: 2e75 7569 6434 2829 290a 2020 2020 2020  .uuid4()).      
+0001be00: 2020 2020 2020 6966 206e 6f6e 6578 6973        if nonexis
+0001be10: 745f 6275 636b 6574 5f75 726c 2e73 7461  t_bucket_url.sta
+0001be20: 7274 7377 6974 6828 2773 3327 293a 0a20  rtswith('s3'):. 
+0001be30: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0001be40: 6f6d 6d61 6e64 203d 2066 2761 7773 2073  ommand = f'aws s
+0001be50: 3361 7069 2068 6561 642d 6275 636b 6574  3api head-bucket
+0001be60: 202d 2d62 7563 6b65 7420 7b6e 6f6e 6578   --bucket {nonex
+0001be70: 6973 745f 6275 636b 6574 5f6e 616d 657d  ist_bucket_name}
+0001be80: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
+0001be90: 2020 6578 7065 6374 6564 5f6f 7574 7075    expected_outpu
+0001bea0: 7420 3d20 2734 3034 270a 2020 2020 2020  t = '404'.      
+0001beb0: 2020 2020 2020 656c 6966 206e 6f6e 6578        elif nonex
+0001bec0: 6973 745f 6275 636b 6574 5f75 726c 2e73  ist_bucket_url.s
+0001bed0: 7461 7274 7377 6974 6828 2767 7327 293a  tartswith('gs'):
+0001bee0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001bef0: 2063 6f6d 6d61 6e64 203d 2066 2767 7375   command = f'gsu
+0001bf00: 7469 6c20 6c73 207b 6e6f 6e65 7869 7374  til ls {nonexist
+0001bf10: 5f62 7563 6b65 745f 7572 6c2e 666f 726d  _bucket_url.form
+0001bf20: 6174 2872 616e 646f 6d5f 6e61 6d65 3d6e  at(random_name=n
+0001bf30: 6f6e 6578 6973 745f 6275 636b 6574 5f6e  onexist_bucket_n
+0001bf40: 616d 6529 7d27 0a20 2020 2020 2020 2020  ame)}'.         
+0001bf50: 2020 2020 2020 2065 7870 6563 7465 645f         expected_
+0001bf60: 6f75 7470 7574 203d 2027 4275 636b 6574  output = 'Bucket
+0001bf70: 4e6f 7446 6f75 6e64 4578 6365 7074 696f  NotFoundExceptio
+0001bf80: 6e27 0a20 2020 2020 2020 2020 2020 2065  n'.            e
+0001bf90: 6c69 6620 6e6f 6e65 7869 7374 5f62 7563  lif nonexist_buc
+0001bfa0: 6b65 745f 7572 6c2e 7374 6172 7473 7769  ket_url.startswi
+0001bfb0: 7468 2827 7232 2729 3a0a 2020 2020 2020  th('r2'):.      
+0001bfc0: 2020 2020 2020 2020 2020 656e 6470 6f69            endpoi
+0001bfd0: 6e74 5f75 726c 203d 2063 6c6f 7564 666c  nt_url = cloudfl
+0001bfe0: 6172 652e 6372 6561 7465 5f65 6e64 706f  are.create_endpo
+0001bff0: 696e 7428 290a 2020 2020 2020 2020 2020  int().          
+0001c000: 2020 2020 2020 636f 6d6d 616e 6420 3d20        command = 
+0001c010: 6627 4157 535f 5348 4152 4544 5f43 5245  f'AWS_SHARED_CRE
+0001c020: 4445 4e54 4941 4c53 5f46 494c 453d 7b63  DENTIALS_FILE={c
+0001c030: 6c6f 7564 666c 6172 652e 5232 5f43 5245  loudflare.R2_CRE
+0001c040: 4445 4e54 4941 4c53 5f50 4154 487d 2061  DENTIALS_PATH} a
+0001c050: 7773 2073 3361 7069 2068 6561 642d 6275  ws s3api head-bu
+0001c060: 636b 6574 202d 2d62 7563 6b65 7420 7b6e  cket --bucket {n
+0001c070: 6f6e 6578 6973 745f 6275 636b 6574 5f6e  onexist_bucket_n
+0001c080: 616d 657d 202d 2d65 6e64 706f 696e 7420  ame} --endpoint 
+0001c090: 7b65 6e64 706f 696e 745f 7572 6c7d 202d  {endpoint_url} -
+0001c0a0: 2d70 726f 6669 6c65 3d72 3227 0a20 2020  -profile=r2'.   
+0001c0b0: 2020 2020 2020 2020 2020 2020 2065 7870               exp
+0001c0c0: 6563 7465 645f 6f75 7470 7574 203d 2027  ected_output = '
+0001c0d0: 3430 3427 0a20 2020 2020 2020 2020 2020  404'.           
+0001c0e0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0001c0f0: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+0001c100: 7565 4572 726f 7228 2755 6e73 7570 706f  ueError('Unsuppo
+0001c110: 7274 6564 2062 7563 6b65 7420 7479 7065  rted bucket type
+0001c120: 2027 0a20 2020 2020 2020 2020 2020 2020   '.             
+0001c130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c140: 2020 2020 6627 7b6e 6f6e 6578 6973 745f      f'{nonexist_
+0001c150: 6275 636b 6574 5f75 726c 7d27 290a 0a20  bucket_url}').. 
+0001c160: 2020 2020 2020 2020 2020 2023 2043 6865             # Che
+0001c170: 636b 2069 6620 6275 636b 6574 2065 7869  ck if bucket exi
+0001c180: 7374 7320 7573 696e 6720 7468 6520 636c  sts using the cl
+0001c190: 693a 0a20 2020 2020 2020 2020 2020 2074  i:.            t
+0001c1a0: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+0001c1b0: 2020 2020 6f75 7420 3d20 7375 6270 726f      out = subpro
+0001c1c0: 6365 7373 2e63 6865 636b 5f6f 7574 7075  cess.check_outpu
+0001c1d0: 7428 636f 6d6d 616e 642c 0a20 2020 2020  t(command,.     
+0001c1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001c1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c210: 7368 656c 6c3d 5472 7565 290a 2020 2020  shell=True).    
-0001c220: 2020 2020 2020 2020 6578 6365 7074 2073          except s
-0001c230: 7562 7072 6f63 6573 732e 4361 6c6c 6564  ubprocess.Called
-0001c240: 5072 6f63 6573 7345 7272 6f72 2061 7320  ProcessError as 
-0001c250: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0001c260: 2020 206f 7574 203d 2065 2e6f 7574 7075     out = e.outpu
-0001c270: 740a 2020 2020 2020 2020 2020 2020 6f75  t.            ou
-0001c280: 7420 3d20 6f75 742e 6465 636f 6465 2827  t = out.decode('
-0001c290: 7574 662d 3827 290a 2020 2020 2020 2020  utf-8').        
-0001c2a0: 2020 2020 6966 2065 7870 6563 7465 645f      if expected_
-0001c2b0: 6f75 7470 7574 2069 6e20 6f75 743a 0a20  output in out:. 
-0001c2c0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-0001c2d0: 7265 616b 0a20 2020 2020 2020 2020 2020  reak.           
-0001c2e0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0001c2f0: 2020 2020 2020 2072 6574 7279 5f63 6f75         retry_cou
-0001c300: 6e74 202b 3d20 310a 2020 2020 2020 2020  nt += 1.        
-0001c310: 2020 2020 2020 2020 6966 2072 6574 7279          if retry
-0001c320: 5f63 6f75 6e74 203e 2033 3a0a 2020 2020  _count > 3:.    
-0001c330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c340: 7261 6973 6520 5275 6e74 696d 6545 7272  raise RuntimeErr
-0001c350: 6f72 2827 556e 6162 6c65 2074 6f20 6669  or('Unable to fi
-0001c360: 6e64 2061 206e 6f6e 6578 6973 7465 6e74  nd a nonexistent
-0001c370: 2062 7563 6b65 7420 270a 2020 2020 2020   bucket '.      
-0001c380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c3a0: 2027 746f 2075 7365 2e20 5468 6973 2069   'to use. This i
-0001c3b0: 7320 6869 676c 7920 756e 6c69 6b65 6c79  s higly unlikely
-0001c3c0: 202d 2027 0a20 2020 2020 2020 2020 2020   - '.           
+0001c200: 2020 2020 2020 2020 2073 7464 6572 723d           stderr=
+0001c210: 7375 6270 726f 6365 7373 2e53 5444 4f55  subprocess.STDOU
+0001c220: 542c 0a20 2020 2020 2020 2020 2020 2020  T,.             
+0001c230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c250: 2073 6865 6c6c 3d54 7275 6529 0a20 2020   shell=True).   
+0001c260: 2020 2020 2020 2020 2065 7863 6570 7420           except 
+0001c270: 7375 6270 726f 6365 7373 2e43 616c 6c65  subprocess.Calle
+0001c280: 6450 726f 6365 7373 4572 726f 7220 6173  dProcessError as
+0001c290: 2065 3a0a 2020 2020 2020 2020 2020 2020   e:.            
+0001c2a0: 2020 2020 6f75 7420 3d20 652e 6f75 7470      out = e.outp
+0001c2b0: 7574 0a20 2020 2020 2020 2020 2020 206f  ut.            o
+0001c2c0: 7574 203d 206f 7574 2e64 6563 6f64 6528  ut = out.decode(
+0001c2d0: 2775 7466 2d38 2729 0a20 2020 2020 2020  'utf-8').       
+0001c2e0: 2020 2020 2069 6620 6578 7065 6374 6564       if expected
+0001c2f0: 5f6f 7574 7075 7420 696e 206f 7574 3a0a  _output in out:.
+0001c300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c310: 6272 6561 6b0a 2020 2020 2020 2020 2020  break.          
+0001c320: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0001c330: 2020 2020 2020 2020 7265 7472 795f 636f          retry_co
+0001c340: 756e 7420 2b3d 2031 0a20 2020 2020 2020  unt += 1.       
+0001c350: 2020 2020 2020 2020 2069 6620 7265 7472           if retr
+0001c360: 795f 636f 756e 7420 3e20 333a 0a20 2020  y_count > 3:.   
+0001c370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c380: 2072 6169 7365 2052 756e 7469 6d65 4572   raise RuntimeEr
+0001c390: 726f 7228 2755 6e61 626c 6520 746f 2066  ror('Unable to f
+0001c3a0: 696e 6420 6120 6e6f 6e65 7869 7374 656e  ind a nonexisten
+0001c3b0: 7420 6275 636b 6574 2027 0a20 2020 2020  t bucket '.     
+0001c3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001c3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c3e0: 2020 2020 2020 2020 2020 2020 2763 6865              'che
-0001c3f0: 636b 2069 6620 7468 6520 7465 7374 7320  ck if the tests 
-0001c400: 6172 6520 636f 7272 6563 742e 2729 0a0a  are correct.')..
-0001c410: 2020 2020 2020 2020 7769 7468 2070 7974          with pyt
-0001c420: 6573 742e 7261 6973 6573 280a 2020 2020  est.raises(.    
-0001c430: 2020 2020 2020 2020 2020 2020 736b 792e              sky.
-0001c440: 6578 6365 7074 696f 6e73 2e53 746f 7261  exceptions.Stora
-0001c450: 6765 4275 636b 6574 4765 7445 7272 6f72  geBucketGetError
-0001c460: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0001c470: 2020 6d61 7463 683d 2741 7474 656d 7074    match='Attempt
-0001c480: 6564 2074 6f20 636f 6e6e 6563 7420 746f  ed to connect to
-0001c490: 2061 206e 6f6e 2d65 7869 7374 656e 7420   a non-existent 
-0001c4a0: 6275 636b 6574 2729 3a0a 2020 2020 2020  bucket'):.      
-0001c4b0: 2020 2020 2020 7374 6f72 6167 655f 6f62        storage_ob
-0001c4c0: 6a20 3d20 7374 6f72 6167 655f 6c69 622e  j = storage_lib.
-0001c4d0: 5374 6f72 6167 6528 736f 7572 6365 3d6e  Storage(source=n
-0001c4e0: 6f6e 6578 6973 745f 6275 636b 6574 5f75  onexist_bucket_u
-0001c4f0: 726c 2e66 6f72 6d61 7428 0a20 2020 2020  rl.format(.     
-0001c500: 2020 2020 2020 2020 2020 2072 616e 646f             rando
-0001c510: 6d5f 6e61 6d65 3d6e 6f6e 6578 6973 745f  m_name=nonexist_
-0001c520: 6275 636b 6574 5f6e 616d 6529 290a 0a20  bucket_name)).. 
-0001c530: 2020 2040 7079 7465 7374 2e6d 6172 6b2e     @pytest.mark.
-0001c540: 7061 7261 6d65 7472 697a 6528 2770 7269  parametrize('pri
-0001c550: 7661 7465 5f62 7563 6b65 7427 2c0a 2020  vate_bucket',.  
-0001c560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c570: 2020 2020 2020 2020 2020 205b 6627 7333             [f's3
-0001c580: 3a2f 2f69 6d61 6765 6e65 7427 2c20 6627  ://imagenet', f'
-0001c590: 6773 3a2f 2f69 6d61 6765 6e65 7427 5d29  gs://imagenet'])
-0001c5a0: 0a20 2020 2064 6566 2074 6573 745f 7072  .    def test_pr
-0001c5b0: 6976 6174 655f 6275 636b 6574 2873 656c  ivate_bucket(sel
-0001c5c0: 662c 2070 7269 7661 7465 5f62 7563 6b65  f, private_bucke
-0001c5d0: 7429 3a0a 2020 2020 2020 2020 2320 4174  t):.        # At
-0001c5e0: 7465 6d70 7473 2074 6f20 6163 6365 7373  tempts to access
-0001c5f0: 2070 7269 7661 7465 2062 7563 6b65 7473   private buckets
-0001c600: 206e 6f74 2062 656c 6f6e 6769 6e67 2074   not belonging t
-0001c610: 6f20 7468 6520 7573 6572 2e0a 2020 2020  o the user..    
-0001c620: 2020 2020 2320 5468 6573 6520 6275 636b      # These buck
-0001c630: 6574 7320 6172 6520 6b6e 6f77 6e20 746f  ets are known to
-0001c640: 2062 6520 7072 6976 6174 652c 2062 7574   be private, but
-0001c650: 206d 6179 206e 6565 6420 746f 2062 6520   may need to be 
-0001c660: 7570 6461 7465 6420 6966 0a20 2020 2020  updated if.     
-0001c670: 2020 2023 2074 6865 7920 6172 6520 7265     # they are re
-0001c680: 6d6f 7665 6420 6279 2074 6865 6972 206f  moved by their o
-0001c690: 776e 6572 732e 0a20 2020 2020 2020 2070  wners..        p
-0001c6a0: 7269 7661 7465 5f62 7563 6b65 745f 6e61  rivate_bucket_na
-0001c6b0: 6d65 203d 2075 726c 6c69 622e 7061 7273  me = urllib.pars
-0001c6c0: 652e 7572 6c73 706c 6974 2870 7269 7661  e.urlsplit(priva
-0001c6d0: 7465 5f62 7563 6b65 7429 2e6e 6574 6c6f  te_bucket).netlo
-0001c6e0: 630a 2020 2020 2020 2020 7769 7468 2070  c.        with p
-0001c6f0: 7974 6573 742e 7261 6973 6573 280a 2020  ytest.raises(.  
-0001c700: 2020 2020 2020 2020 2020 2020 2020 736b                sk
-0001c710: 792e 6578 6365 7074 696f 6e73 2e53 746f  y.exceptions.Sto
-0001c720: 7261 6765 4275 636b 6574 4765 7445 7272  rageBucketGetErr
-0001c730: 6f72 2c0a 2020 2020 2020 2020 2020 2020  or,.            
-0001c740: 2020 2020 6d61 7463 683d 7374 6f72 6167      match=storag
-0001c750: 655f 6c69 622e 5f42 5543 4b45 545f 4641  e_lib._BUCKET_FA
-0001c760: 494c 5f54 4f5f 434f 4e4e 4543 545f 4d45  IL_TO_CONNECT_ME
-0001c770: 5353 4147 452e 666f 726d 6174 280a 2020  SSAGE.format(.  
-0001c780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c790: 2020 6e61 6d65 3d70 7269 7661 7465 5f62    name=private_b
-0001c7a0: 7563 6b65 745f 6e61 6d65 2929 3a0a 2020  ucket_name)):.  
-0001c7b0: 2020 2020 2020 2020 2020 7374 6f72 6167            storag
-0001c7c0: 655f 6f62 6a20 3d20 7374 6f72 6167 655f  e_obj = storage_
-0001c7d0: 6c69 622e 5374 6f72 6167 6528 736f 7572  lib.Storage(sour
-0001c7e0: 6365 3d70 7269 7661 7465 5f62 7563 6b65  ce=private_bucke
-0001c7f0: 7429 0a0a 2020 2020 4070 7974 6573 742e  t)..    @pytest.
-0001c800: 6d61 726b 2e70 6172 616d 6574 7269 7a65  mark.parametrize
-0001c810: 2827 6578 745f 6275 636b 6574 5f66 6978  ('ext_bucket_fix
-0001c820: 7475 7265 2c20 7374 6f72 655f 7479 7065  ture, store_type
-0001c830: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-0001c840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c850: 5b28 2774 6d70 5f61 7773 636c 695f 6275  [('tmp_awscli_bu
-0001c860: 636b 6574 272c 2073 746f 7261 6765 5f6c  cket', storage_l
-0001c870: 6962 2e53 746f 7265 5479 7065 2e53 3329  ib.StoreType.S3)
-0001c880: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0001c890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c8a0: 2827 746d 705f 6773 7574 696c 5f62 7563  ('tmp_gsutil_buc
-0001c8b0: 6b65 7427 2c20 7374 6f72 6167 655f 6c69  ket', storage_li
-0001c8c0: 622e 5374 6f72 6554 7970 652e 4743 5329  b.StoreType.GCS)
-0001c8d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0001c8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c8f0: 7079 7465 7374 2e70 6172 616d 2827 746d  pytest.param('tm
-0001c900: 705f 6177 7363 6c69 5f62 7563 6b65 745f  p_awscli_bucket_
-0001c910: 7232 272c 0a20 2020 2020 2020 2020 2020  r2',.           
+0001c3e0: 2020 2774 6f20 7573 652e 2054 6869 7320    'to use. This 
+0001c3f0: 6973 2068 6967 6c79 2075 6e6c 696b 656c  is higly unlikel
+0001c400: 7920 2d20 270a 2020 2020 2020 2020 2020  y - '.          
+0001c410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c420: 2020 2020 2020 2020 2020 2020 2027 6368               'ch
+0001c430: 6563 6b20 6966 2074 6865 2074 6573 7473  eck if the tests
+0001c440: 2061 7265 2063 6f72 7265 6374 2e27 290a   are correct.').
+0001c450: 0a20 2020 2020 2020 2077 6974 6820 7079  .        with py
+0001c460: 7465 7374 2e72 6169 7365 7328 0a20 2020  test.raises(.   
+0001c470: 2020 2020 2020 2020 2020 2020 2073 6b79               sky
+0001c480: 2e65 7863 6570 7469 6f6e 732e 5374 6f72  .exceptions.Stor
+0001c490: 6167 6542 7563 6b65 7447 6574 4572 726f  ageBucketGetErro
+0001c4a0: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
+0001c4b0: 2020 206d 6174 6368 3d27 4174 7465 6d70     match='Attemp
+0001c4c0: 7465 6420 746f 2063 6f6e 6e65 6374 2074  ted to connect t
+0001c4d0: 6f20 6120 6e6f 6e2d 6578 6973 7465 6e74  o a non-existent
+0001c4e0: 2062 7563 6b65 7427 293a 0a20 2020 2020   bucket'):.     
+0001c4f0: 2020 2020 2020 2073 746f 7261 6765 5f6f         storage_o
+0001c500: 626a 203d 2073 746f 7261 6765 5f6c 6962  bj = storage_lib
+0001c510: 2e53 746f 7261 6765 2873 6f75 7263 653d  .Storage(source=
+0001c520: 6e6f 6e65 7869 7374 5f62 7563 6b65 745f  nonexist_bucket_
+0001c530: 7572 6c2e 666f 726d 6174 280a 2020 2020  url.format(.    
+0001c540: 2020 2020 2020 2020 2020 2020 7261 6e64              rand
+0001c550: 6f6d 5f6e 616d 653d 6e6f 6e65 7869 7374  om_name=nonexist
+0001c560: 5f62 7563 6b65 745f 6e61 6d65 2929 0a0a  _bucket_name))..
+0001c570: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
+0001c580: 2e70 6172 616d 6574 7269 7a65 2827 7072  .parametrize('pr
+0001c590: 6976 6174 655f 6275 636b 6574 272c 0a20  ivate_bucket',. 
+0001c5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c5b0: 2020 2020 2020 2020 2020 2020 5b66 2773              [f's
+0001c5c0: 333a 2f2f 696d 6167 656e 6574 272c 2066  3://imagenet', f
+0001c5d0: 2767 733a 2f2f 696d 6167 656e 6574 275d  'gs://imagenet']
+0001c5e0: 290a 2020 2020 6465 6620 7465 7374 5f70  ).    def test_p
+0001c5f0: 7269 7661 7465 5f62 7563 6b65 7428 7365  rivate_bucket(se
+0001c600: 6c66 2c20 7072 6976 6174 655f 6275 636b  lf, private_buck
+0001c610: 6574 293a 0a20 2020 2020 2020 2023 2041  et):.        # A
+0001c620: 7474 656d 7074 7320 746f 2061 6363 6573  ttempts to acces
+0001c630: 7320 7072 6976 6174 6520 6275 636b 6574  s private bucket
+0001c640: 7320 6e6f 7420 6265 6c6f 6e67 696e 6720  s not belonging 
+0001c650: 746f 2074 6865 2075 7365 722e 0a20 2020  to the user..   
+0001c660: 2020 2020 2023 2054 6865 7365 2062 7563       # These buc
+0001c670: 6b65 7473 2061 7265 206b 6e6f 776e 2074  kets are known t
+0001c680: 6f20 6265 2070 7269 7661 7465 2c20 6275  o be private, bu
+0001c690: 7420 6d61 7920 6e65 6564 2074 6f20 6265  t may need to be
+0001c6a0: 2075 7064 6174 6564 2069 660a 2020 2020   updated if.    
+0001c6b0: 2020 2020 2320 7468 6579 2061 7265 2072      # they are r
+0001c6c0: 656d 6f76 6564 2062 7920 7468 6569 7220  emoved by their 
+0001c6d0: 6f77 6e65 7273 2e0a 2020 2020 2020 2020  owners..        
+0001c6e0: 7072 6976 6174 655f 6275 636b 6574 5f6e  private_bucket_n
+0001c6f0: 616d 6520 3d20 7572 6c6c 6962 2e70 6172  ame = urllib.par
+0001c700: 7365 2e75 726c 7370 6c69 7428 7072 6976  se.urlsplit(priv
+0001c710: 6174 655f 6275 636b 6574 292e 6e65 746c  ate_bucket).netl
+0001c720: 6f63 0a20 2020 2020 2020 2077 6974 6820  oc.        with 
+0001c730: 7079 7465 7374 2e72 6169 7365 7328 0a20  pytest.raises(. 
+0001c740: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001c750: 6b79 2e65 7863 6570 7469 6f6e 732e 5374  ky.exceptions.St
+0001c760: 6f72 6167 6542 7563 6b65 7447 6574 4572  orageBucketGetEr
+0001c770: 726f 722c 0a20 2020 2020 2020 2020 2020  ror,.           
+0001c780: 2020 2020 206d 6174 6368 3d73 746f 7261       match=stora
+0001c790: 6765 5f6c 6962 2e5f 4255 434b 4554 5f46  ge_lib._BUCKET_F
+0001c7a0: 4149 4c5f 544f 5f43 4f4e 4e45 4354 5f4d  AIL_TO_CONNECT_M
+0001c7b0: 4553 5341 4745 2e66 6f72 6d61 7428 0a20  ESSAGE.format(. 
+0001c7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c7d0: 2020 206e 616d 653d 7072 6976 6174 655f     name=private_
+0001c7e0: 6275 636b 6574 5f6e 616d 6529 293a 0a20  bucket_name)):. 
+0001c7f0: 2020 2020 2020 2020 2020 2073 746f 7261             stora
+0001c800: 6765 5f6f 626a 203d 2073 746f 7261 6765  ge_obj = storage
+0001c810: 5f6c 6962 2e53 746f 7261 6765 2873 6f75  _lib.Storage(sou
+0001c820: 7263 653d 7072 6976 6174 655f 6275 636b  rce=private_buck
+0001c830: 6574 290a 0a20 2020 2040 7079 7465 7374  et)..    @pytest
+0001c840: 2e6d 6172 6b2e 7061 7261 6d65 7472 697a  .mark.parametriz
+0001c850: 6528 2765 7874 5f62 7563 6b65 745f 6669  e('ext_bucket_fi
+0001c860: 7874 7572 652c 2073 746f 7265 5f74 7970  xture, store_typ
+0001c870: 6527 2c0a 2020 2020 2020 2020 2020 2020  e',.            
+0001c880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c890: 205b 2827 746d 705f 6177 7363 6c69 5f62   [('tmp_awscli_b
+0001c8a0: 7563 6b65 7427 2c20 7374 6f72 6167 655f  ucket', storage_
+0001c8b0: 6c69 622e 5374 6f72 6554 7970 652e 5333  lib.StoreType.S3
+0001c8c0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+0001c8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c8e0: 2028 2774 6d70 5f67 7375 7469 6c5f 6275   ('tmp_gsutil_bu
+0001c8f0: 636b 6574 272c 2073 746f 7261 6765 5f6c  cket', storage_l
+0001c900: 6962 2e53 746f 7265 5479 7065 2e47 4353  ib.StoreType.GCS
+0001c910: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
 0001c920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c940: 7374 6f72 6167 655f 6c69 622e 5374 6f72  storage_lib.Stor
-0001c950: 6554 7970 652e 5232 2c0a 2020 2020 2020  eType.R2,.      
+0001c930: 2070 7974 6573 742e 7061 7261 6d28 2774   pytest.param('t
+0001c940: 6d70 5f61 7773 636c 695f 6275 636b 6574  mp_awscli_bucket
+0001c950: 5f72 3227 2c0a 2020 2020 2020 2020 2020  _r2',.          
 0001c960: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001c970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c980: 2020 2020 206d 6172 6b73 3d70 7974 6573       marks=pytes
-0001c990: 742e 6d61 726b 2e63 6c6f 7564 666c 6172  t.mark.cloudflar
-0001c9a0: 6529 5d29 0a20 2020 2064 6566 2074 6573  e)]).    def tes
-0001c9b0: 745f 7570 6c6f 6164 5f74 6f5f 6578 6973  t_upload_to_exis
-0001c9c0: 7469 6e67 5f62 7563 6b65 7428 7365 6c66  ting_bucket(self
-0001c9d0: 2c20 6578 745f 6275 636b 6574 5f66 6978  , ext_bucket_fix
-0001c9e0: 7475 7265 2c20 7265 7175 6573 742c 0a20  ture, request,. 
-0001c9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ca00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ca10: 2020 2020 2020 746d 705f 736f 7572 6365        tmp_source
-0001ca20: 2c20 7374 6f72 655f 7479 7065 293a 0a20  , store_type):. 
-0001ca30: 2020 2020 2020 2023 2054 7269 6573 2075         # Tries u
-0001ca40: 706c 6f61 6469 6e67 2065 7869 7374 696e  ploading existin
-0001ca50: 6720 6669 6c65 7320 746f 206e 6577 6c79  g files to newly
-0001ca60: 2063 7265 6174 6564 2062 7563 6b65 7420   created bucket 
-0001ca70: 286f 7574 7369 6465 206f 660a 2020 2020  (outside of.    
-0001ca80: 2020 2020 2320 736b 7929 2061 6e64 2076      # sky) and v
-0001ca90: 6572 6966 6965 7320 7468 6174 2066 696c  erifies that fil
-0001caa0: 6573 2061 7265 2077 7269 7474 656e 2e0a  es are written..
-0001cab0: 2020 2020 2020 2020 6275 636b 6574 5f6e          bucket_n
-0001cac0: 616d 6520 3d20 7265 7175 6573 742e 6765  ame = request.ge
-0001cad0: 7466 6978 7475 7265 7661 6c75 6528 6578  tfixturevalue(ex
-0001cae0: 745f 6275 636b 6574 5f66 6978 7475 7265  t_bucket_fixture
-0001caf0: 290a 2020 2020 2020 2020 7374 6f72 6167  ).        storag
-0001cb00: 655f 6f62 6a20 3d20 7374 6f72 6167 655f  e_obj = storage_
-0001cb10: 6c69 622e 5374 6f72 6167 6528 6e61 6d65  lib.Storage(name
-0001cb20: 3d62 7563 6b65 745f 6e61 6d65 2c20 736f  =bucket_name, so
-0001cb30: 7572 6365 3d74 6d70 5f73 6f75 7263 6529  urce=tmp_source)
-0001cb40: 0a20 2020 2020 2020 2073 746f 7261 6765  .        storage
-0001cb50: 5f6f 626a 2e61 6464 5f73 746f 7265 2873  _obj.add_store(s
-0001cb60: 746f 7265 5f74 7970 6529 0a0a 2020 2020  tore_type)..    
-0001cb70: 2020 2020 2320 4368 6563 6b20 6966 2074      # Check if t
-0001cb80: 6d70 5f73 6f75 7263 652f 746d 702d 6669  mp_source/tmp-fi
-0001cb90: 6c65 2065 7869 7374 7320 696e 2074 6865  le exists in the
-0001cba0: 2062 7563 6b65 7420 7573 696e 6720 6177   bucket using aw
-0001cbb0: 7320 636c 690a 2020 2020 2020 2020 6f75  s cli.        ou
-0001cbc0: 7420 3d20 7375 6270 726f 6365 7373 2e63  t = subprocess.c
-0001cbd0: 6865 636b 5f6f 7574 7075 7428 7365 6c66  heck_output(self
-0001cbe0: 2e63 6c69 5f6c 735f 636d 6428 7374 6f72  .cli_ls_cmd(stor
-0001cbf0: 655f 7479 7065 2c20 6275 636b 6574 5f6e  e_type, bucket_n
-0001cc00: 616d 6529 2c0a 2020 2020 2020 2020 2020  ame),.          
-0001cc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cc20: 2020 2020 2020 2020 2020 2020 7368 656c              shel
-0001cc30: 6c3d 5472 7565 290a 2020 2020 2020 2020  l=True).        
-0001cc40: 6173 7365 7274 2027 746d 702d 6669 6c65  assert 'tmp-file
-0001cc50: 2720 696e 206f 7574 2e64 6563 6f64 6528  ' in out.decode(
-0001cc60: 2775 7466 2d38 2729 2c20 5c0a 2020 2020  'utf-8'), \.    
-0001cc70: 2020 2020 2020 2020 2746 696c 6520 6e6f          'File no
-0001cc80: 7420 666f 756e 6420 696e 2062 7563 6b65  t found in bucke
-0001cc90: 7420 2d20 6f75 7470 7574 2077 6173 203a  t - output was :
-0001cca0: 207b 7d27 2e66 6f72 6d61 7428 6f75 742e   {}'.format(out.
-0001ccb0: 6465 636f 6465 0a20 2020 2020 2020 2020  decode.         
-0001ccc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ccd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ccf0: 2020 2020 2020 2028 2775 7466 2d38 2729         ('utf-8')
-0001cd00: 290a 0a20 2020 2020 2020 2023 2043 6865  )..        # Che
-0001cd10: 636b 2073 796d 6c69 6e6b 7320 2d20 7379  ck symlinks - sy
-0001cd20: 6d6c 696e 6b73 2064 6f6e 2774 2067 6574  mlinks don't get
-0001cd30: 2063 6f70 6965 6420 6279 2073 6b79 2073   copied by sky s
-0001cd40: 746f 7261 6765 0a20 2020 2020 2020 2061  torage.        a
-0001cd50: 7373 6572 7420 2870 6174 686c 6962 2e50  ssert (pathlib.P
-0001cd60: 6174 6828 746d 705f 736f 7572 6365 2920  ath(tmp_source) 
-0001cd70: 2f20 2763 6972 636c 652d 6c69 6e6b 2729  / 'circle-link')
-0001cd80: 2e69 735f 7379 6d6c 696e 6b28 292c 2028  .is_symlink(), (
-0001cd90: 0a20 2020 2020 2020 2020 2020 2027 6369  .            'ci
-0001cda0: 7263 6c65 2d6c 696e 6b20 7761 7320 6e6f  rcle-link was no
-0001cdb0: 7420 666f 756e 6420 696e 2074 6865 2075  t found in the u
-0001cdc0: 706c 6f61 6420 736f 7572 6365 202d 2027  pload source - '
-0001cdd0: 0a20 2020 2020 2020 2020 2020 2027 6172  .            'ar
-0001cde0: 6520 7468 6520 7465 7374 2066 6978 7475  e the test fixtu
-0001cdf0: 7265 7320 636f 7272 6563 743f 2729 0a20  res correct?'). 
-0001ce00: 2020 2020 2020 2061 7373 6572 7420 2763         assert 'c
-0001ce10: 6972 636c 652d 6c69 6e6b 2720 6e6f 7420  ircle-link' not 
-0001ce20: 696e 206f 7574 2e64 6563 6f64 6528 2775  in out.decode('u
-0001ce30: 7466 2d38 2729 2c20 280a 2020 2020 2020  tf-8'), (.      
-0001ce40: 2020 2020 2020 2753 796d 6c69 6e6b 2066        'Symlink f
-0001ce50: 6f75 6e64 2069 6e20 6275 636b 6574 202d  ound in bucket -
-0001ce60: 206c 7320 6f75 7470 7574 2077 6173 203a   ls output was :
-0001ce70: 207b 7d27 2e66 6f72 6d61 7428 0a20 2020   {}'.format(.   
-0001ce80: 2020 2020 2020 2020 2020 2020 206f 7574               out
-0001ce90: 2e64 6563 6f64 6528 2775 7466 2d38 2729  .decode('utf-8')
-0001cea0: 2929 0a0a 2020 2020 2020 2020 2320 5275  ))..        # Ru
-0001ceb0: 6e20 736b 7920 7374 6f72 6167 6520 6c73  n sky storage ls
-0001cec0: 2074 6f20 6368 6563 6b20 6966 2073 746f   to check if sto
-0001ced0: 7261 6765 206f 626a 6563 7420 6578 6973  rage object exis
-0001cee0: 7473 2069 6e20 7468 6520 6f75 7470 7574  ts in the output
-0001cef0: 2e0a 2020 2020 2020 2020 2320 4974 2073  ..        # It s
-0001cf00: 686f 756c 6420 6e6f 7420 6578 6973 7420  hould not exist 
-0001cf10: 6265 6361 7573 6520 7468 6520 6275 636b  because the buck
-0001cf20: 6574 2077 6173 2063 7265 6174 6564 2065  et was created e
-0001cf30: 7874 6572 6e61 6c6c 792e 0a20 2020 2020  xternally..     
-0001cf40: 2020 206f 7574 203d 2073 7562 7072 6f63     out = subproc
-0001cf50: 6573 732e 6368 6563 6b5f 6f75 7470 7574  ess.check_output
-0001cf60: 285b 2773 6b79 272c 2027 7374 6f72 6167  (['sky', 'storag
-0001cf70: 6527 2c20 276c 7327 5d29 0a20 2020 2020  e', 'ls']).     
-0001cf80: 2020 2061 7373 6572 7420 7374 6f72 6167     assert storag
-0001cf90: 655f 6f62 6a2e 6e61 6d65 206e 6f74 2069  e_obj.name not i
-0001cfa0: 6e20 6f75 742e 6465 636f 6465 2827 7574  n out.decode('ut
-0001cfb0: 662d 3827 290a 0a20 2020 2064 6566 2074  f-8')..    def t
-0001cfc0: 6573 745f 636f 7079 5f6d 6f75 6e74 5f65  est_copy_mount_e
-0001cfd0: 7869 7374 696e 675f 7374 6f72 6167 6528  xisting_storage(
-0001cfe0: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
-0001cff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d000: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0001d010: 6d70 5f63 6f70 795f 6d6e 745f 6578 6973  mp_copy_mnt_exis
-0001d020: 7469 6e67 5f73 746f 7261 6765 5f6f 626a  ting_storage_obj
-0001d030: 293a 0a20 2020 2020 2020 2023 2043 7265  ):.        # Cre
-0001d040: 6174 6573 2061 2062 7563 6b65 7420 7769  ates a bucket wi
-0001d050: 7468 206e 6f20 736f 7572 6365 2069 6e20  th no source in 
-0001d060: 4d4f 554e 5420 6d6f 6465 2028 656d 7074  MOUNT mode (empt
-0001d070: 7920 6275 636b 6574 292c 2061 6e64 0a20  y bucket), and. 
-0001d080: 2020 2020 2020 2023 2074 6865 6e20 7472         # then tr
-0001d090: 6965 7320 746f 206c 6f61 6420 7468 6520  ies to load the 
-0001d0a0: 7361 6d65 2073 746f 7261 6765 2069 6e20  same storage in 
-0001d0b0: 434f 5059 206d 6f64 652e 0a20 2020 2020  COPY mode..     
-0001d0c0: 2020 2074 6d70 5f63 6f70 795f 6d6e 745f     tmp_copy_mnt_
-0001d0d0: 6578 6973 7469 6e67 5f73 746f 7261 6765  existing_storage
-0001d0e0: 5f6f 626a 2e61 6464 5f73 746f 7265 2873  _obj.add_store(s
-0001d0f0: 746f 7261 6765 5f6c 6962 2e53 746f 7265  torage_lib.Store
-0001d100: 5479 7065 2e53 3329 0a20 2020 2020 2020  Type.S3).       
-0001d110: 2073 746f 7261 6765 5f6e 616d 6520 3d20   storage_name = 
-0001d120: 746d 705f 636f 7079 5f6d 6e74 5f65 7869  tmp_copy_mnt_exi
-0001d130: 7374 696e 675f 7374 6f72 6167 655f 6f62  sting_storage_ob
-0001d140: 6a2e 6e61 6d65 0a0a 2020 2020 2020 2020  j.name..        
-0001d150: 2320 4368 6563 6b20 6073 6b79 2073 746f  # Check `sky sto
-0001d160: 7261 6765 206c 7360 2074 6f20 656e 7375  rage ls` to ensu
-0001d170: 7265 2073 746f 7261 6765 206f 626a 6563  re storage objec
-0001d180: 7420 6578 6973 7473 0a20 2020 2020 2020  t exists.       
-0001d190: 206f 7574 203d 2073 7562 7072 6f63 6573   out = subproces
-0001d1a0: 732e 6368 6563 6b5f 6f75 7470 7574 285b  s.check_output([
-0001d1b0: 2773 6b79 272c 2027 7374 6f72 6167 6527  'sky', 'storage'
-0001d1c0: 2c20 276c 7327 5d29 2e64 6563 6f64 6528  , 'ls']).decode(
-0001d1d0: 2775 7466 2d38 2729 0a20 2020 2020 2020  'utf-8').       
-0001d1e0: 2061 7373 6572 7420 7374 6f72 6167 655f   assert storage_
-0001d1f0: 6e61 6d65 2069 6e20 6f75 742c 2066 2753  name in out, f'S
-0001d200: 746f 7261 6765 207b 7374 6f72 6167 655f  torage {storage_
-0001d210: 6e61 6d65 7d20 6e6f 7420 666f 756e 6420  name} not found 
-0001d220: 696e 2073 6b79 2073 746f 7261 6765 206c  in sky storage l
-0001d230: 732e 270a 0a20 2020 2040 7079 7465 7374  s.'..    @pytest
-0001d240: 2e6d 6172 6b2e 7061 7261 6d65 7472 697a  .mark.parametriz
-0001d250: 6528 2773 746f 7265 5f74 7970 6527 2c20  e('store_type', 
-0001d260: 5b0a 2020 2020 2020 2020 7374 6f72 6167  [.        storag
-0001d270: 655f 6c69 622e 5374 6f72 6554 7970 652e  e_lib.StoreType.
-0001d280: 5333 2c20 7374 6f72 6167 655f 6c69 622e  S3, storage_lib.
-0001d290: 5374 6f72 6554 7970 652e 4743 532c 0a20  StoreType.GCS,. 
-0001d2a0: 2020 2020 2020 2070 7974 6573 742e 7061         pytest.pa
-0001d2b0: 7261 6d28 7374 6f72 6167 655f 6c69 622e  ram(storage_lib.
-0001d2c0: 5374 6f72 6554 7970 652e 5232 2c20 6d61  StoreType.R2, ma
-0001d2d0: 726b 733d 7079 7465 7374 2e6d 6172 6b2e  rks=pytest.mark.
-0001d2e0: 636c 6f75 6466 6c61 7265 290a 2020 2020  cloudflare).    
-0001d2f0: 5d29 0a20 2020 2064 6566 2074 6573 745f  ]).    def test_
-0001d300: 6c69 7374 5f73 6f75 7263 6528 7365 6c66  list_source(self
-0001d310: 2c20 746d 705f 6c6f 6361 6c5f 6c69 7374  , tmp_local_list
-0001d320: 5f73 746f 7261 6765 5f6f 626a 2c20 7374  _storage_obj, st
-0001d330: 6f72 655f 7479 7065 293a 0a20 2020 2020  ore_type):.     
-0001d340: 2020 2023 2055 7365 7320 6120 6c69 7374     # Uses a list
-0001d350: 2069 6e20 7468 6520 736f 7572 6365 2066   in the source f
-0001d360: 6965 6c64 2074 6f20 7370 6563 6966 7920  ield to specify 
-0001d370: 6120 6669 6c65 2061 6e64 2061 2064 6972  a file and a dir
-0001d380: 6563 746f 7279 2074 6f0a 2020 2020 2020  ectory to.      
-0001d390: 2020 2320 6265 2075 706c 6f61 6465 6420    # be uploaded 
-0001d3a0: 746f 2074 6865 2073 746f 7261 6765 206f  to the storage o
-0001d3b0: 626a 6563 742e 0a20 2020 2020 2020 2074  bject..        t
-0001d3c0: 6d70 5f6c 6f63 616c 5f6c 6973 745f 7374  mp_local_list_st
-0001d3d0: 6f72 6167 655f 6f62 6a2e 6164 645f 7374  orage_obj.add_st
-0001d3e0: 6f72 6528 7374 6f72 655f 7479 7065 290a  ore(store_type).
-0001d3f0: 0a20 2020 2020 2020 2023 2043 6865 636b  .        # Check
-0001d400: 2069 6620 746d 702d 6669 6c65 2065 7869   if tmp-file exi
-0001d410: 7374 7320 696e 2074 6865 2062 7563 6b65  sts in the bucke
-0001d420: 7420 726f 6f74 2075 7369 6e67 2063 6c69  t root using cli
-0001d430: 0a20 2020 2020 2020 206f 7574 203d 2073  .        out = s
-0001d440: 7562 7072 6f63 6573 732e 6368 6563 6b5f  ubprocess.check_
-0001d450: 6f75 7470 7574 2873 656c 662e 636c 695f  output(self.cli_
-0001d460: 6c73 5f63 6d64 280a 2020 2020 2020 2020  ls_cmd(.        
-0001d470: 2020 2020 7374 6f72 655f 7479 7065 2c20      store_type, 
-0001d480: 746d 705f 6c6f 6361 6c5f 6c69 7374 5f73  tmp_local_list_s
-0001d490: 746f 7261 6765 5f6f 626a 2e6e 616d 6529  torage_obj.name)
-0001d4a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0001d4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d4c0: 2020 2020 2020 2020 7368 656c 6c3d 5472          shell=Tr
-0001d4d0: 7565 290a 2020 2020 2020 2020 6173 7365  ue).        asse
-0001d4e0: 7274 2027 746d 702d 6669 6c65 2720 696e  rt 'tmp-file' in
-0001d4f0: 206f 7574 2e64 6563 6f64 6528 2775 7466   out.decode('utf
-0001d500: 2d38 2729 2c20 5c0a 2020 2020 2020 2020  -8'), \.        
-0001d510: 2020 2020 2746 696c 6520 6e6f 7420 666f      'File not fo
-0001d520: 756e 6420 696e 2062 7563 6b65 7420 2d20  und in bucket - 
-0001d530: 6f75 7470 7574 2077 6173 203a 207b 7d27  output was : {}'
-0001d540: 2e66 6f72 6d61 7428 6f75 742e 6465 636f  .format(out.deco
-0001d550: 6465 0a20 2020 2020 2020 2020 2020 2020  de.             
-0001d560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d590: 2020 2028 2775 7466 2d38 2729 290a 0a20     ('utf-8')).. 
-0001d5a0: 2020 2020 2020 2023 2043 6865 636b 2069         # Check i
-0001d5b0: 6620 746d 702d 6669 6c65 2065 7869 7374  f tmp-file exist
-0001d5c0: 7320 696e 2074 6865 2062 7563 6b65 742f  s in the bucket/
-0001d5d0: 746d 702d 736f 7572 6365 2075 7369 6e67  tmp-source using
-0001d5e0: 2063 6c69 0a20 2020 2020 2020 206f 7574   cli.        out
-0001d5f0: 203d 2073 7562 7072 6f63 6573 732e 6368   = subprocess.ch
-0001d600: 6563 6b5f 6f75 7470 7574 2873 656c 662e  eck_output(self.
-0001d610: 636c 695f 6c73 5f63 6d64 280a 2020 2020  cli_ls_cmd(.    
-0001d620: 2020 2020 2020 2020 7374 6f72 655f 7479          store_ty
-0001d630: 7065 2c20 746d 705f 6c6f 6361 6c5f 6c69  pe, tmp_local_li
-0001d640: 7374 5f73 746f 7261 6765 5f6f 626a 2e6e  st_storage_obj.n
-0001d650: 616d 652c 2027 746d 702d 736f 7572 6365  ame, 'tmp-source
-0001d660: 2f27 292c 0a20 2020 2020 2020 2020 2020  /'),.           
-0001d670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d680: 2020 2020 2020 2020 2020 2073 6865 6c6c             shell
-0001d690: 3d54 7275 6529 0a20 2020 2020 2020 2061  =True).        a
-0001d6a0: 7373 6572 7420 2774 6d70 2d66 696c 6527  ssert 'tmp-file'
-0001d6b0: 2069 6e20 6f75 742e 6465 636f 6465 2827   in out.decode('
-0001d6c0: 7574 662d 3827 292c 205c 0a20 2020 2020  utf-8'), \.     
-0001d6d0: 2020 2020 2020 2027 4669 6c65 206e 6f74         'File not
-0001d6e0: 2066 6f75 6e64 2069 6e20 6275 636b 6574   found in bucket
-0001d6f0: 202d 206f 7574 7075 7420 7761 7320 3a20   - output was : 
-0001d700: 7b7d 272e 666f 726d 6174 286f 7574 2e64  {}'.format(out.d
-0001d710: 6563 6f64 650a 2020 2020 2020 2020 2020  ecode.          
-0001d720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d750: 2020 2020 2020 2827 7574 662d 3827 2929        ('utf-8'))
-0001d760: 0a0a 2020 2020 4070 7974 6573 742e 6d61  ..    @pytest.ma
-0001d770: 726b 2e70 6172 616d 6574 7269 7a65 2827  rk.parametrize('
-0001d780: 696e 7661 6c69 645f 6e61 6d65 5f6c 6973  invalid_name_lis
-0001d790: 742c 2073 746f 7265 5f74 7970 6527 2c0a  t, store_type',.
-0001d7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d7b0: 2020 2020 2020 2020 2020 2020 205b 2841               [(A
-0001d7c0: 5753 5f49 4e56 414c 4944 5f4e 414d 4553  WS_INVALID_NAMES
-0001d7d0: 2c20 7374 6f72 6167 655f 6c69 622e 5374  , storage_lib.St
-0001d7e0: 6f72 6554 7970 652e 5333 292c 0a20 2020  oreType.S3),.   
-0001d7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d800: 2020 2020 2020 2020 2020 2028 4743 535f             (GCS_
-0001d810: 494e 5641 4c49 445f 4e41 4d45 532c 2073  INVALID_NAMES, s
-0001d820: 746f 7261 6765 5f6c 6962 2e53 746f 7265  torage_lib.Store
-0001d830: 5479 7065 2e47 4353 292c 0a20 2020 2020  Type.GCS),.     
-0001d840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d850: 2020 2020 2020 2020 2070 7974 6573 742e           pytest.
-0001d860: 7061 7261 6d28 4157 535f 494e 5641 4c49  param(AWS_INVALI
-0001d870: 445f 4e41 4d45 532c 0a20 2020 2020 2020  D_NAMES,.       
+0001c980: 2073 746f 7261 6765 5f6c 6962 2e53 746f   storage_lib.Sto
+0001c990: 7265 5479 7065 2e52 322c 0a20 2020 2020  reType.R2,.     
+0001c9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c9c0: 2020 2020 2020 6d61 726b 733d 7079 7465        marks=pyte
+0001c9d0: 7374 2e6d 6172 6b2e 636c 6f75 6466 6c61  st.mark.cloudfla
+0001c9e0: 7265 295d 290a 2020 2020 6465 6620 7465  re)]).    def te
+0001c9f0: 7374 5f75 706c 6f61 645f 746f 5f65 7869  st_upload_to_exi
+0001ca00: 7374 696e 675f 6275 636b 6574 2873 656c  sting_bucket(sel
+0001ca10: 662c 2065 7874 5f62 7563 6b65 745f 6669  f, ext_bucket_fi
+0001ca20: 7874 7572 652c 2072 6571 7565 7374 2c0a  xture, request,.
+0001ca30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ca40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ca50: 2020 2020 2020 2074 6d70 5f73 6f75 7263         tmp_sourc
+0001ca60: 652c 2073 746f 7265 5f74 7970 6529 3a0a  e, store_type):.
+0001ca70: 2020 2020 2020 2020 2320 5472 6965 7320          # Tries 
+0001ca80: 7570 6c6f 6164 696e 6720 6578 6973 7469  uploading existi
+0001ca90: 6e67 2066 696c 6573 2074 6f20 6e65 776c  ng files to newl
+0001caa0: 7920 6372 6561 7465 6420 6275 636b 6574  y created bucket
+0001cab0: 2028 6f75 7473 6964 6520 6f66 0a20 2020   (outside of.   
+0001cac0: 2020 2020 2023 2073 6b79 2920 616e 6420       # sky) and 
+0001cad0: 7665 7269 6669 6573 2074 6861 7420 6669  verifies that fi
+0001cae0: 6c65 7320 6172 6520 7772 6974 7465 6e2e  les are written.
+0001caf0: 0a20 2020 2020 2020 2062 7563 6b65 745f  .        bucket_
+0001cb00: 6e61 6d65 203d 2072 6571 7565 7374 2e67  name = request.g
+0001cb10: 6574 6669 7874 7572 6576 616c 7565 2865  etfixturevalue(e
+0001cb20: 7874 5f62 7563 6b65 745f 6669 7874 7572  xt_bucket_fixtur
+0001cb30: 6529 0a20 2020 2020 2020 2073 746f 7261  e).        stora
+0001cb40: 6765 5f6f 626a 203d 2073 746f 7261 6765  ge_obj = storage
+0001cb50: 5f6c 6962 2e53 746f 7261 6765 286e 616d  _lib.Storage(nam
+0001cb60: 653d 6275 636b 6574 5f6e 616d 652c 2073  e=bucket_name, s
+0001cb70: 6f75 7263 653d 746d 705f 736f 7572 6365  ource=tmp_source
+0001cb80: 290a 2020 2020 2020 2020 7374 6f72 6167  ).        storag
+0001cb90: 655f 6f62 6a2e 6164 645f 7374 6f72 6528  e_obj.add_store(
+0001cba0: 7374 6f72 655f 7479 7065 290a 0a20 2020  store_type)..   
+0001cbb0: 2020 2020 2023 2043 6865 636b 2069 6620       # Check if 
+0001cbc0: 746d 705f 736f 7572 6365 2f74 6d70 2d66  tmp_source/tmp-f
+0001cbd0: 696c 6520 6578 6973 7473 2069 6e20 7468  ile exists in th
+0001cbe0: 6520 6275 636b 6574 2075 7369 6e67 2061  e bucket using a
+0001cbf0: 7773 2063 6c69 0a20 2020 2020 2020 206f  ws cli.        o
+0001cc00: 7574 203d 2073 7562 7072 6f63 6573 732e  ut = subprocess.
+0001cc10: 6368 6563 6b5f 6f75 7470 7574 2873 656c  check_output(sel
+0001cc20: 662e 636c 695f 6c73 5f63 6d64 2873 746f  f.cli_ls_cmd(sto
+0001cc30: 7265 5f74 7970 652c 2062 7563 6b65 745f  re_type, bucket_
+0001cc40: 6e61 6d65 292c 0a20 2020 2020 2020 2020  name),.         
+0001cc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cc60: 2020 2020 2020 2020 2020 2020 2073 6865               she
+0001cc70: 6c6c 3d54 7275 6529 0a20 2020 2020 2020  ll=True).       
+0001cc80: 2061 7373 6572 7420 2774 6d70 2d66 696c   assert 'tmp-fil
+0001cc90: 6527 2069 6e20 6f75 742e 6465 636f 6465  e' in out.decode
+0001cca0: 2827 7574 662d 3827 292c 205c 0a20 2020  ('utf-8'), \.   
+0001ccb0: 2020 2020 2020 2020 2027 4669 6c65 206e           'File n
+0001ccc0: 6f74 2066 6f75 6e64 2069 6e20 6275 636b  ot found in buck
+0001ccd0: 6574 202d 206f 7574 7075 7420 7761 7320  et - output was 
+0001cce0: 3a20 7b7d 272e 666f 726d 6174 286f 7574  : {}'.format(out
+0001ccf0: 2e64 6563 6f64 650a 2020 2020 2020 2020  .decode.        
+0001cd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cd10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cd30: 2020 2020 2020 2020 2827 7574 662d 3827          ('utf-8'
+0001cd40: 2929 0a0a 2020 2020 2020 2020 2320 4368  ))..        # Ch
+0001cd50: 6563 6b20 7379 6d6c 696e 6b73 202d 2073  eck symlinks - s
+0001cd60: 796d 6c69 6e6b 7320 646f 6e27 7420 6765  ymlinks don't ge
+0001cd70: 7420 636f 7069 6564 2062 7920 736b 7920  t copied by sky 
+0001cd80: 7374 6f72 6167 650a 2020 2020 2020 2020  storage.        
+0001cd90: 6173 7365 7274 2028 7061 7468 6c69 622e  assert (pathlib.
+0001cda0: 5061 7468 2874 6d70 5f73 6f75 7263 6529  Path(tmp_source)
+0001cdb0: 202f 2027 6369 7263 6c65 2d6c 696e 6b27   / 'circle-link'
+0001cdc0: 292e 6973 5f73 796d 6c69 6e6b 2829 2c20  ).is_symlink(), 
+0001cdd0: 280a 2020 2020 2020 2020 2020 2020 2763  (.            'c
+0001cde0: 6972 636c 652d 6c69 6e6b 2077 6173 206e  ircle-link was n
+0001cdf0: 6f74 2066 6f75 6e64 2069 6e20 7468 6520  ot found in the 
+0001ce00: 7570 6c6f 6164 2073 6f75 7263 6520 2d20  upload source - 
+0001ce10: 270a 2020 2020 2020 2020 2020 2020 2761  '.            'a
+0001ce20: 7265 2074 6865 2074 6573 7420 6669 7874  re the test fixt
+0001ce30: 7572 6573 2063 6f72 7265 6374 3f27 290a  ures correct?').
+0001ce40: 2020 2020 2020 2020 6173 7365 7274 2027          assert '
+0001ce50: 6369 7263 6c65 2d6c 696e 6b27 206e 6f74  circle-link' not
+0001ce60: 2069 6e20 6f75 742e 6465 636f 6465 2827   in out.decode('
+0001ce70: 7574 662d 3827 292c 2028 0a20 2020 2020  utf-8'), (.     
+0001ce80: 2020 2020 2020 2027 5379 6d6c 696e 6b20         'Symlink 
+0001ce90: 666f 756e 6420 696e 2062 7563 6b65 7420  found in bucket 
+0001cea0: 2d20 6c73 206f 7574 7075 7420 7761 7320  - ls output was 
+0001ceb0: 3a20 7b7d 272e 666f 726d 6174 280a 2020  : {}'.format(.  
+0001cec0: 2020 2020 2020 2020 2020 2020 2020 6f75                ou
+0001ced0: 742e 6465 636f 6465 2827 7574 662d 3827  t.decode('utf-8'
+0001cee0: 2929 290a 0a20 2020 2020 2020 2023 2052  )))..        # R
+0001cef0: 756e 2073 6b79 2073 746f 7261 6765 206c  un sky storage l
+0001cf00: 7320 746f 2063 6865 636b 2069 6620 7374  s to check if st
+0001cf10: 6f72 6167 6520 6f62 6a65 6374 2065 7869  orage object exi
+0001cf20: 7374 7320 696e 2074 6865 206f 7574 7075  sts in the outpu
+0001cf30: 742e 0a20 2020 2020 2020 2023 2049 7420  t..        # It 
+0001cf40: 7368 6f75 6c64 206e 6f74 2065 7869 7374  should not exist
+0001cf50: 2062 6563 6175 7365 2074 6865 2062 7563   because the buc
+0001cf60: 6b65 7420 7761 7320 6372 6561 7465 6420  ket was created 
+0001cf70: 6578 7465 726e 616c 6c79 2e0a 2020 2020  externally..    
+0001cf80: 2020 2020 6f75 7420 3d20 7375 6270 726f      out = subpro
+0001cf90: 6365 7373 2e63 6865 636b 5f6f 7574 7075  cess.check_outpu
+0001cfa0: 7428 5b27 736b 7927 2c20 2773 746f 7261  t(['sky', 'stora
+0001cfb0: 6765 272c 2027 6c73 275d 290a 2020 2020  ge', 'ls']).    
+0001cfc0: 2020 2020 6173 7365 7274 2073 746f 7261      assert stora
+0001cfd0: 6765 5f6f 626a 2e6e 616d 6520 6e6f 7420  ge_obj.name not 
+0001cfe0: 696e 206f 7574 2e64 6563 6f64 6528 2775  in out.decode('u
+0001cff0: 7466 2d38 2729 0a0a 2020 2020 6465 6620  tf-8')..    def 
+0001d000: 7465 7374 5f63 6f70 795f 6d6f 756e 745f  test_copy_mount_
+0001d010: 6578 6973 7469 6e67 5f73 746f 7261 6765  existing_storage
+0001d020: 2873 656c 662c 0a20 2020 2020 2020 2020  (self,.         
+0001d030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d050: 746d 705f 636f 7079 5f6d 6e74 5f65 7869  tmp_copy_mnt_exi
+0001d060: 7374 696e 675f 7374 6f72 6167 655f 6f62  sting_storage_ob
+0001d070: 6a29 3a0a 2020 2020 2020 2020 2320 4372  j):.        # Cr
+0001d080: 6561 7465 7320 6120 6275 636b 6574 2077  eates a bucket w
+0001d090: 6974 6820 6e6f 2073 6f75 7263 6520 696e  ith no source in
+0001d0a0: 204d 4f55 4e54 206d 6f64 6520 2865 6d70   MOUNT mode (emp
+0001d0b0: 7479 2062 7563 6b65 7429 2c20 616e 640a  ty bucket), and.
+0001d0c0: 2020 2020 2020 2020 2320 7468 656e 2074          # then t
+0001d0d0: 7269 6573 2074 6f20 6c6f 6164 2074 6865  ries to load the
+0001d0e0: 2073 616d 6520 7374 6f72 6167 6520 696e   same storage in
+0001d0f0: 2043 4f50 5920 6d6f 6465 2e0a 2020 2020   COPY mode..    
+0001d100: 2020 2020 746d 705f 636f 7079 5f6d 6e74      tmp_copy_mnt
+0001d110: 5f65 7869 7374 696e 675f 7374 6f72 6167  _existing_storag
+0001d120: 655f 6f62 6a2e 6164 645f 7374 6f72 6528  e_obj.add_store(
+0001d130: 7374 6f72 6167 655f 6c69 622e 5374 6f72  storage_lib.Stor
+0001d140: 6554 7970 652e 5333 290a 2020 2020 2020  eType.S3).      
+0001d150: 2020 7374 6f72 6167 655f 6e61 6d65 203d    storage_name =
+0001d160: 2074 6d70 5f63 6f70 795f 6d6e 745f 6578   tmp_copy_mnt_ex
+0001d170: 6973 7469 6e67 5f73 746f 7261 6765 5f6f  isting_storage_o
+0001d180: 626a 2e6e 616d 650a 0a20 2020 2020 2020  bj.name..       
+0001d190: 2023 2043 6865 636b 2060 736b 7920 7374   # Check `sky st
+0001d1a0: 6f72 6167 6520 6c73 6020 746f 2065 6e73  orage ls` to ens
+0001d1b0: 7572 6520 7374 6f72 6167 6520 6f62 6a65  ure storage obje
+0001d1c0: 6374 2065 7869 7374 730a 2020 2020 2020  ct exists.      
+0001d1d0: 2020 6f75 7420 3d20 7375 6270 726f 6365    out = subproce
+0001d1e0: 7373 2e63 6865 636b 5f6f 7574 7075 7428  ss.check_output(
+0001d1f0: 5b27 736b 7927 2c20 2773 746f 7261 6765  ['sky', 'storage
+0001d200: 272c 2027 6c73 275d 292e 6465 636f 6465  ', 'ls']).decode
+0001d210: 2827 7574 662d 3827 290a 2020 2020 2020  ('utf-8').      
+0001d220: 2020 6173 7365 7274 2073 746f 7261 6765    assert storage
+0001d230: 5f6e 616d 6520 696e 206f 7574 2c20 6627  _name in out, f'
+0001d240: 5374 6f72 6167 6520 7b73 746f 7261 6765  Storage {storage
+0001d250: 5f6e 616d 657d 206e 6f74 2066 6f75 6e64  _name} not found
+0001d260: 2069 6e20 736b 7920 7374 6f72 6167 6520   in sky storage 
+0001d270: 6c73 2e27 0a0a 2020 2020 4070 7974 6573  ls.'..    @pytes
+0001d280: 742e 6d61 726b 2e70 6172 616d 6574 7269  t.mark.parametri
+0001d290: 7a65 2827 7374 6f72 655f 7479 7065 272c  ze('store_type',
+0001d2a0: 205b 0a20 2020 2020 2020 2073 746f 7261   [.        stora
+0001d2b0: 6765 5f6c 6962 2e53 746f 7265 5479 7065  ge_lib.StoreType
+0001d2c0: 2e53 332c 2073 746f 7261 6765 5f6c 6962  .S3, storage_lib
+0001d2d0: 2e53 746f 7265 5479 7065 2e47 4353 2c0a  .StoreType.GCS,.
+0001d2e0: 2020 2020 2020 2020 7079 7465 7374 2e70          pytest.p
+0001d2f0: 6172 616d 2873 746f 7261 6765 5f6c 6962  aram(storage_lib
+0001d300: 2e53 746f 7265 5479 7065 2e52 322c 206d  .StoreType.R2, m
+0001d310: 6172 6b73 3d70 7974 6573 742e 6d61 726b  arks=pytest.mark
+0001d320: 2e63 6c6f 7564 666c 6172 6529 0a20 2020  .cloudflare).   
+0001d330: 205d 290a 2020 2020 6465 6620 7465 7374   ]).    def test
+0001d340: 5f6c 6973 745f 736f 7572 6365 2873 656c  _list_source(sel
+0001d350: 662c 2074 6d70 5f6c 6f63 616c 5f6c 6973  f, tmp_local_lis
+0001d360: 745f 7374 6f72 6167 655f 6f62 6a2c 2073  t_storage_obj, s
+0001d370: 746f 7265 5f74 7970 6529 3a0a 2020 2020  tore_type):.    
+0001d380: 2020 2020 2320 5573 6573 2061 206c 6973      # Uses a lis
+0001d390: 7420 696e 2074 6865 2073 6f75 7263 6520  t in the source 
+0001d3a0: 6669 656c 6420 746f 2073 7065 6369 6679  field to specify
+0001d3b0: 2061 2066 696c 6520 616e 6420 6120 6469   a file and a di
+0001d3c0: 7265 6374 6f72 7920 746f 0a20 2020 2020  rectory to.     
+0001d3d0: 2020 2023 2062 6520 7570 6c6f 6164 6564     # be uploaded
+0001d3e0: 2074 6f20 7468 6520 7374 6f72 6167 6520   to the storage 
+0001d3f0: 6f62 6a65 6374 2e0a 2020 2020 2020 2020  object..        
+0001d400: 746d 705f 6c6f 6361 6c5f 6c69 7374 5f73  tmp_local_list_s
+0001d410: 746f 7261 6765 5f6f 626a 2e61 6464 5f73  torage_obj.add_s
+0001d420: 746f 7265 2873 746f 7265 5f74 7970 6529  tore(store_type)
+0001d430: 0a0a 2020 2020 2020 2020 2320 4368 6563  ..        # Chec
+0001d440: 6b20 6966 2074 6d70 2d66 696c 6520 6578  k if tmp-file ex
+0001d450: 6973 7473 2069 6e20 7468 6520 6275 636b  ists in the buck
+0001d460: 6574 2072 6f6f 7420 7573 696e 6720 636c  et root using cl
+0001d470: 690a 2020 2020 2020 2020 6f75 7420 3d20  i.        out = 
+0001d480: 7375 6270 726f 6365 7373 2e63 6865 636b  subprocess.check
+0001d490: 5f6f 7574 7075 7428 7365 6c66 2e63 6c69  _output(self.cli
+0001d4a0: 5f6c 735f 636d 6428 0a20 2020 2020 2020  _ls_cmd(.       
+0001d4b0: 2020 2020 2073 746f 7265 5f74 7970 652c       store_type,
+0001d4c0: 2074 6d70 5f6c 6f63 616c 5f6c 6973 745f   tmp_local_list_
+0001d4d0: 7374 6f72 6167 655f 6f62 6a2e 6e61 6d65  storage_obj.name
+0001d4e0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+0001d4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d500: 2020 2020 2020 2020 2073 6865 6c6c 3d54           shell=T
+0001d510: 7275 6529 0a20 2020 2020 2020 2061 7373  rue).        ass
+0001d520: 6572 7420 2774 6d70 2d66 696c 6527 2069  ert 'tmp-file' i
+0001d530: 6e20 6f75 742e 6465 636f 6465 2827 7574  n out.decode('ut
+0001d540: 662d 3827 292c 205c 0a20 2020 2020 2020  f-8'), \.       
+0001d550: 2020 2020 2027 4669 6c65 206e 6f74 2066       'File not f
+0001d560: 6f75 6e64 2069 6e20 6275 636b 6574 202d  ound in bucket -
+0001d570: 206f 7574 7075 7420 7761 7320 3a20 7b7d   output was : {}
+0001d580: 272e 666f 726d 6174 286f 7574 2e64 6563  '.format(out.dec
+0001d590: 6f64 650a 2020 2020 2020 2020 2020 2020  ode.            
+0001d5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d5d0: 2020 2020 2827 7574 662d 3827 2929 0a0a      ('utf-8'))..
+0001d5e0: 2020 2020 2020 2020 2320 4368 6563 6b20          # Check 
+0001d5f0: 6966 2074 6d70 2d66 696c 6520 6578 6973  if tmp-file exis
+0001d600: 7473 2069 6e20 7468 6520 6275 636b 6574  ts in the bucket
+0001d610: 2f74 6d70 2d73 6f75 7263 6520 7573 696e  /tmp-source usin
+0001d620: 6720 636c 690a 2020 2020 2020 2020 6f75  g cli.        ou
+0001d630: 7420 3d20 7375 6270 726f 6365 7373 2e63  t = subprocess.c
+0001d640: 6865 636b 5f6f 7574 7075 7428 7365 6c66  heck_output(self
+0001d650: 2e63 6c69 5f6c 735f 636d 6428 0a20 2020  .cli_ls_cmd(.   
+0001d660: 2020 2020 2020 2020 2073 746f 7265 5f74           store_t
+0001d670: 7970 652c 2074 6d70 5f6c 6f63 616c 5f6c  ype, tmp_local_l
+0001d680: 6973 745f 7374 6f72 6167 655f 6f62 6a2e  ist_storage_obj.
+0001d690: 6e61 6d65 2c20 2774 6d70 2d73 6f75 7263  name, 'tmp-sourc
+0001d6a0: 652f 2729 2c0a 2020 2020 2020 2020 2020  e/'),.          
+0001d6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d6c0: 2020 2020 2020 2020 2020 2020 7368 656c              shel
+0001d6d0: 6c3d 5472 7565 290a 2020 2020 2020 2020  l=True).        
+0001d6e0: 6173 7365 7274 2027 746d 702d 6669 6c65  assert 'tmp-file
+0001d6f0: 2720 696e 206f 7574 2e64 6563 6f64 6528  ' in out.decode(
+0001d700: 2775 7466 2d38 2729 2c20 5c0a 2020 2020  'utf-8'), \.    
+0001d710: 2020 2020 2020 2020 2746 696c 6520 6e6f          'File no
+0001d720: 7420 666f 756e 6420 696e 2062 7563 6b65  t found in bucke
+0001d730: 7420 2d20 6f75 7470 7574 2077 6173 203a  t - output was :
+0001d740: 207b 7d27 2e66 6f72 6d61 7428 6f75 742e   {}'.format(out.
+0001d750: 6465 636f 6465 0a20 2020 2020 2020 2020  decode.         
+0001d760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d790: 2020 2020 2020 2028 2775 7466 2d38 2729         ('utf-8')
+0001d7a0: 290a 0a20 2020 2040 7079 7465 7374 2e6d  )..    @pytest.m
+0001d7b0: 6172 6b2e 7061 7261 6d65 7472 697a 6528  ark.parametrize(
+0001d7c0: 2769 6e76 616c 6964 5f6e 616d 655f 6c69  'invalid_name_li
+0001d7d0: 7374 2c20 7374 6f72 655f 7479 7065 272c  st, store_type',
+0001d7e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001d7f0: 2020 2020 2020 2020 2020 2020 2020 5b28                [(
+0001d800: 4157 535f 494e 5641 4c49 445f 4e41 4d45  AWS_INVALID_NAME
+0001d810: 532c 2073 746f 7261 6765 5f6c 6962 2e53  S, storage_lib.S
+0001d820: 746f 7265 5479 7065 2e53 3329 2c0a 2020  toreType.S3),.  
+0001d830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d840: 2020 2020 2020 2020 2020 2020 2847 4353              (GCS
+0001d850: 5f49 4e56 414c 4944 5f4e 414d 4553 2c20  _INVALID_NAMES, 
+0001d860: 7374 6f72 6167 655f 6c69 622e 5374 6f72  storage_lib.Stor
+0001d870: 6554 7970 652e 4743 5329 2c0a 2020 2020  eType.GCS),.    
 0001d880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d8a0: 2020 2020 7374 6f72 6167 655f 6c69 622e      storage_lib.
-0001d8b0: 5374 6f72 6554 7970 652e 5232 2c0a 2020  StoreType.R2,.  
+0001d890: 2020 2020 2020 2020 2020 7079 7465 7374            pytest
+0001d8a0: 2e70 6172 616d 2841 5753 5f49 4e56 414c  .param(AWS_INVAL
+0001d8b0: 4944 5f4e 414d 4553 2c0a 2020 2020 2020  ID_NAMES,.      
 0001d8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001d8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d8e0: 2020 2020 2020 2020 206d 6172 6b73 3d70           marks=p
-0001d8f0: 7974 6573 742e 6d61 726b 2e63 6c6f 7564  ytest.mark.cloud
-0001d900: 666c 6172 6529 5d29 0a20 2020 2064 6566  flare)]).    def
-0001d910: 2074 6573 745f 696e 7661 6c69 645f 6e61   test_invalid_na
-0001d920: 6d65 7328 7365 6c66 2c20 696e 7661 6c69  mes(self, invali
-0001d930: 645f 6e61 6d65 5f6c 6973 742c 2073 746f  d_name_list, sto
-0001d940: 7265 5f74 7970 6529 3a0a 2020 2020 2020  re_type):.      
-0001d950: 2020 2320 5573 6573 2061 206c 6973 7420    # Uses a list 
-0001d960: 696e 2074 6865 2073 6f75 7263 6520 6669  in the source fi
-0001d970: 656c 6420 746f 2073 7065 6369 6679 2061  eld to specify a
-0001d980: 2066 696c 6520 616e 6420 6120 6469 7265   file and a dire
-0001d990: 6374 6f72 7920 746f 0a20 2020 2020 2020  ctory to.       
-0001d9a0: 2023 2062 6520 7570 6c6f 6164 6564 2074   # be uploaded t
-0001d9b0: 6f20 7468 6520 7374 6f72 6167 6520 6f62  o the storage ob
-0001d9c0: 6a65 6374 2e0a 2020 2020 2020 2020 666f  ject..        fo
-0001d9d0: 7220 6e61 6d65 2069 6e20 696e 7661 6c69  r name in invali
-0001d9e0: 645f 6e61 6d65 5f6c 6973 743a 0a20 2020  d_name_list:.   
-0001d9f0: 2020 2020 2020 2020 2077 6974 6820 7079           with py
-0001da00: 7465 7374 2e72 6169 7365 7328 736b 792e  test.raises(sky.
-0001da10: 6578 6365 7074 696f 6e73 2e53 746f 7261  exceptions.Stora
-0001da20: 6765 4e61 6d65 4572 726f 7229 3a0a 2020  geNameError):.  
-0001da30: 2020 2020 2020 2020 2020 2020 2020 7374                st
-0001da40: 6f72 6167 655f 6f62 6a20 3d20 7374 6f72  orage_obj = stor
-0001da50: 6167 655f 6c69 622e 5374 6f72 6167 6528  age_lib.Storage(
-0001da60: 6e61 6d65 3d6e 616d 6529 0a20 2020 2020  name=name).     
-0001da70: 2020 2020 2020 2020 2020 2073 746f 7261             stora
-0001da80: 6765 5f6f 626a 2e61 6464 5f73 746f 7265  ge_obj.add_store
-0001da90: 2873 746f 7265 5f74 7970 6529 0a0a 0a23  (store_type)...#
-0001daa0: 202d 2d2d 2d2d 2d2d 2d2d 2d20 5465 7374   ---------- Test
-0001dab0: 696e 6720 5941 4d4c 2053 7065 6373 202d  ing YAML Specs -
-0001dac0: 2d2d 2d2d 2d2d 2d2d 2d0a 2320 4f75 7220  ---------.# Our 
-0001dad0: 736b 7920 7374 6f72 6167 6520 7265 7175  sky storage requ
-0001dae0: 6972 6573 2063 7265 6465 6e74 6961 6c73  ires credentials
-0001daf0: 2074 6f20 6368 6563 6b20 7468 6520 6275   to check the bu
-0001db00: 636b 6574 2065 7869 7374 616e 6365 2077  cket existance w
-0001db10: 6865 6e0a 2320 6c6f 6164 696e 6720 6120  hen.# loading a 
-0001db20: 7461 736b 2066 726f 6d20 7468 6520 7961  task from the ya
-0001db30: 6d6c 2066 696c 652c 2073 6f20 7765 2063  ml file, so we c
-0001db40: 616e 6e6f 7420 6d61 6b65 2069 7420 6120  annot make it a 
-0001db50: 756e 6974 2074 6573 742e 0a63 6c61 7373  unit test..class
-0001db60: 2054 6573 7459 616d 6c53 7065 6373 3a0a   TestYamlSpecs:.
-0001db70: 2020 2020 2320 544f 444f 287a 6877 7529      # TODO(zhwu)
-0001db80: 3a20 4164 6420 7465 7374 2066 6f72 2060  : Add test for `
-0001db90: 746f 5f79 616d 6c5f 636f 6e66 6967 6020  to_yaml_config` 
-0001dba0: 666f 7220 7468 6520 5374 6f72 6167 6520  for the Storage 
-0001dbb0: 6f62 6a65 6374 2e0a 2020 2020 2320 2057  object..    #  W
-0001dbc0: 6520 7368 6f75 6c64 206e 6f74 2075 7365  e should not use
-0001dbd0: 2060 6578 616d 706c 6573 2f73 746f 7261   `examples/stora
-0001dbe0: 6765 5f64 656d 6f2e 7961 6d6c 6020 6865  ge_demo.yaml` he
-0001dbf0: 7265 2c20 7369 6e63 6520 6974 2072 6571  re, since it req
-0001dc00: 7569 7265 730a 2020 2020 2320 2075 7365  uires.    #  use
-0001dc10: 7273 2074 6f20 656e 7375 7265 2062 7563  rs to ensure buc
-0001dc20: 6b65 7420 6e61 6d65 7320 746f 206e 6f74  ket names to not
-0001dc30: 2065 7869 7374 2061 6e64 2f6f 7220 6265   exist and/or be
-0001dc40: 2075 6e69 7175 652e 0a20 2020 205f 5445   unique..    _TE
-0001dc50: 5354 5f59 414d 4c5f 5041 5448 5320 3d20  ST_YAML_PATHS = 
-0001dc60: 5b0a 2020 2020 2020 2020 2765 7861 6d70  [.        'examp
-0001dc70: 6c65 732f 6d69 6e69 6d61 6c2e 7961 6d6c  les/minimal.yaml
-0001dc80: 272c 2027 6578 616d 706c 6573 2f6d 616e  ', 'examples/man
-0001dc90: 6167 6564 5f73 706f 742e 7961 6d6c 272c  aged_spot.yaml',
-0001dca0: 0a20 2020 2020 2020 2027 6578 616d 706c  .        'exampl
-0001dcb0: 6573 2f75 7369 6e67 5f66 696c 655f 6d6f  es/using_file_mo
-0001dcc0: 756e 7473 2e79 616d 6c27 2c20 2765 7861  unts.yaml', 'exa
-0001dcd0: 6d70 6c65 732f 7265 736e 6574 5f61 7070  mples/resnet_app
-0001dce0: 2e79 616d 6c27 2c0a 2020 2020 2020 2020  .yaml',.        
-0001dcf0: 2765 7861 6d70 6c65 732f 6d75 6c74 695f  'examples/multi_
-0001dd00: 686f 7374 6e61 6d65 2e79 616d 6c27 0a20  hostname.yaml'. 
-0001dd10: 2020 205d 0a0a 2020 2020 6465 6620 5f69     ]..    def _i
-0001dd20: 735f 6469 6374 5f73 7562 7365 7428 7365  s_dict_subset(se
-0001dd30: 6c66 2c20 6431 2c20 6432 293a 0a20 2020  lf, d1, d2):.   
-0001dd40: 2020 2020 2022 2222 4368 6563 6b20 6966       """Check if
-0001dd50: 2064 3120 6973 2074 6865 2073 7562 7365   d1 is the subse
-0001dd60: 7420 6f66 2064 322e 2222 220a 2020 2020  t of d2.""".    
-0001dd70: 2020 2020 666f 7220 6b2c 2076 2069 6e20      for k, v in 
-0001dd80: 6431 2e69 7465 6d73 2829 3a0a 2020 2020  d1.items():.    
-0001dd90: 2020 2020 2020 2020 6966 206b 206e 6f74          if k not
-0001dda0: 2069 6e20 6432 3a0a 2020 2020 2020 2020   in d2:.        
-0001ddb0: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-0001ddc0: 7461 6e63 6528 762c 206c 6973 7429 206f  tance(v, list) o
-0001ddd0: 7220 6973 696e 7374 616e 6365 2876 2c20  r isinstance(v, 
-0001dde0: 6469 6374 293a 0a20 2020 2020 2020 2020  dict):.         
-0001ddf0: 2020 2020 2020 2020 2020 2061 7373 6572             asser
-0001de00: 7420 6c65 6e28 7629 203d 3d20 302c 2028  t len(v) == 0, (
-0001de10: 6b2c 2076 290a 2020 2020 2020 2020 2020  k, v).          
-0001de20: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0001de30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001de40: 6173 7365 7274 2046 616c 7365 2c20 286b  assert False, (k
-0001de50: 2c20 7629 0a20 2020 2020 2020 2020 2020  , v).           
-0001de60: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
-0001de70: 2876 2c20 6469 6374 293a 0a20 2020 2020  (v, dict):.     
-0001de80: 2020 2020 2020 2020 2020 2061 7373 6572             asser
-0001de90: 7420 6973 696e 7374 616e 6365 2864 325b  t isinstance(d2[
-0001dea0: 6b5d 2c20 6469 6374 292c 2028 6b2c 2076  k], dict), (k, v
-0001deb0: 2c20 6432 290a 2020 2020 2020 2020 2020  , d2).          
-0001dec0: 2020 2020 2020 7365 6c66 2e5f 6973 5f64        self._is_d
-0001ded0: 6963 745f 7375 6273 6574 2876 2c20 6432  ict_subset(v, d2
-0001dee0: 5b6b 5d29 0a20 2020 2020 2020 2020 2020  [k]).           
-0001def0: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
-0001df00: 2876 2c20 7374 7229 3a0a 2020 2020 2020  (v, str):.      
-0001df10: 2020 2020 2020 2020 2020 6966 206b 203d            if k =
-0001df20: 3d20 2761 6363 656c 6572 6174 6f72 7327  = 'accelerators'
-0001df30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001df40: 2020 2020 2020 7265 736f 7572 6365 7320        resources 
-0001df50: 3d20 736b 792e 5265 736f 7572 6365 7328  = sky.Resources(
-0001df60: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0001df70: 2020 2020 2020 7265 736f 7572 6365 732e        resources.
-0001df80: 5f73 6574 5f61 6363 656c 6572 6174 6f72  _set_accelerator
-0001df90: 7328 762c 204e 6f6e 6529 0a20 2020 2020  s(v, None).     
-0001dfa0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-0001dfb0: 7373 6572 7420 7265 736f 7572 6365 732e  ssert resources.
-0001dfc0: 6163 6365 6c65 7261 746f 7273 203d 3d20  accelerators == 
-0001dfd0: 6432 5b6b 5d2c 2028 6b2c 2076 2c20 6432  d2[k], (k, v, d2
-0001dfe0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0001dff0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0001e000: 2020 2020 2020 2020 2020 2020 6173 7365              asse
-0001e010: 7274 2076 2e6c 6f77 6572 2829 203d 3d20  rt v.lower() == 
-0001e020: 6432 5b6b 5d2e 6c6f 7765 7228 292c 2028  d2[k].lower(), (
-0001e030: 6b2c 2076 2c20 6432 5b6b 5d29 0a20 2020  k, v, d2[k]).   
-0001e040: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-0001e050: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-0001e060: 7373 6572 7420 7620 3d3d 2064 325b 6b5d  ssert v == d2[k]
-0001e070: 2c20 286b 2c20 762c 2064 325b 6b5d 290a  , (k, v, d2[k]).
-0001e080: 0a20 2020 2064 6566 205f 6368 6563 6b5f  .    def _check_
-0001e090: 6571 7569 7661 6c65 6e74 2873 656c 662c  equivalent(self,
-0001e0a0: 2079 616d 6c5f 7061 7468 293a 0a20 2020   yaml_path):.   
-0001e0b0: 2020 2020 2022 2222 4368 6563 6b20 6966       """Check if
-0001e0c0: 2074 6865 2079 616d 6c20 6973 2065 7175   the yaml is equ
-0001e0d0: 6976 616c 656e 7420 6166 7465 7220 6c6f  ivalent after lo
-0001e0e0: 6164 2061 6e64 2064 756d 7020 6167 6169  ad and dump agai
-0001e0f0: 6e2e 2222 220a 2020 2020 2020 2020 6f72  n.""".        or
-0001e100: 6967 696e 5f74 6173 6b5f 636f 6e66 6967  igin_task_config
-0001e110: 203d 2063 6f6d 6d6f 6e5f 7574 696c 732e   = common_utils.
-0001e120: 7265 6164 5f79 616d 6c28 7961 6d6c 5f70  read_yaml(yaml_p
-0001e130: 6174 6829 0a0a 2020 2020 2020 2020 7461  ath)..        ta
-0001e140: 736b 203d 2073 6b79 2e54 6173 6b2e 6672  sk = sky.Task.fr
-0001e150: 6f6d 5f79 616d 6c28 7961 6d6c 5f70 6174  om_yaml(yaml_pat
-0001e160: 6829 0a20 2020 2020 2020 206e 6577 5f74  h).        new_t
-0001e170: 6173 6b5f 636f 6e66 6967 203d 2074 6173  ask_config = tas
-0001e180: 6b2e 746f 5f79 616d 6c5f 636f 6e66 6967  k.to_yaml_config
-0001e190: 2829 0a20 2020 2020 2020 2023 2064 3120  ().        # d1 
-0001e1a0: 3c3d 2064 320a 2020 2020 2020 2020 7365  <= d2.        se
-0001e1b0: 6c66 2e5f 6973 5f64 6963 745f 7375 6273  lf._is_dict_subs
-0001e1c0: 6574 286f 7269 6769 6e5f 7461 736b 5f63  et(origin_task_c
-0001e1d0: 6f6e 6669 672c 206e 6577 5f74 6173 6b5f  onfig, new_task_
-0001e1e0: 636f 6e66 6967 290a 0a20 2020 2064 6566  config)..    def
-0001e1f0: 2074 6573 745f 6c6f 6164 5f64 756d 705f   test_load_dump_
-0001e200: 7961 6d6c 5f63 6f6e 6669 675f 6571 7569  yaml_config_equi
-0001e210: 7661 6c65 6e74 2873 656c 6629 3a0a 2020  valent(self):.  
-0001e220: 2020 2020 2020 2222 2254 6573 7420 6966        """Test if
-0001e230: 2074 6865 2079 616d 6c20 636f 6e66 6967   the yaml config
-0001e240: 2069 7320 6571 7569 7661 6c65 6e74 2061   is equivalent a
-0001e250: 6674 6572 206c 6f61 6420 616e 6420 6475  fter load and du
-0001e260: 6d70 2061 6761 696e 2e22 2222 0a20 2020  mp again.""".   
-0001e270: 2020 2020 2070 6174 686c 6962 2e50 6174       pathlib.Pat
-0001e280: 6828 277e 2f64 6174 6173 6574 7327 292e  h('~/datasets').
-0001e290: 6578 7061 6e64 7573 6572 2829 2e6d 6b64  expanduser().mkd
-0001e2a0: 6972 2865 7869 7374 5f6f 6b3d 5472 7565  ir(exist_ok=True
-0001e2b0: 290a 2020 2020 2020 2020 7061 7468 6c69  ).        pathli
-0001e2c0: 622e 5061 7468 2827 7e2f 746d 7066 696c  b.Path('~/tmpfil
-0001e2d0: 6527 292e 6578 7061 6e64 7573 6572 2829  e').expanduser()
-0001e2e0: 2e74 6f75 6368 2829 0a20 2020 2020 2020  .touch().       
-0001e2f0: 2070 6174 686c 6962 2e50 6174 6828 277e   pathlib.Path('~
-0001e300: 2f2e 7373 6827 292e 6578 7061 6e64 7573  /.ssh').expandus
-0001e310: 6572 2829 2e6d 6b64 6972 2865 7869 7374  er().mkdir(exist
-0001e320: 5f6f 6b3d 5472 7565 290a 2020 2020 2020  _ok=True).      
+0001d8e0: 2020 2020 2073 746f 7261 6765 5f6c 6962       storage_lib
+0001d8f0: 2e53 746f 7265 5479 7065 2e52 322c 0a20  .StoreType.R2,. 
+0001d900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d920: 2020 2020 2020 2020 2020 6d61 726b 733d            marks=
+0001d930: 7079 7465 7374 2e6d 6172 6b2e 636c 6f75  pytest.mark.clou
+0001d940: 6466 6c61 7265 295d 290a 2020 2020 6465  dflare)]).    de
+0001d950: 6620 7465 7374 5f69 6e76 616c 6964 5f6e  f test_invalid_n
+0001d960: 616d 6573 2873 656c 662c 2069 6e76 616c  ames(self, inval
+0001d970: 6964 5f6e 616d 655f 6c69 7374 2c20 7374  id_name_list, st
+0001d980: 6f72 655f 7479 7065 293a 0a20 2020 2020  ore_type):.     
+0001d990: 2020 2023 2055 7365 7320 6120 6c69 7374     # Uses a list
+0001d9a0: 2069 6e20 7468 6520 736f 7572 6365 2066   in the source f
+0001d9b0: 6965 6c64 2074 6f20 7370 6563 6966 7920  ield to specify 
+0001d9c0: 6120 6669 6c65 2061 6e64 2061 2064 6972  a file and a dir
+0001d9d0: 6563 746f 7279 2074 6f0a 2020 2020 2020  ectory to.      
+0001d9e0: 2020 2320 6265 2075 706c 6f61 6465 6420    # be uploaded 
+0001d9f0: 746f 2074 6865 2073 746f 7261 6765 206f  to the storage o
+0001da00: 626a 6563 742e 0a20 2020 2020 2020 2066  bject..        f
+0001da10: 6f72 206e 616d 6520 696e 2069 6e76 616c  or name in inval
+0001da20: 6964 5f6e 616d 655f 6c69 7374 3a0a 2020  id_name_list:.  
+0001da30: 2020 2020 2020 2020 2020 7769 7468 2070            with p
+0001da40: 7974 6573 742e 7261 6973 6573 2873 6b79  ytest.raises(sky
+0001da50: 2e65 7863 6570 7469 6f6e 732e 5374 6f72  .exceptions.Stor
+0001da60: 6167 654e 616d 6545 7272 6f72 293a 0a20  ageNameError):. 
+0001da70: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001da80: 746f 7261 6765 5f6f 626a 203d 2073 746f  torage_obj = sto
+0001da90: 7261 6765 5f6c 6962 2e53 746f 7261 6765  rage_lib.Storage
+0001daa0: 286e 616d 653d 6e61 6d65 290a 2020 2020  (name=name).    
+0001dab0: 2020 2020 2020 2020 2020 2020 7374 6f72              stor
+0001dac0: 6167 655f 6f62 6a2e 6164 645f 7374 6f72  age_obj.add_stor
+0001dad0: 6528 7374 6f72 655f 7479 7065 290a 0a0a  e(store_type)...
+0001dae0: 2320 2d2d 2d2d 2d2d 2d2d 2d2d 2054 6573  # ---------- Tes
+0001daf0: 7469 6e67 2059 414d 4c20 5370 6563 7320  ting YAML Specs 
+0001db00: 2d2d 2d2d 2d2d 2d2d 2d2d 0a23 204f 7572  ----------.# Our
+0001db10: 2073 6b79 2073 746f 7261 6765 2072 6571   sky storage req
+0001db20: 7569 7265 7320 6372 6564 656e 7469 616c  uires credential
+0001db30: 7320 746f 2063 6865 636b 2074 6865 2062  s to check the b
+0001db40: 7563 6b65 7420 6578 6973 7461 6e63 6520  ucket existance 
+0001db50: 7768 656e 0a23 206c 6f61 6469 6e67 2061  when.# loading a
+0001db60: 2074 6173 6b20 6672 6f6d 2074 6865 2079   task from the y
+0001db70: 616d 6c20 6669 6c65 2c20 736f 2077 6520  aml file, so we 
+0001db80: 6361 6e6e 6f74 206d 616b 6520 6974 2061  cannot make it a
+0001db90: 2075 6e69 7420 7465 7374 2e0a 636c 6173   unit test..clas
+0001dba0: 7320 5465 7374 5961 6d6c 5370 6563 733a  s TestYamlSpecs:
+0001dbb0: 0a20 2020 2023 2054 4f44 4f28 7a68 7775  .    # TODO(zhwu
+0001dbc0: 293a 2041 6464 2074 6573 7420 666f 7220  ): Add test for 
+0001dbd0: 6074 6f5f 7961 6d6c 5f63 6f6e 6669 6760  `to_yaml_config`
+0001dbe0: 2066 6f72 2074 6865 2053 746f 7261 6765   for the Storage
+0001dbf0: 206f 626a 6563 742e 0a20 2020 2023 2020   object..    #  
+0001dc00: 5765 2073 686f 756c 6420 6e6f 7420 7573  We should not us
+0001dc10: 6520 6065 7861 6d70 6c65 732f 7374 6f72  e `examples/stor
+0001dc20: 6167 655f 6465 6d6f 2e79 616d 6c60 2068  age_demo.yaml` h
+0001dc30: 6572 652c 2073 696e 6365 2069 7420 7265  ere, since it re
+0001dc40: 7175 6972 6573 0a20 2020 2023 2020 7573  quires.    #  us
+0001dc50: 6572 7320 746f 2065 6e73 7572 6520 6275  ers to ensure bu
+0001dc60: 636b 6574 206e 616d 6573 2074 6f20 6e6f  cket names to no
+0001dc70: 7420 6578 6973 7420 616e 642f 6f72 2062  t exist and/or b
+0001dc80: 6520 756e 6971 7565 2e0a 2020 2020 5f54  e unique..    _T
+0001dc90: 4553 545f 5941 4d4c 5f50 4154 4853 203d  EST_YAML_PATHS =
+0001dca0: 205b 0a20 2020 2020 2020 2027 6578 616d   [.        'exam
+0001dcb0: 706c 6573 2f6d 696e 696d 616c 2e79 616d  ples/minimal.yam
+0001dcc0: 6c27 2c20 2765 7861 6d70 6c65 732f 6d61  l', 'examples/ma
+0001dcd0: 6e61 6765 645f 7370 6f74 2e79 616d 6c27  naged_spot.yaml'
+0001dce0: 2c0a 2020 2020 2020 2020 2765 7861 6d70  ,.        'examp
+0001dcf0: 6c65 732f 7573 696e 675f 6669 6c65 5f6d  les/using_file_m
+0001dd00: 6f75 6e74 732e 7961 6d6c 272c 2027 6578  ounts.yaml', 'ex
+0001dd10: 616d 706c 6573 2f72 6573 6e65 745f 6170  amples/resnet_ap
+0001dd20: 702e 7961 6d6c 272c 0a20 2020 2020 2020  p.yaml',.       
+0001dd30: 2027 6578 616d 706c 6573 2f6d 756c 7469   'examples/multi
+0001dd40: 5f68 6f73 746e 616d 652e 7961 6d6c 270a  _hostname.yaml'.
+0001dd50: 2020 2020 5d0a 0a20 2020 2064 6566 205f      ]..    def _
+0001dd60: 6973 5f64 6963 745f 7375 6273 6574 2873  is_dict_subset(s
+0001dd70: 656c 662c 2064 312c 2064 3229 3a0a 2020  elf, d1, d2):.  
+0001dd80: 2020 2020 2020 2222 2243 6865 636b 2069        """Check i
+0001dd90: 6620 6431 2069 7320 7468 6520 7375 6273  f d1 is the subs
+0001dda0: 6574 206f 6620 6432 2e22 2222 0a20 2020  et of d2.""".   
+0001ddb0: 2020 2020 2066 6f72 206b 2c20 7620 696e       for k, v in
+0001ddc0: 2064 312e 6974 656d 7328 293a 0a20 2020   d1.items():.   
+0001ddd0: 2020 2020 2020 2020 2069 6620 6b20 6e6f           if k no
+0001dde0: 7420 696e 2064 323a 0a20 2020 2020 2020  t in d2:.       
+0001ddf0: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
+0001de00: 7374 616e 6365 2876 2c20 6c69 7374 2920  stance(v, list) 
+0001de10: 6f72 2069 7369 6e73 7461 6e63 6528 762c  or isinstance(v,
+0001de20: 2064 6963 7429 3a0a 2020 2020 2020 2020   dict):.        
+0001de30: 2020 2020 2020 2020 2020 2020 6173 7365              asse
+0001de40: 7274 206c 656e 2876 2920 3d3d 2030 2c20  rt len(v) == 0, 
+0001de50: 286b 2c20 7629 0a20 2020 2020 2020 2020  (k, v).         
+0001de60: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0001de70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001de80: 2061 7373 6572 7420 4661 6c73 652c 2028   assert False, (
+0001de90: 6b2c 2076 290a 2020 2020 2020 2020 2020  k, v).          
+0001dea0: 2020 656c 6966 2069 7369 6e73 7461 6e63    elif isinstanc
+0001deb0: 6528 762c 2064 6963 7429 3a0a 2020 2020  e(v, dict):.    
+0001dec0: 2020 2020 2020 2020 2020 2020 6173 7365              asse
+0001ded0: 7274 2069 7369 6e73 7461 6e63 6528 6432  rt isinstance(d2
+0001dee0: 5b6b 5d2c 2064 6963 7429 2c20 286b 2c20  [k], dict), (k, 
+0001def0: 762c 2064 3229 0a20 2020 2020 2020 2020  v, d2).         
+0001df00: 2020 2020 2020 2073 656c 662e 5f69 735f         self._is_
+0001df10: 6469 6374 5f73 7562 7365 7428 762c 2064  dict_subset(v, d
+0001df20: 325b 6b5d 290a 2020 2020 2020 2020 2020  2[k]).          
+0001df30: 2020 656c 6966 2069 7369 6e73 7461 6e63    elif isinstanc
+0001df40: 6528 762c 2073 7472 293a 0a20 2020 2020  e(v, str):.     
+0001df50: 2020 2020 2020 2020 2020 2069 6620 6b20             if k 
+0001df60: 3d3d 2027 6163 6365 6c65 7261 746f 7273  == 'accelerators
+0001df70: 273a 0a20 2020 2020 2020 2020 2020 2020  ':.             
+0001df80: 2020 2020 2020 2072 6573 6f75 7263 6573         resources
+0001df90: 203d 2073 6b79 2e52 6573 6f75 7263 6573   = sky.Resources
+0001dfa0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+0001dfb0: 2020 2020 2020 2072 6573 6f75 7263 6573         resources
+0001dfc0: 2e5f 7365 745f 6163 6365 6c65 7261 746f  ._set_accelerato
+0001dfd0: 7273 2876 2c20 4e6f 6e65 290a 2020 2020  rs(v, None).    
+0001dfe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dff0: 6173 7365 7274 2072 6573 6f75 7263 6573  assert resources
+0001e000: 2e61 6363 656c 6572 6174 6f72 7320 3d3d  .accelerators ==
+0001e010: 2064 325b 6b5d 2c20 286b 2c20 762c 2064   d2[k], (k, v, d
+0001e020: 3229 0a20 2020 2020 2020 2020 2020 2020  2).             
+0001e030: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0001e040: 2020 2020 2020 2020 2020 2020 2061 7373               ass
+0001e050: 6572 7420 762e 6c6f 7765 7228 2920 3d3d  ert v.lower() ==
+0001e060: 2064 325b 6b5d 2e6c 6f77 6572 2829 2c20   d2[k].lower(), 
+0001e070: 286b 2c20 762c 2064 325b 6b5d 290a 2020  (k, v, d2[k]).  
+0001e080: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+0001e090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e0a0: 6173 7365 7274 2076 203d 3d20 6432 5b6b  assert v == d2[k
+0001e0b0: 5d2c 2028 6b2c 2076 2c20 6432 5b6b 5d29  ], (k, v, d2[k])
+0001e0c0: 0a0a 2020 2020 6465 6620 5f63 6865 636b  ..    def _check
+0001e0d0: 5f65 7175 6976 616c 656e 7428 7365 6c66  _equivalent(self
+0001e0e0: 2c20 7961 6d6c 5f70 6174 6829 3a0a 2020  , yaml_path):.  
+0001e0f0: 2020 2020 2020 2222 2243 6865 636b 2069        """Check i
+0001e100: 6620 7468 6520 7961 6d6c 2069 7320 6571  f the yaml is eq
+0001e110: 7569 7661 6c65 6e74 2061 6674 6572 206c  uivalent after l
+0001e120: 6f61 6420 616e 6420 6475 6d70 2061 6761  oad and dump aga
+0001e130: 696e 2e22 2222 0a20 2020 2020 2020 206f  in.""".        o
+0001e140: 7269 6769 6e5f 7461 736b 5f63 6f6e 6669  rigin_task_confi
+0001e150: 6720 3d20 636f 6d6d 6f6e 5f75 7469 6c73  g = common_utils
+0001e160: 2e72 6561 645f 7961 6d6c 2879 616d 6c5f  .read_yaml(yaml_
+0001e170: 7061 7468 290a 0a20 2020 2020 2020 2074  path)..        t
+0001e180: 6173 6b20 3d20 736b 792e 5461 736b 2e66  ask = sky.Task.f
+0001e190: 726f 6d5f 7961 6d6c 2879 616d 6c5f 7061  rom_yaml(yaml_pa
+0001e1a0: 7468 290a 2020 2020 2020 2020 6e65 775f  th).        new_
+0001e1b0: 7461 736b 5f63 6f6e 6669 6720 3d20 7461  task_config = ta
+0001e1c0: 736b 2e74 6f5f 7961 6d6c 5f63 6f6e 6669  sk.to_yaml_confi
+0001e1d0: 6728 290a 2020 2020 2020 2020 2320 6431  g().        # d1
+0001e1e0: 203c 3d20 6432 0a20 2020 2020 2020 2073   <= d2.        s
+0001e1f0: 656c 662e 5f69 735f 6469 6374 5f73 7562  elf._is_dict_sub
+0001e200: 7365 7428 6f72 6967 696e 5f74 6173 6b5f  set(origin_task_
+0001e210: 636f 6e66 6967 2c20 6e65 775f 7461 736b  config, new_task
+0001e220: 5f63 6f6e 6669 6729 0a0a 2020 2020 6465  _config)..    de
+0001e230: 6620 7465 7374 5f6c 6f61 645f 6475 6d70  f test_load_dump
+0001e240: 5f79 616d 6c5f 636f 6e66 6967 5f65 7175  _yaml_config_equ
+0001e250: 6976 616c 656e 7428 7365 6c66 293a 0a20  ivalent(self):. 
+0001e260: 2020 2020 2020 2022 2222 5465 7374 2069         """Test i
+0001e270: 6620 7468 6520 7961 6d6c 2063 6f6e 6669  f the yaml confi
+0001e280: 6720 6973 2065 7175 6976 616c 656e 7420  g is equivalent 
+0001e290: 6166 7465 7220 6c6f 6164 2061 6e64 2064  after load and d
+0001e2a0: 756d 7020 6167 6169 6e2e 2222 220a 2020  ump again.""".  
+0001e2b0: 2020 2020 2020 7061 7468 6c69 622e 5061        pathlib.Pa
+0001e2c0: 7468 2827 7e2f 6461 7461 7365 7473 2729  th('~/datasets')
+0001e2d0: 2e65 7870 616e 6475 7365 7228 292e 6d6b  .expanduser().mk
+0001e2e0: 6469 7228 6578 6973 745f 6f6b 3d54 7275  dir(exist_ok=Tru
+0001e2f0: 6529 0a20 2020 2020 2020 2070 6174 686c  e).        pathl
+0001e300: 6962 2e50 6174 6828 277e 2f74 6d70 6669  ib.Path('~/tmpfi
+0001e310: 6c65 2729 2e65 7870 616e 6475 7365 7228  le').expanduser(
+0001e320: 292e 746f 7563 6828 290a 2020 2020 2020  ).touch().      
 0001e330: 2020 7061 7468 6c69 622e 5061 7468 2827    pathlib.Path('
-0001e340: 7e2f 2e73 7368 2f69 645f 7273 612e 7075  ~/.ssh/id_rsa.pu
-0001e350: 6227 292e 6578 7061 6e64 7573 6572 2829  b').expanduser()
-0001e360: 2e74 6f75 6368 2829 0a20 2020 2020 2020  .touch().       
-0001e370: 2070 6174 686c 6962 2e50 6174 6828 277e   pathlib.Path('~
-0001e380: 2f74 6d70 2d77 6f72 6b64 6972 2729 2e65  /tmp-workdir').e
-0001e390: 7870 616e 6475 7365 7228 292e 6d6b 6469  xpanduser().mkdi
-0001e3a0: 7228 6578 6973 745f 6f6b 3d54 7275 6529  r(exist_ok=True)
-0001e3b0: 0a20 2020 2020 2020 2070 6174 686c 6962  .        pathlib
-0001e3c0: 2e50 6174 6828 277e 2f44 6f77 6e6c 6f61  .Path('~/Downloa
-0001e3d0: 6473 2f74 7075 2729 2e65 7870 616e 6475  ds/tpu').expandu
-0001e3e0: 7365 7228 292e 6d6b 6469 7228 7061 7265  ser().mkdir(pare
-0001e3f0: 6e74 733d 5472 7565 2c0a 2020 2020 2020  nts=True,.      
-0001e400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e430: 2020 2020 2065 7869 7374 5f6f 6b3d 5472       exist_ok=Tr
-0001e440: 7565 290a 2020 2020 2020 2020 666f 7220  ue).        for 
-0001e450: 7961 6d6c 5f70 6174 6820 696e 2073 656c  yaml_path in sel
-0001e460: 662e 5f54 4553 545f 5941 4d4c 5f50 4154  f._TEST_YAML_PAT
-0001e470: 4853 3a0a 2020 2020 2020 2020 2020 2020  HS:.            
-0001e480: 7365 6c66 2e5f 6368 6563 6b5f 6571 7569  self._check_equi
-0001e490: 7661 6c65 6e74 2879 616d 6c5f 7061 7468  valent(yaml_path
-0001e4a0: 290a                                     ).
+0001e340: 7e2f 2e73 7368 2729 2e65 7870 616e 6475  ~/.ssh').expandu
+0001e350: 7365 7228 292e 6d6b 6469 7228 6578 6973  ser().mkdir(exis
+0001e360: 745f 6f6b 3d54 7275 6529 0a20 2020 2020  t_ok=True).     
+0001e370: 2020 2070 6174 686c 6962 2e50 6174 6828     pathlib.Path(
+0001e380: 277e 2f2e 7373 682f 6964 5f72 7361 2e70  '~/.ssh/id_rsa.p
+0001e390: 7562 2729 2e65 7870 616e 6475 7365 7228  ub').expanduser(
+0001e3a0: 292e 746f 7563 6828 290a 2020 2020 2020  ).touch().      
+0001e3b0: 2020 7061 7468 6c69 622e 5061 7468 2827    pathlib.Path('
+0001e3c0: 7e2f 746d 702d 776f 726b 6469 7227 292e  ~/tmp-workdir').
+0001e3d0: 6578 7061 6e64 7573 6572 2829 2e6d 6b64  expanduser().mkd
+0001e3e0: 6972 2865 7869 7374 5f6f 6b3d 5472 7565  ir(exist_ok=True
+0001e3f0: 290a 2020 2020 2020 2020 7061 7468 6c69  ).        pathli
+0001e400: 622e 5061 7468 2827 7e2f 446f 776e 6c6f  b.Path('~/Downlo
+0001e410: 6164 732f 7470 7527 292e 6578 7061 6e64  ads/tpu').expand
+0001e420: 7573 6572 2829 2e6d 6b64 6972 2870 6172  user().mkdir(par
+0001e430: 656e 7473 3d54 7275 652c 0a20 2020 2020  ents=True,.     
+0001e440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e470: 2020 2020 2020 6578 6973 745f 6f6b 3d54        exist_ok=T
+0001e480: 7275 6529 0a20 2020 2020 2020 2066 6f72  rue).        for
+0001e490: 2079 616d 6c5f 7061 7468 2069 6e20 7365   yaml_path in se
+0001e4a0: 6c66 2e5f 5445 5354 5f59 414d 4c5f 5041  lf._TEST_YAML_PA
+0001e4b0: 5448 533a 0a20 2020 2020 2020 2020 2020  THS:.           
+0001e4c0: 2073 656c 662e 5f63 6865 636b 5f65 7175   self._check_equ
+0001e4d0: 6976 616c 656e 7428 7961 6d6c 5f70 6174  ivalent(yaml_pat
+0001e4e0: 6829 0a                                  h).
```

### Comparing `skypilot-nightly-1.0.0.dev20230717/tests/test_spot.py` & `skypilot-nightly-1.0.0.dev20230718/tests/test_spot.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/tests/test_storage.py` & `skypilot-nightly-1.0.0.dev20230718/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230717/tests/test_wheels.py` & `skypilot-nightly-1.0.0.dev20230718/tests/test_wheels.py`

 * *Files identical despite different names*

