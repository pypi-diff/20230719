# Comparing `tmp/landingai-0.2.6.tar.gz` & `tmp/landingai-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "landingai-0.2.6.tar", max compression
+gzip compressed data, was "landingai-0.2.7.tar", max compression
```

## Comparing `landingai-0.2.6.tar` & `landingai-0.2.7.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0     1063 2023-07-14 23:22:44.010675 landingai-0.2.6/LICENSE.md
--rw-r--r--   0        0        0     6743 2023-07-14 23:22:44.010675 landingai-0.2.6/README.md
--rw-r--r--   0        0        0      354 2023-07-14 23:22:44.046676 landingai-0.2.6/landingai/__init__.py
--rw-r--r--   0        0        0     6451 2023-07-14 23:22:44.046676 landingai-0.2.6/landingai/common.py
--rw-r--r--   0        0        0       72 2023-07-14 23:22:44.046676 landingai-0.2.6/landingai/data_management/__init__.py
--rw-r--r--   0        0        0     8714 2023-07-14 23:22:44.046676 landingai-0.2.6/landingai/data_management/client.py
--rw-r--r--   0        0        0    21135 2023-07-14 23:22:44.046676 landingai-0.2.6/landingai/data_management/media.py
--rw-r--r--   0        0        0     4722 2023-07-14 23:22:44.046676 landingai-0.2.6/landingai/data_management/metadata.py
--rw-r--r--   0        0        0     2188 2023-07-14 23:22:44.046676 landingai-0.2.6/landingai/data_management/utils.py
--rw-r--r--   0        0        0     9730 2023-07-14 23:22:44.046676 landingai-0.2.6/landingai/exceptions.py
--rw-r--r--   0        0        0  1594400 2023-07-14 23:22:44.058676 landingai-0.2.6/landingai/fonts/default_font_ch_en.ttf
--rw-r--r--   0        0        0     5915 2023-07-14 23:22:44.058676 landingai-0.2.6/landingai/image_source_ops.py
--rw-r--r--   0        0        0     1502 2023-07-14 23:22:44.058676 landingai-0.2.6/landingai/notebook_utils.py
--rw-r--r--   0        0        0      420 2023-07-14 23:22:44.058676 landingai-0.2.6/landingai/pipeline/__init__.py
--rw-r--r--   0        0        0    16449 2023-07-14 23:22:44.058676 landingai-0.2.6/landingai/pipeline/frameset.py
--rw-r--r--   0        0        0    11810 2023-07-14 23:22:44.058676 landingai-0.2.6/landingai/pipeline/image_source.py
--rw-r--r--   0        0        0     1339 2023-07-14 23:22:44.058676 landingai-0.2.6/landingai/pipeline/postprocessing.py
--rw-r--r--   0        0        0     8389 2023-07-14 23:22:44.058676 landingai-0.2.6/landingai/postprocess.py
--rw-r--r--   0        0        0    25559 2023-07-14 23:22:44.058676 landingai-0.2.6/landingai/predict.py
--rw-r--r--   0        0        0     6462 2023-07-14 23:22:44.058676 landingai-0.2.6/landingai/st_utils.py
--rw-r--r--   0        0        0       40 2023-07-14 23:22:44.058676 landingai-0.2.6/landingai/storage/__init__.py
--rw-r--r--   0        0        0     4439 2023-07-14 23:22:44.058676 landingai-0.2.6/landingai/storage/data_access.py
--rw-r--r--   0        0        0     4340 2023-07-14 23:22:44.058676 landingai-0.2.6/landingai/storage/snowflake.py
--rw-r--r--   0        0        0     1503 2023-07-14 23:22:44.058676 landingai-0.2.6/landingai/telemetry.py
--rw-r--r--   0        0        0     1685 2023-07-14 23:22:44.058676 landingai-0.2.6/landingai/transform.py
--rw-r--r--   0        0        0     1598 2023-07-14 23:22:44.058676 landingai-0.2.6/landingai/utils.py
--rw-r--r--   0        0        0    13403 2023-07-14 23:22:44.058676 landingai-0.2.6/landingai/visualize.py
--rw-r--r--   0        0        0     2606 2023-07-14 23:22:44.886702 landingai-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     7988 1970-01-01 00:00:00.000000 landingai-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-18 22:05:40.715681 landingai-0.2.7/LICENSE.md
+-rw-r--r--   0        0        0     6743 2023-07-18 22:05:40.715681 landingai-0.2.7/README.md
+-rw-r--r--   0        0        0      354 2023-07-18 22:05:40.747681 landingai-0.2.7/landingai/__init__.py
+-rw-r--r--   0        0        0     6451 2023-07-18 22:05:40.747681 landingai-0.2.7/landingai/common.py
+-rw-r--r--   0        0        0       72 2023-07-18 22:05:40.747681 landingai-0.2.7/landingai/data_management/__init__.py
+-rw-r--r--   0        0        0     8714 2023-07-18 22:05:40.747681 landingai-0.2.7/landingai/data_management/client.py
+-rw-r--r--   0        0        0    21135 2023-07-18 22:05:40.747681 landingai-0.2.7/landingai/data_management/media.py
+-rw-r--r--   0        0        0     4722 2023-07-18 22:05:40.747681 landingai-0.2.7/landingai/data_management/metadata.py
+-rw-r--r--   0        0        0     2188 2023-07-18 22:05:40.747681 landingai-0.2.7/landingai/data_management/utils.py
+-rw-r--r--   0        0        0     9730 2023-07-18 22:05:40.747681 landingai-0.2.7/landingai/exceptions.py
+-rw-r--r--   0        0        0  1594400 2023-07-18 22:05:40.759681 landingai-0.2.7/landingai/fonts/default_font_ch_en.ttf
+-rw-r--r--   0        0        0     5915 2023-07-18 22:05:40.759681 landingai-0.2.7/landingai/image_source_ops.py
+-rw-r--r--   0        0        0     1502 2023-07-18 22:05:40.759681 landingai-0.2.7/landingai/notebook_utils.py
+-rw-r--r--   0        0        0      420 2023-07-18 22:05:40.759681 landingai-0.2.7/landingai/pipeline/__init__.py
+-rw-r--r--   0        0        0    16449 2023-07-18 22:05:40.759681 landingai-0.2.7/landingai/pipeline/frameset.py
+-rw-r--r--   0        0        0    11810 2023-07-18 22:05:40.759681 landingai-0.2.7/landingai/pipeline/image_source.py
+-rw-r--r--   0        0        0     1339 2023-07-18 22:05:40.759681 landingai-0.2.7/landingai/pipeline/postprocessing.py
+-rw-r--r--   0        0        0     8389 2023-07-18 22:05:40.759681 landingai-0.2.7/landingai/postprocess.py
+-rw-r--r--   0        0        0    25762 2023-07-18 22:05:40.759681 landingai-0.2.7/landingai/predict.py
+-rw-r--r--   0        0        0     6462 2023-07-18 22:05:40.759681 landingai-0.2.7/landingai/st_utils.py
+-rw-r--r--   0        0        0       40 2023-07-18 22:05:40.759681 landingai-0.2.7/landingai/storage/__init__.py
+-rw-r--r--   0        0        0     4439 2023-07-18 22:05:40.759681 landingai-0.2.7/landingai/storage/data_access.py
+-rw-r--r--   0        0        0     4340 2023-07-18 22:05:40.759681 landingai-0.2.7/landingai/storage/snowflake.py
+-rw-r--r--   0        0        0     1503 2023-07-18 22:05:40.759681 landingai-0.2.7/landingai/telemetry.py
+-rw-r--r--   0        0        0     5869 2023-07-18 22:05:40.759681 landingai-0.2.7/landingai/timer.py
+-rw-r--r--   0        0        0     1685 2023-07-18 22:05:40.763681 landingai-0.2.7/landingai/transform.py
+-rw-r--r--   0        0        0     1598 2023-07-18 22:05:40.763681 landingai-0.2.7/landingai/utils.py
+-rw-r--r--   0        0        0    13403 2023-07-18 22:05:40.763681 landingai-0.2.7/landingai/visualize.py
+-rw-r--r--   0        0        0     2606 2023-07-18 22:05:41.447679 landingai-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     7988 1970-01-01 00:00:00.000000 landingai-0.2.7/PKG-INFO
```

### Comparing `landingai-0.2.6/LICENSE.md` & `landingai-0.2.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `landingai-0.2.6/README.md` & `landingai-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `landingai-0.2.6/landingai/common.py` & `landingai-0.2.7/landingai/common.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.6/landingai/data_management/client.py` & `landingai-0.2.7/landingai/data_management/client.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.6/landingai/data_management/media.py` & `landingai-0.2.7/landingai/data_management/media.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.6/landingai/data_management/metadata.py` & `landingai-0.2.7/landingai/data_management/metadata.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.6/landingai/data_management/utils.py` & `landingai-0.2.7/landingai/data_management/utils.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.6/landingai/exceptions.py` & `landingai-0.2.7/landingai/exceptions.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.6/landingai/fonts/default_font_ch_en.ttf` & `landingai-0.2.7/landingai/fonts/default_font_ch_en.ttf`

 * *Files identical despite different names*

### Comparing `landingai-0.2.6/landingai/image_source_ops.py` & `landingai-0.2.7/landingai/image_source_ops.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.6/landingai/notebook_utils.py` & `landingai-0.2.7/landingai/notebook_utils.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.6/landingai/pipeline/frameset.py` & `landingai-0.2.7/landingai/pipeline/frameset.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.6/landingai/pipeline/image_source.py` & `landingai-0.2.7/landingai/pipeline/image_source.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.6/landingai/pipeline/postprocessing.py` & `landingai-0.2.7/landingai/pipeline/postprocessing.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.6/landingai/postprocess.py` & `landingai-0.2.7/landingai/postprocess.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.6/landingai/predict.py` & `landingai-0.2.7/landingai/predict.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     ObjectDetectionPrediction,
     OcrPrediction,
     Prediction,
     SegmentationPrediction,
 )
 from landingai.exceptions import HttpResponse
 from landingai.telemetry import get_runtime_environment_info, is_running_in_pytest
+from landingai.timer import Timer
 from landingai.utils import load_api_credential, serialize_image
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class Predictor:
     """A class that calls your inference endpoint on the LandingLens platform."""
@@ -61,14 +62,15 @@
         """Build the HTTP headers for the request to the Cloud inference endpoint(s)."""
         headers = {
             "contentType": "application/json",
             "apikey": api_key.api_key,
         }
         return headers
 
+    @Timer(name="Predictor.predict")
     def predict(
         self, image: Union[np.ndarray, PIL.Image.Image], **kwargs: Any
     ) -> List[Prediction]:
         """Call the inference endpoint and return the prediction result.
 
         Parameters
         ----------
@@ -116,14 +118,15 @@
             LANDINGAI_API_KEY or from the .env file.
         """
         self._threshold = threshold
         self._api_credential = load_api_credential(api_key)
         headers = self._build_default_headers(self._api_credential)
         self._session = _create_session(Predictor._url, self._num_retry, headers)
 
+    @Timer(name="OcrPredictor.predict")
     def predict(
         self, image: Union[np.ndarray, PIL.Image.Image], **kwargs: Any
     ) -> List[Prediction]:
         """Run OCR on the input image and return the prediction result.
 
         Parameters
         ----------
@@ -194,14 +197,15 @@
         port: int,
     ) -> None:
         self._url = f"http://{host}:{port}/images"
         self._session = _create_session(
             self._url, self._num_retry, {"contentType": "multipart/form-data"}
         )
 
+    @Timer(name="EdgePredictor.predict")
     def predict(
         self, image: Union[np.ndarray, PIL.Image.Image], **kwargs: Any
     ) -> List[Prediction]:
         """Run Edge inference on the input image and return the prediction result.
 
         Parameters
         ----------
@@ -677,14 +681,15 @@
     session.mount(
         url, HTTPAdapter(max_retries=retries)
     )  # Since POST is not idempotent we will ony retry on the this specific API
     session.headers.update(headers)
     return session
 
 
+@Timer(name="_do_inference", log_fn=_LOGGER.debug)
 def _do_inference(
     session: Session,
     endpoint_url: str,
     files: List[Any],
     payload: Dict[str, Any],
     extractor_class: Type[_Extractor],
     *,
```

### Comparing `landingai-0.2.6/landingai/st_utils.py` & `landingai-0.2.7/landingai/st_utils.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.6/landingai/storage/data_access.py` & `landingai-0.2.7/landingai/storage/data_access.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.6/landingai/storage/snowflake.py` & `landingai-0.2.7/landingai/storage/snowflake.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.6/landingai/telemetry.py` & `landingai-0.2.7/landingai/telemetry.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.6/landingai/transform.py` & `landingai-0.2.7/landingai/transform.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.6/landingai/utils.py` & `landingai-0.2.7/landingai/utils.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.6/landingai/visualize.py` & `landingai-0.2.7/landingai/visualize.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.6/pyproject.toml` & `landingai-0.2.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "landingai"
-version = "0.2.6"
+version = "0.2.7"
 description = "Helper library for interacting with Landing AI LandingLens"
 authors = ["Landing AI <dev@landing.ai>"]
 readme = "README.md"
 packages = [{include = "landingai"}]
 
 [tool.poetry.urls]
 "Homepage" = "https://landing.ai"
```

### Comparing `landingai-0.2.6/PKG-INFO` & `landingai-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: landingai
-Version: 0.2.6
+Version: 0.2.7
 Summary: Helper library for interacting with Landing AI LandingLens
 Author: Landing AI
 Author-email: dev@landing.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

