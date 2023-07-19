# Comparing `tmp/zimran-events-0.3.0.tar.gz` & `tmp/zimran-events-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zimran-events-0.3.0.tar", last modified: Wed Jul 12 12:39:04 2023, max compression
+gzip compressed data, was "zimran-events-0.3.1.tar", last modified: Wed Jul 19 08:30:34 2023, max compression
```

## Comparing `zimran-events-0.3.0.tar` & `zimran-events-0.3.1.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:39:04.041852 zimran-events-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-12 12:38:56.000000 zimran-events-0.3.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-12 12:38:56.000000 zimran-events-0.3.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-12 12:38:56.000000 zimran-events-0.3.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:39:04.041852 zimran-events-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:39:04.041852 zimran-events-0.3.0/.github/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-07-12 12:38:56.000000 zimran-events-0.3.0/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:39:04.041852 zimran-events-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-12 12:38:56.000000 zimran-events-0.3.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-12 12:38:56.000000 zimran-events-0.3.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-07-12 12:38:56.000000 zimran-events-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-12 12:38:56.000000 zimran-events-0.3.0/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-12 12:38:56.000000 zimran-events-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-12 12:38:56.000000 zimran-events-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-07-12 12:39:04.041852 zimran-events-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-12 12:38:56.000000 zimran-events-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-07-12 12:38:56.000000 zimran-events-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-12 12:38:56.000000 zimran-events-0.3.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 12:39:04.041852 zimran-events-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:39:04.041852 zimran-events-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-12 12:38:56.000000 zimran-events-0.3.0/tests/test_legacy_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-12 12:38:56.000000 zimran-events-0.3.0/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:39:04.041852 zimran-events-0.3.0/zimran/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:39:04.041852 zimran-events-0.3.0/zimran/events/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-12 12:38:56.000000 zimran-events-0.3.0/zimran/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-07-12 12:38:56.000000 zimran-events-0.3.0/zimran/events/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-12 12:38:56.000000 zimran-events-0.3.0/zimran/events/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-07-12 12:38:56.000000 zimran-events-0.3.0/zimran/events/consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-12 12:38:56.000000 zimran-events-0.3.0/zimran/events/dto.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-12 12:38:56.000000 zimran-events-0.3.0/zimran/events/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-12 12:38:56.000000 zimran-events-0.3.0/zimran/events/producer.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-12 12:38:56.000000 zimran-events-0.3.0/zimran/events/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-12 12:38:56.000000 zimran-events-0.3.0/zimran/events/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:39:04.041852 zimran-events-0.3.0/zimran_events.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-07-12 12:39:04.000000 zimran-events-0.3.0/zimran_events.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-12 12:39:04.000000 zimran-events-0.3.0/zimran_events.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 12:39:04.000000 zimran-events-0.3.0/zimran_events.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-12 12:39:04.000000 zimran-events-0.3.0/zimran_events.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-12 12:39:04.000000 zimran-events-0.3.0/zimran_events.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:30:34.700029 zimran-events-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-19 08:30:21.000000 zimran-events-0.3.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-19 08:30:21.000000 zimran-events-0.3.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-19 08:30:21.000000 zimran-events-0.3.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:30:34.696029 zimran-events-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:30:34.700029 zimran-events-0.3.1/.github/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-07-19 08:30:21.000000 zimran-events-0.3.1/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:30:34.700029 zimran-events-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-19 08:30:21.000000 zimran-events-0.3.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-19 08:30:21.000000 zimran-events-0.3.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-07-19 08:30:21.000000 zimran-events-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-19 08:30:21.000000 zimran-events-0.3.1/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-19 08:30:21.000000 zimran-events-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-19 08:30:21.000000 zimran-events-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-07-19 08:30:34.700029 zimran-events-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-19 08:30:21.000000 zimran-events-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-07-19 08:30:21.000000 zimran-events-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-19 08:30:21.000000 zimran-events-0.3.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 08:30:34.700029 zimran-events-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:30:34.700029 zimran-events-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-19 08:30:21.000000 zimran-events-0.3.1/tests/test_legacy_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-19 08:30:21.000000 zimran-events-0.3.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:30:34.696029 zimran-events-0.3.1/zimran/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:30:34.700029 zimran-events-0.3.1/zimran/events/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-19 08:30:21.000000 zimran-events-0.3.1/zimran/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-07-19 08:30:21.000000 zimran-events-0.3.1/zimran/events/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-19 08:30:21.000000 zimran-events-0.3.1/zimran/events/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-07-19 08:30:21.000000 zimran-events-0.3.1/zimran/events/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-19 08:30:21.000000 zimran-events-0.3.1/zimran/events/dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-19 08:30:21.000000 zimran-events-0.3.1/zimran/events/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-07-19 08:30:21.000000 zimran-events-0.3.1/zimran/events/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-19 08:30:21.000000 zimran-events-0.3.1/zimran/events/producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-19 08:30:21.000000 zimran-events-0.3.1/zimran/events/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-19 08:30:21.000000 zimran-events-0.3.1/zimran/events/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:30:34.700029 zimran-events-0.3.1/zimran_events.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-07-19 08:30:34.000000 zimran-events-0.3.1/zimran_events.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-19 08:30:34.000000 zimran-events-0.3.1/zimran_events.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 08:30:34.000000 zimran-events-0.3.1/zimran_events.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-19 08:30:34.000000 zimran-events-0.3.1/zimran_events.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-19 08:30:34.000000 zimran-events-0.3.1/zimran_events.egg-info/top_level.txt
```

### Comparing `zimran-events-0.3.0/.github/scripts/release.py` & `zimran-events-0.3.1/.github/scripts/release.py`

 * *Files identical despite different names*

### Comparing `zimran-events-0.3.0/.github/workflows/publish.yml` & `zimran-events-0.3.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `zimran-events-0.3.0/.gitignore` & `zimran-events-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `zimran-events-0.3.0/.pre-commit-config.yaml` & `zimran-events-0.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `zimran-events-0.3.0/LICENSE` & `zimran-events-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zimran-events-0.3.0/PKG-INFO` & `zimran-events-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zimran-events
-Version: 0.3.0
+Version: 0.3.1
 Summary: The zimran-events provides amqp interface
 Author-email: Talgat Abdraimov <abdraimov.talga@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Talgat Abdraimov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `zimran-events-0.3.0/README.md` & `zimran-events-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `zimran-events-0.3.0/pyproject.toml` & `zimran-events-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.4.0", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zimran-events"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
   { name="Talgat Abdraimov", email="abdraimov.talga@gmail.com" },
 ]
 description = "The zimran-events provides amqp interface"
 readme = "README.md"
 requires-python = ">=3.10"
 license = { file = "LICENSE" }
```

### Comparing `zimran-events-0.3.0/tests/test_utils.py` & `zimran-events-0.3.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `zimran-events-0.3.0/zimran/events/connection.py` & `zimran-events-0.3.1/zimran/events/connection.py`

 * *Files identical despite different names*

### Comparing `zimran-events-0.3.0/zimran/events/consumer.py` & `zimran-events-0.3.1/zimran/events/consumer.py`

 * *Files identical despite different names*

### Comparing `zimran-events-0.3.0/zimran/events/dto.py` & `zimran-events-0.3.1/zimran/events/dto.py`

 * *Files identical despite different names*

### Comparing `zimran-events-0.3.0/zimran/events/producer.py` & `zimran-events-0.3.1/zimran/events/producer.py`

 * *Files identical despite different names*

### Comparing `zimran-events-0.3.0/zimran/events/utils.py` & `zimran-events-0.3.1/zimran/events/utils.py`

 * *Files identical despite different names*

### Comparing `zimran-events-0.3.0/zimran_events.egg-info/PKG-INFO` & `zimran-events-0.3.1/zimran_events.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zimran-events
-Version: 0.3.0
+Version: 0.3.1
 Summary: The zimran-events provides amqp interface
 Author-email: Talgat Abdraimov <abdraimov.talga@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Talgat Abdraimov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `zimran-events-0.3.0/zimran_events.egg-info/SOURCES.txt` & `zimran-events-0.3.1/zimran_events.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 tests/test_utils.py
 zimran/events/__init__.py
 zimran/events/connection.py
 zimran/events/constants.py
 zimran/events/consumer.py
 zimran/events/dto.py
 zimran/events/exceptions.py
+zimran/events/patterns.py
 zimran/events/producer.py
 zimran/events/schemas.py
 zimran/events/utils.py
 zimran_events.egg-info/PKG-INFO
 zimran_events.egg-info/SOURCES.txt
 zimran_events.egg-info/dependency_links.txt
 zimran_events.egg-info/requires.txt
```

