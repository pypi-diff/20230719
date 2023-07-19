# Comparing `tmp/cre-0.4.0.tar.gz` & `tmp/cre-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cre-0.4.0.tar", last modified: Tue Jul 18 17:55:38 2023, max compression
+gzip compressed data, was "cre-0.4.1.tar", last modified: Tue Jul 18 18:12:36 2023, max compression
```

## Comparing `cre-0.4.0.tar` & `cre-0.4.1.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxr-x   0 danny     (1000) danny     (1000)        0 2023-07-18 17:55:38.298666 cre-0.4.0/
--rw-rw-r--   0 danny     (1000) danny     (1000)       61 2023-07-18 17:53:58.000000 cre-0.4.0/.gitignore
--rw-rw-r--   0 danny     (1000) danny     (1000)     1073 2023-07-18 16:48:38.000000 cre-0.4.0/LICENSE.txt
--rw-rw-r--   0 danny     (1000) danny     (1000)      695 2023-07-18 17:55:38.298666 cre-0.4.0/PKG-INFO
--rw-rw-r--   0 danny     (1000) danny     (1000)    11270 2023-02-21 03:43:23.000000 cre-0.4.0/README.md
-drwxrwxr-x   0 danny     (1000) danny     (1000)        0 2023-07-18 17:55:38.294666 cre-0.4.0/console/
--rw-rw-r--   0 danny     (1000) danny     (1000)      573 2022-06-12 05:16:49.000000 cre-0.4.0/console/cre_exec.py
-drwxrwxr-x   0 danny     (1000) danny     (1000)        0 2023-07-18 17:55:38.298666 cre-0.4.0/cre/
--rw-rw-r--   0 danny     (1000) danny     (1000)     1107 2023-02-21 20:06:54.000000 cre-0.4.0/cre/__init__.py
--rw-rw-r--   0 danny     (1000) danny     (1000)     2116 2023-02-27 02:33:38.000000 cre-0.4.0/cre/attr_filter.py
--rw-rw-r--   0 danny     (1000) danny     (1000)       34 2022-06-12 05:16:49.000000 cre-0.4.0/cre/caching.py
-drwxrwxr-x   0 danny     (1000) danny     (1000)        0 2023-07-18 17:55:38.298666 cre-0.4.0/cre/cfuncs/
--rw-rw-r--   0 danny     (1000) danny     (1000)      137 2022-06-12 05:16:49.000000 cre-0.4.0/cre/cfuncs/__init__.py
--rw-rw-r--   0 danny     (1000) danny     (1000)     2768 2022-09-06 21:55:51.000000 cre-0.4.0/cre/cfuncs/cre_cfuncs.c
--rw-rw-r--   0 danny     (1000) danny     (1000)     3603 2023-05-01 14:43:41.000000 cre-0.4.0/cre/change_event.py
--rw-rw-r--   0 danny     (1000) danny     (1000)    77543 2023-06-02 04:34:43.000000 cre-0.4.0/cre/conditions.py
--rw-rw-r--   0 danny     (1000) danny     (1000)    15471 2023-06-02 04:46:55.000000 cre-0.4.0/cre/context.py
--rw-rw-r--   0 danny     (1000) danny     (1000)     8289 2023-05-01 16:10:37.000000 cre-0.4.0/cre/core.py
--rw-rw-r--   0 danny     (1000) danny     (1000)     2621 2023-05-14 16:29:49.000000 cre-0.4.0/cre/default_funcs.py
--rw-rw-r--   0 danny     (1000) danny     (1000)    17363 2023-06-02 01:45:53.000000 cre-0.4.0/cre/dynamic_exec.py
--rw-rw-r--   0 danny     (1000) danny     (1000)    47344 2023-05-27 16:52:23.000000 cre-0.4.0/cre/fact.py
--rw-rw-r--   0 danny     (1000) danny     (1000)    16306 2023-02-21 03:58:09.000000 cre-0.4.0/cre/fact_intrinsics.py
--rw-rw-r--   0 danny     (1000) danny     (1000)    93320 2023-07-01 20:52:29.000000 cre-0.4.0/cre/func.py
--rw-rw-r--   0 danny     (1000) danny     (1000)      656 2023-05-08 03:39:17.000000 cre-0.4.0/cre/garbage3.py
--rw-rw-r--   0 danny     (1000) danny     (1000)     1088 2023-04-15 18:57:56.000000 cre-0.4.0/cre/garbage31.py
--rw-rw-r--   0 danny     (1000) danny     (1000)    80851 2023-06-01 22:01:56.000000 cre-0.4.0/cre/garbage_sc_stash.py
--rw-rw-r--   0 danny     (1000) danny     (1000)    80080 2023-06-01 22:09:06.000000 cre-0.4.0/cre/garbage_sc_stash2.py
--rw-rw-r--   0 danny     (1000) danny     (1000)     3850 2023-06-05 14:24:45.000000 cre-0.4.0/cre/gval.py
--rw-rw-r--   0 danny     (1000) danny     (1000)     2270 2023-05-11 22:41:34.000000 cre-0.4.0/cre/hashing.py
--rw-rw-r--   0 danny     (1000) danny     (1000)     8288 2022-06-12 05:16:49.000000 cre-0.4.0/cre/make_source.py
--rw-rw-r--   0 danny     (1000) danny     (1000)    81594 2023-06-05 04:30:24.000000 cre-0.4.0/cre/matching.py
--rw-rw-r--   0 danny     (1000) danny     (1000)    38451 2023-06-05 03:56:00.000000 cre-0.4.0/cre/memset.py
--rw-rw-r--   0 danny     (1000) danny     (1000)    20497 2023-05-25 18:45:58.000000 cre-0.4.0/cre/obj.py
--rw-rw-r--   0 danny     (1000) danny     (1000)     5440 2023-02-21 03:58:09.000000 cre-0.4.0/cre/rule.py
--rwxrwxr-x   0 danny     (1000) danny     (1000)      217 2022-06-12 05:16:49.000000 cre-0.4.0/cre/run_tests
--rw-rw-r--   0 danny     (1000) danny     (1000)    81185 2023-07-01 04:12:55.000000 cre-0.4.0/cre/sc_planner.py
--rw-rw-r--   0 danny     (1000) danny     (1000)     9511 2023-02-20 22:35:46.000000 cre-0.4.0/cre/structref.py
--rw-rw-r--   0 danny     (1000) danny     (1000)     4365 2023-06-30 10:50:15.000000 cre-0.4.0/cre/token.py
--rw-rw-r--   0 danny     (1000) danny     (1000)    12224 2023-04-28 20:21:41.000000 cre-0.4.0/cre/tuple_fact.py
--rw-rw-r--   0 danny     (1000) danny     (1000)    10483 2023-05-07 23:44:51.000000 cre-0.4.0/cre/type_conv.py
--rw-rw-r--   0 danny     (1000) danny     (1000)    47635 2023-05-08 00:32:29.000000 cre-0.4.0/cre/utils.py
--rw-rw-r--   0 danny     (1000) danny     (1000)    38375 2023-06-13 20:23:15.000000 cre-0.4.0/cre/var.py
--rw-rw-r--   0 danny     (1000) danny     (1000)     6072 2022-06-12 05:16:49.000000 cre-0.4.0/cre/vector.py
--rw-rw-r--   0 danny     (1000) danny     (1000)       22 2023-04-29 18:30:06.000000 cre-0.4.0/cre/version.py
-drwxrwxr-x   0 danny     (1000) danny     (1000)        0 2023-07-18 17:55:38.298666 cre-0.4.0/cre.egg-info/
--rw-rw-r--   0 danny     (1000) danny     (1000)      695 2023-07-18 17:55:38.000000 cre-0.4.0/cre.egg-info/PKG-INFO
--rw-rw-r--   0 danny     (1000) danny     (1000)     1348 2023-07-18 17:55:38.000000 cre-0.4.0/cre.egg-info/SOURCES.txt
--rw-rw-r--   0 danny     (1000) danny     (1000)        1 2023-07-18 17:55:38.000000 cre-0.4.0/cre.egg-info/dependency_links.txt
--rw-rw-r--   0 danny     (1000) danny     (1000)       46 2023-07-18 17:55:38.000000 cre-0.4.0/cre.egg-info/entry_points.txt
--rw-rw-r--   0 danny     (1000) danny     (1000)       55 2023-07-18 17:55:38.000000 cre-0.4.0/cre.egg-info/requires.txt
--rw-rw-r--   0 danny     (1000) danny     (1000)       27 2023-07-18 17:55:38.000000 cre-0.4.0/cre.egg-info/top_level.txt
-drwxrwxr-x   0 danny     (1000) danny     (1000)        0 2023-07-18 17:55:38.298666 cre-0.4.0/cre_caching/
--rw-rw-r--   0 danny     (1000) danny     (1000)       34 2022-06-12 05:16:49.000000 cre-0.4.0/cre_caching/__init__.py
--rw-rw-r--   0 danny     (1000) danny     (1000)     8199 2023-05-24 20:20:42.000000 cre-0.4.0/cre_caching/caching.py
-drwxrwxr-x   0 danny     (1000) danny     (1000)        0 2023-07-18 17:55:38.298666 cre-0.4.0/notes/
--rw-rw-r--   0 danny     (1000) danny     (1000)     3560 2022-06-12 05:16:49.000000 cre-0.4.0/notes/SeqGrammarInduction.txt
--rw-rw-r--   0 danny     (1000) danny     (1000)        1 2023-07-18 17:37:22.000000 cre-0.4.0/pyproject.toml
--rw-rw-r--   0 danny     (1000) danny     (1000)       24 2023-07-18 17:53:26.000000 cre-0.4.0/requirements.txt
--rw-rw-r--   0 danny     (1000) danny     (1000)       67 2023-07-18 17:55:38.298666 cre-0.4.0/setup.cfg
--rw-rw-r--   0 danny     (1000) danny     (1000)     3407 2023-07-18 17:50:45.000000 cre-0.4.0/setup.py
-drwxrwxr-x   0 danny     (1000) danny     (1000)        0 2023-07-18 17:55:38.298666 cre-0.4.0/tests/
--rw-rw-r--   0 danny     (1000) danny     (1000)    16694 2023-06-02 04:03:51.000000 cre-0.4.0/tests/test_conditions.py
--rw-rw-r--   0 danny     (1000) danny     (1000)    19089 2023-06-02 05:12:00.000000 cre-0.4.0/tests/test_cre_func.py
--rw-rw-r--   0 danny     (1000) danny     (1000)    28780 2023-02-21 03:58:22.000000 cre-0.4.0/tests/test_fact.py
--rw-rw-r--   0 danny     (1000) danny     (1000)     6378 2023-05-08 00:34:10.000000 cre-0.4.0/tests/test_feature_applier.py
--rw-rw-r--   0 danny     (1000) danny     (1000)     5101 2023-05-15 19:52:19.000000 cre-0.4.0/tests/test_flattener.py
--rw-rw-r--   0 danny     (1000) danny     (1000)     2466 2023-01-22 23:11:50.000000 cre-0.4.0/tests/test_incr_processor.py
--rw-rw-r--   0 danny     (1000) danny     (1000)     1326 2022-06-12 05:16:49.000000 cre-0.4.0/tests/test_make_source.py
--rw-rw-r--   0 danny     (1000) danny     (1000)    23167 2023-05-08 00:29:11.000000 cre-0.4.0/tests/test_matching.py
--rw-rw-r--   0 danny     (1000) danny     (1000)    19201 2023-05-08 03:49:51.000000 cre-0.4.0/tests/test_memset.py
--rw-rw-r--   0 danny     (1000) danny     (1000)    16939 2023-05-08 00:36:44.000000 cre-0.4.0/tests/test_processing_pipeline.py
--rw-rw-r--   0 danny     (1000) danny     (1000)    10230 2023-05-08 00:39:06.000000 cre-0.4.0/tests/test_relative_encoder.py
--rw-rw-r--   0 danny     (1000) danny     (1000)      714 2023-02-16 07:15:18.000000 cre-0.4.0/tests/test_rule.py
--rw-rw-r--   0 danny     (1000) danny     (1000)    32453 2023-07-01 04:32:30.000000 cre-0.4.0/tests/test_sc_planner.py
--rw-rw-r--   0 danny     (1000) danny     (1000)     6565 2023-02-21 03:58:22.000000 cre-0.4.0/tests/test_tuple_fact.py
--rw-rw-r--   0 danny     (1000) danny     (1000)     3440 2023-02-20 06:20:35.000000 cre-0.4.0/tests/test_type_conv.py
--rw-rw-r--   0 danny     (1000) danny     (1000)     7282 2023-02-20 05:54:27.000000 cre-0.4.0/tests/test_utils.py
--rw-rw-r--   0 danny     (1000) danny     (1000)     4416 2023-04-29 17:16:43.000000 cre-0.4.0/tests/test_vectorizer.py
+drwxrwxr-x   0 danny     (1000) danny     (1000)        0 2023-07-18 18:12:36.174164 cre-0.4.1/
+-rw-rw-r--   0 danny     (1000) danny     (1000)       61 2023-07-18 17:53:58.000000 cre-0.4.1/.gitignore
+-rw-rw-r--   0 danny     (1000) danny     (1000)     1073 2023-07-18 16:48:38.000000 cre-0.4.1/LICENSE.txt
+-rw-rw-r--   0 danny     (1000) danny     (1000)      695 2023-07-18 18:12:36.174164 cre-0.4.1/PKG-INFO
+-rw-rw-r--   0 danny     (1000) danny     (1000)    11270 2023-02-21 03:43:23.000000 cre-0.4.1/README.md
+drwxrwxr-x   0 danny     (1000) danny     (1000)        0 2023-07-18 18:12:36.170164 cre-0.4.1/console/
+-rw-rw-r--   0 danny     (1000) danny     (1000)      573 2022-06-12 05:16:49.000000 cre-0.4.1/console/cre_exec.py
+drwxrwxr-x   0 danny     (1000) danny     (1000)        0 2023-07-18 18:12:36.174164 cre-0.4.1/cre/
+-rw-rw-r--   0 danny     (1000) danny     (1000)     1107 2023-02-21 20:06:54.000000 cre-0.4.1/cre/__init__.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)     2116 2023-02-27 02:33:38.000000 cre-0.4.1/cre/attr_filter.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)       34 2022-06-12 05:16:49.000000 cre-0.4.1/cre/caching.py
+drwxrwxr-x   0 danny     (1000) danny     (1000)        0 2023-07-18 18:12:36.174164 cre-0.4.1/cre/cfuncs/
+-rw-rw-r--   0 danny     (1000) danny     (1000)      137 2022-06-12 05:16:49.000000 cre-0.4.1/cre/cfuncs/__init__.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)     2768 2022-09-06 21:55:51.000000 cre-0.4.1/cre/cfuncs/cre_cfuncs.c
+-rw-rw-r--   0 danny     (1000) danny     (1000)     3603 2023-05-01 14:43:41.000000 cre-0.4.1/cre/change_event.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)    77543 2023-06-02 04:34:43.000000 cre-0.4.1/cre/conditions.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)    15471 2023-06-02 04:46:55.000000 cre-0.4.1/cre/context.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)     8289 2023-05-01 16:10:37.000000 cre-0.4.1/cre/core.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)     2621 2023-05-14 16:29:49.000000 cre-0.4.1/cre/default_funcs.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)    17363 2023-06-02 01:45:53.000000 cre-0.4.1/cre/dynamic_exec.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)    47344 2023-05-27 16:52:23.000000 cre-0.4.1/cre/fact.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)    16306 2023-02-21 03:58:09.000000 cre-0.4.1/cre/fact_intrinsics.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)    93320 2023-07-01 20:52:29.000000 cre-0.4.1/cre/func.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)      656 2023-05-08 03:39:17.000000 cre-0.4.1/cre/garbage3.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)     1088 2023-04-15 18:57:56.000000 cre-0.4.1/cre/garbage31.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)    80851 2023-06-01 22:01:56.000000 cre-0.4.1/cre/garbage_sc_stash.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)    80080 2023-06-01 22:09:06.000000 cre-0.4.1/cre/garbage_sc_stash2.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)     3850 2023-06-05 14:24:45.000000 cre-0.4.1/cre/gval.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)     2270 2023-05-11 22:41:34.000000 cre-0.4.1/cre/hashing.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)     8288 2022-06-12 05:16:49.000000 cre-0.4.1/cre/make_source.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)    81594 2023-06-05 04:30:24.000000 cre-0.4.1/cre/matching.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)    38451 2023-06-05 03:56:00.000000 cre-0.4.1/cre/memset.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)    20497 2023-05-25 18:45:58.000000 cre-0.4.1/cre/obj.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)     5440 2023-02-21 03:58:09.000000 cre-0.4.1/cre/rule.py
+-rwxrwxr-x   0 danny     (1000) danny     (1000)      217 2022-06-12 05:16:49.000000 cre-0.4.1/cre/run_tests
+-rw-rw-r--   0 danny     (1000) danny     (1000)    81185 2023-07-01 04:12:55.000000 cre-0.4.1/cre/sc_planner.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)     9511 2023-02-20 22:35:46.000000 cre-0.4.1/cre/structref.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)     4365 2023-06-30 10:50:15.000000 cre-0.4.1/cre/token.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)    12224 2023-04-28 20:21:41.000000 cre-0.4.1/cre/tuple_fact.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)    10483 2023-05-07 23:44:51.000000 cre-0.4.1/cre/type_conv.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)    47635 2023-05-08 00:32:29.000000 cre-0.4.1/cre/utils.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)    38375 2023-06-13 20:23:15.000000 cre-0.4.1/cre/var.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)     6072 2022-06-12 05:16:49.000000 cre-0.4.1/cre/vector.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)       22 2023-04-29 18:30:06.000000 cre-0.4.1/cre/version.py
+drwxrwxr-x   0 danny     (1000) danny     (1000)        0 2023-07-18 18:12:36.174164 cre-0.4.1/cre.egg-info/
+-rw-rw-r--   0 danny     (1000) danny     (1000)      695 2023-07-18 18:12:36.000000 cre-0.4.1/cre.egg-info/PKG-INFO
+-rw-rw-r--   0 danny     (1000) danny     (1000)     1348 2023-07-18 18:12:36.000000 cre-0.4.1/cre.egg-info/SOURCES.txt
+-rw-rw-r--   0 danny     (1000) danny     (1000)        1 2023-07-18 18:12:36.000000 cre-0.4.1/cre.egg-info/dependency_links.txt
+-rw-rw-r--   0 danny     (1000) danny     (1000)       46 2023-07-18 18:12:36.000000 cre-0.4.1/cre.egg-info/entry_points.txt
+-rw-rw-r--   0 danny     (1000) danny     (1000)       55 2023-07-18 18:12:36.000000 cre-0.4.1/cre.egg-info/requires.txt
+-rw-rw-r--   0 danny     (1000) danny     (1000)       27 2023-07-18 18:12:36.000000 cre-0.4.1/cre.egg-info/top_level.txt
+drwxrwxr-x   0 danny     (1000) danny     (1000)        0 2023-07-18 18:12:36.174164 cre-0.4.1/cre_caching/
+-rw-rw-r--   0 danny     (1000) danny     (1000)       34 2022-06-12 05:16:49.000000 cre-0.4.1/cre_caching/__init__.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)     8199 2023-05-24 20:20:42.000000 cre-0.4.1/cre_caching/caching.py
+drwxrwxr-x   0 danny     (1000) danny     (1000)        0 2023-07-18 18:12:36.174164 cre-0.4.1/notes/
+-rw-rw-r--   0 danny     (1000) danny     (1000)     3560 2022-06-12 05:16:49.000000 cre-0.4.1/notes/SeqGrammarInduction.txt
+-rw-rw-r--   0 danny     (1000) danny     (1000)        1 2023-07-18 17:37:22.000000 cre-0.4.1/pyproject.toml
+-rw-rw-r--   0 danny     (1000) danny     (1000)       24 2023-07-18 17:53:26.000000 cre-0.4.1/requirements.txt
+-rw-rw-r--   0 danny     (1000) danny     (1000)       67 2023-07-18 18:12:36.174164 cre-0.4.1/setup.cfg
+-rw-rw-r--   0 danny     (1000) danny     (1000)     3681 2023-07-18 18:11:53.000000 cre-0.4.1/setup.py
+drwxrwxr-x   0 danny     (1000) danny     (1000)        0 2023-07-18 18:12:36.174164 cre-0.4.1/tests/
+-rw-rw-r--   0 danny     (1000) danny     (1000)    16694 2023-06-02 04:03:51.000000 cre-0.4.1/tests/test_conditions.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)    19089 2023-06-02 05:12:00.000000 cre-0.4.1/tests/test_cre_func.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)    28780 2023-02-21 03:58:22.000000 cre-0.4.1/tests/test_fact.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)     6378 2023-05-08 00:34:10.000000 cre-0.4.1/tests/test_feature_applier.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)     5101 2023-05-15 19:52:19.000000 cre-0.4.1/tests/test_flattener.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)     2466 2023-01-22 23:11:50.000000 cre-0.4.1/tests/test_incr_processor.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)     1326 2022-06-12 05:16:49.000000 cre-0.4.1/tests/test_make_source.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)    23167 2023-05-08 00:29:11.000000 cre-0.4.1/tests/test_matching.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)    19201 2023-05-08 03:49:51.000000 cre-0.4.1/tests/test_memset.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)    16939 2023-05-08 00:36:44.000000 cre-0.4.1/tests/test_processing_pipeline.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)    10230 2023-05-08 00:39:06.000000 cre-0.4.1/tests/test_relative_encoder.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)      714 2023-02-16 07:15:18.000000 cre-0.4.1/tests/test_rule.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)    32453 2023-07-01 04:32:30.000000 cre-0.4.1/tests/test_sc_planner.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)     6565 2023-02-21 03:58:22.000000 cre-0.4.1/tests/test_tuple_fact.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)     3440 2023-02-20 06:20:35.000000 cre-0.4.1/tests/test_type_conv.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)     7282 2023-02-20 05:54:27.000000 cre-0.4.1/tests/test_utils.py
+-rw-rw-r--   0 danny     (1000) danny     (1000)     4416 2023-04-29 17:16:43.000000 cre-0.4.1/tests/test_vectorizer.py
```

### Comparing `cre-0.4.0/LICENSE.txt` & `cre-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/PKG-INFO` & `cre-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cre
-Version: 0.4.0
+Version: 0.4.1
 Summary: A rule engine for Python powered by numba.
 Home-page: https://github.com/DannyWeitekamp/Cognitive-Rule-Engine
 Author: Daniel Weitekamp
 Author-email: dannyweitekamp@gmail.com
 License: MIT
 Keywords: rule engine,expert system,production rules
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cre-0.4.0/README.md` & `cre-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/console/cre_exec.py` & `cre-0.4.1/console/cre_exec.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/cre/__init__.py` & `cre-0.4.1/cre/__init__.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/cre/attr_filter.py` & `cre-0.4.1/cre/attr_filter.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/cre/cfuncs/cre_cfuncs.c` & `cre-0.4.1/cre/cfuncs/cre_cfuncs.c`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/cre/change_event.py` & `cre-0.4.1/cre/change_event.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/cre/conditions.py` & `cre-0.4.1/cre/conditions.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/cre/context.py` & `cre-0.4.1/cre/context.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/cre/core.py` & `cre-0.4.1/cre/core.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/cre/default_funcs.py` & `cre-0.4.1/cre/default_funcs.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/cre/dynamic_exec.py` & `cre-0.4.1/cre/dynamic_exec.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/cre/fact.py` & `cre-0.4.1/cre/fact.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/cre/fact_intrinsics.py` & `cre-0.4.1/cre/fact_intrinsics.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/cre/func.py` & `cre-0.4.1/cre/func.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/cre/garbage3.py` & `cre-0.4.1/cre/garbage3.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/cre/garbage31.py` & `cre-0.4.1/cre/garbage31.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/cre/garbage_sc_stash.py` & `cre-0.4.1/cre/garbage_sc_stash.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/cre/garbage_sc_stash2.py` & `cre-0.4.1/cre/garbage_sc_stash2.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/cre/gval.py` & `cre-0.4.1/cre/gval.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/cre/hashing.py` & `cre-0.4.1/cre/hashing.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/cre/make_source.py` & `cre-0.4.1/cre/make_source.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/cre/matching.py` & `cre-0.4.1/cre/matching.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/cre/memset.py` & `cre-0.4.1/cre/memset.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/cre/obj.py` & `cre-0.4.1/cre/obj.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/cre/rule.py` & `cre-0.4.1/cre/rule.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/cre/sc_planner.py` & `cre-0.4.1/cre/sc_planner.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/cre/structref.py` & `cre-0.4.1/cre/structref.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/cre/token.py` & `cre-0.4.1/cre/token.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/cre/tuple_fact.py` & `cre-0.4.1/cre/tuple_fact.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/cre/type_conv.py` & `cre-0.4.1/cre/type_conv.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/cre/utils.py` & `cre-0.4.1/cre/utils.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/cre/var.py` & `cre-0.4.1/cre/var.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/cre/vector.py` & `cre-0.4.1/cre/vector.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/cre.egg-info/PKG-INFO` & `cre-0.4.1/cre.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cre
-Version: 0.4.0
+Version: 0.4.1
 Summary: A rule engine for Python powered by numba.
 Home-page: https://github.com/DannyWeitekamp/Cognitive-Rule-Engine
 Author: Daniel Weitekamp
 Author-email: dannyweitekamp@gmail.com
 License: MIT
 Keywords: rule engine,expert system,production rules
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cre-0.4.0/cre.egg-info/SOURCES.txt` & `cre-0.4.1/cre.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/cre_caching/caching.py` & `cre-0.4.1/cre_caching/caching.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/notes/SeqGrammarInduction.txt` & `cre-0.4.1/notes/SeqGrammarInduction.txt`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/setup.py` & `cre-0.4.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 mo = re.search(VSRE, verstrline, re.M)
 if mo:
     __version__ = mo.group(1)
 else:
     raise RuntimeError("Unable to find version string in %s." % (VERSIONFILE,))
 
 # TODO: Remove once version dependancy issues in caching are fixed
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 
 
 # Read requirements.txt for requirements
 with open('requirements.txt') as f: 
     requirements = f.readlines() 
 
   
@@ -63,20 +63,29 @@
     if not os.path.exists(python_headers_path):
         major = sys.version_info.major
         minor = sys.version_info.minor
         raise ModuleNotFoundError(
     f"Ensure python headers installed: `sudo apt-get install libpython{major}.{minor}-dev`"
         )
 
-    numba = ensure_numba()
-    numba_path = numba.extending.include_path()
+    include_dirs = [sysconfig.get_path('include')]
+
+    # Numba is required ahead of time to compile the cfunc extension module.
+    #  But if installing from PyPi then we'll get it precompiled.
+    try:
+        numba = ensure_numba()
+        numba_path = numba.extending.include_path()
+        include_dirs = [numba_path, sysconfig.get_path('include')]
+    except:
+        pass
+
     cre_c_funcs = Extension(
         name='cre_cfuncs', 
         sources=['cre/cfuncs/cre_cfuncs.c'],
-        include_dirs=[numba_path, sysconfig.get_path('include')]
+        include_dirs=include_dirs
     )
     return [cre_c_funcs]
 
   
 setup( 
         name ='cre', 
         version = __version__,
```

### Comparing `cre-0.4.0/tests/test_conditions.py` & `cre-0.4.1/tests/test_conditions.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/tests/test_cre_func.py` & `cre-0.4.1/tests/test_cre_func.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/tests/test_fact.py` & `cre-0.4.1/tests/test_fact.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/tests/test_feature_applier.py` & `cre-0.4.1/tests/test_feature_applier.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/tests/test_flattener.py` & `cre-0.4.1/tests/test_flattener.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/tests/test_incr_processor.py` & `cre-0.4.1/tests/test_incr_processor.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/tests/test_make_source.py` & `cre-0.4.1/tests/test_make_source.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/tests/test_matching.py` & `cre-0.4.1/tests/test_matching.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/tests/test_memset.py` & `cre-0.4.1/tests/test_memset.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/tests/test_processing_pipeline.py` & `cre-0.4.1/tests/test_processing_pipeline.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/tests/test_relative_encoder.py` & `cre-0.4.1/tests/test_relative_encoder.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/tests/test_rule.py` & `cre-0.4.1/tests/test_rule.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/tests/test_sc_planner.py` & `cre-0.4.1/tests/test_sc_planner.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/tests/test_tuple_fact.py` & `cre-0.4.1/tests/test_tuple_fact.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/tests/test_type_conv.py` & `cre-0.4.1/tests/test_type_conv.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/tests/test_utils.py` & `cre-0.4.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `cre-0.4.0/tests/test_vectorizer.py` & `cre-0.4.1/tests/test_vectorizer.py`

 * *Files identical despite different names*

