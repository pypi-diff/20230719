# Comparing `tmp/similarity_ts_cli-1.0.0.tar.gz` & `tmp/similarity_ts_cli-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "similarity_ts_cli-1.0.0.tar", last modified: Tue Jul 18 06:46:27 2023, max compression
+gzip compressed data, was "similarity_ts_cli-1.0.1.tar", last modified: Wed Jul 19 11:49:12 2023, max compression
```

## Comparing `similarity_ts_cli-1.0.0.tar` & `similarity_ts_cli-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-18 06:46:27.485705 similarity_ts_cli-1.0.0/
--rw-r--r--   0 afdez      (501) staff       (20)     1079 2023-07-16 10:03:02.000000 similarity_ts_cli-1.0.0/LICENSE
--rw-r--r--   0 afdez      (501) staff       (20)    12046 2023-07-18 06:46:27.485486 similarity_ts_cli-1.0.0/PKG-INFO
--rw-r--r--   0 afdez      (501) staff       (20)    11303 2023-07-18 06:45:51.000000 similarity_ts_cli-1.0.0/README.md
--rw-r--r--   0 afdez      (501) staff       (20)      981 2023-07-18 06:33:51.000000 similarity_ts_cli-1.0.0/pyproject.toml
--rw-r--r--   0 afdez      (501) staff       (20)       38 2023-07-18 06:46:27.485765 similarity_ts_cli-1.0.0/setup.cfg
-drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-18 06:46:27.482695 similarity_ts_cli-1.0.0/src/
-drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-18 06:46:27.483952 similarity_ts_cli-1.0.0/src/similarity_ts_cli/
--rw-r--r--   0 afdez      (501) staff       (20)        0 2023-07-16 09:41:32.000000 similarity_ts_cli-1.0.0/src/similarity_ts_cli/__init__.py
--rw-r--r--   0 afdez      (501) staff       (20)     8055 2023-07-17 10:40:14.000000 similarity_ts_cli-1.0.0/src/similarity_ts_cli/cli.py
-drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-18 06:46:27.485220 similarity_ts_cli-1.0.0/src/similarity_ts_cli.egg-info/
--rw-r--r--   0 afdez      (501) staff       (20)    12046 2023-07-18 06:46:27.000000 similarity_ts_cli-1.0.0/src/similarity_ts_cli.egg-info/PKG-INFO
--rw-r--r--   0 afdez      (501) staff       (20)      367 2023-07-18 06:46:27.000000 similarity_ts_cli-1.0.0/src/similarity_ts_cli.egg-info/SOURCES.txt
--rw-r--r--   0 afdez      (501) staff       (20)        1 2023-07-18 06:46:27.000000 similarity_ts_cli-1.0.0/src/similarity_ts_cli.egg-info/dependency_links.txt
--rw-r--r--   0 afdez      (501) staff       (20)       65 2023-07-18 06:46:27.000000 similarity_ts_cli-1.0.0/src/similarity_ts_cli.egg-info/entry_points.txt
--rw-r--r--   0 afdez      (501) staff       (20)       19 2023-07-18 06:46:27.000000 similarity_ts_cli-1.0.0/src/similarity_ts_cli.egg-info/requires.txt
--rw-r--r--   0 afdez      (501) staff       (20)       18 2023-07-18 06:46:27.000000 similarity_ts_cli-1.0.0/src/similarity_ts_cli.egg-info/top_level.txt
+drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-19 11:49:12.123666 similarity_ts_cli-1.0.1/
+-rw-r--r--   0 afdez      (501) staff       (20)     1079 2023-07-16 10:03:02.000000 similarity_ts_cli-1.0.1/LICENSE
+-rw-r--r--   0 afdez      (501) staff       (20)    12252 2023-07-19 11:49:12.123111 similarity_ts_cli-1.0.1/PKG-INFO
+-rw-r--r--   0 afdez      (501) staff       (20)    11509 2023-07-19 11:47:57.000000 similarity_ts_cli-1.0.1/README.md
+-rw-r--r--   0 afdez      (501) staff       (20)      981 2023-07-19 11:44:09.000000 similarity_ts_cli-1.0.1/pyproject.toml
+-rw-r--r--   0 afdez      (501) staff       (20)       38 2023-07-19 11:49:12.123729 similarity_ts_cli-1.0.1/setup.cfg
+drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-19 11:49:12.119834 similarity_ts_cli-1.0.1/src/
+drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-19 11:49:12.121073 similarity_ts_cli-1.0.1/src/similarity_ts_cli/
+-rw-r--r--   0 afdez      (501) staff       (20)        0 2023-07-16 09:41:32.000000 similarity_ts_cli-1.0.1/src/similarity_ts_cli/__init__.py
+-rw-r--r--   0 afdez      (501) staff       (20)     8055 2023-07-17 10:40:14.000000 similarity_ts_cli-1.0.1/src/similarity_ts_cli/cli.py
+drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-19 11:49:12.122806 similarity_ts_cli-1.0.1/src/similarity_ts_cli.egg-info/
+-rw-r--r--   0 afdez      (501) staff       (20)    12252 2023-07-19 11:49:12.000000 similarity_ts_cli-1.0.1/src/similarity_ts_cli.egg-info/PKG-INFO
+-rw-r--r--   0 afdez      (501) staff       (20)      367 2023-07-19 11:49:12.000000 similarity_ts_cli-1.0.1/src/similarity_ts_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 afdez      (501) staff       (20)        1 2023-07-19 11:49:12.000000 similarity_ts_cli-1.0.1/src/similarity_ts_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 afdez      (501) staff       (20)       65 2023-07-19 11:49:12.000000 similarity_ts_cli-1.0.1/src/similarity_ts_cli.egg-info/entry_points.txt
+-rw-r--r--   0 afdez      (501) staff       (20)       19 2023-07-19 11:49:12.000000 similarity_ts_cli-1.0.1/src/similarity_ts_cli.egg-info/requires.txt
+-rw-r--r--   0 afdez      (501) staff       (20)       18 2023-07-19 11:49:12.000000 similarity_ts_cli-1.0.1/src/similarity_ts_cli.egg-info/top_level.txt
```

### Comparing `similarity_ts_cli-1.0.0/LICENSE` & `similarity_ts_cli-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `similarity_ts_cli-1.0.0/PKG-INFO` & `similarity_ts_cli-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 Metadata-Version: 2.1
 Name: similarity_ts_cli
-Version: 1.0.0
+Version: 1.0.1
 Summary: SimilarityTS-cli is an open-source tool designed to facilitate the usage of SimilarityTS package from a command line interface
 Author-email: Alejandro Fernández-Montes <afdez@us.es>, Damián Fernández-Cerero <damiancerero@us.es>, Felipe Escalera González <fescalera@us.es>
 Project-URL: Homepage, https://github.com/alejandrofdez-us/similarity-ts-cli
 Project-URL: Bug Tracker, https://github.com/alejandrofdez-us/similarity-ts-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![version](https://img.shields.io/badge/version-1.0-blue)](https://github.com/alejandrofdez-us/similarity-ts/releases)
+[![version](https://img.shields.io/badge/pypi-1.0.1-blue)](https://pypi.org/project/similarity-ts-cli/)
 [![Python 3.9](https://img.shields.io/badge/python-3.9-darkgreen)](https://www.python.org/downloads/release/python-390/)
-[![last-update](https://img.shields.io/badge/last_update-07/XY/2023-brightgreen)](https://github.com/alejandrofdez-us/similarity-ts/commits/main)
-![license](https://img.shields.io/badge/license-MIT-orange)
+[![last-update](https://img.shields.io/badge/last_update-07/18/2023-brightgreen)](https://github.com/alejandrofdez-us/similarity-ts-cli/commits/main)
+[![license](https://img.shields.io/badge/license-MIT-orange)](LICENSE)
 
 # SimilarityTS-cli: Command-line interface for SimilarityTS package
 
 ## Table of Contents
 
 - [Description](#description)
 - [Installation](#installation)
 - [Usage](#usage)
-- [Advanced usage](#advanced-usage)
 - [License](#license)
+- [Acknowledgements](#acknowledgements)
 
 ## Description
 
-SimilarityTS-cli is a command-line interface tool that act as an interface of the SimilarityTS package. Similarity-TS package facilitates the evaluation and comparison of
+SimilarityTS-cli is a command-line interface tool that act as an interface of the [SimilarityTS package](https://github.com/alejandrofdez-us/similarity-ts). Similarity-TS package facilitates the evaluation and comparison of
 multivariate time series data. It provides a comprehensive toolkit for analyzing, visualizing, and reporting multiple
 metrics and figures derived from time series datasets. The toolkit simplifies the process of evaluating the similarity of
 time series by offering data preprocessing, metrics computation, visualization, statistical analysis, and report generation
 functionalities. With its customizable features, SimilarityTS empowers researchers and data
 scientists to gain insights, identify patterns, and make informed decisions based on their time series data.
 
-This command-line interface is OS independant and can be easily installed and used.
+This command-line interface is OS independent and can be easily installed and used.
 
 ### Available metrics
 
 This toolkit can compute the following metrics:
 
 - `kl`: Kullback-Leibler divergence
 - `js`: Jensen-Shannon divergence
@@ -115,19 +115,21 @@
 Constraints:
 
 - `-ts1` time-series file and `-ts2` time-series file(s) must:
     - have the same dimensionality (number of columns)
     - not include a timestamp column
     - include only numeric values
     - include the same header (if present)
-- if a header is present as first row, use the `-head` argument
+- if a header is present as first row, use the `-head` argument.
 - all `-ts2` time-series files must have the same length (number of rows).
 
 Note: the column delimiter is automatically detected.
 
+If your data include categorical values, it might be pre-processed to convert them to numerical values. All `ts2s` time-series must have the same length (number of rows).
+
 If `-ts1` time-series file is longer (more rows) than `-ts2` time-series file(s), the `-ts1` time series will be
 divided in windows of the same
 length as the `-ts2` time-series file(s).
 
 For each `-ts2` time-series file, the most similar window (*) from `-ts1` time series is selected.
 
 Finally, metrics and figures that assess the similarity between each pair of `-ts2` time-series file and its
@@ -137,15 +139,15 @@
 similar `-ts1` time-series window per each `-ts2` time-series file(s).`dtw` is the default value, however, any of
 the
 [metrics](#available-metrics) are also available for this purpose using this argument.
 
 Users can provide metrics or figures to be computed/generated:
 
 - `-m` the [metrics](#available-metrics) names to be computed as a list separated by spaces.
-- `-f` the [figures](#available-figures) names to be computed as a list separated by spaces
+- `-f` the [figures](#available-figures) names to be computed as a list separated by spaces.
 
 If no metrics nor figures are provided, the tool will compute all the available metrics and figures.
 
 The following arguments are also available for fine-tuning:
 
 - `-ts_freq_secs` the frequency in seconds in which samples were taken just to generate the delta figures. By default is
   `1` second.
@@ -169,19 +171,14 @@
    Every metric computation and figure generated will be found in the `results/{timestamp}/` directory.
 
 1. Two time series computing only DTW metric and DTW figure:
     ```Bash
     similarity-ts-cli -ts1 data_samples/alibaba2018/ts1_machine_usage_days_1_to_8_grouped_300_seconds.csv -ts2 data_samples/alibaba2018/ts2/sample_0.csv -head -m dtw -f dtw
     ```
 
-1. Two time series computing only DTW metric and DTW figure:
-    ```Bash
-    similarity-ts-cli -ts1 data_samples/alibaba2018/ts1_machine_usage_days_1_to_8_grouped_300_seconds.csv -ts2 data_samples/alibaba2018/ts2/sample_0.csv -head -m dtw -f dtw
-    ```
-
 1. A time series and all time series within a directory computing every metric and figure in SimilarityTS toolkit:
     ```Bash
     similarity-ts-cli -ts1 data_samples/alibaba2018/ts1_machine_usage_days_1_to_8_grouped_300_seconds.csv -ts2 data_samples/alibaba2018/ts2 -head -m js mmd dtw ks kl cc cp hi -f delta dtw 2d pca tsne
     ```
 
 1. Comparison between time series specifying the frequency in seconds in which samples were taken:
     ```Bash
@@ -206,7 +203,10 @@
 
     ```Bash
     similarity-ts-cli -ts1 data_samples/alibaba2018/ts1_machine_usage_days_1_to_8_grouped_300_seconds.csv -ts2 data_samples/alibaba2018/ts2 -head -m mmd dtw ks kl cc cp hi -f delta dtw 2d pca tsne -w_select_met cc -ts_freq_secs 300 -strd 5
     ```
 ## License
 
 SimilarityTS toolkit is free and open-source software licensed under the [MIT license](LICENSE).
+
+## Acknowledgements
+Project PID2021-122208OB-I00, PROYEXCEL\_00286 and  TED2021-132695B-I00 project, funded by MCIN / AEI / 10.13039 / 501100011033, by Andalusian Regional Government, and by the European Union - NextGenerationEU.
```

### Comparing `similarity_ts_cli-1.0.0/README.md` & `similarity_ts_cli-1.0.1/src/similarity_ts_cli.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,707 +1,766 @@
-00000000: 5b21 5b76 6572 7369 6f6e 5d28 6874 7470  [![version](http
-00000010: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000020: 696f 2f62 6164 6765 2f76 6572 7369 6f6e  io/badge/version
-00000030: 2d31 2e30 2d62 6c75 6529 5d28 6874 7470  -1.0-blue)](http
-00000040: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f61  s://github.com/a
-00000050: 6c65 6a61 6e64 726f 6664 657a 2d75 732f  lejandrofdez-us/
-00000060: 7369 6d69 6c61 7269 7479 2d74 732f 7265  similarity-ts/re
-00000070: 6c65 6173 6573 290a 5b21 5b50 7974 686f  leases).[![Pytho
-00000080: 6e20 332e 395d 2868 7474 7073 3a2f 2f69  n 3.9](https://i
-00000090: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
-000000a0: 6467 652f 7079 7468 6f6e 2d33 2e39 2d64  dge/python-3.9-d
-000000b0: 6172 6b67 7265 656e 295d 2868 7474 7073  arkgreen)](https
-000000c0: 3a2f 2f77 7777 2e70 7974 686f 6e2e 6f72  ://www.python.or
-000000d0: 672f 646f 776e 6c6f 6164 732f 7265 6c65  g/downloads/rele
-000000e0: 6173 652f 7079 7468 6f6e 2d33 3930 2f29  ase/python-390/)
-000000f0: 0a5b 215b 6c61 7374 2d75 7064 6174 655d  .[![last-update]
-00000100: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-00000110: 656c 6473 2e69 6f2f 6261 6467 652f 6c61  elds.io/badge/la
-00000120: 7374 5f75 7064 6174 652d 3037 2f58 592f  st_update-07/XY/
-00000130: 3230 3233 2d62 7269 6768 7467 7265 656e  2023-brightgreen
-00000140: 295d 2868 7474 7073 3a2f 2f67 6974 6875  )](https://githu
-00000150: 622e 636f 6d2f 616c 656a 616e 6472 6f66  b.com/alejandrof
-00000160: 6465 7a2d 7573 2f73 696d 696c 6172 6974  dez-us/similarit
-00000170: 792d 7473 2f63 6f6d 6d69 7473 2f6d 6169  y-ts/commits/mai
-00000180: 6e29 0a21 5b6c 6963 656e 7365 5d28 6874  n).![license](ht
-00000190: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-000001a0: 732e 696f 2f62 6164 6765 2f6c 6963 656e  s.io/badge/licen
-000001b0: 7365 2d4d 4954 2d6f 7261 6e67 6529 0a0a  se-MIT-orange)..
-000001c0: 2320 5369 6d69 6c61 7269 7479 5453 2d63  # SimilarityTS-c
-000001d0: 6c69 3a20 436f 6d6d 616e 642d 6c69 6e65  li: Command-line
-000001e0: 2069 6e74 6572 6661 6365 2066 6f72 2053   interface for S
-000001f0: 696d 696c 6172 6974 7954 5320 7061 636b  imilarityTS pack
-00000200: 6167 650a 0a23 2320 5461 626c 6520 6f66  age..## Table of
-00000210: 2043 6f6e 7465 6e74 730a 0a2d 205b 4465   Contents..- [De
-00000220: 7363 7269 7074 696f 6e5d 2823 6465 7363  scription](#desc
-00000230: 7269 7074 696f 6e29 0a2d 205b 496e 7374  ription).- [Inst
-00000240: 616c 6c61 7469 6f6e 5d28 2369 6e73 7461  allation](#insta
-00000250: 6c6c 6174 696f 6e29 0a2d 205b 5573 6167  llation).- [Usag
-00000260: 655d 2823 7573 6167 6529 0a2d 205b 4164  e](#usage).- [Ad
-00000270: 7661 6e63 6564 2075 7361 6765 5d28 2361  vanced usage](#a
-00000280: 6476 616e 6365 642d 7573 6167 6529 0a2d  dvanced-usage).-
-00000290: 205b 4c69 6365 6e73 655d 2823 6c69 6365   [License](#lice
-000002a0: 6e73 6529 0a0a 2323 2044 6573 6372 6970  nse)..## Descrip
-000002b0: 7469 6f6e 0a0a 5369 6d69 6c61 7269 7479  tion..Similarity
-000002c0: 5453 2d63 6c69 2069 7320 6120 636f 6d6d  TS-cli is a comm
-000002d0: 616e 642d 6c69 6e65 2069 6e74 6572 6661  and-line interfa
-000002e0: 6365 2074 6f6f 6c20 7468 6174 2061 6374  ce tool that act
-000002f0: 2061 7320 616e 2069 6e74 6572 6661 6365   as an interface
-00000300: 206f 6620 7468 6520 5369 6d69 6c61 7269   of the Similari
-00000310: 7479 5453 2070 6163 6b61 6765 2e20 5369  tyTS package. Si
-00000320: 6d69 6c61 7269 7479 2d54 5320 7061 636b  milarity-TS pack
-00000330: 6167 6520 6661 6369 6c69 7461 7465 7320  age facilitates 
-00000340: 7468 6520 6576 616c 7561 7469 6f6e 2061  the evaluation a
-00000350: 6e64 2063 6f6d 7061 7269 736f 6e20 6f66  nd comparison of
-00000360: 0a6d 756c 7469 7661 7269 6174 6520 7469  .multivariate ti
-00000370: 6d65 2073 6572 6965 7320 6461 7461 2e20  me series data. 
-00000380: 4974 2070 726f 7669 6465 7320 6120 636f  It provides a co
-00000390: 6d70 7265 6865 6e73 6976 6520 746f 6f6c  mprehensive tool
-000003a0: 6b69 7420 666f 7220 616e 616c 797a 696e  kit for analyzin
-000003b0: 672c 2076 6973 7561 6c69 7a69 6e67 2c20  g, visualizing, 
-000003c0: 616e 6420 7265 706f 7274 696e 6720 6d75  and reporting mu
-000003d0: 6c74 6970 6c65 0a6d 6574 7269 6373 2061  ltiple.metrics a
-000003e0: 6e64 2066 6967 7572 6573 2064 6572 6976  nd figures deriv
-000003f0: 6564 2066 726f 6d20 7469 6d65 2073 6572  ed from time ser
-00000400: 6965 7320 6461 7461 7365 7473 2e20 5468  ies datasets. Th
-00000410: 6520 746f 6f6c 6b69 7420 7369 6d70 6c69  e toolkit simpli
-00000420: 6669 6573 2074 6865 2070 726f 6365 7373  fies the process
-00000430: 206f 6620 6576 616c 7561 7469 6e67 2074   of evaluating t
-00000440: 6865 2073 696d 696c 6172 6974 7920 6f66  he similarity of
-00000450: 0a74 696d 6520 7365 7269 6573 2062 7920  .time series by 
-00000460: 6f66 6665 7269 6e67 2064 6174 6120 7072  offering data pr
-00000470: 6570 726f 6365 7373 696e 672c 206d 6574  eprocessing, met
-00000480: 7269 6373 2063 6f6d 7075 7461 7469 6f6e  rics computation
-00000490: 2c20 7669 7375 616c 697a 6174 696f 6e2c  , visualization,
-000004a0: 2073 7461 7469 7374 6963 616c 2061 6e61   statistical ana
-000004b0: 6c79 7369 732c 2061 6e64 2072 6570 6f72  lysis, and repor
-000004c0: 7420 6765 6e65 7261 7469 6f6e 0a66 756e  t generation.fun
-000004d0: 6374 696f 6e61 6c69 7469 6573 2e20 5769  ctionalities. Wi
-000004e0: 7468 2069 7473 2063 7573 746f 6d69 7a61  th its customiza
-000004f0: 626c 6520 6665 6174 7572 6573 2c20 5369  ble features, Si
-00000500: 6d69 6c61 7269 7479 5453 2065 6d70 6f77  milarityTS empow
-00000510: 6572 7320 7265 7365 6172 6368 6572 7320  ers researchers 
-00000520: 616e 6420 6461 7461 0a73 6369 656e 7469  and data.scienti
-00000530: 7374 7320 746f 2067 6169 6e20 696e 7369  sts to gain insi
-00000540: 6768 7473 2c20 6964 656e 7469 6679 2070  ghts, identify p
-00000550: 6174 7465 726e 732c 2061 6e64 206d 616b  atterns, and mak
-00000560: 6520 696e 666f 726d 6564 2064 6563 6973  e informed decis
-00000570: 696f 6e73 2062 6173 6564 206f 6e20 7468  ions based on th
-00000580: 6569 7220 7469 6d65 2073 6572 6965 7320  eir time series 
-00000590: 6461 7461 2e0a 0a54 6869 7320 636f 6d6d  data...This comm
-000005a0: 616e 642d 6c69 6e65 2069 6e74 6572 6661  and-line interfa
-000005b0: 6365 2069 7320 4f53 2069 6e64 6570 656e  ce is OS indepen
-000005c0: 6461 6e74 2061 6e64 2063 616e 2062 6520  dant and can be 
-000005d0: 6561 7369 6c79 2069 6e73 7461 6c6c 6564  easily installed
-000005e0: 2061 6e64 2075 7365 642e 0a0a 2323 2320   and used...### 
-000005f0: 4176 6169 6c61 626c 6520 6d65 7472 6963  Available metric
-00000600: 730a 0a54 6869 7320 746f 6f6c 6b69 7420  s..This toolkit 
-00000610: 6361 6e20 636f 6d70 7574 6520 7468 6520  can compute the 
-00000620: 666f 6c6c 6f77 696e 6720 6d65 7472 6963  following metric
-00000630: 733a 0a0a 2d20 606b 6c60 3a20 4b75 6c6c  s:..- `kl`: Kull
-00000640: 6261 636b 2d4c 6569 626c 6572 2064 6976  back-Leibler div
-00000650: 6572 6765 6e63 650a 2d20 606a 7360 3a20  ergence.- `js`: 
-00000660: 4a65 6e73 656e 2d53 6861 6e6e 6f6e 2064  Jensen-Shannon d
-00000670: 6976 6572 6765 6e63 650a 2d20 606b 7360  ivergence.- `ks`
-00000680: 3a20 4b6f 6c6d 6f67 6f72 6f76 2d53 6d69  : Kolmogorov-Smi
-00000690: 726e 6f76 2074 6573 740a 2d20 606d 6d64  rnov test.- `mmd
-000006a0: 603a 204d 6178 696d 756d 204d 6561 6e20  `: Maximum Mean 
-000006b0: 4469 7363 7265 7061 6e63 790a 2d20 6064  Discrepancy.- `d
-000006c0: 7477 6020 4479 6e61 6d69 6320 5469 6d65  tw` Dynamic Time
-000006d0: 2057 6172 7069 6e67 0a2d 2060 6363 603a   Warping.- `cc`:
-000006e0: 2044 6966 6665 7265 6e63 6520 6f66 2063   Difference of c
-000006f0: 6f2d 7661 7269 616e 6365 730a 2d20 6063  o-variances.- `c
-00000700: 7060 3a20 4469 6666 6572 656e 6365 206f  p`: Difference o
-00000710: 6620 636f 7272 656c 6174 696f 6e73 0a2d  f correlations.-
-00000720: 2060 6869 603a 2044 6966 6665 7265 6e63   `hi`: Differenc
-00000730: 6520 6f66 2068 6973 746f 6772 616d 730a  e of histograms.
-00000740: 0a23 2323 2041 7661 696c 6162 6c65 2066  .### Available f
-00000750: 6967 7572 6573 0a0a 5468 6973 2074 6f6f  igures..This too
-00000760: 6c6b 6974 2063 616e 2067 656e 6572 6174  lkit can generat
-00000770: 6520 7468 6520 666f 6c6c 6f77 696e 6720  e the following 
-00000780: 6669 6775 7265 733a 0a0a 2d20 6032 6460  figures:..- `2d`
-00000790: 3a20 7468 6520 6f72 6469 6e61 7279 2067  : the ordinary g
-000007a0: 7261 7068 6963 616c 2072 6570 7265 7365  raphical represe
-000007b0: 6e74 6174 696f 6e20 6f66 2074 6865 2074  ntation of the t
-000007c0: 696d 6520 7365 7269 6573 2069 6e20 6120  ime series in a 
-000007d0: 3244 2066 6967 7572 6520 7769 7468 2074  2D figure with t
-000007e0: 6865 2074 696d 6520 7265 7072 6573 656e  he time represen
-000007f0: 7465 6420 6f6e 2074 6865 2078 2061 7869  ted on the x axi
-00000800: 730a 2020 616e 6420 7468 6520 6461 7461  s.  and the data
-00000810: 2076 616c 7565 7320 6f6e 2074 6865 2079   values on the y
-00000820: 2d61 7869 7320 666f 720a 2020 2020 2d20  -axis for.    - 
-00000830: 7468 6520 636f 6d70 6c65 7465 206d 756c  the complete mul
-00000840: 7469 7661 7269 6174 6520 7469 6d65 2073  tivariate time s
-00000850: 6572 6965 733b 2061 6e64 0a20 2020 202d  eries; and.    -
-00000860: 2061 2070 6c6f 7420 7065 7220 636f 6c75   a plot per colu
-00000870: 6d6e 2e0a 0a20 2045 6163 6820 6765 6e65  mn...  Each gene
-00000880: 7261 7465 6420 6669 6775 7265 2070 6c6f  rated figure plo
-00000890: 7473 2062 6f74 6820 7468 6520 6074 7331  ts both the `ts1
-000008a0: 6020 616e 6420 7468 6520 6074 7332 6020  ` and the `ts2` 
-000008b0: 6461 7461 2074 6f20 6561 7369 6c79 206f  data to easily o
-000008c0: 6274 6169 6e20 6b65 7920 696e 7369 6768  btain key insigh
-000008d0: 7473 2069 6e74 6f0a 2020 7468 6520 7369  ts into.  the si
-000008e0: 6d69 6c61 7269 7469 6573 206f 7220 6469  milarities or di
-000008f0: 6666 6572 656e 6365 7320 6265 7477 6565  fferences betwee
-00000900: 6e20 7468 656d 2e0a 2020 2020 3c64 6976  n them..    <div
-00000910: 3e0a 2020 2020 3c69 6d67 2073 7263 3d22  >.    <img src="
-00000920: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000930: 6f6d 2f61 6c65 6a61 6e64 726f 6664 657a  om/alejandrofdez
-00000940: 2d75 732f 7369 6d69 6c61 7269 7479 2d74  -us/similarity-t
-00000950: 732f 626c 6f62 2f65 3562 3134 3762 3134  s/blob/e5b147b14
-00000960: 3539 3730 6633 6139 3333 3531 6131 3030  5970f3a93351a100
-00000970: 3430 3232 6662 3330 6432 3066 3566 302f  4022fb30d20f5f0/
-00000980: 646f 6373 2f66 6967 7572 6573 2f32 645f  docs/figures/2d_
-00000990: 7361 6d70 6c65 5f33 5f63 6f6d 706c 6574  sample_3_complet
-000009a0: 655f 5453 5f31 5f76 735f 5453 5f32 2e70  e_TS_1_vs_TS_2.p
-000009b0: 6e67 3f72 6177 3d74 7275 6522 2061 6c74  ng?raw=true" alt
-000009c0: 3d22 3244 2046 6967 7572 6520 636f 6d70  ="2D Figure comp
-000009d0: 6c65 7465 223e 0a20 2020 203c 696d 6720  lete">.    <img 
-000009e0: 7372 633d 2268 7474 7073 3a2f 2f67 6974  src="https://git
-000009f0: 6875 622e 636f 6d2f 616c 656a 616e 6472  hub.com/alejandr
-00000a00: 6f66 6465 7a2d 7573 2f73 696d 696c 6172  ofdez-us/similar
-00000a10: 6974 792d 7473 2f62 6c6f 622f 6535 6231  ity-ts/blob/e5b1
-00000a20: 3437 6231 3435 3937 3066 3361 3933 3335  47b145970f3a9335
-00000a30: 3161 3130 3034 3032 3266 6233 3064 3230  1a1004022fb30d20
-00000a40: 6635 6630 2f64 6f63 732f 6669 6775 7265  f5f0/docs/figure
-00000a50: 732f 3264 5f73 616d 706c 655f 335f 6370  s/2d_sample_3_cp
-00000a60: 755f 7574 696c 5f70 6572 6365 6e74 5f54  u_util_percent_T
-00000a70: 535f 315f 7673 5f54 535f 322e 706e 673f  S_1_vs_TS_2.png?
-00000a80: 7261 773d 7472 7565 2220 616c 743d 2232  raw=true" alt="2
-00000a90: 4420 4669 6775 7265 2066 6f72 2075 7365  D Figure for use
-00000aa0: 6420 4350 5520 7065 7263 656e 7461 6765  d CPU percentage
-00000ab0: 223e 0a20 2020 203c 2f64 6976 3e0a 2d20  ">.    </div>.- 
-00000ac0: 6064 656c 7461 603a 2074 6865 2064 6966  `delta`: the dif
-00000ad0: 6665 7265 6e63 6573 2062 6574 7765 656e  ferences between
-00000ae0: 2074 6865 2076 616c 7565 7320 6f66 2065   the values of e
-00000af0: 6163 6820 636f 6c75 6d6e 2067 726f 7570  ach column group
-00000b00: 6564 2062 7920 7065 7269 6f64 7320 6f66  ed by periods of
-00000b10: 2074 696d 652e 2046 6f72 2069 6e73 7461   time. For insta
-00000b20: 6e63 652c 2074 6865 2064 6966 6665 7265  nce, the differe
-00000b30: 6e63 6573 0a20 2062 6574 7765 656e 2074  nces.  between t
-00000b40: 6865 2070 6572 6365 6e74 6167 6520 6f66  he percentage of
-00000b50: 2063 7075 2075 7365 6420 6576 6572 7920   cpu used every 
-00000b60: 3130 2c20 3235 206f 7220 3530 206d 696e  10, 25 or 50 min
-00000b70: 7574 6573 2e20 5468 6573 6520 6465 6c74  utes. These delt
-00000b80: 6120 6361 6e20 6265 2075 7365 6420 6173  a can be used as
-00000b90: 2061 206d 6561 6e73 206f 6620 636f 6d70   a means of comp
-00000ba0: 6172 6973 6f6e 2062 6574 7765 656e 0a20  arison between. 
-00000bb0: 2074 696d 6520 7365 7269 6573 2073 686f   time series sho
-00000bc0: 7274 2d2f 6d69 642d 2f6c 6f6e 672d 7465  rt-/mid-/long-te
-00000bd0: 726d 2070 6174 7465 726e 732e 0a20 2020  rm patterns..   
-00000be0: 203c 6469 763e 0a20 2020 203c 696d 6720   <div>.    <img 
-00000bf0: 7372 633d 2268 7474 7073 3a2f 2f67 6974  src="https://git
-00000c00: 6875 622e 636f 6d2f 616c 656a 616e 6472  hub.com/alejandr
-00000c10: 6f66 6465 7a2d 7573 2f73 696d 696c 6172  ofdez-us/similar
-00000c20: 6974 792d 7473 2f62 6c6f 622f 6535 6231  ity-ts/blob/e5b1
-00000c30: 3437 6231 3435 3937 3066 3361 3933 3335  47b145970f3a9335
-00000c40: 3161 3130 3034 3032 3266 6233 3064 3230  1a1004022fb30d20
-00000c50: 6635 6630 2f64 6f63 732f 6669 6775 7265  f5f0/docs/figure
-00000c60: 732f 6465 6c74 615f 7361 6d70 6c65 5f33  s/delta_sample_3
-00000c70: 5f63 7075 5f75 7469 6c5f 7065 7263 656e  _cpu_util_percen
-00000c80: 745f 5453 5f31 5f76 735f 5453 5f32 5f28  t_TS_1_vs_TS_2_(
-00000c90: 6772 6f75 7065 645f 6279 5f31 305f 6d69  grouped_by_10_mi
-00000ca0: 6e75 7465 7329 2e70 6e67 3f72 6177 3d74  nutes).png?raw=t
-00000cb0: 7275 6522 2061 6c74 3d22 4465 6c74 6120  rue" alt="Delta 
-00000cc0: 4669 6775 7265 2066 6f72 2075 7365 6420  Figure for used 
-00000cd0: 4350 5520 7065 7263 656e 7461 6765 2067  CPU percentage g
-00000ce0: 726f 7570 6564 2062 7920 3130 206d 696e  rouped by 10 min
-00000cf0: 7574 6573 223e 0a20 2020 203c 696d 6720  utes">.    <img 
-00000d00: 7372 633d 2268 7474 7073 3a2f 2f67 6974  src="https://git
-00000d10: 6875 622e 636f 6d2f 616c 656a 616e 6472  hub.com/alejandr
-00000d20: 6f66 6465 7a2d 7573 2f73 696d 696c 6172  ofdez-us/similar
-00000d30: 6974 792d 7473 2f62 6c6f 622f 6535 6231  ity-ts/blob/e5b1
-00000d40: 3437 6231 3435 3937 3066 3361 3933 3335  47b145970f3a9335
-00000d50: 3161 3130 3034 3032 3266 6233 3064 3230  1a1004022fb30d20
-00000d60: 6635 6630 2f64 6f63 732f 6669 6775 7265  f5f0/docs/figure
-00000d70: 732f 6465 6c74 615f 7361 6d70 6c65 5f33  s/delta_sample_3
-00000d80: 5f63 7075 5f75 7469 6c5f 7065 7263 656e  _cpu_util_percen
-00000d90: 745f 5453 5f31 5f76 735f 5453 5f32 5f28  t_TS_1_vs_TS_2_(
-00000da0: 6772 6f75 7065 645f 6279 5f32 355f 6d69  grouped_by_25_mi
-00000db0: 6e75 7465 7329 2e70 6e67 3f72 6177 3d74  nutes).png?raw=t
-00000dc0: 7275 6522 2061 6c74 3d22 4465 6c74 6120  rue" alt="Delta 
-00000dd0: 4669 6775 7265 2066 6f72 2075 7365 6420  Figure for used 
-00000de0: 4350 5520 7065 7263 656e 7461 6765 2067  CPU percentage g
-00000df0: 726f 7570 6564 2062 7920 3235 206d 696e  rouped by 25 min
-00000e00: 7574 6573 223e 0a20 2020 203c 696d 6720  utes">.    <img 
-00000e10: 7372 633d 2268 7474 7073 3a2f 2f67 6974  src="https://git
-00000e20: 6875 622e 636f 6d2f 616c 656a 616e 6472  hub.com/alejandr
-00000e30: 6f66 6465 7a2d 7573 2f73 696d 696c 6172  ofdez-us/similar
-00000e40: 6974 792d 7473 2f62 6c6f 622f 6535 6231  ity-ts/blob/e5b1
-00000e50: 3437 6231 3435 3937 3066 3361 3933 3335  47b145970f3a9335
-00000e60: 3161 3130 3034 3032 3266 6233 3064 3230  1a1004022fb30d20
-00000e70: 6635 6630 2f64 6f63 732f 6669 6775 7265  f5f0/docs/figure
-00000e80: 732f 6465 6c74 615f 7361 6d70 6c65 5f33  s/delta_sample_3
-00000e90: 5f63 7075 5f75 7469 6c5f 7065 7263 656e  _cpu_util_percen
-00000ea0: 745f 5453 5f31 5f76 735f 5453 5f32 5f28  t_TS_1_vs_TS_2_(
-00000eb0: 6772 6f75 7065 645f 6279 5f35 305f 6d69  grouped_by_50_mi
-00000ec0: 6e75 7465 7329 2e70 6e67 3f72 6177 3d74  nutes).png?raw=t
-00000ed0: 7275 6522 2061 6c74 3d22 4465 6c74 6120  rue" alt="Delta 
-00000ee0: 4669 6775 7265 2066 6f72 2075 7365 6420  Figure for used 
-00000ef0: 4350 5520 7065 7263 656e 7461 6765 2067  CPU percentage g
-00000f00: 726f 7570 6564 2062 7920 3530 206d 696e  rouped by 50 min
-00000f10: 7574 6573 223e 0a20 2020 203c 2f64 6976  utes">.    </div
-00000f20: 3e0a 0a2d 2060 7063 6160 3a20 7468 6520  >..- `pca`: the 
-00000f30: 6c69 6e65 6172 2064 696d 656e 7369 6f6e  linear dimension
-00000f40: 616c 6974 7920 7265 6475 6374 696f 6e20  ality reduction 
-00000f50: 7465 6368 6e69 7175 6520 7468 6174 2061  technique that a
-00000f60: 696d 7320 746f 2066 696e 6420 7468 6520  ims to find the 
-00000f70: 7072 696e 6369 7061 6c20 636f 6d70 6f6e  principal compon
-00000f80: 656e 7473 206f 6620 6120 6461 7461 2073  ents of a data s
-00000f90: 6574 2062 790a 2020 636f 6d70 7574 696e  et by.  computin
-00000fa0: 6720 7468 6520 6c69 6e65 6172 2063 6f6d  g the linear com
-00000fb0: 6269 6e61 7469 6f6e 7320 6f66 2074 6865  binations of the
-00000fc0: 206f 7269 6769 6e61 6c20 6368 6172 6163   original charac
-00000fd0: 7465 7269 7374 6963 7320 7468 6174 2065  teristics that e
-00000fe0: 7870 6c61 696e 2074 6865 206d 6f73 7420  xplain the most 
-00000ff0: 7661 7269 616e 6365 2069 6e20 7468 6520  variance in the 
-00001000: 6461 7461 2e0a 2020 2020 3c64 6976 2061  data..    <div a
-00001010: 6c69 676e 3d22 6365 6e74 6572 223e 0a20  lign="center">. 
-00001020: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
-00001030: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001040: 616c 656a 616e 6472 6f66 6465 7a2d 7573  alejandrofdez-us
-00001050: 2f73 696d 696c 6172 6974 792d 7473 2f62  /similarity-ts/b
-00001060: 6c6f 622f 6535 6231 3437 6231 3435 3937  lob/e5b147b14597
-00001070: 3066 3361 3933 3335 3161 3130 3034 3032  0f3a93351a100402
-00001080: 3266 6233 3064 3230 6635 6630 2f64 6f63  2fb30d20f5f0/doc
-00001090: 732f 6669 6775 7265 732f 5043 412e 706e  s/figures/PCA.pn
-000010a0: 673f 7261 773d 7472 7565 2220 616c 743d  g?raw=true" alt=
-000010b0: 2250 4341 2046 6967 7572 6522 2077 6964  "PCA Figure" wid
-000010c0: 7468 3d22 3435 3022 3e0a 2020 2020 3c2f  th="450">.    </
-000010d0: 6469 763e 0a2d 2060 7473 6e65 603a 2061  div>.- `tsne`: a
-000010e0: 2074 6f6f 6c20 666f 7220 7669 7375 616c   tool for visual
-000010f0: 6973 696e 6720 6869 6768 2d64 696d 656e  ising high-dimen
-00001100: 7369 6f6e 616c 2064 6174 6120 7365 7473  sional data sets
-00001110: 2069 6e20 6120 3244 206f 7220 3344 2067   in a 2D or 3D g
-00001120: 7261 7068 6963 616c 2072 6570 7265 7365  raphical represe
-00001130: 6e74 6174 696f 6e20 616c 6c6f 7769 6e67  ntation allowing
-00001140: 2074 6865 2063 7265 6174 696f 6e0a 2020   the creation.  
-00001150: 6f66 2061 2073 696e 676c 6520 6d61 7020  of a single map 
-00001160: 7468 6174 2072 6576 6561 6c73 2074 6865  that reveals the
-00001170: 2073 7472 7563 7475 7265 206f 6620 7468   structure of th
-00001180: 6520 6461 7461 2061 7420 6d61 6e79 2064  e data at many d
-00001190: 6966 6665 7265 6e74 2073 6361 6c65 732e  ifferent scales.
-000011a0: 0a20 2020 203c 6469 7620 616c 6967 6e3d  .    <div align=
-000011b0: 2263 656e 7465 7222 3e0a 2020 2020 3c69  "center">.    <i
-000011c0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-000011d0: 6769 7468 7562 2e63 6f6d 2f61 6c65 6a61  github.com/aleja
-000011e0: 6e64 726f 6664 657a 2d75 732f 7369 6d69  ndrofdez-us/simi
-000011f0: 6c61 7269 7479 2d74 732f 626c 6f62 2f65  larity-ts/blob/e
-00001200: 3562 3134 3762 3134 3539 3730 6633 6139  5b147b145970f3a9
-00001210: 3333 3531 6131 3030 3430 3232 6662 3330  3351a1004022fb30
-00001220: 6432 3066 3566 302f 646f 6373 2f66 6967  d20f5f0/docs/fig
-00001230: 7572 6573 2f74 2d53 4e45 2d69 7465 725f  ures/t-SNE-iter_
-00001240: 3330 302d 7065 7270 6c65 7869 7479 5f35  300-perplexity_5
-00001250: 2e70 6e67 3f72 6177 3d74 7275 6522 2061  .png?raw=true" a
-00001260: 6c74 3d22 5453 4e45 2046 6967 7572 6520  lt="TSNE Figure 
-00001270: 3330 3020 6974 6572 6174 696f 6e73 2035  300 iterations 5
-00001280: 2070 6572 706c 6578 6974 7922 2077 6964   perplexity" wid
-00001290: 7468 3d22 3435 3022 3e0a 2020 2020 3c69  th="450">.    <i
-000012a0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-000012b0: 6769 7468 7562 2e63 6f6d 2f61 6c65 6a61  github.com/aleja
-000012c0: 6e64 726f 6664 657a 2d75 732f 7369 6d69  ndrofdez-us/simi
-000012d0: 6c61 7269 7479 2d74 732f 626c 6f62 2f65  larity-ts/blob/e
-000012e0: 3562 3134 3762 3134 3539 3730 6633 6139  5b147b145970f3a9
-000012f0: 3333 3531 6131 3030 3430 3232 6662 3330  3351a1004022fb30
-00001300: 6432 3066 3566 302f 646f 6373 2f66 6967  d20f5f0/docs/fig
-00001310: 7572 6573 2f74 2d53 4e45 2d69 7465 725f  ures/t-SNE-iter_
-00001320: 3130 3030 2d70 6572 706c 6578 6974 795f  1000-perplexity_
-00001330: 352e 706e 673f 7261 773d 7472 7565 2220  5.png?raw=true" 
-00001340: 616c 743d 2254 534e 4520 4669 6775 7265  alt="TSNE Figure
-00001350: 2031 3030 3020 6974 6572 6174 696f 6e73   1000 iterations
-00001360: 2035 2070 6572 706c 6578 6974 7922 2077   5 perplexity" w
-00001370: 6964 7468 3d22 3435 3022 3e0a 2020 2020  idth="450">.    
-00001380: 3c2f 6469 763e 0a2d 2060 6474 7760 2070  </div>.- `dtw` p
-00001390: 6174 683a 2049 6e20 6164 6469 7469 6f6e  ath: In addition
-000013a0: 2074 6f20 7468 6520 6e75 6d65 7269 6361   to the numerica
-000013b0: 6c20 7369 6d69 6c61 7269 7479 206d 6561  l similarity mea
-000013c0: 7375 7265 2c20 7468 6520 6772 6170 6869  sure, the graphi
-000013d0: 6361 6c20 7265 7072 6573 656e 7461 7469  cal representati
-000013e0: 6f6e 206f 6620 7468 6520 4454 5720 7061  on of the DTW pa
-000013f0: 7468 206f 6620 6561 6368 0a20 2063 6f6c  th of each.  col
-00001400: 756d 6e20 6361 6e20 6265 2075 7365 6675  umn can be usefu
-00001410: 6c20 746f 2062 6574 7465 7220 616e 616c  l to better anal
-00001420: 7973 6520 7468 6520 7369 6d69 6c61 7269  yse the similari
-00001430: 7469 6573 206f 7220 6469 6666 6572 656e  ties or differen
-00001440: 6365 7320 6265 7477 6565 6e20 7468 6520  ces between the 
-00001450: 7469 6d65 2073 6572 6965 7320 636f 6c75  time series colu
-00001460: 6d6e 732e 204e 6f74 6963 6520 7468 6174  mns. Notice that
-00001470: 0a20 2074 6865 7265 2069 7320 6e6f 206d  .  there is no m
-00001480: 756c 7469 7661 7269 6174 6520 7265 7072  ultivariate repr
-00001490: 6573 656e 7461 7469 6f6e 206f 6620 4454  esentation of DT
-000014a0: 5720 7061 7468 732c 206f 6e6c 7920 7369  W paths, only si
-000014b0: 6e67 6c65 2063 6f6c 756d 6e20 7265 7072  ngle column repr
-000014c0: 6573 656e 7461 7469 6f6e 732e 0a20 2020  esentations..   
-000014d0: 203c 6469 763e 0a20 2020 203c 696d 6720   <div>.    <img 
-000014e0: 7372 633d 2268 7474 7073 3a2f 2f67 6974  src="https://git
-000014f0: 6875 622e 636f 6d2f 616c 656a 616e 6472  hub.com/alejandr
-00001500: 6f66 6465 7a2d 7573 2f73 696d 696c 6172  ofdez-us/similar
-00001510: 6974 792d 7473 2f62 6c6f 622f 6535 6231  ity-ts/blob/e5b1
-00001520: 3437 6231 3435 3937 3066 3361 3933 3335  47b145970f3a9335
-00001530: 3161 3130 3034 3032 3266 6233 3064 3230  1a1004022fb30d20
-00001540: 6635 6630 2f64 6f63 732f 6669 6775 7265  f5f0/docs/figure
-00001550: 732f 4454 575f 7361 6d70 6c65 5f33 5f63  s/DTW_sample_3_c
-00001560: 7075 5f75 7469 6c5f 7065 7263 656e 742e  pu_util_percent.
-00001570: 706e 673f 7261 773d 7472 7565 2220 616c  png?raw=true" al
-00001580: 743d 2244 5457 2046 6967 7572 6520 666f  t="DTW Figure fo
-00001590: 7220 6370 7522 3e0a 2020 2020 3c2f 6469  r cpu">.    </di
-000015a0: 763e 0a0a 2323 2049 6e73 7461 6c6c 6174  v>..## Installat
-000015b0: 696f 6e0a 0a54 6f20 696e 7374 616c 6c20  ion..To install 
-000015c0: 7468 6520 746f 6f6c 2069 6e20 796f 7572  the tool in your
-000015d0: 206c 6f63 616c 2065 6e76 6972 6f6e 6d65   local environme
-000015e0: 6e74 2c20 6a75 7374 2072 756e 2066 6f6c  nt, just run fol
-000015f0: 6c6f 7720 636f 6d6d 616e 643a 0a0a 6060  low command:..``
-00001600: 6042 6173 680a 7069 7020 696e 7374 616c  `Bash.pip instal
-00001610: 6c20 7369 6d69 6c61 7269 7479 2d74 732d  l similarity-ts-
-00001620: 636c 6920 0a60 6060 0a0a 2323 2055 7361  cli .```..## Usa
-00001630: 6765 0a0a 5573 6572 7320 6d75 7374 2070  ge..Users must p
-00001640: 726f 7669 6465 2060 2e63 7376 6020 6669  rovide `.csv` fi
-00001650: 6c65 7320 636f 6e74 6169 6e69 6e67 206d  les containing m
-00001660: 756c 7469 7661 7269 6174 6520 7469 6d65  ultivariate time
-00001670: 2073 6572 6965 7320 6279 2075 7369 6e67   series by using
-00001680: 2074 6865 2061 7267 756d 656e 7473 2060   the arguments `
-00001690: 2d74 7331 6020 616e 6420 602d 7473 3260  -ts1` and `-ts2`
-000016a0: 2e0a 0a2d 2060 2d74 7331 6020 7368 6f75  ...- `-ts1` shou
-000016b0: 6c64 2070 6f69 6e74 2074 6f20 6120 7369  ld point to a si
-000016c0: 6e67 6c65 2060 6373 7660 2066 696c 656e  ngle `csv` filen
-000016d0: 616d 652e 2054 6869 7320 7469 6d65 2073  ame. This time s
-000016e0: 6572 6965 7320 6d61 7920 7265 7072 6573  eries may repres
-000016f0: 656e 7420 7468 6520 6261 7365 6c69 6e65  ent the baseline
-00001700: 206f 7220 6772 6f75 6e64 2074 7275 7468   or ground truth
-00001710: 2074 696d 650a 2020 7365 7269 6573 2e0a   time.  series..
-00001720: 2d20 602d 7473 3260 2063 616e 2070 6f69  - `-ts2` can poi
-00001730: 6e74 2074 6f20 616e 6f74 6865 7220 7369  nt to another si
-00001740: 6e67 6c65 2060 6373 7660 2066 696c 656e  ngle `csv` filen
-00001750: 616d 6520 6f72 2061 2064 6972 6563 746f  ame or a directo
-00001760: 7279 2074 6861 7420 636f 6e74 6169 6e73  ry that contains
-00001770: 206d 756c 7469 706c 6520 6063 7376 6020   multiple `csv` 
-00001780: 6669 6c65 7320 746f 2062 650a 2020 636f  files to be.  co
-00001790: 6d70 6172 6564 2077 6974 6820 602d 7473  mpared with `-ts
-000017a0: 3160 2066 696c 652e 0a2d 2060 2d68 6561  1` file..- `-hea
-000017b0: 6460 2069 6620 796f 7572 2074 696d 6520  d` if your time 
-000017c0: 7365 7269 6573 2066 696c 6573 2069 6e63  series files inc
-000017d0: 6c75 6465 2061 2068 6561 6465 7220 7468  lude a header th
-000017e0: 6973 2061 7267 756d 656e 7420 6d75 7374  is argument must
-000017f0: 2062 6520 7072 6573 656e 742e 2049 6620   be present. If 
-00001800: 6e6f 7420 7072 6573 656e 742c 2074 6865  not present, the
-00001810: 2073 6f66 7477 6172 650a 2020 756e 6465   software.  unde
-00001820: 7273 7461 6e64 7320 7468 6174 2063 7376  rstands that csv
-00001830: 2066 696c 6573 2064 6f6e 2774 2069 6e63   files don't inc
-00001840: 6c75 6465 2061 2068 6561 6465 7220 726f  lude a header ro
-00001850: 772e 0a0a 436f 6e73 7472 6169 6e74 733a  w...Constraints:
-00001860: 0a0a 2d20 602d 7473 3160 2074 696d 652d  ..- `-ts1` time-
-00001870: 7365 7269 6573 2066 696c 6520 616e 6420  series file and 
-00001880: 602d 7473 3260 2074 696d 652d 7365 7269  `-ts2` time-seri
-00001890: 6573 2066 696c 6528 7329 206d 7573 743a  es file(s) must:
-000018a0: 0a20 2020 202d 2068 6176 6520 7468 6520  .    - have the 
-000018b0: 7361 6d65 2064 696d 656e 7369 6f6e 616c  same dimensional
-000018c0: 6974 7920 286e 756d 6265 7220 6f66 2063  ity (number of c
-000018d0: 6f6c 756d 6e73 290a 2020 2020 2d20 6e6f  olumns).    - no
-000018e0: 7420 696e 636c 7564 6520 6120 7469 6d65  t include a time
-000018f0: 7374 616d 7020 636f 6c75 6d6e 0a20 2020  stamp column.   
-00001900: 202d 2069 6e63 6c75 6465 206f 6e6c 7920   - include only 
-00001910: 6e75 6d65 7269 6320 7661 6c75 6573 0a20  numeric values. 
-00001920: 2020 202d 2069 6e63 6c75 6465 2074 6865     - include the
-00001930: 2073 616d 6520 6865 6164 6572 2028 6966   same header (if
-00001940: 2070 7265 7365 6e74 290a 2d20 6966 2061   present).- if a
-00001950: 2068 6561 6465 7220 6973 2070 7265 7365   header is prese
-00001960: 6e74 2061 7320 6669 7273 7420 726f 772c  nt as first row,
-00001970: 2075 7365 2074 6865 2060 2d68 6561 6460   use the `-head`
-00001980: 2061 7267 756d 656e 740a 2d20 616c 6c20   argument.- all 
-00001990: 602d 7473 3260 2074 696d 652d 7365 7269  `-ts2` time-seri
-000019a0: 6573 2066 696c 6573 206d 7573 7420 6861  es files must ha
-000019b0: 7665 2074 6865 2073 616d 6520 6c65 6e67  ve the same leng
-000019c0: 7468 2028 6e75 6d62 6572 206f 6620 726f  th (number of ro
-000019d0: 7773 292e 0a0a 4e6f 7465 3a20 7468 6520  ws)...Note: the 
-000019e0: 636f 6c75 6d6e 2064 656c 696d 6974 6572  column delimiter
-000019f0: 2069 7320 6175 746f 6d61 7469 6361 6c6c   is automaticall
-00001a00: 7920 6465 7465 6374 6564 2e0a 0a49 6620  y detected...If 
-00001a10: 602d 7473 3160 2074 696d 652d 7365 7269  `-ts1` time-seri
-00001a20: 6573 2066 696c 6520 6973 206c 6f6e 6765  es file is longe
-00001a30: 7220 286d 6f72 6520 726f 7773 2920 7468  r (more rows) th
-00001a40: 616e 2060 2d74 7332 6020 7469 6d65 2d73  an `-ts2` time-s
-00001a50: 6572 6965 7320 6669 6c65 2873 292c 2074  eries file(s), t
-00001a60: 6865 2060 2d74 7331 6020 7469 6d65 2073  he `-ts1` time s
-00001a70: 6572 6965 7320 7769 6c6c 2062 650a 6469  eries will be.di
-00001a80: 7669 6465 6420 696e 2077 696e 646f 7773  vided in windows
-00001a90: 206f 6620 7468 6520 7361 6d65 0a6c 656e   of the same.len
-00001aa0: 6774 6820 6173 2074 6865 2060 2d74 7332  gth as the `-ts2
-00001ab0: 6020 7469 6d65 2d73 6572 6965 7320 6669  ` time-series fi
-00001ac0: 6c65 2873 292e 0a0a 466f 7220 6561 6368  le(s)...For each
-00001ad0: 2060 2d74 7332 6020 7469 6d65 2d73 6572   `-ts2` time-ser
-00001ae0: 6965 7320 6669 6c65 2c20 7468 6520 6d6f  ies file, the mo
-00001af0: 7374 2073 696d 696c 6172 2077 696e 646f  st similar windo
-00001b00: 7720 282a 2920 6672 6f6d 2060 2d74 7331  w (*) from `-ts1
-00001b10: 6020 7469 6d65 2073 6572 6965 7320 6973  ` time series is
-00001b20: 2073 656c 6563 7465 642e 0a0a 4669 6e61   selected...Fina
-00001b30: 6c6c 792c 206d 6574 7269 6373 2061 6e64  lly, metrics and
-00001b40: 2066 6967 7572 6573 2074 6861 7420 6173   figures that as
-00001b50: 7365 7373 2074 6865 2073 696d 696c 6172  sess the similar
-00001b60: 6974 7920 6265 7477 6565 6e20 6561 6368  ity between each
-00001b70: 2070 6169 7220 6f66 2060 2d74 7332 6020   pair of `-ts2` 
-00001b80: 7469 6d65 2d73 6572 6965 7320 6669 6c65  time-series file
-00001b90: 2061 6e64 2069 7473 0a61 7373 6f63 6961   and its.associa
-00001ba0: 7465 6420 6d6f 7374 2073 696d 696c 6172  ted most similar
-00001bb0: 2060 2d74 7331 6020 7769 6e64 6f77 2061   `-ts1` window a
-00001bc0: 7265 2063 6f6d 7075 7465 642e 0a0a 282a  re computed...(*
-00001bd0: 2920 602d 775f 7365 6c65 6374 5f6d 6574  ) `-w_select_met
-00001be0: 6020 6973 2074 6865 206d 6574 7269 6320  ` is the metric 
-00001bf0: 7573 6564 2066 6f72 2074 6865 2073 656c  used for the sel
-00001c00: 6563 7469 6f6e 206f 6620 7468 6520 6d6f  ection of the mo
-00001c10: 7374 0a73 696d 696c 6172 2060 2d74 7331  st.similar `-ts1
-00001c20: 6020 7469 6d65 2d73 6572 6965 7320 7769  ` time-series wi
-00001c30: 6e64 6f77 2070 6572 2065 6163 6820 602d  ndow per each `-
-00001c40: 7473 3260 2074 696d 652d 7365 7269 6573  ts2` time-series
-00001c50: 2066 696c 6528 7329 2e60 6474 7760 2069   file(s).`dtw` i
-00001c60: 7320 7468 6520 6465 6661 756c 7420 7661  s the default va
-00001c70: 6c75 652c 2068 6f77 6576 6572 2c20 616e  lue, however, an
-00001c80: 7920 6f66 0a74 6865 0a5b 6d65 7472 6963  y of.the.[metric
-00001c90: 735d 2823 6176 6169 6c61 626c 652d 6d65  s](#available-me
-00001ca0: 7472 6963 7329 2061 7265 2061 6c73 6f20  trics) are also 
-00001cb0: 6176 6169 6c61 626c 6520 666f 7220 7468  available for th
-00001cc0: 6973 2070 7572 706f 7365 2075 7369 6e67  is purpose using
-00001cd0: 2074 6869 7320 6172 6775 6d65 6e74 2e0a   this argument..
-00001ce0: 0a55 7365 7273 2063 616e 2070 726f 7669  .Users can provi
-00001cf0: 6465 206d 6574 7269 6373 206f 7220 6669  de metrics or fi
-00001d00: 6775 7265 7320 746f 2062 6520 636f 6d70  gures to be comp
-00001d10: 7574 6564 2f67 656e 6572 6174 6564 3a0a  uted/generated:.
-00001d20: 0a2d 2060 2d6d 6020 7468 6520 5b6d 6574  .- `-m` the [met
-00001d30: 7269 6373 5d28 2361 7661 696c 6162 6c65  rics](#available
-00001d40: 2d6d 6574 7269 6373 2920 6e61 6d65 7320  -metrics) names 
-00001d50: 746f 2062 6520 636f 6d70 7574 6564 2061  to be computed a
-00001d60: 7320 6120 6c69 7374 2073 6570 6172 6174  s a list separat
-00001d70: 6564 2062 7920 7370 6163 6573 2e0a 2d20  ed by spaces..- 
-00001d80: 602d 6660 2074 6865 205b 6669 6775 7265  `-f` the [figure
-00001d90: 735d 2823 6176 6169 6c61 626c 652d 6669  s](#available-fi
-00001da0: 6775 7265 7329 206e 616d 6573 2074 6f20  gures) names to 
-00001db0: 6265 2063 6f6d 7075 7465 6420 6173 2061  be computed as a
-00001dc0: 206c 6973 7420 7365 7061 7261 7465 6420   list separated 
-00001dd0: 6279 2073 7061 6365 730a 0a49 6620 6e6f  by spaces..If no
-00001de0: 206d 6574 7269 6373 206e 6f72 2066 6967   metrics nor fig
-00001df0: 7572 6573 2061 7265 2070 726f 7669 6465  ures are provide
-00001e00: 642c 2074 6865 2074 6f6f 6c20 7769 6c6c  d, the tool will
-00001e10: 2063 6f6d 7075 7465 2061 6c6c 2074 6865   compute all the
-00001e20: 2061 7661 696c 6162 6c65 206d 6574 7269   available metri
-00001e30: 6373 2061 6e64 2066 6967 7572 6573 2e0a  cs and figures..
-00001e40: 0a54 6865 2066 6f6c 6c6f 7769 6e67 2061  .The following a
-00001e50: 7267 756d 656e 7473 2061 7265 2061 6c73  rguments are als
-00001e60: 6f20 6176 6169 6c61 626c 6520 666f 7220  o available for 
-00001e70: 6669 6e65 2d74 756e 696e 673a 0a0a 2d20  fine-tuning:..- 
-00001e80: 602d 7473 5f66 7265 715f 7365 6373 6020  `-ts_freq_secs` 
-00001e90: 7468 6520 6672 6571 7565 6e63 7920 696e  the frequency in
-00001ea0: 2073 6563 6f6e 6473 2069 6e20 7768 6963   seconds in whic
-00001eb0: 6820 7361 6d70 6c65 7320 7765 7265 2074  h samples were t
-00001ec0: 616b 656e 206a 7573 7420 746f 2067 656e  aken just to gen
-00001ed0: 6572 6174 6520 7468 6520 6465 6c74 6120  erate the delta 
-00001ee0: 6669 6775 7265 732e 2042 7920 6465 6661  figures. By defa
-00001ef0: 756c 7420 6973 0a20 2060 3160 2073 6563  ult is.  `1` sec
-00001f00: 6f6e 642e 0a2d 2060 2d73 7472 6460 2077  ond..- `-strd` w
-00001f10: 6865 6e20 6074 7331 6020 7469 6d65 2d73  hen `ts1` time-s
-00001f20: 6572 6965 7320 6973 206c 6f6e 6765 7220  eries is longer 
-00001f30: 7468 616e 2060 7473 3260 2074 696d 652d  than `ts2` time-
-00001f40: 7365 7269 6573 2066 696c 6528 7329 2074  series file(s) t
-00001f50: 6865 2077 696e 646f 7773 2061 7265 2063  he windows are c
-00001f60: 6f6d 7075 7465 6420 6279 2075 7369 6e67  omputed by using
-00001f70: 2061 0a20 2073 7472 6964 6520 6f66 2060   a.  stride of `
-00001f80: 3160 2062 7920 6465 6661 756c 742e 2053  1` by default. S
-00001f90: 6f6d 6574 696d 6573 2075 7369 6e67 2061  ometimes using a
-00001fa0: 206c 6172 6765 7220 7661 6c75 6520 666f   larger value fo
-00001fb0: 7220 7468 6520 7374 7269 6465 2070 6172  r the stride par
-00001fc0: 616d 6574 6572 2069 6d70 726f 7665 7320  ameter improves 
-00001fd0: 7468 6520 7065 7266 6f72 6d61 6e63 6520  the performance 
-00001fe0: 6279 2073 6b69 7070 696e 670a 2020 7468  by skipping.  th
-00001ff0: 6520 636f 6d70 7574 6174 696f 6e20 6f66  e computation of
-00002000: 2073 696d 696c 6172 6974 7920 6265 7477   similarity betw
-00002010: 6565 6e20 736f 206d 616e 7920 7769 6e64  een so many wind
-00002020: 6f77 732e 0a0a 2323 2320 4261 7369 6320  ows...### Basic 
-00002030: 7573 6167 6520 6578 616d 706c 6573 3a0a  usage examples:.
-00002040: 0a53 6f6d 6520 6578 616d 706c 6573 206f  .Some examples o
-00002050: 6620 6576 616c 7561 7469 6f6e 206f 6620  f evaluation of 
-00002060: 7369 6d69 6c61 7269 7479 2061 7265 2073  similarity are s
-00002070: 686f 776e 2062 656c 6f77 2e20 596f 7520  hown below. You 
-00002080: 6361 6e20 646f 776e 6c6f 6164 2073 6f6d  can download som
-00002090: 6520 7465 7374 2064 6174 6120 6279 2072  e test data by r
-000020a0: 756e 6e69 6e67 2074 6865 2066 6f6c 6c6f  unning the follo
-000020b0: 7769 6e67 2063 6f6d 6d61 6e64 3a0a 0a60  wing command:..`
-000020c0: 6060 4261 7368 0a77 6765 7420 6874 7470  ``Bash.wget http
-000020d0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f61  s://github.com/a
-000020e0: 6c65 6a61 6e64 726f 6664 657a 2d75 732f  lejandrofdez-us/
-000020f0: 7369 6d69 6c61 7269 7479 2d74 732d 636c  similarity-ts-cl
-00002100: 692f 7261 772f 6d61 696e 2f64 6174 615f  i/raw/main/data_
-00002110: 7361 6d70 6c65 732e 7a69 7020 2626 2075  samples.zip && u
-00002120: 6e7a 6970 2064 6174 615f 7361 6d70 6c65  nzip data_sample
-00002130: 732e 7a69 700a 6060 600a 4f72 206d 616e  s.zip.```.Or man
-00002140: 7561 6c6c 7920 646f 776e 6c6f 6164 2061  ually download a
-00002150: 6e64 2075 6e7a 6970 2066 726f 6d20 6874  nd unzip from ht
-00002160: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00002170: 2f61 6c65 6a61 6e64 726f 6664 657a 2d75  /alejandrofdez-u
-00002180: 732f 7369 6d69 6c61 7269 7479 2d74 732d  s/similarity-ts-
-00002190: 636c 692f 7261 772f 6d61 696e 2f64 6174  cli/raw/main/dat
-000021a0: 615f 7361 6d70 6c65 732e 7a69 7020 2e0a  a_samples.zip ..
-000021b0: 0a31 2e20 4120 7469 6d65 2073 6572 6965  .1. A time serie
-000021c0: 7320 616e 6420 616c 6c20 7469 6d65 2073  s and all time s
-000021d0: 6572 6965 7320 636f 6d70 7574 696e 6720  eries computing 
-000021e0: 616c 6c20 6d65 7472 6963 7320 616e 6420  all metrics and 
-000021f0: 6669 6775 7265 733a 0a20 2020 2060 6060  figures:.    ```
-00002200: 4261 7368 0a20 2020 2073 696d 696c 6172  Bash.    similar
-00002210: 6974 792d 7473 2d63 6c69 202d 7473 3120  ity-ts-cli -ts1 
-00002220: 6461 7461 5f73 616d 706c 6573 2f61 6c69  data_samples/ali
-00002230: 6261 6261 3230 3138 2f74 7331 5f6d 6163  baba2018/ts1_mac
-00002240: 6869 6e65 5f75 7361 6765 5f64 6179 735f  hine_usage_days_
-00002250: 315f 746f 5f38 5f67 726f 7570 6564 5f33  1_to_8_grouped_3
-00002260: 3030 5f73 6563 6f6e 6473 2e63 7376 202d  00_seconds.csv -
-00002270: 7473 3220 6461 7461 5f73 616d 706c 6573  ts2 data_samples
-00002280: 2f61 6c69 6261 6261 3230 3138 2f74 7332  /alibaba2018/ts2
-00002290: 202d 6865 6164 0a20 2020 2060 6060 0a20   -head.    ```. 
-000022a0: 2020 4576 6572 7920 6d65 7472 6963 2063    Every metric c
-000022b0: 6f6d 7075 7461 7469 6f6e 2061 6e64 2066  omputation and f
-000022c0: 6967 7572 6520 6765 6e65 7261 7465 6420  igure generated 
-000022d0: 7769 6c6c 2062 6520 666f 756e 6420 696e  will be found in
-000022e0: 2074 6865 2060 7265 7375 6c74 732f 7b74   the `results/{t
-000022f0: 696d 6573 7461 6d70 7d2f 6020 6469 7265  imestamp}/` dire
-00002300: 6374 6f72 792e 0a0a 312e 2054 776f 2074  ctory...1. Two t
-00002310: 696d 6520 7365 7269 6573 2063 6f6d 7075  ime series compu
-00002320: 7469 6e67 206f 6e6c 7920 4454 5720 6d65  ting only DTW me
-00002330: 7472 6963 2061 6e64 2044 5457 2066 6967  tric and DTW fig
-00002340: 7572 653a 0a20 2020 2060 6060 4261 7368  ure:.    ```Bash
-00002350: 0a20 2020 2073 696d 696c 6172 6974 792d  .    similarity-
-00002360: 7473 2d63 6c69 202d 7473 3120 6461 7461  ts-cli -ts1 data
-00002370: 5f73 616d 706c 6573 2f61 6c69 6261 6261  _samples/alibaba
-00002380: 3230 3138 2f74 7331 5f6d 6163 6869 6e65  2018/ts1_machine
-00002390: 5f75 7361 6765 5f64 6179 735f 315f 746f  _usage_days_1_to
-000023a0: 5f38 5f67 726f 7570 6564 5f33 3030 5f73  _8_grouped_300_s
-000023b0: 6563 6f6e 6473 2e63 7376 202d 7473 3220  econds.csv -ts2 
-000023c0: 6461 7461 5f73 616d 706c 6573 2f61 6c69  data_samples/ali
-000023d0: 6261 6261 3230 3138 2f74 7332 2f73 616d  baba2018/ts2/sam
-000023e0: 706c 655f 302e 6373 7620 2d68 6561 6420  ple_0.csv -head 
-000023f0: 2d6d 2064 7477 202d 6620 6474 770a 2020  -m dtw -f dtw.  
-00002400: 2020 6060 600a 0a31 2e20 5477 6f20 7469    ```..1. Two ti
-00002410: 6d65 2073 6572 6965 7320 636f 6d70 7574  me series comput
-00002420: 696e 6720 6f6e 6c79 2044 5457 206d 6574  ing only DTW met
-00002430: 7269 6320 616e 6420 4454 5720 6669 6775  ric and DTW figu
-00002440: 7265 3a0a 2020 2020 6060 6042 6173 680a  re:.    ```Bash.
-00002450: 2020 2020 7369 6d69 6c61 7269 7479 2d74      similarity-t
-00002460: 732d 636c 6920 2d74 7331 2064 6174 615f  s-cli -ts1 data_
-00002470: 7361 6d70 6c65 732f 616c 6962 6162 6132  samples/alibaba2
-00002480: 3031 382f 7473 315f 6d61 6368 696e 655f  018/ts1_machine_
-00002490: 7573 6167 655f 6461 7973 5f31 5f74 6f5f  usage_days_1_to_
-000024a0: 385f 6772 6f75 7065 645f 3330 305f 7365  8_grouped_300_se
-000024b0: 636f 6e64 732e 6373 7620 2d74 7332 2064  conds.csv -ts2 d
-000024c0: 6174 615f 7361 6d70 6c65 732f 616c 6962  ata_samples/alib
-000024d0: 6162 6132 3031 382f 7473 322f 7361 6d70  aba2018/ts2/samp
-000024e0: 6c65 5f30 2e63 7376 202d 6865 6164 202d  le_0.csv -head -
-000024f0: 6d20 6474 7720 2d66 2064 7477 0a20 2020  m dtw -f dtw.   
-00002500: 2060 6060 0a0a 312e 2041 2074 696d 6520   ```..1. A time 
-00002510: 7365 7269 6573 2061 6e64 2061 6c6c 2074  series and all t
-00002520: 696d 6520 7365 7269 6573 2077 6974 6869  ime series withi
-00002530: 6e20 6120 6469 7265 6374 6f72 7920 636f  n a directory co
-00002540: 6d70 7574 696e 6720 6576 6572 7920 6d65  mputing every me
-00002550: 7472 6963 2061 6e64 2066 6967 7572 6520  tric and figure 
-00002560: 696e 2053 696d 696c 6172 6974 7954 5320  in SimilarityTS 
-00002570: 746f 6f6c 6b69 743a 0a20 2020 2060 6060  toolkit:.    ```
-00002580: 4261 7368 0a20 2020 2073 696d 696c 6172  Bash.    similar
-00002590: 6974 792d 7473 2d63 6c69 202d 7473 3120  ity-ts-cli -ts1 
-000025a0: 6461 7461 5f73 616d 706c 6573 2f61 6c69  data_samples/ali
-000025b0: 6261 6261 3230 3138 2f74 7331 5f6d 6163  baba2018/ts1_mac
-000025c0: 6869 6e65 5f75 7361 6765 5f64 6179 735f  hine_usage_days_
-000025d0: 315f 746f 5f38 5f67 726f 7570 6564 5f33  1_to_8_grouped_3
-000025e0: 3030 5f73 6563 6f6e 6473 2e63 7376 202d  00_seconds.csv -
-000025f0: 7473 3220 6461 7461 5f73 616d 706c 6573  ts2 data_samples
-00002600: 2f61 6c69 6261 6261 3230 3138 2f74 7332  /alibaba2018/ts2
-00002610: 202d 6865 6164 202d 6d20 6a73 206d 6d64   -head -m js mmd
-00002620: 2064 7477 206b 7320 6b6c 2063 6320 6370   dtw ks kl cc cp
-00002630: 2068 6920 2d66 2064 656c 7461 2064 7477   hi -f delta dtw
-00002640: 2032 6420 7063 6120 7473 6e65 0a20 2020   2d pca tsne.   
-00002650: 2060 6060 0a0a 312e 2043 6f6d 7061 7269   ```..1. Compari
-00002660: 736f 6e20 6265 7477 6565 6e20 7469 6d65  son between time
-00002670: 2073 6572 6965 7320 7370 6563 6966 7969   series specifyi
-00002680: 6e67 2074 6865 2066 7265 7175 656e 6379  ng the frequency
-00002690: 2069 6e20 7365 636f 6e64 7320 696e 2077   in seconds in w
-000026a0: 6869 6368 2073 616d 706c 6573 2077 6572  hich samples wer
-000026b0: 6520 7461 6b65 6e3a 0a20 2020 2060 6060  e taken:.    ```
-000026c0: 4261 7368 0a20 2020 2073 696d 696c 6172  Bash.    similar
-000026d0: 6974 792d 7473 2d63 6c69 202d 7473 3120  ity-ts-cli -ts1 
-000026e0: 6461 7461 5f73 616d 706c 6573 2f61 6c69  data_samples/ali
-000026f0: 6261 6261 3230 3138 2f74 7331 5f6d 6163  baba2018/ts1_mac
-00002700: 6869 6e65 5f75 7361 6765 5f64 6179 735f  hine_usage_days_
-00002710: 315f 746f 5f38 5f67 726f 7570 6564 5f33  1_to_8_grouped_3
-00002720: 3030 5f73 6563 6f6e 6473 2e63 7376 202d  00_seconds.csv -
-00002730: 7473 3220 6461 7461 5f73 616d 706c 6573  ts2 data_samples
-00002740: 2f61 6c69 6261 6261 3230 3138 2f74 7332  /alibaba2018/ts2
-00002750: 202d 6865 6164 202d 6d20 6474 7720 2d66   -head -m dtw -f
-00002760: 2064 7477 202d 7473 5f66 7265 715f 7365   dtw -ts_freq_se
-00002770: 6373 2033 3030 0a20 2020 2060 6060 0a0a  cs 300.    ```..
-00002780: 312e 2043 6f6d 7061 7269 736f 6e20 6265  1. Comparison be
-00002790: 7477 6565 6e20 7469 6d65 2073 6572 6965  tween time serie
-000027a0: 7320 7370 6563 6966 7969 6e67 2074 6865  s specifying the
-000027b0: 2073 7472 6964 6520 7468 6174 2064 6574   stride that det
-000027c0: 6572 6d69 6e65 7320 7468 6520 7374 6570  ermines the step
-000027d0: 206f 7220 6469 7374 616e 6365 2062 7920   or distance by 
-000027e0: 7768 6963 6820 6120 6669 7865 642d 7369  which a fixed-si
-000027f0: 7a65 0a20 2020 7769 6e64 6f77 206d 6f76  ze.   window mov
-00002800: 6573 206f 7665 7220 7468 6520 6669 7273  es over the firs
-00002810: 7420 7469 6d65 2073 6572 6965 733a 0a20  t time series:. 
-00002820: 2020 2060 6060 4261 7368 0a20 2020 2073     ```Bash.    s
-00002830: 696d 696c 6172 6974 792d 7473 2d63 6c69  imilarity-ts-cli
-00002840: 202d 7473 3120 6461 7461 5f73 616d 706c   -ts1 data_sampl
-00002850: 6573 2f61 6c69 6261 6261 3230 3138 2f74  es/alibaba2018/t
-00002860: 7331 5f6d 6163 6869 6e65 5f75 7361 6765  s1_machine_usage
-00002870: 5f64 6179 735f 315f 746f 5f38 5f67 726f  _days_1_to_8_gro
-00002880: 7570 6564 5f33 3030 5f73 6563 6f6e 6473  uped_300_seconds
-00002890: 2e63 7376 202d 7473 3220 6461 7461 5f73  .csv -ts2 data_s
-000028a0: 616d 706c 6573 2f61 6c69 6261 6261 3230  amples/alibaba20
-000028b0: 3138 2f74 7332 202d 6865 6164 202d 6d20  18/ts2 -head -m 
-000028c0: 6474 7720 2d66 2064 7477 202d 7374 7264  dtw -f dtw -strd
-000028d0: 2035 0a20 2020 2060 6060 0a0a 312e 2043   5.    ```..1. C
-000028e0: 6f6d 7061 7269 736f 6e20 6265 7477 6565  omparison betwee
-000028f0: 6e20 7469 6d65 2073 6572 6965 7320 7370  n time series sp
-00002900: 6563 6966 7969 6e67 2074 6865 2077 696e  ecifying the win
-00002910: 646f 7720 7365 6c65 6374 696f 6e20 6d65  dow selection me
-00002920: 7472 6963 2074 6f20 6265 2075 7365 6420  tric to be used 
-00002930: 7768 656e 2073 656c 6563 7469 6e67 2074  when selecting t
-00002940: 6865 206d 6f73 7420 7369 6d69 6c61 720a  he most similar.
-00002950: 2020 2077 696e 646f 7773 2069 6e0a 2020     windows in.  
-00002960: 2074 6865 2066 6972 7374 2074 696d 6520   the first time 
-00002970: 7365 7269 6573 3a0a 0a20 2020 2060 6060  series:..    ```
-00002980: 4261 7368 0a20 2020 2073 696d 696c 6172  Bash.    similar
-00002990: 6974 792d 7473 2d63 6c69 202d 7473 3120  ity-ts-cli -ts1 
-000029a0: 6461 7461 5f73 616d 706c 6573 2f61 6c69  data_samples/ali
-000029b0: 6261 6261 3230 3138 2f74 7331 5f6d 6163  baba2018/ts1_mac
-000029c0: 6869 6e65 5f75 7361 6765 5f64 6179 735f  hine_usage_days_
-000029d0: 315f 746f 5f38 5f67 726f 7570 6564 5f33  1_to_8_grouped_3
-000029e0: 3030 5f73 6563 6f6e 6473 2e63 7376 202d  00_seconds.csv -
-000029f0: 7473 3220 6461 7461 5f73 616d 706c 6573  ts2 data_samples
-00002a00: 2f61 6c69 6261 6261 3230 3138 2f74 7332  /alibaba2018/ts2
-00002a10: 202d 6865 6164 202d 6d20 6474 7720 2d66   -head -m dtw -f
-00002a20: 2064 7477 202d 775f 7365 6c65 6374 5f6d   dtw -w_select_m
-00002a30: 6574 206a 730a 2020 2020 6060 600a 0a31  et js.    ```..1
-00002a40: 2e20 5573 696e 6720 6f75 7220 7361 6d70  . Using our samp
-00002a50: 6c65 2074 696d 6520 7365 7269 6573 2074  le time series t
-00002a60: 6f20 636f 6d70 7574 6520 6576 6572 7920  o compute every 
-00002a70: 7369 6e67 6c65 206d 6574 7269 6320 616e  single metric an
-00002a80: 6420 6669 6775 7265 2077 6974 6820 6120  d figure with a 
-00002a90: 6669 7865 6420 7469 6d65 7374 616d 7020  fixed timestamp 
-00002aa0: 6672 6571 7565 6e63 7920 616e 6420 7374  frequency and st
-00002ab0: 7269 6465 3a0a 0a20 2020 2060 6060 4261  ride:..    ```Ba
-00002ac0: 7368 0a20 2020 2073 696d 696c 6172 6974  sh.    similarit
-00002ad0: 792d 7473 2d63 6c69 202d 7473 3120 6461  y-ts-cli -ts1 da
-00002ae0: 7461 5f73 616d 706c 6573 2f61 6c69 6261  ta_samples/aliba
-00002af0: 6261 3230 3138 2f74 7331 5f6d 6163 6869  ba2018/ts1_machi
-00002b00: 6e65 5f75 7361 6765 5f64 6179 735f 315f  ne_usage_days_1_
-00002b10: 746f 5f38 5f67 726f 7570 6564 5f33 3030  to_8_grouped_300
-00002b20: 5f73 6563 6f6e 6473 2e63 7376 202d 7473  _seconds.csv -ts
-00002b30: 3220 6461 7461 5f73 616d 706c 6573 2f61  2 data_samples/a
-00002b40: 6c69 6261 6261 3230 3138 2f74 7332 202d  libaba2018/ts2 -
-00002b50: 6865 6164 202d 6d20 6d6d 6420 6474 7720  head -m mmd dtw 
-00002b60: 6b73 206b 6c20 6363 2063 7020 6869 202d  ks kl cc cp hi -
-00002b70: 6620 6465 6c74 6120 6474 7720 3264 2070  f delta dtw 2d p
-00002b80: 6361 2074 736e 6520 2d77 5f73 656c 6563  ca tsne -w_selec
-00002b90: 745f 6d65 7420 6363 202d 7473 5f66 7265  t_met cc -ts_fre
-00002ba0: 715f 7365 6373 2033 3030 202d 7374 7264  q_secs 300 -strd
-00002bb0: 2035 0a20 2020 2060 6060 0a23 2320 4c69   5.    ```.## Li
-00002bc0: 6365 6e73 650a 0a53 696d 696c 6172 6974  cense..Similarit
-00002bd0: 7954 5320 746f 6f6c 6b69 7420 6973 2066  yTS toolkit is f
-00002be0: 7265 6520 616e 6420 6f70 656e 2d73 6f75  ree and open-sou
-00002bf0: 7263 6520 736f 6674 7761 7265 206c 6963  rce software lic
-00002c00: 656e 7365 6420 756e 6465 7220 7468 6520  ensed under the 
-00002c10: 5b4d 4954 206c 6963 656e 7365 5d28 4c49  [MIT license](LI
-00002c20: 4345 4e53 4529 2e                        CENSE).
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 7369 6d69  : 2.1.Name: simi
+00000020: 6c61 7269 7479 2d74 732d 636c 690a 5665  larity-ts-cli.Ve
+00000030: 7273 696f 6e3a 2031 2e30 2e31 0a53 756d  rsion: 1.0.1.Sum
+00000040: 6d61 7279 3a20 5369 6d69 6c61 7269 7479  mary: Similarity
+00000050: 5453 2d63 6c69 2069 7320 616e 206f 7065  TS-cli is an ope
+00000060: 6e2d 736f 7572 6365 2074 6f6f 6c20 6465  n-source tool de
+00000070: 7369 676e 6564 2074 6f20 6661 6369 6c69  signed to facili
+00000080: 7461 7465 2074 6865 2075 7361 6765 206f  tate the usage o
+00000090: 6620 5369 6d69 6c61 7269 7479 5453 2070  f SimilarityTS p
+000000a0: 6163 6b61 6765 2066 726f 6d20 6120 636f  ackage from a co
+000000b0: 6d6d 616e 6420 6c69 6e65 2069 6e74 6572  mmand line inter
+000000c0: 6661 6365 0a41 7574 686f 722d 656d 6169  face.Author-emai
+000000d0: 6c3a 2041 6c65 6a61 6e64 726f 2046 6572  l: Alejandro Fer
+000000e0: 6ec3 a16e 6465 7a2d 4d6f 6e74 6573 203c  n..ndez-Montes <
+000000f0: 6166 6465 7a40 7573 2e65 733e 2c20 4461  afdez@us.es>, Da
+00000100: 6d69 c3a1 6e20 4665 726e c3a1 6e64 657a  mi..n Fern..ndez
+00000110: 2d43 6572 6572 6f20 3c64 616d 6961 6e63  -Cerero <damianc
+00000120: 6572 6572 6f40 7573 2e65 733e 2c20 4665  erero@us.es>, Fe
+00000130: 6c69 7065 2045 7363 616c 6572 6120 476f  lipe Escalera Go
+00000140: 6e7a c3a1 6c65 7a20 3c66 6573 6361 6c65  nz..lez <fescale
+00000150: 7261 4075 732e 6573 3e0a 5072 6f6a 6563  ra@us.es>.Projec
+00000160: 742d 5552 4c3a 2048 6f6d 6570 6167 652c  t-URL: Homepage,
+00000170: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00000180: 636f 6d2f 616c 656a 616e 6472 6f66 6465  com/alejandrofde
+00000190: 7a2d 7573 2f73 696d 696c 6172 6974 792d  z-us/similarity-
+000001a0: 7473 2d63 6c69 0a50 726f 6a65 6374 2d55  ts-cli.Project-U
+000001b0: 524c 3a20 4275 6720 5472 6163 6b65 722c  RL: Bug Tracker,
+000001c0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+000001d0: 636f 6d2f 616c 656a 616e 6472 6f66 6465  com/alejandrofde
+000001e0: 7a2d 7573 2f73 696d 696c 6172 6974 792d  z-us/similarity-
+000001f0: 7473 2d63 6c69 2f69 7373 7565 730a 436c  ts-cli/issues.Cl
+00000200: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+00000210: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000220: 3a20 5079 7468 6f6e 203a 3a20 330a 436c  : Python :: 3.Cl
+00000230: 6173 7369 6669 6572 3a20 4c69 6365 6e73  assifier: Licens
+00000240: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
+00000250: 6420 3a3a 204d 4954 204c 6963 656e 7365  d :: MIT License
+00000260: 0a43 6c61 7373 6966 6965 723a 204f 7065  .Classifier: Ope
+00000270: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
+00000280: 204f 5320 496e 6465 7065 6e64 656e 740a   OS Independent.
+00000290: 5265 7175 6972 6573 2d50 7974 686f 6e3a  Requires-Python:
+000002a0: 203e 3d33 2e39 0a44 6573 6372 6970 7469   >=3.9.Descripti
+000002b0: 6f6e 2d43 6f6e 7465 6e74 2d54 7970 653a  on-Content-Type:
+000002c0: 2074 6578 742f 6d61 726b 646f 776e 0a4c   text/markdown.L
+000002d0: 6963 656e 7365 2d46 696c 653a 204c 4943  icense-File: LIC
+000002e0: 454e 5345 0a0a 5b21 5b76 6572 7369 6f6e  ENSE..[![version
+000002f0: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+00000300: 6965 6c64 732e 696f 2f62 6164 6765 2f70  ields.io/badge/p
+00000310: 7970 692d 312e 302e 312d 626c 7565 295d  ypi-1.0.1-blue)]
+00000320: 2868 7474 7073 3a2f 2f70 7970 692e 6f72  (https://pypi.or
+00000330: 672f 7072 6f6a 6563 742f 7369 6d69 6c61  g/project/simila
+00000340: 7269 7479 2d74 732d 636c 692f 290a 5b21  rity-ts-cli/).[!
+00000350: 5b50 7974 686f 6e20 332e 395d 2868 7474  [Python 3.9](htt
+00000360: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000370: 2e69 6f2f 6261 6467 652f 7079 7468 6f6e  .io/badge/python
+00000380: 2d33 2e39 2d64 6172 6b67 7265 656e 295d  -3.9-darkgreen)]
+00000390: 2868 7474 7073 3a2f 2f77 7777 2e70 7974  (https://www.pyt
+000003a0: 686f 6e2e 6f72 672f 646f 776e 6c6f 6164  hon.org/download
+000003b0: 732f 7265 6c65 6173 652f 7079 7468 6f6e  s/release/python
+000003c0: 2d33 3930 2f29 0a5b 215b 6c61 7374 2d75  -390/).[![last-u
+000003d0: 7064 6174 655d 2868 7474 7073 3a2f 2f69  pdate](https://i
+000003e0: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
+000003f0: 6467 652f 6c61 7374 5f75 7064 6174 652d  dge/last_update-
+00000400: 3037 2f31 382f 3230 3233 2d62 7269 6768  07/18/2023-brigh
+00000410: 7467 7265 656e 295d 2868 7474 7073 3a2f  tgreen)](https:/
+00000420: 2f67 6974 6875 622e 636f 6d2f 616c 656a  /github.com/alej
+00000430: 616e 6472 6f66 6465 7a2d 7573 2f73 696d  androfdez-us/sim
+00000440: 696c 6172 6974 792d 7473 2d63 6c69 2f63  ilarity-ts-cli/c
+00000450: 6f6d 6d69 7473 2f6d 6169 6e29 0a5b 215b  ommits/main).[![
+00000460: 6c69 6365 6e73 655d 2868 7474 7073 3a2f  license](https:/
+00000470: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000480: 6261 6467 652f 6c69 6365 6e73 652d 4d49  badge/license-MI
+00000490: 542d 6f72 616e 6765 295d 284c 4943 454e  T-orange)](LICEN
+000004a0: 5345 290a 0a23 2053 696d 696c 6172 6974  SE)..# Similarit
+000004b0: 7954 532d 636c 693a 2043 6f6d 6d61 6e64  yTS-cli: Command
+000004c0: 2d6c 696e 6520 696e 7465 7266 6163 6520  -line interface 
+000004d0: 666f 7220 5369 6d69 6c61 7269 7479 5453  for SimilarityTS
+000004e0: 2070 6163 6b61 6765 0a0a 2323 2054 6162   package..## Tab
+000004f0: 6c65 206f 6620 436f 6e74 656e 7473 0a0a  le of Contents..
+00000500: 2d20 5b44 6573 6372 6970 7469 6f6e 5d28  - [Description](
+00000510: 2364 6573 6372 6970 7469 6f6e 290a 2d20  #description).- 
+00000520: 5b49 6e73 7461 6c6c 6174 696f 6e5d 2823  [Installation](#
+00000530: 696e 7374 616c 6c61 7469 6f6e 290a 2d20  installation).- 
+00000540: 5b55 7361 6765 5d28 2375 7361 6765 290a  [Usage](#usage).
+00000550: 2d20 5b4c 6963 656e 7365 5d28 236c 6963  - [License](#lic
+00000560: 656e 7365 290a 2d20 5b41 636b 6e6f 776c  ense).- [Acknowl
+00000570: 6564 6765 6d65 6e74 735d 2823 6163 6b6e  edgements](#ackn
+00000580: 6f77 6c65 6467 656d 656e 7473 290a 0a23  owledgements)..#
+00000590: 2320 4465 7363 7269 7074 696f 6e0a 0a53  # Description..S
+000005a0: 696d 696c 6172 6974 7954 532d 636c 6920  imilarityTS-cli 
+000005b0: 6973 2061 2063 6f6d 6d61 6e64 2d6c 696e  is a command-lin
+000005c0: 6520 696e 7465 7266 6163 6520 746f 6f6c  e interface tool
+000005d0: 2074 6861 7420 6163 7420 6173 2061 6e20   that act as an 
+000005e0: 696e 7465 7266 6163 6520 6f66 2074 6865  interface of the
+000005f0: 205b 5369 6d69 6c61 7269 7479 5453 2070   [SimilarityTS p
+00000600: 6163 6b61 6765 5d28 6874 7470 733a 2f2f  ackage](https://
+00000610: 6769 7468 7562 2e63 6f6d 2f61 6c65 6a61  github.com/aleja
+00000620: 6e64 726f 6664 657a 2d75 732f 7369 6d69  ndrofdez-us/simi
+00000630: 6c61 7269 7479 2d74 7329 2e20 5369 6d69  larity-ts). Simi
+00000640: 6c61 7269 7479 2d54 5320 7061 636b 6167  larity-TS packag
+00000650: 6520 6661 6369 6c69 7461 7465 7320 7468  e facilitates th
+00000660: 6520 6576 616c 7561 7469 6f6e 2061 6e64  e evaluation and
+00000670: 2063 6f6d 7061 7269 736f 6e20 6f66 0a6d   comparison of.m
+00000680: 756c 7469 7661 7269 6174 6520 7469 6d65  ultivariate time
+00000690: 2073 6572 6965 7320 6461 7461 2e20 4974   series data. It
+000006a0: 2070 726f 7669 6465 7320 6120 636f 6d70   provides a comp
+000006b0: 7265 6865 6e73 6976 6520 746f 6f6c 6b69  rehensive toolki
+000006c0: 7420 666f 7220 616e 616c 797a 696e 672c  t for analyzing,
+000006d0: 2076 6973 7561 6c69 7a69 6e67 2c20 616e   visualizing, an
+000006e0: 6420 7265 706f 7274 696e 6720 6d75 6c74  d reporting mult
+000006f0: 6970 6c65 0a6d 6574 7269 6373 2061 6e64  iple.metrics and
+00000700: 2066 6967 7572 6573 2064 6572 6976 6564   figures derived
+00000710: 2066 726f 6d20 7469 6d65 2073 6572 6965   from time serie
+00000720: 7320 6461 7461 7365 7473 2e20 5468 6520  s datasets. The 
+00000730: 746f 6f6c 6b69 7420 7369 6d70 6c69 6669  toolkit simplifi
+00000740: 6573 2074 6865 2070 726f 6365 7373 206f  es the process o
+00000750: 6620 6576 616c 7561 7469 6e67 2074 6865  f evaluating the
+00000760: 2073 696d 696c 6172 6974 7920 6f66 0a74   similarity of.t
+00000770: 696d 6520 7365 7269 6573 2062 7920 6f66  ime series by of
+00000780: 6665 7269 6e67 2064 6174 6120 7072 6570  fering data prep
+00000790: 726f 6365 7373 696e 672c 206d 6574 7269  rocessing, metri
+000007a0: 6373 2063 6f6d 7075 7461 7469 6f6e 2c20  cs computation, 
+000007b0: 7669 7375 616c 697a 6174 696f 6e2c 2073  visualization, s
+000007c0: 7461 7469 7374 6963 616c 2061 6e61 6c79  tatistical analy
+000007d0: 7369 732c 2061 6e64 2072 6570 6f72 7420  sis, and report 
+000007e0: 6765 6e65 7261 7469 6f6e 0a66 756e 6374  generation.funct
+000007f0: 696f 6e61 6c69 7469 6573 2e20 5769 7468  ionalities. With
+00000800: 2069 7473 2063 7573 746f 6d69 7a61 626c   its customizabl
+00000810: 6520 6665 6174 7572 6573 2c20 5369 6d69  e features, Simi
+00000820: 6c61 7269 7479 5453 2065 6d70 6f77 6572  larityTS empower
+00000830: 7320 7265 7365 6172 6368 6572 7320 616e  s researchers an
+00000840: 6420 6461 7461 0a73 6369 656e 7469 7374  d data.scientist
+00000850: 7320 746f 2067 6169 6e20 696e 7369 6768  s to gain insigh
+00000860: 7473 2c20 6964 656e 7469 6679 2070 6174  ts, identify pat
+00000870: 7465 726e 732c 2061 6e64 206d 616b 6520  terns, and make 
+00000880: 696e 666f 726d 6564 2064 6563 6973 696f  informed decisio
+00000890: 6e73 2062 6173 6564 206f 6e20 7468 6569  ns based on thei
+000008a0: 7220 7469 6d65 2073 6572 6965 7320 6461  r time series da
+000008b0: 7461 2e0a 0a54 6869 7320 636f 6d6d 616e  ta...This comman
+000008c0: 642d 6c69 6e65 2069 6e74 6572 6661 6365  d-line interface
+000008d0: 2069 7320 4f53 2069 6e64 6570 656e 6465   is OS independe
+000008e0: 6e74 2061 6e64 2063 616e 2062 6520 6561  nt and can be ea
+000008f0: 7369 6c79 2069 6e73 7461 6c6c 6564 2061  sily installed a
+00000900: 6e64 2075 7365 642e 0a0a 2323 2320 4176  nd used...### Av
+00000910: 6169 6c61 626c 6520 6d65 7472 6963 730a  ailable metrics.
+00000920: 0a54 6869 7320 746f 6f6c 6b69 7420 6361  .This toolkit ca
+00000930: 6e20 636f 6d70 7574 6520 7468 6520 666f  n compute the fo
+00000940: 6c6c 6f77 696e 6720 6d65 7472 6963 733a  llowing metrics:
+00000950: 0a0a 2d20 606b 6c60 3a20 4b75 6c6c 6261  ..- `kl`: Kullba
+00000960: 636b 2d4c 6569 626c 6572 2064 6976 6572  ck-Leibler diver
+00000970: 6765 6e63 650a 2d20 606a 7360 3a20 4a65  gence.- `js`: Je
+00000980: 6e73 656e 2d53 6861 6e6e 6f6e 2064 6976  nsen-Shannon div
+00000990: 6572 6765 6e63 650a 2d20 606b 7360 3a20  ergence.- `ks`: 
+000009a0: 4b6f 6c6d 6f67 6f72 6f76 2d53 6d69 726e  Kolmogorov-Smirn
+000009b0: 6f76 2074 6573 740a 2d20 606d 6d64 603a  ov test.- `mmd`:
+000009c0: 204d 6178 696d 756d 204d 6561 6e20 4469   Maximum Mean Di
+000009d0: 7363 7265 7061 6e63 790a 2d20 6064 7477  screpancy.- `dtw
+000009e0: 6020 4479 6e61 6d69 6320 5469 6d65 2057  ` Dynamic Time W
+000009f0: 6172 7069 6e67 0a2d 2060 6363 603a 2044  arping.- `cc`: D
+00000a00: 6966 6665 7265 6e63 6520 6f66 2063 6f2d  ifference of co-
+00000a10: 7661 7269 616e 6365 730a 2d20 6063 7060  variances.- `cp`
+00000a20: 3a20 4469 6666 6572 656e 6365 206f 6620  : Difference of 
+00000a30: 636f 7272 656c 6174 696f 6e73 0a2d 2060  correlations.- `
+00000a40: 6869 603a 2044 6966 6665 7265 6e63 6520  hi`: Difference 
+00000a50: 6f66 2068 6973 746f 6772 616d 730a 0a23  of histograms..#
+00000a60: 2323 2041 7661 696c 6162 6c65 2066 6967  ## Available fig
+00000a70: 7572 6573 0a0a 5468 6973 2074 6f6f 6c6b  ures..This toolk
+00000a80: 6974 2063 616e 2067 656e 6572 6174 6520  it can generate 
+00000a90: 7468 6520 666f 6c6c 6f77 696e 6720 6669  the following fi
+00000aa0: 6775 7265 733a 0a0a 2d20 6032 6460 3a20  gures:..- `2d`: 
+00000ab0: 7468 6520 6f72 6469 6e61 7279 2067 7261  the ordinary gra
+00000ac0: 7068 6963 616c 2072 6570 7265 7365 6e74  phical represent
+00000ad0: 6174 696f 6e20 6f66 2074 6865 2074 696d  ation of the tim
+00000ae0: 6520 7365 7269 6573 2069 6e20 6120 3244  e series in a 2D
+00000af0: 2066 6967 7572 6520 7769 7468 2074 6865   figure with the
+00000b00: 2074 696d 6520 7265 7072 6573 656e 7465   time represente
+00000b10: 6420 6f6e 2074 6865 2078 2061 7869 730a  d on the x axis.
+00000b20: 2020 616e 6420 7468 6520 6461 7461 2076    and the data v
+00000b30: 616c 7565 7320 6f6e 2074 6865 2079 2d61  alues on the y-a
+00000b40: 7869 7320 666f 720a 2020 2020 2d20 7468  xis for.    - th
+00000b50: 6520 636f 6d70 6c65 7465 206d 756c 7469  e complete multi
+00000b60: 7661 7269 6174 6520 7469 6d65 2073 6572  variate time ser
+00000b70: 6965 733b 2061 6e64 0a20 2020 202d 2061  ies; and.    - a
+00000b80: 2070 6c6f 7420 7065 7220 636f 6c75 6d6e   plot per column
+00000b90: 2e0a 0a20 2045 6163 6820 6765 6e65 7261  ...  Each genera
+00000ba0: 7465 6420 6669 6775 7265 2070 6c6f 7473  ted figure plots
+00000bb0: 2062 6f74 6820 7468 6520 6074 7331 6020   both the `ts1` 
+00000bc0: 616e 6420 7468 6520 6074 7332 6020 6461  and the `ts2` da
+00000bd0: 7461 2074 6f20 6561 7369 6c79 206f 6274  ta to easily obt
+00000be0: 6169 6e20 6b65 7920 696e 7369 6768 7473  ain key insights
+00000bf0: 2069 6e74 6f0a 2020 7468 6520 7369 6d69   into.  the simi
+00000c00: 6c61 7269 7469 6573 206f 7220 6469 6666  larities or diff
+00000c10: 6572 656e 6365 7320 6265 7477 6565 6e20  erences between 
+00000c20: 7468 656d 2e0a 2020 2020 3c64 6976 3e0a  them..    <div>.
+00000c30: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
+00000c40: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000c50: 2f61 6c65 6a61 6e64 726f 6664 657a 2d75  /alejandrofdez-u
+00000c60: 732f 7369 6d69 6c61 7269 7479 2d74 732f  s/similarity-ts/
+00000c70: 626c 6f62 2f65 3562 3134 3762 3134 3539  blob/e5b147b1459
+00000c80: 3730 6633 6139 3333 3531 6131 3030 3430  70f3a93351a10040
+00000c90: 3232 6662 3330 6432 3066 3566 302f 646f  22fb30d20f5f0/do
+00000ca0: 6373 2f66 6967 7572 6573 2f32 645f 7361  cs/figures/2d_sa
+00000cb0: 6d70 6c65 5f33 5f63 6f6d 706c 6574 655f  mple_3_complete_
+00000cc0: 5453 5f31 5f76 735f 5453 5f32 2e70 6e67  TS_1_vs_TS_2.png
+00000cd0: 3f72 6177 3d74 7275 6522 2061 6c74 3d22  ?raw=true" alt="
+00000ce0: 3244 2046 6967 7572 6520 636f 6d70 6c65  2D Figure comple
+00000cf0: 7465 223e 0a20 2020 203c 696d 6720 7372  te">.    <img sr
+00000d00: 633d 2268 7474 7073 3a2f 2f67 6974 6875  c="https://githu
+00000d10: 622e 636f 6d2f 616c 656a 616e 6472 6f66  b.com/alejandrof
+00000d20: 6465 7a2d 7573 2f73 696d 696c 6172 6974  dez-us/similarit
+00000d30: 792d 7473 2f62 6c6f 622f 6535 6231 3437  y-ts/blob/e5b147
+00000d40: 6231 3435 3937 3066 3361 3933 3335 3161  b145970f3a93351a
+00000d50: 3130 3034 3032 3266 6233 3064 3230 6635  1004022fb30d20f5
+00000d60: 6630 2f64 6f63 732f 6669 6775 7265 732f  f0/docs/figures/
+00000d70: 3264 5f73 616d 706c 655f 335f 6370 755f  2d_sample_3_cpu_
+00000d80: 7574 696c 5f70 6572 6365 6e74 5f54 535f  util_percent_TS_
+00000d90: 315f 7673 5f54 535f 322e 706e 673f 7261  1_vs_TS_2.png?ra
+00000da0: 773d 7472 7565 2220 616c 743d 2232 4420  w=true" alt="2D 
+00000db0: 4669 6775 7265 2066 6f72 2075 7365 6420  Figure for used 
+00000dc0: 4350 5520 7065 7263 656e 7461 6765 223e  CPU percentage">
+00000dd0: 0a20 2020 203c 2f64 6976 3e0a 2d20 6064  .    </div>.- `d
+00000de0: 656c 7461 603a 2074 6865 2064 6966 6665  elta`: the diffe
+00000df0: 7265 6e63 6573 2062 6574 7765 656e 2074  rences between t
+00000e00: 6865 2076 616c 7565 7320 6f66 2065 6163  he values of eac
+00000e10: 6820 636f 6c75 6d6e 2067 726f 7570 6564  h column grouped
+00000e20: 2062 7920 7065 7269 6f64 7320 6f66 2074   by periods of t
+00000e30: 696d 652e 2046 6f72 2069 6e73 7461 6e63  ime. For instanc
+00000e40: 652c 2074 6865 2064 6966 6665 7265 6e63  e, the differenc
+00000e50: 6573 0a20 2062 6574 7765 656e 2074 6865  es.  between the
+00000e60: 2070 6572 6365 6e74 6167 6520 6f66 2063   percentage of c
+00000e70: 7075 2075 7365 6420 6576 6572 7920 3130  pu used every 10
+00000e80: 2c20 3235 206f 7220 3530 206d 696e 7574  , 25 or 50 minut
+00000e90: 6573 2e20 5468 6573 6520 6465 6c74 6120  es. These delta 
+00000ea0: 6361 6e20 6265 2075 7365 6420 6173 2061  can be used as a
+00000eb0: 206d 6561 6e73 206f 6620 636f 6d70 6172   means of compar
+00000ec0: 6973 6f6e 2062 6574 7765 656e 0a20 2074  ison between.  t
+00000ed0: 696d 6520 7365 7269 6573 2073 686f 7274  ime series short
+00000ee0: 2d2f 6d69 642d 2f6c 6f6e 672d 7465 726d  -/mid-/long-term
+00000ef0: 2070 6174 7465 726e 732e 0a20 2020 203c   patterns..    <
+00000f00: 6469 763e 0a20 2020 203c 696d 6720 7372  div>.    <img sr
+00000f10: 633d 2268 7474 7073 3a2f 2f67 6974 6875  c="https://githu
+00000f20: 622e 636f 6d2f 616c 656a 616e 6472 6f66  b.com/alejandrof
+00000f30: 6465 7a2d 7573 2f73 696d 696c 6172 6974  dez-us/similarit
+00000f40: 792d 7473 2f62 6c6f 622f 6535 6231 3437  y-ts/blob/e5b147
+00000f50: 6231 3435 3937 3066 3361 3933 3335 3161  b145970f3a93351a
+00000f60: 3130 3034 3032 3266 6233 3064 3230 6635  1004022fb30d20f5
+00000f70: 6630 2f64 6f63 732f 6669 6775 7265 732f  f0/docs/figures/
+00000f80: 6465 6c74 615f 7361 6d70 6c65 5f33 5f63  delta_sample_3_c
+00000f90: 7075 5f75 7469 6c5f 7065 7263 656e 745f  pu_util_percent_
+00000fa0: 5453 5f31 5f76 735f 5453 5f32 5f28 6772  TS_1_vs_TS_2_(gr
+00000fb0: 6f75 7065 645f 6279 5f31 305f 6d69 6e75  ouped_by_10_minu
+00000fc0: 7465 7329 2e70 6e67 3f72 6177 3d74 7275  tes).png?raw=tru
+00000fd0: 6522 2061 6c74 3d22 4465 6c74 6120 4669  e" alt="Delta Fi
+00000fe0: 6775 7265 2066 6f72 2075 7365 6420 4350  gure for used CP
+00000ff0: 5520 7065 7263 656e 7461 6765 2067 726f  U percentage gro
+00001000: 7570 6564 2062 7920 3130 206d 696e 7574  uped by 10 minut
+00001010: 6573 223e 0a20 2020 203c 696d 6720 7372  es">.    <img sr
+00001020: 633d 2268 7474 7073 3a2f 2f67 6974 6875  c="https://githu
+00001030: 622e 636f 6d2f 616c 656a 616e 6472 6f66  b.com/alejandrof
+00001040: 6465 7a2d 7573 2f73 696d 696c 6172 6974  dez-us/similarit
+00001050: 792d 7473 2f62 6c6f 622f 6535 6231 3437  y-ts/blob/e5b147
+00001060: 6231 3435 3937 3066 3361 3933 3335 3161  b145970f3a93351a
+00001070: 3130 3034 3032 3266 6233 3064 3230 6635  1004022fb30d20f5
+00001080: 6630 2f64 6f63 732f 6669 6775 7265 732f  f0/docs/figures/
+00001090: 6465 6c74 615f 7361 6d70 6c65 5f33 5f63  delta_sample_3_c
+000010a0: 7075 5f75 7469 6c5f 7065 7263 656e 745f  pu_util_percent_
+000010b0: 5453 5f31 5f76 735f 5453 5f32 5f28 6772  TS_1_vs_TS_2_(gr
+000010c0: 6f75 7065 645f 6279 5f32 355f 6d69 6e75  ouped_by_25_minu
+000010d0: 7465 7329 2e70 6e67 3f72 6177 3d74 7275  tes).png?raw=tru
+000010e0: 6522 2061 6c74 3d22 4465 6c74 6120 4669  e" alt="Delta Fi
+000010f0: 6775 7265 2066 6f72 2075 7365 6420 4350  gure for used CP
+00001100: 5520 7065 7263 656e 7461 6765 2067 726f  U percentage gro
+00001110: 7570 6564 2062 7920 3235 206d 696e 7574  uped by 25 minut
+00001120: 6573 223e 0a20 2020 203c 696d 6720 7372  es">.    <img sr
+00001130: 633d 2268 7474 7073 3a2f 2f67 6974 6875  c="https://githu
+00001140: 622e 636f 6d2f 616c 656a 616e 6472 6f66  b.com/alejandrof
+00001150: 6465 7a2d 7573 2f73 696d 696c 6172 6974  dez-us/similarit
+00001160: 792d 7473 2f62 6c6f 622f 6535 6231 3437  y-ts/blob/e5b147
+00001170: 6231 3435 3937 3066 3361 3933 3335 3161  b145970f3a93351a
+00001180: 3130 3034 3032 3266 6233 3064 3230 6635  1004022fb30d20f5
+00001190: 6630 2f64 6f63 732f 6669 6775 7265 732f  f0/docs/figures/
+000011a0: 6465 6c74 615f 7361 6d70 6c65 5f33 5f63  delta_sample_3_c
+000011b0: 7075 5f75 7469 6c5f 7065 7263 656e 745f  pu_util_percent_
+000011c0: 5453 5f31 5f76 735f 5453 5f32 5f28 6772  TS_1_vs_TS_2_(gr
+000011d0: 6f75 7065 645f 6279 5f35 305f 6d69 6e75  ouped_by_50_minu
+000011e0: 7465 7329 2e70 6e67 3f72 6177 3d74 7275  tes).png?raw=tru
+000011f0: 6522 2061 6c74 3d22 4465 6c74 6120 4669  e" alt="Delta Fi
+00001200: 6775 7265 2066 6f72 2075 7365 6420 4350  gure for used CP
+00001210: 5520 7065 7263 656e 7461 6765 2067 726f  U percentage gro
+00001220: 7570 6564 2062 7920 3530 206d 696e 7574  uped by 50 minut
+00001230: 6573 223e 0a20 2020 203c 2f64 6976 3e0a  es">.    </div>.
+00001240: 0a2d 2060 7063 6160 3a20 7468 6520 6c69  .- `pca`: the li
+00001250: 6e65 6172 2064 696d 656e 7369 6f6e 616c  near dimensional
+00001260: 6974 7920 7265 6475 6374 696f 6e20 7465  ity reduction te
+00001270: 6368 6e69 7175 6520 7468 6174 2061 696d  chnique that aim
+00001280: 7320 746f 2066 696e 6420 7468 6520 7072  s to find the pr
+00001290: 696e 6369 7061 6c20 636f 6d70 6f6e 656e  incipal componen
+000012a0: 7473 206f 6620 6120 6461 7461 2073 6574  ts of a data set
+000012b0: 2062 790a 2020 636f 6d70 7574 696e 6720   by.  computing 
+000012c0: 7468 6520 6c69 6e65 6172 2063 6f6d 6269  the linear combi
+000012d0: 6e61 7469 6f6e 7320 6f66 2074 6865 206f  nations of the o
+000012e0: 7269 6769 6e61 6c20 6368 6172 6163 7465  riginal characte
+000012f0: 7269 7374 6963 7320 7468 6174 2065 7870  ristics that exp
+00001300: 6c61 696e 2074 6865 206d 6f73 7420 7661  lain the most va
+00001310: 7269 616e 6365 2069 6e20 7468 6520 6461  riance in the da
+00001320: 7461 2e0a 2020 2020 3c64 6976 2061 6c69  ta..    <div ali
+00001330: 676e 3d22 6365 6e74 6572 223e 0a20 2020  gn="center">.   
+00001340: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
+00001350: 3a2f 2f67 6974 6875 622e 636f 6d2f 616c  ://github.com/al
+00001360: 656a 616e 6472 6f66 6465 7a2d 7573 2f73  ejandrofdez-us/s
+00001370: 696d 696c 6172 6974 792d 7473 2f62 6c6f  imilarity-ts/blo
+00001380: 622f 6535 6231 3437 6231 3435 3937 3066  b/e5b147b145970f
+00001390: 3361 3933 3335 3161 3130 3034 3032 3266  3a93351a1004022f
+000013a0: 6233 3064 3230 6635 6630 2f64 6f63 732f  b30d20f5f0/docs/
+000013b0: 6669 6775 7265 732f 5043 412e 706e 673f  figures/PCA.png?
+000013c0: 7261 773d 7472 7565 2220 616c 743d 2250  raw=true" alt="P
+000013d0: 4341 2046 6967 7572 6522 2077 6964 7468  CA Figure" width
+000013e0: 3d22 3435 3022 3e0a 2020 2020 3c2f 6469  ="450">.    </di
+000013f0: 763e 0a2d 2060 7473 6e65 603a 2061 2074  v>.- `tsne`: a t
+00001400: 6f6f 6c20 666f 7220 7669 7375 616c 6973  ool for visualis
+00001410: 696e 6720 6869 6768 2d64 696d 656e 7369  ing high-dimensi
+00001420: 6f6e 616c 2064 6174 6120 7365 7473 2069  onal data sets i
+00001430: 6e20 6120 3244 206f 7220 3344 2067 7261  n a 2D or 3D gra
+00001440: 7068 6963 616c 2072 6570 7265 7365 6e74  phical represent
+00001450: 6174 696f 6e20 616c 6c6f 7769 6e67 2074  ation allowing t
+00001460: 6865 2063 7265 6174 696f 6e0a 2020 6f66  he creation.  of
+00001470: 2061 2073 696e 676c 6520 6d61 7020 7468   a single map th
+00001480: 6174 2072 6576 6561 6c73 2074 6865 2073  at reveals the s
+00001490: 7472 7563 7475 7265 206f 6620 7468 6520  tructure of the 
+000014a0: 6461 7461 2061 7420 6d61 6e79 2064 6966  data at many dif
+000014b0: 6665 7265 6e74 2073 6361 6c65 732e 0a20  ferent scales.. 
+000014c0: 2020 203c 6469 7620 616c 6967 6e3d 2263     <div align="c
+000014d0: 656e 7465 7222 3e0a 2020 2020 3c69 6d67  enter">.    <img
+000014e0: 2073 7263 3d22 6874 7470 733a 2f2f 6769   src="https://gi
+000014f0: 7468 7562 2e63 6f6d 2f61 6c65 6a61 6e64  thub.com/alejand
+00001500: 726f 6664 657a 2d75 732f 7369 6d69 6c61  rofdez-us/simila
+00001510: 7269 7479 2d74 732f 626c 6f62 2f65 3562  rity-ts/blob/e5b
+00001520: 3134 3762 3134 3539 3730 6633 6139 3333  147b145970f3a933
+00001530: 3531 6131 3030 3430 3232 6662 3330 6432  51a1004022fb30d2
+00001540: 3066 3566 302f 646f 6373 2f66 6967 7572  0f5f0/docs/figur
+00001550: 6573 2f74 2d53 4e45 2d69 7465 725f 3330  es/t-SNE-iter_30
+00001560: 302d 7065 7270 6c65 7869 7479 5f35 2e70  0-perplexity_5.p
+00001570: 6e67 3f72 6177 3d74 7275 6522 2061 6c74  ng?raw=true" alt
+00001580: 3d22 5453 4e45 2046 6967 7572 6520 3330  ="TSNE Figure 30
+00001590: 3020 6974 6572 6174 696f 6e73 2035 2070  0 iterations 5 p
+000015a0: 6572 706c 6578 6974 7922 2077 6964 7468  erplexity" width
+000015b0: 3d22 3435 3022 3e0a 2020 2020 3c69 6d67  ="450">.    <img
+000015c0: 2073 7263 3d22 6874 7470 733a 2f2f 6769   src="https://gi
+000015d0: 7468 7562 2e63 6f6d 2f61 6c65 6a61 6e64  thub.com/alejand
+000015e0: 726f 6664 657a 2d75 732f 7369 6d69 6c61  rofdez-us/simila
+000015f0: 7269 7479 2d74 732f 626c 6f62 2f65 3562  rity-ts/blob/e5b
+00001600: 3134 3762 3134 3539 3730 6633 6139 3333  147b145970f3a933
+00001610: 3531 6131 3030 3430 3232 6662 3330 6432  51a1004022fb30d2
+00001620: 3066 3566 302f 646f 6373 2f66 6967 7572  0f5f0/docs/figur
+00001630: 6573 2f74 2d53 4e45 2d69 7465 725f 3130  es/t-SNE-iter_10
+00001640: 3030 2d70 6572 706c 6578 6974 795f 352e  00-perplexity_5.
+00001650: 706e 673f 7261 773d 7472 7565 2220 616c  png?raw=true" al
+00001660: 743d 2254 534e 4520 4669 6775 7265 2031  t="TSNE Figure 1
+00001670: 3030 3020 6974 6572 6174 696f 6e73 2035  000 iterations 5
+00001680: 2070 6572 706c 6578 6974 7922 2077 6964   perplexity" wid
+00001690: 7468 3d22 3435 3022 3e0a 2020 2020 3c2f  th="450">.    </
+000016a0: 6469 763e 0a2d 2060 6474 7760 2070 6174  div>.- `dtw` pat
+000016b0: 683a 2049 6e20 6164 6469 7469 6f6e 2074  h: In addition t
+000016c0: 6f20 7468 6520 6e75 6d65 7269 6361 6c20  o the numerical 
+000016d0: 7369 6d69 6c61 7269 7479 206d 6561 7375  similarity measu
+000016e0: 7265 2c20 7468 6520 6772 6170 6869 6361  re, the graphica
+000016f0: 6c20 7265 7072 6573 656e 7461 7469 6f6e  l representation
+00001700: 206f 6620 7468 6520 4454 5720 7061 7468   of the DTW path
+00001710: 206f 6620 6561 6368 0a20 2063 6f6c 756d   of each.  colum
+00001720: 6e20 6361 6e20 6265 2075 7365 6675 6c20  n can be useful 
+00001730: 746f 2062 6574 7465 7220 616e 616c 7973  to better analys
+00001740: 6520 7468 6520 7369 6d69 6c61 7269 7469  e the similariti
+00001750: 6573 206f 7220 6469 6666 6572 656e 6365  es or difference
+00001760: 7320 6265 7477 6565 6e20 7468 6520 7469  s between the ti
+00001770: 6d65 2073 6572 6965 7320 636f 6c75 6d6e  me series column
+00001780: 732e 204e 6f74 6963 6520 7468 6174 0a20  s. Notice that. 
+00001790: 2074 6865 7265 2069 7320 6e6f 206d 756c   there is no mul
+000017a0: 7469 7661 7269 6174 6520 7265 7072 6573  tivariate repres
+000017b0: 656e 7461 7469 6f6e 206f 6620 4454 5720  entation of DTW 
+000017c0: 7061 7468 732c 206f 6e6c 7920 7369 6e67  paths, only sing
+000017d0: 6c65 2063 6f6c 756d 6e20 7265 7072 6573  le column repres
+000017e0: 656e 7461 7469 6f6e 732e 0a20 2020 203c  entations..    <
+000017f0: 6469 763e 0a20 2020 203c 696d 6720 7372  div>.    <img sr
+00001800: 633d 2268 7474 7073 3a2f 2f67 6974 6875  c="https://githu
+00001810: 622e 636f 6d2f 616c 656a 616e 6472 6f66  b.com/alejandrof
+00001820: 6465 7a2d 7573 2f73 696d 696c 6172 6974  dez-us/similarit
+00001830: 792d 7473 2f62 6c6f 622f 6535 6231 3437  y-ts/blob/e5b147
+00001840: 6231 3435 3937 3066 3361 3933 3335 3161  b145970f3a93351a
+00001850: 3130 3034 3032 3266 6233 3064 3230 6635  1004022fb30d20f5
+00001860: 6630 2f64 6f63 732f 6669 6775 7265 732f  f0/docs/figures/
+00001870: 4454 575f 7361 6d70 6c65 5f33 5f63 7075  DTW_sample_3_cpu
+00001880: 5f75 7469 6c5f 7065 7263 656e 742e 706e  _util_percent.pn
+00001890: 673f 7261 773d 7472 7565 2220 616c 743d  g?raw=true" alt=
+000018a0: 2244 5457 2046 6967 7572 6520 666f 7220  "DTW Figure for 
+000018b0: 6370 7522 3e0a 2020 2020 3c2f 6469 763e  cpu">.    </div>
+000018c0: 0a0a 2323 2049 6e73 7461 6c6c 6174 696f  ..## Installatio
+000018d0: 6e0a 0a54 6f20 696e 7374 616c 6c20 7468  n..To install th
+000018e0: 6520 746f 6f6c 2069 6e20 796f 7572 206c  e tool in your l
+000018f0: 6f63 616c 2065 6e76 6972 6f6e 6d65 6e74  ocal environment
+00001900: 2c20 6a75 7374 2072 756e 2066 6f6c 6c6f  , just run follo
+00001910: 7720 636f 6d6d 616e 643a 0a0a 6060 6042  w command:..```B
+00001920: 6173 680a 7069 7020 696e 7374 616c 6c20  ash.pip install 
+00001930: 7369 6d69 6c61 7269 7479 2d74 732d 636c  similarity-ts-cl
+00001940: 6920 0a60 6060 0a0a 2323 2055 7361 6765  i .```..## Usage
+00001950: 0a0a 5573 6572 7320 6d75 7374 2070 726f  ..Users must pro
+00001960: 7669 6465 2060 2e63 7376 6020 6669 6c65  vide `.csv` file
+00001970: 7320 636f 6e74 6169 6e69 6e67 206d 756c  s containing mul
+00001980: 7469 7661 7269 6174 6520 7469 6d65 2073  tivariate time s
+00001990: 6572 6965 7320 6279 2075 7369 6e67 2074  eries by using t
+000019a0: 6865 2061 7267 756d 656e 7473 2060 2d74  he arguments `-t
+000019b0: 7331 6020 616e 6420 602d 7473 3260 2e0a  s1` and `-ts2`..
+000019c0: 0a2d 2060 2d74 7331 6020 7368 6f75 6c64  .- `-ts1` should
+000019d0: 2070 6f69 6e74 2074 6f20 6120 7369 6e67   point to a sing
+000019e0: 6c65 2060 6373 7660 2066 696c 656e 616d  le `csv` filenam
+000019f0: 652e 2054 6869 7320 7469 6d65 2073 6572  e. This time ser
+00001a00: 6965 7320 6d61 7920 7265 7072 6573 656e  ies may represen
+00001a10: 7420 7468 6520 6261 7365 6c69 6e65 206f  t the baseline o
+00001a20: 7220 6772 6f75 6e64 2074 7275 7468 2074  r ground truth t
+00001a30: 696d 650a 2020 7365 7269 6573 2e0a 2d20  ime.  series..- 
+00001a40: 602d 7473 3260 2063 616e 2070 6f69 6e74  `-ts2` can point
+00001a50: 2074 6f20 616e 6f74 6865 7220 7369 6e67   to another sing
+00001a60: 6c65 2060 6373 7660 2066 696c 656e 616d  le `csv` filenam
+00001a70: 6520 6f72 2061 2064 6972 6563 746f 7279  e or a directory
+00001a80: 2074 6861 7420 636f 6e74 6169 6e73 206d   that contains m
+00001a90: 756c 7469 706c 6520 6063 7376 6020 6669  ultiple `csv` fi
+00001aa0: 6c65 7320 746f 2062 650a 2020 636f 6d70  les to be.  comp
+00001ab0: 6172 6564 2077 6974 6820 602d 7473 3160  ared with `-ts1`
+00001ac0: 2066 696c 652e 0a2d 2060 2d68 6561 6460   file..- `-head`
+00001ad0: 2069 6620 796f 7572 2074 696d 6520 7365   if your time se
+00001ae0: 7269 6573 2066 696c 6573 2069 6e63 6c75  ries files inclu
+00001af0: 6465 2061 2068 6561 6465 7220 7468 6973  de a header this
+00001b00: 2061 7267 756d 656e 7420 6d75 7374 2062   argument must b
+00001b10: 6520 7072 6573 656e 742e 2049 6620 6e6f  e present. If no
+00001b20: 7420 7072 6573 656e 742c 2074 6865 2073  t present, the s
+00001b30: 6f66 7477 6172 650a 2020 756e 6465 7273  oftware.  unders
+00001b40: 7461 6e64 7320 7468 6174 2063 7376 2066  tands that csv f
+00001b50: 696c 6573 2064 6f6e 2774 2069 6e63 6c75  iles don't inclu
+00001b60: 6465 2061 2068 6561 6465 7220 726f 772e  de a header row.
+00001b70: 0a0a 436f 6e73 7472 6169 6e74 733a 0a0a  ..Constraints:..
+00001b80: 2d20 602d 7473 3160 2074 696d 652d 7365  - `-ts1` time-se
+00001b90: 7269 6573 2066 696c 6520 616e 6420 602d  ries file and `-
+00001ba0: 7473 3260 2074 696d 652d 7365 7269 6573  ts2` time-series
+00001bb0: 2066 696c 6528 7329 206d 7573 743a 0a20   file(s) must:. 
+00001bc0: 2020 202d 2068 6176 6520 7468 6520 7361     - have the sa
+00001bd0: 6d65 2064 696d 656e 7369 6f6e 616c 6974  me dimensionalit
+00001be0: 7920 286e 756d 6265 7220 6f66 2063 6f6c  y (number of col
+00001bf0: 756d 6e73 290a 2020 2020 2d20 6e6f 7420  umns).    - not 
+00001c00: 696e 636c 7564 6520 6120 7469 6d65 7374  include a timest
+00001c10: 616d 7020 636f 6c75 6d6e 0a20 2020 202d  amp column.    -
+00001c20: 2069 6e63 6c75 6465 206f 6e6c 7920 6e75   include only nu
+00001c30: 6d65 7269 6320 7661 6c75 6573 0a20 2020  meric values.   
+00001c40: 202d 2069 6e63 6c75 6465 2074 6865 2073   - include the s
+00001c50: 616d 6520 6865 6164 6572 2028 6966 2070  ame header (if p
+00001c60: 7265 7365 6e74 290a 2d20 6966 2061 2068  resent).- if a h
+00001c70: 6561 6465 7220 6973 2070 7265 7365 6e74  eader is present
+00001c80: 2061 7320 6669 7273 7420 726f 772c 2075   as first row, u
+00001c90: 7365 2074 6865 2060 2d68 6561 6460 2061  se the `-head` a
+00001ca0: 7267 756d 656e 742e 0a2d 2061 6c6c 2060  rgument..- all `
+00001cb0: 2d74 7332 6020 7469 6d65 2d73 6572 6965  -ts2` time-serie
+00001cc0: 7320 6669 6c65 7320 6d75 7374 2068 6176  s files must hav
+00001cd0: 6520 7468 6520 7361 6d65 206c 656e 6774  e the same lengt
+00001ce0: 6820 286e 756d 6265 7220 6f66 2072 6f77  h (number of row
+00001cf0: 7329 2e0a 0a4e 6f74 653a 2074 6865 2063  s)...Note: the c
+00001d00: 6f6c 756d 6e20 6465 6c69 6d69 7465 7220  olumn delimiter 
+00001d10: 6973 2061 7574 6f6d 6174 6963 616c 6c79  is automatically
+00001d20: 2064 6574 6563 7465 642e 0a0a 4966 2079   detected...If y
+00001d30: 6f75 7220 6461 7461 2069 6e63 6c75 6465  our data include
+00001d40: 2063 6174 6567 6f72 6963 616c 2076 616c   categorical val
+00001d50: 7565 732c 2069 7420 6d69 6768 7420 6265  ues, it might be
+00001d60: 2070 7265 2d70 726f 6365 7373 6564 2074   pre-processed t
+00001d70: 6f20 636f 6e76 6572 7420 7468 656d 2074  o convert them t
+00001d80: 6f20 6e75 6d65 7269 6361 6c20 7661 6c75  o numerical valu
+00001d90: 6573 2e20 416c 6c20 6074 7332 7360 2074  es. All `ts2s` t
+00001da0: 696d 652d 7365 7269 6573 206d 7573 7420  ime-series must 
+00001db0: 6861 7665 2074 6865 2073 616d 6520 6c65  have the same le
+00001dc0: 6e67 7468 2028 6e75 6d62 6572 206f 6620  ngth (number of 
+00001dd0: 726f 7773 292e 0a0a 4966 2060 2d74 7331  rows)...If `-ts1
+00001de0: 6020 7469 6d65 2d73 6572 6965 7320 6669  ` time-series fi
+00001df0: 6c65 2069 7320 6c6f 6e67 6572 2028 6d6f  le is longer (mo
+00001e00: 7265 2072 6f77 7329 2074 6861 6e20 602d  re rows) than `-
+00001e10: 7473 3260 2074 696d 652d 7365 7269 6573  ts2` time-series
+00001e20: 2066 696c 6528 7329 2c20 7468 6520 602d   file(s), the `-
+00001e30: 7473 3160 2074 696d 6520 7365 7269 6573  ts1` time series
+00001e40: 2077 696c 6c20 6265 0a64 6976 6964 6564   will be.divided
+00001e50: 2069 6e20 7769 6e64 6f77 7320 6f66 2074   in windows of t
+00001e60: 6865 2073 616d 650a 6c65 6e67 7468 2061  he same.length a
+00001e70: 7320 7468 6520 602d 7473 3260 2074 696d  s the `-ts2` tim
+00001e80: 652d 7365 7269 6573 2066 696c 6528 7329  e-series file(s)
+00001e90: 2e0a 0a46 6f72 2065 6163 6820 602d 7473  ...For each `-ts
+00001ea0: 3260 2074 696d 652d 7365 7269 6573 2066  2` time-series f
+00001eb0: 696c 652c 2074 6865 206d 6f73 7420 7369  ile, the most si
+00001ec0: 6d69 6c61 7220 7769 6e64 6f77 2028 2a29  milar window (*)
+00001ed0: 2066 726f 6d20 602d 7473 3160 2074 696d   from `-ts1` tim
+00001ee0: 6520 7365 7269 6573 2069 7320 7365 6c65  e series is sele
+00001ef0: 6374 6564 2e0a 0a46 696e 616c 6c79 2c20  cted...Finally, 
+00001f00: 6d65 7472 6963 7320 616e 6420 6669 6775  metrics and figu
+00001f10: 7265 7320 7468 6174 2061 7373 6573 7320  res that assess 
+00001f20: 7468 6520 7369 6d69 6c61 7269 7479 2062  the similarity b
+00001f30: 6574 7765 656e 2065 6163 6820 7061 6972  etween each pair
+00001f40: 206f 6620 602d 7473 3260 2074 696d 652d   of `-ts2` time-
+00001f50: 7365 7269 6573 2066 696c 6520 616e 6420  series file and 
+00001f60: 6974 730a 6173 736f 6369 6174 6564 206d  its.associated m
+00001f70: 6f73 7420 7369 6d69 6c61 7220 602d 7473  ost similar `-ts
+00001f80: 3160 2077 696e 646f 7720 6172 6520 636f  1` window are co
+00001f90: 6d70 7574 6564 2e0a 0a28 2a29 2060 2d77  mputed...(*) `-w
+00001fa0: 5f73 656c 6563 745f 6d65 7460 2069 7320  _select_met` is 
+00001fb0: 7468 6520 6d65 7472 6963 2075 7365 6420  the metric used 
+00001fc0: 666f 7220 7468 6520 7365 6c65 6374 696f  for the selectio
+00001fd0: 6e20 6f66 2074 6865 206d 6f73 740a 7369  n of the most.si
+00001fe0: 6d69 6c61 7220 602d 7473 3160 2074 696d  milar `-ts1` tim
+00001ff0: 652d 7365 7269 6573 2077 696e 646f 7720  e-series window 
+00002000: 7065 7220 6561 6368 2060 2d74 7332 6020  per each `-ts2` 
+00002010: 7469 6d65 2d73 6572 6965 7320 6669 6c65  time-series file
+00002020: 2873 292e 6064 7477 6020 6973 2074 6865  (s).`dtw` is the
+00002030: 2064 6566 6175 6c74 2076 616c 7565 2c20   default value, 
+00002040: 686f 7765 7665 722c 2061 6e79 206f 660a  however, any of.
+00002050: 7468 650a 5b6d 6574 7269 6373 5d28 2361  the.[metrics](#a
+00002060: 7661 696c 6162 6c65 2d6d 6574 7269 6373  vailable-metrics
+00002070: 2920 6172 6520 616c 736f 2061 7661 696c  ) are also avail
+00002080: 6162 6c65 2066 6f72 2074 6869 7320 7075  able for this pu
+00002090: 7270 6f73 6520 7573 696e 6720 7468 6973  rpose using this
+000020a0: 2061 7267 756d 656e 742e 0a0a 5573 6572   argument...User
+000020b0: 7320 6361 6e20 7072 6f76 6964 6520 6d65  s can provide me
+000020c0: 7472 6963 7320 6f72 2066 6967 7572 6573  trics or figures
+000020d0: 2074 6f20 6265 2063 6f6d 7075 7465 642f   to be computed/
+000020e0: 6765 6e65 7261 7465 643a 0a0a 2d20 602d  generated:..- `-
+000020f0: 6d60 2074 6865 205b 6d65 7472 6963 735d  m` the [metrics]
+00002100: 2823 6176 6169 6c61 626c 652d 6d65 7472  (#available-metr
+00002110: 6963 7329 206e 616d 6573 2074 6f20 6265  ics) names to be
+00002120: 2063 6f6d 7075 7465 6420 6173 2061 206c   computed as a l
+00002130: 6973 7420 7365 7061 7261 7465 6420 6279  ist separated by
+00002140: 2073 7061 6365 732e 0a2d 2060 2d66 6020   spaces..- `-f` 
+00002150: 7468 6520 5b66 6967 7572 6573 5d28 2361  the [figures](#a
+00002160: 7661 696c 6162 6c65 2d66 6967 7572 6573  vailable-figures
+00002170: 2920 6e61 6d65 7320 746f 2062 6520 636f  ) names to be co
+00002180: 6d70 7574 6564 2061 7320 6120 6c69 7374  mputed as a list
+00002190: 2073 6570 6172 6174 6564 2062 7920 7370   separated by sp
+000021a0: 6163 6573 2e0a 0a49 6620 6e6f 206d 6574  aces...If no met
+000021b0: 7269 6373 206e 6f72 2066 6967 7572 6573  rics nor figures
+000021c0: 2061 7265 2070 726f 7669 6465 642c 2074   are provided, t
+000021d0: 6865 2074 6f6f 6c20 7769 6c6c 2063 6f6d  he tool will com
+000021e0: 7075 7465 2061 6c6c 2074 6865 2061 7661  pute all the ava
+000021f0: 696c 6162 6c65 206d 6574 7269 6373 2061  ilable metrics a
+00002200: 6e64 2066 6967 7572 6573 2e0a 0a54 6865  nd figures...The
+00002210: 2066 6f6c 6c6f 7769 6e67 2061 7267 756d   following argum
+00002220: 656e 7473 2061 7265 2061 6c73 6f20 6176  ents are also av
+00002230: 6169 6c61 626c 6520 666f 7220 6669 6e65  ailable for fine
+00002240: 2d74 756e 696e 673a 0a0a 2d20 602d 7473  -tuning:..- `-ts
+00002250: 5f66 7265 715f 7365 6373 6020 7468 6520  _freq_secs` the 
+00002260: 6672 6571 7565 6e63 7920 696e 2073 6563  frequency in sec
+00002270: 6f6e 6473 2069 6e20 7768 6963 6820 7361  onds in which sa
+00002280: 6d70 6c65 7320 7765 7265 2074 616b 656e  mples were taken
+00002290: 206a 7573 7420 746f 2067 656e 6572 6174   just to generat
+000022a0: 6520 7468 6520 6465 6c74 6120 6669 6775  e the delta figu
+000022b0: 7265 732e 2042 7920 6465 6661 756c 7420  res. By default 
+000022c0: 6973 0a20 2060 3160 2073 6563 6f6e 642e  is.  `1` second.
+000022d0: 0a2d 2060 2d73 7472 6460 2077 6865 6e20  .- `-strd` when 
+000022e0: 6074 7331 6020 7469 6d65 2d73 6572 6965  `ts1` time-serie
+000022f0: 7320 6973 206c 6f6e 6765 7220 7468 616e  s is longer than
+00002300: 2060 7473 3260 2074 696d 652d 7365 7269   `ts2` time-seri
+00002310: 6573 2066 696c 6528 7329 2074 6865 2077  es file(s) the w
+00002320: 696e 646f 7773 2061 7265 2063 6f6d 7075  indows are compu
+00002330: 7465 6420 6279 2075 7369 6e67 2061 0a20  ted by using a. 
+00002340: 2073 7472 6964 6520 6f66 2060 3160 2062   stride of `1` b
+00002350: 7920 6465 6661 756c 742e 2053 6f6d 6574  y default. Somet
+00002360: 696d 6573 2075 7369 6e67 2061 206c 6172  imes using a lar
+00002370: 6765 7220 7661 6c75 6520 666f 7220 7468  ger value for th
+00002380: 6520 7374 7269 6465 2070 6172 616d 6574  e stride paramet
+00002390: 6572 2069 6d70 726f 7665 7320 7468 6520  er improves the 
+000023a0: 7065 7266 6f72 6d61 6e63 6520 6279 2073  performance by s
+000023b0: 6b69 7070 696e 670a 2020 7468 6520 636f  kipping.  the co
+000023c0: 6d70 7574 6174 696f 6e20 6f66 2073 696d  mputation of sim
+000023d0: 696c 6172 6974 7920 6265 7477 6565 6e20  ilarity between 
+000023e0: 736f 206d 616e 7920 7769 6e64 6f77 732e  so many windows.
+000023f0: 0a0a 2323 2320 4261 7369 6320 7573 6167  ..### Basic usag
+00002400: 6520 6578 616d 706c 6573 3a0a 0a53 6f6d  e examples:..Som
+00002410: 6520 6578 616d 706c 6573 206f 6620 6576  e examples of ev
+00002420: 616c 7561 7469 6f6e 206f 6620 7369 6d69  aluation of simi
+00002430: 6c61 7269 7479 2061 7265 2073 686f 776e  larity are shown
+00002440: 2062 656c 6f77 2e20 596f 7520 6361 6e20   below. You can 
+00002450: 646f 776e 6c6f 6164 2073 6f6d 6520 7465  download some te
+00002460: 7374 2064 6174 6120 6279 2072 756e 6e69  st data by runni
+00002470: 6e67 2074 6865 2066 6f6c 6c6f 7769 6e67  ng the following
+00002480: 2063 6f6d 6d61 6e64 3a0a 0a60 6060 4261   command:..```Ba
+00002490: 7368 0a77 6765 7420 6874 7470 733a 2f2f  sh.wget https://
+000024a0: 6769 7468 7562 2e63 6f6d 2f61 6c65 6a61  github.com/aleja
+000024b0: 6e64 726f 6664 657a 2d75 732f 7369 6d69  ndrofdez-us/simi
+000024c0: 6c61 7269 7479 2d74 732d 636c 692f 7261  larity-ts-cli/ra
+000024d0: 772f 6d61 696e 2f64 6174 615f 7361 6d70  w/main/data_samp
+000024e0: 6c65 732e 7a69 7020 2626 2075 6e7a 6970  les.zip && unzip
+000024f0: 2064 6174 615f 7361 6d70 6c65 732e 7a69   data_samples.zi
+00002500: 700a 6060 600a 4f72 206d 616e 7561 6c6c  p.```.Or manuall
+00002510: 7920 646f 776e 6c6f 6164 2061 6e64 2075  y download and u
+00002520: 6e7a 6970 2066 726f 6d20 6874 7470 733a  nzip from https:
+00002530: 2f2f 6769 7468 7562 2e63 6f6d 2f61 6c65  //github.com/ale
+00002540: 6a61 6e64 726f 6664 657a 2d75 732f 7369  jandrofdez-us/si
+00002550: 6d69 6c61 7269 7479 2d74 732d 636c 692f  milarity-ts-cli/
+00002560: 7261 772f 6d61 696e 2f64 6174 615f 7361  raw/main/data_sa
+00002570: 6d70 6c65 732e 7a69 7020 2e0a 0a31 2e20  mples.zip ...1. 
+00002580: 4120 7469 6d65 2073 6572 6965 7320 616e  A time series an
+00002590: 6420 616c 6c20 7469 6d65 2073 6572 6965  d all time serie
+000025a0: 7320 636f 6d70 7574 696e 6720 616c 6c20  s computing all 
+000025b0: 6d65 7472 6963 7320 616e 6420 6669 6775  metrics and figu
+000025c0: 7265 733a 0a20 2020 2060 6060 4261 7368  res:.    ```Bash
+000025d0: 0a20 2020 2073 696d 696c 6172 6974 792d  .    similarity-
+000025e0: 7473 2d63 6c69 202d 7473 3120 6461 7461  ts-cli -ts1 data
+000025f0: 5f73 616d 706c 6573 2f61 6c69 6261 6261  _samples/alibaba
+00002600: 3230 3138 2f74 7331 5f6d 6163 6869 6e65  2018/ts1_machine
+00002610: 5f75 7361 6765 5f64 6179 735f 315f 746f  _usage_days_1_to
+00002620: 5f38 5f67 726f 7570 6564 5f33 3030 5f73  _8_grouped_300_s
+00002630: 6563 6f6e 6473 2e63 7376 202d 7473 3220  econds.csv -ts2 
+00002640: 6461 7461 5f73 616d 706c 6573 2f61 6c69  data_samples/ali
+00002650: 6261 6261 3230 3138 2f74 7332 202d 6865  baba2018/ts2 -he
+00002660: 6164 0a20 2020 2060 6060 0a20 2020 4576  ad.    ```.   Ev
+00002670: 6572 7920 6d65 7472 6963 2063 6f6d 7075  ery metric compu
+00002680: 7461 7469 6f6e 2061 6e64 2066 6967 7572  tation and figur
+00002690: 6520 6765 6e65 7261 7465 6420 7769 6c6c  e generated will
+000026a0: 2062 6520 666f 756e 6420 696e 2074 6865   be found in the
+000026b0: 2060 7265 7375 6c74 732f 7b74 696d 6573   `results/{times
+000026c0: 7461 6d70 7d2f 6020 6469 7265 6374 6f72  tamp}/` director
+000026d0: 792e 0a0a 312e 2054 776f 2074 696d 6520  y...1. Two time 
+000026e0: 7365 7269 6573 2063 6f6d 7075 7469 6e67  series computing
+000026f0: 206f 6e6c 7920 4454 5720 6d65 7472 6963   only DTW metric
+00002700: 2061 6e64 2044 5457 2066 6967 7572 653a   and DTW figure:
+00002710: 0a20 2020 2060 6060 4261 7368 0a20 2020  .    ```Bash.   
+00002720: 2073 696d 696c 6172 6974 792d 7473 2d63   similarity-ts-c
+00002730: 6c69 202d 7473 3120 6461 7461 5f73 616d  li -ts1 data_sam
+00002740: 706c 6573 2f61 6c69 6261 6261 3230 3138  ples/alibaba2018
+00002750: 2f74 7331 5f6d 6163 6869 6e65 5f75 7361  /ts1_machine_usa
+00002760: 6765 5f64 6179 735f 315f 746f 5f38 5f67  ge_days_1_to_8_g
+00002770: 726f 7570 6564 5f33 3030 5f73 6563 6f6e  rouped_300_secon
+00002780: 6473 2e63 7376 202d 7473 3220 6461 7461  ds.csv -ts2 data
+00002790: 5f73 616d 706c 6573 2f61 6c69 6261 6261  _samples/alibaba
+000027a0: 3230 3138 2f74 7332 2f73 616d 706c 655f  2018/ts2/sample_
+000027b0: 302e 6373 7620 2d68 6561 6420 2d6d 2064  0.csv -head -m d
+000027c0: 7477 202d 6620 6474 770a 2020 2020 6060  tw -f dtw.    ``
+000027d0: 600a 0a31 2e20 4120 7469 6d65 2073 6572  `..1. A time ser
+000027e0: 6965 7320 616e 6420 616c 6c20 7469 6d65  ies and all time
+000027f0: 2073 6572 6965 7320 7769 7468 696e 2061   series within a
+00002800: 2064 6972 6563 746f 7279 2063 6f6d 7075   directory compu
+00002810: 7469 6e67 2065 7665 7279 206d 6574 7269  ting every metri
+00002820: 6320 616e 6420 6669 6775 7265 2069 6e20  c and figure in 
+00002830: 5369 6d69 6c61 7269 7479 5453 2074 6f6f  SimilarityTS too
+00002840: 6c6b 6974 3a0a 2020 2020 6060 6042 6173  lkit:.    ```Bas
+00002850: 680a 2020 2020 7369 6d69 6c61 7269 7479  h.    similarity
+00002860: 2d74 732d 636c 6920 2d74 7331 2064 6174  -ts-cli -ts1 dat
+00002870: 615f 7361 6d70 6c65 732f 616c 6962 6162  a_samples/alibab
+00002880: 6132 3031 382f 7473 315f 6d61 6368 696e  a2018/ts1_machin
+00002890: 655f 7573 6167 655f 6461 7973 5f31 5f74  e_usage_days_1_t
+000028a0: 6f5f 385f 6772 6f75 7065 645f 3330 305f  o_8_grouped_300_
+000028b0: 7365 636f 6e64 732e 6373 7620 2d74 7332  seconds.csv -ts2
+000028c0: 2064 6174 615f 7361 6d70 6c65 732f 616c   data_samples/al
+000028d0: 6962 6162 6132 3031 382f 7473 3220 2d68  ibaba2018/ts2 -h
+000028e0: 6561 6420 2d6d 206a 7320 6d6d 6420 6474  ead -m js mmd dt
+000028f0: 7720 6b73 206b 6c20 6363 2063 7020 6869  w ks kl cc cp hi
+00002900: 202d 6620 6465 6c74 6120 6474 7720 3264   -f delta dtw 2d
+00002910: 2070 6361 2074 736e 650a 2020 2020 6060   pca tsne.    ``
+00002920: 600a 0a31 2e20 436f 6d70 6172 6973 6f6e  `..1. Comparison
+00002930: 2062 6574 7765 656e 2074 696d 6520 7365   between time se
+00002940: 7269 6573 2073 7065 6369 6679 696e 6720  ries specifying 
+00002950: 7468 6520 6672 6571 7565 6e63 7920 696e  the frequency in
+00002960: 2073 6563 6f6e 6473 2069 6e20 7768 6963   seconds in whic
+00002970: 6820 7361 6d70 6c65 7320 7765 7265 2074  h samples were t
+00002980: 616b 656e 3a0a 2020 2020 6060 6042 6173  aken:.    ```Bas
+00002990: 680a 2020 2020 7369 6d69 6c61 7269 7479  h.    similarity
+000029a0: 2d74 732d 636c 6920 2d74 7331 2064 6174  -ts-cli -ts1 dat
+000029b0: 615f 7361 6d70 6c65 732f 616c 6962 6162  a_samples/alibab
+000029c0: 6132 3031 382f 7473 315f 6d61 6368 696e  a2018/ts1_machin
+000029d0: 655f 7573 6167 655f 6461 7973 5f31 5f74  e_usage_days_1_t
+000029e0: 6f5f 385f 6772 6f75 7065 645f 3330 305f  o_8_grouped_300_
+000029f0: 7365 636f 6e64 732e 6373 7620 2d74 7332  seconds.csv -ts2
+00002a00: 2064 6174 615f 7361 6d70 6c65 732f 616c   data_samples/al
+00002a10: 6962 6162 6132 3031 382f 7473 3220 2d68  ibaba2018/ts2 -h
+00002a20: 6561 6420 2d6d 2064 7477 202d 6620 6474  ead -m dtw -f dt
+00002a30: 7720 2d74 735f 6672 6571 5f73 6563 7320  w -ts_freq_secs 
+00002a40: 3330 300a 2020 2020 6060 600a 0a31 2e20  300.    ```..1. 
+00002a50: 436f 6d70 6172 6973 6f6e 2062 6574 7765  Comparison betwe
+00002a60: 656e 2074 696d 6520 7365 7269 6573 2073  en time series s
+00002a70: 7065 6369 6679 696e 6720 7468 6520 7374  pecifying the st
+00002a80: 7269 6465 2074 6861 7420 6465 7465 726d  ride that determ
+00002a90: 696e 6573 2074 6865 2073 7465 7020 6f72  ines the step or
+00002aa0: 2064 6973 7461 6e63 6520 6279 2077 6869   distance by whi
+00002ab0: 6368 2061 2066 6978 6564 2d73 697a 650a  ch a fixed-size.
+00002ac0: 2020 2077 696e 646f 7720 6d6f 7665 7320     window moves 
+00002ad0: 6f76 6572 2074 6865 2066 6972 7374 2074  over the first t
+00002ae0: 696d 6520 7365 7269 6573 3a0a 2020 2020  ime series:.    
+00002af0: 6060 6042 6173 680a 2020 2020 7369 6d69  ```Bash.    simi
+00002b00: 6c61 7269 7479 2d74 732d 636c 6920 2d74  larity-ts-cli -t
+00002b10: 7331 2064 6174 615f 7361 6d70 6c65 732f  s1 data_samples/
+00002b20: 616c 6962 6162 6132 3031 382f 7473 315f  alibaba2018/ts1_
+00002b30: 6d61 6368 696e 655f 7573 6167 655f 6461  machine_usage_da
+00002b40: 7973 5f31 5f74 6f5f 385f 6772 6f75 7065  ys_1_to_8_groupe
+00002b50: 645f 3330 305f 7365 636f 6e64 732e 6373  d_300_seconds.cs
+00002b60: 7620 2d74 7332 2064 6174 615f 7361 6d70  v -ts2 data_samp
+00002b70: 6c65 732f 616c 6962 6162 6132 3031 382f  les/alibaba2018/
+00002b80: 7473 3220 2d68 6561 6420 2d6d 2064 7477  ts2 -head -m dtw
+00002b90: 202d 6620 6474 7720 2d73 7472 6420 350a   -f dtw -strd 5.
+00002ba0: 2020 2020 6060 600a 0a31 2e20 436f 6d70      ```..1. Comp
+00002bb0: 6172 6973 6f6e 2062 6574 7765 656e 2074  arison between t
+00002bc0: 696d 6520 7365 7269 6573 2073 7065 6369  ime series speci
+00002bd0: 6679 696e 6720 7468 6520 7769 6e64 6f77  fying the window
+00002be0: 2073 656c 6563 7469 6f6e 206d 6574 7269   selection metri
+00002bf0: 6320 746f 2062 6520 7573 6564 2077 6865  c to be used whe
+00002c00: 6e20 7365 6c65 6374 696e 6720 7468 6520  n selecting the 
+00002c10: 6d6f 7374 2073 696d 696c 6172 0a20 2020  most similar.   
+00002c20: 7769 6e64 6f77 7320 696e 0a20 2020 7468  windows in.   th
+00002c30: 6520 6669 7273 7420 7469 6d65 2073 6572  e first time ser
+00002c40: 6965 733a 0a0a 2020 2020 6060 6042 6173  ies:..    ```Bas
+00002c50: 680a 2020 2020 7369 6d69 6c61 7269 7479  h.    similarity
+00002c60: 2d74 732d 636c 6920 2d74 7331 2064 6174  -ts-cli -ts1 dat
+00002c70: 615f 7361 6d70 6c65 732f 616c 6962 6162  a_samples/alibab
+00002c80: 6132 3031 382f 7473 315f 6d61 6368 696e  a2018/ts1_machin
+00002c90: 655f 7573 6167 655f 6461 7973 5f31 5f74  e_usage_days_1_t
+00002ca0: 6f5f 385f 6772 6f75 7065 645f 3330 305f  o_8_grouped_300_
+00002cb0: 7365 636f 6e64 732e 6373 7620 2d74 7332  seconds.csv -ts2
+00002cc0: 2064 6174 615f 7361 6d70 6c65 732f 616c   data_samples/al
+00002cd0: 6962 6162 6132 3031 382f 7473 3220 2d68  ibaba2018/ts2 -h
+00002ce0: 6561 6420 2d6d 2064 7477 202d 6620 6474  ead -m dtw -f dt
+00002cf0: 7720 2d77 5f73 656c 6563 745f 6d65 7420  w -w_select_met 
+00002d00: 6a73 0a20 2020 2060 6060 0a0a 312e 2055  js.    ```..1. U
+00002d10: 7369 6e67 206f 7572 2073 616d 706c 6520  sing our sample 
+00002d20: 7469 6d65 2073 6572 6965 7320 746f 2063  time series to c
+00002d30: 6f6d 7075 7465 2065 7665 7279 2073 696e  ompute every sin
+00002d40: 676c 6520 6d65 7472 6963 2061 6e64 2066  gle metric and f
+00002d50: 6967 7572 6520 7769 7468 2061 2066 6978  igure with a fix
+00002d60: 6564 2074 696d 6573 7461 6d70 2066 7265  ed timestamp fre
+00002d70: 7175 656e 6379 2061 6e64 2073 7472 6964  quency and strid
+00002d80: 653a 0a0a 2020 2020 6060 6042 6173 680a  e:..    ```Bash.
+00002d90: 2020 2020 7369 6d69 6c61 7269 7479 2d74      similarity-t
+00002da0: 732d 636c 6920 2d74 7331 2064 6174 615f  s-cli -ts1 data_
+00002db0: 7361 6d70 6c65 732f 616c 6962 6162 6132  samples/alibaba2
+00002dc0: 3031 382f 7473 315f 6d61 6368 696e 655f  018/ts1_machine_
+00002dd0: 7573 6167 655f 6461 7973 5f31 5f74 6f5f  usage_days_1_to_
+00002de0: 385f 6772 6f75 7065 645f 3330 305f 7365  8_grouped_300_se
+00002df0: 636f 6e64 732e 6373 7620 2d74 7332 2064  conds.csv -ts2 d
+00002e00: 6174 615f 7361 6d70 6c65 732f 616c 6962  ata_samples/alib
+00002e10: 6162 6132 3031 382f 7473 3220 2d68 6561  aba2018/ts2 -hea
+00002e20: 6420 2d6d 206d 6d64 2064 7477 206b 7320  d -m mmd dtw ks 
+00002e30: 6b6c 2063 6320 6370 2068 6920 2d66 2064  kl cc cp hi -f d
+00002e40: 656c 7461 2064 7477 2032 6420 7063 6120  elta dtw 2d pca 
+00002e50: 7473 6e65 202d 775f 7365 6c65 6374 5f6d  tsne -w_select_m
+00002e60: 6574 2063 6320 2d74 735f 6672 6571 5f73  et cc -ts_freq_s
+00002e70: 6563 7320 3330 3020 2d73 7472 6420 350a  ecs 300 -strd 5.
+00002e80: 2020 2020 6060 600a 2323 204c 6963 656e      ```.## Licen
+00002e90: 7365 0a0a 5369 6d69 6c61 7269 7479 5453  se..SimilarityTS
+00002ea0: 2074 6f6f 6c6b 6974 2069 7320 6672 6565   toolkit is free
+00002eb0: 2061 6e64 206f 7065 6e2d 736f 7572 6365   and open-source
+00002ec0: 2073 6f66 7477 6172 6520 6c69 6365 6e73   software licens
+00002ed0: 6564 2075 6e64 6572 2074 6865 205b 4d49  ed under the [MI
+00002ee0: 5420 6c69 6365 6e73 655d 284c 4943 454e  T license](LICEN
+00002ef0: 5345 292e 0a0a 2323 2041 636b 6e6f 776c  SE)...## Acknowl
+00002f00: 6564 6765 6d65 6e74 730a 5072 6f6a 6563  edgements.Projec
+00002f10: 7420 5049 4432 3032 312d 3132 3232 3038  t PID2021-122208
+00002f20: 4f42 2d49 3030 2c20 5052 4f59 4558 4345  OB-I00, PROYEXCE
+00002f30: 4c5c 5f30 3032 3836 2061 6e64 2020 5445  L\_00286 and  TE
+00002f40: 4432 3032 312d 3133 3236 3935 422d 4930  D2021-132695B-I0
+00002f50: 3020 7072 6f6a 6563 742c 2066 756e 6465  0 project, funde
+00002f60: 6420 6279 204d 4349 4e20 2f20 4145 4920  d by MCIN / AEI 
+00002f70: 2f20 3130 2e31 3330 3339 202f 2035 3031  / 10.13039 / 501
+00002f80: 3130 3030 3131 3033 332c 2062 7920 416e  100011033, by An
+00002f90: 6461 6c75 7369 616e 2052 6567 696f 6e61  dalusian Regiona
+00002fa0: 6c20 476f 7665 726e 6d65 6e74 2c20 616e  l Government, an
+00002fb0: 6420 6279 2074 6865 2045 7572 6f70 6561  d by the Europea
+00002fc0: 6e20 556e 696f 6e20 2d20 4e65 7874 4765  n Union - NextGe
+00002fd0: 6e65 7261 7469 6f6e 4555 2e0a            nerationEU..
```

### Comparing `similarity_ts_cli-1.0.0/pyproject.toml` & `similarity_ts_cli-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "similarity_ts_cli"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
     { name = "Alejandro Fernández-Montes", email = "afdez@us.es" },
     { name = "Damián Fernández-Cerero", email = "damiancerero@us.es" },
     { name = "Felipe Escalera González", email = "fescalera@us.es" },
 ]
 dependencies = ["similarity-ts", "tqdm"]
 description = "SimilarityTS-cli is an open-source tool designed to facilitate the usage of SimilarityTS package from a command line interface"
```

### Comparing `similarity_ts_cli-1.0.0/src/similarity_ts_cli/cli.py` & `similarity_ts_cli-1.0.1/src/similarity_ts_cli/cli.py`

 * *Files identical despite different names*

### Comparing `similarity_ts_cli-1.0.0/src/similarity_ts_cli.egg-info/PKG-INFO` & `similarity_ts_cli-1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,753 +1,720 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 7369 6d69  : 2.1.Name: simi
-00000020: 6c61 7269 7479 2d74 732d 636c 690a 5665  larity-ts-cli.Ve
-00000030: 7273 696f 6e3a 2031 2e30 2e30 0a53 756d  rsion: 1.0.0.Sum
-00000040: 6d61 7279 3a20 5369 6d69 6c61 7269 7479  mary: Similarity
-00000050: 5453 2d63 6c69 2069 7320 616e 206f 7065  TS-cli is an ope
-00000060: 6e2d 736f 7572 6365 2074 6f6f 6c20 6465  n-source tool de
-00000070: 7369 676e 6564 2074 6f20 6661 6369 6c69  signed to facili
-00000080: 7461 7465 2074 6865 2075 7361 6765 206f  tate the usage o
-00000090: 6620 5369 6d69 6c61 7269 7479 5453 2070  f SimilarityTS p
-000000a0: 6163 6b61 6765 2066 726f 6d20 6120 636f  ackage from a co
-000000b0: 6d6d 616e 6420 6c69 6e65 2069 6e74 6572  mmand line inter
-000000c0: 6661 6365 0a41 7574 686f 722d 656d 6169  face.Author-emai
-000000d0: 6c3a 2041 6c65 6a61 6e64 726f 2046 6572  l: Alejandro Fer
-000000e0: 6ec3 a16e 6465 7a2d 4d6f 6e74 6573 203c  n..ndez-Montes <
-000000f0: 6166 6465 7a40 7573 2e65 733e 2c20 4461  afdez@us.es>, Da
-00000100: 6d69 c3a1 6e20 4665 726e c3a1 6e64 657a  mi..n Fern..ndez
-00000110: 2d43 6572 6572 6f20 3c64 616d 6961 6e63  -Cerero <damianc
-00000120: 6572 6572 6f40 7573 2e65 733e 2c20 4665  erero@us.es>, Fe
-00000130: 6c69 7065 2045 7363 616c 6572 6120 476f  lipe Escalera Go
-00000140: 6e7a c3a1 6c65 7a20 3c66 6573 6361 6c65  nz..lez <fescale
-00000150: 7261 4075 732e 6573 3e0a 5072 6f6a 6563  ra@us.es>.Projec
-00000160: 742d 5552 4c3a 2048 6f6d 6570 6167 652c  t-URL: Homepage,
-00000170: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00000180: 636f 6d2f 616c 656a 616e 6472 6f66 6465  com/alejandrofde
-00000190: 7a2d 7573 2f73 696d 696c 6172 6974 792d  z-us/similarity-
-000001a0: 7473 2d63 6c69 0a50 726f 6a65 6374 2d55  ts-cli.Project-U
-000001b0: 524c 3a20 4275 6720 5472 6163 6b65 722c  RL: Bug Tracker,
-000001c0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-000001d0: 636f 6d2f 616c 656a 616e 6472 6f66 6465  com/alejandrofde
-000001e0: 7a2d 7573 2f73 696d 696c 6172 6974 792d  z-us/similarity-
-000001f0: 7473 2d63 6c69 2f69 7373 7565 730a 436c  ts-cli/issues.Cl
-00000200: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
-00000210: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000220: 3a20 5079 7468 6f6e 203a 3a20 330a 436c  : Python :: 3.Cl
-00000230: 6173 7369 6669 6572 3a20 4c69 6365 6e73  assifier: Licens
-00000240: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
-00000250: 6420 3a3a 204d 4954 204c 6963 656e 7365  d :: MIT License
-00000260: 0a43 6c61 7373 6966 6965 723a 204f 7065  .Classifier: Ope
-00000270: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
-00000280: 204f 5320 496e 6465 7065 6e64 656e 740a   OS Independent.
-00000290: 5265 7175 6972 6573 2d50 7974 686f 6e3a  Requires-Python:
-000002a0: 203e 3d33 2e39 0a44 6573 6372 6970 7469   >=3.9.Descripti
-000002b0: 6f6e 2d43 6f6e 7465 6e74 2d54 7970 653a  on-Content-Type:
-000002c0: 2074 6578 742f 6d61 726b 646f 776e 0a4c   text/markdown.L
-000002d0: 6963 656e 7365 2d46 696c 653a 204c 4943  icense-File: LIC
-000002e0: 454e 5345 0a0a 5b21 5b76 6572 7369 6f6e  ENSE..[![version
-000002f0: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-00000300: 6965 6c64 732e 696f 2f62 6164 6765 2f76  ields.io/badge/v
-00000310: 6572 7369 6f6e 2d31 2e30 2d62 6c75 6529  ersion-1.0-blue)
+00000000: 5b21 5b76 6572 7369 6f6e 5d28 6874 7470  [![version](http
+00000010: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000020: 696f 2f62 6164 6765 2f70 7970 692d 312e  io/badge/pypi-1.
+00000030: 302e 312d 626c 7565 295d 2868 7474 7073  0.1-blue)](https
+00000040: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
+00000050: 6563 742f 7369 6d69 6c61 7269 7479 2d74  ect/similarity-t
+00000060: 732d 636c 692f 290a 5b21 5b50 7974 686f  s-cli/).[![Pytho
+00000070: 6e20 332e 395d 2868 7474 7073 3a2f 2f69  n 3.9](https://i
+00000080: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
+00000090: 6467 652f 7079 7468 6f6e 2d33 2e39 2d64  dge/python-3.9-d
+000000a0: 6172 6b67 7265 656e 295d 2868 7474 7073  arkgreen)](https
+000000b0: 3a2f 2f77 7777 2e70 7974 686f 6e2e 6f72  ://www.python.or
+000000c0: 672f 646f 776e 6c6f 6164 732f 7265 6c65  g/downloads/rele
+000000d0: 6173 652f 7079 7468 6f6e 2d33 3930 2f29  ase/python-390/)
+000000e0: 0a5b 215b 6c61 7374 2d75 7064 6174 655d  .[![last-update]
+000000f0: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+00000100: 656c 6473 2e69 6f2f 6261 6467 652f 6c61  elds.io/badge/la
+00000110: 7374 5f75 7064 6174 652d 3037 2f31 382f  st_update-07/18/
+00000120: 3230 3233 2d62 7269 6768 7467 7265 656e  2023-brightgreen
+00000130: 295d 2868 7474 7073 3a2f 2f67 6974 6875  )](https://githu
+00000140: 622e 636f 6d2f 616c 656a 616e 6472 6f66  b.com/alejandrof
+00000150: 6465 7a2d 7573 2f73 696d 696c 6172 6974  dez-us/similarit
+00000160: 792d 7473 2d63 6c69 2f63 6f6d 6d69 7473  y-ts-cli/commits
+00000170: 2f6d 6169 6e29 0a5b 215b 6c69 6365 6e73  /main).[![licens
+00000180: 655d 2868 7474 7073 3a2f 2f69 6d67 2e73  e](https://img.s
+00000190: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
+000001a0: 6c69 6365 6e73 652d 4d49 542d 6f72 616e  license-MIT-oran
+000001b0: 6765 295d 284c 4943 454e 5345 290a 0a23  ge)](LICENSE)..#
+000001c0: 2053 696d 696c 6172 6974 7954 532d 636c   SimilarityTS-cl
+000001d0: 693a 2043 6f6d 6d61 6e64 2d6c 696e 6520  i: Command-line 
+000001e0: 696e 7465 7266 6163 6520 666f 7220 5369  interface for Si
+000001f0: 6d69 6c61 7269 7479 5453 2070 6163 6b61  milarityTS packa
+00000200: 6765 0a0a 2323 2054 6162 6c65 206f 6620  ge..## Table of 
+00000210: 436f 6e74 656e 7473 0a0a 2d20 5b44 6573  Contents..- [Des
+00000220: 6372 6970 7469 6f6e 5d28 2364 6573 6372  cription](#descr
+00000230: 6970 7469 6f6e 290a 2d20 5b49 6e73 7461  iption).- [Insta
+00000240: 6c6c 6174 696f 6e5d 2823 696e 7374 616c  llation](#instal
+00000250: 6c61 7469 6f6e 290a 2d20 5b55 7361 6765  lation).- [Usage
+00000260: 5d28 2375 7361 6765 290a 2d20 5b4c 6963  ](#usage).- [Lic
+00000270: 656e 7365 5d28 236c 6963 656e 7365 290a  ense](#license).
+00000280: 2d20 5b41 636b 6e6f 776c 6564 6765 6d65  - [Acknowledgeme
+00000290: 6e74 735d 2823 6163 6b6e 6f77 6c65 6467  nts](#acknowledg
+000002a0: 656d 656e 7473 290a 0a23 2320 4465 7363  ements)..## Desc
+000002b0: 7269 7074 696f 6e0a 0a53 696d 696c 6172  ription..Similar
+000002c0: 6974 7954 532d 636c 6920 6973 2061 2063  ityTS-cli is a c
+000002d0: 6f6d 6d61 6e64 2d6c 696e 6520 696e 7465  ommand-line inte
+000002e0: 7266 6163 6520 746f 6f6c 2074 6861 7420  rface tool that 
+000002f0: 6163 7420 6173 2061 6e20 696e 7465 7266  act as an interf
+00000300: 6163 6520 6f66 2074 6865 205b 5369 6d69  ace of the [Simi
+00000310: 6c61 7269 7479 5453 2070 6163 6b61 6765  larityTS package
 00000320: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
 00000330: 2e63 6f6d 2f61 6c65 6a61 6e64 726f 6664  .com/alejandrofd
 00000340: 657a 2d75 732f 7369 6d69 6c61 7269 7479  ez-us/similarity
-00000350: 2d74 732f 7265 6c65 6173 6573 290a 5b21  -ts/releases).[!
-00000360: 5b50 7974 686f 6e20 332e 395d 2868 7474  [Python 3.9](htt
-00000370: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00000380: 2e69 6f2f 6261 6467 652f 7079 7468 6f6e  .io/badge/python
-00000390: 2d33 2e39 2d64 6172 6b67 7265 656e 295d  -3.9-darkgreen)]
-000003a0: 2868 7474 7073 3a2f 2f77 7777 2e70 7974  (https://www.pyt
-000003b0: 686f 6e2e 6f72 672f 646f 776e 6c6f 6164  hon.org/download
-000003c0: 732f 7265 6c65 6173 652f 7079 7468 6f6e  s/release/python
-000003d0: 2d33 3930 2f29 0a5b 215b 6c61 7374 2d75  -390/).[![last-u
-000003e0: 7064 6174 655d 2868 7474 7073 3a2f 2f69  pdate](https://i
-000003f0: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
-00000400: 6467 652f 6c61 7374 5f75 7064 6174 652d  dge/last_update-
-00000410: 3037 2f58 592f 3230 3233 2d62 7269 6768  07/XY/2023-brigh
-00000420: 7467 7265 656e 295d 2868 7474 7073 3a2f  tgreen)](https:/
-00000430: 2f67 6974 6875 622e 636f 6d2f 616c 656a  /github.com/alej
-00000440: 616e 6472 6f66 6465 7a2d 7573 2f73 696d  androfdez-us/sim
-00000450: 696c 6172 6974 792d 7473 2f63 6f6d 6d69  ilarity-ts/commi
-00000460: 7473 2f6d 6169 6e29 0a21 5b6c 6963 656e  ts/main).![licen
-00000470: 7365 5d28 6874 7470 733a 2f2f 696d 672e  se](https://img.
-00000480: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
-00000490: 2f6c 6963 656e 7365 2d4d 4954 2d6f 7261  /license-MIT-ora
-000004a0: 6e67 6529 0a0a 2320 5369 6d69 6c61 7269  nge)..# Similari
-000004b0: 7479 5453 2d63 6c69 3a20 436f 6d6d 616e  tyTS-cli: Comman
-000004c0: 642d 6c69 6e65 2069 6e74 6572 6661 6365  d-line interface
-000004d0: 2066 6f72 2053 696d 696c 6172 6974 7954   for SimilarityT
-000004e0: 5320 7061 636b 6167 650a 0a23 2320 5461  S package..## Ta
-000004f0: 626c 6520 6f66 2043 6f6e 7465 6e74 730a  ble of Contents.
-00000500: 0a2d 205b 4465 7363 7269 7074 696f 6e5d  .- [Description]
-00000510: 2823 6465 7363 7269 7074 696f 6e29 0a2d  (#description).-
-00000520: 205b 496e 7374 616c 6c61 7469 6f6e 5d28   [Installation](
-00000530: 2369 6e73 7461 6c6c 6174 696f 6e29 0a2d  #installation).-
-00000540: 205b 5573 6167 655d 2823 7573 6167 6529   [Usage](#usage)
-00000550: 0a2d 205b 4164 7661 6e63 6564 2075 7361  .- [Advanced usa
-00000560: 6765 5d28 2361 6476 616e 6365 642d 7573  ge](#advanced-us
-00000570: 6167 6529 0a2d 205b 4c69 6365 6e73 655d  age).- [License]
-00000580: 2823 6c69 6365 6e73 6529 0a0a 2323 2044  (#license)..## D
-00000590: 6573 6372 6970 7469 6f6e 0a0a 5369 6d69  escription..Simi
-000005a0: 6c61 7269 7479 5453 2d63 6c69 2069 7320  larityTS-cli is 
-000005b0: 6120 636f 6d6d 616e 642d 6c69 6e65 2069  a command-line i
-000005c0: 6e74 6572 6661 6365 2074 6f6f 6c20 7468  nterface tool th
-000005d0: 6174 2061 6374 2061 7320 616e 2069 6e74  at act as an int
-000005e0: 6572 6661 6365 206f 6620 7468 6520 5369  erface of the Si
-000005f0: 6d69 6c61 7269 7479 5453 2070 6163 6b61  milarityTS packa
-00000600: 6765 2e20 5369 6d69 6c61 7269 7479 2d54  ge. Similarity-T
-00000610: 5320 7061 636b 6167 6520 6661 6369 6c69  S package facili
-00000620: 7461 7465 7320 7468 6520 6576 616c 7561  tates the evalua
-00000630: 7469 6f6e 2061 6e64 2063 6f6d 7061 7269  tion and compari
-00000640: 736f 6e20 6f66 0a6d 756c 7469 7661 7269  son of.multivari
-00000650: 6174 6520 7469 6d65 2073 6572 6965 7320  ate time series 
-00000660: 6461 7461 2e20 4974 2070 726f 7669 6465  data. It provide
-00000670: 7320 6120 636f 6d70 7265 6865 6e73 6976  s a comprehensiv
-00000680: 6520 746f 6f6c 6b69 7420 666f 7220 616e  e toolkit for an
-00000690: 616c 797a 696e 672c 2076 6973 7561 6c69  alyzing, visuali
-000006a0: 7a69 6e67 2c20 616e 6420 7265 706f 7274  zing, and report
-000006b0: 696e 6720 6d75 6c74 6970 6c65 0a6d 6574  ing multiple.met
-000006c0: 7269 6373 2061 6e64 2066 6967 7572 6573  rics and figures
-000006d0: 2064 6572 6976 6564 2066 726f 6d20 7469   derived from ti
-000006e0: 6d65 2073 6572 6965 7320 6461 7461 7365  me series datase
-000006f0: 7473 2e20 5468 6520 746f 6f6c 6b69 7420  ts. The toolkit 
-00000700: 7369 6d70 6c69 6669 6573 2074 6865 2070  simplifies the p
-00000710: 726f 6365 7373 206f 6620 6576 616c 7561  rocess of evalua
-00000720: 7469 6e67 2074 6865 2073 696d 696c 6172  ting the similar
-00000730: 6974 7920 6f66 0a74 696d 6520 7365 7269  ity of.time seri
-00000740: 6573 2062 7920 6f66 6665 7269 6e67 2064  es by offering d
-00000750: 6174 6120 7072 6570 726f 6365 7373 696e  ata preprocessin
-00000760: 672c 206d 6574 7269 6373 2063 6f6d 7075  g, metrics compu
-00000770: 7461 7469 6f6e 2c20 7669 7375 616c 697a  tation, visualiz
-00000780: 6174 696f 6e2c 2073 7461 7469 7374 6963  ation, statistic
-00000790: 616c 2061 6e61 6c79 7369 732c 2061 6e64  al analysis, and
-000007a0: 2072 6570 6f72 7420 6765 6e65 7261 7469   report generati
-000007b0: 6f6e 0a66 756e 6374 696f 6e61 6c69 7469  on.functionaliti
-000007c0: 6573 2e20 5769 7468 2069 7473 2063 7573  es. With its cus
-000007d0: 746f 6d69 7a61 626c 6520 6665 6174 7572  tomizable featur
-000007e0: 6573 2c20 5369 6d69 6c61 7269 7479 5453  es, SimilarityTS
-000007f0: 2065 6d70 6f77 6572 7320 7265 7365 6172   empowers resear
-00000800: 6368 6572 7320 616e 6420 6461 7461 0a73  chers and data.s
-00000810: 6369 656e 7469 7374 7320 746f 2067 6169  cientists to gai
-00000820: 6e20 696e 7369 6768 7473 2c20 6964 656e  n insights, iden
-00000830: 7469 6679 2070 6174 7465 726e 732c 2061  tify patterns, a
-00000840: 6e64 206d 616b 6520 696e 666f 726d 6564  nd make informed
-00000850: 2064 6563 6973 696f 6e73 2062 6173 6564   decisions based
-00000860: 206f 6e20 7468 6569 7220 7469 6d65 2073   on their time s
-00000870: 6572 6965 7320 6461 7461 2e0a 0a54 6869  eries data...Thi
-00000880: 7320 636f 6d6d 616e 642d 6c69 6e65 2069  s command-line i
-00000890: 6e74 6572 6661 6365 2069 7320 4f53 2069  nterface is OS i
-000008a0: 6e64 6570 656e 6461 6e74 2061 6e64 2063  ndependant and c
-000008b0: 616e 2062 6520 6561 7369 6c79 2069 6e73  an be easily ins
-000008c0: 7461 6c6c 6564 2061 6e64 2075 7365 642e  talled and used.
-000008d0: 0a0a 2323 2320 4176 6169 6c61 626c 6520  ..### Available 
-000008e0: 6d65 7472 6963 730a 0a54 6869 7320 746f  metrics..This to
-000008f0: 6f6c 6b69 7420 6361 6e20 636f 6d70 7574  olkit can comput
-00000900: 6520 7468 6520 666f 6c6c 6f77 696e 6720  e the following 
-00000910: 6d65 7472 6963 733a 0a0a 2d20 606b 6c60  metrics:..- `kl`
-00000920: 3a20 4b75 6c6c 6261 636b 2d4c 6569 626c  : Kullback-Leibl
-00000930: 6572 2064 6976 6572 6765 6e63 650a 2d20  er divergence.- 
-00000940: 606a 7360 3a20 4a65 6e73 656e 2d53 6861  `js`: Jensen-Sha
-00000950: 6e6e 6f6e 2064 6976 6572 6765 6e63 650a  nnon divergence.
-00000960: 2d20 606b 7360 3a20 4b6f 6c6d 6f67 6f72  - `ks`: Kolmogor
-00000970: 6f76 2d53 6d69 726e 6f76 2074 6573 740a  ov-Smirnov test.
-00000980: 2d20 606d 6d64 603a 204d 6178 696d 756d  - `mmd`: Maximum
-00000990: 204d 6561 6e20 4469 7363 7265 7061 6e63   Mean Discrepanc
-000009a0: 790a 2d20 6064 7477 6020 4479 6e61 6d69  y.- `dtw` Dynami
-000009b0: 6320 5469 6d65 2057 6172 7069 6e67 0a2d  c Time Warping.-
-000009c0: 2060 6363 603a 2044 6966 6665 7265 6e63   `cc`: Differenc
-000009d0: 6520 6f66 2063 6f2d 7661 7269 616e 6365  e of co-variance
-000009e0: 730a 2d20 6063 7060 3a20 4469 6666 6572  s.- `cp`: Differ
-000009f0: 656e 6365 206f 6620 636f 7272 656c 6174  ence of correlat
-00000a00: 696f 6e73 0a2d 2060 6869 603a 2044 6966  ions.- `hi`: Dif
-00000a10: 6665 7265 6e63 6520 6f66 2068 6973 746f  ference of histo
-00000a20: 6772 616d 730a 0a23 2323 2041 7661 696c  grams..### Avail
-00000a30: 6162 6c65 2066 6967 7572 6573 0a0a 5468  able figures..Th
-00000a40: 6973 2074 6f6f 6c6b 6974 2063 616e 2067  is toolkit can g
-00000a50: 656e 6572 6174 6520 7468 6520 666f 6c6c  enerate the foll
-00000a60: 6f77 696e 6720 6669 6775 7265 733a 0a0a  owing figures:..
-00000a70: 2d20 6032 6460 3a20 7468 6520 6f72 6469  - `2d`: the ordi
-00000a80: 6e61 7279 2067 7261 7068 6963 616c 2072  nary graphical r
-00000a90: 6570 7265 7365 6e74 6174 696f 6e20 6f66  epresentation of
-00000aa0: 2074 6865 2074 696d 6520 7365 7269 6573   the time series
-00000ab0: 2069 6e20 6120 3244 2066 6967 7572 6520   in a 2D figure 
-00000ac0: 7769 7468 2074 6865 2074 696d 6520 7265  with the time re
-00000ad0: 7072 6573 656e 7465 6420 6f6e 2074 6865  presented on the
-00000ae0: 2078 2061 7869 730a 2020 616e 6420 7468   x axis.  and th
-00000af0: 6520 6461 7461 2076 616c 7565 7320 6f6e  e data values on
-00000b00: 2074 6865 2079 2d61 7869 7320 666f 720a   the y-axis for.
-00000b10: 2020 2020 2d20 7468 6520 636f 6d70 6c65      - the comple
-00000b20: 7465 206d 756c 7469 7661 7269 6174 6520  te multivariate 
-00000b30: 7469 6d65 2073 6572 6965 733b 2061 6e64  time series; and
-00000b40: 0a20 2020 202d 2061 2070 6c6f 7420 7065  .    - a plot pe
-00000b50: 7220 636f 6c75 6d6e 2e0a 0a20 2045 6163  r column...  Eac
-00000b60: 6820 6765 6e65 7261 7465 6420 6669 6775  h generated figu
-00000b70: 7265 2070 6c6f 7473 2062 6f74 6820 7468  re plots both th
-00000b80: 6520 6074 7331 6020 616e 6420 7468 6520  e `ts1` and the 
-00000b90: 6074 7332 6020 6461 7461 2074 6f20 6561  `ts2` data to ea
-00000ba0: 7369 6c79 206f 6274 6169 6e20 6b65 7920  sily obtain key 
-00000bb0: 696e 7369 6768 7473 2069 6e74 6f0a 2020  insights into.  
-00000bc0: 7468 6520 7369 6d69 6c61 7269 7469 6573  the similarities
-00000bd0: 206f 7220 6469 6666 6572 656e 6365 7320   or differences 
-00000be0: 6265 7477 6565 6e20 7468 656d 2e0a 2020  between them..  
-00000bf0: 2020 3c64 6976 3e0a 2020 2020 3c69 6d67    <div>.    <img
-00000c00: 2073 7263 3d22 6874 7470 733a 2f2f 6769   src="https://gi
-00000c10: 7468 7562 2e63 6f6d 2f61 6c65 6a61 6e64  thub.com/alejand
-00000c20: 726f 6664 657a 2d75 732f 7369 6d69 6c61  rofdez-us/simila
-00000c30: 7269 7479 2d74 732f 626c 6f62 2f65 3562  rity-ts/blob/e5b
-00000c40: 3134 3762 3134 3539 3730 6633 6139 3333  147b145970f3a933
-00000c50: 3531 6131 3030 3430 3232 6662 3330 6432  51a1004022fb30d2
-00000c60: 3066 3566 302f 646f 6373 2f66 6967 7572  0f5f0/docs/figur
-00000c70: 6573 2f32 645f 7361 6d70 6c65 5f33 5f63  es/2d_sample_3_c
-00000c80: 6f6d 706c 6574 655f 5453 5f31 5f76 735f  omplete_TS_1_vs_
-00000c90: 5453 5f32 2e70 6e67 3f72 6177 3d74 7275  TS_2.png?raw=tru
-00000ca0: 6522 2061 6c74 3d22 3244 2046 6967 7572  e" alt="2D Figur
-00000cb0: 6520 636f 6d70 6c65 7465 223e 0a20 2020  e complete">.   
-00000cc0: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
-00000cd0: 3a2f 2f67 6974 6875 622e 636f 6d2f 616c  ://github.com/al
-00000ce0: 656a 616e 6472 6f66 6465 7a2d 7573 2f73  ejandrofdez-us/s
-00000cf0: 696d 696c 6172 6974 792d 7473 2f62 6c6f  imilarity-ts/blo
-00000d00: 622f 6535 6231 3437 6231 3435 3937 3066  b/e5b147b145970f
-00000d10: 3361 3933 3335 3161 3130 3034 3032 3266  3a93351a1004022f
-00000d20: 6233 3064 3230 6635 6630 2f64 6f63 732f  b30d20f5f0/docs/
-00000d30: 6669 6775 7265 732f 3264 5f73 616d 706c  figures/2d_sampl
-00000d40: 655f 335f 6370 755f 7574 696c 5f70 6572  e_3_cpu_util_per
-00000d50: 6365 6e74 5f54 535f 315f 7673 5f54 535f  cent_TS_1_vs_TS_
-00000d60: 322e 706e 673f 7261 773d 7472 7565 2220  2.png?raw=true" 
-00000d70: 616c 743d 2232 4420 4669 6775 7265 2066  alt="2D Figure f
-00000d80: 6f72 2075 7365 6420 4350 5520 7065 7263  or used CPU perc
-00000d90: 656e 7461 6765 223e 0a20 2020 203c 2f64  entage">.    </d
-00000da0: 6976 3e0a 2d20 6064 656c 7461 603a 2074  iv>.- `delta`: t
-00000db0: 6865 2064 6966 6665 7265 6e63 6573 2062  he differences b
-00000dc0: 6574 7765 656e 2074 6865 2076 616c 7565  etween the value
-00000dd0: 7320 6f66 2065 6163 6820 636f 6c75 6d6e  s of each column
-00000de0: 2067 726f 7570 6564 2062 7920 7065 7269   grouped by peri
-00000df0: 6f64 7320 6f66 2074 696d 652e 2046 6f72  ods of time. For
-00000e00: 2069 6e73 7461 6e63 652c 2074 6865 2064   instance, the d
-00000e10: 6966 6665 7265 6e63 6573 0a20 2062 6574  ifferences.  bet
-00000e20: 7765 656e 2074 6865 2070 6572 6365 6e74  ween the percent
-00000e30: 6167 6520 6f66 2063 7075 2075 7365 6420  age of cpu used 
-00000e40: 6576 6572 7920 3130 2c20 3235 206f 7220  every 10, 25 or 
-00000e50: 3530 206d 696e 7574 6573 2e20 5468 6573  50 minutes. Thes
-00000e60: 6520 6465 6c74 6120 6361 6e20 6265 2075  e delta can be u
-00000e70: 7365 6420 6173 2061 206d 6561 6e73 206f  sed as a means o
-00000e80: 6620 636f 6d70 6172 6973 6f6e 2062 6574  f comparison bet
-00000e90: 7765 656e 0a20 2074 696d 6520 7365 7269  ween.  time seri
-00000ea0: 6573 2073 686f 7274 2d2f 6d69 642d 2f6c  es short-/mid-/l
-00000eb0: 6f6e 672d 7465 726d 2070 6174 7465 726e  ong-term pattern
-00000ec0: 732e 0a20 2020 203c 6469 763e 0a20 2020  s..    <div>.   
-00000ed0: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
-00000ee0: 3a2f 2f67 6974 6875 622e 636f 6d2f 616c  ://github.com/al
-00000ef0: 656a 616e 6472 6f66 6465 7a2d 7573 2f73  ejandrofdez-us/s
-00000f00: 696d 696c 6172 6974 792d 7473 2f62 6c6f  imilarity-ts/blo
-00000f10: 622f 6535 6231 3437 6231 3435 3937 3066  b/e5b147b145970f
-00000f20: 3361 3933 3335 3161 3130 3034 3032 3266  3a93351a1004022f
-00000f30: 6233 3064 3230 6635 6630 2f64 6f63 732f  b30d20f5f0/docs/
-00000f40: 6669 6775 7265 732f 6465 6c74 615f 7361  figures/delta_sa
-00000f50: 6d70 6c65 5f33 5f63 7075 5f75 7469 6c5f  mple_3_cpu_util_
-00000f60: 7065 7263 656e 745f 5453 5f31 5f76 735f  percent_TS_1_vs_
-00000f70: 5453 5f32 5f28 6772 6f75 7065 645f 6279  TS_2_(grouped_by
-00000f80: 5f31 305f 6d69 6e75 7465 7329 2e70 6e67  _10_minutes).png
-00000f90: 3f72 6177 3d74 7275 6522 2061 6c74 3d22  ?raw=true" alt="
-00000fa0: 4465 6c74 6120 4669 6775 7265 2066 6f72  Delta Figure for
-00000fb0: 2075 7365 6420 4350 5520 7065 7263 656e   used CPU percen
-00000fc0: 7461 6765 2067 726f 7570 6564 2062 7920  tage grouped by 
-00000fd0: 3130 206d 696e 7574 6573 223e 0a20 2020  10 minutes">.   
-00000fe0: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
-00000ff0: 3a2f 2f67 6974 6875 622e 636f 6d2f 616c  ://github.com/al
-00001000: 656a 616e 6472 6f66 6465 7a2d 7573 2f73  ejandrofdez-us/s
-00001010: 696d 696c 6172 6974 792d 7473 2f62 6c6f  imilarity-ts/blo
-00001020: 622f 6535 6231 3437 6231 3435 3937 3066  b/e5b147b145970f
-00001030: 3361 3933 3335 3161 3130 3034 3032 3266  3a93351a1004022f
-00001040: 6233 3064 3230 6635 6630 2f64 6f63 732f  b30d20f5f0/docs/
-00001050: 6669 6775 7265 732f 6465 6c74 615f 7361  figures/delta_sa
-00001060: 6d70 6c65 5f33 5f63 7075 5f75 7469 6c5f  mple_3_cpu_util_
-00001070: 7065 7263 656e 745f 5453 5f31 5f76 735f  percent_TS_1_vs_
-00001080: 5453 5f32 5f28 6772 6f75 7065 645f 6279  TS_2_(grouped_by
-00001090: 5f32 355f 6d69 6e75 7465 7329 2e70 6e67  _25_minutes).png
-000010a0: 3f72 6177 3d74 7275 6522 2061 6c74 3d22  ?raw=true" alt="
-000010b0: 4465 6c74 6120 4669 6775 7265 2066 6f72  Delta Figure for
-000010c0: 2075 7365 6420 4350 5520 7065 7263 656e   used CPU percen
-000010d0: 7461 6765 2067 726f 7570 6564 2062 7920  tage grouped by 
-000010e0: 3235 206d 696e 7574 6573 223e 0a20 2020  25 minutes">.   
-000010f0: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
-00001100: 3a2f 2f67 6974 6875 622e 636f 6d2f 616c  ://github.com/al
-00001110: 656a 616e 6472 6f66 6465 7a2d 7573 2f73  ejandrofdez-us/s
-00001120: 696d 696c 6172 6974 792d 7473 2f62 6c6f  imilarity-ts/blo
-00001130: 622f 6535 6231 3437 6231 3435 3937 3066  b/e5b147b145970f
-00001140: 3361 3933 3335 3161 3130 3034 3032 3266  3a93351a1004022f
-00001150: 6233 3064 3230 6635 6630 2f64 6f63 732f  b30d20f5f0/docs/
-00001160: 6669 6775 7265 732f 6465 6c74 615f 7361  figures/delta_sa
-00001170: 6d70 6c65 5f33 5f63 7075 5f75 7469 6c5f  mple_3_cpu_util_
-00001180: 7065 7263 656e 745f 5453 5f31 5f76 735f  percent_TS_1_vs_
-00001190: 5453 5f32 5f28 6772 6f75 7065 645f 6279  TS_2_(grouped_by
-000011a0: 5f35 305f 6d69 6e75 7465 7329 2e70 6e67  _50_minutes).png
-000011b0: 3f72 6177 3d74 7275 6522 2061 6c74 3d22  ?raw=true" alt="
-000011c0: 4465 6c74 6120 4669 6775 7265 2066 6f72  Delta Figure for
-000011d0: 2075 7365 6420 4350 5520 7065 7263 656e   used CPU percen
-000011e0: 7461 6765 2067 726f 7570 6564 2062 7920  tage grouped by 
-000011f0: 3530 206d 696e 7574 6573 223e 0a20 2020  50 minutes">.   
-00001200: 203c 2f64 6976 3e0a 0a2d 2060 7063 6160   </div>..- `pca`
-00001210: 3a20 7468 6520 6c69 6e65 6172 2064 696d  : the linear dim
-00001220: 656e 7369 6f6e 616c 6974 7920 7265 6475  ensionality redu
-00001230: 6374 696f 6e20 7465 6368 6e69 7175 6520  ction technique 
-00001240: 7468 6174 2061 696d 7320 746f 2066 696e  that aims to fin
-00001250: 6420 7468 6520 7072 696e 6369 7061 6c20  d the principal 
-00001260: 636f 6d70 6f6e 656e 7473 206f 6620 6120  components of a 
-00001270: 6461 7461 2073 6574 2062 790a 2020 636f  data set by.  co
-00001280: 6d70 7574 696e 6720 7468 6520 6c69 6e65  mputing the line
-00001290: 6172 2063 6f6d 6269 6e61 7469 6f6e 7320  ar combinations 
-000012a0: 6f66 2074 6865 206f 7269 6769 6e61 6c20  of the original 
-000012b0: 6368 6172 6163 7465 7269 7374 6963 7320  characteristics 
-000012c0: 7468 6174 2065 7870 6c61 696e 2074 6865  that explain the
-000012d0: 206d 6f73 7420 7661 7269 616e 6365 2069   most variance i
-000012e0: 6e20 7468 6520 6461 7461 2e0a 2020 2020  n the data..    
-000012f0: 3c64 6976 2061 6c69 676e 3d22 6365 6e74  <div align="cent
-00001300: 6572 223e 0a20 2020 203c 696d 6720 7372  er">.    <img sr
-00001310: 633d 2268 7474 7073 3a2f 2f67 6974 6875  c="https://githu
-00001320: 622e 636f 6d2f 616c 656a 616e 6472 6f66  b.com/alejandrof
-00001330: 6465 7a2d 7573 2f73 696d 696c 6172 6974  dez-us/similarit
-00001340: 792d 7473 2f62 6c6f 622f 6535 6231 3437  y-ts/blob/e5b147
-00001350: 6231 3435 3937 3066 3361 3933 3335 3161  b145970f3a93351a
-00001360: 3130 3034 3032 3266 6233 3064 3230 6635  1004022fb30d20f5
-00001370: 6630 2f64 6f63 732f 6669 6775 7265 732f  f0/docs/figures/
-00001380: 5043 412e 706e 673f 7261 773d 7472 7565  PCA.png?raw=true
-00001390: 2220 616c 743d 2250 4341 2046 6967 7572  " alt="PCA Figur
-000013a0: 6522 2077 6964 7468 3d22 3435 3022 3e0a  e" width="450">.
-000013b0: 2020 2020 3c2f 6469 763e 0a2d 2060 7473      </div>.- `ts
-000013c0: 6e65 603a 2061 2074 6f6f 6c20 666f 7220  ne`: a tool for 
-000013d0: 7669 7375 616c 6973 696e 6720 6869 6768  visualising high
-000013e0: 2d64 696d 656e 7369 6f6e 616c 2064 6174  -dimensional dat
-000013f0: 6120 7365 7473 2069 6e20 6120 3244 206f  a sets in a 2D o
-00001400: 7220 3344 2067 7261 7068 6963 616c 2072  r 3D graphical r
-00001410: 6570 7265 7365 6e74 6174 696f 6e20 616c  epresentation al
-00001420: 6c6f 7769 6e67 2074 6865 2063 7265 6174  lowing the creat
-00001430: 696f 6e0a 2020 6f66 2061 2073 696e 676c  ion.  of a singl
-00001440: 6520 6d61 7020 7468 6174 2072 6576 6561  e map that revea
-00001450: 6c73 2074 6865 2073 7472 7563 7475 7265  ls the structure
-00001460: 206f 6620 7468 6520 6461 7461 2061 7420   of the data at 
-00001470: 6d61 6e79 2064 6966 6665 7265 6e74 2073  many different s
-00001480: 6361 6c65 732e 0a20 2020 203c 6469 7620  cales..    <div 
-00001490: 616c 6967 6e3d 2263 656e 7465 7222 3e0a  align="center">.
-000014a0: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
-000014b0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000014c0: 2f61 6c65 6a61 6e64 726f 6664 657a 2d75  /alejandrofdez-u
-000014d0: 732f 7369 6d69 6c61 7269 7479 2d74 732f  s/similarity-ts/
-000014e0: 626c 6f62 2f65 3562 3134 3762 3134 3539  blob/e5b147b1459
-000014f0: 3730 6633 6139 3333 3531 6131 3030 3430  70f3a93351a10040
-00001500: 3232 6662 3330 6432 3066 3566 302f 646f  22fb30d20f5f0/do
-00001510: 6373 2f66 6967 7572 6573 2f74 2d53 4e45  cs/figures/t-SNE
-00001520: 2d69 7465 725f 3330 302d 7065 7270 6c65  -iter_300-perple
-00001530: 7869 7479 5f35 2e70 6e67 3f72 6177 3d74  xity_5.png?raw=t
-00001540: 7275 6522 2061 6c74 3d22 5453 4e45 2046  rue" alt="TSNE F
-00001550: 6967 7572 6520 3330 3020 6974 6572 6174  igure 300 iterat
-00001560: 696f 6e73 2035 2070 6572 706c 6578 6974  ions 5 perplexit
-00001570: 7922 2077 6964 7468 3d22 3435 3022 3e0a  y" width="450">.
-00001580: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
-00001590: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000015a0: 2f61 6c65 6a61 6e64 726f 6664 657a 2d75  /alejandrofdez-u
-000015b0: 732f 7369 6d69 6c61 7269 7479 2d74 732f  s/similarity-ts/
-000015c0: 626c 6f62 2f65 3562 3134 3762 3134 3539  blob/e5b147b1459
-000015d0: 3730 6633 6139 3333 3531 6131 3030 3430  70f3a93351a10040
-000015e0: 3232 6662 3330 6432 3066 3566 302f 646f  22fb30d20f5f0/do
-000015f0: 6373 2f66 6967 7572 6573 2f74 2d53 4e45  cs/figures/t-SNE
-00001600: 2d69 7465 725f 3130 3030 2d70 6572 706c  -iter_1000-perpl
-00001610: 6578 6974 795f 352e 706e 673f 7261 773d  exity_5.png?raw=
-00001620: 7472 7565 2220 616c 743d 2254 534e 4520  true" alt="TSNE 
-00001630: 4669 6775 7265 2031 3030 3020 6974 6572  Figure 1000 iter
-00001640: 6174 696f 6e73 2035 2070 6572 706c 6578  ations 5 perplex
-00001650: 6974 7922 2077 6964 7468 3d22 3435 3022  ity" width="450"
-00001660: 3e0a 2020 2020 3c2f 6469 763e 0a2d 2060  >.    </div>.- `
-00001670: 6474 7760 2070 6174 683a 2049 6e20 6164  dtw` path: In ad
-00001680: 6469 7469 6f6e 2074 6f20 7468 6520 6e75  dition to the nu
-00001690: 6d65 7269 6361 6c20 7369 6d69 6c61 7269  merical similari
-000016a0: 7479 206d 6561 7375 7265 2c20 7468 6520  ty measure, the 
-000016b0: 6772 6170 6869 6361 6c20 7265 7072 6573  graphical repres
-000016c0: 656e 7461 7469 6f6e 206f 6620 7468 6520  entation of the 
-000016d0: 4454 5720 7061 7468 206f 6620 6561 6368  DTW path of each
-000016e0: 0a20 2063 6f6c 756d 6e20 6361 6e20 6265  .  column can be
-000016f0: 2075 7365 6675 6c20 746f 2062 6574 7465   useful to bette
-00001700: 7220 616e 616c 7973 6520 7468 6520 7369  r analyse the si
-00001710: 6d69 6c61 7269 7469 6573 206f 7220 6469  milarities or di
-00001720: 6666 6572 656e 6365 7320 6265 7477 6565  fferences betwee
-00001730: 6e20 7468 6520 7469 6d65 2073 6572 6965  n the time serie
-00001740: 7320 636f 6c75 6d6e 732e 204e 6f74 6963  s columns. Notic
-00001750: 6520 7468 6174 0a20 2074 6865 7265 2069  e that.  there i
-00001760: 7320 6e6f 206d 756c 7469 7661 7269 6174  s no multivariat
-00001770: 6520 7265 7072 6573 656e 7461 7469 6f6e  e representation
-00001780: 206f 6620 4454 5720 7061 7468 732c 206f   of DTW paths, o
-00001790: 6e6c 7920 7369 6e67 6c65 2063 6f6c 756d  nly single colum
-000017a0: 6e20 7265 7072 6573 656e 7461 7469 6f6e  n representation
-000017b0: 732e 0a20 2020 203c 6469 763e 0a20 2020  s..    <div>.   
-000017c0: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
-000017d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 616c  ://github.com/al
-000017e0: 656a 616e 6472 6f66 6465 7a2d 7573 2f73  ejandrofdez-us/s
-000017f0: 696d 696c 6172 6974 792d 7473 2f62 6c6f  imilarity-ts/blo
-00001800: 622f 6535 6231 3437 6231 3435 3937 3066  b/e5b147b145970f
-00001810: 3361 3933 3335 3161 3130 3034 3032 3266  3a93351a1004022f
-00001820: 6233 3064 3230 6635 6630 2f64 6f63 732f  b30d20f5f0/docs/
-00001830: 6669 6775 7265 732f 4454 575f 7361 6d70  figures/DTW_samp
-00001840: 6c65 5f33 5f63 7075 5f75 7469 6c5f 7065  le_3_cpu_util_pe
-00001850: 7263 656e 742e 706e 673f 7261 773d 7472  rcent.png?raw=tr
-00001860: 7565 2220 616c 743d 2244 5457 2046 6967  ue" alt="DTW Fig
-00001870: 7572 6520 666f 7220 6370 7522 3e0a 2020  ure for cpu">.  
-00001880: 2020 3c2f 6469 763e 0a0a 2323 2049 6e73    </div>..## Ins
-00001890: 7461 6c6c 6174 696f 6e0a 0a54 6f20 696e  tallation..To in
-000018a0: 7374 616c 6c20 7468 6520 746f 6f6c 2069  stall the tool i
-000018b0: 6e20 796f 7572 206c 6f63 616c 2065 6e76  n your local env
-000018c0: 6972 6f6e 6d65 6e74 2c20 6a75 7374 2072  ironment, just r
-000018d0: 756e 2066 6f6c 6c6f 7720 636f 6d6d 616e  un follow comman
-000018e0: 643a 0a0a 6060 6042 6173 680a 7069 7020  d:..```Bash.pip 
-000018f0: 696e 7374 616c 6c20 7369 6d69 6c61 7269  install similari
-00001900: 7479 2d74 732d 636c 6920 0a60 6060 0a0a  ty-ts-cli .```..
-00001910: 2323 2055 7361 6765 0a0a 5573 6572 7320  ## Usage..Users 
-00001920: 6d75 7374 2070 726f 7669 6465 2060 2e63  must provide `.c
-00001930: 7376 6020 6669 6c65 7320 636f 6e74 6169  sv` files contai
-00001940: 6e69 6e67 206d 756c 7469 7661 7269 6174  ning multivariat
-00001950: 6520 7469 6d65 2073 6572 6965 7320 6279  e time series by
-00001960: 2075 7369 6e67 2074 6865 2061 7267 756d   using the argum
-00001970: 656e 7473 2060 2d74 7331 6020 616e 6420  ents `-ts1` and 
-00001980: 602d 7473 3260 2e0a 0a2d 2060 2d74 7331  `-ts2`...- `-ts1
-00001990: 6020 7368 6f75 6c64 2070 6f69 6e74 2074  ` should point t
-000019a0: 6f20 6120 7369 6e67 6c65 2060 6373 7660  o a single `csv`
-000019b0: 2066 696c 656e 616d 652e 2054 6869 7320   filename. This 
-000019c0: 7469 6d65 2073 6572 6965 7320 6d61 7920  time series may 
-000019d0: 7265 7072 6573 656e 7420 7468 6520 6261  represent the ba
-000019e0: 7365 6c69 6e65 206f 7220 6772 6f75 6e64  seline or ground
-000019f0: 2074 7275 7468 2074 696d 650a 2020 7365   truth time.  se
-00001a00: 7269 6573 2e0a 2d20 602d 7473 3260 2063  ries..- `-ts2` c
-00001a10: 616e 2070 6f69 6e74 2074 6f20 616e 6f74  an point to anot
-00001a20: 6865 7220 7369 6e67 6c65 2060 6373 7660  her single `csv`
-00001a30: 2066 696c 656e 616d 6520 6f72 2061 2064   filename or a d
-00001a40: 6972 6563 746f 7279 2074 6861 7420 636f  irectory that co
-00001a50: 6e74 6169 6e73 206d 756c 7469 706c 6520  ntains multiple 
-00001a60: 6063 7376 6020 6669 6c65 7320 746f 2062  `csv` files to b
-00001a70: 650a 2020 636f 6d70 6172 6564 2077 6974  e.  compared wit
-00001a80: 6820 602d 7473 3160 2066 696c 652e 0a2d  h `-ts1` file..-
-00001a90: 2060 2d68 6561 6460 2069 6620 796f 7572   `-head` if your
-00001aa0: 2074 696d 6520 7365 7269 6573 2066 696c   time series fil
-00001ab0: 6573 2069 6e63 6c75 6465 2061 2068 6561  es include a hea
-00001ac0: 6465 7220 7468 6973 2061 7267 756d 656e  der this argumen
-00001ad0: 7420 6d75 7374 2062 6520 7072 6573 656e  t must be presen
-00001ae0: 742e 2049 6620 6e6f 7420 7072 6573 656e  t. If not presen
-00001af0: 742c 2074 6865 2073 6f66 7477 6172 650a  t, the software.
-00001b00: 2020 756e 6465 7273 7461 6e64 7320 7468    understands th
-00001b10: 6174 2063 7376 2066 696c 6573 2064 6f6e  at csv files don
-00001b20: 2774 2069 6e63 6c75 6465 2061 2068 6561  't include a hea
-00001b30: 6465 7220 726f 772e 0a0a 436f 6e73 7472  der row...Constr
-00001b40: 6169 6e74 733a 0a0a 2d20 602d 7473 3160  aints:..- `-ts1`
-00001b50: 2074 696d 652d 7365 7269 6573 2066 696c   time-series fil
-00001b60: 6520 616e 6420 602d 7473 3260 2074 696d  e and `-ts2` tim
-00001b70: 652d 7365 7269 6573 2066 696c 6528 7329  e-series file(s)
-00001b80: 206d 7573 743a 0a20 2020 202d 2068 6176   must:.    - hav
-00001b90: 6520 7468 6520 7361 6d65 2064 696d 656e  e the same dimen
-00001ba0: 7369 6f6e 616c 6974 7920 286e 756d 6265  sionality (numbe
-00001bb0: 7220 6f66 2063 6f6c 756d 6e73 290a 2020  r of columns).  
-00001bc0: 2020 2d20 6e6f 7420 696e 636c 7564 6520    - not include 
-00001bd0: 6120 7469 6d65 7374 616d 7020 636f 6c75  a timestamp colu
-00001be0: 6d6e 0a20 2020 202d 2069 6e63 6c75 6465  mn.    - include
-00001bf0: 206f 6e6c 7920 6e75 6d65 7269 6320 7661   only numeric va
-00001c00: 6c75 6573 0a20 2020 202d 2069 6e63 6c75  lues.    - inclu
-00001c10: 6465 2074 6865 2073 616d 6520 6865 6164  de the same head
-00001c20: 6572 2028 6966 2070 7265 7365 6e74 290a  er (if present).
-00001c30: 2d20 6966 2061 2068 6561 6465 7220 6973  - if a header is
-00001c40: 2070 7265 7365 6e74 2061 7320 6669 7273   present as firs
-00001c50: 7420 726f 772c 2075 7365 2074 6865 2060  t row, use the `
-00001c60: 2d68 6561 6460 2061 7267 756d 656e 740a  -head` argument.
-00001c70: 2d20 616c 6c20 602d 7473 3260 2074 696d  - all `-ts2` tim
-00001c80: 652d 7365 7269 6573 2066 696c 6573 206d  e-series files m
-00001c90: 7573 7420 6861 7665 2074 6865 2073 616d  ust have the sam
-00001ca0: 6520 6c65 6e67 7468 2028 6e75 6d62 6572  e length (number
-00001cb0: 206f 6620 726f 7773 292e 0a0a 4e6f 7465   of rows)...Note
-00001cc0: 3a20 7468 6520 636f 6c75 6d6e 2064 656c  : the column del
-00001cd0: 696d 6974 6572 2069 7320 6175 746f 6d61  imiter is automa
-00001ce0: 7469 6361 6c6c 7920 6465 7465 6374 6564  tically detected
-00001cf0: 2e0a 0a49 6620 602d 7473 3160 2074 696d  ...If `-ts1` tim
-00001d00: 652d 7365 7269 6573 2066 696c 6520 6973  e-series file is
-00001d10: 206c 6f6e 6765 7220 286d 6f72 6520 726f   longer (more ro
-00001d20: 7773 2920 7468 616e 2060 2d74 7332 6020  ws) than `-ts2` 
-00001d30: 7469 6d65 2d73 6572 6965 7320 6669 6c65  time-series file
-00001d40: 2873 292c 2074 6865 2060 2d74 7331 6020  (s), the `-ts1` 
-00001d50: 7469 6d65 2073 6572 6965 7320 7769 6c6c  time series will
-00001d60: 2062 650a 6469 7669 6465 6420 696e 2077   be.divided in w
-00001d70: 696e 646f 7773 206f 6620 7468 6520 7361  indows of the sa
-00001d80: 6d65 0a6c 656e 6774 6820 6173 2074 6865  me.length as the
-00001d90: 2060 2d74 7332 6020 7469 6d65 2d73 6572   `-ts2` time-ser
-00001da0: 6965 7320 6669 6c65 2873 292e 0a0a 466f  ies file(s)...Fo
-00001db0: 7220 6561 6368 2060 2d74 7332 6020 7469  r each `-ts2` ti
-00001dc0: 6d65 2d73 6572 6965 7320 6669 6c65 2c20  me-series file, 
-00001dd0: 7468 6520 6d6f 7374 2073 696d 696c 6172  the most similar
-00001de0: 2077 696e 646f 7720 282a 2920 6672 6f6d   window (*) from
-00001df0: 2060 2d74 7331 6020 7469 6d65 2073 6572   `-ts1` time ser
-00001e00: 6965 7320 6973 2073 656c 6563 7465 642e  ies is selected.
-00001e10: 0a0a 4669 6e61 6c6c 792c 206d 6574 7269  ..Finally, metri
-00001e20: 6373 2061 6e64 2066 6967 7572 6573 2074  cs and figures t
-00001e30: 6861 7420 6173 7365 7373 2074 6865 2073  hat assess the s
-00001e40: 696d 696c 6172 6974 7920 6265 7477 6565  imilarity betwee
-00001e50: 6e20 6561 6368 2070 6169 7220 6f66 2060  n each pair of `
-00001e60: 2d74 7332 6020 7469 6d65 2d73 6572 6965  -ts2` time-serie
-00001e70: 7320 6669 6c65 2061 6e64 2069 7473 0a61  s file and its.a
-00001e80: 7373 6f63 6961 7465 6420 6d6f 7374 2073  ssociated most s
-00001e90: 696d 696c 6172 2060 2d74 7331 6020 7769  imilar `-ts1` wi
-00001ea0: 6e64 6f77 2061 7265 2063 6f6d 7075 7465  ndow are compute
-00001eb0: 642e 0a0a 282a 2920 602d 775f 7365 6c65  d...(*) `-w_sele
-00001ec0: 6374 5f6d 6574 6020 6973 2074 6865 206d  ct_met` is the m
-00001ed0: 6574 7269 6320 7573 6564 2066 6f72 2074  etric used for t
-00001ee0: 6865 2073 656c 6563 7469 6f6e 206f 6620  he selection of 
-00001ef0: 7468 6520 6d6f 7374 0a73 696d 696c 6172  the most.similar
-00001f00: 2060 2d74 7331 6020 7469 6d65 2d73 6572   `-ts1` time-ser
-00001f10: 6965 7320 7769 6e64 6f77 2070 6572 2065  ies window per e
-00001f20: 6163 6820 602d 7473 3260 2074 696d 652d  ach `-ts2` time-
-00001f30: 7365 7269 6573 2066 696c 6528 7329 2e60  series file(s).`
-00001f40: 6474 7760 2069 7320 7468 6520 6465 6661  dtw` is the defa
-00001f50: 756c 7420 7661 6c75 652c 2068 6f77 6576  ult value, howev
-00001f60: 6572 2c20 616e 7920 6f66 0a74 6865 0a5b  er, any of.the.[
-00001f70: 6d65 7472 6963 735d 2823 6176 6169 6c61  metrics](#availa
-00001f80: 626c 652d 6d65 7472 6963 7329 2061 7265  ble-metrics) are
-00001f90: 2061 6c73 6f20 6176 6169 6c61 626c 6520   also available 
-00001fa0: 666f 7220 7468 6973 2070 7572 706f 7365  for this purpose
-00001fb0: 2075 7369 6e67 2074 6869 7320 6172 6775   using this argu
-00001fc0: 6d65 6e74 2e0a 0a55 7365 7273 2063 616e  ment...Users can
-00001fd0: 2070 726f 7669 6465 206d 6574 7269 6373   provide metrics
-00001fe0: 206f 7220 6669 6775 7265 7320 746f 2062   or figures to b
-00001ff0: 6520 636f 6d70 7574 6564 2f67 656e 6572  e computed/gener
-00002000: 6174 6564 3a0a 0a2d 2060 2d6d 6020 7468  ated:..- `-m` th
-00002010: 6520 5b6d 6574 7269 6373 5d28 2361 7661  e [metrics](#ava
-00002020: 696c 6162 6c65 2d6d 6574 7269 6373 2920  ilable-metrics) 
-00002030: 6e61 6d65 7320 746f 2062 6520 636f 6d70  names to be comp
-00002040: 7574 6564 2061 7320 6120 6c69 7374 2073  uted as a list s
-00002050: 6570 6172 6174 6564 2062 7920 7370 6163  eparated by spac
-00002060: 6573 2e0a 2d20 602d 6660 2074 6865 205b  es..- `-f` the [
-00002070: 6669 6775 7265 735d 2823 6176 6169 6c61  figures](#availa
-00002080: 626c 652d 6669 6775 7265 7329 206e 616d  ble-figures) nam
-00002090: 6573 2074 6f20 6265 2063 6f6d 7075 7465  es to be compute
-000020a0: 6420 6173 2061 206c 6973 7420 7365 7061  d as a list sepa
-000020b0: 7261 7465 6420 6279 2073 7061 6365 730a  rated by spaces.
-000020c0: 0a49 6620 6e6f 206d 6574 7269 6373 206e  .If no metrics n
-000020d0: 6f72 2066 6967 7572 6573 2061 7265 2070  or figures are p
-000020e0: 726f 7669 6465 642c 2074 6865 2074 6f6f  rovided, the too
-000020f0: 6c20 7769 6c6c 2063 6f6d 7075 7465 2061  l will compute a
-00002100: 6c6c 2074 6865 2061 7661 696c 6162 6c65  ll the available
-00002110: 206d 6574 7269 6373 2061 6e64 2066 6967   metrics and fig
-00002120: 7572 6573 2e0a 0a54 6865 2066 6f6c 6c6f  ures...The follo
-00002130: 7769 6e67 2061 7267 756d 656e 7473 2061  wing arguments a
-00002140: 7265 2061 6c73 6f20 6176 6169 6c61 626c  re also availabl
-00002150: 6520 666f 7220 6669 6e65 2d74 756e 696e  e for fine-tunin
-00002160: 673a 0a0a 2d20 602d 7473 5f66 7265 715f  g:..- `-ts_freq_
-00002170: 7365 6373 6020 7468 6520 6672 6571 7565  secs` the freque
-00002180: 6e63 7920 696e 2073 6563 6f6e 6473 2069  ncy in seconds i
-00002190: 6e20 7768 6963 6820 7361 6d70 6c65 7320  n which samples 
-000021a0: 7765 7265 2074 616b 656e 206a 7573 7420  were taken just 
-000021b0: 746f 2067 656e 6572 6174 6520 7468 6520  to generate the 
-000021c0: 6465 6c74 6120 6669 6775 7265 732e 2042  delta figures. B
-000021d0: 7920 6465 6661 756c 7420 6973 0a20 2060  y default is.  `
-000021e0: 3160 2073 6563 6f6e 642e 0a2d 2060 2d73  1` second..- `-s
-000021f0: 7472 6460 2077 6865 6e20 6074 7331 6020  trd` when `ts1` 
-00002200: 7469 6d65 2d73 6572 6965 7320 6973 206c  time-series is l
-00002210: 6f6e 6765 7220 7468 616e 2060 7473 3260  onger than `ts2`
-00002220: 2074 696d 652d 7365 7269 6573 2066 696c   time-series fil
-00002230: 6528 7329 2074 6865 2077 696e 646f 7773  e(s) the windows
-00002240: 2061 7265 2063 6f6d 7075 7465 6420 6279   are computed by
-00002250: 2075 7369 6e67 2061 0a20 2073 7472 6964   using a.  strid
-00002260: 6520 6f66 2060 3160 2062 7920 6465 6661  e of `1` by defa
-00002270: 756c 742e 2053 6f6d 6574 696d 6573 2075  ult. Sometimes u
-00002280: 7369 6e67 2061 206c 6172 6765 7220 7661  sing a larger va
-00002290: 6c75 6520 666f 7220 7468 6520 7374 7269  lue for the stri
-000022a0: 6465 2070 6172 616d 6574 6572 2069 6d70  de parameter imp
-000022b0: 726f 7665 7320 7468 6520 7065 7266 6f72  roves the perfor
-000022c0: 6d61 6e63 6520 6279 2073 6b69 7070 696e  mance by skippin
-000022d0: 670a 2020 7468 6520 636f 6d70 7574 6174  g.  the computat
-000022e0: 696f 6e20 6f66 2073 696d 696c 6172 6974  ion of similarit
-000022f0: 7920 6265 7477 6565 6e20 736f 206d 616e  y between so man
-00002300: 7920 7769 6e64 6f77 732e 0a0a 2323 2320  y windows...### 
-00002310: 4261 7369 6320 7573 6167 6520 6578 616d  Basic usage exam
-00002320: 706c 6573 3a0a 0a53 6f6d 6520 6578 616d  ples:..Some exam
-00002330: 706c 6573 206f 6620 6576 616c 7561 7469  ples of evaluati
-00002340: 6f6e 206f 6620 7369 6d69 6c61 7269 7479  on of similarity
-00002350: 2061 7265 2073 686f 776e 2062 656c 6f77   are shown below
-00002360: 2e20 596f 7520 6361 6e20 646f 776e 6c6f  . You can downlo
-00002370: 6164 2073 6f6d 6520 7465 7374 2064 6174  ad some test dat
-00002380: 6120 6279 2072 756e 6e69 6e67 2074 6865  a by running the
-00002390: 2066 6f6c 6c6f 7769 6e67 2063 6f6d 6d61   following comma
-000023a0: 6e64 3a0a 0a60 6060 4261 7368 0a77 6765  nd:..```Bash.wge
-000023b0: 7420 6874 7470 733a 2f2f 6769 7468 7562  t https://github
-000023c0: 2e63 6f6d 2f61 6c65 6a61 6e64 726f 6664  .com/alejandrofd
-000023d0: 657a 2d75 732f 7369 6d69 6c61 7269 7479  ez-us/similarity
-000023e0: 2d74 732d 636c 692f 7261 772f 6d61 696e  -ts-cli/raw/main
-000023f0: 2f64 6174 615f 7361 6d70 6c65 732e 7a69  /data_samples.zi
-00002400: 7020 2626 2075 6e7a 6970 2064 6174 615f  p && unzip data_
-00002410: 7361 6d70 6c65 732e 7a69 700a 6060 600a  samples.zip.```.
-00002420: 4f72 206d 616e 7561 6c6c 7920 646f 776e  Or manually down
-00002430: 6c6f 6164 2061 6e64 2075 6e7a 6970 2066  load and unzip f
-00002440: 726f 6d20 6874 7470 733a 2f2f 6769 7468  rom https://gith
-00002450: 7562 2e63 6f6d 2f61 6c65 6a61 6e64 726f  ub.com/alejandro
-00002460: 6664 657a 2d75 732f 7369 6d69 6c61 7269  fdez-us/similari
-00002470: 7479 2d74 732d 636c 692f 7261 772f 6d61  ty-ts-cli/raw/ma
-00002480: 696e 2f64 6174 615f 7361 6d70 6c65 732e  in/data_samples.
-00002490: 7a69 7020 2e0a 0a31 2e20 4120 7469 6d65  zip ...1. A time
-000024a0: 2073 6572 6965 7320 616e 6420 616c 6c20   series and all 
-000024b0: 7469 6d65 2073 6572 6965 7320 636f 6d70  time series comp
-000024c0: 7574 696e 6720 616c 6c20 6d65 7472 6963  uting all metric
-000024d0: 7320 616e 6420 6669 6775 7265 733a 0a20  s and figures:. 
-000024e0: 2020 2060 6060 4261 7368 0a20 2020 2073     ```Bash.    s
-000024f0: 696d 696c 6172 6974 792d 7473 2d63 6c69  imilarity-ts-cli
-00002500: 202d 7473 3120 6461 7461 5f73 616d 706c   -ts1 data_sampl
-00002510: 6573 2f61 6c69 6261 6261 3230 3138 2f74  es/alibaba2018/t
-00002520: 7331 5f6d 6163 6869 6e65 5f75 7361 6765  s1_machine_usage
-00002530: 5f64 6179 735f 315f 746f 5f38 5f67 726f  _days_1_to_8_gro
-00002540: 7570 6564 5f33 3030 5f73 6563 6f6e 6473  uped_300_seconds
-00002550: 2e63 7376 202d 7473 3220 6461 7461 5f73  .csv -ts2 data_s
-00002560: 616d 706c 6573 2f61 6c69 6261 6261 3230  amples/alibaba20
-00002570: 3138 2f74 7332 202d 6865 6164 0a20 2020  18/ts2 -head.   
-00002580: 2060 6060 0a20 2020 4576 6572 7920 6d65   ```.   Every me
-00002590: 7472 6963 2063 6f6d 7075 7461 7469 6f6e  tric computation
-000025a0: 2061 6e64 2066 6967 7572 6520 6765 6e65   and figure gene
-000025b0: 7261 7465 6420 7769 6c6c 2062 6520 666f  rated will be fo
-000025c0: 756e 6420 696e 2074 6865 2060 7265 7375  und in the `resu
-000025d0: 6c74 732f 7b74 696d 6573 7461 6d70 7d2f  lts/{timestamp}/
-000025e0: 6020 6469 7265 6374 6f72 792e 0a0a 312e  ` directory...1.
-000025f0: 2054 776f 2074 696d 6520 7365 7269 6573   Two time series
-00002600: 2063 6f6d 7075 7469 6e67 206f 6e6c 7920   computing only 
-00002610: 4454 5720 6d65 7472 6963 2061 6e64 2044  DTW metric and D
-00002620: 5457 2066 6967 7572 653a 0a20 2020 2060  TW figure:.    `
-00002630: 6060 4261 7368 0a20 2020 2073 696d 696c  ``Bash.    simil
-00002640: 6172 6974 792d 7473 2d63 6c69 202d 7473  arity-ts-cli -ts
-00002650: 3120 6461 7461 5f73 616d 706c 6573 2f61  1 data_samples/a
-00002660: 6c69 6261 6261 3230 3138 2f74 7331 5f6d  libaba2018/ts1_m
-00002670: 6163 6869 6e65 5f75 7361 6765 5f64 6179  achine_usage_day
-00002680: 735f 315f 746f 5f38 5f67 726f 7570 6564  s_1_to_8_grouped
-00002690: 5f33 3030 5f73 6563 6f6e 6473 2e63 7376  _300_seconds.csv
-000026a0: 202d 7473 3220 6461 7461 5f73 616d 706c   -ts2 data_sampl
-000026b0: 6573 2f61 6c69 6261 6261 3230 3138 2f74  es/alibaba2018/t
-000026c0: 7332 2f73 616d 706c 655f 302e 6373 7620  s2/sample_0.csv 
-000026d0: 2d68 6561 6420 2d6d 2064 7477 202d 6620  -head -m dtw -f 
-000026e0: 6474 770a 2020 2020 6060 600a 0a31 2e20  dtw.    ```..1. 
-000026f0: 5477 6f20 7469 6d65 2073 6572 6965 7320  Two time series 
-00002700: 636f 6d70 7574 696e 6720 6f6e 6c79 2044  computing only D
-00002710: 5457 206d 6574 7269 6320 616e 6420 4454  TW metric and DT
-00002720: 5720 6669 6775 7265 3a0a 2020 2020 6060  W figure:.    ``
-00002730: 6042 6173 680a 2020 2020 7369 6d69 6c61  `Bash.    simila
-00002740: 7269 7479 2d74 732d 636c 6920 2d74 7331  rity-ts-cli -ts1
-00002750: 2064 6174 615f 7361 6d70 6c65 732f 616c   data_samples/al
-00002760: 6962 6162 6132 3031 382f 7473 315f 6d61  ibaba2018/ts1_ma
-00002770: 6368 696e 655f 7573 6167 655f 6461 7973  chine_usage_days
-00002780: 5f31 5f74 6f5f 385f 6772 6f75 7065 645f  _1_to_8_grouped_
-00002790: 3330 305f 7365 636f 6e64 732e 6373 7620  300_seconds.csv 
-000027a0: 2d74 7332 2064 6174 615f 7361 6d70 6c65  -ts2 data_sample
-000027b0: 732f 616c 6962 6162 6132 3031 382f 7473  s/alibaba2018/ts
-000027c0: 322f 7361 6d70 6c65 5f30 2e63 7376 202d  2/sample_0.csv -
-000027d0: 6865 6164 202d 6d20 6474 7720 2d66 2064  head -m dtw -f d
-000027e0: 7477 0a20 2020 2060 6060 0a0a 312e 2041  tw.    ```..1. A
-000027f0: 2074 696d 6520 7365 7269 6573 2061 6e64   time series and
-00002800: 2061 6c6c 2074 696d 6520 7365 7269 6573   all time series
-00002810: 2077 6974 6869 6e20 6120 6469 7265 6374   within a direct
-00002820: 6f72 7920 636f 6d70 7574 696e 6720 6576  ory computing ev
-00002830: 6572 7920 6d65 7472 6963 2061 6e64 2066  ery metric and f
-00002840: 6967 7572 6520 696e 2053 696d 696c 6172  igure in Similar
-00002850: 6974 7954 5320 746f 6f6c 6b69 743a 0a20  ityTS toolkit:. 
-00002860: 2020 2060 6060 4261 7368 0a20 2020 2073     ```Bash.    s
-00002870: 696d 696c 6172 6974 792d 7473 2d63 6c69  imilarity-ts-cli
-00002880: 202d 7473 3120 6461 7461 5f73 616d 706c   -ts1 data_sampl
-00002890: 6573 2f61 6c69 6261 6261 3230 3138 2f74  es/alibaba2018/t
-000028a0: 7331 5f6d 6163 6869 6e65 5f75 7361 6765  s1_machine_usage
-000028b0: 5f64 6179 735f 315f 746f 5f38 5f67 726f  _days_1_to_8_gro
-000028c0: 7570 6564 5f33 3030 5f73 6563 6f6e 6473  uped_300_seconds
-000028d0: 2e63 7376 202d 7473 3220 6461 7461 5f73  .csv -ts2 data_s
-000028e0: 616d 706c 6573 2f61 6c69 6261 6261 3230  amples/alibaba20
-000028f0: 3138 2f74 7332 202d 6865 6164 202d 6d20  18/ts2 -head -m 
-00002900: 6a73 206d 6d64 2064 7477 206b 7320 6b6c  js mmd dtw ks kl
-00002910: 2063 6320 6370 2068 6920 2d66 2064 656c   cc cp hi -f del
-00002920: 7461 2064 7477 2032 6420 7063 6120 7473  ta dtw 2d pca ts
-00002930: 6e65 0a20 2020 2060 6060 0a0a 312e 2043  ne.    ```..1. C
-00002940: 6f6d 7061 7269 736f 6e20 6265 7477 6565  omparison betwee
-00002950: 6e20 7469 6d65 2073 6572 6965 7320 7370  n time series sp
-00002960: 6563 6966 7969 6e67 2074 6865 2066 7265  ecifying the fre
-00002970: 7175 656e 6379 2069 6e20 7365 636f 6e64  quency in second
-00002980: 7320 696e 2077 6869 6368 2073 616d 706c  s in which sampl
-00002990: 6573 2077 6572 6520 7461 6b65 6e3a 0a20  es were taken:. 
-000029a0: 2020 2060 6060 4261 7368 0a20 2020 2073     ```Bash.    s
-000029b0: 696d 696c 6172 6974 792d 7473 2d63 6c69  imilarity-ts-cli
-000029c0: 202d 7473 3120 6461 7461 5f73 616d 706c   -ts1 data_sampl
-000029d0: 6573 2f61 6c69 6261 6261 3230 3138 2f74  es/alibaba2018/t
-000029e0: 7331 5f6d 6163 6869 6e65 5f75 7361 6765  s1_machine_usage
-000029f0: 5f64 6179 735f 315f 746f 5f38 5f67 726f  _days_1_to_8_gro
-00002a00: 7570 6564 5f33 3030 5f73 6563 6f6e 6473  uped_300_seconds
-00002a10: 2e63 7376 202d 7473 3220 6461 7461 5f73  .csv -ts2 data_s
-00002a20: 616d 706c 6573 2f61 6c69 6261 6261 3230  amples/alibaba20
-00002a30: 3138 2f74 7332 202d 6865 6164 202d 6d20  18/ts2 -head -m 
-00002a40: 6474 7720 2d66 2064 7477 202d 7473 5f66  dtw -f dtw -ts_f
-00002a50: 7265 715f 7365 6373 2033 3030 0a20 2020  req_secs 300.   
-00002a60: 2060 6060 0a0a 312e 2043 6f6d 7061 7269   ```..1. Compari
-00002a70: 736f 6e20 6265 7477 6565 6e20 7469 6d65  son between time
-00002a80: 2073 6572 6965 7320 7370 6563 6966 7969   series specifyi
-00002a90: 6e67 2074 6865 2073 7472 6964 6520 7468  ng the stride th
-00002aa0: 6174 2064 6574 6572 6d69 6e65 7320 7468  at determines th
-00002ab0: 6520 7374 6570 206f 7220 6469 7374 616e  e step or distan
-00002ac0: 6365 2062 7920 7768 6963 6820 6120 6669  ce by which a fi
-00002ad0: 7865 642d 7369 7a65 0a20 2020 7769 6e64  xed-size.   wind
-00002ae0: 6f77 206d 6f76 6573 206f 7665 7220 7468  ow moves over th
-00002af0: 6520 6669 7273 7420 7469 6d65 2073 6572  e first time ser
-00002b00: 6965 733a 0a20 2020 2060 6060 4261 7368  ies:.    ```Bash
-00002b10: 0a20 2020 2073 696d 696c 6172 6974 792d  .    similarity-
-00002b20: 7473 2d63 6c69 202d 7473 3120 6461 7461  ts-cli -ts1 data
-00002b30: 5f73 616d 706c 6573 2f61 6c69 6261 6261  _samples/alibaba
-00002b40: 3230 3138 2f74 7331 5f6d 6163 6869 6e65  2018/ts1_machine
-00002b50: 5f75 7361 6765 5f64 6179 735f 315f 746f  _usage_days_1_to
-00002b60: 5f38 5f67 726f 7570 6564 5f33 3030 5f73  _8_grouped_300_s
-00002b70: 6563 6f6e 6473 2e63 7376 202d 7473 3220  econds.csv -ts2 
-00002b80: 6461 7461 5f73 616d 706c 6573 2f61 6c69  data_samples/ali
-00002b90: 6261 6261 3230 3138 2f74 7332 202d 6865  baba2018/ts2 -he
-00002ba0: 6164 202d 6d20 6474 7720 2d66 2064 7477  ad -m dtw -f dtw
-00002bb0: 202d 7374 7264 2035 0a20 2020 2060 6060   -strd 5.    ```
-00002bc0: 0a0a 312e 2043 6f6d 7061 7269 736f 6e20  ..1. Comparison 
-00002bd0: 6265 7477 6565 6e20 7469 6d65 2073 6572  between time ser
-00002be0: 6965 7320 7370 6563 6966 7969 6e67 2074  ies specifying t
-00002bf0: 6865 2077 696e 646f 7720 7365 6c65 6374  he window select
-00002c00: 696f 6e20 6d65 7472 6963 2074 6f20 6265  ion metric to be
-00002c10: 2075 7365 6420 7768 656e 2073 656c 6563   used when selec
-00002c20: 7469 6e67 2074 6865 206d 6f73 7420 7369  ting the most si
-00002c30: 6d69 6c61 720a 2020 2077 696e 646f 7773  milar.   windows
-00002c40: 2069 6e0a 2020 2074 6865 2066 6972 7374   in.   the first
-00002c50: 2074 696d 6520 7365 7269 6573 3a0a 0a20   time series:.. 
-00002c60: 2020 2060 6060 4261 7368 0a20 2020 2073     ```Bash.    s
-00002c70: 696d 696c 6172 6974 792d 7473 2d63 6c69  imilarity-ts-cli
-00002c80: 202d 7473 3120 6461 7461 5f73 616d 706c   -ts1 data_sampl
-00002c90: 6573 2f61 6c69 6261 6261 3230 3138 2f74  es/alibaba2018/t
-00002ca0: 7331 5f6d 6163 6869 6e65 5f75 7361 6765  s1_machine_usage
-00002cb0: 5f64 6179 735f 315f 746f 5f38 5f67 726f  _days_1_to_8_gro
-00002cc0: 7570 6564 5f33 3030 5f73 6563 6f6e 6473  uped_300_seconds
-00002cd0: 2e63 7376 202d 7473 3220 6461 7461 5f73  .csv -ts2 data_s
-00002ce0: 616d 706c 6573 2f61 6c69 6261 6261 3230  amples/alibaba20
-00002cf0: 3138 2f74 7332 202d 6865 6164 202d 6d20  18/ts2 -head -m 
-00002d00: 6474 7720 2d66 2064 7477 202d 775f 7365  dtw -f dtw -w_se
-00002d10: 6c65 6374 5f6d 6574 206a 730a 2020 2020  lect_met js.    
-00002d20: 6060 600a 0a31 2e20 5573 696e 6720 6f75  ```..1. Using ou
-00002d30: 7220 7361 6d70 6c65 2074 696d 6520 7365  r sample time se
-00002d40: 7269 6573 2074 6f20 636f 6d70 7574 6520  ries to compute 
-00002d50: 6576 6572 7920 7369 6e67 6c65 206d 6574  every single met
-00002d60: 7269 6320 616e 6420 6669 6775 7265 2077  ric and figure w
-00002d70: 6974 6820 6120 6669 7865 6420 7469 6d65  ith a fixed time
-00002d80: 7374 616d 7020 6672 6571 7565 6e63 7920  stamp frequency 
-00002d90: 616e 6420 7374 7269 6465 3a0a 0a20 2020  and stride:..   
-00002da0: 2060 6060 4261 7368 0a20 2020 2073 696d   ```Bash.    sim
-00002db0: 696c 6172 6974 792d 7473 2d63 6c69 202d  ilarity-ts-cli -
-00002dc0: 7473 3120 6461 7461 5f73 616d 706c 6573  ts1 data_samples
-00002dd0: 2f61 6c69 6261 6261 3230 3138 2f74 7331  /alibaba2018/ts1
-00002de0: 5f6d 6163 6869 6e65 5f75 7361 6765 5f64  _machine_usage_d
-00002df0: 6179 735f 315f 746f 5f38 5f67 726f 7570  ays_1_to_8_group
-00002e00: 6564 5f33 3030 5f73 6563 6f6e 6473 2e63  ed_300_seconds.c
-00002e10: 7376 202d 7473 3220 6461 7461 5f73 616d  sv -ts2 data_sam
-00002e20: 706c 6573 2f61 6c69 6261 6261 3230 3138  ples/alibaba2018
-00002e30: 2f74 7332 202d 6865 6164 202d 6d20 6d6d  /ts2 -head -m mm
-00002e40: 6420 6474 7720 6b73 206b 6c20 6363 2063  d dtw ks kl cc c
-00002e50: 7020 6869 202d 6620 6465 6c74 6120 6474  p hi -f delta dt
-00002e60: 7720 3264 2070 6361 2074 736e 6520 2d77  w 2d pca tsne -w
-00002e70: 5f73 656c 6563 745f 6d65 7420 6363 202d  _select_met cc -
-00002e80: 7473 5f66 7265 715f 7365 6373 2033 3030  ts_freq_secs 300
-00002e90: 202d 7374 7264 2035 0a20 2020 2060 6060   -strd 5.    ```
-00002ea0: 0a23 2320 4c69 6365 6e73 650a 0a53 696d  .## License..Sim
-00002eb0: 696c 6172 6974 7954 5320 746f 6f6c 6b69  ilarityTS toolki
-00002ec0: 7420 6973 2066 7265 6520 616e 6420 6f70  t is free and op
-00002ed0: 656e 2d73 6f75 7263 6520 736f 6674 7761  en-source softwa
-00002ee0: 7265 206c 6963 656e 7365 6420 756e 6465  re licensed unde
-00002ef0: 7220 7468 6520 5b4d 4954 206c 6963 656e  r the [MIT licen
-00002f00: 7365 5d28 4c49 4345 4e53 4529 2e0a       se](LICENSE)..
+00000350: 2d74 7329 2e20 5369 6d69 6c61 7269 7479  -ts). Similarity
+00000360: 2d54 5320 7061 636b 6167 6520 6661 6369  -TS package faci
+00000370: 6c69 7461 7465 7320 7468 6520 6576 616c  litates the eval
+00000380: 7561 7469 6f6e 2061 6e64 2063 6f6d 7061  uation and compa
+00000390: 7269 736f 6e20 6f66 0a6d 756c 7469 7661  rison of.multiva
+000003a0: 7269 6174 6520 7469 6d65 2073 6572 6965  riate time serie
+000003b0: 7320 6461 7461 2e20 4974 2070 726f 7669  s data. It provi
+000003c0: 6465 7320 6120 636f 6d70 7265 6865 6e73  des a comprehens
+000003d0: 6976 6520 746f 6f6c 6b69 7420 666f 7220  ive toolkit for 
+000003e0: 616e 616c 797a 696e 672c 2076 6973 7561  analyzing, visua
+000003f0: 6c69 7a69 6e67 2c20 616e 6420 7265 706f  lizing, and repo
+00000400: 7274 696e 6720 6d75 6c74 6970 6c65 0a6d  rting multiple.m
+00000410: 6574 7269 6373 2061 6e64 2066 6967 7572  etrics and figur
+00000420: 6573 2064 6572 6976 6564 2066 726f 6d20  es derived from 
+00000430: 7469 6d65 2073 6572 6965 7320 6461 7461  time series data
+00000440: 7365 7473 2e20 5468 6520 746f 6f6c 6b69  sets. The toolki
+00000450: 7420 7369 6d70 6c69 6669 6573 2074 6865  t simplifies the
+00000460: 2070 726f 6365 7373 206f 6620 6576 616c   process of eval
+00000470: 7561 7469 6e67 2074 6865 2073 696d 696c  uating the simil
+00000480: 6172 6974 7920 6f66 0a74 696d 6520 7365  arity of.time se
+00000490: 7269 6573 2062 7920 6f66 6665 7269 6e67  ries by offering
+000004a0: 2064 6174 6120 7072 6570 726f 6365 7373   data preprocess
+000004b0: 696e 672c 206d 6574 7269 6373 2063 6f6d  ing, metrics com
+000004c0: 7075 7461 7469 6f6e 2c20 7669 7375 616c  putation, visual
+000004d0: 697a 6174 696f 6e2c 2073 7461 7469 7374  ization, statist
+000004e0: 6963 616c 2061 6e61 6c79 7369 732c 2061  ical analysis, a
+000004f0: 6e64 2072 6570 6f72 7420 6765 6e65 7261  nd report genera
+00000500: 7469 6f6e 0a66 756e 6374 696f 6e61 6c69  tion.functionali
+00000510: 7469 6573 2e20 5769 7468 2069 7473 2063  ties. With its c
+00000520: 7573 746f 6d69 7a61 626c 6520 6665 6174  ustomizable feat
+00000530: 7572 6573 2c20 5369 6d69 6c61 7269 7479  ures, Similarity
+00000540: 5453 2065 6d70 6f77 6572 7320 7265 7365  TS empowers rese
+00000550: 6172 6368 6572 7320 616e 6420 6461 7461  archers and data
+00000560: 0a73 6369 656e 7469 7374 7320 746f 2067  .scientists to g
+00000570: 6169 6e20 696e 7369 6768 7473 2c20 6964  ain insights, id
+00000580: 656e 7469 6679 2070 6174 7465 726e 732c  entify patterns,
+00000590: 2061 6e64 206d 616b 6520 696e 666f 726d   and make inform
+000005a0: 6564 2064 6563 6973 696f 6e73 2062 6173  ed decisions bas
+000005b0: 6564 206f 6e20 7468 6569 7220 7469 6d65  ed on their time
+000005c0: 2073 6572 6965 7320 6461 7461 2e0a 0a54   series data...T
+000005d0: 6869 7320 636f 6d6d 616e 642d 6c69 6e65  his command-line
+000005e0: 2069 6e74 6572 6661 6365 2069 7320 4f53   interface is OS
+000005f0: 2069 6e64 6570 656e 6465 6e74 2061 6e64   independent and
+00000600: 2063 616e 2062 6520 6561 7369 6c79 2069   can be easily i
+00000610: 6e73 7461 6c6c 6564 2061 6e64 2075 7365  nstalled and use
+00000620: 642e 0a0a 2323 2320 4176 6169 6c61 626c  d...### Availabl
+00000630: 6520 6d65 7472 6963 730a 0a54 6869 7320  e metrics..This 
+00000640: 746f 6f6c 6b69 7420 6361 6e20 636f 6d70  toolkit can comp
+00000650: 7574 6520 7468 6520 666f 6c6c 6f77 696e  ute the followin
+00000660: 6720 6d65 7472 6963 733a 0a0a 2d20 606b  g metrics:..- `k
+00000670: 6c60 3a20 4b75 6c6c 6261 636b 2d4c 6569  l`: Kullback-Lei
+00000680: 626c 6572 2064 6976 6572 6765 6e63 650a  bler divergence.
+00000690: 2d20 606a 7360 3a20 4a65 6e73 656e 2d53  - `js`: Jensen-S
+000006a0: 6861 6e6e 6f6e 2064 6976 6572 6765 6e63  hannon divergenc
+000006b0: 650a 2d20 606b 7360 3a20 4b6f 6c6d 6f67  e.- `ks`: Kolmog
+000006c0: 6f72 6f76 2d53 6d69 726e 6f76 2074 6573  orov-Smirnov tes
+000006d0: 740a 2d20 606d 6d64 603a 204d 6178 696d  t.- `mmd`: Maxim
+000006e0: 756d 204d 6561 6e20 4469 7363 7265 7061  um Mean Discrepa
+000006f0: 6e63 790a 2d20 6064 7477 6020 4479 6e61  ncy.- `dtw` Dyna
+00000700: 6d69 6320 5469 6d65 2057 6172 7069 6e67  mic Time Warping
+00000710: 0a2d 2060 6363 603a 2044 6966 6665 7265  .- `cc`: Differe
+00000720: 6e63 6520 6f66 2063 6f2d 7661 7269 616e  nce of co-varian
+00000730: 6365 730a 2d20 6063 7060 3a20 4469 6666  ces.- `cp`: Diff
+00000740: 6572 656e 6365 206f 6620 636f 7272 656c  erence of correl
+00000750: 6174 696f 6e73 0a2d 2060 6869 603a 2044  ations.- `hi`: D
+00000760: 6966 6665 7265 6e63 6520 6f66 2068 6973  ifference of his
+00000770: 746f 6772 616d 730a 0a23 2323 2041 7661  tograms..### Ava
+00000780: 696c 6162 6c65 2066 6967 7572 6573 0a0a  ilable figures..
+00000790: 5468 6973 2074 6f6f 6c6b 6974 2063 616e  This toolkit can
+000007a0: 2067 656e 6572 6174 6520 7468 6520 666f   generate the fo
+000007b0: 6c6c 6f77 696e 6720 6669 6775 7265 733a  llowing figures:
+000007c0: 0a0a 2d20 6032 6460 3a20 7468 6520 6f72  ..- `2d`: the or
+000007d0: 6469 6e61 7279 2067 7261 7068 6963 616c  dinary graphical
+000007e0: 2072 6570 7265 7365 6e74 6174 696f 6e20   representation 
+000007f0: 6f66 2074 6865 2074 696d 6520 7365 7269  of the time seri
+00000800: 6573 2069 6e20 6120 3244 2066 6967 7572  es in a 2D figur
+00000810: 6520 7769 7468 2074 6865 2074 696d 6520  e with the time 
+00000820: 7265 7072 6573 656e 7465 6420 6f6e 2074  represented on t
+00000830: 6865 2078 2061 7869 730a 2020 616e 6420  he x axis.  and 
+00000840: 7468 6520 6461 7461 2076 616c 7565 7320  the data values 
+00000850: 6f6e 2074 6865 2079 2d61 7869 7320 666f  on the y-axis fo
+00000860: 720a 2020 2020 2d20 7468 6520 636f 6d70  r.    - the comp
+00000870: 6c65 7465 206d 756c 7469 7661 7269 6174  lete multivariat
+00000880: 6520 7469 6d65 2073 6572 6965 733b 2061  e time series; a
+00000890: 6e64 0a20 2020 202d 2061 2070 6c6f 7420  nd.    - a plot 
+000008a0: 7065 7220 636f 6c75 6d6e 2e0a 0a20 2045  per column...  E
+000008b0: 6163 6820 6765 6e65 7261 7465 6420 6669  ach generated fi
+000008c0: 6775 7265 2070 6c6f 7473 2062 6f74 6820  gure plots both 
+000008d0: 7468 6520 6074 7331 6020 616e 6420 7468  the `ts1` and th
+000008e0: 6520 6074 7332 6020 6461 7461 2074 6f20  e `ts2` data to 
+000008f0: 6561 7369 6c79 206f 6274 6169 6e20 6b65  easily obtain ke
+00000900: 7920 696e 7369 6768 7473 2069 6e74 6f0a  y insights into.
+00000910: 2020 7468 6520 7369 6d69 6c61 7269 7469    the similariti
+00000920: 6573 206f 7220 6469 6666 6572 656e 6365  es or difference
+00000930: 7320 6265 7477 6565 6e20 7468 656d 2e0a  s between them..
+00000940: 2020 2020 3c64 6976 3e0a 2020 2020 3c69      <div>.    <i
+00000950: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00000960: 6769 7468 7562 2e63 6f6d 2f61 6c65 6a61  github.com/aleja
+00000970: 6e64 726f 6664 657a 2d75 732f 7369 6d69  ndrofdez-us/simi
+00000980: 6c61 7269 7479 2d74 732f 626c 6f62 2f65  larity-ts/blob/e
+00000990: 3562 3134 3762 3134 3539 3730 6633 6139  5b147b145970f3a9
+000009a0: 3333 3531 6131 3030 3430 3232 6662 3330  3351a1004022fb30
+000009b0: 6432 3066 3566 302f 646f 6373 2f66 6967  d20f5f0/docs/fig
+000009c0: 7572 6573 2f32 645f 7361 6d70 6c65 5f33  ures/2d_sample_3
+000009d0: 5f63 6f6d 706c 6574 655f 5453 5f31 5f76  _complete_TS_1_v
+000009e0: 735f 5453 5f32 2e70 6e67 3f72 6177 3d74  s_TS_2.png?raw=t
+000009f0: 7275 6522 2061 6c74 3d22 3244 2046 6967  rue" alt="2D Fig
+00000a00: 7572 6520 636f 6d70 6c65 7465 223e 0a20  ure complete">. 
+00000a10: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
+00000a20: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000a30: 616c 656a 616e 6472 6f66 6465 7a2d 7573  alejandrofdez-us
+00000a40: 2f73 696d 696c 6172 6974 792d 7473 2f62  /similarity-ts/b
+00000a50: 6c6f 622f 6535 6231 3437 6231 3435 3937  lob/e5b147b14597
+00000a60: 3066 3361 3933 3335 3161 3130 3034 3032  0f3a93351a100402
+00000a70: 3266 6233 3064 3230 6635 6630 2f64 6f63  2fb30d20f5f0/doc
+00000a80: 732f 6669 6775 7265 732f 3264 5f73 616d  s/figures/2d_sam
+00000a90: 706c 655f 335f 6370 755f 7574 696c 5f70  ple_3_cpu_util_p
+00000aa0: 6572 6365 6e74 5f54 535f 315f 7673 5f54  ercent_TS_1_vs_T
+00000ab0: 535f 322e 706e 673f 7261 773d 7472 7565  S_2.png?raw=true
+00000ac0: 2220 616c 743d 2232 4420 4669 6775 7265  " alt="2D Figure
+00000ad0: 2066 6f72 2075 7365 6420 4350 5520 7065   for used CPU pe
+00000ae0: 7263 656e 7461 6765 223e 0a20 2020 203c  rcentage">.    <
+00000af0: 2f64 6976 3e0a 2d20 6064 656c 7461 603a  /div>.- `delta`:
+00000b00: 2074 6865 2064 6966 6665 7265 6e63 6573   the differences
+00000b10: 2062 6574 7765 656e 2074 6865 2076 616c   between the val
+00000b20: 7565 7320 6f66 2065 6163 6820 636f 6c75  ues of each colu
+00000b30: 6d6e 2067 726f 7570 6564 2062 7920 7065  mn grouped by pe
+00000b40: 7269 6f64 7320 6f66 2074 696d 652e 2046  riods of time. F
+00000b50: 6f72 2069 6e73 7461 6e63 652c 2074 6865  or instance, the
+00000b60: 2064 6966 6665 7265 6e63 6573 0a20 2062   differences.  b
+00000b70: 6574 7765 656e 2074 6865 2070 6572 6365  etween the perce
+00000b80: 6e74 6167 6520 6f66 2063 7075 2075 7365  ntage of cpu use
+00000b90: 6420 6576 6572 7920 3130 2c20 3235 206f  d every 10, 25 o
+00000ba0: 7220 3530 206d 696e 7574 6573 2e20 5468  r 50 minutes. Th
+00000bb0: 6573 6520 6465 6c74 6120 6361 6e20 6265  ese delta can be
+00000bc0: 2075 7365 6420 6173 2061 206d 6561 6e73   used as a means
+00000bd0: 206f 6620 636f 6d70 6172 6973 6f6e 2062   of comparison b
+00000be0: 6574 7765 656e 0a20 2074 696d 6520 7365  etween.  time se
+00000bf0: 7269 6573 2073 686f 7274 2d2f 6d69 642d  ries short-/mid-
+00000c00: 2f6c 6f6e 672d 7465 726d 2070 6174 7465  /long-term patte
+00000c10: 726e 732e 0a20 2020 203c 6469 763e 0a20  rns..    <div>. 
+00000c20: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
+00000c30: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000c40: 616c 656a 616e 6472 6f66 6465 7a2d 7573  alejandrofdez-us
+00000c50: 2f73 696d 696c 6172 6974 792d 7473 2f62  /similarity-ts/b
+00000c60: 6c6f 622f 6535 6231 3437 6231 3435 3937  lob/e5b147b14597
+00000c70: 3066 3361 3933 3335 3161 3130 3034 3032  0f3a93351a100402
+00000c80: 3266 6233 3064 3230 6635 6630 2f64 6f63  2fb30d20f5f0/doc
+00000c90: 732f 6669 6775 7265 732f 6465 6c74 615f  s/figures/delta_
+00000ca0: 7361 6d70 6c65 5f33 5f63 7075 5f75 7469  sample_3_cpu_uti
+00000cb0: 6c5f 7065 7263 656e 745f 5453 5f31 5f76  l_percent_TS_1_v
+00000cc0: 735f 5453 5f32 5f28 6772 6f75 7065 645f  s_TS_2_(grouped_
+00000cd0: 6279 5f31 305f 6d69 6e75 7465 7329 2e70  by_10_minutes).p
+00000ce0: 6e67 3f72 6177 3d74 7275 6522 2061 6c74  ng?raw=true" alt
+00000cf0: 3d22 4465 6c74 6120 4669 6775 7265 2066  ="Delta Figure f
+00000d00: 6f72 2075 7365 6420 4350 5520 7065 7263  or used CPU perc
+00000d10: 656e 7461 6765 2067 726f 7570 6564 2062  entage grouped b
+00000d20: 7920 3130 206d 696e 7574 6573 223e 0a20  y 10 minutes">. 
+00000d30: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
+00000d40: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000d50: 616c 656a 616e 6472 6f66 6465 7a2d 7573  alejandrofdez-us
+00000d60: 2f73 696d 696c 6172 6974 792d 7473 2f62  /similarity-ts/b
+00000d70: 6c6f 622f 6535 6231 3437 6231 3435 3937  lob/e5b147b14597
+00000d80: 3066 3361 3933 3335 3161 3130 3034 3032  0f3a93351a100402
+00000d90: 3266 6233 3064 3230 6635 6630 2f64 6f63  2fb30d20f5f0/doc
+00000da0: 732f 6669 6775 7265 732f 6465 6c74 615f  s/figures/delta_
+00000db0: 7361 6d70 6c65 5f33 5f63 7075 5f75 7469  sample_3_cpu_uti
+00000dc0: 6c5f 7065 7263 656e 745f 5453 5f31 5f76  l_percent_TS_1_v
+00000dd0: 735f 5453 5f32 5f28 6772 6f75 7065 645f  s_TS_2_(grouped_
+00000de0: 6279 5f32 355f 6d69 6e75 7465 7329 2e70  by_25_minutes).p
+00000df0: 6e67 3f72 6177 3d74 7275 6522 2061 6c74  ng?raw=true" alt
+00000e00: 3d22 4465 6c74 6120 4669 6775 7265 2066  ="Delta Figure f
+00000e10: 6f72 2075 7365 6420 4350 5520 7065 7263  or used CPU perc
+00000e20: 656e 7461 6765 2067 726f 7570 6564 2062  entage grouped b
+00000e30: 7920 3235 206d 696e 7574 6573 223e 0a20  y 25 minutes">. 
+00000e40: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
+00000e50: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000e60: 616c 656a 616e 6472 6f66 6465 7a2d 7573  alejandrofdez-us
+00000e70: 2f73 696d 696c 6172 6974 792d 7473 2f62  /similarity-ts/b
+00000e80: 6c6f 622f 6535 6231 3437 6231 3435 3937  lob/e5b147b14597
+00000e90: 3066 3361 3933 3335 3161 3130 3034 3032  0f3a93351a100402
+00000ea0: 3266 6233 3064 3230 6635 6630 2f64 6f63  2fb30d20f5f0/doc
+00000eb0: 732f 6669 6775 7265 732f 6465 6c74 615f  s/figures/delta_
+00000ec0: 7361 6d70 6c65 5f33 5f63 7075 5f75 7469  sample_3_cpu_uti
+00000ed0: 6c5f 7065 7263 656e 745f 5453 5f31 5f76  l_percent_TS_1_v
+00000ee0: 735f 5453 5f32 5f28 6772 6f75 7065 645f  s_TS_2_(grouped_
+00000ef0: 6279 5f35 305f 6d69 6e75 7465 7329 2e70  by_50_minutes).p
+00000f00: 6e67 3f72 6177 3d74 7275 6522 2061 6c74  ng?raw=true" alt
+00000f10: 3d22 4465 6c74 6120 4669 6775 7265 2066  ="Delta Figure f
+00000f20: 6f72 2075 7365 6420 4350 5520 7065 7263  or used CPU perc
+00000f30: 656e 7461 6765 2067 726f 7570 6564 2062  entage grouped b
+00000f40: 7920 3530 206d 696e 7574 6573 223e 0a20  y 50 minutes">. 
+00000f50: 2020 203c 2f64 6976 3e0a 0a2d 2060 7063     </div>..- `pc
+00000f60: 6160 3a20 7468 6520 6c69 6e65 6172 2064  a`: the linear d
+00000f70: 696d 656e 7369 6f6e 616c 6974 7920 7265  imensionality re
+00000f80: 6475 6374 696f 6e20 7465 6368 6e69 7175  duction techniqu
+00000f90: 6520 7468 6174 2061 696d 7320 746f 2066  e that aims to f
+00000fa0: 696e 6420 7468 6520 7072 696e 6369 7061  ind the principa
+00000fb0: 6c20 636f 6d70 6f6e 656e 7473 206f 6620  l components of 
+00000fc0: 6120 6461 7461 2073 6574 2062 790a 2020  a data set by.  
+00000fd0: 636f 6d70 7574 696e 6720 7468 6520 6c69  computing the li
+00000fe0: 6e65 6172 2063 6f6d 6269 6e61 7469 6f6e  near combination
+00000ff0: 7320 6f66 2074 6865 206f 7269 6769 6e61  s of the origina
+00001000: 6c20 6368 6172 6163 7465 7269 7374 6963  l characteristic
+00001010: 7320 7468 6174 2065 7870 6c61 696e 2074  s that explain t
+00001020: 6865 206d 6f73 7420 7661 7269 616e 6365  he most variance
+00001030: 2069 6e20 7468 6520 6461 7461 2e0a 2020   in the data..  
+00001040: 2020 3c64 6976 2061 6c69 676e 3d22 6365    <div align="ce
+00001050: 6e74 6572 223e 0a20 2020 203c 696d 6720  nter">.    <img 
+00001060: 7372 633d 2268 7474 7073 3a2f 2f67 6974  src="https://git
+00001070: 6875 622e 636f 6d2f 616c 656a 616e 6472  hub.com/alejandr
+00001080: 6f66 6465 7a2d 7573 2f73 696d 696c 6172  ofdez-us/similar
+00001090: 6974 792d 7473 2f62 6c6f 622f 6535 6231  ity-ts/blob/e5b1
+000010a0: 3437 6231 3435 3937 3066 3361 3933 3335  47b145970f3a9335
+000010b0: 3161 3130 3034 3032 3266 6233 3064 3230  1a1004022fb30d20
+000010c0: 6635 6630 2f64 6f63 732f 6669 6775 7265  f5f0/docs/figure
+000010d0: 732f 5043 412e 706e 673f 7261 773d 7472  s/PCA.png?raw=tr
+000010e0: 7565 2220 616c 743d 2250 4341 2046 6967  ue" alt="PCA Fig
+000010f0: 7572 6522 2077 6964 7468 3d22 3435 3022  ure" width="450"
+00001100: 3e0a 2020 2020 3c2f 6469 763e 0a2d 2060  >.    </div>.- `
+00001110: 7473 6e65 603a 2061 2074 6f6f 6c20 666f  tsne`: a tool fo
+00001120: 7220 7669 7375 616c 6973 696e 6720 6869  r visualising hi
+00001130: 6768 2d64 696d 656e 7369 6f6e 616c 2064  gh-dimensional d
+00001140: 6174 6120 7365 7473 2069 6e20 6120 3244  ata sets in a 2D
+00001150: 206f 7220 3344 2067 7261 7068 6963 616c   or 3D graphical
+00001160: 2072 6570 7265 7365 6e74 6174 696f 6e20   representation 
+00001170: 616c 6c6f 7769 6e67 2074 6865 2063 7265  allowing the cre
+00001180: 6174 696f 6e0a 2020 6f66 2061 2073 696e  ation.  of a sin
+00001190: 676c 6520 6d61 7020 7468 6174 2072 6576  gle map that rev
+000011a0: 6561 6c73 2074 6865 2073 7472 7563 7475  eals the structu
+000011b0: 7265 206f 6620 7468 6520 6461 7461 2061  re of the data a
+000011c0: 7420 6d61 6e79 2064 6966 6665 7265 6e74  t many different
+000011d0: 2073 6361 6c65 732e 0a20 2020 203c 6469   scales..    <di
+000011e0: 7620 616c 6967 6e3d 2263 656e 7465 7222  v align="center"
+000011f0: 3e0a 2020 2020 3c69 6d67 2073 7263 3d22  >.    <img src="
+00001200: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001210: 6f6d 2f61 6c65 6a61 6e64 726f 6664 657a  om/alejandrofdez
+00001220: 2d75 732f 7369 6d69 6c61 7269 7479 2d74  -us/similarity-t
+00001230: 732f 626c 6f62 2f65 3562 3134 3762 3134  s/blob/e5b147b14
+00001240: 3539 3730 6633 6139 3333 3531 6131 3030  5970f3a93351a100
+00001250: 3430 3232 6662 3330 6432 3066 3566 302f  4022fb30d20f5f0/
+00001260: 646f 6373 2f66 6967 7572 6573 2f74 2d53  docs/figures/t-S
+00001270: 4e45 2d69 7465 725f 3330 302d 7065 7270  NE-iter_300-perp
+00001280: 6c65 7869 7479 5f35 2e70 6e67 3f72 6177  lexity_5.png?raw
+00001290: 3d74 7275 6522 2061 6c74 3d22 5453 4e45  =true" alt="TSNE
+000012a0: 2046 6967 7572 6520 3330 3020 6974 6572   Figure 300 iter
+000012b0: 6174 696f 6e73 2035 2070 6572 706c 6578  ations 5 perplex
+000012c0: 6974 7922 2077 6964 7468 3d22 3435 3022  ity" width="450"
+000012d0: 3e0a 2020 2020 3c69 6d67 2073 7263 3d22  >.    <img src="
+000012e0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000012f0: 6f6d 2f61 6c65 6a61 6e64 726f 6664 657a  om/alejandrofdez
+00001300: 2d75 732f 7369 6d69 6c61 7269 7479 2d74  -us/similarity-t
+00001310: 732f 626c 6f62 2f65 3562 3134 3762 3134  s/blob/e5b147b14
+00001320: 3539 3730 6633 6139 3333 3531 6131 3030  5970f3a93351a100
+00001330: 3430 3232 6662 3330 6432 3066 3566 302f  4022fb30d20f5f0/
+00001340: 646f 6373 2f66 6967 7572 6573 2f74 2d53  docs/figures/t-S
+00001350: 4e45 2d69 7465 725f 3130 3030 2d70 6572  NE-iter_1000-per
+00001360: 706c 6578 6974 795f 352e 706e 673f 7261  plexity_5.png?ra
+00001370: 773d 7472 7565 2220 616c 743d 2254 534e  w=true" alt="TSN
+00001380: 4520 4669 6775 7265 2031 3030 3020 6974  E Figure 1000 it
+00001390: 6572 6174 696f 6e73 2035 2070 6572 706c  erations 5 perpl
+000013a0: 6578 6974 7922 2077 6964 7468 3d22 3435  exity" width="45
+000013b0: 3022 3e0a 2020 2020 3c2f 6469 763e 0a2d  0">.    </div>.-
+000013c0: 2060 6474 7760 2070 6174 683a 2049 6e20   `dtw` path: In 
+000013d0: 6164 6469 7469 6f6e 2074 6f20 7468 6520  addition to the 
+000013e0: 6e75 6d65 7269 6361 6c20 7369 6d69 6c61  numerical simila
+000013f0: 7269 7479 206d 6561 7375 7265 2c20 7468  rity measure, th
+00001400: 6520 6772 6170 6869 6361 6c20 7265 7072  e graphical repr
+00001410: 6573 656e 7461 7469 6f6e 206f 6620 7468  esentation of th
+00001420: 6520 4454 5720 7061 7468 206f 6620 6561  e DTW path of ea
+00001430: 6368 0a20 2063 6f6c 756d 6e20 6361 6e20  ch.  column can 
+00001440: 6265 2075 7365 6675 6c20 746f 2062 6574  be useful to bet
+00001450: 7465 7220 616e 616c 7973 6520 7468 6520  ter analyse the 
+00001460: 7369 6d69 6c61 7269 7469 6573 206f 7220  similarities or 
+00001470: 6469 6666 6572 656e 6365 7320 6265 7477  differences betw
+00001480: 6565 6e20 7468 6520 7469 6d65 2073 6572  een the time ser
+00001490: 6965 7320 636f 6c75 6d6e 732e 204e 6f74  ies columns. Not
+000014a0: 6963 6520 7468 6174 0a20 2074 6865 7265  ice that.  there
+000014b0: 2069 7320 6e6f 206d 756c 7469 7661 7269   is no multivari
+000014c0: 6174 6520 7265 7072 6573 656e 7461 7469  ate representati
+000014d0: 6f6e 206f 6620 4454 5720 7061 7468 732c  on of DTW paths,
+000014e0: 206f 6e6c 7920 7369 6e67 6c65 2063 6f6c   only single col
+000014f0: 756d 6e20 7265 7072 6573 656e 7461 7469  umn representati
+00001500: 6f6e 732e 0a20 2020 203c 6469 763e 0a20  ons..    <div>. 
+00001510: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
+00001520: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001530: 616c 656a 616e 6472 6f66 6465 7a2d 7573  alejandrofdez-us
+00001540: 2f73 696d 696c 6172 6974 792d 7473 2f62  /similarity-ts/b
+00001550: 6c6f 622f 6535 6231 3437 6231 3435 3937  lob/e5b147b14597
+00001560: 3066 3361 3933 3335 3161 3130 3034 3032  0f3a93351a100402
+00001570: 3266 6233 3064 3230 6635 6630 2f64 6f63  2fb30d20f5f0/doc
+00001580: 732f 6669 6775 7265 732f 4454 575f 7361  s/figures/DTW_sa
+00001590: 6d70 6c65 5f33 5f63 7075 5f75 7469 6c5f  mple_3_cpu_util_
+000015a0: 7065 7263 656e 742e 706e 673f 7261 773d  percent.png?raw=
+000015b0: 7472 7565 2220 616c 743d 2244 5457 2046  true" alt="DTW F
+000015c0: 6967 7572 6520 666f 7220 6370 7522 3e0a  igure for cpu">.
+000015d0: 2020 2020 3c2f 6469 763e 0a0a 2323 2049      </div>..## I
+000015e0: 6e73 7461 6c6c 6174 696f 6e0a 0a54 6f20  nstallation..To 
+000015f0: 696e 7374 616c 6c20 7468 6520 746f 6f6c  install the tool
+00001600: 2069 6e20 796f 7572 206c 6f63 616c 2065   in your local e
+00001610: 6e76 6972 6f6e 6d65 6e74 2c20 6a75 7374  nvironment, just
+00001620: 2072 756e 2066 6f6c 6c6f 7720 636f 6d6d   run follow comm
+00001630: 616e 643a 0a0a 6060 6042 6173 680a 7069  and:..```Bash.pi
+00001640: 7020 696e 7374 616c 6c20 7369 6d69 6c61  p install simila
+00001650: 7269 7479 2d74 732d 636c 6920 0a60 6060  rity-ts-cli .```
+00001660: 0a0a 2323 2055 7361 6765 0a0a 5573 6572  ..## Usage..User
+00001670: 7320 6d75 7374 2070 726f 7669 6465 2060  s must provide `
+00001680: 2e63 7376 6020 6669 6c65 7320 636f 6e74  .csv` files cont
+00001690: 6169 6e69 6e67 206d 756c 7469 7661 7269  aining multivari
+000016a0: 6174 6520 7469 6d65 2073 6572 6965 7320  ate time series 
+000016b0: 6279 2075 7369 6e67 2074 6865 2061 7267  by using the arg
+000016c0: 756d 656e 7473 2060 2d74 7331 6020 616e  uments `-ts1` an
+000016d0: 6420 602d 7473 3260 2e0a 0a2d 2060 2d74  d `-ts2`...- `-t
+000016e0: 7331 6020 7368 6f75 6c64 2070 6f69 6e74  s1` should point
+000016f0: 2074 6f20 6120 7369 6e67 6c65 2060 6373   to a single `cs
+00001700: 7660 2066 696c 656e 616d 652e 2054 6869  v` filename. Thi
+00001710: 7320 7469 6d65 2073 6572 6965 7320 6d61  s time series ma
+00001720: 7920 7265 7072 6573 656e 7420 7468 6520  y represent the 
+00001730: 6261 7365 6c69 6e65 206f 7220 6772 6f75  baseline or grou
+00001740: 6e64 2074 7275 7468 2074 696d 650a 2020  nd truth time.  
+00001750: 7365 7269 6573 2e0a 2d20 602d 7473 3260  series..- `-ts2`
+00001760: 2063 616e 2070 6f69 6e74 2074 6f20 616e   can point to an
+00001770: 6f74 6865 7220 7369 6e67 6c65 2060 6373  other single `cs
+00001780: 7660 2066 696c 656e 616d 6520 6f72 2061  v` filename or a
+00001790: 2064 6972 6563 746f 7279 2074 6861 7420   directory that 
+000017a0: 636f 6e74 6169 6e73 206d 756c 7469 706c  contains multipl
+000017b0: 6520 6063 7376 6020 6669 6c65 7320 746f  e `csv` files to
+000017c0: 2062 650a 2020 636f 6d70 6172 6564 2077   be.  compared w
+000017d0: 6974 6820 602d 7473 3160 2066 696c 652e  ith `-ts1` file.
+000017e0: 0a2d 2060 2d68 6561 6460 2069 6620 796f  .- `-head` if yo
+000017f0: 7572 2074 696d 6520 7365 7269 6573 2066  ur time series f
+00001800: 696c 6573 2069 6e63 6c75 6465 2061 2068  iles include a h
+00001810: 6561 6465 7220 7468 6973 2061 7267 756d  eader this argum
+00001820: 656e 7420 6d75 7374 2062 6520 7072 6573  ent must be pres
+00001830: 656e 742e 2049 6620 6e6f 7420 7072 6573  ent. If not pres
+00001840: 656e 742c 2074 6865 2073 6f66 7477 6172  ent, the softwar
+00001850: 650a 2020 756e 6465 7273 7461 6e64 7320  e.  understands 
+00001860: 7468 6174 2063 7376 2066 696c 6573 2064  that csv files d
+00001870: 6f6e 2774 2069 6e63 6c75 6465 2061 2068  on't include a h
+00001880: 6561 6465 7220 726f 772e 0a0a 436f 6e73  eader row...Cons
+00001890: 7472 6169 6e74 733a 0a0a 2d20 602d 7473  traints:..- `-ts
+000018a0: 3160 2074 696d 652d 7365 7269 6573 2066  1` time-series f
+000018b0: 696c 6520 616e 6420 602d 7473 3260 2074  ile and `-ts2` t
+000018c0: 696d 652d 7365 7269 6573 2066 696c 6528  ime-series file(
+000018d0: 7329 206d 7573 743a 0a20 2020 202d 2068  s) must:.    - h
+000018e0: 6176 6520 7468 6520 7361 6d65 2064 696d  ave the same dim
+000018f0: 656e 7369 6f6e 616c 6974 7920 286e 756d  ensionality (num
+00001900: 6265 7220 6f66 2063 6f6c 756d 6e73 290a  ber of columns).
+00001910: 2020 2020 2d20 6e6f 7420 696e 636c 7564      - not includ
+00001920: 6520 6120 7469 6d65 7374 616d 7020 636f  e a timestamp co
+00001930: 6c75 6d6e 0a20 2020 202d 2069 6e63 6c75  lumn.    - inclu
+00001940: 6465 206f 6e6c 7920 6e75 6d65 7269 6320  de only numeric 
+00001950: 7661 6c75 6573 0a20 2020 202d 2069 6e63  values.    - inc
+00001960: 6c75 6465 2074 6865 2073 616d 6520 6865  lude the same he
+00001970: 6164 6572 2028 6966 2070 7265 7365 6e74  ader (if present
+00001980: 290a 2d20 6966 2061 2068 6561 6465 7220  ).- if a header 
+00001990: 6973 2070 7265 7365 6e74 2061 7320 6669  is present as fi
+000019a0: 7273 7420 726f 772c 2075 7365 2074 6865  rst row, use the
+000019b0: 2060 2d68 6561 6460 2061 7267 756d 656e   `-head` argumen
+000019c0: 742e 0a2d 2061 6c6c 2060 2d74 7332 6020  t..- all `-ts2` 
+000019d0: 7469 6d65 2d73 6572 6965 7320 6669 6c65  time-series file
+000019e0: 7320 6d75 7374 2068 6176 6520 7468 6520  s must have the 
+000019f0: 7361 6d65 206c 656e 6774 6820 286e 756d  same length (num
+00001a00: 6265 7220 6f66 2072 6f77 7329 2e0a 0a4e  ber of rows)...N
+00001a10: 6f74 653a 2074 6865 2063 6f6c 756d 6e20  ote: the column 
+00001a20: 6465 6c69 6d69 7465 7220 6973 2061 7574  delimiter is aut
+00001a30: 6f6d 6174 6963 616c 6c79 2064 6574 6563  omatically detec
+00001a40: 7465 642e 0a0a 4966 2079 6f75 7220 6461  ted...If your da
+00001a50: 7461 2069 6e63 6c75 6465 2063 6174 6567  ta include categ
+00001a60: 6f72 6963 616c 2076 616c 7565 732c 2069  orical values, i
+00001a70: 7420 6d69 6768 7420 6265 2070 7265 2d70  t might be pre-p
+00001a80: 726f 6365 7373 6564 2074 6f20 636f 6e76  rocessed to conv
+00001a90: 6572 7420 7468 656d 2074 6f20 6e75 6d65  ert them to nume
+00001aa0: 7269 6361 6c20 7661 6c75 6573 2e20 416c  rical values. Al
+00001ab0: 6c20 6074 7332 7360 2074 696d 652d 7365  l `ts2s` time-se
+00001ac0: 7269 6573 206d 7573 7420 6861 7665 2074  ries must have t
+00001ad0: 6865 2073 616d 6520 6c65 6e67 7468 2028  he same length (
+00001ae0: 6e75 6d62 6572 206f 6620 726f 7773 292e  number of rows).
+00001af0: 0a0a 4966 2060 2d74 7331 6020 7469 6d65  ..If `-ts1` time
+00001b00: 2d73 6572 6965 7320 6669 6c65 2069 7320  -series file is 
+00001b10: 6c6f 6e67 6572 2028 6d6f 7265 2072 6f77  longer (more row
+00001b20: 7329 2074 6861 6e20 602d 7473 3260 2074  s) than `-ts2` t
+00001b30: 696d 652d 7365 7269 6573 2066 696c 6528  ime-series file(
+00001b40: 7329 2c20 7468 6520 602d 7473 3160 2074  s), the `-ts1` t
+00001b50: 696d 6520 7365 7269 6573 2077 696c 6c20  ime series will 
+00001b60: 6265 0a64 6976 6964 6564 2069 6e20 7769  be.divided in wi
+00001b70: 6e64 6f77 7320 6f66 2074 6865 2073 616d  ndows of the sam
+00001b80: 650a 6c65 6e67 7468 2061 7320 7468 6520  e.length as the 
+00001b90: 602d 7473 3260 2074 696d 652d 7365 7269  `-ts2` time-seri
+00001ba0: 6573 2066 696c 6528 7329 2e0a 0a46 6f72  es file(s)...For
+00001bb0: 2065 6163 6820 602d 7473 3260 2074 696d   each `-ts2` tim
+00001bc0: 652d 7365 7269 6573 2066 696c 652c 2074  e-series file, t
+00001bd0: 6865 206d 6f73 7420 7369 6d69 6c61 7220  he most similar 
+00001be0: 7769 6e64 6f77 2028 2a29 2066 726f 6d20  window (*) from 
+00001bf0: 602d 7473 3160 2074 696d 6520 7365 7269  `-ts1` time seri
+00001c00: 6573 2069 7320 7365 6c65 6374 6564 2e0a  es is selected..
+00001c10: 0a46 696e 616c 6c79 2c20 6d65 7472 6963  .Finally, metric
+00001c20: 7320 616e 6420 6669 6775 7265 7320 7468  s and figures th
+00001c30: 6174 2061 7373 6573 7320 7468 6520 7369  at assess the si
+00001c40: 6d69 6c61 7269 7479 2062 6574 7765 656e  milarity between
+00001c50: 2065 6163 6820 7061 6972 206f 6620 602d   each pair of `-
+00001c60: 7473 3260 2074 696d 652d 7365 7269 6573  ts2` time-series
+00001c70: 2066 696c 6520 616e 6420 6974 730a 6173   file and its.as
+00001c80: 736f 6369 6174 6564 206d 6f73 7420 7369  sociated most si
+00001c90: 6d69 6c61 7220 602d 7473 3160 2077 696e  milar `-ts1` win
+00001ca0: 646f 7720 6172 6520 636f 6d70 7574 6564  dow are computed
+00001cb0: 2e0a 0a28 2a29 2060 2d77 5f73 656c 6563  ...(*) `-w_selec
+00001cc0: 745f 6d65 7460 2069 7320 7468 6520 6d65  t_met` is the me
+00001cd0: 7472 6963 2075 7365 6420 666f 7220 7468  tric used for th
+00001ce0: 6520 7365 6c65 6374 696f 6e20 6f66 2074  e selection of t
+00001cf0: 6865 206d 6f73 740a 7369 6d69 6c61 7220  he most.similar 
+00001d00: 602d 7473 3160 2074 696d 652d 7365 7269  `-ts1` time-seri
+00001d10: 6573 2077 696e 646f 7720 7065 7220 6561  es window per ea
+00001d20: 6368 2060 2d74 7332 6020 7469 6d65 2d73  ch `-ts2` time-s
+00001d30: 6572 6965 7320 6669 6c65 2873 292e 6064  eries file(s).`d
+00001d40: 7477 6020 6973 2074 6865 2064 6566 6175  tw` is the defau
+00001d50: 6c74 2076 616c 7565 2c20 686f 7765 7665  lt value, howeve
+00001d60: 722c 2061 6e79 206f 660a 7468 650a 5b6d  r, any of.the.[m
+00001d70: 6574 7269 6373 5d28 2361 7661 696c 6162  etrics](#availab
+00001d80: 6c65 2d6d 6574 7269 6373 2920 6172 6520  le-metrics) are 
+00001d90: 616c 736f 2061 7661 696c 6162 6c65 2066  also available f
+00001da0: 6f72 2074 6869 7320 7075 7270 6f73 6520  or this purpose 
+00001db0: 7573 696e 6720 7468 6973 2061 7267 756d  using this argum
+00001dc0: 656e 742e 0a0a 5573 6572 7320 6361 6e20  ent...Users can 
+00001dd0: 7072 6f76 6964 6520 6d65 7472 6963 7320  provide metrics 
+00001de0: 6f72 2066 6967 7572 6573 2074 6f20 6265  or figures to be
+00001df0: 2063 6f6d 7075 7465 642f 6765 6e65 7261   computed/genera
+00001e00: 7465 643a 0a0a 2d20 602d 6d60 2074 6865  ted:..- `-m` the
+00001e10: 205b 6d65 7472 6963 735d 2823 6176 6169   [metrics](#avai
+00001e20: 6c61 626c 652d 6d65 7472 6963 7329 206e  lable-metrics) n
+00001e30: 616d 6573 2074 6f20 6265 2063 6f6d 7075  ames to be compu
+00001e40: 7465 6420 6173 2061 206c 6973 7420 7365  ted as a list se
+00001e50: 7061 7261 7465 6420 6279 2073 7061 6365  parated by space
+00001e60: 732e 0a2d 2060 2d66 6020 7468 6520 5b66  s..- `-f` the [f
+00001e70: 6967 7572 6573 5d28 2361 7661 696c 6162  igures](#availab
+00001e80: 6c65 2d66 6967 7572 6573 2920 6e61 6d65  le-figures) name
+00001e90: 7320 746f 2062 6520 636f 6d70 7574 6564  s to be computed
+00001ea0: 2061 7320 6120 6c69 7374 2073 6570 6172   as a list separ
+00001eb0: 6174 6564 2062 7920 7370 6163 6573 2e0a  ated by spaces..
+00001ec0: 0a49 6620 6e6f 206d 6574 7269 6373 206e  .If no metrics n
+00001ed0: 6f72 2066 6967 7572 6573 2061 7265 2070  or figures are p
+00001ee0: 726f 7669 6465 642c 2074 6865 2074 6f6f  rovided, the too
+00001ef0: 6c20 7769 6c6c 2063 6f6d 7075 7465 2061  l will compute a
+00001f00: 6c6c 2074 6865 2061 7661 696c 6162 6c65  ll the available
+00001f10: 206d 6574 7269 6373 2061 6e64 2066 6967   metrics and fig
+00001f20: 7572 6573 2e0a 0a54 6865 2066 6f6c 6c6f  ures...The follo
+00001f30: 7769 6e67 2061 7267 756d 656e 7473 2061  wing arguments a
+00001f40: 7265 2061 6c73 6f20 6176 6169 6c61 626c  re also availabl
+00001f50: 6520 666f 7220 6669 6e65 2d74 756e 696e  e for fine-tunin
+00001f60: 673a 0a0a 2d20 602d 7473 5f66 7265 715f  g:..- `-ts_freq_
+00001f70: 7365 6373 6020 7468 6520 6672 6571 7565  secs` the freque
+00001f80: 6e63 7920 696e 2073 6563 6f6e 6473 2069  ncy in seconds i
+00001f90: 6e20 7768 6963 6820 7361 6d70 6c65 7320  n which samples 
+00001fa0: 7765 7265 2074 616b 656e 206a 7573 7420  were taken just 
+00001fb0: 746f 2067 656e 6572 6174 6520 7468 6520  to generate the 
+00001fc0: 6465 6c74 6120 6669 6775 7265 732e 2042  delta figures. B
+00001fd0: 7920 6465 6661 756c 7420 6973 0a20 2060  y default is.  `
+00001fe0: 3160 2073 6563 6f6e 642e 0a2d 2060 2d73  1` second..- `-s
+00001ff0: 7472 6460 2077 6865 6e20 6074 7331 6020  trd` when `ts1` 
+00002000: 7469 6d65 2d73 6572 6965 7320 6973 206c  time-series is l
+00002010: 6f6e 6765 7220 7468 616e 2060 7473 3260  onger than `ts2`
+00002020: 2074 696d 652d 7365 7269 6573 2066 696c   time-series fil
+00002030: 6528 7329 2074 6865 2077 696e 646f 7773  e(s) the windows
+00002040: 2061 7265 2063 6f6d 7075 7465 6420 6279   are computed by
+00002050: 2075 7369 6e67 2061 0a20 2073 7472 6964   using a.  strid
+00002060: 6520 6f66 2060 3160 2062 7920 6465 6661  e of `1` by defa
+00002070: 756c 742e 2053 6f6d 6574 696d 6573 2075  ult. Sometimes u
+00002080: 7369 6e67 2061 206c 6172 6765 7220 7661  sing a larger va
+00002090: 6c75 6520 666f 7220 7468 6520 7374 7269  lue for the stri
+000020a0: 6465 2070 6172 616d 6574 6572 2069 6d70  de parameter imp
+000020b0: 726f 7665 7320 7468 6520 7065 7266 6f72  roves the perfor
+000020c0: 6d61 6e63 6520 6279 2073 6b69 7070 696e  mance by skippin
+000020d0: 670a 2020 7468 6520 636f 6d70 7574 6174  g.  the computat
+000020e0: 696f 6e20 6f66 2073 696d 696c 6172 6974  ion of similarit
+000020f0: 7920 6265 7477 6565 6e20 736f 206d 616e  y between so man
+00002100: 7920 7769 6e64 6f77 732e 0a0a 2323 2320  y windows...### 
+00002110: 4261 7369 6320 7573 6167 6520 6578 616d  Basic usage exam
+00002120: 706c 6573 3a0a 0a53 6f6d 6520 6578 616d  ples:..Some exam
+00002130: 706c 6573 206f 6620 6576 616c 7561 7469  ples of evaluati
+00002140: 6f6e 206f 6620 7369 6d69 6c61 7269 7479  on of similarity
+00002150: 2061 7265 2073 686f 776e 2062 656c 6f77   are shown below
+00002160: 2e20 596f 7520 6361 6e20 646f 776e 6c6f  . You can downlo
+00002170: 6164 2073 6f6d 6520 7465 7374 2064 6174  ad some test dat
+00002180: 6120 6279 2072 756e 6e69 6e67 2074 6865  a by running the
+00002190: 2066 6f6c 6c6f 7769 6e67 2063 6f6d 6d61   following comma
+000021a0: 6e64 3a0a 0a60 6060 4261 7368 0a77 6765  nd:..```Bash.wge
+000021b0: 7420 6874 7470 733a 2f2f 6769 7468 7562  t https://github
+000021c0: 2e63 6f6d 2f61 6c65 6a61 6e64 726f 6664  .com/alejandrofd
+000021d0: 657a 2d75 732f 7369 6d69 6c61 7269 7479  ez-us/similarity
+000021e0: 2d74 732d 636c 692f 7261 772f 6d61 696e  -ts-cli/raw/main
+000021f0: 2f64 6174 615f 7361 6d70 6c65 732e 7a69  /data_samples.zi
+00002200: 7020 2626 2075 6e7a 6970 2064 6174 615f  p && unzip data_
+00002210: 7361 6d70 6c65 732e 7a69 700a 6060 600a  samples.zip.```.
+00002220: 4f72 206d 616e 7561 6c6c 7920 646f 776e  Or manually down
+00002230: 6c6f 6164 2061 6e64 2075 6e7a 6970 2066  load and unzip f
+00002240: 726f 6d20 6874 7470 733a 2f2f 6769 7468  rom https://gith
+00002250: 7562 2e63 6f6d 2f61 6c65 6a61 6e64 726f  ub.com/alejandro
+00002260: 6664 657a 2d75 732f 7369 6d69 6c61 7269  fdez-us/similari
+00002270: 7479 2d74 732d 636c 692f 7261 772f 6d61  ty-ts-cli/raw/ma
+00002280: 696e 2f64 6174 615f 7361 6d70 6c65 732e  in/data_samples.
+00002290: 7a69 7020 2e0a 0a31 2e20 4120 7469 6d65  zip ...1. A time
+000022a0: 2073 6572 6965 7320 616e 6420 616c 6c20   series and all 
+000022b0: 7469 6d65 2073 6572 6965 7320 636f 6d70  time series comp
+000022c0: 7574 696e 6720 616c 6c20 6d65 7472 6963  uting all metric
+000022d0: 7320 616e 6420 6669 6775 7265 733a 0a20  s and figures:. 
+000022e0: 2020 2060 6060 4261 7368 0a20 2020 2073     ```Bash.    s
+000022f0: 696d 696c 6172 6974 792d 7473 2d63 6c69  imilarity-ts-cli
+00002300: 202d 7473 3120 6461 7461 5f73 616d 706c   -ts1 data_sampl
+00002310: 6573 2f61 6c69 6261 6261 3230 3138 2f74  es/alibaba2018/t
+00002320: 7331 5f6d 6163 6869 6e65 5f75 7361 6765  s1_machine_usage
+00002330: 5f64 6179 735f 315f 746f 5f38 5f67 726f  _days_1_to_8_gro
+00002340: 7570 6564 5f33 3030 5f73 6563 6f6e 6473  uped_300_seconds
+00002350: 2e63 7376 202d 7473 3220 6461 7461 5f73  .csv -ts2 data_s
+00002360: 616d 706c 6573 2f61 6c69 6261 6261 3230  amples/alibaba20
+00002370: 3138 2f74 7332 202d 6865 6164 0a20 2020  18/ts2 -head.   
+00002380: 2060 6060 0a20 2020 4576 6572 7920 6d65   ```.   Every me
+00002390: 7472 6963 2063 6f6d 7075 7461 7469 6f6e  tric computation
+000023a0: 2061 6e64 2066 6967 7572 6520 6765 6e65   and figure gene
+000023b0: 7261 7465 6420 7769 6c6c 2062 6520 666f  rated will be fo
+000023c0: 756e 6420 696e 2074 6865 2060 7265 7375  und in the `resu
+000023d0: 6c74 732f 7b74 696d 6573 7461 6d70 7d2f  lts/{timestamp}/
+000023e0: 6020 6469 7265 6374 6f72 792e 0a0a 312e  ` directory...1.
+000023f0: 2054 776f 2074 696d 6520 7365 7269 6573   Two time series
+00002400: 2063 6f6d 7075 7469 6e67 206f 6e6c 7920   computing only 
+00002410: 4454 5720 6d65 7472 6963 2061 6e64 2044  DTW metric and D
+00002420: 5457 2066 6967 7572 653a 0a20 2020 2060  TW figure:.    `
+00002430: 6060 4261 7368 0a20 2020 2073 696d 696c  ``Bash.    simil
+00002440: 6172 6974 792d 7473 2d63 6c69 202d 7473  arity-ts-cli -ts
+00002450: 3120 6461 7461 5f73 616d 706c 6573 2f61  1 data_samples/a
+00002460: 6c69 6261 6261 3230 3138 2f74 7331 5f6d  libaba2018/ts1_m
+00002470: 6163 6869 6e65 5f75 7361 6765 5f64 6179  achine_usage_day
+00002480: 735f 315f 746f 5f38 5f67 726f 7570 6564  s_1_to_8_grouped
+00002490: 5f33 3030 5f73 6563 6f6e 6473 2e63 7376  _300_seconds.csv
+000024a0: 202d 7473 3220 6461 7461 5f73 616d 706c   -ts2 data_sampl
+000024b0: 6573 2f61 6c69 6261 6261 3230 3138 2f74  es/alibaba2018/t
+000024c0: 7332 2f73 616d 706c 655f 302e 6373 7620  s2/sample_0.csv 
+000024d0: 2d68 6561 6420 2d6d 2064 7477 202d 6620  -head -m dtw -f 
+000024e0: 6474 770a 2020 2020 6060 600a 0a31 2e20  dtw.    ```..1. 
+000024f0: 4120 7469 6d65 2073 6572 6965 7320 616e  A time series an
+00002500: 6420 616c 6c20 7469 6d65 2073 6572 6965  d all time serie
+00002510: 7320 7769 7468 696e 2061 2064 6972 6563  s within a direc
+00002520: 746f 7279 2063 6f6d 7075 7469 6e67 2065  tory computing e
+00002530: 7665 7279 206d 6574 7269 6320 616e 6420  very metric and 
+00002540: 6669 6775 7265 2069 6e20 5369 6d69 6c61  figure in Simila
+00002550: 7269 7479 5453 2074 6f6f 6c6b 6974 3a0a  rityTS toolkit:.
+00002560: 2020 2020 6060 6042 6173 680a 2020 2020      ```Bash.    
+00002570: 7369 6d69 6c61 7269 7479 2d74 732d 636c  similarity-ts-cl
+00002580: 6920 2d74 7331 2064 6174 615f 7361 6d70  i -ts1 data_samp
+00002590: 6c65 732f 616c 6962 6162 6132 3031 382f  les/alibaba2018/
+000025a0: 7473 315f 6d61 6368 696e 655f 7573 6167  ts1_machine_usag
+000025b0: 655f 6461 7973 5f31 5f74 6f5f 385f 6772  e_days_1_to_8_gr
+000025c0: 6f75 7065 645f 3330 305f 7365 636f 6e64  ouped_300_second
+000025d0: 732e 6373 7620 2d74 7332 2064 6174 615f  s.csv -ts2 data_
+000025e0: 7361 6d70 6c65 732f 616c 6962 6162 6132  samples/alibaba2
+000025f0: 3031 382f 7473 3220 2d68 6561 6420 2d6d  018/ts2 -head -m
+00002600: 206a 7320 6d6d 6420 6474 7720 6b73 206b   js mmd dtw ks k
+00002610: 6c20 6363 2063 7020 6869 202d 6620 6465  l cc cp hi -f de
+00002620: 6c74 6120 6474 7720 3264 2070 6361 2074  lta dtw 2d pca t
+00002630: 736e 650a 2020 2020 6060 600a 0a31 2e20  sne.    ```..1. 
+00002640: 436f 6d70 6172 6973 6f6e 2062 6574 7765  Comparison betwe
+00002650: 656e 2074 696d 6520 7365 7269 6573 2073  en time series s
+00002660: 7065 6369 6679 696e 6720 7468 6520 6672  pecifying the fr
+00002670: 6571 7565 6e63 7920 696e 2073 6563 6f6e  equency in secon
+00002680: 6473 2069 6e20 7768 6963 6820 7361 6d70  ds in which samp
+00002690: 6c65 7320 7765 7265 2074 616b 656e 3a0a  les were taken:.
+000026a0: 2020 2020 6060 6042 6173 680a 2020 2020      ```Bash.    
+000026b0: 7369 6d69 6c61 7269 7479 2d74 732d 636c  similarity-ts-cl
+000026c0: 6920 2d74 7331 2064 6174 615f 7361 6d70  i -ts1 data_samp
+000026d0: 6c65 732f 616c 6962 6162 6132 3031 382f  les/alibaba2018/
+000026e0: 7473 315f 6d61 6368 696e 655f 7573 6167  ts1_machine_usag
+000026f0: 655f 6461 7973 5f31 5f74 6f5f 385f 6772  e_days_1_to_8_gr
+00002700: 6f75 7065 645f 3330 305f 7365 636f 6e64  ouped_300_second
+00002710: 732e 6373 7620 2d74 7332 2064 6174 615f  s.csv -ts2 data_
+00002720: 7361 6d70 6c65 732f 616c 6962 6162 6132  samples/alibaba2
+00002730: 3031 382f 7473 3220 2d68 6561 6420 2d6d  018/ts2 -head -m
+00002740: 2064 7477 202d 6620 6474 7720 2d74 735f   dtw -f dtw -ts_
+00002750: 6672 6571 5f73 6563 7320 3330 300a 2020  freq_secs 300.  
+00002760: 2020 6060 600a 0a31 2e20 436f 6d70 6172    ```..1. Compar
+00002770: 6973 6f6e 2062 6574 7765 656e 2074 696d  ison between tim
+00002780: 6520 7365 7269 6573 2073 7065 6369 6679  e series specify
+00002790: 696e 6720 7468 6520 7374 7269 6465 2074  ing the stride t
+000027a0: 6861 7420 6465 7465 726d 696e 6573 2074  hat determines t
+000027b0: 6865 2073 7465 7020 6f72 2064 6973 7461  he step or dista
+000027c0: 6e63 6520 6279 2077 6869 6368 2061 2066  nce by which a f
+000027d0: 6978 6564 2d73 697a 650a 2020 2077 696e  ixed-size.   win
+000027e0: 646f 7720 6d6f 7665 7320 6f76 6572 2074  dow moves over t
+000027f0: 6865 2066 6972 7374 2074 696d 6520 7365  he first time se
+00002800: 7269 6573 3a0a 2020 2020 6060 6042 6173  ries:.    ```Bas
+00002810: 680a 2020 2020 7369 6d69 6c61 7269 7479  h.    similarity
+00002820: 2d74 732d 636c 6920 2d74 7331 2064 6174  -ts-cli -ts1 dat
+00002830: 615f 7361 6d70 6c65 732f 616c 6962 6162  a_samples/alibab
+00002840: 6132 3031 382f 7473 315f 6d61 6368 696e  a2018/ts1_machin
+00002850: 655f 7573 6167 655f 6461 7973 5f31 5f74  e_usage_days_1_t
+00002860: 6f5f 385f 6772 6f75 7065 645f 3330 305f  o_8_grouped_300_
+00002870: 7365 636f 6e64 732e 6373 7620 2d74 7332  seconds.csv -ts2
+00002880: 2064 6174 615f 7361 6d70 6c65 732f 616c   data_samples/al
+00002890: 6962 6162 6132 3031 382f 7473 3220 2d68  ibaba2018/ts2 -h
+000028a0: 6561 6420 2d6d 2064 7477 202d 6620 6474  ead -m dtw -f dt
+000028b0: 7720 2d73 7472 6420 350a 2020 2020 6060  w -strd 5.    ``
+000028c0: 600a 0a31 2e20 436f 6d70 6172 6973 6f6e  `..1. Comparison
+000028d0: 2062 6574 7765 656e 2074 696d 6520 7365   between time se
+000028e0: 7269 6573 2073 7065 6369 6679 696e 6720  ries specifying 
+000028f0: 7468 6520 7769 6e64 6f77 2073 656c 6563  the window selec
+00002900: 7469 6f6e 206d 6574 7269 6320 746f 2062  tion metric to b
+00002910: 6520 7573 6564 2077 6865 6e20 7365 6c65  e used when sele
+00002920: 6374 696e 6720 7468 6520 6d6f 7374 2073  cting the most s
+00002930: 696d 696c 6172 0a20 2020 7769 6e64 6f77  imilar.   window
+00002940: 7320 696e 0a20 2020 7468 6520 6669 7273  s in.   the firs
+00002950: 7420 7469 6d65 2073 6572 6965 733a 0a0a  t time series:..
+00002960: 2020 2020 6060 6042 6173 680a 2020 2020      ```Bash.    
+00002970: 7369 6d69 6c61 7269 7479 2d74 732d 636c  similarity-ts-cl
+00002980: 6920 2d74 7331 2064 6174 615f 7361 6d70  i -ts1 data_samp
+00002990: 6c65 732f 616c 6962 6162 6132 3031 382f  les/alibaba2018/
+000029a0: 7473 315f 6d61 6368 696e 655f 7573 6167  ts1_machine_usag
+000029b0: 655f 6461 7973 5f31 5f74 6f5f 385f 6772  e_days_1_to_8_gr
+000029c0: 6f75 7065 645f 3330 305f 7365 636f 6e64  ouped_300_second
+000029d0: 732e 6373 7620 2d74 7332 2064 6174 615f  s.csv -ts2 data_
+000029e0: 7361 6d70 6c65 732f 616c 6962 6162 6132  samples/alibaba2
+000029f0: 3031 382f 7473 3220 2d68 6561 6420 2d6d  018/ts2 -head -m
+00002a00: 2064 7477 202d 6620 6474 7720 2d77 5f73   dtw -f dtw -w_s
+00002a10: 656c 6563 745f 6d65 7420 6a73 0a20 2020  elect_met js.   
+00002a20: 2060 6060 0a0a 312e 2055 7369 6e67 206f   ```..1. Using o
+00002a30: 7572 2073 616d 706c 6520 7469 6d65 2073  ur sample time s
+00002a40: 6572 6965 7320 746f 2063 6f6d 7075 7465  eries to compute
+00002a50: 2065 7665 7279 2073 696e 676c 6520 6d65   every single me
+00002a60: 7472 6963 2061 6e64 2066 6967 7572 6520  tric and figure 
+00002a70: 7769 7468 2061 2066 6978 6564 2074 696d  with a fixed tim
+00002a80: 6573 7461 6d70 2066 7265 7175 656e 6379  estamp frequency
+00002a90: 2061 6e64 2073 7472 6964 653a 0a0a 2020   and stride:..  
+00002aa0: 2020 6060 6042 6173 680a 2020 2020 7369    ```Bash.    si
+00002ab0: 6d69 6c61 7269 7479 2d74 732d 636c 6920  milarity-ts-cli 
+00002ac0: 2d74 7331 2064 6174 615f 7361 6d70 6c65  -ts1 data_sample
+00002ad0: 732f 616c 6962 6162 6132 3031 382f 7473  s/alibaba2018/ts
+00002ae0: 315f 6d61 6368 696e 655f 7573 6167 655f  1_machine_usage_
+00002af0: 6461 7973 5f31 5f74 6f5f 385f 6772 6f75  days_1_to_8_grou
+00002b00: 7065 645f 3330 305f 7365 636f 6e64 732e  ped_300_seconds.
+00002b10: 6373 7620 2d74 7332 2064 6174 615f 7361  csv -ts2 data_sa
+00002b20: 6d70 6c65 732f 616c 6962 6162 6132 3031  mples/alibaba201
+00002b30: 382f 7473 3220 2d68 6561 6420 2d6d 206d  8/ts2 -head -m m
+00002b40: 6d64 2064 7477 206b 7320 6b6c 2063 6320  md dtw ks kl cc 
+00002b50: 6370 2068 6920 2d66 2064 656c 7461 2064  cp hi -f delta d
+00002b60: 7477 2032 6420 7063 6120 7473 6e65 202d  tw 2d pca tsne -
+00002b70: 775f 7365 6c65 6374 5f6d 6574 2063 6320  w_select_met cc 
+00002b80: 2d74 735f 6672 6571 5f73 6563 7320 3330  -ts_freq_secs 30
+00002b90: 3020 2d73 7472 6420 350a 2020 2020 6060  0 -strd 5.    ``
+00002ba0: 600a 2323 204c 6963 656e 7365 0a0a 5369  `.## License..Si
+00002bb0: 6d69 6c61 7269 7479 5453 2074 6f6f 6c6b  milarityTS toolk
+00002bc0: 6974 2069 7320 6672 6565 2061 6e64 206f  it is free and o
+00002bd0: 7065 6e2d 736f 7572 6365 2073 6f66 7477  pen-source softw
+00002be0: 6172 6520 6c69 6365 6e73 6564 2075 6e64  are licensed und
+00002bf0: 6572 2074 6865 205b 4d49 5420 6c69 6365  er the [MIT lice
+00002c00: 6e73 655d 284c 4943 454e 5345 292e 0a0a  nse](LICENSE)...
+00002c10: 2323 2041 636b 6e6f 776c 6564 6765 6d65  ## Acknowledgeme
+00002c20: 6e74 730a 5072 6f6a 6563 7420 5049 4432  nts.Project PID2
+00002c30: 3032 312d 3132 3232 3038 4f42 2d49 3030  021-122208OB-I00
+00002c40: 2c20 5052 4f59 4558 4345 4c5c 5f30 3032  , PROYEXCEL\_002
+00002c50: 3836 2061 6e64 2020 5445 4432 3032 312d  86 and  TED2021-
+00002c60: 3133 3236 3935 422d 4930 3020 7072 6f6a  132695B-I00 proj
+00002c70: 6563 742c 2066 756e 6465 6420 6279 204d  ect, funded by M
+00002c80: 4349 4e20 2f20 4145 4920 2f20 3130 2e31  CIN / AEI / 10.1
+00002c90: 3330 3339 202f 2035 3031 3130 3030 3131  3039 / 501100011
+00002ca0: 3033 332c 2062 7920 416e 6461 6c75 7369  033, by Andalusi
+00002cb0: 616e 2052 6567 696f 6e61 6c20 476f 7665  an Regional Gove
+00002cc0: 726e 6d65 6e74 2c20 616e 6420 6279 2074  rnment, and by t
+00002cd0: 6865 2045 7572 6f70 6561 6e20 556e 696f  he European Unio
+00002ce0: 6e20 2d20 4e65 7874 4765 6e65 7261 7469  n - NextGenerati
+00002cf0: 6f6e 4555 2e                             onEU.
```

