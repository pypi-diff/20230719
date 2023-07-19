# Comparing `tmp/openla_feature_representation-0.1.0a5.tar.gz` & `tmp/openla_feature_representation-0.1.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openla_feature_representation-0.1.0a5.tar", max compression
+gzip compressed data, was "openla_feature_representation-0.1.1a2.tar", max compression
```

## Comparing `openla_feature_representation-0.1.0a5.tar` & `openla_feature_representation-0.1.1a2.tar`

### file list

```diff
@@ -1,6 +1,11 @@
--rw-r--r--   0        0        0     1061 2023-06-12 07:23:54.810526 openla_feature_representation-0.1.0a5/LICENSE
--rw-r--r--   0        0        0     4426 2023-07-03 01:39:09.235628 openla_feature_representation-0.1.0a5/README.md
--rw-r--r--   0        0        0       32 2023-06-23 06:28:03.604924 openla_feature_representation-0.1.0a5/openla_feature_representation/__init__.py
--rw-r--r--   0        0        0    15978 2023-06-28 05:02:19.897260 openla_feature_representation-0.1.0a5/openla_feature_representation/openla_e2vec.py
--rw-r--r--   0        0        0      478 2023-07-03 01:40:04.288741 openla_feature_representation-0.1.0a5/pyproject.toml
--rw-r--r--   0        0        0     5061 1970-01-01 00:00:00.000000 openla_feature_representation-0.1.0a5/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-12 07:23:54.810526 openla_feature_representation-0.1.1a2/LICENSE
+-rw-r--r--   0        0        0     5867 2023-07-11 07:33:03.678501 openla_feature_representation-0.1.1a2/README.md
+-rw-r--r--   0        0        0      119 2023-07-03 04:59:58.021381 openla_feature_representation-0.1.1a2/openla_feature_representation/__init__.py
+-rw-r--r--   0        0        0       77 2023-07-03 04:59:58.021619 openla_feature_representation-0.1.1a2/openla_feature_representation/alp/__init__.py
+-rw-r--r--   0        0        0    17877 2023-07-03 04:59:58.021933 openla_feature_representation-0.1.1a2/openla_feature_representation/alp/extract_feature_alp.py
+-rw-r--r--   0        0        0     4140 2023-07-03 04:59:58.022118 openla_feature_representation-0.1.1a2/openla_feature_representation/alp/features_extracted_function.py
+-rw-r--r--   0        0        0    12068 2023-07-03 04:59:58.022306 openla_feature_representation-0.1.1a2/openla_feature_representation/alp/load_dataset.py
+-rw-r--r--   0        0        0     5761 2023-07-03 04:59:58.022503 openla_feature_representation-0.1.1a2/openla_feature_representation/alp/utils.py
+-rw-r--r--   0        0        0    15978 2023-07-03 04:59:58.022609 openla_feature_representation-0.1.1a2/openla_feature_representation/e2vec/openla_e2vec.py
+-rw-r--r--   0        0        0      478 2023-07-19 00:51:00.610428 openla_feature_representation-0.1.1a2/pyproject.toml
+-rw-r--r--   0        0        0     6502 1970-01-01 00:00:00.000000 openla_feature_representation-0.1.1a2/PKG-INFO
```

### Comparing `openla_feature_representation-0.1.0a5/LICENSE` & `openla_feature_representation-0.1.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `openla_feature_representation-0.1.0a5/openla_feature_representation/openla_e2vec.py` & `openla_feature_representation-0.1.1a2/openla_feature_representation/e2vec/openla_e2vec.py`

 * *Files identical despite different names*

### Comparing `openla_feature_representation-0.1.0a5/PKG-INFO` & `openla_feature_representation-0.1.1a2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: openla-feature-representation
-Version: 0.1.0a5
-Summary: A Python module that adds features to OpenLA data to make it easier to use for ML
-Author: LIMU
-Author-email: repository@limu.ait.kyushu-u.ac.jp
-Requires-Python: >=3.8,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: fasttext-wheel (>=0.9.2,<0.10.0)
-Requires-Dist: openla (>=0.2.8,<0.3.0)
-Description-Content-Type: text/markdown
-
 # openla-feature-representation: generate features for EventStream data
 
 ## Introduction
 
 openla-feature-representation is an open-source Python module that generates features from [OpenLA](https://limu.ait.kyushu-u.ac.jp/~openLA/) EventStream data, to make the data easier to use for ML.
 
 ## Installation
@@ -141,11 +125,39 @@
 - `vector_path` needs a string, but it is currently unused (to be removed)
 - `info_dir` is the path to a directory with the dataset (see below)
 - `course_id` is a string to identify files for the course to analyze within the `info_dir` directory
 - `concat_mode` needs to be "time" or "week"
 - `start` is the minute in the data the sentence generation should start (optional)
 - `period` is the number of minutes worth of sentences that should be generated each time (optional)
 
-## Datasets for OpenLA
+## Usage of the ALP (Active Learner Point) functions
+
+ALP is a set of metrics that take BookRoll (ebook) and Moodle activity per lecture into account: attendance, report submissions, course views, slide views, adding markers or memos, and other actions.
+
+First, the `aggregate_feature` function aggregates the number of times each user took any of the actions above for each lecture, resulting on a DataFrame that we will call `features_df` on this example. These are the features ALP will work with.
+
+```py
+from openla_feature_representation import aggregate_feature
+features_df = aggregate_feature(course_id=course_id)
+```
+
+- `course_id` is an `int` to identify files for the course to analyze within the `Dataset` directory
 
-This module uses data in the same format as OpenLA. Please refer to the [OpenLA documentation](https://limu.ait.kyushu-u.ac.jp/~openLA/) for further information.
+To further ready the data for ML and other analysis, the `feature2ALP` function returns a DataFrame that we will call `alp_df`, in which the feature is replaced by a number from 0 to 5 with the following meaning:
+
+- `5`: Top 10%, or attending the lecture, or submitting a report
+- `4`: Top 20%
+- `3`: Top 30%, or being late to the lecture, or submitting late
+- `2`: Top 40%
+- `1`: Top 50%
+- `0`: Bottom 50%, or not attending, or not submitting
+
+The additional `alp_df_normalized` DataFrame returned by the function is the same data as `alp_df`, only normalized to `1`.
+
+```py
+from openla_feature_representation import feature2ALP
+alp_df, alp_df_normalized = feature2ALP(features_df=features_df)
+```
+
+## Datasets for OpenLA
 
+This module uses data in the same or a similar format as OpenLA. Please refer to the [OpenLA documentation](https://limu.ait.kyushu-u.ac.jp/~openLA/) for further information.
```

