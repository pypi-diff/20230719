# Comparing `tmp/dao-analyzer-1.2.7.dev6.tar.gz` & `tmp/dao-analyzer-1.2.7.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dao-analyzer-1.2.7.dev6.tar", last modified: Tue May 16 07:25:07 2023, max compression
+gzip compressed data, was "dao-analyzer-1.2.7.dev7.tar", last modified: Wed Jul 19 15:55:56 2023, max compression
```

## Comparing `dao-analyzer-1.2.7.dev6.tar` & `dao-analyzer-1.2.7.dev7.tar`

### file list

```diff
@@ -1,440 +1,413 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:07.059643 dao-analyzer-1.2.7.dev6/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/.envrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:06.955642 dao-analyzer-1.2.7.dev6/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:06.955642 dao-analyzer-1.2.7.dev6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/.github/workflows/check_continue.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/.github/workflows/update_aragon_names.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/.hintrc
--rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/ABOUT.md
--rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9861 2023-05-16 07:25:07.059643 dao-analyzer-1.2.7.dev6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:06.955642 dao-analyzer-1.2.7.dev6/cache_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/cache_scripts/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/cache_scripts/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/cache_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/cache_scripts/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:06.959642 dao-analyzer-1.2.7.dev6/cache_scripts/aragon/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/cache_scripts/aragon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7412 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/cache_scripts/aragon/dao_names.json
--rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/cache_scripts/aragon/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/cache_scripts/argparser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:06.959642 dao-analyzer-1.2.7.dev6/cache_scripts/common/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/cache_scripts/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/cache_scripts/common/api_requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/cache_scripts/common/blockscout.py
--rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/cache_scripts/common/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/cache_scripts/common/cryptocompare.py
--rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/cache_scripts/common/graphql.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/cache_scripts/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:06.959642 dao-analyzer-1.2.7.dev6/cache_scripts/daohaus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/cache_scripts/daohaus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/cache_scripts/daohaus/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:06.959642 dao-analyzer-1.2.7.dev6/cache_scripts/daostack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/cache_scripts/daostack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/cache_scripts/daostack/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/cache_scripts/endpoints.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     5042 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/cache_scripts/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/cache_scripts/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:06.939642 dao-analyzer-1.2.7.dev6/dao_analyzer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:06.963642 dao-analyzer-1.2.7.dev6/dao_analyzer/web/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-16 07:25:06.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:06.963642 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:06.963642 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:06.963642 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/business/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/business/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16209 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/business/app_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:06.963642 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/business/metric_adapter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/business/metric_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/business/metric_adapter/asset_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/business/metric_adapter/asset_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/business/metric_adapter/basic_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/business/metric_adapter/cast_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/business/metric_adapter/installed_apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/business/metric_adapter/vote_outcome.py
--rw-r--r--   0 runner    (1001) docker     (123)   399465 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/class_diagram.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:06.967642 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/data_access/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/data_access/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:06.967642 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/data_access/daos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/data_access/daos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:06.967642 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/metric_dao_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/srcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:06.971642 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_active_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_active_token_holders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_active_voters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_approval_vote_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_assets_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_assets_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_cast_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_casted_votes_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_casted_votes_voters_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_installed_apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_new_additions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_organization_activity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_total_token_holders.py
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_vote_outcome.py
--rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/data_access/daos/platform_dao.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:06.971642 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/presentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/presentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:06.971642 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/resources/strings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:06.971642 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:06.971642 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:06.971642 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/api/graphql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/api/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/api/graphql/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/api/graphql/query_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:06.971642 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/business/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/business/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/business/i_metric_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/business/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:06.971642 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/business/transfers/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/business/transfers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/business/transfers/hierarchical_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/business/transfers/n_stacked_serie.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:06.975642 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/business/transfers/organization/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/business/transfers/organization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/business/transfers/organization/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/business/transfers/organization/organization_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/business/transfers/organization/organization_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/business/transfers/organization/participation_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/business/transfers/organization/platform.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/business/transfers/serie.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/business/transfers/stacked_serie.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/business/transfers/tabular_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:06.975642 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/data_access/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/data_access/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:06.975642 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/data_access/daos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/data_access/daos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:06.975642 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/data_access/daos/metric/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/data_access/daos/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/data_access/daos/metric/metric_dao.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/data_access/daos/metric/srcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:06.975642 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/imetric_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/st_assets_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/st_assets_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/data_access/daos/platform_dao.py
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/data_access/pandas_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:06.975642 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/data_access/requesters/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/data_access/requesters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/data_access/requesters/cache_requester.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/data_access/requesters/irequester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/data_access/requesters/join_cache_requester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:06.975642 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:06.979642 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/about_view/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/about_view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/about_view/about_view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:06.979642 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/charts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/charts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/charts/chart_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/charts/chart_sum_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/charts/dt_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:06.979642 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/chart_pane_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/chart_pane_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/data_table_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/data_table_layout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:06.983642 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/figure/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/figure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/figure/bar_figure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/figure/calplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/figure/double_scatter_figure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/figure/figure.py
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/figure/figure_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/figure/multi_bar_figure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/figure/treemap_figure.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/ilayout.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/layout_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:06.983642 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/dashboard_view/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/dashboard_view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/dashboard_view/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/dashboard_view/dashboard_view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:06.983642 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/main_view/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/main_view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/main_view/main_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/main_view/main_view_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:06.983642 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/resources/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/resources/strings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:06.983642 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:06.983642 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/business/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/business/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16026 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/business/app_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:06.991642 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/business/metric_adapter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/business/metric_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/business/metric_adapter/asset_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/business/metric_adapter/asset_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/business/metric_adapter/basic_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/business/metric_adapter/proposal_outcome.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/business/metric_adapter/proposal_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/business/metric_adapter/votes_type.py
--rw-r--r--   0 runner    (1001) docker     (123)   418772 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/class_diagram.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:06.991642 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/data_access/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/data_access/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:06.991642 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:06.995643 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/metric_dao_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/srcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:06.999642 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_active_members.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_active_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_active_voters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_approval_proposal_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_assets_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_assets_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_new_additions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_organization_activity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_proposal_outcome.py
--rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_proposal_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_total_members.py
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_voters_percentage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_votes_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_votes_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_votes_voters_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/platform_dao.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:06.999642 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/presentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/presentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:07.003642 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/resources/strings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:07.003642 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:07.003642 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/business/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/business/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17742 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/business/app_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:07.007643 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/business/metric_adapter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/business/metric_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/business/metric_adapter/asset_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/business/metric_adapter/asset_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/business/metric_adapter/majority_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/business/metric_adapter/metric_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/business/metric_adapter/proposal_boost_outcome.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/business/metric_adapter/success_ratio_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/business/metric_adapter/vote_type.py
--rw-r--r--   0 runner    (1001) docker     (123)   461806 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/class_diagram.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:07.007643 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/data_access/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/data_access/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:07.007643 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/data_access/daos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/data_access/daos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:07.007643 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/metric_dao_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/srcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:07.015643 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_active_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_active_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_approval_proposal_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_assets_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_assets_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_different_voters_stakers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_organization_activity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_proposal_majority.py
--rw-r--r--   0 runner    (1001) docker     (123)     9374 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_proposal_outcome.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_time_serie.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_total_reputation_holders.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_total_votes_stakes_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_voters_percentage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_votes_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_votes_voters_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5611 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/data_access/daos/platform_dao.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:07.015643 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/presentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/presentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:07.015643 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/resources/strings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:07.023643 dao-analyzer-1.2.7.dev6/dao_analyzer/web/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/assets/ABOUT.md
--rw-r--r--   0 runner    (1001) docker     (123)    65944 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/assets/aragon.png
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/assets/callbacks.js
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/assets/cc-by.png
--rw-r--r--   0 runner    (1001) docker     (123)    18045 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/assets/dao-analyzer_header.svg
--rw-r--r--   0 runner    (1001) docker     (123)    36174 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/assets/dao-analyzer_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    54135 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/assets/daohaus.png
--rw-r--r--   0 runner    (1001) docker     (123)    16481 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/assets/daostack.png
--rw-r--r--   0 runner    (1001) docker     (123)   101409 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/assets/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    58578 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/assets/github_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/assets/ico-github.svg
--rw-r--r--   0 runner    (1001) docker     (123)    17972 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/assets/img_header.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   129808 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/assets/kaggle_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/assets/logo-GPL.png
--rw-r--r--   0 runner    (1001) docker     (123)    10979 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/assets/logo-erc.png
--rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/assets/logo-grasia.png
--rw-r--r--   0 runner    (1001) docker     (123)    12180 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/assets/logo-ministerio.png
--rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/assets/logo-ucm.png
--rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/assets/logo_dao_analyzer.png
--rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/assets/logo_dao_analyzer.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/assets/logo_dao_analyzer_orig.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10237 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/assets/stylesheet.css
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer/web/matomo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:06.959642 dao-analyzer-1.2.7.dev6/dao_analyzer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9861 2023-05-16 07:25:06.000000 dao-analyzer-1.2.7.dev6/dao_analyzer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19562 2023-05-16 07:25:06.000000 dao-analyzer-1.2.7.dev6/dao_analyzer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 07:25:06.000000 dao-analyzer-1.2.7.dev6/dao_analyzer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-16 07:25:06.000000 dao-analyzer-1.2.7.dev6/dao_analyzer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-16 07:25:06.000000 dao-analyzer-1.2.7.dev6/dao_analyzer.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-16 07:25:06.000000 dao-analyzer-1.2.7.dev6/dao_analyzer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-16 07:25:06.000000 dao-analyzer-1.2.7.dev6/dao_analyzer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:07.027643 dao-analyzer-1.2.7.dev6/dao_analyzer_components/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer_components/.babelrc
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer_components/.eslintrc
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer_components/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer_components/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer_components/_validate_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:07.031643 dao-analyzer-1.2.7.dev6/dao_analyzer_components/dao_analyzer_components/
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-16 07:24:46.000000 dao-analyzer-1.2.7.dev6/dao_analyzer_components/dao_analyzer_components/DAOInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-16 07:24:46.000000 dao-analyzer-1.2.7.dev6/dao_analyzer_components/dao_analyzer_components/DataPoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-16 07:24:46.000000 dao-analyzer-1.2.7.dev6/dao_analyzer_components/dao_analyzer_components/ParticipationStat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-16 07:24:46.000000 dao-analyzer-1.2.7.dev6/dao_analyzer_components/dao_analyzer_components/PlatformInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-05-16 07:24:46.000000 dao-analyzer-1.2.7.dev6/dao_analyzer_components/dao_analyzer_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-16 07:24:46.000000 dao-analyzer-1.2.7.dev6/dao_analyzer_components/dao_analyzer_components/_imports_.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-16 07:24:46.000000 dao-analyzer-1.2.7.dev6/dao_analyzer_components/dao_analyzer_components/dao_analyzer_components.css
--rw-r--r--   0 runner    (1001) docker     (123)    13291 2023-05-16 07:24:46.000000 dao-analyzer-1.2.7.dev6/dao_analyzer_components/dao_analyzer_components/dao_analyzer_components.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    17779 2023-05-16 07:24:46.000000 dao-analyzer-1.2.7.dev6/dao_analyzer_components/dao_analyzer_components/dao_analyzer_components.min.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     5984 2023-05-16 07:24:46.000000 dao-analyzer-1.2.7.dev6/dao_analyzer_components/dao_analyzer_components/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-05-16 07:24:46.000000 dao-analyzer-1.2.7.dev6/dao_analyzer_components/dao_analyzer_components/package-info.json
--rw-r--r--   0 runner    (1001) docker     (123)   630253 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer_components/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer_components/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:07.031643 dao-analyzer-1.2.7.dev6/dao_analyzer_components/public/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer_components/public/index.html
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer_components/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer_components/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:06.947642 dao-analyzer-1.2.7.dev6/dao_analyzer_components/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:07.035643 dao-analyzer-1.2.7.dev6/dao_analyzer_components/src/demo/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer_components/src/demo/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:07.035643 dao-analyzer-1.2.7.dev6/dao_analyzer_components/src/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:07.035643 dao-analyzer-1.2.7.dev6/dao_analyzer_components/src/lib/components/
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer_components/src/lib/components/DAOInfo.jsx
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer_components/src/lib/components/DataPoint.jsx
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer_components/src/lib/components/ParticipationStat.jsx
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer_components/src/lib/components/PlatformInfo.jsx
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer_components/src/lib/index.js
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer_components/webpack.config.js
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/dao_analyzer_components/webpack.demo.config.js
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/gunicorn_config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      197 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/init.sh
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:07.039643 dao-analyzer-1.2.7.dev6/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:07.039643 dao-analyzer-1.2.7.dev6/scripts/archive/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/scripts/archive/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)   339476 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/scripts/archive/names.ipynb
--rwxr-xr-x   0 runner    (1001) docker     (123)     1010 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/scripts/archive/uploadToKaggle.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1790 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/scripts/checkContinue.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     4349 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/scripts/datawarehouseDiff.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      251 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/scripts/deploy.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      111 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/scripts/printArrow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1148 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/scripts/updateAragonNames.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2900 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/scripts/uploadDataWarehouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-05-16 07:25:07.059643 dao-analyzer-1.2.7.dev6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:07.039643 dao-analyzer-1.2.7.dev6/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:07.039643 dao-analyzer-1.2.7.dev6/test/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/mocks/api_requester_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/mocks/unix_date_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:07.039643 dao-analyzer-1.2.7.dev6/test/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:07.043643 dao-analyzer-1.2.7.dev6/test/unit/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/unit/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:07.043643 dao-analyzer-1.2.7.dev6/test/unit/apps/aragon/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/unit/apps/aragon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:07.043643 dao-analyzer-1.2.7.dev6/test/unit/apps/aragon/data_access/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/unit/apps/aragon/data_access/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:07.043643 dao-analyzer-1.2.7.dev6/test/unit/apps/aragon/data_access/daos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/unit/apps/aragon/data_access/daos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:07.043643 dao-analyzer-1.2.7.dev6/test/unit/apps/aragon/data_access/daos/metric/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/unit/apps/aragon/data_access/daos/metric/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:07.043643 dao-analyzer-1.2.7.dev6/test/unit/apps/aragon/data_access/daos/metric/strategy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/unit/apps/aragon/data_access/daos/metric/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/unit/apps/aragon/data_access/daos/metric/strategy/test_aragon_st_new_additions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_active_organization_aragon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_active_token_holders.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_cast_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_installed_apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_vote_outcome.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:07.047643 dao-analyzer-1.2.7.dev6/test/unit/apps/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/unit/apps/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:07.047643 dao-analyzer-1.2.7.dev6/test/unit/apps/common/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/unit/apps/common/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:07.047643 dao-analyzer-1.2.7.dev6/test/unit/apps/common/api/graphql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/unit/apps/common/api/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/unit/apps/common/api/graphql/test_query_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:07.047643 dao-analyzer-1.2.7.dev6/test/unit/apps/common/business/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/unit/apps/common/business/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:07.047643 dao-analyzer-1.2.7.dev6/test/unit/apps/common/business/transfers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/unit/apps/common/business/transfers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/unit/apps/common/business/transfers/test_organization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:07.047643 dao-analyzer-1.2.7.dev6/test/unit/apps/common/data_access/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/unit/apps/common/data_access/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:07.047643 dao-analyzer-1.2.7.dev6/test/unit/apps/common/data_access/daos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/unit/apps/common/data_access/daos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:07.047643 dao-analyzer-1.2.7.dev6/test/unit/apps/daohaus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/unit/apps/daohaus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:07.047643 dao-analyzer-1.2.7.dev6/test/unit/apps/daohaus/data_access/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/unit/apps/daohaus/data_access/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:07.051643 dao-analyzer-1.2.7.dev6/test/unit/apps/daohaus/data_access/daos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/unit/apps/daohaus/data_access/daos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:07.051643 dao-analyzer-1.2.7.dev6/test/unit/apps/daohaus/data_access/daos/metric/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/unit/apps/daohaus/data_access/daos/metric/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:07.051643 dao-analyzer-1.2.7.dev6/test/unit/apps/daohaus/data_access/daos/metric/strategy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/unit/apps/daohaus/data_access/daos/metric/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_active_members.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_active_organization_daohaus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_active_voters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_dproposal_outcome.py
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_new_additions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_proposal_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_total_members.py
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_votes_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:07.051643 dao-analyzer-1.2.7.dev6/test/unit/apps/daostack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/unit/apps/daostack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:07.055643 dao-analyzer-1.2.7.dev6/test/unit/apps/daostack/data_access/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/unit/apps/daostack/data_access/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:07.055643 dao-analyzer-1.2.7.dev6/test/unit/apps/daostack/data_access/daos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/unit/apps/daostack/data_access/daos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:07.055643 dao-analyzer-1.2.7.dev6/test/unit/apps/daostack/data_access/daos/metric/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/unit/apps/daostack/data_access/daos/metric/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:07.055643 dao-analyzer-1.2.7.dev6/test/unit/apps/daostack/data_access/daos/metric/strategy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/unit/apps/daostack/data_access/daos/metric/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_active_organization_daostack.py
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_active_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_diff_voters_stakers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_proposal_majority.py
--rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_proposal_outcome.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_time_serie.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_voters_percentage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:07.059643 dao-analyzer-1.2.7.dev6/test/unit/apps/daostack/data_access/requesters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/unit/apps/daostack/data_access/requesters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:07.059643 dao-analyzer-1.2.7.dev6/test/unit/components/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-16 07:24:45.000000 dao-analyzer-1.2.7.dev6/test/unit/components/test_dao_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.981898 dao-analyzer-1.2.7.dev7/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/.envrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.925896 dao-analyzer-1.2.7.dev7/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.925896 dao-analyzer-1.2.7.dev7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/.github/workflows/check_continue.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/.github/workflows/update_aragon_names.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/.hintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/ABOUT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9904 2023-07-19 15:55:56.981898 dao-analyzer-1.2.7.dev7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8673 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.909896 dao-analyzer-1.2.7.dev7/dao_analyzer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.925896 dao-analyzer-1.2.7.dev7/dao_analyzer/web/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-19 15:55:56.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.925896 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.925896 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.929896 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/business/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/business/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16209 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/business/app_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.933896 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/business/metric_adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/business/metric_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/business/metric_adapter/asset_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/business/metric_adapter/asset_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/business/metric_adapter/basic_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/business/metric_adapter/cast_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/business/metric_adapter/installed_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/business/metric_adapter/vote_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)   399465 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/class_diagram.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.933896 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/data_access/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/data_access/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.933896 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/data_access/daos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/data_access/daos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.933896 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/metric_dao_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/srcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.937896 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_active_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_active_token_holders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_active_voters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_approval_vote_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_assets_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_assets_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_cast_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_casted_votes_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_casted_votes_voters_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_installed_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_new_additions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_organization_activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_total_token_holders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_vote_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/data_access/daos/platform_dao.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.937896 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/presentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/presentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.937896 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/resources/strings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.937896 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.937896 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.937896 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/api/graphql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/api/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/api/graphql/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/api/graphql/query_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.937896 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/business/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/business/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/business/i_metric_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/business/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.937896 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/business/transfers/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/business/transfers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/business/transfers/hierarchical_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/business/transfers/n_stacked_serie.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.937896 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/business/transfers/organization/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/business/transfers/organization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/business/transfers/organization/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/business/transfers/organization/organization_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/business/transfers/organization/organization_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/business/transfers/organization/participation_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/business/transfers/organization/platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/business/transfers/serie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/business/transfers/stacked_serie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/business/transfers/tabular_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.941897 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/data_access/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/data_access/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.941897 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/data_access/daos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/data_access/daos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.941897 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/data_access/daos/metric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/data_access/daos/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/data_access/daos/metric/metric_dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/data_access/daos/metric/srcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.941897 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/imetric_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/st_assets_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/st_assets_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/data_access/daos/platform_dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/data_access/pandas_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.941897 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/data_access/requesters/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/data_access/requesters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/data_access/requesters/cache_requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/data_access/requesters/irequester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/data_access/requesters/join_cache_requester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.941897 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.941897 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/about_view/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/about_view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/about_view/about_view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.941897 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/charts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/charts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/charts/chart_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/charts/chart_sum_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/charts/dt_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.945897 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/chart_pane_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/chart_pane_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/data_table_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/data_table_layout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.945897 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/figure/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/figure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/figure/bar_figure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/figure/calplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/figure/double_scatter_figure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/figure/figure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/figure/figure_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/figure/multi_bar_figure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/figure/treemap_figure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/ilayout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/layout_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.945897 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/dashboard_view/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/dashboard_view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/dashboard_view/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/dashboard_view/dashboard_view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.945897 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/main_view/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/main_view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/main_view/main_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/main_view/main_view_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.945897 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/resources/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/resources/strings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.945897 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.949897 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/business/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/business/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16026 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/business/app_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.949897 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/business/metric_adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/business/metric_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/business/metric_adapter/asset_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/business/metric_adapter/asset_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/business/metric_adapter/basic_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/business/metric_adapter/proposal_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/business/metric_adapter/proposal_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/business/metric_adapter/votes_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)   418772 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/class_diagram.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.949897 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/data_access/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/data_access/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.949897 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.949897 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/metric_dao_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/srcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.953897 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_active_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_active_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_active_voters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_approval_proposal_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_assets_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_assets_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_new_additions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_organization_activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_proposal_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_proposal_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_total_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_voters_percentage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_votes_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_votes_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_votes_voters_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/platform_dao.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.953897 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/presentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/presentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.953897 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/resources/strings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.953897 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.953897 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/business/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/business/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17742 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/business/app_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.957897 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/business/metric_adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/business/metric_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/business/metric_adapter/asset_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/business/metric_adapter/asset_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/business/metric_adapter/majority_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/business/metric_adapter/metric_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/business/metric_adapter/proposal_boost_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/business/metric_adapter/success_ratio_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/business/metric_adapter/vote_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)   461806 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/class_diagram.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.957897 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/data_access/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/data_access/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.957897 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/data_access/daos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/data_access/daos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.957897 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/metric_dao_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/srcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.961897 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_active_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_active_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_approval_proposal_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_assets_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_assets_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_different_voters_stakers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_organization_activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_proposal_majority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9374 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_proposal_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_time_serie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_total_reputation_holders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_total_votes_stakes_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_voters_percentage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_votes_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_votes_voters_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5611 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/data_access/daos/platform_dao.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.961897 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/presentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/presentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.961897 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/resources/strings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.965897 dao-analyzer-1.2.7.dev7/dao_analyzer/web/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/assets/ABOUT.md
+-rw-r--r--   0 runner    (1001) docker     (123)    65944 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/assets/aragon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/assets/callbacks.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/assets/cc-by.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18045 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/assets/dao-analyzer_header.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    36174 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/assets/dao-analyzer_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    54135 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/assets/daohaus.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16481 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/assets/daostack.png
+-rw-r--r--   0 runner    (1001) docker     (123)   101409 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/assets/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    58578 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/assets/github_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/assets/ico-github.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    17972 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/assets/img_header.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   129808 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/assets/kaggle_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/assets/logo-GPL.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10979 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/assets/logo-erc.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/assets/logo-grasia.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12180 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/assets/logo-ministerio.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/assets/logo-ucm.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/assets/logo_dao_analyzer.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/assets/logo_dao_analyzer.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/assets/logo_dao_analyzer_orig.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10237 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/assets/stylesheet.css
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer/web/matomo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.925896 dao-analyzer-1.2.7.dev7/dao_analyzer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9904 2023-07-19 15:55:56.000000 dao-analyzer-1.2.7.dev7/dao_analyzer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18890 2023-07-19 15:55:56.000000 dao-analyzer-1.2.7.dev7/dao_analyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 15:55:56.000000 dao-analyzer-1.2.7.dev7/dao_analyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-19 15:55:56.000000 dao-analyzer-1.2.7.dev7/dao_analyzer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-19 15:55:56.000000 dao-analyzer-1.2.7.dev7/dao_analyzer.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-19 15:55:56.000000 dao-analyzer-1.2.7.dev7/dao_analyzer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-19 15:55:56.000000 dao-analyzer-1.2.7.dev7/dao_analyzer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.965897 dao-analyzer-1.2.7.dev7/dao_analyzer_components/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer_components/.babelrc
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer_components/.eslintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer_components/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer_components/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer_components/_validate_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.969897 dao-analyzer-1.2.7.dev7/dao_analyzer_components/dao_analyzer_components/
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-19 15:55:39.000000 dao-analyzer-1.2.7.dev7/dao_analyzer_components/dao_analyzer_components/DAOInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-19 15:55:39.000000 dao-analyzer-1.2.7.dev7/dao_analyzer_components/dao_analyzer_components/DataPoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-19 15:55:40.000000 dao-analyzer-1.2.7.dev7/dao_analyzer_components/dao_analyzer_components/ParticipationStat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-19 15:55:40.000000 dao-analyzer-1.2.7.dev7/dao_analyzer_components/dao_analyzer_components/PlatformInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-07-19 15:55:39.000000 dao-analyzer-1.2.7.dev7/dao_analyzer_components/dao_analyzer_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-19 15:55:39.000000 dao-analyzer-1.2.7.dev7/dao_analyzer_components/dao_analyzer_components/_imports_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-19 15:55:39.000000 dao-analyzer-1.2.7.dev7/dao_analyzer_components/dao_analyzer_components/dao_analyzer_components.css
+-rw-r--r--   0 runner    (1001) docker     (123)    13291 2023-07-19 15:55:39.000000 dao-analyzer-1.2.7.dev7/dao_analyzer_components/dao_analyzer_components/dao_analyzer_components.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17779 2023-07-19 15:55:39.000000 dao-analyzer-1.2.7.dev7/dao_analyzer_components/dao_analyzer_components/dao_analyzer_components.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     5984 2023-07-19 15:55:39.000000 dao-analyzer-1.2.7.dev7/dao_analyzer_components/dao_analyzer_components/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-19 15:55:40.000000 dao-analyzer-1.2.7.dev7/dao_analyzer_components/dao_analyzer_components/package-info.json
+-rw-r--r--   0 runner    (1001) docker     (123)   630253 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer_components/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer_components/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.969897 dao-analyzer-1.2.7.dev7/dao_analyzer_components/public/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer_components/public/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer_components/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer_components/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.917896 dao-analyzer-1.2.7.dev7/dao_analyzer_components/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.969897 dao-analyzer-1.2.7.dev7/dao_analyzer_components/src/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer_components/src/demo/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.969897 dao-analyzer-1.2.7.dev7/dao_analyzer_components/src/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.969897 dao-analyzer-1.2.7.dev7/dao_analyzer_components/src/lib/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer_components/src/lib/components/DAOInfo.jsx
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer_components/src/lib/components/DataPoint.jsx
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer_components/src/lib/components/ParticipationStat.jsx
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer_components/src/lib/components/PlatformInfo.jsx
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer_components/src/lib/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer_components/webpack.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/dao_analyzer_components/webpack.demo.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/gunicorn_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      197 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/init.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.969897 dao-analyzer-1.2.7.dev7/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.973898 dao-analyzer-1.2.7.dev7/scripts/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/scripts/archive/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   339476 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/scripts/archive/names.ipynb
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1010 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/scripts/archive/uploadToKaggle.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1790 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/scripts/checkContinue.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4349 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/scripts/datawarehouseDiff.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      251 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/scripts/deploy.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      111 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/scripts/printArrow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1148 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/scripts/updateAragonNames.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2900 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/scripts/uploadDataWarehouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-19 15:55:56.981898 dao-analyzer-1.2.7.dev7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.973898 dao-analyzer-1.2.7.dev7/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.973898 dao-analyzer-1.2.7.dev7/test/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/mocks/api_requester_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/mocks/unix_date_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.973898 dao-analyzer-1.2.7.dev7/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.973898 dao-analyzer-1.2.7.dev7/test/unit/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/unit/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.973898 dao-analyzer-1.2.7.dev7/test/unit/apps/aragon/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/unit/apps/aragon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.973898 dao-analyzer-1.2.7.dev7/test/unit/apps/aragon/data_access/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/unit/apps/aragon/data_access/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.973898 dao-analyzer-1.2.7.dev7/test/unit/apps/aragon/data_access/daos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/unit/apps/aragon/data_access/daos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.973898 dao-analyzer-1.2.7.dev7/test/unit/apps/aragon/data_access/daos/metric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/unit/apps/aragon/data_access/daos/metric/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.973898 dao-analyzer-1.2.7.dev7/test/unit/apps/aragon/data_access/daos/metric/strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/unit/apps/aragon/data_access/daos/metric/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/unit/apps/aragon/data_access/daos/metric/strategy/test_aragon_st_new_additions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_active_organization_aragon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_active_token_holders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_cast_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_installed_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_vote_outcome.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.973898 dao-analyzer-1.2.7.dev7/test/unit/apps/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/unit/apps/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.973898 dao-analyzer-1.2.7.dev7/test/unit/apps/common/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/unit/apps/common/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.977898 dao-analyzer-1.2.7.dev7/test/unit/apps/common/api/graphql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/unit/apps/common/api/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/unit/apps/common/api/graphql/test_query_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.977898 dao-analyzer-1.2.7.dev7/test/unit/apps/common/business/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/unit/apps/common/business/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.977898 dao-analyzer-1.2.7.dev7/test/unit/apps/common/business/transfers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/unit/apps/common/business/transfers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/unit/apps/common/business/transfers/test_organization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.977898 dao-analyzer-1.2.7.dev7/test/unit/apps/common/data_access/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/unit/apps/common/data_access/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.977898 dao-analyzer-1.2.7.dev7/test/unit/apps/common/data_access/daos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/unit/apps/common/data_access/daos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.977898 dao-analyzer-1.2.7.dev7/test/unit/apps/daohaus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/unit/apps/daohaus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.977898 dao-analyzer-1.2.7.dev7/test/unit/apps/daohaus/data_access/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/unit/apps/daohaus/data_access/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.977898 dao-analyzer-1.2.7.dev7/test/unit/apps/daohaus/data_access/daos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/unit/apps/daohaus/data_access/daos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.977898 dao-analyzer-1.2.7.dev7/test/unit/apps/daohaus/data_access/daos/metric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/unit/apps/daohaus/data_access/daos/metric/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.977898 dao-analyzer-1.2.7.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_active_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_active_organization_daohaus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_active_voters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_dproposal_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_new_additions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_proposal_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_total_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_votes_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.981898 dao-analyzer-1.2.7.dev7/test/unit/apps/daostack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/unit/apps/daostack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.981898 dao-analyzer-1.2.7.dev7/test/unit/apps/daostack/data_access/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/unit/apps/daostack/data_access/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.981898 dao-analyzer-1.2.7.dev7/test/unit/apps/daostack/data_access/daos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/unit/apps/daostack/data_access/daos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.981898 dao-analyzer-1.2.7.dev7/test/unit/apps/daostack/data_access/daos/metric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/unit/apps/daostack/data_access/daos/metric/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.981898 dao-analyzer-1.2.7.dev7/test/unit/apps/daostack/data_access/daos/metric/strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/unit/apps/daostack/data_access/daos/metric/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_active_organization_daostack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_active_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_diff_voters_stakers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_proposal_majority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_proposal_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_time_serie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_voters_percentage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.981898 dao-analyzer-1.2.7.dev7/test/unit/apps/daostack/data_access/requesters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/unit/apps/daostack/data_access/requesters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:55:56.981898 dao-analyzer-1.2.7.dev7/test/unit/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-19 15:55:38.000000 dao-analyzer-1.2.7.dev7/test/unit/components/test_dao_info.py
```

### Comparing `dao-analyzer-1.2.7.dev6/.github/dependabot.yml` & `dao-analyzer-1.2.7.dev7/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/.github/workflows/check_continue.yml` & `dao-analyzer-1.2.7.dev7/.github/workflows/check_continue.yml`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/.github/workflows/ci.yml` & `dao-analyzer-1.2.7.dev7/.github/workflows/ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
       env:
         NODE_AUTH_TOKEN: ${{ secrets.NPM_TOKEN }}
 
   testing_python:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.8","3.9","3.10"]
+        python-version: ["3.8","3.9","3.10", "3.11"]
     env:
       DEBUG: TRUE
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
```

### Comparing `dao-analyzer-1.2.7.dev6/.github/workflows/update_aragon_names.yml` & `dao-analyzer-1.2.7.dev7/.github/workflows/update_aragon_names.yml`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/.gitignore` & `dao-analyzer-1.2.7.dev7/.gitignore`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/ABOUT.md` & `dao-analyzer-1.2.7.dev7/ABOUT.md`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/CHANGELOG.md` & `dao-analyzer-1.2.7.dev7/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/CITATION.cff` & `dao-analyzer-1.2.7.dev7/CITATION.cff`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/Dockerfile` & `dao-analyzer-1.2.7.dev7/Dockerfile`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/LICENSE` & `dao-analyzer-1.2.7.dev7/LICENSE`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/PKG-INFO` & `dao-analyzer-1.2.7.dev7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dao-analyzer
-Version: 1.2.7.dev6
+Version: 1.2.7.dev7
 Summary: "A tool to monitor DAO activity"
 Home-page: https://dao-analyzer.science
 Author: David Davó
 Author-email: ddavo@ucm.es
 Project-URL: Source, https://github.com/Grasia/dao-analyzer
 Project-URL: Bug Tracker, https://github.com/Grasia/dao-analyzer/issues
 Project-URL: Changelog, https://github.com/Grasia/dao-analyzer/blob/master/CHANGELOG.md
@@ -14,14 +14,15 @@
 Classifier: Framework :: Dash
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Sociology
 Classifier: Typing :: Typed
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docker
@@ -63,29 +64,29 @@
 - [Acknowledgements](#acknowledgements)
 - [Cite as](#cite-as)
 
 
 ## Set-up & Running (Download app)
 You can either install it on your local machine, or if you prefer it, you can use the official docker image.
 
-> If you only want to retrieve the data used by our application, you can follow [this guide](./cache_scripts/README.md) instead
+> If you only want to retrieve the data used by our application, go to [grasia/dao-scripts](https://github.com/Grasia/dao-scripts) instead
 
 The easiest method by far to download and run the application is to use pip to install it
 
 ```
 pip install dao-analyzer
 ```
 
 Then, you can run the app using the commands `daoa-cache-scripts` and `daoa-server`
 
 ### How to run it?
 Before launching the app, you have to run the following script in order to enable the cache stored in `datawarehouse`:
 
 ```
-daoa-cache-scripts
+dao-scripts
 ```
 
 After a few minutes, you can now run the app with:
 
 ```
 daoa-server
 ```
@@ -144,15 +145,15 @@
 
 > `dao-analyzer` is the container name, you can put whatever you want, but remember
 > to change it also on the following command
 
 Now, you can update the datawarehouse using:
 
 ```
-docker exec -it dao-analyzer python -m cache_scripts
+docker exec -it dao-analyzer dao-scripts
 ```
 
 You can even add it to your system as a cron job to update it daily, weekly, etc...
 
 ## Technical details
 
 ### Architecture
```

#### html2text {}

```diff
@@ -1,23 +1,24 @@
-Metadata-Version: 2.1 Name: dao-analyzer Version: 1.2.7.dev6 Summary: "A tool
+Metadata-Version: 2.1 Name: dao-analyzer Version: 1.2.7.dev7 Summary: "A tool
 to monitor DAO activity" Home-page: https://dao-analyzer.science Author: David
 DavÃ³ Author-email: ddavo@ucm.es Project-URL: Source, https://github.com/
 Grasia/dao-analyzer Project-URL: Bug Tracker, https://github.com/Grasia/dao-
 analyzer/issues Project-URL: Changelog, https://github.com/Grasia/dao-analyzer/
 blob/master/CHANGELOG.md Classifier: Development Status :: 5 - Production/
 Stable Classifier: Environment :: Console Classifier: Environment :: Web
 Environment Classifier: Framework :: Dash Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: GNU General Public
 License v3 (GPLv3) Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Topic :: Scientific/Engineering :: Visualization Classifier: Topic :: Sociology
-Classifier: Typing :: Typed Classifier: Topic :: Utilities Requires-Python:
->=3.8 Description-Content-Type: text/markdown Provides-Extra: docker Provides-
-Extra: dev License-File: LICENSE
+Programming Language :: Python :: 3.11 Classifier: Topic :: Scientific/
+Engineering :: Visualization Classifier: Topic :: Sociology Classifier: Typing
+:: Typed Classifier: Topic :: Utilities Requires-Python: >=3.8 Description-
+Content-Type: text/markdown Provides-Extra: docker Provides-Extra: dev License-
+File: LICENSE
                   [./dao_analyzer/web/assets/github_logo.png]
                [PyPI] [DOI_10.5281/zenodo.7669689.svg] [License]
 # DAO-Analyzer It is a tool to visualize DAO metrics. Currently, it shows DAO
 from [DAOstack](https://daostack.io/), [DAOhaus](https://daohaus.club/), and
 [Aragon](https://aragon.org/). Web site: [http://dao-analyzer.science/](http://
 dao-analyzer.science/) ## Table of contents  - [Set-up \& Running (Download
 app)](#set-up--running-download-app) - [How to run it?](#how-to-run-it) -
@@ -26,21 +27,21 @@
 (#technical-details) - [Architecture](#architecture) - [Debugging](#debugging)
 - [How to test it?](#how-to-test-it) - [Flags for hypothesis testing](#flags-
 for-hypothesis-testing) - [Deploy](#deploy) - [Matomo integration](#matomo-
 integration) - [Data](#data) - [Publications](#publications) -
 [Acknowledgements](#acknowledgements) - [Cite as](#cite-as) ## Set-up & Running
 (Download app) You can either install it on your local machine, or if you
 prefer it, you can use the official docker image. > If you only want to
-retrieve the data used by our application, you can follow [this guide](./
-cache_scripts/README.md) instead The easiest method by far to download and run
-the application is to use pip to install it ``` pip install dao-analyzer ```
-Then, you can run the app using the commands `daoa-cache-scripts` and `daoa-
-server` ### How to run it? Before launching the app, you have to run the
-following script in order to enable the cache stored in `datawarehouse`: ```
-daoa-cache-scripts ``` After a few minutes, you can now run the app with: ```
+retrieve the data used by our application, go to [grasia/dao-scripts](https://
+github.com/Grasia/dao-scripts) instead The easiest method by far to download
+and run the application is to use pip to install it ``` pip install dao-
+analyzer ``` Then, you can run the app using the commands `daoa-cache-scripts`
+and `daoa-server` ### How to run it? Before launching the app, you have to run
+the following script in order to enable the cache stored in `datawarehouse`:
+``` dao-scripts ``` After a few minutes, you can now run the app with: ```
 daoa-server ``` Now, visit `http://127.0.0.1:8050` or the address given in the
 program output with your web browser. ### Environment variables To be able to
 access all the features of dao-analyzer, you can specify the following
 environment variables: ``` # The CrytptoCompare API key to be used to get token
 prices DAOA_CC_API_KEY = "your_api_key" # The path of the datawarehouse
 DAOA_DW_PATH = './datawarehouse' # <-- Default value ``` ## Build application
 Enter in your terminal (git must be installed) and write down: `git clone
@@ -56,54 +57,53 @@
 container/dao-analyzer). The tags with the `-cached` suffix have a pre-
 populated data warehouse (this means the image uses more space, but takes less
 time to load). To use it, just run the command: ``` docker run --name dao-
 analyzer -it -p80:80 ghcr.io/grasia/dao-analyzer:latest ``` or ``` docker run -
 -name dao-analyzer -it -p80:80 ghcr.io/grasia/dao-analyzer:latest-cached ``` >
 `dao-analyzer` is the container name, you can put whatever you want, but
 remember > to change it also on the following command Now, you can update the
-datawarehouse using: ``` docker exec -it dao-analyzer python -m cache_scripts
-``` You can even add it to your system as a cron job to update it daily,
-weekly, etc... ## Technical details ### Architecture There is available a class
-diagram of the [DAOstack app](https://github.com/Grasia/dao-analyzer/blob/
-master/dao_analyzer/apps/daostack/class_diagram.png), the [DAOhaus app](https:/
-/github.com/Grasia/dao-analyzer/blob/master/dao_analyzer/apps/daohaus/
-class_diagram.png), and the [Aragon app](https://github.com/Grasia/dao-
-analyzer/blob/master/dao_analyzer/apps/aragon/class_diagram.png). ### Debugging
-This app uses `flask`, so you can use the `FLASK_ENV` variable, which also
-enables debug mode (among other things) when set to `development`. ``` export
-FLASK_ENV=development ``` ### How to test it? Run all tests with: `tox` or
-`python3 -m pytest test/` #### Flags for hypothesis testing Use this flag `--
-hypothesis-show-statistics` to show statistics. Use the flag `--hypothesis-
-seed=` to set a fixed seed, it's useful to reproduce a failure. ## Deploy In
-order to fully deploy the app, use the `deploy.sh` script, which installs all
-the Python dependencies, updates the datawarehouse, and runs the web-app with
-gunicorn, using the `gunicorn_config.py` file. ### Matomo integration To enable
-Matomo integration, you just have to pass the following environment variables
-like this: ```bash DAOA_MATOMO_URL = "https://matomo.example.com"
-DAOA_MATOMO_SITE_ID = 1 ``` You can check if the integration is working
-visiting the page and then your dashboard. The integration uses Javascript, so
-if there are any errors, you should be able to see them using "Inspect view" in
-your browser. ## Data The data is updated daily and published in [Kaggle]
-(https://www.kaggle.com/datasets/daviddavo/dao-analyzer) ## Publications *
-Javier Arroyo, David DavÃ³, Elena MartÃ­nez-Vicente, Youssef Faqir-Rhazoui, and
-Samer Hassan (2022). "DAO-Analyzer: Exploring Activity and Participation in
-Blockchain Organizations.". Companion Publication of the 2022 Conference on
-Computer Supported Cooperative Work and Social Computing (CSCW'22 Companion).
-ACM, 193â196. * [Freely available here](https://doi.org/10.1145/
-3500868.3559707) * Youssef Faqir-Rhazoui, Javier Arroyo and Samer Hassan
-(2021). "A comparative analysis of the platforms for decentralized autonomous
-organizations in the Ethereum blockchain." Journal of Internet Services and
-Applications volume 12, Article number: 9. * [Freely available here](https://
-jisajournal.springeropen.com/articles/10.1186/s13174-021-00139-6). * Youssef
-Faqir-Rhazoui, Miller Janny Ariza-GarzÃ³n, Javier Arroyo and Samer Hassan
-(2021). "Effect of the Gas Price Surges on User Activity in the DAOs of the
-Ethereum Blockchain." Extended Abstracts of the 2021 CHI Conference on Human
-Factors in Computing Systems, Article No.: 407, Pages 1â7. * [Freely
-available here](https://dl.acm.org/doi/pdf/10.1145/
-3411763.3451755?casa_token=cU40LWnMO0EAAAAA:
+datawarehouse using: ``` docker exec -it dao-analyzer dao-scripts ``` You can
+even add it to your system as a cron job to update it daily, weekly, etc... ##
+Technical details ### Architecture There is available a class diagram of the
+[DAOstack app](https://github.com/Grasia/dao-analyzer/blob/master/dao_analyzer/
+apps/daostack/class_diagram.png), the [DAOhaus app](https://github.com/Grasia/
+dao-analyzer/blob/master/dao_analyzer/apps/daohaus/class_diagram.png), and the
+[Aragon app](https://github.com/Grasia/dao-analyzer/blob/master/dao_analyzer/
+apps/aragon/class_diagram.png). ### Debugging This app uses `flask`, so you can
+use the `FLASK_ENV` variable, which also enables debug mode (among other
+things) when set to `development`. ``` export FLASK_ENV=development ``` ### How
+to test it? Run all tests with: `tox` or `python3 -m pytest test/` #### Flags
+for hypothesis testing Use this flag `--hypothesis-show-statistics` to show
+statistics. Use the flag `--hypothesis-seed=` to set a fixed seed, it's useful
+to reproduce a failure. ## Deploy In order to fully deploy the app, use the
+`deploy.sh` script, which installs all the Python dependencies, updates the
+datawarehouse, and runs the web-app with gunicorn, using the
+`gunicorn_config.py` file. ### Matomo integration To enable Matomo integration,
+you just have to pass the following environment variables like this: ```bash
+DAOA_MATOMO_URL = "https://matomo.example.com" DAOA_MATOMO_SITE_ID = 1 ``` You
+can check if the integration is working visiting the page and then your
+dashboard. The integration uses Javascript, so if there are any errors, you
+should be able to see them using "Inspect view" in your browser. ## Data The
+data is updated daily and published in [Kaggle](https://www.kaggle.com/
+datasets/daviddavo/dao-analyzer) ## Publications * Javier Arroyo, David DavÃ³,
+Elena MartÃ­nez-Vicente, Youssef Faqir-Rhazoui, and Samer Hassan (2022). "DAO-
+Analyzer: Exploring Activity and Participation in Blockchain Organizations.".
+Companion Publication of the 2022 Conference on Computer Supported Cooperative
+Work and Social Computing (CSCW'22 Companion). ACM, 193â196. * [Freely
+available here](https://doi.org/10.1145/3500868.3559707) * Youssef Faqir-
+Rhazoui, Javier Arroyo and Samer Hassan (2021). "A comparative analysis of the
+platforms for decentralized autonomous organizations in the Ethereum
+blockchain." Journal of Internet Services and Applications volume 12, Article
+number: 9. * [Freely available here](https://jisajournal.springeropen.com/
+articles/10.1186/s13174-021-00139-6). * Youssef Faqir-Rhazoui, Miller Janny
+Ariza-GarzÃ³n, Javier Arroyo and Samer Hassan (2021). "Effect of the Gas Price
+Surges on User Activity in the DAOs of the Ethereum Blockchain." Extended
+Abstracts of the 2021 CHI Conference on Human Factors in Computing Systems,
+Article No.: 407, Pages 1â7. * [Freely available here](https://dl.acm.org/
+doi/pdf/10.1145/3411763.3451755?casa_token=cU40LWnMO0EAAAAA:
 608tLS07Ya0KuhrBXihSSCRqMV72jDOu0XfP3jXnH64z4c2glcY43w69feOikee4t2oxoQ4doxAFjg).
 * Youssef Faqir-Rhazoui, Javier Arroyo, and Samer Hassan (2021). "A Scalable
 Voting System: Validation of Holographic Consensus in DAOstack." Proceedings of
 the 54th Hawaii International Conference on System Sciences, 5557-5566. *
 [Freely available here](https://scholarspace.manoa.hawaii.edu/bitstream/10125/
 71296/0543.pdf). * Youssef Faqir-Rhazoui, Javier Arroyo, and Samer Hassan.
 (2020). An overview of Decentralized Autonomous Organizations on the
```

### Comparing `dao-analyzer-1.2.7.dev6/README.md` & `dao-analyzer-1.2.7.dev7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -33,29 +33,29 @@
 - [Acknowledgements](#acknowledgements)
 - [Cite as](#cite-as)
 
 
 ## Set-up & Running (Download app)
 You can either install it on your local machine, or if you prefer it, you can use the official docker image.
 
-> If you only want to retrieve the data used by our application, you can follow [this guide](./cache_scripts/README.md) instead
+> If you only want to retrieve the data used by our application, go to [grasia/dao-scripts](https://github.com/Grasia/dao-scripts) instead
 
 The easiest method by far to download and run the application is to use pip to install it
 
 ```
 pip install dao-analyzer
 ```
 
 Then, you can run the app using the commands `daoa-cache-scripts` and `daoa-server`
 
 ### How to run it?
 Before launching the app, you have to run the following script in order to enable the cache stored in `datawarehouse`:
 
 ```
-daoa-cache-scripts
+dao-scripts
 ```
 
 After a few minutes, you can now run the app with:
 
 ```
 daoa-server
 ```
@@ -114,15 +114,15 @@
 
 > `dao-analyzer` is the container name, you can put whatever you want, but remember
 > to change it also on the following command
 
 Now, you can update the datawarehouse using:
 
 ```
-docker exec -it dao-analyzer python -m cache_scripts
+docker exec -it dao-analyzer dao-scripts
 ```
 
 You can even add it to your system as a cron job to update it daily, weekly, etc...
 
 ## Technical details
 
 ### Architecture
```

#### html2text {}

```diff
@@ -10,21 +10,21 @@
 (#technical-details) - [Architecture](#architecture) - [Debugging](#debugging)
 - [How to test it?](#how-to-test-it) - [Flags for hypothesis testing](#flags-
 for-hypothesis-testing) - [Deploy](#deploy) - [Matomo integration](#matomo-
 integration) - [Data](#data) - [Publications](#publications) -
 [Acknowledgements](#acknowledgements) - [Cite as](#cite-as) ## Set-up & Running
 (Download app) You can either install it on your local machine, or if you
 prefer it, you can use the official docker image. > If you only want to
-retrieve the data used by our application, you can follow [this guide](./
-cache_scripts/README.md) instead The easiest method by far to download and run
-the application is to use pip to install it ``` pip install dao-analyzer ```
-Then, you can run the app using the commands `daoa-cache-scripts` and `daoa-
-server` ### How to run it? Before launching the app, you have to run the
-following script in order to enable the cache stored in `datawarehouse`: ```
-daoa-cache-scripts ``` After a few minutes, you can now run the app with: ```
+retrieve the data used by our application, go to [grasia/dao-scripts](https://
+github.com/Grasia/dao-scripts) instead The easiest method by far to download
+and run the application is to use pip to install it ``` pip install dao-
+analyzer ``` Then, you can run the app using the commands `daoa-cache-scripts`
+and `daoa-server` ### How to run it? Before launching the app, you have to run
+the following script in order to enable the cache stored in `datawarehouse`:
+``` dao-scripts ``` After a few minutes, you can now run the app with: ```
 daoa-server ``` Now, visit `http://127.0.0.1:8050` or the address given in the
 program output with your web browser. ### Environment variables To be able to
 access all the features of dao-analyzer, you can specify the following
 environment variables: ``` # The CrytptoCompare API key to be used to get token
 prices DAOA_CC_API_KEY = "your_api_key" # The path of the datawarehouse
 DAOA_DW_PATH = './datawarehouse' # <-- Default value ``` ## Build application
 Enter in your terminal (git must be installed) and write down: `git clone
@@ -40,54 +40,53 @@
 container/dao-analyzer). The tags with the `-cached` suffix have a pre-
 populated data warehouse (this means the image uses more space, but takes less
 time to load). To use it, just run the command: ``` docker run --name dao-
 analyzer -it -p80:80 ghcr.io/grasia/dao-analyzer:latest ``` or ``` docker run -
 -name dao-analyzer -it -p80:80 ghcr.io/grasia/dao-analyzer:latest-cached ``` >
 `dao-analyzer` is the container name, you can put whatever you want, but
 remember > to change it also on the following command Now, you can update the
-datawarehouse using: ``` docker exec -it dao-analyzer python -m cache_scripts
-``` You can even add it to your system as a cron job to update it daily,
-weekly, etc... ## Technical details ### Architecture There is available a class
-diagram of the [DAOstack app](https://github.com/Grasia/dao-analyzer/blob/
-master/dao_analyzer/apps/daostack/class_diagram.png), the [DAOhaus app](https:/
-/github.com/Grasia/dao-analyzer/blob/master/dao_analyzer/apps/daohaus/
-class_diagram.png), and the [Aragon app](https://github.com/Grasia/dao-
-analyzer/blob/master/dao_analyzer/apps/aragon/class_diagram.png). ### Debugging
-This app uses `flask`, so you can use the `FLASK_ENV` variable, which also
-enables debug mode (among other things) when set to `development`. ``` export
-FLASK_ENV=development ``` ### How to test it? Run all tests with: `tox` or
-`python3 -m pytest test/` #### Flags for hypothesis testing Use this flag `--
-hypothesis-show-statistics` to show statistics. Use the flag `--hypothesis-
-seed=` to set a fixed seed, it's useful to reproduce a failure. ## Deploy In
-order to fully deploy the app, use the `deploy.sh` script, which installs all
-the Python dependencies, updates the datawarehouse, and runs the web-app with
-gunicorn, using the `gunicorn_config.py` file. ### Matomo integration To enable
-Matomo integration, you just have to pass the following environment variables
-like this: ```bash DAOA_MATOMO_URL = "https://matomo.example.com"
-DAOA_MATOMO_SITE_ID = 1 ``` You can check if the integration is working
-visiting the page and then your dashboard. The integration uses Javascript, so
-if there are any errors, you should be able to see them using "Inspect view" in
-your browser. ## Data The data is updated daily and published in [Kaggle]
-(https://www.kaggle.com/datasets/daviddavo/dao-analyzer) ## Publications *
-Javier Arroyo, David DavÃ³, Elena MartÃ­nez-Vicente, Youssef Faqir-Rhazoui, and
-Samer Hassan (2022). "DAO-Analyzer: Exploring Activity and Participation in
-Blockchain Organizations.". Companion Publication of the 2022 Conference on
-Computer Supported Cooperative Work and Social Computing (CSCW'22 Companion).
-ACM, 193â196. * [Freely available here](https://doi.org/10.1145/
-3500868.3559707) * Youssef Faqir-Rhazoui, Javier Arroyo and Samer Hassan
-(2021). "A comparative analysis of the platforms for decentralized autonomous
-organizations in the Ethereum blockchain." Journal of Internet Services and
-Applications volume 12, Article number: 9. * [Freely available here](https://
-jisajournal.springeropen.com/articles/10.1186/s13174-021-00139-6). * Youssef
-Faqir-Rhazoui, Miller Janny Ariza-GarzÃ³n, Javier Arroyo and Samer Hassan
-(2021). "Effect of the Gas Price Surges on User Activity in the DAOs of the
-Ethereum Blockchain." Extended Abstracts of the 2021 CHI Conference on Human
-Factors in Computing Systems, Article No.: 407, Pages 1â7. * [Freely
-available here](https://dl.acm.org/doi/pdf/10.1145/
-3411763.3451755?casa_token=cU40LWnMO0EAAAAA:
+datawarehouse using: ``` docker exec -it dao-analyzer dao-scripts ``` You can
+even add it to your system as a cron job to update it daily, weekly, etc... ##
+Technical details ### Architecture There is available a class diagram of the
+[DAOstack app](https://github.com/Grasia/dao-analyzer/blob/master/dao_analyzer/
+apps/daostack/class_diagram.png), the [DAOhaus app](https://github.com/Grasia/
+dao-analyzer/blob/master/dao_analyzer/apps/daohaus/class_diagram.png), and the
+[Aragon app](https://github.com/Grasia/dao-analyzer/blob/master/dao_analyzer/
+apps/aragon/class_diagram.png). ### Debugging This app uses `flask`, so you can
+use the `FLASK_ENV` variable, which also enables debug mode (among other
+things) when set to `development`. ``` export FLASK_ENV=development ``` ### How
+to test it? Run all tests with: `tox` or `python3 -m pytest test/` #### Flags
+for hypothesis testing Use this flag `--hypothesis-show-statistics` to show
+statistics. Use the flag `--hypothesis-seed=` to set a fixed seed, it's useful
+to reproduce a failure. ## Deploy In order to fully deploy the app, use the
+`deploy.sh` script, which installs all the Python dependencies, updates the
+datawarehouse, and runs the web-app with gunicorn, using the
+`gunicorn_config.py` file. ### Matomo integration To enable Matomo integration,
+you just have to pass the following environment variables like this: ```bash
+DAOA_MATOMO_URL = "https://matomo.example.com" DAOA_MATOMO_SITE_ID = 1 ``` You
+can check if the integration is working visiting the page and then your
+dashboard. The integration uses Javascript, so if there are any errors, you
+should be able to see them using "Inspect view" in your browser. ## Data The
+data is updated daily and published in [Kaggle](https://www.kaggle.com/
+datasets/daviddavo/dao-analyzer) ## Publications * Javier Arroyo, David DavÃ³,
+Elena MartÃ­nez-Vicente, Youssef Faqir-Rhazoui, and Samer Hassan (2022). "DAO-
+Analyzer: Exploring Activity and Participation in Blockchain Organizations.".
+Companion Publication of the 2022 Conference on Computer Supported Cooperative
+Work and Social Computing (CSCW'22 Companion). ACM, 193â196. * [Freely
+available here](https://doi.org/10.1145/3500868.3559707) * Youssef Faqir-
+Rhazoui, Javier Arroyo and Samer Hassan (2021). "A comparative analysis of the
+platforms for decentralized autonomous organizations in the Ethereum
+blockchain." Journal of Internet Services and Applications volume 12, Article
+number: 9. * [Freely available here](https://jisajournal.springeropen.com/
+articles/10.1186/s13174-021-00139-6). * Youssef Faqir-Rhazoui, Miller Janny
+Ariza-GarzÃ³n, Javier Arroyo and Samer Hassan (2021). "Effect of the Gas Price
+Surges on User Activity in the DAOs of the Ethereum Blockchain." Extended
+Abstracts of the 2021 CHI Conference on Human Factors in Computing Systems,
+Article No.: 407, Pages 1â7. * [Freely available here](https://dl.acm.org/
+doi/pdf/10.1145/3411763.3451755?casa_token=cU40LWnMO0EAAAAA:
 608tLS07Ya0KuhrBXihSSCRqMV72jDOu0XfP3jXnH64z4c2glcY43w69feOikee4t2oxoQ4doxAFjg).
 * Youssef Faqir-Rhazoui, Javier Arroyo, and Samer Hassan (2021). "A Scalable
 Voting System: Validation of Holographic Consensus in DAOstack." Proceedings of
 the 54th Hawaii International Conference on System Sciences, 5557-5566. *
 [Freely available here](https://scholarspace.manoa.hawaii.edu/bitstream/10125/
 71296/0543.pdf). * Youssef Faqir-Rhazoui, Javier Arroyo, and Samer Hassan.
 (2020). An overview of Decentralized Autonomous Organizations on the
```

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/app.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/app.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/business/app_service.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/business/app_service.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/business/metric_adapter/asset_tokens.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/business/metric_adapter/asset_tokens.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/business/metric_adapter/asset_values.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/business/metric_adapter/asset_values.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/business/metric_adapter/basic_adapter.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/business/metric_adapter/basic_adapter.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/business/metric_adapter/cast_type.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/business/metric_adapter/cast_type.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/business/metric_adapter/installed_apps.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/business/metric_adapter/installed_apps.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/business/metric_adapter/vote_outcome.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/business/metric_adapter/vote_outcome.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/class_diagram.png` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/class_diagram.png`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/metric_dao_factory.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/metric_dao_factory.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/srcs.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/srcs.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_active_organization.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_active_organization.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_active_token_holders.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_active_token_holders.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_active_voters.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_active_voters.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_approval_vote_rate.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_approval_vote_rate.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_cast_type.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_cast_type.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_casted_votes_rate.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_casted_votes_rate.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_casted_votes_voters_rate.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_casted_votes_voters_rate.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_installed_apps.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_installed_apps.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_new_additions.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_new_additions.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_organization_activity.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_organization_activity.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_total_token_holders.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_total_token_holders.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_vote_outcome.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/data_access/daos/metric/strategy/st_vote_outcome.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/data_access/daos/platform_dao.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/data_access/daos/platform_dao.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/aragon/resources/strings.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/aragon/resources/strings.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/api/graphql/query.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/api/graphql/query.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/api/graphql/query_builder.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/api/graphql/query_builder.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/business/i_metric_adapter.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/business/i_metric_adapter.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/business/singleton.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/business/singleton.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/business/transfers/hierarchical_data.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/business/transfers/hierarchical_data.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/business/transfers/n_stacked_serie.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/business/transfers/n_stacked_serie.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/business/transfers/organization/organization.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/business/transfers/organization/organization.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/business/transfers/organization/organization_filter.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/business/transfers/organization/organization_filter.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/business/transfers/organization/organization_list.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/business/transfers/organization/organization_list.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/business/transfers/organization/participation_stats.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/business/transfers/organization/participation_stats.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/business/transfers/organization/platform.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/business/transfers/organization/platform.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/business/transfers/serie.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/business/transfers/serie.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/business/transfers/stacked_serie.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/business/transfers/stacked_serie.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/business/transfers/tabular_data.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/business/transfers/tabular_data.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/data_access/daos/metric/metric_dao.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/data_access/daos/metric/metric_dao.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/imetric_strategy.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/imetric_strategy.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/st_assets_tokens.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/st_assets_tokens.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/st_assets_values.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/data_access/daos/metric/strategy/st_assets_values.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/data_access/daos/platform_dao.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/data_access/daos/platform_dao.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/data_access/pandas_utils.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/data_access/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/data_access/requesters/cache_requester.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/data_access/requesters/cache_requester.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/data_access/requesters/irequester.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/data_access/requesters/irequester.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/data_access/requesters/join_cache_requester.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/data_access/requesters/join_cache_requester.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/about_view/about_view.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/about_view/about_view.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/charts/chart_controller.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/charts/chart_controller.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/charts/chart_sum_controller.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/charts/chart_sum_controller.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/charts/dt_controller.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/charts/dt_controller.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/chart_pane_configuration.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/chart_pane_configuration.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/chart_pane_layout.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/chart_pane_layout.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/data_table_layout.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/data_table_layout.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/figure/bar_figure.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/figure/bar_figure.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/figure/calplot.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/figure/calplot.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/figure/double_scatter_figure.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/figure/double_scatter_figure.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/figure/figure.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/figure/figure.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/figure/figure_configuration.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/figure/figure_configuration.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/figure/multi_bar_figure.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/figure/multi_bar_figure.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/figure/treemap_figure.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/figure/treemap_figure.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/charts/layout/layout_configuration.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/charts/layout/layout_configuration.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/dashboard_view/controller.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/dashboard_view/controller.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/dashboard_view/dashboard_view.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/dashboard_view/dashboard_view.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/main_view/main_view.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/main_view/main_view.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/presentation/main_view/main_view_controller.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/presentation/main_view/main_view_controller.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/resources/colors.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/resources/colors.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/common/resources/strings.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/common/resources/strings.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/business/app_service.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/business/app_service.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/business/metric_adapter/asset_tokens.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/business/metric_adapter/asset_tokens.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/business/metric_adapter/asset_values.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/business/metric_adapter/asset_values.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/business/metric_adapter/basic_adapter.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/business/metric_adapter/basic_adapter.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/business/metric_adapter/proposal_outcome.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/business/metric_adapter/proposal_outcome.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/business/metric_adapter/proposal_type.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/business/metric_adapter/proposal_type.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/business/metric_adapter/votes_type.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/business/metric_adapter/votes_type.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/class_diagram.png` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/class_diagram.png`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/metric_dao_factory.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/metric_dao_factory.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/srcs.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/srcs.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_active_members.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_active_members.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_active_organization.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_active_organization.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_active_voters.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_active_voters.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_approval_proposal_rate.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_approval_proposal_rate.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_new_additions.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_new_additions.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_organization_activity.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_organization_activity.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_proposal_outcome.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_proposal_outcome.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_proposal_type.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_proposal_type.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_total_members.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_total_members.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_voters_percentage.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_voters_percentage.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_votes_rate.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_votes_rate.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_votes_type.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_votes_type.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_votes_voters_rate.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/metric/strategy/st_votes_voters_rate.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/data_access/daos/platform_dao.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/data_access/daos/platform_dao.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daohaus/resources/strings.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daohaus/resources/strings.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/business/app_service.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/business/app_service.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/business/metric_adapter/asset_tokens.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/business/metric_adapter/asset_tokens.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/business/metric_adapter/asset_values.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/business/metric_adapter/asset_values.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/business/metric_adapter/majority_type.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/business/metric_adapter/majority_type.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/business/metric_adapter/metric_adapter.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/business/metric_adapter/metric_adapter.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/business/metric_adapter/proposal_boost_outcome.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/business/metric_adapter/proposal_boost_outcome.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/business/metric_adapter/success_ratio_type.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/business/metric_adapter/success_ratio_type.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/business/metric_adapter/vote_type.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/business/metric_adapter/vote_type.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/class_diagram.png` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/class_diagram.png`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/metric_dao_factory.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/metric_dao_factory.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/srcs.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/srcs.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_active_organization.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_active_organization.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_active_users.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_active_users.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_approval_proposal_rate.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_approval_proposal_rate.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_different_voters_stakers.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_different_voters_stakers.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_organization_activity.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_organization_activity.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_proposal_majority.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_proposal_majority.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_proposal_outcome.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_proposal_outcome.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_time_serie.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_time_serie.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_total_reputation_holders.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_total_reputation_holders.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_total_votes_stakes_option.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_total_votes_stakes_option.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_voters_percentage.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_voters_percentage.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_votes_rate.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_votes_rate.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_votes_voters_rate.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/data_access/daos/metric/strategy/st_votes_voters_rate.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/data_access/daos/platform_dao.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/data_access/daos/platform_dao.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/apps/daostack/resources/strings.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/apps/daostack/resources/strings.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/assets/ABOUT.md` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/assets/ABOUT.md`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/assets/aragon.png` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/assets/aragon.png`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/assets/callbacks.js` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/assets/callbacks.js`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/assets/cc-by.png` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/assets/cc-by.png`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/assets/dao-analyzer_header.svg` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/assets/dao-analyzer_header.svg`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/assets/dao-analyzer_logo.svg` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/assets/dao-analyzer_logo.svg`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/assets/daohaus.png` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/assets/daohaus.png`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/assets/daostack.png` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/assets/daostack.png`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/assets/favicon.ico` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/assets/github_logo.png` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/assets/github_logo.png`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/assets/ico-github.svg` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/assets/ico-github.svg`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/assets/img_header.jpg` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/assets/img_header.jpg`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/assets/kaggle_logo.png` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/assets/kaggle_logo.png`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/assets/logo-GPL.png` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/assets/logo-GPL.png`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/assets/logo-erc.png` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/assets/logo-erc.png`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/assets/logo-grasia.png` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/assets/logo-grasia.png`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/assets/logo-ministerio.png` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/assets/logo-ministerio.png`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/assets/logo-ucm.png` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/assets/logo-ucm.png`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/assets/logo_dao_analyzer.png` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/assets/logo_dao_analyzer.png`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/assets/logo_dao_analyzer.svg` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/assets/logo_dao_analyzer.svg`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/assets/logo_dao_analyzer_orig.svg` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/assets/logo_dao_analyzer_orig.svg`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/assets/stylesheet.css` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/assets/stylesheet.css`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/logs.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/logs.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer/web/matomo.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer/web/matomo.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer.egg-info/PKG-INFO` & `dao-analyzer-1.2.7.dev7/dao_analyzer.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dao-analyzer
-Version: 1.2.7.dev6
+Version: 1.2.7.dev7
 Summary: "A tool to monitor DAO activity"
 Home-page: https://dao-analyzer.science
 Author: David Davó
 Author-email: ddavo@ucm.es
 Project-URL: Source, https://github.com/Grasia/dao-analyzer
 Project-URL: Bug Tracker, https://github.com/Grasia/dao-analyzer/issues
 Project-URL: Changelog, https://github.com/Grasia/dao-analyzer/blob/master/CHANGELOG.md
@@ -14,14 +14,15 @@
 Classifier: Framework :: Dash
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Sociology
 Classifier: Typing :: Typed
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docker
@@ -63,29 +64,29 @@
 - [Acknowledgements](#acknowledgements)
 - [Cite as](#cite-as)
 
 
 ## Set-up & Running (Download app)
 You can either install it on your local machine, or if you prefer it, you can use the official docker image.
 
-> If you only want to retrieve the data used by our application, you can follow [this guide](./cache_scripts/README.md) instead
+> If you only want to retrieve the data used by our application, go to [grasia/dao-scripts](https://github.com/Grasia/dao-scripts) instead
 
 The easiest method by far to download and run the application is to use pip to install it
 
 ```
 pip install dao-analyzer
 ```
 
 Then, you can run the app using the commands `daoa-cache-scripts` and `daoa-server`
 
 ### How to run it?
 Before launching the app, you have to run the following script in order to enable the cache stored in `datawarehouse`:
 
 ```
-daoa-cache-scripts
+dao-scripts
 ```
 
 After a few minutes, you can now run the app with:
 
 ```
 daoa-server
 ```
@@ -144,15 +145,15 @@
 
 > `dao-analyzer` is the container name, you can put whatever you want, but remember
 > to change it also on the following command
 
 Now, you can update the datawarehouse using:
 
 ```
-docker exec -it dao-analyzer python -m cache_scripts
+docker exec -it dao-analyzer dao-scripts
 ```
 
 You can even add it to your system as a cron job to update it daily, weekly, etc...
 
 ## Technical details
 
 ### Architecture
```

#### html2text {}

```diff
@@ -1,23 +1,24 @@
-Metadata-Version: 2.1 Name: dao-analyzer Version: 1.2.7.dev6 Summary: "A tool
+Metadata-Version: 2.1 Name: dao-analyzer Version: 1.2.7.dev7 Summary: "A tool
 to monitor DAO activity" Home-page: https://dao-analyzer.science Author: David
 DavÃ³ Author-email: ddavo@ucm.es Project-URL: Source, https://github.com/
 Grasia/dao-analyzer Project-URL: Bug Tracker, https://github.com/Grasia/dao-
 analyzer/issues Project-URL: Changelog, https://github.com/Grasia/dao-analyzer/
 blob/master/CHANGELOG.md Classifier: Development Status :: 5 - Production/
 Stable Classifier: Environment :: Console Classifier: Environment :: Web
 Environment Classifier: Framework :: Dash Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: GNU General Public
 License v3 (GPLv3) Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Topic :: Scientific/Engineering :: Visualization Classifier: Topic :: Sociology
-Classifier: Typing :: Typed Classifier: Topic :: Utilities Requires-Python:
->=3.8 Description-Content-Type: text/markdown Provides-Extra: docker Provides-
-Extra: dev License-File: LICENSE
+Programming Language :: Python :: 3.11 Classifier: Topic :: Scientific/
+Engineering :: Visualization Classifier: Topic :: Sociology Classifier: Typing
+:: Typed Classifier: Topic :: Utilities Requires-Python: >=3.8 Description-
+Content-Type: text/markdown Provides-Extra: docker Provides-Extra: dev License-
+File: LICENSE
                   [./dao_analyzer/web/assets/github_logo.png]
                [PyPI] [DOI_10.5281/zenodo.7669689.svg] [License]
 # DAO-Analyzer It is a tool to visualize DAO metrics. Currently, it shows DAO
 from [DAOstack](https://daostack.io/), [DAOhaus](https://daohaus.club/), and
 [Aragon](https://aragon.org/). Web site: [http://dao-analyzer.science/](http://
 dao-analyzer.science/) ## Table of contents  - [Set-up \& Running (Download
 app)](#set-up--running-download-app) - [How to run it?](#how-to-run-it) -
@@ -26,21 +27,21 @@
 (#technical-details) - [Architecture](#architecture) - [Debugging](#debugging)
 - [How to test it?](#how-to-test-it) - [Flags for hypothesis testing](#flags-
 for-hypothesis-testing) - [Deploy](#deploy) - [Matomo integration](#matomo-
 integration) - [Data](#data) - [Publications](#publications) -
 [Acknowledgements](#acknowledgements) - [Cite as](#cite-as) ## Set-up & Running
 (Download app) You can either install it on your local machine, or if you
 prefer it, you can use the official docker image. > If you only want to
-retrieve the data used by our application, you can follow [this guide](./
-cache_scripts/README.md) instead The easiest method by far to download and run
-the application is to use pip to install it ``` pip install dao-analyzer ```
-Then, you can run the app using the commands `daoa-cache-scripts` and `daoa-
-server` ### How to run it? Before launching the app, you have to run the
-following script in order to enable the cache stored in `datawarehouse`: ```
-daoa-cache-scripts ``` After a few minutes, you can now run the app with: ```
+retrieve the data used by our application, go to [grasia/dao-scripts](https://
+github.com/Grasia/dao-scripts) instead The easiest method by far to download
+and run the application is to use pip to install it ``` pip install dao-
+analyzer ``` Then, you can run the app using the commands `daoa-cache-scripts`
+and `daoa-server` ### How to run it? Before launching the app, you have to run
+the following script in order to enable the cache stored in `datawarehouse`:
+``` dao-scripts ``` After a few minutes, you can now run the app with: ```
 daoa-server ``` Now, visit `http://127.0.0.1:8050` or the address given in the
 program output with your web browser. ### Environment variables To be able to
 access all the features of dao-analyzer, you can specify the following
 environment variables: ``` # The CrytptoCompare API key to be used to get token
 prices DAOA_CC_API_KEY = "your_api_key" # The path of the datawarehouse
 DAOA_DW_PATH = './datawarehouse' # <-- Default value ``` ## Build application
 Enter in your terminal (git must be installed) and write down: `git clone
@@ -56,54 +57,53 @@
 container/dao-analyzer). The tags with the `-cached` suffix have a pre-
 populated data warehouse (this means the image uses more space, but takes less
 time to load). To use it, just run the command: ``` docker run --name dao-
 analyzer -it -p80:80 ghcr.io/grasia/dao-analyzer:latest ``` or ``` docker run -
 -name dao-analyzer -it -p80:80 ghcr.io/grasia/dao-analyzer:latest-cached ``` >
 `dao-analyzer` is the container name, you can put whatever you want, but
 remember > to change it also on the following command Now, you can update the
-datawarehouse using: ``` docker exec -it dao-analyzer python -m cache_scripts
-``` You can even add it to your system as a cron job to update it daily,
-weekly, etc... ## Technical details ### Architecture There is available a class
-diagram of the [DAOstack app](https://github.com/Grasia/dao-analyzer/blob/
-master/dao_analyzer/apps/daostack/class_diagram.png), the [DAOhaus app](https:/
-/github.com/Grasia/dao-analyzer/blob/master/dao_analyzer/apps/daohaus/
-class_diagram.png), and the [Aragon app](https://github.com/Grasia/dao-
-analyzer/blob/master/dao_analyzer/apps/aragon/class_diagram.png). ### Debugging
-This app uses `flask`, so you can use the `FLASK_ENV` variable, which also
-enables debug mode (among other things) when set to `development`. ``` export
-FLASK_ENV=development ``` ### How to test it? Run all tests with: `tox` or
-`python3 -m pytest test/` #### Flags for hypothesis testing Use this flag `--
-hypothesis-show-statistics` to show statistics. Use the flag `--hypothesis-
-seed=` to set a fixed seed, it's useful to reproduce a failure. ## Deploy In
-order to fully deploy the app, use the `deploy.sh` script, which installs all
-the Python dependencies, updates the datawarehouse, and runs the web-app with
-gunicorn, using the `gunicorn_config.py` file. ### Matomo integration To enable
-Matomo integration, you just have to pass the following environment variables
-like this: ```bash DAOA_MATOMO_URL = "https://matomo.example.com"
-DAOA_MATOMO_SITE_ID = 1 ``` You can check if the integration is working
-visiting the page and then your dashboard. The integration uses Javascript, so
-if there are any errors, you should be able to see them using "Inspect view" in
-your browser. ## Data The data is updated daily and published in [Kaggle]
-(https://www.kaggle.com/datasets/daviddavo/dao-analyzer) ## Publications *
-Javier Arroyo, David DavÃ³, Elena MartÃ­nez-Vicente, Youssef Faqir-Rhazoui, and
-Samer Hassan (2022). "DAO-Analyzer: Exploring Activity and Participation in
-Blockchain Organizations.". Companion Publication of the 2022 Conference on
-Computer Supported Cooperative Work and Social Computing (CSCW'22 Companion).
-ACM, 193â196. * [Freely available here](https://doi.org/10.1145/
-3500868.3559707) * Youssef Faqir-Rhazoui, Javier Arroyo and Samer Hassan
-(2021). "A comparative analysis of the platforms for decentralized autonomous
-organizations in the Ethereum blockchain." Journal of Internet Services and
-Applications volume 12, Article number: 9. * [Freely available here](https://
-jisajournal.springeropen.com/articles/10.1186/s13174-021-00139-6). * Youssef
-Faqir-Rhazoui, Miller Janny Ariza-GarzÃ³n, Javier Arroyo and Samer Hassan
-(2021). "Effect of the Gas Price Surges on User Activity in the DAOs of the
-Ethereum Blockchain." Extended Abstracts of the 2021 CHI Conference on Human
-Factors in Computing Systems, Article No.: 407, Pages 1â7. * [Freely
-available here](https://dl.acm.org/doi/pdf/10.1145/
-3411763.3451755?casa_token=cU40LWnMO0EAAAAA:
+datawarehouse using: ``` docker exec -it dao-analyzer dao-scripts ``` You can
+even add it to your system as a cron job to update it daily, weekly, etc... ##
+Technical details ### Architecture There is available a class diagram of the
+[DAOstack app](https://github.com/Grasia/dao-analyzer/blob/master/dao_analyzer/
+apps/daostack/class_diagram.png), the [DAOhaus app](https://github.com/Grasia/
+dao-analyzer/blob/master/dao_analyzer/apps/daohaus/class_diagram.png), and the
+[Aragon app](https://github.com/Grasia/dao-analyzer/blob/master/dao_analyzer/
+apps/aragon/class_diagram.png). ### Debugging This app uses `flask`, so you can
+use the `FLASK_ENV` variable, which also enables debug mode (among other
+things) when set to `development`. ``` export FLASK_ENV=development ``` ### How
+to test it? Run all tests with: `tox` or `python3 -m pytest test/` #### Flags
+for hypothesis testing Use this flag `--hypothesis-show-statistics` to show
+statistics. Use the flag `--hypothesis-seed=` to set a fixed seed, it's useful
+to reproduce a failure. ## Deploy In order to fully deploy the app, use the
+`deploy.sh` script, which installs all the Python dependencies, updates the
+datawarehouse, and runs the web-app with gunicorn, using the
+`gunicorn_config.py` file. ### Matomo integration To enable Matomo integration,
+you just have to pass the following environment variables like this: ```bash
+DAOA_MATOMO_URL = "https://matomo.example.com" DAOA_MATOMO_SITE_ID = 1 ``` You
+can check if the integration is working visiting the page and then your
+dashboard. The integration uses Javascript, so if there are any errors, you
+should be able to see them using "Inspect view" in your browser. ## Data The
+data is updated daily and published in [Kaggle](https://www.kaggle.com/
+datasets/daviddavo/dao-analyzer) ## Publications * Javier Arroyo, David DavÃ³,
+Elena MartÃ­nez-Vicente, Youssef Faqir-Rhazoui, and Samer Hassan (2022). "DAO-
+Analyzer: Exploring Activity and Participation in Blockchain Organizations.".
+Companion Publication of the 2022 Conference on Computer Supported Cooperative
+Work and Social Computing (CSCW'22 Companion). ACM, 193â196. * [Freely
+available here](https://doi.org/10.1145/3500868.3559707) * Youssef Faqir-
+Rhazoui, Javier Arroyo and Samer Hassan (2021). "A comparative analysis of the
+platforms for decentralized autonomous organizations in the Ethereum
+blockchain." Journal of Internet Services and Applications volume 12, Article
+number: 9. * [Freely available here](https://jisajournal.springeropen.com/
+articles/10.1186/s13174-021-00139-6). * Youssef Faqir-Rhazoui, Miller Janny
+Ariza-GarzÃ³n, Javier Arroyo and Samer Hassan (2021). "Effect of the Gas Price
+Surges on User Activity in the DAOs of the Ethereum Blockchain." Extended
+Abstracts of the 2021 CHI Conference on Human Factors in Computing Systems,
+Article No.: 407, Pages 1â7. * [Freely available here](https://dl.acm.org/
+doi/pdf/10.1145/3411763.3451755?casa_token=cU40LWnMO0EAAAAA:
 608tLS07Ya0KuhrBXihSSCRqMV72jDOu0XfP3jXnH64z4c2glcY43w69feOikee4t2oxoQ4doxAFjg).
 * Youssef Faqir-Rhazoui, Javier Arroyo, and Samer Hassan (2021). "A Scalable
 Voting System: Validation of Holographic Consensus in DAOstack." Proceedings of
 the 54th Hawaii International Conference on System Sciences, 5557-5566. *
 [Freely available here](https://scholarspace.manoa.hawaii.edu/bitstream/10125/
 71296/0543.pdf). * Youssef Faqir-Rhazoui, Javier Arroyo, and Samer Hassan.
 (2020). An overview of Decentralized Autonomous Organizations on the
```

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer.egg-info/SOURCES.txt` & `dao-analyzer-1.2.7.dev7/dao_analyzer.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -14,36 +14,14 @@
 pyproject.toml
 setup.cfg
 setup.py
 .github/dependabot.yml
 .github/workflows/check_continue.yml
 .github/workflows/ci.yml
 .github/workflows/update_aragon_names.yml
-cache_scripts/CHANGELOG.md
-cache_scripts/README.md
-cache_scripts/__init__.py
-cache_scripts/__main__.py
-cache_scripts/argparser.py
-cache_scripts/config.py
-cache_scripts/endpoints.json
-cache_scripts/main.py
-cache_scripts/metadata.py
-cache_scripts/aragon/__init__.py
-cache_scripts/aragon/dao_names.json
-cache_scripts/aragon/runner.py
-cache_scripts/common/__init__.py
-cache_scripts/common/api_requester.py
-cache_scripts/common/blockscout.py
-cache_scripts/common/common.py
-cache_scripts/common/cryptocompare.py
-cache_scripts/common/graphql.py
-cache_scripts/daohaus/__init__.py
-cache_scripts/daohaus/runner.py
-cache_scripts/daostack/__init__.py
-cache_scripts/daostack/runner.py
 dao_analyzer.egg-info/PKG-INFO
 dao_analyzer.egg-info/SOURCES.txt
 dao_analyzer.egg-info/dependency_links.txt
 dao_analyzer.egg-info/entry_points.txt
 dao_analyzer.egg-info/namespace_packages.txt
 dao_analyzer.egg-info/requires.txt
 dao_analyzer.egg-info/top_level.txt
```

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer_components/.eslintrc` & `dao-analyzer-1.2.7.dev7/dao_analyzer_components/.eslintrc`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer_components/MANIFEST.in` & `dao-analyzer-1.2.7.dev7/dao_analyzer_components/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer_components/_validate_init.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer_components/_validate_init.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer_components/dao_analyzer_components/DAOInfo.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer_components/dao_analyzer_components/DAOInfo.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer_components/dao_analyzer_components/DataPoint.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer_components/dao_analyzer_components/DataPoint.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer_components/dao_analyzer_components/ParticipationStat.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer_components/dao_analyzer_components/ParticipationStat.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer_components/dao_analyzer_components/PlatformInfo.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer_components/dao_analyzer_components/PlatformInfo.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer_components/dao_analyzer_components/__init__.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer_components/dao_analyzer_components/__init__.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer_components/dao_analyzer_components/dao_analyzer_components.css` & `dao-analyzer-1.2.7.dev7/dao_analyzer_components/dao_analyzer_components/dao_analyzer_components.css`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer_components/dao_analyzer_components/dao_analyzer_components.min.js` & `dao-analyzer-1.2.7.dev7/dao_analyzer_components/dao_analyzer_components/dao_analyzer_components.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -42,15 +42,15 @@
             var t = function(e) {
                     return /\/_dash-component-suites\//.test(e.src)
                 }(n()),
                 o = r(e);
             if (!t) return o;
             var i = o.split("/"),
                 a = i.slice(-1)[0].split(".");
-            return a.splice(1, 0, "v0_0_22m1684221826"), i.splice(-1, 1, a.join(".")), i.join("/")
+            return a.splice(1, 0, "v0_0_22m1689782076"), i.splice(-1, 1, a.join(".")), i.join("/")
         }
     }
     var o = {};
     t.r(o), t.d(o, {
         DAOInfo: () => g,
         DataPoint: () => z,
         ParticipationStat: () => b,
```

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer_components/dao_analyzer_components/dao_analyzer_components.min.js.map` & `dao-analyzer-1.2.7.dev7/dao_analyzer_components/dao_analyzer_components/dao_analyzer_components.min.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.989010989010989%*

 * *Differences: {"'sourcesContent'": "{insert: [(1, 'var getCurrentScript = function() {\\n    var script = "*

 * *                     'document.currentScript;\\n    if (!script) {\\n        /* Shim for IE11 and '*

 * *                     'below */\\n        /* Do not take into account async scripts and inline '*

 * *                     'scripts */\\n\\n        var doc_scripts = '*

 * *                     "document.getElementsByTagName(\\'script\\');\\n        var scripts = "*

 * *                     '[];\\n\\n        for (var i = 0; i < doc_ […]*

```diff
@@ -107,15 +107,15 @@
         "webpack:///./src/lib/components/ParticipationStat.jsx",
         "webpack:///./src/lib/components/DAOInfo.jsx",
         "webpack:///./src/lib/components/PlatformInfo.jsx",
         "webpack:///./src/lib/components/DataPoint.jsx"
     ],
     "sourcesContent": [
         "// The require scope\nvar __webpack_require__ = {};\n\n",
-        "var getCurrentScript = function() {\n    var script = document.currentScript;\n    if (!script) {\n        /* Shim for IE11 and below */\n        /* Do not take into account async scripts and inline scripts */\n\n        var doc_scripts = document.getElementsByTagName('script');\n        var scripts = [];\n\n        for (var i = 0; i < doc_scripts.length; i++) {\n            scripts.push(doc_scripts[i]);\n        }\n\n        scripts = scripts.filter(function(s) { return !s.async && !s.text && !s.textContent; });\n        script = scripts.slice(-1)[0];\n    }\n\n    return script;\n};\n\nvar isLocalScript = function(script) {\n    return /\\/_dash-component-suites\\//.test(script.src);\n};\n\nObject.defineProperty(__webpack_require__, 'p', {\n    get: (function () {\n        var script = getCurrentScript();\n\n        var url = script.src.split('/').slice(0, -1).join('/') + '/';\n\n        return function() {\n            return url;\n        };\n    })()\n});\n\nif (typeof jsonpScriptSrc !== 'undefined') {\n    var __jsonpScriptSrc__ = jsonpScriptSrc;\n    jsonpScriptSrc = function(chunkId) {\n        var script = getCurrentScript();\n        var isLocal = isLocalScript(script);\n\n        var src = __jsonpScriptSrc__(chunkId);\n\n        if(!isLocal) {\n            return src;\n        }\n\n        var srcFragments = src.split('/');\n        var fileFragments = srcFragments.slice(-1)[0].split('.');\n\n        fileFragments.splice(1, 0, \"v0_0_22m1684221826\");\n        srcFragments.splice(-1, 1, fileFragments.join('.'))\n\n        return srcFragments.join('/');\n    };\n}\n",
+        "var getCurrentScript = function() {\n    var script = document.currentScript;\n    if (!script) {\n        /* Shim for IE11 and below */\n        /* Do not take into account async scripts and inline scripts */\n\n        var doc_scripts = document.getElementsByTagName('script');\n        var scripts = [];\n\n        for (var i = 0; i < doc_scripts.length; i++) {\n            scripts.push(doc_scripts[i]);\n        }\n\n        scripts = scripts.filter(function(s) { return !s.async && !s.text && !s.textContent; });\n        script = scripts.slice(-1)[0];\n    }\n\n    return script;\n};\n\nvar isLocalScript = function(script) {\n    return /\\/_dash-component-suites\\//.test(script.src);\n};\n\nObject.defineProperty(__webpack_require__, 'p', {\n    get: (function () {\n        var script = getCurrentScript();\n\n        var url = script.src.split('/').slice(0, -1).join('/') + '/';\n\n        return function() {\n            return url;\n        };\n    })()\n});\n\nif (typeof jsonpScriptSrc !== 'undefined') {\n    var __jsonpScriptSrc__ = jsonpScriptSrc;\n    jsonpScriptSrc = function(chunkId) {\n        var script = getCurrentScript();\n        var isLocal = isLocalScript(script);\n\n        var src = __jsonpScriptSrc__(chunkId);\n\n        if(!isLocal) {\n            return src;\n        }\n\n        var srcFragments = src.split('/');\n        var fileFragments = srcFragments.slice(-1)[0].split('.');\n\n        fileFragments.splice(1, 0, \"v0_0_22m1689782076\");\n        srcFragments.splice(-1, 1, fileFragments.join('.'))\n\n        return srcFragments.join('/');\n    };\n}\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
         "const __WEBPACK_NAMESPACE_OBJECT__ = window[\"React\"];",
         "const __WEBPACK_NAMESPACE_OBJECT__ = window[\"PropTypes\"];",
         "import React, { Component } from 'react';\nimport PropTypes from 'prop-types';\n\n/** \n * This class will be used by DAOInfo and PlatformInfo\n */\nexport default class ParticipationStat extends Component {\n    render () {\n        const { text, value } = this.props;\n        if (value) {\n            return (<div><b>{value}</b> {text}</div>);\n        } else {\n            return (<div>{text}</div>);\n        }\n    }\n}\n\nParticipationStat.propTypes = {\n    /**\n     * The text to show\n     */\n    text: PropTypes.string.isRequired,\n\n    /**\n     * The value to highlight, which will be appended to text\n     */\n    value: PropTypes.string,\n\n    /**\n     * The key used by React for optimization\n     */\n    key: PropTypes.string,\n}\n",
```

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer_components/dao_analyzer_components/metadata.json` & `dao-analyzer-1.2.7.dev7/dao_analyzer_components/dao_analyzer_components/metadata.json`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer_components/dao_analyzer_components/package-info.json` & `dao-analyzer-1.2.7.dev7/dao_analyzer_components/dao_analyzer_components/package-info.json`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer_components/package-lock.json` & `dao-analyzer-1.2.7.dev7/dao_analyzer_components/package-lock.json`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer_components/package.json` & `dao-analyzer-1.2.7.dev7/dao_analyzer_components/package.json`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer_components/setup.py` & `dao-analyzer-1.2.7.dev7/dao_analyzer_components/setup.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer_components/src/lib/components/DAOInfo.jsx` & `dao-analyzer-1.2.7.dev7/dao_analyzer_components/src/lib/components/DAOInfo.jsx`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer_components/src/lib/components/DataPoint.jsx` & `dao-analyzer-1.2.7.dev7/dao_analyzer_components/src/lib/components/DataPoint.jsx`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer_components/src/lib/components/ParticipationStat.jsx` & `dao-analyzer-1.2.7.dev7/dao_analyzer_components/src/lib/components/ParticipationStat.jsx`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer_components/src/lib/components/PlatformInfo.jsx` & `dao-analyzer-1.2.7.dev7/dao_analyzer_components/src/lib/components/PlatformInfo.jsx`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/dao_analyzer_components/webpack.config.js` & `dao-analyzer-1.2.7.dev7/dao_analyzer_components/webpack.config.js`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/scripts/archive/names.ipynb` & `dao-analyzer-1.2.7.dev7/scripts/archive/names.ipynb`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/scripts/archive/uploadToKaggle.sh` & `dao-analyzer-1.2.7.dev7/scripts/archive/uploadToKaggle.sh`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/scripts/checkContinue.sh` & `dao-analyzer-1.2.7.dev7/scripts/checkContinue.sh`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/scripts/datawarehouseDiff.py` & `dao-analyzer-1.2.7.dev7/scripts/datawarehouseDiff.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/scripts/updateAragonNames.py` & `dao-analyzer-1.2.7.dev7/scripts/updateAragonNames.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/scripts/uploadDataWarehouse.py` & `dao-analyzer-1.2.7.dev7/scripts/uploadDataWarehouse.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/setup.cfg` & `dao-analyzer-1.2.7.dev7/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -17,22 +17,24 @@
 	Framework :: Dash
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Scientific/Engineering :: Visualization
 	Topic :: Sociology
 	Typing :: Typed
 	Topic :: Utilities
 
 [options]
 python_requires = >= 3.8
 install_requires = 
+	dao-scripts == 1.1.9
 	dash >= 2.5.0, <2.6.0
 	dash-bootstrap-components >= 1.1.0
 	Werkzeug < 2.1.0 # Waiting for upstream fix on dash part
 	flask >= 2.0.2
 	gql >= 3.0.0a1
 	millify >= 0.1.1
 	numpy >= 1.17.3
@@ -57,15 +59,14 @@
 	package-info.json
 	dao_analyzer_components.min.js
 	dao_analyzer_components.min.js.map
 	dao_analyzer_components.css
 
 [options.entry_points]
 console_scripts = 
-	daoa-cache-scripts = dao_analyzer.cache_scripts.main:main
 	daoa-server = dao_analyzer.web.app:main
 
 [options.extras_require]
 docker = 
 	gunicorn >= 20.1.0
 	kaggle >= 1.5.12
 	zenodo-client >= 0.3.0
@@ -100,15 +101,15 @@
 	__pycache__,
 	.*,
 	dist
 max-complexity = 10
 max-line-length = 100
 
 [tox:tox]
-envlist = py{38,39,310}
+envlist = py{38,39,310,311}
 
 [testenv]
 deps = .[dev]
 wheel_build_env = build
 commands = 
 	pytest
 
@@ -120,12 +121,13 @@
 	flake8 .
 
 [gh-actions]
 python = 
 	3.8: py38
 	3.9: py39
 	3.10: py310
+	3.11: py311
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `dao-analyzer-1.2.7.dev6/setup.py` & `dao-analyzer-1.2.7.dev7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,14 @@
     if version.dirty:
         return get_local_node_and_date(version)
     else:
         return ""
 
 package_dir = {
   'dao_analyzer.web': 'dao_analyzer/web',
-  'dao_analyzer.cache_scripts':  'cache_scripts',
   # Unfortunately, this package can't be in the same namespace as the others
   # see https://github.com/plotly/dash/issues/2236
   'dao_analyzer_components': 'dao_analyzer_components/dao_analyzer_components',
 }
 
 def util_add_prefix_to_list(prefix, package_list):
     return [ '.'.join([prefix, p]) for p in package_list]
```

### Comparing `dao-analyzer-1.2.7.dev6/test/mocks/api_requester_mock.py` & `dao-analyzer-1.2.7.dev7/test/mocks/api_requester_mock.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/test/mocks/unix_date_builder.py` & `dao-analyzer-1.2.7.dev7/test/mocks/unix_date_builder.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/test/unit/apps/aragon/data_access/daos/metric/strategy/test_aragon_st_new_additions.py` & `dao-analyzer-1.2.7.dev7/test/unit/apps/aragon/data_access/daos/metric/strategy/test_aragon_st_new_additions.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_active_organization_aragon.py` & `dao-analyzer-1.2.7.dev7/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_active_organization_aragon.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_active_token_holders.py` & `dao-analyzer-1.2.7.dev7/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_active_token_holders.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_cast_type.py` & `dao-analyzer-1.2.7.dev7/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_cast_type.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_installed_apps.py` & `dao-analyzer-1.2.7.dev7/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_installed_apps.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_vote_outcome.py` & `dao-analyzer-1.2.7.dev7/test/unit/apps/aragon/data_access/daos/metric/strategy/test_st_vote_outcome.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/test/unit/apps/common/api/graphql/test_query_builder.py` & `dao-analyzer-1.2.7.dev7/test/unit/apps/common/api/graphql/test_query_builder.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/test/unit/apps/common/business/transfers/test_organization.py` & `dao-analyzer-1.2.7.dev7/test/unit/apps/common/business/transfers/test_organization.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_active_members.py` & `dao-analyzer-1.2.7.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_active_members.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_active_organization_daohaus.py` & `dao-analyzer-1.2.7.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_active_organization_daohaus.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_active_voters.py` & `dao-analyzer-1.2.7.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_active_voters.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_dproposal_outcome.py` & `dao-analyzer-1.2.7.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_dproposal_outcome.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_new_additions.py` & `dao-analyzer-1.2.7.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_new_additions.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_proposal_type.py` & `dao-analyzer-1.2.7.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_proposal_type.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_total_members.py` & `dao-analyzer-1.2.7.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_total_members.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_votes_type.py` & `dao-analyzer-1.2.7.dev7/test/unit/apps/daohaus/data_access/daos/metric/strategy/test_st_votes_type.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_active_organization_daostack.py` & `dao-analyzer-1.2.7.dev7/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_active_organization_daostack.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_active_users.py` & `dao-analyzer-1.2.7.dev7/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_active_users.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_diff_voters_stakers.py` & `dao-analyzer-1.2.7.dev7/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_diff_voters_stakers.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_proposal_majority.py` & `dao-analyzer-1.2.7.dev7/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_proposal_majority.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_proposal_outcome.py` & `dao-analyzer-1.2.7.dev7/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_proposal_outcome.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_time_serie.py` & `dao-analyzer-1.2.7.dev7/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_time_serie.py`

 * *Files identical despite different names*

### Comparing `dao-analyzer-1.2.7.dev6/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_voters_percentage.py` & `dao-analyzer-1.2.7.dev7/test/unit/apps/daostack/data_access/daos/metric/strategy/test_st_voters_percentage.py`

 * *Files identical despite different names*

