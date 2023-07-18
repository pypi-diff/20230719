# Comparing `tmp/vector_vault-2.1.1.tar.gz` & `tmp/vector_vault-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-2.1.1.tar", last modified: Tue Jul 18 22:47:04 2023, max compression
+gzip compressed data, was "vector_vault-2.1.2.tar", last modified: Tue Jul 18 22:48:31 2023, max compression
```

## Comparing `vector_vault-2.1.1.tar` & `vector_vault-2.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-07-18 22:47:04.142625 vector_vault-2.1.1/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-2.1.1/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    27248 2023-07-18 22:47:04.142345 vector_vault-2.1.1/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    26538 2023-07-16 05:57:03.000000 vector_vault-2.1.1/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-07-18 22:47:04.142670 vector_vault-2.1.1/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1060 2023-07-18 22:46:47.000000 vector_vault-2.1.1/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-07-18 22:47:04.138528 vector_vault-2.1.1/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    27248 2023-07-18 22:47:04.000000 vector_vault-2.1.1/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      456 2023-07-18 22:47:04.000000 vector_vault-2.1.1/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-07-18 22:47:04.000000 vector_vault-2.1.1/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-07-18 22:47:04.000000 vector_vault-2.1.1/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-07-18 22:47:04.000000 vector_vault-2.1.1/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-07-18 22:47:04.142050 vector_vault-2.1.1/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-06-09 19:04:41.000000 vector_vault-2.1.1/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)    13294 2023-07-16 01:36:29.000000 vector_vault-2.1.1/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-06-27 02:14:51.000000 vector_vault-2.1.1/vectorvault/cloud_api.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3148 2023-07-18 22:45:16.000000 vector_vault-2.1.1/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1883 2023-06-08 04:35:26.000000 vector_vault-2.1.1/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-06-08 04:35:41.000000 vector_vault-2.1.1/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     2600 2023-07-18 22:45:26.000000 vector_vault-2.1.1/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)    16189 2023-06-10 21:42:18.000000 vector_vault-2.1.1/vectorvault/tools_gpt.py
--rw-r--r--   0 johnrood   (501) staff       (20)    36436 2023-07-18 22:45:52.000000 vector_vault-2.1.1/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     4084 2023-07-16 04:42:19.000000 vector_vault-2.1.1/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-2.1.1/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-07-18 22:48:31.278995 vector_vault-2.1.2/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-2.1.2/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    27248 2023-07-18 22:48:31.278867 vector_vault-2.1.2/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    26538 2023-07-16 05:57:03.000000 vector_vault-2.1.2/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-07-18 22:48:31.279033 vector_vault-2.1.2/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1060 2023-07-18 22:48:25.000000 vector_vault-2.1.2/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-07-18 22:48:31.274719 vector_vault-2.1.2/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    27248 2023-07-18 22:48:31.000000 vector_vault-2.1.2/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      456 2023-07-18 22:48:31.000000 vector_vault-2.1.2/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-07-18 22:48:31.000000 vector_vault-2.1.2/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-07-18 22:48:31.000000 vector_vault-2.1.2/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-07-18 22:48:31.000000 vector_vault-2.1.2/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-07-18 22:48:31.278514 vector_vault-2.1.2/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-06-09 19:04:41.000000 vector_vault-2.1.2/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    13294 2023-07-16 01:36:29.000000 vector_vault-2.1.2/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-06-27 02:14:51.000000 vector_vault-2.1.2/vectorvault/cloud_api.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3148 2023-07-18 22:45:16.000000 vector_vault-2.1.2/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1883 2023-06-08 04:35:26.000000 vector_vault-2.1.2/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-06-08 04:35:41.000000 vector_vault-2.1.2/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     2600 2023-07-18 22:45:26.000000 vector_vault-2.1.2/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    16190 2023-07-18 22:48:19.000000 vector_vault-2.1.2/vectorvault/tools_gpt.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    36436 2023-07-18 22:45:52.000000 vector_vault-2.1.2/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     4084 2023-07-16 04:42:19.000000 vector_vault-2.1.2/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-2.1.2/vectorvault/wrap.py
```

### Comparing `vector_vault-2.1.1/LICENSE` & `vector_vault-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.1/PKG-INFO` & `vector_vault-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 2.1.1
+Version: 2.1.2
 Summary: Vector Vault: Customize ChatGPT and unleash the full potential of generative AI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-2.1.1/README.md` & `vector_vault-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.1/setup.py` & `vector_vault-2.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="2.1.1",
+    version="2.1.2",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="Vector Vault: Customize ChatGPT and unleash the full potential of generative AI with Vector Vault",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-2.1.1/vector_vault.egg-info/PKG-INFO` & `vector_vault-2.1.2/vector_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 2.1.1
+Version: 2.1.2
 Summary: Vector Vault: Customize ChatGPT and unleash the full potential of generative AI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-2.1.1/vectorvault/ai.py` & `vector_vault-2.1.2/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.1/vectorvault/cloud_api.py` & `vector_vault-2.1.2/vectorvault/cloud_api.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.1/vectorvault/cloudmanager.py` & `vector_vault-2.1.2/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.1/vectorvault/creds.py` & `vector_vault-2.1.2/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.1/vectorvault/download.py` & `vector_vault-2.1.2/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.1/vectorvault/itemize.py` & `vector_vault-2.1.2/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.1/vectorvault/tools_gpt.py` & `vector_vault-2.1.2/vectorvault/tools_gpt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ai import AI
+from .ai import AI
 import time
 
 '''
     ToolsGPT is a set of tools special to large language models. 
     Every tool turns subjectivity into objectivity.
     
     Objectivity is needed for code.
```

### Comparing `vector_vault-2.1.1/vectorvault/vault.py` & `vector_vault-2.1.2/vectorvault/vault.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.1/vectorvault/vecreq.py` & `vector_vault-2.1.2/vectorvault/vecreq.py`

 * *Files identical despite different names*

