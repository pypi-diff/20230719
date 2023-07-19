# Comparing `tmp/neomodel-5.0.1.tar.gz` & `tmp/neomodel-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neomodel-5.0.1.tar", last modified: Thu Jun  1 16:08:29 2023, max compression
+gzip compressed data, was "neomodel-5.1.0.tar", last modified: Wed Jul 19 14:10:58 2023, max compression
```

## Comparing `neomodel-5.0.1.tar` & `neomodel-5.1.0.tar`

### file list

```diff
@@ -1,111 +1,117 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:08:29.497851 neomodel-5.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 16:08:17.000000 neomodel-5.0.1/.env
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:08:29.489851 neomodel-5.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-01 16:08:17.000000 neomodel-5.0.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:08:29.489851 neomodel-5.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-06-01 16:08:17.000000 neomodel-5.0.1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-06-01 16:08:17.000000 neomodel-5.0.1/.github/workflows/integration-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-01 16:08:17.000000 neomodel-5.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-01 16:08:17.000000 neomodel-5.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-01 16:08:17.000000 neomodel-5.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-01 16:08:17.000000 neomodel-5.0.1/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15896 2023-06-01 16:08:17.000000 neomodel-5.0.1/Changelog
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-01 16:08:17.000000 neomodel-5.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-06-01 16:08:29.497851 neomodel-5.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-06-01 16:08:17.000000 neomodel-5.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-01 16:08:17.000000 neomodel-5.0.1/dev
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:08:29.489851 neomodel-5.0.1/doc/
--rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:08:29.493851 neomodel-5.0.1/doc/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:08:29.493851 neomodel-5.0.1/doc/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/source/_static/neomodel-148.png
--rw-r--r--   0 runner    (1001) docker     (123)     9528 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/source/_static/neomodel-300.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:08:29.489851 neomodel-5.0.1/doc/source/_themes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:08:29.493851 neomodel-5.0.1/doc/source/_themes/alabaster/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/source/_themes/alabaster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/source/_themes/alabaster/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/source/_themes/alabaster/about.html
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/source/_themes/alabaster/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/source/_themes/alabaster/navigation.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:08:29.493851 neomodel-5.0.1/doc/source/_themes/alabaster/static/
--rw-r--r--   0 runner    (1001) docker     (123)     9905 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/source/_themes/alabaster/static/alabaster.css_t
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/source/_themes/alabaster/support.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/source/_themes/alabaster/theme.conf
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/source/batch.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9076 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/source/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/source/cypher.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/source/extending.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/source/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/source/hooks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/source/module_documentation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/source/properties.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/source/queries.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11814 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/source/relationships.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/source/spatial_properties.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/source/transactions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-01 16:08:17.000000 neomodel-5.0.1/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:08:29.493851 neomodel-5.0.1/neomodel/
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-01 16:08:17.000000 neomodel-5.0.1/neomodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-06-01 16:08:17.000000 neomodel-5.0.1/neomodel/cardinality.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-01 16:08:17.000000 neomodel-5.0.1/neomodel/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:08:29.497851 neomodel-5.0.1/neomodel/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-01 16:08:17.000000 neomodel-5.0.1/neomodel/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-01 16:08:17.000000 neomodel-5.0.1/neomodel/contrib/semi_structured.py
--rw-r--r--   0 runner    (1001) docker     (123)    14800 2023-06-01 16:08:17.000000 neomodel-5.0.1/neomodel/contrib/spatial_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    22464 2023-06-01 16:08:17.000000 neomodel-5.0.1/neomodel/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     8706 2023-06-01 16:08:17.000000 neomodel-5.0.1/neomodel/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-01 16:08:17.000000 neomodel-5.0.1/neomodel/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    28792 2023-06-01 16:08:17.000000 neomodel-5.0.1/neomodel/match.py
--rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-06-01 16:08:17.000000 neomodel-5.0.1/neomodel/match_q.py
--rw-r--r--   0 runner    (1001) docker     (123)    18532 2023-06-01 16:08:17.000000 neomodel-5.0.1/neomodel/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-06-01 16:08:17.000000 neomodel-5.0.1/neomodel/relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)    17147 2023-06-01 16:08:17.000000 neomodel-5.0.1/neomodel/relationship_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    14887 2023-06-01 16:08:17.000000 neomodel-5.0.1/neomodel/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:08:29.497851 neomodel-5.0.1/neomodel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-06-01 16:08:29.000000 neomodel-5.0.1/neomodel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-06-01 16:08:29.000000 neomodel-5.0.1/neomodel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 16:08:29.000000 neomodel-5.0.1/neomodel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-01 16:08:29.000000 neomodel-5.0.1/neomodel.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-01 16:08:29.000000 neomodel-5.0.1/neomodel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-01 16:08:29.000000 neomodel-5.0.1/neomodel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-01 16:08:17.000000 neomodel-5.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-01 16:08:17.000000 neomodel-5.0.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:08:29.497851 neomodel-5.0.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-01 16:08:17.000000 neomodel-5.0.1/scripts/docker-neo4j.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1959 2023-06-01 16:08:17.000000 neomodel-5.0.1/scripts/neomodel_install_labels.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1044 2023-06-01 16:08:17.000000 neomodel-5.0.1/scripts/neomodel_remove_labels.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 16:08:29.497851 neomodel-5.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:08:29.497851 neomodel-5.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_cardinality.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:08:29.497851 neomodel-5.0.1/test/test_contrib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_contrib/test_semi_structured.py
--rw-r--r--   0 runner    (1001) docker     (123)    13020 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_contrib/test_spatial_datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     8997 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_contrib/test_spatial_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_cypher.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_issue112.py
--rw-r--r--   0 runner    (1001) docker     (123)    14083 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_issue283.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_issue600.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_label_drop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_label_install.py
--rw-r--r--   0 runner    (1001) docker     (123)    13365 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_match_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6588 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    12384 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_relationship_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_relationships.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_relative_relationships.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-01 16:08:17.000000 neomodel-5.0.1/tests-with-docker-compose.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:10:58.391070 neomodel-5.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 14:10:46.000000 neomodel-5.1.0/.env
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:10:58.379069 neomodel-5.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-19 14:10:46.000000 neomodel-5.1.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:10:58.379069 neomodel-5.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-07-19 14:10:46.000000 neomodel-5.1.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-19 14:10:46.000000 neomodel-5.1.0/.github/workflows/integration-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-19 14:10:46.000000 neomodel-5.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-19 14:10:46.000000 neomodel-5.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-19 14:10:46.000000 neomodel-5.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-19 14:10:46.000000 neomodel-5.1.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-19 14:10:46.000000 neomodel-5.1.0/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16119 2023-07-19 14:10:46.000000 neomodel-5.1.0/Changelog
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-19 14:10:46.000000 neomodel-5.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-07-19 14:10:58.387070 neomodel-5.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-07-19 14:10:46.000000 neomodel-5.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-19 14:10:46.000000 neomodel-5.1.0/dev
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:10:58.379069 neomodel-5.1.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-07-19 14:10:46.000000 neomodel-5.1.0/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-07-19 14:10:46.000000 neomodel-5.1.0/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-19 14:10:46.000000 neomodel-5.1.0/doc/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:10:58.379069 neomodel-5.1.0/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:10:58.379069 neomodel-5.1.0/doc/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-07-19 14:10:46.000000 neomodel-5.1.0/doc/source/_static/neomodel-148.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9528 2023-07-19 14:10:46.000000 neomodel-5.1.0/doc/source/_static/neomodel-300.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:10:58.375069 neomodel-5.1.0/doc/source/_themes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:10:58.383069 neomodel-5.1.0/doc/source/_themes/alabaster/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-19 14:10:46.000000 neomodel-5.1.0/doc/source/_themes/alabaster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-19 14:10:46.000000 neomodel-5.1.0/doc/source/_themes/alabaster/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-19 14:10:46.000000 neomodel-5.1.0/doc/source/_themes/alabaster/about.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-19 14:10:46.000000 neomodel-5.1.0/doc/source/_themes/alabaster/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-19 14:10:46.000000 neomodel-5.1.0/doc/source/_themes/alabaster/navigation.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:10:58.383069 neomodel-5.1.0/doc/source/_themes/alabaster/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     9905 2023-07-19 14:10:46.000000 neomodel-5.1.0/doc/source/_themes/alabaster/static/alabaster.css_t
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-07-19 14:10:46.000000 neomodel-5.1.0/doc/source/_themes/alabaster/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-19 14:10:46.000000 neomodel-5.1.0/doc/source/_themes/alabaster/theme.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-19 14:10:46.000000 neomodel-5.1.0/doc/source/batch.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9076 2023-07-19 14:10:46.000000 neomodel-5.1.0/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-19 14:10:46.000000 neomodel-5.1.0/doc/source/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-19 14:10:46.000000 neomodel-5.1.0/doc/source/cypher.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12252 2023-07-19 14:10:46.000000 neomodel-5.1.0/doc/source/extending.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-07-19 14:10:46.000000 neomodel-5.1.0/doc/source/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-19 14:10:46.000000 neomodel-5.1.0/doc/source/hooks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-19 14:10:46.000000 neomodel-5.1.0/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-19 14:10:46.000000 neomodel-5.1.0/doc/source/module_documentation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-07-19 14:10:46.000000 neomodel-5.1.0/doc/source/properties.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-07-19 14:10:46.000000 neomodel-5.1.0/doc/source/queries.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11814 2023-07-19 14:10:46.000000 neomodel-5.1.0/doc/source/relationships.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-07-19 14:10:46.000000 neomodel-5.1.0/doc/source/spatial_properties.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-07-19 14:10:46.000000 neomodel-5.1.0/doc/source/transactions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-19 14:10:46.000000 neomodel-5.1.0/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:10:58.383069 neomodel-5.1.0/docker-scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-19 14:10:46.000000 neomodel-5.1.0/docker-scripts/docker-neo4j.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-19 14:10:46.000000 neomodel-5.1.0/docker-scripts/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-19 14:10:46.000000 neomodel-5.1.0/docker-scripts/tests-with-docker-compose.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:10:58.383069 neomodel-5.1.0/neomodel/
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-19 14:10:46.000000 neomodel-5.1.0/neomodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-07-19 14:10:46.000000 neomodel-5.1.0/neomodel/cardinality.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-19 14:10:46.000000 neomodel-5.1.0/neomodel/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:10:58.383069 neomodel-5.1.0/neomodel/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-19 14:10:46.000000 neomodel-5.1.0/neomodel/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-19 14:10:46.000000 neomodel-5.1.0/neomodel/contrib/semi_structured.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26520 2023-07-19 14:10:46.000000 neomodel-5.1.0/neomodel/contrib/spatial_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24148 2023-07-19 14:10:46.000000 neomodel-5.1.0/neomodel/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-07-19 14:10:46.000000 neomodel-5.1.0/neomodel/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-19 14:10:46.000000 neomodel-5.1.0/neomodel/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33920 2023-07-19 14:10:46.000000 neomodel-5.1.0/neomodel/match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-07-19 14:10:46.000000 neomodel-5.1.0/neomodel/match_q.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18532 2023-07-19 14:10:46.000000 neomodel-5.1.0/neomodel/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-07-19 14:10:46.000000 neomodel-5.1.0/neomodel/relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17522 2023-07-19 14:10:46.000000 neomodel-5.1.0/neomodel/relationship_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:10:58.387070 neomodel-5.1.0/neomodel/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 14:10:46.000000 neomodel-5.1.0/neomodel/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1953 2023-07-19 14:10:46.000000 neomodel-5.1.0/neomodel/scripts/neomodel_install_labels.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1038 2023-07-19 14:10:46.000000 neomodel-5.1.0/neomodel/scripts/neomodel_remove_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16564 2023-07-19 14:10:46.000000 neomodel-5.1.0/neomodel/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:10:58.383069 neomodel-5.1.0/neomodel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-07-19 14:10:58.000000 neomodel-5.1.0/neomodel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-07-19 14:10:58.000000 neomodel-5.1.0/neomodel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 14:10:58.000000 neomodel-5.1.0/neomodel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-19 14:10:58.000000 neomodel-5.1.0/neomodel.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-19 14:10:58.000000 neomodel-5.1.0/neomodel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 14:10:58.000000 neomodel-5.1.0/neomodel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-19 14:10:46.000000 neomodel-5.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-19 14:10:46.000000 neomodel-5.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 14:10:58.391070 neomodel-5.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:10:58.387070 neomodel-5.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 14:10:46.000000 neomodel-5.1.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-07-19 14:10:46.000000 neomodel-5.1.0/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-19 14:10:46.000000 neomodel-5.1.0/test/test_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-07-19 14:10:46.000000 neomodel-5.1.0/test/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-07-19 14:10:46.000000 neomodel-5.1.0/test/test_cardinality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-19 14:10:46.000000 neomodel-5.1.0/test/test_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:10:58.387070 neomodel-5.1.0/test/test_contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 14:10:46.000000 neomodel-5.1.0/test/test_contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-19 14:10:46.000000 neomodel-5.1.0/test/test_contrib/test_semi_structured.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14863 2023-07-19 14:10:46.000000 neomodel-5.1.0/test/test_contrib/test_spatial_datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-07-19 14:10:46.000000 neomodel-5.1.0/test/test_contrib/test_spatial_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-19 14:10:46.000000 neomodel-5.1.0/test/test_cypher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-19 14:10:46.000000 neomodel-5.1.0/test/test_database_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-19 14:10:46.000000 neomodel-5.1.0/test/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-19 14:10:46.000000 neomodel-5.1.0/test/test_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-19 14:10:46.000000 neomodel-5.1.0/test/test_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-19 14:10:46.000000 neomodel-5.1.0/test/test_issue112.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14083 2023-07-19 14:10:46.000000 neomodel-5.1.0/test/test_issue283.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-19 14:10:46.000000 neomodel-5.1.0/test/test_issue600.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-19 14:10:46.000000 neomodel-5.1.0/test/test_label_drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-19 14:10:46.000000 neomodel-5.1.0/test/test_label_install.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14845 2023-07-19 14:10:46.000000 neomodel-5.1.0/test/test_match_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-07-19 14:10:46.000000 neomodel-5.1.0/test/test_migration_neo4j_5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-07-19 14:10:46.000000 neomodel-5.1.0/test/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-19 14:10:46.000000 neomodel-5.1.0/test/test_multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12400 2023-07-19 14:10:46.000000 neomodel-5.1.0/test/test_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-07-19 14:10:46.000000 neomodel-5.1.0/test/test_relationship_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-07-19 14:10:46.000000 neomodel-5.1.0/test/test_relationships.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-19 14:10:46.000000 neomodel-5.1.0/test/test_relative_relationships.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-07-19 14:10:46.000000 neomodel-5.1.0/test/test_transactions.py
```

### Comparing `neomodel-5.0.1/.github/workflows/codeql-analysis.yml` & `neomodel-5.1.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.1/.github/workflows/integration-tests.yml` & `neomodel-5.1.0/.github/workflows/integration-tests.yml`

 * *Files 23% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 # This workflow will install Python dependencies, run tests and lint with a variety of Python versions
 # For more information see: https://docs.github.com/en/actions/automating-builds-and-tests/building-and-testing-python
 
 name: Integration tests
 
 on:
   push:
-    branches: [ "master" ]
+    branches: [ "master", "rc/**" ]
   pull_request:
-    branches: [ "master", "rc/*" ]
+    branches: [ "master", "rc/**" ]
 
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
         python-version: ["3.11", "3.10", "3.9", "3.8", "3.7"]
-        neo4j-version: ["5.4", "4.4"]
+        neo4j-version: ["enterprise", "5.5-enterprise", "4.4-enterprise"]
 
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python-version }}
     - name: Creating Neo4j Container
       run: |
-        chmod +x ./scripts/docker-neo4j.sh
-        sh ./scripts/docker-neo4j.sh ${{ matrix.neo4j-version }}
+        chmod +x ./docker-scripts/docker-neo4j.sh
+        sh ./docker-scripts/docker-neo4j.sh ${{ matrix.neo4j-version }}
         sleep 30s
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -e '.[dev]'
     - name: Test with pytest
       env:
         AURA_TEST_DB_USER: ${{ secrets.AURA_TEST_DB_USER }}
         AURA_TEST_DB_PASSWORD: ${{ secrets.AURA_TEST_DB_PASSWORD }}
         AURA_TEST_DB_HOSTNAME: ${{ secrets.AURA_TEST_DB_HOSTNAME }}
       run: |
         pytest --cov=neomodel --cov-report=html:coverage_report
     - name: Upload coverage reports to Codecov
-      uses: codecov/codecov-action@v3
+      uses: codecov/codecov-action@v3
```

### Comparing `neomodel-5.0.1/.github/workflows/python-publish.yml` & `neomodel-5.1.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.1/AUTHORS.txt` & `neomodel-5.1.0/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.1/Changelog` & `neomodel-5.1.0/Changelog`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,18 @@
+Version 5.1.0 2023-07
+* Bumped neo4j-driver version to 5.10.0
+* Breaking change : When using neomodel along with Neo4j version 5, use StructuredNode and StructuredRel's element_id property instead of id. If you have Cypher queries which currently use the id() function, migrate them to elementId() instead.
+If you use Neo4j version 4.4, this change should be transparent to you, and you should keep using id() function in Cypher since elementId() is not implemented in 4.4.
+* Bump Shapely to >= 2.0.0
+* Fix schema scripts invocation
+* Removed custom __str__ method, part of NodeClassRegistry, from Database() (db) object.
+
 Version 5.0.1 2023-06
 * Removed deprecated methods StructuredRel.delete and RelationshipManager.search
 * Extended test coverage, fixed some typos, improve linting
-* Upcoming breaking change notice : Version 5.1.0 will introduce a breaking change for users targeting a Neo4j database in version 5. This release will introduce Neo4j's new element_id, which replaces id. The breaking change will happen if you have custom Cypher queries that do things like "WHERE id(n)=$id" => you will have to use Cypher's elementId() function instead starting from neomodel 5.1.0
 
 Version 5.0.0 2023-03
 * Confirmed support of Neo4j versions 5.x and 4.4 (LTS)
 * Dropped support of EOL Neo4j versions (4.3 and below)
 * Confirmed support of Python 3.11
 * Migrated RelationshipTo/RelationshipFrom from a method to a class for consistency.
 * Add support for relationship indexes
```

### Comparing `neomodel-5.0.1/LICENSE` & `neomodel-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.1/PKG-INFO` & `neomodel-5.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neomodel
-Version: 5.0.1
+Version: 5.1.0
 Summary: An object mapper for the neo4j graph database.
 Author-email: Robin Edwards <robin.ge@gmail.com>
 Maintainer: Cristina Escalante
 Maintainer-email: Athanasios Anastasiou <athanastasiou@gmail.com>, Marius Conjeaud <marius.conjeaud@outlook.com>
 License: MIT
 Project-URL: documentation, https://neomodel.readthedocs.io/en/latest/
 Project-URL: repository, http://github.com/neo4j-contrib/neomodel
```

### Comparing `neomodel-5.0.1/README.rst` & `neomodel-5.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.1/doc/Makefile` & `neomodel-5.1.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.1/doc/make.bat` & `neomodel-5.1.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.1/doc/source/_static/neomodel-148.png` & `neomodel-5.1.0/doc/source/_static/neomodel-148.png`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.1/doc/source/_static/neomodel-300.png` & `neomodel-5.1.0/doc/source/_static/neomodel-300.png`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.1/doc/source/_themes/alabaster/about.html` & `neomodel-5.1.0/doc/source/_themes/alabaster/about.html`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.1/doc/source/_themes/alabaster/layout.html` & `neomodel-5.1.0/doc/source/_themes/alabaster/layout.html`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.1/doc/source/_themes/alabaster/static/alabaster.css_t` & `neomodel-5.1.0/doc/source/_themes/alabaster/static/alabaster.css_t`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.1/doc/source/_themes/alabaster/support.py` & `neomodel-5.1.0/doc/source/_themes/alabaster/support.py`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.1/doc/source/_themes/alabaster/theme.conf` & `neomodel-5.1.0/doc/source/_themes/alabaster/theme.conf`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.1/doc/source/batch.rst` & `neomodel-5.1.0/doc/source/batch.rst`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.1/doc/source/conf.py` & `neomodel-5.1.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.1/doc/source/configuration.rst` & `neomodel-5.1.0/doc/source/configuration.rst`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.1/doc/source/cypher.rst` & `neomodel-5.1.0/doc/source/cypher.rst`

 * *Files 11% similar despite different names*

```diff
@@ -29,11 +29,13 @@
 
 You may log queries and timings by setting the environment variable `NEOMODEL_CYPHER_DEBUG` to `1`.
 
 Utilities
 =========
 The following utility functions are available::
 
-    clear_neo4j_database(db)  # deletes all nodes and relationships
+    # Deletes all nodes and relationships.
+    # Optionally, can drop all constraints and/or indexes. It preserves the default lookup indexes
+    clear_neo4j_database(db, clear_constraints=False, clear_indexes=False)
 
-    # Change database password (you will need to call db.set_connection(...) after
-    change_neo4j_password(db, new_password)
+    # Change database password (you will need to call db.set_connection(...) to reset connection)
+    change_neo4j_password(db, user, new_password)
```

### Comparing `neomodel-5.0.1/doc/source/extending.rst` & `neomodel-5.1.0/doc/source/extending.rst`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,35 @@
     class Shopper(User):
         balance = IntegerProperty(index=True)
 
         def credit_account(self, amount):
             self.balance = self.balance + int(amount)
             self.save()
 
+
+Optional Labels
+---------------
+Sometimes it is useful to allow a node to have extra labels in addition to the
+ones Neomodel defines by default using class names.
+
+Nemodel constructs sets of labels to give to a node in Neo4j by looking at the
+names of the node classes that node is/inherits from. It also constructs a
+mapping of the reverse, expected node labels to node classes, in order to do
+object resolution.
+
+In order for object resolution to work on Node Classes that could have extra
+labels, the `__optional_labels__` property must be defined as a list of strings::
+
+    class Shopper(StructuredNode):
+        __optional_labels__ = ["SuperSaver", "SeniorDiscount"]
+        balance = IntegerProperty(index=True)
+
+.. warning:: The size of the node class mapping grows exponentially with optional labels. Use with some caution.
+
+
 Mixins
 ------
 Mixins can be used to share functionality between nodes classes::
 
     class UserMixin:
         name = StringProperty(unique_index=True)
         password = StringProperty()
```

### Comparing `neomodel-5.0.1/doc/source/getting_started.rst` & `neomodel-5.1.0/doc/source/getting_started.rst`

 * *Files 18% similar despite different names*

```diff
@@ -49,32 +49,39 @@
     from neomodel import config
 
     config.DATABASE_URL = os.environ["NEO4J_BOLT_URL"]
 
 Defining Node Entities and Relationships
 ========================================
 
-Below is a definition of two related nodes `Person` and `Country`: ::
+Below is a definition of three related nodes `Person`, `City` and `Country`: ::
 
     from neomodel import (config, StructuredNode, StringProperty, IntegerProperty,
         UniqueIdProperty, RelationshipTo)
 
     config.DATABASE_URL = 'bolt://neo4j:password@localhost:7687'
 
     class Country(StructuredNode):
         code = StringProperty(unique_index=True, required=True)
 
+    class City(StructuredNode):
+        name = StringProperty(required=True)
+        country = RelationshipTo(Country, 'FROM_COUNTRY')
+
     class Person(StructuredNode):
         uid = UniqueIdProperty()
         name = StringProperty(unique_index=True)
         age = IntegerProperty(index=True, default=0)
 
         # traverse outgoing IS_FROM relations, inflate to Country objects
         country = RelationshipTo(Country, 'IS_FROM')
 
+        # traverse outgoing LIVES_IN relations, inflate to City objects
+        city = RelationshipTo(City, 'LIVES_IN')
+
 Nodes are defined in the same way classes are defined in Python with the only difference that data members of those
 classes that are intended to be stored to the database must be defined as ``neomodel`` property objects. For more
 detailed information on property objects please see the section on :ref:`property_types`.
 
 **If** you have a need to attach "ad-hoc" properties to nodes that have not been specified at its definition, then 
 consider deriving from the :ref:`semistructurednode_doc` class.
 
@@ -114,15 +121,15 @@
 Using convenience methods such as::
 
     jim = Person(name='Jim', age=3).save() # Create
     jim.age = 4
     jim.save() # Update, (with validation)
     jim.delete()
     jim.refresh() # reload properties from the database
-    jim.id # neo4j internal id
+    jim.element_id # neo4j internal element id
 
 Retrieving nodes
 ================
 
 Using the ``.nodes`` class property::
 
     # Return all nodes
@@ -150,14 +157,17 @@
 Relationships
 =============
 
 Working with relationships::
 
     germany = Country(code='DE').save()
     jim.country.connect(germany)
+    berlin = City(name='Berlin').save()
+    berlin.country.connect(germany)
+    jim.city.connect(berlin)
 
     if jim.country.is_connected(germany):
         print("Jim's from Germany")
 
     for p in germany.inhabitant.all():
         print(p.name) # Jim
 
@@ -179,7 +189,52 @@
     # Remove all of Jim's country relationships
     jim.country.disconnect_all()
 
     jim.country.connect(usa)
     # Replace Jim's country relationship with a new one
     jim.country.replace(germany)
 
+
+Retrieving additional relations
+===============================
+
+To avoid queries multiplication, you have the possibility to retrieve
+additional relations with a single call::
+
+    # The following call will generate one MATCH with traversal per
+    # item in .fetch_relations() call
+    results = Person.nodes.all().fetch_relations('country')
+    for result in results:
+        print(result[0]) # Person
+        print(result[1]) # associated Country
+
+You can traverse more than one hop in your relations using the
+following syntax::
+
+    # Go from person to City then Country
+    Person.nodes.all().fetch_relations('city__country')
+
+You can also force the use of an ``OPTIONAL MATCH`` statement using
+the following syntax::
+
+    from neomodel.match import Optional
+
+    results = Person.nodes.all().fetch_relations(Optional('country'))
+
+.. note::
+
+   You can fetch one or more relations within the same call
+   to `.fetch_relations()` and you can mix optional and non-optional
+   relations, like::
+
+    Person.nodes.all().fetch_relations('city__country', Optional('country'))
+
+.. warning::
+
+   This feature is still a work in progress for extending path traversal and fecthing.
+   It currently stops at returning the resolved objects as they are returned in Cypher.
+   So for instance, if your path looks like ``(startNode:Person)-[r1]->(middleNode:City)<-[r2]-(endNode:Country)``,
+   then you will get a list of results, where each result is a list of ``(startNode, r1, middleNode, r2, endNode)``.
+   These will be resolved by neomodel, so ``startNode`` will be a ``Person`` class as defined in neomodel for example.
+
+   If you want to go further in the resolution process, you have to develop your own parser (for now).
+
```

### Comparing `neomodel-5.0.1/doc/source/hooks.rst` & `neomodel-5.1.0/doc/source/hooks.rst`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.1/doc/source/index.rst` & `neomodel-5.1.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.1/doc/source/module_documentation.rst` & `neomodel-5.1.0/doc/source/module_documentation.rst`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.1/doc/source/properties.rst` & `neomodel-5.1.0/doc/source/properties.rst`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.1/doc/source/queries.rst` & `neomodel-5.1.0/doc/source/queries.rst`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.1/doc/source/relationships.rst` & `neomodel-5.1.0/doc/source/relationships.rst`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.1/doc/source/spatial_properties.rst` & `neomodel-5.1.0/doc/source/spatial_properties.rst`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.1/doc/source/transactions.rst` & `neomodel-5.1.0/doc/source/transactions.rst`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.1/docker-compose.yml` & `neomodel-5.1.0/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.1/neomodel/__init__.py` & `neomodel-5.1.0/neomodel/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,8 +34,8 @@
 from .relationship import StructuredRel
 from .util import change_neo4j_password, clear_neo4j_database
 
 __author__ = "Robin Edwards"
 __email__ = "robin.ge@gmail.com"
 __license__ = "MIT"
 __package__ = "neomodel"
-__version__ = "5.0.1"
+__version__ = "5.1.0"
```

### Comparing `neomodel-5.0.1/neomodel/cardinality.py` & `neomodel-5.1.0/neomodel/cardinality.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,12 +124,12 @@
         """
         Connect a node
 
         :param node:
         :param properties: relationship properties
         :return: True / rel instance
         """
-        if not hasattr(self.source, "id"):
+        if not hasattr(self.source, "element_id"):
             raise ValueError("Node has not been saved cannot connect!")
         if len(self):
             raise AttemptedCardinalityViolation("Node already has one relationship")
         return super().connect(node, properties)
```

### Comparing `neomodel-5.0.1/neomodel/contrib/semi_structured.py` & `neomodel-5.1.0/neomodel/contrib/semi_structured.py`

 * *Files 17% similar despite different names*

```diff
@@ -22,17 +22,17 @@
     """
 
     __abstract_node__ = True
 
     @classmethod
     def inflate(cls, node):
         # support lazy loading
-        if isinstance(node, int):
+        if isinstance(node, str) or isinstance(node, int):
             snode = cls()
-            snode.id = node
+            snode.element_id_property = node
         else:
             props = {}
             node_properties = {}
             for key, prop in cls.__all_properties__:
                 node_properties = _get_node_properties(node)
                 if key in node_properties:
                     props[key] = prop.inflate(node_properties[key], node)
@@ -40,24 +40,25 @@
                     props[key] = prop.default_value()
                 else:
                     props[key] = None
             # handle properties not defined on the class
             for free_key in (x for x in node_properties if x not in props):
                 if hasattr(cls, free_key):
                     raise InflateConflict(
-                        cls, free_key, node_properties[free_key], node.id
+                        cls, free_key, node_properties[free_key], node.element_id
                     )
                 props[free_key] = node_properties[free_key]
 
             snode = cls(**props)
-            snode.id = node.id
+            snode.element_id_property = node.element_id
 
         return snode
 
     @classmethod
     def deflate(cls, node_props, obj=None, skip_empty=False):
         deflated = super().deflate(node_props, obj, skip_empty=skip_empty)
         for key in [k for k in node_props if k not in deflated]:
-            if hasattr(cls, key):
-                raise DeflateConflict(cls, key, deflated[key], obj.id)
+            if hasattr(cls, key) and (getattr(cls,key).required or not skip_empty):
+                raise DeflateConflict(cls, key, deflated[key], obj.element_id)
+
         node_props.update(deflated)
         return node_props
```

### Comparing `neomodel-5.0.1/neomodel/contrib/spatial_properties.py` & `neomodel-5.1.0/neomodel/contrib/spatial_properties.py`

 * *Files 24% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 __author__ = "Athanasios Anastasiou"
 
 import neo4j.spatial
 
 # If shapely is not installed, its import will fail and the spatial properties will not be available
 try:
     from shapely.geometry import Point as ShapelyPoint
+    from shapely import __version__ as shapely_version
+    from shapely.coords import CoordinateSequence 
 except ImportError as exc:
     raise ImportError(
         "NEOMODEL ERROR: Shapely not found. If required, you can install Shapely via "
         "`pip install shapely`."
     ) from exc
 
 from neomodel.properties import Property, validator
@@ -45,222 +47,453 @@
 SRID_TO_CRS = {
     7203: "cartesian",
     9157: "cartesian-3d",
     4326: "wgs-84",
     4979: "wgs-84-3d",
 }
 
-
-class NeomodelPoint(ShapelyPoint):
-    """
-    Abstracts the Point spatial data type of Neo4j.
-
-    Note:
-    At the time of writing, Neo4j supports 2 main variants of Point:
-        1. A generic point defined over a Cartesian plane
-            * The minimum data to define a point is x, y [,z] when crs is either "cartesian" or "cartesian-3d"
-        2. A generic point defined over the WGS84 ellipsoid
-            * The minimum data to define a point is longitude, latitude [,Height] and the crs is then assumed
-              to be "wgs-84".
-    """
-
-    # def __init__(self, *args, crs=None, x=None, y=None, z=None, latitude=None, longitude=None, height=None, **kwargs):
-    def __init__(self, *args, **kwargs):
+# Taking into account the Shapely 2.0.0 changes in the way POINT objects are initialisd.
+if int("".join(shapely_version.split(".")[0:3])) < 200:
+    class NeomodelPoint(ShapelyPoint):
         """
-        Creates a NeomodelPoint.
-
-        :param args: Positional arguments to emulate the behaviour of Shapely's Point (and specifically the copy
-        constructor)
-        :type args: list
-        :param crs: Coordinate Reference System, must be one of ['cartesian', 'cartesian-3d', 'wgs-84', 'wgs-84-3d']
-        :type crs: str
-        :param x: x coordinate of point
-        :type x: float
-        :param y: y coordinate of point
-        :type y: float
-        :param z: z coordinate of point if the crs is cartesian-3d
-        :type z: float
-        :param latitude: Latitude of point
-        :type latitude: float
-        :param longitude: Longitude of point
-        :type longitude: float
-        :param height: Height of point if the crs is wgs-84-3d
-        :type height: float
-        :param kwargs: Dictionary of keyword arguments
-        :type kwargs: dict
+        Abstracts the Point spatial data type of Neo4j.
+    
+        Note:
+        At the time of writing, Neo4j supports 2 main variants of Point:
+            1. A generic point defined over a Cartesian plane
+                * The minimum data to define a point is x, y [,z] when crs is either "cartesian" or "cartesian-3d"
+            2. A generic point defined over the WGS84 ellipsoid
+                * The minimum data to define a point is longitude, latitude [,Height] and the crs is then assumed
+                  to be "wgs-84".
         """
-
-        # Python2.7 Workaround for the order that the arguments get passed to the functions
-        crs = kwargs.pop("crs", None)
-        x = kwargs.pop("x", None)
-        y = kwargs.pop("y", None)
-        z = kwargs.pop("z", None)
-        longitude = kwargs.pop("longitude", None)
-        latitude = kwargs.pop("latitude", None)
-        height = kwargs.pop("height", None)
-
-        _x, _y, _z = None, None, None
-
-        # CRS validity check is common to both types of constructors that follow
-        if crs is not None and crs not in ACCEPTABLE_CRS:
-            raise ValueError(f"Invalid CRS({crs}). Expected one of {','.join(ACCEPTABLE_CRS)}")
-        self._crs = crs
-
-        # If positional arguments have been supplied, then this is a possible call to the copy constructor or
-        # initialisation by a coordinate iterable as per ShapelyPoint constructor.
-        if len(args) > 0:
-            # If a coordinate iterable was passed, emulate a call with x,y[,z] parameters
-            if isinstance(args[0], (tuple, list)):
-                # Check dimensionality of tuple
-                if len(args[0]) < 2 or len(args[0]) > 3:
-                    raise ValueError(f"Invalid vector dimensions. Expected 2 or 3, received {len(args[0])}")
-                x = args[0][0]
-                y = args[0][1]
-                if len(args[0]) == 3:
-                    z = args[0][2]
-            # If another "Point" was passed, then this is a call to the copy constructor
-            elif isinstance(args[0], ShapelyPoint):
-                super().__init__(args[0])
-                # If the other Point was a NeomodelPoint then it bears the CRS that is used to
-                # interpret the points and this has to be carried over.
-                if isinstance(args[0], NeomodelPoint):
-                    self._crs = args[0]._crs
-                else:
-                    # This allows NeomodelPoint((0,0),crs="wgs-84") which will interpret the tuple as
-                    # (longitude,latitude) even though it was not specified as such with the named arguments.
-                    #
-                    # NOTE: Notice the indexing on the coordinates `args[0].coords[0]`. Coordinates are always an
-                    # iterable which for Points has length of 1 but for other geometrical objects (e.g. boundaries)
-                    # might be longer. This will come back to bite you, if you assume that `coords` is what it pretends
-                    # to be (i.e. coords gives access to the actual coordinates NOT an iterable).
-                    #
-                    if len(args[0].coords[0]) == 2:
-                        if crs is None:
-                            self._crs = "cartesian"
-                    elif len(args[0].coords[0]) == 3:
-                        if crs is None:
-                            self._crs = "cartesian-3d"
+    
+        # def __init__(self, *args, crs=None, x=None, y=None, z=None, latitude=None, longitude=None, height=None, **kwargs):
+        def __init__(self, *args, **kwargs):
+            """
+            Creates a NeomodelPoint.
+    
+            :param args: Positional arguments to emulate the behaviour of Shapely's Point (and specifically the copy
+            constructor)
+            :type args: list
+            :param crs: Coordinate Reference System, must be one of ['cartesian', 'cartesian-3d', 'wgs-84', 'wgs-84-3d']
+            :type crs: str
+            :param x: x coordinate of point
+            :type x: float
+            :param y: y coordinate of point
+            :type y: float
+            :param z: z coordinate of point if the crs is cartesian-3d
+            :type z: float
+            :param latitude: Latitude of point
+            :type latitude: float
+            :param longitude: Longitude of point
+            :type longitude: float
+            :param height: Height of point if the crs is wgs-84-3d
+            :type height: float
+            :param kwargs: Dictionary of keyword arguments
+            :type kwargs: dict
+            """
+    
+            # Python2.7 Workaround for the order that the arguments get passed to the functions
+            crs = kwargs.pop("crs", None)
+            x = kwargs.pop("x", None)
+            y = kwargs.pop("y", None)
+            z = kwargs.pop("z", None)
+            longitude = kwargs.pop("longitude", None)
+            latitude = kwargs.pop("latitude", None)
+            height = kwargs.pop("height", None)
+    
+            _x, _y, _z = None, None, None
+    
+            # CRS validity check is common to both types of constructors that follow
+            if crs is not None and crs not in ACCEPTABLE_CRS:
+                raise ValueError(f"Invalid CRS({crs}). Expected one of {','.join(ACCEPTABLE_CRS)}")
+            self._crs = crs
+    
+            # If positional arguments have been supplied, then this is a possible call to the copy constructor or
+            # initialisation by a coordinate iterable as per ShapelyPoint constructor.
+            if len(args) > 0:
+                # If a coordinate iterable was passed, emulate a call with x,y[,z] parameters
+                if isinstance(args[0], (tuple, list)):
+                    # Check dimensionality of tuple
+                    if len(args[0]) < 2 or len(args[0]) > 3:
+                        raise ValueError(f"Invalid vector dimensions. Expected 2 or 3, received {len(args[0])}")
+                    x = args[0][0]
+                    y = args[0][1]
+                    if len(args[0]) == 3:
+                        z = args[0][2]
+                # If another "Point" was passed, then this is a call to the copy constructor
+                elif isinstance(args[0], ShapelyPoint):
+                    super().__init__(args[0])
+                    # If the other Point was a NeomodelPoint then it bears the CRS that is used to
+                    # interpret the points and this has to be carried over.
+                    if isinstance(args[0], NeomodelPoint):
+                        self._crs = args[0]._crs
                     else:
-                        raise ValueError(f"Invalid vector dimensions. Expected 2 or 3, received {len(args[0].coords[0])}")
-                return
+                        # This allows NeomodelPoint((0,0),crs="wgs-84") which will interpret the tuple as
+                        # (longitude,latitude) even though it was not specified as such with the named arguments.
+                        #
+                        # NOTE: Notice the indexing on the coordinates `args[0].coords[0]`. Coordinates are always an
+                        # iterable which for Points has length of 1 but for other geometrical objects (e.g. boundaries)
+                        # might be longer. This will come back to bite you, if you assume that `coords` is what it pretends
+                        # to be (i.e. coords gives access to the actual coordinates NOT an iterable).
+                        #
+                        if len(args[0].coords[0]) == 2:
+                            if crs is None:
+                                self._crs = "cartesian"
+                        elif len(args[0].coords[0]) == 3:
+                            if crs is None:
+                                self._crs = "cartesian-3d"
+                        else:
+                            raise ValueError(f"Invalid vector dimensions. Expected 2 or 3, received {len(args[0].coords[0])}")
+                    return
+                else:
+                    raise TypeError(f"Invalid object passed to copy constructor. Expected NeomodelPoint or shapely Point, received {type(args[0])}")
+    
+            # Initialisation is either via x,y[,z] XOR longitude,latitude[,height]. Specifying both leads to an error.
+            if any(i is not None for i in [x, y, z]) and any(
+                i is not None for i in [latitude, longitude, height]
+            ):
+                raise ValueError(
+                    "Invalid instantiation via arguments. "
+                    "A Point can be defined either by x,y,z coordinates OR latitude,longitude,height but not "
+                    "a combination of these terms"
+                )
+    
+            # Specifying no initialisation argument at this point in the constructor is flagged as an error
+            if all(i is None for i in [x, y, z, latitude, longitude, height]):
+                raise ValueError(
+                    "Invalid instantiation via no arguments. "
+                    "A Point needs default values either in x,y,z or longitude, latitude, height coordinates"
+                )
+    
+            # Geographical Point Initialisation
+            if latitude is not None and longitude is not None:
+                if height is not None:
+                    if self._crs is None:
+                        self._crs = "wgs-84-3d"
+                    _z = height
+                else:
+                    if self._crs is None:
+                        self._crs = "wgs-84"
+                _x = longitude
+                _y = latitude
+    
+            # Geometrical Point Initialisation
+            if x is not None and y is not None:
+                if z is not None:
+                    if self._crs is None:
+                        self._crs = "cartesian-3d"
+                    _z = z
+                else:
+                    if self._crs is None:
+                        self._crs = "cartesian"
+                _x = x
+                _y = y
+    
+            if _z is None:
+                if "-3d" not in self._crs:
+                    super().__init__((float(_x), float(_y)), **kwargs)
+                else:
+                    raise ValueError(f"Invalid vector dimensions(2) for given CRS({self._crs}).")
             else:
-                raise TypeError(f"Invalid object passed to copy constructor. Expected NeomodelPoint or shapely Point, received {type(args[0])}")
+                if "-3d" in self._crs:
+                    super().__init__((float(_x), float(_y), float(_z)), **kwargs)
+                else:
+                    raise ValueError(f"Invalid vector dimensions(3) for given CRS({self._crs}).")
+    
+        @property
+        def crs(self):
+            return self._crs
+    
+        @property
+        def x(self):
+            if not self._crs.startswith("cartesian"):
+                raise AttributeError(
+                    f'Invalid coordinate ("x") for points defined over {self.crs}'
+                )
+            return super().x
+    
+        @property
+        def y(self):
+            if not self._crs.startswith("cartesian"):
+                raise AttributeError(
+                    f'Invalid coordinate ("y") for points defined over {self.crs}'
+                )
+            return super().y
+    
+        @property
+        def z(self):
+            if not self._crs == "cartesian-3d":
+                raise AttributeError(
+                    f'Invalid coordinate ("z") for points defined over {self.crs}'
+                )
+            return super().z
+    
+        @property
+        def latitude(self):
+            if not self._crs.startswith("wgs-84"):
+                raise AttributeError(
+                    f'Invalid coordinate ("latitude") for points defined over {self.crs}'
+                )
+            return super().y
+    
+        @property
+        def longitude(self):
+            if not self._crs.startswith("wgs-84"):
+                raise AttributeError(
+                    f'Invalid coordinate ("longitude") for points defined over {self.crs}'
+                )
+            return super().x
+    
+        @property
+        def height(self):
+            if not self._crs == "wgs-84-3d":
+                raise AttributeError(
+                    f'Invalid coordinate ("height") for points defined over {self.crs}'
+                )
+            return super().z
+    
+        # The following operations are necessary here due to the way queries (and more importantly their parameters) get
+        # combined and evaluated in neomodel. Specifically, query expressions get duplicated with deep copies and any valid
+        # datatype values should also implement these operations.
+        def __copy__(self):
+            return NeomodelPoint(self)
+    
+        def __deepcopy__(self, memo):
+            return NeomodelPoint(self)
 
-        # Initialisation is either via x,y[,z] XOR longitude,latitude[,height]. Specifying both leads to an error.
-        if any(i is not None for i in [x, y, z]) and any(
-            i is not None for i in [latitude, longitude, height]
-        ):
-            raise ValueError(
-                "Invalid instantiation via arguments. "
-                "A Point can be defined either by x,y,z coordinates OR latitude,longitude,height but not "
-                "a combination of these terms"
-            )
-
-        # Specifying no initialisation argument at this point in the constructor is flagged as an error
-        if all(i is None for i in [x, y, z, latitude, longitude, height]):
-            raise ValueError(
-                "Invalid instantiation via no arguments. "
-                "A Point needs default values either in x,y,z or longitude, latitude, height coordinates"
-            )
-
-        # Geographical Point Initialisation
-        if latitude is not None and longitude is not None:
-            if height is not None:
-                if self._crs is None:
-                    self._crs = "wgs-84-3d"
-                _z = height
-            else:
-                if self._crs is None:
-                    self._crs = "wgs-84"
-            _x = longitude
-            _y = latitude
-
-        # Geometrical Point Initialisation
-        if x is not None and y is not None:
-            if z is not None:
-                if self._crs is None:
-                    self._crs = "cartesian-3d"
-                _z = z
-            else:
-                if self._crs is None:
-                    self._crs = "cartesian"
-            _x = x
-            _y = y
-
-        if _z is None:
-            if "-3d" not in self._crs:
-                super().__init__((float(_x), float(_y)), **kwargs)
-            else:
-                raise ValueError(f"Invalid vector dimensions(2) for given CRS({self._crs}).")
-        else:
-            if "-3d" in self._crs:
-                super().__init__((float(_x), float(_y), float(_z)), **kwargs)
+else:
+    class NeomodelPoint:
+        """
+        Abstracts the Point spatial data type of Neo4j.
+    
+        Note:
+        At the time of writing, Neo4j supports 2 main variants of Point:
+            1. A generic point defined over a Cartesian plane
+                * The minimum data to define a point is x, y [,z] when crs is either "cartesian" or "cartesian-3d"
+            2. A generic point defined over the WGS84 ellipsoid
+                * The minimum data to define a point is longitude, latitude [,Height] and the crs is then assumed
+                  to be "wgs-84".
+        """
+    
+        # def __init__(self, *args, crs=None, x=None, y=None, z=None, latitude=None, longitude=None, height=None, **kwargs):
+        def __init__(self, *args, **kwargs):
+            """
+            Creates a NeomodelPoint.
+    
+            :param args: Positional arguments to emulate the behaviour of Shapely's Point (and specifically the copy
+            constructor)
+            :type args: list
+            :param crs: Coordinate Reference System, must be one of ['cartesian', 'cartesian-3d', 'wgs-84', 'wgs-84-3d']
+            :type crs: str
+            :param x: x coordinate of point
+            :type x: float
+            :param y: y coordinate of point
+            :type y: float
+            :param z: z coordinate of point if the crs is cartesian-3d
+            :type z: float
+            :param latitude: Latitude of point
+            :type latitude: float
+            :param longitude: Longitude of point
+            :type longitude: float
+            :param height: Height of point if the crs is wgs-84-3d
+            :type height: float
+            :param kwargs: Dictionary of keyword arguments
+            :type kwargs: dict
+            """
+    
+            # Python2.7 Workaround for the order that the arguments get passed to the functions
+            crs = kwargs.pop("crs", None)
+            x = kwargs.pop("x", None)
+            y = kwargs.pop("y", None)
+            z = kwargs.pop("z", None)
+            longitude = kwargs.pop("longitude", None)
+            latitude = kwargs.pop("latitude", None)
+            height = kwargs.pop("height", None)
+    
+            _x, _y, _z = None, None, None
+    
+            # CRS validity check is common to both types of constructors that follow
+            if crs is not None and crs not in ACCEPTABLE_CRS:
+                raise ValueError(f"Invalid CRS({crs}). Expected one of {','.join(ACCEPTABLE_CRS)}")
+            self._crs = crs
+    
+            # If positional arguments have been supplied, then this is a possible call to the copy constructor or
+            # initialisation by a coordinate iterable as per ShapelyPoint constructor.
+            if len(args) > 0:
+                # If a coordinate iterable was passed, emulate a call with x,y[,z] parameters
+                if isinstance(args[0], (tuple, list)):
+                    # Check dimensionality of tuple
+                    if len(args[0]) < 2 or len(args[0]) > 3:
+                        raise ValueError(f"Invalid vector dimensions. Expected 2 or 3, received {len(args[0])}")
+                    x = args[0][0]
+                    y = args[0][1]
+                    if len(args[0]) == 3:
+                        z = args[0][2]
+                # If another "Point" was passed, then this is a call to the copy constructor
+                elif isinstance(args[0], (ShapelyPoint, NeomodelPoint)):
+                    if isinstance(args[0], ShapelyPoint):
+                        self._shapely_point = ShapelyPoint(args[0])
+                    # If the other Point was a NeomodelPoint then it bears the CRS that is used to
+                    # interpret the points and this has to be carried over.
+                    if isinstance(args[0], NeomodelPoint):
+                        self._shapely_point = ShapelyPoint(args[0].coords)
+                        self._crs = args[0].crs
+                    else:
+                        # This allows NeomodelPoint((0,0),crs="wgs-84") which will interpret the tuple as
+                        # (longitude,latitude) even though it was not specified as such with the named arguments.
+                        #
+                        # NOTE: Notice the indexing on the coordinates `args[0].coords[0]`. Coordinates are always an
+                        # iterable which for Points has length of 1 but for other geometrical objects (e.g. boundaries)
+                        # might be longer. This will come back to bite you, if you assume that `coords` is what it pretends
+                        # to be (i.e. coords gives access to the actual coordinates NOT an iterable).
+                        #
+                        if len(args[0].coords[0]) == 2:
+                            if crs is None:
+                                self._crs = "cartesian"
+                        elif len(args[0].coords[0]) == 3:
+                            if crs is None:
+                                self._crs = "cartesian-3d"
+                        else:
+                            raise ValueError(f"Invalid vector dimensions. Expected 2 or 3, received {len(args[0].coords[0])}")
+                    return
+                else:
+                    raise TypeError(f"Invalid object passed to copy constructor. Expected NeomodelPoint or shapely Point, received {type(args[0])}")
+    
+            # Initialisation is either via x,y[,z] XOR longitude,latitude[,height]. Specifying both leads to an error.
+            if any(i is not None for i in [x, y, z]) and any(
+                i is not None for i in [latitude, longitude, height]
+            ):
+                raise ValueError(
+                    "Invalid instantiation via arguments. "
+                    "A Point can be defined either by x,y,z coordinates OR latitude,longitude,height but not "
+                    "a combination of these terms"
+                )
+    
+            # Specifying no initialisation argument at this point in the constructor is flagged as an error
+            if all(i is None for i in [x, y, z, latitude, longitude, height]):
+                raise ValueError(
+                    "Invalid instantiation via no arguments. "
+                    "A Point needs default values either in x,y,z or longitude, latitude, height coordinates"
+                )
+    
+            # Geographical Point Initialisation
+            if latitude is not None and longitude is not None:
+                if height is not None:
+                    if self._crs is None:
+                        self._crs = "wgs-84-3d"
+                    _z = height
+                else:
+                    if self._crs is None:
+                        self._crs = "wgs-84"
+                _x = longitude
+                _y = latitude
+    
+            # Geometrical Point Initialisation
+            if x is not None and y is not None:
+                if z is not None:
+                    if self._crs is None:
+                        self._crs = "cartesian-3d"
+                    _z = z
+                else:
+                    if self._crs is None:
+                        self._crs = "cartesian"
+                _x = x
+                _y = y
+    
+            if _z is None:
+                if "-3d" not in self._crs:
+                    self._shapely_point = ShapelyPoint((float(_x), float(_y)))
+                else:
+                    raise ValueError(f"Invalid vector dimensions(2) for given CRS({self._crs}).")
             else:
-                raise ValueError(f"Invalid vector dimensions(3) for given CRS({self._crs}).")
-
-    @property
-    def crs(self):
-        return self._crs
-
-    @property
-    def x(self):
-        if not self._crs.startswith("cartesian"):
-            raise AttributeError(
-                f'Invalid coordinate ("x") for points defined over {self.crs}'
-            )
-        return super().x
-
-    @property
-    def y(self):
-        if not self._crs.startswith("cartesian"):
-            raise AttributeError(
-                f'Invalid coordinate ("y") for points defined over {self.crs}'
-            )
-        return super().y
-
-    @property
-    def z(self):
-        if not self._crs == "cartesian-3d":
-            raise AttributeError(
-                f'Invalid coordinate ("z") for points defined over {self.crs}'
-            )
-        return super().z
-
-    @property
-    def latitude(self):
-        if not self._crs.startswith("wgs-84"):
-            raise AttributeError(
-                f'Invalid coordinate ("latitude") for points defined over {self.crs}'
-            )
-        return super().y
-
-    @property
-    def longitude(self):
-        if not self._crs.startswith("wgs-84"):
-            raise AttributeError(
-                f'Invalid coordinate ("longitude") for points defined over {self.crs}'
-            )
-        return super().x
-
-    @property
-    def height(self):
-        if not self._crs == "wgs-84-3d":
-            raise AttributeError(
-                f'Invalid coordinate ("height") for points defined over {self.crs}'
-            )
-        return super().z
-
-    # The following operations are necessary here due to the way queries (and more importantly their parameters) get
-    # combined and evaluated in neomodel. Specifically, query expressions get duplicated with deep copies and any valid
-    # datatype values should also implement these operations.
-    def __copy__(self):
-        return NeomodelPoint(self)
+                if "-3d" in self._crs:
+                    self._shapely_point = ShapelyPoint((float(_x), float(_y), float(_z)))
+                else:
+                    raise ValueError(f"Invalid vector dimensions(3) for given CRS({self._crs}).")
 
-    def __deepcopy__(self, memo):
-        return NeomodelPoint(self)
+               
+        @property
+        def crs(self):
+            return self._crs
+    
+        @property
+        def x(self):
+            if not self._crs.startswith("cartesian"):
+                raise TypeError(
+                    f'Invalid coordinate ("x") for points defined over {self.crs}'
+                )
+            return self._shapely_point.x
+    
+        @property
+        def y(self):
+            if not self._crs.startswith("cartesian"):
+                raise TypeError(
+                    f'Invalid coordinate ("y") for points defined over {self.crs}'
+                )
+            return self._shapely_point.y
+    
+        @property
+        def z(self):
+            if not self._crs == "cartesian-3d":
+                raise TypeError(
+                    f'Invalid coordinate ("z") for points defined over {self.crs}'
+                )
+            return self._shapely_point.z
+    
+        @property
+        def latitude(self):
+            if not self._crs.startswith("wgs-84"):
+                raise TypeError(
+                    f'Invalid coordinate ("latitude") for points defined over {self.crs}'
+                )
+            return self._shapely_point.y
+    
+        @property
+        def longitude(self):
+            if not self._crs.startswith("wgs-84"):
+                raise TypeError(
+                    f'Invalid coordinate ("longitude") for points defined over {self.crs}'
+                )
+            return self._shapely_point.x
+    
+        @property
+        def height(self):
+            if not self._crs == "wgs-84-3d":
+                raise TypeError(
+                    f'Invalid coordinate ("height") for points defined over {self.crs}'
+                )
+            return self._shapely_point.z
+    
+        # The following operations are necessary here due to the way queries (and more importantly their parameters) get
+        # combined and evaluated in neomodel. Specifically, query expressions get duplicated with deep copies and any valid
+        # datatype values should also implement these operations.
+        def __copy__(self):
+            return NeomodelPoint(self)
+    
+        def __deepcopy__(self, memo):
+            return NeomodelPoint(self)
+
+        def __getattr__(self, attr):
+            """
+            Route messages to the right underlying object.
+            """
+            return getattr(self._shapely_point, attr)
+
+        def __eq__(self, other):
+            """
+            Compare objects by value
+            """
+            if not isinstance(other, (ShapelyPoint, NeomodelPoint)):
+                raise ValueException(f"NeomodelPoint equality comparison expected NeomodelPoint or Shapely Point, received {type(other)}")
+            else:
+                if isinstance(other, ShapelyPoint):
+                    return self.coords[0] == other.coords[0]
+                else:
+                    return self.coords[0] == other.coords[0] and self.crs == other.crs
 
 
 class PointProperty(Property):
     """
     Validates points which can participate in spatial queries.
     """
```

### Comparing `neomodel-5.0.1/neomodel/core.py` & `neomodel-5.1.0/neomodel/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import re
 import sys
 import warnings
+from itertools import combinations
 
 from neo4j.exceptions import ClientError
 
 from neomodel import config
 from neomodel.exceptions import DoesNotExist, NodeClassAlreadyDefined
 from neomodel.hooks import hooks
 from neomodel.properties import Property, PropertyManager
@@ -38,34 +38,29 @@
             )
     if not quiet:
         stdout.write("\n")
 
 
 def drop_indexes(quiet=True, stdout=None):
     """
-    Discover and drop all indexes.
+    Discover and drop all indexes, except the automatically created token lookup indexes.
 
     :type: bool
     :return: None
     """
     if not stdout or stdout is None:
         stdout = sys.stdout
 
-    results, meta = db.cypher_query("SHOW INDEXES")
-    results_as_dict = [dict(zip(meta, row)) for row in results]
-    for index in results_as_dict:
-        # Neo4j 4.3 introduced token lookup indexes
-        # Two are created automatically so should not be dropped
-        # They can be recognized because their labelsOrTypes and properties arrays are empty
-        if index["labelsOrTypes"] and index["properties"]:
-            db.cypher_query("DROP INDEX " + index["name"])
-            if not quiet:
-                stdout.write(
-                    f' - Dropping index on labels {",".join(index["labelsOrTypes"])} with properties {",".join(index["properties"])}.\n'
-                )
+    indexes = db.list_indexes(exclude_token_lookup=True)
+    for index in indexes:
+        db.cypher_query("DROP INDEX " + index["name"])
+        if not quiet:
+            stdout.write(
+                f' - Dropping index on labels {",".join(index["labelsOrTypes"])} with properties {",".join(index["properties"])}.\n'
+            )
     if not quiet:
         stdout.write("\n")
 
 
 def remove_all_labels(stdout=None):
     """
     Calls functions for dropping constraints and indexes.
@@ -244,23 +239,35 @@
                 cls.defined_properties(properties=False, rels=False).items()
             )
             cls.__all_relationships__ = tuple(
                 cls.defined_properties(aliases=False, properties=False).items()
             )
 
             cls.__label__ = namespace.get("__label__", name)
+            cls.__optional_labels__ = namespace.get("__optional_labels__", [])
 
             if config.AUTO_INSTALL_LABELS:
                 install_labels(cls, quiet=False)
 
-            label_set = frozenset(cls.inherited_labels())
-            if label_set not in db._NODE_CLASS_REGISTRY:
-                db._NODE_CLASS_REGISTRY[label_set] = cls
-            else:
-                raise NodeClassAlreadyDefined(cls, db._NODE_CLASS_REGISTRY)
+            base_label_set = frozenset(cls.inherited_labels())
+            optional_label_set = set(cls.inherited_optional_labels())
+
+            # Construct all possible combinations of labels + optional labels
+            possible_label_combinations = [
+                frozenset(set(x).union(base_label_set))
+                for i in range(1, len(optional_label_set) + 1)
+                for x in combinations(optional_label_set, i)
+            ]
+            possible_label_combinations.append(base_label_set)
+
+            for label_set in possible_label_combinations:
+                if label_set not in db._NODE_CLASS_REGISTRY:
+                    db._NODE_CLASS_REGISTRY[label_set] = cls
+                else:
+                    raise NodeClassAlreadyDefined(cls, db._NODE_CLASS_REGISTRY)
 
         return cls
 
 
 NodeBase = NodeMeta("NodeBase", (PropertyManager,), {"__abstract_node__": True})
 
 
@@ -286,16 +293,16 @@
             self.__dict__[key] = val.build_manager(self, key)
 
         super().__init__(*args, **kwargs)
 
     def __eq__(self, other):
         if not isinstance(other, (StructuredNode,)):
             return False
-        if hasattr(self, "id") and hasattr(other, "id"):
-            return self.id == other.id
+        if hasattr(self, "element_id") and hasattr(other, "element_id"):
+            return self.element_id == other.element_id
         return False
 
     def __ne__(self, other):
         return not self.__eq__(other)
 
     def __repr__(self):
         return f"<{self.__class__.__name__}: {self}>"
@@ -312,14 +319,32 @@
         :return: NodeSet
         :rtype: NodeSet
         """
         from .match import NodeSet
 
         return NodeSet(cls)
 
+    @property
+    def element_id(self):
+        return (
+            int(self.element_id_property)
+            if db.database_version.startswith("4")
+            else self.element_id_property
+        )
+
+    # Version 4.4 support - id is deprecated in version 5.x
+    @property
+    def id(self):
+        try:
+            return int(self.element_id_property)
+        except (TypeError, ValueError):
+            raise ValueError(
+                "id is deprecated in Neo4j version 5, please migrate to element_id. If you use the id in a Cypher query, replace id() by elementId()."
+            )
+
     # methods
 
     @classmethod
     def _build_merge_query(
         cls, merge_params, update_existing=False, lazy=False, relationship=None
     ):
         """
@@ -329,33 +354,40 @@
         :type merge_params: list of dict
         :param update_existing: True to update properties of existing nodes, default False to keep existing values.
         :type update_existing: bool
         :rtype: tuple
         """
         query_params = dict(merge_params=merge_params)
         n_merge_labels = ":".join(cls.inherited_labels())
-        n_merge_prm = ", ".join((f"{getattr(cls, p).db_property or p}: params.create.{getattr(cls, p).db_property or p}" for p in cls.__required_properties__))
+        n_merge_prm = ", ".join(
+            (
+                f"{getattr(cls, p).db_property or p}: params.create.{getattr(cls, p).db_property or p}"
+                for p in cls.__required_properties__
+            )
+        )
         n_merge = f"n:{n_merge_labels} {{{n_merge_prm}}}"
         if relationship is None:
             # create "simple" unwind query
             query = f"UNWIND $merge_params as params\n MERGE ({n_merge})\n "
         else:
             # validate relationship
             if not isinstance(relationship.source, StructuredNode):
-                raise ValueError(f"relationship source [{repr(relationship.source)}] is not a StructuredNode")
+                raise ValueError(
+                    f"relationship source [{repr(relationship.source)}] is not a StructuredNode"
+                )
             relation_type = relationship.definition.get("relation_type")
             if not relation_type:
                 raise ValueError(
                     "No relation_type is specified on provided relationship"
                 )
 
             from .match import _rel_helper
 
-            query_params["source_id"] = relationship.source.id
-            query = f"MATCH (source:{relationship.source.__label__}) WHERE ID(source) = $source_id\n "
+            query_params["source_id"] = relationship.source.element_id
+            query = f"MATCH (source:{relationship.source.__label__}) WHERE {db.get_id_method()}(source) = $source_id\n "
             query += "WITH source\n UNWIND $merge_params as params \n "
             query += "MERGE "
             query += _rel_helper(
                 lhs="source",
                 rhs=n_merge,
                 ident=None,
                 relation_type=relation_type,
@@ -365,25 +397,21 @@
         query += "ON CREATE SET n = params.create\n "
         # if update_existing, write properties on match as well
         if update_existing is True:
             query += "ON MATCH SET n += params.update\n"
 
         # close query
         if lazy:
-            query += "RETURN id(n)"
+            query += f"RETURN {db.get_id_method()}(n)"
         else:
             query += "RETURN n"
 
         return query, query_params
 
     @classmethod
-    def category(cls):
-        raise NotImplementedError(f"Category was deprecated and has now been removed, the functionality is now achieved using the {cls.__name__}.nodes attribute")
-
-    @classmethod
     def create(cls, *props, **kwargs):
         """
         Call to CREATE with parameters map. A new instance will be created and saved.
 
         :param props: dict of properties to create the nodes.
         :type props: tuple
         :param lazy: False by default, specify True to get nodes with id only without the parameters.
@@ -400,15 +428,15 @@
 
         lazy = kwargs.get("lazy", False)
         # create mapped query
         query = f"CREATE (n:{':'.join(cls.inherited_labels())} $create_params)"
 
         # close query
         if lazy:
-            query += " RETURN id(n)"
+            query += f" RETURN {db.get_id_method()}(n)"
         else:
             query += " RETURN n"
 
         results = []
         for item in [
             cls.deflate(p, obj=_UnsavedNode(), skip_empty=True) for p in props
         ]:
@@ -480,31 +508,29 @@
         :param params: query parameters
         :type: dict
         :return: list containing query results
         :rtype: list
         """
         self._pre_action_check("cypher")
         params = params or {}
-        params.update({"self": self.id})
+        params.update({"self": self.element_id})
         return db.cypher_query(query, params)
 
     @hooks
     def delete(self):
         """
-        Delete a node and it's relationships
+        Delete a node and its relationships
 
         :return: True
         """
         self._pre_action_check("delete")
         self.cypher(
-            "MATCH (self) WHERE id(self)=$self "
-            "OPTIONAL MATCH (self)-[r]-()"
-            " DELETE r, self"
+            f"MATCH (self) WHERE {db.get_id_method()}(self)=$self DETACH DELETE self"
         )
-        delattr(self, "id")
+        delattr(self, "element_id_property")
         self.deleted = True
         return True
 
     @classmethod
     def get_or_create(cls, *props, **kwargs):
         """
         Call to MERGE with parameters map. A new instance will be created and saved if does not already exist,
@@ -546,17 +572,17 @@
     def inflate(cls, node):
         """
         Inflate a raw neo4j_driver node to a neomodel node
         :param node:
         :return: node object
         """
         # support lazy loading
-        if isinstance(node, int):
+        if isinstance(node, str) or isinstance(node, int):
             snode = cls()
-            snode.id = node
+            snode.element_id_property = node
         else:
             node_properties = _get_node_properties(node)
             props = {}
             for key, prop in cls.__all_properties__:
                 # map property name from database to object property
                 db_property = prop.db_property or key
 
@@ -564,15 +590,15 @@
                     props[key] = prop.inflate(node_properties[db_property], node)
                 elif prop.has_default:
                     props[key] = prop.default_value()
                 else:
                     props[key] = None
 
             snode = cls(**props)
-            snode.id = node.id
+            snode.element_id_property = node.element_id
 
         return snode
 
     @classmethod
     def inherited_labels(cls):
         """
         Return list of labels from nodes class hierarchy.
@@ -581,41 +607,60 @@
         """
         return [
             scls.__label__
             for scls in cls.mro()
             if hasattr(scls, "__label__") and not hasattr(scls, "__abstract_node__")
         ]
 
+    @classmethod
+    def inherited_optional_labels(cls):
+        """
+        Return list of optional labels from nodes class hierarchy.
+
+        :return: list
+        :rtype: list
+        """
+        return [
+            label
+            for scls in cls.mro()
+            for label in getattr(scls, "__optional_labels__", [])
+            if not hasattr(scls, "__abstract_node__")
+        ]
+
     def labels(self):
         """
         Returns list of labels tied to the node from neo4j.
 
         :return: list of labels
         :rtype: list
         """
         self._pre_action_check("labels")
-        return self.cypher("MATCH (n) WHERE id(n)=$self " "RETURN labels(n)")[0][0][0]
+        return self.cypher(
+            f"MATCH (n) WHERE {db.get_id_method()}(n)=$self " "RETURN labels(n)"
+        )[0][0][0]
 
     def _pre_action_check(self, action):
         if hasattr(self, "deleted") and self.deleted:
             raise ValueError(
                 f"{self.__class__.__name__}.{action}() attempted on deleted node"
             )
-        if not hasattr(self, "id"):
+        if not hasattr(self, "element_id"):
             raise ValueError(
                 f"{self.__class__.__name__}.{action}() attempted on unsaved node"
             )
 
     def refresh(self):
         """
         Reload the node from neo4j
         """
         self._pre_action_check("refresh")
-        if hasattr(self, "id"):
-            request = self.cypher("MATCH (n) WHERE id(n)=$self" " RETURN n")[0]
+        if hasattr(self, "element_id"):
+            request = self.cypher(
+                f"MATCH (n) WHERE {db.get_id_method()}(n)=$self RETURN n"
+            )[0]
             if not request or not request[0]:
                 raise self.__class__.DoesNotExist("Can't refresh non existent node")
             node = self.inflate(request[0][0])
             for key, val in node.__properties__.items():
                 setattr(self, key, val)
         else:
             raise ValueError("Can't refresh unsaved node")
@@ -625,24 +670,29 @@
         """
         Save the node to neo4j or raise an exception
 
         :return: the node instance
         """
 
         # create or update instance node
-        if hasattr(self, "id"):
+        if hasattr(self, "element_id"):
             # update
             params = self.deflate(self.__properties__, self)
-            query = "MATCH (n) WHERE id(n)=$self \n"
-            query += "\n".join(
-                [f"SET n.{key} = ${key}" + "\n" for key in params.keys()]
-            )
-            for label in self.inherited_labels():
-                query += f"SET n:`{label}`\n"
+            query = f"MATCH (n) WHERE {db.get_id_method()}(n)=$self\n"
+
+            if params:
+                query += "SET "
+                query += ",\n".join([f"n.{key} = ${key}" for key in params])
+                query += "\n"
+            if self.inherited_labels():
+                query += "\n".join(
+                    [f"SET n:`{label}`" for label in self.inherited_labels()]
+                )
             self.cypher(query, params)
         elif hasattr(self, "deleted") and self.deleted:
             raise ValueError(
                 f"{self.__class__.__name__}.save() attempted on deleted node"
             )
         else:  # create
-            self.id = self.create(self.__properties__)[0].id
+            created_node = self.create(self.__properties__)[0]
+            self.element_id_property = created_node.element_id
         return self
```

### Comparing `neomodel-5.0.1/neomodel/exceptions.py` & `neomodel-5.1.0/neomodel/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 class NeomodelException(Exception):
     """
     A base class that identifies all exceptions raised by :mod:`neomodel`.
     """
+
     pass
 
 
 class AttemptedCardinalityViolation(NeomodelException):
     """
     Attempted to alter the database state against the cardinality definitions.
 
     Example: a relationship of type `One` trying to connect a second node.
     """
+
     pass
 
 
 class CardinalityViolation(NeomodelException):
     """
     The state of database doesn't match the nodes cardinality definition.
 
@@ -22,15 +24,17 @@
     """
 
     def __init__(self, rel_manager, actual):
         self.rel_manager = str(rel_manager)
         self.actual = str(actual)
 
     def __str__(self):
-        return f"CardinalityViolation: Expected: {self.rel_manager}, got: {self.actual}."
+        return (
+            f"CardinalityViolation: Expected: {self.rel_manager}, got: {self.actual}."
+        )
 
 
 class ModelDefinitionException(NeomodelException):
     """
     Abstract exception to handle error conditions related to the node-to-class registry.
     """
 
@@ -84,14 +88,15 @@
     a data model object.
     """
 
     def __str__(self):
         relationship_type = self.db_node_rel_class.type
         return f"Relationship of type {relationship_type} does not resolve to any of the known objects\n{self._get_node_class_registry_formatted()}\n"
 
+
 class RelationshipClassRedefined(ModelDefinitionException):
     """
     Raised when an attempt is made to re-map a relationship label to a relationship model of an entirely different type
     """
 
     def __init__(
         self,
@@ -124,14 +129,15 @@
     """
 
     def __str__(self):
         node_class_labels = ",".join(self.db_node_rel_class.inherited_labels())
 
         return f"Class {self.db_node_rel_class.__module__}.{self.db_node_rel_class.__name__} with labels {node_class_labels} already defined:\n{self._get_node_class_registry_formatted()}\n"
 
+
 class ConstraintValidationFailed(ValueError, NeomodelException):
     def __init__(self, msg):
         self.message = msg
 
 
 class DeflateError(ValueError, NeomodelException):
     def __init__(self, key, cls, msg, obj):
@@ -182,37 +188,40 @@
         self.node_class = cls
         self.msg = msg
         self.obj = repr(obj)
 
     def __str__(self):
         return f"Attempting to inflate property '{self.property_name}' on {self.obj} of class '{self.node_class.__name__}': {self.msg}"
 
+
 class DeflateConflict(InflateConflict):
     def __init__(self, cls, key, value, nid):
         self.cls_name = cls.__name__
         self.property_name = key
         self.value = value
         self.nid = nid if nid else "(unsaved)"
 
     def __str__(self):
         return f"Found trying to set property '{self.property_name}' with value '{self.value}' on node {self.nid} although class {self.cls_name} already has a property '{self.property_name}'"
 
+
 class MultipleNodesReturned(ValueError, NeomodelException):
     def __init__(self, msg):
         self.message = msg
 
 
 class NotConnected(NeomodelException):
     def __init__(self, action, node1, node2):
         self.action = action
         self.node1 = node1
         self.node2 = node2
 
     def __str__(self):
-        return f"Error performing '{self.action}' - Node {self.node1.id} of type '{self.node1.__class__.__name__}' is not connected to {self.node2.id} of type '{self.node2.__class__.__name__}'."
+        return f"Error performing '{self.action}' - Node {self.node1.element_id} of type '{self.node1.__class__.__name__}' is not connected to {self.node2.element_id} of type '{self.node2.__class__.__name__}'."
+
 
 class RequiredProperty(NeomodelException):
     def __init__(self, key, cls):
         self.property_name = key
         self.node_class = cls
 
     def __str__(self):
```

### Comparing `neomodel-5.0.1/neomodel/match.py` & `neomodel-5.1.0/neomodel/match.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import inspect
 import re
+from collections import defaultdict
+from dataclasses import dataclass
 
 from .core import StructuredNode, db
 from .exceptions import MultipleNodesReturned
 from .match_q import Q, QBase
 from .properties import AliasProperty
 
 OUTGOING, INCOMING, EITHER = 1, -1, 0
@@ -39,22 +41,23 @@
     :param ident: A specific identity to name the relationship, or None.
     :type ident: str
     :param relation_type: None for all direct rels, * for all of any length, or a name of an explicit rel.
     :type relation_type: str
     :param direction: None or EITHER for all OUTGOING,INCOMING,EITHER. Otherwise OUTGOING or INCOMING.
     :param relation_properties: dictionary of relationship properties to match
     :returns: string
-    """ 
+    """
     rel_props = ""
 
     if relation_properties:
-        rel_props_str = ', '.join((f"{key}: {value}" for key, value in relation_properties.items()))
+        rel_props_str = ", ".join(
+            (f"{key}: {value}" for key, value in relation_properties.items())
+        )
         rel_props = f" {{{rel_props_str}}}"
 
-    
     rel_def = ""
     # direct, relation_type=None is unspecified, relation_type
     if relation_type is None:
         rel_def = ""
     # all("*" wildcard) relation_type
     elif relation_type == "*":
         rel_def = "[*]"
@@ -65,16 +68,22 @@
     stmt = ""
     if direction == OUTGOING:
         stmt = f"-{rel_def}->"
     elif direction == INCOMING:
         stmt = f"<-{rel_def}-"
     else:
         stmt = f"-{rel_def}-"
-        
-    return f"({lhs}){stmt}({rhs})"
+
+    # Make sure not to add parenthesis when they are already present
+    if lhs[-1] != ")":
+        lhs = f"({lhs})"
+    if rhs[-1] != ")":
+        rhs = f"({rhs})"
+
+    return f"{lhs}{stmt}{rhs}"
 
 
 def _rel_merge_helper(
     lhs,
     rhs,
     ident="neomodelident",
     relation_type=None,
@@ -109,19 +118,33 @@
     else:
         stmt = "-{0}-"
 
     rel_props = ""
     rel_none_props = ""
 
     if relation_properties:
-        rel_props_str = ", ".join((f"{key}: {value}" for key, value in relation_properties.items() if value is not None))
+        rel_props_str = ", ".join(
+            (
+                f"{key}: {value}"
+                for key, value in relation_properties.items()
+                if value is not None
+            )
+        )
         rel_props = f" {{{rel_props_str}}}"
         if None in relation_properties.values():
-            rel_prop_val_str = ", ".join((f"{ident}.{key}=${key!s}" for key, value in relation_properties.items() if value is None))
-            rel_none_props = f" ON CREATE SET {rel_prop_val_str} ON MATCH SET {rel_prop_val_str}"
+            rel_prop_val_str = ", ".join(
+                (
+                    f"{ident}.{key}=${key!s}"
+                    for key, value in relation_properties.items()
+                    if value is None
+                )
+            )
+            rel_none_props = (
+                f" ON CREATE SET {rel_prop_val_str} ON MATCH SET {rel_prop_val_str}"
+            )
     # direct, relation_type=None is unspecified, relation_type
     if relation_type is None:
         stmt = stmt.format("")
     # all("*" wildcard) relation_type
     elif relation_type == "*":
         stmt = stmt.format("[*]")
     else:
@@ -183,17 +206,15 @@
     For a StructuredNode class install Traversal objects for each
     relationship definition on a NodeSet instance
     """
     rels = cls.defined_properties(rels=True, aliases=False, properties=False)
 
     for key in rels.keys():
         if hasattr(node_set, key):
-            raise ValueError(
-                f"Cannot install traversal '{key}' exists on NodeSet"
-            )
+            raise ValueError(f"Cannot install traversal '{key}' exists on NodeSet")
 
         rel = getattr(cls, key)
         rel._lookup_node_class()
 
         traversal = Traversal(source=node_set, name=key, definition=rel.definition)
         setattr(node_set, key, traversal)
 
@@ -261,17 +282,15 @@
     """
     rel_definitions = cls.defined_properties(properties=False, rels=True, aliases=False)
 
     match, dont_match = {}, {}
 
     for key, value in kwargs.items():
         if key not in rel_definitions:
-            raise ValueError(
-                f"No such relation {key} defined on a {cls.__name__}"
-            )
+            raise ValueError(f"No such relation {key} defined on a {cls.__name__}")
 
         rhs_ident = key
 
         rel_definitions[key]._lookup_node_class()
 
         if value is True:
             match[rhs_ident] = rel_definitions[key].definition
@@ -284,20 +303,25 @@
 
     return match, dont_match
 
 
 class QueryBuilder:
     def __init__(self, node_set):
         self.node_set = node_set
-        self._ast = {"match": [], "where": []}
+        self._ast = {"match": [], "where": [], "optional match": []}
         self._query_params = {}
         self._place_holder_registry = {}
         self._ident_count = 0
+        self._node_counters = defaultdict(int)
 
     def build_ast(self):
+        if hasattr(self.node_set, "relations_to_fetch"):
+            for relation in self.node_set.relations_to_fetch:
+                self.build_traversal_from_path(relation, self.node_set.source)
+
         self.build_source(self.node_set)
 
         if hasattr(self.node_set, "skip"):
             self._ast["skip"] = self.node_set.skip
         if hasattr(self.node_set, "limit"):
             self._ast["limit"] = self.node_set.limit
 
@@ -337,17 +361,15 @@
         return "r" + str(self._ident_count)
 
     def build_order_by(self, ident, source):
         if "?" in source._order_by:
             self._ast["with"] = f"{ident}, rand() as r"
             self._ast["order_by"] = "r"
         else:
-            self._ast["order_by"] = [
-                f"{ident}.{p}" for p in source._order_by
-            ]
+            self._ast["order_by"] = [f"{ident}.{p}" for p in source._order_by]
 
     def build_traversal(self, traversal):
         """
         traverse a relationship from a node to a set of nodes
         """
         # build source
         rhs_label = ":" + traversal.target_class.__label__
@@ -368,36 +390,96 @@
         self._ast["match"].append(stmt)
 
         if traversal.filters:
             self.build_where_stmt(rel_ident, traversal.filters)
 
         return traversal.name
 
+    def _additional_return(self, name):
+        key = "additional_return"
+        if key not in self._ast:
+            self._ast[key] = []
+        if name not in self._ast[key] and name != self._ast.get("return"):
+            self._ast[key].append(name)
+
+    def build_traversal_from_path(self, relation: dict, source_class) -> str:
+        path: str = relation["path"]
+        stmt: str = ""
+        source_class_iterator = source_class
+        for index, part in enumerate(path.split("__")):
+            relationship = getattr(source_class_iterator, part)
+            # build source
+            if "node_class" not in relationship.definition:
+                relationship._lookup_node_class()
+            rhs_label = relationship.definition["node_class"].__label__
+            rel_reference = f'{relationship.definition["node_class"]}_{part}'
+            self._node_counters[rel_reference] += 1
+            rhs_name = (
+                f"{rhs_label.lower()}_{part}_{self._node_counters[rel_reference]}"
+            )
+            rhs_ident = f"{rhs_name}:{rhs_label}"
+            self._additional_return(rhs_name)
+            if not stmt:
+                lhs_label = source_class_iterator.__label__
+                lhs_name = lhs_label.lower()
+                lhs_ident = f"{lhs_name}:{lhs_label}"
+                if not index:
+                    # This is the first one, we make sure that 'return'
+                    # contains the primary node so _contains() works
+                    # as usual
+                    self._ast["return"] = lhs_name
+                else:
+                    self._additional_return(lhs_name)
+            else:
+                lhs_ident = stmt
+
+            rel_ident = self.create_ident()
+            self._additional_return(rel_ident)
+            stmt = _rel_helper(
+                lhs=lhs_ident,
+                rhs=rhs_ident,
+                ident=rel_ident,
+                direction=relationship.definition["direction"],
+                relation_type=relationship.definition["relation_type"],
+            )
+            source_class_iterator = relationship.definition["node_class"]
+
+        if relation.get("optional"):
+            self._ast["optional match"].append(stmt)
+        else:
+            self._ast["match"].append(stmt)
+        return rhs_name
+
     def build_node(self, node):
         ident = node.__class__.__name__.lower()
         place_holder = self._register_place_holder(ident)
 
         # Hack to emulate START to lookup a node by id
-        _node_lookup = f"MATCH ({ident}) WHERE id({ident})=${place_holder} WITH {ident}"
+        _node_lookup = f"MATCH ({ident}) WHERE {db.get_id_method()}({ident})=${place_holder} WITH {ident}"
         self._ast["lookup"] = _node_lookup
 
-        self._query_params[place_holder] = node.id
+        self._query_params[place_holder] = node.element_id
 
         self._ast["return"] = ident
         self._ast["result_class"] = node.__class__
         return ident
 
     def build_label(self, ident, cls):
         """
         match nodes by a label
         """
         ident_w_label = ident + ":" + cls.__label__
-        self._ast["match"].append(f"({ident_w_label})")
-        self._ast["return"] = ident
-        self._ast["result_class"] = cls
+
+        if not self._ast.get("return") and (
+            "additional_return" not in self._ast
+            or ident not in self._ast["additional_return"]
+        ):
+            self._ast["match"].append(f"({ident_w_label})")
+            self._ast["return"] = ident
+            self._ast["result_class"] = cls
         return ident
 
     def build_additional_match(self, ident, node_set):
         """
         handle additional matches supplied by 'has()' calls
         """
         source_ident = ident
@@ -469,41 +551,59 @@
                     negate = True
                     row = row["__NOT__"]
 
                 for prop, operator_and_val in row.items():
                     operator, val = operator_and_val
                     if operator in _UNARY_OPERATORS:
                         # unary operators do not have a parameter
-                        statement = f"{'NOT' if negate else ''} {ident}.{prop} {operator}"
+                        statement = (
+                            f"{'NOT' if negate else ''} {ident}.{prop} {operator}"
+                        )
                     else:
                         place_holder = self._register_place_holder(ident + "_" + prop)
                         statement = f"{'NOT' if negate else ''} {ident}.{prop} {operator} ${place_holder}"
                         self._query_params[place_holder] = val
                     stmts.append(statement)
 
             self._ast["where"].append(" AND ".join(stmts))
 
     def build_query(self):
         query = ""
 
         if "lookup" in self._ast:
             query += self._ast["lookup"]
 
-        query += " MATCH "
-        query += ", ".join([f"({i})" for i in self._ast["match"]])
+        # Instead of using only one MATCH statement for every relation
+        # to follow, we use one MATCH per relation (to avoid cartesian
+        # product issues...).
+        # There might be optimizations to be done, using projections,
+        # or pusing patterns instead of a chain of OPTIONAL MATCH.
+        if len(self._ast["match"]) > 0:
+            query += " MATCH "
+            query += " MATCH ".join(i for i in self._ast["match"])
+
+        if len(self._ast["optional match"]):
+            query += " OPTIONAL MATCH "
+            query += " OPTIONAL MATCH ".join(i for i in self._ast["optional match"])
 
         if "where" in self._ast and self._ast["where"]:
             query += " WHERE "
             query += " AND ".join(self._ast["where"])
 
         if "with" in self._ast and self._ast["with"]:
             query += " WITH "
             query += self._ast["with"]
 
-        query += " RETURN " + self._ast["return"]
+        query += " RETURN "
+        if "return" in self._ast:
+            query += self._ast["return"]
+        if "additional_return" in self._ast:
+            if "return" in self._ast:
+                query += ", "
+            query += ", ".join(self._ast["additional_return"])
 
         if "order_by" in self._ast and self._ast["order_by"]:
             query += " ORDER BY "
             query += ", ".join(self._ast["order_by"])
 
         if "skip" in self._ast:
             query += f" SKIP {self._ast['skip']:d}"
@@ -513,39 +613,50 @@
 
         return query
 
     def _count(self):
         self._ast["return"] = f"count({self._ast['return']})"
         # drop order_by, results in an invalid query
         self._ast.pop("order_by", None)
+        # drop additional_return to avoid unexpected result
+        self._ast.pop("additional_return", None)
         query = self.build_query()
         results, _ = db.cypher_query(query, self._query_params)
         return int(results[0][0])
 
-    def _contains(self, node_id):
+    def _contains(self, node_element_id):
         # inject id = into ast
+        if "return" not in self._ast:
+            print(self._ast["additional_return"])
+            self._ast["return"] = self._ast["additional_return"][0]
         ident = self._ast["return"]
         place_holder = self._register_place_holder(ident + "_contains")
-        self._ast["where"].append(f"id({ident}) = ${place_holder}")
-        self._query_params[place_holder] = node_id
+        self._ast["where"].append(f"{db.get_id_method()}({ident}) = ${place_holder}")
+        self._query_params[place_holder] = node_element_id
         return self._count() >= 1
 
     def _execute(self, lazy=False):
         if lazy:
-            # inject id = into ast
-            self._ast["return"] = f"id({self._ast['return']})"
+            # inject id() into return or return_set
+            if "return" in self._ast:
+                self._ast["return"] = f"{db.get_id_method()}({self._ast['return']})"
+            else:
+                self._ast["additional_return"] = [
+                    f"{db.get_id_method()}({item})"
+                    for item in self._ast["additional_return"]
+                ]
         query = self.build_query()
         results, _ = db.cypher_query(query, self._query_params, resolve_objects=True)
         # The following is not as elegant as it could be but had to be copied from the
         # version prior to cypher_query with the resolve_objects capability.
         # It seems that certain calls are only supposed to be focusing to the first
         # result item returned (?)
-        if results:
+        if results and len(results[0]) == 1:
             return [n[0] for n in results]
-        return []
+        return results
 
 
 class BaseSet:
     """
     Base class for all node sets.
 
     Contains common python magic methods, __len__, __contains__ etc
@@ -572,16 +683,16 @@
         return self.query_cls(self).build_ast()._count() > 0
 
     def __nonzero__(self):
         return self.query_cls(self).build_ast()._count() > 0
 
     def __contains__(self, obj):
         if isinstance(obj, StructuredNode):
-            if hasattr(obj, "id"):
-                return self.query_cls(self).build_ast()._contains(int(obj.id))
+            if hasattr(obj, "element_id"):
+                return self.query_cls(self).build_ast()._contains(obj.element_id)
             raise ValueError("Unsaved node: " + repr(obj))
 
         raise ValueError("Expecting StructuredNode instance")
 
     def __getitem__(self, key):
         if isinstance(key, slice):
             if key.stop and key.start:
@@ -599,14 +710,21 @@
             self.limit = 1
 
             return self.query_cls(self).build_ast()._execute()[0]
 
         return None
 
 
+@dataclass
+class Optional:
+    """Simple relation qualifier."""
+
+    relation: str
+
+
 class NodeSet(BaseSet):
     """
     A class representing as set of nodes matching common query parameters
     """
 
     def __init__(self, source):
         self.source = source  # could be a Traverse object or a node class
@@ -625,14 +743,16 @@
         self.filters = []
         self.q_filters = Q()
 
         # used by has()
         self.must_match = {}
         self.dont_match = {}
 
+        self.relations_to_fetch: list = []
+
     def _get(self, limit=None, lazy=False, **kwargs):
         self.filter(**kwargs)
         if limit:
             self.limit = limit
         return self.query_cls(self).build_ast()._execute(lazy)
 
     def get(self, lazy=False, **kwargs):
@@ -773,14 +893,26 @@
                 if isinstance(property_obj, AliasProperty):
                     prop = property_obj.aliased_to()
 
                 self._order_by.append(prop + (" DESC" if desc else ""))
 
         return self
 
+    def fetch_relations(self, *relation_names):
+        """Specify a set of relations to return."""
+        relations = []
+        for relation_name in relation_names:
+            if isinstance(relation_name, Optional):
+                item = {"path": relation_name.relation, "optional": True}
+            else:
+                item = {"path": relation_name}
+            relations.append(item)
+        self.relations_to_fetch = relations
+        return self
+
 
 class Traversal(BaseSet):
     """
     Models a traversal from a node to another.
 
     :param source: Starting of the traversal.
     :type source: A :class:`~neomodel.core.StructuredNode` subclass, an
@@ -814,17 +946,15 @@
         invalid_keys = set(definition) - {
             "direction",
             "model",
             "node_class",
             "relation_type",
         }
         if invalid_keys:
-            raise ValueError(
-                f"Unallowed keys in Traversal definition: {invalid_keys}"
-            )
+            raise ValueError(f"Prohibited keys in Traversal definition: {invalid_keys}")
 
         self.definition = definition
         self.target_class = definition["node_class"]
         self.name = name
         self.filters = []
 
     def match(self, **kwargs):
```

### Comparing `neomodel-5.0.1/neomodel/match_q.py` & `neomodel-5.1.0/neomodel/match_q.py`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.1/neomodel/properties.py` & `neomodel-5.1.0/neomodel/properties.py`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.1/neomodel/relationship_manager.py` & `neomodel-5.1.0/neomodel/relationship_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,23 +60,23 @@
     def __str__(self):
         direction = "either"
         if self.definition["direction"] == OUTGOING:
             direction = "a outgoing"
         elif self.definition["direction"] == INCOMING:
             direction = "a incoming"
 
-        return f"{self.description} in {direction} direction of type {self.definition['relation_type']} on node ({self.source.id}) of class '{self.source_class.__name__}'"
+        return f"{self.description} in {direction} direction of type {self.definition['relation_type']} on node ({self.source.element_id}) of class '{self.source_class.__name__}'"
 
     def _check_node(self, obj):
         """check for valid node i.e correct class and is saved"""
         if not issubclass(type(obj), self.definition["node_class"]):
             raise ValueError(
                 "Expected node of class " + self.definition["node_class"].__name__
             )
-        if not hasattr(obj, "id"):
+        if not hasattr(obj, "element_id"):
             raise ValueError("Can't perform operation on unsaved node " + repr(obj))
 
     @check_source
     def connect(self, node, properties=None):
         """
         Connect a node
 
@@ -116,19 +116,19 @@
             lhs="us",
             rhs="them",
             ident="r",
             relation_properties=rel_prop,
             **self.definition,
         )
         q = (
-            "MATCH (them), (us) WHERE id(them)=$them and id(us)=$self "
+            f"MATCH (them), (us) WHERE {db.get_id_method()}(them)=$them and {db.get_id_method()}(us)=$self "
             "MERGE" + new_rel
         )
 
-        params["them"] = node.id
+        params["them"] = node.element_id
 
         if not rel_model:
             self.source.cypher(q, params)
             return True
 
         rel_ = self.source.cypher(q + " RETURN r", params)[0][0][0]
         rel_instance = self._set_start_end_cls(rel_model.inflate(rel_), node)
@@ -160,17 +160,17 @@
         :return: StructuredRel
         """
         self._check_node(node)
         my_rel = _rel_helper(lhs="us", rhs="them", ident="r", **self.definition)
         q = (
             "MATCH "
             + my_rel
-            + " WHERE id(them)=$them and id(us)=$self RETURN r LIMIT 1"
+            + f" WHERE {db.get_id_method()}(them)=$them and {db.get_id_method()}(us)=$self RETURN r LIMIT 1"
         )
-        rels = self.source.cypher(q, {"them": node.id})[0]
+        rels = self.source.cypher(q, {"them": node.element_id})[0]
         if not rels:
             return
 
         rel_model = self.definition.get("model") or StructuredRel
 
         return self._set_start_end_cls(rel_model.inflate(rels[0][0]), node)
 
@@ -181,16 +181,16 @@
 
         :param node:
         :return: [StructuredRel]
         """
         self._check_node(node)
 
         my_rel = _rel_helper(lhs="us", rhs="them", ident="r", **self.definition)
-        q = "MATCH " + my_rel + " WHERE id(them)=$them and id(us)=$self RETURN r "
-        rels = self.source.cypher(q, {"them": node.id})[0]
+        q = f"MATCH {my_rel} WHERE {db.get_id_method()}(them)=$them and {db.get_id_method()}(us)=$self RETURN r "
+        rels = self.source.cypher(q, {"them": node.element_id})[0]
         if not rels:
             return []
 
         rel_model = self.definition.get("model") or StructuredRel
         return [
             self._set_start_end_cls(rel_model.inflate(rel[0]), node) for rel in rels
         ]
@@ -214,71 +214,73 @@
         :param old_node:
         :param new_node:
         :return: None
         """
 
         self._check_node(old_node)
         self._check_node(new_node)
-        if old_node.id == new_node.id:
+        if old_node.element_id == new_node.element_id:
             return
         old_rel = _rel_helper(lhs="us", rhs="old", ident="r", **self.definition)
 
         # get list of properties on the existing rel
         result, _ = self.source.cypher(
-            "MATCH (us), (old) WHERE id(us)=$self and id(old)=$old "
-            "MATCH " + old_rel + " RETURN r",
-            {"old": old_node.id},
+            f"""
+                MATCH (us), (old) WHERE {db.get_id_method()}(us)=$self and {db.get_id_method()}(old)=$old
+                MATCH {old_rel} RETURN r
+            """,
+            {"old": old_node.element_id},
         )
         if result:
             node_properties = _get_node_properties(result[0][0])
             existing_properties = node_properties.keys()
         else:
             raise NotConnected("reconnect", self.source, old_node)
 
         # remove old relationship and create new one
         new_rel = _rel_merge_helper(lhs="us", rhs="new", ident="r2", **self.definition)
         q = (
             "MATCH (us), (old), (new) "
-            "WHERE id(us)=$self and id(old)=$old and id(new)=$new "
+            f"WHERE {db.get_id_method()}(us)=$self and {db.get_id_method()}(old)=$old and {db.get_id_method()}(new)=$new "
             "MATCH " + old_rel
         )
         q += " MERGE" + new_rel
 
         # copy over properties if we have
         for p in existing_properties:
             q += "".join([f" SET r2.{prop} = r.{prop}" for prop in existing_properties])
         q += " WITH r DELETE r"
 
-        self.source.cypher(q, {"old": old_node.id, "new": new_node.id})
+        self.source.cypher(q, {"old": old_node.element_id, "new": new_node.element_id})
 
     @check_source
     def disconnect(self, node):
         """
         Disconnect a node
 
         :param node:
         :return:
         """
         rel = _rel_helper(lhs="a", rhs="b", ident="r", **self.definition)
-        q = (
-            "MATCH (a), (b) WHERE id(a)=$self and id(b)=$them "
-            "MATCH " + rel + " DELETE r"
-        )
-        self.source.cypher(q, {"them": node.id})
+        q = f"""
+                MATCH (a), (b) WHERE {db.get_id_method()}(a)=$self and {db.get_id_method()}(b)=$them
+                MATCH {rel} DELETE r
+            """
+        self.source.cypher(q, {"them": node.element_id})
 
     @check_source
     def disconnect_all(self):
         """
         Disconnect all nodes
 
         :return:
         """
         rhs = "b:" + self.definition["node_class"].__label__
         rel = _rel_helper(lhs="a", rhs=rhs, ident="r", **self.definition)
-        q = "MATCH (a) WHERE id(a)=$self MATCH " + rel + " DELETE r"
+        q = f"MATCH (a) WHERE {db.get_id_method()}(a)=$self MATCH " + rel + " DELETE r"
         self.source.cypher(q)
 
     @check_source
     def _new_traversal(self):
         return Traversal(self.source, self.name, self.definition)
 
     # The methods below simply proxy the match engine.
```

### Comparing `neomodel-5.0.1/neomodel/util.py` & `neomodel-5.1.0/neomodel/util.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import logging
 import os
 import sys
 import time
 import warnings
 from threading import local
+from typing import Optional, Sequence
 from urllib.parse import quote, unquote, urlparse
 
 from neo4j import DEFAULT_DATABASE, GraphDatabase, basic_auth
+from neo4j.api import Bookmarks
 from neo4j.exceptions import ClientError, SessionExpired
 from neo4j.graph import Node, Relationship
 
 from neomodel import config, core
 from neomodel.exceptions import (
     ConstraintValidationFailed,
     NodeClassNotDefined,
@@ -33,66 +35,48 @@
         if not _db.url:
             _db.set_connection(config.DATABASE_URL)
         return func(self, *args, **kwargs)
 
     return wrapper
 
 
-def change_neo4j_password(db, new_password):
-    db.cypher_query("CALL dbms.changePassword($password)", {"password": new_password})
+def change_neo4j_password(db, user, new_password):
+    db.cypher_query(f"ALTER USER {user} SET PASSWORD '{new_password}'")
 
 
 def clear_neo4j_database(db, clear_constraints=False, clear_indexes=False):
-    db.cypher_query("MATCH (a) DETACH DELETE a")
+    db.cypher_query(
+        """
+        MATCH (a)
+        CALL { WITH a DETACH DELETE a }
+        IN TRANSACTIONS OF 5000 rows
+    """
+    )
     if clear_constraints:
         core.drop_constraints()
     if clear_indexes:
         core.drop_indexes()
 
 
-# pylint:disable=too-few-public-methods
-class NodeClassRegistry:
+class Database(local):
     """
-    A singleton class via which all instances share the same Node Class Registry.
+    A singleton object via which all operations from neomodel to the Neo4j backend are handled with.
     """
 
-    # Maintains a lookup directory that is used by cypher_query
-    # to infer which class to instantiate by examining the labels of the
-    # node in the resultset.
-    # _NODE_CLASS_REGISTRY is populated automatically by the constructor
-    # of the NodeMeta type.
     _NODE_CLASS_REGISTRY = {}
 
     def __init__(self):
-        self.__dict__["_NODE_CLASS_REGISTRY"] = self._NODE_CLASS_REGISTRY
-
-    def __str__(self):
-        ncr_items = list(
-            map(
-                lambda x: f"{','.join(x[0])} --> {x[1]}",
-                self._NODE_CLASS_REGISTRY.items(),
-            )
-        )
-        return "\n".join(ncr_items)
-
-
-class Database(local, NodeClassRegistry):
-    """
-    A singleton object via which all operations from neomodel to the Neo4j backend are handled with.
-    """
-
-    def __init__(self):
-        """ """
         self._active_transaction = None
         self.url = None
         self.driver = None
         self._session = None
         self._pid = None
         self._database_name = DEFAULT_DATABASE
         self.protocol_version = None
+        self.database_version = None
 
     def set_connection(self, url):
         """
         Sets the connection URL to the address a Neo4j server is set up at
         """
         p_start = url.replace(":", "", 1).find(":") + 2
         p_end = url.rfind("@")
@@ -130,24 +114,29 @@
             "max_transaction_retry_time": config.MAX_TRANSACTION_RETRY_TIME,
             "resolver": config.RESOLVER,
             "user_agent": config.USER_AGENT,
         }
 
         if "+s" not in parsed_url.scheme:
             options["encrypted"] = config.ENCRYPTED
-            options["trust"] = config.TRUST
+            options["trusted_certificates"] = config.TRUSTED_CERTIFICATES
 
         self.driver = GraphDatabase.driver(
             parsed_url.scheme + "://" + hostname, **options
         )
         self.url = url
         self._pid = os.getpid()
         self._active_transaction = None
         self._database_name = DEFAULT_DATABASE if database_name == "" else database_name
 
+        results = self.cypher_query(
+            "CALL dbms.components() yield versions return versions[0]"
+        )
+        self.database_version = results[0][0][0]
+
     @property
     def transaction(self):
         """
         Returns the current transaction object
         """
         return TransactionProxy(self)
 
@@ -158,54 +147,61 @@
     @property
     def read_transaction(self):
         return TransactionProxy(self, access_mode="READ")
 
     @ensure_connection
     def begin(self, access_mode=None, **parameters):
         """
-        Begins a new transaction, raises SystemError exception if a transaction is in progress
+        Begins a new transaction. Raises SystemError if a transaction is already active.
         """
-        if self._active_transaction:
+        if (
+            hasattr(self, "_active_transaction")
+            and self._active_transaction is not None
+        ):
             raise SystemError("Transaction in progress")
         self._session = self.driver.session(
             default_access_mode=access_mode,
             database=self._database_name,
             **parameters,
         )
         self._active_transaction = self._session.begin_transaction()
 
     @ensure_connection
     def commit(self):
         """
-        Commits the current transaction
+        Commits the current transaction and closes its session
 
-        :return: last_bookmark
+        :return: last_bookmarks
         """
         try:
             self._active_transaction.commit()
-            last_bookmark = self._session.last_bookmark()
+            last_bookmarks = self._session.last_bookmarks()
         finally:
             # In case when something went wrong during
             # committing changes to the database
             # we have to close an active transaction and session.
+            self._active_transaction.close()
+            self._session.close()
             self._active_transaction = None
             self._session = None
 
-        return last_bookmark
+        return last_bookmarks
 
     @ensure_connection
     def rollback(self):
         """
-        Rolls back the current transaction
+        Rolls back the current transaction and closes its session
         """
         try:
             self._active_transaction.rollback()
         finally:
             # In case when something went wrong during changes rollback,
             # we have to close an active transaction and session
+            self._active_transaction.close()
+            self._session.close()
             self._active_transaction = None
             self._session = None
 
     def _object_resolution(self, result_list):
         """
         Performs in place automatic object resolution on a set of results
         returned by cypher_query.
@@ -291,22 +287,47 @@
         :type: bool
         :param retry_on_session_expire: Whether or not to attempt the same query again if the transaction has expired
         :type: bool
         :param resolve_objects: Whether to attempt to resolve the returned nodes to data model objects automatically
         :type: bool
         """
 
-        if self._pid != os.getpid():
-            self.set_connection(self.url)
-
         if self._active_transaction:
-            session = self._active_transaction
+            # Use current session is a transaction is currently active
+            results, meta = self._run_cypher_query(
+                self._active_transaction,
+                query,
+                params,
+                handle_unique,
+                retry_on_session_expire,
+                resolve_objects,
+            )
         else:
-            session = self.driver.session(database=self._database_name)
+            # Otherwise create a new session in a with to dispose of it after it has been run
+            with self.driver.session(database=self._database_name) as session:
+                results, meta = self._run_cypher_query(
+                    session,
+                    query,
+                    params,
+                    handle_unique,
+                    retry_on_session_expire,
+                    resolve_objects,
+                )
 
+        return results, meta
+
+    def _run_cypher_query(
+        self,
+        session,
+        query,
+        params,
+        handle_unique,
+        retry_on_session_expire,
+        resolve_objects,
+    ):
         try:
             # Retrieve the data
             start = time.time()
             response = session.run(query, params)
             results, meta = [list(r.values()) for r in response], response.keys()
             end = time.time()
 
@@ -343,34 +364,62 @@
                 + "\nparams: "
                 + repr(params)
                 + f"\ntook: {tte:.2g}s\n"
             )
 
         return results, meta
 
+    def get_id_method(self) -> str:
+        if self.database_version.startswith("4"):
+            return "id"
+        else:
+            return "elementId"
+
+    def list_indexes(self, exclude_token_lookup=False) -> Sequence[dict]:
+        """Returns all indexes existing in the database
+
+        Arguments:
+            exclude_token_lookup[bool]: Exclude automatically create token lookup indexes
+
+        Returns:
+            Sequence[dict]: List of dictionaries, each entry being an index definition
+        """
+        indexes, meta_indexes = self.cypher_query("SHOW INDEXES")
+        indexes_as_dict = [dict(zip(meta_indexes, row)) for row in indexes]
+
+        if exclude_token_lookup:
+            indexes_as_dict = [
+                obj for obj in indexes_as_dict if obj["type"] != "LOOKUP"
+            ]
+
+        return indexes_as_dict
+
+    def list_constraints(self) -> Sequence[dict]:
+        """Returns all constraints existing in the database
+
+        Returns:
+            Sequence[dict]: List of dictionaries, each entry being a constraint definition
+        """
+        constraints, meta_constraints = self.cypher_query("SHOW CONSTRAINTS")
+        constraints_as_dict = [dict(zip(meta_constraints, row)) for row in constraints]
+
+        return constraints_as_dict
+
 
 class TransactionProxy:
-    bookmarks = None
+    bookmarks: Optional[Bookmarks] = None
 
     def __init__(self, db, access_mode=None):
         self.db = db
         self.access_mode = access_mode
 
     @ensure_connection
     def __enter__(self):
-        if self.bookmarks is None:
-            self.db.begin(access_mode=self.access_mode)
-        else:
-            bookmarks = (
-                (self.bookmarks,)
-                if isinstance(self.bookmarks, (str, bytes))
-                else tuple(self.bookmarks)
-            )
-            self.db.begin(access_mode=self.access_mode, bookmarks=bookmarks)
-            self.bookmarks = None
+        self.db.begin(access_mode=self.access_mode, bookmarks=self.bookmarks)
+        self.bookmarks = None
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         if exc_value:
             self.db.rollback()
 
         if exc_type is ClientError:
```

### Comparing `neomodel-5.0.1/neomodel.egg-info/PKG-INFO` & `neomodel-5.1.0/neomodel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neomodel
-Version: 5.0.1
+Version: 5.1.0
 Summary: An object mapper for the neo4j graph database.
 Author-email: Robin Edwards <robin.ge@gmail.com>
 Maintainer: Cristina Escalante
 Maintainer-email: Athanasios Anastasiou <athanastasiou@gmail.com>, Marius Conjeaud <marius.conjeaud@outlook.com>
 License: MIT
 Project-URL: documentation, https://neomodel.readthedocs.io/en/latest/
 Project-URL: repository, http://github.com/neo4j-contrib/neomodel
```

### Comparing `neomodel-5.0.1/neomodel.egg-info/SOURCES.txt` & `neomodel-5.1.0/neomodel.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 .env
 .gitignore
 .pre-commit-config.yaml
+.readthedocs.yaml
 AUTHORS.txt
 Changelog
 LICENSE
 README.rst
 dev
 docker-compose.yml
 pyproject.toml
 requirements.txt
-tests-with-docker-compose.sh
 .github/dependabot.yml
 .github/workflows/codeql-analysis.yml
 .github/workflows/integration-tests.yml
 .github/workflows/python-publish.yml
 doc/Makefile
 doc/make.bat
+doc/requirements.txt
 doc/source/batch.rst
 doc/source/conf.py
 doc/source/configuration.rst
 doc/source/cypher.rst
 doc/source/extending.rst
 doc/source/getting_started.rst
 doc/source/hooks.rst
@@ -36,14 +37,17 @@
 doc/source/_themes/alabaster/_version.py
 doc/source/_themes/alabaster/about.html
 doc/source/_themes/alabaster/layout.html
 doc/source/_themes/alabaster/navigation.html
 doc/source/_themes/alabaster/support.py
 doc/source/_themes/alabaster/theme.conf
 doc/source/_themes/alabaster/static/alabaster.css_t
+docker-scripts/docker-neo4j.sh
+docker-scripts/readme.md
+docker-scripts/tests-with-docker-compose.sh
 neomodel/__init__.py
 neomodel/cardinality.py
 neomodel/config.py
 neomodel/core.py
 neomodel/exceptions.py
 neomodel/hooks.py
 neomodel/match.py
@@ -57,38 +61,39 @@
 neomodel.egg-info/dependency_links.txt
 neomodel.egg-info/entry_points.txt
 neomodel.egg-info/requires.txt
 neomodel.egg-info/top_level.txt
 neomodel/contrib/__init__.py
 neomodel/contrib/semi_structured.py
 neomodel/contrib/spatial_properties.py
-scripts/docker-neo4j.sh
-scripts/neomodel_install_labels.py
-scripts/neomodel_remove_labels.py
+neomodel/scripts/__init__.py
+neomodel/scripts/neomodel_install_labels.py
+neomodel/scripts/neomodel_remove_labels.py
 test/__init__.py
 test/conftest.py
 test/test_alias.py
 test/test_batch.py
 test/test_cardinality.py
 test/test_connection.py
 test/test_cypher.py
+test/test_database_management.py
 test/test_exceptions.py
 test/test_hooks.py
 test/test_indexing.py
 test/test_issue112.py
 test/test_issue283.py
 test/test_issue600.py
 test/test_label_drop.py
 test/test_label_install.py
 test/test_match_api.py
+test/test_migration_neo4j_5.py
 test/test_models.py
 test/test_multiprocessing.py
 test/test_properties.py
 test/test_relationship_models.py
 test/test_relationships.py
 test/test_relative_relationships.py
 test/test_transactions.py
-test/utils.py
 test/test_contrib/__init__.py
 test/test_contrib/test_semi_structured.py
 test/test_contrib/test_spatial_datatypes.py
 test/test_contrib/test_spatial_properties.py
```

### Comparing `neomodel-5.0.1/pyproject.toml` & `neomodel-5.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -29,34 +29,34 @@
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python',
     'Topic :: Software Development :: Libraries :: Python Modules',
     "Programming Language :: Python :: 3",
     "Topic :: Database",
 ]
 dependencies = [
-    "neo4j-driver==4.4.10",
+    "neo4j==5.10.0",
     "pytz>=2021.1",
     "neobolt==1.7.17",
     "six==1.16.0",
 ]
-version='5.0.1'
+version='5.1.0'
 
 [project.urls]
 documentation = "https://neomodel.readthedocs.io/en/latest/"
 repository = "http://github.com/neo4j-contrib/neomodel"
 changelog = "https://github.com/neo4j-contrib/neomodel/releases"
 
 [project.optional-dependencies]
 dev = [
     "pytest>=7.1",
     "pytest-cov>=4.0",
     "pre-commit",
     "black",
     "isort",
-    "Shapely>=1.8.1,<1.9"
+    "Shapely>=2.0.0"
 ]
 
 [tool.pytest.ini_options]
 addopts = "--resetdb"
 testpaths = "test"
 
 [tool.isort]
@@ -70,9 +70,9 @@
 good-names = 'i,j,k,ex,_,e,fn,x,y,z,id,db,q'
 
 [tool.pylint.'DESIGN']
 max-attributes = 10
 max-args = 8
 
 [project.scripts]
-neomodel_install_labels = "scripts.neomodel_install_labels:main"
-neomodel_remove_labels = "scripts.neomodel_remove_labels:main"
+neomodel_install_labels = "neomodel.scripts.neomodel_install_labels:main"
+neomodel_remove_labels = "neomodel.scripts.neomodel_remove_labels:main"
```

### Comparing `neomodel-5.0.1/scripts/neomodel_install_labels.py` & `neomodel-5.1.0/neomodel/scripts/neomodel_install_labels.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from __future__ import print_function
 
 import sys
 from argparse import ArgumentParser
 from importlib import import_module
 from os import environ, path
 
-from neomodel import db, install_all_labels
+from .. import db, install_all_labels
 
 
 def load_python_module_or_file(name):
     # Is a file
     if name.lower().endswith(".py"):
         basedir = path.dirname(path.abspath(name))
         # Add base directory to pythonpath
```

### Comparing `neomodel-5.0.1/scripts/neomodel_remove_labels.py` & `neomodel-5.1.0/neomodel/scripts/neomodel_remove_labels.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 from __future__ import print_function
 
 from argparse import ArgumentParser
 from os import environ
 
-from neomodel import db, remove_all_labels
+from .. import db, remove_all_labels
 
 
 def main():
     parser = ArgumentParser(
         description="""
         Drop all indexes and constraints on labels from schema in Neo4j database.
```

### Comparing `neomodel-5.0.1/test/conftest.py` & `neomodel-5.1.0/test/conftest.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,14 +21,15 @@
         "--resetdb",
         action="store_true",
         help="Ensures that the database is clear prior to running tests for neomodel",
         default=False,
     )
 
 
+@pytest.hookimpl
 def pytest_collection_modifyitems(items):
     connect_to_aura_items = []
     normal_items = []
 
     # Separate all tests into two groups: those with "connect_to_aura" in their name, and all others
     for item in items:
         if "connect_to_aura" in item.name:
@@ -42,14 +43,15 @@
     # Add all connect_to_aura tests to the end of the list
     new_order.extend(connect_to_aura_items)
 
     # Replace the original items list with the new order
     items[:] = new_order
 
 
+@pytest.hookimpl
 def pytest_sessionstart(session):
     """
     Provides initial connection to the database and sets up the rest of the test suite
 
     :param session: The session object. Please see <https://docs.pytest.org/en/latest/reference.html#_pytest.hookspec.pytest_sessionstart>`_
     :type Session object: For more information please see <https://docs.pytest.org/en/latest/reference.html#session>`_
     """
@@ -57,55 +59,24 @@
     warnings.simplefilter("default")
 
     config.DATABASE_URL = os.environ.get(
         "NEO4J_BOLT_URL", "bolt://neo4j:foobarbaz@localhost:7687"
     )
     config.AUTO_INSTALL_LABELS = True
 
-    try:
-        # Clear the database if required
-        database_is_populated, _ = db.cypher_query(
-            "MATCH (a) return count(a)>0 as database_is_populated"
+    # Clear the database if required
+    database_is_populated, _ = db.cypher_query(
+        "MATCH (a) return count(a)>0 as database_is_populated"
+    )
+    if database_is_populated[0][0] and not session.config.getoption("resetdb"):
+        raise SystemError(
+            "Please note: The database seems to be populated.\n\tEither delete all nodes and edges manually, or set the --resetdb parameter when calling pytest\n\n\tpytest --resetdb."
         )
-        if database_is_populated[0][0] and not session.config.getoption("resetdb"):
-            raise SystemError(
-                "Please note: The database seems to be populated.\n\tEither delete all nodes and edges manually, or set the --resetdb parameter when calling pytest\n\n\tpytest --resetdb."
-            )
-        else:
-            clear_neo4j_database(db, clear_constraints=True, clear_indexes=True)
-    except (CypherError, ClientError) as ce:
-        # Handle instance without password being changed
-        if (
-            "The credentials you provided were valid, but must be changed before you can use this instance"
-            in str(ce)
-        ):
-            warnings.warn(
-                "New database with no password set, setting password to 'test'"
-            )
-            try:
-                change_neo4j_password(db, "test")
-                # Ensures that multiprocessing tests can use the new password
-                config.DATABASE_URL = "bolt://neo4j:test@localhost:7687"
-                db.set_connection("bolt://neo4j:test@localhost:7687")
-                warnings.warn(
-                    "Please 'export NEO4J_BOLT_URL=bolt://neo4j:test@localhost:7687' for subsequent test runs"
-                )
-            except (CypherError, ClientError) as e:
-                if (
-                    "The credentials you provided were valid, but must be changed before you can use this instance"
-                    in str(e)
-                ):
-                    warnings.warn(
-                        "You appear to be running on version 4.0+ of Neo4j, without having changed the password."
-                        "Please manually log in, change your password, then update the config.DATABASE_URL call at line 32 in this file"
-                    )
-                else:
-                    raise e
-        else:
-            raise ce
+    else:
+        clear_neo4j_database(db, clear_constraints=True, clear_indexes=True)
 
 
 def version_to_dec(a_version_string):
     """
     Converts a version string to a number to allow for quick checks on the versions of specific components.
 
     :param a_version_string: The version string under test (e.g. '3.4.0')
```

### Comparing `neomodel-5.0.1/test/test_alias.py` & `neomodel-5.1.0/test/test_alias.py`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.1/test/test_batch.py` & `neomodel-5.1.0/test/test_batch.py`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.1/test/test_cardinality.py` & `neomodel-5.1.0/test/test_cardinality.py`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.1/test/test_contrib/test_semi_structured.py` & `neomodel-5.1.0/test/test_contrib/test_semi_structured.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,14 +7,19 @@
     age = IntegerProperty(index=True)
 
 
 class Dummy(SemiStructuredNode):
     pass
 
 
+def test_to_save_to_model_with_required_only():
+    u = UserProf(email="dummy@test.com")
+    assert u.save()
+
+
 def test_save_to_model_with_extras():
     u = UserProf(email="jim@test.com", age=3, bar=99)
     u.foo = True
     assert u.save()
     u = UserProf.nodes.get(age=3)
     assert u.foo is True
     assert u.bar == 99
```

### Comparing `neomodel-5.0.1/test/test_contrib/test_spatial_datatypes.py` & `neomodel-5.1.0/test/test_contrib/test_spatial_datatypes.py`

 * *Files 10% similar despite different names*

```diff
@@ -258,24 +258,21 @@
     )
 
     # Absurd CRS
     with pytest.raises(ValueError, match=r"Invalid CRS\(blue_hotel\)"):
         _ = neomodel.contrib.spatial_properties.NeomodelPoint((0, 0), crs="blue_hotel")
 
     # Absurd coord dimensionality
-    with pytest.raises(
-        ValueError,
-        match="Invalid vector dimensions. Expected 2 or 3, received 7",
-    ):
+    with pytest.raises(ValueError,):
         _ = neomodel.contrib.spatial_properties.NeomodelPoint(
             (0, 0, 0, 0, 0, 0, 0), crs="cartesian"
         )
 
     # Absurd datatype passed to copy constructor
-    with pytest.raises(TypeError, match="Invalid object passed to copy constructor"):
+    with pytest.raises(TypeError,):
         _ = neomodel.contrib.spatial_properties.NeomodelPoint(
             "it don't mean a thing if it ain't got that swing",
             crs="cartesian",
         )
 
     # Trying to instantiate a point with any of BOTH x,y,z or longitude, latitude, height
     with pytest.raises(ValueError, match="Invalid instantiation via arguments"):
@@ -289,26 +286,35 @@
         )
 
     # Trying to instantiate a point with absolutely NO parameters
     with pytest.raises(ValueError, match="Invalid instantiation via no arguments"):
         _ = neomodel.contrib.spatial_properties.NeomodelPoint()
 
 
-def test_property_accessors_depending_on_crs():
+def test_property_accessors_depending_on_crs_shapely_lt_2():
     """
     Tests that points are accessed via their respective accessors.
 
     :return:
     """
 
     # Neo4j versions lower than 3.4.0 do not support Point. In that case, skip the test.
     check_and_skip_neo4j_least_version(
         340, "This version does not support spatial data types."
     )
 
+    # Check the version of Shapely installed to run the appropriate tests:
+    try:
+        from shapely import __version__
+    except ImportError:
+        pytest.skip("Shapely not installed")
+
+    if int("".join(__version__.split(".")[0:3])) >= 200:
+        pytest.skip("Shapely 2 is installed, skipping earlier version test")
+
     # Geometrical points only have x,y,z coordinates
     new_point = neomodel.contrib.spatial_properties.NeomodelPoint(
         (0.0, 0.0, 0.0), crs="cartesian-3d"
     )
     with pytest.raises(AttributeError, match=r'Invalid coordinate \("longitude"\)'):
         new_point.longitude
     with pytest.raises(AttributeError, match=r'Invalid coordinate \("latitude"\)'):
@@ -323,14 +329,57 @@
     with pytest.raises(AttributeError, match=r'Invalid coordinate \("x"\)'):
         new_point.x
     with pytest.raises(AttributeError, match=r'Invalid coordinate \("y"\)'):
         new_point.y
     with pytest.raises(AttributeError, match=r'Invalid coordinate \("z"\)'):
         new_point.z
 
+    
+def test_property_accessors_depending_on_crs_shapely_gte_2():
+    """
+    Tests that points are accessed via their respective accessors.
+
+    :return:
+    """
+
+    # Neo4j versions lower than 3.4.0 do not support Point. In that case, skip the test.
+    check_and_skip_neo4j_least_version(
+        340, "This version does not support spatial data types."
+    )
+
+    # Check the version of Shapely installed to run the appropriate tests:
+    try:
+        from shapely import __version__
+    except ImportError:
+        pytest.skip("Shapely not installed")
+
+    if int("".join(__version__.split(".")[0:3])) < 200:
+        pytest.skip("Shapely < 2.0.0 is installed, skipping test")
+    # Geometrical points only have x,y,z coordinates
+    new_point = neomodel.contrib.spatial_properties.NeomodelPoint(
+        (0.0, 0.0, 0.0), crs="cartesian-3d"
+    )
+    with pytest.raises(TypeError, match=r'Invalid coordinate \("longitude"\)'):
+        new_point.longitude
+    with pytest.raises(TypeError, match=r'Invalid coordinate \("latitude"\)'):
+        new_point.latitude
+    with pytest.raises(TypeError, match=r'Invalid coordinate \("height"\)'):
+        new_point.height
+
+    # Geographical points only have longitude, latitude, height coordinates
+    new_point = neomodel.contrib.spatial_properties.NeomodelPoint(
+        (0.0, 0.0, 0.0), crs="wgs-84-3d"
+    )
+    with pytest.raises(TypeError, match=r'Invalid coordinate \("x"\)'):
+        new_point.x
+    with pytest.raises(TypeError, match=r'Invalid coordinate \("y"\)'):
+        new_point.y
+    with pytest.raises(TypeError, match=r'Invalid coordinate \("z"\)'):
+        new_point.z
+
 
 def test_property_accessors():
     """
     Tests that points are accessed via their respective accessors and that these accessors return the right values.
 
     :return:
     """
```

### Comparing `neomodel-5.0.1/test/test_contrib/test_spatial_properties.py` & `neomodel-5.1.0/test/test_contrib/test_spatial_properties.py`

 * *Files 4% similar despite different names*

```diff
@@ -259,7 +259,24 @@
     ).save()
 
     a_property = TestStorageRetrievalProperty.nodes.get(
         location=neomodel.contrib.spatial_properties.NeomodelPoint((0, 0))
     )
 
     assert a_restaurant.description == a_property.description
+
+def test_equality_with_other_objects():
+    """
+    Performs equality tests and ensures tha ``NeomodelPoint`` can be compared with ShapelyPoint and NeomodelPoint only.
+    """
+    try:
+        import shapely.geometry
+        from shapely import __version__
+    except ImportError:
+        pytest.skip("Shapely module not present")
+
+    if int("".join(__version__.split(".")[0:3])) < 200:
+        pytest.skip(f"Shapely 2.0 not present (Current version is {__version__}")
+
+    assert neomodel.contrib.spatial_properties.NeomodelPoint((0,0)) == neomodel.contrib.spatial_properties.NeomodelPoint(x=0, y=0)
+    assert neomodel.contrib.spatial_properties.NeomodelPoint((0,0)) == shapely.geometry.Point((0,0))
+
```

### Comparing `neomodel-5.0.1/test/test_cypher.py` & `neomodel-5.1.0/test/test_cypher.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 from neo4j.exceptions import ClientError as CypherError
 
 from neomodel import StringProperty, StructuredNode
+from neomodel.core import db
 
 
 class User2(StructuredNode):
     email = StringProperty()
 
 
 def test_cypher():
     """
     test result format is backward compatible with earlier versions of neomodel
     """
 
     jim = User2(email="jim1@test.com").save()
-    data, meta = jim.cypher("MATCH (a) WHERE id(a)=$self RETURN a.email")
+    data, meta = jim.cypher(
+        f"MATCH (a) WHERE {db.get_id_method()}(a)=$self RETURN a.email"
+    )
     assert data[0][0] == "jim1@test.com"
     assert "a.email" in meta
 
     data, meta = jim.cypher(
-        "MATCH (a) WHERE id(a)=$self" " MATCH (a)<-[:USER2]-(b) " "RETURN a, b, 3"
+        f"""
+            MATCH (a) WHERE {db.get_id_method()}(a)=$self
+            MATCH (a)<-[:USER2]-(b)
+            RETURN a, b, 3
+        """
     )
     assert "a" in meta and "b" in meta
 
 
 def test_cypher_syntax_error():
     jim = User2(email="jim1@test.com").save()
     try:
-        jim.cypher("MATCH a WHERE id(a)={self} RETURN xx")
+        jim.cypher(f"MATCH a WHERE {db.get_id_method()}(a)={{self}} RETURN xx")
     except CypherError as e:
         assert hasattr(e, "message")
         assert hasattr(e, "code")
     else:
         assert False, "CypherError not raised."
```

### Comparing `neomodel-5.0.1/test/test_exceptions.py` & `neomodel-5.1.0/test/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.1/test/test_hooks.py` & `neomodel-5.1.0/test/test_hooks.py`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.1/test/test_indexing.py` & `neomodel-5.1.0/test/test_indexing.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,47 @@
 from pytest import raises
 
-from neomodel import IntegerProperty, StringProperty, StructuredNode, UniqueProperty
+from neomodel import (
+    IntegerProperty,
+    StringProperty,
+    StructuredNode,
+    UniqueProperty,
+    install_labels,
+)
+from neomodel.core import db
+from neomodel.exceptions import ConstraintValidationFailed
 
 
 class Human(StructuredNode):
     name = StringProperty(unique_index=True)
     age = IntegerProperty(index=True)
 
 
 def test_unique_error():
+    install_labels(Human)
     Human(name="j1m", age=13).save()
     try:
         Human(name="j1m", age=14).save()
     except UniqueProperty as e:
         assert str(e).find("j1m")
         assert str(e).find("name")
-        assert str(e).find("FooBarr")
     else:
         assert False, "UniqueProperty not raised."
 
 
+def test_existence_constraint_error():
+    db.cypher_query(
+        "CREATE CONSTRAINT test_existence_constraint FOR (n:Human) REQUIRE n.age IS NOT NULL"
+    )
+    with raises(ConstraintValidationFailed, match=r"must have the property"):
+        Human(name="Scarlett").save()
+
+    db.cypher_query("DROP CONSTRAINT test_existence_constraint")
+
+
 def test_optional_properties_dont_get_indexed():
     Human(name="99", age=99).save()
     h = Human.nodes.get(age=99)
     assert h
     assert h.name == "99"
 
     Human(name="98", age=98).save()
```

### Comparing `neomodel-5.0.1/test/test_issue283.py` & `neomodel-5.1.0/test/test_issue283.py`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.1/test/test_issue600.py` & `neomodel-5.1.0/test/test_issue600.py`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.1/test/test_label_drop.py` & `neomodel-5.1.0/test/test_label_drop.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,46 @@
-from test.utils import get_db_constraints_as_dict, get_db_indexes_as_dict
-
 from neo4j.exceptions import ClientError
 
 from neomodel import StringProperty, StructuredNode, config
 from neomodel.core import db, remove_all_labels
 
 config.AUTO_INSTALL_LABELS = True
 
 
 class ConstraintAndIndex(StructuredNode):
     name = StringProperty(unique_index=True)
     last_name = StringProperty(index=True)
 
 
 def test_drop_labels():
-    constraints_before = get_db_constraints_as_dict()
-    indexes_before = get_db_indexes_as_dict()
+    constraints_before = db.list_constraints()
+    indexes_before = db.list_indexes(exclude_token_lookup=True)
 
     assert len(constraints_before) > 0
     assert len(indexes_before) > 0
 
     remove_all_labels()
 
-    constraints = get_db_constraints_as_dict()
-    indexes = get_db_indexes_as_dict()
+    constraints = db.list_constraints()
+    indexes = db.list_indexes(exclude_token_lookup=True)
 
     assert len(constraints) == 0
-    # Ignore the automatically created LOOKUP indexes
-    assert len([index for index in indexes if index["labelsOrTypes"]]) == 0
+    assert len(indexes) == 0
 
     # Recreating all old constraints and indexes
     for constraint in constraints_before:
         constraint_type_clause = "UNIQUE"
         if constraint["type"] == "NODE_PROPERTY_EXISTENCE":
             constraint_type_clause = "NOT NULL"
         elif constraint["type"] == "NODE_KEY":
             constraint_type_clause = "NODE KEY"
 
         db.cypher_query(
             f'CREATE CONSTRAINT {constraint["name"]} FOR (n:{constraint["labelsOrTypes"][0]}) REQUIRE n.{constraint["properties"][0]} IS {constraint_type_clause}'
         )
     for index in indexes_before:
         try:
-            # Ignore the automatically created LOOKUP indexes
-            if index["labelsOrTypes"] is None or index["labelsOrTypes"] == []:
-                continue
             db.cypher_query(
                 f'CREATE INDEX {index["name"]} FOR (n:{index["labelsOrTypes"][0]}) ON (n.{index["properties"][0]})'
             )
         except ClientError:
             pass
```

### Comparing `neomodel-5.0.1/test/test_label_install.py` & `neomodel-5.1.0/test/test_label_install.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from test.utils import get_db_constraints_as_dict, get_db_indexes_as_dict
-
 from six import StringIO
 
 from neomodel import (
     RelationshipTo,
     StringProperty,
     StructuredNode,
     StructuredRel,
@@ -51,31 +49,31 @@
 config.AUTO_INSTALL_LABELS = True
 
 
 def test_labels_were_not_installed():
     bob = NodeWithConstraint(name="bob").save()
     bob2 = NodeWithConstraint(name="bob").save()
     bob3 = NodeWithConstraint(name="bob").save()
-    assert bob.id != bob3.id
+    assert bob.element_id != bob3.element_id
 
     for n in NodeWithConstraint.nodes.all():
         n.delete()
 
 
 def test_install_all():
     drop_constraints()
     install_labels(AbstractNode)
     # run install all labels
     install_all_labels()
 
-    indexes = get_db_indexes_as_dict()
+    indexes = db.list_indexes()
     index_names = [index["name"] for index in indexes]
     assert "index_INDEXED_REL_indexed_rel_prop" in index_names
 
-    constraints = get_db_constraints_as_dict()
+    constraints = db.list_constraints()
     constraint_names = [constraint["name"] for constraint in constraints]
     assert "constraint_unique_NodeWithConstraint_name" in constraint_names
     assert "constraint_unique_SomeNotUniqueNode_id" in constraint_names
 
     # remove constraint for above test
     _drop_constraints_for_label_and_property("NoConstraintsSetup", "name")
```

### Comparing `neomodel-5.0.1/test/test_match_api.py` & `neomodel-5.1.0/test/test_match_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,32 +10,38 @@
     RelationshipFrom,
     RelationshipTo,
     StringProperty,
     StructuredNode,
     StructuredRel,
 )
 from neomodel.exceptions import MultipleNodesReturned
-from neomodel.match import NodeSet, QueryBuilder, Traversal
+from neomodel.match import NodeSet, Optional, QueryBuilder, Traversal
 
 
 class SupplierRel(StructuredRel):
     since = DateTimeProperty(default=datetime.now)
     courier = StringProperty()
 
 
 class Supplier(StructuredNode):
     name = StringProperty()
     delivery_cost = IntegerProperty()
     coffees = RelationshipTo("Coffee", "COFFEE SUPPLIERS")
 
 
+class Species(StructuredNode):
+    name = StringProperty()
+    coffees = RelationshipFrom("Coffee", "COFFEE SPECIES", model=StructuredRel)
+
+
 class Coffee(StructuredNode):
     name = StringProperty(unique_index=True)
     price = IntegerProperty()
     suppliers = RelationshipFrom(Supplier, "COFFEE SUPPLIERS", model=SupplierRel)
+    species = RelationshipTo(Species, "COFFEE SPECIES", model=StructuredRel)
     id_ = IntegerProperty()
 
 
 def test_filter_exclude_via_labels():
     Coffee(name="Java", price=99).save()
 
     node_set = NodeSet(Coffee)
@@ -116,16 +122,17 @@
     nescafe.suppliers.connect(tesco)
     tesco.coffees.connect(Coffee(name="Decafe", price=2).save())
 
     ns = NodeSet(NodeSet(source=nescafe).suppliers.match()).coffees.match()
     qb = QueryBuilder(ns).build_ast()
 
     results = qb._execute()
-    assert len(results) == 1
+    assert len(results) == 2
     assert results[0].name == "Decafe"
+    assert results[1].name == "Nescafe plus"
 
 
 def test_count():
     Coffee(name="Nescafe Gold", price=99).save()
     count = QueryBuilder(NodeSet(source=Coffee)).build_ast()._count()
     assert count > 0
 
@@ -419,7 +426,49 @@
     nescafe_gold.suppliers.connect(lidl)
 
     lidl_supplier = (
         NodeSet(Coffee.nodes.filter(price=11).suppliers).filter(delivery_cost=3).all()
     )
 
     assert lidl in lidl_supplier
+
+
+def test_fetch_relations():
+    arabica = Species(name="Arabica").save()
+    robusta = Species(name="Robusta").save()
+    nescafe = Coffee(name="Nescafe 1000", price=99).save()
+    nescafe_gold = Coffee(name="Nescafe 1001", price=11).save()
+
+    tesco = Supplier(name="Sainsburys", delivery_cost=3).save()
+    nescafe.suppliers.connect(tesco)
+    nescafe_gold.suppliers.connect(tesco)
+    nescafe.species.connect(arabica)
+
+    result = (
+        Supplier.nodes.filter(name="Sainsburys")
+        .fetch_relations("coffees__species")
+        .all()
+    )
+    assert arabica in result[0]
+    assert robusta not in result[0]
+    assert tesco in result[0]
+    assert nescafe in result[0]
+    assert nescafe_gold not in result[0]
+
+    result = (
+        Species.nodes.filter(name="Robusta")
+        .fetch_relations(Optional("coffees__suppliers"))
+        .all()
+    )
+    assert result[0][0] is None
+
+    # len() should only consider Suppliers
+    count = len(
+        Supplier.nodes.filter(name="Sainsburys")
+        .fetch_relations("coffees__species")
+        .all()
+    )
+    assert count == 1
+
+    assert tesco in Supplier.nodes.fetch_relations("coffees__species").filter(
+        name="Sainsburys"
+    )
```

### Comparing `neomodel-5.0.1/test/test_models.py` & `neomodel-5.1.0/test/test_models.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from neomodel import (
     DateProperty,
     IntegerProperty,
     StringProperty,
     StructuredNode,
     install_labels,
 )
+from neomodel.core import db
 from neomodel.exceptions import RequiredProperty, UniqueProperty
 
 
 class User(StructuredNode):
     email = StringProperty(unique_index=True, required=True)
     age = IntegerProperty(index=True)
 
@@ -23,14 +24,18 @@
         return self.email
 
     @email_alias.setter  # noqa
     def email_alias(self, value):
         self.email = value
 
 
+class NodeWithoutProperty(StructuredNode):
+    pass
+
+
 def test_issue_233():
     class BaseIssue233(StructuredNode):
         __abstract_node__ = True
 
         def __getitem__(self, item):
             return self.__dict__[item]
 
@@ -91,19 +96,25 @@
     n = User.nodes.first_or_none(email="matt@nothere.com")
     assert n is None
 
 
 def test_save_to_model():
     u = User(email="jim@test.com", age=3)
     assert u.save()
-    assert u.id > 0
+    assert u.element_id != ""
     assert u.email == "jim@test.com"
     assert u.age == 3
 
 
+def test_save_node_without_properties():
+    n = NodeWithoutProperty()
+    assert n.save()
+    assert n.element_id != ""
+
+
 def test_unique():
     install_labels(User)
     User(email="jim1@test.com", age=3).save()
     with raises(UniqueProperty):
         User(email="jim1@test.com", age=3).save()
 
 
@@ -180,21 +191,24 @@
 
     assert c.age == 16
 
     c.refresh()
     assert c.age == 20
     assert c.my_custom_prop == "value"
 
-    c = Customer2.inflate(c.id)
+    c = Customer2.inflate(c.element_id)
     c.age = 30
     c.refresh()
 
     assert c.age == 20
 
-    c = Customer2.inflate(999)
+    if db.database_version.startswith("4"):
+        c = Customer2.inflate(999)
+    else:
+        c = Customer2.inflate("4:xxxxxx:999")
     with raises(Customer2.DoesNotExist):
         c.refresh()
 
 
 def test_setting_value_to_none():
     c = Customer2(email="alice@bob.com", age=42).save()
     assert c.age is not None
@@ -224,14 +238,38 @@
     assert Shopper.__label__ == "Shopper"
     assert jim.balance == 350
     assert len(jim.inherited_labels()) == 1
     assert len(jim.labels()) == 1
     assert jim.labels()[0] == "Shopper"
 
 
+def test_inherited_optional_labels():
+    class BaseOptional(StructuredNode):
+        __optional_labels__ = ["Alive"]
+        name = StringProperty(unique_index=True)
+
+    class ExtendedOptional(BaseOptional):
+        __optional_labels__ = ["RewardsMember"]
+        balance = IntegerProperty(index=True)
+
+        def credit_account(self, amount):
+            self.balance = self.balance + int(amount)
+            self.save()
+
+    henry = ExtendedOptional(name="henry", balance=300).save()
+    henry.credit_account(50)
+
+    assert ExtendedOptional.__label__ == "ExtendedOptional"
+    assert henry.balance == 350
+    assert len(henry.inherited_labels()) == 2
+    assert len(henry.labels()) == 2
+
+    assert set(henry.inherited_optional_labels()) == {"Alive", "RewardsMember"}
+
+
 def test_mixins():
     class UserMixin:
         name = StringProperty(unique_index=True)
         password = StringProperty()
 
     class CreditMixin:
         balance = IntegerProperty(index=True)
```

### Comparing `neomodel-5.0.1/test/test_properties.py` & `neomodel-5.1.0/test/test_properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -385,15 +385,15 @@
 
 def test_indexed_array():
     class IndexArray(StructuredNode):
         ai = ArrayProperty(unique_index=True)
 
     b = IndexArray(ai=[1, 2]).save()
     c = IndexArray.nodes.get(ai=[1, 2])
-    assert b.id == c.id
+    assert b.element_id == c.element_id
 
 
 def test_unique_index_prop_not_required():
     class ConstrainedTestNode(StructuredNode):
         required_property = StringProperty(required=True)
         unique_property = StringProperty(unique_index=True)
         unique_required_property = StringProperty(unique_index=True, required=True)
```

### Comparing `neomodel-5.0.1/test/test_relationship_models.py` & `neomodel-5.1.0/test/test_relationship_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -119,32 +119,32 @@
 def test_multiple_rels_exist_issue_223():
     # check a badger can dislike a stoat for multiple reasons
     phill = Badger(name="Phill").save()
     ian = Stoat(name="Stoat").save()
 
     rel_a = phill.hates.connect(ian, {"reason": "a"})
     rel_b = phill.hates.connect(ian, {"reason": "b"})
-    assert rel_a.id != rel_b.id
+    assert rel_a.element_id != rel_b.element_id
 
     ian_a = phill.hates.match(reason="a")[0]
     ian_b = phill.hates.match(reason="b")[0]
-    assert ian_a.id == ian_b.id
+    assert ian_a.element_id == ian_b.element_id
 
 
 def test_retrieve_all_rels():
     tom = Badger(name="tom").save()
     ian = Stoat(name="ian").save()
 
     rel_a = tom.hates.connect(ian, {"reason": "a"})
     rel_b = tom.hates.connect(ian, {"reason": "b"})
 
     rels = tom.hates.all_relationships(ian)
     assert len(rels) == 2
-    assert rels[0].id in [rel_a.id, rel_b.id]
-    assert rels[1].id in [rel_a.id, rel_b.id]
+    assert rels[0].element_id in [rel_a.element_id, rel_b.element_id]
+    assert rels[1].element_id in [rel_a.element_id, rel_b.element_id]
 
 
 def test_save_hook_on_rel_model():
     HOOKS_CALLED["pre_save"] = 0
     HOOKS_CALLED["post_save"] = 0
 
     paul = Badger(name="PaulB").save()
```

### Comparing `neomodel-5.0.1/test/test_relationships.py` & `neomodel-5.1.0/test/test_relationships.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     Relationship,
     RelationshipFrom,
     RelationshipTo,
     StringProperty,
     StructuredNode,
     StructuredRel,
 )
+from neomodel.core import db
 
 
 class PersonWithRels(StructuredNode):
     name = StringProperty(unique_index=True)
     age = IntegerProperty(index=True)
     is_from = RelationshipTo("Country", "IS_FROM")
     knows = Relationship("PersonWithRels", "KNOWS")
@@ -86,18 +87,18 @@
 
     rey.knows.connect(sakis)
     assert rey.knows.is_connected(sakis)
     assert sakis.knows.is_connected(rey)
     sakis.knows.connect(rey)
 
     result, _ = sakis.cypher(
-        """MATCH (us), (them)
-            WHERE id(us)=$self and id(them)=$them
+        f"""MATCH (us), (them)
+            WHERE {db.get_id_method()}(us)=$self and {db.get_id_method()}(them)=$them
             MATCH (us)-[r:KNOWS]-(them) RETURN COUNT(r)""",
-        {"them": rey.id},
+        {"them": rey.element_id},
     )
     assert int(result[0][0]) == 1
 
     rel = rey.knows.relationship(sakis)
     assert isinstance(rel, StructuredRel)
 
     rels = rey.knows.all_relationships(sakis)
```

### Comparing `neomodel-5.0.1/test/test_relative_relationships.py` & `neomodel-5.1.0/test/test_relative_relationships.py`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.1/test/test_transactions.py` & `neomodel-5.1.0/test/test_transactions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import pytest
+from neo4j.api import Bookmarks
+from neo4j.exceptions import ClientError, TransactionError
 from pytest import raises
 
 from neomodel import StringProperty, StructuredNode, UniqueProperty, db, install_labels
 
 
 class APerson(StructuredNode):
     name = StringProperty(unique_index=True)
@@ -67,14 +69,44 @@
     with db.transaction:
         APerson(name="Alice").save()
         APerson(name="Bob").save()
 
         assert len([p.name for p in APerson.nodes]) == 2
 
 
+def test_read_transaction():
+    APerson(name="Johnny").save()
+
+    with db.read_transaction:
+        people = APerson.nodes.all()
+        assert people
+
+    with pytest.raises(TransactionError):
+        with db.read_transaction:
+            with pytest.raises(ClientError) as e:
+                APerson(name="Gina").save()
+            assert e.value.code == "Neo.ClientError.Statement.AccessMode"
+
+
+def test_write_transaction():
+    with db.write_transaction:
+        APerson(name="Amelia").save()
+
+    amelia = APerson.nodes.get(name="Amelia")
+    assert amelia
+
+
+def double_transaction():
+    db.begin()
+    with pytest.raises(SystemError, match=r"Transaction in progress"):
+        db.begin()
+
+    db.rollback()
+
+
 def test_set_connection_works():
     assert APerson(name="New guy 1").save()
     from socket import gaierror
 
     old_url = db.url
     with raises(ValueError):
         db.set_connection("bolt://user:password@6.6.6.6.6.6.6.6:7687")
@@ -91,29 +123,29 @@
 
 
 def test_bookmark_transaction_decorator(skip_neo4j_before_330):
     for p in APerson.nodes:
         p.delete()
 
     # should work
-    result, bookmark = in_a_tx("Ruth", bookmarks=None)
+    result, bookmarks = in_a_tx("Ruth", bookmarks=None)
     assert result is None
-    assert isinstance(bookmark, str)
+    assert isinstance(bookmarks, Bookmarks)
 
     # should bail but raise correct error
     with raises(UniqueProperty):
         in_a_tx("Jane", "Ruth")
 
     assert "Jane" not in [p.name for p in APerson.nodes]
 
 
 def test_bookmark_transaction_as_a_context(skip_neo4j_before_330):
     with db.transaction as transaction:
         APerson(name="Tanya").save()
-    assert isinstance(transaction.last_bookmark, str)
+    assert isinstance(transaction.last_bookmark, Bookmarks)
 
     assert APerson.nodes.filter(name="Tanya")
 
     with raises(UniqueProperty):
         with db.transaction as transaction:
             APerson(name="Tanya").save()
     assert not hasattr(transaction, "last_bookmark")
@@ -133,38 +165,30 @@
 
 
 def test_bookmark_passed_in_to_context(skip_neo4j_before_330, spy_on_db_begin):
     transaction = db.transaction
     with transaction:
         pass
 
-    assert spy_on_db_begin[-1] == ((), {"access_mode": None})
+    assert spy_on_db_begin[-1] == ((), {"access_mode": None, "bookmarks": None})
     last_bookmark = transaction.last_bookmark
 
     transaction.bookmarks = last_bookmark
     with transaction:
         pass
     assert spy_on_db_begin[-1] == (
         (),
-        {"access_mode": None, "bookmarks": (last_bookmark,)},
-    )
-
-    transaction.bookmarks = [last_bookmark]
-    with transaction:
-        pass
-    assert spy_on_db_begin[-1] == (
-        (),
-        {"access_mode": None, "bookmarks": (last_bookmark,)},
+        {"access_mode": None, "bookmarks": last_bookmark},
     )
 
 
 def test_query_inside_bookmark_transaction(skip_neo4j_before_330):
     for p in APerson.nodes:
         p.delete()
 
     with db.transaction as transaction:
         APerson(name="Alice").save()
         APerson(name="Bob").save()
 
         assert len([p.name for p in APerson.nodes]) == 2
 
-    assert isinstance(transaction.last_bookmark, str)
+    assert isinstance(transaction.last_bookmark, Bookmarks)
```

### Comparing `neomodel-5.0.1/tests-with-docker-compose.sh` & `neomodel-5.1.0/docker-scripts/tests-with-docker-compose.sh`

 * *Files identical despite different names*

