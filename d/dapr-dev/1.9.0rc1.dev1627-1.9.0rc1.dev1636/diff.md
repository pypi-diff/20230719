# Comparing `tmp/dapr-dev-1.9.0rc1.dev1627.tar.gz` & `tmp/dapr-dev-1.9.0rc1.dev1636.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dapr-dev-1.9.0rc1.dev1627.tar", last modified: Fri Jul 14 18:52:06 2023, max compression
+gzip compressed data, was "dist/dapr-dev-1.9.0rc1.dev1636.tar", last modified: Tue Jul 18 22:44:51 2023, max compression
```

## Comparing `dapr-dev-1.9.0rc1.dev1627.tar` & `dapr-dev-1.9.0rc1.dev1636.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:52:06.000000 dapr-dev-1.9.0rc1.dev1627/
--rw-r--r--   0 runner    (1001) docker     (123)    11378 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-14 18:52:06.000000 dapr-dev-1.9.0rc1.dev1627/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:52:06.000000 dapr-dev-1.9.0rc1.dev1627/dapr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:52:06.000000 dapr-dev-1.9.0rc1.dev1627/dapr/actor/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/actor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/actor/actor_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:52:06.000000 dapr-dev-1.9.0rc1.dev1627/dapr/actor/client/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/actor/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/actor/client/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/actor/id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:52:06.000000 dapr-dev-1.9.0rc1.dev1627/dapr/actor/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/actor/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/actor/runtime/_call_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/actor/runtime/_method_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/actor/runtime/_reminder_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/actor/runtime/_state_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/actor/runtime/_timer_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/actor/runtime/_type_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/actor/runtime/_type_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10127 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/actor/runtime/actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/actor/runtime/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/actor/runtime/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/actor/runtime/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/actor/runtime/method_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/actor/runtime/reentrancy_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/actor/runtime/remindable.py
--rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/actor/runtime/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/actor/runtime/state_change.py
--rw-r--r--   0 runner    (1001) docker     (123)    11161 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/actor/runtime/state_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:52:06.000000 dapr-dev-1.9.0rc1.dev1627/dapr/aio/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:52:06.000000 dapr-dev-1.9.0rc1.dev1627/dapr/aio/clients/
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/aio/clients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:52:06.000000 dapr-dev-1.9.0rc1.dev1627/dapr/aio/clients/grpc/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/aio/clients/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/aio/clients/grpc/_asynchelpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    61807 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/aio/clients/grpc/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:52:06.000000 dapr-dev-1.9.0rc1.dev1627/dapr/clients/
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/clients/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/clients/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:52:06.000000 dapr-dev-1.9.0rc1.dev1627/dapr/clients/grpc/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/clients/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6856 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/clients/grpc/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10595 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/clients/grpc/_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    31949 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/clients/grpc/_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/clients/grpc/_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    60809 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/clients/grpc/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:52:06.000000 dapr-dev-1.9.0rc1.dev1627/dapr/clients/http/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/clients/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/clients/http/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/clients/http/dapr_actor_http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/clients/http/dapr_invocation_http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:52:06.000000 dapr-dev-1.9.0rc1.dev1627/dapr/conf/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/conf/global_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:52:06.000000 dapr-dev-1.9.0rc1.dev1627/dapr/proto/
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/proto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:52:06.000000 dapr-dev-1.9.0rc1.dev1627/dapr/proto/common/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/proto/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:52:06.000000 dapr-dev-1.9.0rc1.dev1627/dapr/proto/common/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/proto/common/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8801 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/proto/common/v1/common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/proto/common/v1/common_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:52:06.000000 dapr-dev-1.9.0rc1.dev1627/dapr/proto/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/proto/runtime/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:52:06.000000 dapr-dev-1.9.0rc1.dev1627/dapr/proto/runtime/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/proto/runtime/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18899 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/proto/runtime/v1/appcallback_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    16126 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/proto/runtime/v1/appcallback_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    91774 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/proto/runtime/v1/dapr_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    86821 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/proto/runtime/v1/dapr_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:52:06.000000 dapr-dev-1.9.0rc1.dev1627/dapr/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/serializers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/serializers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/serializers/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:52:06.000000 dapr-dev-1.9.0rc1.dev1627/dapr/version/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/dapr/version/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:52:06.000000 dapr-dev-1.9.0rc1.dev1627/dapr_dev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-14 18:52:06.000000 dapr-dev-1.9.0rc1.dev1627/dapr_dev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-14 18:52:06.000000 dapr-dev-1.9.0rc1.dev1627/dapr_dev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 18:52:06.000000 dapr-dev-1.9.0rc1.dev1627/dapr_dev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 18:52:06.000000 dapr-dev-1.9.0rc1.dev1627/dapr_dev.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-14 18:52:06.000000 dapr-dev-1.9.0rc1.dev1627/dapr_dev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-14 18:52:06.000000 dapr-dev-1.9.0rc1.dev1627/dapr_dev.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-14 18:52:06.000000 dapr-dev-1.9.0rc1.dev1627/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-14 18:51:50.000000 dapr-dev-1.9.0rc1.dev1627/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:44:51.000000 dapr-dev-1.9.0rc1.dev1636/
+-rw-r--r--   0 runner    (1001) docker     (123)    11378 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-18 22:44:51.000000 dapr-dev-1.9.0rc1.dev1636/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:44:51.000000 dapr-dev-1.9.0rc1.dev1636/dapr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:44:51.000000 dapr-dev-1.9.0rc1.dev1636/dapr/actor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/actor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/actor/actor_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:44:51.000000 dapr-dev-1.9.0rc1.dev1636/dapr/actor/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/actor/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/actor/client/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/actor/id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:44:51.000000 dapr-dev-1.9.0rc1.dev1636/dapr/actor/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/actor/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/actor/runtime/_call_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/actor/runtime/_method_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/actor/runtime/_reminder_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/actor/runtime/_state_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/actor/runtime/_timer_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/actor/runtime/_type_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/actor/runtime/_type_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10127 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/actor/runtime/actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/actor/runtime/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/actor/runtime/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/actor/runtime/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/actor/runtime/method_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/actor/runtime/reentrancy_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/actor/runtime/remindable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/actor/runtime/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/actor/runtime/state_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11161 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/actor/runtime/state_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:44:51.000000 dapr-dev-1.9.0rc1.dev1636/dapr/aio/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:44:51.000000 dapr-dev-1.9.0rc1.dev1636/dapr/aio/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/aio/clients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:44:51.000000 dapr-dev-1.9.0rc1.dev1636/dapr/aio/clients/grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/aio/clients/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/aio/clients/grpc/_asynchelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61807 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/aio/clients/grpc/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:44:51.000000 dapr-dev-1.9.0rc1.dev1636/dapr/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/clients/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/clients/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:44:51.000000 dapr-dev-1.9.0rc1.dev1636/dapr/clients/grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/clients/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6856 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/clients/grpc/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10595 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/clients/grpc/_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31949 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/clients/grpc/_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/clients/grpc/_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60809 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/clients/grpc/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:44:51.000000 dapr-dev-1.9.0rc1.dev1636/dapr/clients/http/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/clients/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/clients/http/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/clients/http/dapr_actor_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/clients/http/dapr_invocation_http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:44:51.000000 dapr-dev-1.9.0rc1.dev1636/dapr/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/conf/global_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:44:51.000000 dapr-dev-1.9.0rc1.dev1636/dapr/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/proto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:44:51.000000 dapr-dev-1.9.0rc1.dev1636/dapr/proto/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/proto/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:44:51.000000 dapr-dev-1.9.0rc1.dev1636/dapr/proto/common/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/proto/common/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8801 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/proto/common/v1/common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/proto/common/v1/common_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:44:51.000000 dapr-dev-1.9.0rc1.dev1636/dapr/proto/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/proto/runtime/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:44:51.000000 dapr-dev-1.9.0rc1.dev1636/dapr/proto/runtime/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/proto/runtime/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18899 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/proto/runtime/v1/appcallback_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16126 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/proto/runtime/v1/appcallback_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91774 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/proto/runtime/v1/dapr_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86821 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/proto/runtime/v1/dapr_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:44:51.000000 dapr-dev-1.9.0rc1.dev1636/dapr/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/serializers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/serializers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/serializers/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:44:51.000000 dapr-dev-1.9.0rc1.dev1636/dapr/version/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/dapr/version/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:44:51.000000 dapr-dev-1.9.0rc1.dev1636/dapr_dev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-18 22:44:51.000000 dapr-dev-1.9.0rc1.dev1636/dapr_dev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-18 22:44:51.000000 dapr-dev-1.9.0rc1.dev1636/dapr_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 22:44:51.000000 dapr-dev-1.9.0rc1.dev1636/dapr_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 22:44:51.000000 dapr-dev-1.9.0rc1.dev1636/dapr_dev.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-18 22:44:51.000000 dapr-dev-1.9.0rc1.dev1636/dapr_dev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-18 22:44:51.000000 dapr-dev-1.9.0rc1.dev1636/dapr_dev.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-18 22:44:51.000000 dapr-dev-1.9.0rc1.dev1636/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-18 22:44:37.000000 dapr-dev-1.9.0rc1.dev1636/setup.py
```

### Comparing `dapr-dev-1.9.0rc1.dev1627/LICENSE` & `dapr-dev-1.9.0rc1.dev1636/LICENSE`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/PKG-INFO` & `dapr-dev-1.9.0rc1.dev1636/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: dapr-dev
-Version: 1.9.0rc1.dev1627
+Version: 1.9.0rc1.dev1636
 Summary: The developmental release for Dapr Python SDK.
 Home-page: https://dapr.io/
 Author: Dapr Authors
 Author-email: daprweb@microsoft.com
 License: Apache
 Project-URL: Documentation, https://github.com/dapr/docs
 Project-URL: Source, https://github.com/dapr/python-sdk
```

### Comparing `dapr-dev-1.9.0rc1.dev1627/README.md` & `dapr-dev-1.9.0rc1.dev1636/README.md`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/actor/__init__.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/actor/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/actor/actor_interface.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/actor/actor_interface.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/actor/client/__init__.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/actor/client/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/actor/client/proxy.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/actor/client/proxy.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/actor/id.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/actor/id.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/actor/runtime/__init__.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/actor/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/actor/runtime/_call_type.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/actor/runtime/_call_type.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/actor/runtime/_method_context.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/actor/runtime/_method_context.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/actor/runtime/_reminder_data.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/actor/runtime/_reminder_data.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/actor/runtime/_state_provider.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/actor/runtime/_state_provider.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/actor/runtime/_timer_data.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/actor/runtime/_timer_data.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/actor/runtime/_type_information.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/actor/runtime/_type_information.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/actor/runtime/_type_utils.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/actor/runtime/_type_utils.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/actor/runtime/actor.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/actor/runtime/actor.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/actor/runtime/config.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/actor/runtime/config.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/actor/runtime/context.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/actor/runtime/context.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/actor/runtime/manager.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/actor/runtime/manager.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/actor/runtime/method_dispatcher.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/actor/runtime/method_dispatcher.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/actor/runtime/reentrancy_context.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/actor/runtime/reentrancy_context.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/actor/runtime/remindable.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/actor/runtime/remindable.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/actor/runtime/runtime.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/actor/runtime/runtime.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/actor/runtime/state_change.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/actor/runtime/state_change.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/actor/runtime/state_manager.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/actor/runtime/state_manager.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/aio/clients/__init__.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/aio/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/aio/clients/grpc/__init__.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/aio/clients/grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/aio/clients/grpc/_asynchelpers.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/aio/clients/grpc/_asynchelpers.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/aio/clients/grpc/client.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/aio/clients/grpc/client.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/clients/__init__.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/clients/base.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/clients/base.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/clients/exceptions.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/clients/exceptions.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/clients/grpc/__init__.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/clients/grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/clients/grpc/_helpers.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/clients/grpc/_helpers.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/clients/grpc/_request.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/clients/grpc/_request.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/clients/grpc/_response.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/clients/grpc/_response.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/clients/grpc/_state.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/clients/grpc/_state.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/clients/grpc/client.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/clients/grpc/client.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/clients/http/__init__.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/clients/http/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/clients/http/client.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/clients/http/client.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/clients/http/dapr_actor_http_client.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/clients/http/dapr_actor_http_client.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/clients/http/dapr_invocation_http_client.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/clients/http/dapr_invocation_http_client.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/conf/__init__.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/conf/global_settings.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/conf/global_settings.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/proto/__init__.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/proto/common/__init__.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/proto/common/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/proto/common/v1/__init__.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/proto/common/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/proto/common/v1/common_pb2.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/proto/common/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/proto/runtime/__init__.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/proto/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/proto/runtime/v1/__init__.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/proto/runtime/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/proto/runtime/v1/appcallback_pb2.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/proto/runtime/v1/appcallback_pb2.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/proto/runtime/v1/appcallback_pb2_grpc.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/proto/runtime/v1/appcallback_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/proto/runtime/v1/dapr_pb2.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/proto/runtime/v1/dapr_pb2.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/proto/runtime/v1/dapr_pb2_grpc.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/proto/runtime/v1/dapr_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/serializers/__init__.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/serializers/base.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/serializers/base.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/serializers/json.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/serializers/json.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/serializers/util.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/serializers/util.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr/version/version.py` & `dapr-dev-1.9.0rc1.dev1636/dapr/version/version.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr_dev.egg-info/PKG-INFO` & `dapr-dev-1.9.0rc1.dev1636/dapr_dev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: dapr-dev
-Version: 1.9.0rc1.dev1627
+Version: 1.9.0rc1.dev1636
 Summary: The developmental release for Dapr Python SDK.
 Home-page: https://dapr.io/
 Author: Dapr Authors
 Author-email: daprweb@microsoft.com
 License: Apache
 Project-URL: Documentation, https://github.com/dapr/docs
 Project-URL: Source, https://github.com/dapr/python-sdk
```

### Comparing `dapr-dev-1.9.0rc1.dev1627/dapr_dev.egg-info/SOURCES.txt` & `dapr-dev-1.9.0rc1.dev1636/dapr_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/setup.cfg` & `dapr-dev-1.9.0rc1.dev1636/setup.cfg`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1627/setup.py` & `dapr-dev-1.9.0rc1.dev1636/setup.py`

 * *Files identical despite different names*

