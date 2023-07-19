# Comparing `tmp/OmniEvent-0.1.6.tar.gz` & `tmp/OmniEvent-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OmniEvent-0.1.6.tar", last modified: Mon May 15 04:53:37 2023, max compression
+gzip compressed data, was "OmniEvent-0.1.7.tar", last modified: Wed Jul 19 06:30:30 2023, max compression
```

## Comparing `OmniEvent-0.1.6.tar` & `OmniEvent-0.1.7.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwsr-x   0 ph        (1004) ph        (1004)        0 2023-05-15 04:53:37.590532 OmniEvent-0.1.6/
--rw-rw-r--   0 ph        (1004) ph        (1004)     1049 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/LICENSE
-drwxrwsr-x   0 ph        (1004) ph        (1004)        0 2023-05-15 04:53:37.582532 OmniEvent-0.1.6/OmniEvent/
--rw-rw-r--   0 ph        (1004) ph        (1004)        0 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/__init__.py
-drwxrwsr-x   0 ph        (1004) ph        (1004)        0 2023-05-15 04:53:37.586532 OmniEvent-0.1.6/OmniEvent/aggregation/
--rw-rw-r--   0 ph        (1004) ph        (1004)        0 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/aggregation/__init__.py
--rw-rw-r--   0 ph        (1004) ph        (1004)    20012 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/aggregation/aggregation.py
--rw-rw-r--   0 ph        (1004) ph        (1004)    13142 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/arguments.py
-drwxrwsr-x   0 ph        (1004) ph        (1004)        0 2023-05-15 04:53:37.586532 OmniEvent-0.1.6/OmniEvent/backbone/
--rw-rw-r--   0 ph        (1004) ph        (1004)        0 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/backbone/__init__.py
--rw-rw-r--   0 ph        (1004) ph        (1004)    14972 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/backbone/backbone.py
-drwxrwsr-x   0 ph        (1004) ph        (1004)        0 2023-05-15 04:53:37.586532 OmniEvent-0.1.6/OmniEvent/evaluation/
--rw-rw-r--   0 ph        (1004) ph        (1004)        0 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/evaluation/__init__.py
--rw-rw-r--   0 ph        (1004) ph        (1004)    27628 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/evaluation/convert_format.py
--rw-rw-r--   0 ph        (1004) ph        (1004)    15442 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/evaluation/dump_result.py
--rw-rw-r--   0 ph        (1004) ph        (1004)    18870 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/evaluation/metric.py
--rw-rw-r--   0 ph        (1004) ph        (1004)    20868 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/evaluation/utils.py
-drwxrwsr-x   0 ph        (1004) ph        (1004)        0 2023-05-15 04:53:37.586532 OmniEvent-0.1.6/OmniEvent/head/
--rw-rw-r--   0 ph        (1004) ph        (1004)        0 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/head/__init__.py
--rw-rw-r--   0 ph        (1004) ph        (1004)     2297 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/head/classification.py
--rw-rw-r--   0 ph        (1004) ph        (1004)    13128 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/head/crf.py
--rw-rw-r--   0 ph        (1004) ph        (1004)      508 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/head/head.py
--rw-rw-r--   0 ph        (1004) ph        (1004)     5354 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/infer.py
-drwxrwsr-x   0 ph        (1004) ph        (1004)        0 2023-05-15 04:53:37.586532 OmniEvent-0.1.6/OmniEvent/infer_module/
--rw-rw-r--   0 ph        (1004) ph        (1004)        0 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/infer_module/__init__.py
--rw-rw-r--   0 ph        (1004) ph        (1004)     1755 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/infer_module/io_format.py
--rw-rw-r--   0 ph        (1004) ph        (1004)     9832 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/infer_module/seq2seq.py
-drwxrwsr-x   0 ph        (1004) ph        (1004)        0 2023-05-15 04:53:37.590532 OmniEvent-0.1.6/OmniEvent/input_engineering/
--rw-rw-r--   0 ph        (1004) ph        (1004)        0 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/input_engineering/__init__.py
--rw-rw-r--   0 ph        (1004) ph        (1004)    21674 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/input_engineering/base_processor.py
--rw-rw-r--   0 ph        (1004) ph        (1004)    18195 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/input_engineering/input_utils.py
--rw-rw-r--   0 ph        (1004) ph        (1004)    11310 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/input_engineering/mrc_converter.py
--rw-rw-r--   0 ph        (1004) ph        (1004)    20815 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/input_engineering/mrc_processor.py
--rw-rw-r--   0 ph        (1004) ph        (1004)    14875 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/input_engineering/seq2seq_processor.py
--rw-rw-r--   0 ph        (1004) ph        (1004)    13751 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/input_engineering/sequence_labeling_processor.py
--rw-rw-r--   0 ph        (1004) ph        (1004)    18459 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/input_engineering/token_classification_processor.py
--rw-rw-r--   0 ph        (1004) ph        (1004)    11756 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/input_engineering/tokenizer.py
--rw-rw-r--   0 ph        (1004) ph        (1004)    12996 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/input_engineering/whitespace_tokenizer.py
-drwxrwsr-x   0 ph        (1004) ph        (1004)        0 2023-05-15 04:53:37.590532 OmniEvent-0.1.6/OmniEvent/model/
--rw-rw-r--   0 ph        (1004) ph        (1004)        0 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/model/__init__.py
--rw-rw-r--   0 ph        (1004) ph        (1004)    12627 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/model/constraint_decoding.py
--rw-rw-r--   0 ph        (1004) ph        (1004)     2342 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/model/label_smoother_sum.py
--rw-rw-r--   0 ph        (1004) ph        (1004)    12488 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/model/model.py
--rw-rw-r--   0 ph        (1004) ph        (1004)    10211 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/trainer.py
--rw-rw-r--   0 ph        (1004) ph        (1004)    18172 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/trainer_seq2seq.py
--rw-rw-r--   0 ph        (1004) ph        (1004)     2300 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/OmniEvent/utils.py
-drwxrwsr-x   0 ph        (1004) ph        (1004)        0 2023-05-15 04:53:37.586532 OmniEvent-0.1.6/OmniEvent.egg-info/
--rw-rw-r--   0 ph        (1004) ph        (1004)    22831 2023-05-15 04:53:37.000000 OmniEvent-0.1.6/OmniEvent.egg-info/PKG-INFO
--rw-rw-r--   0 ph        (1004) ph        (1004)     1473 2023-05-15 04:53:37.000000 OmniEvent-0.1.6/OmniEvent.egg-info/SOURCES.txt
--rw-rw-r--   0 ph        (1004) ph        (1004)        1 2023-05-15 04:53:37.000000 OmniEvent-0.1.6/OmniEvent.egg-info/dependency_links.txt
--rw-rw-r--   0 ph        (1004) ph        (1004)      153 2023-05-15 04:53:37.000000 OmniEvent-0.1.6/OmniEvent.egg-info/requires.txt
--rw-rw-r--   0 ph        (1004) ph        (1004)       10 2023-05-15 04:53:37.000000 OmniEvent-0.1.6/OmniEvent.egg-info/top_level.txt
--rw-rw-r--   0 ph        (1004) ph        (1004)    22831 2023-05-15 04:53:37.590532 OmniEvent-0.1.6/PKG-INFO
--rw-rw-r--   0 ph        (1004) ph        (1004)    21269 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/README.md
--rw-rw-r--   0 ph        (1004) ph        (1004)      926 2023-05-15 04:52:34.000000 OmniEvent-0.1.6/pyproject.toml
--rw-rw-r--   0 ph        (1004) ph        (1004)       38 2023-05-15 04:53:37.590532 OmniEvent-0.1.6/setup.cfg
-drwxrwsr-x   0 ph        (1004) ph        (1004)        0 2023-05-15 04:53:37.590532 OmniEvent-0.1.6/tests/
--rw-rw-r--   0 ph        (1004) ph        (1004)      780 2023-05-15 04:26:00.000000 OmniEvent-0.1.6/tests/test_infer.py
+drwxrwsr-x   0 ph        (1004) ph        (1004)        0 2023-07-19 06:30:30.623780 OmniEvent-0.1.7/
+-rw-rw-r--   0 ph        (1004) ph        (1004)     1049 2023-05-15 04:26:00.000000 OmniEvent-0.1.7/LICENSE
+drwxrwsr-x   0 ph        (1004) ph        (1004)        0 2023-07-19 06:30:30.575781 OmniEvent-0.1.7/OmniEvent/
+-rw-rw-r--   0 ph        (1004) ph        (1004)        0 2023-05-15 04:26:00.000000 OmniEvent-0.1.7/OmniEvent/__init__.py
+drwxrwsr-x   0 ph        (1004) ph        (1004)        0 2023-07-19 06:30:30.575781 OmniEvent-0.1.7/OmniEvent/aggregation/
+-rw-rw-r--   0 ph        (1004) ph        (1004)        0 2023-05-15 04:26:00.000000 OmniEvent-0.1.7/OmniEvent/aggregation/__init__.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)    20012 2023-05-15 04:26:00.000000 OmniEvent-0.1.7/OmniEvent/aggregation/aggregation.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)    13142 2023-05-15 04:26:00.000000 OmniEvent-0.1.7/OmniEvent/arguments.py
+drwxrwsr-x   0 ph        (1004) ph        (1004)        0 2023-07-19 06:30:30.579781 OmniEvent-0.1.7/OmniEvent/backbone/
+-rw-rw-r--   0 ph        (1004) ph        (1004)        0 2023-05-15 04:26:00.000000 OmniEvent-0.1.7/OmniEvent/backbone/__init__.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)    14972 2023-05-15 04:26:00.000000 OmniEvent-0.1.7/OmniEvent/backbone/backbone.py
+drwxrwsr-x   0 ph        (1004) ph        (1004)        0 2023-07-19 06:30:30.579781 OmniEvent-0.1.7/OmniEvent/evaluation/
+-rw-rw-r--   0 ph        (1004) ph        (1004)        0 2023-05-15 04:26:00.000000 OmniEvent-0.1.7/OmniEvent/evaluation/__init__.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)    27628 2023-05-15 04:26:00.000000 OmniEvent-0.1.7/OmniEvent/evaluation/convert_format.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)    15442 2023-05-15 04:26:00.000000 OmniEvent-0.1.7/OmniEvent/evaluation/dump_result.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)    18870 2023-05-15 04:26:00.000000 OmniEvent-0.1.7/OmniEvent/evaluation/metric.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)    20868 2023-05-15 04:26:00.000000 OmniEvent-0.1.7/OmniEvent/evaluation/utils.py
+drwxrwsr-x   0 ph        (1004) ph        (1004)        0 2023-07-19 06:30:30.587781 OmniEvent-0.1.7/OmniEvent/head/
+-rw-rw-r--   0 ph        (1004) ph        (1004)        0 2023-05-15 04:26:00.000000 OmniEvent-0.1.7/OmniEvent/head/__init__.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)     2297 2023-05-15 04:26:00.000000 OmniEvent-0.1.7/OmniEvent/head/classification.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)    13128 2023-05-15 04:26:00.000000 OmniEvent-0.1.7/OmniEvent/head/crf.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)      508 2023-05-15 04:26:00.000000 OmniEvent-0.1.7/OmniEvent/head/head.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)     5362 2023-07-19 06:15:33.000000 OmniEvent-0.1.7/OmniEvent/infer.py
+drwxrwsr-x   0 ph        (1004) ph        (1004)        0 2023-07-19 06:30:30.611780 OmniEvent-0.1.7/OmniEvent/infer_module/
+-rw-rw-r--   0 ph        (1004) ph        (1004)        0 2023-05-15 04:26:00.000000 OmniEvent-0.1.7/OmniEvent/infer_module/__init__.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)     1755 2023-05-15 04:26:00.000000 OmniEvent-0.1.7/OmniEvent/infer_module/io_format.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)     9839 2023-07-19 06:16:02.000000 OmniEvent-0.1.7/OmniEvent/infer_module/seq2seq.py
+drwxrwsr-x   0 ph        (1004) ph        (1004)        0 2023-07-19 06:30:30.611780 OmniEvent-0.1.7/OmniEvent/input_engineering/
+-rw-rw-r--   0 ph        (1004) ph        (1004)        0 2023-05-15 04:26:00.000000 OmniEvent-0.1.7/OmniEvent/input_engineering/__init__.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)    21674 2023-05-15 04:26:00.000000 OmniEvent-0.1.7/OmniEvent/input_engineering/base_processor.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)    18195 2023-05-15 04:26:00.000000 OmniEvent-0.1.7/OmniEvent/input_engineering/input_utils.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)    11310 2023-05-15 04:26:00.000000 OmniEvent-0.1.7/OmniEvent/input_engineering/mrc_converter.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)    20815 2023-05-15 04:26:00.000000 OmniEvent-0.1.7/OmniEvent/input_engineering/mrc_processor.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)    14875 2023-05-15 04:26:00.000000 OmniEvent-0.1.7/OmniEvent/input_engineering/seq2seq_processor.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)    13751 2023-05-15 04:26:00.000000 OmniEvent-0.1.7/OmniEvent/input_engineering/sequence_labeling_processor.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)    18459 2023-05-15 04:26:00.000000 OmniEvent-0.1.7/OmniEvent/input_engineering/token_classification_processor.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)    11756 2023-05-15 04:26:00.000000 OmniEvent-0.1.7/OmniEvent/input_engineering/tokenizer.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)    12996 2023-05-15 04:26:00.000000 OmniEvent-0.1.7/OmniEvent/input_engineering/whitespace_tokenizer.py
+drwxrwsr-x   0 ph        (1004) ph        (1004)        0 2023-07-19 06:30:30.611780 OmniEvent-0.1.7/OmniEvent/model/
+-rw-rw-r--   0 ph        (1004) ph        (1004)        0 2023-05-15 04:26:00.000000 OmniEvent-0.1.7/OmniEvent/model/__init__.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)    12627 2023-05-15 04:26:00.000000 OmniEvent-0.1.7/OmniEvent/model/constraint_decoding.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)     2342 2023-05-15 04:26:00.000000 OmniEvent-0.1.7/OmniEvent/model/label_smoother_sum.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)    12488 2023-05-15 04:26:00.000000 OmniEvent-0.1.7/OmniEvent/model/model.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)    10211 2023-05-15 04:26:00.000000 OmniEvent-0.1.7/OmniEvent/trainer.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)    18172 2023-05-15 04:26:00.000000 OmniEvent-0.1.7/OmniEvent/trainer_seq2seq.py
+-rw-rw-r--   0 ph        (1004) ph        (1004)     2300 2023-05-15 04:26:00.000000 OmniEvent-0.1.7/OmniEvent/utils.py
+drwxrwsr-x   0 ph        (1004) ph        (1004)        0 2023-07-19 06:30:30.575781 OmniEvent-0.1.7/OmniEvent.egg-info/
+-rw-rw-r--   0 ph        (1004) ph        (1004)    22831 2023-07-19 06:30:30.000000 OmniEvent-0.1.7/OmniEvent.egg-info/PKG-INFO
+-rw-rw-r--   0 ph        (1004) ph        (1004)     1473 2023-07-19 06:30:30.000000 OmniEvent-0.1.7/OmniEvent.egg-info/SOURCES.txt
+-rw-rw-r--   0 ph        (1004) ph        (1004)        1 2023-07-19 06:30:30.000000 OmniEvent-0.1.7/OmniEvent.egg-info/dependency_links.txt
+-rw-rw-r--   0 ph        (1004) ph        (1004)      153 2023-07-19 06:30:30.000000 OmniEvent-0.1.7/OmniEvent.egg-info/requires.txt
+-rw-rw-r--   0 ph        (1004) ph        (1004)       10 2023-07-19 06:30:30.000000 OmniEvent-0.1.7/OmniEvent.egg-info/top_level.txt
+-rw-rw-r--   0 ph        (1004) ph        (1004)    22831 2023-07-19 06:30:30.623780 OmniEvent-0.1.7/PKG-INFO
+-rw-rw-r--   0 ph        (1004) ph        (1004)    21269 2023-07-19 06:28:52.000000 OmniEvent-0.1.7/README.md
+-rw-rw-r--   0 ph        (1004) ph        (1004)      926 2023-07-19 06:28:57.000000 OmniEvent-0.1.7/pyproject.toml
+-rw-rw-r--   0 ph        (1004) ph        (1004)       38 2023-07-19 06:30:30.623780 OmniEvent-0.1.7/setup.cfg
+drwxrwsr-x   0 ph        (1004) ph        (1004)        0 2023-07-19 06:30:30.615780 OmniEvent-0.1.7/tests/
+-rw-rw-r--   0 ph        (1004) ph        (1004)      780 2023-05-15 04:26:00.000000 OmniEvent-0.1.7/tests/test_infer.py
```

### Comparing `OmniEvent-0.1.6/LICENSE` & `OmniEvent-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `OmniEvent-0.1.6/OmniEvent/aggregation/aggregation.py` & `OmniEvent-0.1.7/OmniEvent/aggregation/aggregation.py`

 * *Files identical despite different names*

### Comparing `OmniEvent-0.1.6/OmniEvent/arguments.py` & `OmniEvent-0.1.7/OmniEvent/arguments.py`

 * *Files identical despite different names*

### Comparing `OmniEvent-0.1.6/OmniEvent/backbone/backbone.py` & `OmniEvent-0.1.7/OmniEvent/backbone/backbone.py`

 * *Files identical despite different names*

### Comparing `OmniEvent-0.1.6/OmniEvent/evaluation/convert_format.py` & `OmniEvent-0.1.7/OmniEvent/evaluation/convert_format.py`

 * *Files identical despite different names*

### Comparing `OmniEvent-0.1.6/OmniEvent/evaluation/dump_result.py` & `OmniEvent-0.1.7/OmniEvent/evaluation/dump_result.py`

 * *Files identical despite different names*

### Comparing `OmniEvent-0.1.6/OmniEvent/evaluation/metric.py` & `OmniEvent-0.1.7/OmniEvent/evaluation/metric.py`

 * *Files identical despite different names*

### Comparing `OmniEvent-0.1.6/OmniEvent/evaluation/utils.py` & `OmniEvent-0.1.7/OmniEvent/evaluation/utils.py`

 * *Files identical despite different names*

### Comparing `OmniEvent-0.1.6/OmniEvent/head/classification.py` & `OmniEvent-0.1.7/OmniEvent/head/classification.py`

 * *Files identical despite different names*

### Comparing `OmniEvent-0.1.6/OmniEvent/head/crf.py` & `OmniEvent-0.1.7/OmniEvent/head/crf.py`

 * *Files identical despite different names*

### Comparing `OmniEvent-0.1.6/OmniEvent/infer.py` & `OmniEvent-0.1.7/OmniEvent/infer.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
         results = get_ed_result([text], events)
     elif task == "EAE":
         if model is None or tokenizer is None:
             eae_model, eae_tokenizer = get_pretrained("s2s-mt5-eae", device)
         else:
             eae_model, eae_tokenizer = model, tokenizer
         instances = prepare_for_eae_from_input([text], [triggers], [schema])
-        arguments = do_event_argument_extraction(eae_model, eae_tokenizer, instances)
+        arguments = do_event_argument_extraction(eae_model, eae_tokenizer, instances, device)
         results = get_eae_result(instances, arguments)
     elif task == "EE":
         if model is None or tokenizer is None:
             ed_model, ed_tokenizer = get_pretrained("s2s-mt5-ed", device)
             eae_model, eae_tokenizer = get_pretrained("s2s-mt5-eae", device)
         else:
             ed_model, ed_tokenizer = model[0], tokenizer[0]
```

### Comparing `OmniEvent-0.1.6/OmniEvent/infer_module/io_format.py` & `OmniEvent-0.1.7/OmniEvent/infer_module/io_format.py`

 * *Files identical despite different names*

### Comparing `OmniEvent-0.1.6/OmniEvent/infer_module/seq2seq.py` & `OmniEvent-0.1.7/OmniEvent/infer_module/seq2seq.py`

 * *Files 1% similar despite different names*

```diff
@@ -263,15 +263,15 @@
     pred_triggers = []
     for i, pred in enumerate(decoded_preds):
         pred = clean_str(pred)
         pred_triggers.extend(extract_argument(pred, i))
     return pred_triggers
 
 
-def do_event_argument_extraction(model, tokenizer, instances, device):
+def do_event_argument_extraction(model, tokenizer, instances, device="cuda"):
     data_processor = EAEProcessor(tokenizer)
     inputs = data_processor.tokenize(instances, device)
     decoded_preds = generate(model, tokenizer, inputs)
     def clean_str(x_str):
         for to_remove_token in [tokenizer.eos_token, tokenizer.pad_token]:
             x_str = x_str.replace(to_remove_token, '')
         return x_str.strip()
```

### Comparing `OmniEvent-0.1.6/OmniEvent/input_engineering/base_processor.py` & `OmniEvent-0.1.7/OmniEvent/input_engineering/base_processor.py`

 * *Files identical despite different names*

### Comparing `OmniEvent-0.1.6/OmniEvent/input_engineering/input_utils.py` & `OmniEvent-0.1.7/OmniEvent/input_engineering/input_utils.py`

 * *Files identical despite different names*

### Comparing `OmniEvent-0.1.6/OmniEvent/input_engineering/mrc_converter.py` & `OmniEvent-0.1.7/OmniEvent/input_engineering/mrc_converter.py`

 * *Files identical despite different names*

### Comparing `OmniEvent-0.1.6/OmniEvent/input_engineering/mrc_processor.py` & `OmniEvent-0.1.7/OmniEvent/input_engineering/mrc_processor.py`

 * *Files identical despite different names*

### Comparing `OmniEvent-0.1.6/OmniEvent/input_engineering/seq2seq_processor.py` & `OmniEvent-0.1.7/OmniEvent/input_engineering/seq2seq_processor.py`

 * *Files identical despite different names*

### Comparing `OmniEvent-0.1.6/OmniEvent/input_engineering/sequence_labeling_processor.py` & `OmniEvent-0.1.7/OmniEvent/input_engineering/sequence_labeling_processor.py`

 * *Files identical despite different names*

### Comparing `OmniEvent-0.1.6/OmniEvent/input_engineering/token_classification_processor.py` & `OmniEvent-0.1.7/OmniEvent/input_engineering/token_classification_processor.py`

 * *Files identical despite different names*

### Comparing `OmniEvent-0.1.6/OmniEvent/input_engineering/tokenizer.py` & `OmniEvent-0.1.7/OmniEvent/input_engineering/tokenizer.py`

 * *Files identical despite different names*

### Comparing `OmniEvent-0.1.6/OmniEvent/input_engineering/whitespace_tokenizer.py` & `OmniEvent-0.1.7/OmniEvent/input_engineering/whitespace_tokenizer.py`

 * *Files identical despite different names*

### Comparing `OmniEvent-0.1.6/OmniEvent/model/constraint_decoding.py` & `OmniEvent-0.1.7/OmniEvent/model/constraint_decoding.py`

 * *Files identical despite different names*

### Comparing `OmniEvent-0.1.6/OmniEvent/model/label_smoother_sum.py` & `OmniEvent-0.1.7/OmniEvent/model/label_smoother_sum.py`

 * *Files identical despite different names*

### Comparing `OmniEvent-0.1.6/OmniEvent/model/model.py` & `OmniEvent-0.1.7/OmniEvent/model/model.py`

 * *Files identical despite different names*

### Comparing `OmniEvent-0.1.6/OmniEvent/trainer.py` & `OmniEvent-0.1.7/OmniEvent/trainer.py`

 * *Files identical despite different names*

### Comparing `OmniEvent-0.1.6/OmniEvent/trainer_seq2seq.py` & `OmniEvent-0.1.7/OmniEvent/trainer_seq2seq.py`

 * *Files identical despite different names*

### Comparing `OmniEvent-0.1.6/OmniEvent/utils.py` & `OmniEvent-0.1.7/OmniEvent/utils.py`

 * *Files identical despite different names*

### Comparing `OmniEvent-0.1.6/OmniEvent.egg-info/PKG-INFO` & `OmniEvent-0.1.7/OmniEvent.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OmniEvent
-Version: 0.1.6
+Version: 0.1.7
 Summary: A tookit for event extraction.
 License: Copyright (c) 2022 THUKEG
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
@@ -27,15 +27,15 @@
 ------
 
 <p align="center">  
     <a href="http://103.238.162.34:9621/">
         <img alt="Demo" src="https://img.shields.io/badge/Demo-site-green">
     </a>
     <a href="https://pypi.org/project/OmniEvent/">
-        <img alt="PyPI" src="https://img.shields.io/badge/Pypi-v.0.1.1-blue">
+        <img alt="PyPI" src="https://img.shields.io/badge/Pypi-v.0.1.7-blue">
     </a>
     <a href="https://omnievent.readthedocs.io/en/latest/">
         <img alt="Documentation" src="https://img.shields.io/badge/Doc-site-red">
     </a>
     <a href="https://github.com/THU-KEG/OmniEvent/blob/main/LICENSE">
         <img alt="License" src="https://img.shields.io/badge/License-MIT-blue">
     </a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: OmniEvent Version: 0.1.6 Summary: A tookit for
+Metadata-Version: 2.1 Name: OmniEvent Version: 0.1.7 Summary: A tookit for
 event extraction. License: Copyright (c) 2022 THUKEG Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions: The above copyright notice and this
```

### Comparing `OmniEvent-0.1.6/OmniEvent.egg-info/SOURCES.txt` & `OmniEvent-0.1.7/OmniEvent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OmniEvent-0.1.6/PKG-INFO` & `OmniEvent-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OmniEvent
-Version: 0.1.6
+Version: 0.1.7
 Summary: A tookit for event extraction.
 License: Copyright (c) 2022 THUKEG
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
@@ -27,15 +27,15 @@
 ------
 
 <p align="center">  
     <a href="http://103.238.162.34:9621/">
         <img alt="Demo" src="https://img.shields.io/badge/Demo-site-green">
     </a>
     <a href="https://pypi.org/project/OmniEvent/">
-        <img alt="PyPI" src="https://img.shields.io/badge/Pypi-v.0.1.1-blue">
+        <img alt="PyPI" src="https://img.shields.io/badge/Pypi-v.0.1.7-blue">
     </a>
     <a href="https://omnievent.readthedocs.io/en/latest/">
         <img alt="Documentation" src="https://img.shields.io/badge/Doc-site-red">
     </a>
     <a href="https://github.com/THU-KEG/OmniEvent/blob/main/LICENSE">
         <img alt="License" src="https://img.shields.io/badge/License-MIT-blue">
     </a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: OmniEvent Version: 0.1.6 Summary: A tookit for
+Metadata-Version: 2.1 Name: OmniEvent Version: 0.1.7 Summary: A tookit for
 event extraction. License: Copyright (c) 2022 THUKEG Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions: The above copyright notice and this
```

### Comparing `OmniEvent-0.1.6/README.md` & `OmniEvent-0.1.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ------
 
 <p align="center">  
     <a href="http://103.238.162.34:9621/">
         <img alt="Demo" src="https://img.shields.io/badge/Demo-site-green">
     </a>
     <a href="https://pypi.org/project/OmniEvent/">
-        <img alt="PyPI" src="https://img.shields.io/badge/Pypi-v.0.1.1-blue">
+        <img alt="PyPI" src="https://img.shields.io/badge/Pypi-v.0.1.7-blue">
     </a>
     <a href="https://omnievent.readthedocs.io/en/latest/">
         <img alt="Documentation" src="https://img.shields.io/badge/Doc-site-red">
     </a>
     <a href="https://github.com/THU-KEG/OmniEvent/blob/main/LICENSE">
         <img alt="License" src="https://img.shields.io/badge/License-MIT-blue">
     </a>
```

### Comparing `OmniEvent-0.1.6/pyproject.toml` & `OmniEvent-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "OmniEvent.input_engineering",
     "OmniEvent.model"
 ]
 
 
 [project]
 name = "OmniEvent"
-version = "0.1.6"
+version = "0.1.7"
 description = "A tookit for event extraction."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `OmniEvent-0.1.6/tests/test_infer.py` & `OmniEvent-0.1.7/tests/test_infer.py`

 * *Files identical despite different names*

