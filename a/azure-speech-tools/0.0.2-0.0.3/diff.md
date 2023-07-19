# Comparing `tmp/azure_speech_tools-0.0.2.tar.gz` & `tmp/azure_speech_tools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure_speech_tools-0.0.2.tar", last modified: Mon Jul 17 14:47:15 2023, max compression
+gzip compressed data, was "azure_speech_tools-0.0.3.tar", last modified: Wed Jul 19 05:37:40 2023, max compression
```

## Comparing `azure_speech_tools-0.0.2.tar` & `azure_speech_tools-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 pranavp   (1000) pranavp   (1000)        0 2023-07-17 14:47:15.246044 azure_speech_tools-0.0.2/
--rw-r--r--   0 pranavp   (1000) pranavp   (1000)       39 2023-07-17 09:45:25.000000 azure_speech_tools-0.0.2/MANIFEST.in
--rw-r--r--   0 pranavp   (1000) pranavp   (1000)      183 2023-07-17 14:47:15.246044 azure_speech_tools-0.0.2/PKG-INFO
-drwxr-xr-x   0 pranavp   (1000) pranavp   (1000)        0 2023-07-17 14:47:15.246044 azure_speech_tools-0.0.2/azure_speech_tools/
--rw-r--r--   0 pranavp   (1000) pranavp   (1000)       80 2023-07-17 09:44:29.000000 azure_speech_tools-0.0.2/azure_speech_tools/__init__.py
-drwxr-xr-x   0 pranavp   (1000) pranavp   (1000)        0 2023-07-17 14:47:15.246044 azure_speech_tools-0.0.2/azure_speech_tools/tools/
--rw-r--r--   0 pranavp   (1000) pranavp   (1000)       80 2023-07-17 09:46:09.000000 azure_speech_tools-0.0.2/azure_speech_tools/tools/__init__.py
--rw-r--r--   0 pranavp   (1000) pranavp   (1000)     1516 2023-07-17 14:10:46.000000 azure_speech_tools-0.0.2/azure_speech_tools/tools/azure_speech_tts.py
--rw-r--r--   0 pranavp   (1000) pranavp   (1000)      503 2023-07-17 10:04:13.000000 azure_speech_tools-0.0.2/azure_speech_tools/tools/utils.py
-drwxr-xr-x   0 pranavp   (1000) pranavp   (1000)        0 2023-07-17 14:47:15.246044 azure_speech_tools-0.0.2/azure_speech_tools/yamls/
--rw-r--r--   0 pranavp   (1000) pranavp   (1000)      601 2023-07-17 14:17:18.000000 azure_speech_tools-0.0.2/azure_speech_tools/yamls/azure_speech_tts.yaml
-drwxr-xr-x   0 pranavp   (1000) pranavp   (1000)        0 2023-07-17 14:47:15.246044 azure_speech_tools-0.0.2/azure_speech_tools.egg-info/
--rw-r--r--   0 pranavp   (1000) pranavp   (1000)      183 2023-07-17 14:47:15.000000 azure_speech_tools-0.0.2/azure_speech_tools.egg-info/PKG-INFO
--rw-r--r--   0 pranavp   (1000) pranavp   (1000)      468 2023-07-17 14:47:15.000000 azure_speech_tools-0.0.2/azure_speech_tools.egg-info/SOURCES.txt
--rw-r--r--   0 pranavp   (1000) pranavp   (1000)        1 2023-07-17 14:47:15.000000 azure_speech_tools-0.0.2/azure_speech_tools.egg-info/dependency_links.txt
--rw-r--r--   0 pranavp   (1000) pranavp   (1000)       78 2023-07-17 14:47:15.000000 azure_speech_tools-0.0.2/azure_speech_tools.egg-info/entry_points.txt
--rw-r--r--   0 pranavp   (1000) pranavp   (1000)       65 2023-07-17 14:47:15.000000 azure_speech_tools-0.0.2/azure_speech_tools.egg-info/requires.txt
--rw-r--r--   0 pranavp   (1000) pranavp   (1000)       19 2023-07-17 14:47:15.000000 azure_speech_tools-0.0.2/azure_speech_tools.egg-info/top_level.txt
--rw-r--r--   0 pranavp   (1000) pranavp   (1000)       38 2023-07-17 14:47:15.246044 azure_speech_tools-0.0.2/setup.cfg
--rw-r--r--   0 pranavp   (1000) pranavp   (1000)      543 2023-07-17 14:46:41.000000 azure_speech_tools-0.0.2/setup.py
+drwxr-xr-x   0 pranavp   (1000) pranavp   (1000)        0 2023-07-19 05:37:40.879226 azure_speech_tools-0.0.3/
+-rw-r--r--   0 pranavp   (1000) pranavp   (1000)       39 2023-07-17 09:45:25.000000 azure_speech_tools-0.0.3/MANIFEST.in
+-rw-r--r--   0 pranavp   (1000) pranavp   (1000)      183 2023-07-19 05:37:40.879226 azure_speech_tools-0.0.3/PKG-INFO
+drwxr-xr-x   0 pranavp   (1000) pranavp   (1000)        0 2023-07-19 05:37:40.879226 azure_speech_tools-0.0.3/azure_speech_tools/
+-rw-r--r--   0 pranavp   (1000) pranavp   (1000)       80 2023-07-17 09:44:29.000000 azure_speech_tools-0.0.3/azure_speech_tools/__init__.py
+drwxr-xr-x   0 pranavp   (1000) pranavp   (1000)        0 2023-07-19 05:37:40.879226 azure_speech_tools-0.0.3/azure_speech_tools/tools/
+-rw-r--r--   0 pranavp   (1000) pranavp   (1000)       80 2023-07-17 09:46:09.000000 azure_speech_tools-0.0.3/azure_speech_tools/tools/__init__.py
+-rw-r--r--   0 pranavp   (1000) pranavp   (1000)     1113 2023-07-19 05:29:14.000000 azure_speech_tools-0.0.3/azure_speech_tools/tools/azure_speech_sr.py
+-rw-r--r--   0 pranavp   (1000) pranavp   (1000)     1516 2023-07-17 14:10:46.000000 azure_speech_tools-0.0.3/azure_speech_tools/tools/azure_speech_tts.py
+-rw-r--r--   0 pranavp   (1000) pranavp   (1000)      568 2023-07-17 17:25:13.000000 azure_speech_tools-0.0.3/azure_speech_tools/tools/utils.py
+drwxr-xr-x   0 pranavp   (1000) pranavp   (1000)        0 2023-07-19 05:37:40.879226 azure_speech_tools-0.0.3/azure_speech_tools/yamls/
+-rw-r--r--   0 pranavp   (1000) pranavp   (1000)      494 2023-07-19 05:33:45.000000 azure_speech_tools-0.0.3/azure_speech_tools/yamls/azure_speech_sr.yaml
+-rw-r--r--   0 pranavp   (1000) pranavp   (1000)      623 2023-07-19 05:15:47.000000 azure_speech_tools-0.0.3/azure_speech_tools/yamls/azure_speech_tts.yaml
+drwxr-xr-x   0 pranavp   (1000) pranavp   (1000)        0 2023-07-19 05:37:40.879226 azure_speech_tools-0.0.3/azure_speech_tools.egg-info/
+-rw-r--r--   0 pranavp   (1000) pranavp   (1000)      183 2023-07-19 05:37:40.000000 azure_speech_tools-0.0.3/azure_speech_tools.egg-info/PKG-INFO
+-rw-r--r--   0 pranavp   (1000) pranavp   (1000)      558 2023-07-19 05:37:40.000000 azure_speech_tools-0.0.3/azure_speech_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 pranavp   (1000) pranavp   (1000)        1 2023-07-19 05:37:40.000000 azure_speech_tools-0.0.3/azure_speech_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 pranavp   (1000) pranavp   (1000)       78 2023-07-19 05:37:40.000000 azure_speech_tools-0.0.3/azure_speech_tools.egg-info/entry_points.txt
+-rw-r--r--   0 pranavp   (1000) pranavp   (1000)       65 2023-07-19 05:37:40.000000 azure_speech_tools-0.0.3/azure_speech_tools.egg-info/requires.txt
+-rw-r--r--   0 pranavp   (1000) pranavp   (1000)       19 2023-07-19 05:37:40.000000 azure_speech_tools-0.0.3/azure_speech_tools.egg-info/top_level.txt
+-rw-r--r--   0 pranavp   (1000) pranavp   (1000)       38 2023-07-19 05:37:40.879226 azure_speech_tools-0.0.3/setup.cfg
+-rw-r--r--   0 pranavp   (1000) pranavp   (1000)      543 2023-07-19 05:37:00.000000 azure_speech_tools-0.0.3/setup.py
```

### Comparing `azure_speech_tools-0.0.2/azure_speech_tools/tools/azure_speech_tts.py` & `azure_speech_tools-0.0.3/azure_speech_tools/tools/azure_speech_tts.py`

 * *Files identical despite different names*

### Comparing `azure_speech_tools-0.0.2/azure_speech_tools/yamls/azure_speech_tts.yaml` & `azure_speech_tools-0.0.3/azure_speech_tools/yamls/azure_speech_tts.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -14,10 +14,10 @@
       type:
       - string
     voice_name:
       default: en-us-jennyneural
       type:
       - string
   module: azure_speech_tools.tools.azure_speech_tts
-  name: Azure Speech Service TTS
-  description: This tool uses the Azure Speech Service to convert text to speech and upload the result to a blob.
+  name: Azure AI Text-To-Speech Service
+  description: This tool uses the Azure AI services to convert text to speech and upload the result to an Azure storage account.
   type: python
```

### Comparing `azure_speech_tools-0.0.2/setup.py` & `azure_speech_tools-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="azure_speech_tools",
-    version="0.0.2",
+    version="0.0.3",
     description="This is the Azure Speech Services tools package",
     packages=find_packages(),
     install_requires=[
         "azure-cognitiveservices-speech",
         "azure-storage-blob",
         "azure-identity",
     ],
```

