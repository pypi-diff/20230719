# Comparing `tmp/sliceguard-0.0.7.tar.gz` & `tmp/sliceguard-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sliceguard-0.0.7.tar", last modified: Thu Jul 13 09:11:13 2023, max compression
+gzip compressed data, was "sliceguard-0.0.8.tar", last modified: Wed Jul 19 11:05:23 2023, max compression
```

## Comparing `sliceguard-0.0.7.tar` & `sliceguard-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-13 09:11:13.050232 sliceguard-0.0.7/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1065 2023-06-14 07:59:41.000000 sliceguard-0.0.7/LICENSE
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     4146 2023-07-13 09:11:13.050232 sliceguard-0.0.7/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     3491 2023-07-13 08:54:42.000000 sliceguard-0.0.7/README.md
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1064 2023-07-13 08:55:35.000000 sliceguard-0.0.7/pyproject.toml
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-07-13 09:11:13.050232 sliceguard-0.0.7/setup.cfg
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-13 09:11:13.050232 sliceguard-0.0.7/sliceguard/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       44 2023-07-05 08:28:25.000000 sliceguard-0.0.7/sliceguard/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     6129 2023-07-07 08:09:57.000000 sliceguard-0.0.7/sliceguard/detection.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2843 2023-07-11 15:29:58.000000 sliceguard-0.0.7/sliceguard/embedding_utils.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     4378 2023-07-11 15:29:58.000000 sliceguard-0.0.7/sliceguard/explanation.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    10671 2023-07-13 08:54:42.000000 sliceguard-0.0.7/sliceguard/sliceguard.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     8510 2023-07-13 08:54:42.000000 sliceguard-0.0.7/sliceguard/utils.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-13 09:11:13.050232 sliceguard-0.0.7/sliceguard.egg-info/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     4146 2023-07-13 09:11:13.000000 sliceguard-0.0.7/sliceguard.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      374 2023-07-13 09:11:13.000000 sliceguard-0.0.7/sliceguard.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-07-13 09:11:13.000000 sliceguard-0.0.7/sliceguard.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      247 2023-07-13 09:11:13.000000 sliceguard-0.0.7/sliceguard.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       11 2023-07-13 09:11:13.000000 sliceguard-0.0.7/sliceguard.egg-info/top_level.txt
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-13 09:11:13.050232 sliceguard-0.0.7/tests/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     4742 2023-07-11 15:29:58.000000 sliceguard-0.0.7/tests/test_sliceguard.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-19 11:05:23.093813 sliceguard-0.0.8/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1065 2023-06-14 07:59:41.000000 sliceguard-0.0.8/LICENSE
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4245 2023-07-19 11:05:23.093813 sliceguard-0.0.8/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3590 2023-07-19 11:03:05.000000 sliceguard-0.0.8/README.md
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1088 2023-07-19 11:03:35.000000 sliceguard-0.0.8/pyproject.toml
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-07-19 11:05:23.093813 sliceguard-0.0.8/setup.cfg
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-19 11:05:23.093813 sliceguard-0.0.8/sliceguard/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       44 2023-07-05 08:28:25.000000 sliceguard-0.0.8/sliceguard/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    10000 2023-07-19 11:03:05.000000 sliceguard-0.0.8/sliceguard/detection.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4985 2023-07-19 11:03:05.000000 sliceguard-0.0.8/sliceguard/embedding_utils.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4378 2023-07-11 15:29:58.000000 sliceguard-0.0.8/sliceguard/explanation.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    11179 2023-07-19 11:03:05.000000 sliceguard-0.0.8/sliceguard/sliceguard.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     8800 2023-07-19 11:03:05.000000 sliceguard-0.0.8/sliceguard/utils.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-19 11:05:23.093813 sliceguard-0.0.8/sliceguard.egg-info/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4245 2023-07-19 11:05:23.000000 sliceguard-0.0.8/sliceguard.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      374 2023-07-19 11:05:23.000000 sliceguard-0.0.8/sliceguard.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-07-19 11:05:23.000000 sliceguard-0.0.8/sliceguard.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      264 2023-07-19 11:05:23.000000 sliceguard-0.0.8/sliceguard.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       11 2023-07-19 11:05:23.000000 sliceguard-0.0.8/sliceguard.egg-info/top_level.txt
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-19 11:05:23.093813 sliceguard-0.0.8/tests/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4742 2023-07-11 15:29:58.000000 sliceguard-0.0.8/tests/test_sliceguard.py
```

### Comparing `sliceguard-0.0.7/LICENSE` & `sliceguard-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sliceguard-0.0.7/PKG-INFO` & `sliceguard-0.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sliceguard
-Version: 0.0.7
+Version: 0.0.8
 Summary: A library for detecting critical data slices in structured and unstructured data based on features, metadata and model predictions.
 Author-email: Renumics GmbH <info@renumics.com>, Daniel Klitzke <daniel.klitzke@renumics.com>
 Project-URL: Homepage, https://github.com/Renumics/sliceguard
 Project-URL: Bug Tracker, https://github.com/Renumics/sliceguard/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -73,16 +73,17 @@
 [Evaluating automatic speech recognition models beyond global metrics — A tutorial using OpenAI’s Whisper as an example](https://medium.com/@daniel-klitzke/evaluating-automatic-speech-recognition-models-beyond-global-metrics-a-tutorial-using-openais-54b63c4dadbd)
 
 ## 🗺️ Public Roadmap
 - [x] Detection of problematic data slices
 - [x] Basic explanation of found issues via feature importances
 - [x] Limited embedding computation for images, audio, text
 - [x] Extended embedding support, e.g., more embedding models and allow precomputed embeddings
-- [ ] Speed up embedding computation using datasets library
+- [x] Speed up embedding computation using datasets library
 - [ ] Soft Dependencies for embedding computation as torch dependencies are large
 - [ ] Improve Spotlight report with embeddings in simmap and histogram for univariate analysis
 - [ ] Extensive documentation and examples for common cases
 - [ ] Data connectors for faster application on common data formats
 - [ ] Improved explanations for found issues, e.g., via SHAP
 - [ ] Generation of a summary report doing predefined checks
 - [ ] Allow for control features in order to account for expected variations when running checks
 - [ ] Improved issue detection algorithm, avoiding duplicate detections of similar problems and outliers influencing the segment detection
+- [ ] Large data support for detection and reporting, e.g., 500k audio samples with transcriptions
```

### Comparing `sliceguard-0.0.7/README.md` & `sliceguard-0.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -59,16 +59,17 @@
 [Evaluating automatic speech recognition models beyond global metrics — A tutorial using OpenAI’s Whisper as an example](https://medium.com/@daniel-klitzke/evaluating-automatic-speech-recognition-models-beyond-global-metrics-a-tutorial-using-openais-54b63c4dadbd)
 
 ## 🗺️ Public Roadmap
 - [x] Detection of problematic data slices
 - [x] Basic explanation of found issues via feature importances
 - [x] Limited embedding computation for images, audio, text
 - [x] Extended embedding support, e.g., more embedding models and allow precomputed embeddings
-- [ ] Speed up embedding computation using datasets library
+- [x] Speed up embedding computation using datasets library
 - [ ] Soft Dependencies for embedding computation as torch dependencies are large
 - [ ] Improve Spotlight report with embeddings in simmap and histogram for univariate analysis
 - [ ] Extensive documentation and examples for common cases
 - [ ] Data connectors for faster application on common data formats
 - [ ] Improved explanations for found issues, e.g., via SHAP
 - [ ] Generation of a summary report doing predefined checks
 - [ ] Allow for control features in order to account for expected variations when running checks
 - [ ] Improved issue detection algorithm, avoiding duplicate detections of similar problems and outliers influencing the segment detection
+- [ ] Large data support for detection and reporting, e.g., 500k audio samples with transcriptions
```

### Comparing `sliceguard-0.0.7/pyproject.toml` & `sliceguard-0.0.8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sliceguard"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Renumics GmbH", email="info@renumics.com"},
   { name="Daniel Klitzke", email="daniel.klitzke@renumics.com"}
 ]
 description = "A library for detecting critical data slices in structured and unstructured data based on features, metadata and model predictions."
 readme = "README.md"
 requires-python = ">=3.7"
@@ -17,14 +17,15 @@
   "hnne >= 0.1.8",
   "numpy>=1.17.2",
   "pandas >= 2.0.0",
   "fairlearn >= 0.8.0",
   "scikit-learn >= 1.2.2",
   "umap-learn >= 0.5.3",
   "transformers >= 4.30.2",
+  "datasets >= 2.13.1",
   "torch >= 2.0.1",
   "torchaudio >= 2.0.2",
   "sentence-transformers >= 2.2.1",
   "tqdm >= 4.65.0",
   "Pillow >= 9.5.0",
   "renumics-spotlight >= 1.3.0rc4",
   "plotly >= 5.15.0",
```

### Comparing `sliceguard-0.0.7/sliceguard/explanation.py` & `sliceguard-0.0.8/sliceguard/explanation.py`

 * *Files identical despite different names*

### Comparing `sliceguard-0.0.7/sliceguard/sliceguard.py` & `sliceguard-0.0.8/sliceguard/sliceguard.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,38 +34,44 @@
         features: List[str],
         y: str,
         y_pred: str,
         metric: Callable,
         min_support: int = None,
         min_drop: float = None,
         metric_mode: Literal["min", "max"] = "max",
+        remove_outliers: bool = False,
         feature_types: Dict[
             str, Literal["raw", "nominal", "ordinal", "numerical", "embedding"]
         ] = {},
         feature_orders: Dict[str, list] = {},
         precomputed_embeddings: Dict[str, np.array] = {},
         embedding_models: Dict[str, str] = {},
         hf_auth_token=None,
+        hf_num_proc=None,
+        hf_batch_size=1,
     ):
         """
         Find slices that are classified badly by your model.
 
         :param data: A pandas dataframe containing your data.
         :param features: A list of columns that contains features to feed into your model but also metadata.
         :param y: The column containing the ground-truth label.
         :param y_pred: The column containing your models prediction.
         :param metric: A callable metric function that must correspond to the form metric(y_true, y_pred) -> scikit-learn style.
         :min_support: Minimum support for clusters that are listed as issues. If you are more looking towards outliers choose small values, if you target biases choose higher values.
         :min_drop: Minimum metric drop a cluster has to have to be counted as issue compared to the result on the whole dataset.
         :param metric_mode: What do you optimize your metric for? max is the right choice for accuracy while e.g. min is good for regression error.
+        :param remove_outliers: Account for outliers that disturb cluster detection.
         :param feature_types: Specify how your feature should be treated in encoding and normalizing.
         :param feature_orders: If your feature is ordinal, specify the order of that should be used for encoding. This is required for EVERY ordinal feature.
         :param precomputed_embeddings: Supply precomputed embeddings for raw columns. E.g. if repeatedly running checks on your data.
         :param embedding_model: Supply embedding models that should be used to compute embedding vectors from raw data.
         :param hf_auth_token: The authentification token used to download embedding models from the huggingface hub.
+        :param hf_num_proc: Multiprocessing used in audio/image preprocessing.
+        :param hf_batch_size: Batch size used in computing embeddings.
         """
 
         assert (
             (
                 all(
                     [
                         (f in data.columns or f in precomputed_embeddings)
@@ -90,35 +96,43 @@
         encoded_data, prereduced_embeddings, raw_embeddings = encode_normalize_features(
             features,
             feature_types,
             feature_orders,
             precomputed_embeddings,
             embedding_models,
             hf_auth_token,
+            hf_num_proc,
+            hf_batch_size,
             df,
         )
 
         # Perform detection of problematic clusters based on the given features
         # 1. A hierarchical clustering is performed and metrics are calculated for all hierarchies
         # 2. hierarchy level that is most indicative of a real problem is then determined
         # 3. the reason for the problem e.g. feature combination or rule that is characteristic for the cluster is determined.
 
         (
             mfs,
             clustering_df,
             clustering_cols,
             clustering_metric_cols,
-        ) = generate_metric_frames(encoded_data, df, y, y_pred, metric)
+        ) = generate_metric_frames(encoded_data, df, y, y_pred, metric, remove_outliers)
 
         if len(mfs) > 0:
             overall_metric = mfs[0].overall.values[0]
             print(f"The overall metric value is {overall_metric}")
 
         group_dfs = detect_issues(
-            mfs, clustering_df, clustering_cols, min_drop, min_support, metric_mode
+            mfs,
+            clustering_df,
+            clustering_cols,
+            min_drop,
+            min_support,
+            metric_mode,
+            remove_outliers,
         )
 
         num_issues = np.sum([group_df["issue"].sum() for group_df in group_dfs])
 
         print(f"Identified {num_issues} problematic slices.")
 
         # Construct the issue dataframe that is returned by this method
@@ -206,26 +220,28 @@
 
         data_issue_order = np.argsort(data_issue_severity)
         if self._metric_mode == "min":
             data_issue_order = data_issue_order[::-1]
 
         spotlight.show(
             df,
-            dtype={ **spotlight_dtype, **embedding_dtypes},
+            dtype={**spotlight_dtype, **embedding_dtypes},
             issues=np.array(data_issues)[data_issue_order].tolist(),
             layout=layout.layout(
                 [
                     [layout.table()],
                     [layout.similaritymap()],
                     [layout.histogram()],
                 ],
                 [[layout.widgets.Inspector()], [layout.widgets.Issues()]],
             ),
         )
-        return df # Return the create report dataframe in case caller wants to process it
+        return (
+            df  # Return the create report dataframe in case caller wants to process it
+        )
 
     def _plot_clustering_overview(self):
         """
         Debugging method to get an overview on the last clustering structure.
         """
         # for i in range(len(self._clustering_cols)):
         # cur_clustering_cols = self._clustering_cols[:i+1]
```

### Comparing `sliceguard-0.0.7/sliceguard/utils.py` & `sliceguard-0.0.8/sliceguard/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Dict, Literal
+from typing import List, Dict, Literal, Optional
 
 import numpy as np
 import pandas as pd
 from sklearn.preprocessing import OneHotEncoder, OrdinalEncoder, RobustScaler
 import umap
 
 from .embedding_utils import (
@@ -68,14 +68,16 @@
 def encode_normalize_features(
     features: List[str],
     feature_types: Dict[str, Literal["raw", "nominal", "ordinal", "numerical"]],
     feature_orders: Dict[str, list],
     precomputed_embeddings: Dict[str, np.array],
     embedding_models: Dict[str, str],
     hf_auth_token: str,
+    hf_num_proc: Optional[int],
+    hf_batch_size: int,
     df: pd.DataFrame,
 ):
     """
     :param features: Names of features that should be encoded and normalized for later processing.
     :param feature_types: The previously inferred or given types of the respective features.
     :param feature_orders: If ordinal features are present you have to supply an order for each of them.
     :param precomputed_embeddings: Precomputed embeddings that the user might supply.
@@ -121,14 +123,16 @@
         elif feature_type == "raw" or feature_type == "embedding":
             # Print model that will be used for computing embeddings
             if col in df.columns and col not in precomputed_embeddings:
                 hf_model_params = (
                     {
                         "model_name": embedding_models[col],
                         "hf_auth_token": hf_auth_token,
+                        "hf_num_proc": hf_num_proc,
+                        "hf_batch_size": hf_batch_size,
                     }
                     if col in embedding_models
                     else {}
                 )
                 if "model_name" in hf_model_params:
                     print(
                         f"Using {hf_model_params['model_name']} for computing embeddings for feature {col}."
@@ -139,15 +143,17 @@
                     )
             # Set first entry as for checking type of raw data.
             if col in df.columns:
                 first_entry = df[col].iloc[0]
             if col in precomputed_embeddings:  # use precomputed embeddings when given
                 embeddings = precomputed_embeddings[col]
                 assert len(embeddings) == len(df)
-                raw_embeddings[col] = embeddings # also save them here as they are used in report
+                raw_embeddings[
+                    col
+                ] = embeddings  # also save them here as they are used in report
             elif first_entry.lower().endswith(
                 ".wav"
             ):  # TODO: Improve data type inference for raw data
                 embeddings = generate_audio_embeddings(
                     df[col].values, **hf_model_params
                 )
                 raw_embeddings[col] = embeddings
@@ -162,17 +168,19 @@
                 raw_embeddings[col] = embeddings
             else:  # Treat as text if nothing known
                 embeddings = generate_text_embeddings(df[col].values, **hf_model_params)
                 raw_embeddings[col] = embeddings
 
             # TODO: Potentially filter out entries without valid embedding or replace with mean?
             reduced_embeddings = umap.UMAP(
-                # n_neighbors=min(len(df) - 1, 30),
+                n_neighbors=min(embeddings.shape[0] - 1, 15),
+                n_components=min(
+                    embeddings.shape[0]-2, 8
+                ),  # TODO: Do not hardcode this, probably determine based on embedding size and variance. Also, check implications on normlization.
                 # min_dist=0.0,
-                n_components=8, # TODO: Do not hardcode this, probably determine based on embedding size and variance. Also, check implications on normlization.
                 random_state=42,
             ).fit_transform(embeddings)
 
             # TODO: Check if normalization makes sense. Probably do not normalize dimensiosn indenpendently!
             # reduced_embeddings = RobustScaler(
             #     quantile_range=(2.5, 97.5)
             # ).fit_transform(
```

### Comparing `sliceguard-0.0.7/sliceguard.egg-info/PKG-INFO` & `sliceguard-0.0.8/sliceguard.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sliceguard
-Version: 0.0.7
+Version: 0.0.8
 Summary: A library for detecting critical data slices in structured and unstructured data based on features, metadata and model predictions.
 Author-email: Renumics GmbH <info@renumics.com>, Daniel Klitzke <daniel.klitzke@renumics.com>
 Project-URL: Homepage, https://github.com/Renumics/sliceguard
 Project-URL: Bug Tracker, https://github.com/Renumics/sliceguard/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -73,16 +73,17 @@
 [Evaluating automatic speech recognition models beyond global metrics — A tutorial using OpenAI’s Whisper as an example](https://medium.com/@daniel-klitzke/evaluating-automatic-speech-recognition-models-beyond-global-metrics-a-tutorial-using-openais-54b63c4dadbd)
 
 ## 🗺️ Public Roadmap
 - [x] Detection of problematic data slices
 - [x] Basic explanation of found issues via feature importances
 - [x] Limited embedding computation for images, audio, text
 - [x] Extended embedding support, e.g., more embedding models and allow precomputed embeddings
-- [ ] Speed up embedding computation using datasets library
+- [x] Speed up embedding computation using datasets library
 - [ ] Soft Dependencies for embedding computation as torch dependencies are large
 - [ ] Improve Spotlight report with embeddings in simmap and histogram for univariate analysis
 - [ ] Extensive documentation and examples for common cases
 - [ ] Data connectors for faster application on common data formats
 - [ ] Improved explanations for found issues, e.g., via SHAP
 - [ ] Generation of a summary report doing predefined checks
 - [ ] Allow for control features in order to account for expected variations when running checks
 - [ ] Improved issue detection algorithm, avoiding duplicate detections of similar problems and outliers influencing the segment detection
+- [ ] Large data support for detection and reporting, e.g., 500k audio samples with transcriptions
```

### Comparing `sliceguard-0.0.7/tests/test_sliceguard.py` & `sliceguard-0.0.8/tests/test_sliceguard.py`

 * *Files identical despite different names*

