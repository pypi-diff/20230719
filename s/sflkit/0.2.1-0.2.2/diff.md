# Comparing `tmp/sflkit-0.2.1.tar.gz` & `tmp/sflkit-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sflkit-0.2.1.tar", last modified: Tue Jul 18 09:34:38 2023, max compression
+gzip compressed data, was "sflkit-0.2.2.tar", last modified: Wed Jul 19 11:37:28 2023, max compression
```

## Comparing `sflkit-0.2.1.tar` & `sflkit-0.2.2.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-18 09:34:38.050030 sflkit-0.2.1/
--rw-r--r--   0 marius     (501) staff       (20)     1112 2023-03-23 09:55:10.000000 sflkit-0.2.1/LICENSE
--rw-r--r--   0 marius     (501) staff       (20)     4817 2023-07-18 09:34:38.050166 sflkit-0.2.1/PKG-INFO
--rw-r--r--   0 marius     (501) staff       (20)     4062 2023-03-24 13:14:28.000000 sflkit-0.2.1/README.md
--rw-r--r--   0 marius     (501) staff       (20)      809 2023-07-18 08:52:29.000000 sflkit-0.2.1/pyproject.toml
--rw-r--r--   0 marius     (501) staff       (20)     1278 2023-07-18 09:34:38.051113 sflkit-0.2.1/setup.cfg
--rw-r--r--   0 marius     (501) staff       (20)       39 2023-03-23 09:55:13.000000 sflkit-0.2.1/setup.py
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-18 09:34:38.023363 sflkit-0.2.1/src/
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-18 09:34:38.029558 sflkit-0.2.1/src/SFLKit.egg-info/
--rw-r--r--   0 marius     (501) staff       (20)     4817 2023-07-18 09:34:38.000000 sflkit-0.2.1/src/SFLKit.egg-info/PKG-INFO
--rw-r--r--   0 marius     (501) staff       (20)     1848 2023-07-18 09:34:38.000000 sflkit-0.2.1/src/SFLKit.egg-info/SOURCES.txt
--rw-r--r--   0 marius     (501) staff       (20)        1 2023-07-18 09:34:38.000000 sflkit-0.2.1/src/SFLKit.egg-info/dependency_links.txt
--rw-r--r--   0 marius     (501) staff       (20)       43 2023-07-18 09:34:38.000000 sflkit-0.2.1/src/SFLKit.egg-info/entry_points.txt
--rw-r--r--   0 marius     (501) staff       (20)      311 2023-07-18 09:34:38.000000 sflkit-0.2.1/src/SFLKit.egg-info/requires.txt
--rw-r--r--   0 marius     (501) staff       (20)        7 2023-07-18 09:34:38.000000 sflkit-0.2.1/src/SFLKit.egg-info/top_level.txt
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-18 09:34:38.031857 sflkit-0.2.1/src/sflkit/
--rw-r--r--   0 marius     (501) staff       (20)     2330 2023-07-18 09:25:52.000000 sflkit-0.2.1/src/sflkit/__init__.py
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-18 09:34:38.036781 sflkit-0.2.1/src/sflkit/analysis/
--rw-r--r--   0 marius     (501) staff       (20)      161 2023-03-23 09:55:13.000000 sflkit-0.2.1/src/sflkit/analysis/__init__.py
--rw-r--r--   0 marius     (501) staff       (20)     3331 2023-03-24 10:29:50.000000 sflkit-0.2.1/src/sflkit/analysis/analysis_type.py
--rw-r--r--   0 marius     (501) staff       (20)     2228 2023-03-23 17:28:40.000000 sflkit-0.2.1/src/sflkit/analysis/analyzer.py
--rw-r--r--   0 marius     (501) staff       (20)    13819 2023-07-18 09:22:13.000000 sflkit-0.2.1/src/sflkit/analysis/factory.py
--rw-r--r--   0 marius     (501) staff       (20)     1511 2023-03-23 09:55:13.000000 sflkit-0.2.1/src/sflkit/analysis/mapping.py
--rw-r--r--   0 marius     (501) staff       (20)    10727 2023-07-18 09:22:13.000000 sflkit-0.2.1/src/sflkit/analysis/predicate.py
--rw-r--r--   0 marius     (501) staff       (20)     1045 2023-03-24 10:29:08.000000 sflkit-0.2.1/src/sflkit/analysis/similarity.py
--rw-r--r--   0 marius     (501) staff       (20)    17373 2023-07-18 09:22:46.000000 sflkit-0.2.1/src/sflkit/analysis/spectra.py
--rw-r--r--   0 marius     (501) staff       (20)     1224 2023-03-23 15:58:48.000000 sflkit-0.2.1/src/sflkit/analysis/suggestion.py
--rw-r--r--   0 marius     (501) staff       (20)     3643 2023-07-18 08:52:29.000000 sflkit-0.2.1/src/sflkit/cli.py
--rw-r--r--   0 marius     (501) staff       (20)     3432 2023-03-23 09:55:13.000000 sflkit-0.2.1/src/sflkit/color.py
--rw-r--r--   0 marius     (501) staff       (20)    10920 2023-07-18 09:25:52.000000 sflkit-0.2.1/src/sflkit/config.py
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-18 09:34:38.038086 sflkit-0.2.1/src/sflkit/instrumentation/
--rw-r--r--   0 marius     (501) staff       (20)      661 2023-07-18 09:22:46.000000 sflkit-0.2.1/src/sflkit/instrumentation/__init__.py
--rw-r--r--   0 marius     (501) staff       (20)     3382 2023-07-18 09:23:43.000000 sflkit-0.2.1/src/sflkit/instrumentation/dir_instrumentation.py
--rw-r--r--   0 marius     (501) staff       (20)      446 2023-03-23 09:55:13.000000 sflkit-0.2.1/src/sflkit/instrumentation/file_instrumentation.py
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-18 09:34:38.041049 sflkit-0.2.1/src/sflkit/language/
--rw-r--r--   0 marius     (501) staff       (20)      151 2023-03-23 09:55:13.000000 sflkit-0.2.1/src/sflkit/language/__init__.py
--rw-r--r--   0 marius     (501) staff       (20)      353 2023-03-24 09:13:32.000000 sflkit-0.2.1/src/sflkit/language/extract.py
--rw-r--r--   0 marius     (501) staff       (20)      654 2023-03-23 15:08:14.000000 sflkit-0.2.1/src/sflkit/language/finder.py
--rw-r--r--   0 marius     (501) staff       (20)     3798 2023-07-18 09:25:18.000000 sflkit-0.2.1/src/sflkit/language/language.py
--rw-r--r--   0 marius     (501) staff       (20)     4066 2023-07-18 09:24:46.000000 sflkit-0.2.1/src/sflkit/language/meta.py
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-18 09:34:38.042765 sflkit-0.2.1/src/sflkit/language/python/
--rw-r--r--   0 marius     (501) staff       (20)        0 2023-03-23 09:55:13.000000 sflkit-0.2.1/src/sflkit/language/python/__init__.py
--rw-r--r--   0 marius     (501) staff       (20)     8602 2023-07-18 09:24:46.000000 sflkit-0.2.1/src/sflkit/language/python/extract.py
--rw-r--r--   0 marius     (501) staff       (20)    26800 2023-07-18 09:31:57.000000 sflkit-0.2.1/src/sflkit/language/python/factory.py
--rw-r--r--   0 marius     (501) staff       (20)     2990 2023-03-23 09:55:13.000000 sflkit-0.2.1/src/sflkit/language/python/finder.py
--rw-r--r--   0 marius     (501) staff       (20)     6119 2023-03-23 09:55:13.000000 sflkit-0.2.1/src/sflkit/language/python/visitor.py
--rw-r--r--   0 marius     (501) staff       (20)     1085 2023-07-18 08:52:29.000000 sflkit-0.2.1/src/sflkit/language/visitor.py
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-18 09:34:38.044432 sflkit-0.2.1/src/sflkit/model/
--rw-r--r--   0 marius     (501) staff       (20)      163 2023-03-23 09:55:13.000000 sflkit-0.2.1/src/sflkit/model/__init__.py
--rw-r--r--   0 marius     (501) staff       (20)      806 2023-07-18 09:25:18.000000 sflkit-0.2.1/src/sflkit/model/event_file.py
--rw-r--r--   0 marius     (501) staff       (20)     2073 2023-03-23 09:55:13.000000 sflkit-0.2.1/src/sflkit/model/model.py
--rw-r--r--   0 marius     (501) staff       (20)     1007 2023-03-23 09:55:13.000000 sflkit-0.2.1/src/sflkit/model/scope.py
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-18 09:34:38.045379 sflkit-0.2.1/src/sflkit/runners/
--rw-r--r--   0 marius     (501) staff       (20)      293 2023-06-28 09:49:26.000000 sflkit-0.2.1/src/sflkit/runners/__init__.py
--rw-r--r--   0 marius     (501) staff       (20)     7338 2023-07-18 08:52:29.000000 sflkit-0.2.1/src/sflkit/runners/run.py
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-18 09:34:38.049704 sflkit-0.2.1/tests/
--rw-r--r--   0 marius     (501) staff       (20)     7993 2023-07-18 09:27:16.000000 sflkit-0.2.1/tests/test_analysis_objects.py
--rw-r--r--   0 marius     (501) staff       (20)     2057 2023-03-23 18:03:53.000000 sflkit-0.2.1/tests/test_cli.py
--rw-r--r--   0 marius     (501) staff       (20)     1025 2023-03-24 09:19:40.000000 sflkit-0.2.1/tests/test_color.py
--rw-r--r--   0 marius     (501) staff       (20)     6194 2023-07-18 09:28:33.000000 sflkit-0.2.1/tests/test_config.py
--rw-r--r--   0 marius     (501) staff       (20)    14215 2023-07-18 09:30:53.000000 sflkit-0.2.1/tests/test_events.py
--rw-r--r--   0 marius     (501) staff       (20)     1318 2023-03-23 17:37:40.000000 sflkit-0.2.1/tests/test_execution.py
--rw-r--r--   0 marius     (501) staff       (20)     5090 2023-07-18 09:32:50.000000 sflkit-0.2.1/tests/test_instrumentation.py
--rw-r--r--   0 marius     (501) staff       (20)     8856 2023-07-18 09:28:00.000000 sflkit-0.2.1/tests/test_language.py
--rw-r--r--   0 marius     (501) staff       (20)     2773 2023-03-23 09:55:13.000000 sflkit-0.2.1/tests/test_predicates.py
--rw-r--r--   0 marius     (501) staff       (20)     6061 2023-06-28 09:49:26.000000 sflkit-0.2.1/tests/test_runner.py
--rw-r--r--   0 marius     (501) staff       (20)      615 2023-03-23 15:20:53.000000 sflkit-0.2.1/tests/test_scope.py
--rw-r--r--   0 marius     (501) staff       (20)     4279 2023-07-18 09:27:50.000000 sflkit-0.2.1/tests/test_spectra.py
--rw-r--r--   0 marius     (501) staff       (20)    11301 2023-03-24 12:11:43.000000 sflkit-0.2.1/tests/test_suggestions.py
--rw-r--r--   0 marius     (501) staff       (20)     1912 2023-03-23 09:55:13.000000 sflkit-0.2.1/tests/test_visitors.py
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-19 11:37:28.333675 sflkit-0.2.2/
+-rw-r--r--   0 marius     (501) staff       (20)     1112 2023-03-23 09:55:10.000000 sflkit-0.2.2/LICENSE
+-rw-r--r--   0 marius     (501) staff       (20)     4817 2023-07-19 11:37:28.333795 sflkit-0.2.2/PKG-INFO
+-rw-r--r--   0 marius     (501) staff       (20)     4062 2023-03-24 13:14:28.000000 sflkit-0.2.2/README.md
+-rw-r--r--   0 marius     (501) staff       (20)      809 2023-07-19 11:35:55.000000 sflkit-0.2.2/pyproject.toml
+-rw-r--r--   0 marius     (501) staff       (20)     1278 2023-07-19 11:37:28.334380 sflkit-0.2.2/setup.cfg
+-rw-r--r--   0 marius     (501) staff       (20)       39 2023-03-23 09:55:13.000000 sflkit-0.2.2/setup.py
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-19 11:37:28.299399 sflkit-0.2.2/src/
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-19 11:37:28.305022 sflkit-0.2.2/src/SFLKit.egg-info/
+-rw-r--r--   0 marius     (501) staff       (20)     4817 2023-07-19 11:37:28.000000 sflkit-0.2.2/src/SFLKit.egg-info/PKG-INFO
+-rw-r--r--   0 marius     (501) staff       (20)     1848 2023-07-19 11:37:28.000000 sflkit-0.2.2/src/SFLKit.egg-info/SOURCES.txt
+-rw-r--r--   0 marius     (501) staff       (20)        1 2023-07-19 11:37:28.000000 sflkit-0.2.2/src/SFLKit.egg-info/dependency_links.txt
+-rw-r--r--   0 marius     (501) staff       (20)       43 2023-07-19 11:37:28.000000 sflkit-0.2.2/src/SFLKit.egg-info/entry_points.txt
+-rw-r--r--   0 marius     (501) staff       (20)      311 2023-07-19 11:37:28.000000 sflkit-0.2.2/src/SFLKit.egg-info/requires.txt
+-rw-r--r--   0 marius     (501) staff       (20)        7 2023-07-19 11:37:28.000000 sflkit-0.2.2/src/SFLKit.egg-info/top_level.txt
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-19 11:37:28.307020 sflkit-0.2.2/src/sflkit/
+-rw-r--r--   0 marius     (501) staff       (20)     2330 2023-07-19 11:36:10.000000 sflkit-0.2.2/src/sflkit/__init__.py
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-19 11:37:28.314881 sflkit-0.2.2/src/sflkit/analysis/
+-rw-r--r--   0 marius     (501) staff       (20)      161 2023-03-23 09:55:13.000000 sflkit-0.2.2/src/sflkit/analysis/__init__.py
+-rw-r--r--   0 marius     (501) staff       (20)     3331 2023-03-24 10:29:50.000000 sflkit-0.2.2/src/sflkit/analysis/analysis_type.py
+-rw-r--r--   0 marius     (501) staff       (20)     2228 2023-03-23 17:28:40.000000 sflkit-0.2.2/src/sflkit/analysis/analyzer.py
+-rw-r--r--   0 marius     (501) staff       (20)    13819 2023-07-18 09:22:13.000000 sflkit-0.2.2/src/sflkit/analysis/factory.py
+-rw-r--r--   0 marius     (501) staff       (20)     1511 2023-03-23 09:55:13.000000 sflkit-0.2.2/src/sflkit/analysis/mapping.py
+-rw-r--r--   0 marius     (501) staff       (20)    10727 2023-07-18 09:22:13.000000 sflkit-0.2.2/src/sflkit/analysis/predicate.py
+-rw-r--r--   0 marius     (501) staff       (20)     1045 2023-03-24 10:29:08.000000 sflkit-0.2.2/src/sflkit/analysis/similarity.py
+-rw-r--r--   0 marius     (501) staff       (20)    17373 2023-07-18 09:22:46.000000 sflkit-0.2.2/src/sflkit/analysis/spectra.py
+-rw-r--r--   0 marius     (501) staff       (20)     1224 2023-03-23 15:58:48.000000 sflkit-0.2.2/src/sflkit/analysis/suggestion.py
+-rw-r--r--   0 marius     (501) staff       (20)     3643 2023-07-18 08:52:29.000000 sflkit-0.2.2/src/sflkit/cli.py
+-rw-r--r--   0 marius     (501) staff       (20)     3432 2023-03-23 09:55:13.000000 sflkit-0.2.2/src/sflkit/color.py
+-rw-r--r--   0 marius     (501) staff       (20)    10920 2023-07-18 09:25:52.000000 sflkit-0.2.2/src/sflkit/config.py
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-19 11:37:28.316891 sflkit-0.2.2/src/sflkit/instrumentation/
+-rw-r--r--   0 marius     (501) staff       (20)      661 2023-07-18 09:22:46.000000 sflkit-0.2.2/src/sflkit/instrumentation/__init__.py
+-rw-r--r--   0 marius     (501) staff       (20)     3382 2023-07-18 09:23:43.000000 sflkit-0.2.2/src/sflkit/instrumentation/dir_instrumentation.py
+-rw-r--r--   0 marius     (501) staff       (20)      446 2023-03-23 09:55:13.000000 sflkit-0.2.2/src/sflkit/instrumentation/file_instrumentation.py
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-19 11:37:28.320524 sflkit-0.2.2/src/sflkit/language/
+-rw-r--r--   0 marius     (501) staff       (20)      151 2023-03-23 09:55:13.000000 sflkit-0.2.2/src/sflkit/language/__init__.py
+-rw-r--r--   0 marius     (501) staff       (20)      353 2023-03-24 09:13:32.000000 sflkit-0.2.2/src/sflkit/language/extract.py
+-rw-r--r--   0 marius     (501) staff       (20)      654 2023-03-23 15:08:14.000000 sflkit-0.2.2/src/sflkit/language/finder.py
+-rw-r--r--   0 marius     (501) staff       (20)     3798 2023-07-18 09:25:18.000000 sflkit-0.2.2/src/sflkit/language/language.py
+-rw-r--r--   0 marius     (501) staff       (20)     4066 2023-07-18 09:24:46.000000 sflkit-0.2.2/src/sflkit/language/meta.py
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-19 11:37:28.323161 sflkit-0.2.2/src/sflkit/language/python/
+-rw-r--r--   0 marius     (501) staff       (20)        0 2023-03-23 09:55:13.000000 sflkit-0.2.2/src/sflkit/language/python/__init__.py
+-rw-r--r--   0 marius     (501) staff       (20)     8602 2023-07-18 09:24:46.000000 sflkit-0.2.2/src/sflkit/language/python/extract.py
+-rw-r--r--   0 marius     (501) staff       (20)    26800 2023-07-18 09:31:57.000000 sflkit-0.2.2/src/sflkit/language/python/factory.py
+-rw-r--r--   0 marius     (501) staff       (20)     2990 2023-03-23 09:55:13.000000 sflkit-0.2.2/src/sflkit/language/python/finder.py
+-rw-r--r--   0 marius     (501) staff       (20)     6119 2023-03-23 09:55:13.000000 sflkit-0.2.2/src/sflkit/language/python/visitor.py
+-rw-r--r--   0 marius     (501) staff       (20)     1085 2023-07-18 08:52:29.000000 sflkit-0.2.2/src/sflkit/language/visitor.py
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-19 11:37:28.324800 sflkit-0.2.2/src/sflkit/model/
+-rw-r--r--   0 marius     (501) staff       (20)      163 2023-03-23 09:55:13.000000 sflkit-0.2.2/src/sflkit/model/__init__.py
+-rw-r--r--   0 marius     (501) staff       (20)      806 2023-07-18 09:25:18.000000 sflkit-0.2.2/src/sflkit/model/event_file.py
+-rw-r--r--   0 marius     (501) staff       (20)     2073 2023-03-23 09:55:13.000000 sflkit-0.2.2/src/sflkit/model/model.py
+-rw-r--r--   0 marius     (501) staff       (20)     1007 2023-03-23 09:55:13.000000 sflkit-0.2.2/src/sflkit/model/scope.py
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-19 11:37:28.325416 sflkit-0.2.2/src/sflkit/runners/
+-rw-r--r--   0 marius     (501) staff       (20)      362 2023-07-19 11:34:17.000000 sflkit-0.2.2/src/sflkit/runners/__init__.py
+-rw-r--r--   0 marius     (501) staff       (20)     8604 2023-07-19 11:31:52.000000 sflkit-0.2.2/src/sflkit/runners/run.py
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-19 11:37:28.333196 sflkit-0.2.2/tests/
+-rw-r--r--   0 marius     (501) staff       (20)     7993 2023-07-18 09:27:16.000000 sflkit-0.2.2/tests/test_analysis_objects.py
+-rw-r--r--   0 marius     (501) staff       (20)     2057 2023-03-23 18:03:53.000000 sflkit-0.2.2/tests/test_cli.py
+-rw-r--r--   0 marius     (501) staff       (20)     1025 2023-03-24 09:19:40.000000 sflkit-0.2.2/tests/test_color.py
+-rw-r--r--   0 marius     (501) staff       (20)     6194 2023-07-18 09:28:33.000000 sflkit-0.2.2/tests/test_config.py
+-rw-r--r--   0 marius     (501) staff       (20)    14215 2023-07-18 09:30:53.000000 sflkit-0.2.2/tests/test_events.py
+-rw-r--r--   0 marius     (501) staff       (20)     1318 2023-03-23 17:37:40.000000 sflkit-0.2.2/tests/test_execution.py
+-rw-r--r--   0 marius     (501) staff       (20)     5090 2023-07-18 09:32:50.000000 sflkit-0.2.2/tests/test_instrumentation.py
+-rw-r--r--   0 marius     (501) staff       (20)     8856 2023-07-18 09:28:00.000000 sflkit-0.2.2/tests/test_language.py
+-rw-r--r--   0 marius     (501) staff       (20)     2773 2023-03-23 09:55:13.000000 sflkit-0.2.2/tests/test_predicates.py
+-rw-r--r--   0 marius     (501) staff       (20)     7727 2023-07-19 11:35:28.000000 sflkit-0.2.2/tests/test_runner.py
+-rw-r--r--   0 marius     (501) staff       (20)      615 2023-03-23 15:20:53.000000 sflkit-0.2.2/tests/test_scope.py
+-rw-r--r--   0 marius     (501) staff       (20)     4279 2023-07-18 09:27:50.000000 sflkit-0.2.2/tests/test_spectra.py
+-rw-r--r--   0 marius     (501) staff       (20)    11301 2023-03-24 12:11:43.000000 sflkit-0.2.2/tests/test_suggestions.py
+-rw-r--r--   0 marius     (501) staff       (20)     1912 2023-03-23 09:55:13.000000 sflkit-0.2.2/tests/test_visitors.py
```

### Comparing `sflkit-0.2.1/LICENSE` & `sflkit-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.1/PKG-INFO` & `sflkit-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sflkit
-Version: 0.2.1
+Version: 0.2.2
 Summary: SFLKit: : A Workbench for Statistical Fault Localization
 Home-page: https://github.com/uds-se/sflkit
 Author: Marius Smytzek & Andreas Zeller
 Author-email: Marius Smytzek <marius.smytzek@cispa.de>
 Project-URL: Homepage, https://github.com/uds-se/sflkit/
 Project-URL: Bug Tracker, https://github.com/uds-se/sflkit/issues
 Classifier: Intended Audience :: Science/Research
```

### Comparing `sflkit-0.2.1/README.md` & `sflkit-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.1/pyproject.toml` & `sflkit-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=67.6.0",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sflkit"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
     { name = "Marius Smytzek", email = "marius.smytzek@cispa.de" },
 ]
 description = "SFLKit: : A Workbench for Statistical Fault Localization"
 readme = "README.md"
 license = { file = "COPYING" }
 requires-python = ">=3.10"
```

### Comparing `sflkit-0.2.1/setup.cfg` & `sflkit-0.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.1/src/SFLKit.egg-info/PKG-INFO` & `sflkit-0.2.2/src/SFLKit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sflkit
-Version: 0.2.1
+Version: 0.2.2
 Summary: SFLKit: : A Workbench for Statistical Fault Localization
 Home-page: https://github.com/uds-se/sflkit
 Author: Marius Smytzek & Andreas Zeller
 Author-email: Marius Smytzek <marius.smytzek@cispa.de>
 Project-URL: Homepage, https://github.com/uds-se/sflkit/
 Project-URL: Bug Tracker, https://github.com/uds-se/sflkit/issues
 Classifier: Intended Audience :: Science/Research
```

### Comparing `sflkit-0.2.1/src/SFLKit.egg-info/SOURCES.txt` & `sflkit-0.2.2/src/SFLKit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.1/src/sflkit/__init__.py` & `sflkit-0.2.2/src/sflkit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 from sflkit.analysis.analyzer import Analyzer
 from sflkit.analysis.predicate import Predicate
 from sflkit.config import Config, parse_config
 from sflkit.instrumentation.dir_instrumentation import DirInstrumentation
 
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 
 
 def instrument_config(conf: Config, event_dump: str = None):
     instrumentation = DirInstrumentation(conf.visitor)
     instrumentation.instrument(
         conf.target_path,
         conf.instrument_working,
```

### Comparing `sflkit-0.2.1/src/sflkit/analysis/analysis_type.py` & `sflkit-0.2.2/src/sflkit/analysis/analysis_type.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.1/src/sflkit/analysis/analyzer.py` & `sflkit-0.2.2/src/sflkit/analysis/analyzer.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.1/src/sflkit/analysis/factory.py` & `sflkit-0.2.2/src/sflkit/analysis/factory.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.1/src/sflkit/analysis/mapping.py` & `sflkit-0.2.2/src/sflkit/analysis/mapping.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.1/src/sflkit/analysis/predicate.py` & `sflkit-0.2.2/src/sflkit/analysis/predicate.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.1/src/sflkit/analysis/similarity.py` & `sflkit-0.2.2/src/sflkit/analysis/similarity.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.1/src/sflkit/analysis/spectra.py` & `sflkit-0.2.2/src/sflkit/analysis/spectra.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.1/src/sflkit/analysis/suggestion.py` & `sflkit-0.2.2/src/sflkit/analysis/suggestion.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.1/src/sflkit/cli.py` & `sflkit-0.2.2/src/sflkit/cli.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.1/src/sflkit/color.py` & `sflkit-0.2.2/src/sflkit/color.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.1/src/sflkit/config.py` & `sflkit-0.2.2/src/sflkit/config.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.1/src/sflkit/instrumentation/__init__.py` & `sflkit-0.2.2/src/sflkit/instrumentation/__init__.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.1/src/sflkit/instrumentation/dir_instrumentation.py` & `sflkit-0.2.2/src/sflkit/instrumentation/dir_instrumentation.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.1/src/sflkit/language/finder.py` & `sflkit-0.2.2/src/sflkit/language/finder.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.1/src/sflkit/language/language.py` & `sflkit-0.2.2/src/sflkit/language/language.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.1/src/sflkit/language/meta.py` & `sflkit-0.2.2/src/sflkit/language/meta.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.1/src/sflkit/language/python/extract.py` & `sflkit-0.2.2/src/sflkit/language/python/extract.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.1/src/sflkit/language/python/factory.py` & `sflkit-0.2.2/src/sflkit/language/python/factory.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.1/src/sflkit/language/python/finder.py` & `sflkit-0.2.2/src/sflkit/language/python/finder.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.1/src/sflkit/language/python/visitor.py` & `sflkit-0.2.2/src/sflkit/language/python/visitor.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.1/src/sflkit/language/visitor.py` & `sflkit-0.2.2/src/sflkit/language/visitor.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.1/src/sflkit/model/event_file.py` & `sflkit-0.2.2/src/sflkit/model/event_file.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.1/src/sflkit/model/model.py` & `sflkit-0.2.2/src/sflkit/model/model.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.1/src/sflkit/model/scope.py` & `sflkit-0.2.2/src/sflkit/model/scope.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.1/src/sflkit/runners/run.py` & `sflkit-0.2.2/src/sflkit/runners/run.py`

 * *Files 10% similar despite different names*

```diff
@@ -234,7 +234,46 @@
                 return TestResult.UNDEFINED
         else:
             return TestResult.UNDEFINED
 
 
 class UnittestRunner(Runner):
     pass
+
+
+class InputRunner(Runner):
+    def __init__(
+        self,
+        access: os.PathLike,
+        passing: List[str | List[str]],
+        failing: List[str | List[str]],
+    ):
+        super().__init__()
+        self.access = access
+        self.passing: Dict[str, List[str]] = self._prepare_tests(passing, "passing")
+        self.failing: Dict[str, List[str]] = self._prepare_tests(failing, "failing")
+
+    @staticmethod
+    def _prepare_tests(tests: List[str | List[str]], prefix: str):
+        return {
+            f"{prefix}_{i}": (test if isinstance(test, list) else test.split("\n"))
+            for i, test in enumerate(tests)
+        }
+
+    def get_tests(self, directory: Path, environ: Environment = None) -> List[str]:
+        return list(self.passing.keys()) + list(self.failing.keys())
+
+    def run_test(
+        self, directory: Path, test: str, environ: Environment = None
+    ) -> TestResult:
+        if "passing" in test:
+            test = self.passing[test]
+            result = TestResult.PASSING
+        else:
+            test = self.failing[test]
+            result = TestResult.FAILING
+        subprocess.run(
+            ["python", "-m", self.access] + test,
+            env=environ,
+            cwd=directory,
+        )
+        return result
```

### Comparing `sflkit-0.2.1/tests/test_analysis_objects.py` & `sflkit-0.2.2/tests/test_analysis_objects.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.1/tests/test_cli.py` & `sflkit-0.2.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.1/tests/test_color.py` & `sflkit-0.2.2/tests/test_color.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.1/tests/test_config.py` & `sflkit-0.2.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.1/tests/test_events.py` & `sflkit-0.2.2/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.1/tests/test_execution.py` & `sflkit-0.2.2/tests/test_execution.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.1/tests/test_instrumentation.py` & `sflkit-0.2.2/tests/test_instrumentation.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.1/tests/test_language.py` & `sflkit-0.2.2/tests/test_language.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.1/tests/test_predicates.py` & `sflkit-0.2.2/tests/test_predicates.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.1/tests/test_runner.py` & `sflkit-0.2.2/tests/test_runner.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 import os
 from pathlib import Path
 
 from sflkit import Config, instrument_config, Analyzer
 from sflkit.analysis.analysis_type import AnalysisType
 from sflkit.analysis.suggestion import Location
 from sflkit.model import EventFile
-from sflkit.runners.run import PytestTree, Package, Module, Function, PytestRunner
+from sflkit.runners.run import (
+    PytestTree,
+    Package,
+    Module,
+    Function,
+    PytestRunner,
+    InputRunner,
+)
 from tests.utils import BaseTest
 
 
 class RunnerTests(BaseTest):
     PYTEST_COLLECT = (
         "================================================================================================"
         "============================= test session starts =============================================="
@@ -138,7 +145,49 @@
         )
         analyzer.analyze()
         predicates = analyzer.get_analysis_by_type(AnalysisType.LINE)
         suggestions = sorted(map(lambda p: p.get_suggestion(), predicates))
         self.assertEqual(1, suggestions[-1].suspiciousness)
         self.assertEqual(1, len(suggestions[-1].lines))
         self.assertEqual(Location("middle.py", 7), suggestions[-1].lines[0])
+
+    def test_input_runner(self):
+        config = Config.create(
+            path=os.path.join(self.TEST_RESOURCES, BaseTest.TEST_SUGGESTIONS),
+            language="python",
+            events="line",
+            predicates="line",
+            working=BaseTest.TEST_DIR,
+            exclude="tests",
+        )
+        instrument_config(config)
+        runner = InputRunner(
+            "main.py",
+            failing=[["2", "1", "3"]],
+            passing=[["3", "2", "1"], ["3", "1", "2"]],
+        )
+        output = Path(BaseTest.TEST_DIR, "events").absolute()
+        runner.run(Path(BaseTest.TEST_DIR), output)
+        self.assertPathExists(output)
+        self.assertPathExists(output / "passing")
+        self.assertPathExists(output / "failing")
+        self.assertPathExists(output / "undefined")
+        analyzer = Analyzer(
+            [
+                EventFile(
+                    output / "failing" / os.listdir(output / "failing")[0],
+                    0,
+                    failing=True,
+                )
+            ],
+            [
+                EventFile(output / "passing" / path, run_id)
+                for run_id, path in enumerate(os.listdir(output / "passing"), start=1)
+            ],
+            config.factory,
+        )
+        analyzer.analyze()
+        predicates = analyzer.get_analysis_by_type(AnalysisType.LINE)
+        suggestions = sorted(map(lambda p: p.get_suggestion(), predicates))
+        self.assertEqual(1, suggestions[-1].suspiciousness)
+        self.assertEqual(1, len(suggestions[-1].lines))
+        self.assertEqual(Location("main.py", 10), suggestions[-1].lines[0])
```

### Comparing `sflkit-0.2.1/tests/test_scope.py` & `sflkit-0.2.2/tests/test_scope.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.1/tests/test_spectra.py` & `sflkit-0.2.2/tests/test_spectra.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.1/tests/test_suggestions.py` & `sflkit-0.2.2/tests/test_suggestions.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.1/tests/test_visitors.py` & `sflkit-0.2.2/tests/test_visitors.py`

 * *Files identical despite different names*

