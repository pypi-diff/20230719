# Comparing `tmp/pipeln-0.1.0.tar.gz` & `tmp/pipeln-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipeln-0.1.0.tar", last modified: Thu Jul 28 00:02:13 2022, max compression
+gzip compressed data, was "pipeln-0.2.0.tar", last modified: Tue Jul 18 22:09:45 2023, max compression
```

## Comparing `pipeln-0.1.0.tar` & `pipeln-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 00:02:13.791506 pipeln-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1075 2022-07-28 00:01:58.000000 pipeln-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1240 2022-07-28 00:02:13.791506 pipeln-0.1.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 00:02:13.791506 pipeln-0.1.0/Pipeln/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-28 00:01:58.000000 pipeln-0.1.0/Pipeln/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2379 2022-07-28 00:01:58.000000 pipeln-0.1.0/Pipeln/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (121)      965 2022-07-28 00:01:58.000000 pipeln-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 00:02:13.791506 pipeln-0.1.0/pipeln.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1240 2022-07-28 00:02:13.000000 pipeln-0.1.0/pipeln.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      213 2022-07-28 00:02:13.000000 pipeln-0.1.0/pipeln.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-28 00:02:13.000000 pipeln-0.1.0/pipeln.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-07-28 00:02:13.000000 pipeln-0.1.0/pipeln.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-07-28 00:02:13.000000 pipeln-0.1.0/pipeln.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-28 00:02:13.791506 pipeln-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      705 2022-07-28 00:01:58.000000 pipeln-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:09:45.567151 pipeln-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-18 22:09:33.000000 pipeln-0.2.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-18 22:09:33.000000 pipeln-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-18 22:09:33.000000 pipeln-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-18 22:09:45.567151 pipeln-0.2.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:09:45.567151 pipeln-0.2.0/Pipeln/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-18 22:09:33.000000 pipeln-0.2.0/Pipeln/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-18 22:09:33.000000 pipeln-0.2.0/Pipeln/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-07-18 22:09:33.000000 pipeln-0.2.0/Pipeln/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-07-18 22:09:33.000000 pipeln-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:09:45.567151 pipeln-0.2.0/pipeln.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-18 22:09:45.000000 pipeln-0.2.0/pipeln.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-18 22:09:45.000000 pipeln-0.2.0/pipeln.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 22:09:45.000000 pipeln-0.2.0/pipeln.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-18 22:09:45.000000 pipeln-0.2.0/pipeln.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 22:09:33.000000 pipeln-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 22:09:45.567151 pipeln-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-18 22:09:33.000000 pipeln-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:09:45.567151 pipeln-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-18 22:09:33.000000 pipeln-0.2.0/tests/test_pipeline.py
```

### Comparing `pipeln-0.1.0/LICENSE` & `pipeln-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pipeln-0.1.0/setup.py` & `pipeln-0.2.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,29 @@
+import os
+
+# Use the VERSION file to get Pipeln version
+version_file = os.path.join(os.path.dirname(__file__), "Pipeln", "VERSION")
+with open(version_file) as fh:
+    pipeln_version = fh.read().strip()
+
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     LONG_DESC = fh.read()
 
     setup(
         long_description=LONG_DESC,
         long_description_content_type='text/markdown',
         name='pipeln',
         packages=find_packages(include=['Pipeln']),
-        version='0.1.0',
-        description='A package to create a custom pipeline',
+        version=pipeln_version,
+        description='A Python package to create a custom pipeline',
         author='Adrián H.S',
         author_email='adrihs.dev@gmail.com',
         license='MIT',
-        install_requires=['pandas', 'numpy'],
+        install_requires=[],
         setup_requires=['pytest-runner'],
         url='https://github.com/Adri-Hdez/Pipeln',
         tests_require=['pytest'],
         test_suite='tests',
         include_package_data=True,
-)
+    )
```

