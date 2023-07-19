# Comparing `tmp/landingai-0.2.7.tar.gz` & `tmp/landingai-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "landingai-0.2.7.tar", max compression
+gzip compressed data, was "landingai-0.2.8.tar", max compression
```

## Comparing `landingai-0.2.7.tar` & `landingai-0.2.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1063 2023-07-18 22:05:40.715681 landingai-0.2.7/LICENSE.md
--rw-r--r--   0        0        0     6743 2023-07-18 22:05:40.715681 landingai-0.2.7/README.md
--rw-r--r--   0        0        0      354 2023-07-18 22:05:40.747681 landingai-0.2.7/landingai/__init__.py
--rw-r--r--   0        0        0     6451 2023-07-18 22:05:40.747681 landingai-0.2.7/landingai/common.py
--rw-r--r--   0        0        0       72 2023-07-18 22:05:40.747681 landingai-0.2.7/landingai/data_management/__init__.py
--rw-r--r--   0        0        0     8714 2023-07-18 22:05:40.747681 landingai-0.2.7/landingai/data_management/client.py
--rw-r--r--   0        0        0    21135 2023-07-18 22:05:40.747681 landingai-0.2.7/landingai/data_management/media.py
--rw-r--r--   0        0        0     4722 2023-07-18 22:05:40.747681 landingai-0.2.7/landingai/data_management/metadata.py
--rw-r--r--   0        0        0     2188 2023-07-18 22:05:40.747681 landingai-0.2.7/landingai/data_management/utils.py
--rw-r--r--   0        0        0     9730 2023-07-18 22:05:40.747681 landingai-0.2.7/landingai/exceptions.py
--rw-r--r--   0        0        0  1594400 2023-07-18 22:05:40.759681 landingai-0.2.7/landingai/fonts/default_font_ch_en.ttf
--rw-r--r--   0        0        0     5915 2023-07-18 22:05:40.759681 landingai-0.2.7/landingai/image_source_ops.py
--rw-r--r--   0        0        0     1502 2023-07-18 22:05:40.759681 landingai-0.2.7/landingai/notebook_utils.py
--rw-r--r--   0        0        0      420 2023-07-18 22:05:40.759681 landingai-0.2.7/landingai/pipeline/__init__.py
--rw-r--r--   0        0        0    16449 2023-07-18 22:05:40.759681 landingai-0.2.7/landingai/pipeline/frameset.py
--rw-r--r--   0        0        0    11810 2023-07-18 22:05:40.759681 landingai-0.2.7/landingai/pipeline/image_source.py
--rw-r--r--   0        0        0     1339 2023-07-18 22:05:40.759681 landingai-0.2.7/landingai/pipeline/postprocessing.py
--rw-r--r--   0        0        0     8389 2023-07-18 22:05:40.759681 landingai-0.2.7/landingai/postprocess.py
--rw-r--r--   0        0        0    25762 2023-07-18 22:05:40.759681 landingai-0.2.7/landingai/predict.py
--rw-r--r--   0        0        0     6462 2023-07-18 22:05:40.759681 landingai-0.2.7/landingai/st_utils.py
--rw-r--r--   0        0        0       40 2023-07-18 22:05:40.759681 landingai-0.2.7/landingai/storage/__init__.py
--rw-r--r--   0        0        0     4439 2023-07-18 22:05:40.759681 landingai-0.2.7/landingai/storage/data_access.py
--rw-r--r--   0        0        0     4340 2023-07-18 22:05:40.759681 landingai-0.2.7/landingai/storage/snowflake.py
--rw-r--r--   0        0        0     1503 2023-07-18 22:05:40.759681 landingai-0.2.7/landingai/telemetry.py
--rw-r--r--   0        0        0     5869 2023-07-18 22:05:40.759681 landingai-0.2.7/landingai/timer.py
--rw-r--r--   0        0        0     1685 2023-07-18 22:05:40.763681 landingai-0.2.7/landingai/transform.py
--rw-r--r--   0        0        0     1598 2023-07-18 22:05:40.763681 landingai-0.2.7/landingai/utils.py
--rw-r--r--   0        0        0    13403 2023-07-18 22:05:40.763681 landingai-0.2.7/landingai/visualize.py
--rw-r--r--   0        0        0     2606 2023-07-18 22:05:41.447679 landingai-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     7988 1970-01-01 00:00:00.000000 landingai-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-19 00:57:21.427837 landingai-0.2.8/LICENSE.md
+-rw-r--r--   0        0        0     6743 2023-07-19 00:57:21.427837 landingai-0.2.8/README.md
+-rw-r--r--   0        0        0      354 2023-07-19 00:57:21.455837 landingai-0.2.8/landingai/__init__.py
+-rw-r--r--   0        0        0     6451 2023-07-19 00:57:21.455837 landingai-0.2.8/landingai/common.py
+-rw-r--r--   0        0        0       72 2023-07-19 00:57:21.455837 landingai-0.2.8/landingai/data_management/__init__.py
+-rw-r--r--   0        0        0     8714 2023-07-19 00:57:21.455837 landingai-0.2.8/landingai/data_management/client.py
+-rw-r--r--   0        0        0    21178 2023-07-19 00:57:21.455837 landingai-0.2.8/landingai/data_management/media.py
+-rw-r--r--   0        0        0     4722 2023-07-19 00:57:21.455837 landingai-0.2.8/landingai/data_management/metadata.py
+-rw-r--r--   0        0        0     2188 2023-07-19 00:57:21.455837 landingai-0.2.8/landingai/data_management/utils.py
+-rw-r--r--   0        0        0     9730 2023-07-19 00:57:21.455837 landingai-0.2.8/landingai/exceptions.py
+-rw-r--r--   0        0        0  1594400 2023-07-19 00:57:21.463837 landingai-0.2.8/landingai/fonts/default_font_ch_en.ttf
+-rw-r--r--   0        0        0     5915 2023-07-19 00:57:21.467837 landingai-0.2.8/landingai/image_source_ops.py
+-rw-r--r--   0        0        0     1502 2023-07-19 00:57:21.467837 landingai-0.2.8/landingai/notebook_utils.py
+-rw-r--r--   0        0        0      420 2023-07-19 00:57:21.467837 landingai-0.2.8/landingai/pipeline/__init__.py
+-rw-r--r--   0        0        0    16449 2023-07-19 00:57:21.467837 landingai-0.2.8/landingai/pipeline/frameset.py
+-rw-r--r--   0        0        0    11810 2023-07-19 00:57:21.467837 landingai-0.2.8/landingai/pipeline/image_source.py
+-rw-r--r--   0        0        0     1339 2023-07-19 00:57:21.467837 landingai-0.2.8/landingai/pipeline/postprocessing.py
+-rw-r--r--   0        0        0     8389 2023-07-19 00:57:21.467837 landingai-0.2.8/landingai/postprocess.py
+-rw-r--r--   0        0        0    25677 2023-07-19 00:57:21.467837 landingai-0.2.8/landingai/predict.py
+-rw-r--r--   0        0        0     6462 2023-07-19 00:57:21.467837 landingai-0.2.8/landingai/st_utils.py
+-rw-r--r--   0        0        0       40 2023-07-19 00:57:21.467837 landingai-0.2.8/landingai/storage/__init__.py
+-rw-r--r--   0        0        0     4439 2023-07-19 00:57:21.467837 landingai-0.2.8/landingai/storage/data_access.py
+-rw-r--r--   0        0        0     4340 2023-07-19 00:57:21.467837 landingai-0.2.8/landingai/storage/snowflake.py
+-rw-r--r--   0        0        0     1503 2023-07-19 00:57:21.467837 landingai-0.2.8/landingai/telemetry.py
+-rw-r--r--   0        0        0     5869 2023-07-19 00:57:21.467837 landingai-0.2.8/landingai/timer.py
+-rw-r--r--   0        0        0     1685 2023-07-19 00:57:21.467837 landingai-0.2.8/landingai/transform.py
+-rw-r--r--   0        0        0     2812 2023-07-19 00:57:21.467837 landingai-0.2.8/landingai/utils.py
+-rw-r--r--   0        0        0    13403 2023-07-19 00:57:21.467837 landingai-0.2.8/landingai/visualize.py
+-rw-r--r--   0        0        0     2606 2023-07-19 00:57:22.255844 landingai-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     7988 1970-01-01 00:00:00.000000 landingai-0.2.8/PKG-INFO
```

### Comparing `landingai-0.2.7/LICENSE.md` & `landingai-0.2.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `landingai-0.2.7/README.md` & `landingai-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `landingai-0.2.7/landingai/common.py` & `landingai-0.2.8/landingai/common.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.7/landingai/data_management/client.py` & `landingai-0.2.8/landingai/data_management/client.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.7/landingai/data_management/media.py` & `landingai-0.2.8/landingai/data_management/media.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,24 +25,24 @@
 from landingai.data_management.utils import (
     PrettyPrintable,
     obj_to_dict,
     obj_to_params,
     validate_metadata,
 )
 from landingai.exceptions import DuplicateUploadError, HttpError
-from landingai.utils import serialize_image
+from landingai.utils import _LLENS_SUPPORTED_IMAGE_FORMATS, serialize_image
 
 MediaType = Enum("MediaType", ["image", "video"])
 SrcType = Enum("SrcType", ["user", "production_line", "prism"])
 ThumbnailSize = Enum(
     "ThumbnailSize", ["50x50", "250x250", "500x500", "750x750", "1000x1000"]
 )
 
 
-_ALLOWED_EXTENSIONS = ["jpg", "jpeg", "png", "bmp", "tiff"]
+_ALLOWED_EXTENSIONS = _LLENS_SUPPORTED_IMAGE_FORMATS + ["TIFF", "TIF"]
 _HIDDEN_FILES_TO_IGNORE = ["thumbs.db", "desktop.ini", ".ds_store"]
 
 _CONCURRENCY_LIMIT = 5
 _LOGGER = logging.getLogger(__name__)
 
 
 class Media:
@@ -199,15 +199,15 @@
                 ts = int(datetime.now().timestamp() * 1000)
                 filename = f"image_{ts}.{ext}"
             else:
                 assert isinstance(source, str)
                 filename = os.path.basename(source)
                 ext = os.path.splitext(filename)[-1][1:]
             # Validate extension
-            if validate_extensions and ext.lower() not in _ALLOWED_EXTENSIONS:
+            if validate_extensions and ext.upper() not in _ALLOWED_EXTENSIONS:
                 raise ValueError(
                     f"""Unexpected extension {ext}. Allowed extensions are: {_ALLOWED_EXTENSIONS}.
                     If you want to attempt the upload anyway, set validate_extensions=False.
                     This may result in an unexpected behavior - e.g. file not showing up in data browser."""
                 )
             # Create an async task
             file_tasks = _upload_media(
@@ -449,15 +449,15 @@
     task_to_filename = {}
     tasks = []
     for root, _, filenames in os.walk(path):
         for filename in filenames:
             ext = os.path.splitext(filename)[-1][1:]
             if filename.lower() in _HIDDEN_FILES_TO_IGNORE:
                 pass
-            elif ext.lower() in _ALLOWED_EXTENSIONS or not validate_extensions:
+            elif ext.upper() in _ALLOWED_EXTENSIONS or not validate_extensions:
                 loop = asyncio.get_event_loop()
                 task = loop.create_task(
                     _upload_media_with_semaphore(
                         client,
                         dataset_id,
                         filename,
                         os.path.join(root, filename),
```

### Comparing `landingai-0.2.7/landingai/data_management/metadata.py` & `landingai-0.2.8/landingai/data_management/metadata.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.7/landingai/data_management/utils.py` & `landingai-0.2.8/landingai/data_management/utils.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.7/landingai/exceptions.py` & `landingai-0.2.8/landingai/exceptions.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.7/landingai/fonts/default_font_ch_en.ttf` & `landingai-0.2.8/landingai/fonts/default_font_ch_en.ttf`

 * *Files identical despite different names*

### Comparing `landingai-0.2.7/landingai/image_source_ops.py` & `landingai-0.2.8/landingai/image_source_ops.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.7/landingai/notebook_utils.py` & `landingai-0.2.8/landingai/notebook_utils.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.7/landingai/pipeline/frameset.py` & `landingai-0.2.8/landingai/pipeline/frameset.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.7/landingai/pipeline/image_source.py` & `landingai-0.2.8/landingai/pipeline/image_source.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.7/landingai/pipeline/postprocessing.py` & `landingai-0.2.8/landingai/pipeline/postprocessing.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.7/landingai/postprocess.py` & `landingai-0.2.8/landingai/postprocess.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.7/landingai/predict.py` & `landingai-0.2.8/landingai/predict.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         Returns
         -------
         The inference result in a list of dictionary
             Each dictionary is a prediction result.
             The inference result has been filtered by the confidence threshold set in LandingLens and sorted by confidence score in descending order.
         """
         buffer_bytes = serialize_image(image)
-        files = [("file", ("image.png", buffer_bytes, "image/png"))]
+        files = {"file": buffer_bytes}
         payload = {
             "endpoint_id": self._endpoint_id,
             "device_type": "pylib",
         }
         _add_defualt_query_params(payload)
         return _do_inference(
             self._session, Predictor._url, files, payload, _CloudExtractor
@@ -145,15 +145,15 @@
         Returns
         -------
         List[OcrPrediction]
             A list of OCR prediction result.
         """
 
         buffer_bytes = serialize_image(image)
-        files = [("images", ("image.png", buffer_bytes, "image/png"))]
+        files = {"images": buffer_bytes}
         mode: str = kwargs.get("mode", "multi-text")
         if mode not in ["multi-text", "single-text"]:
             raise ValueError(
                 f"mode must be either 'multi-text' or 'single-text', but got: {mode}"
             )
         if mode == "single-text" and "regions_of_interest" not in kwargs:
             raise ValueError(
@@ -214,15 +214,15 @@
 
         Returns
         -------
         List[Prediction]
             A list of prediction result.
         """
         buffer_bytes = serialize_image(image)
-        files = [("file", ("image.png", buffer_bytes, "image/png"))]
+        files = {"file": buffer_bytes}
         return _do_inference(self._session, self._url, files, {}, _EdgeExtractor)
 
 
 class _Extractor:
     """The base class for all extractors. This is useful for type checking."""
 
     @staticmethod
@@ -685,15 +685,15 @@
     return session
 
 
 @Timer(name="_do_inference", log_fn=_LOGGER.debug)
 def _do_inference(
     session: Session,
     endpoint_url: str,
-    files: List[Any],
+    files: Dict[str, Any],
     payload: Dict[str, Any],
     extractor_class: Type[_Extractor],
     *,
     data: Optional[Dict[str, Any]] = None,
 ) -> List[Prediction]:
     """Call the inference endpoint and extract the prediction result."""
     try:
```

### Comparing `landingai-0.2.7/landingai/st_utils.py` & `landingai-0.2.8/landingai/st_utils.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.7/landingai/storage/data_access.py` & `landingai-0.2.8/landingai/storage/data_access.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.7/landingai/storage/snowflake.py` & `landingai-0.2.8/landingai/storage/snowflake.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.7/landingai/telemetry.py` & `landingai-0.2.8/landingai/telemetry.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.7/landingai/timer.py` & `landingai-0.2.8/landingai/timer.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.7/landingai/transform.py` & `landingai-0.2.8/landingai/transform.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.7/landingai/visualize.py` & `landingai-0.2.8/landingai/visualize.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.7/pyproject.toml` & `landingai-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "landingai"
-version = "0.2.7"
+version = "0.2.8"
 description = "Helper library for interacting with Landing AI LandingLens"
 authors = ["Landing AI <dev@landing.ai>"]
 readme = "README.md"
 packages = [{include = "landingai"}]
 
 [tool.poetry.urls]
 "Homepage" = "https://landing.ai"
```

### Comparing `landingai-0.2.7/PKG-INFO` & `landingai-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: landingai
-Version: 0.2.7
+Version: 0.2.8
 Summary: Helper library for interacting with Landing AI LandingLens
 Author: Landing AI
 Author-email: dev@landing.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

