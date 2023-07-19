# Comparing `tmp/nids_transformers-0.0.1.tar.gz` & `tmp/nids_transformers-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nids_transformers-0.0.1.tar", last modified: Wed Jul 19 01:17:48 2023, max compression
+gzip compressed data, was "nids_transformers-0.0.2.tar", last modified: Wed Jul 19 01:41:46 2023, max compression
```

## Comparing `nids_transformers-0.0.1.tar` & `nids_transformers-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,19 @@
-drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-19 01:17:48.058775 nids_transformers-0.0.1/
--rw-r--r--   0 rdp        (501) staff       (20)      515 2023-07-19 01:17:48.058608 nids_transformers-0.0.1/PKG-INFO
--rw-r--r--   0 rdp        (501) staff       (20)        0 2023-07-19 01:11:31.000000 nids_transformers-0.0.1/README.md
-drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-19 01:17:48.057487 nids_transformers-0.0.1/nids_transformers/
--rw-r--r--   0 rdp        (501) staff       (20)     9453 2023-07-19 00:50:51.000000 nids_transformers-0.0.1/nids_transformers/NIDSTransformers.py
--rw-r--r--   0 rdp        (501) staff       (20)       35 2023-07-19 00:52:36.000000 nids_transformers-0.0.1/nids_transformers/__init__.py
-drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-19 01:17:48.058412 nids_transformers-0.0.1/nids_transformers.egg-info/
--rw-r--r--   0 rdp        (501) staff       (20)      515 2023-07-19 01:17:48.000000 nids_transformers-0.0.1/nids_transformers.egg-info/PKG-INFO
--rw-r--r--   0 rdp        (501) staff       (20)      290 2023-07-19 01:17:48.000000 nids_transformers-0.0.1/nids_transformers.egg-info/SOURCES.txt
--rw-r--r--   0 rdp        (501) staff       (20)        1 2023-07-19 01:17:48.000000 nids_transformers-0.0.1/nids_transformers.egg-info/dependency_links.txt
--rw-r--r--   0 rdp        (501) staff       (20)      177 2023-07-19 01:17:48.000000 nids_transformers-0.0.1/nids_transformers.egg-info/requires.txt
--rw-r--r--   0 rdp        (501) staff       (20)       18 2023-07-19 01:17:48.000000 nids_transformers-0.0.1/nids_transformers.egg-info/top_level.txt
--rw-r--r--   0 rdp        (501) staff       (20)       38 2023-07-19 01:17:48.058830 nids_transformers-0.0.1/setup.cfg
--rw-r--r--   0 rdp        (501) staff       (20)      893 2023-07-19 01:13:00.000000 nids_transformers-0.0.1/setup.py
+drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-19 01:41:46.349203 nids_transformers-0.0.2/
+-rw-r--r--   0 rdp        (501) staff       (20)  5495089 2023-07-06 03:59:04.000000 nids_transformers-0.0.2/CORPUS.txt
+-rw-r--r--   0 rdp        (501) staff       (20)  1585280 2023-07-19 01:16:55.000000 nids_transformers-0.0.2/KMEANS-CLUSTER-CENTERS.npy
+-rw-r--r--   0 rdp        (501) staff       (20)      106 2023-07-19 01:27:32.000000 nids_transformers-0.0.2/MANIFEST.in
+-rw-r--r--   0 rdp        (501) staff       (20)      515 2023-07-19 01:41:46.348790 nids_transformers-0.0.2/PKG-INFO
+-rw-r--r--   0 rdp        (501) staff       (20)        0 2023-07-19 01:11:31.000000 nids_transformers-0.0.2/README.md
+-rw-r--r--   0 rdp        (501) staff       (20)    23489 2023-07-19 01:14:48.000000 nids_transformers-0.0.2/SCALER.pkl
+-rw-r--r--   0 rdp        (501) staff       (20)  3170432 2023-07-19 01:17:11.000000 nids_transformers-0.0.2/TAGS-NAMES-EMBEDDINGS.npy
+drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-19 01:41:46.347542 nids_transformers-0.0.2/nids_transformers/
+-rw-r--r--   0 rdp        (501) staff       (20)     9718 2023-07-19 01:40:10.000000 nids_transformers-0.0.2/nids_transformers/NIDSTransformers.py
+-rw-r--r--   0 rdp        (501) staff       (20)       35 2023-07-19 00:52:36.000000 nids_transformers-0.0.2/nids_transformers/__init__.py
+drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-19 01:41:46.348470 nids_transformers-0.0.2/nids_transformers.egg-info/
+-rw-r--r--   0 rdp        (501) staff       (20)      515 2023-07-19 01:41:46.000000 nids_transformers-0.0.2/nids_transformers.egg-info/PKG-INFO
+-rw-r--r--   0 rdp        (501) staff       (20)      377 2023-07-19 01:41:46.000000 nids_transformers-0.0.2/nids_transformers.egg-info/SOURCES.txt
+-rw-r--r--   0 rdp        (501) staff       (20)        1 2023-07-19 01:41:46.000000 nids_transformers-0.0.2/nids_transformers.egg-info/dependency_links.txt
+-rw-r--r--   0 rdp        (501) staff       (20)      177 2023-07-19 01:41:46.000000 nids_transformers-0.0.2/nids_transformers.egg-info/requires.txt
+-rw-r--r--   0 rdp        (501) staff       (20)       18 2023-07-19 01:41:46.000000 nids_transformers-0.0.2/nids_transformers.egg-info/top_level.txt
+-rw-r--r--   0 rdp        (501) staff       (20)       38 2023-07-19 01:41:46.349288 nids_transformers-0.0.2/setup.cfg
+-rw-r--r--   0 rdp        (501) staff       (20)      924 2023-07-19 01:41:33.000000 nids_transformers-0.0.2/setup.py
```

### Comparing `nids_transformers-0.0.1/PKG-INFO` & `nids_transformers-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nids_transformers
-Version: 0.0.1
+Version: 0.0.2
 Summary: Tag Generation and Text Generation for Network Packets using Transformers
 Home-page: https://github.com/rdpahalavan/BERTSimilarWords
 Author: Pahalavan R D
 Author-email: rdpahalavan24@gmail.com
 License: MIT
 Keywords: NIDS Transformers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nids_transformers-0.0.1/nids_transformers/NIDSTransformers.py` & `nids_transformers-0.0.2/nids_transformers/NIDSTransformers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import torch
 import pandas as pd
 from scapy.all import Ether, CookedLinux
 from BERTSimilar import SimilarWords
 import pickle
 import numpy as np
+import importlib.resources
 import re
 import string
 try:
     ipython = get_ipython()
     from tqdm.notebook import tqdm as tqdms
 except:
     from tqdm import tqdm as tqdms
@@ -20,21 +21,23 @@
     def __init__(self, tags=True, text=True):
         self.device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
         self.scaler_col_names = [str(i) for i in range(768)]
         self.packet = None
         self.tags = None
         self.payload_hex = None
         if tags:
-            with open('./SCALER.pkl', 'rb') as f:
+            with importlib.resources.open_binary('nids_transformers', 'SCALER.pkl') as f:
                 self.scaler = pickle.load(f)
             self.similar = SimilarWords(model='rdpahalavan/bert-network-packet-flow-header-payload',
                                         max_document_length=375, exclude_stopwords=['dos'],
-                                        embeddings_scaler=self.scaler).load_dataset(dataset_path='./CORPUS.txt')
-            self.cluster_centers = np.load('./KMEANS-CLUSTER-CENTERS.npy')
-            self.tag_names = np.load('./TAGS-NAMES-EMBEDDINGS.npy')
+                                        embeddings_scaler=self.scaler).load_dataset(dataset_path=importlib.resources.open_text('nids_transformers', 'CORPUS.txt'))
+            with importlib.resources.open_binary('my_package', 'KMEANS-CLUSTER-CENTERS.npy') as f:
+                self.cluster_centers = np.load(f)
+            with importlib.resources.open_binary('my_package', 'TAGS-NAMES-EMBEDDINGS.npy') as f:
+                self.tag_names = np.load(f)
         if text:
             for i in tqdms(range(1), unit=' it', desc='Provisioning', postfix='Text Generation Model'):
                 PEFT_MODEL = 'rdpahalavan/falcon-adapter-network-packet'
                 config = PeftConfig.from_pretrained(PEFT_MODEL)
                 self.model = AutoModelForCausalLM.from_pretrained(
                     config.base_model_name_or_path,
                     torch_dtype=torch.bfloat16,
```

### Comparing `nids_transformers-0.0.1/nids_transformers.egg-info/PKG-INFO` & `nids_transformers-0.0.2/nids_transformers.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nids-transformers
-Version: 0.0.1
+Version: 0.0.2
 Summary: Tag Generation and Text Generation for Network Packets using Transformers
 Home-page: https://github.com/rdpahalavan/BERTSimilarWords
 Author: Pahalavan R D
 Author-email: rdpahalavan24@gmail.com
 License: MIT
 Keywords: NIDS Transformers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nids_transformers-0.0.1/setup.py` & `nids_transformers-0.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().splitlines()
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name='nids_transformers',
-    version='0.0.1',
+    version='0.0.2',
     description="Tag Generation and Text Generation for Network Packets using Transformers",
     keywords="NIDS Transformers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
     author="Pahalavan R D",
     author_email='rdpahalavan24@gmail.com',
@@ -20,9 +20,10 @@
     python_requires='>=3.7.0',
     url='https://github.com/rdpahalavan/BERTSimilarWords',
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
+    include_package_data=True,
     install_requires=requirements
 )
```

