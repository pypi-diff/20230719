# Comparing `tmp/uqpylab-0.2.tar.gz` & `tmp/uqpylab-0.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/uqpylab-0.2.tar", last modified: Tue Jun  1 11:51:25 2021, max compression
+gzip compressed data, was "uqpylab-0.95.tar", max compression
```

## Comparing `uqpylab-0.2.tar` & `uqpylab-0.95.tar`

### file list

```diff
@@ -1,14 +1,28 @@
-drwxrwxr-x   0 latanioc  (1000) latanioc  (1000)        0 2021-06-01 11:51:25.000000 uqpylab-0.2/
--rw-rw-r--   0 latanioc  (1000) latanioc  (1000)      699 2021-06-01 11:51:25.000000 uqpylab-0.2/PKG-INFO
--rw-rw-r--   0 latanioc  (1000) latanioc  (1000)      172 2021-06-01 11:45:29.000000 uqpylab-0.2/README.md
--rw-rw-r--   0 latanioc  (1000) latanioc  (1000)       38 2021-06-01 11:51:25.000000 uqpylab-0.2/setup.cfg
--rw-r--r--   0 latanioc  (1000) latanioc  (1000)      822 2021-06-01 11:46:59.000000 uqpylab-0.2/setup.py
-drwxrwxr-x   0 latanioc  (1000) latanioc  (1000)        0 2021-06-01 11:51:25.000000 uqpylab-0.2/uqpylab/
--rw-r--r--   0 latanioc  (1000) latanioc  (1000)        0 2020-05-05 10:12:47.000000 uqpylab-0.2/uqpylab/__init__.py
--rw-r--r--   0 latanioc  (1000) latanioc  (1000)       22 2021-06-01 11:40:28.000000 uqpylab-0.2/uqpylab/placeholder.py
-drwxrwxr-x   0 latanioc  (1000) latanioc  (1000)        0 2021-06-01 11:51:25.000000 uqpylab-0.2/uqpylab.egg-info/
--rw-rw-r--   0 latanioc  (1000) latanioc  (1000)      699 2021-06-01 11:51:25.000000 uqpylab-0.2/uqpylab.egg-info/PKG-INFO
--rw-rw-r--   0 latanioc  (1000) latanioc  (1000)      215 2021-06-01 11:51:25.000000 uqpylab-0.2/uqpylab.egg-info/SOURCES.txt
--rw-rw-r--   0 latanioc  (1000) latanioc  (1000)        1 2021-06-01 11:51:25.000000 uqpylab-0.2/uqpylab.egg-info/dependency_links.txt
--rw-rw-r--   0 latanioc  (1000) latanioc  (1000)       23 2021-06-01 11:51:25.000000 uqpylab-0.2/uqpylab.egg-info/requires.txt
--rw-rw-r--   0 latanioc  (1000) latanioc  (1000)        8 2021-06-01 11:51:25.000000 uqpylab-0.2/uqpylab.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1583 2023-07-19 07:41:44.311339 uqpylab-0.95/LICENSE
+-rw-r--r--   0        0        0      813 2023-07-19 07:43:31.363592 uqpylab-0.95/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-12-19 15:54:46.563214 uqpylab-0.95/uqpylab/__init__.py
+-rw-r--r--   0        0        0    17697 2023-07-05 12:14:53.548013 uqpylab-0.95/uqpylab/display_general.py
+-rw-r--r--   0        0        0    24880 2023-07-05 15:06:45.814607 uqpylab-0.95/uqpylab/display_reliability.py
+-rw-r--r--   0        0        0    29148 2023-07-05 12:14:53.548013 uqpylab-0.95/uqpylab/display_sensitivity.py
+-rw-r--r--   0        0        0    20071 2023-06-13 07:17:41.268452 uqpylab-0.95/uqpylab/display_util.py
+-rw-r--r--   0        0        0     7064 2023-03-23 07:39:03.709860 uqpylab-0.95/uqpylab/helpers.py
+-rw-r--r--   0        0        0    39853 2023-07-13 12:14:40.912365 uqpylab-0.95/uqpylab/interface.py
+-rw-r--r--   0        0        0    22908 2023-06-13 07:17:41.268452 uqpylab-0.95/uqpylab/sessions.py
+-rw-r--r--   0        0        0        0 2022-12-19 15:54:46.567214 uqpylab-0.95/uqpylab/test/__init__.py
+-rw-r--r--   0        0        0     1192 2023-03-14 16:08:42.594797 uqpylab-0.95/uqpylab/test/conftest.py
+-rwxr-xr-x   0        0        0       74 2023-03-17 07:58:16.503091 uqpylab-0.95/uqpylab/test/suppress_jupyter_warnings.sh
+-rw-r--r--   0        0        0     6453 2023-07-11 07:50:16.462794 uqpylab-0.95/uqpylab/test/test_analysis.py
+-rw-r--r--   0        0        0     3557 2023-07-11 07:50:16.462794 uqpylab-0.95/uqpylab/test/test_display.py
+-rw-r--r--   0        0        0     3548 2023-07-11 07:50:16.462794 uqpylab-0.95/uqpylab/test/test_inference.py
+-rw-r--r--   0        0        0     1697 2023-07-11 07:50:16.462794 uqpylab-0.95/uqpylab/test/test_input.py
+-rw-r--r--   0        0        0    22388 2023-06-13 07:17:41.272452 uqpylab-0.95/uqpylab/test/test_input_aux_funs.py
+-rw-r--r--   0        0        0     3169 2023-07-11 07:50:16.462794 uqpylab-0.95/uqpylab/test/test_intermids.py
+-rw-r--r--   0        0        0     1824 2023-07-11 07:50:16.462794 uqpylab-0.95/uqpylab/test/test_inversion.py
+-rw-r--r--   0        0        0     2171 2023-07-11 07:50:16.462794 uqpylab-0.95/uqpylab/test/test_mat_input.py
+-rw-r--r--   0        0        0     2101 2023-07-11 07:50:16.462794 uqpylab-0.95/uqpylab/test/test_mat_model.py
+-rw-r--r--   0        0        0     4238 2023-07-11 07:50:16.462794 uqpylab-0.95/uqpylab/test/test_model.py
+-rw-r--r--   0        0        0     2995 2023-07-11 07:50:16.462794 uqpylab-0.95/uqpylab/test/test_sessions.py
+-rw-r--r--   0        0        0     1432 2023-07-11 07:50:16.466794 uqpylab-0.95/uqpylab/test/test_singleton.py
+-rw-r--r--   0        0        0      583 2023-06-13 07:17:41.272452 uqpylab-0.95/uqpylab/test/true_models.py
+-rw-r--r--   0        0        0      899 1970-01-01 00:00:00.000000 uqpylab-0.95/setup.py
+-rw-r--r--   0        0        0      839 1970-01-01 00:00:00.000000 uqpylab-0.95/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

