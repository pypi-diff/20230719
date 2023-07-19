# Comparing `tmp/MarsGT-0.1.6.tar.gz` & `tmp/MarsGT-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MarsGT-0.1.6.tar", last modified: Tue Jul 18 10:30:51 2023, max compression
+gzip compressed data, was "dist/MarsGT-0.1.7.tar", last modified: Wed Jul 19 01:33:44 2023, max compression
```

## Comparing `MarsGT-0.1.6.tar` & `MarsGT-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 duanmaoteng (40439) PCON0022  (6618)        0 2023-07-18 10:30:51.069644 MarsGT-0.1.6/
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)       34 2023-06-03 06:21:54.000000 MarsGT-0.1.6/MANIFEST.in
-drwxr-xr-x   0 duanmaoteng (40439) PCON0022  (6618)        0 2023-07-18 10:30:51.005649 MarsGT-0.1.6/MarsGT/
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)        2 2023-06-03 06:21:57.000000 MarsGT-0.1.6/MarsGT/__init__.py
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     6719 2023-06-03 08:36:23.000000 MarsGT-0.1.6/MarsGT/conv.py
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     8824 2023-07-18 10:28:20.000000 MarsGT-0.1.6/MarsGT/egrn.py
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)    21360 2023-06-03 08:36:23.000000 MarsGT-0.1.6/MarsGT/marsgt_model.py
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     7805 2023-07-18 10:28:36.000000 MarsGT-0.1.6/MarsGT/utils.py
-drwxr-xr-x   0 duanmaoteng (40439) PCON0022  (6618)        0 2023-07-18 10:30:51.057646 MarsGT-0.1.6/MarsGT.egg-info/
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     1091 2023-07-18 10:30:48.000000 MarsGT-0.1.6/MarsGT.egg-info/PKG-INFO
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)      267 2023-07-18 10:30:49.000000 MarsGT-0.1.6/MarsGT.egg-info/SOURCES.txt
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)        1 2023-07-18 10:30:48.000000 MarsGT-0.1.6/MarsGT.egg-info/dependency_links.txt
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)      406 2023-07-18 10:30:48.000000 MarsGT-0.1.6/MarsGT.egg-info/requires.txt
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)        7 2023-07-18 10:30:48.000000 MarsGT-0.1.6/MarsGT.egg-info/top_level.txt
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     1091 2023-07-18 10:30:51.068648 MarsGT-0.1.6/PKG-INFO
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)      730 2023-06-03 06:21:54.000000 MarsGT-0.1.6/README.md
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)       38 2023-07-18 10:30:51.070648 MarsGT-0.1.6/setup.cfg
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     1183 2023-07-18 10:30:06.000000 MarsGT-0.1.6/setup.py
+drwxr-xr-x   0 duanmaoteng (40439) PCON0022  (6618)        0 2023-07-19 01:33:44.586904 MarsGT-0.1.7/
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)       34 2023-06-03 06:21:54.000000 MarsGT-0.1.7/MANIFEST.in
+drwxr-xr-x   0 duanmaoteng (40439) PCON0022  (6618)        0 2023-07-19 01:33:44.545902 MarsGT-0.1.7/MarsGT/
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)        2 2023-06-03 06:21:57.000000 MarsGT-0.1.7/MarsGT/__init__.py
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     6719 2023-06-03 08:36:23.000000 MarsGT-0.1.7/MarsGT/conv.py
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     8824 2023-07-18 10:28:20.000000 MarsGT-0.1.7/MarsGT/egrn.py
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)    21360 2023-06-03 08:36:23.000000 MarsGT-0.1.7/MarsGT/marsgt_model.py
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     7805 2023-07-18 10:28:36.000000 MarsGT-0.1.7/MarsGT/utils.py
+drwxr-xr-x   0 duanmaoteng (40439) PCON0022  (6618)        0 2023-07-19 01:33:44.581912 MarsGT-0.1.7/MarsGT.egg-info/
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     1052 2023-07-19 01:33:44.000000 MarsGT-0.1.7/MarsGT.egg-info/PKG-INFO
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)      267 2023-07-19 01:33:44.000000 MarsGT-0.1.7/MarsGT.egg-info/SOURCES.txt
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)        1 2023-07-19 01:33:44.000000 MarsGT-0.1.7/MarsGT.egg-info/dependency_links.txt
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)      389 2023-07-19 01:33:44.000000 MarsGT-0.1.7/MarsGT.egg-info/requires.txt
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)        7 2023-07-19 01:33:44.000000 MarsGT-0.1.7/MarsGT.egg-info/top_level.txt
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     1052 2023-07-19 01:33:44.584911 MarsGT-0.1.7/PKG-INFO
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)      709 2023-07-19 01:31:01.000000 MarsGT-0.1.7/README.md
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)       38 2023-07-19 01:33:44.587901 MarsGT-0.1.7/setup.cfg
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     1165 2023-07-19 01:30:36.000000 MarsGT-0.1.7/setup.py
```

### Comparing `MarsGT-0.1.6/MarsGT/conv.py` & `MarsGT-0.1.7/MarsGT/conv.py`

 * *Files identical despite different names*

### Comparing `MarsGT-0.1.6/MarsGT/egrn.py` & `MarsGT-0.1.7/MarsGT/egrn.py`

 * *Files identical despite different names*

### Comparing `MarsGT-0.1.6/MarsGT/marsgt_model.py` & `MarsGT-0.1.7/MarsGT/marsgt_model.py`

 * *Files identical despite different names*

### Comparing `MarsGT-0.1.6/MarsGT/utils.py` & `MarsGT-0.1.7/MarsGT/utils.py`

 * *Files identical despite different names*

### Comparing `MarsGT-0.1.6/MarsGT.egg-info/PKG-INFO` & `MarsGT-0.1.7/MarsGT.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: MarsGT
-Version: 0.1.6
+Version: 0.1.7
 Summary: MarsGT: A Python library for rare cell identification (Internal testing only)
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: ==3.8.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: torch_sparse
 Provides-Extra: torch_scatter
 Provides-Extra: torch_cluster
 
 ## Title：MarsGT:Multi-omics data analysis for rare population inference using single-cell graph transformer
 **Note: This project is for internal testing purposes only. Do not use it in a production environment.**
 
-DeepMARS, for rare cell identification from matched scRNA-seq (snRNA-seq) and scATAC-seq (snATAC-seq),includes genes, enhancers, and cells in a heterogeneous graph to simultaneously identify major cell clusters and rare cell clusters based on eRegulon.
+MarsGT, for rare cell identification from matched scRNA-seq (snRNA-seq) and scATAC-seq (snATAC-seq),includes genes, enhancers, and cells in a heterogeneous graph to simultaneously identify major cell clusters and rare cell clusters based on eRegulon.
 ## Installation
 
 ### System Requirements
 
 * Python 3.8.0 or higher
 
 ### Installation Steps
@@ -26,9 +24,7 @@
 ```bash
 pip install -r requirements.txt
 ```
 * use pip to install MarsGT:
 ```bash
 pip install MarsGT
 ```
-
-
```

### Comparing `MarsGT-0.1.6/PKG-INFO` & `MarsGT-0.1.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: MarsGT
-Version: 0.1.6
+Version: 0.1.7
 Summary: MarsGT: A Python library for rare cell identification (Internal testing only)
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: ==3.8.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: torch_sparse
 Provides-Extra: torch_scatter
 Provides-Extra: torch_cluster
 
 ## Title：MarsGT:Multi-omics data analysis for rare population inference using single-cell graph transformer
 **Note: This project is for internal testing purposes only. Do not use it in a production environment.**
 
-DeepMARS, for rare cell identification from matched scRNA-seq (snRNA-seq) and scATAC-seq (snATAC-seq),includes genes, enhancers, and cells in a heterogeneous graph to simultaneously identify major cell clusters and rare cell clusters based on eRegulon.
+MarsGT, for rare cell identification from matched scRNA-seq (snRNA-seq) and scATAC-seq (snATAC-seq),includes genes, enhancers, and cells in a heterogeneous graph to simultaneously identify major cell clusters and rare cell clusters based on eRegulon.
 ## Installation
 
 ### System Requirements
 
 * Python 3.8.0 or higher
 
 ### Installation Steps
@@ -26,9 +24,7 @@
 ```bash
 pip install -r requirements.txt
 ```
 * use pip to install MarsGT:
 ```bash
 pip install MarsGT
 ```
-
-
```

### Comparing `MarsGT-0.1.6/setup.py` & `MarsGT-0.1.7/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
     
 setup(
     name="MarsGT",
-    version='0.1.6',
+    version='0.1.7',
     packages=find_packages(),
     install_requires=[
         'anndata==0.8.0',
         'dill==0.3.4',
         'matplotlib==3.5.1',
         'numpy==1.22.3',
         'pandas==1.4.2',
         'scipy==1.9.1',
         'seaborn==0.11.2',
         'scikit-learn==1.1.2',
-        'torch==1.12.0',
+        'torch==1.12.0+cpu',
         'torch-geometric==2.1.0.post1',
         'torchmetrics==0.9.3',
         'xlwt==1.3.0',
         'tqdm==4.64.0',
         'scanpy==1.9.1',
         'leidenalg==0.8.10',
         'ipywidgets==8.0.6'
     ],
     extras_require={
-        "torch_sparse": ["torch-sparse==0.6.15+pt112cu102"], 
-        "torch_scatter": ["torch-scatter==2.1.0+pt112cu102"],
-        "torch_cluster": ["torch-scatter==1.6.0+pt112cu102"]
+        "torch_sparse": ["torch-sparse==0.6.12+cpu"],
+        "torch_scatter": ["torch-scatter==2.0.9+cpu"],
+        "torch_cluster": ["torch-cluster==1.5.9+cpu"]
     },
-    python_requires='==3.8.0',
+    python_requires='>=3.8.0',
     description="MarsGT: A Python library for rare cell identification (Internal testing only)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "License :: OSI Approved :: MIT License"
     ]
 )
```

