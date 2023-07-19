# Comparing `tmp/neurondm-0.1.5.tar.gz` & `tmp/neurondm-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurondm-0.1.5.tar", last modified: Wed May 17 20:20:52 2023, max compression
+gzip compressed data, was "neurondm-0.1.6.tar", last modified: Wed Jul 19 03:43:16 2023, max compression
```

## Comparing `neurondm-0.1.5.tar` & `neurondm-0.1.6.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-05-17 20:20:52.186375 neurondm-0.1.5/
--rw-r--r--   0 tom       (1000) tom       (1000)       35 2023-05-16 03:35:52.000000 neurondm-0.1.5/.coveragerc
--rw-r--r--   0 tom       (1000) tom       (1000)     1080 2023-05-16 03:35:52.000000 neurondm-0.1.5/LICENSE
--rw-r--r--   0 tom       (1000) tom       (1000)     4080 2023-05-17 20:20:52.186375 neurondm-0.1.5/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)     2885 2023-05-16 03:35:52.000000 neurondm-0.1.5/README.md
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-05-17 20:20:52.181375 neurondm-0.1.5/docs/
--rw-r--r--   0 tom       (1000) tom       (1000)    46880 2023-05-16 03:35:52.000000 neurondm-0.1.5/docs/NeuronLangExample.ipynb
--rw-r--r--   0 tom       (1000) tom       (1000)    11858 2023-05-16 03:35:52.000000 neurondm-0.1.5/docs/basic-model.org
--rw-r--r--   0 tom       (1000) tom       (1000)     3267 2023-05-17 20:15:44.000000 neurondm-0.1.5/docs/composer.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1618 2023-05-16 03:35:52.000000 neurondm-0.1.5/docs/neurons_notebook.md
--rw-r--r--   0 tom       (1000) tom       (1000)     9180 2023-05-16 03:35:52.000000 neurondm-0.1.5/docs/types.org
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-05-17 20:20:52.182375 neurondm-0.1.5/neurondm/
--rw-r--r--   0 tom       (1000) tom       (1000)       69 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)      199 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/auth-config.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)    68696 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/build.py
--rw-r--r--   0 tom       (1000) tom       (1000)   150961 2023-05-17 20:15:44.000000 neurondm-0.1.5/neurondm/core.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)     4459 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/example.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)     6333 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/indicators.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3843 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/lang.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-05-17 20:20:52.184375 neurondm-0.1.5/neurondm/models/
--rw-r--r--   0 tom       (1000) tom       (1000)      642 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/models/README.md
--rw-r--r--   0 tom       (1000) tom       (1000)      219 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/models/__init__.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)    14860 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/models/allen_cell_types.py
--rw-r--r--   0 tom       (1000) tom       (1000)    12913 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/models/allen_type_specimen_mapping.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3853 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/models/apinat_npo.py
--rw-r--r--   0 tom       (1000) tom       (1000)     6540 2023-05-16 06:04:48.000000 neurondm-0.1.5/neurondm/models/apinat_pops_more.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)     4389 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/models/basic_neurons.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)     3001 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/models/bolew.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)    28861 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/models/cuts.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)    35426 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/models/huang2017.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)    20675 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/models/keast2020.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)     6991 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/models/ma2015.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1310 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/models/nerves.py
--rw-r--r--   0 tom       (1000) tom       (1000)     6704 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/models/nlp.py
--rw-r--r--   0 tom       (1000) tom       (1000)     4334 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/models/pcl.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)     4341 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/models/phenotype_direct.py
--rw-r--r--   0 tom       (1000) tom       (1000)     6624 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/orders.py
--rwxr-xr-x   0 tom       (1000) tom       (1000)    13633 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/phenotype_namespaces.py
--rw-r--r--   0 tom       (1000) tom       (1000)    29628 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/sheets.py
--rw-r--r--   0 tom       (1000) tom       (1000)    15634 2023-05-16 03:35:52.000000 neurondm-0.1.5/neurondm/simple.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-05-17 20:20:52.183375 neurondm-0.1.5/neurondm.egg-info/
--rw-r--r--   0 tom       (1000) tom       (1000)     4080 2023-05-17 20:20:51.000000 neurondm-0.1.5/neurondm.egg-info/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)     1364 2023-05-17 20:20:52.000000 neurondm-0.1.5/neurondm.egg-info/SOURCES.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        1 2023-05-17 20:20:51.000000 neurondm-0.1.5/neurondm.egg-info/dependency_links.txt
--rw-r--r--   0 tom       (1000) tom       (1000)      168 2023-05-17 20:20:51.000000 neurondm-0.1.5/neurondm.egg-info/requires.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        9 2023-05-17 20:20:51.000000 neurondm-0.1.5/neurondm.egg-info/top_level.txt
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-05-17 20:20:52.185375 neurondm-0.1.5/resources/
--rw-r--r--   0 tom       (1000) tom       (1000)   104921 2023-05-17 20:20:51.000000 neurondm-0.1.5/resources/part-of-self.ttl
--rw-r--r--   0 tom       (1000) tom       (1000)    26995 2023-05-17 20:20:51.000000 neurondm-0.1.5/resources/phenotype-core.ttl
--rw-r--r--   0 tom       (1000) tom       (1000)    14792 2023-05-17 20:20:51.000000 neurondm-0.1.5/resources/phenotype-indicators.ttl
--rw-r--r--   0 tom       (1000) tom       (1000)    37820 2023-05-17 20:20:51.000000 neurondm-0.1.5/resources/phenotypes.ttl
--rw-r--r--   0 tom       (1000) tom       (1000)      166 2023-05-17 20:20:52.186375 neurondm-0.1.5/setup.cfg
--rw-r--r--   0 tom       (1000) tom       (1000)     4513 2023-05-16 06:44:23.000000 neurondm-0.1.5/setup.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-05-17 20:20:52.186375 neurondm-0.1.5/test/
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2023-05-16 03:35:52.000000 neurondm-0.1.5/test/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1202 2023-05-17 18:34:54.000000 neurondm-0.1.5/test/common.py
--rw-r--r--   0 tom       (1000) tom       (1000)      407 2023-05-17 18:34:54.000000 neurondm-0.1.5/test/test_0_fix_sys_modules.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2403 2023-05-16 05:56:35.000000 neurondm-0.1.5/test/test_integration.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2316 2023-05-16 03:35:52.000000 neurondm-0.1.5/test/test_label.py
--rw-r--r--   0 tom       (1000) tom       (1000)      387 2023-05-16 03:35:52.000000 neurondm-0.1.5/test/test_load.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2023 2023-05-16 03:35:52.000000 neurondm-0.1.5/test/test_madness.py
--rw-r--r--   0 tom       (1000) tom       (1000)    10400 2023-05-16 03:35:52.000000 neurondm-0.1.5/test/test_neurons.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3399 2023-05-16 03:35:52.000000 neurondm-0.1.5/test/test_simple.py
--rw-r--r--   0 tom       (1000) tom       (1000)      754 2023-05-16 03:35:52.000000 neurondm-0.1.5/test/test_triples.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1253 2023-05-16 03:35:52.000000 neurondm-0.1.5/test/test_write.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-19 03:43:16.679680 neurondm-0.1.6/
+-rw-r--r--   0 tom       (1000) tom       (1000)       35 2023-07-19 03:21:26.000000 neurondm-0.1.6/.coveragerc
+-rw-r--r--   0 tom       (1000) tom       (1000)     1080 2023-07-19 03:21:26.000000 neurondm-0.1.6/LICENSE
+-rw-r--r--   0 tom       (1000) tom       (1000)     4080 2023-07-19 03:43:16.679680 neurondm-0.1.6/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)     2885 2023-07-19 03:21:26.000000 neurondm-0.1.6/README.md
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-19 03:43:16.673681 neurondm-0.1.6/docs/
+-rw-r--r--   0 tom       (1000) tom       (1000)    35150 2023-07-19 03:21:26.000000 neurondm-0.1.6/docs/NeuronLangExample.ipynb
+-rw-r--r--   0 tom       (1000) tom       (1000)    11858 2023-07-19 03:21:26.000000 neurondm-0.1.6/docs/basic-model.org
+-rw-r--r--   0 tom       (1000) tom       (1000)     8852 2023-07-19 03:21:26.000000 neurondm-0.1.6/docs/composer.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1618 2023-07-19 03:21:26.000000 neurondm-0.1.6/docs/neurons_notebook.md
+-rw-r--r--   0 tom       (1000) tom       (1000)     9180 2023-07-19 03:21:26.000000 neurondm-0.1.6/docs/types.org
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-19 03:43:16.675680 neurondm-0.1.6/neurondm/
+-rw-r--r--   0 tom       (1000) tom       (1000)       69 2023-07-19 03:22:19.000000 neurondm-0.1.6/neurondm/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      199 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/auth-config.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)    68696 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/build.py
+-rw-r--r--   0 tom       (1000) tom       (1000)   152101 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/core.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)     4459 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/example.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)     6333 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/indicators.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3843 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/lang.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-19 03:43:16.677681 neurondm-0.1.6/neurondm/models/
+-rw-r--r--   0 tom       (1000) tom       (1000)      642 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/models/README.md
+-rw-r--r--   0 tom       (1000) tom       (1000)      219 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/models/__init__.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)    14860 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/models/allen_cell_types.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    12913 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/models/allen_type_specimen_mapping.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3853 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/models/apinat_npo.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    10886 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/models/apinat_pops_more.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)     4389 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/models/basic_neurons.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)     3001 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/models/bolew.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)    28861 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/models/cuts.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)    35426 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/models/huang2017.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)    20675 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/models/keast2020.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)     6991 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/models/ma2015.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1310 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/models/nerves.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     6685 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/models/nlp.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     4334 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/models/pcl.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)     4341 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/models/phenotype_direct.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     8922 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/orders.py
+-rwxr-xr-x   0 tom       (1000) tom       (1000)    13633 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/phenotype_namespaces.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    29628 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/sheets.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    15634 2023-07-19 03:21:26.000000 neurondm-0.1.6/neurondm/simple.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-19 03:43:16.675680 neurondm-0.1.6/neurondm.egg-info/
+-rw-r--r--   0 tom       (1000) tom       (1000)     4080 2023-07-19 03:43:16.000000 neurondm-0.1.6/neurondm.egg-info/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)     1364 2023-07-19 03:43:16.000000 neurondm-0.1.6/neurondm.egg-info/SOURCES.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)        1 2023-07-19 03:43:16.000000 neurondm-0.1.6/neurondm.egg-info/dependency_links.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)      168 2023-07-19 03:43:16.000000 neurondm-0.1.6/neurondm.egg-info/requires.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)        9 2023-07-19 03:43:16.000000 neurondm-0.1.6/neurondm.egg-info/top_level.txt
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-19 03:43:16.678681 neurondm-0.1.6/resources/
+-rw-r--r--   0 tom       (1000) tom       (1000)   104921 2023-07-19 03:43:15.000000 neurondm-0.1.6/resources/part-of-self.ttl
+-rw-r--r--   0 tom       (1000) tom       (1000)    27641 2023-07-19 03:43:15.000000 neurondm-0.1.6/resources/phenotype-core.ttl
+-rw-r--r--   0 tom       (1000) tom       (1000)    14792 2023-07-19 03:43:15.000000 neurondm-0.1.6/resources/phenotype-indicators.ttl
+-rw-r--r--   0 tom       (1000) tom       (1000)    37820 2023-07-19 03:43:15.000000 neurondm-0.1.6/resources/phenotypes.ttl
+-rw-r--r--   0 tom       (1000) tom       (1000)      166 2023-07-19 03:43:16.679680 neurondm-0.1.6/setup.cfg
+-rw-r--r--   0 tom       (1000) tom       (1000)     4513 2023-07-19 03:21:26.000000 neurondm-0.1.6/setup.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-19 03:43:16.679680 neurondm-0.1.6/test/
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2023-07-19 03:21:26.000000 neurondm-0.1.6/test/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1202 2023-07-19 03:21:26.000000 neurondm-0.1.6/test/common.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      407 2023-07-19 03:21:26.000000 neurondm-0.1.6/test/test_0_fix_sys_modules.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2403 2023-07-19 03:21:26.000000 neurondm-0.1.6/test/test_integration.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2316 2023-07-19 03:21:26.000000 neurondm-0.1.6/test/test_label.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      387 2023-07-19 03:21:26.000000 neurondm-0.1.6/test/test_load.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2023 2023-07-19 03:21:26.000000 neurondm-0.1.6/test/test_madness.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    10400 2023-07-19 03:21:26.000000 neurondm-0.1.6/test/test_neurons.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3399 2023-07-19 03:21:26.000000 neurondm-0.1.6/test/test_simple.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      754 2023-07-19 03:21:26.000000 neurondm-0.1.6/test/test_triples.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1253 2023-07-19 03:21:26.000000 neurondm-0.1.6/test/test_write.py
```

### Comparing `neurondm-0.1.5/LICENSE` & `neurondm-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.5/PKG-INFO` & `neurondm-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurondm
-Version: 0.1.5
+Version: 0.1.6
 Summary: A data model for neuron types.
 Home-page: https://github.com/tgbugs/pyontutils/tree/master/neurondm
 Author: Tom Gillespie
 Author-email: tgbugs@gmail.com
 License: MIT
 Keywords: neuron types NIF ontology neuroscience phenotype OWL rdf rdflib data model
 Classifier: Development Status :: 4 - Beta
```

### Comparing `neurondm-0.1.5/README.md` & `neurondm-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.5/docs/NeuronLangExample.ipynb` & `neurondm-0.1.6/docs/NeuronLangExample.ipynb`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9834081711121911%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(0, "Neuron Lang is a python based domain specific '*

 * *            'language for naming neurons. Neurons are modelled as collections of phenotypes with '*

 * *            'semantics backed by Web Ontology Language (OWL2) classes. Neuron Lang provides tools '*

 * *            'for mapping to and from collections of local names for phenotypes by using ontology '*

 * *            'identifiers as the common language underlying all local naming. These tools also let '*

 * *            'us autom […]*

```diff
@@ -1,14 +1,14 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Neuron Lang is a python based DSL for naming neurons. Neurons are modelled as collections of phenotypes with semantics backed by Web Ontology Language (OWL2) classes. Neuron Lang provides tools for mapping to and from collections of local names for phenotypes by using ontology identifiers as the common language underlying all local naming. These tools also let us automatically generate names for neurons in a regular and consistent way using a set of rules operating on the neurons' constitutent phenotypes. Neuron Lang can export to python or to any serialziation supported by rdflib, however [deterministic turtle](https://github.com/tgbugs/pyontutils/blob/master/ttlser/docs/ttlser.md) (ttl) is prefered. Neuron Lang depends on files from the [NIF-Ontology](https://github.com/SciCrunch/NIF-Ontology).\n",
+                "Neuron Lang is a python based domain specific language for naming neurons. Neurons are modelled as collections of phenotypes with semantics backed by Web Ontology Language (OWL2) classes. Neuron Lang provides tools for mapping to and from collections of local names for phenotypes by using ontology identifiers as the common language underlying all local naming. These tools also let us automatically generate names for neurons in a regular and consistent way using a set of rules operating on the neurons' constitutent phenotypes. Neuron Lang can export to python or to any serialziation supported by rdflib, however [deterministic turtle](https://github.com/tgbugs/pyontutils/blob/master/ttlser/docs/ttlser.md) (ttl) is prefered.\n",
                 "\n",
                 "This notebook has examples of how to use Neuron Lang to:\n",
                 "* Define neurons and phenotypes.\n",
                 "* Export all defined neurons.\n",
                 "* Use `%scig` magic to search for existing ontology identifiers\n",
                 "* Use `LocalNameManager` to create abbreviations for phenotypes.\n",
                 "* Bind local names in the current python namespace using `with` or `setLocalNames`.\n",
@@ -25,19 +25,25 @@
                 "## Setup for any file defining neurons"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": []
+                }
+            ],
             "source": [
-                "from neurondm import *\n",
+                "from neurondm.lang import *\n",
                 "# set predicates in the event that the default config options do not work\n",
-                "# if you cloned the NIF-Ontology into a nonstandard location change ontology_local_repo in devconfig.yaml\n",
+                "# if NIF-Ontology is in a nonstandard location change ontology-local-repo in ~/.config/pyontutils/config.yaml\n",
                 "from pyontutils.namespaces import ilxtr as pred\n",
                 "from neurondm import phenotype_namespaces as phns\n",
                 "\n",
                 "config = Config('neuron-lang-notebook')\n",
                 "# By default Config saves ontology files in NIF-Ontology/ttl/generated/neurons/\n",
                 "# and python files in pyontutils/neurondm/neurondm/compiled/\n",
                 "\n",
@@ -96,15 +102,15 @@
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Neuron(Phenotype('NCBITaxon:10090',\n",
-                        "                 'ilxtr:hasInstanceInSpecies',\n",
+                        "                 'ilxtr:hasInstanceInTaxon',\n",
                         "                 label='Mus musculus'),\n",
                         "       Phenotype('UBERON:0000955',\n",
                         "                 'ilxtr:hasSomaLocatedIn',\n",
                         "                 label='brain'))\n"
                     ]
                 }
             ],
@@ -118,15 +124,15 @@
             "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Neuron(Phenotype('NCBITaxon:10090', 'ilxtr:hasInstanceInSpecies', label='Mus musculus'), Phenotype('UBERON:0000955', 'ilxtr:hasSomaLocatedIn', label='brain'))\n"
+                        "Neuron(Phenotype('NCBITaxon:10090', 'ilxtr:hasInstanceInTaxon', label='Mus musculus'), Phenotype('UBERON:0000955', 'ilxtr:hasSomaLocatedIn', label='brain'))\n"
                     ]
                 }
             ],
             "source": [
                 "print(repr(myFirstNeuron))  # NOTE: this is equivalent to typing `myFirstNeuron` and running the cell"
             ]
         },
@@ -153,43 +159,54 @@
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "@prefix : <file:///ERROR/EMPTY/PREFIX/BANNED/> .\n",
                         "@prefix ilxtr: <http://uri.interlex.org/tgbugs/uris/readable/> .\n",
                         "@prefix NCBITaxon: <http://purl.obolibrary.org/obo/NCBITaxon_> .\n",
                         "@prefix owl: <http://www.w3.org/2002/07/owl#> .\n",
+                        "@prefix partOf: <http://purl.obolibrary.org/obo/BFO_0000050> .\n",
                         "@prefix prov: <http://www.w3.org/ns/prov#> .\n",
                         "@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .\n",
                         "@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .\n",
                         "@prefix SAO: <http://uri.neuinfo.org/nif/nifstd/sao> .\n",
+                        "@prefix skos: <http://www.w3.org/2004/02/skos/core#> .\n",
                         "@prefix TEMP: <http://uri.interlex.org/temp/uris/> .\n",
                         "@prefix UBERON: <http://purl.obolibrary.org/obo/UBERON_> .\n",
-                        "@prefix xml: <http://www.w3.org/XML/1998/namespace> .\n",
-                        "@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .\n",
                         "\n",
-                        "<https://raw.githubusercontent.com/SciCrunch/NIF-Ontology/neurons/ttl/generated/neurons/neuron-lang-notebook.ttl> a owl:Ontology ;\n",
-                        "    owl:imports <https://raw.githubusercontent.com/SciCrunch/NIF-Ontology/neurons/ttl/phenotype-core.ttl>,\n",
+                        "<https://raw.githubusercontent.com/SciCrunch/NIF-Ontology/dev/./neuron-lang-notebook.ttl> a owl:Ontology ;\n",
+                        "    owl:imports <https://raw.githubusercontent.com/SciCrunch/NIF-Ontology/dev/ttl/phenotype-core.ttl>,\n",
+                        "        <https://raw.githubusercontent.com/SciCrunch/NIF-Ontology/dev/ttl/phenotype-indicators.ttl>,\n",
+                        "        <https://raw.githubusercontent.com/SciCrunch/NIF-Ontology/dev/ttl/phenotypes.ttl>,\n",
+                        "        <https://raw.githubusercontent.com/SciCrunch/NIF-Ontology/neurons/ttl/phenotype-core.ttl>,\n",
+                        "        <https://raw.githubusercontent.com/SciCrunch/NIF-Ontology/neurons/ttl/phenotype-indicators.ttl>,\n",
                         "        <https://raw.githubusercontent.com/SciCrunch/NIF-Ontology/neurons/ttl/phenotypes.ttl> ;\n",
-                        "    prov:wasGeneratedBy <https://github.com/tgbugs/pyontutils/blob/f8c3c5c5a3ac8b259009d30153214fb056a13274/neurondm/neurondm/core.py#L555> .\n",
+                        "    prov:wasGeneratedBy <https://github.com/tgbugs/pyontutils/blob/uncommitted@501fd005/neurondm/neurondm/core.py#L1487> .\n",
                         "\n",
                         "### Classes\n",
                         "\n",
-                        "TEMP:0-p0-NCBITaxon-10090-0-p3-UBERON-0000955 a owl:Class ;\n",
+                        "TEMP:SAO-1417703748-0-ilxtr-hasInstanceInTaxon-NCBITaxon-10090-0-ilxtr-hasSomaLocatedIn-UBERON-0000955 a owl:Class ;\n",
                         "    owl:equivalentClass [ a owl:Class ;\n",
                         "            owl:intersectionOf (\n",
                         "                    SAO:1417703748\n",
                         "                    [ a owl:Restriction ;\n",
-                        "                        owl:onProperty ilxtr:hasInstanceInSpecies ;\n",
+                        "                        owl:onProperty ilxtr:hasInstanceInTaxon ;\n",
                         "                        owl:someValuesFrom NCBITaxon:10090 ]\n",
                         "                    [ a owl:Restriction ;\n",
                         "                        owl:onProperty ilxtr:hasSomaLocatedIn ;\n",
-                        "                        owl:someValuesFrom UBERON:0000955 ] ) ] ;\n",
-                        "    rdfs:label \"Mus musculus brain neuron\" .\n",
+                        "                        owl:someValuesFrom [ a owl:Restriction ;\n",
+                        "                                owl:onProperty partOf: ;\n",
+                        "                                owl:someValuesFrom UBERON:0000955 ] ] ) ] ;\n",
+                        "    rdfs:label \"Mus musculus brain neuron\" ;\n",
+                        "    skos:prefLabel \"Mus musculus brain neuron\" ;\n",
+                        "    ilxtr:genLabel \"Mus musculus brain neuron\" ;\n",
+                        "    ilxtr:localLabel \"Mus musculus brain neuron\" ;\n",
+                        "    ilxtr:simpleLabel \"Mus musculus brain neuron\" ;\n",
+                        "    ilxtr:simpleLocalLabel \"Mus musculus brain neuron\" .\n",
                         "\n",
-                        "### Serialized using the pyontutils deterministic serializer v1.2.0\n",
+                        "### Serialized using the ttlser deterministic serializer v1.2.1\n",
                         "\n"
                     ]
                 }
             ],
             "source": [
                 "# view the turtle (ttl) serialization of all neurons\n",
                 "turtle = config.ttl()\n",
@@ -201,50 +218,65 @@
             "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "#!/usr/bin/env python3.7\n",
-                        "from neurondm.core import *\n",
+                        "#!/usr/bin/env python3\n",
+                        "from neurondm.lang import *\n",
                         "\n",
-                        "config = Config('neuron-lang-notebook')\n",
+                        "config = Config('neuron-lang-notebook',\n",
+                        "                file=__file__,\n",
+                        "                ttl_export_dir='~/.local/share/neurondm/git-repo')\n",
                         "\n",
                         "# Mus musculus brain neuron\n",
                         "Neuron(Phenotype('NCBITaxon:10090',\n",
-                        "                 'ilxtr:hasInstanceInSpecies',\n",
+                        "                 'ilxtr:hasInstanceInTaxon',\n",
                         "                 label='Mus musculus'),\n",
                         "       Phenotype('UBERON:0000955',\n",
                         "                 'ilxtr:hasSomaLocatedIn',\n",
-                        "                 label='brain'))\n"
+                        "                 label='brain'))\n",
+                        "\n"
                     ]
                 }
             ],
             "source": [
                 "# view the python serialization of all neurons for the current config\n",
                 "python = config.python()\n",
                 "print(python)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 8,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": []
+                }
+            ],
             "source": [
                 "# write the turtle file defined in cell 1\n",
                 "config.write()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 9,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": []
+                }
+            ],
             "source": [
                 "# write a python file that has the same name as the file in cell 1\n",
                 "# but with python safe separators and a .py extension\n",
                 "config.write_python()"
             ]
         },
         {
@@ -253,15 +285,15 @@
             "metadata": {
                 "scrolled": true
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "[Neuron(Phenotype('NCBITaxon:10090', 'ilxtr:hasInstanceInSpecies', label='Mus musculus'), Phenotype('UBERON:0000955', 'ilxtr:hasSomaLocatedIn', label='brain'))]"
+                            "[Neuron(Phenotype('NCBITaxon:10090', 'ilxtr:hasInstanceInTaxon', label='Mus musculus'), Phenotype('UBERON:0000955', 'ilxtr:hasSomaLocatedIn', label='brain'))]"
                         ]
                     },
                     "execution_count": 10,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -288,32 +320,34 @@
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Look look up ontology terms on the command line.\n",
                         "\n",
                         "Usage:\n",
-                        "    scig v [--local --verbose --key=KEY] <id>...\n",
-                        "    scig i [--local --verbose --key=KEY] <id>...\n",
-                        "    scig t [--local --verbose --limit=LIMIT --key=KEY --prefix=P...] <term>...\n",
-                        "    scig s [--local --verbose --limit=LIMIT --key=KEY --prefix=P...] <term>...\n",
-                        "    scig g [--local --verbose --rt=RELTYPE --edges --key=KEY] <id>...\n",
-                        "    scig e [--local --verbose --key=KEY] <p> <s> <o>\n",
-                        "    scig c [--local --verbose --key=KEY]\n",
-                        "    scig cy [--verbose --limit=LIMIT] <query>\n",
-                        "    scig onts [options]\n",
+                        "    scig v    [--api=A --local --verbose --key=KEY] <id>...\n",
+                        "    scig i    [--api=A --local --verbose --key=KEY] <id>...\n",
+                        "    scig t    [--api=A --local --verbose --limit=LIMIT --key=KEY --prefix=P...] <term>...\n",
+                        "    scig s    [--api=A --local --verbose --limit=LIMIT --key=KEY --prefix=P...] <term>...\n",
+                        "    scig g    [--api=A --local --verbose --rt=RELTYPE --edges --key=KEY] <id>...\n",
+                        "    scig e    [--api=A --local --verbose --key=KEY] <p> <s> <o>\n",
+                        "    scig c    [--api=A --local --verbose --key=KEY]\n",
+                        "    scig cy   [--api=A --local --verbose --limit=LIMIT] <query>\n",
+                        "    scig onts [--api=A --local --verbose --key=KEY]\n",
                         "\n",
                         "Options:\n",
+                        "    -a --api=A          Full url to SciGraph api endpoint\n",
                         "    -e --edges          print edges only\n",
                         "    -l --local          hit the local scigraph server\n",
                         "    -v --verbose        print the full uri\n",
                         "    -t --limit=LIMIT    limit number of results [default: 10]\n",
                         "    -k --key=KEY        api key\n",
                         "    -w --warn           warn on errors\n",
-                        "    -p --prefix=P...    filter by prefix\n"
+                        "    -p --prefix=P       filter by prefix\n",
+                        "    -r --rt=RELTYPE     relationshipType\n"
                     ]
                 }
             ],
             "source": [
                 "import neurondm.lang\n",
                 "\n",
                 "%scig --help"
@@ -325,24 +359,24 @@
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "hippocampus\n",
-                        "http://localhost:9000/scigraph/vocabulary/term/hippocampus?limit=1\n",
-                        "\tUBERON:0001954\n",
+                        "http://selene:9000/scigraph/vocabulary/term/hippocampus?limit=1\n",
+                        "\tFMA:275020\n",
                         "\t\tabbreviations: []\n",
                         "\t\tacronyms: []\n",
-                        "\t\tcategories: ['anatomical entity']\n",
-                        "\t\tdefinitions: ['A part of the brain consisting of a three layered cortex located in the forebrain bordering the medial surface of the lateral ventricle. The term hippocampus is often used synonymously with hippocampal formation which consists of the hippocampus proper or Cornu Ammonis, the dentate gyrus and the subiculum.']\n",
+                        "\t\tcategories: []\n",
+                        "\t\tdefinitions: ['Gyrus of limbic lobe, each instance of which is convoluted mass of gray matter extending the entire length of the floor of the temporal horn of some lateral ventricle; it is part of some limbic system and plays major roles in short term memory and spatial navigation.']\n",
                         "\t\tdeprecated: False\n",
-                        "\t\tiri: http://purl.obolibrary.org/obo/UBERON_0001954\n",
-                        "\t\tlabels: [\"Ammon's horn\"]\n",
-                        "\t\tsynonyms: ['ammon horn', 'ammon gyrus', 'cornu ammonis', 'hippocampus proprius', 'hippocampus', \"Ammon's horn\", 'hippocampus proper', 'hippocampus major', 'Ammons horn', 'Ammon horn fields']\n",
+                        "\t\tiri: http://purl.org/sig/ont/fma/fma275020\n",
+                        "\t\tlabels: ['Hippocampus']\n",
+                        "\t\tsynonyms: ['Hippocampus']\n",
                         "\n"
                     ]
                 }
             ],
             "source": [
                 "# use -t to limit the number of results\n",
                 "%scig -t 1 t hippocampus -v"
@@ -362,15 +396,15 @@
                         "\t\tabbreviations: []\n",
                         "\t\tacronyms: []\n",
                         "\t\tcategories: ['organism']\n",
                         "\t\tdefinitions: []\n",
                         "\t\tdeprecated: False\n",
                         "\t\tiri: http://purl.obolibrary.org/obo/NCBITaxon_9544\n",
                         "\t\tlabels: ['Macaca mulatta']\n",
-                        "\t\tsynonyms: ['Rhesus monkey', 'rhesus macaque', 'rhesus monkeys', 'rhesus macaques']\n",
+                        "\t\tsynonyms: ['Rhesus monkey', 'rhesus macaque', 'rhesus monkeys', 'rhesus macaques', 'Cercopithecus mulatta']\n",
                         "\n"
                     ]
                 }
             ],
             "source": [
                 "# you can escape spaces with \\\n",
                 "%scig t macaca\\ mulatta"
@@ -390,15 +424,15 @@
                         "\t\tabbreviations: []\n",
                         "\t\tacronyms: []\n",
                         "\t\tcategories: []\n",
                         "\t\tdefinitions: ['A membrane-bounded organelle of eukaryotic cells that contains the chromosomes. It is the primary site of DNA replication and RNA synthesis in the cell (Gene Ontology).']\n",
                         "\t\tdeprecated: False\n",
                         "\t\tiri: http://uri.neuinfo.org/nif/nifstd/sao1702920020\n",
                         "\t\tlabels: ['Nucleus']\n",
-                        "\t\tsynonyms: []\n",
+                        "\t\tsynonyms: ['Nucleus']\n",
                         "\n"
                     ]
                 }
             ],
             "source": [
                 "# quotes also allow search with spaces\n",
                 "%scig -t 1 s 'nucleus basalis of meynert'"
@@ -418,26 +452,26 @@
                         "\t\tabbreviations: []\n",
                         "\t\tacronyms: []\n",
                         "\t\tcategories: []\n",
                         "\t\tdefinitions: ['Catalysis of the reaction: 2 hydrogen peroxide = O2 + 2 H2O.']\n",
                         "\t\tdeprecated: False\n",
                         "\t\tiri: http://purl.obolibrary.org/obo/GO_0004096\n",
                         "\t\tlabels: ['catalase activity']\n",
-                        "\t\tsynonyms: ['catalase-peroxidase activity', 'optidase activity', 'hydrogen-peroxide:hydrogen-peroxide oxidoreductase activity', 'equilase activity', 'haem catalase activity', 'caperase activity', 'catalase reaction', 'CAT', 'manganese catalase activity', 'heme catalase activity', 'bacterial catalase-peroxidase activity']\n",
+                        "\t\tsynonyms: ['optidase activity', 'catalase-peroxidase activity', 'hydrogen-peroxide:hydrogen-peroxide oxidoreductase activity', 'equilase activity', 'haem catalase activity', 'caperase activity', 'catalase reaction', 'CAT', 'manganese catalase activity', 'heme catalase activity', 'bacterial catalase-peroxidase activity']\n",
                         "\n",
                         "mouse\n",
-                        "\tBIRNLEX:167\n",
+                        "\tEMAPA:25765\n",
                         "\t\tabbreviations: []\n",
                         "\t\tacronyms: []\n",
-                        "\t\tcategories: ['organism']\n",
+                        "\t\tcategories: []\n",
                         "\t\tdefinitions: []\n",
                         "\t\tdeprecated: False\n",
-                        "\t\tiri: http://uri.neuinfo.org/nif/nifstd/birnlex_167\n",
-                        "\t\tlabels: ['Mouse']\n",
-                        "\t\tsynonyms: ['mouse', 'Mus musculus', 'house mouse']\n",
+                        "\t\tiri: http://purl.obolibrary.org/obo/EMAPA_25765\n",
+                        "\t\tlabels: ['mouse']\n",
+                        "\t\tsynonyms: []\n",
                         "\n"
                     ]
                 }
             ],
             "source": [
                 "# without quotes scig will search multiple terms at once\n",
                 "%scig -t 1 t cat mouse"
@@ -457,16 +491,16 @@
                 "scrolled": true
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "synonyms: ['homotypical cortex', 'isocortex', 'neopallium']\n",
-                        "subjects: UBERON:0017631 UBERON:0003547 UBERON:0022776 UBERON:0001058 UBERON:0010403 UBERON:0003544 UBERON:0002616 UBERON:0005838 UBERON:0013694 UBERON:0013146 UBERON:0003947 UBERON:6003626 UBERON:0010009 UBERON:0006795 UBERON:0005075 UBERON:0013118 UBERON:0001059 UBERON:0007702 UBERON:0008998 UBERON:0000454 UBERON:0003053 UBERON:0006796 UBERON:0003052 UBERON:0005282 UBERON:0003528 UBERON:0000315\n"
+                        "synonyms: ['Isocortex (sensu lato)', 'Homogenetic cortex', 'N\u00e9ocortex', 'Isocortex', 'Neopallial cortex', 'Cortex completus', 'Neocortex', 'Cerebral neocortex', 'Neopallium']\n",
+                        "subjects: UBERON:0022353 UBERON:0015599 UBERON:0005970 UBERON:0023415 UBERON:0001891 UBERON:0000454 UBERON:0022783 UBERON:0002028 UBERON:0005075 UBERON:0024043 UBERON:0023390 UBERON:0007702 UBERON:0023416 UBERON:0001890 UBERON:0003499 UBERON:0024078 UBERON:0002308 CL:0002590 UBERON:0023862 UBERON:0001944 UBERON:0023752 UBERON:0024110 UBERON:0023867 UBERON:0013118 UBERON:2002244 UBERON:0017631 UBERON:0022776 UBERON:0013694 UBERON:0006795 UBERON:0023417 UBERON:0001059 UBERON:0005408 UBERON:0014933 UBERON:0024201 UBERON:0003528 UBERON:0005282 UBERON:0008998 UBERON:0006796 UBERON:0003052 CL:2000005 UBERON:0003544 CL:2000044 UBERON:0002092 UBERON:0003547 UBERON:0024193 UBERON:0005838 UBERON:0022791 UBERON:0024183 UBERON:0023852 UBERON:0002138 UBERON:0002616 UBERON:0023868 UBERON:0003053 UBERON:0002298 UBERON:0023865 UBERON:0016636 UBERON:0023787 UBERON:0001058 UBERON:0039175 UBERON:0014908 UBERON:0010009 UBERON:0023564 UBERON:0023861 UBERON:0010403 UBERON:0003549 CL:2000043 UBERON:0013146 UBERON:8480001 UBERON:0006487 UBERON:0024090 UBERON:0003947 UBERON:6003626\n"
                     ]
                 }
             ],
             "source": [
                 "from pyontutils.scigraph_client import Graph, Vocabulary\n",
                 "\n",
                 "sgg = Graph()\n",
@@ -514,15 +548,15 @@
                         "       Phenotype('UBERON:0000955',\n",
                         "                 'ilxtr:hasSomaLocatedIn',\n",
                         "                 label='brain'),\n",
                         "       Phenotype('PR:000013502',\n",
                         "                 'ilxtr:hasExpressionPhenotype',\n",
                         "                 label='parvalbumin alpha'))\n",
                         "\u001b[31mrepr inside inside:\u001b[0m Neuron(Rat, brain, PV)\n",
-                        "\u001b[31mrepr outside inside:\u001b[0m Neuron(Mouse, brain)\n",
+                        "\u001b[31mrepr outside inside:\u001b[0m Neuron(Phenotype('NCBITaxon:10090', 'ilxtr:hasInstanceInTaxon', label='Mus musculus'), brain)\n",
                         "\u001b[31mrepr inside outside:\u001b[0m Neuron(Phenotype('NCBITaxon:10116', 'ilxtr:hasInstanceInSpecies', label='Rattus norvegicus'), Phenotype('UBERON:0000955', 'ilxtr:hasSomaLocatedIn', label='brain'), Phenotype('PR:000013502', 'ilxtr:hasExpressionPhenotype', label='parvalbumin alpha'))\n",
                         "\u001b[34mRat fails as expected.\u001b[0m\n"
                     ]
                 }
             ],
             "source": [
                 "from neurondm import LocalNameManager\n",
@@ -575,43 +609,43 @@
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "\u001b[31mNamespaces:\u001b[0m ['Test', 'Layers', 'PaxRatLayers', 'Regions', 'PaxRatRegions', 'Species', 'BBP', 'CUT']\n",
                         "\u001b[31mThe error:\u001b[0m Mapping between LocalNames and phenotypes must be injective.\n",
-                        "Cannot cannot bind 'LOOK_AT_THE_CUTE_LITTLE_GUY' to Phenotype('NCBITaxon:10116', 'ilxtr:hasInstanceInSpecies', label='Rattus norvegicus').\n",
+                        "Cannot cannot bind 'LOOK_AT_THE_CUTE_LITTLE_GUY' to Phenotype('NCBITaxon:10116', 'ilxtr:hasInstanceInTaxon', label='Rattus norvegicus').\n",
                         "It is already bound to 'Rat'\n",
                         "\u001b[31mMore species:\u001b[0m\n",
                         "Neuron(Phenotype('NCBITaxon:9685',\n",
                         "                 'ilxtr:hasInstanceInSpecies',\n",
-                        "                 label='Felis catus'),\n",
+                        "                 label='Cat'),\n",
                         "       Phenotype('UBERON:0005391',\n",
-                        "                 'ilxtr:hasLayerLocationPhenotype',\n",
+                        "                 'ilxtr:hasSomaLocatedInLayer',\n",
                         "                 label='cortical layer II'),\n",
                         "       Phenotype('CHEBI:15355',\n",
                         "                 'ilxtr:hasExpressionPhenotype',\n",
                         "                 label='acetylcholine'))\n",
                         "Neuron(Phenotype('NCBITaxon:9685',\n",
                         "                 'ilxtr:hasInstanceInSpecies',\n",
-                        "                 label='Felis catus'),\n",
+                        "                 label='Cat'),\n",
                         "       Phenotype('UBERON:0005392',\n",
-                        "                 'ilxtr:hasLayerLocationPhenotype',\n",
+                        "                 'ilxtr:hasSomaLocatedInLayer',\n",
                         "                 label='cortical layer III'),\n",
                         "       NegPhenotype('CHEBI:15355',\n",
                         "                    'ilxtr:hasExpressionPhenotype',\n",
                         "                    label='acetylcholine'))\n",
                         "\u001b[31mDirect usage:\u001b[0m\n",
                         "Neuron(Phenotype('NCBITaxon:10090',\n",
-                        "                 'ilxtr:hasInstanceInSpecies',\n",
+                        "                 'ilxtr:hasInstanceInTaxon',\n",
                         "                 label='Mus musculus'),\n",
                         "       Phenotype('CHEBI:15355',\n",
                         "                 'ilxtr:hasExpressionPhenotype',\n",
                         "                 label='acetylcholine'))\n",
-                        "\u001b[31mgetLocalNames:\u001b[0m ['CA1', 'CA2', 'CA3', 'CTX', 'L1', 'L2', 'L23', 'L3', 'L4', 'L5', 'L56', 'L6', 'Mouse', 'Rat', 'S1', 'SLA', 'SLM', 'SLU', 'SO', 'SPy', 'SR', 'V1', 'brain', 'setBy_MoreSpecies']\n",
+                        "\u001b[31mgetLocalNames:\u001b[0m ['CA1', 'CA2', 'CA3', 'CTX', 'Human', 'L1', 'L2', 'L23', 'L3', 'L4', 'L5', 'L56', 'L6', 'Mouse', 'Rat', 'S1', 'SLA', 'SLM', 'SLU', 'SO', 'SPy', 'SR', 'V1', 'brain', 'setBy_MoreSpecies']\n",
                         "\u001b[34mNeuron(Mouse, PV) fails as expected\u001b[0m\n"
                     ]
                 }
             ],
             "source": [
                 "cellguard()\n",
                 "\n",
@@ -686,51 +720,44 @@
                     "text": [
                         "\u001b[31mexample 1:\u001b[0m\n",
                         "Neuron(Rat, CA1, CCK)\n",
                         "Neuron(Rat, CA1, NPY)\n",
                         "Neuron(Rat, CA1, PC)\n",
                         "\n",
                         "\u001b[31mexample 2:\u001b[0m\n",
-                        "(Phenotype('NCBITaxon:10116', 'ilxtr:hasInstanceInSpecies', label='Rattus norvegicus'), Phenotype('PAXRAT:322', 'ilxtr:hasSomaLocatedIn', label='field CA1 of the hippocampus (paxrat)'))\n",
+                        "(Phenotype('NCBITaxon:10116', 'ilxtr:hasInstanceInTaxon', label='Rattus norvegicus'), Phenotype('PAXRAT:322', 'ilxtr:hasSomaLocatedIn', label='field CA1 of the hippocampus (paxrat)'))\n",
                         "\n",
                         "\u001b[31merror when setting context:\u001b[0m Cannot change the context of an instantiated neuron. \n",
                         "\n",
                         "\u001b[31mexample 3:\u001b[0m\n",
                         "Neuron(Mouse)\n",
                         "Neuron(Mouse, CCK)\n",
                         "\n",
-                        "\u001b[31mneuron ok:\u001b[0m\n",
-                        "Neuron(Phenotype('NCBITaxon:10116',\n",
-                        "                 'ilxtr:hasInstanceInSpecies',\n",
-                        "                 label='Rattus norvegicus'))\n",
-                        "\n",
-                        "\u001b[34mNeuron(Rat, Mouse) fails as expected\n",
-                        "\u001b[0m\n",
                         "\u001b[31mexample 4:\u001b[0m\n",
                         "Neuron(Rat, CA1, PC)\n",
                         "Neuron(Rat, CA1, PC, VIP)\n",
                         "Neuron(Mouse, CCK)\n",
                         "Neuron(Mouse, CCK, SOM)\n",
                         "Neuron(Rat, CA1, SLM, PC)\n",
                         "Neuron(Rat, CA1, SLM, PC, SOM)\n",
                         "Neuron(Rat, CA1, PC, SOM)\n",
                         "Neuron(Phenotype('NCBITaxon:10116',\n",
-                        "                 'ilxtr:hasInstanceInSpecies',\n",
+                        "                 'ilxtr:hasInstanceInTaxon',\n",
                         "                 label='Rattus norvegicus'),\n",
                         "       Phenotype('UBERON:0001950',\n",
                         "                 'ilxtr:hasSomaLocatedIn',\n",
                         "                 label='neocortex'))\n",
                         "Neuron(Phenotype('NCBITaxon:10116',\n",
-                        "                 'ilxtr:hasInstanceInSpecies',\n",
+                        "                 'ilxtr:hasInstanceInTaxon',\n",
                         "                 label='Rattus norvegicus'),\n",
                         "       Phenotype('UBERON:0001950',\n",
                         "                 'ilxtr:hasSomaLocatedIn',\n",
                         "                 label='neocortex'),\n",
                         "       Phenotype('PAXRAT:509',\n",
-                        "                 'ilxtr:hasLayerLocationPhenotype',\n",
+                        "                 'ilxtr:hasSomaLocatedInLayer',\n",
                         "                 label='layer 1 (paxrat)'))\n"
                     ]
                 }
             ],
             "source": [
                 "cellguard(True)\n",
                 "\n",
@@ -754,22 +781,14 @@
                 "\n",
                 "# you can also use with as syntax when creating a context\n",
                 "with Neuron(Mouse) as n4:\n",
                 "    n5 = Neuron(CCK)\n",
                 "\n",
                 "print(tc.red('example 3:'), *map(repr, (n4, n5)), '', sep='\\n')\n",
                 "\n",
-                "# contexts cannot violate disjointness axioms\n",
-                "try:\n",
-                "    with Neuron(Rat):\n",
-                "        print(tc.red('neuron ok:'), Neuron(), '', sep='\\n')\n",
-                "        with Neuron(Mouse):\n",
-                "            print('This will not print')\n",
-                "except TypeError: print(tc.blue('Neuron(Rat, Mouse) fails as expected\\n'))\n",
-                "\n",
                 "# if you define a new neuron inside a context it will carry\n",
                 "# that context with it if used to define a new context\n",
                 "\n",
                 "# context does not nest for neurons defined outside a with\n",
                 "\n",
                 "with n3:\n",
                 "    n6 = Neuron(VIP)\n",
@@ -805,17 +824,16 @@
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "\u001b[31mcreated with context:\u001b[0m Neuron(CA1, SPy, TPC, DA, CCK, NPY, SOM)\n",
-                        "\u001b[34mNeuron(S1, CA1) fails as expected\u001b[0m Disjointness violated for http://uri.interlex.org/tgbugs/uris/readable/hasSomaLocatedIn due to [Phenotype('PAXRAT:322', 'ilxtr:hasSomaLocatedIn', label='field CA1 of the hippocampus (paxrat)'), Phenotype('PAXRAT:794', 'ilxtr:hasSomaLocatedIn', label='primary somatosensory cortex (paxrat)')]\n",
                         "\u001b[31mSuccess:\u001b[0m Neuron(Rat, S1, L4, PC)\n",
-                        "\u001b[31mgetLocalContext:\u001b[0m CA1 SPy DA CCK NPY SOM\n",
+                        "\u001b[31mgetLocalContext:\u001b[0m CA1 Py DA CCK NPY SST\n",
                         "\u001b[31mno context:\u001b[0m Neuron(brain)\n"
                     ]
                 }
             ],
             "source": [
                 "cellguard(True)\n",
                 "\n",
@@ -888,62 +906,31 @@
                 "    'HBP_CELL:0000148': Neuron(Rat, STRI, MSN, D1),\n",
                 "    'HBP_CELL:0000149': Neuron(Rat, CA3, PC),\n",
                 "        }\n",
                 "neurons['HBP_CELL:0000013']\n",
                 "\n",
                 "cellguard()"
             ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "## Disjointness\n",
-                "Neuron Lang enforces basic disjointness on phenotypes of 'data' level neurons\n"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 22,
-            "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "\u001b[34mNeuron(Mouse, Rat) fails as expected\u001b[0m\n",
-                        "Disjointness violated for http://uri.interlex.org/tgbugs/uris/readable/hasInstanceInSpecies due to [Phenotype('NCBITaxon:10090', 'ilxtr:hasInstanceInSpecies', label='Mus musculus'), Phenotype('NCBITaxon:10116', 'ilxtr:hasInstanceInSpecies', label='Rattus norvegicus')]\n"
-                    ]
-                }
-            ],
-            "source": [
-                "cellguard(True)\n",
-                "\n",
-                "try: Neuron(Mouse, Rat)\n",
-                "except TypeError as e: print(tc.blue('Neuron(Mouse, Rat) fails as expected'), e, sep='\\n')\n",
-                "    \n",
-                "cellguard()"
-            ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.6.8"
+            "version": "3.10.11"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `neurondm-0.1.5/docs/basic-model.org` & `neurondm-0.1.6/docs/basic-model.org`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.5/docs/neurons_notebook.md` & `neurondm-0.1.6/docs/neurons_notebook.md`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.5/docs/types.org` & `neurondm-0.1.6/docs/types.org`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.5/neurondm/build.py` & `neurondm-0.1.6/neurondm/build.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.5/neurondm/core.py` & `neurondm-0.1.6/neurondm/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,33 +15,37 @@
 import ontquery as oq
 import orthauth as oa
 from rdflib.extras import infixowl
 from git import Repo
 from ttlser import natsort
 from augpathlib import RepoPath
 from pyontutils import combinators as cmb
-from pyontutils.core import Ont, makeGraph, OntId as bOntId, OntTerm as bOntTerm
+from pyontutils.core import Ont, OntId as bOntId, OntTerm as bOntTerm
 from pyontutils.core import OntConjunctiveGraph, OntResAny, OntResIri, OntResPath
 from pyontutils.utils import stack_magic, injective_dict, makeSimpleLogger, cacheout
 from pyontutils.utils import TermColors as tc, subclasses, get_working_dir
 from pyontutils.config import auth as pauth, working_dir
 from pyontutils.scigraph import Graph, Vocabulary
 from pyontutils.qnamefix import cull_prefixes
 from pyontutils.annotation import AnnotationMixin
 from pyontutils.namespaces import makePrefixes, OntCuries, definition, replacedBy, partOf
 from pyontutils.namespaces import TEMP, UBERON, ilxtr, PREFIXES as uPREFIXES, NIFRID
 from pyontutils.namespaces import rdf, rdfs, owl, skos
+from . import orders
+
+orders.to_rdf, orders.from_rdf = orders.bind_rdflib()
 
 log = makeSimpleLogger('neurondm')
 auth = oa.configure_here('auth-config.py', __name__, include=pauth)
 cfg = oa.core.ConfigBase(None)  # FIXME hack to expand paths
 ont_checkout_ok = auth.get('nifstd-checkout-ok')
 RDFL = oq.plugin.get('rdflib')
 _SGR = oq.plugin.get('SciGraph')
 _done = set()
+_partial_order_linker = ilxtr.neuronPartialOrder
 
 __all__ = [
     'AND',
     'OR',
     'Config',
     'getPhenotypePredicates',
     'graphBase',
@@ -106,14 +110,20 @@
     phenoPreds = type('PhenoPreds', (whenyoujustneedastaticiterable,), classDict)  # FIXME this makes it impossible to add fake data
     predicate_supers = {s:tuple(o for o in
                                 graph.transitive_objects(s, rdfs.subPropertyOf)
                                 if o != s) for s in out}
 
     return phenoPreds, predicate_supers
 
+
+def add_partial_orders(graph, nested):
+    for s, nst in nested.items():
+        bn = orders.to_rdf(graph, nst)
+        graph.add((s, _partial_order_linker, bn))
+
 # label maker
 
 class order_deco:
     """ define functions in order to get order! """
     def __init__(self):
         self.order = tuple()
 
@@ -420,14 +430,17 @@
     @od
     def hasConnectionPhenotype(self, phenotypes):
         yield from self._with_thing_located_in('connecting-to', phenotypes)
     @od
     def hasExperimentalPhenotype(self, phenotypes):
         yield from self._default(phenotypes)
     @od
+    def hasAnatomicalSystemPhenotype(self, phenotypes):
+        yield from self._default(phenotypes)
+    @od
     def hasClassificationPhenotype(self, phenotypes):
         yield from self._default(phenotypes)
     @od
     def hasPhenotype(self, phenotypes):
         yield from self._default(phenotypes)
     @od
     def hasPhenotypeModifier(self, phenotypes):
@@ -1108,14 +1121,16 @@
                 if len(graphBase.python_subclasses) == 2:  # FIXME magic number for Neuron and NeuronCUT
                     ebms = [type(OntId(s).suffix, (NeuronCUT,), dict(owlClass=s))
                             for s in self.load_graph[:rdfs.subClassOf:NeuronEBM.owlClass]
                             if not graphBase.knownClasses.append(s)]
                 else:
                     ebms = []
 
+                graphBase._nested = orders.from_rdf(self.load_graph, _partial_order_linker)
+
                 class_types = [(type, s) for s in self.load_graph[:rdf.type:owl.Class]
                                for type in mostDerived(getClassType(s, self.load_graph)) if type]
                 sc = None
                 for sc in chain(graphBase.python_subclasses, ebms):
                     sc.owlClass
                     iris = [s for type, s in class_types if type == sc.owlClass]
                     if iris:
@@ -1466,15 +1481,15 @@
         OntCuries(PREFIXES)
 
         # input graph setup
         in_graph = core_graph
         for ig in use_in_paths:
             in_graph.parse(ig, format='turtle')
 
-        nin_graph = makeGraph('', prefixes=PREFIXES, graph=in_graph)
+        in_graph.namespace_manager.populate_from(PREFIXES)
         graphBase.in_graph = in_graph
         graphBase.ignore_existing = ignore_existing
 
         # output graph setup
         if out_graph is None:
             _sources = sources
             _source_file = source_file
@@ -1497,23 +1512,22 @@
             #out_graph = rdflib.Graph()
             # in thise case we also want to wipe any existing python Neuron entires
             # that we use to serialize so that behavior is consistent
             NeuronBase.existing_pes = {}
             NeuronBase.existing_ids = {}
         else:
             no = None
-            graphBase.ng = makeGraph('', prefixes=PREFIXES, graph=out_graph)
-        #new_graph = makeGraph('', prefixes=PREFIXES, graph=out_graph)
+            out_graph.namespace_manager.populate_from(PREFIXES)
+
         graphBase.out_graph = out_graph
 
         # python output setup
         graphBase.compiled_location = compiled_location
 
-        # makeGraph setup
-        new_graph = graphBase.ng #= new_graph
+        new_graph = graphBase.ng  # FIXME remove this usage
         new_graph.filename = out_graph_path
 
         if iri is not None:
             ontid = rdflib.URIRef(iri)
         else:
             ontid = rdflib.URIRef('file://' + out_graph_path)  # do not use Path().absolute() it will leak
 
@@ -2459,36 +2473,38 @@
 
     @classmethod
     def _load_existing(cls, iris):
         # TODO rename pes -> phenotypes
         if not cls._loading:
             NeuronBase._loading = True  # block all other neuron loading
             try:
-                log.debug(str([i for i in iris if '4164' in i or '100212' in i]))
+                #log.debug(str([i for i in iris if '4164' in i or '100212' in i]))
                 for iri in iris:
                         # rod/cone issue
                         #breakpoint()
                     try:
-                        n = cls(id_=iri, override=True)#, out_graph=cls.config.load_graph)  # I think we can get away without this
-                        if iri.endswith('4164') or iri.endswith('100212'):
-                            log.debug(f'{iri} -> {n}')
+                        _po = cls._nested[iri] if iri in cls._nested else None
+                        n = cls(id_=iri, override=True, partialOrder=_po)#, out_graph=cls.config.load_graph)  # I think we can get away without this
+                        #if iri.endswith('4164') or iri.endswith('100212'):
+                            #log.debug(f'{iri} -> {n}')
 
                         # because we just call Config again an everything resets
                     except cls.owlClassMismatch as e:
                         log.exception(e)
                         continue
                     except AttributeError as e:
                         log.critical(str(e))
                         raise e
             finally:
                 NeuronBase._loading = False
 
     def __init__(self, *phenotypeEdges, id_=None, label=None, override=False,
-                 equivalentNeurons=tuple(), disjointNeurons=tuple(), definition=None):
+                 equivalentNeurons=tuple(), disjointNeurons=tuple(), partialOrder=None, definition=None):
         self._sighed = False
+        self._nested_partial_order = partialOrder
         if id_ and (equivalentNeurons or disjointNeurons):
             # FIXME does this work!?
             raise TypeError('Neurons defined by id may not use equivalent or disjoint')
 
         super().__init__()
         self._replay = []  # fix for idiocy of using setters to write to the graph
         self._localContext = self.__context
@@ -2616,16 +2632,31 @@
         self.existing_pes[self] = self.Class
         if self._replay:
             rep = self._replay
             self._replay = []
             for p, *os in rep:
                 self.add_objects(p, *os)
 
+        if self._nested_partial_order is not None:
+            bn = orders.to_rdf(graph, self._nested_partial_order)
+            graph.add((s, ilxtr.neuronPartialOrder, bn))
+
         self._sighed = True
 
+    def partialOrder(self, nested=None):
+        """ nested is a the nested list version of the partial order
+
+            if you have an adj list use orders.adj_to_nst before
+            passing in here """
+
+        if self._nested_partial_order is None and nested is not None:
+            self._nested_partial_order = nested
+
+        return self._nested_partial_order
+
     def removeDuplicateSuperProperties(self, rawpes):
         # find any duplicate phenotype values
         # check their dimensions to see if one is a subProperty of the other
         # keep only the most granular
         _cands = defaultdict(set)
         for pe in rawpes:
             _cands[pe.p].add(pe)
@@ -3626,14 +3657,15 @@
 objective for any entry here should be to have it ultimately implemented as
 a rule plus operating from single standard ontology file. """
 if False:  # calling Config at top level breaks import for all normal users
     Config(import_no_net=True)  # explicitly load the core graph TODO need a lighter weight way to do this
 else:
     # note: this solves part of the problem, but mostly defers it until later
     _g = OntConjunctiveGraph()
+    _g.namespace_manager.populate_from(uPREFIXES)
     graphBase.core_graph = _g
 
 
 OntologyGlobalConventions = _ogc = injective_dict(
     Vertebrata = Phenotype('NCBITaxon:7742', 'ilxtr:hasInstanceInTaxon'),  # fix annoying labels
 
     L1 = Phenotype('UBERON:0005390', 'ilxtr:hasSomaLocatedInLayer'),
```

### Comparing `neurondm-0.1.5/neurondm/example.py` & `neurondm-0.1.6/neurondm/example.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.5/neurondm/indicators.py` & `neurondm-0.1.6/neurondm/indicators.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.5/neurondm/lang.py` & `neurondm-0.1.6/neurondm/lang.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.5/neurondm/models/README.md` & `neurondm-0.1.6/neurondm/models/README.md`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.5/neurondm/models/allen_cell_types.py` & `neurondm-0.1.6/neurondm/models/allen_cell_types.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.5/neurondm/models/allen_type_specimen_mapping.py` & `neurondm-0.1.6/neurondm/models/allen_type_specimen_mapping.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.5/neurondm/models/apinat_npo.py` & `neurondm-0.1.6/neurondm/models/apinat_npo.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.5/neurondm/models/basic_neurons.py` & `neurondm-0.1.6/neurondm/models/basic_neurons.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.5/neurondm/models/bolew.py` & `neurondm-0.1.6/neurondm/models/bolew.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.5/neurondm/models/cuts.py` & `neurondm-0.1.6/neurondm/models/cuts.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.5/neurondm/models/huang2017.py` & `neurondm-0.1.6/neurondm/models/huang2017.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.5/neurondm/models/keast2020.py` & `neurondm-0.1.6/neurondm/models/keast2020.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.5/neurondm/models/ma2015.py` & `neurondm-0.1.6/neurondm/models/ma2015.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.5/neurondm/models/nerves.py` & `neurondm-0.1.6/neurondm/models/nerves.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.5/neurondm/models/nlp.py` & `neurondm-0.1.6/neurondm/models/nlp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import re
 from collections import defaultdict
 import rdflib
 from pyontutils.sheets import Sheet
 from pyontutils.namespaces import ilxtr, TEMP, rdfs, skos, owl, interlex_namespace
-from neurondm.core import Config, NeuronEBM, Phenotype, NegPhenotype, log, OntId
+from neurondm.core import Config, NeuronEBM, Phenotype, NegPhenotype, log, OntId, add_partial_orders
 from neurondm import orders
 
-orders.to_rdf = orders.bind_rdflib()
-
 
 class NeuronSparcNlp(NeuronEBM):
     owlClass = ilxtr.NeuronSparcNlp
     shortname = 'sprcnlp'
 
 
 class NLP1(Sheet):
@@ -45,14 +43,15 @@
         'Soma': ilxtr.hasSomaLocatedIn,
         'Axon terminal': ilxtr.hasAxonPresynapticElementIn,
         'Axon': ilxtr.hasAxonLocatedIn,
         'Dendrite': ilxtr.hasDendriteLocatedIn,
         'Axon sensory terminal': ilxtr.hasAxonSensorySubcellularElementIn,
         'hasInstanceInTaxon': ilxtr.hasInstanceInTaxon,
         'hasPhenotype': ilxtr.hasPhenotype,
+        'hasAnatomicalSystemPhenotype': ilxtr.hasAnatomicalSystemPhenotype,
         'hasBiologicalSex': ilxtr.hasBiologicalSex,
         'hasCircuitRolePhenotype': ilxtr.hasCircuitRolePhenotype,
         'hasForwardConnectionPhenotype': ilxtr.hasForwardConnectionPhenotype,  # FIXME this needs to be unionOf
     }[sheet_pred]
     return p
 
 
@@ -68,28 +67,22 @@
                     if j == b:
                         edge =  iu, ju
                         edges.append(edge)
 
     return edges
 
 
-def add_partial_orders(graph, nested):
-    for s, nst in nested.items():
-        bn = orders.to_rdf(graph, nst)
-        graph.add((s, ilxtr.neuronPartialOrder, bn))
-
-
 def main():
     cs = [c() for c in sheet_classes]
     trips = [[cl] + [c.value for c in
                      (r.id(), r.relationship(), r.identifier())]
              for cl in cs for r in cl.rows()
              if r.row_index > 0 and r.id().value
              #and (not hasattr(r, 'exclude') or not r.exclude().value)
-             and r.proposed_action().value != "Don't add"
+             and r.proposed_action().value.lower() != "don't add"
              ]
 
     to_add = []
 
     def vl(meth):
         return rdflib.Literal(meth().value)
 
@@ -103,32 +96,34 @@
     dd = defaultdict(list)
     ec = {}
     for cl in cs:
         _, nlpns = snames[cl.sheet_name]
         for r in cl.rows():
             if (r.row_index > 0 and
                 r.id().value and
-                r.proposed_action().value != "Don't add"):
+                r.proposed_action().value.lower() != "don't add"):
                 # extra trips
                 #print(repr(r.id()))
                 s = OntId(nlpns[r.id().value])
                 #print(s)
                 asdf(s, ilxtr.sentenceNumber, r.sentence_number)
                 asdf(s, ilxtr.curatorNote, r.different_from_existing)
                 asdf(s, ilxtr.curatorNote, r.curation_notes)
                 asdf(s, ilxtr.reviewNote, r.review_notes)
                 asdf(s, ilxtr.reference, r.reference_pubmed_id__doi_or_text)
+                asdf(s, ilxtr.literatureCitation, r.literature_citation)
                 asdf(s, rdfs.label, r.neuron_population_label_a_to_b_via_c)
                 if hasattr(r, 'alert_explanation'):
                     asdf(s, ilxtr.alertNote, r.alert_explanation)
 
                 if hasattr(r, 'explicit_complement') and r.explicit_complement().value:
                     p = map_predicates(r.relationship().value)
                     o = OntId(r.explicit_complement().value)
                     ec[(s, p)] = o
+
                 if hasattr(r, 'axonal_course_poset') and r.axonal_course_poset().value:
                     # s.u and OntId(...).u to avoid duplicate subjects/objects in the graph
                     # due to type vs instance issues for rdflib.URIRef and OntId
                     dd[s.u].append((int(r.axonal_course_poset().value), OntId(r.identifier().value).u))
 
     sorders = {k:sorted(v) for k, v in dd.items()}
     sadj = {k:ind_to_adj(v) for k, v in sorders.items()}
```

### Comparing `neurondm-0.1.5/neurondm/models/pcl.py` & `neurondm-0.1.6/neurondm/models/pcl.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.5/neurondm/models/phenotype_direct.py` & `neurondm-0.1.6/neurondm/models/phenotype_direct.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.5/neurondm/orders.py` & `neurondm-0.1.6/neurondm/orders.py`

 * *Files 23% similar despite different names*

```diff
@@ -76,28 +76,74 @@
     # shortest that are sufficient to cover all nodes, essentially
     # the longest single path through the tree and then branches
     raise NotImplementedError('TODO')
 
 
 def bind_rdflib():
     import rdflib
+    from pyontutils.namespaces import rdf
+
     def to_rdf(g, nested):
         if isinstance(nested, list) or isinstance(nested, tuple):
             bn0 = rdflib.BNode()
             rdflib.collection.Collection(g, bn0, (to_rdf(g, n) for n in nested))
             return bn0
         elif isinstance(nested, rl):
             bn1 = rdflib.BNode()
             return nested.to_rdf(to_rdf, g, bn1)
         elif isinstance(nested, rdflib.term.Node):
             return nested
         else:
             return rdflib.Literal(nested)
 
-    return to_rdf
+    def from_rdf(g, linker, to_python=False):
+        nested = {}
+        for s, o in g[:linker:]:
+            l = tuple(getlist(g, o, to_python=to_python))
+            nested[s] = l
+
+        return nested
+
+    def getlist(g, bn0, to_python=False):
+        def f(node, g):
+            o = None
+            for o in g[node:rdf.first:]:
+                if isinstance(o, rdflib.BNode):
+                    # unfortunately we have to branch on the result type
+                    # or have to look ahead to see if the list continues
+                    # picked the look ahead so that we don't have to check
+                    # length and we don't have to know about the rl type
+                    if list(g[o:rdf.first]):  # list continues
+                        # XXX watch out for malformed lists that might not
+                        # have a rdf:first ?
+                        yield tuple(getlist(g, o, to_python=to_python))
+                    else:  # likely [ :a :b ] case
+                        yield from getlist(g, o, to_python=to_python)
+
+                else:
+                    if to_python and isinstance(o, rdflib.Literal):
+                        yield o.toPython()
+                    else:
+                        yield o
+
+            for o in g[node:rdf.rest:]:
+                if o != rdf.nil:
+                    yield from getlist(g, o, to_python=to_python)
+
+            if o is None and isinstance(node, rdflib.BNode):  # [ :a  :b ] case
+                for p, o in g[node:]:
+                    if to_python:
+                        yield rl((p.toPython() if isinstance(p, rdflib.Literal) else p),
+                                 (o.toPython() if isinstance(o, rdflib.Literal) else o),)
+                    else:
+                        yield rl(p, o)
+
+        yield from g.transitiveClosure(f, bn0)
+
+    return to_rdf, from_rdf
 
 
 class rl:
     def __init__(self, region, layer=None):
         self.region = region
         self.layer = layer
 
@@ -131,15 +177,15 @@
                 type(self.layer) == type(self.layer) and
                 self.layer is not None and
                 self.layer < self.layer)
 
 
 def test():
     from pprint import pprint
-    to_rdf = bind_rdflib()
+    to_rdf, from_rdf = bind_rdflib()
     adj_test = (
         ("a", "b"),
         ("b", "c"),
         ("c", "d"),
         ("d", "e"),
         ("d", "k"),
 
@@ -235,12 +281,20 @@
     rej_6 = nst_to_adj(nst_6)
     pprint(('nst_6', nst_6))
     pprint(('rej_6', rej_6))
     assert sorted(adj_6) == sorted(rej_6)
     bn = to_rdf(g, nst_6)
     g.add((ilxtr['sub-6'], ilxtr.predicate, bn))
 
+    un_rdf = from_rdf(g, ilxtr.predicate, to_python=True)
+    assert un_rdf[ilxtr['sub-1']] == tuple(nested)
+    assert un_rdf[ilxtr['sub-2']] == tuple(nst_2)
+    assert un_rdf[ilxtr['sub-3']] == tuple(nst_3)
+    assert un_rdf[ilxtr['sub-4']] == tuple(nst_4)
+    un_rdf[ilxtr['sub-5']] == tuple(nst_5)  # non-invertable case due to layer=None ambiguity
+    assert un_rdf[ilxtr['sub-6']] == tuple(nst_6)
+
     g.debug()
 
 
 if __name__ == '__main__':
     test()
```

### Comparing `neurondm-0.1.5/neurondm/phenotype_namespaces.py` & `neurondm-0.1.6/neurondm/phenotype_namespaces.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.5/neurondm/sheets.py` & `neurondm-0.1.6/neurondm/sheets.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.5/neurondm/simple.py` & `neurondm-0.1.6/neurondm/simple.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.5/neurondm.egg-info/PKG-INFO` & `neurondm-0.1.6/neurondm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurondm
-Version: 0.1.5
+Version: 0.1.6
 Summary: A data model for neuron types.
 Home-page: https://github.com/tgbugs/pyontutils/tree/master/neurondm
 Author: Tom Gillespie
 Author-email: tgbugs@gmail.com
 License: MIT
 Keywords: neuron types NIF ontology neuroscience phenotype OWL rdf rdflib data model
 Classifier: Development Status :: 4 - Beta
```

### Comparing `neurondm-0.1.5/neurondm.egg-info/SOURCES.txt` & `neurondm-0.1.6/neurondm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.5/resources/part-of-self.ttl` & `neurondm-0.1.6/resources/part-of-self.ttl`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.5/resources/phenotype-core.ttl` & `neurondm-0.1.6/resources/phenotype-core.ttl`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,22 @@
 
 <https://raw.githubusercontent.com/SciCrunch/NIF-Ontology/neurons/ttl/phenotype-core.ttl> a owl:Ontology ;
     rdfs:label "NIF Phenotype core" ;
     rdfs:comment "This is the core set of predicates used to model phenotypes and the parent class for phenotypes." .
 
 ### Object Properties
 
+ilxtr:hasAnatomicalSystemPhenotype a owl:AsymmetricProperty,
+        owl:IrreflexiveProperty,
+        owl:ObjectProperty ;
+    rdfs:label "hasAnatomicalSystemPhenotype" ;
+    skos:definition "Expresses a relationship between a neuron type and some anatomical criteria, such as being located in a particular system. Note that this NOT a subPropertOf hasLocationPhenotype." ;
+    rdfs:subPropertyOf ilxtr:hasPhenotype ;
+    rdfs:comment "This is used to differentiate things like parasympathetic preganglionic from raw hasPhenotype. This can be used in cases where the meaning is clear to the domain experts, but has not been fully formalized." .
+
 ilxtr:hasAxonLocatedIn a owl:AsymmetricProperty,
         owl:IrreflexiveProperty,
         owl:ObjectProperty ;
     rdfs:label "hasAxonLocatedIn" ;
     rdfs:subPropertyOf ilxtr:hasProcessLocatedIn .
 
 ilxtr:hasAxonMorphologicalPhenotype a owl:AsymmetricProperty,
```

### Comparing `neurondm-0.1.5/resources/phenotype-indicators.ttl` & `neurondm-0.1.6/resources/phenotype-indicators.ttl`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.5/resources/phenotypes.ttl` & `neurondm-0.1.6/resources/phenotypes.ttl`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.5/setup.py` & `neurondm-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.5/test/common.py` & `neurondm-0.1.6/test/common.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.5/test/test_integration.py` & `neurondm-0.1.6/test/test_integration.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.5/test/test_label.py` & `neurondm-0.1.6/test/test_label.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.5/test/test_madness.py` & `neurondm-0.1.6/test/test_madness.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.5/test/test_neurons.py` & `neurondm-0.1.6/test/test_neurons.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.5/test/test_simple.py` & `neurondm-0.1.6/test/test_simple.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.5/test/test_triples.py` & `neurondm-0.1.6/test/test_triples.py`

 * *Files identical despite different names*

### Comparing `neurondm-0.1.5/test/test_write.py` & `neurondm-0.1.6/test/test_write.py`

 * *Files identical despite different names*

