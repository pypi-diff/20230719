# Comparing `tmp/medicc2-1.0.0.tar.gz` & `tmp/medicc2-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medicc2-1.0.0.tar", last modified: Wed May 24 14:35:41 2023, max compression
+gzip compressed data, was "medicc2-1.0.2.tar", last modified: Tue Jul 18 23:14:01 2023, max compression
```

## Comparing `medicc2-1.0.0.tar` & `medicc2-1.0.2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-24 14:35:41.323091 medicc2-1.0.0/
--rw-r--r--   0 tom        (501) staff       (20)    36109 2023-05-23 14:44:50.000000 medicc2-1.0.0/LICENSE
--rw-r--r--   0 tom        (501) staff       (20)    19731 2023-05-24 14:35:41.322712 medicc2-1.0.0/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)    19147 2023-05-24 14:32:47.000000 medicc2-1.0.0/README.md
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-24 14:35:41.289239 medicc2-1.0.0/fstlib/
--rw-r--r--   0 tom        (501) staff       (20)      550 2023-05-24 13:14:05.000000 medicc2-1.0.0/fstlib/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    15634 2023-05-24 13:14:05.000000 medicc2-1.0.0/fstlib/algos.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-24 14:35:41.296795 medicc2-1.0.0/fstlib/cext/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-05-23 14:44:52.000000 medicc2-1.0.0/fstlib/cext/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     2100 2023-05-23 14:50:54.000000 medicc2-1.0.0/fstlib/cext/cios.pxd
--rw-r--r--   0 tom        (501) staff       (20)      869 2023-05-23 14:50:54.000000 medicc2-1.0.0/fstlib/cext/cmemory.pxd
--rw-r--r--   0 tom        (501) staff       (20)    16320 2023-05-23 14:50:54.000000 medicc2-1.0.0/fstlib/cext/cops.h
--rw-r--r--   0 tom        (501) staff       (20)     1018 2023-05-23 14:50:54.000000 medicc2-1.0.0/fstlib/cext/cops.pxd
--rw-r--r--   0 tom        (501) staff       (20)    22785 2023-05-23 14:50:54.000000 medicc2-1.0.0/fstlib/cext/cpywrapfst.pxd
--rw-r--r--   0 tom        (501) staff       (20)   287465 2023-05-24 14:35:39.000000 medicc2-1.0.0/fstlib/cext/ops.cpp
--rw-r--r--   0 tom        (501) staff       (20)     2419 2023-05-24 13:14:05.000000 medicc2-1.0.0/fstlib/cext/ops.pyx
--rw-r--r--   0 tom        (501) staff       (20)  2752037 2023-05-24 14:35:40.000000 medicc2-1.0.0/fstlib/cext/pywrapfst.cpp
--rw-r--r--   0 tom        (501) staff       (20)    16028 2023-05-23 14:50:54.000000 medicc2-1.0.0/fstlib/cext/pywrapfst.pxd
--rw-r--r--   0 tom        (501) staff       (20)   149233 2023-05-23 14:50:54.000000 medicc2-1.0.0/fstlib/cext/pywrapfst.pyx
--rw-r--r--   0 tom        (501) staff       (20)    18739 2023-05-24 13:14:05.000000 medicc2-1.0.0/fstlib/core.py
--rw-r--r--   0 tom        (501) staff       (20)     7036 2023-05-24 13:14:05.000000 medicc2-1.0.0/fstlib/ext.py
--rw-r--r--   0 tom        (501) staff       (20)    10235 2023-05-24 13:14:05.000000 medicc2-1.0.0/fstlib/factory.py
--rw-r--r--   0 tom        (501) staff       (20)      397 2023-05-23 14:44:52.000000 medicc2-1.0.0/fstlib/logging_conf.yaml
--rw-r--r--   0 tom        (501) staff       (20)     2609 2023-05-24 13:14:05.000000 medicc2-1.0.0/fstlib/paths.py
--rw-r--r--   0 tom        (501) staff       (20)     1446 2023-05-23 14:44:52.000000 medicc2-1.0.0/fstlib/test_fstlib.py
--rw-r--r--   0 tom        (501) staff       (20)     5794 2023-05-24 13:14:05.000000 medicc2-1.0.0/fstlib/tools.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-24 14:35:41.302316 medicc2-1.0.0/medicc/
--rw-r--r--   0 tom        (501) staff       (20)      629 2023-05-23 14:44:50.000000 medicc2-1.0.0/medicc/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     3540 2023-05-23 14:44:50.000000 medicc2-1.0.0/medicc/ancestors.py
--rw-r--r--   0 tom        (501) staff       (20)    10115 2023-05-23 14:44:50.000000 medicc2-1.0.0/medicc/bootstrap.py
--rw-r--r--   0 tom        (501) staff       (20)    20683 2023-05-23 14:44:50.000000 medicc2-1.0.0/medicc/core.py
--rw-r--r--   0 tom        (501) staff       (20)    23763 2023-05-23 14:44:50.000000 medicc2-1.0.0/medicc/event_reconstruction.py
--rw-r--r--   0 tom        (501) staff       (20)     8045 2023-05-23 14:44:50.000000 medicc2-1.0.0/medicc/factory.py
--rw-r--r--   0 tom        (501) staff       (20)    15900 2023-05-23 14:44:50.000000 medicc2-1.0.0/medicc/io.py
--rw-r--r--   0 tom        (501) staff       (20)      780 2023-05-23 14:44:50.000000 medicc2-1.0.0/medicc/logging_conf.yaml
--rw-r--r--   0 tom        (501) staff       (20)     5483 2023-05-23 14:44:50.000000 medicc2-1.0.0/medicc/nj.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-24 14:35:41.317004 medicc2-1.0.0/medicc/objects/
--rw-r--r--   0 tom        (501) staff       (20)    56129 2023-05-23 14:44:50.000000 medicc2-1.0.0/medicc/objects/Davoli_2013_TSG_OG_genes.bed
--rw-r--r--   0 tom        (501) staff       (20)     1382 2023-05-23 14:44:50.000000 medicc2-1.0.0/medicc/objects/hg19_chromosome_arms.bed
--rw-r--r--   0 tom        (501) staff       (20)     1382 2023-05-23 14:44:50.000000 medicc2-1.0.0/medicc/objects/hg38_chromosome_arms.bed
--rw-r--r--   0 tom        (501) staff       (20)   253982 2023-05-23 14:44:50.000000 medicc2-1.0.0/medicc/objects/no_wgd_asymm.fst
--rw-r--r--   0 tom        (501) staff       (20)   572114 2023-05-23 14:44:50.000000 medicc2-1.0.0/medicc/objects/wgd_1_asymm.fst
--rw-r--r--   0 tom        (501) staff       (20)   689774 2023-05-23 14:44:50.000000 medicc2-1.0.0/medicc/objects/wgd_2_asymm.fst
--rw-r--r--   0 tom        (501) staff       (20)   783870 2023-05-23 14:44:50.000000 medicc2-1.0.0/medicc/objects/wgd_asymm.fst
--rw-r--r--   0 tom        (501) staff       (20)   546246 2023-05-23 14:44:50.000000 medicc2-1.0.0/medicc/objects/wgd_total_cn_1_asymm.fst
--rw-r--r--   0 tom        (501) staff       (20)   656310 2023-05-23 14:44:50.000000 medicc2-1.0.0/medicc/objects/wgd_total_cn_asymm.fst
--rw-r--r--   0 tom        (501) staff       (20)   519890 2023-05-23 14:44:50.000000 medicc2-1.0.0/medicc/objects/wgd_x2_1_asymm.fst
--rw-r--r--   0 tom        (501) staff       (20)   591554 2023-05-23 14:44:50.000000 medicc2-1.0.0/medicc/objects/wgd_x2_asymm.fst
--rw-r--r--   0 tom        (501) staff       (20)    42216 2023-05-23 14:44:50.000000 medicc2-1.0.0/medicc/plot.py
--rw-r--r--   0 tom        (501) staff       (20)     7644 2023-05-23 14:44:50.000000 medicc2-1.0.0/medicc/sim.py
--rw-r--r--   0 tom        (501) staff       (20)     2646 2023-05-23 14:44:50.000000 medicc2-1.0.0/medicc/stats.py
--rw-r--r--   0 tom        (501) staff       (20)     4934 2023-05-23 14:44:50.000000 medicc2-1.0.0/medicc/test_fsts.py
--rw-r--r--   0 tom        (501) staff       (20)    21224 2023-05-23 14:44:50.000000 medicc2-1.0.0/medicc/test_medicc.py
--rw-r--r--   0 tom        (501) staff       (20)     5150 2023-05-24 14:32:47.000000 medicc2-1.0.0/medicc/tools.py
--rw-r--r--   0 tom        (501) staff       (20)    14892 2023-05-24 13:15:32.000000 medicc2-1.0.0/medicc2
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-24 14:35:41.322245 medicc2-1.0.0/medicc2.egg-info/
--rw-r--r--   0 tom        (501) staff       (20)    19731 2023-05-24 14:35:41.000000 medicc2-1.0.0/medicc2.egg-info/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)     1286 2023-05-24 14:35:41.000000 medicc2-1.0.0/medicc2.egg-info/SOURCES.txt
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-05-24 14:35:41.000000 medicc2-1.0.0/medicc2.egg-info/dependency_links.txt
--rw-r--r--   0 tom        (501) staff       (20)      120 2023-05-24 14:35:41.000000 medicc2-1.0.0/medicc2.egg-info/requires.txt
--rw-r--r--   0 tom        (501) staff       (20)       14 2023-05-24 14:35:41.000000 medicc2-1.0.0/medicc2.egg-info/top_level.txt
--rw-r--r--   0 tom        (501) staff       (20)       70 2023-05-23 14:44:50.000000 medicc2-1.0.0/pyproject.toml
--rw-r--r--   0 tom        (501) staff       (20)       38 2023-05-24 14:35:41.323259 medicc2-1.0.0/setup.cfg
--rw-r--r--   0 tom        (501) staff       (20)     2169 2023-05-24 14:32:47.000000 medicc2-1.0.0/setup.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 23:14:01.084370 medicc2-1.0.2/
+-rw-r--r--   0 tom        (501) staff       (20)    36109 2023-05-23 14:44:50.000000 medicc2-1.0.2/LICENSE
+-rw-r--r--   0 tom        (501) staff       (20)    19922 2023-07-18 23:14:01.084097 medicc2-1.0.2/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)    19338 2023-07-17 15:27:43.000000 medicc2-1.0.2/README.md
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 23:14:01.056154 medicc2-1.0.2/fstlib/
+-rw-r--r--   0 tom        (501) staff       (20)      550 2023-05-24 13:14:05.000000 medicc2-1.0.2/fstlib/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)    15634 2023-05-24 13:14:05.000000 medicc2-1.0.2/fstlib/algos.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 23:14:01.068379 medicc2-1.0.2/fstlib/cext/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-07-18 13:55:35.000000 medicc2-1.0.2/fstlib/cext/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     2100 2023-07-18 13:55:35.000000 medicc2-1.0.2/fstlib/cext/cios.pxd
+-rw-r--r--   0 tom        (501) staff       (20)      869 2023-07-18 13:55:35.000000 medicc2-1.0.2/fstlib/cext/cmemory.pxd
+-rw-r--r--   0 tom        (501) staff       (20)    16320 2023-07-18 13:55:35.000000 medicc2-1.0.2/fstlib/cext/cops.h
+-rw-r--r--   0 tom        (501) staff       (20)     1018 2023-07-18 13:55:35.000000 medicc2-1.0.2/fstlib/cext/cops.pxd
+-rw-r--r--   0 tom        (501) staff       (20)    22785 2023-07-18 13:55:35.000000 medicc2-1.0.2/fstlib/cext/cpywrapfst.pxd
+-rw-r--r--   0 tom        (501) staff       (20)   288324 2023-07-18 23:13:59.000000 medicc2-1.0.2/fstlib/cext/ops.cpp
+-rw-r--r--   0 tom        (501) staff       (20)     2419 2023-07-18 13:55:35.000000 medicc2-1.0.2/fstlib/cext/ops.pyx
+-rw-r--r--   0 tom        (501) staff       (20)  2753477 2023-07-18 23:14:00.000000 medicc2-1.0.2/fstlib/cext/pywrapfst.cpp
+-rw-r--r--   0 tom        (501) staff       (20)    16028 2023-07-18 13:55:35.000000 medicc2-1.0.2/fstlib/cext/pywrapfst.pxd
+-rw-r--r--   0 tom        (501) staff       (20)   149233 2023-07-18 13:55:35.000000 medicc2-1.0.2/fstlib/cext/pywrapfst.pyx
+-rw-r--r--   0 tom        (501) staff       (20)    18739 2023-05-24 13:14:05.000000 medicc2-1.0.2/fstlib/core.py
+-rw-r--r--   0 tom        (501) staff       (20)     7036 2023-05-24 13:14:05.000000 medicc2-1.0.2/fstlib/ext.py
+-rw-r--r--   0 tom        (501) staff       (20)    10235 2023-05-24 13:14:05.000000 medicc2-1.0.2/fstlib/factory.py
+-rw-r--r--   0 tom        (501) staff       (20)      397 2023-05-23 14:44:52.000000 medicc2-1.0.2/fstlib/logging_conf.yaml
+-rw-r--r--   0 tom        (501) staff       (20)     2609 2023-05-24 13:14:05.000000 medicc2-1.0.2/fstlib/paths.py
+-rw-r--r--   0 tom        (501) staff       (20)     1446 2023-05-23 14:44:52.000000 medicc2-1.0.2/fstlib/test_fstlib.py
+-rw-r--r--   0 tom        (501) staff       (20)     5794 2023-05-24 13:14:05.000000 medicc2-1.0.2/fstlib/tools.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 23:14:01.074085 medicc2-1.0.2/medicc/
+-rw-r--r--   0 tom        (501) staff       (20)      629 2023-05-23 14:44:50.000000 medicc2-1.0.2/medicc/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     3540 2023-07-12 09:13:51.000000 medicc2-1.0.2/medicc/ancestors.py
+-rw-r--r--   0 tom        (501) staff       (20)    10115 2023-05-23 14:44:50.000000 medicc2-1.0.2/medicc/bootstrap.py
+-rw-r--r--   0 tom        (501) staff       (20)    20683 2023-07-17 15:38:29.000000 medicc2-1.0.2/medicc/core.py
+-rw-r--r--   0 tom        (501) staff       (20)    23763 2023-07-12 09:13:51.000000 medicc2-1.0.2/medicc/event_reconstruction.py
+-rw-r--r--   0 tom        (501) staff       (20)     8045 2023-07-12 09:13:51.000000 medicc2-1.0.2/medicc/factory.py
+-rw-r--r--   0 tom        (501) staff       (20)    15900 2023-07-17 15:27:37.000000 medicc2-1.0.2/medicc/io.py
+-rw-r--r--   0 tom        (501) staff       (20)      780 2023-05-23 14:44:50.000000 medicc2-1.0.2/medicc/logging_conf.yaml
+-rw-r--r--   0 tom        (501) staff       (20)     5483 2023-07-17 15:27:37.000000 medicc2-1.0.2/medicc/nj.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 23:14:01.081768 medicc2-1.0.2/medicc/objects/
+-rw-r--r--   0 tom        (501) staff       (20)    56129 2023-05-23 14:44:50.000000 medicc2-1.0.2/medicc/objects/Davoli_2013_TSG_OG_genes.bed
+-rw-r--r--   0 tom        (501) staff       (20)     1382 2023-05-23 14:44:50.000000 medicc2-1.0.2/medicc/objects/hg19_chromosome_arms.bed
+-rw-r--r--   0 tom        (501) staff       (20)     1382 2023-05-23 14:44:50.000000 medicc2-1.0.2/medicc/objects/hg38_chromosome_arms.bed
+-rw-r--r--   0 tom        (501) staff       (20)   253982 2023-05-24 23:42:20.000000 medicc2-1.0.2/medicc/objects/no_wgd_asymm.fst
+-rw-r--r--   0 tom        (501) staff       (20)   572114 2023-05-24 23:42:20.000000 medicc2-1.0.2/medicc/objects/wgd_1_asymm.fst
+-rw-r--r--   0 tom        (501) staff       (20)   689774 2023-05-24 23:42:20.000000 medicc2-1.0.2/medicc/objects/wgd_2_asymm.fst
+-rw-r--r--   0 tom        (501) staff       (20)   783870 2023-05-24 23:42:20.000000 medicc2-1.0.2/medicc/objects/wgd_asymm.fst
+-rw-r--r--   0 tom        (501) staff       (20)   546246 2023-05-24 23:42:20.000000 medicc2-1.0.2/medicc/objects/wgd_total_cn_1_asymm.fst
+-rw-r--r--   0 tom        (501) staff       (20)   656310 2023-05-24 23:42:20.000000 medicc2-1.0.2/medicc/objects/wgd_total_cn_asymm.fst
+-rw-r--r--   0 tom        (501) staff       (20)   519890 2023-05-24 23:42:20.000000 medicc2-1.0.2/medicc/objects/wgd_x2_1_asymm.fst
+-rw-r--r--   0 tom        (501) staff       (20)   591554 2023-05-24 23:42:20.000000 medicc2-1.0.2/medicc/objects/wgd_x2_asymm.fst
+-rw-r--r--   0 tom        (501) staff       (20)    42035 2023-07-18 12:30:05.000000 medicc2-1.0.2/medicc/plot.py
+-rw-r--r--   0 tom        (501) staff       (20)     7644 2023-07-17 15:27:37.000000 medicc2-1.0.2/medicc/sim.py
+-rw-r--r--   0 tom        (501) staff       (20)     2646 2023-05-23 14:44:50.000000 medicc2-1.0.2/medicc/stats.py
+-rw-r--r--   0 tom        (501) staff       (20)     4934 2023-05-23 14:44:50.000000 medicc2-1.0.2/medicc/test_fsts.py
+-rw-r--r--   0 tom        (501) staff       (20)    21224 2023-07-18 12:52:56.000000 medicc2-1.0.2/medicc/test_medicc.py
+-rw-r--r--   0 tom        (501) staff       (20)     5150 2023-07-17 15:34:04.000000 medicc2-1.0.2/medicc/tools.py
+-rw-r--r--   0 tom        (501) staff       (20)    14892 2023-07-17 15:35:57.000000 medicc2-1.0.2/medicc2
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 23:14:01.083772 medicc2-1.0.2/medicc2.egg-info/
+-rw-r--r--   0 tom        (501) staff       (20)    19922 2023-07-18 23:14:01.000000 medicc2-1.0.2/medicc2.egg-info/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)     1286 2023-07-18 23:14:01.000000 medicc2-1.0.2/medicc2.egg-info/SOURCES.txt
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-07-18 23:14:01.000000 medicc2-1.0.2/medicc2.egg-info/dependency_links.txt
+-rw-r--r--   0 tom        (501) staff       (20)      120 2023-07-18 23:14:01.000000 medicc2-1.0.2/medicc2.egg-info/requires.txt
+-rw-r--r--   0 tom        (501) staff       (20)       14 2023-07-18 23:14:01.000000 medicc2-1.0.2/medicc2.egg-info/top_level.txt
+-rw-r--r--   0 tom        (501) staff       (20)       78 2023-07-18 23:09:22.000000 medicc2-1.0.2/pyproject.toml
+-rw-r--r--   0 tom        (501) staff       (20)       38 2023-07-18 23:14:01.084434 medicc2-1.0.2/setup.cfg
+-rw-r--r--   0 tom        (501) staff       (20)     2169 2023-07-18 23:13:09.000000 medicc2-1.0.2/setup.py
```

### Comparing `medicc2-1.0.0/LICENSE` & `medicc2-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `medicc2-1.0.0/PKG-INFO` & `medicc2-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,20 @@
-Metadata-Version: 2.1
-Name: medicc2
-Version: 1.0.0
-Summary: Whole-genome doubling-aware copy number phylogenies for cancer evolution
-Home-page: https://bitbucket.org/schwarzlab/medicc2
-Author: Tom L Kaufmann, Marina Petkovic, Roland F Schwarz
-Author-email: tkau93@gmail.com, marina.55kovic@gmail.com, roland.f.schwarz@gmail.com
-License: GPL-3
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-Provides-Extra: Parallelization
-License-File: LICENSE
-
 # MEDICC2 - Whole-genome doubling-aware copy number phylogenies for cancer evolution
 
 [![PyPI](https://img.shields.io/pypi/v/medicc2?color=green)](https://pypi.org/project/medicc2/)
 [![Conda](https://img.shields.io/conda/v/bioconda/medicc2?color=green)](https://anaconda.org/bioconda/medicc2)
 
 For more information see the accompanying publication [Whole-genome doubling-aware copy number phylogenies for cancer evolution with MEDICC2](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-022-02794-9).
 
 # Installation
 Install MEDICC2 via conda (recommended), pip or from source. MEDICC2 was developed and tested on unix-built systems (Linux and MacOS). For Windows users we recommended WSL2.
 
-Note that the notebooks and examples are not included when installing from conda or pip. When installing from pip or source, you need to make sure to have a working version of `gcc` and `gxx` installed.
+Note that the notebooks and examples are not included when installing from conda or pip.
+
+For all installation methods you need to make sure to have a working version of the GNU Compiler Collection (`gcc`, `gxx` as well as related packages such as `libgcc-ng`) installed.
 
 
 ## Installation via conda (recommended)
 It is best to use a dedicated conda environment for your MEDICC2 installation with `conda create -n medicc_env`.
 
 After activating the environment with `conda activate medicc_env` you can install MEDICC2 via `conda install -c bioconda -c conda-forge medicc2`.
 
@@ -74,15 +61,15 @@
 * `--regions-bed`: BED file for regions of interest to compare copy-number events to
 * `-v`, `--verbose`: Enable verbose output. Default: False
 * `-vv`, `--debug`: Enable more verbose output Default: False
 * `--maxcn`: Expert option: maximum CN at which the input is capped. Does not change FST. Default: 8
 * `--prune-weight`: Expert option: Prune weight in ancestor reconstruction. Values >0 might result in more accurate ancestors but will require more time and memory. Default: 0
 * `--fst`: Expert option: path to an alternative FST. Default: None
 * `--fst-chr-separator`: Expert option: character used to separate chromosomes in the FST. Default: 'X'
-* `--wgd_x2`: Expert option: Treat WGD as a x2 operation. Default: False
+* `--wgd-x2`: Expert option: Treat WGD as a x2 operation. Default: False
 
 
 ## Input files
 Input files can be either in fasta or tsv format:
 
 * **tsv (recommended):** Files should have the following columns: `sample_id`, `chrom`, `start`, `end` as well as columns for the copy numbers. MEDICC expects the copy number columns to be called `cn_a` and `cn_b`. Using the flag `--input-allele-columns` you can set your own copy number columns. If you want to use total copy numbers, make sure to use the flag `--total-copy-numbers`. Important: MEDICC2 does not create total copy numbers for you. You will have to calculate total copy numbers yourself and then specify the column using the `--input-allele-columns` flag.
 * **fasta:** A description file should be provided to MEDICC. This file should include one line per file with the name of the chromosome and the corresponding file names. If fasta files are provided you have to use the flag `--input-type fasta`.
@@ -97,14 +84,15 @@
 MEDICC creates the following output files:
 
 * `_final_tree.new`, `_final_tree.xml`, `_final_tree.png`: The final phylogenetic tree in Newick and XML format as well as an image
 * `_pairwise_distances.tsv`: A NxN matrix (N being the number of samples) of pairwise distances calculated with the symmetric MEDICC2 distance
 * `_final_cn_profiles.tsv`: Copy-number profiles of the input as well as the newly internal nodes. Also includes additional information such as whether a gain or loss has happened
 * `_cn_profiles.pdf`: Combined plot of the phylogenetic tree as well as the copy-number profiles of all samples (including the internal nodes)
 * `_branch_lengths.tsv`: List of all branches and their corresponding lenghts of the final tree
+* `_summary.tsv`: Contains summary information about the created tree. If the `--events` flag was set, this includes the WGD status.
 
 *optional (see "Event Reconstruction" below)*
 
 * `_copynumber_events_df.tsv`: List of all copy-number events detected. The entries for WGD events have non-meaningful values for chrom, cn_child, etc. Note that the events derived are not unambiguous.
 * `_events_overlap.tsv`: Overlap of copy-number events with regions of interest
 
 
@@ -151,15 +139,15 @@
 MEDICCC2 can overlap the inferred events with regions of interest such as chromosome arms or oncogenes. 
 This process requires the installation of `pyranges` which might be incompatible with newer version of python and/or numpy.
 The overlap is turned off by default. You can turn on the overlapping with the ``--chromosomes-bed` and `--regions-bed` flag by providing bed-files with regions of interest. By default MEDICC2 uses hg38 chromosome-arms and a list of genes taken from Davoli et al. Cell 2013. This data is present as BED files in the `medicc/objects` folder. Invoke these using the flags `--chromosomes-bed "default"` and/or `--regions-bed "default"`.
 Users can specify regions of interest of their own in BED format by providing the `--chromosomes-bed` or `--regions-bed` flags.
 
 
 ## Single sample WGD detection
-If you are interested in the WGD status of individual samples in your data, have a look at the notebook `notebooks/single_sample_wgd_detection.py`. By replacing the input data with your data you can easily calculate the WGD status of any copy-number input.
+If you are interested in the WGD status of individual samples in your data, have a look at the notebook `notebooks/WGD_detection.ipynb`. By replacing the input data with your data you can easily calculate the WGD status of any copy-number input.
 
 
 # Issues
 If you experience problems with MEDICC2 please [file an issue directly on Bitbucket](https://bitbucket.org/schwarzlab/medicc2/issues/new) or [contact us directly](tom.kaufmann@mdc-berlin.de). 
 
 ## Known Issues
```

### Comparing `medicc2-1.0.0/README.md` & `medicc2-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,35 @@
+Metadata-Version: 2.1
+Name: medicc2
+Version: 1.0.2
+Summary: Whole-genome doubling-aware copy number phylogenies for cancer evolution
+Home-page: https://bitbucket.org/schwarzlab/medicc2
+Author: Tom L Kaufmann, Marina Petkovic, Roland F Schwarz
+Author-email: tkau93@gmail.com, marina.55kovic@gmail.com, roland.f.schwarz@gmail.com
+License: GPL-3
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+Provides-Extra: Parallelization
+License-File: LICENSE
+
 # MEDICC2 - Whole-genome doubling-aware copy number phylogenies for cancer evolution
 
 [![PyPI](https://img.shields.io/pypi/v/medicc2?color=green)](https://pypi.org/project/medicc2/)
 [![Conda](https://img.shields.io/conda/v/bioconda/medicc2?color=green)](https://anaconda.org/bioconda/medicc2)
 
 For more information see the accompanying publication [Whole-genome doubling-aware copy number phylogenies for cancer evolution with MEDICC2](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-022-02794-9).
 
 # Installation
 Install MEDICC2 via conda (recommended), pip or from source. MEDICC2 was developed and tested on unix-built systems (Linux and MacOS). For Windows users we recommended WSL2.
 
-Note that the notebooks and examples are not included when installing from conda or pip. When installing from pip or source, you need to make sure to have a working version of `gcc` and `gxx` installed.
+Note that the notebooks and examples are not included when installing from conda or pip.
+
+For all installation methods you need to make sure to have a working version of the GNU Compiler Collection (`gcc`, `gxx` as well as related packages such as `libgcc-ng`) installed.
 
 
 ## Installation via conda (recommended)
 It is best to use a dedicated conda environment for your MEDICC2 installation with `conda create -n medicc_env`.
 
 After activating the environment with `conda activate medicc_env` you can install MEDICC2 via `conda install -c bioconda -c conda-forge medicc2`.
 
@@ -59,15 +76,15 @@
 * `--regions-bed`: BED file for regions of interest to compare copy-number events to
 * `-v`, `--verbose`: Enable verbose output. Default: False
 * `-vv`, `--debug`: Enable more verbose output Default: False
 * `--maxcn`: Expert option: maximum CN at which the input is capped. Does not change FST. Default: 8
 * `--prune-weight`: Expert option: Prune weight in ancestor reconstruction. Values >0 might result in more accurate ancestors but will require more time and memory. Default: 0
 * `--fst`: Expert option: path to an alternative FST. Default: None
 * `--fst-chr-separator`: Expert option: character used to separate chromosomes in the FST. Default: 'X'
-* `--wgd_x2`: Expert option: Treat WGD as a x2 operation. Default: False
+* `--wgd-x2`: Expert option: Treat WGD as a x2 operation. Default: False
 
 
 ## Input files
 Input files can be either in fasta or tsv format:
 
 * **tsv (recommended):** Files should have the following columns: `sample_id`, `chrom`, `start`, `end` as well as columns for the copy numbers. MEDICC expects the copy number columns to be called `cn_a` and `cn_b`. Using the flag `--input-allele-columns` you can set your own copy number columns. If you want to use total copy numbers, make sure to use the flag `--total-copy-numbers`. Important: MEDICC2 does not create total copy numbers for you. You will have to calculate total copy numbers yourself and then specify the column using the `--input-allele-columns` flag.
 * **fasta:** A description file should be provided to MEDICC. This file should include one line per file with the name of the chromosome and the corresponding file names. If fasta files are provided you have to use the flag `--input-type fasta`.
@@ -82,14 +99,15 @@
 MEDICC creates the following output files:
 
 * `_final_tree.new`, `_final_tree.xml`, `_final_tree.png`: The final phylogenetic tree in Newick and XML format as well as an image
 * `_pairwise_distances.tsv`: A NxN matrix (N being the number of samples) of pairwise distances calculated with the symmetric MEDICC2 distance
 * `_final_cn_profiles.tsv`: Copy-number profiles of the input as well as the newly internal nodes. Also includes additional information such as whether a gain or loss has happened
 * `_cn_profiles.pdf`: Combined plot of the phylogenetic tree as well as the copy-number profiles of all samples (including the internal nodes)
 * `_branch_lengths.tsv`: List of all branches and their corresponding lenghts of the final tree
+* `_summary.tsv`: Contains summary information about the created tree. If the `--events` flag was set, this includes the WGD status.
 
 *optional (see "Event Reconstruction" below)*
 
 * `_copynumber_events_df.tsv`: List of all copy-number events detected. The entries for WGD events have non-meaningful values for chrom, cn_child, etc. Note that the events derived are not unambiguous.
 * `_events_overlap.tsv`: Overlap of copy-number events with regions of interest
 
 
@@ -136,15 +154,15 @@
 MEDICCC2 can overlap the inferred events with regions of interest such as chromosome arms or oncogenes. 
 This process requires the installation of `pyranges` which might be incompatible with newer version of python and/or numpy.
 The overlap is turned off by default. You can turn on the overlapping with the ``--chromosomes-bed` and `--regions-bed` flag by providing bed-files with regions of interest. By default MEDICC2 uses hg38 chromosome-arms and a list of genes taken from Davoli et al. Cell 2013. This data is present as BED files in the `medicc/objects` folder. Invoke these using the flags `--chromosomes-bed "default"` and/or `--regions-bed "default"`.
 Users can specify regions of interest of their own in BED format by providing the `--chromosomes-bed` or `--regions-bed` flags.
 
 
 ## Single sample WGD detection
-If you are interested in the WGD status of individual samples in your data, have a look at the notebook `notebooks/single_sample_wgd_detection.py`. By replacing the input data with your data you can easily calculate the WGD status of any copy-number input.
+If you are interested in the WGD status of individual samples in your data, have a look at the notebook `notebooks/WGD_detection.ipynb`. By replacing the input data with your data you can easily calculate the WGD status of any copy-number input.
 
 
 # Issues
 If you experience problems with MEDICC2 please [file an issue directly on Bitbucket](https://bitbucket.org/schwarzlab/medicc2/issues/new) or [contact us directly](tom.kaufmann@mdc-berlin.de). 
 
 ## Known Issues
```

### Comparing `medicc2-1.0.0/fstlib/__init__.py` & `medicc2-1.0.2/fstlib/__init__.py`

 * *Files identical despite different names*

### Comparing `medicc2-1.0.0/fstlib/algos.py` & `medicc2-1.0.2/fstlib/algos.py`

 * *Files identical despite different names*

### Comparing `medicc2-1.0.0/fstlib/cext/cios.pxd` & `medicc2-1.0.2/fstlib/cext/cios.pxd`

 * *Files identical despite different names*

### Comparing `medicc2-1.0.0/fstlib/cext/cmemory.pxd` & `medicc2-1.0.2/fstlib/cext/cmemory.pxd`

 * *Files identical despite different names*

### Comparing `medicc2-1.0.0/fstlib/cext/cops.h` & `medicc2-1.0.2/fstlib/cext/cops.h`

 * *Files identical despite different names*

### Comparing `medicc2-1.0.0/fstlib/cext/cops.pxd` & `medicc2-1.0.2/fstlib/cext/cops.pxd`

 * *Files identical despite different names*

### Comparing `medicc2-1.0.0/fstlib/cext/cpywrapfst.pxd` & `medicc2-1.0.2/fstlib/cext/cpywrapfst.pxd`

 * *Files identical despite different names*

### Comparing `medicc2-1.0.0/fstlib/cext/ops.cpp` & `medicc2-1.0.2/fstlib/cext/ops.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.34 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "fstlib/cext/cops.h"
         ],
@@ -36,16 +36,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_34"
-#define CYTHON_HEX_VERSION 0x001D22F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -105,18 +105,22 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -406,17 +410,14 @@
     operator T&() { return *ptr; }
     template<typename U> bool operator ==(U other) { return *ptr == other; }
     template<typename U> bool operator !=(U other) { return *ptr != other; }
   private:
     T *ptr;
 };
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -486,14 +487,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -2400,30 +2406,30 @@
 /* ArgTypeTest.proto */
 #define __Pyx_ArgTypeTest(obj, type, none_allowed, name, exact)\
     ((likely((Py_TYPE(obj) == type) | (none_allowed && (obj == Py_None)))) ? 1 :\
         __Pyx__ArgTypeTest(obj, type, name, exact))
 static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_36
+#define __PYX_HAVE_RT_ImportType_proto_0_29_36
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+enum __Pyx_ImportType_CheckSize_0_29_36 {
+   __Pyx_ImportType_CheckSize_Error_0_29_36 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_36 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_36 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size);
 #endif
 
 /* GetVTable.proto */
 static void* __Pyx_GetVtable(PyObject *dict);
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
@@ -2546,15 +2552,15 @@
 #endif
 #define __Pyx_PyException_Check(obj) __Pyx_TypeCheck(obj, PyExc_Exception)
 
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* FunctionImport.proto */
-static int __Pyx_ImportFunction(PyObject *module, const char *funcname, void (**f)(void), const char *sig);
+static int __Pyx_ImportFunction_0_29_36(PyObject *module, const char *funcname, void (**f)(void), const char *sig);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 
 /* Module declarations from 'libcpp.vector' */
 
@@ -4712,88 +4718,50 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule("fstlib.cext.pywrapfst"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 71, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_6fstlib_4cext_9pywrapfst_Weight = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "Weight", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst_Weight), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_6fstlib_4cext_9pywrapfst_Weight),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_6fstlib_4cext_9pywrapfst_Weight) __PYX_ERR(2, 71, __pyx_L1_error)
+  __pyx_ptype_6fstlib_4cext_9pywrapfst_Weight = __Pyx_ImportType_0_29_36(__pyx_t_1, "fstlib.cext.pywrapfst", "Weight", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst_Weight), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_6fstlib_4cext_9pywrapfst_Weight),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_6fstlib_4cext_9pywrapfst_Weight) __PYX_ERR(2, 71, __pyx_L1_error)
   __pyx_vtabptr_6fstlib_4cext_9pywrapfst_Weight = (struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst_Weight*)__Pyx_GetVtable(__pyx_ptype_6fstlib_4cext_9pywrapfst_Weight->tp_dict); if (unlikely(!__pyx_vtabptr_6fstlib_4cext_9pywrapfst_Weight)) __PYX_ERR(2, 71, __pyx_L1_error)
-  __pyx_ptype_6fstlib_4cext_9pywrapfst_SymbolTableView = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "SymbolTableView", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst_SymbolTableView), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_6fstlib_4cext_9pywrapfst_SymbolTableView),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_6fstlib_4cext_9pywrapfst_SymbolTableView) __PYX_ERR(2, 107, __pyx_L1_error)
+  __pyx_ptype_6fstlib_4cext_9pywrapfst_SymbolTableView = __Pyx_ImportType_0_29_36(__pyx_t_1, "fstlib.cext.pywrapfst", "SymbolTableView", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst_SymbolTableView), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_6fstlib_4cext_9pywrapfst_SymbolTableView),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_6fstlib_4cext_9pywrapfst_SymbolTableView) __PYX_ERR(2, 107, __pyx_L1_error)
   __pyx_vtabptr_6fstlib_4cext_9pywrapfst_SymbolTableView = (struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst_SymbolTableView*)__Pyx_GetVtable(__pyx_ptype_6fstlib_4cext_9pywrapfst_SymbolTableView->tp_dict); if (unlikely(!__pyx_vtabptr_6fstlib_4cext_9pywrapfst_SymbolTableView)) __PYX_ERR(2, 107, __pyx_L1_error)
-  __pyx_ptype_6fstlib_4cext_9pywrapfst__EncodeMapperSymbolTableView = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "_EncodeMapperSymbolTableView", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst__EncodeMapperSymbolTableView), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_6fstlib_4cext_9pywrapfst__EncodeMapperSymbolTableView),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_6fstlib_4cext_9pywrapfst__EncodeMapperSymbolTableView) __PYX_ERR(2, 138, __pyx_L1_error)
+  __pyx_ptype_6fstlib_4cext_9pywrapfst__EncodeMapperSymbolTableView = __Pyx_ImportType_0_29_36(__pyx_t_1, "fstlib.cext.pywrapfst", "_EncodeMapperSymbolTableView", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst__EncodeMapperSymbolTableView), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_6fstlib_4cext_9pywrapfst__EncodeMapperSymbolTableView),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_6fstlib_4cext_9pywrapfst__EncodeMapperSymbolTableView) __PYX_ERR(2, 138, __pyx_L1_error)
   __pyx_vtabptr_6fstlib_4cext_9pywrapfst__EncodeMapperSymbolTableView = (struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst__EncodeMapperSymbolTableView*)__Pyx_GetVtable(__pyx_ptype_6fstlib_4cext_9pywrapfst__EncodeMapperSymbolTableView->tp_dict); if (unlikely(!__pyx_vtabptr_6fstlib_4cext_9pywrapfst__EncodeMapperSymbolTableView)) __PYX_ERR(2, 138, __pyx_L1_error)
-  __pyx_ptype_6fstlib_4cext_9pywrapfst__FstSymbolTableView = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "_FstSymbolTableView", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst__FstSymbolTableView), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_6fstlib_4cext_9pywrapfst__FstSymbolTableView),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_6fstlib_4cext_9pywrapfst__FstSymbolTableView) __PYX_ERR(2, 146, __pyx_L1_error)
+  __pyx_ptype_6fstlib_4cext_9pywrapfst__FstSymbolTableView = __Pyx_ImportType_0_29_36(__pyx_t_1, "fstlib.cext.pywrapfst", "_FstSymbolTableView", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst__FstSymbolTableView), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_6fstlib_4cext_9pywrapfst__FstSymbolTableView),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_6fstlib_4cext_9pywrapfst__FstSymbolTableView) __PYX_ERR(2, 146, __pyx_L1_error)
   __pyx_vtabptr_6fstlib_4cext_9pywrapfst__FstSymbolTableView = (struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst__FstSymbolTableView*)__Pyx_GetVtable(__pyx_ptype_6fstlib_4cext_9pywrapfst__FstSymbolTableView->tp_dict); if (unlikely(!__pyx_vtabptr_6fstlib_4cext_9pywrapfst__FstSymbolTableView)) __PYX_ERR(2, 146, __pyx_L1_error)
-  __pyx_ptype_6fstlib_4cext_9pywrapfst__MutableSymbolTable = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "_MutableSymbolTable", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst__MutableSymbolTable), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_6fstlib_4cext_9pywrapfst__MutableSymbolTable),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_6fstlib_4cext_9pywrapfst__MutableSymbolTable) __PYX_ERR(2, 154, __pyx_L1_error)
+  __pyx_ptype_6fstlib_4cext_9pywrapfst__MutableSymbolTable = __Pyx_ImportType_0_29_36(__pyx_t_1, "fstlib.cext.pywrapfst", "_MutableSymbolTable", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst__MutableSymbolTable), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_6fstlib_4cext_9pywrapfst__MutableSymbolTable),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_6fstlib_4cext_9pywrapfst__MutableSymbolTable) __PYX_ERR(2, 154, __pyx_L1_error)
   __pyx_vtabptr_6fstlib_4cext_9pywrapfst__MutableSymbolTable = (struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst__MutableSymbolTable*)__Pyx_GetVtable(__pyx_ptype_6fstlib_4cext_9pywrapfst__MutableSymbolTable->tp_dict); if (unlikely(!__pyx_vtabptr_6fstlib_4cext_9pywrapfst__MutableSymbolTable)) __PYX_ERR(2, 154, __pyx_L1_error)
-  __pyx_ptype_6fstlib_4cext_9pywrapfst__MutableFstSymbolTableView = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "_MutableFstSymbolTableView", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst__MutableFstSymbolTableView), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_6fstlib_4cext_9pywrapfst__MutableFstSymbolTableView),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_6fstlib_4cext_9pywrapfst__MutableFstSymbolTableView) __PYX_ERR(2, 167, __pyx_L1_error)
+  __pyx_ptype_6fstlib_4cext_9pywrapfst__MutableFstSymbolTableView = __Pyx_ImportType_0_29_36(__pyx_t_1, "fstlib.cext.pywrapfst", "_MutableFstSymbolTableView", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst__MutableFstSymbolTableView), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_6fstlib_4cext_9pywrapfst__MutableFstSymbolTableView),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_6fstlib_4cext_9pywrapfst__MutableFstSymbolTableView) __PYX_ERR(2, 167, __pyx_L1_error)
   __pyx_vtabptr_6fstlib_4cext_9pywrapfst__MutableFstSymbolTableView = (struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst__MutableFstSymbolTableView*)__Pyx_GetVtable(__pyx_ptype_6fstlib_4cext_9pywrapfst__MutableFstSymbolTableView->tp_dict); if (unlikely(!__pyx_vtabptr_6fstlib_4cext_9pywrapfst__MutableFstSymbolTableView)) __PYX_ERR(2, 167, __pyx_L1_error)
-  __pyx_ptype_6fstlib_4cext_9pywrapfst_SymbolTable = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "SymbolTable", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst_SymbolTable), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_6fstlib_4cext_9pywrapfst_SymbolTable),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_6fstlib_4cext_9pywrapfst_SymbolTable) __PYX_ERR(2, 175, __pyx_L1_error)
+  __pyx_ptype_6fstlib_4cext_9pywrapfst_SymbolTable = __Pyx_ImportType_0_29_36(__pyx_t_1, "fstlib.cext.pywrapfst", "SymbolTable", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst_SymbolTable), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_6fstlib_4cext_9pywrapfst_SymbolTable),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_6fstlib_4cext_9pywrapfst_SymbolTable) __PYX_ERR(2, 175, __pyx_L1_error)
   __pyx_vtabptr_6fstlib_4cext_9pywrapfst_SymbolTable = (struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst_SymbolTable*)__Pyx_GetVtable(__pyx_ptype_6fstlib_4cext_9pywrapfst_SymbolTable->tp_dict); if (unlikely(!__pyx_vtabptr_6fstlib_4cext_9pywrapfst_SymbolTable)) __PYX_ERR(2, 175, __pyx_L1_error)
-  __pyx_ptype_6fstlib_4cext_9pywrapfst__SymbolTableIterator = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "_SymbolTableIterator", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst__SymbolTableIterator), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_6fstlib_4cext_9pywrapfst__SymbolTableIterator),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_6fstlib_4cext_9pywrapfst__SymbolTableIterator) __PYX_ERR(2, 198, __pyx_L1_error)
-  __pyx_ptype_6fstlib_4cext_9pywrapfst_EncodeMapper = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "EncodeMapper", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst_EncodeMapper), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_6fstlib_4cext_9pywrapfst_EncodeMapper),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_6fstlib_4cext_9pywrapfst_EncodeMapper) __PYX_ERR(2, 210, __pyx_L1_error)
+  __pyx_ptype_6fstlib_4cext_9pywrapfst__SymbolTableIterator = __Pyx_ImportType_0_29_36(__pyx_t_1, "fstlib.cext.pywrapfst", "_SymbolTableIterator", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst__SymbolTableIterator), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_6fstlib_4cext_9pywrapfst__SymbolTableIterator),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_6fstlib_4cext_9pywrapfst__SymbolTableIterator) __PYX_ERR(2, 198, __pyx_L1_error)
+  __pyx_ptype_6fstlib_4cext_9pywrapfst_EncodeMapper = __Pyx_ImportType_0_29_36(__pyx_t_1, "fstlib.cext.pywrapfst", "EncodeMapper", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst_EncodeMapper), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_6fstlib_4cext_9pywrapfst_EncodeMapper),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_6fstlib_4cext_9pywrapfst_EncodeMapper) __PYX_ERR(2, 210, __pyx_L1_error)
   __pyx_vtabptr_6fstlib_4cext_9pywrapfst_EncodeMapper = (struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst_EncodeMapper*)__Pyx_GetVtable(__pyx_ptype_6fstlib_4cext_9pywrapfst_EncodeMapper->tp_dict); if (unlikely(!__pyx_vtabptr_6fstlib_4cext_9pywrapfst_EncodeMapper)) __PYX_ERR(2, 210, __pyx_L1_error)
-  __pyx_ptype_6fstlib_4cext_9pywrapfst_Fst = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "Fst", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst_Fst), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_6fstlib_4cext_9pywrapfst_Fst),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_6fstlib_4cext_9pywrapfst_Fst) __PYX_ERR(2, 247, __pyx_L1_error)
+  __pyx_ptype_6fstlib_4cext_9pywrapfst_Fst = __Pyx_ImportType_0_29_36(__pyx_t_1, "fstlib.cext.pywrapfst", "Fst", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst_Fst), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_6fstlib_4cext_9pywrapfst_Fst),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_6fstlib_4cext_9pywrapfst_Fst) __PYX_ERR(2, 247, __pyx_L1_error)
   __pyx_vtabptr_6fstlib_4cext_9pywrapfst_Fst = (struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst_Fst*)__Pyx_GetVtable(__pyx_ptype_6fstlib_4cext_9pywrapfst_Fst->tp_dict); if (unlikely(!__pyx_vtabptr_6fstlib_4cext_9pywrapfst_Fst)) __PYX_ERR(2, 247, __pyx_L1_error)
-  __pyx_ptype_6fstlib_4cext_9pywrapfst_MutableFst = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "MutableFst", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst_MutableFst), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_6fstlib_4cext_9pywrapfst_MutableFst),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_6fstlib_4cext_9pywrapfst_MutableFst) __PYX_ERR(2, 313, __pyx_L1_error)
+  __pyx_ptype_6fstlib_4cext_9pywrapfst_MutableFst = __Pyx_ImportType_0_29_36(__pyx_t_1, "fstlib.cext.pywrapfst", "MutableFst", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst_MutableFst), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_6fstlib_4cext_9pywrapfst_MutableFst),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_6fstlib_4cext_9pywrapfst_MutableFst) __PYX_ERR(2, 313, __pyx_L1_error)
   __pyx_vtabptr_6fstlib_4cext_9pywrapfst_MutableFst = (struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst_MutableFst*)__Pyx_GetVtable(__pyx_ptype_6fstlib_4cext_9pywrapfst_MutableFst->tp_dict); if (unlikely(!__pyx_vtabptr_6fstlib_4cext_9pywrapfst_MutableFst)) __PYX_ERR(2, 313, __pyx_L1_error)
-  __pyx_ptype_6fstlib_4cext_9pywrapfst_VectorFst = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "VectorFst", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst_VectorFst), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_6fstlib_4cext_9pywrapfst_VectorFst),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_6fstlib_4cext_9pywrapfst_VectorFst) __PYX_ERR(2, 394, __pyx_L1_error)
+  __pyx_ptype_6fstlib_4cext_9pywrapfst_VectorFst = __Pyx_ImportType_0_29_36(__pyx_t_1, "fstlib.cext.pywrapfst", "VectorFst", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst_VectorFst), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_6fstlib_4cext_9pywrapfst_VectorFst),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_6fstlib_4cext_9pywrapfst_VectorFst) __PYX_ERR(2, 394, __pyx_L1_error)
   __pyx_vtabptr_6fstlib_4cext_9pywrapfst_VectorFst = (struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst_VectorFst*)__Pyx_GetVtable(__pyx_ptype_6fstlib_4cext_9pywrapfst_VectorFst->tp_dict); if (unlikely(!__pyx_vtabptr_6fstlib_4cext_9pywrapfst_VectorFst)) __PYX_ERR(2, 394, __pyx_L1_error)
-  __pyx_ptype_6fstlib_4cext_9pywrapfst_Arc = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "Arc", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst_Arc), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_6fstlib_4cext_9pywrapfst_Arc),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_6fstlib_4cext_9pywrapfst_Arc) __PYX_ERR(2, 416, __pyx_L1_error)
+  __pyx_ptype_6fstlib_4cext_9pywrapfst_Arc = __Pyx_ImportType_0_29_36(__pyx_t_1, "fstlib.cext.pywrapfst", "Arc", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst_Arc), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_6fstlib_4cext_9pywrapfst_Arc),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_6fstlib_4cext_9pywrapfst_Arc) __PYX_ERR(2, 416, __pyx_L1_error)
   __pyx_vtabptr_6fstlib_4cext_9pywrapfst_Arc = (struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst_Arc*)__Pyx_GetVtable(__pyx_ptype_6fstlib_4cext_9pywrapfst_Arc->tp_dict); if (unlikely(!__pyx_vtabptr_6fstlib_4cext_9pywrapfst_Arc)) __PYX_ERR(2, 416, __pyx_L1_error)
-  __pyx_ptype_6fstlib_4cext_9pywrapfst__ArcIterator = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "_ArcIterator", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst__ArcIterator), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_6fstlib_4cext_9pywrapfst__ArcIterator),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_6fstlib_4cext_9pywrapfst__ArcIterator) __PYX_ERR(2, 426, __pyx_L1_error)
+  __pyx_ptype_6fstlib_4cext_9pywrapfst__ArcIterator = __Pyx_ImportType_0_29_36(__pyx_t_1, "fstlib.cext.pywrapfst", "_ArcIterator", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst__ArcIterator), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_6fstlib_4cext_9pywrapfst__ArcIterator),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_6fstlib_4cext_9pywrapfst__ArcIterator) __PYX_ERR(2, 426, __pyx_L1_error)
   __pyx_vtabptr_6fstlib_4cext_9pywrapfst__ArcIterator = (struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst__ArcIterator*)__Pyx_GetVtable(__pyx_ptype_6fstlib_4cext_9pywrapfst__ArcIterator->tp_dict); if (unlikely(!__pyx_vtabptr_6fstlib_4cext_9pywrapfst__ArcIterator)) __PYX_ERR(2, 426, __pyx_L1_error)
-  __pyx_ptype_6fstlib_4cext_9pywrapfst__MutableArcIterator = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "_MutableArcIterator", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst__MutableArcIterator), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_6fstlib_4cext_9pywrapfst__MutableArcIterator),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_6fstlib_4cext_9pywrapfst__MutableArcIterator) __PYX_ERR(2, 448, __pyx_L1_error)
+  __pyx_ptype_6fstlib_4cext_9pywrapfst__MutableArcIterator = __Pyx_ImportType_0_29_36(__pyx_t_1, "fstlib.cext.pywrapfst", "_MutableArcIterator", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst__MutableArcIterator), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_6fstlib_4cext_9pywrapfst__MutableArcIterator),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_6fstlib_4cext_9pywrapfst__MutableArcIterator) __PYX_ERR(2, 448, __pyx_L1_error)
   __pyx_vtabptr_6fstlib_4cext_9pywrapfst__MutableArcIterator = (struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst__MutableArcIterator*)__Pyx_GetVtable(__pyx_ptype_6fstlib_4cext_9pywrapfst__MutableArcIterator->tp_dict); if (unlikely(!__pyx_vtabptr_6fstlib_4cext_9pywrapfst__MutableArcIterator)) __PYX_ERR(2, 448, __pyx_L1_error)
-  __pyx_ptype_6fstlib_4cext_9pywrapfst__StateIterator = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "_StateIterator", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst__StateIterator), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_6fstlib_4cext_9pywrapfst__StateIterator),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_6fstlib_4cext_9pywrapfst__StateIterator) __PYX_ERR(2, 472, __pyx_L1_error)
+  __pyx_ptype_6fstlib_4cext_9pywrapfst__StateIterator = __Pyx_ImportType_0_29_36(__pyx_t_1, "fstlib.cext.pywrapfst", "_StateIterator", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst__StateIterator), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_6fstlib_4cext_9pywrapfst__StateIterator),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_6fstlib_4cext_9pywrapfst__StateIterator) __PYX_ERR(2, 472, __pyx_L1_error)
   __pyx_vtabptr_6fstlib_4cext_9pywrapfst__StateIterator = (struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst__StateIterator*)__Pyx_GetVtable(__pyx_ptype_6fstlib_4cext_9pywrapfst__StateIterator->tp_dict); if (unlikely(!__pyx_vtabptr_6fstlib_4cext_9pywrapfst__StateIterator)) __PYX_ERR(2, 472, __pyx_L1_error)
-  __pyx_ptype_6fstlib_4cext_9pywrapfst_Compiler = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "Compiler", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst_Compiler), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_6fstlib_4cext_9pywrapfst_Compiler),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_6fstlib_4cext_9pywrapfst_Compiler) __PYX_ERR(2, 594, __pyx_L1_error)
+  __pyx_ptype_6fstlib_4cext_9pywrapfst_Compiler = __Pyx_ImportType_0_29_36(__pyx_t_1, "fstlib.cext.pywrapfst", "Compiler", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst_Compiler), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_6fstlib_4cext_9pywrapfst_Compiler),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_6fstlib_4cext_9pywrapfst_Compiler) __PYX_ERR(2, 594, __pyx_L1_error)
   __pyx_vtabptr_6fstlib_4cext_9pywrapfst_Compiler = (struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst_Compiler*)__Pyx_GetVtable(__pyx_ptype_6fstlib_4cext_9pywrapfst_Compiler->tp_dict); if (unlikely(!__pyx_vtabptr_6fstlib_4cext_9pywrapfst_Compiler)) __PYX_ERR(2, 594, __pyx_L1_error)
-  __pyx_ptype_6fstlib_4cext_9pywrapfst_FarReader = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "FarReader", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst_FarReader), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_6fstlib_4cext_9pywrapfst_FarReader),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_6fstlib_4cext_9pywrapfst_FarReader) __PYX_ERR(2, 615, __pyx_L1_error)
+  __pyx_ptype_6fstlib_4cext_9pywrapfst_FarReader = __Pyx_ImportType_0_29_36(__pyx_t_1, "fstlib.cext.pywrapfst", "FarReader", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst_FarReader), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_6fstlib_4cext_9pywrapfst_FarReader),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_6fstlib_4cext_9pywrapfst_FarReader) __PYX_ERR(2, 615, __pyx_L1_error)
   __pyx_vtabptr_6fstlib_4cext_9pywrapfst_FarReader = (struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst_FarReader*)__Pyx_GetVtable(__pyx_ptype_6fstlib_4cext_9pywrapfst_FarReader->tp_dict); if (unlikely(!__pyx_vtabptr_6fstlib_4cext_9pywrapfst_FarReader)) __PYX_ERR(2, 615, __pyx_L1_error)
-  __pyx_ptype_6fstlib_4cext_9pywrapfst_FarWriter = __Pyx_ImportType(__pyx_t_1, "fstlib.cext.pywrapfst", "FarWriter", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst_FarWriter), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_6fstlib_4cext_9pywrapfst_FarWriter),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_6fstlib_4cext_9pywrapfst_FarWriter) __PYX_ERR(2, 640, __pyx_L1_error)
+  __pyx_ptype_6fstlib_4cext_9pywrapfst_FarWriter = __Pyx_ImportType_0_29_36(__pyx_t_1, "fstlib.cext.pywrapfst", "FarWriter", sizeof(struct __pyx_obj_6fstlib_4cext_9pywrapfst_FarWriter), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_6fstlib_4cext_9pywrapfst_FarWriter),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_6fstlib_4cext_9pywrapfst_FarWriter) __PYX_ERR(2, 640, __pyx_L1_error)
   __pyx_vtabptr_6fstlib_4cext_9pywrapfst_FarWriter = (struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst_FarWriter*)__Pyx_GetVtable(__pyx_ptype_6fstlib_4cext_9pywrapfst_FarWriter->tp_dict); if (unlikely(!__pyx_vtabptr_6fstlib_4cext_9pywrapfst_FarWriter)) __PYX_ERR(2, 640, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -4814,15 +4782,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_import_code", 0);
   /*--- Function import code ---*/
   __pyx_t_1 = PyImport_ImportModule("fstlib.cext.pywrapfst"); if (!__pyx_t_1) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_ImportFunction(__pyx_t_1, "_init_MutableFst", (void (**)(void))&__pyx_f_6fstlib_4cext_9pywrapfst__init_MutableFst, "struct __pyx_obj_6fstlib_4cext_9pywrapfst_MutableFst *(__pyx_t_6fstlib_4cext_9pywrapfst_MutableFstClass_ptr)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "_init_MutableFst", (void (**)(void))&__pyx_f_6fstlib_4cext_9pywrapfst__init_MutableFst, "struct __pyx_obj_6fstlib_4cext_9pywrapfst_MutableFst *(__pyx_t_6fstlib_4cext_9pywrapfst_MutableFstClass_ptr)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -5344,18 +5312,18 @@
     PyErr_Format(PyExc_TypeError,
         "Argument '%.200s' has incorrect type (expected %.200s, got %.200s)",
         name, type->tp_name, Py_TYPE(obj)->tp_name);
     return 0;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
+#ifndef __PYX_HAVE_RT_ImportType_0_29_36
+#define __PYX_HAVE_RT_ImportType_0_29_36
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -5401,22 +5369,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_36 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_36 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -5906,15 +5874,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -6102,15 +6070,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -6377,17 +6345,17 @@
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
 }
 
 /* FunctionImport */
-#ifndef __PYX_HAVE_RT_ImportFunction
-#define __PYX_HAVE_RT_ImportFunction
-static int __Pyx_ImportFunction(PyObject *module, const char *funcname, void (**f)(void), const char *sig) {
+#ifndef __PYX_HAVE_RT_ImportFunction_0_29_36
+#define __PYX_HAVE_RT_ImportFunction_0_29_36
+static int __Pyx_ImportFunction_0_29_36(PyObject *module, const char *funcname, void (**f)(void), const char *sig) {
     PyObject *d = 0;
     PyObject *cobj = 0;
     union {
         void (*fp)(void);
         void *p;
     } tmp;
     d = PyObject_GetAttrString(module, (char *)"__pyx_capi__");
```

### Comparing `medicc2-1.0.0/fstlib/cext/ops.pyx` & `medicc2-1.0.2/fstlib/cext/ops.pyx`

 * *Files identical despite different names*

### Comparing `medicc2-1.0.0/fstlib/cext/pywrapfst.cpp` & `medicc2-1.0.2/fstlib/cext/pywrapfst.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.34 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "extra_compile_args": [
             "-std=c++17",
@@ -33,16 +33,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_34"
-#define CYTHON_HEX_VERSION 0x001D22F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -102,18 +102,22 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -403,17 +407,14 @@
     operator T&() { return *ptr; }
     template<typename U> bool operator ==(U other) { return *ptr == other; }
     template<typename U> bool operator !=(U other) { return *ptr != other; }
   private:
     T *ptr;
 };
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -483,14 +484,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -49380,15 +49386,15 @@
   new((void*)&(p->_weight)) std::unique_ptr<fst::script::WeightClass> ();
   return o;
 }
 
 static void __pyx_tp_dealloc_6fstlib_4cext_9pywrapfst_Weight(PyObject *o) {
   struct __pyx_obj_6fstlib_4cext_9pywrapfst_Weight *p = (struct __pyx_obj_6fstlib_4cext_9pywrapfst_Weight *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   __Pyx_call_destructor(p->_weight);
   (*Py_TYPE(o)->tp_free)(o);
 }
 
@@ -49544,15 +49550,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst_SymbolTableView __pyx_vtable_6fstlib_4cext_9pywrapfst_SymbolTableView;
 
 static PyObject *__pyx_tp_new_6fstlib_4cext_9pywrapfst_SymbolTableView(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_6fstlib_4cext_9pywrapfst_SymbolTableView *p;
@@ -49566,15 +49572,15 @@
   p = ((struct __pyx_obj_6fstlib_4cext_9pywrapfst_SymbolTableView *)o);
   p->__pyx_vtab = __pyx_vtabptr_6fstlib_4cext_9pywrapfst_SymbolTableView;
   return o;
 }
 
 static void __pyx_tp_dealloc_6fstlib_4cext_9pywrapfst_SymbolTableView(PyObject *o) {
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   (*Py_TYPE(o)->tp_free)(o);
 }
 
 static PyMethodDef __pyx_methods_6fstlib_4cext_9pywrapfst_SymbolTableView[] = {
@@ -49657,15 +49663,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst__EncodeMapperSymbolTableView __pyx_vtable_6fstlib_4cext_9pywrapfst__EncodeMapperSymbolTableView;
 
 static PyObject *__pyx_tp_new_6fstlib_4cext_9pywrapfst__EncodeMapperSymbolTableView(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_6fstlib_4cext_9pywrapfst__EncodeMapperSymbolTableView *p;
@@ -49676,15 +49682,15 @@
   new((void*)&(p->_mapper)) std::shared_ptr<fst::script::EncodeMapperClass> ();
   return o;
 }
 
 static void __pyx_tp_dealloc_6fstlib_4cext_9pywrapfst__EncodeMapperSymbolTableView(PyObject *o) {
   struct __pyx_obj_6fstlib_4cext_9pywrapfst__EncodeMapperSymbolTableView *p = (struct __pyx_obj_6fstlib_4cext_9pywrapfst__EncodeMapperSymbolTableView *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   __Pyx_call_destructor(p->_mapper);
   __pyx_tp_dealloc_6fstlib_4cext_9pywrapfst_SymbolTableView(o);
 }
 
@@ -49763,15 +49769,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst__FstSymbolTableView __pyx_vtable_6fstlib_4cext_9pywrapfst__FstSymbolTableView;
 
 static PyObject *__pyx_tp_new_6fstlib_4cext_9pywrapfst__FstSymbolTableView(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_6fstlib_4cext_9pywrapfst__FstSymbolTableView *p;
@@ -49782,15 +49788,15 @@
   new((void*)&(p->_fst)) std::shared_ptr<fst::script::FstClass> ();
   return o;
 }
 
 static void __pyx_tp_dealloc_6fstlib_4cext_9pywrapfst__FstSymbolTableView(PyObject *o) {
   struct __pyx_obj_6fstlib_4cext_9pywrapfst__FstSymbolTableView *p = (struct __pyx_obj_6fstlib_4cext_9pywrapfst__FstSymbolTableView *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   __Pyx_call_destructor(p->_fst);
   __pyx_tp_dealloc_6fstlib_4cext_9pywrapfst_SymbolTableView(o);
 }
 
@@ -49869,15 +49875,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst__MutableSymbolTable __pyx_vtable_6fstlib_4cext_9pywrapfst__MutableSymbolTable;
 
 static PyObject *__pyx_tp_new_6fstlib_4cext_9pywrapfst__MutableSymbolTable(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_6fstlib_4cext_9pywrapfst__MutableSymbolTable *p;
@@ -49966,15 +49972,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst__MutableFstSymbolTableView __pyx_vtable_6fstlib_4cext_9pywrapfst__MutableFstSymbolTableView;
 
 static PyObject *__pyx_tp_new_6fstlib_4cext_9pywrapfst__MutableFstSymbolTableView(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_6fstlib_4cext_9pywrapfst__MutableFstSymbolTableView *p;
@@ -49985,15 +49991,15 @@
   new((void*)&(p->_mfst)) std::shared_ptr<fst::script::MutableFstClass> ();
   return o;
 }
 
 static void __pyx_tp_dealloc_6fstlib_4cext_9pywrapfst__MutableFstSymbolTableView(PyObject *o) {
   struct __pyx_obj_6fstlib_4cext_9pywrapfst__MutableFstSymbolTableView *p = (struct __pyx_obj_6fstlib_4cext_9pywrapfst__MutableFstSymbolTableView *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   __Pyx_call_destructor(p->_mfst);
   __pyx_tp_dealloc_6fstlib_4cext_9pywrapfst_SymbolTableView(o);
 }
 
@@ -50072,15 +50078,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst_SymbolTable __pyx_vtable_6fstlib_4cext_9pywrapfst_SymbolTable;
 
 static PyObject *__pyx_tp_new_6fstlib_4cext_9pywrapfst_SymbolTable(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_6fstlib_4cext_9pywrapfst_SymbolTable *p;
@@ -50091,15 +50097,15 @@
   new((void*)&(p->_smart_table)) std::unique_ptr<fst::SymbolTable> ();
   return o;
 }
 
 static void __pyx_tp_dealloc_6fstlib_4cext_9pywrapfst_SymbolTable(PyObject *o) {
   struct __pyx_obj_6fstlib_4cext_9pywrapfst_SymbolTable *p = (struct __pyx_obj_6fstlib_4cext_9pywrapfst_SymbolTable *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   __Pyx_call_destructor(p->_smart_table);
   __pyx_tp_dealloc_6fstlib_4cext_9pywrapfst_SymbolTableView(o);
 }
 
@@ -50177,15 +50183,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_6fstlib_4cext_9pywrapfst__SymbolTableIterator(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_6fstlib_4cext_9pywrapfst__SymbolTableIterator *p;
   PyObject *o;
@@ -50200,15 +50206,15 @@
   p->_table = ((struct __pyx_obj_6fstlib_4cext_9pywrapfst_SymbolTableView *)Py_None); Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_6fstlib_4cext_9pywrapfst__SymbolTableIterator(PyObject *o) {
   struct __pyx_obj_6fstlib_4cext_9pywrapfst__SymbolTableIterator *p = (struct __pyx_obj_6fstlib_4cext_9pywrapfst__SymbolTableIterator *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   __Pyx_call_destructor(p->_siter);
   Py_CLEAR(p->_table);
   (*Py_TYPE(o)->tp_free)(o);
@@ -50304,15 +50310,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst_EncodeMapper __pyx_vtable_6fstlib_4cext_9pywrapfst_EncodeMapper;
 
 static PyObject *__pyx_tp_new_6fstlib_4cext_9pywrapfst_EncodeMapper(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_6fstlib_4cext_9pywrapfst_EncodeMapper *p;
@@ -50328,15 +50334,15 @@
   new((void*)&(p->_mapper)) std::shared_ptr<fst::script::EncodeMapperClass> ();
   return o;
 }
 
 static void __pyx_tp_dealloc_6fstlib_4cext_9pywrapfst_EncodeMapper(PyObject *o) {
   struct __pyx_obj_6fstlib_4cext_9pywrapfst_EncodeMapper *p = (struct __pyx_obj_6fstlib_4cext_9pywrapfst_EncodeMapper *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   __Pyx_call_destructor(p->_mapper);
   (*Py_TYPE(o)->tp_free)(o);
 }
 
@@ -50420,15 +50426,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst_Fst __pyx_vtable_6fstlib_4cext_9pywrapfst_Fst;
 
 static PyObject *__pyx_tp_new_6fstlib_4cext_9pywrapfst_Fst(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_6fstlib_4cext_9pywrapfst_Fst *p;
@@ -50444,15 +50450,15 @@
   new((void*)&(p->_fst)) std::shared_ptr<fst::script::FstClass> ();
   return o;
 }
 
 static void __pyx_tp_dealloc_6fstlib_4cext_9pywrapfst_Fst(PyObject *o) {
   struct __pyx_obj_6fstlib_4cext_9pywrapfst_Fst *p = (struct __pyx_obj_6fstlib_4cext_9pywrapfst_Fst *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   __Pyx_call_destructor(p->_fst);
   (*Py_TYPE(o)->tp_free)(o);
 }
 
@@ -50546,15 +50552,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst_MutableFst __pyx_vtable_6fstlib_4cext_9pywrapfst_MutableFst;
 
 static PyObject *__pyx_tp_new_6fstlib_4cext_9pywrapfst_MutableFst(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_6fstlib_4cext_9pywrapfst_MutableFst *p;
@@ -50565,15 +50571,15 @@
   new((void*)&(p->_mfst)) std::shared_ptr<fst::script::MutableFstClass> ();
   return o;
 }
 
 static void __pyx_tp_dealloc_6fstlib_4cext_9pywrapfst_MutableFst(PyObject *o) {
   struct __pyx_obj_6fstlib_4cext_9pywrapfst_MutableFst *p = (struct __pyx_obj_6fstlib_4cext_9pywrapfst_MutableFst *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   __Pyx_call_destructor(p->_mfst);
   __pyx_tp_dealloc_6fstlib_4cext_9pywrapfst_Fst(o);
 }
 
@@ -50689,15 +50695,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst_VectorFst __pyx_vtable_6fstlib_4cext_9pywrapfst_VectorFst;
 
 static PyObject *__pyx_tp_new_6fstlib_4cext_9pywrapfst_VectorFst(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_6fstlib_4cext_9pywrapfst_VectorFst *p;
@@ -50783,15 +50789,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst_Arc __pyx_vtable_6fstlib_4cext_9pywrapfst_Arc;
 
 static PyObject *__pyx_tp_new_6fstlib_4cext_9pywrapfst_Arc(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_6fstlib_4cext_9pywrapfst_Arc *p;
@@ -50807,15 +50813,15 @@
   new((void*)&(p->_arc)) std::unique_ptr<fst::script::ArcClass> ();
   return o;
 }
 
 static void __pyx_tp_dealloc_6fstlib_4cext_9pywrapfst_Arc(PyObject *o) {
   struct __pyx_obj_6fstlib_4cext_9pywrapfst_Arc *p = (struct __pyx_obj_6fstlib_4cext_9pywrapfst_Arc *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   __Pyx_call_destructor(p->_arc);
   (*Py_TYPE(o)->tp_free)(o);
 }
 
@@ -50953,15 +50959,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst__ArcIterator __pyx_vtable_6fstlib_4cext_9pywrapfst__ArcIterator;
 
 static PyObject *__pyx_tp_new_6fstlib_4cext_9pywrapfst__ArcIterator(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_6fstlib_4cext_9pywrapfst__ArcIterator *p;
@@ -50978,15 +50984,15 @@
   new((void*)&(p->_aiter)) std::unique_ptr<fst::script::ArcIteratorClass> ();
   return o;
 }
 
 static void __pyx_tp_dealloc_6fstlib_4cext_9pywrapfst__ArcIterator(PyObject *o) {
   struct __pyx_obj_6fstlib_4cext_9pywrapfst__ArcIterator *p = (struct __pyx_obj_6fstlib_4cext_9pywrapfst__ArcIterator *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   __Pyx_call_destructor(p->_fst);
   __Pyx_call_destructor(p->_aiter);
   (*Py_TYPE(o)->tp_free)(o);
 }
@@ -51071,15 +51077,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst__MutableArcIterator __pyx_vtable_6fstlib_4cext_9pywrapfst__MutableArcIterator;
 
 static PyObject *__pyx_tp_new_6fstlib_4cext_9pywrapfst__MutableArcIterator(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_6fstlib_4cext_9pywrapfst__MutableArcIterator *p;
@@ -51096,15 +51102,15 @@
   new((void*)&(p->_aiter)) std::unique_ptr<fst::script::MutableArcIteratorClass> ();
   return o;
 }
 
 static void __pyx_tp_dealloc_6fstlib_4cext_9pywrapfst__MutableArcIterator(PyObject *o) {
   struct __pyx_obj_6fstlib_4cext_9pywrapfst__MutableArcIterator *p = (struct __pyx_obj_6fstlib_4cext_9pywrapfst__MutableArcIterator *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   __Pyx_call_destructor(p->_mfst);
   __Pyx_call_destructor(p->_aiter);
   (*Py_TYPE(o)->tp_free)(o);
 }
@@ -51190,15 +51196,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst__StateIterator __pyx_vtable_6fstlib_4cext_9pywrapfst__StateIterator;
 
 static PyObject *__pyx_tp_new_6fstlib_4cext_9pywrapfst__StateIterator(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_6fstlib_4cext_9pywrapfst__StateIterator *p;
@@ -51215,15 +51221,15 @@
   new((void*)&(p->_siter)) std::unique_ptr<fst::script::StateIteratorClass> ();
   return o;
 }
 
 static void __pyx_tp_dealloc_6fstlib_4cext_9pywrapfst__StateIterator(PyObject *o) {
   struct __pyx_obj_6fstlib_4cext_9pywrapfst__StateIterator *p = (struct __pyx_obj_6fstlib_4cext_9pywrapfst__StateIterator *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   __Pyx_call_destructor(p->_fst);
   __Pyx_call_destructor(p->_siter);
   (*Py_TYPE(o)->tp_free)(o);
 }
@@ -51304,15 +51310,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst_Compiler __pyx_vtable_6fstlib_4cext_9pywrapfst_Compiler;
 
 static PyObject *__pyx_tp_new_6fstlib_4cext_9pywrapfst_Compiler(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_6fstlib_4cext_9pywrapfst_Compiler *p;
@@ -51334,15 +51340,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_6fstlib_4cext_9pywrapfst_Compiler(PyObject *o) {
   struct __pyx_obj_6fstlib_4cext_9pywrapfst_Compiler *p = (struct __pyx_obj_6fstlib_4cext_9pywrapfst_Compiler *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   __Pyx_call_destructor(p->_sstrm);
   __Pyx_call_destructor(p->_fst_type);
   __Pyx_call_destructor(p->_arc_type);
   (*Py_TYPE(o)->tp_free)(o);
@@ -51419,15 +51425,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst_FarReader __pyx_vtable_6fstlib_4cext_9pywrapfst_FarReader;
 
 static PyObject *__pyx_tp_new_6fstlib_4cext_9pywrapfst_FarReader(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_6fstlib_4cext_9pywrapfst_FarReader *p;
@@ -51443,15 +51449,15 @@
   new((void*)&(p->_reader)) std::unique_ptr<fst::script::FarReaderClass> ();
   return o;
 }
 
 static void __pyx_tp_dealloc_6fstlib_4cext_9pywrapfst_FarReader(PyObject *o) {
   struct __pyx_obj_6fstlib_4cext_9pywrapfst_FarReader *p = (struct __pyx_obj_6fstlib_4cext_9pywrapfst_FarReader *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   __Pyx_call_destructor(p->_reader);
   (*Py_TYPE(o)->tp_free)(o);
 }
 static PyObject *__pyx_sq_item_6fstlib_4cext_9pywrapfst_FarReader(PyObject *o, Py_ssize_t i) {
@@ -51563,15 +51569,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_6fstlib_4cext_9pywrapfst_FarWriter __pyx_vtable_6fstlib_4cext_9pywrapfst_FarWriter;
 
 static PyObject *__pyx_tp_new_6fstlib_4cext_9pywrapfst_FarWriter(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_6fstlib_4cext_9pywrapfst_FarWriter *p;
@@ -51587,15 +51593,15 @@
   new((void*)&(p->_writer)) std::unique_ptr<fst::script::FarWriterClass> ();
   return o;
 }
 
 static void __pyx_tp_dealloc_6fstlib_4cext_9pywrapfst_FarWriter(PyObject *o) {
   struct __pyx_obj_6fstlib_4cext_9pywrapfst_FarWriter *p = (struct __pyx_obj_6fstlib_4cext_9pywrapfst_FarWriter *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   __Pyx_call_destructor(p->_writer);
   (*Py_TYPE(o)->tp_free)(o);
 }
 
@@ -51690,15 +51696,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_6fstlib_4cext_9pywrapfst___pyx_scope_struct____iter__ *__pyx_freelist_6fstlib_4cext_9pywrapfst___pyx_scope_struct____iter__[8];
 static int __pyx_freecount_6fstlib_4cext_9pywrapfst___pyx_scope_struct____iter__ = 0;
 
@@ -51799,15 +51805,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {"_read_SymbolTable_from_string", (PyCFunction)__pyx_pw_6fstlib_4cext_9pywrapfst_9_read_SymbolTable_from_string, METH_O, 0},
   {"compact_symbol_table", (PyCFunction)__pyx_pw_6fstlib_4cext_9pywrapfst_11compact_symbol_table, METH_O, __pyx_doc_6fstlib_4cext_9pywrapfst_10compact_symbol_table},
@@ -57808,15 +57814,15 @@
                         } else if (8 * sizeof(size_t) >= 4 * PyLong_SHIFT) {
                             return (size_t) (((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -58004,15 +58010,15 @@
                         } else if (8 * sizeof(int64_t) >= 4 * PyLong_SHIFT) {
                             return (int64_t) (((((((((int64_t)digits[3]) << PyLong_SHIFT) | (int64_t)digits[2]) << PyLong_SHIFT) | (int64_t)digits[1]) << PyLong_SHIFT) | (int64_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -58200,15 +58206,15 @@
                         } else if (8 * sizeof(int32_t) >= 4 * PyLong_SHIFT) {
                             return (int32_t) (((((((((int32_t)digits[3]) << PyLong_SHIFT) | (int32_t)digits[2]) << PyLong_SHIFT) | (int32_t)digits[1]) << PyLong_SHIFT) | (int32_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -58548,15 +58554,15 @@
                         } else if (8 * sizeof(uint8_t) >= 4 * PyLong_SHIFT) {
                             return (uint8_t) (((((((((uint8_t)digits[3]) << PyLong_SHIFT) | (uint8_t)digits[2]) << PyLong_SHIFT) | (uint8_t)digits[1]) << PyLong_SHIFT) | (uint8_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -58744,15 +58750,15 @@
                         } else if (8 * sizeof(uint64_t) >= 4 * PyLong_SHIFT) {
                             return (uint64_t) (((((((((uint64_t)digits[3]) << PyLong_SHIFT) | (uint64_t)digits[2]) << PyLong_SHIFT) | (uint64_t)digits[1]) << PyLong_SHIFT) | (uint64_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -59016,15 +59022,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -59212,15 +59218,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -60485,15 +60491,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static int __pyx_Generator_init(void) {
     __pyx_GeneratorType_type.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
     __pyx_GeneratorType_type.tp_iter = PyObject_SelfIter;
     __pyx_GeneratorType = __Pyx_FetchCommonType(&__pyx_GeneratorType_type);
```

### Comparing `medicc2-1.0.0/fstlib/cext/pywrapfst.pxd` & `medicc2-1.0.2/fstlib/cext/pywrapfst.pxd`

 * *Files identical despite different names*

### Comparing `medicc2-1.0.0/fstlib/cext/pywrapfst.pyx` & `medicc2-1.0.2/fstlib/cext/pywrapfst.pyx`

 * *Files identical despite different names*

### Comparing `medicc2-1.0.0/fstlib/core.py` & `medicc2-1.0.2/fstlib/core.py`

 * *Files identical despite different names*

### Comparing `medicc2-1.0.0/fstlib/ext.py` & `medicc2-1.0.2/fstlib/ext.py`

 * *Files identical despite different names*

### Comparing `medicc2-1.0.0/fstlib/factory.py` & `medicc2-1.0.2/fstlib/factory.py`

 * *Files identical despite different names*

### Comparing `medicc2-1.0.0/fstlib/paths.py` & `medicc2-1.0.2/fstlib/paths.py`

 * *Files identical despite different names*

### Comparing `medicc2-1.0.0/fstlib/test_fstlib.py` & `medicc2-1.0.2/fstlib/test_fstlib.py`

 * *Files identical despite different names*

### Comparing `medicc2-1.0.0/fstlib/tools.py` & `medicc2-1.0.2/fstlib/tools.py`

 * *Files identical despite different names*

### Comparing `medicc2-1.0.0/medicc/__init__.py` & `medicc2-1.0.2/medicc/__init__.py`

 * *Files identical despite different names*

### Comparing `medicc2-1.0.0/medicc/ancestors.py` & `medicc2-1.0.2/medicc/ancestors.py`

 * *Files identical despite different names*

### Comparing `medicc2-1.0.0/medicc/bootstrap.py` & `medicc2-1.0.2/medicc/bootstrap.py`

 * *Files identical despite different names*

### Comparing `medicc2-1.0.0/medicc/core.py` & `medicc2-1.0.2/medicc/core.py`

 * *Files identical despite different names*

### Comparing `medicc2-1.0.0/medicc/event_reconstruction.py` & `medicc2-1.0.2/medicc/event_reconstruction.py`

 * *Files identical despite different names*

### Comparing `medicc2-1.0.0/medicc/factory.py` & `medicc2-1.0.2/medicc/factory.py`

 * *Files identical despite different names*

### Comparing `medicc2-1.0.0/medicc/io.py` & `medicc2-1.0.2/medicc/io.py`

 * *Files identical despite different names*

### Comparing `medicc2-1.0.0/medicc/logging_conf.yaml` & `medicc2-1.0.2/medicc/logging_conf.yaml`

 * *Files identical despite different names*

### Comparing `medicc2-1.0.0/medicc/nj.py` & `medicc2-1.0.2/medicc/nj.py`

 * *Files identical despite different names*

### Comparing `medicc2-1.0.0/medicc/objects/Davoli_2013_TSG_OG_genes.bed` & `medicc2-1.0.2/medicc/objects/Davoli_2013_TSG_OG_genes.bed`

 * *Files identical despite different names*

### Comparing `medicc2-1.0.0/medicc/objects/hg19_chromosome_arms.bed` & `medicc2-1.0.2/medicc/objects/hg19_chromosome_arms.bed`

 * *Files identical despite different names*

### Comparing `medicc2-1.0.0/medicc/objects/hg38_chromosome_arms.bed` & `medicc2-1.0.2/medicc/objects/hg38_chromosome_arms.bed`

 * *Files identical despite different names*

### Comparing `medicc2-1.0.0/medicc/objects/no_wgd_asymm.fst` & `medicc2-1.0.2/medicc/objects/no_wgd_asymm.fst`

 * *Files identical despite different names*

### Comparing `medicc2-1.0.0/medicc/objects/wgd_1_asymm.fst` & `medicc2-1.0.2/medicc/objects/wgd_1_asymm.fst`

 * *Files identical despite different names*

### Comparing `medicc2-1.0.0/medicc/objects/wgd_2_asymm.fst` & `medicc2-1.0.2/medicc/objects/wgd_2_asymm.fst`

 * *Files identical despite different names*

### Comparing `medicc2-1.0.0/medicc/objects/wgd_asymm.fst` & `medicc2-1.0.2/medicc/objects/wgd_asymm.fst`

 * *Files identical despite different names*

### Comparing `medicc2-1.0.0/medicc/objects/wgd_total_cn_1_asymm.fst` & `medicc2-1.0.2/medicc/objects/wgd_total_cn_1_asymm.fst`

 * *Files identical despite different names*

### Comparing `medicc2-1.0.0/medicc/objects/wgd_total_cn_asymm.fst` & `medicc2-1.0.2/medicc/objects/wgd_total_cn_asymm.fst`

 * *Files identical despite different names*

### Comparing `medicc2-1.0.0/medicc/objects/wgd_x2_1_asymm.fst` & `medicc2-1.0.2/medicc/objects/wgd_x2_1_asymm.fst`

 * *Files identical despite different names*

### Comparing `medicc2-1.0.0/medicc/objects/wgd_x2_asymm.fst` & `medicc2-1.0.2/medicc/objects/wgd_x2_asymm.fst`

 * *Files identical despite different names*

### Comparing `medicc2-1.0.0/medicc/plot.py` & `medicc2-1.0.2/medicc/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,38 +79,31 @@
                     "These are: {}".format(np.setdiff1d(allele_columns, df.columns)))
 
     if np.setdiff1d(['is_clonal', 'is_normal', 'is_gain', 'is_loss', 'is_wgd'], df.columns).size > 0:
         if input_tree is None:
             df[['is_normal', 'is_clonal', 'is_gain', 'is_loss', 'is_wgd']] = False
         else:
             df[['is_gain', 'is_loss', 'is_wgd']] = False
+
             cn_change = compute_cn_change(df=df[allele_columns], tree=input_tree, normal_name=normal_name)
-            
             df.loc[(cn_change < 0).any(axis=1), 'is_loss'] = True
             df.loc[(cn_change > 0).any(axis=1), 'is_gain'] = True
 
             is_normal = ~df.unstack('sample_id')[['is_loss', 'is_gain', 'is_wgd']].any(axis=1)
             is_normal.name = 'is_normal'
             mrca = [x for x in input_tree.root.clades if x.name != normal_name][0].name
             is_clonal = ~df.loc[df.index.get_level_values('sample_id')!=mrca].unstack('sample_id')[['is_loss', 'is_gain', 'is_wgd']].any(axis=1)
             is_clonal.name = 'is_clonal'
 
-            df = df.drop(['is_normal', 'is_clonal'], axis=1, errors='ignore')
-            df = (df
-                    .join(is_normal, how='inner')
-                    .reorder_levels(['sample_id', 'chrom', 'start', 'end'])
-                    .sort_index()
-                    .join(is_clonal, how='inner')
-                    .reset_index())
             df = (df
-                    .set_index(['sample_id', 'chrom', 'start', 'end'])
-                    .sort_index())
-
-
-
+                  .drop(['is_normal', 'is_clonal'], axis=1, errors='ignore')
+                  .join(is_normal, on=['chrom', 'start', 'end'], how='inner')
+                  .join(is_clonal, on=['chrom', 'start', 'end'], how='inner')
+                  .sort_index()
+                  )
 
     if hide_normal_chromosomes:
         df = df.join(df.groupby('chrom')['is_normal'].all().to_frame('hide'))
         df = df.query("~hide").drop('hide', axis=1)
 
     if mincn=='auto':
         mincn = df[allele_columns].min().min()
```

### Comparing `medicc2-1.0.0/medicc/sim.py` & `medicc2-1.0.2/medicc/sim.py`

 * *Files identical despite different names*

### Comparing `medicc2-1.0.0/medicc/stats.py` & `medicc2-1.0.2/medicc/stats.py`

 * *Files identical despite different names*

### Comparing `medicc2-1.0.0/medicc/test_fsts.py` & `medicc2-1.0.2/medicc/test_fsts.py`

 * *Files identical despite different names*

### Comparing `medicc2-1.0.0/medicc/test_medicc.py` & `medicc2-1.0.2/medicc/test_medicc.py`

 * *Files identical despite different names*

### Comparing `medicc2-1.0.0/medicc/tools.py` & `medicc2-1.0.2/medicc/tools.py`

 * *Files identical despite different names*

### Comparing `medicc2-1.0.0/medicc2` & `medicc2-1.0.2/medicc2`

 * *Files identical despite different names*

### Comparing `medicc2-1.0.0/medicc2.egg-info/PKG-INFO` & `medicc2-1.0.2/medicc2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicc2
-Version: 1.0.0
+Version: 1.0.2
 Summary: Whole-genome doubling-aware copy number phylogenies for cancer evolution
 Home-page: https://bitbucket.org/schwarzlab/medicc2
 Author: Tom L Kaufmann, Marina Petkovic, Roland F Schwarz
 Author-email: tkau93@gmail.com, marina.55kovic@gmail.com, roland.f.schwarz@gmail.com
 License: GPL-3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -19,15 +19,17 @@
 [![Conda](https://img.shields.io/conda/v/bioconda/medicc2?color=green)](https://anaconda.org/bioconda/medicc2)
 
 For more information see the accompanying publication [Whole-genome doubling-aware copy number phylogenies for cancer evolution with MEDICC2](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-022-02794-9).
 
 # Installation
 Install MEDICC2 via conda (recommended), pip or from source. MEDICC2 was developed and tested on unix-built systems (Linux and MacOS). For Windows users we recommended WSL2.
 
-Note that the notebooks and examples are not included when installing from conda or pip. When installing from pip or source, you need to make sure to have a working version of `gcc` and `gxx` installed.
+Note that the notebooks and examples are not included when installing from conda or pip.
+
+For all installation methods you need to make sure to have a working version of the GNU Compiler Collection (`gcc`, `gxx` as well as related packages such as `libgcc-ng`) installed.
 
 
 ## Installation via conda (recommended)
 It is best to use a dedicated conda environment for your MEDICC2 installation with `conda create -n medicc_env`.
 
 After activating the environment with `conda activate medicc_env` you can install MEDICC2 via `conda install -c bioconda -c conda-forge medicc2`.
 
@@ -74,15 +76,15 @@
 * `--regions-bed`: BED file for regions of interest to compare copy-number events to
 * `-v`, `--verbose`: Enable verbose output. Default: False
 * `-vv`, `--debug`: Enable more verbose output Default: False
 * `--maxcn`: Expert option: maximum CN at which the input is capped. Does not change FST. Default: 8
 * `--prune-weight`: Expert option: Prune weight in ancestor reconstruction. Values >0 might result in more accurate ancestors but will require more time and memory. Default: 0
 * `--fst`: Expert option: path to an alternative FST. Default: None
 * `--fst-chr-separator`: Expert option: character used to separate chromosomes in the FST. Default: 'X'
-* `--wgd_x2`: Expert option: Treat WGD as a x2 operation. Default: False
+* `--wgd-x2`: Expert option: Treat WGD as a x2 operation. Default: False
 
 
 ## Input files
 Input files can be either in fasta or tsv format:
 
 * **tsv (recommended):** Files should have the following columns: `sample_id`, `chrom`, `start`, `end` as well as columns for the copy numbers. MEDICC expects the copy number columns to be called `cn_a` and `cn_b`. Using the flag `--input-allele-columns` you can set your own copy number columns. If you want to use total copy numbers, make sure to use the flag `--total-copy-numbers`. Important: MEDICC2 does not create total copy numbers for you. You will have to calculate total copy numbers yourself and then specify the column using the `--input-allele-columns` flag.
 * **fasta:** A description file should be provided to MEDICC. This file should include one line per file with the name of the chromosome and the corresponding file names. If fasta files are provided you have to use the flag `--input-type fasta`.
@@ -97,14 +99,15 @@
 MEDICC creates the following output files:
 
 * `_final_tree.new`, `_final_tree.xml`, `_final_tree.png`: The final phylogenetic tree in Newick and XML format as well as an image
 * `_pairwise_distances.tsv`: A NxN matrix (N being the number of samples) of pairwise distances calculated with the symmetric MEDICC2 distance
 * `_final_cn_profiles.tsv`: Copy-number profiles of the input as well as the newly internal nodes. Also includes additional information such as whether a gain or loss has happened
 * `_cn_profiles.pdf`: Combined plot of the phylogenetic tree as well as the copy-number profiles of all samples (including the internal nodes)
 * `_branch_lengths.tsv`: List of all branches and their corresponding lenghts of the final tree
+* `_summary.tsv`: Contains summary information about the created tree. If the `--events` flag was set, this includes the WGD status.
 
 *optional (see "Event Reconstruction" below)*
 
 * `_copynumber_events_df.tsv`: List of all copy-number events detected. The entries for WGD events have non-meaningful values for chrom, cn_child, etc. Note that the events derived are not unambiguous.
 * `_events_overlap.tsv`: Overlap of copy-number events with regions of interest
 
 
@@ -151,15 +154,15 @@
 MEDICCC2 can overlap the inferred events with regions of interest such as chromosome arms or oncogenes. 
 This process requires the installation of `pyranges` which might be incompatible with newer version of python and/or numpy.
 The overlap is turned off by default. You can turn on the overlapping with the ``--chromosomes-bed` and `--regions-bed` flag by providing bed-files with regions of interest. By default MEDICC2 uses hg38 chromosome-arms and a list of genes taken from Davoli et al. Cell 2013. This data is present as BED files in the `medicc/objects` folder. Invoke these using the flags `--chromosomes-bed "default"` and/or `--regions-bed "default"`.
 Users can specify regions of interest of their own in BED format by providing the `--chromosomes-bed` or `--regions-bed` flags.
 
 
 ## Single sample WGD detection
-If you are interested in the WGD status of individual samples in your data, have a look at the notebook `notebooks/single_sample_wgd_detection.py`. By replacing the input data with your data you can easily calculate the WGD status of any copy-number input.
+If you are interested in the WGD status of individual samples in your data, have a look at the notebook `notebooks/WGD_detection.ipynb`. By replacing the input data with your data you can easily calculate the WGD status of any copy-number input.
 
 
 # Issues
 If you experience problems with MEDICC2 please [file an issue directly on Bitbucket](https://bitbucket.org/schwarzlab/medicc2/issues/new) or [contact us directly](tom.kaufmann@mdc-berlin.de). 
 
 ## Known Issues
```

### Comparing `medicc2-1.0.0/medicc2.egg-info/SOURCES.txt` & `medicc2-1.0.2/medicc2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medicc2-1.0.0/setup.py` & `medicc2-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 extra_compile_args = ['-std=c++17']
 if sys.platform.startswith("darwin"):
   extra_compile_args.append("-stdlib=libc++")
   extra_compile_args.append("-mmacosx-version-min=10.12")
 
 setup(
     name='medicc2',
-    version='1.0.0',
+    version='1.0.2',
     author='Tom L Kaufmann, Marina Petkovic, Roland F Schwarz',
     author_email='tkau93@gmail.com, marina.55kovic@gmail.com, roland.f.schwarz@gmail.com',
     description='Whole-genome doubling-aware copy number phylogenies for cancer evolution',
     long_description=(Path(__file__).parent / "README.md").read_text(),
     long_description_content_type='text/markdown',
     url='https://bitbucket.org/schwarzlab/medicc2',
     classifiers=[
```

