# Comparing `tmp/meent-0.9.3.tar.gz` & `tmp/meent-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meent-0.9.3.tar", last modified: Mon Jul 17 06:20:29 2023, max compression
+gzip compressed data, was "meent-0.9.4.tar", last modified: Wed Jul 19 12:56:19 2023, max compression
```

## Comparing `meent-0.9.3.tar` & `meent-0.9.4.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:29.113585 meent-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-17 06:20:15.000000 meent-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-17 06:20:29.113585 meent-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-07-17 06:20:15.000000 meent-0.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:29.105585 meent-0.9.3/meent/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-17 06:20:15.000000 meent-0.9.3/meent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-07-17 06:20:15.000000 meent-0.9.3/meent/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:29.105585 meent-0.9.3/meent/nk_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:29.105585 meent-0.9.3/meent/nk_data/filmetrics/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-17 06:20:15.000000 meent-0.9.3/meent/nk_data/filmetrics/Al2O3.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-07-17 06:20:15.000000 meent-0.9.3/meent/nk_data/filmetrics/Si.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-07-17 06:20:15.000000 meent-0.9.3/meent/nk_data/filmetrics/Si3N4.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-07-17 06:20:15.000000 meent-0.9.3/meent/nk_data/filmetrics/SiO2.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:29.105585 meent-0.9.3/meent/nk_data/matlab/
--rw-r--r--   0 runner    (1001) docker     (123)    11222 2023-07-17 06:20:15.000000 meent-0.9.3/meent/nk_data/matlab/p_Si.mat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:29.105585 meent-0.9.3/meent/on_jax/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_jax/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:29.109585 meent-0.9.3/meent/on_jax/emsolver/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_jax/emsolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16856 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_jax/emsolver/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_jax/emsolver/convolution_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    38784 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_jax/emsolver/field_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_jax/emsolver/primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)    14059 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_jax/emsolver/rcwa.py
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_jax/emsolver/scattering_method.py
--rw-r--r--   0 runner    (1001) docker     (123)    10546 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_jax/emsolver/smm_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    14577 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_jax/emsolver/transfer_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_jax/mee.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:29.109585 meent-0.9.3/meent/on_jax/modeler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_jax/modeler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_jax/modeler/modeling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:29.109585 meent-0.9.3/meent/on_jax/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_jax/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_jax/optimizer/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_jax/optimizer/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:29.109585 meent-0.9.3/meent/on_numpy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_numpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:29.109585 meent-0.9.3/meent/on_numpy/emsolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_numpy/emsolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14816 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_numpy/emsolver/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_numpy/emsolver/convolution_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    27387 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_numpy/emsolver/field_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_numpy/emsolver/rcwa.py
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_numpy/emsolver/scattering_method.py
--rw-r--r--   0 runner    (1001) docker     (123)    10530 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_numpy/emsolver/smm_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_numpy/emsolver/transfer_method.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_numpy/mee.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:29.109585 meent-0.9.3/meent/on_numpy/modeler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_numpy/modeler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_numpy/modeler/modeling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:29.109585 meent-0.9.3/meent/on_torch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:29.113585 meent-0.9.3/meent/on_torch/emsolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_torch/emsolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18452 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_torch/emsolver/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    20183 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_torch/emsolver/convolution_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    29243 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_torch/emsolver/field_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_torch/emsolver/primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)    11864 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_torch/emsolver/rcwa.py
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_torch/emsolver/scattering_method.py
--rw-r--r--   0 runner    (1001) docker     (123)    10516 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_torch/emsolver/smm_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    14085 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_torch/emsolver/transfer_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_torch/mee.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:29.113585 meent-0.9.3/meent/on_torch/modeler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_torch/modeler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15839 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_torch/modeler/modeling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:29.113585 meent-0.9.3/meent/on_torch/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_torch/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_torch/optimizer/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-17 06:20:15.000000 meent-0.9.3/meent/on_torch/optimizer/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:29.105585 meent-0.9.3/meent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-17 06:20:29.000000 meent-0.9.3/meent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-17 06:20:29.000000 meent-0.9.3/meent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 06:20:29.000000 meent-0.9.3/meent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-17 06:20:29.000000 meent-0.9.3/meent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-17 06:20:29.000000 meent-0.9.3/meent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 06:20:29.113585 meent-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-17 06:20:15.000000 meent-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:19.286350 meent-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-19 12:56:01.000000 meent-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-19 12:56:19.286350 meent-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-07-19 12:56:01.000000 meent-0.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:19.270350 meent-0.9.4/meent/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-19 12:56:01.000000 meent-0.9.4/meent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-07-19 12:56:01.000000 meent-0.9.4/meent/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:19.270350 meent-0.9.4/meent/nk_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:19.274350 meent-0.9.4/meent/nk_data/filmetrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-19 12:56:01.000000 meent-0.9.4/meent/nk_data/filmetrics/Al2O3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-07-19 12:56:01.000000 meent-0.9.4/meent/nk_data/filmetrics/Si.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-07-19 12:56:01.000000 meent-0.9.4/meent/nk_data/filmetrics/Si3N4.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-07-19 12:56:01.000000 meent-0.9.4/meent/nk_data/filmetrics/SiO2.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:19.274350 meent-0.9.4/meent/nk_data/matlab/
+-rw-r--r--   0 runner    (1001) docker     (123)    11222 2023-07-19 12:56:01.000000 meent-0.9.4/meent/nk_data/matlab/p_Si.mat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:19.274350 meent-0.9.4/meent/on_jax/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_jax/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:19.278350 meent-0.9.4/meent/on_jax/emsolver/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_jax/emsolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16856 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_jax/emsolver/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_jax/emsolver/convolution_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38784 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_jax/emsolver/field_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_jax/emsolver/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14059 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_jax/emsolver/rcwa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_jax/emsolver/scattering_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10546 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_jax/emsolver/smm_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14577 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_jax/emsolver/transfer_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_jax/mee.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:19.278350 meent-0.9.4/meent/on_jax/modeler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_jax/modeler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_jax/modeler/modeling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:19.278350 meent-0.9.4/meent/on_jax/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_jax/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_jax/optimizer/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_jax/optimizer/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:19.278350 meent-0.9.4/meent/on_numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_numpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:19.278350 meent-0.9.4/meent/on_numpy/emsolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_numpy/emsolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14816 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_numpy/emsolver/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_numpy/emsolver/convolution_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27387 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_numpy/emsolver/field_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_numpy/emsolver/rcwa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_numpy/emsolver/scattering_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10530 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_numpy/emsolver/smm_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_numpy/emsolver/transfer_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_numpy/mee.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:19.282350 meent-0.9.4/meent/on_numpy/modeler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_numpy/modeler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_numpy/modeler/modeling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:19.282350 meent-0.9.4/meent/on_torch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:19.286350 meent-0.9.4/meent/on_torch/emsolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_torch/emsolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18452 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_torch/emsolver/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20183 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_torch/emsolver/convolution_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29243 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_torch/emsolver/field_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_torch/emsolver/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11864 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_torch/emsolver/rcwa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_torch/emsolver/scattering_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10516 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_torch/emsolver/smm_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14085 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_torch/emsolver/transfer_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_torch/mee.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:19.286350 meent-0.9.4/meent/on_torch/modeler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_torch/modeler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15628 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_torch/modeler/modeling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:19.286350 meent-0.9.4/meent/on_torch/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_torch/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_torch/optimizer/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-19 12:56:01.000000 meent-0.9.4/meent/on_torch/optimizer/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:19.274350 meent-0.9.4/meent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-19 12:56:19.000000 meent-0.9.4/meent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-19 12:56:19.000000 meent-0.9.4/meent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 12:56:19.000000 meent-0.9.4/meent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-19 12:56:19.000000 meent-0.9.4/meent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-19 12:56:19.000000 meent-0.9.4/meent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 12:56:19.286350 meent-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-19 12:56:01.000000 meent-0.9.4/setup.py
```

### Comparing `meent-0.9.3/LICENSE` & `meent-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `meent-0.9.3/README.md` & `meent-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `meent-0.9.3/meent/main.py` & `meent-0.9.4/meent/main.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.3/meent/nk_data/filmetrics/Al2O3.txt` & `meent-0.9.4/meent/nk_data/filmetrics/Al2O3.txt`

 * *Files identical despite different names*

### Comparing `meent-0.9.3/meent/nk_data/filmetrics/Si.txt` & `meent-0.9.4/meent/nk_data/filmetrics/Si.txt`

 * *Files identical despite different names*

### Comparing `meent-0.9.3/meent/nk_data/filmetrics/Si3N4.txt` & `meent-0.9.4/meent/nk_data/filmetrics/Si3N4.txt`

 * *Files identical despite different names*

### Comparing `meent-0.9.3/meent/nk_data/filmetrics/SiO2.txt` & `meent-0.9.4/meent/nk_data/filmetrics/SiO2.txt`

 * *Files identical despite different names*

### Comparing `meent-0.9.3/meent/nk_data/matlab/p_Si.mat` & `meent-0.9.4/meent/nk_data/matlab/p_Si.mat`

 * *Files identical despite different names*

### Comparing `meent-0.9.3/meent/on_jax/emsolver/_base.py` & `meent-0.9.4/meent/on_jax/emsolver/_base.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.3/meent/on_jax/emsolver/convolution_matrix.py` & `meent-0.9.4/meent/on_jax/emsolver/convolution_matrix.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.3/meent/on_jax/emsolver/field_distribution.py` & `meent-0.9.4/meent/on_jax/emsolver/field_distribution.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.3/meent/on_jax/emsolver/primitives.py` & `meent-0.9.4/meent/on_jax/emsolver/primitives.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.3/meent/on_jax/emsolver/rcwa.py` & `meent-0.9.4/meent/on_jax/emsolver/rcwa.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.3/meent/on_jax/emsolver/scattering_method.py` & `meent-0.9.4/meent/on_jax/emsolver/scattering_method.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.3/meent/on_jax/emsolver/smm_util.py` & `meent-0.9.4/meent/on_jax/emsolver/smm_util.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.3/meent/on_jax/emsolver/transfer_method.py` & `meent-0.9.4/meent/on_jax/emsolver/transfer_method.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.3/meent/on_jax/mee.py` & `meent-0.9.4/meent/on_jax/mee.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.3/meent/on_jax/modeler/modeling.py` & `meent-0.9.4/meent/on_jax/modeler/modeling.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.3/meent/on_jax/optimizer/loss.py` & `meent-0.9.4/meent/on_jax/optimizer/loss.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.3/meent/on_jax/optimizer/optimizer.py` & `meent-0.9.4/meent/on_jax/optimizer/optimizer.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.3/meent/on_numpy/emsolver/_base.py` & `meent-0.9.4/meent/on_numpy/emsolver/_base.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.3/meent/on_numpy/emsolver/convolution_matrix.py` & `meent-0.9.4/meent/on_numpy/emsolver/convolution_matrix.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.3/meent/on_numpy/emsolver/field_distribution.py` & `meent-0.9.4/meent/on_numpy/emsolver/field_distribution.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.3/meent/on_numpy/emsolver/rcwa.py` & `meent-0.9.4/meent/on_numpy/emsolver/rcwa.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.3/meent/on_numpy/emsolver/scattering_method.py` & `meent-0.9.4/meent/on_numpy/emsolver/scattering_method.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.3/meent/on_numpy/emsolver/smm_util.py` & `meent-0.9.4/meent/on_numpy/emsolver/smm_util.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.3/meent/on_numpy/emsolver/transfer_method.py` & `meent-0.9.4/meent/on_numpy/emsolver/transfer_method.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.3/meent/on_numpy/mee.py` & `meent-0.9.4/meent/on_numpy/mee.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.3/meent/on_numpy/modeler/modeling.py` & `meent-0.9.4/meent/on_numpy/modeler/modeling.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.3/meent/on_torch/emsolver/_base.py` & `meent-0.9.4/meent/on_torch/emsolver/_base.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.3/meent/on_torch/emsolver/convolution_matrix.py` & `meent-0.9.4/meent/on_torch/emsolver/convolution_matrix.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.3/meent/on_torch/emsolver/field_distribution.py` & `meent-0.9.4/meent/on_torch/emsolver/field_distribution.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.3/meent/on_torch/emsolver/primitives.py` & `meent-0.9.4/meent/on_torch/emsolver/primitives.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.3/meent/on_torch/emsolver/rcwa.py` & `meent-0.9.4/meent/on_torch/emsolver/rcwa.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.3/meent/on_torch/emsolver/scattering_method.py` & `meent-0.9.4/meent/on_torch/emsolver/scattering_method.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.3/meent/on_torch/emsolver/smm_util.py` & `meent-0.9.4/meent/on_torch/emsolver/smm_util.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.3/meent/on_torch/emsolver/transfer_method.py` & `meent-0.9.4/meent/on_torch/emsolver/transfer_method.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.3/meent/on_torch/mee.py` & `meent-0.9.4/meent/on_torch/mee.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.3/meent/on_torch/modeler/modeling.py` & `meent-0.9.4/meent/on_torch/modeler/modeling.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,198 +38,219 @@
         self.mat_table = None
         self.ucell_info_list = None
         self.period = period
 
     @staticmethod
     def rectangle(cx, cy, lx, ly, base):
 
-        a = torch.hstack([cy - ly / 2, cx - lx / 2])
-        b = torch.hstack([cy + ly / 2, cx + lx / 2])
+        a = torch.hstack([cy - ly / 2, cx - lx / 2])  # row, col
+        b = torch.hstack([cy + ly / 2, cx + lx / 2])  # row, col
 
-        points = torch.vstack([a, b])
-
-        res = [[points[0], points[1], base]]
+        res = [[a, b, base]]  # top_left, bottom_right
         return res
 
     def rectangle_rotate(self, cx, cy, lx, ly, dx, dy, base, angle=None, angle_margin=1E-5):
+        ddx, ddy = dx + 2, dy + 2
+
         if angle is None:
             angle = torch.tensor(0 * torch.pi / 180)
 
-        # TODO
         if 0 * torch.pi / 2 - angle_margin <= abs(angle) % (2 * torch.pi) <= 0 * torch.pi / 2 + angle_margin:
-            return self.rectangle(cx, cy, lx, ly, base), [0, 0], [0, 0]
+            return self.rectangle(cx, cy, lx, ly, base)
         elif 1 * torch.pi / 2 - angle_margin <= abs(angle) % (2 * torch.pi) <= 1 * torch.pi / 2 + angle_margin:
-            return self.rectangle(cx, cy, ly, lx, base), [0, 0], [0, 0]
+            return self.rectangle(cx, cy, ly, lx, base)
         elif 2 * torch.pi / 2 - angle_margin <= abs(angle) % (2 * torch.pi) <= 2 * torch.pi / 2 + angle_margin:
-            return self.rectangle(cx, cy, lx, ly, base), [0, 0], [0, 0]
+            return self.rectangle(cx, cy, lx, ly, base)
         elif 3 * torch.pi / 2 - angle_margin <= abs(angle) % (2 * torch.pi) <= 3 * torch.pi / 2 + angle_margin:
-            return self.rectangle(cx, cy, ly, lx, base), [0, 0], [0, 0]
+            return self.rectangle(cx, cy, ly, lx, base)
         else:
             pass
 
-        x_up = (lx / 2).repeat(dx + 2) * torch.linspace(-1, 1, dx + 2)
-        y_up = torch.tensor([ly / 2] * (dx + 2))
-        x_right = torch.tensor([lx / 2] * (dy + 2))
-        y_right = (ly / 2).repeat(dy + 2) * torch.linspace(1, -1, dy + 2)
-        # y_right = (ly / 2).repeat(dy + 2) * torch.linspace(-1, 1, dy + 2)
-        x_left = torch.tensor([-lx / 2] * (dy + 2))
-        y_left = (ly / 2).repeat(dy + 2) * torch.linspace(-1, 1, dy + 2)
-        x_down = (lx / 2).repeat(dx + 2) * torch.linspace(1, 1, dx + 2)
-        # x_down = (lx / 2).repeat(dx + 2) * torch.linspace(-1, -1, dx + 2)
-        y_down = torch.tensor([-ly / 2] * (dx + 2))
+        angle = angle % (2 * torch.pi)
 
         rotate = torch.ones((2, 2), dtype=torch.complex128)
         rotate[0, 0] = torch.cos(angle)
         rotate[0, 1] = -torch.sin(angle)
         rotate[1, 0] = torch.sin(angle)
         rotate[1, 1] = torch.cos(angle)
 
-        UR = rotate @ torch.hstack([lx / 2, ly / 2])
-        RD = rotate @ torch.hstack([lx / 2, -ly / 2])
-        DL = rotate @ torch.hstack([-lx / 2, -ly / 2])
-        LU = rotate @ torch.hstack([-lx / 2, ly / 2])
-
-        UR += torch.tensor([cx, cy])
-        RD += torch.tensor([cx, cy])
-        DL += torch.tensor([cx, cy])
-        LU += torch.tensor([cx, cy])
-
-        p_up = rotate @ torch.vstack((x_up, y_up))
-        p_down = rotate @ torch.vstack((x_down, y_down))
-        p_left = rotate @ torch.vstack((x_left, y_left))
-        p_right = rotate @ torch.vstack((x_right, y_right))
-
-        p_up[0] += cx
-        p_up[1] += cy
-        # p_up[0], p_up[1] = p_up[0] + cx, p_up[1] + cy
-        p_down[0] += cx
-        p_down[1] += cy
-        p_left[0] += cx
-        p_left[1] += cy
-        p_right[0] += cx
-        p_right[1] += cy
-
-        # TODO: negative angle
-        if 0 < (angle / (torch.pi / 180)) % 360 < 90:
-            angle_new = (angle % (2 * torch.pi)) - 0
+        UR = rotate @ torch.vstack([lx / 2, ly / 2])
+        RD = rotate @ torch.vstack([lx / 2, -ly / 2])
+        DL = rotate @ torch.vstack([-lx / 2, -ly / 2])
+        LU = rotate @ torch.vstack([-lx / 2, ly / 2])
+
+        UR += torch.tensor([[cx], [cy]])
+        RD += torch.tensor([[cx], [cy]])
+        DL += torch.tensor([[cx], [cy]])
+        LU += torch.tensor([[cx], [cy]])
+
+        if 0 < angle < torch.pi / 2:
+            angle_inside = (torch.pi / 2) - angle
 
             # trail = L + U
             top1, top4 = UR, DL
-            length_1, length_2 = lx, ly
-            trail = torch.hstack([p_left, p_up])
-            p_out1, p_out2 = p_left, p_up
 
-            if LU[1].real >= RD[1].real:
+            if LU[1].real > RD[1].real:
                 top2, top3 = LU, RD
+                length_top12, length_top24 = lx, ly
+                top2_left = True
             else:
                 top2, top3 = RD, LU
+                length_top12, length_top24 = ly, lx
+                top2_left = False
 
-        elif 90 < (angle / (torch.pi / 180)) % 360 < 180:
-            angle_new = (angle % (2 * torch.pi)) - torch.pi / 2
+        elif torch.pi / 2 < angle < torch.pi:
 
+            angle_inside = torch.pi - angle
             # trail = U + R
             top1, top4 = RD, LU
-            length_1, length_2 = ly, lx
-            trail = torch.hstack([p_up, p_right])
-            p_out1, p_out2 = p_up, p_right
 
-            if UR[1].real >= DL[1].real:
+            if UR[1].real > DL[1].real:
                 top2, top3 = UR, DL
+                length_top12, length_top24 = ly, lx
+                top2_left = True
             else:
                 top2, top3 = DL, UR
+                length_top12, length_top24 = lx, ly
+                top2_left = False
 
-        elif 180 < (angle / (torch.pi / 180)) % 360 < 270:
-            angle_new = (angle % (2 * torch.pi)) - torch.pi
+        elif torch.pi < angle < torch.pi / 2 * 3:
+            angle_inside = (torch.pi * 3 / 2) - angle
 
             # trail = R + D
             top1, top4 = DL, UR
-            length_1, length_2 = lx, ly
-            trail = torch.hstack([p_right, p_down])
-            p_out1, p_out2 = p_right, p_down
 
-            if RD[1].real >= LU[1].real:
+            if RD[1].real > LU[1].real:
                 top2, top3 = RD, LU
+                length_top12, length_top24 = lx, ly
+                top2_left = True
             else:
                 top2, top3 = LU, RD
-        elif 270 < (angle / (torch.pi / 180)) % 360 < 360:
-            angle_new = (angle % (2 * torch.pi)) - torch.pi * 3 / 2
+                length_top12, length_top24 = ly, lx
+                top2_left = False
 
+        elif torch.pi / 2 * 3 < angle < torch.pi * 2:
+            angle_inside = (torch.pi * 2) - angle
             # trail = D + L
             top1, top4 = LU, RD
-            length_1, length_2 = ly, lx
-            trail = torch.hstack([p_down, p_left])
-            p_out1, p_out2 = p_down, p_left
 
-            if DL[1].real >= UR[1].real:
+            if DL[1].real > UR[1].real:
                 top2, top3 = DL, UR
+                length_top12, length_top24 = ly, lx
+                top2_left = True
             else:
                 top2, top3 = UR, DL
+                length_top12, length_top24 = lx, ly
+                top2_left = False
         else:
             raise ValueError
 
-        obj_list = []
+        # point in region 1(top1~top2), 2(top2~top3) and 3(top3~top4)
 
-        trail_couple = []
-        # trail_couple = torch.zeros(trail.shape, dtype=torch.complex128, requires_grad=False)
-        for i, (x, y) in enumerate(zip(*trail)):
-            # if i == trail.shape[1]-1:
-            #     continue
-
-            if top2[1].real < y.real <= top1[1].real:
-                length = ((x - top1[0]) ** 2 + (y - top1[1]) ** 2) ** (1 / 2)
-                length = length / torch.cos(angle_new)
-                xx = x + length
-
-            elif top3[1].real <= y.real <= top2[1].real:
-                if top3[0].real <= top2[0].real:
-                    length = length_2 / abs(torch.sin(angle_new))
-                # elif top3[0].real > top2[0].real:
-                #     length = length_1 / abs(torch.cos(angle_new))
-                else:
-                    length = length_1 / abs(torch.cos(angle_new))
+        xxx, yyy = [], []
+        xxx_cp, yyy_cp = [], []
+        if top2_left:
 
-                # if (x + length).real < trail[0, i+1].real:
-                #     xx = trail[0, i+1]
-                # else:
-                #     xx = x + length
-                xx = x + length
+            length = length_top12 / torch.sin(angle_inside)
+            top3_cp = [top3[0] - length, top3[1]]
 
-            # elif top4[1].real < y.real < top3[1].real:
-            else:
-                length = ((x - top4[0]) ** 2 + (y - top4[1]) ** 2) ** (1 / 2)
+            for i in range(ddx + 1):
+                x = top1[0] - (top1[0] - top2[0]) / ddx * i
+                y = top1[1] - (top1[1] - top2[1]) / ddy * i
+                xxx.append(x)
+                yyy.append(y)
 
-                # TODO: ?? sin and sin?
-                # if 0 < (angle / (torch.pi / 180)) % 360 < 90 or 180 < (angle / (torch.pi / 180)) % 360 < 270:
-                if 0 < (angle / (torch.pi / 180)) % 360 < 90 or 180 < (angle / (torch.pi / 180)) % 360 < 270:
-                    length = length / abs(torch.sin(angle_new))
-                else:
-                    length = length / abs(torch.sin(angle_new))
+                xxx_cp.append(x + length / ddx * i)
+                yyy_cp.append(y)
+
+            for i in range(ddy + 1):
+
+                x = top2[0] + (top3_cp[0] - top2[0]) / ddx * i
+                y = top2[1] - (top2[1] - top3_cp[1]) / ddy * i
+                xxx.append(x)
+                yyy.append(y)
+
+                xxx_cp.append(x + length)
+                yyy_cp.append(y)
+
+            for i in range(ddx + 1):
+                x = top3_cp[0] + (top4[0] - top3_cp[0]) / ddx * i
+                y = top3_cp[1] - (top3_cp[1] - top4[1]) / ddy * i
+                xxx.append(x)
+                yyy.append(y)
+
+                xxx_cp.append(x + length / ddx * (ddx - i))
+                yyy_cp.append(y)
+
+            obj_list1 = []
+
+            for i in range(len(xxx)):
+                if i == len(xxx) - 1:
+                    break
+                x, y = xxx[i], yyy[i]
+                x_cp, y_cp = xxx_cp[i], yyy_cp[i]
+
+                x_next, y_next = xxx[i + 1], yyy[i + 1]
+                x_cp_next, y_cp_next = xxx_cp[i + 1], yyy_cp[i + 1]
+
+                x_mean = (x + x_next) / 2
+                x_cp_mean = (x_cp + x_cp_next) / 2
+                obj_list1.append([[y_cp_next, x_mean], [y, x_cp_mean], base])
+
+            return obj_list1
+
+        else:
+
+            length = length_top12 / torch.cos(angle_inside)
+            top3_cp = [top3[0] + length, top3[1]]
+
+            for i in range(ddx + 1):
+                x = top1[0] + (top2[0] - top1[0]) / ddx * i
+                y = top1[1] - (top1[1] - top2[1]) / ddy * i
+                xxx.append(x)
+                yyy.append(y)
+
+                xxx_cp.append(x - length / ddx * i)
+                yyy_cp.append(y)
+
+            for i in range(ddy + 1):
+
+                x = top2[0] - (top2[0] - top3_cp[0]) / ddx * i
+                y = top2[1] - (top2[1] - top3_cp[1]) / ddy * i
+                xxx.append(x)
+                yyy.append(y)
+
+                xxx_cp.append(x - length)
+                yyy_cp.append(y)
+
+            for i in range(ddx + 1):
+                x = top3_cp[0] - (top3_cp[0] - top4[0]) / ddx * i
+                y = top3_cp[1] - (top3_cp[1] - top4[1]) / ddy * i
+                xxx.append(x)
+                yyy.append(y)
+
+                xxx_cp.append(x - length / ddx * (ddx - i))
+                yyy_cp.append(y)
+
+            obj_list1 = []
+
+            for i in range(len(xxx)):
+                if i == len(xxx) - 1:
+                    break
+                x, y = xxx[i], yyy[i]
+                x_cp, y_cp = xxx_cp[i], yyy_cp[i]
 
-                xx = x + length
+                x_next, y_next = xxx[i + 1], yyy[i + 1]
+                x_cp_next, y_cp_next = xxx_cp[i + 1], yyy_cp[i + 1]
 
-            # y_next = trail[1, i+1]
-            # trail_couple = trail_couple.clone()
-            # trail_couple[0, i] = xx
-            # trail_couple[1, i] = y
-            trail_couple.append([xx, y])
-
-        trail_couple = torch.as_tensor(trail_couple).T
-        for index, (x, y) in enumerate(zip(*trail)):
-            if index == trail.shape[1] - 1:
-                continue
-
-            xx, yy = trail_couple[:, index]
-            x_next, y_next = trail[:, index + 1]
-            xx_next, yy_next = trail_couple[:, index + 1]
-            x_mean = (x_next + x) / 2
-            xx_mean = (xx_next + xx) / 2
-            # obj_list.append([[x_mean, y], [xx_mean, y_next], base])  # tODO
-            obj_list.append([[y, x_mean], [y_next, xx_mean], base])
+                x_mean = (x + x_next) / 2
+                x_cp_mean = (x_cp + x_cp_next) / 2
+                obj_list1.append([[y_cp_next, x_cp_mean], [y, x_mean], base])
 
-        return obj_list, p_out1, p_out2
+            return obj_list1
 
     def ellipse(self, cx, cy, lx, ly, dx, dy, base, rotation_angle=0 * torch.pi / 180):
         points_x = torch.arange(cx-lx, cx+lx, dx+2)
         points_y = torch.arange(cy-ly, cy+ly, dy+2)
 
         rotate = torch.tensor([torch.cos(rotation_angle), -torch.sin(rotation_angle)],
                               [torch.sin(rotation_angle),  torch.cos(rotation_angle)],
@@ -305,18 +326,18 @@
                     col_list.insert(index, bottom_right[1])
                     break
             else:
                 print('WARNING: Overlapping of the objects in modeling is too complicated. Backprop may not work as expected.')
                 index = bisect_left(col_list, bottom_right[1].real, key=lambda x: x.real)
                 col_list.insert(index, bottom_right[1])
 
-        if not row_list or row_list[-1] != self.period[0]:
-            row_list.append(self.period[0])
-        if not col_list or col_list[-1] != self.period[1]:
-            col_list.append(self.period[1])
+        if not row_list or row_list[-1] != self.period[1]:
+            row_list.append(self.period[1])
+        if not col_list or col_list[-1] != self.period[0]:
+            col_list.append(self.period[0])
 
         if row_list and row_list[0] == 0:
             row_list = row_list[1:]
         if col_list and col_list[0] == 0:
             col_list = col_list[1:]
 
         ucell_layer = torch.ones((len(row_list), len(col_list)), dtype=datatype, requires_grad=True) * pmtvy_base
```

### Comparing `meent-0.9.3/meent/on_torch/optimizer/loss.py` & `meent-0.9.4/meent/on_torch/optimizer/loss.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.3/meent/on_torch/optimizer/optimizer.py` & `meent-0.9.4/meent/on_torch/optimizer/optimizer.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.3/meent.egg-info/SOURCES.txt` & `meent-0.9.4/meent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meent-0.9.3/setup.py` & `meent-0.9.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
             ],
     'pytorch': ['torch>=2.0.0',
                 'tqdm>=4.64.1',
                 ],
 }
 setup(
     name='meent',
-    version='0.9.3',
+    version='0.9.4',
     url='https://github.com/kc-ml2/meent',
     author='KC ML2',
     author_email='yongha@kc-ml2.com',
     packages=['meent'] + find_packages(include=['meent.*']),
     install_requires=[
         'numpy>=1.23.3',
         'scipy>=1.9.1',
```

