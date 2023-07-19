# Comparing `tmp/similarity_ts-1.0.2.tar.gz` & `tmp/similarity_ts-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "similarity_ts-1.0.2.tar", last modified: Tue Jul 18 06:26:24 2023, max compression
+gzip compressed data, was "similarity_ts-1.0.3.tar", last modified: Wed Jul 19 11:49:19 2023, max compression
```

## Comparing `similarity_ts-1.0.2.tar` & `similarity_ts-1.0.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-18 06:26:24.145019 similarity_ts-1.0.2/
--rw-r--r--   0 afdez      (501) staff       (20)     1079 2023-07-16 10:03:12.000000 similarity_ts-1.0.2/LICENSE
--rw-r--r--   0 afdez      (501) staff       (20)    17150 2023-07-18 06:26:24.144744 similarity_ts-1.0.2/PKG-INFO
--rw-r--r--   0 afdez      (501) staff       (20)    16422 2023-07-18 06:26:01.000000 similarity_ts-1.0.2/README.md
--rw-r--r--   0 afdez      (501) staff       (20)      959 2023-07-18 06:26:16.000000 similarity_ts-1.0.2/pyproject.toml
--rw-r--r--   0 afdez      (501) staff       (20)       38 2023-07-18 06:26:24.145078 similarity_ts-1.0.2/setup.cfg
-drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-18 06:26:24.131829 similarity_ts-1.0.2/src/
-drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-18 06:26:24.134630 similarity_ts-1.0.2/src/similarity_ts/
--rw-r--r--   0 afdez      (501) staff       (20)        0 2023-07-14 15:40:23.000000 similarity_ts-1.0.2/src/similarity_ts/__init__.py
-drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-18 06:26:24.137418 similarity_ts-1.0.2/src/similarity_ts/helpers/
--rw-r--r--   0 afdez      (501) staff       (20)        0 2023-07-14 15:40:23.000000 similarity_ts-1.0.2/src/similarity_ts/helpers/__init__.py
--rw-r--r--   0 afdez      (501) staff       (20)     2161 2023-07-17 10:38:41.000000 similarity_ts-1.0.2/src/similarity_ts/helpers/csv_reader_helper.py
--rw-r--r--   0 afdez      (501) staff       (20)     1113 2023-07-16 14:24:04.000000 similarity_ts-1.0.2/src/similarity_ts/helpers/dynamic_import_helper.py
--rw-r--r--   0 afdez      (501) staff       (20)     1928 2023-07-17 11:05:25.000000 similarity_ts-1.0.2/src/similarity_ts/helpers/window_sampler.py
-drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-18 06:26:24.141303 similarity_ts-1.0.2/src/similarity_ts/metrics/
--rw-r--r--   0 afdez      (501) staff       (20)        0 2023-07-14 15:40:23.000000 similarity_ts-1.0.2/src/similarity_ts/metrics/__init__.py
--rw-r--r--   0 afdez      (501) staff       (20)      669 2023-07-17 10:39:19.000000 similarity_ts-1.0.2/src/similarity_ts/metrics/cc.py
--rw-r--r--   0 afdez      (501) staff       (20)      637 2023-07-17 10:39:19.000000 similarity_ts-1.0.2/src/similarity_ts/metrics/cp.py
--rw-r--r--   0 afdez      (501) staff       (20)     1164 2023-07-17 11:15:50.000000 similarity_ts-1.0.2/src/similarity_ts/metrics/dtw.py
--rw-r--r--   0 afdez      (501) staff       (20)     1430 2023-07-17 11:15:50.000000 similarity_ts-1.0.2/src/similarity_ts/metrics/hi.py
--rw-r--r--   0 afdez      (501) staff       (20)     1065 2023-07-17 11:15:50.000000 similarity_ts-1.0.2/src/similarity_ts/metrics/js.py
--rw-r--r--   0 afdez      (501) staff       (20)     3999 2023-07-17 11:15:50.000000 similarity_ts-1.0.2/src/similarity_ts/metrics/kl.py
--rw-r--r--   0 afdez      (501) staff       (20)      889 2023-07-17 11:15:50.000000 similarity_ts-1.0.2/src/similarity_ts/metrics/ks.py
--rw-r--r--   0 afdez      (501) staff       (20)      350 2023-07-17 10:39:19.000000 similarity_ts-1.0.2/src/similarity_ts/metrics/metric.py
--rw-r--r--   0 afdez      (501) staff       (20)      798 2023-07-17 10:39:19.000000 similarity_ts-1.0.2/src/similarity_ts/metrics/metric_computer.py
--rw-r--r--   0 afdez      (501) staff       (20)      321 2023-07-14 17:03:35.000000 similarity_ts-1.0.2/src/similarity_ts/metrics/metric_config.py
--rw-r--r--   0 afdez      (501) staff       (20)     1552 2023-07-17 07:05:11.000000 similarity_ts-1.0.2/src/similarity_ts/metrics/metric_factory.py
--rw-r--r--   0 afdez      (501) staff       (20)     1011 2023-07-17 11:15:50.000000 similarity_ts-1.0.2/src/similarity_ts/metrics/mmd.py
-drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-18 06:26:24.144364 similarity_ts-1.0.2/src/similarity_ts/plots/
--rw-r--r--   0 afdez      (501) staff       (20)        0 2023-07-14 15:40:23.000000 similarity_ts-1.0.2/src/similarity_ts/plots/__init__.py
--rw-r--r--   0 afdez      (501) staff       (20)     4295 2023-07-14 17:42:31.000000 similarity_ts-1.0.2/src/similarity_ts/plots/delta.py
--rw-r--r--   0 afdez      (501) staff       (20)     1064 2023-07-14 17:09:09.000000 similarity_ts-1.0.2/src/similarity_ts/plots/dimensionalty_reduction.py
--rw-r--r--   0 afdez      (501) staff       (20)     1129 2023-07-14 17:18:51.000000 similarity_ts-1.0.2/src/similarity_ts/plots/dtw.py
--rw-r--r--   0 afdez      (501) staff       (20)     1464 2023-07-14 17:18:51.000000 similarity_ts-1.0.2/src/similarity_ts/plots/pca.py
--rw-r--r--   0 afdez      (501) staff       (20)     1162 2023-07-14 17:18:51.000000 similarity_ts-1.0.2/src/similarity_ts/plots/plot.py
--rw-r--r--   0 afdez      (501) staff       (20)      976 2023-07-14 17:56:55.000000 similarity_ts-1.0.2/src/similarity_ts/plots/plot_computer.py
--rw-r--r--   0 afdez      (501) staff       (20)      518 2023-07-14 17:10:27.000000 similarity_ts-1.0.2/src/similarity_ts/plots/plot_config.py
--rw-r--r--   0 afdez      (501) staff       (20)     1681 2023-07-17 07:05:11.000000 similarity_ts-1.0.2/src/similarity_ts/plots/plot_factory.py
--rw-r--r--   0 afdez      (501) staff       (20)     2277 2023-07-14 17:18:51.000000 similarity_ts-1.0.2/src/similarity_ts/plots/tsne.py
--rw-r--r--   0 afdez      (501) staff       (20)     2128 2023-07-14 17:09:09.000000 similarity_ts-1.0.2/src/similarity_ts/plots/two_dimensions.py
--rw-r--r--   0 afdez      (501) staff       (20)     1084 2023-07-14 12:53:28.000000 similarity_ts-1.0.2/src/similarity_ts/similarity_analysis_computer.py
--rw-r--r--   0 afdez      (501) staff       (20)     1755 2023-07-17 11:16:50.000000 similarity_ts-1.0.2/src/similarity_ts/similarity_ts.py
--rw-r--r--   0 afdez      (501) staff       (20)      672 2023-07-14 16:52:41.000000 similarity_ts-1.0.2/src/similarity_ts/similarity_ts_config.py
-drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-18 06:26:24.136014 similarity_ts-1.0.2/src/similarity_ts.egg-info/
--rw-r--r--   0 afdez      (501) staff       (20)    17150 2023-07-18 06:26:24.000000 similarity_ts-1.0.2/src/similarity_ts.egg-info/PKG-INFO
--rw-r--r--   0 afdez      (501) staff       (20)     1445 2023-07-18 06:26:24.000000 similarity_ts-1.0.2/src/similarity_ts.egg-info/SOURCES.txt
--rw-r--r--   0 afdez      (501) staff       (20)        1 2023-07-18 06:26:24.000000 similarity_ts-1.0.2/src/similarity_ts.egg-info/dependency_links.txt
--rw-r--r--   0 afdez      (501) staff       (20)       65 2023-07-18 06:26:24.000000 similarity_ts-1.0.2/src/similarity_ts.egg-info/requires.txt
--rw-r--r--   0 afdez      (501) staff       (20)       14 2023-07-18 06:26:24.000000 similarity_ts-1.0.2/src/similarity_ts.egg-info/top_level.txt
+drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-19 11:49:19.646683 similarity_ts-1.0.3/
+-rw-r--r--   0 afdez      (501) staff       (20)     1079 2023-07-16 10:03:12.000000 similarity_ts-1.0.3/LICENSE
+-rw-r--r--   0 afdez      (501) staff       (20)    17416 2023-07-19 11:49:19.646443 similarity_ts-1.0.3/PKG-INFO
+-rw-r--r--   0 afdez      (501) staff       (20)    16688 2023-07-19 11:48:18.000000 similarity_ts-1.0.3/README.md
+-rw-r--r--   0 afdez      (501) staff       (20)      959 2023-07-19 11:43:47.000000 similarity_ts-1.0.3/pyproject.toml
+-rw-r--r--   0 afdez      (501) staff       (20)       38 2023-07-19 11:49:19.646743 similarity_ts-1.0.3/setup.cfg
+drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-19 11:49:19.632861 similarity_ts-1.0.3/src/
+drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-19 11:49:19.635627 similarity_ts-1.0.3/src/similarity_ts/
+-rw-r--r--   0 afdez      (501) staff       (20)        0 2023-07-14 15:40:23.000000 similarity_ts-1.0.3/src/similarity_ts/__init__.py
+drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-19 11:49:19.638168 similarity_ts-1.0.3/src/similarity_ts/helpers/
+-rw-r--r--   0 afdez      (501) staff       (20)        0 2023-07-14 15:40:23.000000 similarity_ts-1.0.3/src/similarity_ts/helpers/__init__.py
+-rw-r--r--   0 afdez      (501) staff       (20)     2161 2023-07-17 10:38:41.000000 similarity_ts-1.0.3/src/similarity_ts/helpers/csv_reader_helper.py
+-rw-r--r--   0 afdez      (501) staff       (20)     1113 2023-07-16 14:24:04.000000 similarity_ts-1.0.3/src/similarity_ts/helpers/dynamic_import_helper.py
+-rw-r--r--   0 afdez      (501) staff       (20)     1928 2023-07-17 11:05:25.000000 similarity_ts-1.0.3/src/similarity_ts/helpers/window_sampler.py
+drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-19 11:49:19.642182 similarity_ts-1.0.3/src/similarity_ts/metrics/
+-rw-r--r--   0 afdez      (501) staff       (20)        0 2023-07-14 15:40:23.000000 similarity_ts-1.0.3/src/similarity_ts/metrics/__init__.py
+-rw-r--r--   0 afdez      (501) staff       (20)      669 2023-07-17 10:39:19.000000 similarity_ts-1.0.3/src/similarity_ts/metrics/cc.py
+-rw-r--r--   0 afdez      (501) staff       (20)      637 2023-07-17 10:39:19.000000 similarity_ts-1.0.3/src/similarity_ts/metrics/cp.py
+-rw-r--r--   0 afdez      (501) staff       (20)     1164 2023-07-17 11:15:50.000000 similarity_ts-1.0.3/src/similarity_ts/metrics/dtw.py
+-rw-r--r--   0 afdez      (501) staff       (20)     1430 2023-07-17 11:15:50.000000 similarity_ts-1.0.3/src/similarity_ts/metrics/hi.py
+-rw-r--r--   0 afdez      (501) staff       (20)     1065 2023-07-17 11:15:50.000000 similarity_ts-1.0.3/src/similarity_ts/metrics/js.py
+-rw-r--r--   0 afdez      (501) staff       (20)     3999 2023-07-17 11:15:50.000000 similarity_ts-1.0.3/src/similarity_ts/metrics/kl.py
+-rw-r--r--   0 afdez      (501) staff       (20)      889 2023-07-17 11:15:50.000000 similarity_ts-1.0.3/src/similarity_ts/metrics/ks.py
+-rw-r--r--   0 afdez      (501) staff       (20)      350 2023-07-17 10:39:19.000000 similarity_ts-1.0.3/src/similarity_ts/metrics/metric.py
+-rw-r--r--   0 afdez      (501) staff       (20)      798 2023-07-17 10:39:19.000000 similarity_ts-1.0.3/src/similarity_ts/metrics/metric_computer.py
+-rw-r--r--   0 afdez      (501) staff       (20)      321 2023-07-14 17:03:35.000000 similarity_ts-1.0.3/src/similarity_ts/metrics/metric_config.py
+-rw-r--r--   0 afdez      (501) staff       (20)     1552 2023-07-17 07:05:11.000000 similarity_ts-1.0.3/src/similarity_ts/metrics/metric_factory.py
+-rw-r--r--   0 afdez      (501) staff       (20)     1011 2023-07-17 11:15:50.000000 similarity_ts-1.0.3/src/similarity_ts/metrics/mmd.py
+drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-19 11:49:19.646040 similarity_ts-1.0.3/src/similarity_ts/plots/
+-rw-r--r--   0 afdez      (501) staff       (20)        0 2023-07-14 15:40:23.000000 similarity_ts-1.0.3/src/similarity_ts/plots/__init__.py
+-rw-r--r--   0 afdez      (501) staff       (20)     4295 2023-07-14 17:42:31.000000 similarity_ts-1.0.3/src/similarity_ts/plots/delta.py
+-rw-r--r--   0 afdez      (501) staff       (20)     1064 2023-07-14 17:09:09.000000 similarity_ts-1.0.3/src/similarity_ts/plots/dimensionalty_reduction.py
+-rw-r--r--   0 afdez      (501) staff       (20)     1129 2023-07-14 17:18:51.000000 similarity_ts-1.0.3/src/similarity_ts/plots/dtw.py
+-rw-r--r--   0 afdez      (501) staff       (20)     1464 2023-07-14 17:18:51.000000 similarity_ts-1.0.3/src/similarity_ts/plots/pca.py
+-rw-r--r--   0 afdez      (501) staff       (20)     1162 2023-07-14 17:18:51.000000 similarity_ts-1.0.3/src/similarity_ts/plots/plot.py
+-rw-r--r--   0 afdez      (501) staff       (20)      976 2023-07-14 17:56:55.000000 similarity_ts-1.0.3/src/similarity_ts/plots/plot_computer.py
+-rw-r--r--   0 afdez      (501) staff       (20)      518 2023-07-14 17:10:27.000000 similarity_ts-1.0.3/src/similarity_ts/plots/plot_config.py
+-rw-r--r--   0 afdez      (501) staff       (20)     1681 2023-07-17 07:05:11.000000 similarity_ts-1.0.3/src/similarity_ts/plots/plot_factory.py
+-rw-r--r--   0 afdez      (501) staff       (20)     2277 2023-07-14 17:18:51.000000 similarity_ts-1.0.3/src/similarity_ts/plots/tsne.py
+-rw-r--r--   0 afdez      (501) staff       (20)     2128 2023-07-14 17:09:09.000000 similarity_ts-1.0.3/src/similarity_ts/plots/two_dimensions.py
+-rw-r--r--   0 afdez      (501) staff       (20)     1084 2023-07-14 12:53:28.000000 similarity_ts-1.0.3/src/similarity_ts/similarity_analysis_computer.py
+-rw-r--r--   0 afdez      (501) staff       (20)     1755 2023-07-17 11:16:50.000000 similarity_ts-1.0.3/src/similarity_ts/similarity_ts.py
+-rw-r--r--   0 afdez      (501) staff       (20)      672 2023-07-14 16:52:41.000000 similarity_ts-1.0.3/src/similarity_ts/similarity_ts_config.py
+drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-19 11:49:19.636972 similarity_ts-1.0.3/src/similarity_ts.egg-info/
+-rw-r--r--   0 afdez      (501) staff       (20)    17416 2023-07-19 11:49:19.000000 similarity_ts-1.0.3/src/similarity_ts.egg-info/PKG-INFO
+-rw-r--r--   0 afdez      (501) staff       (20)     1445 2023-07-19 11:49:19.000000 similarity_ts-1.0.3/src/similarity_ts.egg-info/SOURCES.txt
+-rw-r--r--   0 afdez      (501) staff       (20)        1 2023-07-19 11:49:19.000000 similarity_ts-1.0.3/src/similarity_ts.egg-info/dependency_links.txt
+-rw-r--r--   0 afdez      (501) staff       (20)       65 2023-07-19 11:49:19.000000 similarity_ts-1.0.3/src/similarity_ts.egg-info/requires.txt
+-rw-r--r--   0 afdez      (501) staff       (20)       14 2023-07-19 11:49:19.000000 similarity_ts-1.0.3/src/similarity_ts.egg-info/top_level.txt
```

### Comparing `similarity_ts-1.0.2/LICENSE` & `similarity_ts-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.2/PKG-INFO` & `similarity_ts-1.0.3/src/similarity_ts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 Metadata-Version: 2.1
-Name: similarity_ts
-Version: 1.0.2
+Name: similarity-ts
+Version: 1.0.3
 Summary: SimilarityTS is an open-source project designed to facilitate the evaluation and comparison of multivariate time series data
 Author-email: Alejandro Fernández-Montes <afdez@us.es>, Damián Fernández-Cerero <damiancerero@us.es>, Felipe Escalera González <fescalera@us.es>
 Project-URL: Homepage, https://github.com/alejandrofdez-us/similarity-ts
 Project-URL: Bug Tracker, https://github.com/alejandrofdez-us/similarity-ts/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![version](https://img.shields.io/badge/version-1.0-blue)](https://github.com/alejandrofdez-us/similarity-ts/releases)
+[![version](https://img.shields.io/badge/pypi-1.0.3-blue)](https://pypi.org/project/similarity-ts/)
 [![Python 3.9](https://img.shields.io/badge/python-3.9-darkgreen)](https://www.python.org/downloads/release/python-390/)
-[![last-update](https://img.shields.io/badge/last_update-07/XY/2023-brightgreen)](https://github.com/alejandrofdez-us/similarity-ts/commits/main)
-![license](https://img.shields.io/badge/license-MIT-orange)
+[![last-update](https://img.shields.io/badge/last_update-07/18/2023-brightgreen)](https://github.com/alejandrofdez-us/similarity-ts-cli/commits/main)
+[![license](https://img.shields.io/badge/license-MIT-orange)](LICENSE)
 
 # SimilarityTS: Toolkit for the Evaluation of Similarity for multivariate time series
 
 ## Table of Contents
 
 - [Package Description](#package-description)
 - [Installation](#installation)
 - [Usage](#usage)
 - [Configuring the toolkit](#configuring-the-toolkit)
 - [Extending the toolkit](#extending-the-toolkit)
 - [License](#license)
+- [Acknowledgements](#acknowledgements)
 
 ## Package Description
 
 SimilarityTS is an open-source package designed to facilitate the evaluation and comparison of
 multivariate time series data. It provides a comprehensive toolkit for analyzing, visualizing, and reporting multiple
 metrics and figures derived from time series datasets. The toolkit simplifies the process of evaluating the similarity of
 time series by offering data preprocessing, metrics computation, visualization, statistical analysis, and report generation
 functionalities. With its customizable features, SimilarityTS empowers researchers and data
 scientists to gain insights, identify patterns, and make informed decisions based on their time series data.
 
-A command line interface tool is also available at: https://github.com/alejandrofdez-us/similarity-ts-cli
+A command line interface tool is also available at: https://github.com/alejandrofdez-us/similarity-ts-cli.
 
 ### Available metrics
 
 This toolkit can compute the following metrics:
 
 - `kl`: Kullback-Leibler divergence
 - `js`: Jensen-Shannon divergence
@@ -103,41 +104,41 @@
 ```
 
 ## Usage
 
 Users must create a new `SimilarityTs` object by calling its constructor and passing the following parameters.
 
 - `ts1` This time series may represent the baseline or ground truth time
-  series as a `numpy` object with shape `[length, num_features]`.
-- `ts2s` A single or a set of time series as a `numpy` object with shape `[num_time_series, length, num_features]`.
+  series as a `numpy` array with shape `[length, num_features]`.
+- `ts2s` A single or a set of time series as a `numpy` array with shape `[num_time_series, length, num_features]`.
 
 
 Constraints:
 
 - `ts1` time-series and `ts2s` time-series file(s) must:
     - have the same dimensionality (number of columns)
-    - do not include a timestamp column
+    - not include a timestamp column
     - include only numeric values
 - all `ts2s` time-series must have the same length (number of rows).
 
 If `ts1` time-series is longer (more rows) than `ts2s` time-series, the `ts1` time series will be
 divided in windows of the same length as the `ts2s` time-series.
 
 For each `ts2s` time-series, the most similar window (*) from `ts1` time series is selected.
 
 Finally, metrics and figures that assess the similarity between each pair of `ts2s` time-series and its
 associated most similar `ts1` window are computed.
 
 (*) The metric used for the selection of the most
-similar `ts1` time-series window per each `ts2s` time-series file is selectable.`dtw` is the default selected metric, however, any of
+similar `ts1` time-series window per each `ts2s` time-series file is selectable. `dtw` is the default selected metric, however, any of
 the
-[metrics](#available-metrics) are also available for this purpose. See the [toolkit configuration section](#configuring-the-toolkit)
+[metrics](#available-metrics) are also available for this purpose. See the [toolkit configuration section](#configuring-the-toolkit).
 
 ### Minimal usage examples:
-Usage examples can be found at: https://github.com/alejandrofdez-us/similarity-ts/tree/main/usage_examples
+Usage examples can be found at: https://github.com/alejandrofdez-us/similarity-ts/tree/main/usage_examples.
 
 1. Compute metrics between random time series (`ts1`: one time series of lenght 200 and 2 dimensions and `ts2`: five time series of length 100 and 2 dimensions):
     ```Python
     import numpy as np
     from similarity_ts.similarity_ts import SimilarityTs
     
     ts1 = np.random.rand(200, 2)
@@ -214,15 +215,15 @@
 - `timestamp_frequency_seconds`: the frequency in seconds in which samples were taken. This is needed to generate the delta figures with correct time magnitudes. By default is
   `1` second.
 - `stride`: when `ts1` time-series is longer than `ts2s` time-series the windows are computed by using a
   stride of `1` by default. Sometimes using a larger value for the stride parameter improves the performance by skipping
   the computation of similarity between so many windows.
 - `window_selection_metric`: the metric used for the selection of the most similar `ts1` time-series window per each `ts2s` time-series file is selectable.`dtw` is the default selected metric, however, any of the [metrics](#available-metrics) are also available for this purpose. See the [toolkit configuration section](#configuring-the-toolkit).
 - `ts2_names`: name of each time series of the `ts2s` set of time series.
-- `header_names`: name of the features
+- `header_names`: name of the features.
 
 
 ## Extending the toolkit
 
 Additionally, users may implement their own metric or figure classes and include them by using the `MetricFactory` or `PlotFactory` register methods. To ensure compatibility with our toolkit, they have to inherit from the base classes `Metric` and `Plot`.
 
 The following code snippet is an example of how to introduce the Euclidean distance metric:
@@ -345,7 +346,10 @@
 if __name__ == '__main__':
     main()
 ```
 
 ## License
 
 SimilarityTS toolkit is free and open-source software licensed under the [MIT license](LICENSE).
+
+## Acknowledgements
+Project PID2021-122208OB-I00, PROYEXCEL\_00286 and  TED2021-132695B-I00 project, funded by MCIN / AEI / 10.13039 / 501100011033, by Andalusian Regional Government, and by the European Union - NextGenerationEU.
```

### Comparing `similarity_ts-1.0.2/README.md` & `similarity_ts-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,1027 +1,1043 @@
 00000000: 5b21 5b76 6572 7369 6f6e 5d28 6874 7470  [![version](http
 00000010: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
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
-000001c0: 2320 5369 6d69 6c61 7269 7479 5453 3a20  # SimilarityTS: 
-000001d0: 546f 6f6c 6b69 7420 666f 7220 7468 6520  Toolkit for the 
-000001e0: 4576 616c 7561 7469 6f6e 206f 6620 5369  Evaluation of Si
-000001f0: 6d69 6c61 7269 7479 2066 6f72 206d 756c  milarity for mul
-00000200: 7469 7661 7269 6174 6520 7469 6d65 2073  tivariate time s
-00000210: 6572 6965 730a 0a23 2320 5461 626c 6520  eries..## Table 
-00000220: 6f66 2043 6f6e 7465 6e74 730a 0a2d 205b  of Contents..- [
-00000230: 5061 636b 6167 6520 4465 7363 7269 7074  Package Descript
-00000240: 696f 6e5d 2823 7061 636b 6167 652d 6465  ion](#package-de
-00000250: 7363 7269 7074 696f 6e29 0a2d 205b 496e  scription).- [In
-00000260: 7374 616c 6c61 7469 6f6e 5d28 2369 6e73  stallation](#ins
-00000270: 7461 6c6c 6174 696f 6e29 0a2d 205b 5573  tallation).- [Us
-00000280: 6167 655d 2823 7573 6167 6529 0a2d 205b  age](#usage).- [
-00000290: 436f 6e66 6967 7572 696e 6720 7468 6520  Configuring the 
-000002a0: 746f 6f6c 6b69 745d 2823 636f 6e66 6967  toolkit](#config
-000002b0: 7572 696e 672d 7468 652d 746f 6f6c 6b69  uring-the-toolki
-000002c0: 7429 0a2d 205b 4578 7465 6e64 696e 6720  t).- [Extending 
-000002d0: 7468 6520 746f 6f6c 6b69 745d 2823 6578  the toolkit](#ex
-000002e0: 7465 6e64 696e 672d 7468 652d 746f 6f6c  tending-the-tool
-000002f0: 6b69 7429 0a2d 205b 4c69 6365 6e73 655d  kit).- [License]
-00000300: 2823 6c69 6365 6e73 6529 0a0a 2323 2050  (#license)..## P
-00000310: 6163 6b61 6765 2044 6573 6372 6970 7469  ackage Descripti
-00000320: 6f6e 0a0a 5369 6d69 6c61 7269 7479 5453  on..SimilarityTS
-00000330: 2069 7320 616e 206f 7065 6e2d 736f 7572   is an open-sour
-00000340: 6365 2070 6163 6b61 6765 2064 6573 6967  ce package desig
-00000350: 6e65 6420 746f 2066 6163 696c 6974 6174  ned to facilitat
-00000360: 6520 7468 6520 6576 616c 7561 7469 6f6e  e the evaluation
-00000370: 2061 6e64 2063 6f6d 7061 7269 736f 6e20   and comparison 
-00000380: 6f66 0a6d 756c 7469 7661 7269 6174 6520  of.multivariate 
-00000390: 7469 6d65 2073 6572 6965 7320 6461 7461  time series data
-000003a0: 2e20 4974 2070 726f 7669 6465 7320 6120  . It provides a 
-000003b0: 636f 6d70 7265 6865 6e73 6976 6520 746f  comprehensive to
-000003c0: 6f6c 6b69 7420 666f 7220 616e 616c 797a  olkit for analyz
-000003d0: 696e 672c 2076 6973 7561 6c69 7a69 6e67  ing, visualizing
-000003e0: 2c20 616e 6420 7265 706f 7274 696e 6720  , and reporting 
-000003f0: 6d75 6c74 6970 6c65 0a6d 6574 7269 6373  multiple.metrics
-00000400: 2061 6e64 2066 6967 7572 6573 2064 6572   and figures der
-00000410: 6976 6564 2066 726f 6d20 7469 6d65 2073  ived from time s
-00000420: 6572 6965 7320 6461 7461 7365 7473 2e20  eries datasets. 
-00000430: 5468 6520 746f 6f6c 6b69 7420 7369 6d70  The toolkit simp
-00000440: 6c69 6669 6573 2074 6865 2070 726f 6365  lifies the proce
-00000450: 7373 206f 6620 6576 616c 7561 7469 6e67  ss of evaluating
-00000460: 2074 6865 2073 696d 696c 6172 6974 7920   the similarity 
-00000470: 6f66 0a74 696d 6520 7365 7269 6573 2062  of.time series b
-00000480: 7920 6f66 6665 7269 6e67 2064 6174 6120  y offering data 
-00000490: 7072 6570 726f 6365 7373 696e 672c 206d  preprocessing, m
-000004a0: 6574 7269 6373 2063 6f6d 7075 7461 7469  etrics computati
-000004b0: 6f6e 2c20 7669 7375 616c 697a 6174 696f  on, visualizatio
-000004c0: 6e2c 2073 7461 7469 7374 6963 616c 2061  n, statistical a
-000004d0: 6e61 6c79 7369 732c 2061 6e64 2072 6570  nalysis, and rep
-000004e0: 6f72 7420 6765 6e65 7261 7469 6f6e 0a66  ort generation.f
-000004f0: 756e 6374 696f 6e61 6c69 7469 6573 2e20  unctionalities. 
-00000500: 5769 7468 2069 7473 2063 7573 746f 6d69  With its customi
-00000510: 7a61 626c 6520 6665 6174 7572 6573 2c20  zable features, 
-00000520: 5369 6d69 6c61 7269 7479 5453 2065 6d70  SimilarityTS emp
-00000530: 6f77 6572 7320 7265 7365 6172 6368 6572  owers researcher
-00000540: 7320 616e 6420 6461 7461 0a73 6369 656e  s and data.scien
-00000550: 7469 7374 7320 746f 2067 6169 6e20 696e  tists to gain in
-00000560: 7369 6768 7473 2c20 6964 656e 7469 6679  sights, identify
-00000570: 2070 6174 7465 726e 732c 2061 6e64 206d   patterns, and m
-00000580: 616b 6520 696e 666f 726d 6564 2064 6563  ake informed dec
-00000590: 6973 696f 6e73 2062 6173 6564 206f 6e20  isions based on 
-000005a0: 7468 6569 7220 7469 6d65 2073 6572 6965  their time serie
-000005b0: 7320 6461 7461 2e0a 0a41 2063 6f6d 6d61  s data...A comma
-000005c0: 6e64 206c 696e 6520 696e 7465 7266 6163  nd line interfac
-000005d0: 6520 746f 6f6c 2069 7320 616c 736f 2061  e tool is also a
-000005e0: 7661 696c 6162 6c65 2061 743a 2068 7474  vailable at: htt
-000005f0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000600: 616c 656a 616e 6472 6f66 6465 7a2d 7573  alejandrofdez-us
-00000610: 2f73 696d 696c 6172 6974 792d 7473 2d63  /similarity-ts-c
-00000620: 6c69 0a0a 2323 2320 4176 6169 6c61 626c  li..### Availabl
-00000630: 6520 6d65 7472 6963 730a 0a54 6869 7320  e metrics..This 
-00000640: 746f 6f6c 6b69 7420 6361 6e20 636f 6d70  toolkit can comp
-00000650: 7574 6520 7468 6520 666f 6c6c 6f77 696e  ute the followin
-00000660: 6720 6d65 7472 6963 733a 0a0a 2d20 606b  g metrics:..- `k
-00000670: 6c60 3a20 4b75 6c6c 6261 636b 2d4c 6569  l`: Kullback-Lei
-00000680: 626c 6572 2064 6976 6572 6765 6e63 650a  bler divergence.
-00000690: 2d20 606a 7360 3a20 4a65 6e73 656e 2d53  - `js`: Jensen-S
-000006a0: 6861 6e6e 6f6e 2064 6976 6572 6765 6e63  hannon divergenc
-000006b0: 650a 2d20 606b 7360 3a20 4b6f 6c6d 6f67  e.- `ks`: Kolmog
-000006c0: 6f72 6f76 2d53 6d69 726e 6f76 2074 6573  orov-Smirnov tes
-000006d0: 740a 2d20 606d 6d64 603a 204d 6178 696d  t.- `mmd`: Maxim
-000006e0: 756d 204d 6561 6e20 4469 7363 7265 7061  um Mean Discrepa
-000006f0: 6e63 790a 2d20 6064 7477 6020 4479 6e61  ncy.- `dtw` Dyna
-00000700: 6d69 6320 5469 6d65 2057 6172 7069 6e67  mic Time Warping
-00000710: 0a2d 2060 6363 603a 2044 6966 6665 7265  .- `cc`: Differe
-00000720: 6e63 6520 6f66 2063 6f2d 7661 7269 616e  nce of co-varian
-00000730: 6365 730a 2d20 6063 7060 3a20 4469 6666  ces.- `cp`: Diff
-00000740: 6572 656e 6365 206f 6620 636f 7272 656c  erence of correl
-00000750: 6174 696f 6e73 0a2d 2060 6869 603a 2044  ations.- `hi`: D
-00000760: 6966 6665 7265 6e63 6520 6f66 2068 6973  ifference of his
-00000770: 746f 6772 616d 730a 0a23 2323 2041 7661  tograms..### Ava
-00000780: 696c 6162 6c65 2066 6967 7572 6573 0a0a  ilable figures..
-00000790: 5468 6973 2074 6f6f 6c6b 6974 2063 616e  This toolkit can
-000007a0: 2067 656e 6572 6174 6520 7468 6520 666f   generate the fo
-000007b0: 6c6c 6f77 696e 6720 6669 6775 7265 733a  llowing figures:
-000007c0: 0a0a 2d20 6032 6460 3a20 7468 6520 6f72  ..- `2d`: the or
-000007d0: 6469 6e61 7279 2067 7261 7068 6963 616c  dinary graphical
-000007e0: 2072 6570 7265 7365 6e74 6174 696f 6e20   representation 
-000007f0: 6f66 2074 6865 2074 696d 6520 7365 7269  of the time seri
-00000800: 6573 2069 6e20 6120 3244 2066 6967 7572  es in a 2D figur
-00000810: 6520 7769 7468 2074 6865 2074 696d 6520  e with the time 
-00000820: 7265 7072 6573 656e 7465 6420 6f6e 2074  represented on t
-00000830: 6865 2078 2061 7869 730a 2020 616e 6420  he x axis.  and 
-00000840: 7468 6520 6461 7461 2076 616c 7565 7320  the data values 
-00000850: 6f6e 2074 6865 2079 2d61 7869 7320 666f  on the y-axis fo
-00000860: 720a 2020 2020 2d20 7468 6520 636f 6d70  r.    - the comp
-00000870: 6c65 7465 206d 756c 7469 7661 7269 6174  lete multivariat
-00000880: 6520 7469 6d65 2073 6572 6965 733b 2061  e time series; a
-00000890: 6e64 0a20 2020 202d 2061 2070 6c6f 7420  nd.    - a plot 
-000008a0: 7065 7220 636f 6c75 6d6e 2e0a 0a20 2045  per column...  E
-000008b0: 6163 6820 6765 6e65 7261 7465 6420 6669  ach generated fi
-000008c0: 6775 7265 2070 6c6f 7473 2062 6f74 6820  gure plots both 
-000008d0: 7468 6520 6074 7331 6020 616e 6420 7468  the `ts1` and th
-000008e0: 6520 6074 7332 6020 6461 7461 2074 6f20  e `ts2` data to 
-000008f0: 6561 7369 6c79 206f 6274 6169 6e20 6b65  easily obtain ke
-00000900: 7920 696e 7369 6768 7473 2069 6e74 6f0a  y insights into.
-00000910: 2020 7468 6520 7369 6d69 6c61 7269 7469    the similariti
-00000920: 6573 206f 7220 6469 6666 6572 656e 6365  es or difference
-00000930: 7320 6265 7477 6565 6e20 7468 656d 2e0a  s between them..
-00000940: 2020 2020 3c64 6976 3e0a 2020 2020 3c69      <div>.    <i
-00000950: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-00000960: 6769 7468 7562 2e63 6f6d 2f61 6c65 6a61  github.com/aleja
-00000970: 6e64 726f 6664 657a 2d75 732f 7369 6d69  ndrofdez-us/simi
-00000980: 6c61 7269 7479 2d74 732f 626c 6f62 2f65  larity-ts/blob/e
-00000990: 3562 3134 3762 3134 3539 3730 6633 6139  5b147b145970f3a9
-000009a0: 3333 3531 6131 3030 3430 3232 6662 3330  3351a1004022fb30
-000009b0: 6432 3066 3566 302f 646f 6373 2f66 6967  d20f5f0/docs/fig
-000009c0: 7572 6573 2f32 645f 7361 6d70 6c65 5f33  ures/2d_sample_3
-000009d0: 5f63 6f6d 706c 6574 655f 5453 5f31 5f76  _complete_TS_1_v
-000009e0: 735f 5453 5f32 2e70 6e67 3f72 6177 3d74  s_TS_2.png?raw=t
-000009f0: 7275 6522 2061 6c74 3d22 3244 2046 6967  rue" alt="2D Fig
-00000a00: 7572 6520 636f 6d70 6c65 7465 223e 0a20  ure complete">. 
-00000a10: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
-00000a20: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000a30: 616c 656a 616e 6472 6f66 6465 7a2d 7573  alejandrofdez-us
-00000a40: 2f73 696d 696c 6172 6974 792d 7473 2f62  /similarity-ts/b
-00000a50: 6c6f 622f 6535 6231 3437 6231 3435 3937  lob/e5b147b14597
-00000a60: 3066 3361 3933 3335 3161 3130 3034 3032  0f3a93351a100402
-00000a70: 3266 6233 3064 3230 6635 6630 2f64 6f63  2fb30d20f5f0/doc
-00000a80: 732f 6669 6775 7265 732f 3264 5f73 616d  s/figures/2d_sam
-00000a90: 706c 655f 335f 6370 755f 7574 696c 5f70  ple_3_cpu_util_p
-00000aa0: 6572 6365 6e74 5f54 535f 315f 7673 5f54  ercent_TS_1_vs_T
-00000ab0: 535f 322e 706e 673f 7261 773d 7472 7565  S_2.png?raw=true
-00000ac0: 2220 616c 743d 2232 4420 4669 6775 7265  " alt="2D Figure
-00000ad0: 2066 6f72 2075 7365 6420 4350 5520 7065   for used CPU pe
-00000ae0: 7263 656e 7461 6765 223e 0a20 2020 203c  rcentage">.    <
-00000af0: 2f64 6976 3e0a 2d20 6064 656c 7461 603a  /div>.- `delta`:
-00000b00: 2074 6865 2064 6966 6665 7265 6e63 6573   the differences
-00000b10: 2062 6574 7765 656e 2074 6865 2076 616c   between the val
-00000b20: 7565 7320 6f66 2065 6163 6820 636f 6c75  ues of each colu
-00000b30: 6d6e 2067 726f 7570 6564 2062 7920 7065  mn grouped by pe
-00000b40: 7269 6f64 7320 6f66 2074 696d 652e 2046  riods of time. F
-00000b50: 6f72 2069 6e73 7461 6e63 652c 2074 6865  or instance, the
-00000b60: 2064 6966 6665 7265 6e63 6573 0a20 2062   differences.  b
-00000b70: 6574 7765 656e 2074 6865 2070 6572 6365  etween the perce
-00000b80: 6e74 6167 6520 6f66 2063 7075 2075 7365  ntage of cpu use
-00000b90: 6420 6576 6572 7920 3130 2c20 3235 206f  d every 10, 25 o
-00000ba0: 7220 3530 206d 696e 7574 6573 2e20 5468  r 50 minutes. Th
-00000bb0: 6573 6520 6465 6c74 6120 6361 6e20 6265  ese delta can be
-00000bc0: 2075 7365 6420 6173 2061 206d 6561 6e73   used as a means
-00000bd0: 206f 6620 636f 6d70 6172 6973 6f6e 2062   of comparison b
-00000be0: 6574 7765 656e 0a20 2074 696d 6520 7365  etween.  time se
-00000bf0: 7269 6573 2073 686f 7274 2d2f 6d69 642d  ries short-/mid-
-00000c00: 2f6c 6f6e 672d 7465 726d 2070 6174 7465  /long-term patte
-00000c10: 726e 732e 0a20 2020 203c 6469 763e 0a20  rns..    <div>. 
-00000c20: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
-00000c30: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000c40: 616c 656a 616e 6472 6f66 6465 7a2d 7573  alejandrofdez-us
-00000c50: 2f73 696d 696c 6172 6974 792d 7473 2f62  /similarity-ts/b
-00000c60: 6c6f 622f 6535 6231 3437 6231 3435 3937  lob/e5b147b14597
-00000c70: 3066 3361 3933 3335 3161 3130 3034 3032  0f3a93351a100402
-00000c80: 3266 6233 3064 3230 6635 6630 2f64 6f63  2fb30d20f5f0/doc
-00000c90: 732f 6669 6775 7265 732f 6465 6c74 615f  s/figures/delta_
-00000ca0: 7361 6d70 6c65 5f33 5f63 7075 5f75 7469  sample_3_cpu_uti
-00000cb0: 6c5f 7065 7263 656e 745f 5453 5f31 5f76  l_percent_TS_1_v
-00000cc0: 735f 5453 5f32 5f28 6772 6f75 7065 645f  s_TS_2_(grouped_
-00000cd0: 6279 5f31 305f 6d69 6e75 7465 7329 2e70  by_10_minutes).p
-00000ce0: 6e67 3f72 6177 3d74 7275 6522 2061 6c74  ng?raw=true" alt
-00000cf0: 3d22 4465 6c74 6120 4669 6775 7265 2066  ="Delta Figure f
-00000d00: 6f72 2075 7365 6420 4350 5520 7065 7263  or used CPU perc
-00000d10: 656e 7461 6765 2067 726f 7570 6564 2062  entage grouped b
-00000d20: 7920 3130 206d 696e 7574 6573 223e 0a20  y 10 minutes">. 
-00000d30: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
-00000d40: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000d50: 616c 656a 616e 6472 6f66 6465 7a2d 7573  alejandrofdez-us
-00000d60: 2f73 696d 696c 6172 6974 792d 7473 2f62  /similarity-ts/b
-00000d70: 6c6f 622f 6535 6231 3437 6231 3435 3937  lob/e5b147b14597
-00000d80: 3066 3361 3933 3335 3161 3130 3034 3032  0f3a93351a100402
-00000d90: 3266 6233 3064 3230 6635 6630 2f64 6f63  2fb30d20f5f0/doc
-00000da0: 732f 6669 6775 7265 732f 6465 6c74 615f  s/figures/delta_
-00000db0: 7361 6d70 6c65 5f33 5f63 7075 5f75 7469  sample_3_cpu_uti
-00000dc0: 6c5f 7065 7263 656e 745f 5453 5f31 5f76  l_percent_TS_1_v
-00000dd0: 735f 5453 5f32 5f28 6772 6f75 7065 645f  s_TS_2_(grouped_
-00000de0: 6279 5f32 355f 6d69 6e75 7465 7329 2e70  by_25_minutes).p
-00000df0: 6e67 3f72 6177 3d74 7275 6522 2061 6c74  ng?raw=true" alt
-00000e00: 3d22 4465 6c74 6120 4669 6775 7265 2066  ="Delta Figure f
-00000e10: 6f72 2075 7365 6420 4350 5520 7065 7263  or used CPU perc
-00000e20: 656e 7461 6765 2067 726f 7570 6564 2062  entage grouped b
-00000e30: 7920 3235 206d 696e 7574 6573 223e 0a20  y 25 minutes">. 
-00000e40: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
-00000e50: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000e60: 616c 656a 616e 6472 6f66 6465 7a2d 7573  alejandrofdez-us
-00000e70: 2f73 696d 696c 6172 6974 792d 7473 2f62  /similarity-ts/b
-00000e80: 6c6f 622f 6535 6231 3437 6231 3435 3937  lob/e5b147b14597
-00000e90: 3066 3361 3933 3335 3161 3130 3034 3032  0f3a93351a100402
-00000ea0: 3266 6233 3064 3230 6635 6630 2f64 6f63  2fb30d20f5f0/doc
-00000eb0: 732f 6669 6775 7265 732f 6465 6c74 615f  s/figures/delta_
-00000ec0: 7361 6d70 6c65 5f33 5f63 7075 5f75 7469  sample_3_cpu_uti
-00000ed0: 6c5f 7065 7263 656e 745f 5453 5f31 5f76  l_percent_TS_1_v
-00000ee0: 735f 5453 5f32 5f28 6772 6f75 7065 645f  s_TS_2_(grouped_
-00000ef0: 6279 5f35 305f 6d69 6e75 7465 7329 2e70  by_50_minutes).p
-00000f00: 6e67 3f72 6177 3d74 7275 6522 2061 6c74  ng?raw=true" alt
-00000f10: 3d22 4465 6c74 6120 4669 6775 7265 2066  ="Delta Figure f
-00000f20: 6f72 2075 7365 6420 4350 5520 7065 7263  or used CPU perc
-00000f30: 656e 7461 6765 2067 726f 7570 6564 2062  entage grouped b
-00000f40: 7920 3530 206d 696e 7574 6573 223e 0a20  y 50 minutes">. 
-00000f50: 2020 203c 2f64 6976 3e0a 0a2d 2060 7063     </div>..- `pc
-00000f60: 6160 3a20 7468 6520 6c69 6e65 6172 2064  a`: the linear d
-00000f70: 696d 656e 7369 6f6e 616c 6974 7920 7265  imensionality re
-00000f80: 6475 6374 696f 6e20 7465 6368 6e69 7175  duction techniqu
-00000f90: 6520 7468 6174 2061 696d 7320 746f 2066  e that aims to f
-00000fa0: 696e 6420 7468 6520 7072 696e 6369 7061  ind the principa
-00000fb0: 6c20 636f 6d70 6f6e 656e 7473 206f 6620  l components of 
-00000fc0: 6120 6461 7461 2073 6574 2062 790a 2020  a data set by.  
-00000fd0: 636f 6d70 7574 696e 6720 7468 6520 6c69  computing the li
-00000fe0: 6e65 6172 2063 6f6d 6269 6e61 7469 6f6e  near combination
-00000ff0: 7320 6f66 2074 6865 206f 7269 6769 6e61  s of the origina
-00001000: 6c20 6368 6172 6163 7465 7269 7374 6963  l characteristic
-00001010: 7320 7468 6174 2065 7870 6c61 696e 2074  s that explain t
-00001020: 6865 206d 6f73 7420 7661 7269 616e 6365  he most variance
-00001030: 2069 6e20 7468 6520 6461 7461 2e0a 2020   in the data..  
-00001040: 2020 3c64 6976 2061 6c69 676e 3d22 6365    <div align="ce
-00001050: 6e74 6572 223e 0a20 2020 203c 696d 6720  nter">.    <img 
-00001060: 7372 633d 2268 7474 7073 3a2f 2f67 6974  src="https://git
-00001070: 6875 622e 636f 6d2f 616c 656a 616e 6472  hub.com/alejandr
-00001080: 6f66 6465 7a2d 7573 2f73 696d 696c 6172  ofdez-us/similar
-00001090: 6974 792d 7473 2f62 6c6f 622f 6535 6231  ity-ts/blob/e5b1
-000010a0: 3437 6231 3435 3937 3066 3361 3933 3335  47b145970f3a9335
-000010b0: 3161 3130 3034 3032 3266 6233 3064 3230  1a1004022fb30d20
-000010c0: 6635 6630 2f64 6f63 732f 6669 6775 7265  f5f0/docs/figure
-000010d0: 732f 5043 412e 706e 673f 7261 773d 7472  s/PCA.png?raw=tr
-000010e0: 7565 2220 616c 743d 2250 4341 2046 6967  ue" alt="PCA Fig
-000010f0: 7572 6522 2077 6964 7468 3d22 3435 3022  ure" width="450"
-00001100: 3e0a 2020 2020 3c2f 6469 763e 0a2d 2060  >.    </div>.- `
-00001110: 7473 6e65 603a 2061 2074 6f6f 6c20 666f  tsne`: a tool fo
-00001120: 7220 7669 7375 616c 6973 696e 6720 6869  r visualising hi
-00001130: 6768 2d64 696d 656e 7369 6f6e 616c 2064  gh-dimensional d
-00001140: 6174 6120 7365 7473 2069 6e20 6120 3244  ata sets in a 2D
-00001150: 206f 7220 3344 2067 7261 7068 6963 616c   or 3D graphical
-00001160: 2072 6570 7265 7365 6e74 6174 696f 6e20   representation 
-00001170: 616c 6c6f 7769 6e67 2074 6865 2063 7265  allowing the cre
-00001180: 6174 696f 6e0a 2020 6f66 2061 2073 696e  ation.  of a sin
-00001190: 676c 6520 6d61 7020 7468 6174 2072 6576  gle map that rev
-000011a0: 6561 6c73 2074 6865 2073 7472 7563 7475  eals the structu
-000011b0: 7265 206f 6620 7468 6520 6461 7461 2061  re of the data a
-000011c0: 7420 6d61 6e79 2064 6966 6665 7265 6e74  t many different
-000011d0: 2073 6361 6c65 732e 0a20 2020 203c 6469   scales..    <di
-000011e0: 7620 616c 6967 6e3d 2263 656e 7465 7222  v align="center"
-000011f0: 3e0a 2020 2020 3c69 6d67 2073 7263 3d22  >.    <img src="
-00001200: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001210: 6f6d 2f61 6c65 6a61 6e64 726f 6664 657a  om/alejandrofdez
-00001220: 2d75 732f 7369 6d69 6c61 7269 7479 2d74  -us/similarity-t
-00001230: 732f 626c 6f62 2f65 3562 3134 3762 3134  s/blob/e5b147b14
-00001240: 3539 3730 6633 6139 3333 3531 6131 3030  5970f3a93351a100
-00001250: 3430 3232 6662 3330 6432 3066 3566 302f  4022fb30d20f5f0/
-00001260: 646f 6373 2f66 6967 7572 6573 2f74 2d53  docs/figures/t-S
-00001270: 4e45 2d69 7465 725f 3330 302d 7065 7270  NE-iter_300-perp
-00001280: 6c65 7869 7479 5f35 2e70 6e67 3f72 6177  lexity_5.png?raw
-00001290: 3d74 7275 6522 2061 6c74 3d22 5453 4e45  =true" alt="TSNE
-000012a0: 2046 6967 7572 6520 3330 3020 6974 6572   Figure 300 iter
-000012b0: 6174 696f 6e73 2035 2070 6572 706c 6578  ations 5 perplex
-000012c0: 6974 7922 2077 6964 7468 3d22 3435 3022  ity" width="450"
-000012d0: 3e0a 2020 2020 3c69 6d67 2073 7263 3d22  >.    <img src="
-000012e0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000012f0: 6f6d 2f61 6c65 6a61 6e64 726f 6664 657a  om/alejandrofdez
-00001300: 2d75 732f 7369 6d69 6c61 7269 7479 2d74  -us/similarity-t
-00001310: 732f 626c 6f62 2f65 3562 3134 3762 3134  s/blob/e5b147b14
-00001320: 3539 3730 6633 6139 3333 3531 6131 3030  5970f3a93351a100
-00001330: 3430 3232 6662 3330 6432 3066 3566 302f  4022fb30d20f5f0/
-00001340: 646f 6373 2f66 6967 7572 6573 2f74 2d53  docs/figures/t-S
-00001350: 4e45 2d69 7465 725f 3130 3030 2d70 6572  NE-iter_1000-per
-00001360: 706c 6578 6974 795f 352e 706e 673f 7261  plexity_5.png?ra
-00001370: 773d 7472 7565 2220 616c 743d 2254 534e  w=true" alt="TSN
-00001380: 4520 4669 6775 7265 2031 3030 3020 6974  E Figure 1000 it
-00001390: 6572 6174 696f 6e73 2035 2070 6572 706c  erations 5 perpl
-000013a0: 6578 6974 7922 2077 6964 7468 3d22 3435  exity" width="45
-000013b0: 3022 3e0a 2020 2020 3c2f 6469 763e 0a2d  0">.    </div>.-
-000013c0: 2060 6474 7760 2070 6174 683a 2049 6e20   `dtw` path: In 
-000013d0: 6164 6469 7469 6f6e 2074 6f20 7468 6520  addition to the 
-000013e0: 6e75 6d65 7269 6361 6c20 7369 6d69 6c61  numerical simila
-000013f0: 7269 7479 206d 6561 7375 7265 2c20 7468  rity measure, th
-00001400: 6520 6772 6170 6869 6361 6c20 7265 7072  e graphical repr
-00001410: 6573 656e 7461 7469 6f6e 206f 6620 7468  esentation of th
-00001420: 6520 4454 5720 7061 7468 206f 6620 6561  e DTW path of ea
-00001430: 6368 0a20 2063 6f6c 756d 6e20 6361 6e20  ch.  column can 
-00001440: 6265 2075 7365 6675 6c20 746f 2062 6574  be useful to bet
-00001450: 7465 7220 616e 616c 7973 6520 7468 6520  ter analyse the 
-00001460: 7369 6d69 6c61 7269 7469 6573 206f 7220  similarities or 
-00001470: 6469 6666 6572 656e 6365 7320 6265 7477  differences betw
-00001480: 6565 6e20 7468 6520 7469 6d65 2073 6572  een the time ser
-00001490: 6965 7320 636f 6c75 6d6e 732e 204e 6f74  ies columns. Not
-000014a0: 6963 6520 7468 6174 0a20 2074 6865 7265  ice that.  there
-000014b0: 2069 7320 6e6f 206d 756c 7469 7661 7269   is no multivari
-000014c0: 6174 6520 7265 7072 6573 656e 7461 7469  ate representati
-000014d0: 6f6e 206f 6620 4454 5720 7061 7468 732c  on of DTW paths,
-000014e0: 206f 6e6c 7920 7369 6e67 6c65 2063 6f6c   only single col
-000014f0: 756d 6e20 7265 7072 6573 656e 7461 7469  umn representati
-00001500: 6f6e 732e 0a20 2020 203c 6469 763e 0a20  ons..    <div>. 
-00001510: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
-00001520: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001530: 616c 656a 616e 6472 6f66 6465 7a2d 7573  alejandrofdez-us
-00001540: 2f73 696d 696c 6172 6974 792d 7473 2f62  /similarity-ts/b
-00001550: 6c6f 622f 6535 6231 3437 6231 3435 3937  lob/e5b147b14597
-00001560: 3066 3361 3933 3335 3161 3130 3034 3032  0f3a93351a100402
-00001570: 3266 6233 3064 3230 6635 6630 2f64 6f63  2fb30d20f5f0/doc
-00001580: 732f 6669 6775 7265 732f 4454 575f 7361  s/figures/DTW_sa
-00001590: 6d70 6c65 5f33 5f63 7075 5f75 7469 6c5f  mple_3_cpu_util_
-000015a0: 7065 7263 656e 742e 706e 673f 7261 773d  percent.png?raw=
-000015b0: 7472 7565 2220 616c 743d 2244 5457 2046  true" alt="DTW F
-000015c0: 6967 7572 6520 666f 7220 6370 7522 3e0a  igure for cpu">.
-000015d0: 2020 2020 3c2f 6469 763e 0a0a 2323 2049      </div>..## I
-000015e0: 6e73 7461 6c6c 6174 696f 6e0a 0a49 6e73  nstallation..Ins
-000015f0: 7461 6c6c 2074 6865 2070 6163 6b61 6765  tall the package
-00001600: 2075 7369 6e67 2070 6970 2069 6e20 796f   using pip in yo
-00001610: 7572 206c 6f63 616c 2065 6e76 6972 6f6e  ur local environ
-00001620: 6d65 6e74 3a0a 0a60 6060 4261 7368 0a70  ment:..```Bash.p
-00001630: 6970 2069 6e73 7461 6c6c 2073 696d 696c  ip install simil
-00001640: 6172 6974 792d 7473 0a60 6060 0a0a 2323  arity-ts.```..##
-00001650: 2055 7361 6765 0a0a 5573 6572 7320 6d75   Usage..Users mu
-00001660: 7374 2063 7265 6174 6520 6120 6e65 7720  st create a new 
-00001670: 6053 696d 696c 6172 6974 7954 7360 206f  `SimilarityTs` o
-00001680: 626a 6563 7420 6279 2063 616c 6c69 6e67  bject by calling
-00001690: 2069 7473 2063 6f6e 7374 7275 6374 6f72   its constructor
-000016a0: 2061 6e64 2070 6173 7369 6e67 2074 6865   and passing the
-000016b0: 2066 6f6c 6c6f 7769 6e67 2070 6172 616d   following param
-000016c0: 6574 6572 732e 0a0a 2d20 6074 7331 6020  eters...- `ts1` 
-000016d0: 5468 6973 2074 696d 6520 7365 7269 6573  This time series
-000016e0: 206d 6179 2072 6570 7265 7365 6e74 2074   may represent t
-000016f0: 6865 2062 6173 656c 696e 6520 6f72 2067  he baseline or g
-00001700: 726f 756e 6420 7472 7574 6820 7469 6d65  round truth time
-00001710: 0a20 2073 6572 6965 7320 6173 2061 2060  .  series as a `
-00001720: 6e75 6d70 7960 206f 626a 6563 7420 7769  numpy` object wi
-00001730: 7468 2073 6861 7065 2060 5b6c 656e 6774  th shape `[lengt
-00001740: 682c 206e 756d 5f66 6561 7475 7265 735d  h, num_features]
-00001750: 602e 0a2d 2060 7473 3273 6020 4120 7369  `..- `ts2s` A si
-00001760: 6e67 6c65 206f 7220 6120 7365 7420 6f66  ngle or a set of
-00001770: 2074 696d 6520 7365 7269 6573 2061 7320   time series as 
-00001780: 6120 606e 756d 7079 6020 6f62 6a65 6374  a `numpy` object
-00001790: 2077 6974 6820 7368 6170 6520 605b 6e75   with shape `[nu
-000017a0: 6d5f 7469 6d65 5f73 6572 6965 732c 206c  m_time_series, l
-000017b0: 656e 6774 682c 206e 756d 5f66 6561 7475  ength, num_featu
-000017c0: 7265 735d 602e 0a0a 0a43 6f6e 7374 7261  res]`....Constra
-000017d0: 696e 7473 3a0a 0a2d 2060 7473 3160 2074  ints:..- `ts1` t
-000017e0: 696d 652d 7365 7269 6573 2061 6e64 2060  ime-series and `
-000017f0: 7473 3273 6020 7469 6d65 2d73 6572 6965  ts2s` time-serie
-00001800: 7320 6669 6c65 2873 2920 6d75 7374 3a0a  s file(s) must:.
-00001810: 2020 2020 2d20 6861 7665 2074 6865 2073      - have the s
-00001820: 616d 6520 6469 6d65 6e73 696f 6e61 6c69  ame dimensionali
-00001830: 7479 2028 6e75 6d62 6572 206f 6620 636f  ty (number of co
-00001840: 6c75 6d6e 7329 0a20 2020 202d 2064 6f20  lumns).    - do 
-00001850: 6e6f 7420 696e 636c 7564 6520 6120 7469  not include a ti
-00001860: 6d65 7374 616d 7020 636f 6c75 6d6e 0a20  mestamp column. 
-00001870: 2020 202d 2069 6e63 6c75 6465 206f 6e6c     - include onl
-00001880: 7920 6e75 6d65 7269 6320 7661 6c75 6573  y numeric values
-00001890: 0a2d 2061 6c6c 2060 7473 3273 6020 7469  .- all `ts2s` ti
-000018a0: 6d65 2d73 6572 6965 7320 6d75 7374 2068  me-series must h
-000018b0: 6176 6520 7468 6520 7361 6d65 206c 656e  ave the same len
-000018c0: 6774 6820 286e 756d 6265 7220 6f66 2072  gth (number of r
-000018d0: 6f77 7329 2e0a 0a49 6620 6074 7331 6020  ows)...If `ts1` 
-000018e0: 7469 6d65 2d73 6572 6965 7320 6973 206c  time-series is l
-000018f0: 6f6e 6765 7220 286d 6f72 6520 726f 7773  onger (more rows
-00001900: 2920 7468 616e 2060 7473 3273 6020 7469  ) than `ts2s` ti
-00001910: 6d65 2d73 6572 6965 732c 2074 6865 2060  me-series, the `
-00001920: 7473 3160 2074 696d 6520 7365 7269 6573  ts1` time series
-00001930: 2077 696c 6c20 6265 0a64 6976 6964 6564   will be.divided
-00001940: 2069 6e20 7769 6e64 6f77 7320 6f66 2074   in windows of t
-00001950: 6865 2073 616d 6520 6c65 6e67 7468 2061  he same length a
-00001960: 7320 7468 6520 6074 7332 7360 2074 696d  s the `ts2s` tim
-00001970: 652d 7365 7269 6573 2e0a 0a46 6f72 2065  e-series...For e
-00001980: 6163 6820 6074 7332 7360 2074 696d 652d  ach `ts2s` time-
-00001990: 7365 7269 6573 2c20 7468 6520 6d6f 7374  series, the most
-000019a0: 2073 696d 696c 6172 2077 696e 646f 7720   similar window 
-000019b0: 282a 2920 6672 6f6d 2060 7473 3160 2074  (*) from `ts1` t
-000019c0: 696d 6520 7365 7269 6573 2069 7320 7365  ime series is se
-000019d0: 6c65 6374 6564 2e0a 0a46 696e 616c 6c79  lected...Finally
-000019e0: 2c20 6d65 7472 6963 7320 616e 6420 6669  , metrics and fi
-000019f0: 6775 7265 7320 7468 6174 2061 7373 6573  gures that asses
-00001a00: 7320 7468 6520 7369 6d69 6c61 7269 7479  s the similarity
-00001a10: 2062 6574 7765 656e 2065 6163 6820 7061   between each pa
-00001a20: 6972 206f 6620 6074 7332 7360 2074 696d  ir of `ts2s` tim
-00001a30: 652d 7365 7269 6573 2061 6e64 2069 7473  e-series and its
-00001a40: 0a61 7373 6f63 6961 7465 6420 6d6f 7374  .associated most
-00001a50: 2073 696d 696c 6172 2060 7473 3160 2077   similar `ts1` w
-00001a60: 696e 646f 7720 6172 6520 636f 6d70 7574  indow are comput
-00001a70: 6564 2e0a 0a28 2a29 2054 6865 206d 6574  ed...(*) The met
-00001a80: 7269 6320 7573 6564 2066 6f72 2074 6865  ric used for the
-00001a90: 2073 656c 6563 7469 6f6e 206f 6620 7468   selection of th
-00001aa0: 6520 6d6f 7374 0a73 696d 696c 6172 2060  e most.similar `
-00001ab0: 7473 3160 2074 696d 652d 7365 7269 6573  ts1` time-series
-00001ac0: 2077 696e 646f 7720 7065 7220 6561 6368   window per each
-00001ad0: 2060 7473 3273 6020 7469 6d65 2d73 6572   `ts2s` time-ser
-00001ae0: 6965 7320 6669 6c65 2069 7320 7365 6c65  ies file is sele
-00001af0: 6374 6162 6c65 2e60 6474 7760 2069 7320  ctable.`dtw` is 
-00001b00: 7468 6520 6465 6661 756c 7420 7365 6c65  the default sele
-00001b10: 6374 6564 206d 6574 7269 632c 2068 6f77  cted metric, how
-00001b20: 6576 6572 2c20 616e 7920 6f66 0a74 6865  ever, any of.the
-00001b30: 0a5b 6d65 7472 6963 735d 2823 6176 6169  .[metrics](#avai
-00001b40: 6c61 626c 652d 6d65 7472 6963 7329 2061  lable-metrics) a
-00001b50: 7265 2061 6c73 6f20 6176 6169 6c61 626c  re also availabl
-00001b60: 6520 666f 7220 7468 6973 2070 7572 706f  e for this purpo
-00001b70: 7365 2e20 5365 6520 7468 6520 5b74 6f6f  se. See the [too
-00001b80: 6c6b 6974 2063 6f6e 6669 6775 7261 7469  lkit configurati
-00001b90: 6f6e 2073 6563 7469 6f6e 5d28 2363 6f6e  on section](#con
-00001ba0: 6669 6775 7269 6e67 2d74 6865 2d74 6f6f  figuring-the-too
-00001bb0: 6c6b 6974 290a 0a23 2323 204d 696e 696d  lkit)..### Minim
-00001bc0: 616c 2075 7361 6765 2065 7861 6d70 6c65  al usage example
-00001bd0: 733a 0a55 7361 6765 2065 7861 6d70 6c65  s:.Usage example
-00001be0: 7320 6361 6e20 6265 2066 6f75 6e64 2061  s can be found a
-00001bf0: 743a 2068 7474 7073 3a2f 2f67 6974 6875  t: https://githu
-00001c00: 622e 636f 6d2f 616c 656a 616e 6472 6f66  b.com/alejandrof
-00001c10: 6465 7a2d 7573 2f73 696d 696c 6172 6974  dez-us/similarit
-00001c20: 792d 7473 2f74 7265 652f 6d61 696e 2f75  y-ts/tree/main/u
-00001c30: 7361 6765 5f65 7861 6d70 6c65 730a 0a31  sage_examples..1
-00001c40: 2e20 436f 6d70 7574 6520 6d65 7472 6963  . Compute metric
-00001c50: 7320 6265 7477 6565 6e20 7261 6e64 6f6d  s between random
-00001c60: 2074 696d 6520 7365 7269 6573 2028 6074   time series (`t
-00001c70: 7331 603a 206f 6e65 2074 696d 6520 7365  s1`: one time se
-00001c80: 7269 6573 206f 6620 6c65 6e67 6874 2032  ries of lenght 2
-00001c90: 3030 2061 6e64 2032 2064 696d 656e 7369  00 and 2 dimensi
-00001ca0: 6f6e 7320 616e 6420 6074 7332 603a 2066  ons and `ts2`: f
-00001cb0: 6976 6520 7469 6d65 2073 6572 6965 7320  ive time series 
-00001cc0: 6f66 206c 656e 6774 6820 3130 3020 616e  of length 100 an
-00001cd0: 6420 3220 6469 6d65 6e73 696f 6e73 293a  d 2 dimensions):
-00001ce0: 0a20 2020 2060 6060 5079 7468 6f6e 0a20  .    ```Python. 
-00001cf0: 2020 2069 6d70 6f72 7420 6e75 6d70 7920     import numpy 
-00001d00: 6173 206e 700a 2020 2020 6672 6f6d 2073  as np.    from s
-00001d10: 696d 696c 6172 6974 795f 7473 2e73 696d  imilarity_ts.sim
-00001d20: 696c 6172 6974 795f 7473 2069 6d70 6f72  ilarity_ts impor
-00001d30: 7420 5369 6d69 6c61 7269 7479 5473 0a20  t SimilarityTs. 
-00001d40: 2020 200a 2020 2020 7473 3120 3d20 6e70     .    ts1 = np
-00001d50: 2e72 616e 646f 6d2e 7261 6e64 2832 3030  .random.rand(200
-00001d60: 2c20 3229 0a20 2020 2074 7332 7320 3d20  , 2).    ts2s = 
-00001d70: 6e70 2e72 616e 646f 6d2e 7261 6e64 2835  np.random.rand(5
-00001d80: 2c20 3130 302c 2032 290a 2020 2020 7369  , 100, 2).    si
-00001d90: 6d69 6c61 7269 7479 5f74 7320 3d20 5369  milarity_ts = Si
-00001da0: 6d69 6c61 7269 7479 5473 2874 7331 2c20  milarityTs(ts1, 
-00001db0: 7473 3273 290a 2020 2020 666f 7220 7473  ts2s).    for ts
-00001dc0: 325f 6e61 6d65 2c20 6d65 7472 6963 5f6e  2_name, metric_n
-00001dd0: 616d 652c 2063 6f6d 7075 7465 645f 6d65  ame, computed_me
-00001de0: 7472 6963 2069 6e20 7369 6d69 6c61 7269  tric in similari
-00001df0: 7479 5f74 732e 6765 745f 6d65 7472 6963  ty_ts.get_metric
-00001e00: 5f63 6f6d 7075 7465 7228 293a 0a20 2020  _computer():.   
-00001e10: 2020 2020 2070 7269 6e74 2866 277b 7473       print(f'{ts
-00001e20: 325f 6e61 6d65 7d2e 207b 6d65 7472 6963  2_name}. {metric
-00001e30: 5f6e 616d 657d 3a20 7b63 6f6d 7075 7465  _name}: {compute
-00001e40: 645f 6d65 7472 6963 7d27 290a 2020 2020  d_metric}').    
-00001e50: 6060 600a 0a31 2e20 436f 6d70 7574 6520  ```..1. Compute 
-00001e60: 6d65 7472 6963 7320 616e 6420 6669 6775  metrics and figu
-00001e70: 7265 7320 6265 7477 6565 6e20 7261 6e64  res between rand
-00001e80: 6f6d 2074 696d 6520 7365 7269 6573 2061  om time series a
-00001e90: 6e64 2073 6176 6520 6669 6775 7265 733a  nd save figures:
-00001ea0: 0a20 2020 2060 6060 5079 7468 6f6e 0a20  .    ```Python. 
-00001eb0: 2020 2069 6d70 6f72 7420 6f73 0a20 2020     import os.   
-00001ec0: 2069 6d70 6f72 7420 6e75 6d70 7920 6173   import numpy as
-00001ed0: 206e 700a 2020 2020 6672 6f6d 2073 696d   np.    from sim
-00001ee0: 696c 6172 6974 795f 7473 2e70 6c6f 7473  ilarity_ts.plots
-00001ef0: 2e70 6c6f 745f 6661 6374 6f72 7920 696d  .plot_factory im
-00001f00: 706f 7274 2050 6c6f 7446 6163 746f 7279  port PlotFactory
-00001f10: 0a20 2020 2066 726f 6d20 7369 6d69 6c61  .    from simila
-00001f20: 7269 7479 5f74 732e 7369 6d69 6c61 7269  rity_ts.similari
-00001f30: 7479 5f74 7320 696d 706f 7274 2053 696d  ty_ts import Sim
-00001f40: 696c 6172 6974 7954 730a 2020 2020 0a20  ilarityTs.    . 
-00001f50: 2020 2064 6566 206d 6169 6e28 293a 0a20     def main():. 
-00001f60: 2020 2020 2020 2074 7331 203d 206e 702e         ts1 = np.
-00001f70: 7261 6e64 6f6d 2e72 616e 6428 3230 302c  random.rand(200,
-00001f80: 2032 290a 2020 2020 2020 2020 7473 3273   2).        ts2s
-00001f90: 203d 206e 702e 7261 6e64 6f6d 2e72 616e   = np.random.ran
-00001fa0: 6428 352c 2031 3030 2c20 3229 0a20 2020  d(5, 100, 2).   
-00001fb0: 2020 2020 2073 696d 696c 6172 6974 795f       similarity_
-00001fc0: 7473 203d 2053 696d 696c 6172 6974 7954  ts = SimilarityT
-00001fd0: 7328 7473 312c 2074 7332 7329 0a20 2020  s(ts1, ts2s).   
-00001fe0: 2020 2020 2066 6f72 2074 7332 5f6e 616d       for ts2_nam
-00001ff0: 652c 206d 6574 7269 635f 6e61 6d65 2c20  e, metric_name, 
-00002000: 636f 6d70 7574 6564 5f6d 6574 7269 6320  computed_metric 
-00002010: 696e 2073 696d 696c 6172 6974 795f 7473  in similarity_ts
-00002020: 2e67 6574 5f6d 6574 7269 635f 636f 6d70  .get_metric_comp
-00002030: 7574 6572 2829 3a0a 2020 2020 2020 2020  uter():.        
-00002040: 2020 2020 7072 696e 7428 6627 7b74 7332      print(f'{ts2
-00002050: 5f6e 616d 657d 2e20 7b6d 6574 7269 635f  _name}. {metric_
-00002060: 6e61 6d65 7d3a 207b 636f 6d70 7574 6564  name}: {computed
-00002070: 5f6d 6574 7269 637d 2729 0a20 2020 2020  _metric}').     
-00002080: 2020 2066 6f72 2074 7332 5f6e 616d 652c     for ts2_name,
-00002090: 2070 6c6f 745f 6e61 6d65 2c20 6765 6e65   plot_name, gene
-000020a0: 7261 7465 645f 706c 6f74 7320 696e 2073  rated_plots in s
-000020b0: 696d 696c 6172 6974 795f 7473 2e67 6574  imilarity_ts.get
-000020c0: 5f70 6c6f 745f 636f 6d70 7574 6572 2829  _plot_computer()
-000020d0: 3a0a 2020 2020 2020 2020 2020 2020 5f5f  :.            __
-000020e0: 7361 7665 5f66 6967 7572 6573 2874 7332  save_figures(ts2
-000020f0: 5f6e 616d 652c 2070 6c6f 745f 6e61 6d65  _name, plot_name
-00002100: 2c20 6765 6e65 7261 7465 645f 706c 6f74  , generated_plot
-00002110: 7329 0a20 2020 200a 2020 2020 0a20 2020  s).    .    .   
-00002120: 2064 6566 205f 5f73 6176 655f 6669 6775   def __save_figu
-00002130: 7265 7328 6669 6c65 6e61 6d65 2c20 706c  res(filename, pl
-00002140: 6f74 5f6e 616d 652c 2067 656e 6572 6174  ot_name, generat
-00002150: 6564 5f70 6c6f 7473 293a 0a20 2020 2020  ed_plots):.     
-00002160: 2020 2066 6f72 2070 6c6f 7420 696e 2067     for plot in g
-00002170: 656e 6572 6174 6564 5f70 6c6f 7473 3a0a  enerated_plots:.
-00002180: 2020 2020 2020 2020 2020 2020 6469 725f              dir_
-00002190: 7061 7468 203d 205f 5f63 7265 6174 655f  path = __create_
-000021a0: 6469 7265 6374 6f72 7928 6669 6c65 6e61  directory(filena
-000021b0: 6d65 2c20 6627 6669 6775 7265 7327 2c20  me, f'figures', 
-000021c0: 706c 6f74 5f6e 616d 6529 0a20 2020 2020  plot_name).     
-000021d0: 2020 2020 2020 2070 6c6f 745b 305d 2e73         plot[0].s
-000021e0: 6176 6566 6967 2866 277b 6469 725f 7061  avefig(f'{dir_pa
-000021f0: 7468 7d7b 706c 6f74 5b30 5d2e 6178 6573  th}{plot[0].axes
-00002200: 5b30 5d2e 6765 745f 7469 746c 6528 297d  [0].get_title()}
-00002210: 2e70 6466 272c 2066 6f72 6d61 743d 2770  .pdf', format='p
-00002220: 6466 272c 2062 626f 785f 696e 6368 6573  df', bbox_inches
-00002230: 3d27 7469 6768 7427 290a 2020 2020 0a20  ='tight').    . 
-00002240: 2020 200a 2020 2020 6465 6620 5f5f 6372     .    def __cr
-00002250: 6561 7465 5f64 6972 6563 746f 7279 2866  eate_directory(f
-00002260: 696c 656e 616d 652c 2070 6174 682c 2070  ilename, path, p
-00002270: 6c6f 745f 6e61 6d65 293a 0a20 2020 2020  lot_name):.     
-00002280: 2020 2069 6620 706c 6f74 5f6e 616d 6520     if plot_name 
-00002290: 696e 2050 6c6f 7446 6163 746f 7279 2e67  in PlotFactory.g
-000022a0: 6574 5f69 6e73 7461 6e63 6528 292e 6669  et_instance().fi
-000022b0: 6775 7265 735f 7265 7175 6972 6573 5f61  gures_requires_a
-000022c0: 6c6c 5f73 616d 706c 6573 3a0a 2020 2020  ll_samples:.    
-000022d0: 2020 2020 2020 2020 6469 725f 7061 7468          dir_path
-000022e0: 203d 2066 277b 7061 7468 7d2f 7b70 6c6f   = f'{path}/{plo
-000022f0: 745f 6e61 6d65 7d2f 270a 2020 2020 2020  t_name}/'.      
-00002300: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00002310: 2020 2020 6f72 6967 696e 616c 5f66 696c      original_fil
-00002320: 656e 616d 6520 3d20 6f73 2e70 6174 682e  ename = os.path.
-00002330: 7370 6c69 7465 7874 2866 696c 656e 616d  splitext(filenam
-00002340: 6529 5b30 5d0a 2020 2020 2020 2020 2020  e)[0].          
-00002350: 2020 6469 725f 7061 7468 203d 2066 277b    dir_path = f'{
-00002360: 7061 7468 7d2f 7b6f 7269 6769 6e61 6c5f  path}/{original_
-00002370: 6669 6c65 6e61 6d65 7d2f 7b70 6c6f 745f  filename}/{plot_
-00002380: 6e61 6d65 7d2f 270a 2020 2020 2020 2020  name}/'.        
-00002390: 6f73 2e6d 616b 6564 6972 7328 6469 725f  os.makedirs(dir_
-000023a0: 7061 7468 2c20 6578 6973 745f 6f6b 3d54  path, exist_ok=T
-000023b0: 7275 6529 0a20 2020 2020 2020 2072 6574  rue).        ret
-000023c0: 7572 6e20 6469 725f 7061 7468 0a20 2020  urn dir_path.   
-000023d0: 200a 2020 2020 6966 205f 5f6e 616d 655f   .    if __name_
-000023e0: 5f20 3d3d 2027 5f5f 6d61 696e 5f5f 273a  _ == '__main__':
-000023f0: 0a20 2020 2020 2020 206d 6169 6e28 290a  .        main().
-00002400: 2020 2020 6060 600a 0a23 2320 436f 6e66      ```..## Conf
-00002410: 6967 7572 696e 6720 7468 6520 546f 6f6c  iguring the Tool
-00002420: 6b69 740a 5573 6572 7320 6361 6e20 7072  kit.Users can pr
-00002430: 6f76 6964 6520 6d65 7472 6963 7320 6f72  ovide metrics or
-00002440: 2066 6967 7572 6573 2074 6f20 6265 2063   figures to be c
-00002450: 6f6d 7075 7465 642f 6765 6e65 7261 7465  omputed/generate
-00002460: 6420 616e 6420 736f 6d65 206f 7468 6572  d and some other
-00002470: 2070 6172 616d 6574 6572 6973 6174 696f   parameterisatio
-00002480: 6e2e 2054 6865 2066 6f6c 6c6f 7769 6e67  n. The following
-00002490: 2063 6f64 6520 736e 6970 7065 7420 0a63   code snippet .c
-000024a0: 7265 6174 6573 2061 2063 6f6e 6669 6775  reates a configu
-000024b0: 7261 7469 6f6e 206f 626a 6563 7420 7468  ration object th
-000024c0: 6174 2073 686f 756c 6420 6265 2070 6173  at should be pas
-000024d0: 7365 6420 746f 2074 6865 2060 5369 6d69  sed to the `Simi
-000024e0: 6c61 7269 7479 5473 6020 636f 6e73 7472  larityTs` constr
-000024f0: 7563 746f 723a 0a60 6060 5079 7468 6f6e  uctor:.```Python
-00002500: 0a64 6566 205f 5f63 7265 6174 655f 7369  .def __create_si
-00002510: 6d69 6c61 7269 7479 5f74 735f 636f 6e66  milarity_ts_conf
-00002520: 6967 2829 3a0a 2020 2020 2320 5468 6520  ig():.    # The 
-00002530: 6c69 7374 206f 6620 6d65 7472 6963 7320  list of metrics 
-00002540: 6e61 6d65 7320 7468 6174 2077 696c 6c20  names that will 
-00002550: 6265 2063 6f6d 7075 7465 640a 2020 2020  be computed.    
-00002560: 6d65 7472 6963 5f63 6f6e 6669 6720 3d20  metric_config = 
-00002570: 4d65 7472 6963 436f 6e66 6967 285b 276a  MetricConfig(['j
-00002580: 7327 2c20 276d 6d64 275d 2920 0a20 2020  s', 'mmd']) .   
-00002590: 2023 2054 6865 206c 6973 7420 6f66 2066   # The list of f
-000025a0: 6967 7572 6520 6e61 6d65 7320 7468 6174  igure names that
-000025b0: 2077 696c 6c20 6265 2067 656e 6572 6174   will be generat
-000025c0: 6564 2061 6e64 2074 6865 2074 696d 6520  ed and the time 
-000025d0: 7374 6570 2069 6e20 7365 636f 6e64 7320  step in seconds 
-000025e0: 6f66 2074 6865 2074 696d 6520 7365 7269  of the time seri
-000025f0: 6573 2e0a 2020 2020 706c 6f74 5f63 6f6e  es..    plot_con
-00002600: 6669 6720 3d20 506c 6f74 436f 6e66 6967  fig = PlotConfig
-00002610: 285b 2764 656c 7461 272c 2027 7063 6127  (['delta', 'pca'
-00002620: 5d2c 2074 696d 6573 7461 6d70 5f66 7265  ], timestamp_fre
-00002630: 7175 656e 6379 5f73 6563 6f6e 6473 3d33  quency_seconds=3
-00002640: 3030 290a 0a20 2020 2023 204e 616d 6520  00)..    # Name 
-00002650: 6f66 2065 6163 6820 7469 6d65 2073 6572  of each time ser
-00002660: 6965 7320 6f66 2074 6865 2074 7332 7320  ies of the ts2s 
-00002670: 7365 7420 6f66 2074 696d 6520 7365 7269  set of time seri
-00002680: 6573 0a20 2020 2074 7332 5f6e 616d 6573  es.    ts2_names
-00002690: 203d 205b 2774 7332 5f31 5f6e 616d 6527   = ['ts2_1_name'
-000026a0: 2c20 2774 7332 5f32 5f6e 616d 6527 2c20  , 'ts2_2_name', 
-000026b0: 2774 7332 5f33 5f6e 616d 6527 2c20 2774  'ts2_3_name', 't
-000026c0: 7332 5f34 5f6e 616d 6527 2c20 2774 7332  s2_4_name', 'ts2
-000026d0: 5f35 5f6e 616d 6527 5d0a 2020 2020 2320  _5_name'].    # 
-000026e0: 4e61 6d65 206f 6620 7468 6520 6665 6174  Name of the feat
-000026f0: 7572 6573 0a20 2020 2068 6561 6465 725f  ures.    header_
-00002700: 6e61 6d65 7320 3d20 5b27 6665 6174 7572  names = ['featur
-00002710: 6531 5f6e 616d 6527 2c20 2766 6561 7475  e1_name', 'featu
-00002720: 7265 325f 6e61 6d65 275d 0a20 2020 200a  re2_name'].    .
-00002730: 2020 2020 2320 4372 6561 7469 6f6e 206f      # Creation o
-00002740: 6620 7468 6520 636f 6e66 6967 7572 6174  f the configurat
-00002750: 696f 6e0a 2020 2020 2020 2320 7374 7269  ion.      # stri
-00002760: 6465 2066 6f72 2063 7574 7469 6e67 2074  de for cutting t
-00002770: 6865 2074 7331 2077 6865 6e20 6e65 6564  he ts1 when need
-00002780: 6564 0a20 2020 2020 2023 206d 6574 7269  ed.      # metri
-00002790: 6320 7573 6564 2066 6f72 2073 656c 6563  c used for selec
-000027a0: 7469 6e67 2074 6865 206d 6f73 7420 7369  ting the most si
-000027b0: 6d69 6c61 7220 7769 6e64 6f77 0a20 2020  milar window.   
-000027c0: 2073 696d 696c 6172 6974 795f 7473 5f63   similarity_ts_c
-000027d0: 6f6e 6669 6720 3d20 5369 6d69 6c61 7269  onfig = Similari
-000027e0: 7479 5473 436f 6e66 6967 286d 6574 7269  tyTsConfig(metri
-000027f0: 635f 636f 6e66 6967 2c20 706c 6f74 5f63  c_config, plot_c
-00002800: 6f6e 6669 672c 0a20 2020 2020 2020 2020  onfig,.         
-00002810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002830: 2020 2020 2073 7472 6964 653d 3130 2c20       stride=10, 
-00002840: 7769 6e64 6f77 5f73 656c 6563 7469 6f6e  window_selection
-00002850: 5f6d 6574 7269 633d 276b 6c27 2c0a 2020  _metric='kl',.  
-00002860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002880: 2020 2020 2020 2020 2020 2020 7473 325f              ts2_
-00002890: 6e61 6d65 733d 7473 325f 6e61 6d65 732c  names=ts2_names,
-000028a0: 2068 6561 6465 725f 6e61 6d65 733d 6865   header_names=he
-000028b0: 6164 6572 5f6e 616d 6573 290a 2020 2020  ader_names).    
-000028c0: 7265 7475 726e 2073 696d 696c 6172 6974  return similarit
-000028d0: 795f 7473 5f63 6f6e 6669 670a 6060 600a  y_ts_config.```.
-000028e0: 0a49 6620 6e6f 206d 6574 7269 6373 206e  .If no metrics n
-000028f0: 6f72 2066 6967 7572 6573 2061 7265 2070  or figures are p
-00002900: 726f 7669 6465 642c 2074 6865 2074 6f6f  rovided, the too
-00002910: 6c20 7769 6c6c 2063 6f6d 7075 7465 2061  l will compute a
-00002920: 6c6c 2074 6865 2061 7661 696c 6162 6c65  ll the available
-00002930: 206d 6574 7269 6373 2061 6e64 2066 6967   metrics and fig
-00002940: 7572 6573 2e0a 0a54 6865 2066 6f6c 6c6f  ures...The follo
-00002950: 7769 6e67 2061 7267 756d 656e 7473 2061  wing arguments a
-00002960: 7265 2061 6c73 6f20 6176 6169 6c61 626c  re also availabl
-00002970: 6520 666f 7220 6669 6e65 2d74 756e 696e  e for fine-tunin
-00002980: 673a 0a0a 2d20 6074 696d 6573 7461 6d70  g:..- `timestamp
-00002990: 5f66 7265 7175 656e 6379 5f73 6563 6f6e  _frequency_secon
-000029a0: 6473 603a 2074 6865 2066 7265 7175 656e  ds`: the frequen
-000029b0: 6379 2069 6e20 7365 636f 6e64 7320 696e  cy in seconds in
-000029c0: 2077 6869 6368 2073 616d 706c 6573 2077   which samples w
-000029d0: 6572 6520 7461 6b65 6e2e 2054 6869 7320  ere taken. This 
-000029e0: 6973 206e 6565 6465 6420 746f 2067 656e  is needed to gen
-000029f0: 6572 6174 6520 7468 6520 6465 6c74 6120  erate the delta 
-00002a00: 6669 6775 7265 7320 7769 7468 2063 6f72  figures with cor
-00002a10: 7265 6374 2074 696d 6520 6d61 676e 6974  rect time magnit
-00002a20: 7564 6573 2e20 4279 2064 6566 6175 6c74  udes. By default
-00002a30: 2069 730a 2020 6031 6020 7365 636f 6e64   is.  `1` second
-00002a40: 2e0a 2d20 6073 7472 6964 6560 3a20 7768  ..- `stride`: wh
-00002a50: 656e 2060 7473 3160 2074 696d 652d 7365  en `ts1` time-se
-00002a60: 7269 6573 2069 7320 6c6f 6e67 6572 2074  ries is longer t
-00002a70: 6861 6e20 6074 7332 7360 2074 696d 652d  han `ts2s` time-
-00002a80: 7365 7269 6573 2074 6865 2077 696e 646f  series the windo
-00002a90: 7773 2061 7265 2063 6f6d 7075 7465 6420  ws are computed 
-00002aa0: 6279 2075 7369 6e67 2061 0a20 2073 7472  by using a.  str
-00002ab0: 6964 6520 6f66 2060 3160 2062 7920 6465  ide of `1` by de
-00002ac0: 6661 756c 742e 2053 6f6d 6574 696d 6573  fault. Sometimes
-00002ad0: 2075 7369 6e67 2061 206c 6172 6765 7220   using a larger 
-00002ae0: 7661 6c75 6520 666f 7220 7468 6520 7374  value for the st
-00002af0: 7269 6465 2070 6172 616d 6574 6572 2069  ride parameter i
-00002b00: 6d70 726f 7665 7320 7468 6520 7065 7266  mproves the perf
-00002b10: 6f72 6d61 6e63 6520 6279 2073 6b69 7070  ormance by skipp
-00002b20: 696e 670a 2020 7468 6520 636f 6d70 7574  ing.  the comput
-00002b30: 6174 696f 6e20 6f66 2073 696d 696c 6172  ation of similar
-00002b40: 6974 7920 6265 7477 6565 6e20 736f 206d  ity between so m
-00002b50: 616e 7920 7769 6e64 6f77 732e 0a2d 2060  any windows..- `
-00002b60: 7769 6e64 6f77 5f73 656c 6563 7469 6f6e  window_selection
-00002b70: 5f6d 6574 7269 6360 3a20 7468 6520 6d65  _metric`: the me
-00002b80: 7472 6963 2075 7365 6420 666f 7220 7468  tric used for th
-00002b90: 6520 7365 6c65 6374 696f 6e20 6f66 2074  e selection of t
-00002ba0: 6865 206d 6f73 7420 7369 6d69 6c61 7220  he most similar 
-00002bb0: 6074 7331 6020 7469 6d65 2d73 6572 6965  `ts1` time-serie
-00002bc0: 7320 7769 6e64 6f77 2070 6572 2065 6163  s window per eac
-00002bd0: 6820 6074 7332 7360 2074 696d 652d 7365  h `ts2s` time-se
-00002be0: 7269 6573 2066 696c 6520 6973 2073 656c  ries file is sel
-00002bf0: 6563 7461 626c 652e 6064 7477 6020 6973  ectable.`dtw` is
-00002c00: 2074 6865 2064 6566 6175 6c74 2073 656c   the default sel
-00002c10: 6563 7465 6420 6d65 7472 6963 2c20 686f  ected metric, ho
-00002c20: 7765 7665 722c 2061 6e79 206f 6620 7468  wever, any of th
-00002c30: 6520 5b6d 6574 7269 6373 5d28 2361 7661  e [metrics](#ava
-00002c40: 696c 6162 6c65 2d6d 6574 7269 6373 2920  ilable-metrics) 
-00002c50: 6172 6520 616c 736f 2061 7661 696c 6162  are also availab
-00002c60: 6c65 2066 6f72 2074 6869 7320 7075 7270  le for this purp
-00002c70: 6f73 652e 2053 6565 2074 6865 205b 746f  ose. See the [to
-00002c80: 6f6c 6b69 7420 636f 6e66 6967 7572 6174  olkit configurat
-00002c90: 696f 6e20 7365 6374 696f 6e5d 2823 636f  ion section](#co
-00002ca0: 6e66 6967 7572 696e 672d 7468 652d 746f  nfiguring-the-to
-00002cb0: 6f6c 6b69 7429 2e0a 2d20 6074 7332 5f6e  olkit)..- `ts2_n
-00002cc0: 616d 6573 603a 206e 616d 6520 6f66 2065  ames`: name of e
-00002cd0: 6163 6820 7469 6d65 2073 6572 6965 7320  ach time series 
-00002ce0: 6f66 2074 6865 2060 7473 3273 6020 7365  of the `ts2s` se
-00002cf0: 7420 6f66 2074 696d 6520 7365 7269 6573  t of time series
-00002d00: 2e0a 2d20 6068 6561 6465 725f 6e61 6d65  ..- `header_name
-00002d10: 7360 3a20 6e61 6d65 206f 6620 7468 6520  s`: name of the 
-00002d20: 6665 6174 7572 6573 0a0a 0a23 2320 4578  features...## Ex
-00002d30: 7465 6e64 696e 6720 7468 6520 746f 6f6c  tending the tool
-00002d40: 6b69 740a 0a41 6464 6974 696f 6e61 6c6c  kit..Additionall
-00002d50: 792c 2075 7365 7273 206d 6179 2069 6d70  y, users may imp
-00002d60: 6c65 6d65 6e74 2074 6865 6972 206f 776e  lement their own
-00002d70: 206d 6574 7269 6320 6f72 2066 6967 7572   metric or figur
-00002d80: 6520 636c 6173 7365 7320 616e 6420 696e  e classes and in
-00002d90: 636c 7564 6520 7468 656d 2062 7920 7573  clude them by us
-00002da0: 696e 6720 7468 6520 604d 6574 7269 6346  ing the `MetricF
-00002db0: 6163 746f 7279 6020 6f72 2060 506c 6f74  actory` or `Plot
-00002dc0: 4661 6374 6f72 7960 2072 6567 6973 7465  Factory` registe
-00002dd0: 7220 6d65 7468 6f64 732e 2054 6f20 656e  r methods. To en
-00002de0: 7375 7265 2063 6f6d 7061 7469 6269 6c69  sure compatibili
-00002df0: 7479 2077 6974 6820 6f75 7220 746f 6f6c  ty with our tool
-00002e00: 6b69 742c 2074 6865 7920 6861 7665 2074  kit, they have t
-00002e10: 6f20 696e 6865 7269 7420 6672 6f6d 2074  o inherit from t
-00002e20: 6865 2062 6173 6520 636c 6173 7365 7320  he base classes 
-00002e30: 604d 6574 7269 6360 2061 6e64 2060 506c  `Metric` and `Pl
-00002e40: 6f74 602e 0a0a 5468 6520 666f 6c6c 6f77  ot`...The follow
-00002e50: 696e 6720 636f 6465 2073 6e69 7070 6574  ing code snippet
-00002e60: 2069 7320 616e 2065 7861 6d70 6c65 206f   is an example o
-00002e70: 6620 686f 7720 746f 2069 6e74 726f 6475  f how to introdu
-00002e80: 6365 2074 6865 2045 7563 6c69 6465 616e  ce the Euclidean
-00002e90: 2064 6973 7461 6e63 6520 6d65 7472 6963   distance metric
-00002ea0: 3a0a 0a60 6060 5079 7468 6f6e 0a23 6575  :..```Python.#eu
-00002eb0: 2e70 790a 696d 706f 7274 206e 756d 7079  .py.import numpy
-00002ec0: 2061 7320 6e70 0a66 726f 6d20 7369 6d69   as np.from simi
-00002ed0: 6c61 7269 7479 5f74 732e 6d65 7472 6963  larity_ts.metric
-00002ee0: 732e 6d65 7472 6963 2069 6d70 6f72 7420  s.metric import 
-00002ef0: 4d65 7472 6963 0a0a 0a63 6c61 7373 2045  Metric...class E
-00002f00: 7563 6c69 6465 616e 4469 7374 616e 6365  uclideanDistance
-00002f10: 284d 6574 7269 6329 3a0a 0a20 2020 2064  (Metric):..    d
-00002f20: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-00002f30: 293a 0a20 2020 2020 2020 2073 7570 6572  ):.        super
-00002f40: 2829 2e5f 5f69 6e69 745f 5f28 290a 2020  ().__init__().  
-00002f50: 2020 2020 2020 7365 6c66 2e6e 616d 6520        self.name 
-00002f60: 3d20 2765 6427 0a0a 2020 2020 6465 6620  = 'ed'..    def 
-00002f70: 636f 6d70 7574 6528 7365 6c66 2c20 7473  compute(self, ts
-00002f80: 312c 2074 7332 2c20 7369 6d69 6c61 7269  1, ts2, similari
-00002f90: 7479 5f74 7329 3a0a 2020 2020 2020 2020  ty_ts):.        
-00002fa0: 6d65 7472 6963 5f72 6573 756c 7420 3d20  metric_result = 
-00002fb0: 7b27 4d75 6c74 6976 6172 6961 7465 273a  {'Multivariate':
-00002fc0: 2073 656c 662e 5f5f 6564 2874 7331 2c20   self.__ed(ts1, 
-00002fd0: 7473 3229 7d0a 2020 2020 2020 2020 7265  ts2)}.        re
-00002fe0: 7475 726e 206d 6574 7269 635f 7265 7375  turn metric_resu
-00002ff0: 6c74 0a0a 2020 2020 6465 6620 636f 6d70  lt..    def comp
-00003000: 7574 655f 6469 7374 616e 6365 2873 656c  ute_distance(sel
-00003010: 662c 2074 7331 2c20 7473 3229 3a0a 2020  f, ts1, ts2):.  
-00003020: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00003030: 662e 5f5f 6564 2874 7331 2c20 7473 3229  f.__ed(ts1, ts2)
-00003040: 0a0a 2020 2020 6465 6620 5f5f 6564 2873  ..    def __ed(s
-00003050: 656c 662c 2074 7331 2c20 7473 3229 3a0a  elf, ts1, ts2):.
-00003060: 2020 2020 2020 2020 7265 7475 726e 206e          return n
-00003070: 702e 6c69 6e61 6c67 2e6e 6f72 6d28 7473  p.linalg.norm(ts
-00003080: 3120 2d20 7473 3229 0a0a 6060 600a 0a41  1 - ts2)..```..A
-00003090: 6674 6572 7761 7264 2c20 7468 6973 206d  fterward, this m
-000030a0: 6574 7269 6320 6361 6e20 6265 2072 6567  etric can be reg
-000030b0: 6973 7465 7265 6420 6279 2075 7369 6e67  istered by using
-000030c0: 2074 6865 2060 7265 6769 7374 6572 5f6d   the `register_m
-000030d0: 6574 7269 6328 6d65 7472 6963 5f63 6c61  etric(metric_cla
-000030e0: 7373 2960 206d 6574 686f 6420 6672 6f6d  ss)` method from
-000030f0: 2060 4d65 7472 6963 4661 6374 6f72 7960   `MetricFactory`
-00003100: 2061 7320 7368 6f77 6e20 696e 2074 6865   as shown in the
-00003110: 2066 6f6c 6c6f 7769 6e67 2063 6f64 6520   following code 
-00003120: 736e 6970 7065 743a 0a60 6060 5079 7468  snippet:.```Pyth
-00003130: 6f6e 0a69 6d70 6f72 7420 6e75 6d70 7920  on.import numpy 
-00003140: 6173 206e 700a 6672 6f6d 2073 696d 696c  as np.from simil
-00003150: 6172 6974 795f 7473 2e73 696d 696c 6172  arity_ts.similar
-00003160: 6974 795f 7473 2069 6d70 6f72 7420 5369  ity_ts import Si
-00003170: 6d69 6c61 7269 7479 5473 0a66 726f 6d20  milarityTs.from 
-00003180: 7369 6d69 6c61 7269 7479 5f74 732e 6d65  similarity_ts.me
-00003190: 7472 6963 732e 6d65 7472 6963 5f66 6163  trics.metric_fac
-000031a0: 746f 7279 2069 6d70 6f72 7420 4d65 7472  tory import Metr
-000031b0: 6963 4661 6374 6f72 790a 6672 6f6d 2065  icFactory.from e
-000031c0: 6420 696d 706f 7274 2045 7563 6c69 6465  d import Euclide
-000031d0: 616e 4469 7374 616e 6365 0a0a 4d65 7472  anDistance..Metr
-000031e0: 6963 4661 6374 6f72 792e 6765 745f 696e  icFactory.get_in
-000031f0: 7374 616e 6365 2829 2e72 6567 6973 7465  stance().registe
-00003200: 725f 6d65 7472 6963 2845 7563 6c69 6465  r_metric(Euclide
-00003210: 616e 4469 7374 616e 6365 290a 7473 3120  anDistance).ts1 
-00003220: 3d20 6e70 2e72 616e 646f 6d2e 7261 6e64  = np.random.rand
-00003230: 2832 3030 2c20 3229 0a74 7332 7320 3d20  (200, 2).ts2s = 
-00003240: 6e70 2e72 616e 646f 6d2e 7261 6e64 2835  np.random.rand(5
-00003250: 2c20 3130 302c 2032 290a 7369 6d69 6c61  , 100, 2).simila
-00003260: 7269 7479 5f74 7320 3d20 5369 6d69 6c61  rity_ts = Simila
-00003270: 7269 7479 5473 2874 7331 2c20 7473 3273  rityTs(ts1, ts2s
-00003280: 290a 666f 7220 7473 325f 6e61 6d65 2c20  ).for ts2_name, 
-00003290: 6d65 7472 6963 5f6e 616d 652c 2063 6f6d  metric_name, com
-000032a0: 7075 7465 645f 6d65 7472 6963 2069 6e20  puted_metric in 
-000032b0: 7369 6d69 6c61 7269 7479 5f74 732e 6765  similarity_ts.ge
-000032c0: 745f 6d65 7472 6963 5f63 6f6d 7075 7465  t_metric_compute
-000032d0: 7228 293a 0a20 2020 2070 7269 6e74 2866  r():.    print(f
-000032e0: 277b 7473 325f 6e61 6d65 7d2e 207b 6d65  '{ts2_name}. {me
-000032f0: 7472 6963 5f6e 616d 657d 3a20 7b63 6f6d  tric_name}: {com
-00003300: 7075 7465 645f 6d65 7472 6963 7d27 290a  puted_metric}').
-00003310: 6060 600a 0a53 696d 696c 6172 6c79 2c20  ```..Similarly, 
-00003320: 6e65 7720 706c 6f74 7320 6361 6e20 6265  new plots can be
-00003330: 2069 6e74 726f 6475 6365 642e 2046 6f72   introduced. For
-00003340: 2069 6e73 7461 6e63 6520 6120 6053 696d   instance a `Sim
-00003350: 696c 6172 6974 7950 6c6f 7442 7943 6f72  ilarityPlotByCor
-00003360: 7265 6c61 7469 6f6e 6020 636f 756c 6420  relation` could 
-00003370: 6265 2064 6566 696e 6564 2061 733a 0a60  be defined as:.`
-00003380: 6060 5079 7468 6f6e 0a23 6363 5f70 6c6f  ``Python.#cc_plo
-00003390: 742e 7079 0a69 6d70 6f72 7420 6e75 6d70  t.py.import nump
-000033a0: 7920 6173 206e 700a 696d 706f 7274 206d  y as np.import m
-000033b0: 6174 706c 6f74 6c69 622e 7079 706c 6f74  atplotlib.pyplot
-000033c0: 2061 7320 706c 740a 6672 6f6d 2073 696d   as plt.from sim
-000033d0: 696c 6172 6974 795f 7473 2e70 6c6f 7473  ilarity_ts.plots
-000033e0: 2e70 6c6f 7420 696d 706f 7274 2050 6c6f  .plot import Plo
-000033f0: 740a 0a0a 636c 6173 7320 5369 6d69 6c61  t...class Simila
-00003400: 7269 7479 506c 6f74 4279 436f 7272 656c  rityPlotByCorrel
-00003410: 6174 696f 6e28 506c 6f74 293a 0a0a 2020  ation(Plot):..  
-00003420: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-00003430: 656c 662c 2066 6967 5f73 697a 653d 2838  elf, fig_size=(8
-00003440: 2c20 3629 293a 0a20 2020 2020 2020 2073  , 6)):.        s
-00003450: 7570 6572 2829 2e5f 5f69 6e69 745f 5f28  uper().__init__(
-00003460: 6669 675f 7369 7a65 290a 2020 2020 2020  fig_size).      
-00003470: 2020 7365 6c66 2e6e 616d 6520 3d20 2763    self.name = 'c
-00003480: 632d 706c 6f74 270a 0a20 2020 2064 6566  c-plot'..    def
-00003490: 2063 6f6d 7075 7465 2873 656c 662c 2073   compute(self, s
-000034a0: 696d 696c 6172 6974 795f 7473 2c20 7473  imilarity_ts, ts
-000034b0: 325f 6669 6c65 6e61 6d65 293a 0a20 2020  2_filename):.   
-000034c0: 2020 2020 2073 7570 6572 2829 2e63 6f6d       super().com
-000034d0: 7075 7465 2873 696d 696c 6172 6974 795f  pute(similarity_
-000034e0: 7473 2c20 7473 325f 6669 6c65 6e61 6d65  ts, ts2_filename
-000034f0: 290a 2020 2020 2020 2020 6e5f 6665 6174  ).        n_feat
-00003500: 7572 6573 203d 2073 656c 662e 7473 312e  ures = self.ts1.
-00003510: 7368 6170 655b 315d 0a20 2020 2020 2020  shape[1].       
-00003520: 2073 696d 696c 6172 6974 7920 3d20 6e70   similarity = np
-00003530: 2e63 6f72 7263 6f65 6628 7365 6c66 2e74  .corrcoef(self.t
-00003540: 7331 2e54 2c20 7365 6c66 2e74 7332 2e54  s1.T, self.ts2.T
-00003550: 290a 2020 2020 2020 2020 6669 672c 2061  ).        fig, a
-00003560: 7820 3d20 706c 742e 7375 6270 6c6f 7473  x = plt.subplots
-00003570: 2829 0a20 2020 2020 2020 2069 6d20 3d20  ().        im = 
-00003580: 6178 2e69 6d73 686f 7728 7369 6d69 6c61  ax.imshow(simila
-00003590: 7269 7479 2c20 636d 6170 3d27 5264 596c  rity, cmap='RdYl
-000035a0: 4275 272c 2076 6d69 6e3d 2d31 2c20 766d  Bu', vmin=-1, vm
-000035b0: 6178 3d31 290a 2020 2020 2020 2020 6178  ax=1).        ax
-000035c0: 2e73 6574 5f78 7469 636b 7328 6e70 2e61  .set_xticks(np.a
-000035d0: 7261 6e67 6528 6e5f 6665 6174 7572 6573  range(n_features
-000035e0: 2a32 2929 0a20 2020 2020 2020 2061 782e  *2)).        ax.
-000035f0: 7365 745f 7974 6963 6b73 286e 702e 6172  set_yticks(np.ar
-00003600: 616e 6765 286e 5f66 6561 7475 7265 732a  ange(n_features*
-00003610: 3229 290a 2020 2020 2020 2020 7874 6963  2)).        xtic
-00003620: 6b6c 6162 656c 7320 3d20 5b66 2774 7331  klabels = [f'ts1
-00003630: 5f7b 6e66 6561 7475 7265 735f 696e 6465  _{nfeatures_inde
-00003640: 787d 2766 6f72 206e 6665 6174 7572 6573  x}'for nfeatures
-00003650: 5f69 6e64 6578 2069 6e20 7261 6e67 6528  _index in range(
-00003660: 312c 206e 5f66 6561 7475 7265 732b 3129  1, n_features+1)
-00003670: 5d0a 2020 2020 2020 2020 7874 6963 6b6c  ].        xtickl
-00003680: 6162 656c 7320 3d20 7874 6963 6b6c 6162  abels = xticklab
-00003690: 656c 7320 2b20 5b66 2774 7332 5f7b 6e66  els + [f'ts2_{nf
-000036a0: 6561 7475 7265 735f 696e 6465 787d 2766  eatures_index}'f
-000036b0: 6f72 206e 6665 6174 7572 6573 5f69 6e64  or nfeatures_ind
-000036c0: 6578 2069 6e20 7261 6e67 6528 312c 206e  ex in range(1, n
-000036d0: 5f66 6561 7475 7265 732b 3129 5d0a 2020  _features+1)].  
-000036e0: 2020 2020 2020 6178 2e73 6574 5f78 7469        ax.set_xti
-000036f0: 636b 6c61 6265 6c73 2878 7469 636b 6c61  cklabels(xtickla
-00003700: 6265 6c73 290a 2020 2020 2020 2020 6178  bels).        ax
-00003710: 2e73 6574 5f79 7469 636b 6c61 6265 6c73  .set_yticklabels
-00003720: 2878 7469 636b 6c61 6265 6c73 290a 2020  (xticklabels).  
-00003730: 2020 2020 2020 6178 2e73 6574 5f78 6c61        ax.set_xla
-00003740: 6265 6c28 2746 6561 7475 7265 2729 0a20  bel('Feature'). 
-00003750: 2020 2020 2020 2061 782e 7365 745f 796c         ax.set_yl
-00003760: 6162 656c 2827 4665 6174 7572 6527 290a  abel('Feature').
-00003770: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-00003780: 2072 616e 6765 286e 5f66 6561 7475 7265   range(n_feature
-00003790: 732a 3229 3a0a 2020 2020 2020 2020 2020  s*2):.          
-000037a0: 2020 666f 7220 6a20 696e 2072 616e 6765    for j in range
-000037b0: 286e 5f66 6561 7475 7265 732a 3229 3a0a  (n_features*2):.
-000037c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000037d0: 6178 2e74 6578 7428 6a2c 2069 2c20 6627  ax.text(j, i, f'
-000037e0: 7b73 696d 696c 6172 6974 795b 692c 206a  {similarity[i, j
-000037f0: 5d3a 2e32 667d 272c 2068 613d 2763 656e  ]:.2f}', ha='cen
-00003800: 7465 7227 2c20 7661 3d27 6365 6e74 6572  ter', va='center
-00003810: 272c 2063 6f6c 6f72 3d27 626c 6163 6b27  ', color='black'
-00003820: 290a 0a20 2020 2020 2020 2063 6261 7220  )..        cbar 
-00003830: 3d20 6178 2e66 6967 7572 652e 636f 6c6f  = ax.figure.colo
-00003840: 7262 6172 2869 6d2c 2061 783d 6178 290a  rbar(im, ax=ax).
-00003850: 2020 2020 2020 2020 6362 6172 2e61 782e          cbar.ax.
-00003860: 7365 745f 796c 6162 656c 2827 5369 6d69  set_ylabel('Simi
-00003870: 6c61 7269 7479 272c 2072 6f74 6174 696f  larity', rotatio
-00003880: 6e3d 2d39 302c 2076 613d 2762 6f74 746f  n=-90, va='botto
-00003890: 6d27 290a 2020 2020 2020 2020 706c 742e  m').        plt.
-000038a0: 7469 746c 6528 2773 696d 696c 6172 6974  title('similarit
-000038b0: 792d 636f 7272 656c 6174 696f 6e27 290a  y-correlation').
-000038c0: 2020 2020 2020 2020 706c 742e 7469 6768          plt.tigh
-000038d0: 745f 6c61 796f 7574 2829 0a20 2020 2020  t_layout().     
-000038e0: 2020 2072 6574 7572 6e20 5b28 6669 672c     return [(fig,
-000038f0: 2061 7829 5d0a 6060 600a 0a41 6674 6572   ax)].```..After
-00003900: 7761 7264 2c20 7468 6973 2070 6c6f 7420  ward, this plot 
-00003910: 6361 6e20 6265 2072 6567 6973 7465 7265  can be registere
-00003920: 6420 6279 2075 7369 6e67 2074 6865 2060  d by using the `
-00003930: 7265 6769 7374 6572 5f70 6c6f 7428 706c  register_plot(pl
-00003940: 6f74 5f63 6c61 7373 2960 206d 6574 686f  ot_class)` metho
-00003950: 6420 6672 6f6d 2060 506c 6f74 4661 6374  d from `PlotFact
-00003960: 6f72 7960 2061 7320 7368 6f77 6e20 696e  ory` as shown in
-00003970: 2074 6865 2066 6f6c 6c6f 7769 6e67 2063   the following c
-00003980: 6f64 6520 736e 6970 7065 7420 7468 6174  ode snippet that
-00003990: 2072 6567 6973 7465 7220 7468 6520 6e65   register the ne
-000039a0: 7720 6d65 7472 6963 2061 6e64 2074 6865  w metric and the
-000039b0: 206e 6577 2070 6c6f 743a 0a60 6060 5079   new plot:.```Py
-000039c0: 7468 6f6e 0a69 6d70 6f72 7420 6f73 0a69  thon.import os.i
-000039d0: 6d70 6f72 7420 6e75 6d70 7920 6173 206e  mport numpy as n
-000039e0: 700a 6672 6f6d 2073 696d 696c 6172 6974  p.from similarit
-000039f0: 795f 7473 2e70 6c6f 7473 2e70 6c6f 745f  y_ts.plots.plot_
-00003a00: 6661 6374 6f72 7920 696d 706f 7274 2050  factory import P
-00003a10: 6c6f 7446 6163 746f 7279 0a66 726f 6d20  lotFactory.from 
-00003a20: 7369 6d69 6c61 7269 7479 5f74 732e 7369  similarity_ts.si
-00003a30: 6d69 6c61 7269 7479 5f74 7320 696d 706f  milarity_ts impo
-00003a40: 7274 2053 696d 696c 6172 6974 7954 730a  rt SimilarityTs.
-00003a50: 6672 6f6d 2073 696d 696c 6172 6974 795f  from similarity_
-00003a60: 7473 2e6d 6574 7269 6373 2e6d 6574 7269  ts.metrics.metri
-00003a70: 635f 6661 6374 6f72 7920 696d 706f 7274  c_factory import
-00003a80: 204d 6574 7269 6346 6163 746f 7279 0a66   MetricFactory.f
-00003a90: 726f 6d20 6564 2069 6d70 6f72 7420 4575  rom ed import Eu
-00003aa0: 636c 6964 6561 6e44 6973 7461 6e63 650a  clideanDistance.
-00003ab0: 6672 6f6d 2063 635f 706c 6f74 2069 6d70  from cc_plot imp
-00003ac0: 6f72 7420 5369 6d69 6c61 7269 7479 506c  ort SimilarityPl
-00003ad0: 6f74 4279 436f 7272 656c 6174 696f 6e0a  otByCorrelation.
-00003ae0: 0a64 6566 206d 6169 6e28 293a 0a20 2020  .def main():.   
-00003af0: 204d 6574 7269 6346 6163 746f 7279 2e67   MetricFactory.g
-00003b00: 6574 5f69 6e73 7461 6e63 6528 292e 7265  et_instance().re
-00003b10: 6769 7374 6572 5f6d 6574 7269 6328 4575  gister_metric(Eu
-00003b20: 636c 6964 6561 6e44 6973 7461 6e63 6529  clideanDistance)
-00003b30: 0a20 2020 2050 6c6f 7446 6163 746f 7279  .    PlotFactory
-00003b40: 2e67 6574 5f69 6e73 7461 6e63 6528 292e  .get_instance().
-00003b50: 7265 6769 7374 6572 5f70 6c6f 7428 5369  register_plot(Si
-00003b60: 6d69 6c61 7269 7479 506c 6f74 4279 436f  milarityPlotByCo
-00003b70: 7272 656c 6174 696f 6e29 0a20 2020 2074  rrelation).    t
-00003b80: 7331 203d 206e 702e 7261 6e64 6f6d 2e72  s1 = np.random.r
-00003b90: 616e 6428 3230 302c 2032 290a 2020 2020  and(200, 2).    
-00003ba0: 7473 3273 203d 206e 702e 7261 6e64 6f6d  ts2s = np.random
-00003bb0: 2e72 616e 6428 352c 2031 3030 2c20 3229  .rand(5, 100, 2)
-00003bc0: 0a20 2020 2073 696d 696c 6172 6974 795f  .    similarity_
-00003bd0: 7473 203d 2053 696d 696c 6172 6974 7954  ts = SimilarityT
-00003be0: 7328 7473 312c 2074 7332 7329 0a20 2020  s(ts1, ts2s).   
-00003bf0: 2066 6f72 2074 7332 5f6e 616d 652c 206d   for ts2_name, m
-00003c00: 6574 7269 635f 6e61 6d65 2c20 636f 6d70  etric_name, comp
-00003c10: 7574 6564 5f6d 6574 7269 6320 696e 2073  uted_metric in s
-00003c20: 696d 696c 6172 6974 795f 7473 2e67 6574  imilarity_ts.get
-00003c30: 5f6d 6574 7269 635f 636f 6d70 7574 6572  _metric_computer
-00003c40: 2829 3a0a 2020 2020 2020 2020 7072 696e  ():.        prin
-00003c50: 7428 6627 7b74 7332 5f6e 616d 657d 2e20  t(f'{ts2_name}. 
-00003c60: 7b6d 6574 7269 635f 6e61 6d65 7d3a 207b  {metric_name}: {
-00003c70: 636f 6d70 7574 6564 5f6d 6574 7269 637d  computed_metric}
-00003c80: 2729 0a20 2020 2066 6f72 2074 7332 5f6e  ').    for ts2_n
-00003c90: 616d 652c 2070 6c6f 745f 6e61 6d65 2c20  ame, plot_name, 
-00003ca0: 6765 6e65 7261 7465 645f 706c 6f74 7320  generated_plots 
-00003cb0: 696e 2073 696d 696c 6172 6974 795f 7473  in similarity_ts
-00003cc0: 2e67 6574 5f70 6c6f 745f 636f 6d70 7574  .get_plot_comput
-00003cd0: 6572 2829 3a0a 2020 2020 2020 2020 5f5f  er():.        __
-00003ce0: 7361 7665 5f66 6967 7572 6573 2874 7332  save_figures(ts2
-00003cf0: 5f6e 616d 652c 2070 6c6f 745f 6e61 6d65  _name, plot_name
-00003d00: 2c20 6765 6e65 7261 7465 645f 706c 6f74  , generated_plot
-00003d10: 7329 0a0a 0a64 6566 205f 5f73 6176 655f  s)...def __save_
-00003d20: 6669 6775 7265 7328 6669 6c65 6e61 6d65  figures(filename
-00003d30: 2c20 706c 6f74 5f6e 616d 652c 2067 656e  , plot_name, gen
-00003d40: 6572 6174 6564 5f70 6c6f 7473 293a 0a20  erated_plots):. 
-00003d50: 2020 2066 6f72 2070 6c6f 7420 696e 2067     for plot in g
-00003d60: 656e 6572 6174 6564 5f70 6c6f 7473 3a0a  enerated_plots:.
-00003d70: 2020 2020 2020 2020 6469 725f 7061 7468          dir_path
-00003d80: 203d 205f 5f63 7265 6174 655f 6469 7265   = __create_dire
-00003d90: 6374 6f72 7928 6669 6c65 6e61 6d65 2c20  ctory(filename, 
-00003da0: 6627 6669 6775 7265 7327 2c20 706c 6f74  f'figures', plot
-00003db0: 5f6e 616d 6529 0a20 2020 2020 2020 2070  _name).        p
-00003dc0: 6c6f 745b 305d 2e73 6176 6566 6967 2866  lot[0].savefig(f
-00003dd0: 277b 6469 725f 7061 7468 7d7b 706c 6f74  '{dir_path}{plot
-00003de0: 5b30 5d2e 6178 6573 5b30 5d2e 6765 745f  [0].axes[0].get_
-00003df0: 7469 746c 6528 297d 2e70 6466 272c 2066  title()}.pdf', f
-00003e00: 6f72 6d61 743d 2770 6466 272c 2062 626f  ormat='pdf', bbo
-00003e10: 785f 696e 6368 6573 3d27 7469 6768 7427  x_inches='tight'
-00003e20: 290a 0a0a 6465 6620 5f5f 6372 6561 7465  )...def __create
-00003e30: 5f64 6972 6563 746f 7279 2866 696c 656e  _directory(filen
-00003e40: 616d 652c 2070 6174 682c 2070 6c6f 745f  ame, path, plot_
-00003e50: 6e61 6d65 293a 0a20 2020 2069 6620 706c  name):.    if pl
-00003e60: 6f74 5f6e 616d 6520 696e 2050 6c6f 7446  ot_name in PlotF
-00003e70: 6163 746f 7279 2e67 6574 5f69 6e73 7461  actory.get_insta
-00003e80: 6e63 6528 292e 6669 6775 7265 735f 7265  nce().figures_re
-00003e90: 7175 6972 6573 5f61 6c6c 5f73 616d 706c  quires_all_sampl
-00003ea0: 6573 3a0a 2020 2020 2020 2020 6469 725f  es:.        dir_
-00003eb0: 7061 7468 203d 2066 277b 7061 7468 7d2f  path = f'{path}/
-00003ec0: 7b70 6c6f 745f 6e61 6d65 7d2f 270a 2020  {plot_name}/'.  
-00003ed0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00003ee0: 6f72 6967 696e 616c 5f66 696c 656e 616d  original_filenam
-00003ef0: 6520 3d20 6f73 2e70 6174 682e 7370 6c69  e = os.path.spli
-00003f00: 7465 7874 2866 696c 656e 616d 6529 5b30  text(filename)[0
-00003f10: 5d0a 2020 2020 2020 2020 6469 725f 7061  ].        dir_pa
-00003f20: 7468 203d 2066 277b 7061 7468 7d2f 7b6f  th = f'{path}/{o
-00003f30: 7269 6769 6e61 6c5f 6669 6c65 6e61 6d65  riginal_filename
-00003f40: 7d2f 7b70 6c6f 745f 6e61 6d65 7d2f 270a  }/{plot_name}/'.
-00003f50: 2020 2020 6f73 2e6d 616b 6564 6972 7328      os.makedirs(
-00003f60: 6469 725f 7061 7468 2c20 6578 6973 745f  dir_path, exist_
-00003f70: 6f6b 3d54 7275 6529 0a20 2020 2072 6574  ok=True).    ret
-00003f80: 7572 6e20 6469 725f 7061 7468 0a0a 6966  urn dir_path..if
-00003f90: 205f 5f6e 616d 655f 5f20 3d3d 2027 5f5f   __name__ == '__
-00003fa0: 6d61 696e 5f5f 273a 0a20 2020 206d 6169  main__':.    mai
-00003fb0: 6e28 290a 6060 600a 0a23 2320 4c69 6365  n().```..## Lice
-00003fc0: 6e73 650a 0a53 696d 696c 6172 6974 7954  nse..SimilarityT
-00003fd0: 5320 746f 6f6c 6b69 7420 6973 2066 7265  S toolkit is fre
-00003fe0: 6520 616e 6420 6f70 656e 2d73 6f75 7263  e and open-sourc
-00003ff0: 6520 736f 6674 7761 7265 206c 6963 656e  e software licen
-00004000: 7365 6420 756e 6465 7220 7468 6520 5b4d  sed under the [M
-00004010: 4954 206c 6963 656e 7365 5d28 4c49 4345  IT license](LICE
-00004020: 4e53 4529 2e0a                           NSE)..
+00000020: 696f 2f62 6164 6765 2f70 7970 692d 312e  io/badge/pypi-1.
+00000030: 302e 332d 626c 7565 295d 2868 7474 7073  0.3-blue)](https
+00000040: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
+00000050: 6563 742f 7369 6d69 6c61 7269 7479 2d74  ect/similarity-t
+00000060: 732f 290a 5b21 5b50 7974 686f 6e20 332e  s/).[![Python 3.
+00000070: 395d 2868 7474 7073 3a2f 2f69 6d67 2e73  9](https://img.s
+00000080: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
+00000090: 7079 7468 6f6e 2d33 2e39 2d64 6172 6b67  python-3.9-darkg
+000000a0: 7265 656e 295d 2868 7474 7073 3a2f 2f77  reen)](https://w
+000000b0: 7777 2e70 7974 686f 6e2e 6f72 672f 646f  ww.python.org/do
+000000c0: 776e 6c6f 6164 732f 7265 6c65 6173 652f  wnloads/release/
+000000d0: 7079 7468 6f6e 2d33 3930 2f29 0a5b 215b  python-390/).[![
+000000e0: 6c61 7374 2d75 7064 6174 655d 2868 7474  last-update](htt
+000000f0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000100: 2e69 6f2f 6261 6467 652f 6c61 7374 5f75  .io/badge/last_u
+00000110: 7064 6174 652d 3037 2f31 382f 3230 3233  pdate-07/18/2023
+00000120: 2d62 7269 6768 7467 7265 656e 295d 2868  -brightgreen)](h
+00000130: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000140: 6d2f 616c 656a 616e 6472 6f66 6465 7a2d  m/alejandrofdez-
+00000150: 7573 2f73 696d 696c 6172 6974 792d 7473  us/similarity-ts
+00000160: 2d63 6c69 2f63 6f6d 6d69 7473 2f6d 6169  -cli/commits/mai
+00000170: 6e29 0a5b 215b 6c69 6365 6e73 655d 2868  n).[![license](h
+00000180: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000190: 6473 2e69 6f2f 6261 6467 652f 6c69 6365  ds.io/badge/lice
+000001a0: 6e73 652d 4d49 542d 6f72 616e 6765 295d  nse-MIT-orange)]
+000001b0: 284c 4943 454e 5345 290a 0a23 2053 696d  (LICENSE)..# Sim
+000001c0: 696c 6172 6974 7954 533a 2054 6f6f 6c6b  ilarityTS: Toolk
+000001d0: 6974 2066 6f72 2074 6865 2045 7661 6c75  it for the Evalu
+000001e0: 6174 696f 6e20 6f66 2053 696d 696c 6172  ation of Similar
+000001f0: 6974 7920 666f 7220 6d75 6c74 6976 6172  ity for multivar
+00000200: 6961 7465 2074 696d 6520 7365 7269 6573  iate time series
+00000210: 0a0a 2323 2054 6162 6c65 206f 6620 436f  ..## Table of Co
+00000220: 6e74 656e 7473 0a0a 2d20 5b50 6163 6b61  ntents..- [Packa
+00000230: 6765 2044 6573 6372 6970 7469 6f6e 5d28  ge Description](
+00000240: 2370 6163 6b61 6765 2d64 6573 6372 6970  #package-descrip
+00000250: 7469 6f6e 290a 2d20 5b49 6e73 7461 6c6c  tion).- [Install
+00000260: 6174 696f 6e5d 2823 696e 7374 616c 6c61  ation](#installa
+00000270: 7469 6f6e 290a 2d20 5b55 7361 6765 5d28  tion).- [Usage](
+00000280: 2375 7361 6765 290a 2d20 5b43 6f6e 6669  #usage).- [Confi
+00000290: 6775 7269 6e67 2074 6865 2074 6f6f 6c6b  guring the toolk
+000002a0: 6974 5d28 2363 6f6e 6669 6775 7269 6e67  it](#configuring
+000002b0: 2d74 6865 2d74 6f6f 6c6b 6974 290a 2d20  -the-toolkit).- 
+000002c0: 5b45 7874 656e 6469 6e67 2074 6865 2074  [Extending the t
+000002d0: 6f6f 6c6b 6974 5d28 2365 7874 656e 6469  oolkit](#extendi
+000002e0: 6e67 2d74 6865 2d74 6f6f 6c6b 6974 290a  ng-the-toolkit).
+000002f0: 2d20 5b4c 6963 656e 7365 5d28 236c 6963  - [License](#lic
+00000300: 656e 7365 290a 2d20 5b41 636b 6e6f 776c  ense).- [Acknowl
+00000310: 6564 6765 6d65 6e74 735d 2823 6163 6b6e  edgements](#ackn
+00000320: 6f77 6c65 6467 656d 656e 7473 290a 0a23  owledgements)..#
+00000330: 2320 5061 636b 6167 6520 4465 7363 7269  # Package Descri
+00000340: 7074 696f 6e0a 0a53 696d 696c 6172 6974  ption..Similarit
+00000350: 7954 5320 6973 2061 6e20 6f70 656e 2d73  yTS is an open-s
+00000360: 6f75 7263 6520 7061 636b 6167 6520 6465  ource package de
+00000370: 7369 676e 6564 2074 6f20 6661 6369 6c69  signed to facili
+00000380: 7461 7465 2074 6865 2065 7661 6c75 6174  tate the evaluat
+00000390: 696f 6e20 616e 6420 636f 6d70 6172 6973  ion and comparis
+000003a0: 6f6e 206f 660a 6d75 6c74 6976 6172 6961  on of.multivaria
+000003b0: 7465 2074 696d 6520 7365 7269 6573 2064  te time series d
+000003c0: 6174 612e 2049 7420 7072 6f76 6964 6573  ata. It provides
+000003d0: 2061 2063 6f6d 7072 6568 656e 7369 7665   a comprehensive
+000003e0: 2074 6f6f 6c6b 6974 2066 6f72 2061 6e61   toolkit for ana
+000003f0: 6c79 7a69 6e67 2c20 7669 7375 616c 697a  lyzing, visualiz
+00000400: 696e 672c 2061 6e64 2072 6570 6f72 7469  ing, and reporti
+00000410: 6e67 206d 756c 7469 706c 650a 6d65 7472  ng multiple.metr
+00000420: 6963 7320 616e 6420 6669 6775 7265 7320  ics and figures 
+00000430: 6465 7269 7665 6420 6672 6f6d 2074 696d  derived from tim
+00000440: 6520 7365 7269 6573 2064 6174 6173 6574  e series dataset
+00000450: 732e 2054 6865 2074 6f6f 6c6b 6974 2073  s. The toolkit s
+00000460: 696d 706c 6966 6965 7320 7468 6520 7072  implifies the pr
+00000470: 6f63 6573 7320 6f66 2065 7661 6c75 6174  ocess of evaluat
+00000480: 696e 6720 7468 6520 7369 6d69 6c61 7269  ing the similari
+00000490: 7479 206f 660a 7469 6d65 2073 6572 6965  ty of.time serie
+000004a0: 7320 6279 206f 6666 6572 696e 6720 6461  s by offering da
+000004b0: 7461 2070 7265 7072 6f63 6573 7369 6e67  ta preprocessing
+000004c0: 2c20 6d65 7472 6963 7320 636f 6d70 7574  , metrics comput
+000004d0: 6174 696f 6e2c 2076 6973 7561 6c69 7a61  ation, visualiza
+000004e0: 7469 6f6e 2c20 7374 6174 6973 7469 6361  tion, statistica
+000004f0: 6c20 616e 616c 7973 6973 2c20 616e 6420  l analysis, and 
+00000500: 7265 706f 7274 2067 656e 6572 6174 696f  report generatio
+00000510: 6e0a 6675 6e63 7469 6f6e 616c 6974 6965  n.functionalitie
+00000520: 732e 2057 6974 6820 6974 7320 6375 7374  s. With its cust
+00000530: 6f6d 697a 6162 6c65 2066 6561 7475 7265  omizable feature
+00000540: 732c 2053 696d 696c 6172 6974 7954 5320  s, SimilarityTS 
+00000550: 656d 706f 7765 7273 2072 6573 6561 7263  empowers researc
+00000560: 6865 7273 2061 6e64 2064 6174 610a 7363  hers and data.sc
+00000570: 6965 6e74 6973 7473 2074 6f20 6761 696e  ientists to gain
+00000580: 2069 6e73 6967 6874 732c 2069 6465 6e74   insights, ident
+00000590: 6966 7920 7061 7474 6572 6e73 2c20 616e  ify patterns, an
+000005a0: 6420 6d61 6b65 2069 6e66 6f72 6d65 6420  d make informed 
+000005b0: 6465 6369 7369 6f6e 7320 6261 7365 6420  decisions based 
+000005c0: 6f6e 2074 6865 6972 2074 696d 6520 7365  on their time se
+000005d0: 7269 6573 2064 6174 612e 0a0a 4120 636f  ries data...A co
+000005e0: 6d6d 616e 6420 6c69 6e65 2069 6e74 6572  mmand line inter
+000005f0: 6661 6365 2074 6f6f 6c20 6973 2061 6c73  face tool is als
+00000600: 6f20 6176 6169 6c61 626c 6520 6174 3a20  o available at: 
+00000610: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000620: 6f6d 2f61 6c65 6a61 6e64 726f 6664 657a  om/alejandrofdez
+00000630: 2d75 732f 7369 6d69 6c61 7269 7479 2d74  -us/similarity-t
+00000640: 732d 636c 692e 0a0a 2323 2320 4176 6169  s-cli...### Avai
+00000650: 6c61 626c 6520 6d65 7472 6963 730a 0a54  lable metrics..T
+00000660: 6869 7320 746f 6f6c 6b69 7420 6361 6e20  his toolkit can 
+00000670: 636f 6d70 7574 6520 7468 6520 666f 6c6c  compute the foll
+00000680: 6f77 696e 6720 6d65 7472 6963 733a 0a0a  owing metrics:..
+00000690: 2d20 606b 6c60 3a20 4b75 6c6c 6261 636b  - `kl`: Kullback
+000006a0: 2d4c 6569 626c 6572 2064 6976 6572 6765  -Leibler diverge
+000006b0: 6e63 650a 2d20 606a 7360 3a20 4a65 6e73  nce.- `js`: Jens
+000006c0: 656e 2d53 6861 6e6e 6f6e 2064 6976 6572  en-Shannon diver
+000006d0: 6765 6e63 650a 2d20 606b 7360 3a20 4b6f  gence.- `ks`: Ko
+000006e0: 6c6d 6f67 6f72 6f76 2d53 6d69 726e 6f76  lmogorov-Smirnov
+000006f0: 2074 6573 740a 2d20 606d 6d64 603a 204d   test.- `mmd`: M
+00000700: 6178 696d 756d 204d 6561 6e20 4469 7363  aximum Mean Disc
+00000710: 7265 7061 6e63 790a 2d20 6064 7477 6020  repancy.- `dtw` 
+00000720: 4479 6e61 6d69 6320 5469 6d65 2057 6172  Dynamic Time War
+00000730: 7069 6e67 0a2d 2060 6363 603a 2044 6966  ping.- `cc`: Dif
+00000740: 6665 7265 6e63 6520 6f66 2063 6f2d 7661  ference of co-va
+00000750: 7269 616e 6365 730a 2d20 6063 7060 3a20  riances.- `cp`: 
+00000760: 4469 6666 6572 656e 6365 206f 6620 636f  Difference of co
+00000770: 7272 656c 6174 696f 6e73 0a2d 2060 6869  rrelations.- `hi
+00000780: 603a 2044 6966 6665 7265 6e63 6520 6f66  `: Difference of
+00000790: 2068 6973 746f 6772 616d 730a 0a23 2323   histograms..###
+000007a0: 2041 7661 696c 6162 6c65 2066 6967 7572   Available figur
+000007b0: 6573 0a0a 5468 6973 2074 6f6f 6c6b 6974  es..This toolkit
+000007c0: 2063 616e 2067 656e 6572 6174 6520 7468   can generate th
+000007d0: 6520 666f 6c6c 6f77 696e 6720 6669 6775  e following figu
+000007e0: 7265 733a 0a0a 2d20 6032 6460 3a20 7468  res:..- `2d`: th
+000007f0: 6520 6f72 6469 6e61 7279 2067 7261 7068  e ordinary graph
+00000800: 6963 616c 2072 6570 7265 7365 6e74 6174  ical representat
+00000810: 696f 6e20 6f66 2074 6865 2074 696d 6520  ion of the time 
+00000820: 7365 7269 6573 2069 6e20 6120 3244 2066  series in a 2D f
+00000830: 6967 7572 6520 7769 7468 2074 6865 2074  igure with the t
+00000840: 696d 6520 7265 7072 6573 656e 7465 6420  ime represented 
+00000850: 6f6e 2074 6865 2078 2061 7869 730a 2020  on the x axis.  
+00000860: 616e 6420 7468 6520 6461 7461 2076 616c  and the data val
+00000870: 7565 7320 6f6e 2074 6865 2079 2d61 7869  ues on the y-axi
+00000880: 7320 666f 720a 2020 2020 2d20 7468 6520  s for.    - the 
+00000890: 636f 6d70 6c65 7465 206d 756c 7469 7661  complete multiva
+000008a0: 7269 6174 6520 7469 6d65 2073 6572 6965  riate time serie
+000008b0: 733b 2061 6e64 0a20 2020 202d 2061 2070  s; and.    - a p
+000008c0: 6c6f 7420 7065 7220 636f 6c75 6d6e 2e0a  lot per column..
+000008d0: 0a20 2045 6163 6820 6765 6e65 7261 7465  .  Each generate
+000008e0: 6420 6669 6775 7265 2070 6c6f 7473 2062  d figure plots b
+000008f0: 6f74 6820 7468 6520 6074 7331 6020 616e  oth the `ts1` an
+00000900: 6420 7468 6520 6074 7332 6020 6461 7461  d the `ts2` data
+00000910: 2074 6f20 6561 7369 6c79 206f 6274 6169   to easily obtai
+00000920: 6e20 6b65 7920 696e 7369 6768 7473 2069  n key insights i
+00000930: 6e74 6f0a 2020 7468 6520 7369 6d69 6c61  nto.  the simila
+00000940: 7269 7469 6573 206f 7220 6469 6666 6572  rities or differ
+00000950: 656e 6365 7320 6265 7477 6565 6e20 7468  ences between th
+00000960: 656d 2e0a 2020 2020 3c64 6976 3e0a 2020  em..    <div>.  
+00000970: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
+00000980: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f61  s://github.com/a
+00000990: 6c65 6a61 6e64 726f 6664 657a 2d75 732f  lejandrofdez-us/
+000009a0: 7369 6d69 6c61 7269 7479 2d74 732f 626c  similarity-ts/bl
+000009b0: 6f62 2f65 3562 3134 3762 3134 3539 3730  ob/e5b147b145970
+000009c0: 6633 6139 3333 3531 6131 3030 3430 3232  f3a93351a1004022
+000009d0: 6662 3330 6432 3066 3566 302f 646f 6373  fb30d20f5f0/docs
+000009e0: 2f66 6967 7572 6573 2f32 645f 7361 6d70  /figures/2d_samp
+000009f0: 6c65 5f33 5f63 6f6d 706c 6574 655f 5453  le_3_complete_TS
+00000a00: 5f31 5f76 735f 5453 5f32 2e70 6e67 3f72  _1_vs_TS_2.png?r
+00000a10: 6177 3d74 7275 6522 2061 6c74 3d22 3244  aw=true" alt="2D
+00000a20: 2046 6967 7572 6520 636f 6d70 6c65 7465   Figure complete
+00000a30: 223e 0a20 2020 203c 696d 6720 7372 633d  ">.    <img src=
+00000a40: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00000a50: 636f 6d2f 616c 656a 616e 6472 6f66 6465  com/alejandrofde
+00000a60: 7a2d 7573 2f73 696d 696c 6172 6974 792d  z-us/similarity-
+00000a70: 7473 2f62 6c6f 622f 6535 6231 3437 6231  ts/blob/e5b147b1
+00000a80: 3435 3937 3066 3361 3933 3335 3161 3130  45970f3a93351a10
+00000a90: 3034 3032 3266 6233 3064 3230 6635 6630  04022fb30d20f5f0
+00000aa0: 2f64 6f63 732f 6669 6775 7265 732f 3264  /docs/figures/2d
+00000ab0: 5f73 616d 706c 655f 335f 6370 755f 7574  _sample_3_cpu_ut
+00000ac0: 696c 5f70 6572 6365 6e74 5f54 535f 315f  il_percent_TS_1_
+00000ad0: 7673 5f54 535f 322e 706e 673f 7261 773d  vs_TS_2.png?raw=
+00000ae0: 7472 7565 2220 616c 743d 2232 4420 4669  true" alt="2D Fi
+00000af0: 6775 7265 2066 6f72 2075 7365 6420 4350  gure for used CP
+00000b00: 5520 7065 7263 656e 7461 6765 223e 0a20  U percentage">. 
+00000b10: 2020 203c 2f64 6976 3e0a 2d20 6064 656c     </div>.- `del
+00000b20: 7461 603a 2074 6865 2064 6966 6665 7265  ta`: the differe
+00000b30: 6e63 6573 2062 6574 7765 656e 2074 6865  nces between the
+00000b40: 2076 616c 7565 7320 6f66 2065 6163 6820   values of each 
+00000b50: 636f 6c75 6d6e 2067 726f 7570 6564 2062  column grouped b
+00000b60: 7920 7065 7269 6f64 7320 6f66 2074 696d  y periods of tim
+00000b70: 652e 2046 6f72 2069 6e73 7461 6e63 652c  e. For instance,
+00000b80: 2074 6865 2064 6966 6665 7265 6e63 6573   the differences
+00000b90: 0a20 2062 6574 7765 656e 2074 6865 2070  .  between the p
+00000ba0: 6572 6365 6e74 6167 6520 6f66 2063 7075  ercentage of cpu
+00000bb0: 2075 7365 6420 6576 6572 7920 3130 2c20   used every 10, 
+00000bc0: 3235 206f 7220 3530 206d 696e 7574 6573  25 or 50 minutes
+00000bd0: 2e20 5468 6573 6520 6465 6c74 6120 6361  . These delta ca
+00000be0: 6e20 6265 2075 7365 6420 6173 2061 206d  n be used as a m
+00000bf0: 6561 6e73 206f 6620 636f 6d70 6172 6973  eans of comparis
+00000c00: 6f6e 2062 6574 7765 656e 0a20 2074 696d  on between.  tim
+00000c10: 6520 7365 7269 6573 2073 686f 7274 2d2f  e series short-/
+00000c20: 6d69 642d 2f6c 6f6e 672d 7465 726d 2070  mid-/long-term p
+00000c30: 6174 7465 726e 732e 0a20 2020 203c 6469  atterns..    <di
+00000c40: 763e 0a20 2020 203c 696d 6720 7372 633d  v>.    <img src=
+00000c50: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00000c60: 636f 6d2f 616c 656a 616e 6472 6f66 6465  com/alejandrofde
+00000c70: 7a2d 7573 2f73 696d 696c 6172 6974 792d  z-us/similarity-
+00000c80: 7473 2f62 6c6f 622f 6535 6231 3437 6231  ts/blob/e5b147b1
+00000c90: 3435 3937 3066 3361 3933 3335 3161 3130  45970f3a93351a10
+00000ca0: 3034 3032 3266 6233 3064 3230 6635 6630  04022fb30d20f5f0
+00000cb0: 2f64 6f63 732f 6669 6775 7265 732f 6465  /docs/figures/de
+00000cc0: 6c74 615f 7361 6d70 6c65 5f33 5f63 7075  lta_sample_3_cpu
+00000cd0: 5f75 7469 6c5f 7065 7263 656e 745f 5453  _util_percent_TS
+00000ce0: 5f31 5f76 735f 5453 5f32 5f28 6772 6f75  _1_vs_TS_2_(grou
+00000cf0: 7065 645f 6279 5f31 305f 6d69 6e75 7465  ped_by_10_minute
+00000d00: 7329 2e70 6e67 3f72 6177 3d74 7275 6522  s).png?raw=true"
+00000d10: 2061 6c74 3d22 4465 6c74 6120 4669 6775   alt="Delta Figu
+00000d20: 7265 2066 6f72 2075 7365 6420 4350 5520  re for used CPU 
+00000d30: 7065 7263 656e 7461 6765 2067 726f 7570  percentage group
+00000d40: 6564 2062 7920 3130 206d 696e 7574 6573  ed by 10 minutes
+00000d50: 223e 0a20 2020 203c 696d 6720 7372 633d  ">.    <img src=
+00000d60: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00000d70: 636f 6d2f 616c 656a 616e 6472 6f66 6465  com/alejandrofde
+00000d80: 7a2d 7573 2f73 696d 696c 6172 6974 792d  z-us/similarity-
+00000d90: 7473 2f62 6c6f 622f 6535 6231 3437 6231  ts/blob/e5b147b1
+00000da0: 3435 3937 3066 3361 3933 3335 3161 3130  45970f3a93351a10
+00000db0: 3034 3032 3266 6233 3064 3230 6635 6630  04022fb30d20f5f0
+00000dc0: 2f64 6f63 732f 6669 6775 7265 732f 6465  /docs/figures/de
+00000dd0: 6c74 615f 7361 6d70 6c65 5f33 5f63 7075  lta_sample_3_cpu
+00000de0: 5f75 7469 6c5f 7065 7263 656e 745f 5453  _util_percent_TS
+00000df0: 5f31 5f76 735f 5453 5f32 5f28 6772 6f75  _1_vs_TS_2_(grou
+00000e00: 7065 645f 6279 5f32 355f 6d69 6e75 7465  ped_by_25_minute
+00000e10: 7329 2e70 6e67 3f72 6177 3d74 7275 6522  s).png?raw=true"
+00000e20: 2061 6c74 3d22 4465 6c74 6120 4669 6775   alt="Delta Figu
+00000e30: 7265 2066 6f72 2075 7365 6420 4350 5520  re for used CPU 
+00000e40: 7065 7263 656e 7461 6765 2067 726f 7570  percentage group
+00000e50: 6564 2062 7920 3235 206d 696e 7574 6573  ed by 25 minutes
+00000e60: 223e 0a20 2020 203c 696d 6720 7372 633d  ">.    <img src=
+00000e70: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00000e80: 636f 6d2f 616c 656a 616e 6472 6f66 6465  com/alejandrofde
+00000e90: 7a2d 7573 2f73 696d 696c 6172 6974 792d  z-us/similarity-
+00000ea0: 7473 2f62 6c6f 622f 6535 6231 3437 6231  ts/blob/e5b147b1
+00000eb0: 3435 3937 3066 3361 3933 3335 3161 3130  45970f3a93351a10
+00000ec0: 3034 3032 3266 6233 3064 3230 6635 6630  04022fb30d20f5f0
+00000ed0: 2f64 6f63 732f 6669 6775 7265 732f 6465  /docs/figures/de
+00000ee0: 6c74 615f 7361 6d70 6c65 5f33 5f63 7075  lta_sample_3_cpu
+00000ef0: 5f75 7469 6c5f 7065 7263 656e 745f 5453  _util_percent_TS
+00000f00: 5f31 5f76 735f 5453 5f32 5f28 6772 6f75  _1_vs_TS_2_(grou
+00000f10: 7065 645f 6279 5f35 305f 6d69 6e75 7465  ped_by_50_minute
+00000f20: 7329 2e70 6e67 3f72 6177 3d74 7275 6522  s).png?raw=true"
+00000f30: 2061 6c74 3d22 4465 6c74 6120 4669 6775   alt="Delta Figu
+00000f40: 7265 2066 6f72 2075 7365 6420 4350 5520  re for used CPU 
+00000f50: 7065 7263 656e 7461 6765 2067 726f 7570  percentage group
+00000f60: 6564 2062 7920 3530 206d 696e 7574 6573  ed by 50 minutes
+00000f70: 223e 0a20 2020 203c 2f64 6976 3e0a 0a2d  ">.    </div>..-
+00000f80: 2060 7063 6160 3a20 7468 6520 6c69 6e65   `pca`: the line
+00000f90: 6172 2064 696d 656e 7369 6f6e 616c 6974  ar dimensionalit
+00000fa0: 7920 7265 6475 6374 696f 6e20 7465 6368  y reduction tech
+00000fb0: 6e69 7175 6520 7468 6174 2061 696d 7320  nique that aims 
+00000fc0: 746f 2066 696e 6420 7468 6520 7072 696e  to find the prin
+00000fd0: 6369 7061 6c20 636f 6d70 6f6e 656e 7473  cipal components
+00000fe0: 206f 6620 6120 6461 7461 2073 6574 2062   of a data set b
+00000ff0: 790a 2020 636f 6d70 7574 696e 6720 7468  y.  computing th
+00001000: 6520 6c69 6e65 6172 2063 6f6d 6269 6e61  e linear combina
+00001010: 7469 6f6e 7320 6f66 2074 6865 206f 7269  tions of the ori
+00001020: 6769 6e61 6c20 6368 6172 6163 7465 7269  ginal characteri
+00001030: 7374 6963 7320 7468 6174 2065 7870 6c61  stics that expla
+00001040: 696e 2074 6865 206d 6f73 7420 7661 7269  in the most vari
+00001050: 616e 6365 2069 6e20 7468 6520 6461 7461  ance in the data
+00001060: 2e0a 2020 2020 3c64 6976 2061 6c69 676e  ..    <div align
+00001070: 3d22 6365 6e74 6572 223e 0a20 2020 203c  ="center">.    <
+00001080: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+00001090: 2f67 6974 6875 622e 636f 6d2f 616c 656a  /github.com/alej
+000010a0: 616e 6472 6f66 6465 7a2d 7573 2f73 696d  androfdez-us/sim
+000010b0: 696c 6172 6974 792d 7473 2f62 6c6f 622f  ilarity-ts/blob/
+000010c0: 6535 6231 3437 6231 3435 3937 3066 3361  e5b147b145970f3a
+000010d0: 3933 3335 3161 3130 3034 3032 3266 6233  93351a1004022fb3
+000010e0: 3064 3230 6635 6630 2f64 6f63 732f 6669  0d20f5f0/docs/fi
+000010f0: 6775 7265 732f 5043 412e 706e 673f 7261  gures/PCA.png?ra
+00001100: 773d 7472 7565 2220 616c 743d 2250 4341  w=true" alt="PCA
+00001110: 2046 6967 7572 6522 2077 6964 7468 3d22   Figure" width="
+00001120: 3435 3022 3e0a 2020 2020 3c2f 6469 763e  450">.    </div>
+00001130: 0a2d 2060 7473 6e65 603a 2061 2074 6f6f  .- `tsne`: a too
+00001140: 6c20 666f 7220 7669 7375 616c 6973 696e  l for visualisin
+00001150: 6720 6869 6768 2d64 696d 656e 7369 6f6e  g high-dimension
+00001160: 616c 2064 6174 6120 7365 7473 2069 6e20  al data sets in 
+00001170: 6120 3244 206f 7220 3344 2067 7261 7068  a 2D or 3D graph
+00001180: 6963 616c 2072 6570 7265 7365 6e74 6174  ical representat
+00001190: 696f 6e20 616c 6c6f 7769 6e67 2074 6865  ion allowing the
+000011a0: 2063 7265 6174 696f 6e0a 2020 6f66 2061   creation.  of a
+000011b0: 2073 696e 676c 6520 6d61 7020 7468 6174   single map that
+000011c0: 2072 6576 6561 6c73 2074 6865 2073 7472   reveals the str
+000011d0: 7563 7475 7265 206f 6620 7468 6520 6461  ucture of the da
+000011e0: 7461 2061 7420 6d61 6e79 2064 6966 6665  ta at many diffe
+000011f0: 7265 6e74 2073 6361 6c65 732e 0a20 2020  rent scales..   
+00001200: 203c 6469 7620 616c 6967 6e3d 2263 656e   <div align="cen
+00001210: 7465 7222 3e0a 2020 2020 3c69 6d67 2073  ter">.    <img s
+00001220: 7263 3d22 6874 7470 733a 2f2f 6769 7468  rc="https://gith
+00001230: 7562 2e63 6f6d 2f61 6c65 6a61 6e64 726f  ub.com/alejandro
+00001240: 6664 657a 2d75 732f 7369 6d69 6c61 7269  fdez-us/similari
+00001250: 7479 2d74 732f 626c 6f62 2f65 3562 3134  ty-ts/blob/e5b14
+00001260: 3762 3134 3539 3730 6633 6139 3333 3531  7b145970f3a93351
+00001270: 6131 3030 3430 3232 6662 3330 6432 3066  a1004022fb30d20f
+00001280: 3566 302f 646f 6373 2f66 6967 7572 6573  5f0/docs/figures
+00001290: 2f74 2d53 4e45 2d69 7465 725f 3330 302d  /t-SNE-iter_300-
+000012a0: 7065 7270 6c65 7869 7479 5f35 2e70 6e67  perplexity_5.png
+000012b0: 3f72 6177 3d74 7275 6522 2061 6c74 3d22  ?raw=true" alt="
+000012c0: 5453 4e45 2046 6967 7572 6520 3330 3020  TSNE Figure 300 
+000012d0: 6974 6572 6174 696f 6e73 2035 2070 6572  iterations 5 per
+000012e0: 706c 6578 6974 7922 2077 6964 7468 3d22  plexity" width="
+000012f0: 3435 3022 3e0a 2020 2020 3c69 6d67 2073  450">.    <img s
+00001300: 7263 3d22 6874 7470 733a 2f2f 6769 7468  rc="https://gith
+00001310: 7562 2e63 6f6d 2f61 6c65 6a61 6e64 726f  ub.com/alejandro
+00001320: 6664 657a 2d75 732f 7369 6d69 6c61 7269  fdez-us/similari
+00001330: 7479 2d74 732f 626c 6f62 2f65 3562 3134  ty-ts/blob/e5b14
+00001340: 3762 3134 3539 3730 6633 6139 3333 3531  7b145970f3a93351
+00001350: 6131 3030 3430 3232 6662 3330 6432 3066  a1004022fb30d20f
+00001360: 3566 302f 646f 6373 2f66 6967 7572 6573  5f0/docs/figures
+00001370: 2f74 2d53 4e45 2d69 7465 725f 3130 3030  /t-SNE-iter_1000
+00001380: 2d70 6572 706c 6578 6974 795f 352e 706e  -perplexity_5.pn
+00001390: 673f 7261 773d 7472 7565 2220 616c 743d  g?raw=true" alt=
+000013a0: 2254 534e 4520 4669 6775 7265 2031 3030  "TSNE Figure 100
+000013b0: 3020 6974 6572 6174 696f 6e73 2035 2070  0 iterations 5 p
+000013c0: 6572 706c 6578 6974 7922 2077 6964 7468  erplexity" width
+000013d0: 3d22 3435 3022 3e0a 2020 2020 3c2f 6469  ="450">.    </di
+000013e0: 763e 0a2d 2060 6474 7760 2070 6174 683a  v>.- `dtw` path:
+000013f0: 2049 6e20 6164 6469 7469 6f6e 2074 6f20   In addition to 
+00001400: 7468 6520 6e75 6d65 7269 6361 6c20 7369  the numerical si
+00001410: 6d69 6c61 7269 7479 206d 6561 7375 7265  milarity measure
+00001420: 2c20 7468 6520 6772 6170 6869 6361 6c20  , the graphical 
+00001430: 7265 7072 6573 656e 7461 7469 6f6e 206f  representation o
+00001440: 6620 7468 6520 4454 5720 7061 7468 206f  f the DTW path o
+00001450: 6620 6561 6368 0a20 2063 6f6c 756d 6e20  f each.  column 
+00001460: 6361 6e20 6265 2075 7365 6675 6c20 746f  can be useful to
+00001470: 2062 6574 7465 7220 616e 616c 7973 6520   better analyse 
+00001480: 7468 6520 7369 6d69 6c61 7269 7469 6573  the similarities
+00001490: 206f 7220 6469 6666 6572 656e 6365 7320   or differences 
+000014a0: 6265 7477 6565 6e20 7468 6520 7469 6d65  between the time
+000014b0: 2073 6572 6965 7320 636f 6c75 6d6e 732e   series columns.
+000014c0: 204e 6f74 6963 6520 7468 6174 0a20 2074   Notice that.  t
+000014d0: 6865 7265 2069 7320 6e6f 206d 756c 7469  here is no multi
+000014e0: 7661 7269 6174 6520 7265 7072 6573 656e  variate represen
+000014f0: 7461 7469 6f6e 206f 6620 4454 5720 7061  tation of DTW pa
+00001500: 7468 732c 206f 6e6c 7920 7369 6e67 6c65  ths, only single
+00001510: 2063 6f6c 756d 6e20 7265 7072 6573 656e   column represen
+00001520: 7461 7469 6f6e 732e 0a20 2020 203c 6469  tations..    <di
+00001530: 763e 0a20 2020 203c 696d 6720 7372 633d  v>.    <img src=
+00001540: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00001550: 636f 6d2f 616c 656a 616e 6472 6f66 6465  com/alejandrofde
+00001560: 7a2d 7573 2f73 696d 696c 6172 6974 792d  z-us/similarity-
+00001570: 7473 2f62 6c6f 622f 6535 6231 3437 6231  ts/blob/e5b147b1
+00001580: 3435 3937 3066 3361 3933 3335 3161 3130  45970f3a93351a10
+00001590: 3034 3032 3266 6233 3064 3230 6635 6630  04022fb30d20f5f0
+000015a0: 2f64 6f63 732f 6669 6775 7265 732f 4454  /docs/figures/DT
+000015b0: 575f 7361 6d70 6c65 5f33 5f63 7075 5f75  W_sample_3_cpu_u
+000015c0: 7469 6c5f 7065 7263 656e 742e 706e 673f  til_percent.png?
+000015d0: 7261 773d 7472 7565 2220 616c 743d 2244  raw=true" alt="D
+000015e0: 5457 2046 6967 7572 6520 666f 7220 6370  TW Figure for cp
+000015f0: 7522 3e0a 2020 2020 3c2f 6469 763e 0a0a  u">.    </div>..
+00001600: 2323 2049 6e73 7461 6c6c 6174 696f 6e0a  ## Installation.
+00001610: 0a49 6e73 7461 6c6c 2074 6865 2070 6163  .Install the pac
+00001620: 6b61 6765 2075 7369 6e67 2070 6970 2069  kage using pip i
+00001630: 6e20 796f 7572 206c 6f63 616c 2065 6e76  n your local env
+00001640: 6972 6f6e 6d65 6e74 3a0a 0a60 6060 4261  ironment:..```Ba
+00001650: 7368 0a70 6970 2069 6e73 7461 6c6c 2073  sh.pip install s
+00001660: 696d 696c 6172 6974 792d 7473 0a60 6060  imilarity-ts.```
+00001670: 0a0a 2323 2055 7361 6765 0a0a 5573 6572  ..## Usage..User
+00001680: 7320 6d75 7374 2063 7265 6174 6520 6120  s must create a 
+00001690: 6e65 7720 6053 696d 696c 6172 6974 7954  new `SimilarityT
+000016a0: 7360 206f 626a 6563 7420 6279 2063 616c  s` object by cal
+000016b0: 6c69 6e67 2069 7473 2063 6f6e 7374 7275  ling its constru
+000016c0: 6374 6f72 2061 6e64 2070 6173 7369 6e67  ctor and passing
+000016d0: 2074 6865 2066 6f6c 6c6f 7769 6e67 2070   the following p
+000016e0: 6172 616d 6574 6572 732e 0a0a 2d20 6074  arameters...- `t
+000016f0: 7331 6020 5468 6973 2074 696d 6520 7365  s1` This time se
+00001700: 7269 6573 206d 6179 2072 6570 7265 7365  ries may represe
+00001710: 6e74 2074 6865 2062 6173 656c 696e 6520  nt the baseline 
+00001720: 6f72 2067 726f 756e 6420 7472 7574 6820  or ground truth 
+00001730: 7469 6d65 0a20 2073 6572 6965 7320 6173  time.  series as
+00001740: 2061 2060 6e75 6d70 7960 2061 7272 6179   a `numpy` array
+00001750: 2077 6974 6820 7368 6170 6520 605b 6c65   with shape `[le
+00001760: 6e67 7468 2c20 6e75 6d5f 6665 6174 7572  ngth, num_featur
+00001770: 6573 5d60 2e0a 2d20 6074 7332 7360 2041  es]`..- `ts2s` A
+00001780: 2073 696e 676c 6520 6f72 2061 2073 6574   single or a set
+00001790: 206f 6620 7469 6d65 2073 6572 6965 7320   of time series 
+000017a0: 6173 2061 2060 6e75 6d70 7960 2061 7272  as a `numpy` arr
+000017b0: 6179 2077 6974 6820 7368 6170 6520 605b  ay with shape `[
+000017c0: 6e75 6d5f 7469 6d65 5f73 6572 6965 732c  num_time_series,
+000017d0: 206c 656e 6774 682c 206e 756d 5f66 6561   length, num_fea
+000017e0: 7475 7265 735d 602e 0a0a 0a43 6f6e 7374  tures]`....Const
+000017f0: 7261 696e 7473 3a0a 0a2d 2060 7473 3160  raints:..- `ts1`
+00001800: 2074 696d 652d 7365 7269 6573 2061 6e64   time-series and
+00001810: 2060 7473 3273 6020 7469 6d65 2d73 6572   `ts2s` time-ser
+00001820: 6965 7320 6669 6c65 2873 2920 6d75 7374  ies file(s) must
+00001830: 3a0a 2020 2020 2d20 6861 7665 2074 6865  :.    - have the
+00001840: 2073 616d 6520 6469 6d65 6e73 696f 6e61   same dimensiona
+00001850: 6c69 7479 2028 6e75 6d62 6572 206f 6620  lity (number of 
+00001860: 636f 6c75 6d6e 7329 0a20 2020 202d 206e  columns).    - n
+00001870: 6f74 2069 6e63 6c75 6465 2061 2074 696d  ot include a tim
+00001880: 6573 7461 6d70 2063 6f6c 756d 6e0a 2020  estamp column.  
+00001890: 2020 2d20 696e 636c 7564 6520 6f6e 6c79    - include only
+000018a0: 206e 756d 6572 6963 2076 616c 7565 730a   numeric values.
+000018b0: 2d20 616c 6c20 6074 7332 7360 2074 696d  - all `ts2s` tim
+000018c0: 652d 7365 7269 6573 206d 7573 7420 6861  e-series must ha
+000018d0: 7665 2074 6865 2073 616d 6520 6c65 6e67  ve the same leng
+000018e0: 7468 2028 6e75 6d62 6572 206f 6620 726f  th (number of ro
+000018f0: 7773 292e 0a0a 4966 2060 7473 3160 2074  ws)...If `ts1` t
+00001900: 696d 652d 7365 7269 6573 2069 7320 6c6f  ime-series is lo
+00001910: 6e67 6572 2028 6d6f 7265 2072 6f77 7329  nger (more rows)
+00001920: 2074 6861 6e20 6074 7332 7360 2074 696d   than `ts2s` tim
+00001930: 652d 7365 7269 6573 2c20 7468 6520 6074  e-series, the `t
+00001940: 7331 6020 7469 6d65 2073 6572 6965 7320  s1` time series 
+00001950: 7769 6c6c 2062 650a 6469 7669 6465 6420  will be.divided 
+00001960: 696e 2077 696e 646f 7773 206f 6620 7468  in windows of th
+00001970: 6520 7361 6d65 206c 656e 6774 6820 6173  e same length as
+00001980: 2074 6865 2060 7473 3273 6020 7469 6d65   the `ts2s` time
+00001990: 2d73 6572 6965 732e 0a0a 466f 7220 6561  -series...For ea
+000019a0: 6368 2060 7473 3273 6020 7469 6d65 2d73  ch `ts2s` time-s
+000019b0: 6572 6965 732c 2074 6865 206d 6f73 7420  eries, the most 
+000019c0: 7369 6d69 6c61 7220 7769 6e64 6f77 2028  similar window (
+000019d0: 2a29 2066 726f 6d20 6074 7331 6020 7469  *) from `ts1` ti
+000019e0: 6d65 2073 6572 6965 7320 6973 2073 656c  me series is sel
+000019f0: 6563 7465 642e 0a0a 4669 6e61 6c6c 792c  ected...Finally,
+00001a00: 206d 6574 7269 6373 2061 6e64 2066 6967   metrics and fig
+00001a10: 7572 6573 2074 6861 7420 6173 7365 7373  ures that assess
+00001a20: 2074 6865 2073 696d 696c 6172 6974 7920   the similarity 
+00001a30: 6265 7477 6565 6e20 6561 6368 2070 6169  between each pai
+00001a40: 7220 6f66 2060 7473 3273 6020 7469 6d65  r of `ts2s` time
+00001a50: 2d73 6572 6965 7320 616e 6420 6974 730a  -series and its.
+00001a60: 6173 736f 6369 6174 6564 206d 6f73 7420  associated most 
+00001a70: 7369 6d69 6c61 7220 6074 7331 6020 7769  similar `ts1` wi
+00001a80: 6e64 6f77 2061 7265 2063 6f6d 7075 7465  ndow are compute
+00001a90: 642e 0a0a 282a 2920 5468 6520 6d65 7472  d...(*) The metr
+00001aa0: 6963 2075 7365 6420 666f 7220 7468 6520  ic used for the 
+00001ab0: 7365 6c65 6374 696f 6e20 6f66 2074 6865  selection of the
+00001ac0: 206d 6f73 740a 7369 6d69 6c61 7220 6074   most.similar `t
+00001ad0: 7331 6020 7469 6d65 2d73 6572 6965 7320  s1` time-series 
+00001ae0: 7769 6e64 6f77 2070 6572 2065 6163 6820  window per each 
+00001af0: 6074 7332 7360 2074 696d 652d 7365 7269  `ts2s` time-seri
+00001b00: 6573 2066 696c 6520 6973 2073 656c 6563  es file is selec
+00001b10: 7461 626c 652e 2060 6474 7760 2069 7320  table. `dtw` is 
+00001b20: 7468 6520 6465 6661 756c 7420 7365 6c65  the default sele
+00001b30: 6374 6564 206d 6574 7269 632c 2068 6f77  cted metric, how
+00001b40: 6576 6572 2c20 616e 7920 6f66 0a74 6865  ever, any of.the
+00001b50: 0a5b 6d65 7472 6963 735d 2823 6176 6169  .[metrics](#avai
+00001b60: 6c61 626c 652d 6d65 7472 6963 7329 2061  lable-metrics) a
+00001b70: 7265 2061 6c73 6f20 6176 6169 6c61 626c  re also availabl
+00001b80: 6520 666f 7220 7468 6973 2070 7572 706f  e for this purpo
+00001b90: 7365 2e20 5365 6520 7468 6520 5b74 6f6f  se. See the [too
+00001ba0: 6c6b 6974 2063 6f6e 6669 6775 7261 7469  lkit configurati
+00001bb0: 6f6e 2073 6563 7469 6f6e 5d28 2363 6f6e  on section](#con
+00001bc0: 6669 6775 7269 6e67 2d74 6865 2d74 6f6f  figuring-the-too
+00001bd0: 6c6b 6974 292e 0a0a 2323 2320 4d69 6e69  lkit)...### Mini
+00001be0: 6d61 6c20 7573 6167 6520 6578 616d 706c  mal usage exampl
+00001bf0: 6573 3a0a 5573 6167 6520 6578 616d 706c  es:.Usage exampl
+00001c00: 6573 2063 616e 2062 6520 666f 756e 6420  es can be found 
+00001c10: 6174 3a20 6874 7470 733a 2f2f 6769 7468  at: https://gith
+00001c20: 7562 2e63 6f6d 2f61 6c65 6a61 6e64 726f  ub.com/alejandro
+00001c30: 6664 657a 2d75 732f 7369 6d69 6c61 7269  fdez-us/similari
+00001c40: 7479 2d74 732f 7472 6565 2f6d 6169 6e2f  ty-ts/tree/main/
+00001c50: 7573 6167 655f 6578 616d 706c 6573 2e0a  usage_examples..
+00001c60: 0a31 2e20 436f 6d70 7574 6520 6d65 7472  .1. Compute metr
+00001c70: 6963 7320 6265 7477 6565 6e20 7261 6e64  ics between rand
+00001c80: 6f6d 2074 696d 6520 7365 7269 6573 2028  om time series (
+00001c90: 6074 7331 603a 206f 6e65 2074 696d 6520  `ts1`: one time 
+00001ca0: 7365 7269 6573 206f 6620 6c65 6e67 6874  series of lenght
+00001cb0: 2032 3030 2061 6e64 2032 2064 696d 656e   200 and 2 dimen
+00001cc0: 7369 6f6e 7320 616e 6420 6074 7332 603a  sions and `ts2`:
+00001cd0: 2066 6976 6520 7469 6d65 2073 6572 6965   five time serie
+00001ce0: 7320 6f66 206c 656e 6774 6820 3130 3020  s of length 100 
+00001cf0: 616e 6420 3220 6469 6d65 6e73 696f 6e73  and 2 dimensions
+00001d00: 293a 0a20 2020 2060 6060 5079 7468 6f6e  ):.    ```Python
+00001d10: 0a20 2020 2069 6d70 6f72 7420 6e75 6d70  .    import nump
+00001d20: 7920 6173 206e 700a 2020 2020 6672 6f6d  y as np.    from
+00001d30: 2073 696d 696c 6172 6974 795f 7473 2e73   similarity_ts.s
+00001d40: 696d 696c 6172 6974 795f 7473 2069 6d70  imilarity_ts imp
+00001d50: 6f72 7420 5369 6d69 6c61 7269 7479 5473  ort SimilarityTs
+00001d60: 0a20 2020 200a 2020 2020 7473 3120 3d20  .    .    ts1 = 
+00001d70: 6e70 2e72 616e 646f 6d2e 7261 6e64 2832  np.random.rand(2
+00001d80: 3030 2c20 3229 0a20 2020 2074 7332 7320  00, 2).    ts2s 
+00001d90: 3d20 6e70 2e72 616e 646f 6d2e 7261 6e64  = np.random.rand
+00001da0: 2835 2c20 3130 302c 2032 290a 2020 2020  (5, 100, 2).    
+00001db0: 7369 6d69 6c61 7269 7479 5f74 7320 3d20  similarity_ts = 
+00001dc0: 5369 6d69 6c61 7269 7479 5473 2874 7331  SimilarityTs(ts1
+00001dd0: 2c20 7473 3273 290a 2020 2020 666f 7220  , ts2s).    for 
+00001de0: 7473 325f 6e61 6d65 2c20 6d65 7472 6963  ts2_name, metric
+00001df0: 5f6e 616d 652c 2063 6f6d 7075 7465 645f  _name, computed_
+00001e00: 6d65 7472 6963 2069 6e20 7369 6d69 6c61  metric in simila
+00001e10: 7269 7479 5f74 732e 6765 745f 6d65 7472  rity_ts.get_metr
+00001e20: 6963 5f63 6f6d 7075 7465 7228 293a 0a20  ic_computer():. 
+00001e30: 2020 2020 2020 2070 7269 6e74 2866 277b         print(f'{
+00001e40: 7473 325f 6e61 6d65 7d2e 207b 6d65 7472  ts2_name}. {metr
+00001e50: 6963 5f6e 616d 657d 3a20 7b63 6f6d 7075  ic_name}: {compu
+00001e60: 7465 645f 6d65 7472 6963 7d27 290a 2020  ted_metric}').  
+00001e70: 2020 6060 600a 0a31 2e20 436f 6d70 7574    ```..1. Comput
+00001e80: 6520 6d65 7472 6963 7320 616e 6420 6669  e metrics and fi
+00001e90: 6775 7265 7320 6265 7477 6565 6e20 7261  gures between ra
+00001ea0: 6e64 6f6d 2074 696d 6520 7365 7269 6573  ndom time series
+00001eb0: 2061 6e64 2073 6176 6520 6669 6775 7265   and save figure
+00001ec0: 733a 0a20 2020 2060 6060 5079 7468 6f6e  s:.    ```Python
+00001ed0: 0a20 2020 2069 6d70 6f72 7420 6f73 0a20  .    import os. 
+00001ee0: 2020 2069 6d70 6f72 7420 6e75 6d70 7920     import numpy 
+00001ef0: 6173 206e 700a 2020 2020 6672 6f6d 2073  as np.    from s
+00001f00: 696d 696c 6172 6974 795f 7473 2e70 6c6f  imilarity_ts.plo
+00001f10: 7473 2e70 6c6f 745f 6661 6374 6f72 7920  ts.plot_factory 
+00001f20: 696d 706f 7274 2050 6c6f 7446 6163 746f  import PlotFacto
+00001f30: 7279 0a20 2020 2066 726f 6d20 7369 6d69  ry.    from simi
+00001f40: 6c61 7269 7479 5f74 732e 7369 6d69 6c61  larity_ts.simila
+00001f50: 7269 7479 5f74 7320 696d 706f 7274 2053  rity_ts import S
+00001f60: 696d 696c 6172 6974 7954 730a 2020 2020  imilarityTs.    
+00001f70: 0a20 2020 2064 6566 206d 6169 6e28 293a  .    def main():
+00001f80: 0a20 2020 2020 2020 2074 7331 203d 206e  .        ts1 = n
+00001f90: 702e 7261 6e64 6f6d 2e72 616e 6428 3230  p.random.rand(20
+00001fa0: 302c 2032 290a 2020 2020 2020 2020 7473  0, 2).        ts
+00001fb0: 3273 203d 206e 702e 7261 6e64 6f6d 2e72  2s = np.random.r
+00001fc0: 616e 6428 352c 2031 3030 2c20 3229 0a20  and(5, 100, 2). 
+00001fd0: 2020 2020 2020 2073 696d 696c 6172 6974         similarit
+00001fe0: 795f 7473 203d 2053 696d 696c 6172 6974  y_ts = Similarit
+00001ff0: 7954 7328 7473 312c 2074 7332 7329 0a20  yTs(ts1, ts2s). 
+00002000: 2020 2020 2020 2066 6f72 2074 7332 5f6e         for ts2_n
+00002010: 616d 652c 206d 6574 7269 635f 6e61 6d65  ame, metric_name
+00002020: 2c20 636f 6d70 7574 6564 5f6d 6574 7269  , computed_metri
+00002030: 6320 696e 2073 696d 696c 6172 6974 795f  c in similarity_
+00002040: 7473 2e67 6574 5f6d 6574 7269 635f 636f  ts.get_metric_co
+00002050: 6d70 7574 6572 2829 3a0a 2020 2020 2020  mputer():.      
+00002060: 2020 2020 2020 7072 696e 7428 6627 7b74        print(f'{t
+00002070: 7332 5f6e 616d 657d 2e20 7b6d 6574 7269  s2_name}. {metri
+00002080: 635f 6e61 6d65 7d3a 207b 636f 6d70 7574  c_name}: {comput
+00002090: 6564 5f6d 6574 7269 637d 2729 0a20 2020  ed_metric}').   
+000020a0: 2020 2020 2066 6f72 2074 7332 5f6e 616d       for ts2_nam
+000020b0: 652c 2070 6c6f 745f 6e61 6d65 2c20 6765  e, plot_name, ge
+000020c0: 6e65 7261 7465 645f 706c 6f74 7320 696e  nerated_plots in
+000020d0: 2073 696d 696c 6172 6974 795f 7473 2e67   similarity_ts.g
+000020e0: 6574 5f70 6c6f 745f 636f 6d70 7574 6572  et_plot_computer
+000020f0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00002100: 5f5f 7361 7665 5f66 6967 7572 6573 2874  __save_figures(t
+00002110: 7332 5f6e 616d 652c 2070 6c6f 745f 6e61  s2_name, plot_na
+00002120: 6d65 2c20 6765 6e65 7261 7465 645f 706c  me, generated_pl
+00002130: 6f74 7329 0a20 2020 200a 2020 2020 0a20  ots).    .    . 
+00002140: 2020 2064 6566 205f 5f73 6176 655f 6669     def __save_fi
+00002150: 6775 7265 7328 6669 6c65 6e61 6d65 2c20  gures(filename, 
+00002160: 706c 6f74 5f6e 616d 652c 2067 656e 6572  plot_name, gener
+00002170: 6174 6564 5f70 6c6f 7473 293a 0a20 2020  ated_plots):.   
+00002180: 2020 2020 2066 6f72 2070 6c6f 7420 696e       for plot in
+00002190: 2067 656e 6572 6174 6564 5f70 6c6f 7473   generated_plots
+000021a0: 3a0a 2020 2020 2020 2020 2020 2020 6469  :.            di
+000021b0: 725f 7061 7468 203d 205f 5f63 7265 6174  r_path = __creat
+000021c0: 655f 6469 7265 6374 6f72 7928 6669 6c65  e_directory(file
+000021d0: 6e61 6d65 2c20 6627 6669 6775 7265 7327  name, f'figures'
+000021e0: 2c20 706c 6f74 5f6e 616d 6529 0a20 2020  , plot_name).   
+000021f0: 2020 2020 2020 2020 2070 6c6f 745b 305d           plot[0]
+00002200: 2e73 6176 6566 6967 2866 277b 6469 725f  .savefig(f'{dir_
+00002210: 7061 7468 7d7b 706c 6f74 5b30 5d2e 6178  path}{plot[0].ax
+00002220: 6573 5b30 5d2e 6765 745f 7469 746c 6528  es[0].get_title(
+00002230: 297d 2e70 6466 272c 2066 6f72 6d61 743d  )}.pdf', format=
+00002240: 2770 6466 272c 2062 626f 785f 696e 6368  'pdf', bbox_inch
+00002250: 6573 3d27 7469 6768 7427 290a 2020 2020  es='tight').    
+00002260: 0a20 2020 200a 2020 2020 6465 6620 5f5f  .    .    def __
+00002270: 6372 6561 7465 5f64 6972 6563 746f 7279  create_directory
+00002280: 2866 696c 656e 616d 652c 2070 6174 682c  (filename, path,
+00002290: 2070 6c6f 745f 6e61 6d65 293a 0a20 2020   plot_name):.   
+000022a0: 2020 2020 2069 6620 706c 6f74 5f6e 616d       if plot_nam
+000022b0: 6520 696e 2050 6c6f 7446 6163 746f 7279  e in PlotFactory
+000022c0: 2e67 6574 5f69 6e73 7461 6e63 6528 292e  .get_instance().
+000022d0: 6669 6775 7265 735f 7265 7175 6972 6573  figures_requires
+000022e0: 5f61 6c6c 5f73 616d 706c 6573 3a0a 2020  _all_samples:.  
+000022f0: 2020 2020 2020 2020 2020 6469 725f 7061            dir_pa
+00002300: 7468 203d 2066 277b 7061 7468 7d2f 7b70  th = f'{path}/{p
+00002310: 6c6f 745f 6e61 6d65 7d2f 270a 2020 2020  lot_name}/'.    
+00002320: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00002330: 2020 2020 2020 6f72 6967 696e 616c 5f66        original_f
+00002340: 696c 656e 616d 6520 3d20 6f73 2e70 6174  ilename = os.pat
+00002350: 682e 7370 6c69 7465 7874 2866 696c 656e  h.splitext(filen
+00002360: 616d 6529 5b30 5d0a 2020 2020 2020 2020  ame)[0].        
+00002370: 2020 2020 6469 725f 7061 7468 203d 2066      dir_path = f
+00002380: 277b 7061 7468 7d2f 7b6f 7269 6769 6e61  '{path}/{origina
+00002390: 6c5f 6669 6c65 6e61 6d65 7d2f 7b70 6c6f  l_filename}/{plo
+000023a0: 745f 6e61 6d65 7d2f 270a 2020 2020 2020  t_name}/'.      
+000023b0: 2020 6f73 2e6d 616b 6564 6972 7328 6469    os.makedirs(di
+000023c0: 725f 7061 7468 2c20 6578 6973 745f 6f6b  r_path, exist_ok
+000023d0: 3d54 7275 6529 0a20 2020 2020 2020 2072  =True).        r
+000023e0: 6574 7572 6e20 6469 725f 7061 7468 0a20  eturn dir_path. 
+000023f0: 2020 200a 2020 2020 6966 205f 5f6e 616d     .    if __nam
+00002400: 655f 5f20 3d3d 2027 5f5f 6d61 696e 5f5f  e__ == '__main__
+00002410: 273a 0a20 2020 2020 2020 206d 6169 6e28  ':.        main(
+00002420: 290a 2020 2020 6060 600a 0a23 2320 436f  ).    ```..## Co
+00002430: 6e66 6967 7572 696e 6720 7468 6520 546f  nfiguring the To
+00002440: 6f6c 6b69 740a 5573 6572 7320 6361 6e20  olkit.Users can 
+00002450: 7072 6f76 6964 6520 6d65 7472 6963 7320  provide metrics 
+00002460: 6f72 2066 6967 7572 6573 2074 6f20 6265  or figures to be
+00002470: 2063 6f6d 7075 7465 642f 6765 6e65 7261   computed/genera
+00002480: 7465 6420 616e 6420 736f 6d65 206f 7468  ted and some oth
+00002490: 6572 2070 6172 616d 6574 6572 6973 6174  er parameterisat
+000024a0: 696f 6e2e 2054 6865 2066 6f6c 6c6f 7769  ion. The followi
+000024b0: 6e67 2063 6f64 6520 736e 6970 7065 7420  ng code snippet 
+000024c0: 0a63 7265 6174 6573 2061 2063 6f6e 6669  .creates a confi
+000024d0: 6775 7261 7469 6f6e 206f 626a 6563 7420  guration object 
+000024e0: 7468 6174 2073 686f 756c 6420 6265 2070  that should be p
+000024f0: 6173 7365 6420 746f 2074 6865 2060 5369  assed to the `Si
+00002500: 6d69 6c61 7269 7479 5473 6020 636f 6e73  milarityTs` cons
+00002510: 7472 7563 746f 723a 0a60 6060 5079 7468  tructor:.```Pyth
+00002520: 6f6e 0a64 6566 205f 5f63 7265 6174 655f  on.def __create_
+00002530: 7369 6d69 6c61 7269 7479 5f74 735f 636f  similarity_ts_co
+00002540: 6e66 6967 2829 3a0a 2020 2020 2320 5468  nfig():.    # Th
+00002550: 6520 6c69 7374 206f 6620 6d65 7472 6963  e list of metric
+00002560: 7320 6e61 6d65 7320 7468 6174 2077 696c  s names that wil
+00002570: 6c20 6265 2063 6f6d 7075 7465 640a 2020  l be computed.  
+00002580: 2020 6d65 7472 6963 5f63 6f6e 6669 6720    metric_config 
+00002590: 3d20 4d65 7472 6963 436f 6e66 6967 285b  = MetricConfig([
+000025a0: 276a 7327 2c20 276d 6d64 275d 2920 0a20  'js', 'mmd']) . 
+000025b0: 2020 2023 2054 6865 206c 6973 7420 6f66     # The list of
+000025c0: 2066 6967 7572 6520 6e61 6d65 7320 7468   figure names th
+000025d0: 6174 2077 696c 6c20 6265 2067 656e 6572  at will be gener
+000025e0: 6174 6564 2061 6e64 2074 6865 2074 696d  ated and the tim
+000025f0: 6520 7374 6570 2069 6e20 7365 636f 6e64  e step in second
+00002600: 7320 6f66 2074 6865 2074 696d 6520 7365  s of the time se
+00002610: 7269 6573 2e0a 2020 2020 706c 6f74 5f63  ries..    plot_c
+00002620: 6f6e 6669 6720 3d20 506c 6f74 436f 6e66  onfig = PlotConf
+00002630: 6967 285b 2764 656c 7461 272c 2027 7063  ig(['delta', 'pc
+00002640: 6127 5d2c 2074 696d 6573 7461 6d70 5f66  a'], timestamp_f
+00002650: 7265 7175 656e 6379 5f73 6563 6f6e 6473  requency_seconds
+00002660: 3d33 3030 290a 0a20 2020 2023 204e 616d  =300)..    # Nam
+00002670: 6520 6f66 2065 6163 6820 7469 6d65 2073  e of each time s
+00002680: 6572 6965 7320 6f66 2074 6865 2074 7332  eries of the ts2
+00002690: 7320 7365 7420 6f66 2074 696d 6520 7365  s set of time se
+000026a0: 7269 6573 0a20 2020 2074 7332 5f6e 616d  ries.    ts2_nam
+000026b0: 6573 203d 205b 2774 7332 5f31 5f6e 616d  es = ['ts2_1_nam
+000026c0: 6527 2c20 2774 7332 5f32 5f6e 616d 6527  e', 'ts2_2_name'
+000026d0: 2c20 2774 7332 5f33 5f6e 616d 6527 2c20  , 'ts2_3_name', 
+000026e0: 2774 7332 5f34 5f6e 616d 6527 2c20 2774  'ts2_4_name', 't
+000026f0: 7332 5f35 5f6e 616d 6527 5d0a 2020 2020  s2_5_name'].    
+00002700: 2320 4e61 6d65 206f 6620 7468 6520 6665  # Name of the fe
+00002710: 6174 7572 6573 0a20 2020 2068 6561 6465  atures.    heade
+00002720: 725f 6e61 6d65 7320 3d20 5b27 6665 6174  r_names = ['feat
+00002730: 7572 6531 5f6e 616d 6527 2c20 2766 6561  ure1_name', 'fea
+00002740: 7475 7265 325f 6e61 6d65 275d 0a20 2020  ture2_name'].   
+00002750: 200a 2020 2020 2320 4372 6561 7469 6f6e   .    # Creation
+00002760: 206f 6620 7468 6520 636f 6e66 6967 7572   of the configur
+00002770: 6174 696f 6e0a 2020 2020 2020 2320 7374  ation.      # st
+00002780: 7269 6465 2066 6f72 2063 7574 7469 6e67  ride for cutting
+00002790: 2074 6865 2074 7331 2077 6865 6e20 6e65   the ts1 when ne
+000027a0: 6564 6564 0a20 2020 2020 2023 206d 6574  eded.      # met
+000027b0: 7269 6320 7573 6564 2066 6f72 2073 656c  ric used for sel
+000027c0: 6563 7469 6e67 2074 6865 206d 6f73 7420  ecting the most 
+000027d0: 7369 6d69 6c61 7220 7769 6e64 6f77 0a20  similar window. 
+000027e0: 2020 2073 696d 696c 6172 6974 795f 7473     similarity_ts
+000027f0: 5f63 6f6e 6669 6720 3d20 5369 6d69 6c61  _config = Simila
+00002800: 7269 7479 5473 436f 6e66 6967 286d 6574  rityTsConfig(met
+00002810: 7269 635f 636f 6e66 6967 2c20 706c 6f74  ric_config, plot
+00002820: 5f63 6f6e 6669 672c 0a20 2020 2020 2020  _config,.       
+00002830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002850: 2020 2020 2020 2073 7472 6964 653d 3130         stride=10
+00002860: 2c20 7769 6e64 6f77 5f73 656c 6563 7469  , window_selecti
+00002870: 6f6e 5f6d 6574 7269 633d 276b 6c27 2c0a  on_metric='kl',.
+00002880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028a0: 2020 2020 2020 2020 2020 2020 2020 7473                ts
+000028b0: 325f 6e61 6d65 733d 7473 325f 6e61 6d65  2_names=ts2_name
+000028c0: 732c 2068 6561 6465 725f 6e61 6d65 733d  s, header_names=
+000028d0: 6865 6164 6572 5f6e 616d 6573 290a 2020  header_names).  
+000028e0: 2020 7265 7475 726e 2073 696d 696c 6172    return similar
+000028f0: 6974 795f 7473 5f63 6f6e 6669 670a 6060  ity_ts_config.``
+00002900: 600a 0a49 6620 6e6f 206d 6574 7269 6373  `..If no metrics
+00002910: 206e 6f72 2066 6967 7572 6573 2061 7265   nor figures are
+00002920: 2070 726f 7669 6465 642c 2074 6865 2074   provided, the t
+00002930: 6f6f 6c20 7769 6c6c 2063 6f6d 7075 7465  ool will compute
+00002940: 2061 6c6c 2074 6865 2061 7661 696c 6162   all the availab
+00002950: 6c65 206d 6574 7269 6373 2061 6e64 2066  le metrics and f
+00002960: 6967 7572 6573 2e0a 0a54 6865 2066 6f6c  igures...The fol
+00002970: 6c6f 7769 6e67 2061 7267 756d 656e 7473  lowing arguments
+00002980: 2061 7265 2061 6c73 6f20 6176 6169 6c61   are also availa
+00002990: 626c 6520 666f 7220 6669 6e65 2d74 756e  ble for fine-tun
+000029a0: 696e 673a 0a0a 2d20 6074 696d 6573 7461  ing:..- `timesta
+000029b0: 6d70 5f66 7265 7175 656e 6379 5f73 6563  mp_frequency_sec
+000029c0: 6f6e 6473 603a 2074 6865 2066 7265 7175  onds`: the frequ
+000029d0: 656e 6379 2069 6e20 7365 636f 6e64 7320  ency in seconds 
+000029e0: 696e 2077 6869 6368 2073 616d 706c 6573  in which samples
+000029f0: 2077 6572 6520 7461 6b65 6e2e 2054 6869   were taken. Thi
+00002a00: 7320 6973 206e 6565 6465 6420 746f 2067  s is needed to g
+00002a10: 656e 6572 6174 6520 7468 6520 6465 6c74  enerate the delt
+00002a20: 6120 6669 6775 7265 7320 7769 7468 2063  a figures with c
+00002a30: 6f72 7265 6374 2074 696d 6520 6d61 676e  orrect time magn
+00002a40: 6974 7564 6573 2e20 4279 2064 6566 6175  itudes. By defau
+00002a50: 6c74 2069 730a 2020 6031 6020 7365 636f  lt is.  `1` seco
+00002a60: 6e64 2e0a 2d20 6073 7472 6964 6560 3a20  nd..- `stride`: 
+00002a70: 7768 656e 2060 7473 3160 2074 696d 652d  when `ts1` time-
+00002a80: 7365 7269 6573 2069 7320 6c6f 6e67 6572  series is longer
+00002a90: 2074 6861 6e20 6074 7332 7360 2074 696d   than `ts2s` tim
+00002aa0: 652d 7365 7269 6573 2074 6865 2077 696e  e-series the win
+00002ab0: 646f 7773 2061 7265 2063 6f6d 7075 7465  dows are compute
+00002ac0: 6420 6279 2075 7369 6e67 2061 0a20 2073  d by using a.  s
+00002ad0: 7472 6964 6520 6f66 2060 3160 2062 7920  tride of `1` by 
+00002ae0: 6465 6661 756c 742e 2053 6f6d 6574 696d  default. Sometim
+00002af0: 6573 2075 7369 6e67 2061 206c 6172 6765  es using a large
+00002b00: 7220 7661 6c75 6520 666f 7220 7468 6520  r value for the 
+00002b10: 7374 7269 6465 2070 6172 616d 6574 6572  stride parameter
+00002b20: 2069 6d70 726f 7665 7320 7468 6520 7065   improves the pe
+00002b30: 7266 6f72 6d61 6e63 6520 6279 2073 6b69  rformance by ski
+00002b40: 7070 696e 670a 2020 7468 6520 636f 6d70  pping.  the comp
+00002b50: 7574 6174 696f 6e20 6f66 2073 696d 696c  utation of simil
+00002b60: 6172 6974 7920 6265 7477 6565 6e20 736f  arity between so
+00002b70: 206d 616e 7920 7769 6e64 6f77 732e 0a2d   many windows..-
+00002b80: 2060 7769 6e64 6f77 5f73 656c 6563 7469   `window_selecti
+00002b90: 6f6e 5f6d 6574 7269 6360 3a20 7468 6520  on_metric`: the 
+00002ba0: 6d65 7472 6963 2075 7365 6420 666f 7220  metric used for 
+00002bb0: 7468 6520 7365 6c65 6374 696f 6e20 6f66  the selection of
+00002bc0: 2074 6865 206d 6f73 7420 7369 6d69 6c61   the most simila
+00002bd0: 7220 6074 7331 6020 7469 6d65 2d73 6572  r `ts1` time-ser
+00002be0: 6965 7320 7769 6e64 6f77 2070 6572 2065  ies window per e
+00002bf0: 6163 6820 6074 7332 7360 2074 696d 652d  ach `ts2s` time-
+00002c00: 7365 7269 6573 2066 696c 6520 6973 2073  series file is s
+00002c10: 656c 6563 7461 626c 652e 6064 7477 6020  electable.`dtw` 
+00002c20: 6973 2074 6865 2064 6566 6175 6c74 2073  is the default s
+00002c30: 656c 6563 7465 6420 6d65 7472 6963 2c20  elected metric, 
+00002c40: 686f 7765 7665 722c 2061 6e79 206f 6620  however, any of 
+00002c50: 7468 6520 5b6d 6574 7269 6373 5d28 2361  the [metrics](#a
+00002c60: 7661 696c 6162 6c65 2d6d 6574 7269 6373  vailable-metrics
+00002c70: 2920 6172 6520 616c 736f 2061 7661 696c  ) are also avail
+00002c80: 6162 6c65 2066 6f72 2074 6869 7320 7075  able for this pu
+00002c90: 7270 6f73 652e 2053 6565 2074 6865 205b  rpose. See the [
+00002ca0: 746f 6f6c 6b69 7420 636f 6e66 6967 7572  toolkit configur
+00002cb0: 6174 696f 6e20 7365 6374 696f 6e5d 2823  ation section](#
+00002cc0: 636f 6e66 6967 7572 696e 672d 7468 652d  configuring-the-
+00002cd0: 746f 6f6c 6b69 7429 2e0a 2d20 6074 7332  toolkit)..- `ts2
+00002ce0: 5f6e 616d 6573 603a 206e 616d 6520 6f66  _names`: name of
+00002cf0: 2065 6163 6820 7469 6d65 2073 6572 6965   each time serie
+00002d00: 7320 6f66 2074 6865 2060 7473 3273 6020  s of the `ts2s` 
+00002d10: 7365 7420 6f66 2074 696d 6520 7365 7269  set of time seri
+00002d20: 6573 2e0a 2d20 6068 6561 6465 725f 6e61  es..- `header_na
+00002d30: 6d65 7360 3a20 6e61 6d65 206f 6620 7468  mes`: name of th
+00002d40: 6520 6665 6174 7572 6573 2e0a 0a0a 2323  e features....##
+00002d50: 2045 7874 656e 6469 6e67 2074 6865 2074   Extending the t
+00002d60: 6f6f 6c6b 6974 0a0a 4164 6469 7469 6f6e  oolkit..Addition
+00002d70: 616c 6c79 2c20 7573 6572 7320 6d61 7920  ally, users may 
+00002d80: 696d 706c 656d 656e 7420 7468 6569 7220  implement their 
+00002d90: 6f77 6e20 6d65 7472 6963 206f 7220 6669  own metric or fi
+00002da0: 6775 7265 2063 6c61 7373 6573 2061 6e64  gure classes and
+00002db0: 2069 6e63 6c75 6465 2074 6865 6d20 6279   include them by
+00002dc0: 2075 7369 6e67 2074 6865 2060 4d65 7472   using the `Metr
+00002dd0: 6963 4661 6374 6f72 7960 206f 7220 6050  icFactory` or `P
+00002de0: 6c6f 7446 6163 746f 7279 6020 7265 6769  lotFactory` regi
+00002df0: 7374 6572 206d 6574 686f 6473 2e20 546f  ster methods. To
+00002e00: 2065 6e73 7572 6520 636f 6d70 6174 6962   ensure compatib
+00002e10: 696c 6974 7920 7769 7468 206f 7572 2074  ility with our t
+00002e20: 6f6f 6c6b 6974 2c20 7468 6579 2068 6176  oolkit, they hav
+00002e30: 6520 746f 2069 6e68 6572 6974 2066 726f  e to inherit fro
+00002e40: 6d20 7468 6520 6261 7365 2063 6c61 7373  m the base class
+00002e50: 6573 2060 4d65 7472 6963 6020 616e 6420  es `Metric` and 
+00002e60: 6050 6c6f 7460 2e0a 0a54 6865 2066 6f6c  `Plot`...The fol
+00002e70: 6c6f 7769 6e67 2063 6f64 6520 736e 6970  lowing code snip
+00002e80: 7065 7420 6973 2061 6e20 6578 616d 706c  pet is an exampl
+00002e90: 6520 6f66 2068 6f77 2074 6f20 696e 7472  e of how to intr
+00002ea0: 6f64 7563 6520 7468 6520 4575 636c 6964  oduce the Euclid
+00002eb0: 6561 6e20 6469 7374 616e 6365 206d 6574  ean distance met
+00002ec0: 7269 633a 0a0a 6060 6050 7974 686f 6e0a  ric:..```Python.
+00002ed0: 2365 752e 7079 0a69 6d70 6f72 7420 6e75  #eu.py.import nu
+00002ee0: 6d70 7920 6173 206e 700a 6672 6f6d 2073  mpy as np.from s
+00002ef0: 696d 696c 6172 6974 795f 7473 2e6d 6574  imilarity_ts.met
+00002f00: 7269 6373 2e6d 6574 7269 6320 696d 706f  rics.metric impo
+00002f10: 7274 204d 6574 7269 630a 0a0a 636c 6173  rt Metric...clas
+00002f20: 7320 4575 636c 6964 6561 6e44 6973 7461  s EuclideanDista
+00002f30: 6e63 6528 4d65 7472 6963 293a 0a0a 2020  nce(Metric):..  
+00002f40: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+00002f50: 656c 6629 3a0a 2020 2020 2020 2020 7375  elf):.        su
+00002f60: 7065 7228 292e 5f5f 696e 6974 5f5f 2829  per().__init__()
+00002f70: 0a20 2020 2020 2020 2073 656c 662e 6e61  .        self.na
+00002f80: 6d65 203d 2027 6564 270a 0a20 2020 2064  me = 'ed'..    d
+00002f90: 6566 2063 6f6d 7075 7465 2873 656c 662c  ef compute(self,
+00002fa0: 2074 7331 2c20 7473 322c 2073 696d 696c   ts1, ts2, simil
+00002fb0: 6172 6974 795f 7473 293a 0a20 2020 2020  arity_ts):.     
+00002fc0: 2020 206d 6574 7269 635f 7265 7375 6c74     metric_result
+00002fd0: 203d 207b 274d 756c 7469 7661 7269 6174   = {'Multivariat
+00002fe0: 6527 3a20 7365 6c66 2e5f 5f65 6428 7473  e': self.__ed(ts
+00002ff0: 312c 2074 7332 297d 0a20 2020 2020 2020  1, ts2)}.       
+00003000: 2072 6574 7572 6e20 6d65 7472 6963 5f72   return metric_r
+00003010: 6573 756c 740a 0a20 2020 2064 6566 2063  esult..    def c
+00003020: 6f6d 7075 7465 5f64 6973 7461 6e63 6528  ompute_distance(
+00003030: 7365 6c66 2c20 7473 312c 2074 7332 293a  self, ts1, ts2):
+00003040: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00003050: 7365 6c66 2e5f 5f65 6428 7473 312c 2074  self.__ed(ts1, t
+00003060: 7332 290a 0a20 2020 2064 6566 205f 5f65  s2)..    def __e
+00003070: 6428 7365 6c66 2c20 7473 312c 2074 7332  d(self, ts1, ts2
+00003080: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
+00003090: 6e20 6e70 2e6c 696e 616c 672e 6e6f 726d  n np.linalg.norm
+000030a0: 2874 7331 202d 2074 7332 290a 0a60 6060  (ts1 - ts2)..```
+000030b0: 0a0a 4166 7465 7277 6172 642c 2074 6869  ..Afterward, thi
+000030c0: 7320 6d65 7472 6963 2063 616e 2062 6520  s metric can be 
+000030d0: 7265 6769 7374 6572 6564 2062 7920 7573  registered by us
+000030e0: 696e 6720 7468 6520 6072 6567 6973 7465  ing the `registe
+000030f0: 725f 6d65 7472 6963 286d 6574 7269 635f  r_metric(metric_
+00003100: 636c 6173 7329 6020 6d65 7468 6f64 2066  class)` method f
+00003110: 726f 6d20 604d 6574 7269 6346 6163 746f  rom `MetricFacto
+00003120: 7279 6020 6173 2073 686f 776e 2069 6e20  ry` as shown in 
+00003130: 7468 6520 666f 6c6c 6f77 696e 6720 636f  the following co
+00003140: 6465 2073 6e69 7070 6574 3a0a 6060 6050  de snippet:.```P
+00003150: 7974 686f 6e0a 696d 706f 7274 206e 756d  ython.import num
+00003160: 7079 2061 7320 6e70 0a66 726f 6d20 7369  py as np.from si
+00003170: 6d69 6c61 7269 7479 5f74 732e 7369 6d69  milarity_ts.simi
+00003180: 6c61 7269 7479 5f74 7320 696d 706f 7274  larity_ts import
+00003190: 2053 696d 696c 6172 6974 7954 730a 6672   SimilarityTs.fr
+000031a0: 6f6d 2073 696d 696c 6172 6974 795f 7473  om similarity_ts
+000031b0: 2e6d 6574 7269 6373 2e6d 6574 7269 635f  .metrics.metric_
+000031c0: 6661 6374 6f72 7920 696d 706f 7274 204d  factory import M
+000031d0: 6574 7269 6346 6163 746f 7279 0a66 726f  etricFactory.fro
+000031e0: 6d20 6564 2069 6d70 6f72 7420 4575 636c  m ed import Eucl
+000031f0: 6964 6561 6e44 6973 7461 6e63 650a 0a4d  ideanDistance..M
+00003200: 6574 7269 6346 6163 746f 7279 2e67 6574  etricFactory.get
+00003210: 5f69 6e73 7461 6e63 6528 292e 7265 6769  _instance().regi
+00003220: 7374 6572 5f6d 6574 7269 6328 4575 636c  ster_metric(Eucl
+00003230: 6964 6561 6e44 6973 7461 6e63 6529 0a74  ideanDistance).t
+00003240: 7331 203d 206e 702e 7261 6e64 6f6d 2e72  s1 = np.random.r
+00003250: 616e 6428 3230 302c 2032 290a 7473 3273  and(200, 2).ts2s
+00003260: 203d 206e 702e 7261 6e64 6f6d 2e72 616e   = np.random.ran
+00003270: 6428 352c 2031 3030 2c20 3229 0a73 696d  d(5, 100, 2).sim
+00003280: 696c 6172 6974 795f 7473 203d 2053 696d  ilarity_ts = Sim
+00003290: 696c 6172 6974 7954 7328 7473 312c 2074  ilarityTs(ts1, t
+000032a0: 7332 7329 0a66 6f72 2074 7332 5f6e 616d  s2s).for ts2_nam
+000032b0: 652c 206d 6574 7269 635f 6e61 6d65 2c20  e, metric_name, 
+000032c0: 636f 6d70 7574 6564 5f6d 6574 7269 6320  computed_metric 
+000032d0: 696e 2073 696d 696c 6172 6974 795f 7473  in similarity_ts
+000032e0: 2e67 6574 5f6d 6574 7269 635f 636f 6d70  .get_metric_comp
+000032f0: 7574 6572 2829 3a0a 2020 2020 7072 696e  uter():.    prin
+00003300: 7428 6627 7b74 7332 5f6e 616d 657d 2e20  t(f'{ts2_name}. 
+00003310: 7b6d 6574 7269 635f 6e61 6d65 7d3a 207b  {metric_name}: {
+00003320: 636f 6d70 7574 6564 5f6d 6574 7269 637d  computed_metric}
+00003330: 2729 0a60 6060 0a0a 5369 6d69 6c61 726c  ').```..Similarl
+00003340: 792c 206e 6577 2070 6c6f 7473 2063 616e  y, new plots can
+00003350: 2062 6520 696e 7472 6f64 7563 6564 2e20   be introduced. 
+00003360: 466f 7220 696e 7374 616e 6365 2061 2060  For instance a `
+00003370: 5369 6d69 6c61 7269 7479 506c 6f74 4279  SimilarityPlotBy
+00003380: 436f 7272 656c 6174 696f 6e60 2063 6f75  Correlation` cou
+00003390: 6c64 2062 6520 6465 6669 6e65 6420 6173  ld be defined as
+000033a0: 3a0a 6060 6050 7974 686f 6e0a 2363 635f  :.```Python.#cc_
+000033b0: 706c 6f74 2e70 790a 696d 706f 7274 206e  plot.py.import n
+000033c0: 756d 7079 2061 7320 6e70 0a69 6d70 6f72  umpy as np.impor
+000033d0: 7420 6d61 7470 6c6f 746c 6962 2e70 7970  t matplotlib.pyp
+000033e0: 6c6f 7420 6173 2070 6c74 0a66 726f 6d20  lot as plt.from 
+000033f0: 7369 6d69 6c61 7269 7479 5f74 732e 706c  similarity_ts.pl
+00003400: 6f74 732e 706c 6f74 2069 6d70 6f72 7420  ots.plot import 
+00003410: 506c 6f74 0a0a 0a63 6c61 7373 2053 696d  Plot...class Sim
+00003420: 696c 6172 6974 7950 6c6f 7442 7943 6f72  ilarityPlotByCor
+00003430: 7265 6c61 7469 6f6e 2850 6c6f 7429 3a0a  relation(Plot):.
+00003440: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+00003450: 5f28 7365 6c66 2c20 6669 675f 7369 7a65  _(self, fig_size
+00003460: 3d28 382c 2036 2929 3a0a 2020 2020 2020  =(8, 6)):.      
+00003470: 2020 7375 7065 7228 292e 5f5f 696e 6974    super().__init
+00003480: 5f5f 2866 6967 5f73 697a 6529 0a20 2020  __(fig_size).   
+00003490: 2020 2020 2073 656c 662e 6e61 6d65 203d       self.name =
+000034a0: 2027 6363 2d70 6c6f 7427 0a0a 2020 2020   'cc-plot'..    
+000034b0: 6465 6620 636f 6d70 7574 6528 7365 6c66  def compute(self
+000034c0: 2c20 7369 6d69 6c61 7269 7479 5f74 732c  , similarity_ts,
+000034d0: 2074 7332 5f66 696c 656e 616d 6529 3a0a   ts2_filename):.
+000034e0: 2020 2020 2020 2020 7375 7065 7228 292e          super().
+000034f0: 636f 6d70 7574 6528 7369 6d69 6c61 7269  compute(similari
+00003500: 7479 5f74 732c 2074 7332 5f66 696c 656e  ty_ts, ts2_filen
+00003510: 616d 6529 0a20 2020 2020 2020 206e 5f66  ame).        n_f
+00003520: 6561 7475 7265 7320 3d20 7365 6c66 2e74  eatures = self.t
+00003530: 7331 2e73 6861 7065 5b31 5d0a 2020 2020  s1.shape[1].    
+00003540: 2020 2020 7369 6d69 6c61 7269 7479 203d      similarity =
+00003550: 206e 702e 636f 7272 636f 6566 2873 656c   np.corrcoef(sel
+00003560: 662e 7473 312e 542c 2073 656c 662e 7473  f.ts1.T, self.ts
+00003570: 322e 5429 0a20 2020 2020 2020 2066 6967  2.T).        fig
+00003580: 2c20 6178 203d 2070 6c74 2e73 7562 706c  , ax = plt.subpl
+00003590: 6f74 7328 290a 2020 2020 2020 2020 696d  ots().        im
+000035a0: 203d 2061 782e 696d 7368 6f77 2873 696d   = ax.imshow(sim
+000035b0: 696c 6172 6974 792c 2063 6d61 703d 2752  ilarity, cmap='R
+000035c0: 6459 6c42 7527 2c20 766d 696e 3d2d 312c  dYlBu', vmin=-1,
+000035d0: 2076 6d61 783d 3129 0a20 2020 2020 2020   vmax=1).       
+000035e0: 2061 782e 7365 745f 7874 6963 6b73 286e   ax.set_xticks(n
+000035f0: 702e 6172 616e 6765 286e 5f66 6561 7475  p.arange(n_featu
+00003600: 7265 732a 3229 290a 2020 2020 2020 2020  res*2)).        
+00003610: 6178 2e73 6574 5f79 7469 636b 7328 6e70  ax.set_yticks(np
+00003620: 2e61 7261 6e67 6528 6e5f 6665 6174 7572  .arange(n_featur
+00003630: 6573 2a32 2929 0a20 2020 2020 2020 2078  es*2)).        x
+00003640: 7469 636b 6c61 6265 6c73 203d 205b 6627  ticklabels = [f'
+00003650: 7473 315f 7b6e 6665 6174 7572 6573 5f69  ts1_{nfeatures_i
+00003660: 6e64 6578 7d27 666f 7220 6e66 6561 7475  ndex}'for nfeatu
+00003670: 7265 735f 696e 6465 7820 696e 2072 616e  res_index in ran
+00003680: 6765 2831 2c20 6e5f 6665 6174 7572 6573  ge(1, n_features
+00003690: 2b31 295d 0a20 2020 2020 2020 2078 7469  +1)].        xti
+000036a0: 636b 6c61 6265 6c73 203d 2078 7469 636b  cklabels = xtick
+000036b0: 6c61 6265 6c73 202b 205b 6627 7473 325f  labels + [f'ts2_
+000036c0: 7b6e 6665 6174 7572 6573 5f69 6e64 6578  {nfeatures_index
+000036d0: 7d27 666f 7220 6e66 6561 7475 7265 735f  }'for nfeatures_
+000036e0: 696e 6465 7820 696e 2072 616e 6765 2831  index in range(1
+000036f0: 2c20 6e5f 6665 6174 7572 6573 2b31 295d  , n_features+1)]
+00003700: 0a20 2020 2020 2020 2061 782e 7365 745f  .        ax.set_
+00003710: 7874 6963 6b6c 6162 656c 7328 7874 6963  xticklabels(xtic
+00003720: 6b6c 6162 656c 7329 0a20 2020 2020 2020  klabels).       
+00003730: 2061 782e 7365 745f 7974 6963 6b6c 6162   ax.set_yticklab
+00003740: 656c 7328 7874 6963 6b6c 6162 656c 7329  els(xticklabels)
+00003750: 0a20 2020 2020 2020 2061 782e 7365 745f  .        ax.set_
+00003760: 786c 6162 656c 2827 4665 6174 7572 6527  xlabel('Feature'
+00003770: 290a 2020 2020 2020 2020 6178 2e73 6574  ).        ax.set
+00003780: 5f79 6c61 6265 6c28 2746 6561 7475 7265  _ylabel('Feature
+00003790: 2729 0a20 2020 2020 2020 2066 6f72 2069  ').        for i
+000037a0: 2069 6e20 7261 6e67 6528 6e5f 6665 6174   in range(n_feat
+000037b0: 7572 6573 2a32 293a 0a20 2020 2020 2020  ures*2):.       
+000037c0: 2020 2020 2066 6f72 206a 2069 6e20 7261       for j in ra
+000037d0: 6e67 6528 6e5f 6665 6174 7572 6573 2a32  nge(n_features*2
+000037e0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000037f0: 2020 2061 782e 7465 7874 286a 2c20 692c     ax.text(j, i,
+00003800: 2066 277b 7369 6d69 6c61 7269 7479 5b69   f'{similarity[i
+00003810: 2c20 6a5d 3a2e 3266 7d27 2c20 6861 3d27  , j]:.2f}', ha='
+00003820: 6365 6e74 6572 272c 2076 613d 2763 656e  center', va='cen
+00003830: 7465 7227 2c20 636f 6c6f 723d 2762 6c61  ter', color='bla
+00003840: 636b 2729 0a0a 2020 2020 2020 2020 6362  ck')..        cb
+00003850: 6172 203d 2061 782e 6669 6775 7265 2e63  ar = ax.figure.c
+00003860: 6f6c 6f72 6261 7228 696d 2c20 6178 3d61  olorbar(im, ax=a
+00003870: 7829 0a20 2020 2020 2020 2063 6261 722e  x).        cbar.
+00003880: 6178 2e73 6574 5f79 6c61 6265 6c28 2753  ax.set_ylabel('S
+00003890: 696d 696c 6172 6974 7927 2c20 726f 7461  imilarity', rota
+000038a0: 7469 6f6e 3d2d 3930 2c20 7661 3d27 626f  tion=-90, va='bo
+000038b0: 7474 6f6d 2729 0a20 2020 2020 2020 2070  ttom').        p
+000038c0: 6c74 2e74 6974 6c65 2827 7369 6d69 6c61  lt.title('simila
+000038d0: 7269 7479 2d63 6f72 7265 6c61 7469 6f6e  rity-correlation
+000038e0: 2729 0a20 2020 2020 2020 2070 6c74 2e74  ').        plt.t
+000038f0: 6967 6874 5f6c 6179 6f75 7428 290a 2020  ight_layout().  
+00003900: 2020 2020 2020 7265 7475 726e 205b 2866        return [(f
+00003910: 6967 2c20 6178 295d 0a60 6060 0a0a 4166  ig, ax)].```..Af
+00003920: 7465 7277 6172 642c 2074 6869 7320 706c  terward, this pl
+00003930: 6f74 2063 616e 2062 6520 7265 6769 7374  ot can be regist
+00003940: 6572 6564 2062 7920 7573 696e 6720 7468  ered by using th
+00003950: 6520 6072 6567 6973 7465 725f 706c 6f74  e `register_plot
+00003960: 2870 6c6f 745f 636c 6173 7329 6020 6d65  (plot_class)` me
+00003970: 7468 6f64 2066 726f 6d20 6050 6c6f 7446  thod from `PlotF
+00003980: 6163 746f 7279 6020 6173 2073 686f 776e  actory` as shown
+00003990: 2069 6e20 7468 6520 666f 6c6c 6f77 696e   in the followin
+000039a0: 6720 636f 6465 2073 6e69 7070 6574 2074  g code snippet t
+000039b0: 6861 7420 7265 6769 7374 6572 2074 6865  hat register the
+000039c0: 206e 6577 206d 6574 7269 6320 616e 6420   new metric and 
+000039d0: 7468 6520 6e65 7720 706c 6f74 3a0a 6060  the new plot:.``
+000039e0: 6050 7974 686f 6e0a 696d 706f 7274 206f  `Python.import o
+000039f0: 730a 696d 706f 7274 206e 756d 7079 2061  s.import numpy a
+00003a00: 7320 6e70 0a66 726f 6d20 7369 6d69 6c61  s np.from simila
+00003a10: 7269 7479 5f74 732e 706c 6f74 732e 706c  rity_ts.plots.pl
+00003a20: 6f74 5f66 6163 746f 7279 2069 6d70 6f72  ot_factory impor
+00003a30: 7420 506c 6f74 4661 6374 6f72 790a 6672  t PlotFactory.fr
+00003a40: 6f6d 2073 696d 696c 6172 6974 795f 7473  om similarity_ts
+00003a50: 2e73 696d 696c 6172 6974 795f 7473 2069  .similarity_ts i
+00003a60: 6d70 6f72 7420 5369 6d69 6c61 7269 7479  mport Similarity
+00003a70: 5473 0a66 726f 6d20 7369 6d69 6c61 7269  Ts.from similari
+00003a80: 7479 5f74 732e 6d65 7472 6963 732e 6d65  ty_ts.metrics.me
+00003a90: 7472 6963 5f66 6163 746f 7279 2069 6d70  tric_factory imp
+00003aa0: 6f72 7420 4d65 7472 6963 4661 6374 6f72  ort MetricFactor
+00003ab0: 790a 6672 6f6d 2065 6420 696d 706f 7274  y.from ed import
+00003ac0: 2045 7563 6c69 6465 616e 4469 7374 616e   EuclideanDistan
+00003ad0: 6365 0a66 726f 6d20 6363 5f70 6c6f 7420  ce.from cc_plot 
+00003ae0: 696d 706f 7274 2053 696d 696c 6172 6974  import Similarit
+00003af0: 7950 6c6f 7442 7943 6f72 7265 6c61 7469  yPlotByCorrelati
+00003b00: 6f6e 0a0a 6465 6620 6d61 696e 2829 3a0a  on..def main():.
+00003b10: 2020 2020 4d65 7472 6963 4661 6374 6f72      MetricFactor
+00003b20: 792e 6765 745f 696e 7374 616e 6365 2829  y.get_instance()
+00003b30: 2e72 6567 6973 7465 725f 6d65 7472 6963  .register_metric
+00003b40: 2845 7563 6c69 6465 616e 4469 7374 616e  (EuclideanDistan
+00003b50: 6365 290a 2020 2020 506c 6f74 4661 6374  ce).    PlotFact
+00003b60: 6f72 792e 6765 745f 696e 7374 616e 6365  ory.get_instance
+00003b70: 2829 2e72 6567 6973 7465 725f 706c 6f74  ().register_plot
+00003b80: 2853 696d 696c 6172 6974 7950 6c6f 7442  (SimilarityPlotB
+00003b90: 7943 6f72 7265 6c61 7469 6f6e 290a 2020  yCorrelation).  
+00003ba0: 2020 7473 3120 3d20 6e70 2e72 616e 646f    ts1 = np.rando
+00003bb0: 6d2e 7261 6e64 2832 3030 2c20 3229 0a20  m.rand(200, 2). 
+00003bc0: 2020 2074 7332 7320 3d20 6e70 2e72 616e     ts2s = np.ran
+00003bd0: 646f 6d2e 7261 6e64 2835 2c20 3130 302c  dom.rand(5, 100,
+00003be0: 2032 290a 2020 2020 7369 6d69 6c61 7269   2).    similari
+00003bf0: 7479 5f74 7320 3d20 5369 6d69 6c61 7269  ty_ts = Similari
+00003c00: 7479 5473 2874 7331 2c20 7473 3273 290a  tyTs(ts1, ts2s).
+00003c10: 2020 2020 666f 7220 7473 325f 6e61 6d65      for ts2_name
+00003c20: 2c20 6d65 7472 6963 5f6e 616d 652c 2063  , metric_name, c
+00003c30: 6f6d 7075 7465 645f 6d65 7472 6963 2069  omputed_metric i
+00003c40: 6e20 7369 6d69 6c61 7269 7479 5f74 732e  n similarity_ts.
+00003c50: 6765 745f 6d65 7472 6963 5f63 6f6d 7075  get_metric_compu
+00003c60: 7465 7228 293a 0a20 2020 2020 2020 2070  ter():.        p
+00003c70: 7269 6e74 2866 277b 7473 325f 6e61 6d65  rint(f'{ts2_name
+00003c80: 7d2e 207b 6d65 7472 6963 5f6e 616d 657d  }. {metric_name}
+00003c90: 3a20 7b63 6f6d 7075 7465 645f 6d65 7472  : {computed_metr
+00003ca0: 6963 7d27 290a 2020 2020 666f 7220 7473  ic}').    for ts
+00003cb0: 325f 6e61 6d65 2c20 706c 6f74 5f6e 616d  2_name, plot_nam
+00003cc0: 652c 2067 656e 6572 6174 6564 5f70 6c6f  e, generated_plo
+00003cd0: 7473 2069 6e20 7369 6d69 6c61 7269 7479  ts in similarity
+00003ce0: 5f74 732e 6765 745f 706c 6f74 5f63 6f6d  _ts.get_plot_com
+00003cf0: 7075 7465 7228 293a 0a20 2020 2020 2020  puter():.       
+00003d00: 205f 5f73 6176 655f 6669 6775 7265 7328   __save_figures(
+00003d10: 7473 325f 6e61 6d65 2c20 706c 6f74 5f6e  ts2_name, plot_n
+00003d20: 616d 652c 2067 656e 6572 6174 6564 5f70  ame, generated_p
+00003d30: 6c6f 7473 290a 0a0a 6465 6620 5f5f 7361  lots)...def __sa
+00003d40: 7665 5f66 6967 7572 6573 2866 696c 656e  ve_figures(filen
+00003d50: 616d 652c 2070 6c6f 745f 6e61 6d65 2c20  ame, plot_name, 
+00003d60: 6765 6e65 7261 7465 645f 706c 6f74 7329  generated_plots)
+00003d70: 3a0a 2020 2020 666f 7220 706c 6f74 2069  :.    for plot i
+00003d80: 6e20 6765 6e65 7261 7465 645f 706c 6f74  n generated_plot
+00003d90: 733a 0a20 2020 2020 2020 2064 6972 5f70  s:.        dir_p
+00003da0: 6174 6820 3d20 5f5f 6372 6561 7465 5f64  ath = __create_d
+00003db0: 6972 6563 746f 7279 2866 696c 656e 616d  irectory(filenam
+00003dc0: 652c 2066 2766 6967 7572 6573 272c 2070  e, f'figures', p
+00003dd0: 6c6f 745f 6e61 6d65 290a 2020 2020 2020  lot_name).      
+00003de0: 2020 706c 6f74 5b30 5d2e 7361 7665 6669    plot[0].savefi
+00003df0: 6728 6627 7b64 6972 5f70 6174 687d 7b70  g(f'{dir_path}{p
+00003e00: 6c6f 745b 305d 2e61 7865 735b 305d 2e67  lot[0].axes[0].g
+00003e10: 6574 5f74 6974 6c65 2829 7d2e 7064 6627  et_title()}.pdf'
+00003e20: 2c20 666f 726d 6174 3d27 7064 6627 2c20  , format='pdf', 
+00003e30: 6262 6f78 5f69 6e63 6865 733d 2774 6967  bbox_inches='tig
+00003e40: 6874 2729 0a0a 0a64 6566 205f 5f63 7265  ht')...def __cre
+00003e50: 6174 655f 6469 7265 6374 6f72 7928 6669  ate_directory(fi
+00003e60: 6c65 6e61 6d65 2c20 7061 7468 2c20 706c  lename, path, pl
+00003e70: 6f74 5f6e 616d 6529 3a0a 2020 2020 6966  ot_name):.    if
+00003e80: 2070 6c6f 745f 6e61 6d65 2069 6e20 506c   plot_name in Pl
+00003e90: 6f74 4661 6374 6f72 792e 6765 745f 696e  otFactory.get_in
+00003ea0: 7374 616e 6365 2829 2e66 6967 7572 6573  stance().figures
+00003eb0: 5f72 6571 7569 7265 735f 616c 6c5f 7361  _requires_all_sa
+00003ec0: 6d70 6c65 733a 0a20 2020 2020 2020 2064  mples:.        d
+00003ed0: 6972 5f70 6174 6820 3d20 6627 7b70 6174  ir_path = f'{pat
+00003ee0: 687d 2f7b 706c 6f74 5f6e 616d 657d 2f27  h}/{plot_name}/'
+00003ef0: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+00003f00: 2020 206f 7269 6769 6e61 6c5f 6669 6c65     original_file
+00003f10: 6e61 6d65 203d 206f 732e 7061 7468 2e73  name = os.path.s
+00003f20: 706c 6974 6578 7428 6669 6c65 6e61 6d65  plitext(filename
+00003f30: 295b 305d 0a20 2020 2020 2020 2064 6972  )[0].        dir
+00003f40: 5f70 6174 6820 3d20 6627 7b70 6174 687d  _path = f'{path}
+00003f50: 2f7b 6f72 6967 696e 616c 5f66 696c 656e  /{original_filen
+00003f60: 616d 657d 2f7b 706c 6f74 5f6e 616d 657d  ame}/{plot_name}
+00003f70: 2f27 0a20 2020 206f 732e 6d61 6b65 6469  /'.    os.makedi
+00003f80: 7273 2864 6972 5f70 6174 682c 2065 7869  rs(dir_path, exi
+00003f90: 7374 5f6f 6b3d 5472 7565 290a 2020 2020  st_ok=True).    
+00003fa0: 7265 7475 726e 2064 6972 5f70 6174 680a  return dir_path.
+00003fb0: 0a69 6620 5f5f 6e61 6d65 5f5f 203d 3d20  .if __name__ == 
+00003fc0: 275f 5f6d 6169 6e5f 5f27 3a0a 2020 2020  '__main__':.    
+00003fd0: 6d61 696e 2829 0a60 6060 0a0a 2323 204c  main().```..## L
+00003fe0: 6963 656e 7365 0a0a 5369 6d69 6c61 7269  icense..Similari
+00003ff0: 7479 5453 2074 6f6f 6c6b 6974 2069 7320  tyTS toolkit is 
+00004000: 6672 6565 2061 6e64 206f 7065 6e2d 736f  free and open-so
+00004010: 7572 6365 2073 6f66 7477 6172 6520 6c69  urce software li
+00004020: 6365 6e73 6564 2075 6e64 6572 2074 6865  censed under the
+00004030: 205b 4d49 5420 6c69 6365 6e73 655d 284c   [MIT license](L
+00004040: 4943 454e 5345 292e 0a0a 2323 2041 636b  ICENSE)...## Ack
+00004050: 6e6f 776c 6564 6765 6d65 6e74 730a 5072  nowledgements.Pr
+00004060: 6f6a 6563 7420 5049 4432 3032 312d 3132  oject PID2021-12
+00004070: 3232 3038 4f42 2d49 3030 2c20 5052 4f59  2208OB-I00, PROY
+00004080: 4558 4345 4c5c 5f30 3032 3836 2061 6e64  EXCEL\_00286 and
+00004090: 2020 5445 4432 3032 312d 3133 3236 3935    TED2021-132695
+000040a0: 422d 4930 3020 7072 6f6a 6563 742c 2066  B-I00 project, f
+000040b0: 756e 6465 6420 6279 204d 4349 4e20 2f20  unded by MCIN / 
+000040c0: 4145 4920 2f20 3130 2e31 3330 3339 202f  AEI / 10.13039 /
+000040d0: 2035 3031 3130 3030 3131 3033 332c 2062   501100011033, b
+000040e0: 7920 416e 6461 6c75 7369 616e 2052 6567  y Andalusian Reg
+000040f0: 696f 6e61 6c20 476f 7665 726e 6d65 6e74  ional Government
+00004100: 2c20 616e 6420 6279 2074 6865 2045 7572  , and by the Eur
+00004110: 6f70 6561 6e20 556e 696f 6e20 2d20 4e65  opean Union - Ne
+00004120: 7874 4765 6e65 7261 7469 6f6e 4555 2e0a  xtGenerationEU..
```

### Comparing `similarity_ts-1.0.2/pyproject.toml` & `similarity_ts-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "similarity_ts"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
     { name = "Alejandro Fernández-Montes", email = "afdez@us.es" },
     { name = "Damián Fernández-Cerero", email = "damiancerero@us.es" },
     { name = "Felipe Escalera González", email = "fescalera@us.es" },
 ]
 dependencies = ["dtaidistance", "matplotlib", "pandas", "scikit-learn", "tqdm", "natsort", "chardet"]
 description = "SimilarityTS is an open-source project designed to facilitate the evaluation and comparison of multivariate time series data"
```

### Comparing `similarity_ts-1.0.2/src/similarity_ts/helpers/csv_reader_helper.py` & `similarity_ts-1.0.3/src/similarity_ts/helpers/csv_reader_helper.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.2/src/similarity_ts/helpers/dynamic_import_helper.py` & `similarity_ts-1.0.3/src/similarity_ts/helpers/dynamic_import_helper.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.2/src/similarity_ts/helpers/window_sampler.py` & `similarity_ts-1.0.3/src/similarity_ts/helpers/window_sampler.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.2/src/similarity_ts/metrics/cc.py` & `similarity_ts-1.0.3/src/similarity_ts/metrics/cc.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.2/src/similarity_ts/metrics/cp.py` & `similarity_ts-1.0.3/src/similarity_ts/metrics/cp.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.2/src/similarity_ts/metrics/dtw.py` & `similarity_ts-1.0.3/src/similarity_ts/metrics/dtw.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.2/src/similarity_ts/metrics/hi.py` & `similarity_ts-1.0.3/src/similarity_ts/metrics/hi.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.2/src/similarity_ts/metrics/js.py` & `similarity_ts-1.0.3/src/similarity_ts/metrics/js.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.2/src/similarity_ts/metrics/kl.py` & `similarity_ts-1.0.3/src/similarity_ts/metrics/kl.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.2/src/similarity_ts/metrics/ks.py` & `similarity_ts-1.0.3/src/similarity_ts/metrics/ks.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.2/src/similarity_ts/metrics/metric_computer.py` & `similarity_ts-1.0.3/src/similarity_ts/metrics/metric_computer.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.2/src/similarity_ts/metrics/metric_factory.py` & `similarity_ts-1.0.3/src/similarity_ts/metrics/metric_factory.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.2/src/similarity_ts/metrics/mmd.py` & `similarity_ts-1.0.3/src/similarity_ts/metrics/mmd.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.2/src/similarity_ts/plots/delta.py` & `similarity_ts-1.0.3/src/similarity_ts/plots/delta.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.2/src/similarity_ts/plots/dimensionalty_reduction.py` & `similarity_ts-1.0.3/src/similarity_ts/plots/dimensionalty_reduction.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.2/src/similarity_ts/plots/dtw.py` & `similarity_ts-1.0.3/src/similarity_ts/plots/dtw.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.2/src/similarity_ts/plots/pca.py` & `similarity_ts-1.0.3/src/similarity_ts/plots/pca.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.2/src/similarity_ts/plots/plot.py` & `similarity_ts-1.0.3/src/similarity_ts/plots/plot.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.2/src/similarity_ts/plots/plot_computer.py` & `similarity_ts-1.0.3/src/similarity_ts/plots/plot_computer.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.2/src/similarity_ts/plots/plot_config.py` & `similarity_ts-1.0.3/src/similarity_ts/plots/plot_config.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.2/src/similarity_ts/plots/plot_factory.py` & `similarity_ts-1.0.3/src/similarity_ts/plots/plot_factory.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.2/src/similarity_ts/plots/tsne.py` & `similarity_ts-1.0.3/src/similarity_ts/plots/tsne.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.2/src/similarity_ts/plots/two_dimensions.py` & `similarity_ts-1.0.3/src/similarity_ts/plots/two_dimensions.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.2/src/similarity_ts/similarity_analysis_computer.py` & `similarity_ts-1.0.3/src/similarity_ts/similarity_analysis_computer.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.2/src/similarity_ts/similarity_ts.py` & `similarity_ts-1.0.3/src/similarity_ts/similarity_ts.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.2/src/similarity_ts/similarity_ts_config.py` & `similarity_ts-1.0.3/src/similarity_ts/similarity_ts_config.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.2/src/similarity_ts.egg-info/PKG-INFO` & `similarity_ts-1.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 Metadata-Version: 2.1
-Name: similarity-ts
-Version: 1.0.2
+Name: similarity_ts
+Version: 1.0.3
 Summary: SimilarityTS is an open-source project designed to facilitate the evaluation and comparison of multivariate time series data
 Author-email: Alejandro Fernández-Montes <afdez@us.es>, Damián Fernández-Cerero <damiancerero@us.es>, Felipe Escalera González <fescalera@us.es>
 Project-URL: Homepage, https://github.com/alejandrofdez-us/similarity-ts
 Project-URL: Bug Tracker, https://github.com/alejandrofdez-us/similarity-ts/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![version](https://img.shields.io/badge/version-1.0-blue)](https://github.com/alejandrofdez-us/similarity-ts/releases)
+[![version](https://img.shields.io/badge/pypi-1.0.3-blue)](https://pypi.org/project/similarity-ts/)
 [![Python 3.9](https://img.shields.io/badge/python-3.9-darkgreen)](https://www.python.org/downloads/release/python-390/)
-[![last-update](https://img.shields.io/badge/last_update-07/XY/2023-brightgreen)](https://github.com/alejandrofdez-us/similarity-ts/commits/main)
-![license](https://img.shields.io/badge/license-MIT-orange)
+[![last-update](https://img.shields.io/badge/last_update-07/18/2023-brightgreen)](https://github.com/alejandrofdez-us/similarity-ts-cli/commits/main)
+[![license](https://img.shields.io/badge/license-MIT-orange)](LICENSE)
 
 # SimilarityTS: Toolkit for the Evaluation of Similarity for multivariate time series
 
 ## Table of Contents
 
 - [Package Description](#package-description)
 - [Installation](#installation)
 - [Usage](#usage)
 - [Configuring the toolkit](#configuring-the-toolkit)
 - [Extending the toolkit](#extending-the-toolkit)
 - [License](#license)
+- [Acknowledgements](#acknowledgements)
 
 ## Package Description
 
 SimilarityTS is an open-source package designed to facilitate the evaluation and comparison of
 multivariate time series data. It provides a comprehensive toolkit for analyzing, visualizing, and reporting multiple
 metrics and figures derived from time series datasets. The toolkit simplifies the process of evaluating the similarity of
 time series by offering data preprocessing, metrics computation, visualization, statistical analysis, and report generation
 functionalities. With its customizable features, SimilarityTS empowers researchers and data
 scientists to gain insights, identify patterns, and make informed decisions based on their time series data.
 
-A command line interface tool is also available at: https://github.com/alejandrofdez-us/similarity-ts-cli
+A command line interface tool is also available at: https://github.com/alejandrofdez-us/similarity-ts-cli.
 
 ### Available metrics
 
 This toolkit can compute the following metrics:
 
 - `kl`: Kullback-Leibler divergence
 - `js`: Jensen-Shannon divergence
@@ -103,41 +104,41 @@
 ```
 
 ## Usage
 
 Users must create a new `SimilarityTs` object by calling its constructor and passing the following parameters.
 
 - `ts1` This time series may represent the baseline or ground truth time
-  series as a `numpy` object with shape `[length, num_features]`.
-- `ts2s` A single or a set of time series as a `numpy` object with shape `[num_time_series, length, num_features]`.
+  series as a `numpy` array with shape `[length, num_features]`.
+- `ts2s` A single or a set of time series as a `numpy` array with shape `[num_time_series, length, num_features]`.
 
 
 Constraints:
 
 - `ts1` time-series and `ts2s` time-series file(s) must:
     - have the same dimensionality (number of columns)
-    - do not include a timestamp column
+    - not include a timestamp column
     - include only numeric values
 - all `ts2s` time-series must have the same length (number of rows).
 
 If `ts1` time-series is longer (more rows) than `ts2s` time-series, the `ts1` time series will be
 divided in windows of the same length as the `ts2s` time-series.
 
 For each `ts2s` time-series, the most similar window (*) from `ts1` time series is selected.
 
 Finally, metrics and figures that assess the similarity between each pair of `ts2s` time-series and its
 associated most similar `ts1` window are computed.
 
 (*) The metric used for the selection of the most
-similar `ts1` time-series window per each `ts2s` time-series file is selectable.`dtw` is the default selected metric, however, any of
+similar `ts1` time-series window per each `ts2s` time-series file is selectable. `dtw` is the default selected metric, however, any of
 the
-[metrics](#available-metrics) are also available for this purpose. See the [toolkit configuration section](#configuring-the-toolkit)
+[metrics](#available-metrics) are also available for this purpose. See the [toolkit configuration section](#configuring-the-toolkit).
 
 ### Minimal usage examples:
-Usage examples can be found at: https://github.com/alejandrofdez-us/similarity-ts/tree/main/usage_examples
+Usage examples can be found at: https://github.com/alejandrofdez-us/similarity-ts/tree/main/usage_examples.
 
 1. Compute metrics between random time series (`ts1`: one time series of lenght 200 and 2 dimensions and `ts2`: five time series of length 100 and 2 dimensions):
     ```Python
     import numpy as np
     from similarity_ts.similarity_ts import SimilarityTs
     
     ts1 = np.random.rand(200, 2)
@@ -214,15 +215,15 @@
 - `timestamp_frequency_seconds`: the frequency in seconds in which samples were taken. This is needed to generate the delta figures with correct time magnitudes. By default is
   `1` second.
 - `stride`: when `ts1` time-series is longer than `ts2s` time-series the windows are computed by using a
   stride of `1` by default. Sometimes using a larger value for the stride parameter improves the performance by skipping
   the computation of similarity between so many windows.
 - `window_selection_metric`: the metric used for the selection of the most similar `ts1` time-series window per each `ts2s` time-series file is selectable.`dtw` is the default selected metric, however, any of the [metrics](#available-metrics) are also available for this purpose. See the [toolkit configuration section](#configuring-the-toolkit).
 - `ts2_names`: name of each time series of the `ts2s` set of time series.
-- `header_names`: name of the features
+- `header_names`: name of the features.
 
 
 ## Extending the toolkit
 
 Additionally, users may implement their own metric or figure classes and include them by using the `MetricFactory` or `PlotFactory` register methods. To ensure compatibility with our toolkit, they have to inherit from the base classes `Metric` and `Plot`.
 
 The following code snippet is an example of how to introduce the Euclidean distance metric:
@@ -345,7 +346,10 @@
 if __name__ == '__main__':
     main()
 ```
 
 ## License
 
 SimilarityTS toolkit is free and open-source software licensed under the [MIT license](LICENSE).
+
+## Acknowledgements
+Project PID2021-122208OB-I00, PROYEXCEL\_00286 and  TED2021-132695B-I00 project, funded by MCIN / AEI / 10.13039 / 501100011033, by Andalusian Regional Government, and by the European Union - NextGenerationEU.
```

### Comparing `similarity_ts-1.0.2/src/similarity_ts.egg-info/SOURCES.txt` & `similarity_ts-1.0.3/src/similarity_ts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

