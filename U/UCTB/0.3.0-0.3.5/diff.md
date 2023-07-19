# Comparing `tmp/UCTB-0.3.0.tar.gz` & `tmp/UCTB-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\UCTB-0.3.0.tar", last modified: Tue Oct 13 08:26:32 2020, max compression
+gzip compressed data, was "dist/UCTB-0.3.5.tar", last modified: Wed Jul 19 08:08:53 2023, max compression
```

## Comparing `UCTB-0.3.0.tar` & `UCTB-0.3.5.tar`

### file list

```diff
@@ -1,52 +1,67 @@
-drwxrwxrwx   0        0        0        0 2020-10-13 08:26:32.000000 UCTB-0.3.0/
--rw-rw-rw-   0        0        0      532 2020-10-13 08:26:32.000000 UCTB-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0       73 2020-09-20 02:05:04.000000 UCTB-0.3.0/README.md
--rw-rw-rw-   0        0        0       42 2020-10-13 08:26:32.000000 UCTB-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1223 2020-10-13 08:24:39.000000 UCTB-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2020-10-13 08:26:32.000000 UCTB-0.3.0/UCTB/
-drwxrwxrwx   0        0        0        0 2020-10-13 08:26:32.000000 UCTB-0.3.0/UCTB/dataset/
--rw-rw-rw-   0        0        0     6360 2020-05-31 14:31:28.000000 UCTB-0.3.0/UCTB/dataset/dataset.py
--rw-rw-rw-   0        0        0    28681 2020-06-08 12:50:58.000000 UCTB-0.3.0/UCTB/dataset/data_loader.py
--rw-rw-rw-   0        0        0      111 2019-12-18 07:02:05.000000 UCTB-0.3.0/UCTB/dataset/__init__.py
-drwxrwxrwx   0        0        0        0 2020-10-13 08:26:32.000000 UCTB-0.3.0/UCTB/evaluation/
--rw-rw-rw-   0        0        0     1861 2019-12-18 07:02:05.000000 UCTB-0.3.0/UCTB/evaluation/metric.py
--rw-rw-rw-   0        0        0       20 2019-12-18 07:02:05.000000 UCTB-0.3.0/UCTB/evaluation/__init__.py
-drwxrwxrwx   0        0        0        0 2020-10-13 08:26:32.000000 UCTB-0.3.0/UCTB/model/
--rw-rw-rw-   0        0        0     5225 2019-12-18 07:02:05.000000 UCTB-0.3.0/UCTB/model/ARIMA.py
--rw-rw-rw-   0        0        0     8874 2019-12-18 07:02:05.000000 UCTB-0.3.0/UCTB/model/DCRNN.py
--rw-rw-rw-   0        0        0     8535 2019-12-18 07:02:05.000000 UCTB-0.3.0/UCTB/model/DeepST.py
--rw-rw-rw-   0        0        0    24368 2019-12-18 07:02:05.000000 UCTB-0.3.0/UCTB/model/GeoMAN.py
--rw-rw-rw-   0        0        0     1446 2019-12-18 07:02:05.000000 UCTB-0.3.0/UCTB/model/HM.py
--rw-rw-rw-   0        0        0     1105 2019-12-18 07:02:05.000000 UCTB-0.3.0/UCTB/model/HMM.py
--rw-rw-rw-   0        0        0    21267 2020-08-30 01:27:27.000000 UCTB-0.3.0/UCTB/model/MCSTGCN.py
--rw-rw-rw-   0        0        0    16601 2020-06-08 13:09:16.000000 UCTB-0.3.0/UCTB/model/STMeta.py
--rw-rw-rw-   0        0        0     6553 2020-02-03 01:55:54.000000 UCTB-0.3.0/UCTB/model/ST_MGCN.py
--rw-rw-rw-   0        0        0     8460 2019-12-18 07:02:05.000000 UCTB-0.3.0/UCTB/model/ST_ResNet.py
--rw-rw-rw-   0        0        0     1987 2019-12-18 07:02:05.000000 UCTB-0.3.0/UCTB/model/XGBoost.py
--rw-rw-rw-   0        0        0      379 2019-12-18 07:02:05.000000 UCTB-0.3.0/UCTB/model/__init__.py
-drwxrwxrwx   0        0        0        0 2020-10-13 08:26:32.000000 UCTB-0.3.0/UCTB/model_unit/
--rw-rw-rw-   0        0        0    15815 2020-06-05 08:34:48.000000 UCTB-0.3.0/UCTB/model_unit/BaseModel.py
--rw-rw-rw-   0        0        0     7414 2019-12-18 07:02:05.000000 UCTB-0.3.0/UCTB/model_unit/DCRNN_CELL.py
--rw-rw-rw-   0        0        0     8262 2020-06-08 11:47:06.000000 UCTB-0.3.0/UCTB/model_unit/GraphModelLayers.py
--rw-rw-rw-   0        0        0     5850 2019-12-18 07:02:05.000000 UCTB-0.3.0/UCTB/model_unit/ST_RNN.py
--rw-rw-rw-   0        0        0      177 2020-06-08 11:47:06.000000 UCTB-0.3.0/UCTB/model_unit/__init__.py
-drwxrwxrwx   0        0        0        0 2020-10-13 08:26:32.000000 UCTB-0.3.0/UCTB/preprocess/
--rw-rw-rw-   0        0        0     8797 2020-07-04 07:17:43.000000 UCTB-0.3.0/UCTB/preprocess/GraphGenerator.py
--rw-rw-rw-   0        0        0     7270 2019-12-18 07:02:05.000000 UCTB-0.3.0/UCTB/preprocess/preprocessor.py
--rw-rw-rw-   0        0        0     2062 2020-06-05 08:34:48.000000 UCTB-0.3.0/UCTB/preprocess/time_utils.py
--rw-rw-rw-   0        0        0      153 2019-12-18 07:02:05.000000 UCTB-0.3.0/UCTB/preprocess/__init__.py
-drwxrwxrwx   0        0        0        0 2020-10-13 08:26:32.000000 UCTB-0.3.0/UCTB/train/
--rw-rw-rw-   0        0        0     3510 2019-12-18 07:02:05.000000 UCTB-0.3.0/UCTB/train/EarlyStopping.py
--rw-rw-rw-   0        0        0     7264 2019-12-18 07:02:05.000000 UCTB-0.3.0/UCTB/train/MiniBatchTrain.py
--rw-rw-rw-   0        0        0      177 2020-05-31 14:31:28.000000 UCTB-0.3.0/UCTB/train/__init__.py
-drwxrwxrwx   0        0        0        0 2020-10-13 08:26:32.000000 UCTB-0.3.0/UCTB/utils/
--rw-rw-rw-   0        0        0     1585 2020-06-05 08:34:48.000000 UCTB-0.3.0/UCTB/utils/make_predict_dataset.py
--rw-rw-rw-   0        0        0     2732 2019-12-18 07:02:05.000000 UCTB-0.3.0/UCTB/utils/multi_threads.py
--rw-rw-rw-   0        0        0      102 2020-06-05 08:34:48.000000 UCTB-0.3.0/UCTB/utils/__init__.py
--rw-rw-rw-   0        0        0      197 2020-10-13 08:23:21.000000 UCTB-0.3.0/UCTB/__init__.py
-drwxrwxrwx   0        0        0        0 2020-10-13 08:26:32.000000 UCTB-0.3.0/UCTB.egg-info/
--rw-rw-rw-   0        0        0        1 2020-10-13 08:26:31.000000 UCTB-0.3.0/UCTB.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      532 2020-10-13 08:26:31.000000 UCTB-0.3.0/UCTB.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2020-10-13 08:26:31.000000 UCTB-0.3.0/UCTB.egg-info/requires.txt
--rw-rw-rw-   0        0        0      995 2020-10-13 08:26:31.000000 UCTB-0.3.0/UCTB.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        5 2020-10-13 08:26:31.000000 UCTB-0.3.0/UCTB.egg-info/top_level.txt
+drwxr-xr-x   0 chenliyue   (501) staff       (20)        0 2023-07-19 08:08:53.000000 UCTB-0.3.5/
+-rw-r--r--   0 chenliyue   (501) staff       (20)     7856 2023-07-19 08:08:53.000000 UCTB-0.3.5/PKG-INFO
+drwxr-xr-x   0 chenliyue   (501) staff       (20)        0 2023-07-19 08:08:53.000000 UCTB-0.3.5/UCTB/
+drwxr-xr-x   0 chenliyue   (501) staff       (20)        0 2023-07-19 08:08:53.000000 UCTB-0.3.5/UCTB/dataset/
+-rw-r--r--   0 chenliyue   (501) staff       (20)    28276 2023-06-22 01:53:10.000000 UCTB-0.3.5/UCTB/dataset/data_loader.py
+-rw-r--r--   0 chenliyue   (501) staff       (20)      111 2022-07-08 12:48:35.000000 UCTB-0.3.5/UCTB/dataset/__init__.py
+-rw-r--r--   0 chenliyue   (501) staff       (20)     6510 2023-03-22 13:38:24.000000 UCTB-0.3.5/UCTB/dataset/dataset.py
+-rw-r--r--   0 chenliyue   (501) staff       (20)     3547 2023-05-21 01:50:16.000000 UCTB-0.3.5/UCTB/dataset/context_loader.py
+drwxr-xr-x   0 chenliyue   (501) staff       (20)        0 2023-07-19 08:08:53.000000 UCTB-0.3.5/UCTB/preprocess/
+-rw-r--r--   0 chenliyue   (501) staff       (20)     9828 2023-07-05 12:10:52.000000 UCTB-0.3.5/UCTB/preprocess/GraphGenerator.py
+-rw-r--r--   0 chenliyue   (501) staff       (20)      172 2023-06-07 12:41:57.000000 UCTB-0.3.5/UCTB/preprocess/__init__.py
+-rw-r--r--   0 chenliyue   (501) staff       (20)     2062 2022-07-08 12:48:35.000000 UCTB-0.3.5/UCTB/preprocess/time_utils.py
+-rw-r--r--   0 chenliyue   (501) staff       (20)    12348 2023-07-05 12:10:52.000000 UCTB-0.3.5/UCTB/preprocess/preprocessor.py
+-rw-r--r--   0 chenliyue   (501) staff       (20)     2895 2022-07-08 12:48:35.000000 UCTB-0.3.5/UCTB/preprocess/dataset_helper.py
+-rw-r--r--   0 chenliyue   (501) staff       (20)      195 2023-03-22 13:38:24.000000 UCTB-0.3.5/UCTB/__init__.py
+drwxr-xr-x   0 chenliyue   (501) staff       (20)        0 2023-07-19 08:08:53.000000 UCTB-0.3.5/UCTB/utils/
+-rw-r--r--   0 chenliyue   (501) staff       (20)     1541 2022-07-08 12:48:35.000000 UCTB-0.3.5/UCTB/utils/make_predict_dataset.py
+-rw-r--r--   0 chenliyue   (501) staff       (20)     9746 2023-06-22 01:53:10.000000 UCTB-0.3.5/UCTB/utils/utils_STGCN.py
+-rw-r--r--   0 chenliyue   (501) staff       (20)      101 2022-07-08 12:48:35.000000 UCTB-0.3.5/UCTB/utils/__init__.py
+-rw-r--r--   0 chenliyue   (501) staff       (20)    12734 2023-06-07 12:41:57.000000 UCTB-0.3.5/UCTB/utils/utils_AGCRN.py
+-rw-r--r--   0 chenliyue   (501) staff       (20)    12334 2023-06-07 12:41:57.000000 UCTB-0.3.5/UCTB/utils/utils_GMAN.py
+-rw-r--r--   0 chenliyue   (501) staff       (20)     9366 2023-06-22 01:53:10.000000 UCTB-0.3.5/UCTB/utils/utils_GraphWaveNet.py
+-rw-r--r--   0 chenliyue   (501) staff       (20)    11879 2023-06-22 01:53:10.000000 UCTB-0.3.5/UCTB/utils/utils_ASTGCN.py
+-rw-r--r--   0 chenliyue   (501) staff       (20)     2657 2022-07-08 12:48:35.000000 UCTB-0.3.5/UCTB/utils/multi_threads.py
+-rw-r--r--   0 chenliyue   (501) staff       (20)     6048 2023-06-22 01:53:10.000000 UCTB-0.3.5/UCTB/utils/utils_STSGCN.py
+drwxr-xr-x   0 chenliyue   (501) staff       (20)        0 2023-07-19 08:08:53.000000 UCTB-0.3.5/UCTB/model/
+-rw-r--r--   0 chenliyue   (501) staff       (20)    16700 2023-06-22 01:53:10.000000 UCTB-0.3.5/UCTB/model/STSGCN.py
+-rw-r--r--   0 chenliyue   (501) staff       (20)     8535 2022-07-08 12:48:35.000000 UCTB-0.3.5/UCTB/model/DeepST.py
+-rw-r--r--   0 chenliyue   (501) staff       (20)    11873 2023-07-05 12:10:52.000000 UCTB-0.3.5/UCTB/model/ASTGCN.py
+-rw-r--r--   0 chenliyue   (501) staff       (20)     8460 2022-07-08 12:48:35.000000 UCTB-0.3.5/UCTB/model/ST_ResNet.py
+-rw-r--r--   0 chenliyue   (501) staff       (20)      556 2023-06-22 01:53:10.000000 UCTB-0.3.5/UCTB/model/__init__.py
+-rw-r--r--   0 chenliyue   (501) staff       (20)     8852 2023-07-05 12:10:52.000000 UCTB-0.3.5/UCTB/model/GraphWaveNet.py
+-rw-r--r--   0 chenliyue   (501) staff       (20)     8677 2023-07-05 12:10:52.000000 UCTB-0.3.5/UCTB/model/DCRNN.py
+-rw-r--r--   0 chenliyue   (501) staff       (20)     1402 2022-07-08 12:48:35.000000 UCTB-0.3.5/UCTB/model/HM.py
+-rw-r--r--   0 chenliyue   (501) staff       (20)     6411 2022-07-08 12:48:35.000000 UCTB-0.3.5/UCTB/model/ST_MGCN.py
+-rw-r--r--   0 chenliyue   (501) staff       (20)    20858 2023-07-05 12:10:52.000000 UCTB-0.3.5/UCTB/model/MCSTGCN.py
+-rw-r--r--   0 chenliyue   (501) staff       (20)     1934 2022-07-08 12:48:35.000000 UCTB-0.3.5/UCTB/model/XGBoost.py
+-rw-r--r--   0 chenliyue   (501) staff       (20)    15081 2023-06-22 01:53:10.000000 UCTB-0.3.5/UCTB/model/GMAN.py
+-rw-r--r--   0 chenliyue   (501) staff       (20)    12666 2023-06-22 02:33:50.000000 UCTB-0.3.5/UCTB/model/STGCN.py
+-rw-r--r--   0 chenliyue   (501) staff       (20)    16585 2023-07-05 12:10:52.000000 UCTB-0.3.5/UCTB/model/STMeta.py
+-rw-r--r--   0 chenliyue   (501) staff       (20)     5868 2022-07-08 12:48:35.000000 UCTB-0.3.5/UCTB/model/ARIMA.py
+-rw-r--r--   0 chenliyue   (501) staff       (20)     1105 2022-07-08 12:48:35.000000 UCTB-0.3.5/UCTB/model/HMM.py
+-rw-r--r--   0 chenliyue   (501) staff       (20)     6776 2023-07-05 12:10:52.000000 UCTB-0.3.5/UCTB/model/AGCRN.py
+-rwxr-xr-x   0 chenliyue   (501) staff       (20)    23966 2022-07-08 12:48:35.000000 UCTB-0.3.5/UCTB/model/GeoMAN.py
+drwxr-xr-x   0 chenliyue   (501) staff       (20)        0 2023-07-19 08:08:53.000000 UCTB-0.3.5/UCTB/train/
+-rw-r--r--   0 chenliyue   (501) staff       (20)     3510 2022-07-08 12:48:35.000000 UCTB-0.3.5/UCTB/train/EarlyStopping.py
+-rw-r--r--   0 chenliyue   (501) staff       (20)      203 2023-04-16 12:21:05.000000 UCTB-0.3.5/UCTB/train/__init__.py
+-rw-r--r--   0 chenliyue   (501) staff       (20)     7264 2022-07-08 12:48:35.000000 UCTB-0.3.5/UCTB/train/MiniBatchTrain.py
+-rw-r--r--   0 chenliyue   (501) staff       (20)     4228 2023-06-07 12:41:57.000000 UCTB-0.3.5/UCTB/train/LossFunction.py
+drwxr-xr-x   0 chenliyue   (501) staff       (20)        0 2023-07-19 08:08:53.000000 UCTB-0.3.5/UCTB/evaluation/
+-rw-r--r--   0 chenliyue   (501) staff       (20)       20 2022-07-08 12:48:35.000000 UCTB-0.3.5/UCTB/evaluation/__init__.py
+-rw-r--r--   0 chenliyue   (501) staff       (20)     1259 2023-04-16 12:34:54.000000 UCTB-0.3.5/UCTB/evaluation/metric.py
+drwxr-xr-x   0 chenliyue   (501) staff       (20)        0 2023-07-19 08:08:53.000000 UCTB-0.3.5/UCTB/model_unit/
+-rw-r--r--   0 chenliyue   (501) staff       (20)     5706 2023-07-05 12:10:52.000000 UCTB-0.3.5/UCTB/model_unit/ST_RNN.py
+-rw-r--r--   0 chenliyue   (501) staff       (20)    15815 2022-07-08 12:48:35.000000 UCTB-0.3.5/UCTB/model_unit/BaseModel.py
+-rw-r--r--   0 chenliyue   (501) staff       (20)     8262 2022-07-08 12:48:35.000000 UCTB-0.3.5/UCTB/model_unit/GraphModelLayers.py
+-rw-r--r--   0 chenliyue   (501) staff       (20)     7225 2023-07-05 12:10:52.000000 UCTB-0.3.5/UCTB/model_unit/DCRNN_CELL.py
+-rw-r--r--   0 chenliyue   (501) staff       (20)      169 2022-07-08 12:48:35.000000 UCTB-0.3.5/UCTB/model_unit/__init__.py
+-rw-r--r--   0 chenliyue   (501) staff       (20)     6883 2023-06-24 07:37:03.000000 UCTB-0.3.5/README.md
+-rw-r--r--   0 chenliyue   (501) staff       (20)     1195 2023-07-19 08:08:11.000000 UCTB-0.3.5/setup.py
+drwxr-xr-x   0 chenliyue   (501) staff       (20)        0 2023-07-19 08:08:53.000000 UCTB-0.3.5/UCTB.egg-info/
+-rw-r--r--   0 chenliyue   (501) staff       (20)     7856 2023-07-19 08:08:53.000000 UCTB-0.3.5/UCTB.egg-info/PKG-INFO
+-rw-r--r--   0 chenliyue   (501) staff       (20)     1379 2023-07-19 08:08:53.000000 UCTB-0.3.5/UCTB.egg-info/SOURCES.txt
+-rw-r--r--   0 chenliyue   (501) staff       (20)      223 2023-07-19 08:08:53.000000 UCTB-0.3.5/UCTB.egg-info/requires.txt
+-rw-r--r--   0 chenliyue   (501) staff       (20)        5 2023-07-19 08:08:53.000000 UCTB-0.3.5/UCTB.egg-info/top_level.txt
+-rw-r--r--   0 chenliyue   (501) staff       (20)        1 2023-07-19 08:08:53.000000 UCTB-0.3.5/UCTB.egg-info/dependency_links.txt
+-rw-r--r--   0 chenliyue   (501) staff       (20)       38 2023-07-19 08:08:53.000000 UCTB-0.3.5/setup.cfg
```

### Comparing `UCTB-0.3.0/UCTB/dataset/dataset.py` & `UCTB-0.3.5/UCTB/dataset/dataset.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 import os
 import wget
 import pickle
 import tarfile
 import numpy as np
 
+
 class DataSet(object):
     """An object storing basic data from a formatted pickle file.
-
     See also `Build your own datasets <./md_file/tutorial.html>`_.
-
     Args:
         dataset (str): A string containing path of the dataset pickle file or a string of name of the dataset.
         city (str or ``None``): ``None`` if dataset is file path, or a string of name of the city. Default: ``None``
         data_dir (str or ``None``): The dataset directory. If set to ``None``, a directory will be created.
             If ``dataset`` is file path, ``data_dir`` should be ``None`` too. Default: ``None``
-
     Attributes:
         data (dict): The data directly from the pickle file. ``data`` may have a ``data['contribute_data']`` dict to
             store supplementary data.
         time_range (list): From ``data['TimeRange']`` in the format of [YYYY-MM-DD, YYYY-MM-DD] indicating the time
             range of the data.
         time_fitness (int): From ``data['TimeFitness']`` indicating how many minutes is a single time slot.
         node_traffic (np.ndarray): Data recording the main stream data of the nodes in during the time range.
@@ -27,18 +25,19 @@
             Its shape is [month_num, node_num, node_num].It's from ``data['Node']['TrafficMonthlyInteraction']``
             and is used to build interaction graph.
             Its an optional attribute and can be set as an empty list if interaction graph is not needed.
         node_station_info (dict): A dict storing the coordinates of nodes. It shall be formatted as {id (may be
             arbitrary): [id (when sorted, should be consistant with index of ``node_traffic``), latitude, longitude,
             other notes]}. It's from ``data['Node']['StationInfo']`` and is used to build distance graph.
             Its an optional attribute and can be set as an empty list if distance graph is not needed.
-        MergeIndex(int): A int number that used to adjust the granularity of the dataset, the granularity of the new 
+        MergeIndex(int): A int number that used to adjust the granularity of the dataset, the granularity of the new
             dataset is time_fitness*MergeIndex. default: 1
         MergeWay(str):can be `sum` and `average`.  default: ``sum
     """
+
     def __init__(self, dataset, MergeIndex, MergeWay, city=None, data_dir=None):
         self.dataset = dataset
         self.city = city
         self.MergeIndex = int(MergeIndex)
         self.MergeWay = MergeWay.lower()
 
         if data_dir is None:
@@ -72,48 +71,50 @@
                 print(e)
                 raise FileExistsError('Download Failed')
 
         with open(pkl_file_name, 'rb') as f:
             self.data = pickle.load(f)
 
         # merge data
-        self.data['TimeFitness']  = int(self.data['TimeFitness']*self.MergeIndex)
-        if len(self.data['Node']['TrafficNode']) > 0:
-            self.data['Node']['TrafficNode'] = self.merge_data(self.data['Node']['TrafficNode'],"node")
-        if len(self.data['Grid']['TrafficGrid']) > 0:
-            self.data['Grid']['TrafficGrid'] = self.merge_data(self.data['Grid']['TrafficGrid'],"grid")
-        if len(self.data['ExternalFeature']['Weather']) > 0:
-            self.data['ExternalFeature']['Weather'] = self.merge_data(self.data['ExternalFeature']['Weather'],"node")
+        if self.MergeIndex > 1:
+            self.data['TimeFitness'] = int(self.data['TimeFitness'] * self.MergeIndex)
+            if len(self.data['Node']['TrafficNode']) > 0:
+                self.data['Node']['TrafficNode'] = self.merge_data(self.data['Node']['TrafficNode'], "node")
+            if len(self.data['Grid']['TrafficGrid']) > 0:
+                self.data['Grid']['TrafficGrid'] = self.merge_data(self.data['Grid']['TrafficGrid'], "grid")
+            if len(self.data['ExternalFeature']['Weather']) > 0:
+                self.data['ExternalFeature']['Weather'] = self.merge_data(self.data['ExternalFeature']['Weather'],
+                                                                          "node")
 
         self.time_range = self.data['TimeRange']
         self.time_fitness = self.data['TimeFitness']
 
         self.node_traffic = self.data['Node']['TrafficNode']
         self.node_monthly_interaction = self.data['Node']['TrafficMonthlyInteraction']
         self.node_station_info = self.data['Node']['StationInfo']
 
         self.grid_traffic = self.data['Grid']['TrafficGrid']
         self.grid_lat_lng = self.data['Grid']['GridLatLng']
 
         self.external_feature_weather = self.data['ExternalFeature']['Weather']
 
-    def merge_data(self,data,dataType):
+    def merge_data(self, data, dataType):
         if self.MergeWay == "sum":
             func = np.sum
         elif self.MergeWay == "average":
             func = np.mean
         elif self.MergeWay == "max":
             func = np.max
         else:
             raise ValueError("Parameter MerWay should be sum or average")
         if data.shape[0] % self.MergeIndex is not 0:
             raise ValueError("time_slots % MergeIndex should be zero")
-        
+
         if dataType.lower() == "node":
-            new = np.zeros((data.shape[0]//self.MergeIndex,data.shape[1]),dtype=np.float32)
-            for new_ind,ind in enumerate(range(0,data.shape[0],self.MergeIndex)):
-                    new[new_ind,:] = func(data[ind:ind+self.MergeIndex,:],axis=0)
+            new = np.zeros((data.shape[0] // self.MergeIndex, data.shape[1]), dtype=np.float32)
+            for new_ind, ind in enumerate(range(0, data.shape[0], self.MergeIndex)):
+                new[new_ind, :] = func(data[ind:ind + self.MergeIndex, :], axis=0)
         elif dataType.lower() == "grid":
-            new = np.zeros((data.shape[0]//self.MergeIndex,data.shape[1],data.shape[2]),dtype=np.float32)
-            for new_ind,ind in enumerate(range(0,data.shape[0],self.MergeIndex)):
-                    new[new_ind,:,:] = func(data[ind:ind+self.MergeIndex,:,:],axis=0)
+            new = np.zeros((data.shape[0] // self.MergeIndex, data.shape[1], data.shape[2]), dtype=np.float32)
+            for new_ind, ind in enumerate(range(0, data.shape[0], self.MergeIndex)):
+                new[new_ind, :, :] = func(data[ind:ind + self.MergeIndex, :, :], axis=0)
         return new
```

### Comparing `UCTB-0.3.0/UCTB/evaluation/metric.py` & `UCTB-0.3.5/UCTB/evaluation/metric.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import numpy as np
 
-
 def rmse(prediction, target, threshold=None):
     """
     Args:
         prediction(ndarray): prediction with shape [batch_size, ...]
         target(ndarray): same shape with prediction, [batch_size, ...]
         threshold(float): data smaller or equal to threshold in target
             will be removed in computing the rmse
@@ -25,19 +24,8 @@
             the smallest threshold in mape is zero.
     """
     assert threshold > 0
     return (np.dot((np.abs(prediction - target) / (target + (1 - (target > threshold)))).reshape([1, -1]),
                    target.reshape([-1, 1]) > threshold) / np.sum(target > threshold))[0, 0]
 
 
-# def rmse_grid(prediction, target, threshold=None):
-#     if threshold is None:
-#         return np.sqrt(np.mean(np.square(prediction - target), axis=0))
-#     else:
-#         return np.sqrt(np.sum(np.square(prediction - target) *
-#                               (target > threshold), axis=0) / np.sum(target > threshold, axis=0))
-#
-#
-# def mape_grid(prediction, target, threshold=0):
-#     assert threshold > 0
-#     return np.sum((np.abs(prediction - target) / (target + (1 - (target > threshold))))
-#                   * (target > threshold), axis=0) / np.sum(target > threshold, axis=0)
+
```

### Comparing `UCTB-0.3.0/UCTB/model/ARIMA.py` & `UCTB-0.3.5/UCTB/model/ARIMA.py`

 * *Files 10% similar despite different names*

```diff
@@ -99,14 +99,25 @@
             time_sequences: The input time_series features.
             forecast_step: The number of predicted future steps. Default: 1
         
         :return: Prediction results with shape of (len(time_sequence)/forecast_step,forecast_step=,1).
         :type: np.ndarray
         '''
         result = []
+        """ origin predict method, output shape is [math.ceil(len(time_sequences) / forecast_step), forecast_step]
         for i in range(0, len(time_sequences), forecast_step):
             fs = forecast_step if ((i + forecast_step) < len(time_sequences)) else (len(time_sequences) - i)
             model = sm.tsa.SARIMAX(time_sequences[i], order=self.order, seasonal_order=self.seasonal_order)
             model_res = model.filter(self.model_res.params)
             p = model_res.forecast(fs).reshape([-1, 1])
             result.append(p)
+        """
+        # new predict method, output shape is [len(time_sequences), forecast_step]
+        for i in range(len(time_sequences)):
+            model = sm.tsa.SARIMAX(time_sequences[i], order=self.order, seasonal_order=self.seasonal_order)
+            model_res = model.filter(self.model_res.params)
+            p = model_res.forecast(forecast_step)
+            p = p.reshape([-1, forecast_step])
+            result.append(p)
+        if forecast_step != 1:
+            result = np.concatenate(result, axis=0)
         return np.array(result, dtype=np.float32)
```

### Comparing `UCTB-0.3.0/UCTB/model/DCRNN.py` & `UCTB-0.3.5/UCTB/model/DCRNN.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,181 +1,181 @@
-import tensorflow as tf
-
-from ..model_unit import BaseModel
-from ..model_unit import DCGRUCell
-
-from tensorflow.contrib import legacy_seq2seq
-
-
-class DCRNN(BaseModel):
-    """
-
-    References:
-        - `Diffusion convolutional recurrent neural network: Data-driven traffic forecasting (Li Yaguang, et al., 2017)
-          <https://arxiv.org/pdf/1707.01926.pdf>`_.
-        - `A TensorFlow implementation of Diffusion Convolutional Recurrent Neural Network (liyaguang)
-          <https://github.com/liyaguang/DCRNN>`_.
-
-    Args:
-        num_nodes(int): Number of nodes in the graph, e.g. number of stations in NYC-Bike dataset.
-        num_diffusion_matrix: Number of diffusion matrix used in model.
-        num_rnn_units: Number of RNN units.
-        num_rnn_layers: Number of RNN layers
-        max_diffusion_step: Number of diffusion steps
-        seq_len: Input sequence length
-        use_curriculum_learning(bool): model's prediction (True) or the previous ground truth in training (False).
-        input_dim: Dimension of the input feature
-        output_dim: Dimension of the output feature
-        cl_decay_steps: When use_curriculum_learning=True, cl_decay_steps is used to adjust the ratio of using ground
-            true labels, where with more training steps, the ratio drops.
-        target_len(int): Output sequence length.
-        lr(float): Learning rate
-        epsilon: epsilon in Adam
-        optimizer_name(str): 'sgd' or 'Adam' optimizer
-        code_version(str): Current version of this model code, which will be used as filename for saving the model
-        model_dir(str): The directory to store model files. Default:'model_dir'.
-        gpu_device(str): To specify the GPU to use. Default: '0'.
-    """
-    def __init__(self,
-                 num_nodes,
-                 num_diffusion_matrix,
-                 num_rnn_units=64,
-                 num_rnn_layers=1,
-                 max_diffusion_step=2,
-                 seq_len=6,
-                 use_curriculum_learning=False,
-                 input_dim=1,
-                 output_dim=1,
-                 cl_decay_steps=1000,
-                 target_len=1,
-                 lr=1e-4,
-                 epsilon=1e-3,
-                 optimizer_name='Adam',
-                 code_version='DCRNN-QuickStart',
-                 model_dir='model_dir',
-                 gpu_device='0', **kwargs):
-
-        super(DCRNN, self).__init__(code_version=code_version, model_dir=model_dir, gpu_device=gpu_device)
-
-        self._num_nodes = num_nodes
-        self._num_diffusion_matrix = num_diffusion_matrix
-        self._num_rnn_units = num_rnn_units
-        self._num_rnn_layers = num_rnn_layers
-        self._max_diffusion_step = max_diffusion_step
-        self._seq_len = seq_len
-        self._use_curriculum_learning = use_curriculum_learning
-        self._input_dim = input_dim
-        self._output_dim = output_dim
-        self._target_len = target_len
-        self._cl_decay_steps = cl_decay_steps
-        self._optimizer_name = optimizer_name
-        self._lr = lr
-        # self._batch_size = batch_size
-        self._epsilon = epsilon
-
-    def build(self, init_vars=True, max_to_keep=5):
-        with self._graph.as_default():
-            inputs = tf.placeholder(tf.float32, shape=(None, self._seq_len,
-                                                       self._num_nodes, self._input_dim), name='inputs')
-            labels = tf.placeholder(tf.float32, shape=(None, self._target_len,
-                                                       self._num_nodes, self._output_dim), name='labels')
-
-            diffusion_matrix = tf.placeholder(tf.float32, shape=(self._num_diffusion_matrix, self._num_nodes,
-                                                                 self._num_nodes), name='diffusion_matrix')
-
-            batch_size = tf.shape(inputs)[0]
-
-            self._input['inputs'] = inputs.name
-            self._input['target'] = labels.name
-            self._input['diffusion_matrix'] = diffusion_matrix.name
-
-            go_symbol = tf.zeros(shape=(tf.shape(inputs)[0], self._num_nodes * self._output_dim))
-
-            cell = DCGRUCell(self._num_rnn_units, self._input_dim, self._num_diffusion_matrix, diffusion_matrix,
-                             max_diffusion_step=self._max_diffusion_step, num_nodes=self._num_nodes)
-
-            cell_with_projection = DCGRUCell(self._num_rnn_units, self._input_dim,
-                                             self._num_diffusion_matrix, diffusion_matrix,
-                                             max_diffusion_step=self._max_diffusion_step,
-                                             num_nodes=self._num_nodes, num_proj=self._output_dim)
-
-            encoding_cells = [cell] * self._num_rnn_layers
-            decoding_cells = [cell] * (self._num_rnn_layers - 1) + [cell_with_projection]
-            encoding_cells = tf.contrib.rnn.MultiRNNCell(encoding_cells, state_is_tuple=True)
-            decoding_cells = tf.contrib.rnn.MultiRNNCell(decoding_cells, state_is_tuple=True)
-
-            global_step = tf.train.get_or_create_global_step()
-
-            # Outputs: (batch_size, timesteps, num_nodes, output_dim)
-            with tf.variable_scope('DCRNN_SEQ'):
-                inputs_unstack = tf.unstack(tf.reshape(inputs, (batch_size,
-                                                                self._seq_len, self._num_nodes * self._input_dim)),
-                                            axis=1)
-                labels_unstack = tf.unstack(
-                    tf.reshape(labels[..., :self._output_dim],
-                               (batch_size, self._target_len, self._num_nodes * self._output_dim)), axis=1)
-                labels_unstack.insert(0, go_symbol)
-
-                def _compute_sampling_threshold(global_step, k):
-                    """
-                    Computes the sampling probability for scheduled sampling using inverse sigmoid.
-                    global_step:
-                    k:
-                    :return:
-                    """
-                    return tf.cast(k / (k + tf.exp(global_step / k)), tf.float32)
-
-                def _loop_function_train(prev, i):
-                    # Return either the model's prediction or the previous ground truth in training.
-                    if self._use_curriculum_learning:
-                        c = tf.random_uniform((), minval=0, maxval=1.)
-                        threshold = _compute_sampling_threshold(global_step, self._cl_decay_steps)
-                        result = tf.cond(tf.less(c, threshold), lambda: labels_unstack[i], lambda: prev)
-                    else:
-                        result = labels_unstack[i]
-                    return result
-
-                def _loop_function_test(prev, i):
-                    # Return the prediction of the model in testing.
-                    return prev
-
-                a, enc_state = tf.contrib.rnn.static_rnn(encoding_cells, inputs_unstack, dtype=tf.float32)
-
-                with tf.variable_scope('train', reuse=False):
-                    train_outputs, _ = legacy_seq2seq.rnn_decoder(labels_unstack, enc_state, decoding_cells,
-                                                                  loop_function=_loop_function_train)
-                with tf.variable_scope('text', reuse=True):
-                    test_outputs, _ = legacy_seq2seq.rnn_decoder(labels_unstack, enc_state, decoding_cells,
-                                                                 loop_function=_loop_function_test)
-
-            # Project the output to output_dim.
-            train_outputs = tf.stack(train_outputs[:-1], axis=1)
-            test_outputs = tf.stack(test_outputs[:-1], axis=1)
-
-            # Configure optimizer
-            optimizer = tf.train.AdamOptimizer(self._lr, epsilon=float(self._epsilon))
-
-            if self._optimizer_name == 'sgd':
-                optimizer = tf.train.GradientDescentOptimizer(self._lr)
-
-            loss = tf.sqrt(tf.reduce_mean(tf.square(train_outputs - labels[:, :, :, 0])))
-
-            train_op = optimizer.minimize(loss)
-
-            self._output['prediction'] = test_outputs.name
-            self._output['loss'] = loss.name
-            self._op['train_op'] = train_op.name
-
-        super(DCRNN, self).build(init_vars=init_vars, max_to_keep=5)
-
-    # Define your '_get_feed_dict function‘, map your input to the tf-model
-    def _get_feed_dict(self,
-                       inputs,
-                       diffusion_matrix,
-                       target=None,):
-        feed_dict = {
-            'inputs': inputs,
-            'diffusion_matrix': diffusion_matrix,
-        }
-        if target is not None:
-            feed_dict['target'] = target
-        return feed_dict
+import tensorflow as tf
+
+from ..model_unit import BaseModel
+from ..model_unit import DCGRUCell
+
+from tensorflow.contrib import legacy_seq2seq
+
+
+class DCRNN(BaseModel):
+    """
+
+    References:
+        - `Diffusion convolutional recurrent neural network: Data-driven traffic forecasting (Li Yaguang, et al., 2017)
+          <https://arxiv.org/pdf/1707.01926.pdf>`_.
+        - `A TensorFlow implementation of Diffusion Convolutional Recurrent Neural Network (liyaguang)
+          <https://github.com/liyaguang/DCRNN>`_.
+
+    Args:
+        num_node(int): Number of nodes in the graph, e.g. number of stations in NYC-Bike dataset.
+        num_diffusion_matrix: Number of diffusion matrix used in model.
+        num_rnn_units: Number of RNN units.
+        num_rnn_layers: Number of RNN layers
+        max_diffusion_step: Number of diffusion steps
+        seq_len: Input sequence length
+        use_curriculum_learning(bool): model's prediction (True) or the previous ground truth in training (False).
+        input_dim: Dimension of the input feature
+        output_dim: Dimension of the output feature
+        cl_decay_steps: When use_curriculum_learning=True, cl_decay_steps is used to adjust the ratio of using ground
+            true labels, where with more training steps, the ratio drops.
+        target_len(int): Output sequence length.
+        lr(float): Learning rate
+        epsilon: epsilon in Adam
+        optimizer_name(str): 'sgd' or 'Adam' optimizer
+        code_version(str): Current version of this model code, which will be used as filename for saving the model
+        model_dir(str): The directory to store model files. Default:'model_dir'.
+        gpu_device(str): To specify the GPU to use. Default: '0'.
+    """
+    def __init__(self,
+                 num_node,
+                 num_diffusion_matrix,
+                 num_rnn_units=64,
+                 num_rnn_layers=1,
+                 max_diffusion_step=2,
+                 seq_len=6,
+                 use_curriculum_learning=False,
+                 input_dim=1,
+                 output_dim=1,
+                 cl_decay_steps=1000,
+                 target_len=1,
+                 lr=1e-4,
+                 epsilon=1e-3,
+                 optimizer_name='Adam',
+                 code_version='DCRNN-QuickStart',
+                 model_dir='model_dir',
+                 gpu_device='0', **kwargs):
+
+        super(DCRNN, self).__init__(code_version=code_version, model_dir=model_dir, gpu_device=gpu_device)
+
+        self._num_node = num_node
+        self._num_diffusion_matrix = num_diffusion_matrix
+        self._num_rnn_units = num_rnn_units
+        self._num_rnn_layers = num_rnn_layers
+        self._max_diffusion_step = max_diffusion_step
+        self._seq_len = seq_len
+        self._use_curriculum_learning = use_curriculum_learning
+        self._input_dim = input_dim
+        self._output_dim = output_dim
+        self._target_len = target_len
+        self._cl_decay_steps = cl_decay_steps
+        self._optimizer_name = optimizer_name
+        self._lr = lr
+        # self._batch_size = batch_size
+        self._epsilon = epsilon
+
+    def build(self, init_vars=True, max_to_keep=5):
+        with self._graph.as_default():
+            inputs = tf.placeholder(tf.float32, shape=(None, self._seq_len,
+                                                       self._num_node, self._input_dim), name='inputs')
+            labels = tf.placeholder(tf.float32, shape=(None, self._target_len,
+                                                       self._num_node, self._output_dim), name='labels')
+
+            diffusion_matrix = tf.placeholder(tf.float32, shape=(self._num_diffusion_matrix, self._num_node,
+                                                                 self._num_node), name='diffusion_matrix')
+
+            batch_size = tf.shape(inputs)[0]
+
+            self._input['inputs'] = inputs.name
+            self._input['target'] = labels.name
+            self._input['diffusion_matrix'] = diffusion_matrix.name
+
+            go_symbol = tf.zeros(shape=(tf.shape(inputs)[0], self._num_node * self._output_dim))
+
+            cell = DCGRUCell(self._num_rnn_units, self._input_dim, self._num_diffusion_matrix, diffusion_matrix,
+                             max_diffusion_step=self._max_diffusion_step, num_node=self._num_node)
+
+            cell_with_projection = DCGRUCell(self._num_rnn_units, self._input_dim,
+                                             self._num_diffusion_matrix, diffusion_matrix,
+                                             max_diffusion_step=self._max_diffusion_step,
+                                             num_node=self._num_node, num_proj=self._output_dim)
+
+            encoding_cells = [cell] * self._num_rnn_layers
+            decoding_cells = [cell] * (self._num_rnn_layers - 1) + [cell_with_projection]
+            encoding_cells = tf.contrib.rnn.MultiRNNCell(encoding_cells, state_is_tuple=True)
+            decoding_cells = tf.contrib.rnn.MultiRNNCell(decoding_cells, state_is_tuple=True)
+
+            global_step = tf.train.get_or_create_global_step()
+
+            # Outputs: (batch_size, timesteps, num_node, output_dim)
+            with tf.variable_scope('DCRNN_SEQ'):
+                inputs_unstack = tf.unstack(tf.reshape(inputs, (batch_size,
+                                                                self._seq_len, self._num_node * self._input_dim)),
+                                            axis=1)
+                labels_unstack = tf.unstack(
+                    tf.reshape(labels[..., :self._output_dim],
+                               (batch_size, self._target_len, self._num_node * self._output_dim)), axis=1)
+                labels_unstack.insert(0, go_symbol)
+
+                def _compute_sampling_threshold(global_step, k):
+                    """
+                    Computes the sampling probability for scheduled sampling using inverse sigmoid.
+                    global_step:
+                    k:
+                    :return:
+                    """
+                    return tf.cast(k / (k + tf.exp(global_step / k)), tf.float32)
+
+                def _loop_function_train(prev, i):
+                    # Return either the model's prediction or the previous ground truth in training.
+                    if self._use_curriculum_learning:
+                        c = tf.random_uniform((), minval=0, maxval=1.)
+                        threshold = _compute_sampling_threshold(global_step, self._cl_decay_steps)
+                        result = tf.cond(tf.less(c, threshold), lambda: labels_unstack[i], lambda: prev)
+                    else:
+                        result = labels_unstack[i]
+                    return result
+
+                def _loop_function_test(prev, i):
+                    # Return the prediction of the model in testing.
+                    return prev
+
+                a, enc_state = tf.contrib.rnn.static_rnn(encoding_cells, inputs_unstack, dtype=tf.float32)
+
+                with tf.variable_scope('train', reuse=False):
+                    train_outputs, _ = legacy_seq2seq.rnn_decoder(labels_unstack, enc_state, decoding_cells,
+                                                                  loop_function=_loop_function_train)
+                with tf.variable_scope('text', reuse=True):
+                    test_outputs, _ = legacy_seq2seq.rnn_decoder(labels_unstack, enc_state, decoding_cells,
+                                                                 loop_function=_loop_function_test)
+
+            # Project the output to output_dim.
+            train_outputs = tf.stack(train_outputs[:-1], axis=1)
+            test_outputs = tf.stack(test_outputs[:-1], axis=1)
+
+            # Configure optimizer
+            optimizer = tf.train.AdamOptimizer(self._lr, epsilon=float(self._epsilon))
+
+            if self._optimizer_name == 'sgd':
+                optimizer = tf.train.GradientDescentOptimizer(self._lr)
+
+            loss = tf.sqrt(tf.reduce_mean(tf.square(train_outputs - labels[:, :, :, 0])))
+
+            train_op = optimizer.minimize(loss)
+
+            self._output['prediction'] = test_outputs.name
+            self._output['loss'] = loss.name
+            self._op['train_op'] = train_op.name
+
+        super(DCRNN, self).build(init_vars=init_vars, max_to_keep=5)
+
+    # Define your '_get_feed_dict function‘, map your input to the tf-model
+    def _get_feed_dict(self,
+                       inputs,
+                       diffusion_matrix,
+                       target=None,):
+        feed_dict = {
+            'inputs': inputs,
+            'diffusion_matrix': diffusion_matrix,
+        }
+        if target is not None:
+            feed_dict['target'] = target
+        return feed_dict
```

### Comparing `UCTB-0.3.0/UCTB/model/DeepST.py` & `UCTB-0.3.5/UCTB/model/DeepST.py`

 * *Files identical despite different names*

### Comparing `UCTB-0.3.0/UCTB/model/GeoMAN.py` & `UCTB-0.3.5/UCTB/model/GeoMAN.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,402 +1,402 @@
-import tensorflow as tf
-from tensorflow.contrib.framework import nest
-from ..model_unit import BaseModel
-
-
-class GeoMAN(BaseModel):
-    """Multi-level Attention Networks for Geo-sensory Time Series Prediction (GeoMAN)
-
-            GeoMAN consists of two major parts: 1) A multi-level attention mechanism (including both local and global
-            spatial attentions in encoder and temporal attention in decoder) to model the dynamic spatio-temporal
-            dependencies; 2) A general fusion module to incorporate the external factors from different domains (e.g.,
-            meteorology, time of day and land use).
-
-            References:
-                - `GeoMAN: Multi-level Attention Networks for Geo-sensory Time Series Prediction (Liang Yuxuan, et al., 2018)
-                  <https://www.ijcai.org/proceedings/2018/0476.pdf>`_.
-                - `An easy implement of GeoMAN using TensorFlow (yoshall & CastleLiang)
-                  <https://github.com/yoshall/GeoMAN>`_.
-
-            Args:
-                total_sensers (int): The number of total sensors used in global attention mechanism.
-                input_dim (int): The number of dimensions of the target sensor's input.
-                external_dim (int): The number of dimensions of the external features.
-                output_dim (int): The number of dimensions of the target sensor's output.
-                input_steps (int): The length of historical input data, a.k.a, input timesteps.
-                output_steps (int): The number of steps that need prediction by one piece of history data, a.k.a, output
-                    timesteps. Have to be 1 now.
-                n_stacked_layers (int): The number of LSTM layers stacked in both encoder and decoder (These two are the
-                    same). Default: 2
-                n_encoder_hidden_units (int): The number of hidden units in each layer of encoder. Default: 128
-                n_decoder_hidden_units (int): The number of hidden units in each layer of decoder. Default: 128
-                dropout_rate (float): Dropout rate of LSTM layers in both encoder and decoder. Default: 0.3
-                lr (float): Learning rate. Default: 0.001
-                gc_rate (float): A clipping ratio for all the gradients. This operation normalizes all gradients so that
-                    their L2-norms are less than or equal to ``gc_rate``. Default: 2.5
-                code_version (str): Current version of this model code. Default: 'GeoMAN-QuickStart'
-                model_dir (str): The directory to store model files. Default:'model_dir'
-                gpu_device (str): To specify the GPU to use. Default: '0'
-                **kwargs (dict): Reserved for future use. May be used to pass parameters to class ``BaseModel``.
-            """
-    def __init__(self,
-                 total_sensers,
-                 input_dim,
-                 external_dim,
-                 output_dim,
-                 input_steps,
-                 output_steps,
-                 n_stacked_layers=2,
-                 n_encoder_hidden_units=128,
-                 n_decoder_hidden_units=128,
-                 dropout_rate=0.3,
-                 lr=0.001,
-                 gc_rate=2.5,
-                 code_version='GeoMAN-QuickStart',
-                 model_dir='model_dir',
-                 gpu_device='0',
-                 **kwargs):
-
-        super(GeoMAN, self).__init__(code_version=code_version, model_dir=model_dir, gpu_device=gpu_device)
-
-        # Architecture
-        self._n_stacked_layers = n_stacked_layers
-        self._n_encoder_hidden_units = n_encoder_hidden_units
-        self._n_decoder_hidden_units = n_decoder_hidden_units
-        self._n_output_decoder = output_dim  # n_output_decoder
-
-        self._n_steps_encoder = input_steps  # encoder_steps
-        self._n_steps_decoder = output_steps  # decoder_steps
-        self._n_input_encoder = input_dim  # n_input_encoder
-        self._n_sensers = total_sensers  # n_sensers
-        self._n_external_input = external_dim  # external_dim
-
-        # Hyperparameters
-        self._dropout_rate = dropout_rate
-        self._lr = lr
-        self._gc_rate = gc_rate
-
-    def build(self, init_vars=True, max_to_keep=5):
-        with self._graph.as_default():
-            with tf.variable_scope('inputs'):
-                local_features = tf.placeholder(tf.float32, shape=[None, self._n_steps_encoder, self._n_input_encoder],
-                                                name='local_features')
-                global_features = tf.placeholder(tf.float32, shape=[None, self._n_steps_encoder, self._n_sensers],
-                                                 name='global_features')
-                external_features = tf.placeholder(tf.float32,
-                                                   shape=[None, self._n_steps_decoder, self._n_external_input],
-                                                   name='external_features')
-                local_attn_states = tf.placeholder(tf.float32,
-                                                   shape=[None, self._n_input_encoder, self._n_steps_encoder],
-                                                   name='local_attn_states')
-                global_attn_states = tf.placeholder(tf.float32, shape=[None, self._n_sensers, self._n_input_encoder,
-                                                                       self._n_steps_encoder],
-                                                    name='global_attn_states')
-            with tf.variable_scope('ground_truth'):
-                targets = tf.placeholder(tf.float32, [None, self._n_steps_decoder, self._n_output_decoder])
-
-            self._input['local_features'] = local_features.name
-            self._input['global_features'] = global_features.name
-            self._input['external_features'] = external_features.name
-            self._input['local_attn_states'] = local_attn_states.name
-            self._input['global_attn_states'] = global_attn_states.name
-            self._input['targets'] = targets.name
-
-            predict_layer = tf.keras.layers.Dense(units=self._n_output_decoder,
-                                                  kernel_initializer=tf.truncated_normal_initializer,
-                                                  bias_initializer=tf.constant_initializer(0.),
-                                                  use_bias=True)
-
-            def _build_cells(n_hidden_units):
-                cells = []
-                for i in range(self._n_stacked_layers):
-                    with tf.variable_scope(f'LSTM_{i}'):
-                        cell = tf.contrib.rnn.BasicLSTMCell(n_hidden_units,
-                                                            forget_bias=1.0,
-                                                            state_is_tuple=True)
-                        cell = tf.nn.rnn_cell.DropoutWrapper(cell, output_keep_prob=1.0 - self._dropout_rate)
-                        cells.append(cell)
-                encoder_cell = tf.contrib.rnn.MultiRNNCell(cells)
-                return encoder_cell
-
-            def _loop_function(prev):
-                """loop function used in the decoder to generate the next input"""
-                return predict_layer(prev)
-
-            def _get_MSE_loss(y_true, y_pred):
-                return tf.reduce_mean(tf.pow(y_true - y_pred, 2), name='MSE_loss')
-
-            def _get_l2reg_loss():
-                # l2 loss
-                reg_loss = 0
-                for tf_var in tf.trainable_variables():
-                    if 'kernel:' in tf_var.name or 'bias:' in tf_var.name:
-                        reg_loss += tf.reduce_mean(tf.nn.l2_loss(tf_var))
-                return 0.001 * reg_loss
-
-            def _spatial_attention(local_features,  # x and X
-                                   global_features,
-                                   local_attention_states,
-                                   global_attention_states,
-                                   encoder_cells,  # to acquire h_{t-1}, s_{t-1}
-                                   ):
-                batch_size = tf.shape(local_features[0])[0]
-                output_size = encoder_cells.output_size
-                with tf.variable_scope('spatial_attention'):
-                    with tf.variable_scope('local_spatial_attn'):
-                        local_attn_length = local_attention_states.get_shape()[1].value  # n_input_encoder
-                        local_attn_size = local_attention_states.get_shape()[2].value  # n_steps_encoder
-                        local_attn = tf.zeros([batch_size, local_attn_length])
-
-                        #  Add local features in attention
-                        x_ik = tf.reshape(local_attention_states,
-                                          [-1, local_attn_length, 1, local_attn_size])  # features
-                        Ul = tf.get_variable('spati_atten_Ul', [1, 1, local_attn_size, local_attn_size])
-                        Ul_x = tf.nn.conv2d(x_ik, Ul, [1, 1, 1, 1], 'SAME')  # U_l * x^{i,k}
-                        vl = tf.get_variable('spati_atten_vl', [local_attn_size])  # v_l
-
-                        def _local_spatial_attention(query):
-                            # If the query is a tuple (when stacked RNN/LSTM), flatten it
-                            if hasattr(query, "__iter__"):
-                                query_list = nest.flatten(query)
-                                for q in query_list:
-                                    ndims = q.get_shape().ndims
-                                    if ndims:
-                                        assert ndims == 2
-                                query = tf.concat(query_list, 1)
-                            with tf.variable_scope('local_spatial_attn_Wl'):
-                                h_s = query
-                                Wl_hs_bl = tf.keras.layers.Dense(units=local_attn_size, use_bias=True)(h_s)
-                                Wl_hs_bl = tf.reshape(Wl_hs_bl, [-1, 1, 1, local_attn_size])
-                                score = tf.reduce_sum(vl * tf.nn.tanh(Wl_hs_bl + Ul_x),
-                                                      [2, 3])  # ! Ux is a 4 dims matrix, have to use reduce_sum here
-                                attention_weights = tf.nn.softmax(score)
-                            return attention_weights
-
-                    with tf.variable_scope('global_spatial_attn'):
-                        global_attn_length = global_attention_states.get_shape()[1].value  # n_sensor
-                        global_n_input = global_attention_states.get_shape()[2].value  # n_input_dim
-                        global_attn_size = global_attention_states.get_shape()[3].value  # n_input_dim
-                        global_attn = tf.zeros([batch_size, global_attn_length])
-
-                        # Add global features in attention
-                        Xl = tf.reshape(global_attention_states,
-                                        [-1, global_attn_length, global_n_input, global_attn_size])
-                        Wg_ug = tf.get_variable('spati_atten_Wg_ug',
-                                                [1, global_n_input, global_attn_size, global_attn_size])
-                        Wg_Xl_ug = tf.nn.conv2d(Xl, Wg_ug, [1, 1, 1, 1], 'SAME')
-                        vg = tf.get_variable('spati_atten_vg', [local_attn_size])
-
-                        # TODO: add U_g * y^l here, where y^l is the first column of local inputs.
-
-                        def _global_spatial_attention(query):
-                            if hasattr(query, "__iter__"):
-                                query_list = nest.flatten(query)
-                                for q in query_list:  # Check that ndims == 2 if specified.
-                                    ndims = q.get_shape().ndims
-                                    if ndims:
-                                        assert ndims == 2
-                                query = tf.concat(query_list, 1)
-                            with tf.variable_scope('global_spatial_attn_Wl'):
-                                h_s = query
-                                Wg_hs_bg = tf.keras.layers.Dense(units=global_attn_size, use_bias=True)(h_s)
-                                Wg_hs_bg = tf.reshape(Wg_hs_bg, [-1, 1, 1, global_attn_size])
-                                score = tf.reduce_sum(vg * tf.nn.tanh(Wg_hs_bg + Wg_Xl_ug), [2, 3])
-                                attention_weights = tf.nn.softmax(score)
-                                # Sometimes it's not easy to find a measurement to denote similarity between sensors,
-                                # here we omit such prior knowledge in eq.[4].
-                                # You can use "a = nn_ops.softmax((1-lambda)*s + lambda*sim)" to encode similarity info,
-                                # where:
-                                #     sim: a vector with length n_sensors, describing the sim between the target sensor and the others
-                                #     lambda: a trade-off.
-                                # attention_weights = tf.softmax((1-self.sm_rate)*score+self.sm_rate*self.similarity_graph)
-                            return attention_weights
-
-                    # Init
-                    zeros = [tf.zeros([batch_size, output_size]) for i in range(2)]
-                    initial_state = [zeros for _ in range(len(encoder_cells._cells))]
-                    state = initial_state
-
-                    # For each timestep
-                    outputs = []
-                    attn_weights = []
-                    for i, (local_input, global_input) in enumerate(zip(local_features, global_features)):
-                        if i > 0: tf.get_variable_scope().reuse_variables()
-
-                        local_context_vector = local_attn * local_input
-                        global_context_vector = global_attn * global_input
-                        x_t = tf.concat([local_context_vector, global_context_vector], axis=1)
-                        encoder_output, state = encoder_cells(x_t, state)  # Update states
-
-                        with tf.variable_scope('local_spatial_attn'):
-                            local_attn = _local_spatial_attention(state)
-                        with tf.variable_scope('global_spatial_attn'):
-                            global_attn = _global_spatial_attention(state)
-                        attn_weights.append((local_attn, global_attn))
-                        outputs.append(encoder_output)
-
-                return outputs, state, attn_weights
-
-            def _temporal_attention(decoder_inputs,
-                                    external_features,
-                                    inital_states,  # the first time, the output of encoder
-                                    attention_states,  # h_o
-                                    decoder_cells):
-                batch_size = tf.shape(decoder_inputs[0])[0]
-                output_size = decoder_cells.output_size
-                input_size = decoder_inputs[0].get_shape().with_rank(2)[1]  # ?
-                state = inital_states
-                with tf.variable_scope('temperal_attention'):
-                    attn_length = attention_states.get_shape()[1].value
-                    attn_size = attention_states.get_shape()[2].value
-
-                    h_o = tf.reshape(attention_states, [-1, attn_length, 1, attn_size])
-                    W_d = tf.get_variable('temperal_attn_Wd', [1, 1, attn_size, attn_size])
-                    W_h = tf.nn.conv2d(h_o, W_d, [1, 1, 1, 1], 'SAME')
-                    v_d = tf.get_variable('temperal_attn_vd', [attn_size])
-
-                    def _attention(query):
-                        if hasattr(query, "__iter__"):
-                            query_list = nest.flatten(query)
-                            for q in query_list:  # Check that ndims == 2 if specified.
-                                ndims = q.get_shape().ndims
-                                if ndims:
-                                    assert ndims == 2
-                            query = tf.concat(query_list, 1)
-                        with tf.variable_scope('attention'):
-                            d_s = query
-                            W_ds_b = tf.keras.layers.Dense(units=attn_size, use_bias=True)(d_s)
-                            W_ds_b = tf.reshape(W_ds_b, [-1, 1, 1, attn_size])
-                            score = tf.reduce_sum(v_d * tf.nn.tanh(W_ds_b + W_h), [2, 3])
-                            attention_weights = tf.nn.softmax(score)
-                            context_vector = tf.reduce_sum(
-                                tf.reshape(attention_weights, [-1, attn_length, 1, 1]) * h_o, [1, 2])
-                            context_vector = tf.reshape(context_vector, [-1, attn_size])
-                        return context_vector
-
-                    # Init
-                    inital_attn = tf.zeros([batch_size, output_size])
-                    attn = inital_attn
-                    outputs = []
-
-                    prev_decoder_output = None  # d_{t-1}
-                    for i, (decoder_input, external_input) in enumerate(zip(decoder_inputs, external_features)):
-                        if i > 0: tf.get_variable_scope().reuse_variables()
-                        if prev_decoder_output is not None and _loop_function is not None:
-                            with tf.variable_scope('loop_function', reuse=True):
-                                decoder_input = _loop_function(prev_decoder_output)
-                        x = tf.concat([decoder_input, external_input, attn], axis=1)
-                        x = tf.keras.layers.Dense(units=input_size, use_bias=True)(x)
-                        decoder_output, state = decoder_cells(x, state)
-                        # Update attention weights
-                        attn = _attention(state)
-                        # Attention output projection
-                        with tf.variable_scope("attn_output_projection"):
-                            x = tf.concat([decoder_output, attn], axis=1)
-                            output = tf.keras.layers.Dense(units=output_size, use_bias=True)(x)
-                        outputs.append(output)
-                        prev_decoder_output = output
-                return outputs, state
-
-            # Handle data
-            local_features, global_features, external_features, targets, decoder_inputs = input_transform(
-                local_features, global_features, external_features, targets)
-
-            with tf.variable_scope('GeoMAN'):
-                with tf.variable_scope('encoder'):
-                    encoder_cells = _build_cells(self._n_encoder_hidden_units)
-                    encoder_outputs, encoder_state, attn_weights = _spatial_attention(local_features,
-                                                                                      global_features,
-                                                                                      local_attn_states,
-                                                                                      global_attn_states,
-                                                                                      encoder_cells)
-                    top_states = [tf.reshape(e, [-1, 1, encoder_cells.output_size]) for e in encoder_outputs]
-                    attention_states = tf.concat(top_states, 1)
-
-                with tf.variable_scope('decoder'):
-                    decoder_cells = _build_cells(self._n_decoder_hidden_units)
-                    decoder_outputs, states = _temporal_attention(decoder_inputs,
-                                                                  external_features,
-                                                                  encoder_state,
-                                                                  attention_states,
-                                                                  decoder_cells)
-
-                with tf.variable_scope('prediction'):
-                    predictions = []
-                    for decoder_output in decoder_outputs:
-                        predictions.append(predict_layer(decoder_output))
-                    predictions = tf.stack(predictions, axis=1, name='predictions')
-
-                with tf.variable_scope('loss'):
-                    targets = tf.stack(targets, axis=1, name='targets')
-                    loss = tf.add(_get_MSE_loss(targets, predictions), _get_l2reg_loss(), name='loss')
-
-                with tf.variable_scope('train_op'):
-                    global_step = tf.train.get_or_create_global_step()
-                    optimizer = tf.train.AdamOptimizer(self._lr)
-                    gradients, variables = zip(*optimizer.compute_gradients(loss))
-                    gradients, _ = tf.clip_by_global_norm(gradients, self._gc_rate)  # clip norm
-                    train_op = optimizer.apply_gradients(zip(gradients, variables), global_step)
-
-                # record output
-                self._output['prediction'] = predictions.name
-                self._output['loss'] = loss.name
-                # record op
-                self._op['train_op'] = train_op.name
-
-        super(GeoMAN, self).build(init_vars=init_vars, max_to_keep=5)
-
-    def _get_feed_dict(self,
-                       local_features,
-                       global_features,
-                       local_attn_states,
-                       global_attn_states,
-                       external_features,
-                       targets):
-        """The method to get feet dict for tensorflow model.
-
-        Users may modify this method according to the format of input.
-
-        Args:
-            local_features (np.ndarray): All the time series generated by the target sensor i, including one target
-                series and other feature series, with shape `(batch, input_steps, input_dim)`.
-            global_features (np.ndarray): Target series generated by all the sensors, with shape `(batch, input_steps,
-                total_sensors)`.
-            local_attn_states (np.ndarray): Equals to ``local_features`` swapped ``input_steps`` and ``input_dim`` axis,
-                with shape `(batch, input_dim, input_steps)`.
-            global_attn_states (np.ndarray): All time series generated by all sensors, with shape `(batch,
-                total_sensors, input_dim, input_steps)`.
-            external_features (np.ndarray): Fused external factors, e.g., temporal factors: meteorology and spatial
-                factors: POIs density, with shape `(batch, output_steps, external_dim)`. All features have to be
-                time series.
-            targets (np.ndarray): Target sensor's labels, with shape `(batch, output_steps, output_dim)`.
-        """
-        feed_dict = {'local_features': local_features, 'global_features': global_features,
-                     'local_attn_states': local_attn_states, 'global_attn_states': global_attn_states,
-                     'external_features': external_features, 'targets': targets}
-        return feed_dict
-
-
-def input_transform(local_features,
-                    global_features,
-                    external_features,
-                    targets):
-    """Split the model's inputs from matrices to lists on timesteps axis."""
-    local_features = split_timesteps(local_features)
-    global_features = split_timesteps(global_features)
-    external_features = split_timesteps(external_features)
-    targets = split_timesteps(targets)
-    decoder_inputs = [tf.zeros_like(targets[0], dtype=tf.float32)] + targets[:-1]  # useless when loop func is employed
-    return local_features, global_features, external_features, targets, decoder_inputs
-
-
-def split_timesteps(inputs):
-    """Split the input matrix from (batch, timesteps, input_dim) to a step list ([[batch, input_dim], ..., ])."""
-    timesteps = inputs.get_shape()[1].value
-    feature_dims = inputs.get_shape()[2].value
-    inputs = tf.transpose(inputs, [1, 0, 2])
-    inputs = tf.reshape(inputs, [-1, feature_dims])
-    inputs = tf.split(inputs, timesteps, 0)
-    return inputs
-
-
-
+import tensorflow as tf
+from tensorflow.contrib.framework import nest
+from ..model_unit import BaseModel
+
+
+class GeoMAN(BaseModel):
+    """Multi-level Attention Networks for Geo-sensory Time Series Prediction (GeoMAN)
+
+            GeoMAN consists of two major parts: 1) A multi-level attention mechanism (including both local and global
+            spatial attentions in encoder and temporal attention in decoder) to model the dynamic spatio-temporal
+            dependencies; 2) A general fusion module to incorporate the external factors from different domains (e.g.,
+            meteorology, time of day and land use).
+
+            References:
+                - `GeoMAN: Multi-level Attention Networks for Geo-sensory Time Series Prediction (Liang Yuxuan, et al., 2018)
+                  <https://www.ijcai.org/proceedings/2018/0476.pdf>`_.
+                - `An easy implement of GeoMAN using TensorFlow (yoshall & CastleLiang)
+                  <https://github.com/yoshall/GeoMAN>`_.
+
+            Args:
+                total_sensers (int): The number of total sensors used in global attention mechanism.
+                input_dim (int): The number of dimensions of the target sensor's input.
+                external_dim (int): The number of dimensions of the external features.
+                output_dim (int): The number of dimensions of the target sensor's output.
+                input_steps (int): The length of historical input data, a.k.a, input timesteps.
+                output_steps (int): The number of steps that need prediction by one piece of history data, a.k.a, output
+                    timesteps. Have to be 1 now.
+                n_stacked_layers (int): The number of LSTM layers stacked in both encoder and decoder (These two are the
+                    same). Default: 2
+                n_encoder_hidden_units (int): The number of hidden units in each layer of encoder. Default: 128
+                n_decoder_hidden_units (int): The number of hidden units in each layer of decoder. Default: 128
+                dropout_rate (float): Dropout rate of LSTM layers in both encoder and decoder. Default: 0.3
+                lr (float): Learning rate. Default: 0.001
+                gc_rate (float): A clipping ratio for all the gradients. This operation normalizes all gradients so that
+                    their L2-norms are less than or equal to ``gc_rate``. Default: 2.5
+                code_version (str): Current version of this model code. Default: 'GeoMAN-QuickStart'
+                model_dir (str): The directory to store model files. Default:'model_dir'
+                gpu_device (str): To specify the GPU to use. Default: '0'
+                **kwargs (dict): Reserved for future use. May be used to pass parameters to class ``BaseModel``.
+            """
+    def __init__(self,
+                 total_sensers,
+                 input_dim,
+                 external_dim,
+                 output_dim,
+                 input_steps,
+                 output_steps,
+                 n_stacked_layers=2,
+                 n_encoder_hidden_units=128,
+                 n_decoder_hidden_units=128,
+                 dropout_rate=0.3,
+                 lr=0.001,
+                 gc_rate=2.5,
+                 code_version='GeoMAN-QuickStart',
+                 model_dir='model_dir',
+                 gpu_device='0',
+                 **kwargs):
+
+        super(GeoMAN, self).__init__(code_version=code_version, model_dir=model_dir, gpu_device=gpu_device)
+
+        # Architecture
+        self._n_stacked_layers = n_stacked_layers
+        self._n_encoder_hidden_units = n_encoder_hidden_units
+        self._n_decoder_hidden_units = n_decoder_hidden_units
+        self._n_output_decoder = output_dim  # n_output_decoder
+
+        self._n_steps_encoder = input_steps  # encoder_steps
+        self._n_steps_decoder = output_steps  # decoder_steps
+        self._n_input_encoder = input_dim  # n_input_encoder
+        self._n_sensers = total_sensers  # n_sensers
+        self._n_external_input = external_dim  # external_dim
+
+        # Hyperparameters
+        self._dropout_rate = dropout_rate
+        self._lr = lr
+        self._gc_rate = gc_rate
+
+    def build(self, init_vars=True, max_to_keep=5):
+        with self._graph.as_default():
+            with tf.variable_scope('inputs'):
+                local_features = tf.placeholder(tf.float32, shape=[None, self._n_steps_encoder, self._n_input_encoder],
+                                                name='local_features')
+                global_features = tf.placeholder(tf.float32, shape=[None, self._n_steps_encoder, self._n_sensers],
+                                                 name='global_features')
+                external_features = tf.placeholder(tf.float32,
+                                                   shape=[None, self._n_steps_decoder, self._n_external_input],
+                                                   name='external_features')
+                local_attn_states = tf.placeholder(tf.float32,
+                                                   shape=[None, self._n_input_encoder, self._n_steps_encoder],
+                                                   name='local_attn_states')
+                global_attn_states = tf.placeholder(tf.float32, shape=[None, self._n_sensers, self._n_input_encoder,
+                                                                       self._n_steps_encoder],
+                                                    name='global_attn_states')
+            with tf.variable_scope('ground_truth'):
+                targets = tf.placeholder(tf.float32, [None, self._n_steps_decoder, self._n_output_decoder])
+
+            self._input['local_features'] = local_features.name
+            self._input['global_features'] = global_features.name
+            self._input['external_features'] = external_features.name
+            self._input['local_attn_states'] = local_attn_states.name
+            self._input['global_attn_states'] = global_attn_states.name
+            self._input['targets'] = targets.name
+
+            predict_layer = tf.keras.layers.Dense(units=self._n_output_decoder,
+                                                  kernel_initializer=tf.truncated_normal_initializer,
+                                                  bias_initializer=tf.constant_initializer(0.),
+                                                  use_bias=True)
+
+            def _build_cells(n_hidden_units):
+                cells = []
+                for i in range(self._n_stacked_layers):
+                    with tf.variable_scope(f'LSTM_{i}'):
+                        cell = tf.contrib.rnn.BasicLSTMCell(n_hidden_units,
+                                                            forget_bias=1.0,
+                                                            state_is_tuple=True)
+                        cell = tf.nn.rnn_cell.DropoutWrapper(cell, output_keep_prob=1.0 - self._dropout_rate)
+                        cells.append(cell)
+                encoder_cell = tf.contrib.rnn.MultiRNNCell(cells)
+                return encoder_cell
+
+            def _loop_function(prev):
+                """loop function used in the decoder to generate the next input"""
+                return predict_layer(prev)
+
+            def _get_MSE_loss(y_true, y_pred):
+                return tf.reduce_mean(tf.pow(y_true - y_pred, 2), name='MSE_loss')
+
+            def _get_l2reg_loss():
+                # l2 loss
+                reg_loss = 0
+                for tf_var in tf.trainable_variables():
+                    if 'kernel:' in tf_var.name or 'bias:' in tf_var.name:
+                        reg_loss += tf.reduce_mean(tf.nn.l2_loss(tf_var))
+                return 0.001 * reg_loss
+
+            def _spatial_attention(local_features,  # x and X
+                                   global_features,
+                                   local_attention_states,
+                                   global_attention_states,
+                                   encoder_cells,  # to acquire h_{t-1}, s_{t-1}
+                                   ):
+                batch_size = tf.shape(local_features[0])[0]
+                output_size = encoder_cells.output_size
+                with tf.variable_scope('spatial_attention'):
+                    with tf.variable_scope('local_spatial_attn'):
+                        local_attn_length = local_attention_states.get_shape()[1].value  # n_input_encoder
+                        local_attn_size = local_attention_states.get_shape()[2].value  # n_steps_encoder
+                        local_attn = tf.zeros([batch_size, local_attn_length])
+
+                        #  Add local features in attention
+                        x_ik = tf.reshape(local_attention_states,
+                                          [-1, local_attn_length, 1, local_attn_size])  # features
+                        Ul = tf.get_variable('spati_atten_Ul', [1, 1, local_attn_size, local_attn_size])
+                        Ul_x = tf.nn.conv2d(x_ik, Ul, [1, 1, 1, 1], 'SAME')  # U_l * x^{i,k}
+                        vl = tf.get_variable('spati_atten_vl', [local_attn_size])  # v_l
+
+                        def _local_spatial_attention(query):
+                            # If the query is a tuple (when stacked RNN/LSTM), flatten it
+                            if hasattr(query, "__iter__"):
+                                query_list = nest.flatten(query)
+                                for q in query_list:
+                                    ndims = q.get_shape().ndims
+                                    if ndims:
+                                        assert ndims == 2
+                                query = tf.concat(query_list, 1)
+                            with tf.variable_scope('local_spatial_attn_Wl'):
+                                h_s = query
+                                Wl_hs_bl = tf.keras.layers.Dense(units=local_attn_size, use_bias=True)(h_s)
+                                Wl_hs_bl = tf.reshape(Wl_hs_bl, [-1, 1, 1, local_attn_size])
+                                score = tf.reduce_sum(vl * tf.nn.tanh(Wl_hs_bl + Ul_x),
+                                                      [2, 3])  # ! Ux is a 4 dims matrix, have to use reduce_sum here
+                                attention_weights = tf.nn.softmax(score)
+                            return attention_weights
+
+                    with tf.variable_scope('global_spatial_attn'):
+                        global_attn_length = global_attention_states.get_shape()[1].value  # n_sensor
+                        global_n_input = global_attention_states.get_shape()[2].value  # n_input_dim
+                        global_attn_size = global_attention_states.get_shape()[3].value  # n_input_dim
+                        global_attn = tf.zeros([batch_size, global_attn_length])
+
+                        # Add global features in attention
+                        Xl = tf.reshape(global_attention_states,
+                                        [-1, global_attn_length, global_n_input, global_attn_size])
+                        Wg_ug = tf.get_variable('spati_atten_Wg_ug',
+                                                [1, global_n_input, global_attn_size, global_attn_size])
+                        Wg_Xl_ug = tf.nn.conv2d(Xl, Wg_ug, [1, 1, 1, 1], 'SAME')
+                        vg = tf.get_variable('spati_atten_vg', [local_attn_size])
+
+                        # TODO: add U_g * y^l here, where y^l is the first column of local inputs.
+
+                        def _global_spatial_attention(query):
+                            if hasattr(query, "__iter__"):
+                                query_list = nest.flatten(query)
+                                for q in query_list:  # Check that ndims == 2 if specified.
+                                    ndims = q.get_shape().ndims
+                                    if ndims:
+                                        assert ndims == 2
+                                query = tf.concat(query_list, 1)
+                            with tf.variable_scope('global_spatial_attn_Wl'):
+                                h_s = query
+                                Wg_hs_bg = tf.keras.layers.Dense(units=global_attn_size, use_bias=True)(h_s)
+                                Wg_hs_bg = tf.reshape(Wg_hs_bg, [-1, 1, 1, global_attn_size])
+                                score = tf.reduce_sum(vg * tf.nn.tanh(Wg_hs_bg + Wg_Xl_ug), [2, 3])
+                                attention_weights = tf.nn.softmax(score)
+                                # Sometimes it's not easy to find a measurement to denote similarity between sensors,
+                                # here we omit such prior knowledge in eq.[4].
+                                # You can use "a = nn_ops.softmax((1-lambda)*s + lambda*sim)" to encode similarity info,
+                                # where:
+                                #     sim: a vector with length n_sensors, describing the sim between the target sensor and the others
+                                #     lambda: a trade-off.
+                                # attention_weights = tf.softmax((1-self.sm_rate)*score+self.sm_rate*self.similarity_graph)
+                            return attention_weights
+
+                    # Init
+                    zeros = [tf.zeros([batch_size, output_size]) for i in range(2)]
+                    initial_state = [zeros for _ in range(len(encoder_cells._cells))]
+                    state = initial_state
+
+                    # For each timestep
+                    outputs = []
+                    attn_weights = []
+                    for i, (local_input, global_input) in enumerate(zip(local_features, global_features)):
+                        if i > 0: tf.get_variable_scope().reuse_variables()
+
+                        local_context_vector = local_attn * local_input
+                        global_context_vector = global_attn * global_input
+                        x_t = tf.concat([local_context_vector, global_context_vector], axis=1)
+                        encoder_output, state = encoder_cells(x_t, state)  # Update states
+
+                        with tf.variable_scope('local_spatial_attn'):
+                            local_attn = _local_spatial_attention(state)
+                        with tf.variable_scope('global_spatial_attn'):
+                            global_attn = _global_spatial_attention(state)
+                        attn_weights.append((local_attn, global_attn))
+                        outputs.append(encoder_output)
+
+                return outputs, state, attn_weights
+
+            def _temporal_attention(decoder_inputs,
+                                    external_features,
+                                    inital_states,  # the first time, the output of encoder
+                                    attention_states,  # h_o
+                                    decoder_cells):
+                batch_size = tf.shape(decoder_inputs[0])[0]
+                output_size = decoder_cells.output_size
+                input_size = decoder_inputs[0].get_shape().with_rank(2)[1]  # ?
+                state = inital_states
+                with tf.variable_scope('temperal_attention'):
+                    attn_length = attention_states.get_shape()[1].value
+                    attn_size = attention_states.get_shape()[2].value
+
+                    h_o = tf.reshape(attention_states, [-1, attn_length, 1, attn_size])
+                    W_d = tf.get_variable('temperal_attn_Wd', [1, 1, attn_size, attn_size])
+                    W_h = tf.nn.conv2d(h_o, W_d, [1, 1, 1, 1], 'SAME')
+                    v_d = tf.get_variable('temperal_attn_vd', [attn_size])
+
+                    def _attention(query):
+                        if hasattr(query, "__iter__"):
+                            query_list = nest.flatten(query)
+                            for q in query_list:  # Check that ndims == 2 if specified.
+                                ndims = q.get_shape().ndims
+                                if ndims:
+                                    assert ndims == 2
+                            query = tf.concat(query_list, 1)
+                        with tf.variable_scope('attention'):
+                            d_s = query
+                            W_ds_b = tf.keras.layers.Dense(units=attn_size, use_bias=True)(d_s)
+                            W_ds_b = tf.reshape(W_ds_b, [-1, 1, 1, attn_size])
+                            score = tf.reduce_sum(v_d * tf.nn.tanh(W_ds_b + W_h), [2, 3])
+                            attention_weights = tf.nn.softmax(score)
+                            context_vector = tf.reduce_sum(
+                                tf.reshape(attention_weights, [-1, attn_length, 1, 1]) * h_o, [1, 2])
+                            context_vector = tf.reshape(context_vector, [-1, attn_size])
+                        return context_vector
+
+                    # Init
+                    inital_attn = tf.zeros([batch_size, output_size])
+                    attn = inital_attn
+                    outputs = []
+
+                    prev_decoder_output = None  # d_{t-1}
+                    for i, (decoder_input, external_input) in enumerate(zip(decoder_inputs, external_features)):
+                        if i > 0: tf.get_variable_scope().reuse_variables()
+                        if prev_decoder_output is not None and _loop_function is not None:
+                            with tf.variable_scope('loop_function', reuse=True):
+                                decoder_input = _loop_function(prev_decoder_output)
+                        x = tf.concat([decoder_input, external_input, attn], axis=1)
+                        x = tf.keras.layers.Dense(units=input_size, use_bias=True)(x)
+                        decoder_output, state = decoder_cells(x, state)
+                        # Update attention weights
+                        attn = _attention(state)
+                        # Attention output projection
+                        with tf.variable_scope("attn_output_projection"):
+                            x = tf.concat([decoder_output, attn], axis=1)
+                            output = tf.keras.layers.Dense(units=output_size, use_bias=True)(x)
+                        outputs.append(output)
+                        prev_decoder_output = output
+                return outputs, state
+
+            # Handle data
+            local_features, global_features, external_features, targets, decoder_inputs = input_transform(
+                local_features, global_features, external_features, targets)
+
+            with tf.variable_scope('GeoMAN'):
+                with tf.variable_scope('encoder'):
+                    encoder_cells = _build_cells(self._n_encoder_hidden_units)
+                    encoder_outputs, encoder_state, attn_weights = _spatial_attention(local_features,
+                                                                                      global_features,
+                                                                                      local_attn_states,
+                                                                                      global_attn_states,
+                                                                                      encoder_cells)
+                    top_states = [tf.reshape(e, [-1, 1, encoder_cells.output_size]) for e in encoder_outputs]
+                    attention_states = tf.concat(top_states, 1)
+
+                with tf.variable_scope('decoder'):
+                    decoder_cells = _build_cells(self._n_decoder_hidden_units)
+                    decoder_outputs, states = _temporal_attention(decoder_inputs,
+                                                                  external_features,
+                                                                  encoder_state,
+                                                                  attention_states,
+                                                                  decoder_cells)
+
+                with tf.variable_scope('prediction'):
+                    predictions = []
+                    for decoder_output in decoder_outputs:
+                        predictions.append(predict_layer(decoder_output))
+                    predictions = tf.stack(predictions, axis=1, name='predictions')
+
+                with tf.variable_scope('loss'):
+                    targets = tf.stack(targets, axis=1, name='targets')
+                    loss = tf.add(_get_MSE_loss(targets, predictions), _get_l2reg_loss(), name='loss')
+
+                with tf.variable_scope('train_op'):
+                    global_step = tf.train.get_or_create_global_step()
+                    optimizer = tf.train.AdamOptimizer(self._lr)
+                    gradients, variables = zip(*optimizer.compute_gradients(loss))
+                    gradients, _ = tf.clip_by_global_norm(gradients, self._gc_rate)  # clip norm
+                    train_op = optimizer.apply_gradients(zip(gradients, variables), global_step)
+
+                # record output
+                self._output['prediction'] = predictions.name
+                self._output['loss'] = loss.name
+                # record op
+                self._op['train_op'] = train_op.name
+
+        super(GeoMAN, self).build(init_vars=init_vars, max_to_keep=5)
+
+    def _get_feed_dict(self,
+                       local_features,
+                       global_features,
+                       local_attn_states,
+                       global_attn_states,
+                       external_features,
+                       targets):
+        """The method to get feet dict for tensorflow model.
+
+        Users may modify this method according to the format of input.
+
+        Args:
+            local_features (np.ndarray): All the time series generated by the target sensor i, including one target
+                series and other feature series, with shape `(batch, input_steps, input_dim)`.
+            global_features (np.ndarray): Target series generated by all the sensors, with shape `(batch, input_steps,
+                total_sensors)`.
+            local_attn_states (np.ndarray): Equals to ``local_features`` swapped ``input_steps`` and ``input_dim`` axis,
+                with shape `(batch, input_dim, input_steps)`.
+            global_attn_states (np.ndarray): All time series generated by all sensors, with shape `(batch,
+                total_sensors, input_dim, input_steps)`.
+            external_features (np.ndarray): Fused external factors, e.g., temporal factors: meteorology and spatial
+                factors: POIs density, with shape `(batch, output_steps, external_dim)`. All features have to be
+                time series.
+            targets (np.ndarray): Target sensor's labels, with shape `(batch, output_steps, output_dim)`.
+        """
+        feed_dict = {'local_features': local_features, 'global_features': global_features,
+                     'local_attn_states': local_attn_states, 'global_attn_states': global_attn_states,
+                     'external_features': external_features, 'targets': targets}
+        return feed_dict
+
+
+def input_transform(local_features,
+                    global_features,
+                    external_features,
+                    targets):
+    """Split the model's inputs from matrices to lists on timesteps axis."""
+    local_features = split_timesteps(local_features)
+    global_features = split_timesteps(global_features)
+    external_features = split_timesteps(external_features)
+    targets = split_timesteps(targets)
+    decoder_inputs = [tf.zeros_like(targets[0], dtype=tf.float32)] + targets[:-1]  # useless when loop func is employed
+    return local_features, global_features, external_features, targets, decoder_inputs
+
+
+def split_timesteps(inputs):
+    """Split the input matrix from (batch, timesteps, input_dim) to a step list ([[batch, input_dim], ..., ])."""
+    timesteps = inputs.get_shape()[1].value
+    feature_dims = inputs.get_shape()[2].value
+    inputs = tf.transpose(inputs, [1, 0, 2])
+    inputs = tf.reshape(inputs, [-1, feature_dims])
+    inputs = tf.split(inputs, timesteps, 0)
+    return inputs
+
+
+
```

### Comparing `UCTB-0.3.0/UCTB/model/HMM.py` & `UCTB-0.3.5/UCTB/model/HMM.py`

 * *Files identical despite different names*

### Comparing `UCTB-0.3.0/UCTB/model/MCSTGCN.py` & `UCTB-0.3.5/UCTB/model/MCSTGCN.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,405 +1,405 @@
-import keras
-import tensorflow as tf
-
-from ..model_unit import BaseModel
-from ..model_unit import GAL, GCL
-from ..model_unit import DCGRUCell
-from ..model_unit import GCLSTMCell
-
-
-class MCSTGCN(BaseModel):
-    """
-        Args:
-            num_node(int): Number of nodes in the graph, e.g. number of stations in NYC-Bike dataset.
-            external_dim(int): Dimension of the external feature, e.g. temperature and wind are two dimension.
-            closeness_len(int): The length of closeness data history. The former consecutive ``closeness_len`` time slots
-            of data will be used as closeness history.
-            period_len(int): The length of period data history. The data of exact same time slots in former consecutive
-            ``period_len`` days will be used as period history.
-            trend_len(int): The length of trend data history. The data of exact same time slots in former consecutive
-            ``trend_len`` weeks (every seven days) will be used as trend history.
-            num_graph(int): Number of graphs used in MCSTGCN.
-            gcn_k(int): The highest order of Chebyshev Polynomial approximation in GCN.
-            gcn_layers(int): Number of GCN layers.
-            gclstm_layers(int): Number of STRNN layers, it works on all modes of MCSTGCN such as GCLSTM and DCRNN.
-            num_hidden_units(int): Number of hidden units of RNN.
-            num_dense_units(int): Number of dense units.
-            graph_merge_gal_units(int): Number of units in GAL for merging different graph features.
-                Only works when graph_merge='gal'
-            graph_merge_gal_num_heads(int): Number of heads in GAL for merging different graph features.
-                Only works when graph_merge='gal'
-            temporal_merge_gal_units(int): Number of units in GAL for merging different temporal features.
-                Only works when temporal_merge='gal'
-            temporal_merge_gal_num_heads(int): Number of heads in GAL for merging different temporal features.
-                Only works when temporal_merge='gal'
-            st_method(str): must in ['GCLSTM', 'DCRNN', 'GRU', 'LSTM'], which refers to different
-                spatial-temporal modeling methods.
-                'GCLSTM': GCN for modeling spatial feature, LSTM for modeling temporal feature.
-                'DCRNN': Diffusion Convolution for modeling spatial feature, GRU for modeling temporam frature.
-                'GRU': Ignore the spatial, and model the temporal feature using GRU
-                'LSTM': Ignore the spatial, and model the temporal feature using LSTM
-            temporal_merge(str): must in ['gal', 'concat'], refers to different temporal merging methods,
-                'gal': merge using GAL,
-                'concat': merge by concat and dense
-            graph_merge(str): must in ['gal', 'concat'], refers to different graph merging methods,
-                'gal': merge using GAL,
-                'concat': merge by concat and dense
-            output_activation(function): activation function, e.g. tf.nn.tanh
-            lr(float): Learning rate. Default: 1e-5
-            code_version(str): Current version of this model code, which will be used as filename for saving the model
-            model_dir(str): The directory to store model files. Default:'model_dir'.
-            gpu_device(str): To specify the GPU to use. Default: '0'.
-        """
-
-    def __init__(self,
-                 num_node,
-                 external_dim,
-                 closeness_len,
-                 period_len,
-                 trend_len,
-
-                 # gcn parameters
-                 num_graph=1,
-                 gcn_k=1,
-                 gcn_layers=1,
-                 gclstm_layers=1,
-
-                 # dense units
-                 num_hidden_units=64,
-                 # LSTM units
-                 num_dense_units=32,
-
-                 # merge parameters
-                 graph_merge_gal_units=32,
-                 graph_merge_gal_num_heads=2,
-                 temporal_merge_gal_units=64,
-                 temporal_merge_gal_num_heads=2,
-
-                 # network structure parameters
-                 st_method='GCLSTM',  # gclstm
-                 temporal_merge='gal',  # gal
-                 graph_merge='gal',  # concat
-
-                 output_activation=tf.nn.sigmoid,
-
-                 lr=1e-4,
-                 code_version='MCSTGCN-QuickStart',
-                 model_dir='model_dir',
-                 gpu_device='0', **kwargs):
-
-        super(MCSTGCN, self).__init__(code_version=code_version, model_dir=model_dir, gpu_device=gpu_device)
-
-        self._num_node = num_node
-        self._gcn_k = gcn_k
-        self._gcn_layer = gcn_layers
-        self._graph_merge_gal_units = graph_merge_gal_units
-        self._graph_merge_gal_num_heads = graph_merge_gal_num_heads
-        self._temporal_merge_gal_units = temporal_merge_gal_units
-        self._temporal_merge_gal_num_heads = temporal_merge_gal_num_heads
-        self._gclstm_layers = gclstm_layers
-        self._num_graph = num_graph
-        self._external_dim = external_dim
-        self._output_activation = output_activation
-
-        self._st_method = st_method.upper()
-        self._temporal_merge = temporal_merge
-        self._graph_merge = graph_merge
-
-        self._closeness_len = int(closeness_len)
-        self._period_len = int(period_len)
-        self._trend_len = int(trend_len)
-        self._num_hidden_unit = num_hidden_units
-        self._num_dense_units = num_dense_units
-        self._lr = lr
-    
-    def build(self, init_vars=True, max_to_keep=5):
-        with self._graph.as_default():
-
-            temporal_features = []
-
-            if self._closeness_len is not None and self._closeness_len > 0:
-                closeness_feature = tf.placeholder(tf.float32, [None, None, self._closeness_len, 1],
-                                                   name='closeness_feature')
-                self._input['closeness_feature'] = closeness_feature.name
-                temporal_features.append([self._closeness_len, closeness_feature, 'closeness_feature'])
-
-            if self._period_len is not None and self._period_len > 0:
-                period_feature = tf.placeholder(tf.float32, [None, None, self._period_len, 1],
-                                                name='period_feature')
-                self._input['period_feature'] = period_feature.name
-                temporal_features.append([self._period_len, period_feature, 'period_feature'])
-
-            if self._trend_len is not None and self._trend_len > 0:
-                trend_feature = tf.placeholder(tf.float32, [None, None, self._trend_len, 1],
-                                               name='trend_feature')
-                self._input['trend_feature'] = trend_feature.name
-                temporal_features.append([self._trend_len, trend_feature, 'trend_feature'])
-
-            if len(temporal_features) > 0:
-                target = tf.placeholder(tf.float32, [None, None, 1], name='target')
-                laplace_matrix = tf.placeholder(tf.float32, [self._num_graph, None, None], name='laplace_matrix')
-                self._input['target'] = target.name
-                self._input['laplace_matrix'] = laplace_matrix.name
-            else:
-                raise ValueError('closeness_len, period_len, trend_len cannot all be zero')
-
-            graph_outputs_list = []
-
-
-            for i, time_step, target_tensor, given_name in enumerate(temporal_features):
-                temporal_features[i][1] = GCL.add_multi_gc_layers(tf.reshape(traffic_flow, [-1, self._num_node, self._input_dim]),
-                                                                  gcn_k=1, gcn_l=1, output_size=self._input_dim,
-                                                                  laplacian_matrix=laplacian_matrix[0],
-                                                                  activation=tf.nn.tanh)
-                pass
-    
-
-
-            for graph_index in range(self._num_graph):
-
-
-                gcn_output = GCL.add_multi_gc_layers(tf.reshape(traffic_flow, [-1, self._num_node, self._input_dim]),
-                                                    gcn_k=1, gcn_l=1, output_size=self._input_dim,
-                                                    laplacian_matrix=laplacian_matrix[graph_index],
-                                                    activation=tf.nn.tanh)
-
-                f_k_g = tf.reshape(f_k_g, [-1, self._T, self._num_node, self._input_dim])
-
-
-
-                outputs_temporal = []
-
-
-                for time_step, target_tensor, given_name in temporal_features:
-
-
-
-
-
-                    if self._st_method == 'GCLSTM':
-
-                        multi_layer_cell = tf.keras.layers.StackedRNNCells(
-                            [GCLSTMCell(units=self._num_hidden_unit, num_nodes=self._num_node,
-                                        laplacian_matrix=laplace_matrix[graph_index],
-                                        gcn_k=self._gcn_k, gcn_l=self._gcn_layer)
-                                for _ in range(self._gclstm_layers)])
-
-                        outputs = tf.keras.layers.RNN(multi_layer_cell)(tf.reshape(target_tensor, [-1, time_step, 1]))
-
-                        st_outputs = tf.reshape(outputs, [-1, 1, self._num_hidden_unit])
-
-                    elif self._st_method == 'DCRNN':
-
-                        cell = DCGRUCell(self._num_hidden_unit, 1, self._num_graph,
-                                            # laplace_matrix will be diffusion_matrix when self._st_method == 'DCRNN'
-                                            laplace_matrix,
-                                            max_diffusion_step=self._gcn_k,
-                                            num_nodes=self._num_node, name=str(graph_index) + given_name)
-
-                        encoding_cells = [cell] * self._gclstm_layers
-                        encoding_cells = tf.contrib.rnn.MultiRNNCell(encoding_cells, state_is_tuple=True)
-
-                        inputs_unstack = tf.unstack(tf.reshape(target_tensor, [-1, self._num_node, time_step]),
-                                                    axis=-1)
-
-                        outputs, _ = \
-                            tf.contrib.rnn.static_rnn(encoding_cells, inputs_unstack, dtype=tf.float32)
-
-                        st_outputs = tf.reshape(outputs[-1], [-1, 1, self._num_hidden_unit])
-
-                    elif self._st_method == 'GRU':
-
-                        cell = tf.keras.layers.GRUCell(units=self._num_hidden_unit)
-                        multi_layer_gru = tf.keras.layers.StackedRNNCells([cell] * self._gclstm_layers)
-                        outputs = tf.keras.layers.RNN(multi_layer_gru)(
-                            tf.reshape(target_tensor, [-1, time_step, 1]))
-                        st_outputs = tf.reshape(outputs, [-1, 1, self._num_hidden_unit])
-
-                    elif self._st_method == 'LSTM':
-
-                        cell = tf.keras.layers.LSTMCell(units=self._num_hidden_unit)
-                        multi_layer_gru = tf.keras.layers.StackedRNNCells([cell] * self._gclstm_layers)
-                        outputs = tf.keras.layers.RNN(multi_layer_gru)(
-                            tf.reshape(target_tensor, [-1, time_step, 1]))
-                        st_outputs = tf.reshape(outputs, [-1, 1, self._num_hidden_unit])
-
-                    outputs_temporal.append(st_outputs)
-
-                if self._temporal_merge == 'concat':
-                    
-                    graph_outputs_list.append(tf.concat(outputs_temporal, axis=-1))
-
-                elif self._temporal_merge == 'gal':
-
-                    _, gal_output = GAL.add_ga_layer_matrix(inputs=tf.concat(outputs_temporal, axis=-2),
-                                                            units=self._temporal_merge_gal_units,
-                                                            num_head=self._temporal_merge_gal_num_heads)
-
-                    graph_outputs_list.append(tf.reduce_mean(gal_output, axis=-2, keepdims=True))
-
-
-
-
-
-
-                if self._st_method in ['GCLSTM', 'DCRNN', 'GRU', 'LSTM']:
-
-                    outputs_temporal = []
-
-                    for time_step, target_tensor, given_name in temporal_features:
-
-                        if self._st_method == 'GCLSTM':
-
-                            multi_layer_cell = tf.keras.layers.StackedRNNCells(
-                                [GCLSTMCell(units=self._num_hidden_unit, num_nodes=self._num_node,
-                                            laplacian_matrix=laplace_matrix[graph_index],
-                                            gcn_k=self._gcn_k, gcn_l=self._gcn_layer)
-                                 for _ in range(self._gclstm_layers)])
-
-                            outputs = tf.keras.layers.RNN(multi_layer_cell)(tf.reshape(target_tensor, [-1, time_step, 1]))
-
-                            st_outputs = tf.reshape(outputs, [-1, 1, self._num_hidden_unit])
-
-                        elif self._st_method == 'DCRNN':
-
-                            cell = DCGRUCell(self._num_hidden_unit, 1, self._num_graph,
-                                             # laplace_matrix will be diffusion_matrix when self._st_method == 'DCRNN'
-                                             laplace_matrix,
-                                             max_diffusion_step=self._gcn_k,
-                                             num_nodes=self._num_node, name=str(graph_index) + given_name)
-
-                            encoding_cells = [cell] * self._gclstm_layers
-                            encoding_cells = tf.contrib.rnn.MultiRNNCell(encoding_cells, state_is_tuple=True)
-
-                            inputs_unstack = tf.unstack(tf.reshape(target_tensor, [-1, self._num_node, time_step]),
-                                                        axis=-1)
-
-                            outputs, _ = \
-                                tf.contrib.rnn.static_rnn(encoding_cells, inputs_unstack, dtype=tf.float32)
-
-                            st_outputs = tf.reshape(outputs[-1], [-1, 1, self._num_hidden_unit])
-
-                        elif self._st_method == 'GRU':
-
-                            cell = tf.keras.layers.GRUCell(units=self._num_hidden_unit)
-                            multi_layer_gru = tf.keras.layers.StackedRNNCells([cell] * self._gclstm_layers)
-                            outputs = tf.keras.layers.RNN(multi_layer_gru)(
-                                tf.reshape(target_tensor, [-1, time_step, 1]))
-                            st_outputs = tf.reshape(outputs, [-1, 1, self._num_hidden_unit])
-
-                        elif self._st_method == 'LSTM':
-
-                            cell = tf.keras.layers.LSTMCell(units=self._num_hidden_unit)
-                            multi_layer_gru = tf.keras.layers.StackedRNNCells([cell] * self._gclstm_layers)
-                            outputs = tf.keras.layers.RNN(multi_layer_gru)(
-                                tf.reshape(target_tensor, [-1, time_step, 1]))
-                            st_outputs = tf.reshape(outputs, [-1, 1, self._num_hidden_unit])
-
-                        outputs_temporal.append(st_outputs)
-
-                    if self._temporal_merge == 'concat':
-                        
-                        graph_outputs_list.append(tf.concat(outputs_temporal, axis=-1))
-
-                    elif self._temporal_merge == 'gal':
-
-                        _, gal_output = GAL.add_ga_layer_matrix(inputs=tf.concat(outputs_temporal, axis=-2),
-                                                                units=self._temporal_merge_gal_units,
-                                                                num_head=self._temporal_merge_gal_num_heads)
-
-                        graph_outputs_list.append(tf.reduce_mean(gal_output, axis=-2, keepdims=True))
-
-            if self._num_graph > 1:
-
-                if self._graph_merge == 'gal':
-                    # (graph, inputs_name, units, num_head, activation=tf.nn.leaky_relu)
-                    _, gal_output = GAL.add_ga_layer_matrix(inputs=tf.concat(graph_outputs_list, axis=-2),
-                                                            units=self._graph_merge_gal_units,
-                                                            num_head=self._graph_merge_gal_num_heads)
-                    dense_inputs = tf.reduce_mean(gal_output, axis=-2, keepdims=True)
-
-                elif self._graph_merge == 'concat':
-
-                    dense_inputs = tf.concat(graph_outputs_list, axis=-1)
-
-            else:
-
-                dense_inputs = graph_outputs_list[-1]
-
-            dense_inputs = tf.reshape(dense_inputs, [-1, self._num_node, 1, dense_inputs.get_shape()[-1].value])
-
-            dense_inputs = tf.keras.layers.BatchNormalization(axis=-1, name='feature_map')(dense_inputs)
-
-            # external dims
-            if self._external_dim is not None and self._external_dim > 0:
-                external_input = tf.placeholder(tf.float32, [None, self._external_dim])
-                self._input['external_feature'] = external_input.name
-                external_dense = tf.keras.layers.Dense(units=10)(external_input)
-                external_dense = tf.tile(tf.reshape(external_dense, [-1, 1, 1, 10]),
-                                         [1, tf.shape(dense_inputs)[1], tf.shape(dense_inputs)[2], 1])
-                dense_inputs = tf.concat([dense_inputs, external_dense], axis=-1)
-
-            dense_output0 = tf.keras.layers.Dense(units=self._num_dense_units,
-                                                  activation=tf.nn.tanh,
-                                                  use_bias=True,
-                                                  kernel_initializer='glorot_uniform',
-                                                  bias_initializer='zeros',
-                                                  kernel_regularizer=tf.keras.regularizers.l2(0.01),
-                                                  bias_regularizer=tf.keras.regularizers.l2(0.01)
-                                                  )(dense_inputs)
-
-            dense_output1 = tf.keras.layers.Dense(units=self._num_dense_units,
-                                                  activation=tf.nn.tanh,
-                                                  use_bias=True,
-                                                  kernel_initializer='glorot_uniform',
-                                                  bias_initializer='zeros',
-                                                  kernel_regularizer=tf.keras.regularizers.l2(0.01),
-                                                  bias_regularizer=tf.keras.regularizers.l2(0.01)
-                                                  )(dense_output0)
-
-            pre_output = tf.keras.layers.Dense(units=1,
-                                               activation=tf.nn.tanh,
-                                               use_bias=True,
-                                               kernel_initializer='glorot_uniform',
-                                               bias_initializer='zeros',
-                                               kernel_regularizer=tf.keras.regularizers.l2(0.01),
-                                               bias_regularizer=tf.keras.regularizers.l2(0.01)
-                                               )(dense_output1)
-
-            prediction = tf.reshape(pre_output, [-1, self._num_node, 1], name='prediction')
-
-            loss_pre = tf.sqrt(tf.reduce_mean(tf.square(target - prediction)), name='loss')
-
-            train_op = tf.train.AdamOptimizer(self._lr).minimize(loss_pre, name='train_op')
-
-            # record output
-            self._output['prediction'] = prediction.name
-            self._output['loss'] = loss_pre.name
-
-            # record train operation
-            self._op['train_op'] = train_op.name
-
-        super(MCSTGCN, self).build(init_vars, max_to_keep)
-
-    # Define your '_get_feed_dict function‘, map your input to the tf-model
-    def _get_feed_dict(self,
-                       laplace_matrix,
-                       closeness_feature=None,
-                       period_feature=None,
-                       trend_feature=None,
-                       target=None,
-                       external_feature=None):
-        feed_dict = {
-            'laplace_matrix': laplace_matrix,
-        }
-        if target is not None:
-            feed_dict['target'] = target
-        if self._external_dim is not None and self._external_dim > 0:
-            feed_dict['external_feature'] = external_feature
-        if self._closeness_len is not None and self._closeness_len > 0:
-            feed_dict['closeness_feature'] = closeness_feature
-        if self._period_len is not None and self._period_len > 0:
-            feed_dict['period_feature'] = period_feature
-        if self._trend_len is not None and self._trend_len > 0:
-            feed_dict['trend_feature'] = trend_feature
-        return feed_dict
+import keras
+import tensorflow as tf
+
+from ..model_unit import BaseModel
+from ..model_unit import GAL, GCL
+from ..model_unit import DCGRUCell
+from ..model_unit import GCLSTMCell
+
+
+class MCSTGCN(BaseModel):
+    """
+        Args:
+            num_node(int): Number of nodes in the graph, e.g. number of stations in NYC-Bike dataset.
+            external_dim(int): Dimension of the external feature, e.g. temperature and wind are two dimension.
+            closeness_len(int): The length of closeness data history. The former consecutive ``closeness_len`` time slots
+            of data will be used as closeness history.
+            period_len(int): The length of period data history. The data of exact same time slots in former consecutive
+            ``period_len`` days will be used as period history.
+            trend_len(int): The length of trend data history. The data of exact same time slots in former consecutive
+            ``trend_len`` weeks (every seven days) will be used as trend history.
+            num_graph(int): Number of graphs used in MCSTGCN.
+            gcn_k(int): The highest order of Chebyshev Polynomial approximation in GCN.
+            gcn_layers(int): Number of GCN layers.
+            gclstm_layers(int): Number of STRNN layers, it works on all modes of MCSTGCN such as GCLSTM and DCRNN.
+            num_hidden_units(int): Number of hidden units of RNN.
+            num_dense_units(int): Number of dense units.
+            graph_merge_gal_units(int): Number of units in GAL for merging different graph features.
+                Only works when graph_merge='gal'
+            graph_merge_gal_num_heads(int): Number of heads in GAL for merging different graph features.
+                Only works when graph_merge='gal'
+            temporal_merge_gal_units(int): Number of units in GAL for merging different temporal features.
+                Only works when temporal_merge='gal'
+            temporal_merge_gal_num_heads(int): Number of heads in GAL for merging different temporal features.
+                Only works when temporal_merge='gal'
+            st_method(str): must in ['GCLSTM', 'DCRNN', 'GRU', 'LSTM'], which refers to different
+                spatial-temporal modeling methods.
+                'GCLSTM': GCN for modeling spatial feature, LSTM for modeling temporal feature.
+                'DCRNN': Diffusion Convolution for modeling spatial feature, GRU for modeling temporam frature.
+                'GRU': Ignore the spatial, and model the temporal feature using GRU
+                'LSTM': Ignore the spatial, and model the temporal feature using LSTM
+            temporal_merge(str): must in ['gal', 'concat'], refers to different temporal merging methods,
+                'gal': merge using GAL,
+                'concat': merge by concat and dense
+            graph_merge(str): must in ['gal', 'concat'], refers to different graph merging methods,
+                'gal': merge using GAL,
+                'concat': merge by concat and dense
+            output_activation(function): activation function, e.g. tf.nn.tanh
+            lr(float): Learning rate. Default: 1e-5
+            code_version(str): Current version of this model code, which will be used as filename for saving the model
+            model_dir(str): The directory to store model files. Default:'model_dir'.
+            gpu_device(str): To specify the GPU to use. Default: '0'.
+        """
+
+    def __init__(self,
+                 num_node,
+                 external_dim,
+                 closeness_len,
+                 period_len,
+                 trend_len,
+
+                 # gcn parameters
+                 num_graph=1,
+                 gcn_k=1,
+                 gcn_layers=1,
+                 gclstm_layers=1,
+
+                 # dense units
+                 num_hidden_units=64,
+                 # LSTM units
+                 num_dense_units=32,
+
+                 # merge parameters
+                 graph_merge_gal_units=32,
+                 graph_merge_gal_num_heads=2,
+                 temporal_merge_gal_units=64,
+                 temporal_merge_gal_num_heads=2,
+
+                 # network structure parameters
+                 st_method='GCLSTM',  # gclstm
+                 temporal_merge='gal',  # gal
+                 graph_merge='gal',  # concat
+
+                 output_activation=tf.nn.sigmoid,
+
+                 lr=1e-4,
+                 code_version='MCSTGCN-QuickStart',
+                 model_dir='model_dir',
+                 gpu_device='0', **kwargs):
+
+        super(MCSTGCN, self).__init__(code_version=code_version, model_dir=model_dir, gpu_device=gpu_device)
+
+        self._num_node = num_node
+        self._gcn_k = gcn_k
+        self._gcn_layer = gcn_layers
+        self._graph_merge_gal_units = graph_merge_gal_units
+        self._graph_merge_gal_num_heads = graph_merge_gal_num_heads
+        self._temporal_merge_gal_units = temporal_merge_gal_units
+        self._temporal_merge_gal_num_heads = temporal_merge_gal_num_heads
+        self._gclstm_layers = gclstm_layers
+        self._num_graph = num_graph
+        self._external_dim = external_dim
+        self._output_activation = output_activation
+
+        self._st_method = st_method.upper()
+        self._temporal_merge = temporal_merge
+        self._graph_merge = graph_merge
+
+        self._closeness_len = int(closeness_len)
+        self._period_len = int(period_len)
+        self._trend_len = int(trend_len)
+        self._num_hidden_unit = num_hidden_units
+        self._num_dense_units = num_dense_units
+        self._lr = lr
+    
+    def build(self, init_vars=True, max_to_keep=5):
+        with self._graph.as_default():
+
+            temporal_features = []
+
+            if self._closeness_len is not None and self._closeness_len > 0:
+                closeness_feature = tf.placeholder(tf.float32, [None, None, self._closeness_len, 1],
+                                                   name='closeness_feature')
+                self._input['closeness_feature'] = closeness_feature.name
+                temporal_features.append([self._closeness_len, closeness_feature, 'closeness_feature'])
+
+            if self._period_len is not None and self._period_len > 0:
+                period_feature = tf.placeholder(tf.float32, [None, None, self._period_len, 1],
+                                                name='period_feature')
+                self._input['period_feature'] = period_feature.name
+                temporal_features.append([self._period_len, period_feature, 'period_feature'])
+
+            if self._trend_len is not None and self._trend_len > 0:
+                trend_feature = tf.placeholder(tf.float32, [None, None, self._trend_len, 1],
+                                               name='trend_feature')
+                self._input['trend_feature'] = trend_feature.name
+                temporal_features.append([self._trend_len, trend_feature, 'trend_feature'])
+
+            if len(temporal_features) > 0:
+                target = tf.placeholder(tf.float32, [None, None, 1], name='target')
+                laplace_matrix = tf.placeholder(tf.float32, [self._num_graph, None, None], name='laplace_matrix')
+                self._input['target'] = target.name
+                self._input['laplace_matrix'] = laplace_matrix.name
+            else:
+                raise ValueError('closeness_len, period_len, trend_len cannot all be zero')
+
+            graph_outputs_list = []
+
+
+            for i, time_step, target_tensor, given_name in enumerate(temporal_features):
+                temporal_features[i][1] = GCL.add_multi_gc_layers(tf.reshape(traffic_flow, [-1, self._num_node, self._input_dim]),
+                                                                  gcn_k=1, gcn_l=1, output_size=self._input_dim,
+                                                                  laplacian_matrix=laplacian_matrix[0],
+                                                                  activation=tf.nn.tanh)
+                pass
+    
+
+
+            for graph_index in range(self._num_graph):
+
+
+                gcn_output = GCL.add_multi_gc_layers(tf.reshape(traffic_flow, [-1, self._num_node, self._input_dim]),
+                                                    gcn_k=1, gcn_l=1, output_size=self._input_dim,
+                                                    laplacian_matrix=laplacian_matrix[graph_index],
+                                                    activation=tf.nn.tanh)
+
+                f_k_g = tf.reshape(f_k_g, [-1, self._T, self._num_node, self._input_dim])
+
+
+
+                outputs_temporal = []
+
+
+                for time_step, target_tensor, given_name in temporal_features:
+
+
+
+
+
+                    if self._st_method == 'GCLSTM':
+
+                        multi_layer_cell = tf.keras.layers.StackedRNNCells(
+                            [GCLSTMCell(units=self._num_hidden_unit, num_node=self._num_node,
+                                        laplacian_matrix=laplace_matrix[graph_index],
+                                        gcn_k=self._gcn_k, gcn_l=self._gcn_layer)
+                                for _ in range(self._gclstm_layers)])
+
+                        outputs = tf.keras.layers.RNN(multi_layer_cell)(tf.reshape(target_tensor, [-1, time_step, 1]))
+
+                        st_outputs = tf.reshape(outputs, [-1, 1, self._num_hidden_unit])
+
+                    elif self._st_method == 'DCRNN':
+
+                        cell = DCGRUCell(self._num_hidden_unit, 1, self._num_graph,
+                                            # laplace_matrix will be diffusion_matrix when self._st_method == 'DCRNN'
+                                            laplace_matrix,
+                                            max_diffusion_step=self._gcn_k,
+                                            num_node=self._num_node, name=str(graph_index) + given_name)
+
+                        encoding_cells = [cell] * self._gclstm_layers
+                        encoding_cells = tf.contrib.rnn.MultiRNNCell(encoding_cells, state_is_tuple=True)
+
+                        inputs_unstack = tf.unstack(tf.reshape(target_tensor, [-1, self._num_node, time_step]),
+                                                    axis=-1)
+
+                        outputs, _ = \
+                            tf.contrib.rnn.static_rnn(encoding_cells, inputs_unstack, dtype=tf.float32)
+
+                        st_outputs = tf.reshape(outputs[-1], [-1, 1, self._num_hidden_unit])
+
+                    elif self._st_method == 'GRU':
+
+                        cell = tf.keras.layers.GRUCell(units=self._num_hidden_unit)
+                        multi_layer_gru = tf.keras.layers.StackedRNNCells([cell] * self._gclstm_layers)
+                        outputs = tf.keras.layers.RNN(multi_layer_gru)(
+                            tf.reshape(target_tensor, [-1, time_step, 1]))
+                        st_outputs = tf.reshape(outputs, [-1, 1, self._num_hidden_unit])
+
+                    elif self._st_method == 'LSTM':
+
+                        cell = tf.keras.layers.LSTMCell(units=self._num_hidden_unit)
+                        multi_layer_gru = tf.keras.layers.StackedRNNCells([cell] * self._gclstm_layers)
+                        outputs = tf.keras.layers.RNN(multi_layer_gru)(
+                            tf.reshape(target_tensor, [-1, time_step, 1]))
+                        st_outputs = tf.reshape(outputs, [-1, 1, self._num_hidden_unit])
+
+                    outputs_temporal.append(st_outputs)
+
+                if self._temporal_merge == 'concat':
+                    
+                    graph_outputs_list.append(tf.concat(outputs_temporal, axis=-1))
+
+                elif self._temporal_merge == 'gal':
+
+                    _, gal_output = GAL.add_ga_layer_matrix(inputs=tf.concat(outputs_temporal, axis=-2),
+                                                            units=self._temporal_merge_gal_units,
+                                                            num_head=self._temporal_merge_gal_num_heads)
+
+                    graph_outputs_list.append(tf.reduce_mean(gal_output, axis=-2, keepdims=True))
+
+
+
+
+
+
+                if self._st_method in ['GCLSTM', 'DCRNN', 'GRU', 'LSTM']:
+
+                    outputs_temporal = []
+
+                    for time_step, target_tensor, given_name in temporal_features:
+
+                        if self._st_method == 'GCLSTM':
+
+                            multi_layer_cell = tf.keras.layers.StackedRNNCells(
+                                [GCLSTMCell(units=self._num_hidden_unit, num_node=self._num_node,
+                                            laplacian_matrix=laplace_matrix[graph_index],
+                                            gcn_k=self._gcn_k, gcn_l=self._gcn_layer)
+                                 for _ in range(self._gclstm_layers)])
+
+                            outputs = tf.keras.layers.RNN(multi_layer_cell)(tf.reshape(target_tensor, [-1, time_step, 1]))
+
+                            st_outputs = tf.reshape(outputs, [-1, 1, self._num_hidden_unit])
+
+                        elif self._st_method == 'DCRNN':
+
+                            cell = DCGRUCell(self._num_hidden_unit, 1, self._num_graph,
+                                             # laplace_matrix will be diffusion_matrix when self._st_method == 'DCRNN'
+                                             laplace_matrix,
+                                             max_diffusion_step=self._gcn_k,
+                                             num_node=self._num_node, name=str(graph_index) + given_name)
+
+                            encoding_cells = [cell] * self._gclstm_layers
+                            encoding_cells = tf.contrib.rnn.MultiRNNCell(encoding_cells, state_is_tuple=True)
+
+                            inputs_unstack = tf.unstack(tf.reshape(target_tensor, [-1, self._num_node, time_step]),
+                                                        axis=-1)
+
+                            outputs, _ = \
+                                tf.contrib.rnn.static_rnn(encoding_cells, inputs_unstack, dtype=tf.float32)
+
+                            st_outputs = tf.reshape(outputs[-1], [-1, 1, self._num_hidden_unit])
+
+                        elif self._st_method == 'GRU':
+
+                            cell = tf.keras.layers.GRUCell(units=self._num_hidden_unit)
+                            multi_layer_gru = tf.keras.layers.StackedRNNCells([cell] * self._gclstm_layers)
+                            outputs = tf.keras.layers.RNN(multi_layer_gru)(
+                                tf.reshape(target_tensor, [-1, time_step, 1]))
+                            st_outputs = tf.reshape(outputs, [-1, 1, self._num_hidden_unit])
+
+                        elif self._st_method == 'LSTM':
+
+                            cell = tf.keras.layers.LSTMCell(units=self._num_hidden_unit)
+                            multi_layer_gru = tf.keras.layers.StackedRNNCells([cell] * self._gclstm_layers)
+                            outputs = tf.keras.layers.RNN(multi_layer_gru)(
+                                tf.reshape(target_tensor, [-1, time_step, 1]))
+                            st_outputs = tf.reshape(outputs, [-1, 1, self._num_hidden_unit])
+
+                        outputs_temporal.append(st_outputs)
+
+                    if self._temporal_merge == 'concat':
+                        
+                        graph_outputs_list.append(tf.concat(outputs_temporal, axis=-1))
+
+                    elif self._temporal_merge == 'gal':
+
+                        _, gal_output = GAL.add_ga_layer_matrix(inputs=tf.concat(outputs_temporal, axis=-2),
+                                                                units=self._temporal_merge_gal_units,
+                                                                num_head=self._temporal_merge_gal_num_heads)
+
+                        graph_outputs_list.append(tf.reduce_mean(gal_output, axis=-2, keepdims=True))
+
+            if self._num_graph > 1:
+
+                if self._graph_merge == 'gal':
+                    # (graph, inputs_name, units, num_head, activation=tf.nn.leaky_relu)
+                    _, gal_output = GAL.add_ga_layer_matrix(inputs=tf.concat(graph_outputs_list, axis=-2),
+                                                            units=self._graph_merge_gal_units,
+                                                            num_head=self._graph_merge_gal_num_heads)
+                    dense_inputs = tf.reduce_mean(gal_output, axis=-2, keepdims=True)
+
+                elif self._graph_merge == 'concat':
+
+                    dense_inputs = tf.concat(graph_outputs_list, axis=-1)
+
+            else:
+
+                dense_inputs = graph_outputs_list[-1]
+
+            dense_inputs = tf.reshape(dense_inputs, [-1, self._num_node, 1, dense_inputs.get_shape()[-1].value])
+
+            dense_inputs = tf.keras.layers.BatchNormalization(axis=-1, name='feature_map')(dense_inputs)
+
+            # external dims
+            if self._external_dim is not None and self._external_dim > 0:
+                external_input = tf.placeholder(tf.float32, [None, self._external_dim])
+                self._input['external_feature'] = external_input.name
+                external_dense = tf.keras.layers.Dense(units=10)(external_input)
+                external_dense = tf.tile(tf.reshape(external_dense, [-1, 1, 1, 10]),
+                                         [1, tf.shape(dense_inputs)[1], tf.shape(dense_inputs)[2], 1])
+                dense_inputs = tf.concat([dense_inputs, external_dense], axis=-1)
+
+            dense_output0 = tf.keras.layers.Dense(units=self._num_dense_units,
+                                                  activation=tf.nn.tanh,
+                                                  use_bias=True,
+                                                  kernel_initializer='glorot_uniform',
+                                                  bias_initializer='zeros',
+                                                  kernel_regularizer=tf.keras.regularizers.l2(0.01),
+                                                  bias_regularizer=tf.keras.regularizers.l2(0.01)
+                                                  )(dense_inputs)
+
+            dense_output1 = tf.keras.layers.Dense(units=self._num_dense_units,
+                                                  activation=tf.nn.tanh,
+                                                  use_bias=True,
+                                                  kernel_initializer='glorot_uniform',
+                                                  bias_initializer='zeros',
+                                                  kernel_regularizer=tf.keras.regularizers.l2(0.01),
+                                                  bias_regularizer=tf.keras.regularizers.l2(0.01)
+                                                  )(dense_output0)
+
+            pre_output = tf.keras.layers.Dense(units=1,
+                                               activation=tf.nn.tanh,
+                                               use_bias=True,
+                                               kernel_initializer='glorot_uniform',
+                                               bias_initializer='zeros',
+                                               kernel_regularizer=tf.keras.regularizers.l2(0.01),
+                                               bias_regularizer=tf.keras.regularizers.l2(0.01)
+                                               )(dense_output1)
+
+            prediction = tf.reshape(pre_output, [-1, self._num_node, 1], name='prediction')
+
+            loss_pre = tf.sqrt(tf.reduce_mean(tf.square(target - prediction)), name='loss')
+
+            train_op = tf.train.AdamOptimizer(self._lr).minimize(loss_pre, name='train_op')
+
+            # record output
+            self._output['prediction'] = prediction.name
+            self._output['loss'] = loss_pre.name
+
+            # record train operation
+            self._op['train_op'] = train_op.name
+
+        super(MCSTGCN, self).build(init_vars, max_to_keep)
+
+    # Define your '_get_feed_dict function‘, map your input to the tf-model
+    def _get_feed_dict(self,
+                       laplace_matrix,
+                       closeness_feature=None,
+                       period_feature=None,
+                       trend_feature=None,
+                       target=None,
+                       external_feature=None):
+        feed_dict = {
+            'laplace_matrix': laplace_matrix,
+        }
+        if target is not None:
+            feed_dict['target'] = target
+        if self._external_dim is not None and self._external_dim > 0:
+            feed_dict['external_feature'] = external_feature
+        if self._closeness_len is not None and self._closeness_len > 0:
+            feed_dict['closeness_feature'] = closeness_feature
+        if self._period_len is not None and self._period_len > 0:
+            feed_dict['period_feature'] = period_feature
+        if self._trend_len is not None and self._trend_len > 0:
+            feed_dict['trend_feature'] = trend_feature
+        return feed_dict
```

### Comparing `UCTB-0.3.0/UCTB/model/STMeta.py` & `UCTB-0.3.5/UCTB/model/STMeta.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,310 +1,313 @@
-import keras
-import tensorflow as tf
-
-from ..model_unit import BaseModel
-from ..model_unit import GAL, GCL
-from ..model_unit import DCGRUCell
-from ..model_unit import GCLSTMCell
-
-
-class STMeta(BaseModel):
-    """
-        Args:
-            num_node(int): Number of nodes in the graph, e.g. number of stations in NYC-Bike dataset.
-            external_dim(int): Dimension of the external feature, e.g. temperature and wind are two dimension.
-            closeness_len(int): The length of closeness data history. The former consecutive ``closeness_len`` time slots
-            of data will be used as closeness history.
-            period_len(int): The length of period data history. The data of exact same time slots in former consecutive
-            ``period_len`` days will be used as period history.
-            trend_len(int): The length of trend data history. The data of exact same time slots in former consecutive
-            ``trend_len`` weeks (every seven days) will be used as trend history.
-            num_graph(int): Number of graphs used in STMeta.
-            gcn_k(int): The highest order of Chebyshev Polynomial approximation in GCN.
-            gcn_layers(int): Number of GCN layers.
-            gclstm_layers(int): Number of STRNN layers, it works on all modes of STMeta such as GCLSTM and DCRNN.
-            num_hidden_units(int): Number of hidden units of RNN.
-            num_dense_units(int): Number of dense units.
-            graph_merge_gal_units(int): Number of units in GAL for merging different graph features.
-                Only works when graph_merge='gal'
-            graph_merge_gal_num_heads(int): Number of heads in GAL for merging different graph features.
-                Only works when graph_merge='gal'
-            temporal_merge_gal_units(int): Number of units in GAL for merging different temporal features.
-                Only works when temporal_merge='gal'
-            temporal_merge_gal_num_heads(int): Number of heads in GAL for merging different temporal features.
-                Only works when temporal_merge='gal'
-            st_method(str): must in ['GCLSTM', 'DCRNN', 'GRU', 'LSTM'], which refers to different
-                spatial-temporal modeling methods.
-                'GCLSTM': GCN for modeling spatial feature, LSTM for modeling temporal feature.
-                'DCRNN': Diffusion Convolution for modeling spatial feature, GRU for modeling temporam frature.
-                'GRU': Ignore the spatial, and model the temporal feature using GRU
-                'LSTM': Ignore the spatial, and model the temporal feature using LSTM
-            temporal_merge(str): must in ['gal', 'concat'], refers to different temporal merging methods,
-                'gal': merge using GAL,
-                'concat': merge by concat and dense
-            graph_merge(str): must in ['gal', 'concat'], refers to different graph merging methods,
-                'gal': merge using GAL,
-                'concat': merge by concat and dense
-            output_activation(function): activation function, e.g. tf.nn.tanh
-            lr(float): Learning rate. Default: 1e-5
-            code_version(str): Current version of this model code, which will be used as filename for saving the model
-            model_dir(str): The directory to store model files. Default:'model_dir'.
-            gpu_device(str): To specify the GPU to use. Default: '0'.
-        """
-
-    def __init__(self,
-                 num_node,
-                 external_dim,
-                 closeness_len,
-                 period_len,
-                 trend_len,
-
-                 # gcn parameters
-                 num_graph=1,
-                 gcn_k=1,
-                 gcn_layers=1,
-                 gclstm_layers=1,
-
-                 # dense units
-                 num_hidden_units=64,
-                 # LSTM units
-                 num_dense_units=32,
-
-                 # merge parameters
-                 graph_merge_gal_units=32,
-                 graph_merge_gal_num_heads=2,
-                 temporal_merge_gal_units=64,
-                 temporal_merge_gal_num_heads=2,
-
-                 # network structure parameters
-                 st_method='GCLSTM',  # gclstm
-                 temporal_merge='gal',  # gal
-                 graph_merge='gal',  # concat
-
-                 output_activation=tf.nn.sigmoid,
-
-                 lr=1e-4,
-                 code_version='STMeta-QuickStart',
-                 model_dir='model_dir',
-                 gpu_device='0', **kwargs):
-
-        super(STMeta, self).__init__(code_version=code_version, model_dir=model_dir, gpu_device=gpu_device)
-
-        self._num_node = num_node
-        self._gcn_k = gcn_k
-        self._gcn_layer = gcn_layers
-        self._graph_merge_gal_units = graph_merge_gal_units
-        self._graph_merge_gal_num_heads = graph_merge_gal_num_heads
-        self._temporal_merge_gal_units = temporal_merge_gal_units
-        self._temporal_merge_gal_num_heads = temporal_merge_gal_num_heads
-        self._gclstm_layers = gclstm_layers
-        self._num_graph = num_graph
-        self._external_dim = external_dim
-        self._output_activation = output_activation
-
-        self._st_method = st_method.upper()
-        self._temporal_merge = temporal_merge
-        self._graph_merge = graph_merge
-
-        self._closeness_len = int(closeness_len)
-        self._period_len = int(period_len)
-        self._trend_len = int(trend_len)
-        self._num_hidden_unit = num_hidden_units
-        self._num_dense_units = num_dense_units
-        self._lr = lr
-    
-    def build(self, init_vars=True, max_to_keep=5):
-        with self._graph.as_default():
-
-            temporal_features = []
-
-            if self._closeness_len is not None and self._closeness_len > 0:
-                closeness_feature = tf.placeholder(tf.float32, [None, None, self._closeness_len, 1],
-                                                   name='closeness_feature')
-                self._input['closeness_feature'] = closeness_feature.name
-                temporal_features.append([self._closeness_len, closeness_feature, 'closeness_feature'])
-
-            if self._period_len is not None and self._period_len > 0:
-                period_feature = tf.placeholder(tf.float32, [None, None, self._period_len, 1],
-                                                name='period_feature')
-                self._input['period_feature'] = period_feature.name
-                temporal_features.append([self._period_len, period_feature, 'period_feature'])
-
-            if self._trend_len is not None and self._trend_len > 0:
-                trend_feature = tf.placeholder(tf.float32, [None, None, self._trend_len, 1],
-                                               name='trend_feature')
-                self._input['trend_feature'] = trend_feature.name
-                temporal_features.append([self._trend_len, trend_feature, 'trend_feature'])
-
-            if len(temporal_features) > 0:
-                target = tf.placeholder(tf.float32, [None, None, 1], name='target')
-                laplace_matrix = tf.placeholder(tf.float32, [self._num_graph, None, None], name='laplace_matrix')
-                self._input['target'] = target.name
-                self._input['laplace_matrix'] = laplace_matrix.name
-            else:
-                raise ValueError('closeness_len, period_len, trend_len cannot all be zero')
-
-            graph_outputs_list = []
-
-            for graph_index in range(self._num_graph):
-
-                if self._st_method in ['GCLSTM', 'DCRNN', 'GRU', 'LSTM']:
-
-                    outputs_temporal = []
-
-                    for time_step, target_tensor, given_name in temporal_features:
-
-                        if self._st_method == 'GCLSTM':
-
-                            multi_layer_cell = tf.keras.layers.StackedRNNCells(
-                                [GCLSTMCell(units=self._num_hidden_unit, num_nodes=self._num_node,
-                                            laplacian_matrix=laplace_matrix[graph_index],
-                                            gcn_k=self._gcn_k, gcn_l=self._gcn_layer)
-                                 for _ in range(self._gclstm_layers)])
-
-                            outputs = tf.keras.layers.RNN(multi_layer_cell)(tf.reshape(target_tensor, [-1, time_step, 1]))
-
-                            st_outputs = tf.reshape(outputs, [-1, 1, self._num_hidden_unit])
-
-                        elif self._st_method == 'DCRNN':
-
-                            cell = DCGRUCell(self._num_hidden_unit, 1, self._num_graph,
-                                             # laplace_matrix will be diffusion_matrix when self._st_method == 'DCRNN'
-                                             laplace_matrix,
-                                             max_diffusion_step=self._gcn_k,
-                                             num_nodes=self._num_node, name=str(graph_index) + given_name)
-
-                            encoding_cells = [cell] * self._gclstm_layers
-                            encoding_cells = tf.contrib.rnn.MultiRNNCell(encoding_cells, state_is_tuple=True)
-
-                            inputs_unstack = tf.unstack(tf.reshape(target_tensor, [-1, self._num_node, time_step]),
-                                                        axis=-1)
-
-                            outputs, _ = \
-                                tf.contrib.rnn.static_rnn(encoding_cells, inputs_unstack, dtype=tf.float32)
-
-                            st_outputs = tf.reshape(outputs[-1], [-1, 1, self._num_hidden_unit])
-
-                        elif self._st_method == 'GRU':
-
-                            cell = tf.keras.layers.GRUCell(units=self._num_hidden_unit)
-                            multi_layer_gru = tf.keras.layers.StackedRNNCells([cell] * self._gclstm_layers)
-                            outputs = tf.keras.layers.RNN(multi_layer_gru)(
-                                tf.reshape(target_tensor, [-1, time_step, 1]))
-                            st_outputs = tf.reshape(outputs, [-1, 1, self._num_hidden_unit])
-
-                        elif self._st_method == 'LSTM':
-
-                            cell = tf.keras.layers.LSTMCell(units=self._num_hidden_unit)
-                            multi_layer_gru = tf.keras.layers.StackedRNNCells([cell] * self._gclstm_layers)
-                            outputs = tf.keras.layers.RNN(multi_layer_gru)(
-                                tf.reshape(target_tensor, [-1, time_step, 1]))
-                            st_outputs = tf.reshape(outputs, [-1, 1, self._num_hidden_unit])
-
-                        outputs_temporal.append(st_outputs)
-
-                    if self._temporal_merge == 'concat':
-                        
-                        graph_outputs_list.append(tf.concat(outputs_temporal, axis=-1))
-
-                    elif self._temporal_merge == 'gal':
-
-                        _, gal_output = GAL.add_ga_layer_matrix(inputs=tf.concat(outputs_temporal, axis=-2),
-                                                                units=self._temporal_merge_gal_units,
-                                                                num_head=self._temporal_merge_gal_num_heads)
-
-                        graph_outputs_list.append(tf.reduce_mean(gal_output, axis=-2, keepdims=True))
-
-            if self._num_graph > 1:
-
-                if self._graph_merge == 'gal':
-                    # (graph, inputs_name, units, num_head, activation=tf.nn.leaky_relu)
-                    _, gal_output = GAL.add_ga_layer_matrix(inputs=tf.concat(graph_outputs_list, axis=-2),
-                                                            units=self._graph_merge_gal_units,
-                                                            num_head=self._graph_merge_gal_num_heads)
-                    dense_inputs = tf.reduce_mean(gal_output, axis=-2, keepdims=True)
-
-                elif self._graph_merge == 'concat':
-
-                    dense_inputs = tf.concat(graph_outputs_list, axis=-1)
-
-            else:
-
-                dense_inputs = graph_outputs_list[-1]
-
-            dense_inputs = tf.reshape(dense_inputs, [-1, self._num_node, 1, dense_inputs.get_shape()[-1].value])
-
-            dense_inputs = tf.keras.layers.BatchNormalization(axis=-1, name='feature_map')(dense_inputs)
-
-            # external dims
-            if self._external_dim is not None and self._external_dim > 0:
-                external_input = tf.placeholder(tf.float32, [None, self._external_dim])
-                self._input['external_feature'] = external_input.name
-                external_dense = tf.keras.layers.Dense(units=10)(external_input)
-                external_dense = tf.tile(tf.reshape(external_dense, [-1, 1, 1, 10]),
-                                         [1, tf.shape(dense_inputs)[1], tf.shape(dense_inputs)[2], 1])
-                dense_inputs = tf.concat([dense_inputs, external_dense], axis=-1)
-
-            dense_output0 = tf.keras.layers.Dense(units=self._num_dense_units,
-                                                  activation=tf.nn.tanh,
-                                                  use_bias=True,
-                                                  kernel_initializer='glorot_uniform',
-                                                  bias_initializer='zeros',
-                                                  kernel_regularizer=tf.keras.regularizers.l2(0.01),
-                                                  bias_regularizer=tf.keras.regularizers.l2(0.01)
-                                                  )(dense_inputs)
-
-            dense_output1 = tf.keras.layers.Dense(units=self._num_dense_units,
-                                                  activation=tf.nn.tanh,
-                                                  use_bias=True,
-                                                  kernel_initializer='glorot_uniform',
-                                                  bias_initializer='zeros',
-                                                  kernel_regularizer=tf.keras.regularizers.l2(0.01),
-                                                  bias_regularizer=tf.keras.regularizers.l2(0.01)
-                                                  )(dense_output0)
-
-            pre_output = tf.keras.layers.Dense(units=1,
-                                               activation=tf.nn.tanh,
-                                               use_bias=True,
-                                               kernel_initializer='glorot_uniform',
-                                               bias_initializer='zeros',
-                                               kernel_regularizer=tf.keras.regularizers.l2(0.01),
-                                               bias_regularizer=tf.keras.regularizers.l2(0.01)
-                                               )(dense_output1)
-
-            prediction = tf.reshape(pre_output, [-1, self._num_node, 1], name='prediction')
-
-            loss_pre = tf.sqrt(tf.reduce_mean(tf.square(target - prediction)), name='loss')
-
-            train_op = tf.train.AdamOptimizer(self._lr).minimize(loss_pre, name='train_op')
-
-            # record output
-            self._output['prediction'] = prediction.name
-            self._output['loss'] = loss_pre.name
-
-            # record train operation
-            self._op['train_op'] = train_op.name
-
-        super(STMeta, self).build(init_vars, max_to_keep)
-
-    # Define your '_get_feed_dict function‘, map your input to the tf-model
-    def _get_feed_dict(self,
-                       laplace_matrix,
-                       closeness_feature=None,
-                       period_feature=None,
-                       trend_feature=None,
-                       target=None,
-                       external_feature=None):
-        feed_dict = {
-            'laplace_matrix': laplace_matrix,
-        }
-        if target is not None:
-            feed_dict['target'] = target
-        if self._external_dim is not None and self._external_dim > 0:
-            feed_dict['external_feature'] = external_feature
-        if self._closeness_len is not None and self._closeness_len > 0:
-            feed_dict['closeness_feature'] = closeness_feature
-        if self._period_len is not None and self._period_len > 0:
-            feed_dict['period_feature'] = period_feature
-        if self._trend_len is not None and self._trend_len > 0:
-            feed_dict['trend_feature'] = trend_feature
-        return feed_dict
+import keras
+import tensorflow as tf
+
+from ..model_unit import BaseModel
+from ..model_unit import GAL, GCL
+from ..model_unit import DCGRUCell
+from ..model_unit import GCLSTMCell
+
+
+class STMeta(BaseModel):
+    """
+        Args:
+            num_node(int): Number of nodes in the graph, e.g. number of stations in NYC-Bike dataset.
+            external_dim(int): Dimension of the external feature, e.g. temperature and wind are two dimension.
+            closeness_len(int): The length of closeness data history. The former consecutive ``closeness_len`` time slots
+            of data will be used as closeness history.
+            period_len(int): The length of period data history. The data of exact same time slots in former consecutive
+            ``period_len`` days will be used as period history.
+            trend_len(int): The length of trend data history. The data of exact same time slots in former consecutive
+            ``trend_len`` weeks (every seven days) will be used as trend history.
+            input_dim(int): The dimension of input features. 1 if "with_tpe" (data_loader parameters) = False, otherwise 0.
+            num_graph(int): Number of graphs used in STMeta.
+            gcn_k(int): The highest order of Chebyshev Polynomial approximation in GCN.
+            gcn_layers(int): Number of GCN layers.
+            gclstm_layers(int): Number of STRNN layers, it works on all modes of STMeta such as GCLSTM and DCRNN.
+            num_hidden_units(int): Number of hidden units of RNN.
+            num_dense_units(int): Number of dense units.
+            graph_merge_gal_units(int): Number of units in GAL for merging different graph features.
+                Only works when graph_merge='gal'
+            graph_merge_gal_num_heads(int): Number of heads in GAL for merging different graph features.
+                Only works when graph_merge='gal'
+            temporal_merge_gal_units(int): Number of units in GAL for merging different temporal features.
+                Only works when temporal_merge='gal'
+            temporal_merge_gal_num_heads(int): Number of heads in GAL for merging different temporal features.
+                Only works when temporal_merge='gal'
+            st_method(str): must in ['GCLSTM', 'DCRNN', 'GRU', 'LSTM'], which refers to different
+                spatial-temporal modeling methods.
+                'GCLSTM': GCN for modeling spatial feature, LSTM for modeling temporal feature.
+                'DCRNN': Diffusion Convolution for modeling spatial feature, GRU for modeling temporam frature.
+                'GRU': Ignore the spatial, and model the temporal feature using GRU
+                'LSTM': Ignore the spatial, and model the temporal feature using LSTM
+            temporal_merge(str): must in ['gal', 'concat'], refers to different temporal merging methods,
+                'gal': merge using GAL,
+                'concat': merge by concat and dense
+            graph_merge(str): must in ['gal', 'concat'], refers to different graph merging methods,
+                'gal': merge using GAL,
+                'concat': merge by concat and dense
+            output_activation(function): activation function, e.g. tf.nn.tanh
+            lr(float): Learning rate. Default: 1e-5
+            code_version(str): Current version of this model code, which will be used as filename for saving the model
+            model_dir(str): The directory to store model files. Default:'model_dir'.
+            gpu_device(str): To specify the GPU to use. Default: '0'.
+        """
+
+    def __init__(self,
+                 num_node,
+                 external_dim,
+                 closeness_len,
+                 period_len,
+                 trend_len,
+                 input_dim=1,
+
+                 # gcn parameters
+                 num_graph=1,
+                 gcn_k=1,
+                 gcn_layers=1,
+                 gclstm_layers=1,
+
+                 # dense units
+                 num_hidden_units=64,
+                 # LSTM units
+                 num_dense_units=32,
+
+                 # merge parameters
+                 graph_merge_gal_units=32,
+                 graph_merge_gal_num_heads=2,
+                 temporal_merge_gal_units=64,
+                 temporal_merge_gal_num_heads=2,
+
+                 # network structure parameters
+                 st_method='GCLSTM',  # gclstm
+                 temporal_merge='gal',  # gal
+                 graph_merge='gal',  # concat
+
+                 output_activation=tf.nn.sigmoid,
+
+                 lr=1e-4,
+                 code_version='STMeta-QuickStart',
+                 model_dir='model_dir',
+                 gpu_device='0', **kwargs):
+
+        super(STMeta, self).__init__(code_version=code_version, model_dir=model_dir, gpu_device=gpu_device)
+
+        self._num_node = num_node
+        self._input_dim = input_dim
+        print("self._input_dim",self._input_dim)
+        self._gcn_k = gcn_k
+        self._gcn_layer = gcn_layers
+        self._graph_merge_gal_units = graph_merge_gal_units
+        self._graph_merge_gal_num_heads = graph_merge_gal_num_heads
+        self._temporal_merge_gal_units = temporal_merge_gal_units
+        self._temporal_merge_gal_num_heads = temporal_merge_gal_num_heads
+        self._gclstm_layers = gclstm_layers
+        self._num_graph = num_graph
+        self._external_dim = external_dim
+        self._output_activation = output_activation
+
+        self._st_method = st_method.upper()
+        self._temporal_merge = temporal_merge
+        self._graph_merge = graph_merge
+
+        self._closeness_len = int(closeness_len)
+        self._period_len = int(period_len)
+        self._trend_len = int(trend_len)
+        self._num_hidden_unit = num_hidden_units
+        self._num_dense_units = num_dense_units
+        self._lr = lr
+    
+    def build(self, init_vars=True, max_to_keep=5):
+        with self._graph.as_default():
+
+            temporal_features = []
+
+            if self._closeness_len is not None and self._closeness_len > 0:
+                closeness_feature = tf.placeholder(tf.float32, [None, None, self._closeness_len, self._input_dim],
+                                                   name='closeness_feature')
+                self._input['closeness_feature'] = closeness_feature.name
+                temporal_features.append([self._closeness_len, closeness_feature, 'closeness_feature'])
+
+            if self._period_len is not None and self._period_len > 0:
+                period_feature = tf.placeholder(tf.float32, [None, None, self._period_len, self._input_dim],
+                                                name='period_feature')
+                self._input['period_feature'] = period_feature.name
+                temporal_features.append([self._period_len, period_feature, 'period_feature'])
+
+            if self._trend_len is not None and self._trend_len > 0:
+                trend_feature = tf.placeholder(tf.float32, [None, None, self._trend_len, self._input_dim],
+                                               name='trend_feature')
+                self._input['trend_feature'] = trend_feature.name
+                temporal_features.append([self._trend_len, trend_feature, 'trend_feature'])
+
+            if len(temporal_features) > 0:
+                target = tf.placeholder(tf.float32, [None, None, 1], name='target')
+                laplace_matrix = tf.placeholder(tf.float32, [self._num_graph, None, None], name='laplace_matrix')
+                self._input['target'] = target.name
+                self._input['laplace_matrix'] = laplace_matrix.name
+            else:
+                raise ValueError('closeness_len, period_len, trend_len cannot all be zero')
+
+            graph_outputs_list = []
+
+            for graph_index in range(self._num_graph):
+
+                if self._st_method in ['GCLSTM', 'DCRNN', 'GRU', 'LSTM']:
+
+                    outputs_temporal = []
+
+                    for time_step, target_tensor, given_name in temporal_features:
+
+                        if self._st_method == 'GCLSTM':
+
+                            multi_layer_cell = tf.keras.layers.StackedRNNCells(
+                                [GCLSTMCell(units=self._num_hidden_unit, num_node=self._num_node,
+                                            laplacian_matrix=laplace_matrix[graph_index],
+                                            gcn_k=self._gcn_k, gcn_l=self._gcn_layer)
+                                 for _ in range(self._gclstm_layers)])
+
+                            outputs = tf.keras.layers.RNN(multi_layer_cell)(tf.reshape(target_tensor, [-1, time_step, self._input_dim]))
+
+                            st_outputs = tf.reshape(outputs, [-1, 1, self._num_hidden_unit])
+
+                        elif self._st_method == 'DCRNN':
+                        # laplace_matrix will be diffusion_matrix when self._st_method == 'DCRNN'
+
+                            encoding_cells = [DCGRUCell(self._num_hidden_unit, self._input_dim, self._num_graph,
+                                             laplace_matrix,
+                                             max_diffusion_step=self._gcn_k,
+                                             num_node=self._num_node, name=str(graph_index) + given_name) for _ in range(self._gclstm_layers)]
+
+                            encoding_cells = tf.contrib.rnn.MultiRNNCell(encoding_cells, state_is_tuple=True)
+
+                            inputs_unstack = tf.unstack(tf.reshape(target_tensor, [-1, self._num_node, time_step]),
+                                                        axis=-1)
+
+                            outputs, _ = \
+                                tf.contrib.rnn.static_rnn(encoding_cells, inputs_unstack, dtype=tf.float32)
+
+                            st_outputs = tf.reshape(outputs[-1], [-1, 1, self._num_hidden_unit])
+
+                        elif self._st_method == 'GRU':
+
+                            multi_layer_gru = tf.keras.layers.StackedRNNCells([tf.keras.layers.GRUCell(units=self._num_hidden_unit) for _ in range(self._gclstm_layers)])
+                            
+                            outputs = tf.keras.layers.RNN(multi_layer_gru)(
+                                tf.reshape(target_tensor, [-1, time_step, self._input_dim]))
+                            st_outputs = tf.reshape(outputs, [-1, 1, self._num_hidden_unit])
+
+                        elif self._st_method == 'LSTM':
+
+                            multi_layer_gru = tf.keras.layers.StackedRNNCells([tf.keras.layers.LSTMCell(units=self._num_hidden_unit) for _ in range(self._gclstm_layers)])
+                            
+                            outputs = tf.keras.layers.RNN(multi_layer_gru)(
+                                tf.reshape(target_tensor, [-1, time_step, self._input_dim]))
+                            st_outputs = tf.reshape(outputs, [-1, 1, self._num_hidden_unit])
+
+                        outputs_temporal.append(st_outputs)
+
+                    if self._temporal_merge == 'concat':
+                        
+                        graph_outputs_list.append(tf.concat(outputs_temporal, axis=-1))
+
+                    elif self._temporal_merge == 'gal':
+
+                        _, gal_output = GAL.add_ga_layer_matrix(inputs=tf.concat(outputs_temporal, axis=-2),
+                                                                units=self._temporal_merge_gal_units,
+                                                                num_head=self._temporal_merge_gal_num_heads)
+
+                        graph_outputs_list.append(tf.reduce_mean(gal_output, axis=-2, keepdims=True))
+
+            if self._num_graph > 1:
+
+                if self._graph_merge == 'gal':
+                    # (graph, inputs_name, units, num_head, activation=tf.nn.leaky_relu)
+                    _, gal_output = GAL.add_ga_layer_matrix(inputs=tf.concat(graph_outputs_list, axis=-2),
+                                                            units=self._graph_merge_gal_units,
+                                                            num_head=self._graph_merge_gal_num_heads)
+                    dense_inputs = tf.reduce_mean(gal_output, axis=-2, keepdims=True)
+
+                elif self._graph_merge == 'concat':
+
+                    dense_inputs = tf.concat(graph_outputs_list, axis=-1)
+
+            else:
+
+                dense_inputs = graph_outputs_list[-1]
+
+            dense_inputs = tf.reshape(dense_inputs, [-1, self._num_node, 1, dense_inputs.get_shape()[-1].value])
+
+            dense_inputs = tf.keras.layers.BatchNormalization(axis=-1, name='feature_map')(dense_inputs)
+
+            # external dims
+            if self._external_dim is not None and self._external_dim > 0:
+                external_input = tf.placeholder(tf.float32, [None, self._external_dim])
+                self._input['external_feature'] = external_input.name
+                external_dense = tf.keras.layers.Dense(units=10)(external_input)
+                external_dense = tf.tile(tf.reshape(external_dense, [-1, 1, 1, 10]),
+                                         [1, tf.shape(dense_inputs)[1], tf.shape(dense_inputs)[2], 1])
+                dense_inputs = tf.concat([dense_inputs, external_dense], axis=-1)
+
+            dense_output0 = tf.keras.layers.Dense(units=self._num_dense_units,
+                                                  activation=tf.nn.tanh,
+                                                  use_bias=True,
+                                                  kernel_initializer='glorot_uniform',
+                                                  bias_initializer='zeros',
+                                                  kernel_regularizer=tf.keras.regularizers.l2(0.01),
+                                                  bias_regularizer=tf.keras.regularizers.l2(0.01)
+                                                  )(dense_inputs)
+
+            dense_output1 = tf.keras.layers.Dense(units=self._num_dense_units,
+                                                  activation=tf.nn.tanh,
+                                                  use_bias=True,
+                                                  kernel_initializer='glorot_uniform',
+                                                  bias_initializer='zeros',
+                                                  kernel_regularizer=tf.keras.regularizers.l2(0.01),
+                                                  bias_regularizer=tf.keras.regularizers.l2(0.01)
+                                                  )(dense_output0)
+
+            pre_output = tf.keras.layers.Dense(units=1,
+                                               activation=tf.nn.tanh,
+                                               use_bias=True,
+                                               kernel_initializer='glorot_uniform',
+                                               bias_initializer='zeros',
+                                               kernel_regularizer=tf.keras.regularizers.l2(0.01),
+                                               bias_regularizer=tf.keras.regularizers.l2(0.01)
+                                               )(dense_output1)
+
+            prediction = tf.reshape(pre_output, [-1, self._num_node, 1], name='prediction')
+
+            loss_pre = tf.sqrt(tf.reduce_mean(tf.square(target - prediction)), name='loss')
+
+            train_op = tf.train.AdamOptimizer(self._lr).minimize(loss_pre, name='train_op')
+
+            # record output
+            self._output['prediction'] = prediction.name
+            self._output['loss'] = loss_pre.name
+
+            # record train operation
+            self._op['train_op'] = train_op.name
+
+        super(STMeta, self).build(init_vars, max_to_keep)
+
+    # Define your '_get_feed_dict function‘, map your input to the tf-model
+    def _get_feed_dict(self,
+                       laplace_matrix,
+                       closeness_feature=None,
+                       period_feature=None,
+                       trend_feature=None,
+                       target=None,
+                       external_feature=None):
+        feed_dict = {
+            'laplace_matrix': laplace_matrix,
+        }
+        if target is not None:
+            feed_dict['target'] = target
+        if self._external_dim is not None and self._external_dim > 0:
+            feed_dict['external_feature'] = external_feature
+        if self._closeness_len is not None and self._closeness_len > 0:
+            feed_dict['closeness_feature'] = closeness_feature
+        if self._period_len is not None and self._period_len > 0:
+            feed_dict['period_feature'] = period_feature
+        if self._trend_len is not None and self._trend_len > 0:
+            feed_dict['trend_feature'] = trend_feature
+        return feed_dict
```

### Comparing `UCTB-0.3.0/UCTB/model/ST_MGCN.py` & `UCTB-0.3.5/UCTB/model/ST_MGCN.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,142 +1,142 @@
-import tensorflow as tf
-
-from ..model_unit import BaseModel
-from ..model_unit.GraphModelLayers import GCL
-
-
-class ST_MGCN(BaseModel):
-    """
-
-    References:
-        - `Spatiotemporal multi-graph convolution network for ride-hailing demand forecasting (Geng Xu, et al., 2019)
-          <http://www-scf.usc.edu/~yaguang/papers/aaai19_multi_graph_convolution.pdf>`_.
-        - `A PyTorch implementation of the ST-MGCN model  (shawnwang-tech)
-          <https://github.com/shawnwang-tech/ST-MGCN-pytorch>`_.
-
-    Args:
-        T(int): Input sequence length
-        input_dim(int): Input feature dimension
-        num_graph(int): Number of graphs used in the model.
-        gcl_k(int): The highest order of Chebyshev Polynomial approximation in GCN.
-        gcl_l(int): Number of GCN layers.
-        lstm_units(int): Number of hidden units of RNN.
-        lstm_layers(int): Number of LSTM layers.
-        lr(float): Learning rate
-        external_dim(int): Dimension of the external feature, e.g. temperature and wind are two dimension.
-        code_version(str): Current version of this model code, which will be used as filename for saving the model
-        model_dir(str): The directory to store model files. Default:'model_dir'.
-        gpu_device(str): To specify the GPU to use. Default: '0'.
-    """
-    def __init__(self,
-                 T,
-                 input_dim,
-                 num_graph,
-                 gcl_k,
-                 gcl_l,
-                 lstm_units,
-                 lstm_layers,
-                 lr,
-                 external_dim,
-                 code_version,
-                 model_dir,
-                 gpu_device):
-
-        super(ST_MGCN, self).__init__(code_version=code_version,
-                                      model_dir=model_dir,
-                                      gpu_device=gpu_device)
-
-        self._T = T
-        self._input_dim = input_dim
-        self._num_graph = num_graph
-        self._gcl_k = gcl_k
-        self._gcl_l = gcl_l
-        self._lstm_units = lstm_units
-        self._lstm_layers = lstm_layers
-        self._lr = lr
-        self._external_dim = external_dim
-
-    def build(self, init_vars=True, max_to_keep=5):
-        with self._graph.as_default():
-            # [batch, T, num_stations, input_dim]
-            traffic_flow = tf.placeholder(tf.float32, [None, self._T, None, self._input_dim])
-            laplacian_matrix = tf.placeholder(tf.float32, [self._num_graph, None, None])
-            target = tf.placeholder(tf.float32, [None, None, 1])
-
-            self._input['traffic_flow'] = traffic_flow.name
-            self._input['laplace_matrix'] = laplacian_matrix.name
-            self._input['target'] = target.name
-
-            station_number = tf.shape(traffic_flow)[-2]
-
-            outputs = []
-
-            for graph_index in range(self._num_graph):
-                with tf.variable_scope('CGRNN_Graph%s' % graph_index, reuse=False):
-                    f_k_g = GCL.add_multi_gc_layers(tf.reshape(traffic_flow, [-1, station_number, self._input_dim]),
-                                                    gcn_k=1, gcn_l=1, output_size=self._input_dim,
-                                                    laplacian_matrix=laplacian_matrix[graph_index],
-                                                    activation=tf.nn.tanh)
-
-                    f_k_g = tf.reshape(f_k_g, [-1, self._T, station_number, self._input_dim])
-
-                    x_hat = tf.concat([f_k_g, traffic_flow], axis=-1)
-
-                    z = tf.reduce_mean(x_hat, axis=-2, keepdims=True)
-
-                    s = tf.layers.dense(tf.layers.dense(z, units=4, use_bias=False, activation=tf.nn.relu),
-                                        units=1, use_bias=False, activation=tf.nn.sigmoid)
-
-                    x_rnn = tf.multiply(traffic_flow, tf.tile(s, [1, 1, station_number, self._input_dim]))
-
-                    x_rnn = tf.reshape(tf.transpose(x_rnn, perm=[0, 2, 1, 3]), [-1, self._T, self._input_dim])
-
-                    for lstm_layer_index in range(self._lstm_layers):
-                        x_rnn = tf.keras.layers.LSTM(units=self._lstm_units,
-                                                     activation='tanh',
-                                                     dropout=0.1,
-                                                     kernel_regularizer=tf.contrib.layers.l2_regularizer(1e-4),
-                                                     return_sequences=True if lstm_layer_index<self._lstm_layers-1
-                                                                      else False)\
-                                                    (x_rnn)
-
-                    H = tf.reshape(x_rnn, [-1, station_number, self._lstm_units])
-
-                    outputs.append(H)
-
-            outputs = tf.reduce_sum(outputs, axis=0)
-
-            # external dims
-            if self._external_dim is not None and self._external_dim > 0:
-                external_input = tf.placeholder(tf.float32, [None, self._external_dim])
-                self._input['external_feature'] = external_input.name
-                external_dense = tf.layers.dense(inputs=external_input, units=10)
-                external_dense = tf.tile(tf.reshape(external_dense, [-1, 1, 10]),
-                                         [1, tf.shape(outputs)[-2], 1])
-                outputs = tf.concat([outputs, external_dense], axis=-1)
-
-            prediction = tf.layers.dense(outputs, units=1)
-
-            loss = tf.sqrt(tf.reduce_mean(tf.square(prediction - target)))
-
-            train_operation = tf.train.AdamOptimizer(self._lr).minimize(loss, name='train_op')
-
-            # record output
-            self._output['prediction'] = prediction.name
-            self._output['loss'] = loss.name
-
-            # record train operation
-            self._op['train_op'] = train_operation.name
-
-            super(ST_MGCN, self).build(init_vars=init_vars, max_to_keep=max_to_keep)
-
-    # Step 1 : Define your '_get_feed_dict function‘, map your input to the tf-model
-    def _get_feed_dict(self, traffic_flow, laplace_matrix, target=None, external_feature=None):
-        feed_dict = {
-            'traffic_flow': traffic_flow,
-            'laplace_matrix': laplace_matrix,
-        }
-        if target is not None:
-            feed_dict['target'] = target
-        if external_feature is not None:
-            feed_dict['external_feature'] = external_feature
-        return feed_dict
+import tensorflow as tf
+
+from ..model_unit import BaseModel
+from ..model_unit.GraphModelLayers import GCL
+
+
+class ST_MGCN(BaseModel):
+    """
+
+    References:
+        - `Spatiotemporal multi-graph convolution network for ride-hailing demand forecasting (Geng Xu, et al., 2019)
+          <http://www-scf.usc.edu/~yaguang/papers/aaai19_multi_graph_convolution.pdf>`_.
+        - `A PyTorch implementation of the ST-MGCN model  (shawnwang-tech)
+          <https://github.com/shawnwang-tech/ST-MGCN-pytorch>`_.
+
+    Args:
+        T(int): Input sequence length
+        input_dim(int): Input feature dimension
+        num_graph(int): Number of graphs used in the model.
+        gcl_k(int): The highest order of Chebyshev Polynomial approximation in GCN.
+        gcl_l(int): Number of GCN layers.
+        lstm_units(int): Number of hidden units of RNN.
+        lstm_layers(int): Number of LSTM layers.
+        lr(float): Learning rate
+        external_dim(int): Dimension of the external feature, e.g. temperature and wind are two dimension.
+        code_version(str): Current version of this model code, which will be used as filename for saving the model
+        model_dir(str): The directory to store model files. Default:'model_dir'.
+        gpu_device(str): To specify the GPU to use. Default: '0'.
+    """
+    def __init__(self,
+                 T,
+                 input_dim,
+                 num_graph,
+                 gcl_k,
+                 gcl_l,
+                 lstm_units,
+                 lstm_layers,
+                 lr,
+                 external_dim,
+                 code_version,
+                 model_dir,
+                 gpu_device):
+
+        super(ST_MGCN, self).__init__(code_version=code_version,
+                                      model_dir=model_dir,
+                                      gpu_device=gpu_device)
+
+        self._T = T
+        self._input_dim = input_dim
+        self._num_graph = num_graph
+        self._gcl_k = gcl_k
+        self._gcl_l = gcl_l
+        self._lstm_units = lstm_units
+        self._lstm_layers = lstm_layers
+        self._lr = lr
+        self._external_dim = external_dim
+
+    def build(self, init_vars=True, max_to_keep=5):
+        with self._graph.as_default():
+            # [batch, T, num_stations, input_dim]
+            traffic_flow = tf.placeholder(tf.float32, [None, self._T, None, self._input_dim])
+            laplacian_matrix = tf.placeholder(tf.float32, [self._num_graph, None, None])
+            target = tf.placeholder(tf.float32, [None, None, 1])
+
+            self._input['traffic_flow'] = traffic_flow.name
+            self._input['laplace_matrix'] = laplacian_matrix.name
+            self._input['target'] = target.name
+
+            station_number = tf.shape(traffic_flow)[-2]
+
+            outputs = []
+
+            for graph_index in range(self._num_graph):
+                with tf.variable_scope('CGRNN_Graph%s' % graph_index, reuse=False):
+                    f_k_g = GCL.add_multi_gc_layers(tf.reshape(traffic_flow, [-1, station_number, self._input_dim]),
+                                                    gcn_k=1, gcn_l=1, output_size=self._input_dim,
+                                                    laplacian_matrix=laplacian_matrix[graph_index],
+                                                    activation=tf.nn.tanh)
+
+                    f_k_g = tf.reshape(f_k_g, [-1, self._T, station_number, self._input_dim])
+
+                    x_hat = tf.concat([f_k_g, traffic_flow], axis=-1)
+
+                    z = tf.reduce_mean(x_hat, axis=-2, keepdims=True)
+
+                    s = tf.layers.dense(tf.layers.dense(z, units=4, use_bias=False, activation=tf.nn.relu),
+                                        units=1, use_bias=False, activation=tf.nn.sigmoid)
+
+                    x_rnn = tf.multiply(traffic_flow, tf.tile(s, [1, 1, station_number, self._input_dim]))
+
+                    x_rnn = tf.reshape(tf.transpose(x_rnn, perm=[0, 2, 1, 3]), [-1, self._T, self._input_dim])
+
+                    for lstm_layer_index in range(self._lstm_layers):
+                        x_rnn = tf.keras.layers.LSTM(units=self._lstm_units,
+                                                     activation='tanh',
+                                                     dropout=0.1,
+                                                     kernel_regularizer=tf.contrib.layers.l2_regularizer(1e-4),
+                                                     return_sequences=True if lstm_layer_index<self._lstm_layers-1
+                                                                      else False)\
+                                                    (x_rnn)
+
+                    H = tf.reshape(x_rnn, [-1, station_number, self._lstm_units])
+
+                    outputs.append(H)
+
+            outputs = tf.reduce_sum(outputs, axis=0)
+
+            # external dims
+            if self._external_dim is not None and self._external_dim > 0:
+                external_input = tf.placeholder(tf.float32, [None, self._external_dim])
+                self._input['external_feature'] = external_input.name
+                external_dense = tf.layers.dense(inputs=external_input, units=10)
+                external_dense = tf.tile(tf.reshape(external_dense, [-1, 1, 10]),
+                                         [1, tf.shape(outputs)[-2], 1])
+                outputs = tf.concat([outputs, external_dense], axis=-1)
+
+            prediction = tf.layers.dense(outputs, units=1)
+
+            loss = tf.sqrt(tf.reduce_mean(tf.square(prediction - target)))
+
+            train_operation = tf.train.AdamOptimizer(self._lr).minimize(loss, name='train_op')
+
+            # record output
+            self._output['prediction'] = prediction.name
+            self._output['loss'] = loss.name
+
+            # record train operation
+            self._op['train_op'] = train_operation.name
+
+            super(ST_MGCN, self).build(init_vars=init_vars, max_to_keep=max_to_keep)
+
+    # Step 1 : Define your '_get_feed_dict function‘, map your input to the tf-model
+    def _get_feed_dict(self, traffic_flow, laplace_matrix, target=None, external_feature=None):
+        feed_dict = {
+            'traffic_flow': traffic_flow,
+            'laplace_matrix': laplace_matrix,
+        }
+        if target is not None:
+            feed_dict['target'] = target
+        if external_feature is not None:
+            feed_dict['external_feature'] = external_feature
+        return feed_dict
```

### Comparing `UCTB-0.3.0/UCTB/model/ST_ResNet.py` & `UCTB-0.3.5/UCTB/model/ST_ResNet.py`

 * *Files identical despite different names*

### Comparing `UCTB-0.3.0/UCTB/model/XGBoost.py` & `UCTB-0.3.5/UCTB/model/XGBoost.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-import xgboost as xgb
-import numpy as np
-
-
-class XGBoost():
-    """
-    XGBoost is an optimized distributed gradient boosting machine learning algorithm.
-
-    Args:
-        *n_estimators (int): Number of boosting iterations. Default: 10
-        *max_depth (int): Maximum tree depth for base learners. Default: 5
-        *verbosity (int): The degree of verbosity. Valid values are 0 (silent) - 3 (debug). Default: 0
-        *objective (string or callable):
-            Specify the learning task and the corresponding learning objective or
-            a custom objective function to be used. Default: ``'reg:squarederror'``
-        *eval_metric (str, list of str, or callable, optional):
-            If a str, should be a built-in evaluation metric to use. See more in
-            `API Reference of XGBoost Library <https://xgboost.readthedocs.io/en/latest/python/python_api.html>`_.
-            Default: ``'rmse'``
-    """
-    def __init__(self, n_estimators=10, max_depth=5, verbosity=0, objective='reg:squarederror', eval_metric='rmse'):
-        
-        self.param = {
-            'max_depth': max_depth,
-            'verbosity ': verbosity,
-            'objective': objective,
-            'eval_metric': eval_metric
-        }
-        self.n_estimators = n_estimators
-
-    def fit(self, X, y):
-        '''
-        Training method. 
-
-        Args:
-            X(np.ndarray/scipy.sparse/pd.DataFrame/dt.Frame): The training input samples.
-            y(np.ndarray, optional): The target values of training samples.
-        '''
-        train_matrix = xgb.DMatrix(X, label=y)
-        self.model = xgb.train(self.param, train_matrix, self.n_estimators)
-
-    def predict(self, X):
-        '''
-        Prediction method.
-        
-        :Returns: Predicted values with shape as [time_slot_num, node_num, 1].
-        :Return type: np.ndarray
-        '''
-        test_matrix = xgb.DMatrix(X)
-        return self.model.predict(test_matrix)
-
-
+import xgboost as xgb
+import numpy as np
+
+
+class XGBoost():
+    """
+    XGBoost is an optimized distributed gradient boosting machine learning algorithm.
+
+    Args:
+        *n_estimators (int): Number of boosting iterations. Default: 10
+        *max_depth (int): Maximum tree depth for base learners. Default: 5
+        *verbosity (int): The degree of verbosity. Valid values are 0 (silent) - 3 (debug). Default: 0
+        *objective (string or callable):
+            Specify the learning task and the corresponding learning objective or
+            a custom objective function to be used. Default: ``'reg:squarederror'``
+        *eval_metric (str, list of str, or callable, optional):
+            If a str, should be a built-in evaluation metric to use. See more in
+            `API Reference of XGBoost Library <https://xgboost.readthedocs.io/en/latest/python/python_api.html>`_.
+            Default: ``'rmse'``
+    """
+    def __init__(self, n_estimators=10, max_depth=5, verbosity=0, objective='reg:squarederror', eval_metric='rmse'):
+        
+        self.param = {
+            'max_depth': max_depth,
+            'verbosity': verbosity,
+            'objective': objective,
+            'eval_metric': eval_metric
+        }
+        self.n_estimators = n_estimators
+
+    def fit(self, X, y):
+        '''
+        Training method. 
+
+        Args:
+            X(np.ndarray/scipy.sparse/pd.DataFrame/dt.Frame): The training input samples.
+            y(np.ndarray, optional): The target values of training samples.
+        '''
+        train_matrix = xgb.DMatrix(X, label=y)
+        self.model = xgb.train(self.param, train_matrix, self.n_estimators)
+
+    def predict(self, X):
+        '''
+        Prediction method.
+        
+        :Returns: Predicted values with shape as [time_slot_num, node_num, 1].
+        :Return type: np.ndarray
+        '''
+        test_matrix = xgb.DMatrix(X)
+        return self.model.predict(test_matrix)
+
+
```

### Comparing `UCTB-0.3.0/UCTB/model_unit/BaseModel.py` & `UCTB-0.3.5/UCTB/model_unit/BaseModel.py`

 * *Files identical despite different names*

### Comparing `UCTB-0.3.0/UCTB/model_unit/DCRNN_CELL.py` & `UCTB-0.3.5/UCTB/model_unit/DCRNN_CELL.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,166 +1,166 @@
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import print_function
-
-import numpy as np
-import tensorflow as tf
-
-from tensorflow.contrib.rnn import RNNCell
-
-
-class DCGRUCell(RNNCell):
-    """Graph Convolution Gated Recurrent Unit cell.
-    """
-
-    def call(self, inputs, **kwargs):
-        pass
-
-    def compute_output_shape(self, input_shape):
-        pass
-
-    def __init__(self, num_units, input_dim, num_graphs, supports, max_diffusion_step, num_nodes, num_proj=None,
-                 activation=tf.nn.tanh, reuse=None, use_gc_for_ru=True, name=None):
-        """
-
-        :param num_units:
-        :param adj_mx:
-        :param max_diffusion_step:
-        :param num_nodes:
-        :param input_size:
-        :param num_proj:
-        :param activation:
-        :param reuse:
-        :param filter_type: "laplacian", "random_walk", "dual_random_walk".
-        :param use_gc_for_ru: whether to use Graph convolution to calculate the reset and update gates.
-        """
-        super(DCGRUCell, self).__init__(_reuse=reuse)
-        self._activation = activation
-        self._num_nodes = num_nodes
-        self._input_dim = input_dim
-        self._num_graphs = num_graphs
-        self._num_proj = num_proj
-        self._num_units = num_units
-        self._max_diffusion_step = max_diffusion_step
-        self._use_gc_for_ru = use_gc_for_ru
-        self._supports = supports
-        self._num_diff_matrix = supports.get_shape()[0].value
-        self._name = name
-
-    @property
-    def state_size(self):
-        return self._num_nodes * self._num_units
-
-    @property
-    def output_size(self):
-        output_size = self._num_nodes * self._num_units
-        if self._num_proj is not None:
-            output_size = self._num_nodes * self._num_proj
-        return output_size
-
-    def __call__(self, inputs, state, scope=None):
-        """Gated recurrent unit (GRU) with Graph Convolution.
-        :param inputs: (B, num_nodes * input_dim)
-
-        :return
-        - Output: A `2-D` tensor with shape `[batch_size x self.output_size]`.
-        - New state: Either a single `2-D` tensor, or a tuple of tensors matching
-            the arity and shapes of `state`
-        """
-        with tf.variable_scope(scope or "dcgru_cell"):
-            with tf.variable_scope("gates"):  # Reset gate and update gate.
-                output_size = 2 * self._num_units
-                # We start with bias of 1.0 to not reset and not update.
-                if self._use_gc_for_ru:
-                    fn = self._gconv
-                else:
-                    fn = self._fc
-                value = tf.nn.sigmoid(fn(inputs, state, output_size, bias_start=1.0))
-                value = tf.reshape(value, (-1, self._num_nodes, output_size))
-                r, u = tf.split(value=value, num_or_size_splits=2, axis=-1)
-                r = tf.reshape(r, (-1, self._num_nodes * self._num_units))
-                u = tf.reshape(u, (-1, self._num_nodes * self._num_units))
-            with tf.variable_scope("candidate"):
-                c = self._gconv(inputs, r * state, self._num_units)
-                if self._activation is not None:
-                    c = self._activation(c)
-            output = new_state = u * state + (1 - u) * c
-            if self._num_proj is not None:
-                with tf.variable_scope("projection"):
-                    w = tf.get_variable('w', shape=(self._num_units, self._num_proj))
-                    output = tf.reshape(new_state, shape=(-1, self._num_units))
-                    output = tf.reshape(tf.matmul(output, w), shape=(-1, self.output_size))
-        return output, new_state
-
-    @staticmethod
-    def _concat(x, x_):
-        x_ = tf.expand_dims(x_, 0)
-        return tf.concat([x, x_], axis=0)
-
-    def _fc(self, inputs, state, output_size, bias_start=0.0):
-        dtype = inputs.dtype
-        batch_size = inputs.get_shape()[0].value
-        inputs = tf.reshape(inputs, (batch_size * self._num_nodes, -1))
-        state = tf.reshape(state, (batch_size * self._num_nodes, -1))
-        inputs_and_state = tf.concat([inputs, state], axis=-1)
-        input_size = inputs_and_state.get_shape()[-1].value
-        weights = tf.get_variable(
-            'weights', [input_size, output_size], dtype=dtype,
-            initializer=tf.contrib.layers.xavier_initializer())
-        value = tf.nn.sigmoid(tf.matmul(inputs_and_state, weights))
-        biases = tf.get_variable("biases", [output_size], dtype=dtype,
-                                 initializer=tf.constant_initializer(bias_start, dtype=dtype))
-        value = tf.nn.bias_add(value, biases)
-        return value
-
-    def _gconv(self, inputs, state, output_size, bias_start=0.0):
-        """Graph convolution between input and the graph matrix.
-
-        :param args: a 2D Tensor or a list of 2D, batch x n, Tensors.
-        :param output_size:
-        :param bias:
-        :param bias_start:
-        :param scope:
-        :return:
-        """
-        # Reshape input and state to (batch_size, num_nodes, input_dim/state_dim)
-        last_dim = inputs.get_shape()[-1].value
-        inputs = tf.reshape(inputs, (-1, self._num_nodes, int(last_dim / self._num_nodes)))
-        state = tf.reshape(state, (-1, self._num_nodes, self._num_units))
-        inputs_and_state = tf.concat([inputs, state], axis=2)
-        input_size = inputs_and_state.get_shape()[2].value
-        dtype = inputs.dtype
-
-        x = inputs_and_state
-        x0 = tf.transpose(x, perm=[1, 2, 0])  # (num_nodes, total_arg_size, batch_size)
-        x0 = tf.reshape(x0, shape=[self._num_nodes, -1])
-        x = tf.expand_dims(x0, axis=0)
-
-        scope = tf.get_variable_scope()
-        with tf.variable_scope(scope.name + (self.name or ''), reuse=False):
-            if self._max_diffusion_step == 0:
-                pass
-            else:
-                for index in range(self._num_diff_matrix):
-                    x1 = tf.matmul(self._supports[index], x0)
-                    x = self._concat(x, x1)
-
-                    for k in range(2, self._max_diffusion_step + 1):
-                        x2 = 2 * tf.matmul(self._supports[index], x1) - x0
-                        x = self._concat(x, x2)
-                        x1, x0 = x2, x1
-
-            num_matrices = self._num_diff_matrix * self._max_diffusion_step + 1  # Adds for x itself.
-            x = tf.reshape(x, shape=[num_matrices, self._num_nodes, input_size, -1])
-            x = tf.transpose(x, perm=[3, 1, 2, 0])  # (batch_size, num_nodes, input_size, order)
-            x = tf.reshape(x, shape=[-1, input_size * num_matrices])
-
-            weights = tf.get_variable(
-                'weights', [input_size * num_matrices, output_size], dtype=dtype,
-                initializer=tf.contrib.layers.xavier_initializer())
-            x = tf.matmul(x, weights)  # (batch_size * self._num_nodes, output_size)
-
-            biases = tf.get_variable("biases", [output_size], dtype=dtype,
-                                     initializer=tf.constant_initializer(bias_start, dtype=dtype))
-            x = tf.nn.bias_add(x, biases)
-        # Reshape res back to 2D: (batch_size, num_node, state_dim) -> (batch_size, num_node * state_dim)
-        return tf.reshape(x, [-1, self._num_nodes * output_size])
+from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
+
+import numpy as np
+import tensorflow as tf
+
+from tensorflow.contrib.rnn import RNNCell
+
+
+class DCGRUCell(RNNCell):
+    """Graph Convolution Gated Recurrent Unit cell.
+    """
+
+    def call(self, inputs, **kwargs):
+        pass
+
+    def compute_output_shape(self, input_shape):
+        pass
+
+    def __init__(self, num_units, input_dim, num_graphs, supports, max_diffusion_step, num_node, num_proj=None,
+                 activation=tf.nn.tanh, reuse=None, use_gc_for_ru=True, name=None):
+        """
+
+        :param num_units:
+        :param adj_mx:
+        :param max_diffusion_step:
+        :param num_node:
+        :param input_size:
+        :param num_proj:
+        :param activation:
+        :param reuse:
+        :param filter_type: "laplacian", "random_walk", "dual_random_walk".
+        :param use_gc_for_ru: whether to use Graph convolution to calculate the reset and update gates.
+        """
+        super(DCGRUCell, self).__init__(_reuse=reuse)
+        self._activation = activation
+        self._num_node = num_node
+        self._input_dim = input_dim
+        self._num_graphs = num_graphs
+        self._num_proj = num_proj
+        self._num_units = num_units
+        self._max_diffusion_step = max_diffusion_step
+        self._use_gc_for_ru = use_gc_for_ru
+        self._supports = supports
+        self._num_diff_matrix = supports.get_shape()[0].value
+        self._name = name
+
+    @property
+    def state_size(self):
+        return self._num_node * self._num_units
+
+    @property
+    def output_size(self):
+        output_size = self._num_node * self._num_units
+        if self._num_proj is not None:
+            output_size = self._num_node * self._num_proj
+        return output_size
+
+    def __call__(self, inputs, state, scope=None):
+        """Gated recurrent unit (GRU) with Graph Convolution.
+        :param inputs: (B, num_node * input_dim)
+
+        :return
+        - Output: A `2-D` tensor with shape `[batch_size x self.output_size]`.
+        - New state: Either a single `2-D` tensor, or a tuple of tensors matching
+            the arity and shapes of `state`
+        """
+        with tf.variable_scope(scope or "dcgru_cell"):
+            with tf.variable_scope("gates"):  # Reset gate and update gate.
+                output_size = 2 * self._num_units
+                # We start with bias of 1.0 to not reset and not update.
+                if self._use_gc_for_ru:
+                    fn = self._gconv
+                else:
+                    fn = self._fc
+                value = tf.nn.sigmoid(fn(inputs, state, output_size, bias_start=1.0))
+                value = tf.reshape(value, (-1, self._num_node, output_size))
+                r, u = tf.split(value=value, num_or_size_splits=2, axis=-1)
+                r = tf.reshape(r, (-1, self._num_node * self._num_units))
+                u = tf.reshape(u, (-1, self._num_node * self._num_units))
+            with tf.variable_scope("candidate"):
+                c = self._gconv(inputs, r * state, self._num_units)
+                if self._activation is not None:
+                    c = self._activation(c)
+            output = new_state = u * state + (1 - u) * c
+            if self._num_proj is not None:
+                with tf.variable_scope("projection"):
+                    w = tf.get_variable('w', shape=(self._num_units, self._num_proj))
+                    output = tf.reshape(new_state, shape=(-1, self._num_units))
+                    output = tf.reshape(tf.matmul(output, w), shape=(-1, self.output_size))
+        return output, new_state
+
+    @staticmethod
+    def _concat(x, x_):
+        x_ = tf.expand_dims(x_, 0)
+        return tf.concat([x, x_], axis=0)
+
+    def _fc(self, inputs, state, output_size, bias_start=0.0):
+        dtype = inputs.dtype
+        batch_size = inputs.get_shape()[0].value
+        inputs = tf.reshape(inputs, (batch_size * self._num_node, -1))
+        state = tf.reshape(state, (batch_size * self._num_node, -1))
+        inputs_and_state = tf.concat([inputs, state], axis=-1)
+        input_size = inputs_and_state.get_shape()[-1].value
+        weights = tf.get_variable(
+            'weights', [input_size, output_size], dtype=dtype,
+            initializer=tf.contrib.layers.xavier_initializer())
+        value = tf.nn.sigmoid(tf.matmul(inputs_and_state, weights))
+        biases = tf.get_variable("biases", [output_size], dtype=dtype,
+                                 initializer=tf.constant_initializer(bias_start, dtype=dtype))
+        value = tf.nn.bias_add(value, biases)
+        return value
+
+    def _gconv(self, inputs, state, output_size, bias_start=0.0):
+        """Graph convolution between input and the graph matrix.
+
+        :param args: a 2D Tensor or a list of 2D, batch x n, Tensors.
+        :param output_size:
+        :param bias:
+        :param bias_start:
+        :param scope:
+        :return:
+        """
+        # Reshape input and state to (batch_size, num_node, input_dim/state_dim)
+        last_dim = inputs.get_shape()[-1].value
+        inputs = tf.reshape(inputs, (-1, self._num_node, int(last_dim / self._num_node)))
+        state = tf.reshape(state, (-1, self._num_node, self._num_units))
+        inputs_and_state = tf.concat([inputs, state], axis=2)
+        input_size = inputs_and_state.get_shape()[2].value
+        dtype = inputs.dtype
+
+        x = inputs_and_state
+        x0 = tf.transpose(x, perm=[1, 2, 0])  # (num_node, total_arg_size, batch_size)
+        x0 = tf.reshape(x0, shape=[self._num_node, -1])
+        x = tf.expand_dims(x0, axis=0)
+
+        scope = tf.get_variable_scope()
+        with tf.variable_scope(scope.name + (self.name or ''), reuse=False):
+            if self._max_diffusion_step == 0:
+                pass
+            else:
+                for index in range(self._num_diff_matrix):
+                    x1 = tf.matmul(self._supports[index], x0)
+                    x = self._concat(x, x1)
+
+                    for k in range(2, self._max_diffusion_step + 1):
+                        x2 = 2 * tf.matmul(self._supports[index], x1) - x0
+                        x = self._concat(x, x2)
+                        x1, x0 = x2, x1
+
+            num_matrices = self._num_diff_matrix * self._max_diffusion_step + 1  # Adds for x itself.
+            x = tf.reshape(x, shape=[num_matrices, self._num_node, input_size, -1])
+            x = tf.transpose(x, perm=[3, 1, 2, 0])  # (batch_size, num_node, input_size, order)
+            x = tf.reshape(x, shape=[-1, input_size * num_matrices])
+
+            weights = tf.get_variable(
+                'weights', [input_size * num_matrices, output_size], dtype=dtype,
+                initializer=tf.contrib.layers.xavier_initializer())
+            x = tf.matmul(x, weights)  # (batch_size * self._num_node, output_size)
+
+            biases = tf.get_variable("biases", [output_size], dtype=dtype,
+                                     initializer=tf.constant_initializer(bias_start, dtype=dtype))
+            x = tf.nn.bias_add(x, biases)
+        # Reshape res back to 2D: (batch_size, num_node, state_dim) -> (batch_size, num_node * state_dim)
+        return tf.reshape(x, [-1, self._num_node * output_size])
```

### Comparing `UCTB-0.3.0/UCTB/model_unit/GraphModelLayers.py` & `UCTB-0.3.5/UCTB/model_unit/GraphModelLayers.py`

 * *Files identical despite different names*

### Comparing `UCTB-0.3.0/UCTB/model_unit/ST_RNN.py` & `UCTB-0.3.5/UCTB/model_unit/ST_RNN.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,139 +1,139 @@
-import tensorflow as tf
-
-from tensorflow.python.framework import dtypes
-from tensorflow.python.keras import backend as K
-from tensorflow.python.keras.utils import tf_utils
-from tensorflow.python.ops import array_ops, linalg_ops, math_ops
-
-
-def _generate_dropout_mask(ones, rate, training=None, count=1):
-    def dropped_inputs():
-        return K.dropout(ones, rate)
-
-    if count > 1:
-        return [
-            K.in_train_phase(dropped_inputs, ones, training=training)
-            for _ in range(count)
-        ]
-    return K.in_train_phase(dropped_inputs, ones, training=training)
-
-
-class GCLSTMCell(tf.keras.layers.LSTMCell):
-
-    """
-    GCLSTMCell is one of our implemented ST-RNN models in handling the spatial and temporal features.
-    We performed GCN on both LSTM inputs and hidden-states. The code is inherited from tf.keras.layers.LSTMCell,
-    thus it can be used almost the same as LSTMCell except that you need to provide the GCN parameters
-    in the __init__ function.
-
-    Args:
-        units(int): number of units of LSTM
-        num_nodes(int): number of nodes in the graph
-        laplacian_matrix(ndarray): laplacian matrix used in GCN, with shape [num_node, num_node]
-        gcn_k(int): highest order of Chebyshev Polynomial approximation in GCN
-        gcn_l(int): number of GCN layers
-        kwargs: other parameters supported by LSTMCell, such as activation, kernel_initializer ... and so on.
-    """
-
-    def __init__(self, units, num_nodes, laplacian_matrix, gcn_k=1, gcn_l=1, **kwargs):
-
-        super().__init__(units, **kwargs)
-
-        self._units = units
-        self._num_node = num_nodes
-        self._gcn_k = gcn_k
-        self._gcn_l = gcn_l
-        self._laplacian_matrix = laplacian_matrix
-
-    @tf_utils.shape_type_conversion
-    def build(self, input_shape):
-        super(GCLSTMCell, self).build(input_shape)
-        input_dim = input_shape[-1]
-        self.kernel = self.add_weight(
-            shape=(input_dim * (self._gcn_k + 1), self.units * 4),
-            name='kernel',
-            initializer=self.kernel_initializer,
-            regularizer=self.kernel_regularizer,
-            constraint=self.kernel_constraint)
-        self.recurrent_kernel = self.add_weight(
-            shape=(self.units * (self._gcn_k + 1), self.units * 4),
-            name='recurrent_kernel',
-            initializer=self.recurrent_initializer,
-            regularizer=self.recurrent_regularizer,
-            constraint=self.recurrent_constraint)
-
-    def kth_cheby_ploy(self, k, tk1=None, tk2=None):
-        if k == 0:
-            return linalg_ops.eye(self._num_node, dtype=dtypes.float32)
-        elif k == 1:
-            return self._laplacian_matrix
-        elif k > 1:
-            return math_ops.matmul(2 * self._laplacian_matrix, tk1) - tk2
-
-    def call(self, inputs, states, training=None):
-
-        if 0 < self.dropout < 1 and self._dropout_mask is None:
-            self._dropout_mask = _generate_dropout_mask(
-                array_ops.ones_like(inputs),
-                self.dropout,
-                training=training,
-                count=4)
-        if (0 < self.recurrent_dropout < 1 and
-                self._recurrent_dropout_mask is None):
-            self._recurrent_dropout_mask = _generate_dropout_mask(
-                array_ops.ones_like(states[0]),
-                self.recurrent_dropout,
-                training=training,
-                count=4)
-
-        input_dim = inputs.get_shape()[-1].value
-
-        # dropout matrices for input units
-        dp_mask = self._dropout_mask
-        # dropout matrices for recurrent units
-        rec_dp_mask = self._recurrent_dropout_mask
-
-        h_tm1 = states[0]  # previous memory state
-        c_tm1 = states[1]  # previous carry state
-
-        if 0. < self.dropout < 1.:
-            inputs *= dp_mask[0]
-        if 0. < self.recurrent_dropout < 1.:
-            h_tm1 *= rec_dp_mask[0]
-
-        # inputs has shape: [batch * num_nodes, input_dim]
-        # h_tm1 has shape: [batch * num_nodes, units]
-        inputs_before_gcn = tf.reshape(tf.transpose(tf.reshape(inputs, [-1, self._num_node, input_dim]),
-                                                    [1, 0, 2]), [self._num_node, -1])
-        h_tm1_before_gcn = tf.reshape(tf.transpose(tf.reshape(h_tm1, [-1, self._num_node, self._units]),
-                                                   [1, 0, 2]), [self._num_node, -1])
-
-        t = []
-        inputs_after_gcn = list()
-        h_tm1_after_gcn = list()
-        for i in range(0, self._gcn_k + 1):
-            t.append(self.kth_cheby_ploy(k=i, tk1=None if i < 1 else t[i - 1], tk2=None if i < 2 else t[i - 2]))
-            inputs_after_gcn.append(tf.matmul(t[-1], inputs_before_gcn))
-            h_tm1_after_gcn.append(tf.matmul(t[-1], h_tm1_before_gcn))
-
-        inputs_after_gcn = tf.reshape(inputs_after_gcn, [self._gcn_k + 1, self._num_node, -1, input_dim])
-        h_tm1_after_gcn = tf.reshape(h_tm1_after_gcn, [self._gcn_k + 1, self._num_node, -1, self._units])
-
-        inputs_after_gcn = tf.reshape(tf.transpose(inputs_after_gcn, [2, 1, 0, 3]), [-1, (self._gcn_k + 1) * input_dim])
-        h_tm1_after_gcn = tf.reshape(tf.transpose(h_tm1_after_gcn, [2, 1, 0, 3]), [-1, (self._gcn_k + 1) * self.units])
-
-        z = K.dot(inputs_after_gcn, self.kernel)
-        z += K.dot(h_tm1_after_gcn, self.recurrent_kernel)
-        if self.use_bias:
-            z = K.bias_add(z, self.bias)
-
-        z0 = z[:, :self.units]
-        z1 = z[:, self.units:2 * self.units]
-        z2 = z[:, 2 * self.units:3 * self.units]
-        z3 = z[:, 3 * self.units:]
-
-        z = (z0, z1, z2, z3)
-        c, o = self._compute_carry_and_output_fused(z, c_tm1)
-
-        h = o * self.activation(c)
-        return h, [h, c]
+import tensorflow as tf
+
+from tensorflow.python.framework import dtypes
+from tensorflow.python.keras import backend as K
+from tensorflow.python.keras.utils import tf_utils
+from tensorflow.python.ops import array_ops, linalg_ops, math_ops
+
+
+def _generate_dropout_mask(ones, rate, training=None, count=1):
+    def dropped_inputs():
+        return K.dropout(ones, rate)
+
+    if count > 1:
+        return [
+            K.in_train_phase(dropped_inputs, ones, training=training)
+            for _ in range(count)
+        ]
+    return K.in_train_phase(dropped_inputs, ones, training=training)
+
+
+class GCLSTMCell(tf.keras.layers.LSTMCell):
+
+    """
+    GCLSTMCell is one of our implemented ST-RNN models in handling the spatial and temporal features.
+    We performed GCN on both LSTM inputs and hidden-states. The code is inherited from tf.keras.layers.LSTMCell,
+    thus it can be used almost the same as LSTMCell except that you need to provide the GCN parameters
+    in the __init__ function.
+
+    Args:
+        units(int): number of units of LSTM
+        num_node(int): number of nodes in the graph
+        laplacian_matrix(ndarray): laplacian matrix used in GCN, with shape [num_node, num_node]
+        gcn_k(int): highest order of Chebyshev Polynomial approximation in GCN
+        gcn_l(int): number of GCN layers
+        kwargs: other parameters supported by LSTMCell, such as activation, kernel_initializer ... and so on.
+    """
+
+    def __init__(self, units, num_node, laplacian_matrix, gcn_k=1, gcn_l=1, **kwargs):
+
+        super().__init__(units, **kwargs)
+
+        self._units = units
+        self._num_node = num_node
+        self._gcn_k = gcn_k
+        self._gcn_l = gcn_l
+        self._laplacian_matrix = laplacian_matrix
+
+    @tf_utils.shape_type_conversion
+    def build(self, input_shape):
+        super(GCLSTMCell, self).build(input_shape)
+        input_dim = input_shape[-1]
+        self.kernel = self.add_weight(
+            shape=(input_dim * (self._gcn_k + 1), self.units * 4),
+            name='kernel',
+            initializer=self.kernel_initializer,
+            regularizer=self.kernel_regularizer,
+            constraint=self.kernel_constraint)
+        self.recurrent_kernel = self.add_weight(
+            shape=(self.units * (self._gcn_k + 1), self.units * 4),
+            name='recurrent_kernel',
+            initializer=self.recurrent_initializer,
+            regularizer=self.recurrent_regularizer,
+            constraint=self.recurrent_constraint)
+
+    def kth_cheby_ploy(self, k, tk1=None, tk2=None):
+        if k == 0:
+            return linalg_ops.eye(self._num_node, dtype=dtypes.float32)
+        elif k == 1:
+            return self._laplacian_matrix
+        elif k > 1:
+            return math_ops.matmul(2 * self._laplacian_matrix, tk1) - tk2
+
+    def call(self, inputs, states, training=None):
+
+        if 0 < self.dropout < 1 and self._dropout_mask is None:
+            self._dropout_mask = _generate_dropout_mask(
+                array_ops.ones_like(inputs),
+                self.dropout,
+                training=training,
+                count=4)
+        if (0 < self.recurrent_dropout < 1 and
+                self._recurrent_dropout_mask is None):
+            self._recurrent_dropout_mask = _generate_dropout_mask(
+                array_ops.ones_like(states[0]),
+                self.recurrent_dropout,
+                training=training,
+                count=4)
+
+        input_dim = inputs.get_shape()[-1].value
+
+        # dropout matrices for input units
+        dp_mask = self._dropout_mask
+        # dropout matrices for recurrent units
+        rec_dp_mask = self._recurrent_dropout_mask
+
+        h_tm1 = states[0]  # previous memory state
+        c_tm1 = states[1]  # previous carry state
+
+        if 0. < self.dropout < 1.:
+            inputs *= dp_mask[0]
+        if 0. < self.recurrent_dropout < 1.:
+            h_tm1 *= rec_dp_mask[0]
+
+        # inputs has shape: [batch * num_node, input_dim]
+        # h_tm1 has shape: [batch * num_node, units]
+        inputs_before_gcn = tf.reshape(tf.transpose(tf.reshape(inputs, [-1, self._num_node, input_dim]),
+                                                    [1, 0, 2]), [self._num_node, -1])
+        h_tm1_before_gcn = tf.reshape(tf.transpose(tf.reshape(h_tm1, [-1, self._num_node, self._units]),
+                                                   [1, 0, 2]), [self._num_node, -1])
+
+        t = []
+        inputs_after_gcn = list()
+        h_tm1_after_gcn = list()
+        for i in range(0, self._gcn_k + 1):
+            t.append(self.kth_cheby_ploy(k=i, tk1=None if i < 1 else t[i - 1], tk2=None if i < 2 else t[i - 2]))
+            inputs_after_gcn.append(tf.matmul(t[-1], inputs_before_gcn))
+            h_tm1_after_gcn.append(tf.matmul(t[-1], h_tm1_before_gcn))
+
+        inputs_after_gcn = tf.reshape(inputs_after_gcn, [self._gcn_k + 1, self._num_node, -1, input_dim])
+        h_tm1_after_gcn = tf.reshape(h_tm1_after_gcn, [self._gcn_k + 1, self._num_node, -1, self._units])
+
+        inputs_after_gcn = tf.reshape(tf.transpose(inputs_after_gcn, [2, 1, 0, 3]), [-1, (self._gcn_k + 1) * input_dim])
+        h_tm1_after_gcn = tf.reshape(tf.transpose(h_tm1_after_gcn, [2, 1, 0, 3]), [-1, (self._gcn_k + 1) * self.units])
+
+        z = K.dot(inputs_after_gcn, self.kernel)
+        z += K.dot(h_tm1_after_gcn, self.recurrent_kernel)
+        if self.use_bias:
+            z = K.bias_add(z, self.bias)
+
+        z0 = z[:, :self.units]
+        z1 = z[:, self.units:2 * self.units]
+        z2 = z[:, 2 * self.units:3 * self.units]
+        z3 = z[:, 3 * self.units:]
+
+        z = (z0, z1, z2, z3)
+        c, o = self._compute_carry_and_output_fused(z, c_tm1)
+
+        h = o * self.activation(c)
+        return h, [h, c]
```

### Comparing `UCTB-0.3.0/UCTB/preprocess/time_utils.py` & `UCTB-0.3.5/UCTB/preprocess/time_utils.py`

 * *Files identical despite different names*

### Comparing `UCTB-0.3.0/UCTB/train/EarlyStopping.py` & `UCTB-0.3.5/UCTB/train/EarlyStopping.py`

 * *Files identical despite different names*

### Comparing `UCTB-0.3.0/UCTB/train/MiniBatchTrain.py` & `UCTB-0.3.5/UCTB/train/MiniBatchTrain.py`

 * *Files identical despite different names*

### Comparing `UCTB-0.3.0/UCTB/utils/make_predict_dataset.py` & `UCTB-0.3.5/UCTB/utils/make_predict_dataset.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-import copy
-import pickle
-import os
-import numpy as np
-
-
-def save_predict_in_dataset(data_loader, predict_val, method):
-    data_dir = os.path.join(os.path.dirname(
-        os.path.dirname(os.path.abspath(__file__))), 'data')
-
-    original_file = os.path.join(data_dir, "{}_{}.pkl".format(
-        data_loader.dataset.dataset, data_loader.dataset.city))
-    file_name = os.path.join(data_dir, "{}_{}_pred.pkl".format(
-        data_loader.dataset.dataset, data_loader.dataset.city))
-
-    if os.path.exists(file_name):
-        with open(file_name, "rb") as fp:
-            pred_data = pickle.load(fp)
-    else:
-        with open(original_file, "rb") as fp:
-            pred_data = pickle.load(fp)
-            pred_data['Pred'] = {}
-
-    loader_id = data_loader.loader_id
-    if loader_id not in pred_data["Pred"].keys():
-        pred_data['Pred'][loader_id] = {}
-
-    pred_data['Pred'][loader_id]["GroundTruth"] = np.squeeze(
-        data_loader.test_y)
-
-    if loader_id.endswith("N"):
-        # use NodeTrafficLoader
-        pred_data['Pred'][loader_id][method] = {}
-        pred_data['Pred'][loader_id][method]["traffic_data_index"] = data_loader.traffic_data_index
-        pred_data['Pred'][loader_id][method]["TrafficNode"] = np.squeeze(
-            predict_val)
-
-    if loader_id.endswith("G"):
-        # use GridTrafficLoader
-        pred_data['Pred'][loader_id][method] = {}
-        pred_data['Pred'][loader_id][method]["TrafficGrid"] = np.squeeze(predict_val)
-
-    with open(file_name, "wb") as fp:
-        pickle.dump(pred_data, fp)
+import copy
+import pickle
+import os
+import numpy as np
+
+
+def save_predict_in_dataset(data_loader, predict_val, method):
+    data_dir = os.path.join(os.path.dirname(
+        os.path.dirname(os.path.abspath(__file__))), 'data')
+
+    original_file = os.path.join(data_dir, "{}_{}.pkl".format(
+        data_loader.dataset.dataset, data_loader.dataset.city))
+    file_name = os.path.join(data_dir, "{}_{}_pred.pkl".format(
+        data_loader.dataset.dataset, data_loader.dataset.city))
+
+    if os.path.exists(file_name):
+        with open(file_name, "rb") as fp:
+            pred_data = pickle.load(fp)
+    else:
+        with open(original_file, "rb") as fp:
+            pred_data = pickle.load(fp)
+            pred_data['Pred'] = {}
+
+    loader_id = data_loader.loader_id
+    if loader_id not in pred_data["Pred"].keys():
+        pred_data['Pred'][loader_id] = {}
+
+    pred_data['Pred'][loader_id]["GroundTruth"] = np.squeeze(
+        data_loader.test_y)
+
+    if loader_id.endswith("N"):
+        # use NodeTrafficLoader
+        pred_data['Pred'][loader_id][method] = {}
+        pred_data['Pred'][loader_id][method]["traffic_data_index"] = data_loader.traffic_data_index
+        pred_data['Pred'][loader_id][method]["TrafficNode"] = np.squeeze(
+            predict_val)
+
+    if loader_id.endswith("G"):
+        # use GridTrafficLoader
+        pred_data['Pred'][loader_id][method] = {}
+        pred_data['Pred'][loader_id][method]["TrafficGrid"] = np.squeeze(predict_val)
+
+    with open(file_name, "wb") as fp:
+        pickle.dump(pred_data, fp)
```

### Comparing `UCTB-0.3.0/UCTB/utils/multi_threads.py` & `UCTB-0.3.5/UCTB/utils/multi_threads.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-import os
-
-from multiprocessing import Pool, Manager
-from functools import reduce
-
-
-# (my_rank, n_jobs, dataList, resultHandleFunction, parameterList)
-def multiple_process(distribute_list, partition_func, task_func, n_jobs, reduce_func, parameters):
-
-    """
-    Args:
-
-        distribute_list(list): The "data" list to be partitioned, such as a list of files which will be
-            distributed among different tasks and each task process a part of the files.
-        partition_func(function): Partition function will be used to cut the distribute_list, it should accept
-            three inputs: distribute_list, i, n_job, where i is the index of jobs (i.e. integer from 0 to n_jobs-1),
-            n_jos is the number of threads; partition function should return a data_list for the job_i
-        task_func(function): Task function, where the inputs are share_queue, locker, data, parameters, no return.
-            pls refer to the DiDi-Data processing codes for more information.
-        n_jobs(int): Number of threads
-        reduce_func(function): Reduce function which combine the outputs from all the threads into one final output.
-        parameters(list): parameters send to the task function
-
-    """
-
-    if callable(partition_func) and callable(task_func) and callable(reduce_func):
-        print('Parent process %s.' % os.getpid())
-
-        manager = Manager()
-        share_queue = manager.Queue()
-        locker = manager.Lock()
-
-        p = Pool()
-        for i in range(n_jobs):
-            p.apply_async(task_func, args=(share_queue, locker, partition_func(distribute_list, i, n_jobs),
-                                           [i] + parameters,))
-        print('Waiting for all sub_processes done...')
-        p.close()
-        p.join()
-        print('All sub_processes done.')
-
-        result_list = []
-        while not share_queue.empty():
-            result_list.append(share_queue.get_nowait())
-
-        return reduce(reduce_func, result_list)
-    else:
-        print('Parameter error')
-
-
-"""
-# Example
-def task(share_queue, locker, data, parameters):
-
-    print('Child process %s with pid %s' % (parameters[0], os.getpid()))
-
-    result = sum(data)
-
-    locker.acquire()
-    share_queue.put(result)
-    locker.release()
-
-
-if __name__ == "__main__":
-
-    data = [e for e in range(1000000)]
-
-    n_job = 4
-
-    sum_result = \
-        multiple_process(distribute_list=data,
-                         partition_func=lambda data, i, n_job: [data[e] for e in range(len(data)) if e % n_job == i],
-                         task_func=task, n_jobs=n_job, reduce_func=lambda x, y: x + y, parameters=[])
-
-    print('Result', sum_result)
+import os
+
+from multiprocessing import Pool, Manager
+from functools import reduce
+
+
+# (my_rank, n_jobs, dataList, resultHandleFunction, parameterList)
+def multiple_process(distribute_list, partition_func, task_func, n_jobs, reduce_func, parameters):
+
+    """
+    Args:
+
+        distribute_list(list): The "data" list to be partitioned, such as a list of files which will be
+            distributed among different tasks and each task process a part of the files.
+        partition_func(function): Partition function will be used to cut the distribute_list, it should accept
+            three inputs: distribute_list, i, n_job, where i is the index of jobs (i.e. integer from 0 to n_jobs-1),
+            n_jos is the number of threads; partition function should return a data_list for the job_i
+        task_func(function): Task function, where the inputs are share_queue, locker, data, parameters, no return.
+            pls refer to the DiDi-Data processing codes for more information.
+        n_jobs(int): Number of threads
+        reduce_func(function): Reduce function which combine the outputs from all the threads into one final output.
+        parameters(list): parameters send to the task function
+
+    """
+
+    if callable(partition_func) and callable(task_func) and callable(reduce_func):
+        print('Parent process %s.' % os.getpid())
+
+        manager = Manager()
+        share_queue = manager.Queue()
+        locker = manager.Lock()
+
+        p = Pool()
+        for i in range(n_jobs):
+            p.apply_async(task_func, args=(share_queue, locker, partition_func(distribute_list, i, n_jobs),
+                                           [i] + parameters,))
+        print('Waiting for all sub_processes done...')
+        p.close()
+        p.join()
+        print('All sub_processes done.')
+
+        result_list = []
+        while not share_queue.empty():
+            result_list.append(share_queue.get_nowait())
+
+        return reduce(reduce_func, result_list)
+    else:
+        print('Parameter error')
+
+
+"""
+# Example
+def task(share_queue, locker, data, parameters):
+
+    print('Child process %s with pid %s' % (parameters[0], os.getpid()))
+
+    result = sum(data)
+
+    locker.acquire()
+    share_queue.put(result)
+    locker.release()
+
+
+if __name__ == "__main__":
+
+    data = [e for e in range(1000000)]
+
+    n_job = 4
+
+    sum_result = \
+        multiple_process(distribute_list=data,
+                         partition_func=lambda data, i, n_job: [data[e] for e in range(len(data)) if e % n_job == i],
+                         task_func=task, n_jobs=n_job, reduce_func=lambda x, y: x + y, parameters=[])
+
+    print('Result', sum_result)
 """
```

### Comparing `UCTB-0.3.0/UCTB.egg-info/SOURCES.txt` & `UCTB-0.3.5/UCTB.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -3,38 +3,53 @@
 UCTB/__init__.py
 UCTB.egg-info/PKG-INFO
 UCTB.egg-info/SOURCES.txt
 UCTB.egg-info/dependency_links.txt
 UCTB.egg-info/requires.txt
 UCTB.egg-info/top_level.txt
 UCTB/dataset/__init__.py
+UCTB/dataset/context_loader.py
 UCTB/dataset/data_loader.py
 UCTB/dataset/dataset.py
 UCTB/evaluation/__init__.py
 UCTB/evaluation/metric.py
+UCTB/model/AGCRN.py
 UCTB/model/ARIMA.py
+UCTB/model/ASTGCN.py
 UCTB/model/DCRNN.py
 UCTB/model/DeepST.py
+UCTB/model/GMAN.py
 UCTB/model/GeoMAN.py
+UCTB/model/GraphWaveNet.py
 UCTB/model/HM.py
 UCTB/model/HMM.py
 UCTB/model/MCSTGCN.py
+UCTB/model/STGCN.py
 UCTB/model/STMeta.py
+UCTB/model/STSGCN.py
 UCTB/model/ST_MGCN.py
 UCTB/model/ST_ResNet.py
 UCTB/model/XGBoost.py
 UCTB/model/__init__.py
 UCTB/model_unit/BaseModel.py
 UCTB/model_unit/DCRNN_CELL.py
 UCTB/model_unit/GraphModelLayers.py
 UCTB/model_unit/ST_RNN.py
 UCTB/model_unit/__init__.py
 UCTB/preprocess/GraphGenerator.py
 UCTB/preprocess/__init__.py
+UCTB/preprocess/dataset_helper.py
 UCTB/preprocess/preprocessor.py
 UCTB/preprocess/time_utils.py
 UCTB/train/EarlyStopping.py
+UCTB/train/LossFunction.py
 UCTB/train/MiniBatchTrain.py
 UCTB/train/__init__.py
 UCTB/utils/__init__.py
 UCTB/utils/make_predict_dataset.py
-UCTB/utils/multi_threads.py
+UCTB/utils/multi_threads.py
+UCTB/utils/utils_AGCRN.py
+UCTB/utils/utils_ASTGCN.py
+UCTB/utils/utils_GMAN.py
+UCTB/utils/utils_GraphWaveNet.py
+UCTB/utils/utils_STGCN.py
+UCTB/utils/utils_STSGCN.py
```

