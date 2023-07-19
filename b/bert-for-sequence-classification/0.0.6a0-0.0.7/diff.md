# Comparing `tmp/bert-for-sequence-classification-0.0.6a0.tar.gz` & `tmp/bert-for-sequence-classification-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bert-for-sequence-classification-0.0.6a0.tar", last modified: Wed Jul 19 12:30:14 2023, max compression
+gzip compressed data, was "bert-for-sequence-classification-0.0.7.tar", last modified: Wed Jul 19 12:37:06 2023, max compression
```

## Comparing `bert-for-sequence-classification-0.0.6a0.tar` & `bert-for-sequence-classification-0.0.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:30:14.105203 bert-for-sequence-classification-0.0.6a0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-19 12:30:00.000000 bert-for-sequence-classification-0.0.6a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-07-19 12:30:14.105203 bert-for-sequence-classification-0.0.6a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-07-19 12:30:00.000000 bert-for-sequence-classification-0.0.6a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:30:14.101203 bert-for-sequence-classification-0.0.6a0/bert_clf/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-19 12:30:00.000000 bert-for-sequence-classification-0.0.6a0/bert_clf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-07-19 12:30:00.000000 bert-for-sequence-classification-0.0.6a0/bert_clf/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:30:14.101203 bert-for-sequence-classification-0.0.6a0/bert_clf/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:30:00.000000 bert-for-sequence-classification-0.0.6a0/bert_clf/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:30:14.105203 bert-for-sequence-classification-0.0.6a0/bert_clf/src/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-07-19 12:30:00.000000 bert-for-sequence-classification-0.0.6a0/bert_clf/src/core/BaseDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-19 12:30:00.000000 bert-for-sequence-classification-0.0.6a0/bert_clf/src/core/BaseModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-19 12:30:00.000000 bert-for-sequence-classification-0.0.6a0/bert_clf/src/core/CLFFabric.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-19 12:30:00.000000 bert-for-sequence-classification-0.0.6a0/bert_clf/src/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-19 12:30:00.000000 bert-for-sequence-classification-0.0.6a0/bert_clf/src/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-19 12:30:00.000000 bert-for-sequence-classification-0.0.6a0/bert_clf/src/early_stopping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:30:14.105203 bert-for-sequence-classification-0.0.6a0/bert_clf/src/models/
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-19 12:30:00.000000 bert-for-sequence-classification-0.0.6a0/bert_clf/src/models/BertCLF.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-19 12:30:00.000000 bert-for-sequence-classification-0.0.6a0/bert_clf/src/models/EncoderCLF.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-19 12:30:00.000000 bert-for-sequence-classification-0.0.6a0/bert_clf/src/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:30:14.105203 bert-for-sequence-classification-0.0.6a0/bert_clf/src/pandas_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-19 12:30:00.000000 bert-for-sequence-classification-0.0.6a0/bert_clf/src/pandas_dataset/PandasDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-19 12:30:00.000000 bert-for-sequence-classification-0.0.6a0/bert_clf/src/pandas_dataset/SimpleDataFrame.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:30:00.000000 bert-for-sequence-classification-0.0.6a0/bert_clf/src/pandas_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-07-19 12:30:00.000000 bert-for-sequence-classification-0.0.6a0/bert_clf/src/preparing_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7868 2023-07-19 12:30:00.000000 bert-for-sequence-classification-0.0.6a0/bert_clf/src/training_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-19 12:30:00.000000 bert-for-sequence-classification-0.0.6a0/bert_clf/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:30:14.105203 bert-for-sequence-classification-0.0.6a0/bert_for_sequence_classification.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-07-19 12:30:14.000000 bert-for-sequence-classification-0.0.6a0/bert_for_sequence_classification.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-19 12:30:14.000000 bert-for-sequence-classification-0.0.6a0/bert_for_sequence_classification.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 12:30:14.000000 bert-for-sequence-classification-0.0.6a0/bert_for_sequence_classification.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-19 12:30:14.000000 bert-for-sequence-classification-0.0.6a0/bert_for_sequence_classification.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-19 12:30:14.000000 bert-for-sequence-classification-0.0.6a0/bert_for_sequence_classification.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-19 12:30:14.000000 bert-for-sequence-classification-0.0.6a0/bert_for_sequence_classification.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-19 12:30:14.105203 bert-for-sequence-classification-0.0.6a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-19 12:30:00.000000 bert-for-sequence-classification-0.0.6a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:37:06.914247 bert-for-sequence-classification-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-19 12:36:55.000000 bert-for-sequence-classification-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-19 12:37:06.914247 bert-for-sequence-classification-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-07-19 12:36:55.000000 bert-for-sequence-classification-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:37:06.906247 bert-for-sequence-classification-0.0.7/bert_clf/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-19 12:36:55.000000 bert-for-sequence-classification-0.0.7/bert_clf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-07-19 12:36:55.000000 bert-for-sequence-classification-0.0.7/bert_clf/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:37:06.910247 bert-for-sequence-classification-0.0.7/bert_clf/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:36:55.000000 bert-for-sequence-classification-0.0.7/bert_clf/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:37:06.910247 bert-for-sequence-classification-0.0.7/bert_clf/src/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-07-19 12:36:55.000000 bert-for-sequence-classification-0.0.7/bert_clf/src/core/BaseDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-19 12:36:55.000000 bert-for-sequence-classification-0.0.7/bert_clf/src/core/BaseModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-19 12:36:55.000000 bert-for-sequence-classification-0.0.7/bert_clf/src/core/CLFFabric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-19 12:36:55.000000 bert-for-sequence-classification-0.0.7/bert_clf/src/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-19 12:36:55.000000 bert-for-sequence-classification-0.0.7/bert_clf/src/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-19 12:36:55.000000 bert-for-sequence-classification-0.0.7/bert_clf/src/early_stopping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:37:06.910247 bert-for-sequence-classification-0.0.7/bert_clf/src/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-19 12:36:55.000000 bert-for-sequence-classification-0.0.7/bert_clf/src/models/BertCLF.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-19 12:36:55.000000 bert-for-sequence-classification-0.0.7/bert_clf/src/models/EncoderCLF.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-19 12:36:55.000000 bert-for-sequence-classification-0.0.7/bert_clf/src/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:37:06.910247 bert-for-sequence-classification-0.0.7/bert_clf/src/pandas_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-19 12:36:55.000000 bert-for-sequence-classification-0.0.7/bert_clf/src/pandas_dataset/PandasDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-19 12:36:55.000000 bert-for-sequence-classification-0.0.7/bert_clf/src/pandas_dataset/SimpleDataFrame.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:36:55.000000 bert-for-sequence-classification-0.0.7/bert_clf/src/pandas_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-07-19 12:36:55.000000 bert-for-sequence-classification-0.0.7/bert_clf/src/preparing_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7868 2023-07-19 12:36:55.000000 bert-for-sequence-classification-0.0.7/bert_clf/src/training_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-19 12:36:56.000000 bert-for-sequence-classification-0.0.7/bert_clf/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:37:06.914247 bert-for-sequence-classification-0.0.7/bert_for_sequence_classification.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-19 12:37:06.000000 bert-for-sequence-classification-0.0.7/bert_for_sequence_classification.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-19 12:37:06.000000 bert-for-sequence-classification-0.0.7/bert_for_sequence_classification.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 12:37:06.000000 bert-for-sequence-classification-0.0.7/bert_for_sequence_classification.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-19 12:37:06.000000 bert-for-sequence-classification-0.0.7/bert_for_sequence_classification.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-19 12:37:06.000000 bert-for-sequence-classification-0.0.7/bert_for_sequence_classification.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-19 12:37:06.000000 bert-for-sequence-classification-0.0.7/bert_for_sequence_classification.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-19 12:37:06.914247 bert-for-sequence-classification-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-19 12:36:56.000000 bert-for-sequence-classification-0.0.7/setup.py
```

### Comparing `bert-for-sequence-classification-0.0.6a0/LICENSE` & `bert-for-sequence-classification-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.6a0/PKG-INFO` & `bert-for-sequence-classification-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bert-for-sequence-classification
-Version: 0.0.6a0
+Version: 0.0.7
 Summary: Easy fine-tuning for BERT models
 Author: Tatiana Iazykova
 Author-email: tania_yazykova@bk.ru
 Keywords: python,bert,deep learning,nlp
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `bert-for-sequence-classification-0.0.6a0/README.md` & `bert-for-sequence-classification-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.6a0/bert_clf/pipeline.py` & `bert-for-sequence-classification-0.0.7/bert_clf/pipeline.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.6a0/bert_clf/src/core/BaseDataset.py` & `bert-for-sequence-classification-0.0.7/bert_clf/src/core/BaseDataset.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.6a0/bert_clf/src/core/BaseModel.py` & `bert-for-sequence-classification-0.0.7/bert_clf/src/core/BaseModel.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.6a0/bert_clf/src/core/CLFFabric.py` & `bert-for-sequence-classification-0.0.7/bert_clf/src/core/CLFFabric.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.6a0/bert_clf/src/dataset.py` & `bert-for-sequence-classification-0.0.7/bert_clf/src/dataset.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.6a0/bert_clf/src/early_stopping.py` & `bert-for-sequence-classification-0.0.7/bert_clf/src/early_stopping.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.6a0/bert_clf/src/models/BertCLF.py` & `bert-for-sequence-classification-0.0.7/bert_clf/src/models/BertCLF.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.6a0/bert_clf/src/models/EncoderCLF.py` & `bert-for-sequence-classification-0.0.7/bert_clf/src/models/EncoderCLF.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.6a0/bert_clf/src/pandas_dataset/PandasDataset.py` & `bert-for-sequence-classification-0.0.7/bert_clf/src/pandas_dataset/PandasDataset.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.6a0/bert_clf/src/pandas_dataset/SimpleDataFrame.py` & `bert-for-sequence-classification-0.0.7/bert_clf/src/pandas_dataset/SimpleDataFrame.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.6a0/bert_clf/src/preparing_data_utils.py` & `bert-for-sequence-classification-0.0.7/bert_clf/src/preparing_data_utils.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.6a0/bert_clf/src/training_utils.py` & `bert-for-sequence-classification-0.0.7/bert_clf/src/training_utils.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.6a0/bert_clf/utils.py` & `bert-for-sequence-classification-0.0.7/bert_clf/utils.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.6a0/bert_for_sequence_classification.egg-info/PKG-INFO` & `bert-for-sequence-classification-0.0.7/bert_for_sequence_classification.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bert-for-sequence-classification
-Version: 0.0.6a0
+Version: 0.0.7
 Summary: Easy fine-tuning for BERT models
 Author: Tatiana Iazykova
 Author-email: tania_yazykova@bk.ru
 Keywords: python,bert,deep learning,nlp
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `bert-for-sequence-classification-0.0.6a0/bert_for_sequence_classification.egg-info/SOURCES.txt` & `bert-for-sequence-classification-0.0.7/bert_for_sequence_classification.egg-info/SOURCES.txt`

 * *Files identical despite different names*

