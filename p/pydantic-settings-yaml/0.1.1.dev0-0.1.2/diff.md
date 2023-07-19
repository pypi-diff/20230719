# Comparing `tmp/pydantic_settings_yaml-0.1.1.dev0.tar.gz` & `tmp/pydantic_settings_yaml-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_settings_yaml-0.1.1.dev0.tar", last modified: Mon Aug  1 07:55:59 2022, max compression
+gzip compressed data, was "pydantic_settings_yaml-0.1.2.tar", last modified: Wed Jul 19 13:14:04 2023, max compression
```

## Comparing `pydantic_settings_yaml-0.1.1.dev0.tar` & `pydantic_settings_yaml-0.1.2.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 07:55:59.057127 pydantic_settings_yaml-0.1.1.dev0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 07:55:59.057127 pydantic_settings_yaml-0.1.1.dev0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 07:55:59.057127 pydantic_settings_yaml-0.1.1.dev0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      454 2022-08-01 07:55:49.000000 pydantic_settings_yaml-0.1.1.dev0/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1348 2022-08-01 07:55:49.000000 pydantic_settings_yaml-0.1.1.dev0/.github/workflows/test_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1807 2022-08-01 07:55:49.000000 pydantic_settings_yaml-0.1.1.dev0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      324 2022-08-01 07:55:49.000000 pydantic_settings_yaml-0.1.1.dev0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-08-01 07:55:49.000000 pydantic_settings_yaml-0.1.1.dev0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1075 2022-08-01 07:55:49.000000 pydantic_settings_yaml-0.1.1.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-08-01 07:55:49.000000 pydantic_settings_yaml-0.1.1.dev0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1328 2022-08-01 07:55:59.057127 pydantic_settings_yaml-0.1.1.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-08-01 07:55:49.000000 pydantic_settings_yaml-0.1.1.dev0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-08-01 07:55:49.000000 pydantic_settings_yaml-0.1.1.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-08-01 07:55:49.000000 pydantic_settings_yaml-0.1.1.dev0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)      268 2022-08-01 07:55:59.057127 pydantic_settings_yaml-0.1.1.dev0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 07:55:59.057127 pydantic_settings_yaml-0.1.1.dev0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 07:55:59.057127 pydantic_settings_yaml-0.1.1.dev0/src/pydantic_settings_yaml/
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-08-01 07:55:49.000000 pydantic_settings_yaml-0.1.1.dev0/src/pydantic_settings_yaml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2762 2022-08-01 07:55:49.000000 pydantic_settings_yaml-0.1.1.dev0/src/pydantic_settings_yaml/base_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 07:55:59.057127 pydantic_settings_yaml-0.1.1.dev0/src/pydantic_settings_yaml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1328 2022-08-01 07:55:59.000000 pydantic_settings_yaml-0.1.1.dev0/src/pydantic_settings_yaml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      679 2022-08-01 07:55:59.000000 pydantic_settings_yaml-0.1.1.dev0/src/pydantic_settings_yaml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-01 07:55:59.000000 pydantic_settings_yaml-0.1.1.dev0/src/pydantic_settings_yaml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-08-01 07:55:59.000000 pydantic_settings_yaml-0.1.1.dev0/src/pydantic_settings_yaml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-08-01 07:55:59.000000 pydantic_settings_yaml-0.1.1.dev0/src/pydantic_settings_yaml.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 07:55:59.057127 pydantic_settings_yaml-0.1.1.dev0/src/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-01 07:55:49.000000 pydantic_settings_yaml-0.1.1.dev0/src/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 07:55:59.057127 pydantic_settings_yaml-0.1.1.dev0/src/tests/data/
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-08-01 07:55:49.000000 pydantic_settings_yaml-0.1.1.dev0/src/tests/data/config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-08-01 07:55:49.000000 pydantic_settings_yaml-0.1.1.dev0/src/tests/data/database_password
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-08-01 07:55:49.000000 pydantic_settings_yaml-0.1.1.dev0/src/tests/data/database_username
--rw-r--r--   0 runner    (1001) docker     (121)     2862 2022-08-01 07:55:49.000000 pydantic_settings_yaml-0.1.1.dev0/src/tests/test_base_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-08-01 07:55:49.000000 pydantic_settings_yaml-0.1.1.dev0/test_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:14:04.460728 pydantic_settings_yaml-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:14:04.456728 pydantic_settings_yaml-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:14:04.460728 pydantic_settings_yaml-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-19 13:13:52.000000 pydantic_settings_yaml-0.1.2/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-19 13:13:52.000000 pydantic_settings_yaml-0.1.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-19 13:13:52.000000 pydantic_settings_yaml-0.1.2/.github/workflows/test_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-19 13:13:52.000000 pydantic_settings_yaml-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-19 13:13:52.000000 pydantic_settings_yaml-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-19 13:13:52.000000 pydantic_settings_yaml-0.1.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-19 13:13:52.000000 pydantic_settings_yaml-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-19 13:13:52.000000 pydantic_settings_yaml-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-19 13:14:04.460728 pydantic_settings_yaml-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-19 13:13:52.000000 pydantic_settings_yaml-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-19 13:13:52.000000 pydantic_settings_yaml-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-19 13:13:52.000000 pydantic_settings_yaml-0.1.2/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-19 13:14:04.460728 pydantic_settings_yaml-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:14:04.456728 pydantic_settings_yaml-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:14:04.460728 pydantic_settings_yaml-0.1.2/src/pydantic_settings_yaml/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-19 13:13:52.000000 pydantic_settings_yaml-0.1.2/src/pydantic_settings_yaml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-07-19 13:13:52.000000 pydantic_settings_yaml-0.1.2/src/pydantic_settings_yaml/base_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:14:04.460728 pydantic_settings_yaml-0.1.2/src/pydantic_settings_yaml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-19 13:14:04.000000 pydantic_settings_yaml-0.1.2/src/pydantic_settings_yaml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-19 13:14:04.000000 pydantic_settings_yaml-0.1.2/src/pydantic_settings_yaml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 13:14:04.000000 pydantic_settings_yaml-0.1.2/src/pydantic_settings_yaml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-19 13:14:04.000000 pydantic_settings_yaml-0.1.2/src/pydantic_settings_yaml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-19 13:14:04.000000 pydantic_settings_yaml-0.1.2/src/pydantic_settings_yaml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:14:04.460728 pydantic_settings_yaml-0.1.2/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 13:13:52.000000 pydantic_settings_yaml-0.1.2/src/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:14:04.460728 pydantic_settings_yaml-0.1.2/src/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-19 13:13:52.000000 pydantic_settings_yaml-0.1.2/src/tests/data/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-19 13:13:52.000000 pydantic_settings_yaml-0.1.2/src/tests/data/database_password
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-19 13:13:52.000000 pydantic_settings_yaml-0.1.2/src/tests/data/database_username
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-19 13:13:52.000000 pydantic_settings_yaml-0.1.2/src/tests/test_base_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-19 13:13:52.000000 pydantic_settings_yaml-0.1.2/test_requirements.txt
```

### Comparing `pydantic_settings_yaml-0.1.1.dev0/.github/workflows/test_and_publish.yml` & `pydantic_settings_yaml-0.1.2/.github/workflows/test_and_publish.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 name: test_and_publish
 
 on:
   push:
-    branches: [ main ]
     tags: [ '*' ]
     paths:
       - 'src/**'
       - './github/workflows/test_and_publish.yaml'
-  pull_request:
-    branches: [ main ]
 
 jobs:
-  test:
+  test_before_publish:
     name: Test on Python ${{ matrix.python_version }}
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python_version: ['3.7', '3.8', '3.9']
     steps:
     - uses: actions/checkout@v2
@@ -30,15 +27,15 @@
     - name: Test with pytest
       run: |
         python -m pytest
   publish:
     name: Build and publish on PyPI
     if: startsWith(github.ref, 'refs/tags')
     runs-on: ubuntu-latest
-    needs: test
+    needs: test_before_publish
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python 3.8
       uses: actions/setup-python@v2
       with:
         python-version: 3.8
     - name: install build
```

### Comparing `pydantic_settings_yaml-0.1.1.dev0/.gitignore` & `pydantic_settings_yaml-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pydantic_settings_yaml-0.1.1.dev0/LICENSE` & `pydantic_settings_yaml-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_settings_yaml-0.1.1.dev0/PKG-INFO` & `pydantic_settings_yaml-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic_settings_yaml
-Version: 0.1.1.dev0
+Version: 0.1.2
 Summary: Yaml support for Pydantic settings
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pydantic-settings-yaml
```

### Comparing `pydantic_settings_yaml-0.1.1.dev0/README.md` & `pydantic_settings_yaml-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_settings_yaml-0.1.1.dev0/src/pydantic_settings_yaml/base_settings.py` & `pydantic_settings_yaml-0.1.2/src/pydantic_settings_yaml/base_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import yaml
 from pydantic import BaseSettings
 
 
 def replace_secrets(secrets_dir: Path, data: str) -> str:
     """
     Replace "<file:xxxx>" secrets in given data
+
     """
     pattern = re.compile(r"\<file\:([^>]*)\>")
 
     for match in pattern.findall(data):
         relpath = Path(match)
         path = secrets_dir / relpath
```

### Comparing `pydantic_settings_yaml-0.1.1.dev0/src/pydantic_settings_yaml.egg-info/PKG-INFO` & `pydantic_settings_yaml-0.1.2/src/pydantic_settings_yaml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-settings-yaml
-Version: 0.1.1.dev0
+Version: 0.1.2
 Summary: Yaml support for Pydantic settings
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pydantic-settings-yaml
```

### Comparing `pydantic_settings_yaml-0.1.1.dev0/src/pydantic_settings_yaml.egg-info/SOURCES.txt` & `pydantic_settings_yaml-0.1.2/src/pydantic_settings_yaml.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 MANIFEST.in
 README.md
 pyproject.toml
 pytest.ini
 setup.cfg
 test_requirements.txt
 .github/workflows/lint.yml
+.github/workflows/test.yml
 .github/workflows/test_and_publish.yml
 src/pydantic_settings_yaml/__init__.py
 src/pydantic_settings_yaml/base_settings.py
 src/pydantic_settings_yaml.egg-info/PKG-INFO
 src/pydantic_settings_yaml.egg-info/SOURCES.txt
 src/pydantic_settings_yaml.egg-info/dependency_links.txt
 src/pydantic_settings_yaml.egg-info/requires.txt
```

### Comparing `pydantic_settings_yaml-0.1.1.dev0/src/tests/test_base_settings.py` & `pydantic_settings_yaml-0.1.2/src/tests/test_base_settings.py`

 * *Files identical despite different names*

