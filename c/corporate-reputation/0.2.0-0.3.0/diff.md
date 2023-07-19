# Comparing `tmp/corporate_reputation-0.2.0.tar.gz` & `tmp/corporate_reputation-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corporate_reputation-0.2.0.tar", max compression
+gzip compressed data, was "corporate_reputation-0.3.0.tar", max compression
```

## Comparing `corporate_reputation-0.2.0.tar` & `corporate_reputation-0.3.0.tar`

### file list

```diff
@@ -1,59 +1,66 @@
--rw-r--r--   0        0        0     1071 2023-07-17 20:56:16.198169 corporate_reputation-0.2.0/LICENSE
--rw-r--r--   0        0        0     3912 2023-07-17 20:56:16.198169 corporate_reputation-0.2.0/README.md
--rw-r--r--   0        0        0     3050 2023-07-17 20:56:47.606474 corporate_reputation-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      288 2023-07-17 20:56:16.198169 corporate_reputation-0.2.0/src/corprep/__cli__.py
--rw-r--r--   0        0        0      379 2023-07-17 20:56:16.198169 corporate_reputation-0.2.0/src/corprep/__init__.py
--rw-r--r--   0        0        0       22 2023-07-17 20:56:47.554474 corporate_reputation-0.2.0/src/corprep/_version.py
--rw-r--r--   0        0        0        0 2023-07-17 20:56:16.198169 corporate_reputation-0.2.0/src/corprep/conf/__init__.py
--rw-r--r--   0        0        0      338 2023-07-17 20:56:47.554474 corporate_reputation-0.2.0/src/corprep/conf/about/__init__.yaml
--rw-r--r--   0        0        0      588 2023-07-17 20:56:16.198169 corporate_reputation-0.2.0/src/corprep/conf/batch/__init__.yaml
--rw-r--r--   0        0        0        0 2023-07-17 20:56:16.198169 corporate_reputation-0.2.0/src/corprep/conf/cmd/__init__.yaml
--rw-r--r--   0        0        0       49 2023-07-17 20:56:16.198169 corporate_reputation-0.2.0/src/corprep/conf/cmd/about.yaml
--rw-r--r--   0        0        0      155 2023-07-17 20:56:16.198169 corporate_reputation-0.2.0/src/corprep/conf/cmd/copy_conf.yaml
--rw-r--r--   0        0        0       83 2023-07-17 20:56:16.198169 corporate_reputation-0.2.0/src/corprep/conf/cmd/run_task.yaml
--rw-r--r--   0        0        0       91 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/cmd/run_workflow.yaml
--rw-r--r--   0        0        0      328 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/config.yaml
--rw-r--r--   0        0        0      569 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/copier/conf.yaml
--rw-r--r--   0        0        0      709 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      322 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      137 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      198 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/mode/__debug__.yaml
--rw-r--r--   0        0        0      926 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/mode/__init__.yaml
--rw-r--r--   0        0        0       61 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/module/__init__.yaml
--rw-r--r--   0        0        0       72 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      846 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/path/__init__.yaml
--rw-r--r--   0        0        0       91 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/path/__task__.yaml
--rw-r--r--   0        0        0      286 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/path/dirnames/__init__.yaml
--rw-r--r--   0        0        0       76 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/pipe/__dataframe__.yaml
--rw-r--r--   0        0        0       77 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/pipe/__dataframe_external_funcs__.yaml
--rw-r--r--   0        0        0       79 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/pipe/__dataframe_instance_methods__.yaml
--rw-r--r--   0        0        0       70 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/pipe/__general_external_funcs__.yaml
--rw-r--r--   0        0        0       72 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/pipe/__general_instance_methods__.yaml
--rw-r--r--   0        0        0      128 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/pipe/__init__.yaml
--rw-r--r--   0        0        0      236 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/pipe/load_dataframes.yaml
--rw-r--r--   0        0        0      105 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/pipe/load_raw_dataset.yaml
--rw-r--r--   0        0        0      241 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/pipe/save_dataframes.yaml
--rw-r--r--   0        0        0       88 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/pipe/save_dataset.yaml
--rw-r--r--   0        0        0       90 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/pipe/test_preprocessing.yaml
--rw-r--r--   0        0        0       69 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/pipeline/__init__.yaml
--rw-r--r--   0        0        0      388 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/pipeline/__test__.yaml
--rw-r--r--   0        0        0      387 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/pipeline/__test_dataframe__.yaml
--rw-r--r--   0        0        0      268 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/pipeline/__test_general__.yaml
--rw-r--r--   0        0        0      377 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/pipeline/datasets.yaml
--rw-r--r--   0        0        0      746 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/project/__init__.yaml
--rw-r--r--   0        0        0      193 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/project/__test__.yaml
--rw-r--r--   0        0        0      221 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/project/corprep.yaml
--rw-r--r--   0        0        0       38 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/running/__init__.yaml
--rw-r--r--   0        0        0      142 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/task/__batch__.yaml
--rw-r--r--   0        0        0      329 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/task/__init__.yaml
--rw-r--r--   0        0        0      183 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/task/__test__.yaml
--rw-r--r--   0        0        0      145 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/task/datasets.yaml
--rw-r--r--   0        0        0      124 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/workflow/__init__.yaml
--rw-r--r--   0        0        0      148 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/workflow/__test__.yaml
--rw-r--r--   0        0        0      150 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/conf/workflow/corprep.yaml
--rw-r--r--   0        0        0      204 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/datasets/__init__.py
--rw-r--r--   0        0        0      872 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/datasets/raw.py
--rw-r--r--   0        0        0        0 2023-07-17 20:56:16.202169 corporate_reputation-0.2.0/src/corprep/py.typed
--rw-r--r--   0        0        0     4698 1970-01-01 00:00:00.000000 corporate_reputation-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-19 09:32:35.022802 corporate_reputation-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3912 2023-07-19 09:32:35.022802 corporate_reputation-0.3.0/README.md
+-rw-r--r--   0        0        0     3088 2023-07-19 09:33:12.842210 corporate_reputation-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      288 2023-07-19 09:32:35.026803 corporate_reputation-0.3.0/src/corprep/__cli__.py
+-rw-r--r--   0        0        0      363 2023-07-19 09:32:35.026803 corporate_reputation-0.3.0/src/corprep/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-19 09:33:12.782205 corporate_reputation-0.3.0/src/corprep/_version.py
+-rw-r--r--   0        0        0        0 2023-07-19 09:32:35.026803 corporate_reputation-0.3.0/src/corprep/absa/__init__.py
+-rw-r--r--   0        0        0     1754 2023-07-19 09:32:35.026803 corporate_reputation-0.3.0/src/corprep/absa/agent.py
+-rw-r--r--   0        0        0     3667 2023-07-19 09:32:35.026803 corporate_reputation-0.3.0/src/corprep/absa/config.py
+-rw-r--r--   0        0        0        0 2023-07-19 09:32:35.026803 corporate_reputation-0.3.0/src/corprep/conf/__init__.py
+-rw-r--r--   0        0        0      338 2023-07-19 09:33:12.782205 corporate_reputation-0.3.0/src/corprep/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      299 2023-07-19 09:32:35.026803 corporate_reputation-0.3.0/src/corprep/conf/absa/default.yaml
+-rw-r--r--   0        0        0     2930 2023-07-19 09:32:35.026803 corporate_reputation-0.3.0/src/corprep/conf/absa/prompts/default.yaml
+-rw-r--r--   0        0        0      588 2023-07-19 09:32:35.026803 corporate_reputation-0.3.0/src/corprep/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0        0 2023-07-19 09:32:35.026803 corporate_reputation-0.3.0/src/corprep/conf/cmd/__init__.yaml
+-rw-r--r--   0        0        0       49 2023-07-19 09:32:35.026803 corporate_reputation-0.3.0/src/corprep/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      159 2023-07-19 09:32:35.026803 corporate_reputation-0.3.0/src/corprep/conf/cmd/copy_conf.yaml
+-rw-r--r--   0        0        0       83 2023-07-19 09:32:35.026803 corporate_reputation-0.3.0/src/corprep/conf/cmd/run_task.yaml
+-rw-r--r--   0        0        0       91 2023-07-19 09:32:35.026803 corporate_reputation-0.3.0/src/corprep/conf/cmd/run_workflow.yaml
+-rw-r--r--   0        0        0      328 2023-07-19 09:32:35.026803 corporate_reputation-0.3.0/src/corprep/conf/config.yaml
+-rw-r--r--   0        0        0      662 2023-07-19 09:32:35.026803 corporate_reputation-0.3.0/src/corprep/conf/copier/__init__.yaml
+-rw-r--r--   0        0        0      709 2023-07-19 09:32:35.026803 corporate_reputation-0.3.0/src/corprep/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      322 2023-07-19 09:32:35.026803 corporate_reputation-0.3.0/src/corprep/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-07-19 09:32:35.026803 corporate_reputation-0.3.0/src/corprep/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-07-19 09:32:35.026803 corporate_reputation-0.3.0/src/corprep/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      137 2023-07-19 09:32:35.026803 corporate_reputation-0.3.0/src/corprep/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      198 2023-07-19 09:32:35.026803 corporate_reputation-0.3.0/src/corprep/conf/mode/__debug__.yaml
+-rw-r--r--   0        0        0      926 2023-07-19 09:32:35.026803 corporate_reputation-0.3.0/src/corprep/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0       61 2023-07-19 09:32:35.026803 corporate_reputation-0.3.0/src/corprep/conf/module/__init__.yaml
+-rw-r--r--   0        0        0       72 2023-07-19 09:32:35.026803 corporate_reputation-0.3.0/src/corprep/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      846 2023-07-19 09:32:35.026803 corporate_reputation-0.3.0/src/corprep/conf/path/__init__.yaml
+-rw-r--r--   0        0        0       91 2023-07-19 09:32:35.026803 corporate_reputation-0.3.0/src/corprep/conf/path/__task__.yaml
+-rw-r--r--   0        0        0      286 2023-07-19 09:32:35.026803 corporate_reputation-0.3.0/src/corprep/conf/path/dirnames/__init__.yaml
+-rw-r--r--   0        0        0       76 2023-07-19 09:32:35.026803 corporate_reputation-0.3.0/src/corprep/conf/pipe/__dataframe__.yaml
+-rw-r--r--   0        0        0       77 2023-07-19 09:32:35.030803 corporate_reputation-0.3.0/src/corprep/conf/pipe/__dataframe_external_funcs__.yaml
+-rw-r--r--   0        0        0       79 2023-07-19 09:32:35.030803 corporate_reputation-0.3.0/src/corprep/conf/pipe/__dataframe_instance_methods__.yaml
+-rw-r--r--   0        0        0       70 2023-07-19 09:32:35.030803 corporate_reputation-0.3.0/src/corprep/conf/pipe/__general_external_funcs__.yaml
+-rw-r--r--   0        0        0       72 2023-07-19 09:32:35.030803 corporate_reputation-0.3.0/src/corprep/conf/pipe/__general_instance_methods__.yaml
+-rw-r--r--   0        0        0      424 2023-07-19 09:32:35.030803 corporate_reputation-0.3.0/src/corprep/conf/pipe/__init__.yaml
+-rw-r--r--   0        0        0      294 2023-07-19 09:32:35.030803 corporate_reputation-0.3.0/src/corprep/conf/pipe/absa_agent_predict.yaml
+-rw-r--r--   0        0        0      274 2023-07-19 09:32:35.030803 corporate_reputation-0.3.0/src/corprep/conf/pipe/dataset_filter.yaml
+-rw-r--r--   0        0        0      150 2023-07-19 09:32:35.030803 corporate_reputation-0.3.0/src/corprep/conf/pipe/dataset_load.yaml
+-rw-r--r--   0        0        0      163 2023-07-19 09:32:35.030803 corporate_reputation-0.3.0/src/corprep/conf/pipe/dataset_load_raw.yaml
+-rw-r--r--   0        0        0      218 2023-07-19 09:32:35.030803 corporate_reputation-0.3.0/src/corprep/conf/pipe/dataset_sample.yaml
+-rw-r--r--   0        0        0      106 2023-07-19 09:32:35.030803 corporate_reputation-0.3.0/src/corprep/conf/pipe/dataset_save.yaml
+-rw-r--r--   0        0        0      217 2023-07-19 09:32:35.030803 corporate_reputation-0.3.0/src/corprep/conf/pipe/dataset_tokenize.yaml
+-rw-r--r--   0        0        0       69 2023-07-19 09:32:35.030803 corporate_reputation-0.3.0/src/corprep/conf/pipeline/__init__.yaml
+-rw-r--r--   0        0        0      388 2023-07-19 09:32:35.030803 corporate_reputation-0.3.0/src/corprep/conf/pipeline/__test__.yaml
+-rw-r--r--   0        0        0      642 2023-07-19 09:32:35.030803 corporate_reputation-0.3.0/src/corprep/conf/pipeline/absa-kakao.yaml
+-rw-r--r--   0        0        0      677 2023-07-19 09:32:35.030803 corporate_reputation-0.3.0/src/corprep/conf/pipeline/datasets-daum.yaml
+-rw-r--r--   0        0        0      622 2023-07-19 09:32:35.030803 corporate_reputation-0.3.0/src/corprep/conf/pipeline/datasets-kakao.yaml
+-rw-r--r--   0        0        0      746 2023-07-19 09:32:35.030803 corporate_reputation-0.3.0/src/corprep/conf/project/__init__.yaml
+-rw-r--r--   0        0        0      221 2023-07-19 09:32:35.030803 corporate_reputation-0.3.0/src/corprep/conf/project/corprep.yaml
+-rw-r--r--   0        0        0       38 2023-07-19 09:32:35.030803 corporate_reputation-0.3.0/src/corprep/conf/running/__init__.yaml
+-rw-r--r--   0        0        0      142 2023-07-19 09:32:35.030803 corporate_reputation-0.3.0/src/corprep/conf/task/__batch__.yaml
+-rw-r--r--   0        0        0      329 2023-07-19 09:32:35.030803 corporate_reputation-0.3.0/src/corprep/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      143 2023-07-19 09:32:35.030803 corporate_reputation-0.3.0/src/corprep/conf/task/absa.yaml
+-rw-r--r--   0        0        0      151 2023-07-19 09:32:35.030803 corporate_reputation-0.3.0/src/corprep/conf/task/datasets.yaml
+-rw-r--r--   0        0        0      124 2023-07-19 09:32:35.030803 corporate_reputation-0.3.0/src/corprep/conf/workflow/__init__.yaml
+-rw-r--r--   0        0        0      192 2023-07-19 09:32:35.030803 corporate_reputation-0.3.0/src/corprep/conf/workflow/corprep.yaml
+-rw-r--r--   0        0        0      204 2023-07-19 09:32:35.030803 corporate_reputation-0.3.0/src/corprep/datasets/__init__.py
+-rw-r--r--   0        0        0     1609 2023-07-19 09:32:35.030803 corporate_reputation-0.3.0/src/corprep/datasets/io.py
+-rw-r--r--   0        0        0      617 2023-07-19 09:32:35.030803 corporate_reputation-0.3.0/src/corprep/datasets/sample.py
+-rw-r--r--   0        0        0      843 2023-07-19 09:32:35.030803 corporate_reputation-0.3.0/src/corprep/datasets/tokenize.py
+-rw-r--r--   0        0        0        0 2023-07-19 09:32:35.030803 corporate_reputation-0.3.0/src/corprep/py.typed
+-rw-r--r--   0        0        0     4779 1970-01-01 00:00:00.000000 corporate_reputation-0.3.0/PKG-INFO
```

### Comparing `corporate_reputation-0.2.0/LICENSE` & `corporate_reputation-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `corporate_reputation-0.2.0/README.md` & `corporate_reputation-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `corporate_reputation-0.2.0/pyproject.toml` & `corporate_reputation-0.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 [tool.poetry]
 name = "corporate-reputation"
-version = "0.2.0"
+version = "0.3.0"
 description = "Unraveling Corporate and CEO Reputation using Aspect-Based Sentiment Analysis and Signal Modeling"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://entelecheia.github.io/corporate-reputation"
 repository = "https://github.com/entelecheia/corporate-reputation"
 readme = "README.md"
 packages = [{ include = "corprep", from = "src" }]
 
 [tool.poetry.scripts]
 corprep = 'corprep.__cli__:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
-hyfi = "^1.2.13"
+hyfi = "^1.2.14"
 ekonlpy = "^1.1.7"
+openai = "^0.27.8"
+backoff = "^2.2.1"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
 isort = "^5.12.0"
```

### Comparing `corporate_reputation-0.2.0/src/corprep/conf/batch/__init__.yaml` & `corporate_reputation-0.3.0/src/corprep/conf/batch/__init__.yaml`

 * *Files identical despite different names*

### Comparing `corporate_reputation-0.2.0/src/corprep/conf/copier/conf.yaml` & `corporate_reputation-0.3.0/src/corprep/conf/copier/__init__.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 # Filetypes to copy.
 filetypes:
   - yaml
   - yml
   - py
 # User-chosen additional file exclusion patterns.
 exclude:
-# User-chosen additional file skip patterns.
+# If `True`, exclude files that match the patterns for testing. (default: True)
+exclude_test_files: true
+# Skip files that already exist?
 skip_if_exists: false
 # Delete `dst_path` if there's an error?
 cleanup_on_error: false
 # When `True`, Overwrite files that already exist, without asking.
 overwrite: false
 # When `True`, produce no real rendering.
 dry_run: false
```

### Comparing `corporate_reputation-0.2.0/src/corprep/conf/dotenv/__init__.yaml` & `corporate_reputation-0.3.0/src/corprep/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `corporate_reputation-0.2.0/src/corprep/conf/hydra/help/help.yaml` & `corporate_reputation-0.3.0/src/corprep/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `corporate_reputation-0.2.0/src/corprep/conf/mode/__init__.yaml` & `corporate_reputation-0.3.0/src/corprep/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `corporate_reputation-0.2.0/src/corprep/conf/path/__init__.yaml` & `corporate_reputation-0.3.0/src/corprep/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `corporate_reputation-0.2.0/src/corprep/conf/project/__init__.yaml` & `corporate_reputation-0.3.0/src/corprep/conf/project/__init__.yaml`

 * *Files identical despite different names*

### Comparing `corporate_reputation-0.2.0/src/corprep/datasets/raw.py` & `corporate_reputation-0.3.0/src/corprep/datasets/io.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,26 +6,61 @@
 from corprep import HyFI  # type: ignore
 
 logger = HyFI.getLogger(__name__)
 
 
 def load_raw_dataset(
     raw_dataset_dir: Union[str, Path],
+    path: str = "json",
+    file_pattern: str = "*.dat",
     verbose: bool = False,
     **kwargs,
 ):
     raw_dataset_dir = Path(raw_dataset_dir)
     raw_data_files = []
     if raw_dataset_dir.exists():
-        raw_data_files = HyFI.get_filepaths(f"{raw_dataset_dir}/*.dat")
+        raw_data_files = HyFI.get_filepaths(f"{raw_dataset_dir}/{file_pattern}")
         logger.info("Found %d raw data files.", len(raw_data_files))
     else:
         logger.warning("No raw data files found.")
         raise FileNotFoundError()
 
-    dataset = HyFI.load_dataset("json", data_files=raw_data_files)
+    dataset = HyFI.load_dataset(path, data_files=raw_data_files)
     ds_train: Dataset = dataset["train"]  # type: ignore
 
-    logger.info("Number of training samples: %d", len(ds_train))
-    logger.info("Dataset features: %s", ds_train.features)
+    logger.info("Number of training samples: %s", len(ds_train))
+    if verbose:
+        print(ds_train[99])
+        print(ds_train[-99])
+        logger.info("Dataset features: %s", ds_train.features)
 
     return ds_train
+
+
+def save_dataset(
+    data: Dataset,
+    dataset_path: Union[str, Path],
+) -> Dataset:
+    """
+    Save a dataset.
+    """
+    data.save_to_disk(dataset_path)
+    logger.info("Dataset saved to %s.", dataset_path)
+
+    return data
+
+
+def load_dataset(
+    dataset_path: str,
+    verbose: bool = False,
+) -> Dataset:
+    """
+    Save a dataset.
+    """
+    data = Dataset.load_from_disk(dataset_path)
+    logger.info("Dataset loaded from %s.", dataset_path)
+    if verbose:
+        print(data[0])
+        print(data[-1])
+        logger.info("Dataset features: %s", data.features)
+
+    return data
```

### Comparing `corporate_reputation-0.2.0/PKG-INFO` & `corporate_reputation-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: corporate-reputation
-Version: 0.2.0
+Version: 0.3.0
 Summary: Unraveling Corporate and CEO Reputation using Aspect-Based Sentiment Analysis and Signal Modeling
 Home-page: https://entelecheia.github.io/corporate-reputation
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: backoff (>=2.2.1,<3.0.0)
 Requires-Dist: ekonlpy (>=1.1.7,<2.0.0)
-Requires-Dist: hyfi (>=1.2.13,<2.0.0)
+Requires-Dist: hyfi (>=1.2.14,<2.0.0)
+Requires-Dist: openai (>=0.27.8,<0.28.0)
 Project-URL: Repository, https://github.com/entelecheia/corporate-reputation
 Description-Content-Type: text/markdown
 
 # Reputation Analysis of Companies and CEOs
 
 [![pypi-image]][pypi-url]
 [![version-image]][release-url]
```

