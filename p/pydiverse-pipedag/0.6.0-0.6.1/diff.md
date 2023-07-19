# Comparing `tmp/pydiverse_pipedag-0.6.0.tar.gz` & `tmp/pydiverse_pipedag-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydiverse_pipedag-0.6.0.tar", max compression
+gzip compressed data, was "pydiverse_pipedag-0.6.1.tar", max compression
```

## Comparing `pydiverse_pipedag-0.6.0.tar` & `pydiverse_pipedag-0.6.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0     1517 2023-07-07 14:19:45.678347 pydiverse_pipedag-0.6.0/LICENSE
--rw-r--r--   0        0        0     7229 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/docs/package/README.md
--rw-r--r--   0        0        0     3262 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/pyproject.toml
--rw-r--r--   0        0        0       13 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/.gitignore
--rw-r--r--   0        0        0      413 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/__init__.py
--rw-r--r--   0        0        0      857 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/_typing.py
--rw-r--r--   0        0        0       97 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/__init__.py
--rw-r--r--   0        0        0     5334 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/blob.py
--rw-r--r--   0        0        0      393 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/lock/__init__.py
--rw-r--r--   0        0        0     6097 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/lock/base.py
--rw-r--r--   0        0        0    13278 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/lock/database.py
--rw-r--r--   0        0        0     2541 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/lock/filelock.py
--rw-r--r--   0        0        0      768 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/lock/nolock.py
--rw-r--r--   0        0        0     3671 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/lock/zookeeper.py
--rw-r--r--   0        0        0      233 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/__init__.py
--rw-r--r--   0        0        0    22728 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/base.py
--rw-r--r--   0        0        0      108 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/cache/__init__.py
--rw-r--r--   0        0        0     3106 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/cache/base.py
--rw-r--r--   0        0        0     6503 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/cache/parquet.py
--rw-r--r--   0        0        0     6800 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/dict.py
--rw-r--r--   0        0        0       67 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/sql/__init__.py
--rw-r--r--   0        0        0    37136 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/sql/ddl.py
--rw-r--r--   0        0        0      187 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/sql/dialects/__init__.py
--rw-r--r--   0        0        0      956 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/sql/dialects/duckdb.py
--rw-r--r--   0        0        0     3013 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/sql/dialects/ibm_db2.py
--rw-r--r--   0        0        0     7776 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/sql/dialects/mssql.py
--rw-r--r--   0        0        0     3706 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/sql/dialects/postgres.py
--rw-r--r--   0        0        0    20048 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/sql/hooks.py
--rw-r--r--   0        0        0     4250 2023-07-07 14:19:45.682347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/sql/reflection.py
--rw-r--r--   0        0        0    42398 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/sql/sql.py
--rw-r--r--   0        0        0       81 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/util/__init__.py
--rw-r--r--   0        0        0     8579 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/util/dtype.py
--rw-r--r--   0        0        0      433 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/context/__init__.py
--rw-r--r--   0        0        0     7916 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/context/context.py
--rw-r--r--   0        0        0    26249 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/context/run_context.py
--rw-r--r--   0        0        0      279 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/core/__init__.py
--rw-r--r--   0        0        0    13716 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/core/config.py
--rw-r--r--   0        0        0    16460 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/core/flow.py
--rw-r--r--   0        0        0     3501 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/core/result.py
--rw-r--r--   0        0        0     5848 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/core/stage.py
--rw-r--r--   0        0        0     7731 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/core/task.py
--rw-r--r--   0        0        0      368 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/engine/__init__.py
--rw-r--r--   0        0        0      654 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/engine/base.py
--rw-r--r--   0        0        0     2789 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/engine/dask.py
--rw-r--r--   0        0        0     6536 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/engine/prefect.py
--rw-r--r--   0        0        0     1447 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/engine/sequential.py
--rw-r--r--   0        0        0     1079 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/errors/__init__.py
--rw-r--r--   0        0        0        0 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/management/__init__.py
--rw-r--r--   0        0        0      620 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/management/cli.py
--rw-r--r--   0        0        0        0 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/management/commands/__init__.py
--rw-r--r--   0        0        0     1734 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/management/commands/clear_metadata.py
--rw-r--r--   0        0        0     2700 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/management/commands/delete_schemas.py
--rw-r--r--   0        0        0      160 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/materialize/__init__.py
--rw-r--r--   0        0        0     8991 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/materialize/cache.py
--rw-r--r--   0        0        0     5431 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/materialize/container.py
--rw-r--r--   0        0        0     9875 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/materialize/core.py
--rw-r--r--   0        0        0     2074 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/materialize/metadata.py
--rw-r--r--   0        0        0    16812 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/materialize/store.py
--rw-r--r--   0        0        0      213 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/util/__init__.py
--rw-r--r--   0        0        0     2061 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/util/deep_map.py
--rw-r--r--   0        0        0     1435 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/util/deep_merge.py
--rw-r--r--   0        0        0      944 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/util/disposable.py
--rw-r--r--   0        0        0     1129 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/util/hashing.py
--rw-r--r--   0        0        0     3298 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/util/import_.py
--rw-r--r--   0        0        0     7992 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/util/ipc.py
--rw-r--r--   0        0        0     4349 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/util/json.py
--rw-r--r--   0        0        0     1377 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/util/naming.py
--rw-r--r--   0        0        0     2847 2023-07-07 14:19:45.686347 pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/util/structlog.py
--rw-r--r--   0        0        0     8890 1970-01-01 00:00:00.000000 pydiverse_pipedag-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1517 2023-07-19 12:57:39.012456 pydiverse_pipedag-0.6.1/LICENSE
+-rw-r--r--   0        0        0     6174 2023-07-19 12:57:39.012456 pydiverse_pipedag-0.6.1/docs/package/README.md
+-rw-r--r--   0        0        0     3421 2023-07-19 12:57:39.016456 pydiverse_pipedag-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0       13 2023-07-19 12:57:39.016456 pydiverse_pipedag-0.6.1/src/pydiverse/.gitignore
+-rw-r--r--   0        0        0      435 2023-07-19 12:57:39.016456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/__init__.py
+-rw-r--r--   0        0        0      857 2023-07-19 12:57:39.016456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/_typing.py
+-rw-r--r--   0        0        0       97 2023-07-19 12:57:39.016456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/backend/__init__.py
+-rw-r--r--   0        0        0     5348 2023-07-19 12:57:39.016456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/backend/blob.py
+-rw-r--r--   0        0        0      393 2023-07-19 12:57:39.016456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/backend/lock/__init__.py
+-rw-r--r--   0        0        0     6097 2023-07-19 12:57:39.016456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/backend/lock/base.py
+-rw-r--r--   0        0        0    13555 2023-07-19 12:57:39.016456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/backend/lock/database.py
+-rw-r--r--   0        0        0     2756 2023-07-19 12:57:39.016456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/backend/lock/filelock.py
+-rw-r--r--   0        0        0      769 2023-07-19 12:57:39.016456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/backend/lock/nolock.py
+-rw-r--r--   0        0        0     3983 2023-07-19 12:57:39.016456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/backend/lock/zookeeper.py
+-rw-r--r--   0        0        0      233 2023-07-19 12:57:39.016456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/backend/table/__init__.py
+-rw-r--r--   0        0        0    23394 2023-07-19 12:57:39.016456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/backend/table/base.py
+-rw-r--r--   0        0        0      108 2023-07-19 12:57:39.016456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/backend/table/cache/__init__.py
+-rw-r--r--   0        0        0     3106 2023-07-19 12:57:39.016456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/backend/table/cache/base.py
+-rw-r--r--   0        0        0     6976 2023-07-19 12:57:39.016456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/backend/table/cache/parquet.py
+-rw-r--r--   0        0        0     6933 2023-07-19 12:57:39.016456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/backend/table/dict.py
+-rw-r--r--   0        0        0      141 2023-07-19 12:57:39.016456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/backend/table/sql/__init__.py
+-rw-r--r--   0        0        0    37136 2023-07-19 12:57:39.016456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/backend/table/sql/ddl.py
+-rw-r--r--   0        0        0      187 2023-07-19 12:57:39.016456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/backend/table/sql/dialects/__init__.py
+-rw-r--r--   0        0        0     1508 2023-07-19 12:57:39.016456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/backend/table/sql/dialects/duckdb.py
+-rw-r--r--   0        0        0     3301 2023-07-19 12:57:39.016456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/backend/table/sql/dialects/ibm_db2.py
+-rw-r--r--   0        0        0     9235 2023-07-19 12:57:39.016456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/backend/table/sql/dialects/mssql.py
+-rw-r--r--   0        0        0     3956 2023-07-19 12:57:39.016456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/backend/table/sql/dialects/postgres.py
+-rw-r--r--   0        0        0    21371 2023-07-19 12:57:39.016456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/backend/table/sql/hooks.py
+-rw-r--r--   0        0        0     4250 2023-07-19 12:57:39.016456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/backend/table/sql/reflection.py
+-rw-r--r--   0        0        0    47185 2023-07-19 12:57:39.016456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/backend/table/sql/sql.py
+-rw-r--r--   0        0        0       81 2023-07-19 12:57:39.016456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/backend/table/util/__init__.py
+-rw-r--r--   0        0        0     8579 2023-07-19 12:57:39.016456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/backend/table/util/dtype.py
+-rw-r--r--   0        0        0      433 2023-07-19 12:57:39.016456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/context/__init__.py
+-rw-r--r--   0        0        0     9874 2023-07-19 12:57:39.016456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/context/context.py
+-rw-r--r--   0        0        0    26325 2023-07-19 12:57:39.016456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/context/run_context.py
+-rw-r--r--   0        0        0      311 2023-07-19 12:57:39.016456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/core/__init__.py
+-rw-r--r--   0        0        0    14956 2023-07-19 12:57:39.020456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/core/config.py
+-rw-r--r--   0        0        0    20430 2023-07-19 12:57:39.020456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/core/flow.py
+-rw-r--r--   0        0        0     4294 2023-07-19 12:57:39.020456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/core/result.py
+-rw-r--r--   0        0        0     7789 2023-07-19 12:57:39.020456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/core/stage.py
+-rw-r--r--   0        0        0     8013 2023-07-19 12:57:39.020456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/core/task.py
+-rw-r--r--   0        0        0      368 2023-07-19 12:57:39.020456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/engine/__init__.py
+-rw-r--r--   0        0        0      654 2023-07-19 12:57:39.020456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/engine/base.py
+-rw-r--r--   0        0        0     3133 2023-07-19 12:57:39.020456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/engine/dask.py
+-rw-r--r--   0        0        0     7269 2023-07-19 12:57:39.020456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/engine/prefect.py
+-rw-r--r--   0        0        0     1388 2023-07-19 12:57:39.020456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/engine/sequential.py
+-rw-r--r--   0        0        0     1079 2023-07-19 12:57:39.020456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/errors/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-19 12:57:39.020456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/management/__init__.py
+-rw-r--r--   0        0        0      620 2023-07-19 12:57:39.020456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/management/cli.py
+-rw-r--r--   0        0        0        0 2023-07-19 12:57:39.020456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/management/commands/__init__.py
+-rw-r--r--   0        0        0     1741 2023-07-19 12:57:39.020456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/management/commands/clear_metadata.py
+-rw-r--r--   0        0        0     2744 2023-07-19 12:57:39.020456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/management/commands/delete_schemas.py
+-rw-r--r--   0        0        0      182 2023-07-19 12:57:39.020456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/materialize/__init__.py
+-rw-r--r--   0        0        0     9114 2023-07-19 12:57:39.020456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/materialize/cache.py
+-rw-r--r--   0        0        0    11091 2023-07-19 12:57:39.020456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/materialize/container.py
+-rw-r--r--   0        0        0    17639 2023-07-19 12:57:39.020456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/materialize/core.py
+-rw-r--r--   0        0        0     2074 2023-07-19 12:57:39.020456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/materialize/metadata.py
+-rw-r--r--   0        0        0    19431 2023-07-19 12:57:39.020456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/materialize/store.py
+-rw-r--r--   0        0        0      213 2023-07-19 12:57:39.020456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/util/__init__.py
+-rw-r--r--   0        0        0     2061 2023-07-19 12:57:39.020456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/util/deep_map.py
+-rw-r--r--   0        0        0     1435 2023-07-19 12:57:39.020456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/util/deep_merge.py
+-rw-r--r--   0        0        0      944 2023-07-19 12:57:39.020456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/util/disposable.py
+-rw-r--r--   0        0        0     1129 2023-07-19 12:57:39.020456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/util/hashing.py
+-rw-r--r--   0        0        0     3736 2023-07-19 12:57:39.020456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/util/import_.py
+-rw-r--r--   0        0        0     7992 2023-07-19 12:57:39.020456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/util/ipc.py
+-rw-r--r--   0        0        0     4400 2023-07-19 12:57:39.020456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/util/json.py
+-rw-r--r--   0        0        0     1377 2023-07-19 12:57:39.020456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/util/naming.py
+-rw-r--r--   0        0        0     2847 2023-07-19 12:57:39.020456 pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/util/structlog.py
+-rw-r--r--   0        0        0     7911 1970-01-01 00:00:00.000000 pydiverse_pipedag-0.6.1/PKG-INFO
```

### Comparing `pydiverse_pipedag-0.6.0/LICENSE` & `pydiverse_pipedag-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.0/docs/package/README.md` & `pydiverse_pipedag-0.6.1/docs/package/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -106,43 +106,31 @@
 if __name__ == "__main__":
     main()
 ```
 
 Create a file called `pipedag.yaml` in the same directory:
 
 ```yaml
-name: pipedag_tests
-table_store_connections:
-  postgres:
-    args:
-      # Postgres: this can be used after running `docker-compose up`  
-      url: "postgresql://{$POSTGRES_USERNAME}:{$POSTGRES_PASSWORD}@127.0.0.1:6543/{instance_id}"
-
 instances:
   __any__:
-    # listen-interface for pipedag context server which synchronizes some task state during DAG execution
     network_interface: "127.0.0.1"
-    # classes to be materialized to table store even without pipedag Table wrapper (we have loose coupling between
-    # pipedag and pydiverse.transform, so consider adding 'pydiverse.transform.Table' in your config)
-    auto_table: ["pandas.DataFrame", "sqlalchemy.sql.elements.TextClause", "sqlalchemy.sql.selectable.Selectable"]
-    fail_fast: true
+    auto_table:
+      - "pandas.DataFrame"
+      - "sqlalchemy.sql.expression.TextClause"
+      - "sqlalchemy.sql.expression.Selectable"
 
+    fail_fast: true
     instance_id: pipedag_default
     table_store:
       class: "pydiverse.pipedag.backend.table.SQLTableStore"
-
-      # Postgres: this can be used after running `docker-compose up`
-      table_store_connection: postgres
       args:
+        url: "postgresql://sa:Pydiverse23@127.0.0.1:6543/{instance_id}"
         create_database_if_not_exists: True
-        
-        # print select statements before being encapsualted in materialize expressions and tables before writing to
-        # database
+
         print_materialize: true
-        # print final sql statements
         print_sql: true
 
       local_table_cache:
         store_input: true
         store_output: true
         use_stored_input_as_cache: true
         class: "pydiverse.pipedag.backend.table.cache.ParquetTableCache"
@@ -151,53 +139,40 @@
 
     blob_store:
       class: "pydiverse.pipedag.backend.blob.FileBlobStore"
       args:
         base_path: "/tmp/pipedag/blobs"
 
     lock_manager:
-      class: "pydiverse.pipedag.backend.lock.ZooKeeperLockManager"
-      args:
-        hosts: "localhost:2181"
+      class: "pydiverse.pipedag.backend.lock.DatabaseLockManager"
 
     orchestration:
       class: "pydiverse.pipedag.engine.SequentialEngine"
 ```
 
-If you don't have a postgres, Microsoft SQL Server, or IBM DB2 database at hand, you can
-start a postgres database with the following `docker-compose.yaml` file:
+If you don't have a postgres database at hand, you can start a postgres database, with the following `docker-compose.yaml` file:
 
 ```yaml
 version: "3.9"
 services:
   postgres:
     image: postgres
     environment:
       POSTGRES_USER: sa
       POSTGRES_PASSWORD: Pydiverse23
-      POSTGRES_PORT: 6543
-    ports:
-      - 6543:5432
-  zoo:
-    image: zookeeper
-    environment:
-      ZOO_4LW_COMMANDS_WHITELIST: ruok
-      ZOO_MAX_CLIENT_CNXNS: 100
     ports:
-      - 2181:2181
+      - "6543:5432"
 ```
 
 Run `docker-compose up` in the directory of your `docker-compose.yaml` and then execute
 the flow script as follows with a shell like `bash` and a python environment that
 includes `pydiverse-pipedag`, `pandas`, and `sqlalchemy`:
 
 ```bash
-export POSTGRES_USERNAME=sa
-export POSTGRES_PASSWORD=Pydiverse23
-python run_pipeline.py
+poetry run python run_pipeline.py
 ```
 
 Finally, you may connect to your localhost postgres database `pipedag_default` and
 look at tables in schemas `stage_1`..`stage_3`.
 
 If you don't have a SQL UI at hand, you may use `psql` command line tool inside the docker container.
 Check out the `NAMES` column in `docker ps` output. If the name of your postgres container is
```

### Comparing `pydiverse_pipedag-0.6.0/pyproject.toml` & `pydiverse_pipedag-0.6.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydiverse-pipedag"
-version = "0.6.0"
+version = "0.6.1"
 description = "A pipeline orchestration library executing tasks within one python session. It takes care of SQL table (de)materialization, caching and cache invalidation. Blob storage is supported as well for example for storing model files."
 authors = [
   "QuantCo, Inc.",
   "Nicolas Camenisch <garnele007@gmail.com>",
   "Martin Trautmann <windiana@users.sf.net>",
 ]
 license = "BSD-3-Clause"
@@ -38,25 +38,28 @@
 pydot = ">=1.4.2"
 click = "^8.1.3"
 pyparsing = ">=3.0"
 
 filelock = { version = ">=3.7.1", optional = true }
 kazoo = { version = ">=2.8.0", optional = true }
 dask = { version = ">=2022.1.0", optional = true }
+prefect = { version = ">=2.6", optional = true }
 
 
 [tool.poetry.extras]
 filelock = ["filelock"]
 zookeeper = ["kazoo"]
 dask = ["dask"]
+prefect = ["prefect"]
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7.2.0"
 pytest-mock = ">=3.10.0"
 pytest-timeout = ">=2.1.0"
+tox = "^4.6.4"
 
 black = { version = "23.3.0", extras = ["d"] }
 ruff = "^0.0.270"
 pre-commit = ">=2.20.0"
 
 kazoo = ">=2.8.0"
 dask = ">=2022.1.0"
@@ -73,31 +76,33 @@
 ibis-framework = { version = ">=5.1.0", extras = ["mssql", "postgres"] }
 polars = ">=0.16.18"
 tidypolars = { version = "^0.2.19", python = "<3.11" }
 connectorx = [
     { version = ">=0.3.1", python = "<3.11" },
     { version = "0.3.2a5", python = "==3.11" }  # Latest full release is broken - unpin when 0.3.2 released
 ]
-# Engines
-prefect = "^1.3"
 # MSSQL
 pyodbc = ">=4.0.35"
 pytsql = ">=1.1.4"
 # IBM DB2
 ibm-db = { version = ">=3.1.4", markers="platform_machine == 'x86_64'" }
 ibm-db-sa = { version = ">=0.3.8", markers="platform_machine == 'x86_64'" }
 
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-Sphinx = "^5.1.1"
-sphinx-rtd-theme = "^1.0.0"
+Sphinx = "^7.0.1"
+furo = "^2023.5.20"
 sphinxcontrib-apidoc = "^0.3.0"
+myst-parser = "^2.0.0"
+sphinx-click = "^4.4.0"
+sphinx-autobuild = "^2021.3.14"
+sphinx-copybutton = "^0.5.2"
 
 [tool.poetry.plugins."console_scripts"]
 pipedag-manage = "pydiverse.pipedag.management.cli:cli"
 
 [tool.black]
 exclude = '''
 /(
```

### Comparing `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/_typing.py` & `pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/_typing.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/blob.py` & `pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/backend/blob.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,19 +22,19 @@
 
 
 class BaseBlobStore(Disposable, ABC):
     """Blob store base class
 
     A blob (binary large object) store is responsible for storing arbitrary
     python objects. This can, for example, be done by serializing them using
-    the python `pickle` module.
+    the python ``pickle`` module.
 
-    A store must use a blob's name (`blob.name`) and stage (`blob.stage`)
+    A store must use a blob's name (``Blob.name``) and stage (``Blob.stage``)
     as the primary keys for storing and retrieving blobs. This means that
-    two different `Blob` objects can be used to store and retrieve the same
+    two different ``Blob`` objects can be used to store and retrieve the same
     data as long as they have the same name and stage.
     """
 
     @abstractmethod
     def init_stage(self, stage: Stage):
         """Initialize a stage and start a transaction"""
 
@@ -74,19 +74,19 @@
         stage.
         """
 
 
 class FileBlobStore(BaseBlobStore):
     """File based blob store
 
-    The FileBlobStore stores blobs in a folder structure on a file system.
+    The ``FileBlobStore`` stores blobs in a folder structure on a file system.
     In the base directory there will be two folders for every stage, one
     for the base and one for the transaction stage. Inside those folders the
     blobs will be stored as pickled files:
-    `base_path/instance_id/STAGE_NAME/BLOB_NAME.pkl`.
+    ``base_path/instance_id/STAGE_NAME/BLOB_NAME.pkl``.
 
     To commit a stage, the only thing that has to be done is to rename
     the appropriate folders.
     """
 
     @classmethod
     def _init_conf_(cls, config: dict[str, Any]):
```

### Comparing `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/lock/base.py` & `pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/backend/lock/base.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/lock/database.py` & `pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/backend/lock/database.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,19 @@
 
     Many databases provide some kind of locking mechanism. Depending on the specific
     database technology, this allows us to implement locking on either the schema
     level (where each stage can be locked and unlocked individually), or only on
     the instance level (where the entire instance including all stages get locked and
     unlocked together).
 
-    The database specific lock implementations can be found at the end of the file.
+    This lock manager uses the same database as the ``SQLTableStore``.
+    No other configuration in the ``args`` section of the config file is required.
+
+    We currently support the following databases:
+    PostgreSQL, Microsoft SQL Server, IBM DB2.
     """
 
     __registered_dialects: dict[str, type[DatabaseLockManager]] = {}
     _dialect_name: str
 
     def __new__(cls, engine: sa.Engine, *args, **kwargs):
         if cls != DatabaseLockManager:
@@ -265,14 +269,19 @@
     def get_lock_object(self, lockable: Lockable):
         if self.connection is None:
             self.connection = self.engine.connect()
 
         name = self.lock_name(lockable)
         return PostgresLock(name, self.connection)
 
+    def dispose(self):
+        self.release_all()
+        self.connection.close()
+        super().dispose()
+
 
 class MSSqlLock(Lock):
     """
     Locking based on application resource locks.
     https://learn.microsoft.com/en-us/sql/relational-databases/system-stored-procedures/sp-getapplock-transact-sql?view=sql-server-ver15
     """
```

### Comparing `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/lock/filelock.py` & `pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/backend/lock/filelock.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,31 +20,35 @@
 @requires(fl, ImportError("FileLockManager requires 'filelock' to be installed."))
 class FileLockManager(BaseLockManager):
     """Lock manager that uses lock files
 
     For details on how exactly the file locking is implemented, check out the
     `filelock documentation`_.
 
-    .. _`filelock documentation`:
-        https://py-filelock.readthedocs.io/en/latest/index.html
+    :param base_path:
+        A path to a folder where the lock files should get stored.
+        To differentiate between different instances, the ``instance_id`` will
+        automatically be appended to the provided path.
+
+    .. _filelock documentation: https://py-filelock.readthedocs.io/en/latest/index.html
     """
 
+    @classmethod
+    def _init_conf_(cls, config: dict[str, Any]):
+        instance_id = normalize_name(ConfigContext.get().instance_id)
+        base_path = Path(config["base_path"]) / instance_id
+        return cls(base_path)
+
     def __init__(self, base_path: str | Path):
         super().__init__()
         self.base_path = Path(base_path).absolute()
         self.locks: dict[Lockable, fl.BaseFileLock] = {}
 
         os.makedirs(self.base_path, exist_ok=True)
 
-    @classmethod
-    def _init_conf_(cls, config: dict[str, Any]):
-        instance_id = normalize_name(ConfigContext.get().instance_id)
-        base_path = Path(config["base_path"]) / instance_id
-        return cls(base_path)
-
     @property
     def supports_stage_level_locking(self):
         return True
 
     def acquire(self, lockable: Lockable):
         if lockable not in self.locks:
             lock_path = self.lock_path(lockable)
```

### Comparing `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/lock/nolock.py` & `pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/backend/lock/nolock.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from __future__ import annotations
 
 from pydiverse.pipedag.backend.lock.base import BaseLockManager, Lockable, LockState
 
 
 class NoLockManager(BaseLockManager):
-    """Non locking lock manager (oxymoron)
-
+    """
     This lock manager doesn't do any locking and only serves as a placeholder
     for an actual lock manager for testing something locally.
 
-    .. WARNING::
-        DON'T USE THIS IN A PRODUCTION ENVIRONMENT. A LOCK MANAGER IS
-        ESSENTIAL TO PREVENT DATA CORRUPTION.
+    .. Warning::
+        This lock manager is not intended for use in a production environment.
+        Using a lock manager is essential for preventing data corruption.
     """
 
     @property
     def supports_stage_level_locking(self):
         return True
 
     def acquire(self, lockable: Lockable):
```

### Comparing `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/lock/zookeeper.py` & `pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/backend/lock/zookeeper.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,19 +19,28 @@
 
 
 @requires(kazoo, ImportError("ZooKeeperLockManager requires 'kazoo' to be installed."))
 class ZooKeeperLockManager(BaseLockManager):
     """Apache ZooKeeper based lock manager
 
     Uses Apache ZooKeeper to establish `fully distributed locks that are
-    globally synchronous` [1]_. The advantage of this approach is that we
-    it is highly reliable and that in case our flow crashes, the acquired
-    locks automatically get released (the locks are ephemeral).
+    globally synchronous`_. The advantage of this approach is that we it is highly
+    reliable and that in case our flow crashes, the acquired locks automatically
+    get released (the locks are ephemeral).
 
-    .. [1] https://zookeeper.apache.org/doc/r3.1.2/recipes.html#sc_recipes_Locks
+    Config File
+    -----------
+    All arguments in the ``args`` section get passed as-is to the initializer
+    of :py:class:`kazoo.client.KazooClient`. Some useful arguments include:
+
+    :param hosts:
+        Comma separated list of hosts to connect.
+
+    .. _fully distributed locks that are globally synchronous:
+        https://zookeeper.apache.org/doc/r3.1.2/recipes.html#sc_recipes_Locks
     """
 
     @classmethod
     def _init_conf_(cls, config: dict[str, Any]):
         client = KazooClient(**config)
         instance_id = normalize_name(ConfigContext.get().instance_id)
         base_path = f"/pipedag/locks/{instance_id}/"
```

### Comparing `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/base.py` & `pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/backend/table/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,16 +36,16 @@
         """Decorator to register a `TableHook`
 
         Each table store should be able to handle tables of various different
         types (e.g. a pandas dataframe, a sqlalchemy select statement, a
         pydiverse transform table, ...). To add table type specific logic to
         a table store so called TableHooks are used.
 
-        This decorator is used to register such a hook:
-        ::
+        This decorator is used to register such a hook::
+
             try:
                 from library import x
             except ImportError as e:
                 warnings.warn(str(e), ImportWarning)
                 x = None
 
             @TableStore.register_table(x)
@@ -332,15 +332,15 @@
         query_str = re.sub(r'["\[\]]', "", query_str)
         query_str = re.sub(
             r'(__tmp|__even|__odd)(?=[ \t\n.;"]|$)', "", query_str.lower()
         )
 
         query_hash = stable_hash("RAW-SQL", query_str)
 
-        table_cache_info = CacheManager.raw_sql_cache_lookup(
+        table_cache_info, raw_sql_metadata = CacheManager.raw_sql_cache_lookup(
             self, task_info.task_cache_info, raw_sql, query_hash
         )
         if not table_cache_info.is_cache_valid():
             TaskContext.get().is_cache_valid = False
             RunContext.get().set_stage_has_changed(task.stage)
 
             prev_objects = self.get_objects_in_stage(raw_sql.stage)
@@ -348,23 +348,31 @@
             post_objects = self.get_objects_in_stage(raw_sql.stage)
 
             # Object names must be sorted to ensure that we can identify the task
             # again in the future even if the objects get returned in a different order.
             prev_objects = sorted(prev_objects)
 
             prev_objects_set = set(prev_objects)
-            new_objects = [o for o in post_objects if o in prev_objects_set]
-            table_cache_info.store_raw_sql_metadata(self, prev_objects, new_objects)
+            new_objects = [o for o in post_objects if o not in prev_objects_set]
+        else:
+            prev_objects = raw_sql_metadata.prev_objects
+            new_objects = raw_sql_metadata.new_objects
+
+        table_cache_info.store_raw_sql_metadata(self, prev_objects, new_objects)
 
         # At this point we MUST also update the cache info, so that any downstream
         # tasks get invalidated if the sql query string changed.
         raw_sql.cache_key = CacheManager.lazy_table_cache_key(
             task_info.task_cache_info.get_task_cache_key(), query_hash
         )
 
+        # Store new_objects as part of raw_sql.
+        all_table_names = set(self.get_table_objects_in_stage(raw_sql.stage))
+        raw_sql.table_names = sorted(o for o in new_objects if o in all_table_names)
+
     @abstractmethod
     def copy_table_to_transaction(self, table: Table):
         """Copy a table from the base stage to the transaction stage
 
         This operation MUST not remove the table from the base stage store
         or modify it in any way.
 
@@ -521,14 +529,24 @@
         table store to determine which objects were produced (or could have been used
         to produce those objects) when executing RawSQL.
 
         :param stage: the stage
         :return: list of object names in the stage at the current point in time.
         """
 
+    @abstractmethod
+    def get_table_objects_in_stage(self, stage: Stage) -> list[str]:
+        """
+        List all table-like objects that are in the current stage.
+
+        :param stage: the stage
+        :return: list of table-like object names in the stage at
+            the current point in time.
+        """
+
 
 class TableHook(Generic[TableHookResolverT], ABC):
     """Base class to define how to handle a specific table
 
     For more information, take a look at the `BaseTableStore.register_table`
     documentation.
     """
```

### Comparing `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/cache/base.py` & `pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/backend/table/cache/base.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/cache/parquet.py` & `pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/backend/table/cache/parquet.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,31 @@
 from pydiverse.pipedag.backend.table.base import TableHook
 from pydiverse.pipedag.backend.table.cache.base import BaseTableCache
 from pydiverse.pipedag.materialize.core import MaterializingTask, TaskInfo
 from pydiverse.pipedag.util import normalize_name
 
 
 class ParquetTableCache(BaseTableCache):
+    """
+    Local Table Cache that stores tables in `Parquet`_ files.
+
+    .. rubric:: Supported Tables
+
+    The `ParquetTableCache` supports Pandas, Polars and pydiverse.transform.
+
+
+    :param base_path:
+        A path to a folder where the Parquet files should get stored.
+        To differentiate between different instances, the ``instance_id`` will
+        automatically be appended to the provided path.
+
+    .. _parquet:
+        https://parquet.apache.org
+    """
+
     @classmethod
     def _init_conf_(cls, config: dict[str, Any]):
         instance_id = normalize_name(ConfigContext.get().instance_id)
 
         config = config.copy()
         base_path = Path(config.pop("base_path")) / instance_id
         return cls(base_path=base_path, **config)
```

### Comparing `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/dict.py` & `pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/backend/table/dict.py`

 * *Files 4% similar despite different names*

```diff
@@ -119,14 +119,17 @@
             return self.lazy_table_metadata[stage.name][cache_key]
         except (TypeError, KeyError):
             raise CacheError("Couldn't find metadata for lazy table") from None
 
     def get_objects_in_stage(self, stage):
         return list(self.store[stage.transaction_name].keys())
 
+    def get_table_objects_in_stage(self, stage: Stage) -> list[str]:
+        return list(self.store[stage.transaction_name].keys())
+
 
 @DictTableStore.register_table(pd)
 class PandasTableHook(TableHook[DictTableStore]):
     @classmethod
     def can_materialize(cls, type_) -> bool:
         return issubclass(type_, pd.DataFrame)
```

### Comparing `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/sql/ddl.py` & `pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/backend/table/sql/ddl.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/sql/dialects/duckdb.py` & `pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/backend/table/sql/dialects/duckdb.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,49 @@
 from __future__ import annotations
 
+from pathlib import Path
+
 import sqlalchemy as sa
 
 from pydiverse.pipedag.backend.table.sql.hooks import IbisTableHook
 from pydiverse.pipedag.backend.table.sql.sql import SQLTableStore
 
 
 class DuckDBTableStore(SQLTableStore):
+    """
+    SQLTableStore that supports `DuckDB <https://duckdb.org>`_.
+
+    Takes the same arguments as
+    :py:class:`SQLTableStore <pydiverse.pipedag.backend.table.SQLTableStore>`
+    """
+
     _dialect_name = "duckdb"
 
     def _metadata_pk(self, name: str, table_name: str):
         sequence = sa.Sequence(f"{table_name}_{name}_seq", metadata=self.sql_metadata)
         return sa.Column(
             name,
             sa.BigInteger(),
             sequence,
             server_default=sequence.next_value(),
             primary_key=True,
         )
 
     def _init_database(self):
+        if not self.create_database_if_not_exists:
+            return
+
         # Duckdb already creates the database file automatically
-        pass
+        # However, the parent directory doesn't get created automatically
+        database = self.engine_url.database
+        if database == ":memory:":
+            return
+
+        database_path = Path(database)
+        database_path.parent.mkdir(parents=True, exist_ok=True)
 
 
 try:
     import ibis
 except ImportError:
     ibis = None
```

### Comparing `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/sql/dialects/ibm_db2.py` & `pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/backend/table/sql/dialects/ibm_db2.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,14 +15,22 @@
 from pydiverse.pipedag.backend.table.sql.reflection import PipedagDB2Reflection
 from pydiverse.pipedag.backend.table.sql.sql import SQLTableStore
 from pydiverse.pipedag.backend.table.util import DType
 from pydiverse.pipedag.materialize import Table
 
 
 class IBMDB2TableStore(SQLTableStore):
+    """
+    SQLTableStore that supports `IBM Db2 <https://www.ibm.com/products/db2>`_.
+    Requires `ibm-db-sa <https://pypi.org/project/ibm-db-sa/>`_ to be installed.
+
+    Takes the same arguments as
+    :py:class:`SQLTableStore <pydiverse.pipedag.backend.table.SQLTableStore>`
+    """
+
     _dialect_name = "ibm_db_sa"
 
     def add_primary_key(
         self,
         table_name: str,
         schema: Schema,
         key_columns: list[str],
```

### Comparing `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/sql/dialects/mssql.py` & `pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/backend/table/sql/dialects/mssql.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,27 +20,55 @@
 from pydiverse.pipedag.backend.table.sql.sql import SQLTableStore
 from pydiverse.pipedag.backend.table.util import DType
 from pydiverse.pipedag.materialize import Table
 from pydiverse.pipedag.materialize.container import RawSql
 
 
 class MSSqlTableStore(SQLTableStore):
+    """
+    SQLTableStore that supports `Microsoft SQL Server`_.
+
+    In addition to the arguments of
+    :py:class:`SQLTableStore <pydiverse.pipedag.backend.table.SQLTableStore>`,
+    it also takes the following arguments:
+
+    :param disable_pytsql:
+        For mssql, a package called `pytsql <https://pypi.org/project/pytsql/>`_ is
+        used for executing RawSql scripts. It has the advantage that it allows for
+        some kind of SQL based print statements. However, it may fail for some
+        statements. For those cases, you can set ``disable_pytsql: true`` to use another
+        logic for splitting up Raw SQL scripts and handing that over to sqlalchemy.
+        This is actually quite a complex process for mssql.
+        Sorry for any inconveniences. We will try to make it work for most tsql code
+        that should be integrated in pipedag pipelines. However, the ultimate goal
+        is to split up monolithic blocks of dynamic sql statements into defined
+        transformations with dynamic aspects written in python.
+
+    :param pytsql_isolate_top_level_statements:
+        This parameter is handed over to `pytsql.executes`_ and causes the script to
+        be split in top level statements that are sent to sqlalchemy separately.
+        The tricky part here is that some magic is done to make DECLARE statements
+        reach across, but it is not guaranteed to be identical to scripts executed
+        by a SQL UI.
+
+    .. _Microsoft SQL Server:
+        https://www.microsoft.com/en/sql-server/
+    .. _pytsql.executes:
+        https://pytsql.readthedocs.io/en/latest/api/pytsql.html#pytsql.executes
+    """
+
     _dialect_name = "mssql"
 
     def __init__(
         self,
         *args,
         disable_pytsql: bool = False,
         pytsql_isolate_top_level_statements: bool = True,
         **kwargs,
     ):
-        """
-        :param disable_pytsql: whether to disable the use of pytsql
-        :param pytsql_isolate_top_level_statements: forward pytsql executes() parameter
-        """
         self.disable_pytsql = disable_pytsql
         self.pytsql_isolate_top_level_statements = pytsql_isolate_top_level_statements
 
         super().__init__(*args, **kwargs)
 
     def _init_database(self):
         self._init_database_with_database("master", {"isolation_level": "AUTOCOMMIT"})
```

### Comparing `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/sql/dialects/postgres.py` & `pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/backend/table/sql/dialects/postgres.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,48 +18,59 @@
 from pydiverse.pipedag.backend.table.sql.sql import SQLTableStore
 from pydiverse.pipedag.backend.table.util import DType
 from pydiverse.pipedag.materialize import Table
 from pydiverse.pipedag.materialize.core import TaskInfo
 
 
 class PostgresTableStore(SQLTableStore):
+    """
+    SQLTableStore that supports `PostgreSQL <https://postgresql.org>`_.
+
+    In addition to the arguments of
+    :py:class:`SQLTableStore <pydiverse.pipedag.backend.table.SQLTableStore>`,
+    it also takes the following arguments:
+
+    :param unlogged_tables:
+        Whether to use `unlogged`_ tables or not.
+        This reduces safety in case of a crash or unclean shutdown, but can
+        significantly increase write performance.
+
+    .. _unlogged:
+        https://www.postgresql.org/docs/9.5/sql-createtable.html
+        #SQL-CREATETABLE-UNLOGGED
+    """
+
     _dialect_name = "postgresql"
 
     def __init__(
         self,
         *args,
         unlogged_tables: bool = False,
         **kwargs,
     ):
-        """
-        :param unlogged_tables: whether to use UNLOGGED tables or not.
-            This reduces safety in case of a crash or unclean shutdown, but can
-            significantly increase write performance.
-            https://www.postgresql.org/docs/9.5/sql-createtable.html#SQL-CREATETABLE-UNLOGGED
-        """
         self.unlogged_tables = unlogged_tables
 
         super().__init__(*args, **kwargs)
 
     def _init_database(self):
         self._init_database_with_database("postgres", {"isolation_level": "AUTOCOMMIT"})
 
 
 @PostgresTableStore.register_table()
 class SQLAlchemyTableHook(SQLAlchemyTableHook):
     @classmethod
     def materialize(
         cls,
         store: PostgresTableStore,
-        table: Table[sa.sql.elements.TextClause | sa.Text],
+        table: Table[sa.sql.expression.TextClause | sa.Text],
         stage_name,
         task_info: TaskInfo | None,
     ):
         obj = table.obj
-        if isinstance(table.obj, (sa.Table, sa.sql.selectable.Alias)):
+        if isinstance(table.obj, (sa.Table, sa.sql.expression.Alias)):
             obj = sa.select("*").select_from(table.obj)
 
         schema = store.get_schema(stage_name)
         store.execute(
             CreateTableAsSelect(
                 table.name,
                 schema,
```

### Comparing `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/sql/hooks.py` & `pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/backend/table/sql/hooks.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from pydiverse.pipedag import ConfigContext
 from pydiverse.pipedag._typing import T
 from pydiverse.pipedag.backend.table.base import TableHook
 from pydiverse.pipedag.backend.table.sql.ddl import (
     CreateTableAsSelect,
     Schema,
 )
-from pydiverse.pipedag.backend.table.sql.sql import SQLTableStore
+from pydiverse.pipedag.backend.table.sql.sql import SQLTableStore, TableReference
 from pydiverse.pipedag.backend.table.util import (
     DType,
     PandasDTypeBackend,
 )
 from pydiverse.pipedag.context import TaskContext
 from pydiverse.pipedag.materialize import Table
 from pydiverse.pipedag.materialize.core import TaskInfo
@@ -31,31 +31,31 @@
 
 
 @SQLTableStore.register_table()
 class SQLAlchemyTableHook(TableHook[SQLTableStore]):
     @classmethod
     def can_materialize(cls, type_) -> bool:
         return issubclass(
-            type_, (sa.sql.elements.TextClause, sa.sql.selectable.Selectable)
+            type_, (sa.sql.expression.TextClause, sa.sql.expression.Selectable)
         )
 
     @classmethod
     def can_retrieve(cls, type_) -> bool:
         return type_ == sa.Table
 
     @classmethod
     def materialize(
         cls,
         store,
-        table: Table[sa.sql.elements.TextClause | sa.Text],
+        table: Table[sa.sql.expression.TextClause | sa.Text],
         stage_name,
         task_info: TaskInfo | None,
     ):
         obj = table.obj
-        if isinstance(table.obj, (sa.Table, sa.sql.selectable.Alias)):
+        if isinstance(table.obj, (sa.Table, sa.sql.expression.Alias)):
             obj = sa.select("*").select_from(table.obj)
 
         source_tables = [
             dict(
                 name=tbl.name,
                 schema=store.get_schema(
                     tbl.stage.transaction_name
@@ -76,15 +76,15 @@
             )
         )
         store.add_indexes(table, schema, early_not_null_possible=True)
 
     @classmethod
     def retrieve(
         cls, store, table, stage_name, as_type: type[sa.Table]
-    ) -> sa.sql.selectable.Selectable:
+    ) -> sa.sql.expression.Selectable:
         schema = store.get_schema(stage_name).get()
         table_name, schema = store.resolve_alias(table.name, schema)
         alias_name = TaskContext.get().name_disambiguator.get_name(table_name)
 
         for retry_iteration in range(4):
             # retry operation since it might have been terminated as a deadlock victim
             try:
@@ -97,15 +97,15 @@
             except (sa.exc.SQLAlchemyError, sa.exc.DBAPIError):
                 if retry_iteration == 3:
                     raise
                 time.sleep(retry_iteration * retry_iteration * 1.2)
 
     @classmethod
     def lazy_query_str(cls, store, obj) -> str:
-        if isinstance(obj, sa.sql.selectable.FromClause):
+        if isinstance(obj, sa.sql.expression.FromClause):
             query = sa.select("*").select_from(obj)
         else:
             query = obj
         query_str = str(
             query.compile(store.engine, compile_kwargs={"literal_binds": True})
         )
         # hacky way to canonicalize query (despite __tmp/__even/__odd suffixes
@@ -113,25 +113,64 @@
         query_str = re.sub(r'["\[\]]', "", query_str)
         query_str = re.sub(
             r'(__tmp|__even|__odd)(?=[ \t\n.;"]|$)', "", query_str.lower()
         )
         return query_str
 
 
+@SQLTableStore.register_table()
+class TableReferenceHook(TableHook[SQLTableStore]):
+    @classmethod
+    def can_materialize(cls, type_) -> bool:
+        return issubclass(type_, TableReference)
+
+    @classmethod
+    def can_retrieve(cls, type_) -> bool:
+        return False
+
+    @classmethod
+    def materialize(
+        cls,
+        store: SQLTableStore,
+        table: Table,
+        stage_name,
+        task_info: TaskInfo | None,
+    ):
+        # For a table reference, we don't need to materialize anything.
+        # This is any table referenced by a table reference should already exist
+        # in the schema.
+        # Instead, we check that the table actually exists.
+        schema = store.get_schema(stage_name).get()
+
+        inspector = sa.inspect(store.engine)
+        has_table = inspector.has_table(table.name, schema)
+
+        if not has_table:
+            raise ValueError(
+                f"Not table with name '{table.name}' found in schema '{schema}' "
+                "(reference by TableReference)."
+            )
+
+        return
+
+    @classmethod
+    def retrieve(cls, *args, **kwargs):
+        raise RuntimeError("This should never get called.")
+
+
 # endregion
 
 # region PANDAS
 
 
 @SQLTableStore.register_table(pd)
 class PandasTableHook(TableHook[SQLTableStore]):
     """
     Allows overriding the default dtype backend to use by setting the `dtype_backend`
-    argument in the `hook_args` section of the table store config:
-    ::
+    argument in the `hook_args` section of the table store config::
 
         hook_args:
           pandas:
             dtype_backend: "arrow" | "numpy"
     """
 
     pd_version = Version(pd.__version__)
@@ -414,17 +453,20 @@
         table: Table,
         stage_name: str,
         as_type: type[polars.dataframe.DataFrame],
     ) -> polars.dataframe.DataFrame:
         schema = store.get_schema(stage_name).get()
         table_name, schema = store.resolve_alias(table.name, schema)
         connection_uri = store.engine_url.render_as_string(hide_password=False)
-        df = polars.read_database(
-            f'SELECT * FROM {schema}."{table_name}"', connection_uri
-        )
+
+        preparer = store.engine.dialect.identifier_preparer
+        q_table = preparer.quote(table_name)
+        q_schema = preparer.format_schema(schema)
+
+        df = polars.read_database(f"SELECT * FROM {q_schema}.{q_table}", connection_uri)
         return df
 
     @classmethod
     def auto_table(cls, obj: polars.dataframe.DataFrame):
         # currently, we don't know how to store a table name inside polars dataframe
         return super().auto_table(obj)
```

### Comparing `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/sql/reflection.py` & `pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/backend/table/sql/reflection.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/sql/sql.py` & `pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/backend/table/sql/sql.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,14 +46,106 @@
 class SQLTableStore(BaseTableStore):
     """Table store that materializes tables to a SQL database
 
     Uses schema swapping for transactions:
     Creates a schema for each stage and a temporary schema for each
     transaction. If all tasks inside a stage succeed, swaps the schemas by
     renaming them.
+
+    The correct dialect specific subclass of ``SQLTableStore`` gets initialized when
+    based on the dialect found in the provided engine url during initialization.
+
+    .. rubric:: Supported Tables
+
+    The `SQLTableStore` can materialize (that is, store task output)
+    and dematerialize (that is, retrieve task input) the following Table types:
+
+    .. list-table::
+       :widths: 30, 30, 30
+       :header-rows: 1
+       :stub-columns: 1
+
+       * - Framework
+         - Materialization
+         - Dematerialization
+
+       * - SQLAlchemy
+         - | :py:class:`sa.sql.expression.Selectable
+                        <sqlalchemy.sql.expression.Selectable>`
+           | :py:class:`sa.sql.expression.TextClause
+                        <sqlalchemy.sql.expression.TextClause>`
+         - :py:class:`sa.Table <sqlalchemy.schema.Table>`
+
+       * - Pandas
+         - :py:class:`pd.DataFrame <pandas.DataFrame>`
+         - :py:class:`pd.DataFrame <pandas.DataFrame>`
+
+       * - Polars
+         - :external+pl:doc:`pl.DataFrame <reference/dataframe/index>`
+         - :external+pl:doc:`pl.DataFrame <reference/dataframe/index>`
+
+       * - tidypolars
+         - :py:class:`tp.Tibble <tidypolars.tibble.Tibble>`
+         - :py:class:`tp.Tibble <tidypolars.tibble.Tibble>`
+
+       * - Ibis
+         - :py:class:`ibis.api.Table <ibis.expr.types.relations.Table>`
+         - :py:class:`ibis.api.Table <ibis.expr.types.relations.Table>`
+
+       * - pydiverse.transform
+         - ``pdt.Table``
+         - | ``pdt.eager.PandasTableImpl``
+           | ``pdt.lazy.SQLTableImpl``
+
+       * - pydiverse.pipedag
+         - | :py:class:`~.TableReference`
+         -
+
+
+    :param url:
+        The :external+sa:ref:`SQLAlchemy engine url <database_urls>`
+        use to connect to the database.
+
+        This URL may contain placeholders like ``{name}`` or ``{instance_id}``
+        (additional ones can be defined in the ``url_attrs_file``) or
+        environment variables like ``{$USER}`` which get substituted with their
+        respective values.
+
+    :param url_attrs_file:
+        Filename of a yaml file which is read shortly before rendering the final
+        engine URL and which is used to replace custom placeholders in ``url``.
+
+        Just like ``url``, this value may also contain placeholders and environment
+        variables which get substituted.
+
+    :param create_database_if_not_exists:
+        If the engine url references a database name that doesn't yet exists,
+        then setting this value to ``True`` tells pipedag to create the database
+        before trying to open a connection to it.
+
+    :param schema_prefix:
+        A prefix that gets placed in front of all schema names created by pipedag.
+
+    :param schema_suffix:
+        A suffix that gets placed behind of all schema names created by pipedag.
+
+    :param avoid_drop_create_schema:
+        If ``True``, no ``CREATE SCHEMA`` or ``DROP SCHEMA`` statements get issued.
+        This is mostly relevant for databases that support automatic schema
+        creation like IBM DB2.
+
+    :param print_materialize:
+        If ``True``, all tables that get materialized get logged.
+
+    :param print_sql:
+        If ``True``, all executed SQL statements get logged.
+
+    :param no_db_locking:
+        Speed up database by telling it we will not rely on it's locking mechanisms.
+        Currently not implemented.
     """
 
     METADATA_SCHEMA = "pipedag_metadata"
     LOCK_SCHEMA = "pipedag_locks"
 
     __registered_dialects: dict[str, type[SQLTableStore]] = {}
     _dialect_name: str
@@ -82,34 +174,14 @@
         schema_prefix: str = "",
         schema_suffix: str = "",
         avoid_drop_create_schema: bool = False,
         print_materialize: bool = False,
         print_sql: bool = False,
         no_db_locking: bool = True,
     ):
-        """
-        Construct table store.
-
-        :param engine_url:
-            URL for SQLAlchemy engine
-        :param create_database_if_not_exists:
-            whether to create database if it does not exist
-        :param schema_prefix:
-            prefix string for schemas
-        :param schema_suffix:
-            suffix string for schemas
-        :param avoid_drop_create_schema
-            avoid creating and dropping schemas
-        :param print_materialize:
-            whether to print select statements before materialization
-        :param print_sql:
-            whether to print final SQL statements (except for metadata)
-        :param no_db_locking:
-            speed up database by telling it we will not rely on it's locking mechanisms
-        """
         super().__init__()
 
         self.create_database_if_not_exists = create_database_if_not_exists
         self.schema_prefix = schema_prefix
         self.schema_suffix = schema_suffix
         self.avoid_drop_create_schema = avoid_drop_create_schema
         self.print_materialize = print_materialize
@@ -387,14 +459,18 @@
     @staticmethod
     def format_sql_string(query_str: str) -> str:
         return textwrap.dedent(query_str).strip()
 
     def execute_raw_sql(self, raw_sql: RawSql):
         """Executed raw SQL statements in the associated transaction stage"""
         for statement in raw_sql.sql.split(";"):
+            if not statement.strip():
+                # Skip empty queries
+                continue
+
             self.execute(statement)
 
     def setup(self):
         super().setup()
         if not self.avoid_drop_create_schema:
             self.execute(CreateSchema(self.metadata_schema, if_not_exists=True))
         with self.engine_connect() as conn:
@@ -1065,40 +1141,96 @@
     def resolve_alias(self, table: str, schema: str) -> tuple[str, str]:
         return table, schema
 
     def get_objects_in_stage(self, stage: Stage):
         schema = self.get_schema(stage.transaction_name)
         return list(self._get_all_objects_in_schema(schema).keys())
 
+    def get_table_objects_in_stage(self, stage: Stage):
+        schema = self.get_schema(stage.current_name).get()
+        inspector = sa.inspect(self.engine)
+
+        tables = inspector.get_table_names(schema)
+        views = inspector.get_view_names(schema)
+        return [*tables, *views]
+
     def get_stage_hash(self, stage: Stage) -> str:
         """Compute hash that represents entire stage's output metadata."""
         # We only need to look in tasks_table since the output_json column is updated
         # after evaluating lazy output objects for cache validity. This is the same
         # information we use for producing input_hash of downstream tasks.
         if self.disable_caching:
             raise NotImplementedError(
                 "computing stage hash with disabled caching is currently not supported"
             )
         with self.engine_connect() as conn:
             result = conn.execute(
                 sa.select(self.tasks_table.c.output_json)
                 .where(self.tasks_table.c.stage == stage.name)
                 .where(self.tasks_table.c.in_transaction_schema.in_([False]))
-                .order_by(self.tasks_table.c.output_json)
-            ).all()
-            result = [row[0] for row in result]
+            ).scalars()
+
+        result = sorted(result)
         return stable_hash(*result)
 
     # DatabaseLockManager
 
     def get_engine_for_locking(self) -> sa.Engine:
         return self._create_engine()
 
     def get_lock_schema(self) -> Schema:
         return self.get_schema(self.LOCK_SCHEMA)
 
 
+class TableReference:
+    """Reference to a user-created table.
+
+    By returning a `TableReference` wrapped in a :py:class:`~.Table` from a task,
+    you can tell pipedag that you yourself created a new table inside
+    the correct schema of the table store.
+    This may be useful if you need to perform a complex load operation to create
+    a table (e.g. load a table from an Oracle database into Postgres
+    using `oracle_fdw`).
+
+    Only supported by :py:class:`~.SQLTableStore`.
+
+    Warning
+    -------
+    Using table references is not recommended unless you know what you are doing.
+    It may lead unexpected behaviour.
+    It also requires accessing non-public parts of the pipedag API which can
+    change without notice.
+
+    Example
+    -------
+    Making sure that the table is created in the correct schema is not trivial,
+    because the schema names usually are different from the stage names.
+    To get the correct schema name, you must use undocumented and non-public
+    parts of the pipedag API. To help you get started, we'll provide you with
+    this example, however, be warned that this might break without notice::
+
+        @materialize(version="1.0")
+        def task():
+            from pydiverse.pipedag.context import ConfigContext, TaskContext
+
+            table_store = ConfigContext.get().store.table_store
+            task = TaskContext.get().task
+
+            # Name of the schema in which you must create the table
+            schema_name = table_store.get_schema(task.stage.transaction_name).get()
+
+            # Use the table store's engine to create a table in the correct schema
+            with table_store.engine.begin() as conn:
+                conn.execute(...)
+
+            # Return a reference to the newly created table
+            return Table(TableReference(), "name_of_table")
+    """
+
+    pass
+
+
 # Load SQLTableStore Hooks
 import pydiverse.pipedag.backend.table.sql.hooks  # noqa
 
 # Load SQLTableStore dialect specific subclasses
 import pydiverse.pipedag.backend.table.sql.dialects  # noqa
```

### Comparing `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/backend/table/util/dtype.py` & `pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/backend/table/util/dtype.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/context/context.py` & `pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/context/context.py`

 * *Files 14% similar despite different names*

```diff
@@ -42,21 +42,25 @@
         with self._lock:
             object.__setattr__(self, "_enter_counter", self._enter_counter - 1)
             if self._enter_counter == 0:
                 if not self._token:
                     raise RuntimeError
                 self._context_var.reset(self._token)
                 object.__setattr__(self, "_token", None)
-                self.close()
+                self._close()
 
-    def close(self):
+    def _close(self):
         """Function that gets called at __exit__"""
 
     @classmethod
     def get(cls: type[T]) -> T:
+        """Returns the current, innermost context instance.
+
+        :raises LookupError: If no such context has been entered yet.
+        """
         return cls._context_var.get()
 
     def __getstate__(self):
         state = self.__dict__.copy()
         del state["_token"]
         del state["_enter_counter"]
         return state
@@ -95,27 +99,49 @@
 class StageCommitTechnique(Enum):
     SCHEMA_SWAP = 0
     READ_VIEWS = 1
 
 
 @frozen(slots=False)
 class ConfigContext(BaseAttrsContext):
-    """
-    Configuration context for running a particular pipedag instance.
+    """Configuration context for running a particular pipedag instance.
+
+    To create a `ConfigContext` instance use :py:meth:`PipedagConfig.get`.
+
+    ..
+        For the most part, the Config context holds serializable config attributes.
+        But it also offers access to the table and blob store, as well as the lock
+        manager and orchestration engine.
+
+        Because we can't pickle those classes (and pipedag supports flow execution
+        across multiple processes / nodes), the lock manager and orchestration engine
+        only get created once per flow execution and then get managed by a central
+        process (in the case of the lock manager this is the RunContextServer).
+
+        The table and blob store on the other hand need to be accessed by many task
+        across multiple threads / processes / nodes. Because they don't contain
+        any state (all state gets stored in the RunContextServer), they get
+        thrown away during pickling and then get recreated on the first access.
+
+    Attributes
+    ----------
+    pipedag_name :
+        :ref:`Name <config-name>` of the config file.
+    flow_name :
+        Name of the flow used for instantiating this config.
+    instance_name :
+        Name of the instance used for instantiating this config.
+    instance_id :
+        The :ref:`instance_id`.
+    attrs :
+        Values from the :ref:`config-attrs` config section, stored in a |Box|_ object.
+        Useful for passing any custom, use case specific config options to your flow.
 
-    For the most part it holds serializable attributes. But it also offers access
-    to blob_store and table_store as well as lock manager and orchestration engine.
-    Lock manager and orchestration engine are managed full cycle by exactly one
-    caller (ServerRunContext / Flow.run()). So this class just offers a way to create
-    a disposable object. Blob_store and table_store on the other hand might be
-    accessed by multi-threaded / multi-processed / multi-node way of orchestrating
-    functions in the pipedag. Since they don't keep real state, they can be
-    thrown away while pickling and will be reloaded on first access of the
-    @cached_property store. Calling ConfigContext.dispose() will close all
-    connections and render this object unusable afterwards.
+        .. |Box| replace:: ``Box``
+        .. _Box: https://github.com/cdgriffith/Box/wiki
     """
 
     _config_dict: dict
 
     # names
     pipedag_name: str
     flow_name: str | None
@@ -181,15 +207,24 @@
         return PipeDAGStore(
             table=table_store,
             blob=blob_store,
             local_table_cache=local_table_cache,
         )
 
     def evolve(self, **changes) -> ConfigContext:
-        """Create a new instance with the changes applied; Wrapper for attrs.evolve"""
+        """Create a new config context instance with the changes applied.
+
+        Because ConfigContext is immutable, this is the only valid way to derive a
+        new instance with some values mutated.
+
+        Wrapper around |attrs.evolve()|_.
+
+        .. |attrs.evolve()| replace:: ``attrs.evolve()``
+        .. _attrs.evolve(): https://www.attrs.org/en/stable/api.html#attrs.evolve
+        """
         evolved = evolve(self, **changes)
 
         # Transfer cached properties
         cached_properties = ["auto_table", "auto_blob", "store"]
         for name in cached_properties:
             if name in self.__dict__:
                 evolved.__dict__[name] = self.__dict__[name]
@@ -199,15 +234,15 @@
 
     def create_lock_manager(self) -> BaseLockManager:
         return load_object(self._config_dict["lock_manager"])
 
     def create_orchestration_engine(self) -> OrchestrationEngine:
         return load_object(self._config_dict["orchestration"])
 
-    def close(self):
+    def _close(self):
         # If the store has been initialized (and thus cached in the __dict__),
         # dispose of it, and remove it from the cache.
         if store := self.__dict__.get("store", None):
             if not self.__dict__.get("__store_inherited", False):
                 store.dispose()
                 self.__dict__.pop("store")
 
@@ -221,23 +256,41 @@
         return state
 
     _context_var = ContextVar("config_context")
 
 
 class StageLockContext(BaseContext):
     """
-    Context manager used to keep stages locked until after flow.run() has been called
+    Context manager used to keep stages locked until after :py:meth:`Flow.run()`.
+
+    By default, pipedag releases stage locks as soon as it is done processing a stage.
+    This means that by the time the flow has finished running, another flow
+    run might already have overwritten any data in those stages.
+    Consequently, calling :py:meth:`Result.get()` might not return the values
+    produced by the current run, but instead those from the other (newer) run.
+
+    To prevent this, you can wrap the calls to :py:meth:`Flow.run()` and
+    :py:meth:`Result.get()` in a `StageLockContext`. This keeps all stages modified
+    by the flow to remain locked until the end of `StageLockContext`.
+
+    Example
+    -------
+    ::
+
+        with StageLockContext():
+            result = flow.run()
+            df = result.get(task_x)
     """
 
     lock_state_handlers: [StageLockStateHandler]
 
     _context_var = ContextVar("stage_lock_context")
 
     def __init__(self):
         self.logger = structlog.get_logger(logger_name=type(self).__name__, id=id(self))
         self.logger.info("Open stage lock context")
         self.lock_state_handlers = []
 
-    def close(self):
+    def _close(self):
         self.logger.info("Close stage lock context")
         for lock_state_handler in self.lock_state_handlers:
             lock_state_handler.dispose()
```

### Comparing `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/context/run_context.py` & `pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/context/run_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,30 +10,32 @@
 from concurrent.futures import Future, ThreadPoolExecutor
 from contextlib import contextmanager
 from contextvars import ContextVar
 from enum import Enum
 from threading import Lock, RLock
 from typing import TYPE_CHECKING, Any
 
+import attrs
 import msgpack
 import structlog
 
 from pydiverse.pipedag.context.context import (
+    BaseAttrsContext,
     BaseContext,
     ConfigContext,
     StageLockContext,
 )
 from pydiverse.pipedag.errors import LockError, RemoteProcessError, StageError
 from pydiverse.pipedag.util import Disposable
 from pydiverse.pipedag.util.ipc import IPCServer
 
 if TYPE_CHECKING:
     from pydiverse.pipedag._typing import T
     from pydiverse.pipedag.backend import BaseLockManager, LockState
-    from pydiverse.pipedag.core import Stage, Subflow, Task
+    from pydiverse.pipedag.core import Flow, Stage, Subflow, Task
     from pydiverse.pipedag.materialize import Blob, Table
 
 
 def synchronized(lock_attr: str):
     def decorator(func: T) -> T:
         @functools.wraps(func)
         def synced_func(self, *args, **kwargs):
@@ -632,26 +634,29 @@
             "remove_names",
             stage.id,
             [t.name for t in tables],
             [b.name for b in blobs],
         )
 
 
-class DematerializeRunContext(BaseContext):
+@attrs.frozen
+class DematerializeRunContext(BaseAttrsContext):
     """Dummy RunContext that returns `COMMITTED` as the stage state for all stages
 
     To dematerialize an object we must know it the associates state has been
     committed or not. This context replaces the RunContext created by
     RunContextServer during the execution of a flow with one that only sets the
     state of each state to `COMMITTED`. This allows us to dematerialize the
     objects that have been stored after a flow has finished running.
     """
 
     _context_var = RunContext._context_var
 
+    flow: Flow
+
     def get_stage_state(self, stage: Stage) -> StageState:
         return StageState.COMMITTED
 
     def validate_stage_lock(self, stage: Stage):
         pass
```

### Comparing `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/core/config.py` & `pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/core/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,33 @@
     def __get__(self, instance, cls):
         if not hasattr(self, "cache"):
             self.cache = self.func(cls)
         return self.cache
 
 
 class PipedagConfig:
+    """
+    This class represents a :doc:`pipedag config file </reference/config>`.
+
+    :param path: Path to the config file to load.
+
+    Attributes
+    ----------
+    default : PipedagConfig
+        The default config file.
+
+        If the environment variable :envvar:`PIPEDAG_CONFIG` is set, then this file
+        will be used as the config file. Otherwise, pipedag searches for a file called
+        ``pipedag.yaml`` or ``pipedag.yml`` in:
+
+        * The current working directory
+        * Any parent directories of the working directory
+        * The user folder
+    """
+
     default: PipedagConfig
 
     def __init__(self, path: str):
         self.path = path
         with open(path) as f:
             self.raw_config = yaml.safe_load(f)
 
@@ -85,14 +104,29 @@
 
     def get(
         self,
         instance: str | None = None,
         flow: str | None = None,
         per_user: bool = False,
     ) -> ConfigContext:
+        """
+        Constructs a :py:class:`ConfigContext`.
+        For more details how the specific ConfigContext instance is constructed,
+        check out the :ref:`specifying instances and flows
+        <reference/config:Specifying instances and flows>` section.
+
+        :param instance: Name of the instance.
+            If no value is provided the ``__any__`` instance gets used.
+        :param flow: Name of the flow.
+            If no value is provided the ``__any__`` flow gets used.
+        :param per_user:
+            Whether to customize the instance id for each user according to
+            :ref:`per_user_template`.
+        """
+
         # TODO: Check that this function only gets called in the main interpreter.
         #       Otherwise certain environment variables might get expanded incorrectly.
         from pydiverse.pipedag.context import ConfigContext
 
         config = self.__get_merged_config_dict(
             instance=instance,
             flow=flow,
@@ -262,15 +296,15 @@
         # TODO: Decide on a list of available variables
         variables = {
             "username": getpass.getuser(),
             "instance_id": config.get("instance_id"),
             "name": self.name,
         }
 
-        for key, val in variables.items():
+        for key, val in list(variables.items()):
             if val is None:
                 variables.pop(key)
 
         for location in locations:
             value: str = _get(config, location, default=None)
             if value is None:
                 continue
@@ -323,15 +357,15 @@
             Path("~").expanduser(),
         ]
     else:
         search_paths = [Path(path) for path in search_paths]
 
     file_names = [name + extension for extension in extensions]
     for path, file_name in itertools.product(search_paths, file_names):
-        config_path = (path / file_name).resolve()
+        config_path: Path = (path / file_name).resolve()
         if config_path.is_file():
             return str(config_path)
 
     raise FileNotFoundError("No config file found")
 
 
 def expand_environment_variables(string: str) -> str:
```

### Comparing `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/core/flow.py` & `pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/core/flow.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,14 +21,43 @@
     from pydiverse.pipedag.core import Result, Stage, Task
     from pydiverse.pipedag.core.stage import CommitStageTask
     from pydiverse.pipedag.core.task import TaskGetItem
     from pydiverse.pipedag.engine import OrchestrationEngine
 
 
 class Flow:
+    """
+    A flow represents a collection of dependent Tasks.
+
+    A flow is defined by using it as a context manager.
+    Any stages and tasks defined inside the flow context will automatically get added
+    to the flow with the correct dependency wiring.
+
+    :param name: The name of the flow.
+
+    Examples
+    --------
+    ::
+
+        @materialize
+        def my_materializing_task():
+            return Table(...)
+
+        with Flow("my_flow") as flow:
+            with Stage("stage_1") as stage_1:
+                task_1 = my_materializing_task()
+                task_2 = another_materializing_task(task_1)
+
+            with Stage("stage_2") as stage_2:
+                task_3 = yet_another_task(task_3)
+                ...
+
+        result = flow.run()
+    """
+
     def __init__(
         self,
         name: str = "default",
     ):
         self.name = name
 
         self.logger = structlog.get_logger(logger_name=type(self).__name__)
@@ -56,14 +85,25 @@
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self._ctx.__exit__()
         del self._ctx
 
         self.explicit_graph = self.build_graph()
 
+    def __getitem__(self, name) -> Stage:
+        """Retrieves a stage by name.
+
+        :param name: The name of the stage.
+        :raises KeyError: if no stage with the specified name exists.
+        """
+
+        if stage := self.stages.get(name):
+            return stage
+        raise KeyError(f"Couldn't find a stage with name '{name}' in flow.")
+
     def add_stage(self, stage: Stage):
         if stage.name in self.stages:
             raise DuplicateNameError(f"Stage with name '{stage.name}' already exists.")
 
         stage.id = len(self.stages)
         self.stages[stage.name] = stage
 
@@ -83,34 +123,14 @@
         if to not in self.graph:
             raise FlowError(
                 f"Can't add edge from {from_} to {to} because `to` is not in the flow."
             )
 
         self.graph.add_edge(from_, to)
 
-    def visualize(self, result: Result | None = None):
-        dot = self.visualize_pydot(result)
-        _display_pydot(dot)
-        return dot
-
-    def visualize_url(self, result: Result | None = None) -> str:
-        dot = self.visualize_pydot(result)
-        return _pydot_url(dot)
-
-    def visualize_pydot(self, result: Result | None = None) -> pydot.Dot:
-        task_style = _generate_task_style(self.tasks, result)
-        dot = _build_pydot(
-            stages=list(self.stages.values()),
-            tasks=self.tasks,
-            graph=self.graph,
-            task_style=task_style,
-        )
-
-        return dot
-
     def build_graph(self) -> nx.DiGraph:
         if not nx.is_directed_acyclic_graph(self.graph):
             raise FlowError("Graph is not a DAG")
 
         explicit_graph = self.graph.copy()
         stages = self.stages.values()
 
@@ -188,47 +208,79 @@
         *components: Task | TaskGetItem | Stage,
         config: ConfigContext = None,
         orchestration_engine: OrchestrationEngine = None,
         fail_fast: bool | None = None,
         ignore_fresh_input: bool = False,
         **kwargs,
     ) -> Result:
-        """Execute a flow
-
-        You can provide an engine to execute the flow with using the `engine`
-        keyword. If no engine is provided, the engine specified in the config
-        file is used.
+        """Execute the flow.
+        This will execute the flow and all tasks within using the orchestration engine.
 
         :param components: An optional selection of tasks or stages that should
-            get executed. If no value is provided, all tasks and stages get executed.
+            get executed. If no values are provided, all tasks and stages get executed.
+
             If you specify a subset of tasks, those tasks get executed even when
             they are cache valid, and they don't get committed.
+
             If you specify a subset of stages, all tasks and substages of those stages
             get executed and committed.
-        :param config: A configuration context with information about
-            the pipe-DAG instance.
-        :param orchestration_engine: The orchestration engine to use.
-        :param fail_fast: True means that errors should be raised as exceptions
-            out of this function.
-        :param ignore_fresh_input: whether cache functions should be disabled that
-            check for fresh input into pipe-DAG
-        :param kwargs: Other keyword arguments. They get passed on directly to the
-            orchestration engine's `.run` method and thus are engine dependant.
+        :param config:
+            A :py:class:`ConfigContext` to use as the configuration for executing
+            this flow. If no config is provided, then pipedag uses the
+            current innermost open ConfigContext, or if no such config exists,
+            it gets the default config from :py:attr:`PipedagConfig.default`.
+        :param orchestration_engine:
+            The orchestration engine to use. If no engine is provided, the
+            orchestration engine from the config gets used.
+        :param fail_fast:
+            Whether exceptions should get raised or swallowed.
+            If set to True, exceptions that occur get immediately raised and the
+            flow gets aborted.
+        :param ignore_fresh_input:
+            When set to True, the task's cache function gets ignored when determining
+            the cache validity of a task.
+        :param kwargs:
+            Other keyword arguments that get passed on directly to the
+            ``run()`` method of the orchestration engine. Consequently, these
+            keyword arguments are engine dependant.
         :return:
-            Result object that gives information whether run was successful
+            A :py:class:`Result` object for the current flow run.
+
+        Examples
+        --------
+        .. code-block:: python
+
+            with Flow() as flow:
+                with Stage("stage_1") as stage_1:
+                    task_1 = ...
+                    task_2 = ...
+
+                with Stage("stage_2") as stage_2:
+                    task_3 = ...
+                    task_4 = ...
+
+            # Execute the entire flow
+            flow.run()
+
+            # Execute (and commit) only stage 1
+            flow.run(stage_1)
+
+            # Execute (but DON'T commit) only task 1 and task 4
+            flow.run(task_1, task_4)
+
         """
 
         subflow = self.get_subflow(*components)
 
         # Get the ConfigContext to use
         if config is None:
             try:
                 config = ConfigContext.get()
             except LookupError:
-                config = PipedagConfig.default.get()
+                config = PipedagConfig.default.get(flow=self.name)
 
         # Evolve config using the arguments passed to flow.run
         config = config.evolve(
             fail_fast=(fail_fast if fail_fast is not None else config.fail_fast),
             ignore_fresh_input=ignore_fresh_input,
             ignore_task_version=(
                 # If subflow consists of a subset of tasks (-> not a subset of stages)
@@ -248,14 +300,77 @@
         self.logger.info("Flow visualization", url=visualization_url)
 
         if not result.successful and config.fail_fast:
             raise result.exception or Exception("Flow run failed")
 
         return result
 
+    def get_stage(self, name: str) -> Stage:
+        """Retrieves a stage by name.
+        Alias for :py:meth:`Flow.__getitem__`.
+
+        :param name: The name of the stage.
+        :return: The stage.
+        :raises KeyError: if no stage with the specified name exists.
+        """
+
+        return self[name]
+
+    # Visualization
+    def visualize(self, result: Result | None = None):
+        """Visualizes the flow as a graph.
+
+        If you are running in a jupyter notebook, the graph will get displayed inline.
+        Otherwise, it will get rendered to a pdf that then gets opened in your browser.
+
+        Requires `Graphviz <https://graphviz.org>`_ to be installed on your computer.
+
+        :param result: An optional :py:class:`Result` instance.
+            If provided, the visualization will contain additional information such
+            as which tasks ran successfully, or failed.
+        """
+        dot = self.visualize_pydot(result)
+        _display_pydot(dot)
+        return dot
+
+    def visualize_url(self, result: Result | None = None) -> str:
+        """Visualizes the flow as a graph and returns a URL to view the visualization.
+
+        If you don't have Graphviz installed on your computer (and thus aren't able to
+        use the :py:meth:`~.visualize()` method) then this is the easiest way to
+        visualize the flow.
+        For this we use a free service called `Kroki <https://kroki.io>`_.
+
+        :param result: An optional :py:class:`Result` instance.
+            If provided, the visualization will contain additional information such
+            as which tasks ran successfully, or failed.
+        :return:
+            A URL that, when opened, displays the graph.
+        """
+        dot = self.visualize_pydot(result)
+        return _pydot_url(dot)
+
+    def visualize_pydot(self, result: Result | None = None) -> pydot.Dot:
+        """Visualizes the flow as a graph and return a ``pydot.Dot`` graph.
+
+        :param result: An optional :py:class:`Result` instance.
+            If provided, the visualization will contain additional information such
+            as which tasks ran successfully, or failed.
+        :return: A ``pydot.Dot`` graph.
+        """
+        task_style = _generate_task_style(self.tasks, result)
+        dot = _build_pydot(
+            stages=list(self.stages.values()),
+            tasks=self.tasks,
+            graph=self.graph,
+            task_style=task_style,
+        )
+
+        return dot
+
 
 class Subflow:
     def __init__(self, flow: Flow, tasks: list[Task], stages: list[Stage]):
         self.flow = flow
         self.name = flow.name
         self.is_tasks_subflow = len(tasks) > 0
```

### Comparing `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/core/result.py` & `pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/core/result.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,24 +5,45 @@
 import structlog
 from attrs import frozen
 
 from pydiverse.pipedag.context import ConfigContext, StageLockContext
 from pydiverse.pipedag.context.run_context import DematerializeRunContext, RunContext
 from pydiverse.pipedag.core.task import Task, TaskGetItem
 from pydiverse.pipedag.errors import LockError
-from pydiverse.pipedag.materialize.core import MaterializingTask
-from pydiverse.pipedag.util import deep_map
 
 if TYPE_CHECKING:
+    import pydot
+
     from pydiverse.pipedag.context.run_context import FinalTaskState
     from pydiverse.pipedag.core import Flow, Subflow
 
 
 @frozen
 class Result:
+    """
+    Flow execution result.
+
+    Attributes
+    ----------
+    flow :
+        The flow that produced this result
+    underlying :
+        The underlying result object returned by the orchestration engine.
+        Depending on the engine, this object might have a different type.
+    successful :
+        Whether the flow execution was successful or not.
+    task_values :
+        A dictionary mapping from tasks to the values returned by them.
+    task_states :
+        A dictionary mapping from tasks to their final states.
+    exception :
+        If an exception was raised during execution, it will get stored in
+        this attribute.
+    """
+
     flow: Flow
     subflow: Subflow
 
     underlying: Any
     successful: bool
     config_context: ConfigContext | None
 
@@ -47,60 +68,65 @@
             config_context=ConfigContext.get(),
             task_values=task_values,
             task_states=RunContext.get().get_task_states(),
             exception=exception,
         )
 
     def get(self, task: Task | TaskGetItem, as_type: type = None) -> Any:
-        """Load the results of a task from the database.
+        """Retrieve the output produced by a task.
+
+        Any tables and blobs returned by a task get loaded from their
+        corresponding store.
+
+        If :ref:`strict_result_get_locking` is set to True, this call, as well as
+        as :py:meth:`Flow.run()` must be wrapped inside a :py:class:`StageLockContext`.
 
-        :param task: The task
+        :param task: The task for which you want to retrieve the output.
         :param as_type: The type as which tables produced by this task should
             be dematerialized. If no type is specified, the input type of
             the task is used.
         :return: The results of the task.
         """
+        from pydiverse.pipedag.materialize.store import dematerialize_output_from_store
+
         if not self.successful:
             logger = structlog.get_logger(logger_name=type(self).__name__)
             logger.warning(
                 "Attention: getting tables from unsuccessful run is unreliable!"
             )
 
-        if isinstance(task, Task):
-            root_task = task
-        else:
-            root_task = task.task
-
-        if as_type is None:
-            assert isinstance(root_task, MaterializingTask)
-            as_type = root_task.input_type
-
         if self.config_context.strict_result_get_locking:
             try:
                 StageLockContext.get()
             except LookupError:
                 raise LockError(
                     "Called Result.get() without opening StageLockContext. Consider"
                     " using 'strict_result_get_locking: false' for interactive"
                     " debugging"
                 ) from None
 
-        # TODO: Check that the results loaded from the database correspond
-        #       to the run_id of this result object.
-        with self.config_context as config_ctx, DematerializeRunContext() as run_ctx:
-
-            def dematerialize_mapper(item):
-                return config_ctx.store.dematerialize_item(
-                    item, as_type=as_type, ctx=run_ctx
-                )
+        if isinstance(task, Task):
+            task_output = self.task_values[task]
+        else:
+            task_output = self.task_values[task.task]
 
-            task_value = self.task_values[root_task]
-            return deep_map(task.resolve_value(task_value), dematerialize_mapper)
+        with self.config_context, DematerializeRunContext(self.flow):
+            store = self.config_context.store
+            return dematerialize_output_from_store(store, task, task_output, as_type)
 
     def visualize(self):
+        """
+        Wrapper for :py:meth:`Flow.visualize()`.
+        """
         return self.subflow.visualize(result=self)
 
-    def visualize_url(self):
+    def visualize_url(self) -> str:
+        """
+        Wrapper for :py:meth:`Flow.visualize_url()`.
+        """
         return self.subflow.visualize_url(result=self)
 
-    def visualize_pydot(self):
+    def visualize_pydot(self) -> pydot.Dot:
+        """
+        Wrapper for :py:meth:`Flow.visualize_pydot()`.
+        """
         return self.subflow.visualize_pydot(result=self)
```

### Comparing `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/core/stage.py` & `pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/core/stage.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,61 +1,45 @@
 from __future__ import annotations
 
+import inspect
 from typing import TYPE_CHECKING
 
 import structlog
 
 from pydiverse.pipedag.context import ConfigContext, DAGContext
 from pydiverse.pipedag.core.task import Task
 from pydiverse.pipedag.errors import StageError
 from pydiverse.pipedag.util import normalize_name
 
 if TYPE_CHECKING:
     from pydiverse.pipedag.core.flow import Flow
 
 
 class Stage:
-    """The Stage class is used to group a collection of related tasks
+    """A stage represents a collection of related tasks.
 
     The main purpose of a Stage is to allow for a transactionality mechanism.
     Only if all tasks inside a stage finish successfully does the stage
     get committed.
 
     All task that get defined inside the stage's context will automatically
     get added to the stage.
 
-    An example of how to use a Stage:
-    ::
-
-        @materialize()
-        def my_materializing_task():
-            return Table(...)
-
-        with Flow("my_flow") as flow:
-            with Stage("stage_1") as stage_1:
-                task_1 = my_materializing_task()
-                task_2 = another_materializing_task(task_1)
-
-            with Stage("stage_2") as stage_2:
-                task_3 = yet_another_task(task_3)
-                ...
-
-        flow.run()
-
-    To ensure that all tasks get executed in the correct order, each
-    MaterializingTask must be an upstream dependency of its stage's
-    CommitStageTask (this is done by calling the `add_task` method) and
-    for each of its upstream dependencies, the associated StageCommitTask
-    must be added as an upstream dependency.
-    This ensures that the stage commit only happens after all tasks have
-    finished writing to the transaction stage, and a task never gets executed
-    before any of its upstream stage dependencies have been committed.
-
     :param name: The name of the stage. Two stages with the same name may
         not be used inside the same flow.
+
+    ..
+        To ensure that all tasks get executed in the correct order, each
+        MaterializingTask must be an upstream dependency of its stage's
+        CommitStageTask (this is done by calling the `add_task` method) and
+        for each of its upstream dependencies, the associated StageCommitTask
+        must be added as an upstream dependency.
+        This ensures that the stage commit only happens after all tasks have
+        finished writing to the transaction stage, and a task never gets executed
+        before any of its upstream stage dependencies have been committed.
     """
 
     def __init__(self, name: str):
         self._name = normalize_name(name)
         self._transaction_name = f"{self._name}__tmp"
 
         self.tasks: list[Task] = []
@@ -65,31 +49,33 @@
         self.logger = structlog.get_logger(logger_name=type(self).__name__, stage=self)
         self.id: int = None  # type: ignore
 
         self._did_enter = False
 
     @property
     def name(self) -> str:
+        """The name of the stage."""
         return self._name
 
     @property
     def transaction_name(self) -> str:
+        """The name temporary transaction stage."""
         return self._transaction_name
 
     def set_transaction_name(self, new_transaction_name):
         # used by stage_commit_technique=READ_VIEWS to change odd/even
         # transaction schemas
         self._transaction_name = new_transaction_name
 
     @property
     def current_name(self) -> str:
-        """The name of the stage where the data currently lives
+        """The name of the stage where the data currently lives.
 
         Before a task has been committed this is the transaction name,
-        after the commit it is the base name.
+        after the commit it is the normal name.
         """
 
         if self.did_commit:
             return self.name
         else:
             return self.transaction_name
 
@@ -98,14 +84,21 @@
         from pydiverse.pipedag.context.run_context import RunContext, StageState
 
         return RunContext.get().get_stage_state(self) == StageState.COMMITTED
 
     def __repr__(self):
         return f"<Stage: {self.name}>"
 
+    def __getstate__(self):
+        state = self.__dict__.copy()
+        state.pop("tasks", None)
+        state.pop("commit_task", None)
+        state.pop("logger", None)
+        return state
+
     def __enter__(self):
         if self._did_enter:
             raise StageError(
                 f"Stage '{self.name}' has already been entered."
                 " Can't reuse the same stage twice."
             )
         self._did_enter = True
@@ -129,58 +122,109 @@
             stage=self,
         )
         self._ctx.__enter__()
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.commit_task = CommitStageTask(self, self._ctx.flow)
-        self._ctx.flow.add_task(self.commit_task)
         self._ctx.__exit__()
         del self._ctx
 
-        if len(self.tasks) == 0:
-            # Empty stage doesn't need to be committed
-            self.commit_task._skip_commit = True
+    def __getitem__(self, item: str | tuple[str, int]) -> Task:
+        """Retrieves a task inside the stage by name.
+
+        You can either subscribe a Stage using just a string (``stage["name"]``) or
+        using a tuple containing a string and an integer (``stage["name", 3]``).
+
+        The string is always interpreted as the name of the task to retrieve. If
+        you also pass in an integer, it is interpreted as the `index` of the task.
+        This means, that if the stage contains multiple tasks with the same name,
+        then you can retrieve a specific instance of that task based on the order
+        in which they were defined.
+
+        :raises KeyError: If no task with the name can be found.
+        :raises IndexError: If the index is out of bounds.
+        :raises ValueError: If multiple matching tasks have been found, but no index
+            has been provided.
+        """
+
+        if isinstance(item, str):
+            name = item
+            index = None
+        elif isinstance(item, tuple):
+            name, index = item
+        else:
+            raise TypeError
+
+        tasks = [task for task in self.tasks if task.name == name]
+        if not tasks:
+            raise KeyError(
+                f"Couldn't find a task with name '{name}' in stage '{self.name}'."
+            )
+
+        if index is None:
+            if len(tasks) == 1:
+                return tasks[0]
+
+            raise ValueError(
+                f"Found more than one task with name '{name}' in stage. "
+                "Specify which task you want by passing in an index."
+            )
+
+        if index < len(tasks):
+            return tasks[index]
+
+        raise IndexError(
+            f"Found only {len(tasks)} instances of task '{name}' in stage, "
+            f"but you requested the tasks with index {index}, "
+            "which is out of bounds."
+        )
 
     def all_tasks(self):
         yield from self.tasks
         yield self.commit_task
 
     def is_inner(self, other: Stage):
         outer = self.outer_stage
         while outer is not None:
             if outer == other:
                 return True
             outer = outer.outer_stage
         return False
 
-    def __getstate__(self):
-        state = self.__dict__.copy()
-        state.pop("tasks", None)
-        state.pop("commit_task", None)
-        state.pop("logger", None)
-        return state
+    def get_task(self, name: str, index: int | None = None) -> Task:
+        """Retrieves a task inside the stage by name.
+        Alias for :py:meth:`Stage.__getitem__`.
+
+        :param name: The name of the task to retrieve.
+        :param index: If multiple task instances with the same name appear inside
+            the stage, you can request a specific one by passing an index.
+        """
+        return self[name, index]
 
 
 class CommitStageTask(Task):
     def __init__(self, stage: Stage, flow: Flow):
-        super().__init__(
-            fn=self.fn,
-            name=f"Commit '{stage.name}'",
-        )
+        # Because the CommitStageTask doesn't get added to the stage.tasks list,
+        # we can't call the super initializer.
+        self.name = f"Commit '{stage.name}'"
+        self.nout = None
 
-        self.stage = stage
+        self.logger = structlog.get_logger(logger_name="Commit Stage", stage=stage)
+
+        self._bound_args = inspect.signature(self.fn).bind()
         self.flow = flow
-        self.upstream_stages = {stage}
-        self.input_tasks = {}
-        self._skip_commit = False
+        self.stage = stage
 
-        self.logger = self.logger.bind(logger_name="Commit Stage", stage=stage)
+        self.flow.add_task(self)
+
+        self.input_tasks = {}
+        self.upstream_stages = [stage]
 
-        self._bound_args = self._signature.bind()
+        self._skip_commit = len(stage.tasks) == 0
         self._visualize_hidden = True
 
     def fn(self):
         if self._skip_commit:
             return
 
         self.logger.info("Committing stage")
```

### Comparing `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/core/task.py` & `pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/core/task.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from __future__ import annotations
 
-import copy
 import inspect
+from collections.abc import Iterable
 from typing import TYPE_CHECKING, Any, Callable
 
 import structlog
 
 from pydiverse.pipedag.context import ConfigContext, DAGContext, RunContext, TaskContext
 from pydiverse.pipedag.context.run_context import FinalTaskState
 from pydiverse.pipedag.errors import FlowError, StageError
 from pydiverse.pipedag.util import deep_map
 from pydiverse.pipedag.util.hashing import stable_hash
 
 if TYPE_CHECKING:
     from pydiverse.pipedag.core import Flow, Stage
 
 
-class Task:
+class UnboundTask:
     """Main building block of flows
 
     Tasks are just fancy functions that can be used inside a flow. As a user
     of pipedag you most likely never interact with the Task class directly,
     but use the @materialize decorator to create a MaterializingTask instead.
 
     :param fn: The function that gets executed by this task.
@@ -45,87 +45,102 @@
         if name is None:
             name = getattr(fn, "__name__", type(self).__name__)
 
         self.fn = fn
         self.name = name
         self.nout = nout
 
-        self.id: int = None  # type: ignore
-        self.flow: Flow = None  # type: ignore
-        self.stage: Stage = None  # type: ignore
-        self.upstream_stages: list[Stage] = None  # type: ignore
-        self.input_tasks: dict[int, Task] = None  # type: ignore
-
+        self._bound_task_type = Task
         self._signature = inspect.signature(fn)
-        self._bound_args: inspect.BoundArguments = None  # type: ignore
-        self.position_hash: str = None  # type: ignore
-
-        self.logger = structlog.get_logger(logger_name=f"Task '{self.name}'", task=self)
-        self._visualize_hidden = False
 
     def __repr__(self):
-        return f"<Task '{self.name}' {hex(id(self))} (id: {self.id})>"
-
-    def __hash__(self):
-        return id(self)
-
-    def __getitem__(self, item):
-        return TaskGetItem(self, self, item)
+        return f"<UnboundTask 'name' {hex(id(self))}>"
 
-    def __iter__(self):
-        if self.nout is None:
-            raise ValueError("Can't iterate over task without specifying `nout`.")
-        for i in range(self.nout):
-            yield TaskGetItem(self, self, i)
-
-    def __call__(self_, *args, **kwargs):
-        """Do the wiring"""
+    def __call__(self, *args, **kwargs) -> Task:
+        """Constructs a `Task` with bound inputs"""
         try:
             ctx = DAGContext.get()
         except LookupError:
             raise FlowError("Can't call pipedag task outside of a flow.") from None
 
         if ctx.stage is None:
             raise StageError("Can't call pipedag task outside of a stage.")
 
-        new = copy.copy(self_)
-        new.flow = ctx.flow
-        new.stage = ctx.stage
-        new.logger = new.logger.bind(logger_name=f"Task '{new.name}'", task=new)
+        # Construct Task
+        bound_args = self._signature.bind(*args, **kwargs)
+        return self._bound_task_type(self, bound_args, ctx.flow, ctx.stage)
 
-        new._bound_args = new._signature.bind(*args, **kwargs)
-        new.position_hash = new.__compute_position_hash()
 
-        new.flow.add_task(new)
-        new.stage.tasks.append(new)
+class Task:
+    def __init__(
+        self,
+        unbound_task: UnboundTask,
+        bound_args: inspect.BoundArguments,
+        flow: Flow,
+        stage: Stage,
+    ):
+        self.fn = unbound_task.fn
+        self.name = unbound_task.name
+        self.nout = unbound_task.nout
+
+        self.logger = structlog.get_logger(logger_name=f"Task '{self.name}'", task=self)
+
+        self._bound_args = bound_args
+        self.flow = flow
+        self.stage = stage
+        self.position_hash = self.__compute_position_hash()
+
+        # The ID gets set by calling flow.add_task
+        self.id: int = None  # type: ignore
+
+        # Do the wiring
+        self.flow.add_task(self)
+        self.stage.tasks.append(self)
 
         # Compute input tasks
-        new.input_tasks = {}
+        self.input_tasks: dict[int, Task] = {}
 
         def visitor(x):
             if isinstance(x, Task):
-                new.input_tasks[x.id] = x
+                self.input_tasks[x.id] = x
             elif isinstance(x, TaskGetItem):
-                new.input_tasks[x.task.id] = x.task
+                self.input_tasks[x.task.id] = x.task
             return x
 
-        deep_map(new._bound_args.args, visitor)
-        deep_map(new._bound_args.kwargs, visitor)
+        deep_map(bound_args.args, visitor)
+        deep_map(bound_args.kwargs, visitor)
 
         # Add upstream edges
-        new.upstream_stages = []
+        self.upstream_stages: list[Stage] = []
+
         upstream_stages_set = set()
-        for input_task in new.input_tasks.values():
-            new.flow.add_edge(input_task, new)
+        for input_task in self.input_tasks.values():
+            self.flow.add_edge(input_task, self)
 
             if input_task.stage not in upstream_stages_set:
                 upstream_stages_set.add(input_task.stage)
-                new.upstream_stages.append(input_task.stage)
+                self.upstream_stages.append(input_task.stage)
+
+        # Private flags
+        self._visualize_hidden = False
 
-        return new
+    def __repr__(self):
+        return f"<Task '{self.name}' {hex(id(self))} (id: {self.id})>"
+
+    def __hash__(self):
+        return id(self)
+
+    def __getitem__(self, item) -> TaskGetItem:
+        return TaskGetItem(self, self, item)
+
+    def __iter__(self) -> Iterable[TaskGetItem]:
+        if self.nout is None:
+            raise ValueError("Can't iterate over task without specifying `nout`.")
+        for i in range(self.nout):
+            yield TaskGetItem(self, self, i)
 
     def run(
         self,
         inputs: dict[int, Any],
         run_context: RunContext = None,
         config_context: ConfigContext = None,
     ):
@@ -214,14 +229,14 @@
         self.item = item
 
         self.position_hash = stable_hash(
             "POS_GET_ITEM", parent.position_hash, repr(self.item)
         )
 
     def __getitem__(self, item):
-        return TaskGetItem(self.task, self, item)
+        return type(self)(self.task, self, item)
 
     def resolve_value(self, task_value: Any):
         parent_value = self.parent.resolve_value(task_value)
         if parent_value is None:
             raise TypeError(f"Parent ({self.parent}) value is None.")
         return parent_value[self.item]
```

### Comparing `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/engine/base.py` & `pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/engine/base.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/engine/dask.py` & `pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/engine/dask.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,15 +19,23 @@
 except ImportError as e:
     warnings.warn(str(e), ImportWarning)
     dask = None
 
 
 @requires(dask, ImportError("DaskEngine requires 'dask' to be installed."))
 class DaskEngine(OrchestrationEngine):
-    """Execute flow in parallel on a single machine using dask"""
+    """
+    Execute a flow in parallel on a single machine using `dask <https://dask.org>`_.
+
+    :param dask_compute_kwargs:
+        Keyword arguments that get passed to :py:func:`dask.compute`.
+        The main kwarg you might be interested in is ``num_workers``,
+        which allows you to specify how many worker processes dask should spawn.
+        By default, it spawns one worker per CPU core.
+    """
 
     def __init__(self, **dask_compute_kwargs):
         self.dask_compute_kwargs = dict(
             traverse=True,
             optimize_graph=False,
             scheduler="processes",
             # Scheduler kwargs
```

### Comparing `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/engine/prefect.py` & `pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/engine/prefect.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,15 +28,24 @@
 
 @requires(prefect, ImportError("Module 'prefect' not installed"))
 @requires(
     prefect_version in SpecifierSet("~=1.0"),
     ImportWarning(f"Requires prefect version 1.x (found {prefect_version})"),
 )
 class PrefectOneEngine(OrchestrationEngine):
-    """Flow execution engine using prefect version 1.x"""
+    """
+    Hands over execution of a flow to `Prefect 1 <https://docs-v1.prefect.io>`_.
+
+    :param flow_kwargs:
+        Optional dictionary of keyword arguments that get passed to the
+        initializer of |prefect1.Flow|_.
+
+    .. |prefect1.Flow| replace:: ``prefect.Flow``
+    .. _prefect1.Flow: https://docs-v1.prefect.io/api/latest/core/flow.html
+    """
 
     def __init__(self, flow_kwargs: dict[str, Any] = None):
         self.flow_kwargs = flow_kwargs or {}
         self.logger = structlog.get_logger(stage=self)
 
     def construct_prefect_flow(self, f: Subflow):
         run_context = RunContext.get()
@@ -108,23 +117,33 @@
             exception=exception,
         )
 
 
 @requires(prefect, ImportError("Module 'prefect' not installed"))
 @requires(
     prefect_version in SpecifierSet("~=2.0"),
-    ImportWarning(f"Requires prefect version 1.x (found {prefect_version})"),
+    ImportWarning(f"Requires prefect version 2.x (found {prefect_version})"),
 )
 class PrefectTwoEngine(OrchestrationEngine):
-    """Flow execution engine using prefect version 2.x"""
+    """
+    Hands over execution of a flow to `Prefect 2 <https://docs.prefect.io>`_.
+
+    :param flow_kwargs:
+        Optional dictionary of keyword arguments that get passed to the
+        initializer of |@prefect2.flow|_ deecorator.
+
+    .. |@prefect2.flow| replace:: ``@prefect.flow``
+    .. _@prefect2.flow:
+            https://docs.prefect.io/latest/api-ref/prefect/flows/#prefect.flows.flow
+    """
 
     def __init__(self, flow_kwargs: dict[str, Any] = None):
         self.flow_kwargs = flow_kwargs or {}
 
-    def construct_prefect_flow(self, f: Subflow):
+    def construct_prefect_flow(self, f: Subflow) -> prefect.Flow:
         from pydiverse.pipedag.materialize.core import MaterializingTask
 
         run_context = RunContext.get()
         config_context = ConfigContext.get()
 
         flow_kwargs = {
             "name": f.name,
@@ -161,31 +180,34 @@
             raise TypeError(f"{type(self).__name__}.run doesn't take kwargs.")
         prefect_flow = self.construct_prefect_flow(flow)
         result = prefect_flow(return_state=True)
 
         # Compute task_values
         task_values = {}
         successful = result.is_completed()
-        for task, state in result.data.items():
-            successful &= state.is_completed()
-            task_values[task] = state.data
+
+        for task, state in result.result().items():
+            if state.is_completed():
+                task_values[task] = state.result()
+            else:
+                successful = False
 
         # If the task failed, extract the exception
         exception = None
         if not successful:
-            for state in result.data.values():
+            for state in result.result().values():
                 if state.is_failed() or state.is_crashed():
                     exception = prefect.states.get_state_exception(state)
                     break
 
         return Result.init_from(
             subflow=flow,
             underlying=result,
             successful=successful,
-            task_values=result,
+            task_values=task_values,
             exception=exception,
         )
 
 
 # Automatic Prefect Version Selection
```

### Comparing `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/engine/sequential.py` & `pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/engine/sequential.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,19 +7,15 @@
 from pydiverse.pipedag.engine.base import OrchestrationEngine
 
 if TYPE_CHECKING:
     from pydiverse.pipedag.core import Subflow
 
 
 class SequentialEngine(OrchestrationEngine):
-    """Execute flow sequentially
-
-    This engine executes all tasks in a flow sequentially in the order
-    that they were defined in.
-    """
+    """Most basic orchestration engine that just executes all tasks sequentially."""
 
     def run(self, flow: Subflow, **run_kwargs):
         run_context = RunContext.get()
         config_context = ConfigContext.get()
 
         results = {}
         exception = None
```

### Comparing `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/errors/__init__.py` & `pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/management/cli.py` & `pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/management/cli.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/management/commands/clear_metadata.py` & `pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/management/commands/clear_metadata.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,17 +4,15 @@
 
 from pydiverse.pipedag import PipedagConfig
 from pydiverse.pipedag.backend.table import SQLTableStore
 from pydiverse.pipedag.backend.table.sql.ddl import DropSchema
 from pydiverse.pipedag.management.cli import cli
 
 
-@cli.command(
-    help="delete all metadata",
-)
+@cli.command()
 @click.option(
     "--config",
     "config_path",
     type=str,
     help="path of the pipedag config file to use",
 )
 @click.option(
@@ -42,14 +40,16 @@
 )
 def clear_metadata(
     config_path: str | None,
     instance: str,
     flow: str | None,
     per_user: bool,
 ):
+    """Clears all pipedag metadata."""
+
     if config_path:
         pipedag_config = PipedagConfig(path=config_path)
     else:
         pipedag_config = PipedagConfig.default
 
     config = pipedag_config.get(
         instance=instance,
```

### Comparing `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/management/commands/delete_schemas.py` & `pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/management/commands/delete_schemas.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,17 +5,15 @@
 
 from pydiverse.pipedag import PipedagConfig
 from pydiverse.pipedag.backend.table import SQLTableStore
 from pydiverse.pipedag.backend.table.sql.ddl import DropSchema, Schema
 from pydiverse.pipedag.management.cli import cli
 
 
-@cli.command(
-    help="deletes all schemas associated with an instance",
-)
+@cli.command()
 @click.option(
     "--config",
     "config_path",
     type=str,
     help="path of the pipedag config file to use",
 )
 @click.option(
@@ -43,14 +41,20 @@
 def delete_schemas(
     config_path: str | None,
     instance: str,
     flow: str | None,
     per_user: bool,
     yes: bool,
 ):
+    """
+    Delete all schemas associated with an instance.
+
+    Only works with SQLTableStore.
+    """
+
     if config_path:
         pipedag_config = PipedagConfig(path=config_path)
     else:
         pipedag_config = PipedagConfig.default
 
     config = pipedag_config.get(
         instance=instance,
```

### Comparing `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/materialize/cache.py` & `pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/materialize/cache.py`

 * *Files 5% similar despite different names*

```diff
@@ -190,15 +190,15 @@
 
     @staticmethod
     def raw_sql_cache_lookup(
         store: BaseTableStore,
         task_cache_info: TaskCacheInfo,
         raw_sql: RawSql,
         query_hash: str,
-    ):
+    ) -> tuple[TableCacheInfo, RawSqlMetadata | None]:
         task_hash = task_cache_info.get_task_cache_key()
         # Store tables
         try:
             # Try retrieving the table from the cache and then copying it
             # to the transaction stage
             metadata = store.retrieve_raw_sql_metadata(
                 query_hash, task_hash, raw_sql.stage
@@ -206,16 +206,20 @@
             store.copy_raw_sql_tables_to_transaction(metadata, raw_sql.stage)
             store.logger.info(f"Lazy cache of stage '{raw_sql.stage}' found")
             is_cache_valid = True
         except CacheError as e:
             # Either not found in cache, or copying failed
             # -> Store using default method
             store.logger.warning("Cache miss for raw-SQL", cause=str(e))
+            metadata = None
             is_cache_valid = False
-        return TableCacheInfo(raw_sql.stage, task_hash, query_hash, is_cache_valid)
+        return (
+            TableCacheInfo(raw_sql.stage, task_hash, query_hash, is_cache_valid),
+            metadata,
+        )
 
     @staticmethod
     def task_cache_key(task: MaterializingTask, input_hash: str, cache_fn_hash: str):
         """Cache key used to judge cache validity of the current task output.
 
         Also referred to as `task_hash`.
```

### Comparing `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/materialize/metadata.py` & `pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/materialize/metadata.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/materialize/store.py` & `pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/materialize/store.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 import itertools
 from typing import Any, Callable
 
 import structlog
 
 from pydiverse.pipedag import Blob, Stage, Table, backend
 from pydiverse.pipedag._typing import Materializable, T
-from pydiverse.pipedag.context import ConfigContext, RunContext
+from pydiverse.pipedag.context import ConfigContext, RunContext, TaskContext
 from pydiverse.pipedag.context.run_context import StageState
 from pydiverse.pipedag.core.config import PipedagConfig
-from pydiverse.pipedag.errors import DuplicateNameError, StageError
+from pydiverse.pipedag.core.task import Task, TaskGetItem
+from pydiverse.pipedag.errors import CacheError, DuplicateNameError, StageError
 from pydiverse.pipedag.materialize.container import RawSql
 from pydiverse.pipedag.materialize.core import MaterializingTask, TaskInfo
 from pydiverse.pipedag.materialize.metadata import TaskMetadata
 from pydiverse.pipedag.util import Disposable, deep_map
 
 
 class PipeDAGStore(Disposable):
@@ -103,25 +104,37 @@
             self.table_store.commit_stage(stage)
             self.blob_store.commit_stage(stage)
 
     # ### Materialization ### #
 
     def dematerialize_item(
         self,
-        item: Table | Blob | Any,
+        item: Table | RawSql | Blob | Any,
         as_type: type[T],
         ctx: RunContext | None = None,
     ):
         if ctx is None:
             ctx = RunContext.get()
 
         if isinstance(item, Table):
             ctx.validate_stage_lock(item.stage)
             obj = self.table_store.retrieve_table_obj(item, as_type=as_type)
             return obj
+        elif isinstance(item, RawSql):
+            ctx.validate_stage_lock(item.stage)
+
+            loaded_tables = {}
+            for table_name in item:
+                table = item[table_name]
+                obj = self.table_store.retrieve_table_obj(table, as_type=as_type)
+                loaded_tables[table_name] = obj
+
+            new_raw_sql = item.copy_without_obj()
+            new_raw_sql.loaded_tables = loaded_tables
+            return new_raw_sql
         elif isinstance(item, Blob):
             ctx.validate_stage_lock(item.stage)
             return self.blob_store.retrieve_blob(item)
         return item
 
     def dematerialize_task_inputs(
         self,
@@ -214,29 +227,29 @@
 
             # Do the materialization
             if isinstance(x, (Table, RawSql, Blob)):
                 if not task.lazy:
                     # task cache_key is output cache_key for eager tables
                     x.cache_key = task_info.task_cache_info.get_task_cache_key()
 
-                if isinstance(x, (Table, Blob)):
-                    x.stage = stage
-                    # Update name:
-                    # - If no name has been provided, generate on automatically
-                    # - If the provided name ends with %%, perform name mangling
-                    object_number = next(auto_suffix_counter)
-                    auto_suffix = (
-                        f"{task_info.task_cache_info.get_task_cache_key()}"
-                        f"_{object_number:04d}"
-                    )
-
-                    if x.name is None:
-                        x.name = task.name + "_" + auto_suffix
-                    elif x.name.endswith("%%"):
-                        x.name = x.name[:-2] + auto_suffix
+                x.stage = stage
+
+                # Update name:
+                # - If no name has been provided, generate on automatically
+                # - If the provided name ends with %%, perform name mangling
+                object_number = next(auto_suffix_counter)
+                auto_suffix = (
+                    f"{task_info.task_cache_info.get_task_cache_key()}"
+                    f"_{object_number:04d}"
+                )
+
+                if x.name is None:
+                    x.name = task.name + "_" + auto_suffix
+                elif x.name.endswith("%%"):
+                    x.name = x.name[:-2] + auto_suffix
 
                 ctx.validate_stage_lock(stage)
                 if isinstance(x, Table):
                     if x.obj is None:
                         raise TypeError("Underlying table object can't be None")
                     tables.append(x)
                 elif isinstance(x, RawSql):
@@ -435,14 +448,46 @@
             blobs,
             self.table_store.copy_table_to_transaction,
             store_raw_sql,
             self.blob_store.copy_blob_to_transaction,
             lambda: self.table_store.store_task_metadata(original_metadata, task.stage),
         )
 
+    def retrieve_most_recent_task_output_from_cache(
+        self, task: MaterializingTask
+    ) -> (Materializable, TaskMetadata):
+        """
+        Retrieves the cached output from the most recent execution of a task.
+
+        This retrieval is done based on the name, stage and position hash
+        of the task.
+
+        :param task: The materializing task for which to retrieve
+            the cached output.
+        :return: The output from the task as well as the corresponding metadata.
+        :raises CacheError: if no matching task exists in the cache
+        """
+
+        # This returns all metadata objects with the same name, stage, AND position
+        # hash as `task`. We utilize the position hash to identify a specific
+        # task instance, if the same task appears multiple times in a stage.
+        metadata = self.table_store.retrieve_all_task_metadata(task)
+
+        if not metadata:
+            raise CacheError(
+                f"Couldn't find cached output for task '{task}'"
+                " with matching position hash."
+            )
+
+        # Choose newest entry
+        newest_metadata = sorted(metadata, key=lambda m: m.timestamp)[-1]
+        cached_output = self.json_decode(newest_metadata.output_json)
+
+        return cached_output, newest_metadata
+
     # ### Utils ### #
 
     def json_encode(self, value: Materializable) -> str:
         """Encode a materializable value as json
 
         In addition to the default types that python can serialise to json,
         this function can also serialise `Table`, `RawSql`, and `Blob` objects.
@@ -455,7 +500,40 @@
     def json_decode(self, value: str) -> Materializable:
         """Decode a materializable value as json
 
         Counterpart for the `json_encode` function. Can decode `Table` and
         `Blob` objects.
         """
         return self.json_decoder.decode(value)
+
+
+def dematerialize_output_from_store(
+    store: PipeDAGStore,
+    task: Task | TaskGetItem,
+    task_output: Materializable,
+    as_type: type | None,
+) -> Any:
+    """
+    Dematerializes a task's output from the store
+
+    Must be called inside a ConfigContext and RunContext. Instead
+    of a RunContext, a DematerializeRunContext can also be used.
+    """
+    if isinstance(task, Task):
+        root_task = task
+    else:
+        root_task = task.task
+
+    if as_type is None:
+        assert isinstance(root_task, MaterializingTask)
+        as_type = root_task.input_type
+
+    run_context = RunContext.get()
+    task_output = task.resolve_value(task_output)
+
+    with TaskContext(task):
+        return deep_map(
+            task_output,
+            lambda item: store.dematerialize_item(
+                item, as_type=as_type, ctx=run_context
+            ),
+        )
```

### Comparing `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/util/deep_map.py` & `pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/util/deep_map.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/util/deep_merge.py` & `pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/util/deep_merge.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/util/disposable.py` & `pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/util/disposable.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/util/hashing.py` & `pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/util/hashing.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/util/import_.py` & `pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/util/import_.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import builtins
 import importlib
+import os
 from collections.abc import Collection
 from typing import Any
 
 
 def requires(requirements: Any | list, exception: BaseException | type[BaseException]):
     """Class decorator for handling optional imports.
 
@@ -19,15 +20,22 @@
 
     def decorator(cls):
         if all(requirements):
             return cls
 
         # Modify class to raise exception
         class RaiserMeta(type):
-            def __getattr__(self, x):
+            def __getattribute__(self, x):
+                # While building the documentation, we set the SPHINX_BUILD env
+                # variable. This allows us to properly generate the documentation
+                # without raising exceptions.
+                if os.environ.get("SPHINX_BUILD"):
+                    return getattr(cls, x)
+                if x in ["__class__", "__doc__", "__name__", "__qualname__"]:
+                    return getattr(cls, x)
                 raise exception
 
         def raiser(*args, **kwargs):
             raise exception
 
         __name = str(cls.__name__)
         __bases = ()
```

### Comparing `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/util/ipc.py` & `pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/util/ipc.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/util/json.py` & `pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/util/json.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,14 +51,15 @@
         }
     if isinstance(o, RawSql):
         return {
             TYPE_KEY: Type.RAW_SQL,
             "stage": o.stage.name,
             "name": o.name,
             "cache_key": o.cache_key,
+            "table_names": o.table_names,
         }
     if isinstance(o, Blob):
         return {
             TYPE_KEY: Type.BLOB,
             "stage": o.stage.name,
             "name": o.name,
             "cache_key": o.cache_key,
@@ -101,32 +102,29 @@
 
     run_context = RunContext.get()
     stages = run_context.flow.stages
 
     if type_ == Type.TABLE:
         tbl = Table(
             name=d["name"],
-            stage=stages[d["stage"]],
             primary_key=d["primary_key"],
             indexes=d["indexes"],
         )
+        tbl.stage = stages[d["stage"]]
         tbl.cache_key = d["cache_key"]
         return tbl
     if type_ == Type.RAW_SQL:
-        raw_sql = RawSql(
-            name=d["name"],
-            stage=stages[d["stage"]],
-        )
+        raw_sql = RawSql(name=d["name"])
+        raw_sql.stage = stages[d["stage"]]
         raw_sql.cache_key = d["cache_key"]
+        raw_sql.table_names = d["table_names"]
         return raw_sql
     if type_ == Type.BLOB:
-        blob = Blob(
-            name=d["name"],
-            stage=stages[d["stage"]],
-        )
+        blob = Blob(name=d["name"])
+        blob.stage = stages[d["stage"]]
         blob.cache_key = d["cache_key"]
         return blob
     if type_ == Type.STAGE:
         return stages[d["name"]]
     if type_ == Type.PIPEDAG_CONFIG:
         # PipedagConfig objects are allowed as input to @materialize tasks,
         # but it is not allowed as output since this might cause trouble
```

### Comparing `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/util/naming.py` & `pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/util/naming.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.0/src/pydiverse/pipedag/util/structlog.py` & `pydiverse_pipedag-0.6.1/src/pydiverse/pipedag/util/structlog.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.0/PKG-INFO` & `pydiverse_pipedag-0.6.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydiverse-pipedag
-Version: 0.6.0
+Version: 0.6.1
 Summary: A pipeline orchestration library executing tasks within one python session. It takes care of SQL table (de)materialization, caching and cache invalidation. Blob storage is supported as well for example for storing model files.
 License: BSD-3-Clause
 Author: QuantCo, Inc.
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -13,27 +13,29 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: SQL
 Classifier: Topic :: Database
 Provides-Extra: dask
 Provides-Extra: filelock
+Provides-Extra: prefect
 Provides-Extra: zookeeper
 Requires-Dist: PyYAML (>=6.0)
 Requires-Dist: SQLAlchemy (>=1.4.39)
 Requires-Dist: attrs (>=22.1.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: cryptography (>=41.0.1)
 Requires-Dist: dask (>=2022.1.0) ; extra == "dask"
 Requires-Dist: filelock (>=3.7.1) ; extra == "filelock"
 Requires-Dist: kazoo (>=2.8.0) ; extra == "zookeeper"
 Requires-Dist: msgpack (>=1.0.4)
 Requires-Dist: networkx (>=2.8)
 Requires-Dist: packaging (>=21.3)
 Requires-Dist: pandas (>=1.4.3)
+Requires-Dist: prefect (>=2.6) ; extra == "prefect"
 Requires-Dist: pyarrow (>=11.0.0)
 Requires-Dist: pydot (>=1.4.2)
 Requires-Dist: pynng (>=0.7.1)
 Requires-Dist: pyparsing (>=3.0)
 Requires-Dist: python-box (>=6.1.0)
 Requires-Dist: structlog (>=22.1.0)
 Requires-Dist: typing-extensions (>=4.1.0,<5.0.0)
@@ -147,43 +149,31 @@
 if __name__ == "__main__":
     main()
 ```
 
 Create a file called `pipedag.yaml` in the same directory:
 
 ```yaml
-name: pipedag_tests
-table_store_connections:
-  postgres:
-    args:
-      # Postgres: this can be used after running `docker-compose up`  
-      url: "postgresql://{$POSTGRES_USERNAME}:{$POSTGRES_PASSWORD}@127.0.0.1:6543/{instance_id}"
-
 instances:
   __any__:
-    # listen-interface for pipedag context server which synchronizes some task state during DAG execution
     network_interface: "127.0.0.1"
-    # classes to be materialized to table store even without pipedag Table wrapper (we have loose coupling between
-    # pipedag and pydiverse.transform, so consider adding 'pydiverse.transform.Table' in your config)
-    auto_table: ["pandas.DataFrame", "sqlalchemy.sql.elements.TextClause", "sqlalchemy.sql.selectable.Selectable"]
-    fail_fast: true
+    auto_table:
+      - "pandas.DataFrame"
+      - "sqlalchemy.sql.expression.TextClause"
+      - "sqlalchemy.sql.expression.Selectable"
 
+    fail_fast: true
     instance_id: pipedag_default
     table_store:
       class: "pydiverse.pipedag.backend.table.SQLTableStore"
-
-      # Postgres: this can be used after running `docker-compose up`
-      table_store_connection: postgres
       args:
+        url: "postgresql://sa:Pydiverse23@127.0.0.1:6543/{instance_id}"
         create_database_if_not_exists: True
-        
-        # print select statements before being encapsualted in materialize expressions and tables before writing to
-        # database
+
         print_materialize: true
-        # print final sql statements
         print_sql: true
 
       local_table_cache:
         store_input: true
         store_output: true
         use_stored_input_as_cache: true
         class: "pydiverse.pipedag.backend.table.cache.ParquetTableCache"
@@ -192,53 +182,40 @@
 
     blob_store:
       class: "pydiverse.pipedag.backend.blob.FileBlobStore"
       args:
         base_path: "/tmp/pipedag/blobs"
 
     lock_manager:
-      class: "pydiverse.pipedag.backend.lock.ZooKeeperLockManager"
-      args:
-        hosts: "localhost:2181"
+      class: "pydiverse.pipedag.backend.lock.DatabaseLockManager"
 
     orchestration:
       class: "pydiverse.pipedag.engine.SequentialEngine"
 ```
 
-If you don't have a postgres, Microsoft SQL Server, or IBM DB2 database at hand, you can
-start a postgres database with the following `docker-compose.yaml` file:
+If you don't have a postgres database at hand, you can start a postgres database, with the following `docker-compose.yaml` file:
 
 ```yaml
 version: "3.9"
 services:
   postgres:
     image: postgres
     environment:
       POSTGRES_USER: sa
       POSTGRES_PASSWORD: Pydiverse23
-      POSTGRES_PORT: 6543
-    ports:
-      - 6543:5432
-  zoo:
-    image: zookeeper
-    environment:
-      ZOO_4LW_COMMANDS_WHITELIST: ruok
-      ZOO_MAX_CLIENT_CNXNS: 100
     ports:
-      - 2181:2181
+      - "6543:5432"
 ```
 
 Run `docker-compose up` in the directory of your `docker-compose.yaml` and then execute
 the flow script as follows with a shell like `bash` and a python environment that
 includes `pydiverse-pipedag`, `pandas`, and `sqlalchemy`:
 
 ```bash
-export POSTGRES_USERNAME=sa
-export POSTGRES_PASSWORD=Pydiverse23
-python run_pipeline.py
+poetry run python run_pipeline.py
 ```
 
 Finally, you may connect to your localhost postgres database `pipedag_default` and
 look at tables in schemas `stage_1`..`stage_3`.
 
 If you don't have a SQL UI at hand, you may use `psql` command line tool inside the docker container.
 Check out the `NAMES` column in `docker ps` output. If the name of your postgres container is
```

