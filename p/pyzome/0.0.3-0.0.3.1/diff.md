# Comparing `tmp/pyzome-0.0.3.tar.gz` & `tmp/pyzome-0.0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyzome-0.0.3.tar", last modified: Tue Jul 11 13:40:22 2023, max compression
+gzip compressed data, was "pyzome-0.0.3.1.tar", last modified: Wed Jul 19 15:36:58 2023, max compression
```

## Comparing `pyzome-0.0.3.tar` & `pyzome-0.0.3.1.tar`

### file list

```diff
@@ -1,64 +1,63 @@
-drwxr-xr-x   0 zdl       (1000) zdl       (1000)        0 2023-07-11 13:40:22.812980 pyzome-0.0.3/
--rw-r--r--   0 zdl       (1000) zdl       (1000)      178 2023-07-11 13:12:44.000000 pyzome-0.0.3/.codecov.yml
--rw-r--r--   0 zdl       (1000) zdl       (1000)      211 2023-07-11 13:12:44.000000 pyzome-0.0.3/.coveragerc
--rw-r--r--   0 zdl       (1000) zdl       (1000)       32 2023-07-11 13:12:44.000000 pyzome-0.0.3/.gitattributes
-drwxr-xr-x   0 zdl       (1000) zdl       (1000)        0 2023-07-11 13:40:22.804980 pyzome-0.0.3/.github/
-drwxr-xr-x   0 zdl       (1000) zdl       (1000)        0 2023-07-11 13:40:22.808980 pyzome-0.0.3/.github/workflows/
--rw-r--r--   0 zdl       (1000) zdl       (1000)     1093 2023-07-11 13:12:44.000000 pyzome-0.0.3/.github/workflows/ci_tests.yml
--rw-r--r--   0 zdl       (1000) zdl       (1000)      904 2023-07-11 13:12:44.000000 pyzome-0.0.3/.gitignore
--rw-r--r--   0 zdl       (1000) zdl       (1000)      824 2023-07-11 13:12:44.000000 pyzome-0.0.3/.readthedocs.yaml
--rw-r--r--   0 zdl       (1000) zdl       (1000)      155 2023-07-11 13:12:44.000000 pyzome-0.0.3/AUTHORS.rst
--rw-r--r--   0 zdl       (1000) zdl       (1000)     3021 2023-07-11 13:12:44.000000 pyzome-0.0.3/CONTRIBUTING.rst
--rw-r--r--   0 zdl       (1000) zdl       (1000)     1527 2023-07-11 13:12:44.000000 pyzome-0.0.3/LICENSE
--rw-r--r--   0 zdl       (1000) zdl       (1000)      359 2023-07-11 13:12:44.000000 pyzome-0.0.3/MANIFEST.in
--rw-r--r--   0 zdl       (1000) zdl       (1000)     2990 2023-07-11 13:40:22.808980 pyzome-0.0.3/PKG-INFO
--rw-r--r--   0 zdl       (1000) zdl       (1000)     2215 2023-07-11 13:12:44.000000 pyzome-0.0.3/README.rst
-drwxr-xr-x   0 zdl       (1000) zdl       (1000)        0 2023-07-11 13:40:22.808980 pyzome-0.0.3/docs/
--rw-r--r--   0 zdl       (1000) zdl       (1000)      638 2023-07-11 13:12:44.000000 pyzome-0.0.3/docs/Makefile
--rw-r--r--   0 zdl       (1000) zdl       (1000)      804 2023-07-11 13:12:44.000000 pyzome-0.0.3/docs/make.bat
--rw-r--r--   0 zdl       (1000) zdl       (1000)        8 2023-07-11 13:12:44.000000 pyzome-0.0.3/docs/requirements.txt
-drwxr-xr-x   0 zdl       (1000) zdl       (1000)        0 2023-07-11 13:40:22.808980 pyzome-0.0.3/docs/source/
--rw-r--r--   0 zdl       (1000) zdl       (1000)      612 2023-07-11 13:12:44.000000 pyzome-0.0.3/docs/source/basic.rst
--rw-r--r--   0 zdl       (1000) zdl       (1000)     1008 2023-07-11 13:12:44.000000 pyzome-0.0.3/docs/source/conf.py
--rw-r--r--   0 zdl       (1000) zdl       (1000)      554 2023-07-11 13:12:44.000000 pyzome-0.0.3/docs/source/index.rst
--rw-r--r--   0 zdl       (1000) zdl       (1000)      716 2023-07-11 13:12:44.000000 pyzome-0.0.3/docs/source/install.rst
--rw-r--r--   0 zdl       (1000) zdl       (1000)     1861 2023-07-11 13:12:44.000000 pyzome-0.0.3/docs/source/intro.rst
--rw-r--r--   0 zdl       (1000) zdl       (1000)      479 2023-07-11 13:12:44.000000 pyzome-0.0.3/docs/source/mock_data.rst
--rw-r--r--   0 zdl       (1000) zdl       (1000)      524 2023-07-11 13:12:44.000000 pyzome-0.0.3/docs/source/qglogp.rst
--rw-r--r--   0 zdl       (1000) zdl       (1000)      263 2023-07-11 13:12:44.000000 pyzome-0.0.3/docs/source/recipes.rst
--rw-r--r--   0 zdl       (1000) zdl       (1000)      249 2023-07-11 13:12:44.000000 pyzome-0.0.3/docs/source/tem.rst
--rw-r--r--   0 zdl       (1000) zdl       (1000)     1442 2023-07-11 13:12:44.000000 pyzome-0.0.3/docs/source/zonal_waves.rst
--rw-r--r--   0 zdl       (1000) zdl       (1000)      946 2023-07-11 13:39:22.000000 pyzome-0.0.3/pyproject.toml
-drwxr-xr-x   0 zdl       (1000) zdl       (1000)        0 2023-07-11 13:40:22.808980 pyzome-0.0.3/pyzome/
--rw-r--r--   0 zdl       (1000) zdl       (1000)      113 2023-07-11 13:39:18.000000 pyzome-0.0.3/pyzome/__init__.py
--rw-r--r--   0 zdl       (1000) zdl       (1000)      211 2023-07-11 13:12:44.000000 pyzome-0.0.3/pyzome/_version.py
--rw-r--r--   0 zdl       (1000) zdl       (1000)     3400 2023-07-11 13:12:44.000000 pyzome-0.0.3/pyzome/basic.py
--rw-r--r--   0 zdl       (1000) zdl       (1000)     8459 2023-07-11 13:12:44.000000 pyzome-0.0.3/pyzome/checks.py
--rw-r--r--   0 zdl       (1000) zdl       (1000)      419 2023-07-11 13:12:44.000000 pyzome-0.0.3/pyzome/constants.py
--rw-r--r--   0 zdl       (1000) zdl       (1000)      885 2023-07-11 13:12:44.000000 pyzome-0.0.3/pyzome/exceptions.py
--rw-r--r--   0 zdl       (1000) zdl       (1000)    10416 2023-07-11 13:12:44.000000 pyzome-0.0.3/pyzome/mock_data.py
--rw-r--r--   0 zdl       (1000) zdl       (1000)    14437 2023-07-11 13:12:44.000000 pyzome-0.0.3/pyzome/qglogp.py
-drwxr-xr-x   0 zdl       (1000) zdl       (1000)        0 2023-07-11 13:40:22.808980 pyzome-0.0.3/pyzome/recipes/
--rw-r--r--   0 zdl       (1000) zdl       (1000)       19 2023-07-11 13:12:44.000000 pyzome-0.0.3/pyzome/recipes/__init__.py
--rw-r--r--   0 zdl       (1000) zdl       (1000)     7050 2023-07-11 13:12:44.000000 pyzome-0.0.3/pyzome/recipes/zmd.py
--rw-r--r--   0 zdl       (1000) zdl       (1000)    12525 2023-07-11 13:12:44.000000 pyzome-0.0.3/pyzome/tem.py
--rw-r--r--   0 zdl       (1000) zdl       (1000)    15427 2023-07-11 13:12:44.000000 pyzome-0.0.3/pyzome/zonal_waves.py
-drwxr-xr-x   0 zdl       (1000) zdl       (1000)        0 2023-07-11 13:40:22.808980 pyzome-0.0.3/pyzome.egg-info/
--rw-r--r--   0 zdl       (1000) zdl       (1000)     2990 2023-07-11 13:40:22.000000 pyzome-0.0.3/pyzome.egg-info/PKG-INFO
--rw-r--r--   0 zdl       (1000) zdl       (1000)     1059 2023-07-11 13:40:22.000000 pyzome-0.0.3/pyzome.egg-info/SOURCES.txt
--rw-r--r--   0 zdl       (1000) zdl       (1000)        1 2023-07-11 13:40:22.000000 pyzome-0.0.3/pyzome.egg-info/dependency_links.txt
--rw-r--r--   0 zdl       (1000) zdl       (1000)       24 2023-07-11 13:40:22.000000 pyzome-0.0.3/pyzome.egg-info/requires.txt
--rw-r--r--   0 zdl       (1000) zdl       (1000)        7 2023-07-11 13:40:22.000000 pyzome-0.0.3/pyzome.egg-info/top_level.txt
--rw-r--r--   0 zdl       (1000) zdl       (1000)      323 2023-07-11 13:12:44.000000 pyzome-0.0.3/requirements-dev.txt
--rw-r--r--   0 zdl       (1000) zdl       (1000)       76 2023-07-11 13:12:44.000000 pyzome-0.0.3/requirements.txt
--rw-r--r--   0 zdl       (1000) zdl       (1000)       38 2023-07-11 13:40:22.812980 pyzome-0.0.3/setup.cfg
--rw-r--r--   0 zdl       (1000) zdl       (1000)       69 2023-07-11 13:12:44.000000 pyzome-0.0.3/setup.py
-drwxr-xr-x   0 zdl       (1000) zdl       (1000)        0 2023-07-11 13:40:22.808980 pyzome-0.0.3/tests/
--rw-r--r--   0 zdl       (1000) zdl       (1000)        0 2023-07-11 13:12:44.000000 pyzome-0.0.3/tests/__init__.py
--rw-r--r--   0 zdl       (1000) zdl       (1000)     1932 2023-07-11 13:12:44.000000 pyzome-0.0.3/tests/test_basic.py
--rw-r--r--   0 zdl       (1000) zdl       (1000)     5751 2023-07-11 13:12:44.000000 pyzome-0.0.3/tests/test_checks.py
--rw-r--r--   0 zdl       (1000) zdl       (1000)    10830 2023-07-11 13:12:44.000000 pyzome-0.0.3/tests/test_mock_data.py
--rw-r--r--   0 zdl       (1000) zdl       (1000)     4844 2023-07-11 13:12:44.000000 pyzome-0.0.3/tests/test_qglogp.py
--rw-r--r--   0 zdl       (1000) zdl       (1000)     2964 2023-07-11 13:12:44.000000 pyzome-0.0.3/tests/test_recipes_zmd.py
--rw-r--r--   0 zdl       (1000) zdl       (1000)     2848 2023-07-11 13:12:44.000000 pyzome-0.0.3/tests/test_tem.py
--rw-r--r--   0 zdl       (1000) zdl       (1000)    13473 2023-07-11 13:12:44.000000 pyzome-0.0.3/tests/test_zonal_waves.py
+drwxr-xr-x   0 zdl       (1000) zdl       (1000)        0 2023-07-19 15:36:58.890442 pyzome-0.0.3.1/
+-rw-r--r--   0 zdl       (1000) zdl       (1000)      178 2023-07-19 14:52:51.000000 pyzome-0.0.3.1/.codecov.yml
+-rw-r--r--   0 zdl       (1000) zdl       (1000)      211 2023-07-19 14:52:51.000000 pyzome-0.0.3.1/.coveragerc
+-rw-r--r--   0 zdl       (1000) zdl       (1000)       32 2023-07-19 14:52:51.000000 pyzome-0.0.3.1/.gitattributes
+drwxr-xr-x   0 zdl       (1000) zdl       (1000)        0 2023-07-19 15:36:58.886442 pyzome-0.0.3.1/.github/
+drwxr-xr-x   0 zdl       (1000) zdl       (1000)        0 2023-07-19 15:36:58.886442 pyzome-0.0.3.1/.github/workflows/
+-rw-r--r--   0 zdl       (1000) zdl       (1000)     1093 2023-07-19 14:52:51.000000 pyzome-0.0.3.1/.github/workflows/ci_tests.yml
+-rw-r--r--   0 zdl       (1000) zdl       (1000)      904 2023-07-19 14:52:51.000000 pyzome-0.0.3.1/.gitignore
+-rw-r--r--   0 zdl       (1000) zdl       (1000)      824 2023-07-19 14:52:51.000000 pyzome-0.0.3.1/.readthedocs.yaml
+-rw-r--r--   0 zdl       (1000) zdl       (1000)      155 2023-07-19 14:52:51.000000 pyzome-0.0.3.1/AUTHORS.rst
+-rw-r--r--   0 zdl       (1000) zdl       (1000)     3021 2023-07-19 14:52:51.000000 pyzome-0.0.3.1/CONTRIBUTING.rst
+-rw-r--r--   0 zdl       (1000) zdl       (1000)     1527 2023-07-19 14:52:51.000000 pyzome-0.0.3.1/LICENSE
+-rw-r--r--   0 zdl       (1000) zdl       (1000)      359 2023-07-19 14:52:51.000000 pyzome-0.0.3.1/MANIFEST.in
+-rw-r--r--   0 zdl       (1000) zdl       (1000)     3093 2023-07-19 15:36:58.890442 pyzome-0.0.3.1/PKG-INFO
+-rw-r--r--   0 zdl       (1000) zdl       (1000)     2316 2023-07-19 14:52:51.000000 pyzome-0.0.3.1/README.rst
+drwxr-xr-x   0 zdl       (1000) zdl       (1000)        0 2023-07-19 15:36:58.886442 pyzome-0.0.3.1/docs/
+-rw-r--r--   0 zdl       (1000) zdl       (1000)      638 2023-07-19 14:52:51.000000 pyzome-0.0.3.1/docs/Makefile
+-rw-r--r--   0 zdl       (1000) zdl       (1000)      804 2023-07-19 14:52:51.000000 pyzome-0.0.3.1/docs/make.bat
+-rw-r--r--   0 zdl       (1000) zdl       (1000)        8 2023-07-19 14:52:51.000000 pyzome-0.0.3.1/docs/requirements.txt
+drwxr-xr-x   0 zdl       (1000) zdl       (1000)        0 2023-07-19 15:36:58.890442 pyzome-0.0.3.1/docs/source/
+-rw-r--r--   0 zdl       (1000) zdl       (1000)      612 2023-07-19 14:52:51.000000 pyzome-0.0.3.1/docs/source/basic.rst
+-rw-r--r--   0 zdl       (1000) zdl       (1000)     1008 2023-07-19 14:52:51.000000 pyzome-0.0.3.1/docs/source/conf.py
+-rw-r--r--   0 zdl       (1000) zdl       (1000)      554 2023-07-19 14:52:51.000000 pyzome-0.0.3.1/docs/source/index.rst
+-rw-r--r--   0 zdl       (1000) zdl       (1000)      743 2023-07-19 14:52:51.000000 pyzome-0.0.3.1/docs/source/install.rst
+-rw-r--r--   0 zdl       (1000) zdl       (1000)     1861 2023-07-19 14:52:51.000000 pyzome-0.0.3.1/docs/source/intro.rst
+-rw-r--r--   0 zdl       (1000) zdl       (1000)      479 2023-07-19 14:52:51.000000 pyzome-0.0.3.1/docs/source/mock_data.rst
+-rw-r--r--   0 zdl       (1000) zdl       (1000)      524 2023-07-19 14:52:51.000000 pyzome-0.0.3.1/docs/source/qglogp.rst
+-rw-r--r--   0 zdl       (1000) zdl       (1000)      263 2023-07-19 14:52:51.000000 pyzome-0.0.3.1/docs/source/recipes.rst
+-rw-r--r--   0 zdl       (1000) zdl       (1000)      249 2023-07-19 14:52:51.000000 pyzome-0.0.3.1/docs/source/tem.rst
+-rw-r--r--   0 zdl       (1000) zdl       (1000)     1442 2023-07-19 14:52:51.000000 pyzome-0.0.3.1/docs/source/zonal_waves.rst
+-rw-r--r--   0 zdl       (1000) zdl       (1000)      949 2023-07-19 15:15:18.000000 pyzome-0.0.3.1/pyproject.toml
+drwxr-xr-x   0 zdl       (1000) zdl       (1000)        0 2023-07-19 15:36:58.890442 pyzome-0.0.3.1/pyzome/
+-rw-r--r--   0 zdl       (1000) zdl       (1000)      115 2023-07-19 15:02:18.000000 pyzome-0.0.3.1/pyzome/__init__.py
+-rw-r--r--   0 zdl       (1000) zdl       (1000)     3400 2023-07-19 14:52:51.000000 pyzome-0.0.3.1/pyzome/basic.py
+-rw-r--r--   0 zdl       (1000) zdl       (1000)     8491 2023-07-19 15:30:52.000000 pyzome-0.0.3.1/pyzome/checks.py
+-rw-r--r--   0 zdl       (1000) zdl       (1000)      419 2023-07-19 14:52:51.000000 pyzome-0.0.3.1/pyzome/constants.py
+-rw-r--r--   0 zdl       (1000) zdl       (1000)      885 2023-07-19 14:52:51.000000 pyzome-0.0.3.1/pyzome/exceptions.py
+-rw-r--r--   0 zdl       (1000) zdl       (1000)    10416 2023-07-19 14:52:51.000000 pyzome-0.0.3.1/pyzome/mock_data.py
+-rw-r--r--   0 zdl       (1000) zdl       (1000)    14437 2023-07-19 14:52:51.000000 pyzome-0.0.3.1/pyzome/qglogp.py
+drwxr-xr-x   0 zdl       (1000) zdl       (1000)        0 2023-07-19 15:36:58.890442 pyzome-0.0.3.1/pyzome/recipes/
+-rw-r--r--   0 zdl       (1000) zdl       (1000)       19 2023-07-19 14:52:51.000000 pyzome-0.0.3.1/pyzome/recipes/__init__.py
+-rw-r--r--   0 zdl       (1000) zdl       (1000)     7050 2023-07-19 14:52:51.000000 pyzome-0.0.3.1/pyzome/recipes/zmd.py
+-rw-r--r--   0 zdl       (1000) zdl       (1000)    12525 2023-07-19 14:52:51.000000 pyzome-0.0.3.1/pyzome/tem.py
+-rw-r--r--   0 zdl       (1000) zdl       (1000)    15427 2023-07-19 14:52:51.000000 pyzome-0.0.3.1/pyzome/zonal_waves.py
+drwxr-xr-x   0 zdl       (1000) zdl       (1000)        0 2023-07-19 15:36:58.890442 pyzome-0.0.3.1/pyzome.egg-info/
+-rw-r--r--   0 zdl       (1000) zdl       (1000)     3093 2023-07-19 15:36:58.000000 pyzome-0.0.3.1/pyzome.egg-info/PKG-INFO
+-rw-r--r--   0 zdl       (1000) zdl       (1000)     1040 2023-07-19 15:36:58.000000 pyzome-0.0.3.1/pyzome.egg-info/SOURCES.txt
+-rw-r--r--   0 zdl       (1000) zdl       (1000)        1 2023-07-19 15:36:58.000000 pyzome-0.0.3.1/pyzome.egg-info/dependency_links.txt
+-rw-r--r--   0 zdl       (1000) zdl       (1000)       24 2023-07-19 15:36:58.000000 pyzome-0.0.3.1/pyzome.egg-info/requires.txt
+-rw-r--r--   0 zdl       (1000) zdl       (1000)        7 2023-07-19 15:36:58.000000 pyzome-0.0.3.1/pyzome.egg-info/top_level.txt
+-rw-r--r--   0 zdl       (1000) zdl       (1000)      323 2023-07-19 14:52:51.000000 pyzome-0.0.3.1/requirements-dev.txt
+-rw-r--r--   0 zdl       (1000) zdl       (1000)       76 2023-07-19 14:52:51.000000 pyzome-0.0.3.1/requirements.txt
+-rw-r--r--   0 zdl       (1000) zdl       (1000)       38 2023-07-19 15:36:58.890442 pyzome-0.0.3.1/setup.cfg
+-rw-r--r--   0 zdl       (1000) zdl       (1000)       69 2023-07-19 14:52:51.000000 pyzome-0.0.3.1/setup.py
+drwxr-xr-x   0 zdl       (1000) zdl       (1000)        0 2023-07-19 15:36:58.890442 pyzome-0.0.3.1/tests/
+-rw-r--r--   0 zdl       (1000) zdl       (1000)        0 2023-07-19 14:52:51.000000 pyzome-0.0.3.1/tests/__init__.py
+-rw-r--r--   0 zdl       (1000) zdl       (1000)     1932 2023-07-19 14:52:51.000000 pyzome-0.0.3.1/tests/test_basic.py
+-rw-r--r--   0 zdl       (1000) zdl       (1000)     5751 2023-07-19 15:29:40.000000 pyzome-0.0.3.1/tests/test_checks.py
+-rw-r--r--   0 zdl       (1000) zdl       (1000)    10830 2023-07-19 14:52:51.000000 pyzome-0.0.3.1/tests/test_mock_data.py
+-rw-r--r--   0 zdl       (1000) zdl       (1000)     4844 2023-07-19 14:52:51.000000 pyzome-0.0.3.1/tests/test_qglogp.py
+-rw-r--r--   0 zdl       (1000) zdl       (1000)     2964 2023-07-19 14:52:51.000000 pyzome-0.0.3.1/tests/test_recipes_zmd.py
+-rw-r--r--   0 zdl       (1000) zdl       (1000)     2848 2023-07-19 14:52:51.000000 pyzome-0.0.3.1/tests/test_tem.py
+-rw-r--r--   0 zdl       (1000) zdl       (1000)    13473 2023-07-19 14:52:51.000000 pyzome-0.0.3.1/tests/test_zonal_waves.py
```

### Comparing `pyzome-0.0.3/.github/workflows/ci_tests.yml` & `pyzome-0.0.3.1/.github/workflows/ci_tests.yml`

 * *Files identical despite different names*

### Comparing `pyzome-0.0.3/.gitignore` & `pyzome-0.0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pyzome-0.0.3/.readthedocs.yaml` & `pyzome-0.0.3.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pyzome-0.0.3/CONTRIBUTING.rst` & `pyzome-0.0.3.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pyzome-0.0.3/LICENSE` & `pyzome-0.0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyzome-0.0.3/PKG-INFO` & `pyzome-0.0.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyzome
-Version: 0.0.3
+Version: 0.0.3.1
 Summary: A collection of tools for computing zonal mean and other related atmospheric circulation diagnostics
 Author-email: "Zachary D. Lawrence" <zachary.lawrence@colorado.edu>
 License: BSD-3-Clause
 Project-URL: Source Code, https://github.com/zdlawrence/pyzome
 Project-URL: Bug Tracker, https://github.com/zdlawrence/pyzome/issues
 Keywords: meteorology,physics
 Classifier: Development Status :: 3 - Alpha
@@ -38,14 +38,20 @@
 It is designed to be used in conjunction with xarray for enabling coordinate- and 
 unit-aware computations. 
 
 pyzome is in an early stage and currently under active development. While much of 
 the core functionality is in place, the API (e.g., function names and call 
 signatures) is still subject to change.
 
+Install
+-------
+pyzome is available on PyPI and can be installed with pip::
+
+    pip install pyzome
+
 
 Features
 --------
 - zonal and meridional mean computations
 - zonal wavenumber decompositions of fields; zonal wave covariances between 2 fields
 - Transformed Eulerian Mean (TEM) diagnostics, such as EP-fluxes and residual velocities
 - quasi-geostrophic diagnostics, such as meridional QGPV gradients and the refractive index
```

### Comparing `pyzome-0.0.3/README.rst` & `pyzome-0.0.3.1/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,20 @@
 It is designed to be used in conjunction with xarray for enabling coordinate- and 
 unit-aware computations. 
 
 pyzome is in an early stage and currently under active development. While much of 
 the core functionality is in place, the API (e.g., function names and call 
 signatures) is still subject to change.
 
+Install
+-------
+pyzome is available on PyPI and can be installed with pip::
+
+    pip install pyzome
+
 
 Features
 --------
 - zonal and meridional mean computations
 - zonal wavenumber decompositions of fields; zonal wave covariances between 2 fields
 - Transformed Eulerian Mean (TEM) diagnostics, such as EP-fluxes and residual velocities
 - quasi-geostrophic diagnostics, such as meridional QGPV gradients and the refractive index
```

### Comparing `pyzome-0.0.3/docs/Makefile` & `pyzome-0.0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyzome-0.0.3/docs/make.bat` & `pyzome-0.0.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyzome-0.0.3/docs/source/basic.rst` & `pyzome-0.0.3.1/docs/source/basic.rst`

 * *Files identical despite different names*

### Comparing `pyzome-0.0.3/docs/source/conf.py` & `pyzome-0.0.3.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pyzome-0.0.3/docs/source/index.rst` & `pyzome-0.0.3.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pyzome-0.0.3/docs/source/install.rst` & `pyzome-0.0.3.1/docs/source/install.rst`

 * *Files 27% similar despite different names*

```diff
@@ -8,20 +8,22 @@
 
 ``pyzome`` currently only requires `numpy <http://www.numpy.org/>`__, 
 `scipy <https://www.scipy.org/>`__, `xarray <http://xarray.pydata.org/en/stable/>`__, 
 and `xrft <https://xrft.readthedocs.io/en/latest/>`__.
 
 Installation
 ------------
+``pyzome`` can be installed using ``pip``::
 
-``pyzome`` is not yet available on PyPI, but it can be
-installed by cloning its Github repository (or downloading the 
-source code) and running::
+    pip install pyzome
+
+Alternatively it can be installed by cloning the Github repository 
+(or downloading the source code) and running::
 
     python setup.py install
 
-in the top-level pyzome directory. Alternatively, you can use pip 
+in the top-level pyzome directory. You can also use pip 
 to install from the cloned/source directory with::
 
     pip install -e .
 
 This will install ``pyzome`` in your current Python environment.
```

### Comparing `pyzome-0.0.3/docs/source/intro.rst` & `pyzome-0.0.3.1/docs/source/intro.rst`

 * *Files identical despite different names*

### Comparing `pyzome-0.0.3/docs/source/qglogp.rst` & `pyzome-0.0.3.1/docs/source/qglogp.rst`

 * *Files identical despite different names*

### Comparing `pyzome-0.0.3/docs/source/zonal_waves.rst` & `pyzome-0.0.3.1/docs/source/zonal_waves.rst`

 * *Files identical despite different names*

### Comparing `pyzome-0.0.3/pyproject.toml` & `pyzome-0.0.3.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=45", "wheel", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyzome"
-version = "0.0.3"
+version = "0.0.3.1"
 authors = [
     {name = "Zachary D. Lawrence", email = "zachary.lawrence@colorado.edu"},
 ]
 description = "A collection of tools for computing zonal mean and other related atmospheric circulation diagnostics"
 readme = "README.rst"
 requires-python = ">=3.8"
 keywords = ["meteorology", "physics"]
@@ -26,8 +26,8 @@
     "scipy",
     "xarray",
     "xrft",
 ]
 
 [project.urls]
 "Source Code" = "https://github.com/zdlawrence/pyzome"
-"Bug Tracker" = "https://github.com/zdlawrence/pyzome/issues"
+"Bug Tracker" = "https://github.com/zdlawrence/pyzome/issues"
```

### Comparing `pyzome-0.0.3/pyzome/basic.py` & `pyzome-0.0.3.1/pyzome/basic.py`

 * *Files identical despite different names*

### Comparing `pyzome-0.0.3/pyzome/checks.py` & `pyzome-0.0.3.1/pyzome/checks.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     dlon = float(lons[1] - lons[0])
 
     # check that all the longitude differences are close to
     # the single dlon, to within 1.0e-3 degrees
     equal_spacing = np.allclose(np.diff(lons), dlon, rtol=0.0, atol=1.0e-3)
 
     # now check that the span+londelta cover 360 degrees
-    full_span = (span + dlon) >= 360.0
+    full_span = np.allclose(span + dlon, 360.0, rtol=0.0, atol=1.0e-3)
 
     if (enforce is True) and (equal_spacing is False):
         msg = "longitudes are not equally spaced"
         raise LongitudeError(msg)
     elif (enforce is True) and (full_span is False):
         msg = "longitudes do not span all 360 degrees"
         raise LongitudeError(msg)
```

### Comparing `pyzome-0.0.3/pyzome/exceptions.py` & `pyzome-0.0.3.1/pyzome/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyzome-0.0.3/pyzome/mock_data.py` & `pyzome-0.0.3.1/pyzome/mock_data.py`

 * *Files identical despite different names*

### Comparing `pyzome-0.0.3/pyzome/qglogp.py` & `pyzome-0.0.3.1/pyzome/qglogp.py`

 * *Files identical despite different names*

### Comparing `pyzome-0.0.3/pyzome/recipes/zmd.py` & `pyzome-0.0.3.1/pyzome/recipes/zmd.py`

 * *Files identical despite different names*

### Comparing `pyzome-0.0.3/pyzome/tem.py` & `pyzome-0.0.3.1/pyzome/tem.py`

 * *Files identical despite different names*

### Comparing `pyzome-0.0.3/pyzome/zonal_waves.py` & `pyzome-0.0.3.1/pyzome/zonal_waves.py`

 * *Files identical despite different names*

### Comparing `pyzome-0.0.3/pyzome.egg-info/PKG-INFO` & `pyzome-0.0.3.1/pyzome.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyzome
-Version: 0.0.3
+Version: 0.0.3.1
 Summary: A collection of tools for computing zonal mean and other related atmospheric circulation diagnostics
 Author-email: "Zachary D. Lawrence" <zachary.lawrence@colorado.edu>
 License: BSD-3-Clause
 Project-URL: Source Code, https://github.com/zdlawrence/pyzome
 Project-URL: Bug Tracker, https://github.com/zdlawrence/pyzome/issues
 Keywords: meteorology,physics
 Classifier: Development Status :: 3 - Alpha
@@ -38,14 +38,20 @@
 It is designed to be used in conjunction with xarray for enabling coordinate- and 
 unit-aware computations. 
 
 pyzome is in an early stage and currently under active development. While much of 
 the core functionality is in place, the API (e.g., function names and call 
 signatures) is still subject to change.
 
+Install
+-------
+pyzome is available on PyPI and can be installed with pip::
+
+    pip install pyzome
+
 
 Features
 --------
 - zonal and meridional mean computations
 - zonal wavenumber decompositions of fields; zonal wave covariances between 2 fields
 - Transformed Eulerian Mean (TEM) diagnostics, such as EP-fluxes and residual velocities
 - quasi-geostrophic diagnostics, such as meridional QGPV gradients and the refractive index
```

### Comparing `pyzome-0.0.3/pyzome.egg-info/SOURCES.txt` & `pyzome-0.0.3.1/pyzome.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 docs/source/intro.rst
 docs/source/mock_data.rst
 docs/source/qglogp.rst
 docs/source/recipes.rst
 docs/source/tem.rst
 docs/source/zonal_waves.rst
 pyzome/__init__.py
-pyzome/_version.py
 pyzome/basic.py
 pyzome/checks.py
 pyzome/constants.py
 pyzome/exceptions.py
 pyzome/mock_data.py
 pyzome/qglogp.py
 pyzome/tem.py
```

### Comparing `pyzome-0.0.3/tests/test_basic.py` & `pyzome-0.0.3.1/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `pyzome-0.0.3/tests/test_checks.py` & `pyzome-0.0.3.1/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `pyzome-0.0.3/tests/test_mock_data.py` & `pyzome-0.0.3.1/tests/test_mock_data.py`

 * *Files identical despite different names*

### Comparing `pyzome-0.0.3/tests/test_qglogp.py` & `pyzome-0.0.3.1/tests/test_qglogp.py`

 * *Files identical despite different names*

### Comparing `pyzome-0.0.3/tests/test_recipes_zmd.py` & `pyzome-0.0.3.1/tests/test_recipes_zmd.py`

 * *Files identical despite different names*

### Comparing `pyzome-0.0.3/tests/test_tem.py` & `pyzome-0.0.3.1/tests/test_tem.py`

 * *Files identical despite different names*

### Comparing `pyzome-0.0.3/tests/test_zonal_waves.py` & `pyzome-0.0.3.1/tests/test_zonal_waves.py`

 * *Files identical despite different names*

