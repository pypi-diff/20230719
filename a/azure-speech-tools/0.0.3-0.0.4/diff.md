# Comparing `tmp/azure_speech_tools-0.0.3.tar.gz` & `tmp/azure_speech_tools-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure_speech_tools-0.0.3.tar", last modified: Wed Jul 19 05:37:40 2023, max compression
+gzip compressed data, was "azure_speech_tools-0.0.4.tar", last modified: Wed Jul 19 05:56:30 2023, max compression
```

## Comparing `azure_speech_tools-0.0.3.tar` & `azure_speech_tools-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 pranavp   (1000) pranavp   (1000)        0 2023-07-19 05:37:40.879226 azure_speech_tools-0.0.3/
--rw-r--r--   0 pranavp   (1000) pranavp   (1000)       39 2023-07-17 09:45:25.000000 azure_speech_tools-0.0.3/MANIFEST.in
--rw-r--r--   0 pranavp   (1000) pranavp   (1000)      183 2023-07-19 05:37:40.879226 azure_speech_tools-0.0.3/PKG-INFO
-drwxr-xr-x   0 pranavp   (1000) pranavp   (1000)        0 2023-07-19 05:37:40.879226 azure_speech_tools-0.0.3/azure_speech_tools/
--rw-r--r--   0 pranavp   (1000) pranavp   (1000)       80 2023-07-17 09:44:29.000000 azure_speech_tools-0.0.3/azure_speech_tools/__init__.py
-drwxr-xr-x   0 pranavp   (1000) pranavp   (1000)        0 2023-07-19 05:37:40.879226 azure_speech_tools-0.0.3/azure_speech_tools/tools/
--rw-r--r--   0 pranavp   (1000) pranavp   (1000)       80 2023-07-17 09:46:09.000000 azure_speech_tools-0.0.3/azure_speech_tools/tools/__init__.py
--rw-r--r--   0 pranavp   (1000) pranavp   (1000)     1113 2023-07-19 05:29:14.000000 azure_speech_tools-0.0.3/azure_speech_tools/tools/azure_speech_sr.py
--rw-r--r--   0 pranavp   (1000) pranavp   (1000)     1516 2023-07-17 14:10:46.000000 azure_speech_tools-0.0.3/azure_speech_tools/tools/azure_speech_tts.py
--rw-r--r--   0 pranavp   (1000) pranavp   (1000)      568 2023-07-17 17:25:13.000000 azure_speech_tools-0.0.3/azure_speech_tools/tools/utils.py
-drwxr-xr-x   0 pranavp   (1000) pranavp   (1000)        0 2023-07-19 05:37:40.879226 azure_speech_tools-0.0.3/azure_speech_tools/yamls/
--rw-r--r--   0 pranavp   (1000) pranavp   (1000)      494 2023-07-19 05:33:45.000000 azure_speech_tools-0.0.3/azure_speech_tools/yamls/azure_speech_sr.yaml
--rw-r--r--   0 pranavp   (1000) pranavp   (1000)      623 2023-07-19 05:15:47.000000 azure_speech_tools-0.0.3/azure_speech_tools/yamls/azure_speech_tts.yaml
-drwxr-xr-x   0 pranavp   (1000) pranavp   (1000)        0 2023-07-19 05:37:40.879226 azure_speech_tools-0.0.3/azure_speech_tools.egg-info/
--rw-r--r--   0 pranavp   (1000) pranavp   (1000)      183 2023-07-19 05:37:40.000000 azure_speech_tools-0.0.3/azure_speech_tools.egg-info/PKG-INFO
--rw-r--r--   0 pranavp   (1000) pranavp   (1000)      558 2023-07-19 05:37:40.000000 azure_speech_tools-0.0.3/azure_speech_tools.egg-info/SOURCES.txt
--rw-r--r--   0 pranavp   (1000) pranavp   (1000)        1 2023-07-19 05:37:40.000000 azure_speech_tools-0.0.3/azure_speech_tools.egg-info/dependency_links.txt
--rw-r--r--   0 pranavp   (1000) pranavp   (1000)       78 2023-07-19 05:37:40.000000 azure_speech_tools-0.0.3/azure_speech_tools.egg-info/entry_points.txt
--rw-r--r--   0 pranavp   (1000) pranavp   (1000)       65 2023-07-19 05:37:40.000000 azure_speech_tools-0.0.3/azure_speech_tools.egg-info/requires.txt
--rw-r--r--   0 pranavp   (1000) pranavp   (1000)       19 2023-07-19 05:37:40.000000 azure_speech_tools-0.0.3/azure_speech_tools.egg-info/top_level.txt
--rw-r--r--   0 pranavp   (1000) pranavp   (1000)       38 2023-07-19 05:37:40.879226 azure_speech_tools-0.0.3/setup.cfg
--rw-r--r--   0 pranavp   (1000) pranavp   (1000)      543 2023-07-19 05:37:00.000000 azure_speech_tools-0.0.3/setup.py
+drwxr-xr-x   0 pranavp   (1000) pranavp   (1000)        0 2023-07-19 05:56:30.435931 azure_speech_tools-0.0.4/
+-rw-r--r--   0 pranavp   (1000) pranavp   (1000)       39 2023-07-17 09:45:25.000000 azure_speech_tools-0.0.4/MANIFEST.in
+-rw-r--r--   0 pranavp   (1000) pranavp   (1000)      183 2023-07-19 05:56:30.435931 azure_speech_tools-0.0.4/PKG-INFO
+drwxr-xr-x   0 pranavp   (1000) pranavp   (1000)        0 2023-07-19 05:56:30.435931 azure_speech_tools-0.0.4/azure_speech_tools/
+-rw-r--r--   0 pranavp   (1000) pranavp   (1000)       80 2023-07-17 09:44:29.000000 azure_speech_tools-0.0.4/azure_speech_tools/__init__.py
+drwxr-xr-x   0 pranavp   (1000) pranavp   (1000)        0 2023-07-19 05:56:30.435931 azure_speech_tools-0.0.4/azure_speech_tools/tools/
+-rw-r--r--   0 pranavp   (1000) pranavp   (1000)       80 2023-07-17 09:46:09.000000 azure_speech_tools-0.0.4/azure_speech_tools/tools/__init__.py
+-rw-r--r--   0 pranavp   (1000) pranavp   (1000)     1217 2023-07-19 05:55:31.000000 azure_speech_tools-0.0.4/azure_speech_tools/tools/azure_speech_sr.py
+-rw-r--r--   0 pranavp   (1000) pranavp   (1000)     1516 2023-07-17 14:10:46.000000 azure_speech_tools-0.0.4/azure_speech_tools/tools/azure_speech_tts.py
+-rw-r--r--   0 pranavp   (1000) pranavp   (1000)      568 2023-07-17 17:25:13.000000 azure_speech_tools-0.0.4/azure_speech_tools/tools/utils.py
+drwxr-xr-x   0 pranavp   (1000) pranavp   (1000)        0 2023-07-19 05:56:30.435931 azure_speech_tools-0.0.4/azure_speech_tools/yamls/
+-rw-r--r--   0 pranavp   (1000) pranavp   (1000)      494 2023-07-19 05:33:45.000000 azure_speech_tools-0.0.4/azure_speech_tools/yamls/azure_speech_sr.yaml
+-rw-r--r--   0 pranavp   (1000) pranavp   (1000)      623 2023-07-19 05:15:47.000000 azure_speech_tools-0.0.4/azure_speech_tools/yamls/azure_speech_tts.yaml
+drwxr-xr-x   0 pranavp   (1000) pranavp   (1000)        0 2023-07-19 05:56:30.435931 azure_speech_tools-0.0.4/azure_speech_tools.egg-info/
+-rw-r--r--   0 pranavp   (1000) pranavp   (1000)      183 2023-07-19 05:56:30.000000 azure_speech_tools-0.0.4/azure_speech_tools.egg-info/PKG-INFO
+-rw-r--r--   0 pranavp   (1000) pranavp   (1000)      558 2023-07-19 05:56:30.000000 azure_speech_tools-0.0.4/azure_speech_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 pranavp   (1000) pranavp   (1000)        1 2023-07-19 05:56:30.000000 azure_speech_tools-0.0.4/azure_speech_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 pranavp   (1000) pranavp   (1000)       78 2023-07-19 05:56:30.000000 azure_speech_tools-0.0.4/azure_speech_tools.egg-info/entry_points.txt
+-rw-r--r--   0 pranavp   (1000) pranavp   (1000)       65 2023-07-19 05:56:30.000000 azure_speech_tools-0.0.4/azure_speech_tools.egg-info/requires.txt
+-rw-r--r--   0 pranavp   (1000) pranavp   (1000)       19 2023-07-19 05:56:30.000000 azure_speech_tools-0.0.4/azure_speech_tools.egg-info/top_level.txt
+-rw-r--r--   0 pranavp   (1000) pranavp   (1000)       38 2023-07-19 05:56:30.445038 azure_speech_tools-0.0.4/setup.cfg
+-rw-r--r--   0 pranavp   (1000) pranavp   (1000)      543 2023-07-19 05:56:00.000000 azure_speech_tools-0.0.4/setup.py
```

### Comparing `azure_speech_tools-0.0.3/azure_speech_tools/tools/azure_speech_sr.py` & `azure_speech_tools-0.0.4/azure_speech_tools/tools/azure_speech_sr.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import os
 import tempfile
 from promptflow import tool
 from promptflow.connections import CustomConnection
 from azure.cognitiveservices.speech import SpeechConfig, SpeechRecognizer, AudioConfig
-from azure.storage.blob import BlobServiceClient
+from azure.storage.blob import BlobClient
 import uuid
 
 @tool
 def azure_speech_sr(connection: CustomConnection, input_blob_url: str, language: str = 'en-US') -> str:
     
     temp_dir = tempfile.gettempdir()
     file_name = str(uuid.uuid4()) + ".wav"
     file_path = os.path.join(temp_dir, file_name)
-    blob_client = BlobServiceClient.from_blob_url(input_blob_url)
+    shared_access_key = connection.azure_storage_access_key
+    credential = shared_access_key
+    blob_client = BlobClient.from_blob_url(input_blob_url, credential=credential)
     with open(file=file_path, mode="wb") as audio_file:
         download_stream = blob_client.download_blob()
         audio_file.write(download_stream.readall())
 
     audio_config = AudioConfig(filename=file_path)
     speech_config = SpeechConfig(subscription=connection.api_key, region=connection.api_region)
     speech_config.speech_recognition_language = language
```

### Comparing `azure_speech_tools-0.0.3/azure_speech_tools/tools/azure_speech_tts.py` & `azure_speech_tools-0.0.4/azure_speech_tools/tools/azure_speech_tts.py`

 * *Files identical despite different names*

### Comparing `azure_speech_tools-0.0.3/azure_speech_tools/tools/utils.py` & `azure_speech_tools-0.0.4/azure_speech_tools/tools/utils.py`

 * *Files identical despite different names*

### Comparing `azure_speech_tools-0.0.3/azure_speech_tools/yamls/azure_speech_tts.yaml` & `azure_speech_tools-0.0.4/azure_speech_tools/yamls/azure_speech_tts.yaml`

 * *Files identical despite different names*

### Comparing `azure_speech_tools-0.0.3/azure_speech_tools.egg-info/SOURCES.txt` & `azure_speech_tools-0.0.4/azure_speech_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azure_speech_tools-0.0.3/setup.py` & `azure_speech_tools-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="azure_speech_tools",
-    version="0.0.3",
+    version="0.0.4",
     description="This is the Azure Speech Services tools package",
     packages=find_packages(),
     install_requires=[
         "azure-cognitiveservices-speech",
         "azure-storage-blob",
         "azure-identity",
     ],
```

