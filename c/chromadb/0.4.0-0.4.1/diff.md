# Comparing `tmp/chromadb-0.4.0.tar.gz` & `tmp/chromadb-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromadb-0.4.0.tar", last modified: Mon Jul 17 23:18:24 2023, max compression
+gzip compressed data, was "chromadb-0.4.1.tar", last modified: Tue Jul 18 23:29:37 2023, max compression
```

## Comparing `chromadb-0.4.0.tar` & `chromadb-0.4.1.tar`

### file list

```diff
@@ -1,237 +1,237 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.353961 chromadb-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-17 23:18:09.000000 chromadb-0.4.0/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.257961 chromadb-0.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.285961 chromadb-0.4.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-17 23:18:09.000000 chromadb-0.4.0/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-17 23:18:09.000000 chromadb-0.4.0/.github/ISSUE_TEMPLATE/feature_request.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-17 23:18:09.000000 chromadb-0.4.0/.github/ISSUE_TEMPLATE/installation_trouble.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.285961 chromadb-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-17 23:18:09.000000 chromadb-0.4.0/.github/workflows/chroma-client-integration-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-17 23:18:09.000000 chromadb-0.4.0/.github/workflows/chroma-integration-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-17 23:18:09.000000 chromadb-0.4.0/.github/workflows/chroma-release-python-client.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-07-17 23:18:09.000000 chromadb-0.4.0/.github/workflows/chroma-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-17 23:18:09.000000 chromadb-0.4.0/.github/workflows/chroma-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-17 23:18:09.000000 chromadb-0.4.0/.github/workflows/pr-review-checklist.yml
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-17 23:18:09.000000 chromadb-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-17 23:18:09.000000 chromadb-0.4.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.285961 chromadb-0.4.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-17 23:18:09.000000 chromadb-0.4.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-07-17 23:18:09.000000 chromadb-0.4.0/DEVELOP.md
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-17 23:18:09.000000 chromadb-0.4.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 23:18:09.000000 chromadb-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-07-17 23:18:24.353961 chromadb-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-17 23:18:09.000000 chromadb-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-17 23:18:09.000000 chromadb-0.4.0/RELEASE_PROCESS.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.289961 chromadb-0.4.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      110 2023-07-17 23:18:09.000000 chromadb-0.4.0/bin/build
--rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-07-17 23:18:09.000000 chromadb-0.4.0/bin/docker_entrypoint.sh
--rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-07-17 23:18:09.000000 chromadb-0.4.0/bin/generate_cloudformation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      487 2023-07-17 23:18:09.000000 chromadb-0.4.0/bin/integration-test
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.289961 chromadb-0.4.0/bin/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-17 23:18:09.000000 chromadb-0.4.0/bin/templates/docker-compose.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      451 2023-07-17 23:18:09.000000 chromadb-0.4.0/bin/test-package.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      321 2023-07-17 23:18:09.000000 chromadb-0.4.0/bin/test-remote
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-17 23:18:09.000000 chromadb-0.4.0/bin/test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      151 2023-07-17 23:18:09.000000 chromadb-0.4.0/bin/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.293961 chromadb-0.4.0/chromadb/
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.297961 chromadb-0.4.0/chromadb/api/
--rw-r--r--   0 runner    (1001) docker     (123)    13188 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/api/fastapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.297961 chromadb-0.4.0/chromadb/api/models/
--rw-r--r--   0 runner    (1001) docker     (123)    15200 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/api/models/Collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    22394 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/api/segment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12405 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/api/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     8133 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.297961 chromadb-0.4.0/chromadb/db/
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/db/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.301961 chromadb-0.4.0/chromadb/db/impl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/db/impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7727 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/db/impl/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/db/impl/sqlite_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/db/migrations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.301961 chromadb-0.4.0/chromadb/db/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/db/mixins/embeddings_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)    16398 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/db/mixins/sysdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/db/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.301961 chromadb-0.4.0/chromadb/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)   368824 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/experimental/density_relevance.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.301961 chromadb-0.4.0/chromadb/ingest/
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/ingest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.301961 chromadb-0.4.0/chromadb/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.301961 chromadb-0.4.0/chromadb/migrations/embeddings_queue/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/migrations/embeddings_queue/00001-embeddings.sqlite.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.301961 chromadb-0.4.0/chromadb/migrations/metadb/
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/migrations/metadb/00001-embedding-metadata.sqlite.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.305961 chromadb-0.4.0/chromadb/migrations/sysdb/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/migrations/sysdb/00001-collections.sqlite.sql
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/migrations/sysdb/00002-segments.sqlite.sql
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/migrations/sysdb/00003-collection-dimension.sqlite.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.305961 chromadb-0.4.0/chromadb/segment/
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/segment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.265961 chromadb-0.4.0/chromadb/segment/impl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.305961 chromadb-0.4.0/chromadb/segment/impl/manager/
--rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/segment/impl/manager/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.305961 chromadb-0.4.0/chromadb/segment/impl/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)    19069 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/segment/impl/metadata/sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.309961 chromadb-0.4.0/chromadb/segment/impl/vector/
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/segment/impl/vector/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/segment/impl/vector/brute_force_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/segment/impl/vector/hnsw_params.py
--rw-r--r--   0 runner    (1001) docker     (123)    10716 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/segment/impl/vector/local_hnsw.py
--rw-r--r--   0 runner    (1001) docker     (123)    15667 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/segment/impl/vector/local_persistent_hnsw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.309961 chromadb-0.4.0/chromadb/server/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.309961 chromadb-0.4.0/chromadb/server/fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/server/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/server/fastapi/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.309961 chromadb-0.4.0/chromadb/telemetry/
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/telemetry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/telemetry/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/telemetry/posthog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.313961 chromadb-0.4.0/chromadb/test/
--rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.313961 chromadb-0.4.0/chromadb/test/db/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.317961 chromadb-0.4.0/chromadb/test/db/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/test/db/migrations/00001-migration-1.psql.sql
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/test/db/migrations/00001-migration-1.sqlite.sql
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/test/db/migrations/00002-migration-2.psql.sql
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/test/db/migrations/00002-migration-2.sqlite.sql
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/test/db/migrations/00003-migration-3.psql.sql
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/test/db/migrations/00003-migration-3.sqlite.sql
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/test/db/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/test/db/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/test/db/test_migrations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10090 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/test/db/test_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.317961 chromadb-0.4.0/chromadb/test/ingest/
--rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/test/ingest/test_producer_consumer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.321961 chromadb-0.4.0/chromadb/test/property/
--rw-r--r--   0 runner    (1001) docker     (123)    11313 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/test/property/invariants.py
--rw-r--r--   0 runner    (1001) docker     (123)    19519 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/test/property/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/test/property/test_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/test/property/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/test/property/test_cross_version_persist.py
--rw-r--r--   0 runner    (1001) docker     (123)    13367 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/test/property/test_embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     9405 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/test/property/test_filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/test/property/test_persist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.321961 chromadb-0.4.0/chromadb/test/segment/
--rw-r--r--   0 runner    (1001) docker     (123)    15572 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/test/segment/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    14604 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/test/segment/test_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)    41277 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/test/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/test/test_chroma.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/test/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/test/test_multithreaded.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.321961 chromadb-0.4.0/chromadb/test/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/test/utils/test_messagid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.321961 chromadb-0.4.0/chromadb/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/utils/distance_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16228 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/utils/embedding_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/utils/messageid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-17 23:18:09.000000 chromadb-0.4.0/chromadb/utils/read_write_lock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.293961 chromadb-0.4.0/chromadb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-07-17 23:18:24.000000 chromadb-0.4.0/chromadb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-07-17 23:18:24.000000 chromadb-0.4.0/chromadb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 23:18:24.000000 chromadb-0.4.0/chromadb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-17 23:18:24.000000 chromadb-0.4.0/chromadb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-17 23:18:24.000000 chromadb-0.4.0/chromadb.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.273961 chromadb-0.4.0/clients/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.329961 chromadb-0.4.0/clients/js/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/.prettierrc.json
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/DEVELOP.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.273961 chromadb-0.4.0/clients/js/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.333961 chromadb-0.4.0/clients/js/examples/browser/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/examples/browser/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/examples/browser/app.ts
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/examples/browser/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/examples/browser/package.json
--rw-r--r--   0 runner    (1001) docker     (123)    68042 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/examples/browser/yarn.lock
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.333961 chromadb-0.4.0/clients/js/examples/node/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/examples/node/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/examples/node/app.js
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/examples/node/package.json
--rw-r--r--   0 runner    (1001) docker     (123)    17080 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/examples/node/yarn.lock
--rwxr-xr-x   0 runner    (1001) docker     (123)     1247 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/genapi.sh
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/jest.config.ts
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/openapitools.json
--rw-r--r--   0 runner    (1001) docker     (123)   448020 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.337961 chromadb-0.4.0/clients/js/src/
--rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/src/ChromaClient.ts
--rw-r--r--   0 runner    (1001) docker     (123)    19757 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/src/Collection.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.337961 chromadb-0.4.0/clients/js/src/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/src/embeddings/CohereEmbeddingFunction.ts
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/src/embeddings/IEmbeddingFunction.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/src/embeddings/OpenAIEmbeddingFunction.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/src/embeddings/TransformersEmbeddingFunction.ts
--rwxr-xr-x   0 runner    (1001) docker     (123)     3402 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/src/embeddings/WebAIEmbeddingFunction.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.341961 chromadb-0.4.0/clients/js/src/generated/
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/src/generated/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    54547 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/src/generated/api.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/src/generated/configuration.ts
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/src/generated/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/src/generated/models.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/src/generated/runtime.ts
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/src/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/src/types.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/src/utils.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.345961 chromadb-0.4.0/clients/js/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/test/add.collections.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/test/client.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/test/collection.client.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/test/collection.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/test/data.ts
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/test/delete.collection.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/test/get.collection.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/test/initClient.ts
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/test/peek.collection.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/test/query.collection.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/test/update.collection.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/test/upsert.collections.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/tsconfig.json
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/tsconfig.module.json
--rw-r--r--   0 runner    (1001) docker     (123)   156893 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/js/yarn.lock
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.349961 chromadb-0.4.0/clients/python/
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/python/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     1257 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/python/build_python_thin_client.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      850 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/python/integration-test.sh
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/python/is_thin_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-17 23:18:09.000000 chromadb-0.4.0/clients/python/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-17 23:18:09.000000 chromadb-0.4.0/docker-compose.server.example.yml
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-17 23:18:09.000000 chromadb-0.4.0/docker-compose.test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-17 23:18:09.000000 chromadb-0.4.0/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.349961 chromadb-0.4.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-17 23:18:09.000000 chromadb-0.4.0/examples/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.349961 chromadb-0.4.0/examples/basic_functionality/
--rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-07-17 23:18:09.000000 chromadb-0.4.0/examples/basic_functionality/alternative_embeddings.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-07-17 23:18:09.000000 chromadb-0.4.0/examples/basic_functionality/local_persistence.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-07-17 23:18:09.000000 chromadb-0.4.0/examples/basic_functionality/where_filtering.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.277961 chromadb-0.4.0/examples/deployments/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.353961 chromadb-0.4.0/examples/deployments/google-cloud-compute/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-17 23:18:09.000000 chromadb-0.4.0/examples/deployments/google-cloud-compute/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-17 23:18:09.000000 chromadb-0.4.0/examples/deployments/google-cloud-compute/chroma.tf
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-17 23:18:09.000000 chromadb-0.4.0/examples/deployments/google-cloud-compute/main.tf
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-17 23:18:09.000000 chromadb-0.4.0/examples/deployments/google-cloud-compute/startup.sh
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-17 23:18:09.000000 chromadb-0.4.0/examples/deployments/google-cloud-compute/variables.tf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.277961 chromadb-0.4.0/examples/use_with/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:18:24.353961 chromadb-0.4.0/examples/use_with/cohere/
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-17 23:18:09.000000 chromadb-0.4.0/examples/use_with/cohere/cohere_js.js
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-07-17 23:18:09.000000 chromadb-0.4.0/examples/use_with/cohere/cohere_python.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-17 23:18:09.000000 chromadb-0.4.0/examples/use_with/cohere/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-17 23:18:09.000000 chromadb-0.4.0/log_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-17 23:18:09.000000 chromadb-0.4.0/pull_request_template.md
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-17 23:18:09.000000 chromadb-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-17 23:18:09.000000 chromadb-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-17 23:18:09.000000 chromadb-0.4.0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 23:18:24.353961 chromadb-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.239898 chromadb-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-18 23:29:22.000000 chromadb-0.4.1/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.159897 chromadb-0.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.179897 chromadb-0.4.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-18 23:29:22.000000 chromadb-0.4.1/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-18 23:29:22.000000 chromadb-0.4.1/.github/ISSUE_TEMPLATE/feature_request.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-18 23:29:22.000000 chromadb-0.4.1/.github/ISSUE_TEMPLATE/installation_trouble.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.183897 chromadb-0.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-18 23:29:22.000000 chromadb-0.4.1/.github/workflows/chroma-client-integration-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-18 23:29:22.000000 chromadb-0.4.1/.github/workflows/chroma-integration-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-18 23:29:22.000000 chromadb-0.4.1/.github/workflows/chroma-release-python-client.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-07-18 23:29:22.000000 chromadb-0.4.1/.github/workflows/chroma-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-18 23:29:22.000000 chromadb-0.4.1/.github/workflows/chroma-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-18 23:29:22.000000 chromadb-0.4.1/.github/workflows/pr-review-checklist.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-18 23:29:22.000000 chromadb-0.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-18 23:29:22.000000 chromadb-0.4.1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.183897 chromadb-0.4.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-18 23:29:22.000000 chromadb-0.4.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-07-18 23:29:22.000000 chromadb-0.4.1/DEVELOP.md
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-18 23:29:22.000000 chromadb-0.4.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-18 23:29:22.000000 chromadb-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-07-18 23:29:37.239898 chromadb-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-18 23:29:22.000000 chromadb-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-18 23:29:22.000000 chromadb-0.4.1/RELEASE_PROCESS.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.187897 chromadb-0.4.1/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      110 2023-07-18 23:29:22.000000 chromadb-0.4.1/bin/build
+-rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-07-18 23:29:22.000000 chromadb-0.4.1/bin/docker_entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-07-18 23:29:22.000000 chromadb-0.4.1/bin/generate_cloudformation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      487 2023-07-18 23:29:22.000000 chromadb-0.4.1/bin/integration-test
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.187897 chromadb-0.4.1/bin/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-18 23:29:22.000000 chromadb-0.4.1/bin/templates/docker-compose.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      451 2023-07-18 23:29:22.000000 chromadb-0.4.1/bin/test-package.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      321 2023-07-18 23:29:22.000000 chromadb-0.4.1/bin/test-remote
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-18 23:29:22.000000 chromadb-0.4.1/bin/test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      151 2023-07-18 23:29:22.000000 chromadb-0.4.1/bin/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.187897 chromadb-0.4.1/chromadb/
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.191897 chromadb-0.4.1/chromadb/api/
+-rw-r--r--   0 runner    (1001) docker     (123)    13188 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/api/fastapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.191897 chromadb-0.4.1/chromadb/api/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    15200 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/api/models/Collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22394 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/api/segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12405 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/api/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.191897 chromadb-0.4.1/chromadb/db/
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/db/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.195897 chromadb-0.4.1/chromadb/db/impl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/db/impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7727 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/db/impl/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/db/impl/sqlite_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/db/migrations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.195897 chromadb-0.4.1/chromadb/db/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/db/mixins/embeddings_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16398 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/db/mixins/sysdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/db/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.195897 chromadb-0.4.1/chromadb/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)   368824 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/experimental/density_relevance.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.195897 chromadb-0.4.1/chromadb/ingest/
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/ingest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.195897 chromadb-0.4.1/chromadb/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.195897 chromadb-0.4.1/chromadb/migrations/embeddings_queue/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/migrations/embeddings_queue/00001-embeddings.sqlite.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.195897 chromadb-0.4.1/chromadb/migrations/metadb/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/migrations/metadb/00001-embedding-metadata.sqlite.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.199897 chromadb-0.4.1/chromadb/migrations/sysdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/migrations/sysdb/00001-collections.sqlite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/migrations/sysdb/00002-segments.sqlite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/migrations/sysdb/00003-collection-dimension.sqlite.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.199897 chromadb-0.4.1/chromadb/segment/
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/segment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.163897 chromadb-0.4.1/chromadb/segment/impl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.199897 chromadb-0.4.1/chromadb/segment/impl/manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/segment/impl/manager/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.199897 chromadb-0.4.1/chromadb/segment/impl/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    19069 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/segment/impl/metadata/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.199897 chromadb-0.4.1/chromadb/segment/impl/vector/
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/segment/impl/vector/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/segment/impl/vector/brute_force_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/segment/impl/vector/hnsw_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10716 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/segment/impl/vector/local_hnsw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15667 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/segment/impl/vector/local_persistent_hnsw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.199897 chromadb-0.4.1/chromadb/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.203897 chromadb-0.4.1/chromadb/server/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/server/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/server/fastapi/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.203897 chromadb-0.4.1/chromadb/telemetry/
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/telemetry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/telemetry/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/telemetry/posthog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.203897 chromadb-0.4.1/chromadb/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.207897 chromadb-0.4.1/chromadb/test/db/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.207897 chromadb-0.4.1/chromadb/test/db/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/test/db/migrations/00001-migration-1.psql.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/test/db/migrations/00001-migration-1.sqlite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/test/db/migrations/00002-migration-2.psql.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/test/db/migrations/00002-migration-2.sqlite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/test/db/migrations/00003-migration-3.psql.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/test/db/migrations/00003-migration-3.sqlite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/test/db/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/test/db/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/test/db/test_migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10090 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/test/db/test_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.207897 chromadb-0.4.1/chromadb/test/ingest/
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/test/ingest/test_producer_consumer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.211897 chromadb-0.4.1/chromadb/test/property/
+-rw-r--r--   0 runner    (1001) docker     (123)    11313 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/test/property/invariants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19519 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/test/property/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/test/property/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/test/property/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/test/property/test_cross_version_persist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13367 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/test/property/test_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9405 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/test/property/test_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/test/property/test_persist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.211897 chromadb-0.4.1/chromadb/test/segment/
+-rw-r--r--   0 runner    (1001) docker     (123)    15572 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/test/segment/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14604 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/test/segment/test_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41277 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/test/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/test/test_chroma.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/test/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/test/test_multithreaded.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.211897 chromadb-0.4.1/chromadb/test/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/test/utils/test_messagid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.215897 chromadb-0.4.1/chromadb/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/utils/distance_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16228 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/utils/embedding_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/utils/messageid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-18 23:29:22.000000 chromadb-0.4.1/chromadb/utils/read_write_lock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.191897 chromadb-0.4.1/chromadb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-07-18 23:29:37.000000 chromadb-0.4.1/chromadb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-07-18 23:29:37.000000 chromadb-0.4.1/chromadb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 23:29:37.000000 chromadb-0.4.1/chromadb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-18 23:29:37.000000 chromadb-0.4.1/chromadb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 23:29:37.000000 chromadb-0.4.1/chromadb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.171897 chromadb-0.4.1/clients/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.219898 chromadb-0.4.1/clients/js/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/.prettierrc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/DEVELOP.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.171897 chromadb-0.4.1/clients/js/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.223898 chromadb-0.4.1/clients/js/examples/browser/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/examples/browser/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/examples/browser/app.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/examples/browser/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/examples/browser/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)    68042 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/examples/browser/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.223898 chromadb-0.4.1/clients/js/examples/node/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/examples/node/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/examples/node/app.js
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/examples/node/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17080 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/examples/node/yarn.lock
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1247 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/genapi.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/jest.config.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/openapitools.json
+-rw-r--r--   0 runner    (1001) docker     (123)   448020 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.223898 chromadb-0.4.1/clients/js/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/src/ChromaClient.ts
+-rw-r--r--   0 runner    (1001) docker     (123)    19757 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/src/Collection.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.227898 chromadb-0.4.1/clients/js/src/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/src/embeddings/CohereEmbeddingFunction.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/src/embeddings/IEmbeddingFunction.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/src/embeddings/OpenAIEmbeddingFunction.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/src/embeddings/TransformersEmbeddingFunction.ts
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3402 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/src/embeddings/WebAIEmbeddingFunction.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.227898 chromadb-0.4.1/clients/js/src/generated/
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/src/generated/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    54547 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/src/generated/api.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/src/generated/configuration.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/src/generated/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/src/generated/models.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/src/generated/runtime.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/src/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/src/types.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/src/utils.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.231898 chromadb-0.4.1/clients/js/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/test/add.collections.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/test/client.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/test/collection.client.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/test/collection.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/test/data.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/test/delete.collection.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/test/get.collection.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/test/initClient.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/test/peek.collection.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/test/query.collection.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/test/update.collection.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/test/upsert.collections.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/tsconfig.module.json
+-rw-r--r--   0 runner    (1001) docker     (123)   156893 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/js/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.235898 chromadb-0.4.1/clients/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/python/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1257 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/python/build_python_thin_client.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      850 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/python/integration-test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/python/is_thin_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-18 23:29:22.000000 chromadb-0.4.1/clients/python/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-18 23:29:22.000000 chromadb-0.4.1/docker-compose.server.example.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-18 23:29:22.000000 chromadb-0.4.1/docker-compose.test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-18 23:29:22.000000 chromadb-0.4.1/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.235898 chromadb-0.4.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-18 23:29:22.000000 chromadb-0.4.1/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.235898 chromadb-0.4.1/examples/basic_functionality/
+-rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-07-18 23:29:22.000000 chromadb-0.4.1/examples/basic_functionality/alternative_embeddings.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-07-18 23:29:22.000000 chromadb-0.4.1/examples/basic_functionality/local_persistence.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-07-18 23:29:22.000000 chromadb-0.4.1/examples/basic_functionality/where_filtering.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.171897 chromadb-0.4.1/examples/deployments/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.239898 chromadb-0.4.1/examples/deployments/google-cloud-compute/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-18 23:29:22.000000 chromadb-0.4.1/examples/deployments/google-cloud-compute/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-18 23:29:22.000000 chromadb-0.4.1/examples/deployments/google-cloud-compute/chroma.tf
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-18 23:29:22.000000 chromadb-0.4.1/examples/deployments/google-cloud-compute/main.tf
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-18 23:29:22.000000 chromadb-0.4.1/examples/deployments/google-cloud-compute/startup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-18 23:29:22.000000 chromadb-0.4.1/examples/deployments/google-cloud-compute/variables.tf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.171897 chromadb-0.4.1/examples/use_with/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:29:37.239898 chromadb-0.4.1/examples/use_with/cohere/
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-18 23:29:22.000000 chromadb-0.4.1/examples/use_with/cohere/cohere_js.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-07-18 23:29:22.000000 chromadb-0.4.1/examples/use_with/cohere/cohere_python.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-18 23:29:22.000000 chromadb-0.4.1/examples/use_with/cohere/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-18 23:29:22.000000 chromadb-0.4.1/log_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-18 23:29:22.000000 chromadb-0.4.1/pull_request_template.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-18 23:29:22.000000 chromadb-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-18 23:29:22.000000 chromadb-0.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-18 23:29:22.000000 chromadb-0.4.1/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 23:29:37.239898 chromadb-0.4.1/setup.cfg
```

### Comparing `chromadb-0.4.0/.github/ISSUE_TEMPLATE/bug_report.yaml` & `chromadb-0.4.1/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/.github/ISSUE_TEMPLATE/feature_request.yaml` & `chromadb-0.4.1/.github/ISSUE_TEMPLATE/feature_request.yaml`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/.github/ISSUE_TEMPLATE/installation_trouble.yaml` & `chromadb-0.4.1/.github/ISSUE_TEMPLATE/installation_trouble.yaml`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/.github/workflows/chroma-client-integration-test.yml` & `chromadb-0.4.1/.github/workflows/chroma-client-integration-test.yml`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/.github/workflows/chroma-integration-test.yml` & `chromadb-0.4.1/.github/workflows/chroma-integration-test.yml`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/.github/workflows/chroma-release-python-client.yml` & `chromadb-0.4.1/.github/workflows/chroma-release-python-client.yml`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/.github/workflows/chroma-release.yml` & `chromadb-0.4.1/.github/workflows/chroma-release.yml`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/.github/workflows/chroma-test.yml` & `chromadb-0.4.1/.github/workflows/chroma-test.yml`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/.github/workflows/pr-review-checklist.yml` & `chromadb-0.4.1/.github/workflows/pr-review-checklist.yml`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/.pre-commit-config.yaml` & `chromadb-0.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/.vscode/settings.json` & `chromadb-0.4.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/DEVELOP.md` & `chromadb-0.4.1/DEVELOP.md`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/Dockerfile` & `chromadb-0.4.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/LICENSE` & `chromadb-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/PKG-INFO` & `chromadb-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromadb
-Version: 0.4.0
+Version: 0.4.1
 Summary: Chroma.
 Author-email: Jeff Huber <jeff@trychroma.com>, Anton Troynikov <anton@trychroma.com>
 Project-URL: Homepage, https://github.com/chroma-core/chroma
 Project-URL: Bug Tracker, https://github.com/chroma-core/chroma/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: chromadb Version: 0.4.0 Summary: Chroma. Author-
+Metadata-Version: 2.1 Name: chromadb Version: 0.4.1 Summary: Chroma. Author-
 email: Jeff Huber
 trychroma.com>, Anton Troynikov
 trychroma.com> Project-URL: Homepage, https://github.com/chroma-core/chroma
 Project-URL: Bug Tracker, https://github.com/chroma-core/chroma/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
```

### Comparing `chromadb-0.4.0/README.md` & `chromadb-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/RELEASE_PROCESS.md` & `chromadb-0.4.1/RELEASE_PROCESS.md`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/bin/generate_cloudformation.py` & `chromadb-0.4.1/bin/generate_cloudformation.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,20 +18,14 @@
 
 path = os.path.dirname(os.path.realpath(__file__))
 version = subprocess.check_output(f"{path}/version").decode("ascii").strip()
 
 with open(f"{path}/templates/docker-compose.yml") as f:
     docker_compose_file = str(f.read())
 
-with open(f"{path}/../config/backup_disk.xml") as f:
-    backup_disk_config = str(f.read())
-
-with open(f"{path}/../config/chroma_users.xml") as f:
-    chroma_users_config = str(f.read())
-
 
 cloud_config_script = """
 #cloud-config
 cloud_final_modules:
 - [scripts-user, always]
 """
 
@@ -47,22 +41,14 @@
 
 cat << EOF > /home/ec2-user/docker-compose.yml
 {docker_compose_file}
 EOF
 
 mkdir /home/ec2-user/config
 
-cat << EOF > /home/ec2-user/config/backup_disk.xml
-{backup_disk_config}
-EOF
-
-cat << EOF > /home/ec2-user/config/chroma_users.xml
-{chroma_users_config}
-EOF
-
 docker-compose -f /home/ec2-user/docker-compose.yml up -d
 """
 
 userdata = f"""Content-Type: multipart/mixed; boundary="//"
 MIME-Version: 1.0
 
 --//
```

### Comparing `chromadb-0.4.0/chromadb/__init__.py` & `chromadb-0.4.1/chromadb/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from chromadb.config import Settings, System
 from chromadb.api import API
 
 logger = logging.getLogger(__name__)
 
 __settings = Settings()
 
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 
 
 def configure(**kwargs) -> None:  # type: ignore
     """Override Chroma's default settings, environment variables or .env files"""
     global __settings
     __settings = chromadb.config.Settings(**kwargs)
```

### Comparing `chromadb-0.4.0/chromadb/api/__init__.py` & `chromadb-0.4.1/chromadb/api/__init__.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/api/fastapi.py` & `chromadb-0.4.1/chromadb/api/fastapi.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/api/models/Collection.py` & `chromadb-0.4.1/chromadb/api/models/Collection.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/api/segment.py` & `chromadb-0.4.1/chromadb/api/segment.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/api/types.py` & `chromadb-0.4.1/chromadb/api/types.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/config.py` & `chromadb-0.4.1/chromadb/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,26 @@
 except ImportError:
     is_thin_client = False
 
 
 logger = logging.getLogger(__name__)
 
 
-LEGACY_ERROR = "You are using a deprecated configuration of Chroma. Please pip install chroma-migrate and run `chroma-migrate` to upgrade your configuration. See https://docs.trychroma.com/migration for more information or join our discord at https://discord.gg/8g5FESbj for help!"
+LEGACY_ERROR = """\033[91mYou are using a deprecated configuration of Chroma.
+
+\033[94mIf you do not have data you wish to migrate, you only need to change how you construct
+your Chroma client. Please see the "New Clients" section of https://docs.trychroma.com/migration.
+________________________________________________________________________________________________
+
+If you do have data you wish to migrate, we have a migration tool you can use in order to
+migrate your data to the new Chroma architecture.
+Please `pip install chroma-migrate` and run `chroma-migrate` to migrate your data and then
+change how you construct your Chroma client.
+
+See https://docs.trychroma.com/migration for more information or join our discord at https://discord.gg/8g5FESbj for help!\033[0m"""
 
 _legacy_config_keys = {
     "chroma_db_impl",
 }
 
 _legacy_config_values = {
     "duckdb",
```

### Comparing `chromadb-0.4.0/chromadb/db/__init__.py` & `chromadb-0.4.1/chromadb/db/__init__.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/db/base.py` & `chromadb-0.4.1/chromadb/db/base.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/db/impl/sqlite.py` & `chromadb-0.4.1/chromadb/db/impl/sqlite.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/db/impl/sqlite_pool.py` & `chromadb-0.4.1/chromadb/db/impl/sqlite_pool.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/db/migrations.py` & `chromadb-0.4.1/chromadb/db/migrations.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/db/mixins/embeddings_queue.py` & `chromadb-0.4.1/chromadb/db/mixins/embeddings_queue.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/db/mixins/sysdb.py` & `chromadb-0.4.1/chromadb/db/mixins/sysdb.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/db/system.py` & `chromadb-0.4.1/chromadb/db/system.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/errors.py` & `chromadb-0.4.1/chromadb/errors.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/experimental/density_relevance.ipynb` & `chromadb-0.4.1/chromadb/experimental/density_relevance.ipynb`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/ingest/__init__.py` & `chromadb-0.4.1/chromadb/ingest/__init__.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/migrations/metadb/00001-embedding-metadata.sqlite.sql` & `chromadb-0.4.1/chromadb/migrations/metadb/00001-embedding-metadata.sqlite.sql`

 * *Files 20% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 );
 
 CREATE TABLE max_seq_id (
     segment_id TEXT PRIMARY KEY,
     seq_id BLOB NOT NULL
 );
 
-CREATE VIRTUAL TABLE embedding_fulltext USING fts5(id, string_value, tokenize="trigram");
+CREATE VIRTUAL TABLE embedding_fulltext USING fts5(id, string_value);
```

### Comparing `chromadb-0.4.0/chromadb/segment/__init__.py` & `chromadb-0.4.1/chromadb/segment/__init__.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/segment/impl/manager/local.py` & `chromadb-0.4.1/chromadb/segment/impl/manager/local.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/segment/impl/metadata/sqlite.py` & `chromadb-0.4.1/chromadb/segment/impl/metadata/sqlite.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/segment/impl/vector/batch.py` & `chromadb-0.4.1/chromadb/segment/impl/vector/batch.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/segment/impl/vector/brute_force_index.py` & `chromadb-0.4.1/chromadb/segment/impl/vector/brute_force_index.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/segment/impl/vector/hnsw_params.py` & `chromadb-0.4.1/chromadb/segment/impl/vector/hnsw_params.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/segment/impl/vector/local_hnsw.py` & `chromadb-0.4.1/chromadb/segment/impl/vector/local_hnsw.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/segment/impl/vector/local_persistent_hnsw.py` & `chromadb-0.4.1/chromadb/segment/impl/vector/local_persistent_hnsw.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/server/fastapi/__init__.py` & `chromadb-0.4.1/chromadb/server/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/server/fastapi/types.py` & `chromadb-0.4.1/chromadb/server/fastapi/types.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/telemetry/__init__.py` & `chromadb-0.4.1/chromadb/telemetry/__init__.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/telemetry/events.py` & `chromadb-0.4.1/chromadb/telemetry/events.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/telemetry/posthog.py` & `chromadb-0.4.1/chromadb/telemetry/posthog.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/test/conftest.py` & `chromadb-0.4.1/chromadb/test/conftest.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/test/db/test_base.py` & `chromadb-0.4.1/chromadb/test/db/test_base.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/test/db/test_migrations.py` & `chromadb-0.4.1/chromadb/test/db/test_migrations.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/test/db/test_system.py` & `chromadb-0.4.1/chromadb/test/db/test_system.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/test/ingest/test_producer_consumer.py` & `chromadb-0.4.1/chromadb/test/ingest/test_producer_consumer.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/test/property/invariants.py` & `chromadb-0.4.1/chromadb/test/property/invariants.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/test/property/strategies.py` & `chromadb-0.4.1/chromadb/test/property/strategies.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/test/property/test_add.py` & `chromadb-0.4.1/chromadb/test/property/test_add.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/test/property/test_collections.py` & `chromadb-0.4.1/chromadb/test/property/test_collections.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/test/property/test_cross_version_persist.py` & `chromadb-0.4.1/chromadb/test/property/test_cross_version_persist.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/test/property/test_embeddings.py` & `chromadb-0.4.1/chromadb/test/property/test_embeddings.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/test/property/test_filtering.py` & `chromadb-0.4.1/chromadb/test/property/test_filtering.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/test/property/test_persist.py` & `chromadb-0.4.1/chromadb/test/property/test_persist.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/test/segment/test_metadata.py` & `chromadb-0.4.1/chromadb/test/segment/test_metadata.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/test/segment/test_vector.py` & `chromadb-0.4.1/chromadb/test/segment/test_vector.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/test/test_api.py` & `chromadb-0.4.1/chromadb/test/test_api.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/test/test_chroma.py` & `chromadb-0.4.1/chromadb/test/test_chroma.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/test/test_client.py` & `chromadb-0.4.1/chromadb/test/test_client.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/test/test_config.py` & `chromadb-0.4.1/chromadb/test/test_config.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/test/test_multithreaded.py` & `chromadb-0.4.1/chromadb/test/test_multithreaded.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/test/utils/test_messagid.py` & `chromadb-0.4.1/chromadb/test/utils/test_messagid.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/types.py` & `chromadb-0.4.1/chromadb/types.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/utils/distance_functions.py` & `chromadb-0.4.1/chromadb/utils/distance_functions.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/utils/embedding_functions.py` & `chromadb-0.4.1/chromadb/utils/embedding_functions.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/utils/messageid.py` & `chromadb-0.4.1/chromadb/utils/messageid.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb/utils/read_write_lock.py` & `chromadb-0.4.1/chromadb/utils/read_write_lock.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/chromadb.egg-info/PKG-INFO` & `chromadb-0.4.1/chromadb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromadb
-Version: 0.4.0
+Version: 0.4.1
 Summary: Chroma.
 Author-email: Jeff Huber <jeff@trychroma.com>, Anton Troynikov <anton@trychroma.com>
 Project-URL: Homepage, https://github.com/chroma-core/chroma
 Project-URL: Bug Tracker, https://github.com/chroma-core/chroma/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: chromadb Version: 0.4.0 Summary: Chroma. Author-
+Metadata-Version: 2.1 Name: chromadb Version: 0.4.1 Summary: Chroma. Author-
 email: Jeff Huber
 trychroma.com>, Anton Troynikov
 trychroma.com> Project-URL: Homepage, https://github.com/chroma-core/chroma
 Project-URL: Bug Tracker, https://github.com/chroma-core/chroma/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
```

### Comparing `chromadb-0.4.0/chromadb.egg-info/SOURCES.txt` & `chromadb-0.4.1/chromadb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/clients/js/DEVELOP.md` & `chromadb-0.4.1/clients/js/DEVELOP.md`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/clients/js/LICENSE` & `chromadb-0.4.1/clients/js/LICENSE`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/clients/js/README.md` & `chromadb-0.4.1/clients/js/README.md`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/clients/js/examples/browser/app.ts` & `chromadb-0.4.1/clients/js/examples/browser/app.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/clients/js/examples/browser/index.html` & `chromadb-0.4.1/clients/js/examples/browser/index.html`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/clients/js/examples/browser/yarn.lock` & `chromadb-0.4.1/clients/js/examples/browser/yarn.lock`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/clients/js/examples/node/app.js` & `chromadb-0.4.1/clients/js/examples/node/app.js`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/clients/js/examples/node/yarn.lock` & `chromadb-0.4.1/clients/js/examples/node/yarn.lock`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/clients/js/genapi.sh` & `chromadb-0.4.1/clients/js/genapi.sh`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/clients/js/package-lock.json` & `chromadb-0.4.1/clients/js/package-lock.json`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/clients/js/package.json` & `chromadb-0.4.1/clients/js/package.json`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/clients/js/src/ChromaClient.ts` & `chromadb-0.4.1/clients/js/src/ChromaClient.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/clients/js/src/Collection.ts` & `chromadb-0.4.1/clients/js/src/Collection.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/clients/js/src/embeddings/CohereEmbeddingFunction.ts` & `chromadb-0.4.1/clients/js/src/embeddings/CohereEmbeddingFunction.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/clients/js/src/embeddings/OpenAIEmbeddingFunction.ts` & `chromadb-0.4.1/clients/js/src/embeddings/OpenAIEmbeddingFunction.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/clients/js/src/embeddings/TransformersEmbeddingFunction.ts` & `chromadb-0.4.1/clients/js/src/embeddings/TransformersEmbeddingFunction.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/clients/js/src/embeddings/WebAIEmbeddingFunction.ts` & `chromadb-0.4.1/clients/js/src/embeddings/WebAIEmbeddingFunction.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/clients/js/src/generated/README.md` & `chromadb-0.4.1/clients/js/src/generated/README.md`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/clients/js/src/generated/api.ts` & `chromadb-0.4.1/clients/js/src/generated/api.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/clients/js/src/generated/configuration.ts` & `chromadb-0.4.1/clients/js/src/generated/configuration.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/clients/js/src/generated/models.ts` & `chromadb-0.4.1/clients/js/src/generated/models.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/clients/js/src/generated/runtime.ts` & `chromadb-0.4.1/clients/js/src/generated/runtime.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/clients/js/src/types.ts` & `chromadb-0.4.1/clients/js/src/types.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/clients/js/src/utils.ts` & `chromadb-0.4.1/clients/js/src/utils.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/clients/js/test/add.collections.test.ts` & `chromadb-0.4.1/clients/js/test/add.collections.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/clients/js/test/client.test.ts` & `chromadb-0.4.1/clients/js/test/client.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/clients/js/test/collection.client.test.ts` & `chromadb-0.4.1/clients/js/test/collection.client.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/clients/js/test/collection.test.ts` & `chromadb-0.4.1/clients/js/test/collection.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/clients/js/test/delete.collection.test.ts` & `chromadb-0.4.1/clients/js/test/delete.collection.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/clients/js/test/get.collection.test.ts` & `chromadb-0.4.1/clients/js/test/get.collection.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/clients/js/test/peek.collection.test.ts` & `chromadb-0.4.1/clients/js/test/peek.collection.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/clients/js/test/query.collection.test.ts` & `chromadb-0.4.1/clients/js/test/query.collection.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/clients/js/test/update.collection.test.ts` & `chromadb-0.4.1/clients/js/test/update.collection.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/clients/js/test/upsert.collections.test.ts` & `chromadb-0.4.1/clients/js/test/upsert.collections.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/clients/js/yarn.lock` & `chromadb-0.4.1/clients/js/yarn.lock`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/clients/python/README.md` & `chromadb-0.4.1/clients/python/README.md`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/clients/python/build_python_thin_client.sh` & `chromadb-0.4.1/clients/python/build_python_thin_client.sh`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/clients/python/integration-test.sh` & `chromadb-0.4.1/clients/python/integration-test.sh`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/clients/python/pyproject.toml` & `chromadb-0.4.1/clients/python/pyproject.toml`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/docker-compose.test.yml` & `chromadb-0.4.1/docker-compose.test.yml`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/examples/README.md` & `chromadb-0.4.1/examples/README.md`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/examples/basic_functionality/alternative_embeddings.ipynb` & `chromadb-0.4.1/examples/basic_functionality/alternative_embeddings.ipynb`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/examples/basic_functionality/local_persistence.ipynb` & `chromadb-0.4.1/examples/basic_functionality/local_persistence.ipynb`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/examples/basic_functionality/where_filtering.ipynb` & `chromadb-0.4.1/examples/basic_functionality/where_filtering.ipynb`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/examples/deployments/google-cloud-compute/README.md` & `chromadb-0.4.1/examples/deployments/google-cloud-compute/README.md`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/examples/deployments/google-cloud-compute/chroma.tf` & `chromadb-0.4.1/examples/deployments/google-cloud-compute/chroma.tf`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/examples/deployments/google-cloud-compute/startup.sh` & `chromadb-0.4.1/examples/deployments/google-cloud-compute/startup.sh`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/examples/use_with/cohere/cohere_js.js` & `chromadb-0.4.1/examples/use_with/cohere/cohere_js.js`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/examples/use_with/cohere/cohere_python.ipynb` & `chromadb-0.4.1/examples/use_with/cohere/cohere_python.ipynb`

 * *Files identical despite different names*

### Comparing `chromadb-0.4.0/pyproject.toml` & `chromadb-0.4.1/pyproject.toml`

 * *Files identical despite different names*

