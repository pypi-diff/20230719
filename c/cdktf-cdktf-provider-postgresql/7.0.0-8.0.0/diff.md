# Comparing `tmp/cdktf-cdktf-provider-postgresql-7.0.0.tar.gz` & `tmp/cdktf-cdktf-provider-postgresql-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-postgresql-7.0.0.tar", last modified: Thu Jun 15 11:32:42 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-postgresql-8.0.0.tar", last modified: Wed Jul 19 03:45:47 2023, max compression
```

## Comparing `cdktf-cdktf-provider-postgresql-7.0.0.tar` & `cdktf-cdktf-provider-postgresql-8.0.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:32:42.859470 cdktf-cdktf-provider-postgresql-7.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-15 11:32:28.000000 cdktf-cdktf-provider-postgresql-7.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 11:32:28.000000 cdktf-cdktf-provider-postgresql-7.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-06-15 11:32:42.859470 cdktf-cdktf-provider-postgresql-7.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-06-15 11:32:28.000000 cdktf-cdktf-provider-postgresql-7.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-15 11:32:28.000000 cdktf-cdktf-provider-postgresql-7.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 11:32:42.859470 cdktf-cdktf-provider-postgresql-7.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-06-15 11:32:28.000000 cdktf-cdktf-provider-postgresql-7.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:32:42.855470 cdktf-cdktf-provider-postgresql-7.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:32:42.855470 cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-06-15 11:32:28.000000 cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:32:42.855470 cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-15 11:32:28.000000 cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   134144 2023-06-15 11:32:28.000000 cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/_jsii/provider-postgresql@7.0.0.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:32:42.859470 cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/data_postgresql_schemas/
--rw-r--r--   0 runner    (1001) docker     (123)    34317 2023-06-15 11:32:28.000000 cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/data_postgresql_schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:32:42.859470 cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/data_postgresql_sequences/
--rw-r--r--   0 runner    (1001) docker     (123)    43102 2023-06-15 11:32:28.000000 cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/data_postgresql_sequences/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:32:42.859470 cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/data_postgresql_tables/
--rw-r--r--   0 runner    (1001) docker     (123)    45760 2023-06-15 11:32:28.000000 cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/data_postgresql_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:32:42.859470 cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/database/
--rw-r--r--   0 runner    (1001) docker     (123)    41869 2023-06-15 11:32:28.000000 cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/database/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:32:42.859470 cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/default_privileges/
--rw-r--r--   0 runner    (1001) docker     (123)    33200 2023-06-15 11:32:28.000000 cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/default_privileges/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:32:42.859470 cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/extension/
--rw-r--r--   0 runner    (1001) docker     (123)    31436 2023-06-15 11:32:28.000000 cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/extension/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:32:42.859470 cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/function_resource/
--rw-r--r--   0 runner    (1001) docker     (123)    54689 2023-06-15 11:32:28.000000 cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/function_resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:32:42.859470 cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/grant/
--rw-r--r--   0 runner    (1001) docker     (123)    35689 2023-06-15 11:32:28.000000 cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/grant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:32:42.859470 cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/grant_role/
--rw-r--r--   0 runner    (1001) docker     (123)    23253 2023-06-15 11:32:28.000000 cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/grant_role/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:32:42.859470 cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/physical_replication_slot/
--rw-r--r--   0 runner    (1001) docker     (123)    17945 2023-06-15 11:32:28.000000 cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/physical_replication_slot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:32:42.859470 cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/provider/
--rw-r--r--   0 runner    (1001) docker     (123)    57620 2023-06-15 11:32:28.000000 cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/provider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:32:42.859470 cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/publication/
--rw-r--r--   0 runner    (1001) docker     (123)    38127 2023-06-15 11:32:28.000000 cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/publication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:32:28.000000 cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:32:42.859470 cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/replication_slot/
--rw-r--r--   0 runner    (1001) docker     (123)    22283 2023-06-15 11:32:28.000000 cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/replication_slot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:32:42.859470 cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/role/
--rw-r--r--   0 runner    (1001) docker     (123)    73740 2023-06-15 11:32:28.000000 cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/role/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:32:42.859470 cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/schema/
--rw-r--r--   0 runner    (1001) docker     (123)    54800 2023-06-15 11:32:28.000000 cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:32:42.859470 cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/server/
--rw-r--r--   0 runner    (1001) docker     (123)    34546 2023-06-15 11:32:28.000000 cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:32:42.859470 cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/subscription/
--rw-r--r--   0 runner    (1001) docker     (123)    31163 2023-06-15 11:32:28.000000 cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/subscription/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:32:42.859470 cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/user_mapping/
--rw-r--r--   0 runner    (1001) docker     (123)    24312 2023-06-15 11:32:28.000000 cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/user_mapping/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:32:42.855470 cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-06-15 11:32:42.000000 cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-15 11:32:42.000000 cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:32:42.000000 cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-15 11:32:42.000000 cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-15 11:32:42.000000 cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:45:47.138218 cdktf-cdktf-provider-postgresql-8.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-07-19 03:45:33.000000 cdktf-cdktf-provider-postgresql-8.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-19 03:45:33.000000 cdktf-cdktf-provider-postgresql-8.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-07-19 03:45:47.138218 cdktf-cdktf-provider-postgresql-8.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-07-19 03:45:33.000000 cdktf-cdktf-provider-postgresql-8.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-19 03:45:33.000000 cdktf-cdktf-provider-postgresql-8.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 03:45:47.138218 cdktf-cdktf-provider-postgresql-8.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-07-19 03:45:33.000000 cdktf-cdktf-provider-postgresql-8.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:45:47.130217 cdktf-cdktf-provider-postgresql-8.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:45:47.134217 cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-07-19 03:45:33.000000 cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:45:47.134217 cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-19 03:45:33.000000 cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   134165 2023-07-19 03:45:33.000000 cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/_jsii/provider-postgresql@8.0.0.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:45:47.134217 cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/data_postgresql_schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)    34317 2023-07-19 03:45:33.000000 cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/data_postgresql_schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:45:47.134217 cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/data_postgresql_sequences/
+-rw-r--r--   0 runner    (1001) docker     (123)    43102 2023-07-19 03:45:33.000000 cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/data_postgresql_sequences/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:45:47.134217 cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/data_postgresql_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)    45760 2023-07-19 03:45:33.000000 cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/data_postgresql_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:45:47.134217 cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/database/
+-rw-r--r--   0 runner    (1001) docker     (123)    41869 2023-07-19 03:45:33.000000 cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/database/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:45:47.138218 cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/default_privileges/
+-rw-r--r--   0 runner    (1001) docker     (123)    33200 2023-07-19 03:45:33.000000 cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/default_privileges/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:45:47.138218 cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/extension/
+-rw-r--r--   0 runner    (1001) docker     (123)    31436 2023-07-19 03:45:33.000000 cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/extension/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:45:47.138218 cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/function_resource/
+-rw-r--r--   0 runner    (1001) docker     (123)    54689 2023-07-19 03:45:33.000000 cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/function_resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:45:47.138218 cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/grant/
+-rw-r--r--   0 runner    (1001) docker     (123)    35689 2023-07-19 03:45:33.000000 cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/grant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:45:47.138218 cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/grant_role/
+-rw-r--r--   0 runner    (1001) docker     (123)    23253 2023-07-19 03:45:33.000000 cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/grant_role/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:45:47.138218 cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/physical_replication_slot/
+-rw-r--r--   0 runner    (1001) docker     (123)    17945 2023-07-19 03:45:33.000000 cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/physical_replication_slot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:45:47.138218 cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)    57620 2023-07-19 03:45:33.000000 cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/provider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:45:47.138218 cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/publication/
+-rw-r--r--   0 runner    (1001) docker     (123)    38127 2023-07-19 03:45:33.000000 cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/publication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 03:45:33.000000 cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:45:47.138218 cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/replication_slot/
+-rw-r--r--   0 runner    (1001) docker     (123)    22283 2023-07-19 03:45:33.000000 cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/replication_slot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:45:47.138218 cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/role/
+-rw-r--r--   0 runner    (1001) docker     (123)    73740 2023-07-19 03:45:33.000000 cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/role/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:45:47.138218 cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)    54800 2023-07-19 03:45:33.000000 cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:45:47.138218 cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/server/
+-rw-r--r--   0 runner    (1001) docker     (123)    34546 2023-07-19 03:45:33.000000 cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:45:47.138218 cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/subscription/
+-rw-r--r--   0 runner    (1001) docker     (123)    31163 2023-07-19 03:45:33.000000 cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/subscription/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:45:47.138218 cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/user_mapping/
+-rw-r--r--   0 runner    (1001) docker     (123)    24312 2023-07-19 03:45:33.000000 cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/user_mapping/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:45:47.134217 cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-07-19 03:45:47.000000 cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-19 03:45:47.000000 cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 03:45:47.000000 cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-19 03:45:47.000000 cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-19 03:45:47.000000 cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-postgresql-7.0.0/LICENSE` & `cdktf-cdktf-provider-postgresql-8.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-postgresql-7.0.0/PKG-INFO` & `cdktf-cdktf-provider-postgresql-8.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-postgresql
-Version: 7.0.0
+Version: 8.0.0
 Summary: Prebuilt postgresql Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-postgresql.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-postgresql.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-postgresql-7.0.0/README.md` & `cdktf-cdktf-provider-postgresql-8.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-postgresql-7.0.0/setup.py` & `cdktf-cdktf-provider-postgresql-8.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-postgresql",
-    "version": "7.0.0",
+    "version": "8.0.0",
     "description": "Prebuilt postgresql Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-postgresql.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -40,25 +40,25 @@
         "cdktf_cdktf_provider_postgresql.schema",
         "cdktf_cdktf_provider_postgresql.server",
         "cdktf_cdktf_provider_postgresql.subscription",
         "cdktf_cdktf_provider_postgresql.user_mapping"
     ],
     "package_data": {
         "cdktf_cdktf_provider_postgresql._jsii": [
-            "provider-postgresql@7.0.0.jsii.tgz"
+            "provider-postgresql@8.0.0.jsii.tgz"
         ],
         "cdktf_cdktf_provider_postgresql": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "cdktf>=0.17.0, <0.18.0",
         "constructs>=10.0.0, <11.0.0",
-        "jsii>=1.84.0, <2.0.0",
+        "jsii>=1.85.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/__init__.py` & `cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/data_postgresql_schemas/__init__.py` & `cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/data_postgresql_schemas/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_postgresql_schemas`
 
-Refer to the Terraform Registory for docs: [`data_postgresql_schemas`](https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/schemas).
+Refer to the Terraform Registory for docs: [`data_postgresql_schemas`](https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/schemas).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataPostgresqlSchemas(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-postgresql.dataPostgresqlSchemas.DataPostgresqlSchemas",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/schemas postgresql_schemas}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/schemas postgresql_schemas}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         database: builtins.str,
@@ -44,25 +44,25 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/schemas postgresql_schemas} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/schemas postgresql_schemas} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param database: The PostgreSQL database which will be queried for schema names. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/schemas#database DataPostgresqlSchemas#database}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/schemas#id DataPostgresqlSchemas#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param include_system_schemas: Determines whether to include system schemas (pg_ prefix and information_schema). 'public' will always be included. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/schemas#include_system_schemas DataPostgresqlSchemas#include_system_schemas}
-        :param like_all_patterns: Expression(s) which will be pattern matched in the query using the PostgreSQL LIKE ALL operator. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/schemas#like_all_patterns DataPostgresqlSchemas#like_all_patterns}
-        :param like_any_patterns: Expression(s) which will be pattern matched in the query using the PostgreSQL LIKE ANY operator. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/schemas#like_any_patterns DataPostgresqlSchemas#like_any_patterns}
-        :param not_like_all_patterns: Expression(s) which will be pattern matched in the query using the PostgreSQL NOT LIKE ALL operator. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/schemas#not_like_all_patterns DataPostgresqlSchemas#not_like_all_patterns}
-        :param regex_pattern: Expression which will be pattern matched in the query using the PostgreSQL ~ (regular expression match) operator. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/schemas#regex_pattern DataPostgresqlSchemas#regex_pattern}
+        :param database: The PostgreSQL database which will be queried for schema names. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/schemas#database DataPostgresqlSchemas#database}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/schemas#id DataPostgresqlSchemas#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param include_system_schemas: Determines whether to include system schemas (pg_ prefix and information_schema). 'public' will always be included. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/schemas#include_system_schemas DataPostgresqlSchemas#include_system_schemas}
+        :param like_all_patterns: Expression(s) which will be pattern matched in the query using the PostgreSQL LIKE ALL operator. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/schemas#like_all_patterns DataPostgresqlSchemas#like_all_patterns}
+        :param like_any_patterns: Expression(s) which will be pattern matched in the query using the PostgreSQL LIKE ANY operator. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/schemas#like_any_patterns DataPostgresqlSchemas#like_any_patterns}
+        :param not_like_all_patterns: Expression(s) which will be pattern matched in the query using the PostgreSQL NOT LIKE ALL operator. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/schemas#not_like_all_patterns DataPostgresqlSchemas#not_like_all_patterns}
+        :param regex_pattern: Expression which will be pattern matched in the query using the PostgreSQL ~ (regular expression match) operator. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/schemas#regex_pattern DataPostgresqlSchemas#regex_pattern}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -298,21 +298,21 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param database: The PostgreSQL database which will be queried for schema names. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/schemas#database DataPostgresqlSchemas#database}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/schemas#id DataPostgresqlSchemas#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param include_system_schemas: Determines whether to include system schemas (pg_ prefix and information_schema). 'public' will always be included. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/schemas#include_system_schemas DataPostgresqlSchemas#include_system_schemas}
-        :param like_all_patterns: Expression(s) which will be pattern matched in the query using the PostgreSQL LIKE ALL operator. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/schemas#like_all_patterns DataPostgresqlSchemas#like_all_patterns}
-        :param like_any_patterns: Expression(s) which will be pattern matched in the query using the PostgreSQL LIKE ANY operator. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/schemas#like_any_patterns DataPostgresqlSchemas#like_any_patterns}
-        :param not_like_all_patterns: Expression(s) which will be pattern matched in the query using the PostgreSQL NOT LIKE ALL operator. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/schemas#not_like_all_patterns DataPostgresqlSchemas#not_like_all_patterns}
-        :param regex_pattern: Expression which will be pattern matched in the query using the PostgreSQL ~ (regular expression match) operator. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/schemas#regex_pattern DataPostgresqlSchemas#regex_pattern}
+        :param database: The PostgreSQL database which will be queried for schema names. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/schemas#database DataPostgresqlSchemas#database}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/schemas#id DataPostgresqlSchemas#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param include_system_schemas: Determines whether to include system schemas (pg_ prefix and information_schema). 'public' will always be included. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/schemas#include_system_schemas DataPostgresqlSchemas#include_system_schemas}
+        :param like_all_patterns: Expression(s) which will be pattern matched in the query using the PostgreSQL LIKE ALL operator. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/schemas#like_all_patterns DataPostgresqlSchemas#like_all_patterns}
+        :param like_any_patterns: Expression(s) which will be pattern matched in the query using the PostgreSQL LIKE ANY operator. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/schemas#like_any_patterns DataPostgresqlSchemas#like_any_patterns}
+        :param not_like_all_patterns: Expression(s) which will be pattern matched in the query using the PostgreSQL NOT LIKE ALL operator. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/schemas#not_like_all_patterns DataPostgresqlSchemas#not_like_all_patterns}
+        :param regex_pattern: Expression which will be pattern matched in the query using the PostgreSQL ~ (regular expression match) operator. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/schemas#regex_pattern DataPostgresqlSchemas#regex_pattern}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__cdec4b4e2ce548128495dedda5738aa53e0dfaba14d828b3106381b135f44e16)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -422,73 +422,73 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def database(self) -> builtins.str:
         '''The PostgreSQL database which will be queried for schema names.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/schemas#database DataPostgresqlSchemas#database}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/schemas#database DataPostgresqlSchemas#database}
         '''
         result = self._values.get("database")
         assert result is not None, "Required property 'database' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/schemas#id DataPostgresqlSchemas#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/schemas#id DataPostgresqlSchemas#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def include_system_schemas(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Determines whether to include system schemas (pg_ prefix and information_schema). 'public' will always be included.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/schemas#include_system_schemas DataPostgresqlSchemas#include_system_schemas}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/schemas#include_system_schemas DataPostgresqlSchemas#include_system_schemas}
         '''
         result = self._values.get("include_system_schemas")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def like_all_patterns(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Expression(s) which will be pattern matched in the query using the PostgreSQL LIKE ALL operator.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/schemas#like_all_patterns DataPostgresqlSchemas#like_all_patterns}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/schemas#like_all_patterns DataPostgresqlSchemas#like_all_patterns}
         '''
         result = self._values.get("like_all_patterns")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def like_any_patterns(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Expression(s) which will be pattern matched in the query using the PostgreSQL LIKE ANY operator.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/schemas#like_any_patterns DataPostgresqlSchemas#like_any_patterns}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/schemas#like_any_patterns DataPostgresqlSchemas#like_any_patterns}
         '''
         result = self._values.get("like_any_patterns")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def not_like_all_patterns(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Expression(s) which will be pattern matched in the query using the PostgreSQL NOT LIKE ALL operator.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/schemas#not_like_all_patterns DataPostgresqlSchemas#not_like_all_patterns}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/schemas#not_like_all_patterns DataPostgresqlSchemas#not_like_all_patterns}
         '''
         result = self._values.get("not_like_all_patterns")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def regex_pattern(self) -> typing.Optional[builtins.str]:
         '''Expression which will be pattern matched in the query using the PostgreSQL ~ (regular expression match) operator.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/schemas#regex_pattern DataPostgresqlSchemas#regex_pattern}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/schemas#regex_pattern DataPostgresqlSchemas#regex_pattern}
         '''
         result = self._values.get("regex_pattern")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/data_postgresql_sequences/__init__.py` & `cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/data_postgresql_sequences/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_postgresql_sequences`
 
-Refer to the Terraform Registory for docs: [`data_postgresql_sequences`](https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/sequences).
+Refer to the Terraform Registory for docs: [`data_postgresql_sequences`](https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/sequences).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataPostgresqlSequences(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-postgresql.dataPostgresqlSequences.DataPostgresqlSequences",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/sequences postgresql_sequences}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/sequences postgresql_sequences}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         database: builtins.str,
@@ -44,25 +44,25 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/sequences postgresql_sequences} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/sequences postgresql_sequences} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param database: The PostgreSQL database which will be queried for sequence names. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/sequences#database DataPostgresqlSequences#database}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/sequences#id DataPostgresqlSequences#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param like_all_patterns: Expression(s) which will be pattern matched against sequence names in the query using the PostgreSQL LIKE ALL operator. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/sequences#like_all_patterns DataPostgresqlSequences#like_all_patterns}
-        :param like_any_patterns: Expression(s) which will be pattern matched against sequence names in the query using the PostgreSQL LIKE ANY operator. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/sequences#like_any_patterns DataPostgresqlSequences#like_any_patterns}
-        :param not_like_all_patterns: Expression(s) which will be pattern matched against sequence names in the query using the PostgreSQL NOT LIKE ALL operator. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/sequences#not_like_all_patterns DataPostgresqlSequences#not_like_all_patterns}
-        :param regex_pattern: Expression which will be pattern matched against sequence names in the query using the PostgreSQL ~ (regular expression match) operator. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/sequences#regex_pattern DataPostgresqlSequences#regex_pattern}
-        :param schemas: The PostgreSQL schema(s) which will be queried for sequence names. Queries all schemas in the database by default. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/sequences#schemas DataPostgresqlSequences#schemas}
+        :param database: The PostgreSQL database which will be queried for sequence names. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/sequences#database DataPostgresqlSequences#database}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/sequences#id DataPostgresqlSequences#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param like_all_patterns: Expression(s) which will be pattern matched against sequence names in the query using the PostgreSQL LIKE ALL operator. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/sequences#like_all_patterns DataPostgresqlSequences#like_all_patterns}
+        :param like_any_patterns: Expression(s) which will be pattern matched against sequence names in the query using the PostgreSQL LIKE ANY operator. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/sequences#like_any_patterns DataPostgresqlSequences#like_any_patterns}
+        :param not_like_all_patterns: Expression(s) which will be pattern matched against sequence names in the query using the PostgreSQL NOT LIKE ALL operator. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/sequences#not_like_all_patterns DataPostgresqlSequences#not_like_all_patterns}
+        :param regex_pattern: Expression which will be pattern matched against sequence names in the query using the PostgreSQL ~ (regular expression match) operator. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/sequences#regex_pattern DataPostgresqlSequences#regex_pattern}
+        :param schemas: The PostgreSQL schema(s) which will be queried for sequence names. Queries all schemas in the database by default. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/sequences#schemas DataPostgresqlSequences#schemas}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -291,21 +291,21 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param database: The PostgreSQL database which will be queried for sequence names. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/sequences#database DataPostgresqlSequences#database}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/sequences#id DataPostgresqlSequences#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param like_all_patterns: Expression(s) which will be pattern matched against sequence names in the query using the PostgreSQL LIKE ALL operator. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/sequences#like_all_patterns DataPostgresqlSequences#like_all_patterns}
-        :param like_any_patterns: Expression(s) which will be pattern matched against sequence names in the query using the PostgreSQL LIKE ANY operator. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/sequences#like_any_patterns DataPostgresqlSequences#like_any_patterns}
-        :param not_like_all_patterns: Expression(s) which will be pattern matched against sequence names in the query using the PostgreSQL NOT LIKE ALL operator. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/sequences#not_like_all_patterns DataPostgresqlSequences#not_like_all_patterns}
-        :param regex_pattern: Expression which will be pattern matched against sequence names in the query using the PostgreSQL ~ (regular expression match) operator. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/sequences#regex_pattern DataPostgresqlSequences#regex_pattern}
-        :param schemas: The PostgreSQL schema(s) which will be queried for sequence names. Queries all schemas in the database by default. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/sequences#schemas DataPostgresqlSequences#schemas}
+        :param database: The PostgreSQL database which will be queried for sequence names. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/sequences#database DataPostgresqlSequences#database}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/sequences#id DataPostgresqlSequences#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param like_all_patterns: Expression(s) which will be pattern matched against sequence names in the query using the PostgreSQL LIKE ALL operator. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/sequences#like_all_patterns DataPostgresqlSequences#like_all_patterns}
+        :param like_any_patterns: Expression(s) which will be pattern matched against sequence names in the query using the PostgreSQL LIKE ANY operator. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/sequences#like_any_patterns DataPostgresqlSequences#like_any_patterns}
+        :param not_like_all_patterns: Expression(s) which will be pattern matched against sequence names in the query using the PostgreSQL NOT LIKE ALL operator. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/sequences#not_like_all_patterns DataPostgresqlSequences#not_like_all_patterns}
+        :param regex_pattern: Expression which will be pattern matched against sequence names in the query using the PostgreSQL ~ (regular expression match) operator. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/sequences#regex_pattern DataPostgresqlSequences#regex_pattern}
+        :param schemas: The PostgreSQL schema(s) which will be queried for sequence names. Queries all schemas in the database by default. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/sequences#schemas DataPostgresqlSequences#schemas}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__619e1c8023bf202cca3b151256dddd6d991091b7529ba0a0aa0e4adad84ecf35)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -415,71 +415,71 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def database(self) -> builtins.str:
         '''The PostgreSQL database which will be queried for sequence names.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/sequences#database DataPostgresqlSequences#database}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/sequences#database DataPostgresqlSequences#database}
         '''
         result = self._values.get("database")
         assert result is not None, "Required property 'database' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/sequences#id DataPostgresqlSequences#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/sequences#id DataPostgresqlSequences#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def like_all_patterns(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Expression(s) which will be pattern matched against sequence names in the query using the PostgreSQL LIKE ALL operator.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/sequences#like_all_patterns DataPostgresqlSequences#like_all_patterns}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/sequences#like_all_patterns DataPostgresqlSequences#like_all_patterns}
         '''
         result = self._values.get("like_all_patterns")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def like_any_patterns(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Expression(s) which will be pattern matched against sequence names in the query using the PostgreSQL LIKE ANY operator.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/sequences#like_any_patterns DataPostgresqlSequences#like_any_patterns}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/sequences#like_any_patterns DataPostgresqlSequences#like_any_patterns}
         '''
         result = self._values.get("like_any_patterns")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def not_like_all_patterns(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Expression(s) which will be pattern matched against sequence names in the query using the PostgreSQL NOT LIKE ALL operator.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/sequences#not_like_all_patterns DataPostgresqlSequences#not_like_all_patterns}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/sequences#not_like_all_patterns DataPostgresqlSequences#not_like_all_patterns}
         '''
         result = self._values.get("not_like_all_patterns")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def regex_pattern(self) -> typing.Optional[builtins.str]:
         '''Expression which will be pattern matched against sequence names in the query using the PostgreSQL ~ (regular expression match) operator.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/sequences#regex_pattern DataPostgresqlSequences#regex_pattern}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/sequences#regex_pattern DataPostgresqlSequences#regex_pattern}
         '''
         result = self._values.get("regex_pattern")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def schemas(self) -> typing.Optional[typing.List[builtins.str]]:
         '''The PostgreSQL schema(s) which will be queried for sequence names. Queries all schemas in the database by default.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/sequences#schemas DataPostgresqlSequences#schemas}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/sequences#schemas DataPostgresqlSequences#schemas}
         '''
         result = self._values.get("schemas")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/data_postgresql_tables/__init__.py` & `cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/data_postgresql_tables/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_postgresql_tables`
 
-Refer to the Terraform Registory for docs: [`data_postgresql_tables`](https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/tables).
+Refer to the Terraform Registory for docs: [`data_postgresql_tables`](https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/tables).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataPostgresqlTables(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-postgresql.dataPostgresqlTables.DataPostgresqlTables",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/tables postgresql_tables}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/tables postgresql_tables}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         database: builtins.str,
@@ -45,26 +45,26 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/tables postgresql_tables} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/tables postgresql_tables} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param database: The PostgreSQL database which will be queried for table names. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/tables#database DataPostgresqlTables#database}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/tables#id DataPostgresqlTables#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param like_all_patterns: Expression(s) which will be pattern matched against table names in the query using the PostgreSQL LIKE ALL operator. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/tables#like_all_patterns DataPostgresqlTables#like_all_patterns}
-        :param like_any_patterns: Expression(s) which will be pattern matched against table names in the query using the PostgreSQL LIKE ANY operator. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/tables#like_any_patterns DataPostgresqlTables#like_any_patterns}
-        :param not_like_all_patterns: Expression(s) which will be pattern matched against table names in the query using the PostgreSQL NOT LIKE ALL operator. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/tables#not_like_all_patterns DataPostgresqlTables#not_like_all_patterns}
-        :param regex_pattern: Expression which will be pattern matched against table names in the query using the PostgreSQL ~ (regular expression match) operator. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/tables#regex_pattern DataPostgresqlTables#regex_pattern}
-        :param schemas: The PostgreSQL schema(s) which will be queried for table names. Queries all schemas in the database by default. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/tables#schemas DataPostgresqlTables#schemas}
-        :param table_types: The PostgreSQL table types which will be queried for table names. Includes all table types by default. Use 'BASE TABLE' for normal tables only Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/tables#table_types DataPostgresqlTables#table_types}
+        :param database: The PostgreSQL database which will be queried for table names. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/tables#database DataPostgresqlTables#database}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/tables#id DataPostgresqlTables#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param like_all_patterns: Expression(s) which will be pattern matched against table names in the query using the PostgreSQL LIKE ALL operator. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/tables#like_all_patterns DataPostgresqlTables#like_all_patterns}
+        :param like_any_patterns: Expression(s) which will be pattern matched against table names in the query using the PostgreSQL LIKE ANY operator. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/tables#like_any_patterns DataPostgresqlTables#like_any_patterns}
+        :param not_like_all_patterns: Expression(s) which will be pattern matched against table names in the query using the PostgreSQL NOT LIKE ALL operator. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/tables#not_like_all_patterns DataPostgresqlTables#not_like_all_patterns}
+        :param regex_pattern: Expression which will be pattern matched against table names in the query using the PostgreSQL ~ (regular expression match) operator. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/tables#regex_pattern DataPostgresqlTables#regex_pattern}
+        :param schemas: The PostgreSQL schema(s) which will be queried for table names. Queries all schemas in the database by default. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/tables#schemas DataPostgresqlTables#schemas}
+        :param table_types: The PostgreSQL table types which will be queried for table names. Includes all table types by default. Use 'BASE TABLE' for normal tables only Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/tables#table_types DataPostgresqlTables#table_types}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -317,22 +317,22 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param database: The PostgreSQL database which will be queried for table names. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/tables#database DataPostgresqlTables#database}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/tables#id DataPostgresqlTables#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param like_all_patterns: Expression(s) which will be pattern matched against table names in the query using the PostgreSQL LIKE ALL operator. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/tables#like_all_patterns DataPostgresqlTables#like_all_patterns}
-        :param like_any_patterns: Expression(s) which will be pattern matched against table names in the query using the PostgreSQL LIKE ANY operator. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/tables#like_any_patterns DataPostgresqlTables#like_any_patterns}
-        :param not_like_all_patterns: Expression(s) which will be pattern matched against table names in the query using the PostgreSQL NOT LIKE ALL operator. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/tables#not_like_all_patterns DataPostgresqlTables#not_like_all_patterns}
-        :param regex_pattern: Expression which will be pattern matched against table names in the query using the PostgreSQL ~ (regular expression match) operator. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/tables#regex_pattern DataPostgresqlTables#regex_pattern}
-        :param schemas: The PostgreSQL schema(s) which will be queried for table names. Queries all schemas in the database by default. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/tables#schemas DataPostgresqlTables#schemas}
-        :param table_types: The PostgreSQL table types which will be queried for table names. Includes all table types by default. Use 'BASE TABLE' for normal tables only Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/tables#table_types DataPostgresqlTables#table_types}
+        :param database: The PostgreSQL database which will be queried for table names. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/tables#database DataPostgresqlTables#database}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/tables#id DataPostgresqlTables#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param like_all_patterns: Expression(s) which will be pattern matched against table names in the query using the PostgreSQL LIKE ALL operator. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/tables#like_all_patterns DataPostgresqlTables#like_all_patterns}
+        :param like_any_patterns: Expression(s) which will be pattern matched against table names in the query using the PostgreSQL LIKE ANY operator. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/tables#like_any_patterns DataPostgresqlTables#like_any_patterns}
+        :param not_like_all_patterns: Expression(s) which will be pattern matched against table names in the query using the PostgreSQL NOT LIKE ALL operator. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/tables#not_like_all_patterns DataPostgresqlTables#not_like_all_patterns}
+        :param regex_pattern: Expression which will be pattern matched against table names in the query using the PostgreSQL ~ (regular expression match) operator. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/tables#regex_pattern DataPostgresqlTables#regex_pattern}
+        :param schemas: The PostgreSQL schema(s) which will be queried for table names. Queries all schemas in the database by default. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/tables#schemas DataPostgresqlTables#schemas}
+        :param table_types: The PostgreSQL table types which will be queried for table names. Includes all table types by default. Use 'BASE TABLE' for normal tables only Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/tables#table_types DataPostgresqlTables#table_types}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__d53b349b190b29730f875970472cbd2390fd55a98ec957d4e3a2c22b7d2001bb)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -445,82 +445,82 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def database(self) -> builtins.str:
         '''The PostgreSQL database which will be queried for table names.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/tables#database DataPostgresqlTables#database}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/tables#database DataPostgresqlTables#database}
         '''
         result = self._values.get("database")
         assert result is not None, "Required property 'database' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/tables#id DataPostgresqlTables#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/tables#id DataPostgresqlTables#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def like_all_patterns(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Expression(s) which will be pattern matched against table names in the query using the PostgreSQL LIKE ALL operator.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/tables#like_all_patterns DataPostgresqlTables#like_all_patterns}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/tables#like_all_patterns DataPostgresqlTables#like_all_patterns}
         '''
         result = self._values.get("like_all_patterns")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def like_any_patterns(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Expression(s) which will be pattern matched against table names in the query using the PostgreSQL LIKE ANY operator.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/tables#like_any_patterns DataPostgresqlTables#like_any_patterns}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/tables#like_any_patterns DataPostgresqlTables#like_any_patterns}
         '''
         result = self._values.get("like_any_patterns")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def not_like_all_patterns(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Expression(s) which will be pattern matched against table names in the query using the PostgreSQL NOT LIKE ALL operator.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/tables#not_like_all_patterns DataPostgresqlTables#not_like_all_patterns}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/tables#not_like_all_patterns DataPostgresqlTables#not_like_all_patterns}
         '''
         result = self._values.get("not_like_all_patterns")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def regex_pattern(self) -> typing.Optional[builtins.str]:
         '''Expression which will be pattern matched against table names in the query using the PostgreSQL ~ (regular expression match) operator.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/tables#regex_pattern DataPostgresqlTables#regex_pattern}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/tables#regex_pattern DataPostgresqlTables#regex_pattern}
         '''
         result = self._values.get("regex_pattern")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def schemas(self) -> typing.Optional[typing.List[builtins.str]]:
         '''The PostgreSQL schema(s) which will be queried for table names. Queries all schemas in the database by default.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/tables#schemas DataPostgresqlTables#schemas}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/tables#schemas DataPostgresqlTables#schemas}
         '''
         result = self._values.get("schemas")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def table_types(self) -> typing.Optional[typing.List[builtins.str]]:
         '''The PostgreSQL table types which will be queried for table names.
 
         Includes all table types by default. Use 'BASE TABLE' for normal tables only
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/data-sources/tables#table_types DataPostgresqlTables#table_types}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/data-sources/tables#table_types DataPostgresqlTables#table_types}
         '''
         result = self._values.get("table_types")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/database/__init__.py` & `cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/database/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `postgresql_database`
 
-Refer to the Terraform Registory for docs: [`postgresql_database`](https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/database).
+Refer to the Terraform Registory for docs: [`postgresql_database`](https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/database).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class Database(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-postgresql.database.Database",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/database postgresql_database}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/database postgresql_database}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         name: builtins.str,
@@ -48,29 +48,29 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/database postgresql_database} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/database postgresql_database} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: The PostgreSQL database name to connect to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/database#name Database#name}
-        :param allow_connections: If false then no one can connect to this database. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/database#allow_connections Database#allow_connections}
-        :param connection_limit: How many concurrent connections can be made to this database. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/database#connection_limit Database#connection_limit}
-        :param encoding: Character set encoding to use in the new database. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/database#encoding Database#encoding}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/database#id Database#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param is_template: If true, then this database can be cloned by any user with CREATEDB privileges. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/database#is_template Database#is_template}
-        :param lc_collate: Collation order (LC_COLLATE) to use in the new database. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/database#lc_collate Database#lc_collate}
-        :param lc_ctype: Character classification (LC_CTYPE) to use in the new database. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/database#lc_ctype Database#lc_ctype}
-        :param owner: The ROLE which owns the database. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/database#owner Database#owner}
-        :param tablespace_name: The name of the tablespace that will be associated with the new database. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/database#tablespace_name Database#tablespace_name}
-        :param template: The name of the template from which to create the new database. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/database#template Database#template}
+        :param name: The PostgreSQL database name to connect to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/database#name Database#name}
+        :param allow_connections: If false then no one can connect to this database. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/database#allow_connections Database#allow_connections}
+        :param connection_limit: How many concurrent connections can be made to this database. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/database#connection_limit Database#connection_limit}
+        :param encoding: Character set encoding to use in the new database. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/database#encoding Database#encoding}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/database#id Database#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param is_template: If true, then this database can be cloned by any user with CREATEDB privileges. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/database#is_template Database#is_template}
+        :param lc_collate: Collation order (LC_COLLATE) to use in the new database. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/database#lc_collate Database#lc_collate}
+        :param lc_ctype: Character classification (LC_CTYPE) to use in the new database. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/database#lc_ctype Database#lc_ctype}
+        :param owner: The ROLE which owns the database. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/database#owner Database#owner}
+        :param tablespace_name: The name of the tablespace that will be associated with the new database. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/database#tablespace_name Database#tablespace_name}
+        :param template: The name of the template from which to create the new database. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/database#template Database#template}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -402,25 +402,25 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: The PostgreSQL database name to connect to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/database#name Database#name}
-        :param allow_connections: If false then no one can connect to this database. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/database#allow_connections Database#allow_connections}
-        :param connection_limit: How many concurrent connections can be made to this database. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/database#connection_limit Database#connection_limit}
-        :param encoding: Character set encoding to use in the new database. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/database#encoding Database#encoding}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/database#id Database#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param is_template: If true, then this database can be cloned by any user with CREATEDB privileges. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/database#is_template Database#is_template}
-        :param lc_collate: Collation order (LC_COLLATE) to use in the new database. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/database#lc_collate Database#lc_collate}
-        :param lc_ctype: Character classification (LC_CTYPE) to use in the new database. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/database#lc_ctype Database#lc_ctype}
-        :param owner: The ROLE which owns the database. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/database#owner Database#owner}
-        :param tablespace_name: The name of the tablespace that will be associated with the new database. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/database#tablespace_name Database#tablespace_name}
-        :param template: The name of the template from which to create the new database. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/database#template Database#template}
+        :param name: The PostgreSQL database name to connect to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/database#name Database#name}
+        :param allow_connections: If false then no one can connect to this database. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/database#allow_connections Database#allow_connections}
+        :param connection_limit: How many concurrent connections can be made to this database. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/database#connection_limit Database#connection_limit}
+        :param encoding: Character set encoding to use in the new database. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/database#encoding Database#encoding}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/database#id Database#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param is_template: If true, then this database can be cloned by any user with CREATEDB privileges. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/database#is_template Database#is_template}
+        :param lc_collate: Collation order (LC_COLLATE) to use in the new database. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/database#lc_collate Database#lc_collate}
+        :param lc_ctype: Character classification (LC_CTYPE) to use in the new database. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/database#lc_ctype Database#lc_ctype}
+        :param owner: The ROLE which owns the database. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/database#owner Database#owner}
+        :param tablespace_name: The name of the tablespace that will be associated with the new database. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/database#tablespace_name Database#tablespace_name}
+        :param template: The name of the template from which to create the new database. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/database#template Database#template}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__35a5c521a99bf34c41e4b2f9faa8089cce3466060837bbfc88129d48a3c40b29)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -542,111 +542,111 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''The PostgreSQL database name to connect to.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/database#name Database#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/database#name Database#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def allow_connections(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''If false then no one can connect to this database.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/database#allow_connections Database#allow_connections}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/database#allow_connections Database#allow_connections}
         '''
         result = self._values.get("allow_connections")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def connection_limit(self) -> typing.Optional[jsii.Number]:
         '''How many concurrent connections can be made to this database.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/database#connection_limit Database#connection_limit}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/database#connection_limit Database#connection_limit}
         '''
         result = self._values.get("connection_limit")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def encoding(self) -> typing.Optional[builtins.str]:
         '''Character set encoding to use in the new database.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/database#encoding Database#encoding}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/database#encoding Database#encoding}
         '''
         result = self._values.get("encoding")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/database#id Database#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/database#id Database#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def is_template(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''If true, then this database can be cloned by any user with CREATEDB privileges.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/database#is_template Database#is_template}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/database#is_template Database#is_template}
         '''
         result = self._values.get("is_template")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def lc_collate(self) -> typing.Optional[builtins.str]:
         '''Collation order (LC_COLLATE) to use in the new database.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/database#lc_collate Database#lc_collate}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/database#lc_collate Database#lc_collate}
         '''
         result = self._values.get("lc_collate")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def lc_ctype(self) -> typing.Optional[builtins.str]:
         '''Character classification (LC_CTYPE) to use in the new database.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/database#lc_ctype Database#lc_ctype}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/database#lc_ctype Database#lc_ctype}
         '''
         result = self._values.get("lc_ctype")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def owner(self) -> typing.Optional[builtins.str]:
         '''The ROLE which owns the database.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/database#owner Database#owner}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/database#owner Database#owner}
         '''
         result = self._values.get("owner")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def tablespace_name(self) -> typing.Optional[builtins.str]:
         '''The name of the tablespace that will be associated with the new database.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/database#tablespace_name Database#tablespace_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/database#tablespace_name Database#tablespace_name}
         '''
         result = self._values.get("tablespace_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def template(self) -> typing.Optional[builtins.str]:
         '''The name of the template from which to create the new database.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/database#template Database#template}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/database#template Database#template}
         '''
         result = self._values.get("template")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/default_privileges/__init__.py` & `cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/default_privileges/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `postgresql_default_privileges`
 
-Refer to the Terraform Registory for docs: [`postgresql_default_privileges`](https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/default_privileges).
+Refer to the Terraform Registory for docs: [`postgresql_default_privileges`](https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/default_privileges).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DefaultPrivileges(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-postgresql.defaultPrivileges.DefaultPrivileges",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/default_privileges postgresql_default_privileges}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/default_privileges postgresql_default_privileges}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         database: builtins.str,
@@ -45,26 +45,26 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/default_privileges postgresql_default_privileges} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/default_privileges postgresql_default_privileges} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param database: The database to grant default privileges for this role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/default_privileges#database DefaultPrivileges#database}
-        :param object_type: The PostgreSQL object type to set the default privileges on (one of: table, sequence, function, type, schema). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/default_privileges#object_type DefaultPrivileges#object_type}
-        :param owner: Target role for which to alter default privileges. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/default_privileges#owner DefaultPrivileges#owner}
-        :param privileges: The list of privileges to apply as default privileges. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/default_privileges#privileges DefaultPrivileges#privileges}
-        :param role: The name of the role to which grant default privileges on. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/default_privileges#role DefaultPrivileges#role}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/default_privileges#id DefaultPrivileges#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param schema: The database schema to set default privileges for this role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/default_privileges#schema DefaultPrivileges#schema}
-        :param with_grant_option: Permit the grant recipient to grant it to others. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/default_privileges#with_grant_option DefaultPrivileges#with_grant_option}
+        :param database: The database to grant default privileges for this role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/default_privileges#database DefaultPrivileges#database}
+        :param object_type: The PostgreSQL object type to set the default privileges on (one of: table, sequence, function, type, schema). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/default_privileges#object_type DefaultPrivileges#object_type}
+        :param owner: Target role for which to alter default privileges. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/default_privileges#owner DefaultPrivileges#owner}
+        :param privileges: The list of privileges to apply as default privileges. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/default_privileges#privileges DefaultPrivileges#privileges}
+        :param role: The name of the role to which grant default privileges on. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/default_privileges#role DefaultPrivileges#role}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/default_privileges#id DefaultPrivileges#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param schema: The database schema to set default privileges for this role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/default_privileges#schema DefaultPrivileges#schema}
+        :param with_grant_option: Permit the grant recipient to grant it to others. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/default_privileges#with_grant_option DefaultPrivileges#with_grant_option}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -303,22 +303,22 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param database: The database to grant default privileges for this role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/default_privileges#database DefaultPrivileges#database}
-        :param object_type: The PostgreSQL object type to set the default privileges on (one of: table, sequence, function, type, schema). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/default_privileges#object_type DefaultPrivileges#object_type}
-        :param owner: Target role for which to alter default privileges. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/default_privileges#owner DefaultPrivileges#owner}
-        :param privileges: The list of privileges to apply as default privileges. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/default_privileges#privileges DefaultPrivileges#privileges}
-        :param role: The name of the role to which grant default privileges on. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/default_privileges#role DefaultPrivileges#role}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/default_privileges#id DefaultPrivileges#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param schema: The database schema to set default privileges for this role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/default_privileges#schema DefaultPrivileges#schema}
-        :param with_grant_option: Permit the grant recipient to grant it to others. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/default_privileges#with_grant_option DefaultPrivileges#with_grant_option}
+        :param database: The database to grant default privileges for this role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/default_privileges#database DefaultPrivileges#database}
+        :param object_type: The PostgreSQL object type to set the default privileges on (one of: table, sequence, function, type, schema). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/default_privileges#object_type DefaultPrivileges#object_type}
+        :param owner: Target role for which to alter default privileges. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/default_privileges#owner DefaultPrivileges#owner}
+        :param privileges: The list of privileges to apply as default privileges. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/default_privileges#privileges DefaultPrivileges#privileges}
+        :param role: The name of the role to which grant default privileges on. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/default_privileges#role DefaultPrivileges#role}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/default_privileges#id DefaultPrivileges#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param schema: The database schema to set default privileges for this role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/default_privileges#schema DefaultPrivileges#schema}
+        :param with_grant_option: Permit the grant recipient to grant it to others. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/default_privileges#with_grant_option DefaultPrivileges#with_grant_option}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__1c435f40ceb2a7f62a7dbfbf537eaf680b4460e45b19948859c945c28973a606)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -427,86 +427,86 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def database(self) -> builtins.str:
         '''The database to grant default privileges for this role.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/default_privileges#database DefaultPrivileges#database}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/default_privileges#database DefaultPrivileges#database}
         '''
         result = self._values.get("database")
         assert result is not None, "Required property 'database' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def object_type(self) -> builtins.str:
         '''The PostgreSQL object type to set the default privileges on (one of: table, sequence, function, type, schema).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/default_privileges#object_type DefaultPrivileges#object_type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/default_privileges#object_type DefaultPrivileges#object_type}
         '''
         result = self._values.get("object_type")
         assert result is not None, "Required property 'object_type' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def owner(self) -> builtins.str:
         '''Target role for which to alter default privileges.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/default_privileges#owner DefaultPrivileges#owner}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/default_privileges#owner DefaultPrivileges#owner}
         '''
         result = self._values.get("owner")
         assert result is not None, "Required property 'owner' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def privileges(self) -> typing.List[builtins.str]:
         '''The list of privileges to apply as default privileges.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/default_privileges#privileges DefaultPrivileges#privileges}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/default_privileges#privileges DefaultPrivileges#privileges}
         '''
         result = self._values.get("privileges")
         assert result is not None, "Required property 'privileges' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     @builtins.property
     def role(self) -> builtins.str:
         '''The name of the role to which grant default privileges on.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/default_privileges#role DefaultPrivileges#role}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/default_privileges#role DefaultPrivileges#role}
         '''
         result = self._values.get("role")
         assert result is not None, "Required property 'role' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/default_privileges#id DefaultPrivileges#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/default_privileges#id DefaultPrivileges#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def schema(self) -> typing.Optional[builtins.str]:
         '''The database schema to set default privileges for this role.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/default_privileges#schema DefaultPrivileges#schema}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/default_privileges#schema DefaultPrivileges#schema}
         '''
         result = self._values.get("schema")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def with_grant_option(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Permit the grant recipient to grant it to others.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/default_privileges#with_grant_option DefaultPrivileges#with_grant_option}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/default_privileges#with_grant_option DefaultPrivileges#with_grant_option}
         '''
         result = self._values.get("with_grant_option")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/extension/__init__.py` & `cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/extension/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `postgresql_extension`
 
-Refer to the Terraform Registory for docs: [`postgresql_extension`](https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/extension).
+Refer to the Terraform Registory for docs: [`postgresql_extension`](https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/extension).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class Extension(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-postgresql.extension.Extension",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/extension postgresql_extension}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/extension postgresql_extension}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         name: builtins.str,
@@ -44,25 +44,25 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/extension postgresql_extension} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/extension postgresql_extension} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/extension#name Extension#name}.
-        :param create_cascade: When true, will also create any extensions that this extension depends on that are not already installed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/extension#create_cascade Extension#create_cascade}
-        :param database: Sets the database to add the extension to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/extension#database Extension#database}
-        :param drop_cascade: When true, will also drop all the objects that depend on the extension, and in turn all objects that depend on those objects. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/extension#drop_cascade Extension#drop_cascade}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/extension#id Extension#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param schema: Sets the schema of an extension. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/extension#schema Extension#schema}
-        :param version: Sets the version number of the extension. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/extension#version Extension#version}
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/extension#name Extension#name}.
+        :param create_cascade: When true, will also create any extensions that this extension depends on that are not already installed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/extension#create_cascade Extension#create_cascade}
+        :param database: Sets the database to add the extension to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/extension#database Extension#database}
+        :param drop_cascade: When true, will also drop all the objects that depend on the extension, and in turn all objects that depend on those objects. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/extension#drop_cascade Extension#drop_cascade}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/extension#id Extension#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param schema: Sets the schema of an extension. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/extension#schema Extension#schema}
+        :param version: Sets the version number of the extension. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/extension#version Extension#version}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -298,21 +298,21 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/extension#name Extension#name}.
-        :param create_cascade: When true, will also create any extensions that this extension depends on that are not already installed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/extension#create_cascade Extension#create_cascade}
-        :param database: Sets the database to add the extension to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/extension#database Extension#database}
-        :param drop_cascade: When true, will also drop all the objects that depend on the extension, and in turn all objects that depend on those objects. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/extension#drop_cascade Extension#drop_cascade}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/extension#id Extension#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param schema: Sets the schema of an extension. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/extension#schema Extension#schema}
-        :param version: Sets the version number of the extension. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/extension#version Extension#version}
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/extension#name Extension#name}.
+        :param create_cascade: When true, will also create any extensions that this extension depends on that are not already installed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/extension#create_cascade Extension#create_cascade}
+        :param database: Sets the database to add the extension to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/extension#database Extension#database}
+        :param drop_cascade: When true, will also drop all the objects that depend on the extension, and in turn all objects that depend on those objects. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/extension#drop_cascade Extension#drop_cascade}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/extension#id Extension#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param schema: Sets the schema of an extension. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/extension#schema Extension#schema}
+        :param version: Sets the version number of the extension. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/extension#version Extension#version}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__a9844e4441cfaf546d81456ca6ea2ada9046a92cf93cdb5725a16da4d72ae4ce)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -420,74 +420,74 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/extension#name Extension#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/extension#name Extension#name}.'''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def create_cascade(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''When true, will also create any extensions that this extension depends on that are not already installed.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/extension#create_cascade Extension#create_cascade}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/extension#create_cascade Extension#create_cascade}
         '''
         result = self._values.get("create_cascade")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def database(self) -> typing.Optional[builtins.str]:
         '''Sets the database to add the extension to.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/extension#database Extension#database}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/extension#database Extension#database}
         '''
         result = self._values.get("database")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def drop_cascade(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''When true, will also drop all the objects that depend on the extension, and in turn all objects that depend on those objects.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/extension#drop_cascade Extension#drop_cascade}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/extension#drop_cascade Extension#drop_cascade}
         '''
         result = self._values.get("drop_cascade")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/extension#id Extension#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/extension#id Extension#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def schema(self) -> typing.Optional[builtins.str]:
         '''Sets the schema of an extension.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/extension#schema Extension#schema}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/extension#schema Extension#schema}
         '''
         result = self._values.get("schema")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def version(self) -> typing.Optional[builtins.str]:
         '''Sets the version number of the extension.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/extension#version Extension#version}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/extension#version Extension#version}
         '''
         result = self._values.get("version")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/function_resource/__init__.py` & `cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/function_resource/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `postgresql_function`
 
-Refer to the Terraform Registory for docs: [`postgresql_function`](https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/function).
+Refer to the Terraform Registory for docs: [`postgresql_function`](https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/function).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class FunctionResource(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-postgresql.functionResource.FunctionResource",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/function postgresql_function}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/function postgresql_function}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         body: builtins.str,
@@ -46,27 +46,27 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/function postgresql_function} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/function postgresql_function} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param body: Body of the function. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/function#body FunctionResource#body}
-        :param name: Name of the function. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/function#name FunctionResource#name}
-        :param arg: arg block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/function#arg FunctionResource#arg}
-        :param database: The database where the function is located. If not specified, the provider default database is used. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/function#database FunctionResource#database}
-        :param drop_cascade: Automatically drop objects that depend on the function (such as operators or triggers), and in turn all objects that depend on those objects. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/function#drop_cascade FunctionResource#drop_cascade}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/function#id FunctionResource#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param language: Language of theof the function. One of: internal, sql, c, plpgsql. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/function#language FunctionResource#language}
-        :param returns: Function return type. If not specified, it will be calculated based on the output arguments. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/function#returns FunctionResource#returns}
-        :param schema: Schema where the function is located. If not specified, the provider default schema is used. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/function#schema FunctionResource#schema}
+        :param body: Body of the function. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/function#body FunctionResource#body}
+        :param name: Name of the function. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/function#name FunctionResource#name}
+        :param arg: arg block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/function#arg FunctionResource#arg}
+        :param database: The database where the function is located. If not specified, the provider default database is used. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/function#database FunctionResource#database}
+        :param drop_cascade: Automatically drop objects that depend on the function (such as operators or triggers), and in turn all objects that depend on those objects. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/function#drop_cascade FunctionResource#drop_cascade}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/function#id FunctionResource#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param language: Language of theof the function. One of: internal, sql, c, plpgsql. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/function#language FunctionResource#language}
+        :param returns: Function return type. If not specified, it will be calculated based on the output arguments. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/function#returns FunctionResource#returns}
+        :param schema: Schema where the function is located. If not specified, the provider default schema is used. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/function#schema FunctionResource#schema}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -316,18 +316,18 @@
         *,
         type: builtins.str,
         default: typing.Optional[builtins.str] = None,
         mode: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param type: The argument type. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/function#type FunctionResource#type}
-        :param default: An expression to be used as default value if the parameter is not specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/function#default FunctionResource#default}
-        :param mode: The argument mode. One of: IN, OUT, INOUT, or VARIADIC. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/function#mode FunctionResource#mode}
-        :param name: The argument name. The name may be required for some languages or depending on the argument mode. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/function#name FunctionResource#name}
+        :param type: The argument type. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/function#type FunctionResource#type}
+        :param default: An expression to be used as default value if the parameter is not specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/function#default FunctionResource#default}
+        :param mode: The argument mode. One of: IN, OUT, INOUT, or VARIADIC. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/function#mode FunctionResource#mode}
+        :param name: The argument name. The name may be required for some languages or depending on the argument mode. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/function#name FunctionResource#name}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__36dddaca1c2a9cadedda015d6884c00e31c924a3cfa14e5fcc1502466efe5ba1)
             check_type(argname="argument type", value=type, expected_type=type_hints["type"])
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
             check_type(argname="argument mode", value=mode, expected_type=type_hints["mode"])
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
@@ -341,43 +341,43 @@
         if name is not None:
             self._values["name"] = name
 
     @builtins.property
     def type(self) -> builtins.str:
         '''The argument type.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/function#type FunctionResource#type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/function#type FunctionResource#type}
         '''
         result = self._values.get("type")
         assert result is not None, "Required property 'type' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
         '''An expression to be used as default value if the parameter is not specified.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/function#default FunctionResource#default}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/function#default FunctionResource#default}
         '''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def mode(self) -> typing.Optional[builtins.str]:
         '''The argument mode. One of: IN, OUT, INOUT, or VARIADIC.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/function#mode FunctionResource#mode}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/function#mode FunctionResource#mode}
         '''
         result = self._values.get("mode")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The argument name. The name may be required for some languages or depending on the argument mode.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/function#name FunctionResource#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/function#name FunctionResource#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -586,21 +586,21 @@
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "type", value)
 
     @builtins.property
     @jsii.member(jsii_name="internalValue")
     def internal_value(
         self,
-    ) -> typing.Optional[typing.Union[FunctionResourceArg, _cdktf_9a9027ec.IResolvable]]:
-        return typing.cast(typing.Optional[typing.Union[FunctionResourceArg, _cdktf_9a9027ec.IResolvable]], jsii.get(self, "internalValue"))
+    ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, FunctionResourceArg]]:
+        return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, FunctionResourceArg]], jsii.get(self, "internalValue"))
 
     @internal_value.setter
     def internal_value(
         self,
-        value: typing.Optional[typing.Union[FunctionResourceArg, _cdktf_9a9027ec.IResolvable]],
+        value: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, FunctionResourceArg]],
     ) -> None:
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__0ca966d1a600f6fbb0ebd5886a435a10dc8449c4e7225dbbbfee9c4b414e1860)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internalValue", value)
 
 
@@ -651,23 +651,23 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param body: Body of the function. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/function#body FunctionResource#body}
-        :param name: Name of the function. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/function#name FunctionResource#name}
-        :param arg: arg block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/function#arg FunctionResource#arg}
-        :param database: The database where the function is located. If not specified, the provider default database is used. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/function#database FunctionResource#database}
-        :param drop_cascade: Automatically drop objects that depend on the function (such as operators or triggers), and in turn all objects that depend on those objects. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/function#drop_cascade FunctionResource#drop_cascade}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/function#id FunctionResource#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param language: Language of theof the function. One of: internal, sql, c, plpgsql. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/function#language FunctionResource#language}
-        :param returns: Function return type. If not specified, it will be calculated based on the output arguments. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/function#returns FunctionResource#returns}
-        :param schema: Schema where the function is located. If not specified, the provider default schema is used. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/function#schema FunctionResource#schema}
+        :param body: Body of the function. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/function#body FunctionResource#body}
+        :param name: Name of the function. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/function#name FunctionResource#name}
+        :param arg: arg block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/function#arg FunctionResource#arg}
+        :param database: The database where the function is located. If not specified, the provider default database is used. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/function#database FunctionResource#database}
+        :param drop_cascade: Automatically drop objects that depend on the function (such as operators or triggers), and in turn all objects that depend on those objects. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/function#drop_cascade FunctionResource#drop_cascade}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/function#id FunctionResource#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param language: Language of theof the function. One of: internal, sql, c, plpgsql. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/function#language FunctionResource#language}
+        :param returns: Function return type. If not specified, it will be calculated based on the output arguments. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/function#returns FunctionResource#returns}
+        :param schema: Schema where the function is located. If not specified, the provider default schema is used. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/function#schema FunctionResource#schema}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__eb26d2000763f502eafe20caf4ff13b4f8623ec653a1ace5c61d18088d4f1bcd)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -782,94 +782,94 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def body(self) -> builtins.str:
         '''Body of the function.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/function#body FunctionResource#body}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/function#body FunctionResource#body}
         '''
         result = self._values.get("body")
         assert result is not None, "Required property 'body' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''Name of the function.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/function#name FunctionResource#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/function#name FunctionResource#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def arg(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[FunctionResourceArg]]]:
         '''arg block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/function#arg FunctionResource#arg}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/function#arg FunctionResource#arg}
         '''
         result = self._values.get("arg")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[FunctionResourceArg]]], result)
 
     @builtins.property
     def database(self) -> typing.Optional[builtins.str]:
         '''The database where the function is located. If not specified, the provider default database is used.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/function#database FunctionResource#database}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/function#database FunctionResource#database}
         '''
         result = self._values.get("database")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def drop_cascade(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Automatically drop objects that depend on the function (such as operators or triggers), and in turn all objects that depend on those objects.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/function#drop_cascade FunctionResource#drop_cascade}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/function#drop_cascade FunctionResource#drop_cascade}
         '''
         result = self._values.get("drop_cascade")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/function#id FunctionResource#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/function#id FunctionResource#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def language(self) -> typing.Optional[builtins.str]:
         '''Language of theof the function. One of: internal, sql, c, plpgsql.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/function#language FunctionResource#language}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/function#language FunctionResource#language}
         '''
         result = self._values.get("language")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def returns(self) -> typing.Optional[builtins.str]:
         '''Function return type. If not specified, it will be calculated based on the output arguments.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/function#returns FunctionResource#returns}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/function#returns FunctionResource#returns}
         '''
         result = self._values.get("returns")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def schema(self) -> typing.Optional[builtins.str]:
         '''Schema where the function is located. If not specified, the provider default schema is used.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/function#schema FunctionResource#schema}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/function#schema FunctionResource#schema}
         '''
         result = self._values.get("schema")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -1048,15 +1048,15 @@
 def _typecheckingstub__df54c0b7228f02f1fafd1b218e4384ef612566d890a155ab3a4bc876ab04789f(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__0ca966d1a600f6fbb0ebd5886a435a10dc8449c4e7225dbbbfee9c4b414e1860(
-    value: typing.Optional[typing.Union[FunctionResourceArg, _cdktf_9a9027ec.IResolvable]],
+    value: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, FunctionResourceArg]],
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__eb26d2000763f502eafe20caf4ff13b4f8623ec653a1ace5c61d18088d4f1bcd(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
```

### Comparing `cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/grant/__init__.py` & `cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/grant/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `postgresql_grant`
 
-Refer to the Terraform Registory for docs: [`postgresql_grant`](https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/grant).
+Refer to the Terraform Registory for docs: [`postgresql_grant`](https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/grant).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class Grant(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-postgresql.grant.Grant",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/grant postgresql_grant}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/grant postgresql_grant}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         database: builtins.str,
@@ -46,27 +46,27 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/grant postgresql_grant} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/grant postgresql_grant} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param database: The database to grant privileges on for this role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/grant#database Grant#database}
-        :param object_type: The PostgreSQL object type to grant the privileges on (one of: database, function, procedure, routine, schema, sequence, table, foreign_data_wrapper, foreign_server, column). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/grant#object_type Grant#object_type}
-        :param privileges: The list of privileges to grant. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/grant#privileges Grant#privileges}
-        :param role: The name of the role to grant privileges on. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/grant#role Grant#role}
-        :param columns: The specific columns to grant privileges on for this role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/grant#columns Grant#columns}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/grant#id Grant#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param objects: The specific objects to grant privileges on for this role (empty means all objects of the requested type). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/grant#objects Grant#objects}
-        :param schema: The database schema to grant privileges on for this role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/grant#schema Grant#schema}
-        :param with_grant_option: Permit the grant recipient to grant it to others. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/grant#with_grant_option Grant#with_grant_option}
+        :param database: The database to grant privileges on for this role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/grant#database Grant#database}
+        :param object_type: The PostgreSQL object type to grant the privileges on (one of: database, function, procedure, routine, schema, sequence, table, foreign_data_wrapper, foreign_server, column). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/grant#object_type Grant#object_type}
+        :param privileges: The list of privileges to grant. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/grant#privileges Grant#privileges}
+        :param role: The name of the role to grant privileges on. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/grant#role Grant#role}
+        :param columns: The specific columns to grant privileges on for this role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/grant#columns Grant#columns}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/grant#id Grant#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param objects: The specific objects to grant privileges on for this role (empty means all objects of the requested type). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/grant#objects Grant#objects}
+        :param schema: The database schema to grant privileges on for this role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/grant#schema Grant#schema}
+        :param with_grant_option: Permit the grant recipient to grant it to others. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/grant#with_grant_option Grant#with_grant_option}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -333,23 +333,23 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param database: The database to grant privileges on for this role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/grant#database Grant#database}
-        :param object_type: The PostgreSQL object type to grant the privileges on (one of: database, function, procedure, routine, schema, sequence, table, foreign_data_wrapper, foreign_server, column). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/grant#object_type Grant#object_type}
-        :param privileges: The list of privileges to grant. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/grant#privileges Grant#privileges}
-        :param role: The name of the role to grant privileges on. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/grant#role Grant#role}
-        :param columns: The specific columns to grant privileges on for this role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/grant#columns Grant#columns}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/grant#id Grant#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param objects: The specific objects to grant privileges on for this role (empty means all objects of the requested type). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/grant#objects Grant#objects}
-        :param schema: The database schema to grant privileges on for this role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/grant#schema Grant#schema}
-        :param with_grant_option: Permit the grant recipient to grant it to others. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/grant#with_grant_option Grant#with_grant_option}
+        :param database: The database to grant privileges on for this role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/grant#database Grant#database}
+        :param object_type: The PostgreSQL object type to grant the privileges on (one of: database, function, procedure, routine, schema, sequence, table, foreign_data_wrapper, foreign_server, column). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/grant#object_type Grant#object_type}
+        :param privileges: The list of privileges to grant. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/grant#privileges Grant#privileges}
+        :param role: The name of the role to grant privileges on. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/grant#role Grant#role}
+        :param columns: The specific columns to grant privileges on for this role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/grant#columns Grant#columns}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/grant#id Grant#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param objects: The specific objects to grant privileges on for this role (empty means all objects of the requested type). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/grant#objects Grant#objects}
+        :param schema: The database schema to grant privileges on for this role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/grant#schema Grant#schema}
+        :param with_grant_option: Permit the grant recipient to grant it to others. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/grant#with_grant_option Grant#with_grant_option}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__be10000ff6b3ae0b422debb2d5ce4447a92f910054bf8ed517b54dae637252ce)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -462,94 +462,94 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def database(self) -> builtins.str:
         '''The database to grant privileges on for this role.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/grant#database Grant#database}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/grant#database Grant#database}
         '''
         result = self._values.get("database")
         assert result is not None, "Required property 'database' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def object_type(self) -> builtins.str:
         '''The PostgreSQL object type to grant the privileges on (one of: database, function, procedure, routine, schema, sequence, table, foreign_data_wrapper, foreign_server, column).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/grant#object_type Grant#object_type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/grant#object_type Grant#object_type}
         '''
         result = self._values.get("object_type")
         assert result is not None, "Required property 'object_type' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def privileges(self) -> typing.List[builtins.str]:
         '''The list of privileges to grant.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/grant#privileges Grant#privileges}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/grant#privileges Grant#privileges}
         '''
         result = self._values.get("privileges")
         assert result is not None, "Required property 'privileges' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     @builtins.property
     def role(self) -> builtins.str:
         '''The name of the role to grant privileges on.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/grant#role Grant#role}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/grant#role Grant#role}
         '''
         result = self._values.get("role")
         assert result is not None, "Required property 'role' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def columns(self) -> typing.Optional[typing.List[builtins.str]]:
         '''The specific columns to grant privileges on for this role.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/grant#columns Grant#columns}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/grant#columns Grant#columns}
         '''
         result = self._values.get("columns")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/grant#id Grant#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/grant#id Grant#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def objects(self) -> typing.Optional[typing.List[builtins.str]]:
         '''The specific objects to grant privileges on for this role (empty means all objects of the requested type).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/grant#objects Grant#objects}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/grant#objects Grant#objects}
         '''
         result = self._values.get("objects")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def schema(self) -> typing.Optional[builtins.str]:
         '''The database schema to grant privileges on for this role.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/grant#schema Grant#schema}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/grant#schema Grant#schema}
         '''
         result = self._values.get("schema")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def with_grant_option(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Permit the grant recipient to grant it to others.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/grant#with_grant_option Grant#with_grant_option}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/grant#with_grant_option Grant#with_grant_option}
         '''
         result = self._values.get("with_grant_option")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/grant_role/__init__.py` & `cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/grant_role/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `postgresql_grant_role`
 
-Refer to the Terraform Registory for docs: [`postgresql_grant_role`](https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/grant_role).
+Refer to the Terraform Registory for docs: [`postgresql_grant_role`](https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/grant_role).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class GrantRole(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-postgresql.grantRole.GrantRole",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/grant_role postgresql_grant_role}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/grant_role postgresql_grant_role}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         grant_role: builtins.str,
@@ -41,22 +41,22 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/grant_role postgresql_grant_role} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/grant_role postgresql_grant_role} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param grant_role: The name of the role that is granted to role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/grant_role#grant_role GrantRole#grant_role}
-        :param role: The name of the role to grant grant_role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/grant_role#role GrantRole#role}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/grant_role#id GrantRole#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param with_admin_option: Permit the grant recipient to grant it to others. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/grant_role#with_admin_option GrantRole#with_admin_option}
+        :param grant_role: The name of the role that is granted to role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/grant_role#grant_role GrantRole#grant_role}
+        :param role: The name of the role to grant grant_role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/grant_role#role GrantRole#role}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/grant_role#id GrantRole#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param with_admin_option: Permit the grant recipient to grant it to others. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/grant_role#with_admin_option GrantRole#with_admin_option}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -211,18 +211,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param grant_role: The name of the role that is granted to role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/grant_role#grant_role GrantRole#grant_role}
-        :param role: The name of the role to grant grant_role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/grant_role#role GrantRole#role}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/grant_role#id GrantRole#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param with_admin_option: Permit the grant recipient to grant it to others. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/grant_role#with_admin_option GrantRole#with_admin_option}
+        :param grant_role: The name of the role that is granted to role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/grant_role#grant_role GrantRole#grant_role}
+        :param role: The name of the role to grant grant_role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/grant_role#role GrantRole#role}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/grant_role#id GrantRole#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param with_admin_option: Permit the grant recipient to grant it to others. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/grant_role#with_admin_option GrantRole#with_admin_option}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__dec030a85aa522b0a5d0cd40cd514b615d17eeab6e6991ae46aeb737a651c419)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -322,47 +322,47 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def grant_role(self) -> builtins.str:
         '''The name of the role that is granted to role.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/grant_role#grant_role GrantRole#grant_role}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/grant_role#grant_role GrantRole#grant_role}
         '''
         result = self._values.get("grant_role")
         assert result is not None, "Required property 'grant_role' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def role(self) -> builtins.str:
         '''The name of the role to grant grant_role.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/grant_role#role GrantRole#role}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/grant_role#role GrantRole#role}
         '''
         result = self._values.get("role")
         assert result is not None, "Required property 'role' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/grant_role#id GrantRole#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/grant_role#id GrantRole#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def with_admin_option(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Permit the grant recipient to grant it to others.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/grant_role#with_admin_option GrantRole#with_admin_option}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/grant_role#with_admin_option GrantRole#with_admin_option}
         '''
         result = self._values.get("with_admin_option")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/physical_replication_slot/__init__.py` & `cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/physical_replication_slot/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `postgresql_physical_replication_slot`
 
-Refer to the Terraform Registory for docs: [`postgresql_physical_replication_slot`](https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/physical_replication_slot).
+Refer to the Terraform Registory for docs: [`postgresql_physical_replication_slot`](https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/physical_replication_slot).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class PhysicalReplicationSlot(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-postgresql.physicalReplicationSlot.PhysicalReplicationSlot",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/physical_replication_slot postgresql_physical_replication_slot}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/physical_replication_slot postgresql_physical_replication_slot}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         name: builtins.str,
@@ -39,20 +39,20 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/physical_replication_slot postgresql_physical_replication_slot} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/physical_replication_slot postgresql_physical_replication_slot} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/physical_replication_slot#name PhysicalReplicationSlot#name}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/physical_replication_slot#id PhysicalReplicationSlot#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/physical_replication_slot#name PhysicalReplicationSlot#name}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/physical_replication_slot#id PhysicalReplicationSlot#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -156,16 +156,16 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/physical_replication_slot#name PhysicalReplicationSlot#name}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/physical_replication_slot#id PhysicalReplicationSlot#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/physical_replication_slot#name PhysicalReplicationSlot#name}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/physical_replication_slot#id PhysicalReplicationSlot#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__9d354cec19a41dc74c3dd3d086ed0f41b930346df9bea361113d0837271bd116)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -258,22 +258,22 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/physical_replication_slot#name PhysicalReplicationSlot#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/physical_replication_slot#name PhysicalReplicationSlot#name}.'''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/physical_replication_slot#id PhysicalReplicationSlot#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/physical_replication_slot#id PhysicalReplicationSlot#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
```

### Comparing `cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/provider/__init__.py` & `cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/provider/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `provider`
 
-Refer to the Terraform Registory for docs: [`postgresql`](https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs).
+Refer to the Terraform Registory for docs: [`postgresql`](https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class PostgresqlProvider(
     _cdktf_9a9027ec.TerraformProvider,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-postgresql.provider.PostgresqlProvider",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs postgresql}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs postgresql}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         alias: typing.Optional[builtins.str] = None,
@@ -49,37 +49,37 @@
         scheme: typing.Optional[builtins.str] = None,
         sslmode: typing.Optional[builtins.str] = None,
         ssl_mode: typing.Optional[builtins.str] = None,
         sslrootcert: typing.Optional[builtins.str] = None,
         superuser: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         username: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs postgresql} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs postgresql} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#alias PostgresqlProvider#alias}
-        :param aws_rds_iam_auth: Use rds_iam instead of password authentication (see: https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/UsingWithRDS.IAMDBAuth.html). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#aws_rds_iam_auth PostgresqlProvider#aws_rds_iam_auth}
-        :param aws_rds_iam_profile: AWS profile to use for IAM auth. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#aws_rds_iam_profile PostgresqlProvider#aws_rds_iam_profile}
-        :param aws_rds_iam_region: AWS region to use for IAM auth. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#aws_rds_iam_region PostgresqlProvider#aws_rds_iam_region}
-        :param clientcert: clientcert block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#clientcert PostgresqlProvider#clientcert}
-        :param connect_timeout: Maximum wait for connection, in seconds. Zero or not specified means wait indefinitely. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#connect_timeout PostgresqlProvider#connect_timeout}
-        :param database: The name of the database to connect to in order to conenct to (defaults to ``postgres``). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#database PostgresqlProvider#database}
-        :param database_username: Database username associated to the connected user (for user name maps). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#database_username PostgresqlProvider#database_username}
-        :param expected_version: Specify the expected version of PostgreSQL. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#expected_version PostgresqlProvider#expected_version}
-        :param host: Name of PostgreSQL server address to connect to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#host PostgresqlProvider#host}
-        :param max_connections: Maximum number of connections to establish to the database. Zero means unlimited. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#max_connections PostgresqlProvider#max_connections}
-        :param password: Password to be used if the PostgreSQL server demands password authentication. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#password PostgresqlProvider#password}
-        :param port: The PostgreSQL port number to connect to at the server host, or socket file name extension for Unix-domain connections. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#port PostgresqlProvider#port}
-        :param scheme: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#scheme PostgresqlProvider#scheme}.
-        :param sslmode: This option determines whether or with what priority a secure SSL TCP/IP connection will be negotiated with the PostgreSQL server. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#sslmode PostgresqlProvider#sslmode}
-        :param ssl_mode: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#ssl_mode PostgresqlProvider#ssl_mode}.
-        :param sslrootcert: The SSL server root certificate file path. The file must contain PEM encoded data. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#sslrootcert PostgresqlProvider#sslrootcert}
-        :param superuser: Specify if the user to connect as is a Postgres superuser or not.If not, some feature might be disabled (e.g.: Refreshing state password from Postgres). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#superuser PostgresqlProvider#superuser}
-        :param username: PostgreSQL user name to connect as. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#username PostgresqlProvider#username}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#alias PostgresqlProvider#alias}
+        :param aws_rds_iam_auth: Use rds_iam instead of password authentication (see: https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/UsingWithRDS.IAMDBAuth.html). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#aws_rds_iam_auth PostgresqlProvider#aws_rds_iam_auth}
+        :param aws_rds_iam_profile: AWS profile to use for IAM auth. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#aws_rds_iam_profile PostgresqlProvider#aws_rds_iam_profile}
+        :param aws_rds_iam_region: AWS region to use for IAM auth. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#aws_rds_iam_region PostgresqlProvider#aws_rds_iam_region}
+        :param clientcert: clientcert block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#clientcert PostgresqlProvider#clientcert}
+        :param connect_timeout: Maximum wait for connection, in seconds. Zero or not specified means wait indefinitely. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#connect_timeout PostgresqlProvider#connect_timeout}
+        :param database: The name of the database to connect to in order to conenct to (defaults to ``postgres``). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#database PostgresqlProvider#database}
+        :param database_username: Database username associated to the connected user (for user name maps). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#database_username PostgresqlProvider#database_username}
+        :param expected_version: Specify the expected version of PostgreSQL. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#expected_version PostgresqlProvider#expected_version}
+        :param host: Name of PostgreSQL server address to connect to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#host PostgresqlProvider#host}
+        :param max_connections: Maximum number of connections to establish to the database. Zero means unlimited. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#max_connections PostgresqlProvider#max_connections}
+        :param password: Password to be used if the PostgreSQL server demands password authentication. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#password PostgresqlProvider#password}
+        :param port: The PostgreSQL port number to connect to at the server host, or socket file name extension for Unix-domain connections. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#port PostgresqlProvider#port}
+        :param scheme: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#scheme PostgresqlProvider#scheme}.
+        :param sslmode: This option determines whether or with what priority a secure SSL TCP/IP connection will be negotiated with the PostgreSQL server. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#sslmode PostgresqlProvider#sslmode}
+        :param ssl_mode: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#ssl_mode PostgresqlProvider#ssl_mode}.
+        :param sslrootcert: The SSL server root certificate file path. The file must contain PEM encoded data. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#sslrootcert PostgresqlProvider#sslrootcert}
+        :param superuser: Specify if the user to connect as is a Postgres superuser or not.If not, some feature might be disabled (e.g.: Refreshing state password from Postgres). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#superuser PostgresqlProvider#superuser}
+        :param username: PostgreSQL user name to connect as. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#username PostgresqlProvider#username}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__873dda44896731f3ed4ac28494dd70199e52e0d56618c8331c8cac2815eb1e7b)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         config = PostgresqlProviderConfig(
             alias=alias,
@@ -535,41 +535,41 @@
     jsii_type="@cdktf/provider-postgresql.provider.PostgresqlProviderClientcert",
     jsii_struct_bases=[],
     name_mapping={"cert": "cert", "key": "key"},
 )
 class PostgresqlProviderClientcert:
     def __init__(self, *, cert: builtins.str, key: builtins.str) -> None:
         '''
-        :param cert: The SSL client certificate file path. The file must contain PEM encoded data. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#cert PostgresqlProvider#cert}
-        :param key: The SSL client certificate private key file path. The file must contain PEM encoded data. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#key PostgresqlProvider#key}
+        :param cert: The SSL client certificate file path. The file must contain PEM encoded data. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#cert PostgresqlProvider#cert}
+        :param key: The SSL client certificate private key file path. The file must contain PEM encoded data. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#key PostgresqlProvider#key}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__17fff281aae5956890689f9551e028540c4b095ea7e40dfc387ca3f724da72f6)
             check_type(argname="argument cert", value=cert, expected_type=type_hints["cert"])
             check_type(argname="argument key", value=key, expected_type=type_hints["key"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "cert": cert,
             "key": key,
         }
 
     @builtins.property
     def cert(self) -> builtins.str:
         '''The SSL client certificate file path. The file must contain PEM encoded data.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#cert PostgresqlProvider#cert}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#cert PostgresqlProvider#cert}
         '''
         result = self._values.get("cert")
         assert result is not None, "Required property 'cert' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def key(self) -> builtins.str:
         '''The SSL client certificate private key file path. The file must contain PEM encoded data.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#key PostgresqlProvider#key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#key PostgresqlProvider#key}
         '''
         result = self._values.get("key")
         assert result is not None, "Required property 'key' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
@@ -629,33 +629,33 @@
         sslmode: typing.Optional[builtins.str] = None,
         ssl_mode: typing.Optional[builtins.str] = None,
         sslrootcert: typing.Optional[builtins.str] = None,
         superuser: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         username: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#alias PostgresqlProvider#alias}
-        :param aws_rds_iam_auth: Use rds_iam instead of password authentication (see: https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/UsingWithRDS.IAMDBAuth.html). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#aws_rds_iam_auth PostgresqlProvider#aws_rds_iam_auth}
-        :param aws_rds_iam_profile: AWS profile to use for IAM auth. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#aws_rds_iam_profile PostgresqlProvider#aws_rds_iam_profile}
-        :param aws_rds_iam_region: AWS region to use for IAM auth. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#aws_rds_iam_region PostgresqlProvider#aws_rds_iam_region}
-        :param clientcert: clientcert block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#clientcert PostgresqlProvider#clientcert}
-        :param connect_timeout: Maximum wait for connection, in seconds. Zero or not specified means wait indefinitely. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#connect_timeout PostgresqlProvider#connect_timeout}
-        :param database: The name of the database to connect to in order to conenct to (defaults to ``postgres``). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#database PostgresqlProvider#database}
-        :param database_username: Database username associated to the connected user (for user name maps). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#database_username PostgresqlProvider#database_username}
-        :param expected_version: Specify the expected version of PostgreSQL. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#expected_version PostgresqlProvider#expected_version}
-        :param host: Name of PostgreSQL server address to connect to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#host PostgresqlProvider#host}
-        :param max_connections: Maximum number of connections to establish to the database. Zero means unlimited. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#max_connections PostgresqlProvider#max_connections}
-        :param password: Password to be used if the PostgreSQL server demands password authentication. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#password PostgresqlProvider#password}
-        :param port: The PostgreSQL port number to connect to at the server host, or socket file name extension for Unix-domain connections. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#port PostgresqlProvider#port}
-        :param scheme: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#scheme PostgresqlProvider#scheme}.
-        :param sslmode: This option determines whether or with what priority a secure SSL TCP/IP connection will be negotiated with the PostgreSQL server. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#sslmode PostgresqlProvider#sslmode}
-        :param ssl_mode: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#ssl_mode PostgresqlProvider#ssl_mode}.
-        :param sslrootcert: The SSL server root certificate file path. The file must contain PEM encoded data. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#sslrootcert PostgresqlProvider#sslrootcert}
-        :param superuser: Specify if the user to connect as is a Postgres superuser or not.If not, some feature might be disabled (e.g.: Refreshing state password from Postgres). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#superuser PostgresqlProvider#superuser}
-        :param username: PostgreSQL user name to connect as. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#username PostgresqlProvider#username}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#alias PostgresqlProvider#alias}
+        :param aws_rds_iam_auth: Use rds_iam instead of password authentication (see: https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/UsingWithRDS.IAMDBAuth.html). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#aws_rds_iam_auth PostgresqlProvider#aws_rds_iam_auth}
+        :param aws_rds_iam_profile: AWS profile to use for IAM auth. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#aws_rds_iam_profile PostgresqlProvider#aws_rds_iam_profile}
+        :param aws_rds_iam_region: AWS region to use for IAM auth. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#aws_rds_iam_region PostgresqlProvider#aws_rds_iam_region}
+        :param clientcert: clientcert block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#clientcert PostgresqlProvider#clientcert}
+        :param connect_timeout: Maximum wait for connection, in seconds. Zero or not specified means wait indefinitely. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#connect_timeout PostgresqlProvider#connect_timeout}
+        :param database: The name of the database to connect to in order to conenct to (defaults to ``postgres``). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#database PostgresqlProvider#database}
+        :param database_username: Database username associated to the connected user (for user name maps). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#database_username PostgresqlProvider#database_username}
+        :param expected_version: Specify the expected version of PostgreSQL. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#expected_version PostgresqlProvider#expected_version}
+        :param host: Name of PostgreSQL server address to connect to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#host PostgresqlProvider#host}
+        :param max_connections: Maximum number of connections to establish to the database. Zero means unlimited. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#max_connections PostgresqlProvider#max_connections}
+        :param password: Password to be used if the PostgreSQL server demands password authentication. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#password PostgresqlProvider#password}
+        :param port: The PostgreSQL port number to connect to at the server host, or socket file name extension for Unix-domain connections. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#port PostgresqlProvider#port}
+        :param scheme: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#scheme PostgresqlProvider#scheme}.
+        :param sslmode: This option determines whether or with what priority a secure SSL TCP/IP connection will be negotiated with the PostgreSQL server. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#sslmode PostgresqlProvider#sslmode}
+        :param ssl_mode: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#ssl_mode PostgresqlProvider#ssl_mode}.
+        :param sslrootcert: The SSL server root certificate file path. The file must contain PEM encoded data. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#sslrootcert PostgresqlProvider#sslrootcert}
+        :param superuser: Specify if the user to connect as is a Postgres superuser or not.If not, some feature might be disabled (e.g.: Refreshing state password from Postgres). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#superuser PostgresqlProvider#superuser}
+        :param username: PostgreSQL user name to connect as. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#username PostgresqlProvider#username}
         '''
         if isinstance(clientcert, dict):
             clientcert = PostgresqlProviderClientcert(**clientcert)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__af0cedc5a2e044ea705446ddbefd2a58e4b5080becd8b24f22f9c36fa4d87d5f)
             check_type(argname="argument alias", value=alias, expected_type=type_hints["alias"])
             check_type(argname="argument aws_rds_iam_auth", value=aws_rds_iam_auth, expected_type=type_hints["aws_rds_iam_auth"])
@@ -716,175 +716,175 @@
         if username is not None:
             self._values["username"] = username
 
     @builtins.property
     def alias(self) -> typing.Optional[builtins.str]:
         '''Alias name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#alias PostgresqlProvider#alias}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#alias PostgresqlProvider#alias}
         '''
         result = self._values.get("alias")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def aws_rds_iam_auth(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Use rds_iam instead of password authentication (see: https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/UsingWithRDS.IAMDBAuth.html).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#aws_rds_iam_auth PostgresqlProvider#aws_rds_iam_auth}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#aws_rds_iam_auth PostgresqlProvider#aws_rds_iam_auth}
         '''
         result = self._values.get("aws_rds_iam_auth")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def aws_rds_iam_profile(self) -> typing.Optional[builtins.str]:
         '''AWS profile to use for IAM auth.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#aws_rds_iam_profile PostgresqlProvider#aws_rds_iam_profile}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#aws_rds_iam_profile PostgresqlProvider#aws_rds_iam_profile}
         '''
         result = self._values.get("aws_rds_iam_profile")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def aws_rds_iam_region(self) -> typing.Optional[builtins.str]:
         '''AWS region to use for IAM auth.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#aws_rds_iam_region PostgresqlProvider#aws_rds_iam_region}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#aws_rds_iam_region PostgresqlProvider#aws_rds_iam_region}
         '''
         result = self._values.get("aws_rds_iam_region")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def clientcert(self) -> typing.Optional[PostgresqlProviderClientcert]:
         '''clientcert block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#clientcert PostgresqlProvider#clientcert}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#clientcert PostgresqlProvider#clientcert}
         '''
         result = self._values.get("clientcert")
         return typing.cast(typing.Optional[PostgresqlProviderClientcert], result)
 
     @builtins.property
     def connect_timeout(self) -> typing.Optional[jsii.Number]:
         '''Maximum wait for connection, in seconds. Zero or not specified means wait indefinitely.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#connect_timeout PostgresqlProvider#connect_timeout}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#connect_timeout PostgresqlProvider#connect_timeout}
         '''
         result = self._values.get("connect_timeout")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def database(self) -> typing.Optional[builtins.str]:
         '''The name of the database to connect to in order to conenct to (defaults to ``postgres``).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#database PostgresqlProvider#database}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#database PostgresqlProvider#database}
         '''
         result = self._values.get("database")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def database_username(self) -> typing.Optional[builtins.str]:
         '''Database username associated to the connected user (for user name maps).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#database_username PostgresqlProvider#database_username}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#database_username PostgresqlProvider#database_username}
         '''
         result = self._values.get("database_username")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def expected_version(self) -> typing.Optional[builtins.str]:
         '''Specify the expected version of PostgreSQL.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#expected_version PostgresqlProvider#expected_version}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#expected_version PostgresqlProvider#expected_version}
         '''
         result = self._values.get("expected_version")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def host(self) -> typing.Optional[builtins.str]:
         '''Name of PostgreSQL server address to connect to.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#host PostgresqlProvider#host}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#host PostgresqlProvider#host}
         '''
         result = self._values.get("host")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def max_connections(self) -> typing.Optional[jsii.Number]:
         '''Maximum number of connections to establish to the database. Zero means unlimited.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#max_connections PostgresqlProvider#max_connections}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#max_connections PostgresqlProvider#max_connections}
         '''
         result = self._values.get("max_connections")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def password(self) -> typing.Optional[builtins.str]:
         '''Password to be used if the PostgreSQL server demands password authentication.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#password PostgresqlProvider#password}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#password PostgresqlProvider#password}
         '''
         result = self._values.get("password")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def port(self) -> typing.Optional[jsii.Number]:
         '''The PostgreSQL port number to connect to at the server host, or socket file name extension for Unix-domain connections.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#port PostgresqlProvider#port}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#port PostgresqlProvider#port}
         '''
         result = self._values.get("port")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def scheme(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#scheme PostgresqlProvider#scheme}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#scheme PostgresqlProvider#scheme}.'''
         result = self._values.get("scheme")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def sslmode(self) -> typing.Optional[builtins.str]:
         '''This option determines whether or with what priority a secure SSL TCP/IP connection will be negotiated with the PostgreSQL server.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#sslmode PostgresqlProvider#sslmode}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#sslmode PostgresqlProvider#sslmode}
         '''
         result = self._values.get("sslmode")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def ssl_mode(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#ssl_mode PostgresqlProvider#ssl_mode}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#ssl_mode PostgresqlProvider#ssl_mode}.'''
         result = self._values.get("ssl_mode")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def sslrootcert(self) -> typing.Optional[builtins.str]:
         '''The SSL server root certificate file path. The file must contain PEM encoded data.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#sslrootcert PostgresqlProvider#sslrootcert}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#sslrootcert PostgresqlProvider#sslrootcert}
         '''
         result = self._values.get("sslrootcert")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def superuser(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Specify if the user to connect as is a Postgres superuser or not.If not, some feature might be disabled (e.g.: Refreshing state password from Postgres).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#superuser PostgresqlProvider#superuser}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#superuser PostgresqlProvider#superuser}
         '''
         result = self._values.get("superuser")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def username(self) -> typing.Optional[builtins.str]:
         '''PostgreSQL user name to connect as.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs#username PostgresqlProvider#username}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs#username PostgresqlProvider#username}
         '''
         result = self._values.get("username")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/publication/__init__.py` & `cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/publication/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `postgresql_publication`
 
-Refer to the Terraform Registory for docs: [`postgresql_publication`](https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/publication).
+Refer to the Terraform Registory for docs: [`postgresql_publication`](https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/publication).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class Publication(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-postgresql.publication.Publication",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/publication postgresql_publication}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/publication postgresql_publication}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         name: builtins.str,
@@ -46,27 +46,27 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/publication postgresql_publication} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/publication postgresql_publication} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/publication#name Publication#name}.
-        :param all_tables: Sets the tables list to publish to ALL tables. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/publication#all_tables Publication#all_tables}
-        :param database: Sets the database to add the publication for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/publication#database Publication#database}
-        :param drop_cascade: When true, will also drop all the objects that depend on the publication, and in turn all objects that depend on those objects. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/publication#drop_cascade Publication#drop_cascade}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/publication#id Publication#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param owner: Sets the owner of the publication. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/publication#owner Publication#owner}
-        :param publish_param: Sets which DML operations will be published. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/publication#publish_param Publication#publish_param}
-        :param publish_via_partition_root_param: Sets whether changes in a partitioned table using the identity and schema of the partitioned table. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/publication#publish_via_partition_root_param Publication#publish_via_partition_root_param}
-        :param tables: Sets the tables list to publish. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/publication#tables Publication#tables}
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/publication#name Publication#name}.
+        :param all_tables: Sets the tables list to publish to ALL tables. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/publication#all_tables Publication#all_tables}
+        :param database: Sets the database to add the publication for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/publication#database Publication#database}
+        :param drop_cascade: When true, will also drop all the objects that depend on the publication, and in turn all objects that depend on those objects. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/publication#drop_cascade Publication#drop_cascade}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/publication#id Publication#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param owner: Sets the owner of the publication. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/publication#owner Publication#owner}
+        :param publish_param: Sets which DML operations will be published. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/publication#publish_param Publication#publish_param}
+        :param publish_via_partition_root_param: Sets whether changes in a partitioned table using the identity and schema of the partitioned table. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/publication#publish_via_partition_root_param Publication#publish_via_partition_root_param}
+        :param tables: Sets the tables list to publish. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/publication#tables Publication#tables}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -355,23 +355,23 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/publication#name Publication#name}.
-        :param all_tables: Sets the tables list to publish to ALL tables. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/publication#all_tables Publication#all_tables}
-        :param database: Sets the database to add the publication for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/publication#database Publication#database}
-        :param drop_cascade: When true, will also drop all the objects that depend on the publication, and in turn all objects that depend on those objects. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/publication#drop_cascade Publication#drop_cascade}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/publication#id Publication#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param owner: Sets the owner of the publication. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/publication#owner Publication#owner}
-        :param publish_param: Sets which DML operations will be published. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/publication#publish_param Publication#publish_param}
-        :param publish_via_partition_root_param: Sets whether changes in a partitioned table using the identity and schema of the partitioned table. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/publication#publish_via_partition_root_param Publication#publish_via_partition_root_param}
-        :param tables: Sets the tables list to publish. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/publication#tables Publication#tables}
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/publication#name Publication#name}.
+        :param all_tables: Sets the tables list to publish to ALL tables. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/publication#all_tables Publication#all_tables}
+        :param database: Sets the database to add the publication for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/publication#database Publication#database}
+        :param drop_cascade: When true, will also drop all the objects that depend on the publication, and in turn all objects that depend on those objects. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/publication#drop_cascade Publication#drop_cascade}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/publication#id Publication#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param owner: Sets the owner of the publication. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/publication#owner Publication#owner}
+        :param publish_param: Sets which DML operations will be published. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/publication#publish_param Publication#publish_param}
+        :param publish_via_partition_root_param: Sets whether changes in a partitioned table using the identity and schema of the partitioned table. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/publication#publish_via_partition_root_param Publication#publish_via_partition_root_param}
+        :param tables: Sets the tables list to publish. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/publication#tables Publication#tables}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__87a1e84803dc8da83afaffe6253d8360fb5fec5c0ce6d14637dadd56ad17e238)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -485,94 +485,94 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/publication#name Publication#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/publication#name Publication#name}.'''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def all_tables(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Sets the tables list to publish to ALL tables.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/publication#all_tables Publication#all_tables}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/publication#all_tables Publication#all_tables}
         '''
         result = self._values.get("all_tables")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def database(self) -> typing.Optional[builtins.str]:
         '''Sets the database to add the publication for.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/publication#database Publication#database}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/publication#database Publication#database}
         '''
         result = self._values.get("database")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def drop_cascade(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''When true, will also drop all the objects that depend on the publication, and in turn all objects that depend on those objects.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/publication#drop_cascade Publication#drop_cascade}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/publication#drop_cascade Publication#drop_cascade}
         '''
         result = self._values.get("drop_cascade")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/publication#id Publication#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/publication#id Publication#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def owner(self) -> typing.Optional[builtins.str]:
         '''Sets the owner of the publication.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/publication#owner Publication#owner}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/publication#owner Publication#owner}
         '''
         result = self._values.get("owner")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def publish_param(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Sets which DML operations will be published.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/publication#publish_param Publication#publish_param}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/publication#publish_param Publication#publish_param}
         '''
         result = self._values.get("publish_param")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def publish_via_partition_root_param(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Sets whether changes in a partitioned table using the identity and schema of the partitioned table.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/publication#publish_via_partition_root_param Publication#publish_via_partition_root_param}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/publication#publish_via_partition_root_param Publication#publish_via_partition_root_param}
         '''
         result = self._values.get("publish_via_partition_root_param")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def tables(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Sets the tables list to publish.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/publication#tables Publication#tables}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/publication#tables Publication#tables}
         '''
         result = self._values.get("tables")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/replication_slot/__init__.py` & `cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/replication_slot/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `postgresql_replication_slot`
 
-Refer to the Terraform Registory for docs: [`postgresql_replication_slot`](https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/replication_slot).
+Refer to the Terraform Registory for docs: [`postgresql_replication_slot`](https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/replication_slot).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class ReplicationSlot(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-postgresql.replicationSlot.ReplicationSlot",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/replication_slot postgresql_replication_slot}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/replication_slot postgresql_replication_slot}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         name: builtins.str,
@@ -41,22 +41,22 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/replication_slot postgresql_replication_slot} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/replication_slot postgresql_replication_slot} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/replication_slot#name ReplicationSlot#name}.
-        :param plugin: Sets the output plugin to use. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/replication_slot#plugin ReplicationSlot#plugin}
-        :param database: Sets the database to add the replication slot to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/replication_slot#database ReplicationSlot#database}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/replication_slot#id ReplicationSlot#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/replication_slot#name ReplicationSlot#name}.
+        :param plugin: Sets the output plugin to use. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/replication_slot#plugin ReplicationSlot#plugin}
+        :param database: Sets the database to add the replication slot to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/replication_slot#database ReplicationSlot#database}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/replication_slot#id ReplicationSlot#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -204,18 +204,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/replication_slot#name ReplicationSlot#name}.
-        :param plugin: Sets the output plugin to use. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/replication_slot#plugin ReplicationSlot#plugin}
-        :param database: Sets the database to add the replication slot to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/replication_slot#database ReplicationSlot#database}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/replication_slot#id ReplicationSlot#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/replication_slot#name ReplicationSlot#name}.
+        :param plugin: Sets the output plugin to use. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/replication_slot#plugin ReplicationSlot#plugin}
+        :param database: Sets the database to add the replication slot to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/replication_slot#database ReplicationSlot#database}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/replication_slot#id ReplicationSlot#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__219559d54d95b8ff259b3306f9b225909225eeaf565ac5b5dfb01f749119c9d1)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -313,41 +313,41 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/replication_slot#name ReplicationSlot#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/replication_slot#name ReplicationSlot#name}.'''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def plugin(self) -> builtins.str:
         '''Sets the output plugin to use.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/replication_slot#plugin ReplicationSlot#plugin}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/replication_slot#plugin ReplicationSlot#plugin}
         '''
         result = self._values.get("plugin")
         assert result is not None, "Required property 'plugin' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def database(self) -> typing.Optional[builtins.str]:
         '''Sets the database to add the replication slot to.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/replication_slot#database ReplicationSlot#database}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/replication_slot#database ReplicationSlot#database}
         '''
         result = self._values.get("database")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/replication_slot#id ReplicationSlot#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/replication_slot#id ReplicationSlot#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
```

### Comparing `cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/role/__init__.py` & `cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/role/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `postgresql_role`
 
-Refer to the Terraform Registory for docs: [`postgresql_role`](https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role).
+Refer to the Terraform Registory for docs: [`postgresql_role`](https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class Role(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-postgresql.role.Role",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role postgresql_role}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role postgresql_role}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         name: builtins.str,
@@ -58,39 +58,39 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role postgresql_role} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role postgresql_role} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: The name of the role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#name Role#name}
-        :param assume_role: Role to switch to at login. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#assume_role Role#assume_role}
-        :param bypass_row_level_security: Determine whether a role bypasses every row-level security (RLS) policy. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#bypass_row_level_security Role#bypass_row_level_security}
-        :param connection_limit: How many concurrent connections can be made with this role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#connection_limit Role#connection_limit}
-        :param create_database: Define a role's ability to create databases. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#create_database Role#create_database}
-        :param create_role: Determine whether this role will be permitted to create new roles. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#create_role Role#create_role}
-        :param encrypted: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#encrypted Role#encrypted}.
-        :param encrypted_password: Control whether the password is stored encrypted in the system catalogs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#encrypted_password Role#encrypted_password}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#id Role#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param idle_in_transaction_session_timeout: Terminate any session with an open transaction that has been idle for longer than the specified duration in milliseconds. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#idle_in_transaction_session_timeout Role#idle_in_transaction_session_timeout}
-        :param inherit: Determine whether a role "inherits" the privileges of roles it is a member of. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#inherit Role#inherit}
-        :param login: Determine whether a role is allowed to log in. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#login Role#login}
-        :param password: Sets the role's password. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#password Role#password}
-        :param replication: Determine whether a role is allowed to initiate streaming replication or put the system in and out of backup mode. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#replication Role#replication}
-        :param roles: Role(s) to grant to this new role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#roles Role#roles}
-        :param search_path: Sets the role's search path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#search_path Role#search_path}
-        :param skip_drop_role: Skip actually running the DROP ROLE command when removing a ROLE from PostgreSQL. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#skip_drop_role Role#skip_drop_role}
-        :param skip_reassign_owned: Skip actually running the REASSIGN OWNED command when removing a role from PostgreSQL. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#skip_reassign_owned Role#skip_reassign_owned}
-        :param statement_timeout: Abort any statement that takes more than the specified number of milliseconds. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#statement_timeout Role#statement_timeout}
-        :param superuser: Determine whether the new role is a "superuser". Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#superuser Role#superuser}
-        :param valid_until: Sets a date and time after which the role's password is no longer valid. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#valid_until Role#valid_until}
+        :param name: The name of the role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#name Role#name}
+        :param assume_role: Role to switch to at login. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#assume_role Role#assume_role}
+        :param bypass_row_level_security: Determine whether a role bypasses every row-level security (RLS) policy. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#bypass_row_level_security Role#bypass_row_level_security}
+        :param connection_limit: How many concurrent connections can be made with this role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#connection_limit Role#connection_limit}
+        :param create_database: Define a role's ability to create databases. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#create_database Role#create_database}
+        :param create_role: Determine whether this role will be permitted to create new roles. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#create_role Role#create_role}
+        :param encrypted: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#encrypted Role#encrypted}.
+        :param encrypted_password: Control whether the password is stored encrypted in the system catalogs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#encrypted_password Role#encrypted_password}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#id Role#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param idle_in_transaction_session_timeout: Terminate any session with an open transaction that has been idle for longer than the specified duration in milliseconds. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#idle_in_transaction_session_timeout Role#idle_in_transaction_session_timeout}
+        :param inherit: Determine whether a role "inherits" the privileges of roles it is a member of. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#inherit Role#inherit}
+        :param login: Determine whether a role is allowed to log in. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#login Role#login}
+        :param password: Sets the role's password. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#password Role#password}
+        :param replication: Determine whether a role is allowed to initiate streaming replication or put the system in and out of backup mode. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#replication Role#replication}
+        :param roles: Role(s) to grant to this new role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#roles Role#roles}
+        :param search_path: Sets the role's search path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#search_path Role#search_path}
+        :param skip_drop_role: Skip actually running the DROP ROLE command when removing a ROLE from PostgreSQL. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#skip_drop_role Role#skip_drop_role}
+        :param skip_reassign_owned: Skip actually running the REASSIGN OWNED command when removing a role from PostgreSQL. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#skip_reassign_owned Role#skip_reassign_owned}
+        :param statement_timeout: Abort any statement that takes more than the specified number of milliseconds. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#statement_timeout Role#statement_timeout}
+        :param superuser: Determine whether the new role is a "superuser". Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#superuser Role#superuser}
+        :param valid_until: Sets a date and time after which the role's password is no longer valid. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#valid_until Role#valid_until}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -710,35 +710,35 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: The name of the role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#name Role#name}
-        :param assume_role: Role to switch to at login. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#assume_role Role#assume_role}
-        :param bypass_row_level_security: Determine whether a role bypasses every row-level security (RLS) policy. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#bypass_row_level_security Role#bypass_row_level_security}
-        :param connection_limit: How many concurrent connections can be made with this role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#connection_limit Role#connection_limit}
-        :param create_database: Define a role's ability to create databases. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#create_database Role#create_database}
-        :param create_role: Determine whether this role will be permitted to create new roles. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#create_role Role#create_role}
-        :param encrypted: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#encrypted Role#encrypted}.
-        :param encrypted_password: Control whether the password is stored encrypted in the system catalogs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#encrypted_password Role#encrypted_password}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#id Role#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param idle_in_transaction_session_timeout: Terminate any session with an open transaction that has been idle for longer than the specified duration in milliseconds. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#idle_in_transaction_session_timeout Role#idle_in_transaction_session_timeout}
-        :param inherit: Determine whether a role "inherits" the privileges of roles it is a member of. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#inherit Role#inherit}
-        :param login: Determine whether a role is allowed to log in. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#login Role#login}
-        :param password: Sets the role's password. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#password Role#password}
-        :param replication: Determine whether a role is allowed to initiate streaming replication or put the system in and out of backup mode. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#replication Role#replication}
-        :param roles: Role(s) to grant to this new role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#roles Role#roles}
-        :param search_path: Sets the role's search path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#search_path Role#search_path}
-        :param skip_drop_role: Skip actually running the DROP ROLE command when removing a ROLE from PostgreSQL. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#skip_drop_role Role#skip_drop_role}
-        :param skip_reassign_owned: Skip actually running the REASSIGN OWNED command when removing a role from PostgreSQL. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#skip_reassign_owned Role#skip_reassign_owned}
-        :param statement_timeout: Abort any statement that takes more than the specified number of milliseconds. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#statement_timeout Role#statement_timeout}
-        :param superuser: Determine whether the new role is a "superuser". Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#superuser Role#superuser}
-        :param valid_until: Sets a date and time after which the role's password is no longer valid. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#valid_until Role#valid_until}
+        :param name: The name of the role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#name Role#name}
+        :param assume_role: Role to switch to at login. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#assume_role Role#assume_role}
+        :param bypass_row_level_security: Determine whether a role bypasses every row-level security (RLS) policy. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#bypass_row_level_security Role#bypass_row_level_security}
+        :param connection_limit: How many concurrent connections can be made with this role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#connection_limit Role#connection_limit}
+        :param create_database: Define a role's ability to create databases. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#create_database Role#create_database}
+        :param create_role: Determine whether this role will be permitted to create new roles. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#create_role Role#create_role}
+        :param encrypted: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#encrypted Role#encrypted}.
+        :param encrypted_password: Control whether the password is stored encrypted in the system catalogs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#encrypted_password Role#encrypted_password}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#id Role#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param idle_in_transaction_session_timeout: Terminate any session with an open transaction that has been idle for longer than the specified duration in milliseconds. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#idle_in_transaction_session_timeout Role#idle_in_transaction_session_timeout}
+        :param inherit: Determine whether a role "inherits" the privileges of roles it is a member of. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#inherit Role#inherit}
+        :param login: Determine whether a role is allowed to log in. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#login Role#login}
+        :param password: Sets the role's password. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#password Role#password}
+        :param replication: Determine whether a role is allowed to initiate streaming replication or put the system in and out of backup mode. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#replication Role#replication}
+        :param roles: Role(s) to grant to this new role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#roles Role#roles}
+        :param search_path: Sets the role's search path. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#search_path Role#search_path}
+        :param skip_drop_role: Skip actually running the DROP ROLE command when removing a ROLE from PostgreSQL. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#skip_drop_role Role#skip_drop_role}
+        :param skip_reassign_owned: Skip actually running the REASSIGN OWNED command when removing a role from PostgreSQL. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#skip_reassign_owned Role#skip_reassign_owned}
+        :param statement_timeout: Abort any statement that takes more than the specified number of milliseconds. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#statement_timeout Role#statement_timeout}
+        :param superuser: Determine whether the new role is a "superuser". Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#superuser Role#superuser}
+        :param valid_until: Sets a date and time after which the role's password is no longer valid. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#valid_until Role#valid_until}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__acfac6cd9793e31e288a66bfff5e43e65f4432f03ded8a4e3c21227a7a60570f)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -890,214 +890,214 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''The name of the role.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#name Role#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#name Role#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def assume_role(self) -> typing.Optional[builtins.str]:
         '''Role to switch to at login.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#assume_role Role#assume_role}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#assume_role Role#assume_role}
         '''
         result = self._values.get("assume_role")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def bypass_row_level_security(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Determine whether a role bypasses every row-level security (RLS) policy.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#bypass_row_level_security Role#bypass_row_level_security}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#bypass_row_level_security Role#bypass_row_level_security}
         '''
         result = self._values.get("bypass_row_level_security")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def connection_limit(self) -> typing.Optional[jsii.Number]:
         '''How many concurrent connections can be made with this role.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#connection_limit Role#connection_limit}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#connection_limit Role#connection_limit}
         '''
         result = self._values.get("connection_limit")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def create_database(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Define a role's ability to create databases.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#create_database Role#create_database}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#create_database Role#create_database}
         '''
         result = self._values.get("create_database")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def create_role(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Determine whether this role will be permitted to create new roles.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#create_role Role#create_role}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#create_role Role#create_role}
         '''
         result = self._values.get("create_role")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def encrypted(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#encrypted Role#encrypted}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#encrypted Role#encrypted}.'''
         result = self._values.get("encrypted")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def encrypted_password(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Control whether the password is stored encrypted in the system catalogs.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#encrypted_password Role#encrypted_password}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#encrypted_password Role#encrypted_password}
         '''
         result = self._values.get("encrypted_password")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#id Role#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#id Role#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def idle_in_transaction_session_timeout(self) -> typing.Optional[jsii.Number]:
         '''Terminate any session with an open transaction that has been idle for longer than the specified duration in milliseconds.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#idle_in_transaction_session_timeout Role#idle_in_transaction_session_timeout}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#idle_in_transaction_session_timeout Role#idle_in_transaction_session_timeout}
         '''
         result = self._values.get("idle_in_transaction_session_timeout")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def inherit(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Determine whether a role "inherits" the privileges of roles it is a member of.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#inherit Role#inherit}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#inherit Role#inherit}
         '''
         result = self._values.get("inherit")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def login(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Determine whether a role is allowed to log in.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#login Role#login}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#login Role#login}
         '''
         result = self._values.get("login")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def password(self) -> typing.Optional[builtins.str]:
         '''Sets the role's password.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#password Role#password}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#password Role#password}
         '''
         result = self._values.get("password")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def replication(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Determine whether a role is allowed to initiate streaming replication or put the system in and out of backup mode.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#replication Role#replication}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#replication Role#replication}
         '''
         result = self._values.get("replication")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def roles(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Role(s) to grant to this new role.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#roles Role#roles}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#roles Role#roles}
         '''
         result = self._values.get("roles")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def search_path(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Sets the role's search path.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#search_path Role#search_path}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#search_path Role#search_path}
         '''
         result = self._values.get("search_path")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def skip_drop_role(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Skip actually running the DROP ROLE command when removing a ROLE from PostgreSQL.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#skip_drop_role Role#skip_drop_role}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#skip_drop_role Role#skip_drop_role}
         '''
         result = self._values.get("skip_drop_role")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def skip_reassign_owned(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Skip actually running the REASSIGN OWNED command when removing a role from PostgreSQL.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#skip_reassign_owned Role#skip_reassign_owned}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#skip_reassign_owned Role#skip_reassign_owned}
         '''
         result = self._values.get("skip_reassign_owned")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def statement_timeout(self) -> typing.Optional[jsii.Number]:
         '''Abort any statement that takes more than the specified number of milliseconds.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#statement_timeout Role#statement_timeout}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#statement_timeout Role#statement_timeout}
         '''
         result = self._values.get("statement_timeout")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def superuser(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Determine whether the new role is a "superuser".
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#superuser Role#superuser}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#superuser Role#superuser}
         '''
         result = self._values.get("superuser")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def valid_until(self) -> typing.Optional[builtins.str]:
         '''Sets a date and time after which the role's password is no longer valid.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/role#valid_until Role#valid_until}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/role#valid_until Role#valid_until}
         '''
         result = self._values.get("valid_until")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/schema/__init__.py` & `cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/schema/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `postgresql_schema`
 
-Refer to the Terraform Registory for docs: [`postgresql_schema`](https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/schema).
+Refer to the Terraform Registory for docs: [`postgresql_schema`](https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/schema).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class Schema(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-postgresql.schema.Schema",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/schema postgresql_schema}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/schema postgresql_schema}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         name: builtins.str,
@@ -44,25 +44,25 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/schema postgresql_schema} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/schema postgresql_schema} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: The name of the schema. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/schema#name Schema#name}
-        :param database: The database name to alter schema. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/schema#database Schema#database}
-        :param drop_cascade: When true, will also drop all the objects that are contained in the schema. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/schema#drop_cascade Schema#drop_cascade}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/schema#id Schema#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param if_not_exists: When true, use the existing schema if it exists. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/schema#if_not_exists Schema#if_not_exists}
-        :param owner: The ROLE name who owns the schema. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/schema#owner Schema#owner}
-        :param policy: policy block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/schema#policy Schema#policy}
+        :param name: The name of the schema. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/schema#name Schema#name}
+        :param database: The database name to alter schema. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/schema#database Schema#database}
+        :param drop_cascade: When true, will also drop all the objects that are contained in the schema. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/schema#drop_cascade Schema#drop_cascade}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/schema#id Schema#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param if_not_exists: When true, use the existing schema if it exists. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/schema#if_not_exists Schema#if_not_exists}
+        :param owner: The ROLE name who owns the schema. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/schema#owner Schema#owner}
+        :param policy: policy block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/schema#policy Schema#policy}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -304,21 +304,21 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: The name of the schema. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/schema#name Schema#name}
-        :param database: The database name to alter schema. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/schema#database Schema#database}
-        :param drop_cascade: When true, will also drop all the objects that are contained in the schema. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/schema#drop_cascade Schema#drop_cascade}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/schema#id Schema#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param if_not_exists: When true, use the existing schema if it exists. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/schema#if_not_exists Schema#if_not_exists}
-        :param owner: The ROLE name who owns the schema. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/schema#owner Schema#owner}
-        :param policy: policy block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/schema#policy Schema#policy}
+        :param name: The name of the schema. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/schema#name Schema#name}
+        :param database: The database name to alter schema. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/schema#database Schema#database}
+        :param drop_cascade: When true, will also drop all the objects that are contained in the schema. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/schema#drop_cascade Schema#drop_cascade}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/schema#id Schema#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param if_not_exists: When true, use the existing schema if it exists. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/schema#if_not_exists Schema#if_not_exists}
+        :param owner: The ROLE name who owns the schema. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/schema#owner Schema#owner}
+        :param policy: policy block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/schema#policy Schema#policy}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__d6b68d53ccc4d4842eb03e82ac9d7082a6c889a1e612dddd7450fb889721976d)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -428,77 +428,77 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''The name of the schema.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/schema#name Schema#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/schema#name Schema#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def database(self) -> typing.Optional[builtins.str]:
         '''The database name to alter schema.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/schema#database Schema#database}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/schema#database Schema#database}
         '''
         result = self._values.get("database")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def drop_cascade(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''When true, will also drop all the objects that are contained in the schema.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/schema#drop_cascade Schema#drop_cascade}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/schema#drop_cascade Schema#drop_cascade}
         '''
         result = self._values.get("drop_cascade")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/schema#id Schema#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/schema#id Schema#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def if_not_exists(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''When true, use the existing schema if it exists.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/schema#if_not_exists Schema#if_not_exists}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/schema#if_not_exists Schema#if_not_exists}
         '''
         result = self._values.get("if_not_exists")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def owner(self) -> typing.Optional[builtins.str]:
         '''The ROLE name who owns the schema.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/schema#owner Schema#owner}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/schema#owner Schema#owner}
         '''
         result = self._values.get("owner")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def policy(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["SchemaPolicy"]]]:
         '''policy block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/schema#policy Schema#policy}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/schema#policy Schema#policy}
         '''
         result = self._values.get("policy")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["SchemaPolicy"]]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -529,19 +529,19 @@
         create: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         create_with_grant: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         role: typing.Optional[builtins.str] = None,
         usage: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         usage_with_grant: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     ) -> None:
         '''
-        :param create: If true, allow the specified ROLEs to CREATE new objects within the schema(s). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/schema#create Schema#create}
-        :param create_with_grant: If true, allow the specified ROLEs to CREATE new objects within the schema(s) and GRANT the same CREATE privilege to different ROLEs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/schema#create_with_grant Schema#create_with_grant}
-        :param role: ROLE who will receive this policy (default: PUBLIC). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/schema#role Schema#role}
-        :param usage: If true, allow the specified ROLEs to use objects within the schema(s). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/schema#usage Schema#usage}
-        :param usage_with_grant: If true, allow the specified ROLEs to use objects within the schema(s) and GRANT the same USAGE privilege to different ROLEs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/schema#usage_with_grant Schema#usage_with_grant}
+        :param create: If true, allow the specified ROLEs to CREATE new objects within the schema(s). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/schema#create Schema#create}
+        :param create_with_grant: If true, allow the specified ROLEs to CREATE new objects within the schema(s) and GRANT the same CREATE privilege to different ROLEs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/schema#create_with_grant Schema#create_with_grant}
+        :param role: ROLE who will receive this policy (default: PUBLIC). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/schema#role Schema#role}
+        :param usage: If true, allow the specified ROLEs to use objects within the schema(s). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/schema#usage Schema#usage}
+        :param usage_with_grant: If true, allow the specified ROLEs to use objects within the schema(s) and GRANT the same USAGE privilege to different ROLEs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/schema#usage_with_grant Schema#usage_with_grant}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__5d3fb1370d42b865d5bb4841a22091f7ebcb3320e54be8d63604b1e6faf6fdae)
             check_type(argname="argument create", value=create, expected_type=type_hints["create"])
             check_type(argname="argument create_with_grant", value=create_with_grant, expected_type=type_hints["create_with_grant"])
             check_type(argname="argument role", value=role, expected_type=type_hints["role"])
             check_type(argname="argument usage", value=usage, expected_type=type_hints["usage"])
@@ -560,57 +560,57 @@
 
     @builtins.property
     def create(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''If true, allow the specified ROLEs to CREATE new objects within the schema(s).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/schema#create Schema#create}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/schema#create Schema#create}
         '''
         result = self._values.get("create")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def create_with_grant(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''If true, allow the specified ROLEs to CREATE new objects within the schema(s) and GRANT the same CREATE privilege to different ROLEs.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/schema#create_with_grant Schema#create_with_grant}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/schema#create_with_grant Schema#create_with_grant}
         '''
         result = self._values.get("create_with_grant")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def role(self) -> typing.Optional[builtins.str]:
         '''ROLE who will receive this policy (default: PUBLIC).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/schema#role Schema#role}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/schema#role Schema#role}
         '''
         result = self._values.get("role")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def usage(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''If true, allow the specified ROLEs to use objects within the schema(s).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/schema#usage Schema#usage}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/schema#usage Schema#usage}
         '''
         result = self._values.get("usage")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def usage_with_grant(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''If true, allow the specified ROLEs to use objects within the schema(s) and GRANT the same USAGE privilege to different ROLEs.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/schema#usage_with_grant Schema#usage_with_grant}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/schema#usage_with_grant Schema#usage_with_grant}
         '''
         result = self._values.get("usage_with_grant")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -868,21 +868,21 @@
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "usageWithGrant", value)
 
     @builtins.property
     @jsii.member(jsii_name="internalValue")
     def internal_value(
         self,
-    ) -> typing.Optional[typing.Union[SchemaPolicy, _cdktf_9a9027ec.IResolvable]]:
-        return typing.cast(typing.Optional[typing.Union[SchemaPolicy, _cdktf_9a9027ec.IResolvable]], jsii.get(self, "internalValue"))
+    ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, SchemaPolicy]]:
+        return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, SchemaPolicy]], jsii.get(self, "internalValue"))
 
     @internal_value.setter
     def internal_value(
         self,
-        value: typing.Optional[typing.Union[SchemaPolicy, _cdktf_9a9027ec.IResolvable]],
+        value: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, SchemaPolicy]],
     ) -> None:
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__fdef3c4530a65047cce832da0dbc6ffbf0b6d8c703961b9c015db8eb64831c20)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internalValue", value)
 
 
@@ -1065,11 +1065,11 @@
 def _typecheckingstub__27c5e0025ae25ad6ae7b7ea5b512e0115f18ef6a477dcb0724c9f8c69a82a373(
     value: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__fdef3c4530a65047cce832da0dbc6ffbf0b6d8c703961b9c015db8eb64831c20(
-    value: typing.Optional[typing.Union[SchemaPolicy, _cdktf_9a9027ec.IResolvable]],
+    value: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, SchemaPolicy]],
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/server/__init__.py` & `cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/server/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `postgresql_server`
 
-Refer to the Terraform Registory for docs: [`postgresql_server`](https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/server).
+Refer to the Terraform Registory for docs: [`postgresql_server`](https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/server).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class Server(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-postgresql.server.Server",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/server postgresql_server}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/server postgresql_server}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         fdw_name: builtins.str,
@@ -45,26 +45,26 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/server postgresql_server} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/server postgresql_server} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param fdw_name: The name of the foreign-data wrapper that manages the server. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/server#fdw_name Server#fdw_name}
-        :param server_name: The name of the foreign server to be created. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/server#server_name Server#server_name}
-        :param drop_cascade: Automatically drop objects that depend on the server (such as user mappings), and in turn all objects that depend on those objects. Drop RESTRICT is the default Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/server#drop_cascade Server#drop_cascade}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/server#id Server#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param options: This clause specifies the options for the server. The options typically define the connection details of the server, but the actual names and values are dependent on the server's foreign-data wrapper Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/server#options Server#options}
-        :param server_owner: The user name of the new owner of the foreign server. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/server#server_owner Server#server_owner}
-        :param server_type: Optional server type, potentially useful to foreign-data wrappers. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/server#server_type Server#server_type}
-        :param server_version: Optional server version, potentially useful to foreign-data wrappers. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/server#server_version Server#server_version}
+        :param fdw_name: The name of the foreign-data wrapper that manages the server. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/server#fdw_name Server#fdw_name}
+        :param server_name: The name of the foreign server to be created. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/server#server_name Server#server_name}
+        :param drop_cascade: Automatically drop objects that depend on the server (such as user mappings), and in turn all objects that depend on those objects. Drop RESTRICT is the default Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/server#drop_cascade Server#drop_cascade}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/server#id Server#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param options: This clause specifies the options for the server. The options typically define the connection details of the server, but the actual names and values are dependent on the server's foreign-data wrapper Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/server#options Server#options}
+        :param server_owner: The user name of the new owner of the foreign server. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/server#server_owner Server#server_owner}
+        :param server_type: Optional server type, potentially useful to foreign-data wrappers. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/server#server_type Server#server_type}
+        :param server_version: Optional server version, potentially useful to foreign-data wrappers. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/server#server_version Server#server_version}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -315,22 +315,22 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param fdw_name: The name of the foreign-data wrapper that manages the server. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/server#fdw_name Server#fdw_name}
-        :param server_name: The name of the foreign server to be created. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/server#server_name Server#server_name}
-        :param drop_cascade: Automatically drop objects that depend on the server (such as user mappings), and in turn all objects that depend on those objects. Drop RESTRICT is the default Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/server#drop_cascade Server#drop_cascade}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/server#id Server#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param options: This clause specifies the options for the server. The options typically define the connection details of the server, but the actual names and values are dependent on the server's foreign-data wrapper Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/server#options Server#options}
-        :param server_owner: The user name of the new owner of the foreign server. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/server#server_owner Server#server_owner}
-        :param server_type: Optional server type, potentially useful to foreign-data wrappers. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/server#server_type Server#server_type}
-        :param server_version: Optional server version, potentially useful to foreign-data wrappers. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/server#server_version Server#server_version}
+        :param fdw_name: The name of the foreign-data wrapper that manages the server. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/server#fdw_name Server#fdw_name}
+        :param server_name: The name of the foreign server to be created. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/server#server_name Server#server_name}
+        :param drop_cascade: Automatically drop objects that depend on the server (such as user mappings), and in turn all objects that depend on those objects. Drop RESTRICT is the default Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/server#drop_cascade Server#drop_cascade}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/server#id Server#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param options: This clause specifies the options for the server. The options typically define the connection details of the server, but the actual names and values are dependent on the server's foreign-data wrapper Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/server#options Server#options}
+        :param server_owner: The user name of the new owner of the foreign server. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/server#server_owner Server#server_owner}
+        :param server_type: Optional server type, potentially useful to foreign-data wrappers. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/server#server_type Server#server_type}
+        :param server_version: Optional server version, potentially useful to foreign-data wrappers. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/server#server_version Server#server_version}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__fb4ad7ff9adc72666377b9ddff1e98a98302eb5f06f9ba59f7d0383675d71840)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -442,87 +442,87 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def fdw_name(self) -> builtins.str:
         '''The name of the foreign-data wrapper that manages the server.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/server#fdw_name Server#fdw_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/server#fdw_name Server#fdw_name}
         '''
         result = self._values.get("fdw_name")
         assert result is not None, "Required property 'fdw_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def server_name(self) -> builtins.str:
         '''The name of the foreign server to be created.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/server#server_name Server#server_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/server#server_name Server#server_name}
         '''
         result = self._values.get("server_name")
         assert result is not None, "Required property 'server_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def drop_cascade(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Automatically drop objects that depend on the server (such as user mappings), and in turn all objects that depend on those objects.
 
         Drop RESTRICT is the default
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/server#drop_cascade Server#drop_cascade}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/server#drop_cascade Server#drop_cascade}
         '''
         result = self._values.get("drop_cascade")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/server#id Server#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/server#id Server#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def options(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
         '''This clause specifies the options for the server.
 
         The options typically define the connection details of the server, but the actual names and values are dependent on the server's foreign-data wrapper
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/server#options Server#options}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/server#options Server#options}
         '''
         result = self._values.get("options")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     @builtins.property
     def server_owner(self) -> typing.Optional[builtins.str]:
         '''The user name of the new owner of the foreign server.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/server#server_owner Server#server_owner}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/server#server_owner Server#server_owner}
         '''
         result = self._values.get("server_owner")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def server_type(self) -> typing.Optional[builtins.str]:
         '''Optional server type, potentially useful to foreign-data wrappers.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/server#server_type Server#server_type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/server#server_type Server#server_type}
         '''
         result = self._values.get("server_type")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def server_version(self) -> typing.Optional[builtins.str]:
         '''Optional server version, potentially useful to foreign-data wrappers.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/server#server_version Server#server_version}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/server#server_version Server#server_version}
         '''
         result = self._values.get("server_version")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/subscription/__init__.py` & `cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/subscription/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `postgresql_subscription`
 
-Refer to the Terraform Registory for docs: [`postgresql_subscription`](https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/subscription).
+Refer to the Terraform Registory for docs: [`postgresql_subscription`](https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/subscription).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class Subscription(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-postgresql.subscription.Subscription",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/subscription postgresql_subscription}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/subscription postgresql_subscription}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         conninfo: builtins.str,
@@ -44,25 +44,25 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/subscription postgresql_subscription} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/subscription postgresql_subscription} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param conninfo: The connection string to the publisher. It should follow the keyword/value format (https://www.postgresql.org/docs/current/libpq-connect.html#LIBPQ-CONNSTRING). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/subscription#conninfo Subscription#conninfo}
-        :param name: The name of the subscription. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/subscription#name Subscription#name}
-        :param publications: Names of the publications on the publisher to subscribe to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/subscription#publications Subscription#publications}
-        :param create_slot: Specifies whether the command should create the replication slot on the publisher. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/subscription#create_slot Subscription#create_slot}
-        :param database: Sets the database to add the subscription for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/subscription#database Subscription#database}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/subscription#id Subscription#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param slot_name: Name of the replication slot to use. The default behavior is to use the name of the subscription for the slot name Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/subscription#slot_name Subscription#slot_name}
+        :param conninfo: The connection string to the publisher. It should follow the keyword/value format (https://www.postgresql.org/docs/current/libpq-connect.html#LIBPQ-CONNSTRING). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/subscription#conninfo Subscription#conninfo}
+        :param name: The name of the subscription. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/subscription#name Subscription#name}
+        :param publications: Names of the publications on the publisher to subscribe to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/subscription#publications Subscription#publications}
+        :param create_slot: Specifies whether the command should create the replication slot on the publisher. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/subscription#create_slot Subscription#create_slot}
+        :param database: Sets the database to add the subscription for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/subscription#database Subscription#database}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/subscription#id Subscription#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param slot_name: Name of the replication slot to use. The default behavior is to use the name of the subscription for the slot name Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/subscription#slot_name Subscription#slot_name}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -283,21 +283,21 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param conninfo: The connection string to the publisher. It should follow the keyword/value format (https://www.postgresql.org/docs/current/libpq-connect.html#LIBPQ-CONNSTRING). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/subscription#conninfo Subscription#conninfo}
-        :param name: The name of the subscription. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/subscription#name Subscription#name}
-        :param publications: Names of the publications on the publisher to subscribe to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/subscription#publications Subscription#publications}
-        :param create_slot: Specifies whether the command should create the replication slot on the publisher. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/subscription#create_slot Subscription#create_slot}
-        :param database: Sets the database to add the subscription for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/subscription#database Subscription#database}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/subscription#id Subscription#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param slot_name: Name of the replication slot to use. The default behavior is to use the name of the subscription for the slot name Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/subscription#slot_name Subscription#slot_name}
+        :param conninfo: The connection string to the publisher. It should follow the keyword/value format (https://www.postgresql.org/docs/current/libpq-connect.html#LIBPQ-CONNSTRING). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/subscription#conninfo Subscription#conninfo}
+        :param name: The name of the subscription. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/subscription#name Subscription#name}
+        :param publications: Names of the publications on the publisher to subscribe to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/subscription#publications Subscription#publications}
+        :param create_slot: Specifies whether the command should create the replication slot on the publisher. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/subscription#create_slot Subscription#create_slot}
+        :param database: Sets the database to add the subscription for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/subscription#database Subscription#database}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/subscription#id Subscription#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param slot_name: Name of the replication slot to use. The default behavior is to use the name of the subscription for the slot name Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/subscription#slot_name Subscription#slot_name}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__d7cff00aba7ad48bf227119b834b6296652e38cb74b17f236c9caaaaae540079)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -405,77 +405,77 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def conninfo(self) -> builtins.str:
         '''The connection string to the publisher. It should follow the keyword/value format (https://www.postgresql.org/docs/current/libpq-connect.html#LIBPQ-CONNSTRING).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/subscription#conninfo Subscription#conninfo}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/subscription#conninfo Subscription#conninfo}
         '''
         result = self._values.get("conninfo")
         assert result is not None, "Required property 'conninfo' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''The name of the subscription.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/subscription#name Subscription#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/subscription#name Subscription#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def publications(self) -> typing.List[builtins.str]:
         '''Names of the publications on the publisher to subscribe to.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/subscription#publications Subscription#publications}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/subscription#publications Subscription#publications}
         '''
         result = self._values.get("publications")
         assert result is not None, "Required property 'publications' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     @builtins.property
     def create_slot(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Specifies whether the command should create the replication slot on the publisher.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/subscription#create_slot Subscription#create_slot}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/subscription#create_slot Subscription#create_slot}
         '''
         result = self._values.get("create_slot")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def database(self) -> typing.Optional[builtins.str]:
         '''Sets the database to add the subscription for.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/subscription#database Subscription#database}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/subscription#database Subscription#database}
         '''
         result = self._values.get("database")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/subscription#id Subscription#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/subscription#id Subscription#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def slot_name(self) -> typing.Optional[builtins.str]:
         '''Name of the replication slot to use.
 
         The default behavior is to use the name of the subscription for the slot name
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/subscription#slot_name Subscription#slot_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/subscription#slot_name Subscription#slot_name}
         '''
         result = self._values.get("slot_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql/user_mapping/__init__.py` & `cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql/user_mapping/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `postgresql_user_mapping`
 
-Refer to the Terraform Registory for docs: [`postgresql_user_mapping`](https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/user_mapping).
+Refer to the Terraform Registory for docs: [`postgresql_user_mapping`](https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/user_mapping).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class UserMapping(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-postgresql.userMapping.UserMapping",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/user_mapping postgresql_user_mapping}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/user_mapping postgresql_user_mapping}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         server_name: builtins.str,
@@ -41,22 +41,22 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/user_mapping postgresql_user_mapping} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/user_mapping postgresql_user_mapping} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param server_name: The name of an existing server for which the user mapping is to be created. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/user_mapping#server_name UserMapping#server_name}
-        :param user_name: The name of an existing user that is mapped to foreign server. CURRENT_ROLE, CURRENT_USER, and USER match the name of the current user. When PUBLIC is specified, a so-called public mapping is created that is used when no user-specific mapping is applicable Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/user_mapping#user_name UserMapping#user_name}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/user_mapping#id UserMapping#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param options: This clause specifies the options of the user mapping. The options typically define the actual user name and password of the mapping. Option names must be unique. The allowed option names and values are specific to the server's foreign-data wrapper Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/user_mapping#options UserMapping#options}
+        :param server_name: The name of an existing server for which the user mapping is to be created. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/user_mapping#server_name UserMapping#server_name}
+        :param user_name: The name of an existing user that is mapped to foreign server. CURRENT_ROLE, CURRENT_USER, and USER match the name of the current user. When PUBLIC is specified, a so-called public mapping is created that is used when no user-specific mapping is applicable Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/user_mapping#user_name UserMapping#user_name}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/user_mapping#id UserMapping#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param options: This clause specifies the options of the user mapping. The options typically define the actual user name and password of the mapping. Option names must be unique. The allowed option names and values are specific to the server's foreign-data wrapper Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/user_mapping#options UserMapping#options}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -206,18 +206,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param server_name: The name of an existing server for which the user mapping is to be created. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/user_mapping#server_name UserMapping#server_name}
-        :param user_name: The name of an existing user that is mapped to foreign server. CURRENT_ROLE, CURRENT_USER, and USER match the name of the current user. When PUBLIC is specified, a so-called public mapping is created that is used when no user-specific mapping is applicable Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/user_mapping#user_name UserMapping#user_name}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/user_mapping#id UserMapping#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param options: This clause specifies the options of the user mapping. The options typically define the actual user name and password of the mapping. Option names must be unique. The allowed option names and values are specific to the server's foreign-data wrapper Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/user_mapping#options UserMapping#options}
+        :param server_name: The name of an existing server for which the user mapping is to be created. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/user_mapping#server_name UserMapping#server_name}
+        :param user_name: The name of an existing user that is mapped to foreign server. CURRENT_ROLE, CURRENT_USER, and USER match the name of the current user. When PUBLIC is specified, a so-called public mapping is created that is used when no user-specific mapping is applicable Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/user_mapping#user_name UserMapping#user_name}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/user_mapping#id UserMapping#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param options: This clause specifies the options of the user mapping. The options typically define the actual user name and password of the mapping. Option names must be unique. The allowed option names and values are specific to the server's foreign-data wrapper Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/user_mapping#options UserMapping#options}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__70b7ab4e0de3ad7210b8d91e53b074d85dcb1f016cfd5589ee0c2042e7c06c31)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -317,49 +317,49 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def server_name(self) -> builtins.str:
         '''The name of an existing server for which the user mapping is to be created.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/user_mapping#server_name UserMapping#server_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/user_mapping#server_name UserMapping#server_name}
         '''
         result = self._values.get("server_name")
         assert result is not None, "Required property 'server_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def user_name(self) -> builtins.str:
         '''The name of an existing user that is mapped to foreign server.
 
         CURRENT_ROLE, CURRENT_USER, and USER match the name of the current user. When PUBLIC is specified, a so-called public mapping is created that is used when no user-specific mapping is applicable
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/user_mapping#user_name UserMapping#user_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/user_mapping#user_name UserMapping#user_name}
         '''
         result = self._values.get("user_name")
         assert result is not None, "Required property 'user_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/user_mapping#id UserMapping#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/user_mapping#id UserMapping#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def options(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
         '''This clause specifies the options of the user mapping.
 
         The options typically define the actual user name and password of the mapping. Option names must be unique. The allowed option names and values are specific to the server's foreign-data wrapper
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.19.0/docs/resources/user_mapping#options UserMapping#options}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/cyrilgdn/postgresql/1.20.0/docs/resources/user_mapping#options UserMapping#options}
         '''
         result = self._values.get("options")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql.egg-info/PKG-INFO` & `cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-postgresql
-Version: 7.0.0
+Version: 8.0.0
 Summary: Prebuilt postgresql Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-postgresql.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-postgresql.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-postgresql-7.0.0/src/cdktf_cdktf_provider_postgresql.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-postgresql-8.0.0/src/cdktf_cdktf_provider_postgresql.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdktf_cdktf_provider_postgresql/py.typed
 src/cdktf_cdktf_provider_postgresql.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_postgresql.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_postgresql.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_postgresql.egg-info/requires.txt
 src/cdktf_cdktf_provider_postgresql.egg-info/top_level.txt
 src/cdktf_cdktf_provider_postgresql/_jsii/__init__.py
-src/cdktf_cdktf_provider_postgresql/_jsii/provider-postgresql@7.0.0.jsii.tgz
+src/cdktf_cdktf_provider_postgresql/_jsii/provider-postgresql@8.0.0.jsii.tgz
 src/cdktf_cdktf_provider_postgresql/data_postgresql_schemas/__init__.py
 src/cdktf_cdktf_provider_postgresql/data_postgresql_sequences/__init__.py
 src/cdktf_cdktf_provider_postgresql/data_postgresql_tables/__init__.py
 src/cdktf_cdktf_provider_postgresql/database/__init__.py
 src/cdktf_cdktf_provider_postgresql/default_privileges/__init__.py
 src/cdktf_cdktf_provider_postgresql/extension/__init__.py
 src/cdktf_cdktf_provider_postgresql/function_resource/__init__.py
```

