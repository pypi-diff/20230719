# Comparing `tmp/fun_sentence_splitter-0.2.344.tar.gz` & `tmp/fun_sentence_splitter-0.2.366.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fun_sentence_splitter-0.2.344.tar", max compression
+gzip compressed data, was "fun_sentence_splitter-0.2.366.tar", max compression
```

## Comparing `fun_sentence_splitter-0.2.344.tar` & `fun_sentence_splitter-0.2.366.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1067 2023-07-14 08:44:10.055927 fun_sentence_splitter-0.2.344/LICENSE
--rw-r--r--   0        0        0     1247 2023-07-14 08:44:10.055927 fun_sentence_splitter-0.2.344/README.md
--rw-r--r--   0        0        0       57 2023-07-14 08:44:10.055927 fun_sentence_splitter-0.2.344/fun_sentence_splitter/__init__.py
--rw-r--r--   0        0        0     3383 2023-07-14 08:44:10.055927 fun_sentence_splitter-0.2.344/fun_sentence_splitter/sentence_splitter.py
--rw-r--r--   0        0        0     1423 2023-07-14 08:44:10.055927 fun_sentence_splitter-0.2.344/pyproject.toml
--rw-r--r--   0        0        0     1760 1970-01-01 00:00:00.000000 fun_sentence_splitter-0.2.344/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-19 05:57:41.810358 fun_sentence_splitter-0.2.366/LICENSE
+-rw-r--r--   0        0        0      771 2023-07-19 05:57:41.810358 fun_sentence_splitter-0.2.366/README.md
+-rw-r--r--   0        0        0       57 2023-07-19 05:57:41.810358 fun_sentence_splitter-0.2.366/fun_sentence_splitter/__init__.py
+-rw-r--r--   0        0        0     3383 2023-07-19 05:57:41.810358 fun_sentence_splitter-0.2.366/fun_sentence_splitter/sentence_splitter.py
+-rw-r--r--   0        0        0     1423 2023-07-19 05:57:41.810358 fun_sentence_splitter-0.2.366/pyproject.toml
+-rw-r--r--   0        0        0     1284 1970-01-01 00:00:00.000000 fun_sentence_splitter-0.2.366/PKG-INFO
```

### Comparing `fun_sentence_splitter-0.2.344/LICENSE` & `fun_sentence_splitter-0.2.366/LICENSE`

 * *Files identical despite different names*

### Comparing `fun_sentence_splitter-0.2.344/fun_sentence_splitter/sentence_splitter.py` & `fun_sentence_splitter-0.2.366/fun_sentence_splitter/sentence_splitter.py`

 * *Files identical despite different names*

### Comparing `fun_sentence_splitter-0.2.344/PKG-INFO` & `fun_sentence_splitter-0.2.366/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: fun-sentence-splitter
-Version: 0.2.344
+Version: 0.2.366
 Summary: A fundamental sentence splitter based on spacy.
 License: MIT
 Author: Medical AI Engineering
 Author-email: engineering@m-ai.rhenus.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: spacy (==3.4.4)
+Requires-Dist: spacy (==3.6.0)
 Description-Content-Type: text/markdown
 
 # Fun Sentence Splitter
 
 A fundamental sentence splitter based on [spacy](https://spacy.io/).
 
 ## Requirements
@@ -35,33 +35,16 @@
 ruff .
 mypy .
 pytest --cov=fun_sentence_splitter
 ```
 
 ## Run Evaluation
 
-1. Change the `spacy` dependency in the `pyproject.toml` to the version you want to evaluate and run:
-
-    ```shell
-    poetry lock --no-update
-    poetry install
-    ```
-
-2. Download the Spacy language model you want to evaluate, e.g.:
-
-    ```shell
-    python -m spacy download de_core_news_lg
-    ```
-
-Evaluate:
-
 ```shell
-python -m tests.evaluate_sentence_splitter path/to/splits_dir [--spacy-model de_core_news_lg] [--max-len 47]
+./evaluate.sh path/to/splits_dir
 ```
 
 `path/to/splits_dir`: directory containing pairs of *.split and *.txt files. .split files contain the expected
 sentences, each on a separate line. .txt files contain the original text to split.
 
-`--spacy-model`: name or location of the spacy language model. Optional, defaults to `de_core_news_sm`.
-
-`--max-len`: maximum line length before before spacy is used. Optional, defaults to `100`.
+The evaluation script will automatically update the spacy dependency and download the required language models.
```

