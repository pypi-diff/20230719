# Comparing `tmp/stanscofi-1.1.0.tar.gz` & `tmp/stanscofi-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stanscofi-1.1.0.tar", last modified: Fri Jun 30 16:51:54 2023, max compression
+gzip compressed data, was "stanscofi-2.0.0.tar", last modified: Wed Jul 19 12:00:08 2023, max compression
```

## Comparing `stanscofi-1.1.0.tar` & `stanscofi-2.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:54.115854 stanscofi-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-06-30 16:51:54.115854 stanscofi-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-06-30 16:51:43.000000 stanscofi-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-30 16:51:43.000000 stanscofi-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 16:51:54.115854 stanscofi-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-30 16:51:44.000000 stanscofi-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:54.111854 stanscofi-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:54.115854 stanscofi-1.1.0/src/stanscofi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:43.000000 stanscofi-1.1.0/src/stanscofi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27734 2023-06-30 16:51:43.000000 stanscofi-1.1.0/src/stanscofi/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    19202 2023-06-30 16:51:43.000000 stanscofi-1.1.0/src/stanscofi/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    19340 2023-06-30 16:51:43.000000 stanscofi-1.1.0/src/stanscofi/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    19399 2023-06-30 16:51:43.000000 stanscofi-1.1.0/src/stanscofi/training_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    20389 2023-06-30 16:51:43.000000 stanscofi-1.1.0/src/stanscofi/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10978 2023-06-30 16:51:43.000000 stanscofi-1.1.0/src/stanscofi/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:54.115854 stanscofi-1.1.0/src/stanscofi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-06-30 16:51:54.000000 stanscofi-1.1.0/src/stanscofi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-30 16:51:54.000000 stanscofi-1.1.0/src/stanscofi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 16:51:54.000000 stanscofi-1.1.0/src/stanscofi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-30 16:51:54.000000 stanscofi-1.1.0/src/stanscofi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-30 16:51:54.000000 stanscofi-1.1.0/src/stanscofi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:00:08.767777 stanscofi-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6559 2023-07-19 12:00:08.763777 stanscofi-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-07-19 11:59:57.000000 stanscofi-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-19 11:59:57.000000 stanscofi-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 12:00:08.767777 stanscofi-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-19 11:59:58.000000 stanscofi-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:00:08.763777 stanscofi-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:00:08.763777 stanscofi-2.0.0/src/stanscofi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 11:59:57.000000 stanscofi-2.0.0/src/stanscofi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27484 2023-07-19 11:59:57.000000 stanscofi-2.0.0/src/stanscofi/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17051 2023-07-19 11:59:57.000000 stanscofi-2.0.0/src/stanscofi/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19372 2023-07-19 11:59:57.000000 stanscofi-2.0.0/src/stanscofi/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20417 2023-07-19 11:59:57.000000 stanscofi-2.0.0/src/stanscofi/training_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20459 2023-07-19 11:59:57.000000 stanscofi-2.0.0/src/stanscofi/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13228 2023-07-19 11:59:57.000000 stanscofi-2.0.0/src/stanscofi/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:00:08.763777 stanscofi-2.0.0/src/stanscofi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6559 2023-07-19 12:00:08.000000 stanscofi-2.0.0/src/stanscofi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-19 12:00:08.000000 stanscofi-2.0.0/src/stanscofi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 12:00:08.000000 stanscofi-2.0.0/src/stanscofi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-19 12:00:08.000000 stanscofi-2.0.0/src/stanscofi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-19 12:00:08.000000 stanscofi-2.0.0/src/stanscofi.egg-info/top_level.txt
```

### Comparing `stanscofi-1.1.0/PKG-INFO` & `stanscofi-2.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stanscofi
-Version: 1.1.0
+Version: 2.0.0
 Summary: Package for STANdard drug Screening by COllaborative FIltering. Performs benchmarks against datasets and SotA algorithms, and implements training, validation and testing procedures.
 Home-page: https://github.com/RECeSS-EU-Project/stanscofi
 Author: Clémence Réda
 Author-email: recess-project@proton.me
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -14,15 +14,15 @@
 
 ![funding logo](https://raw.githubusercontent.com/RECeSS-EU-Project/RECeSS-EU-Project.github.io/main/assets/images/header%2BEU_rescale.jpg)
 
 # STANdard for drug Screening by COllaborative FIltering (stanscofi) Python Package
 
 This repository is a part of the EU-funded [RECeSS project](https://recess-eu-project.github.io) (#101102016), and hosts the code for the open-source Python package *stanscofi* for the development of collaborative filtering-based drug repurposing algorithms.
 
-[![Python Version](https://img.shields.io/badge/python-3.8%7C3.9%7C3.10-pink)](https://badge.fury.io/py/stanscofi) [![PyPI version](https://img.shields.io/pypi/v/stanscofi.svg)](https://badge.fury.io/py/stanscofi) [![Anaconda version](https://anaconda.org/recess/stanscofi/badges/version.svg)](https://anaconda.org/recess/stanscofi) [![Zenodo version](https://zenodo.org/badge/DOI/10.5281/zenodo.8038847.svg)](https://doi.org/10.5281/zenodo.8038847) ![GitHub](https://img.shields.io/github/license/recess-eu-project/stanscofi.svg) [![Build Status](https://github.com/recess-eu-project/stanscofi/actions/workflows/post-push-test.yml/badge.svg)](https://github.com/recess-eu-project/stanscofi/actions/workflows/post-push-test.yml) [![Codecov](https://codecov.io/github/recess-eu-project/stanscofi/coverage.svg?branch=master)](https://codecov.io/github/recess-eu-project/stanscofi?branch=master) [![Codefactor](https://www.codefactor.io/repository/github/recess-eu-project/stanscofi/badge?style=plastic)](https://www.codefactor.io/repository/github/recess-eu-project/stanscofi)
+[![Python Version](https://img.shields.io/badge/python-3.8%7C3.9-pink)](https://badge.fury.io/py/stanscofi) [![PyPI version](https://img.shields.io/pypi/v/stanscofi.svg)](https://badge.fury.io/py/stanscofi) [![Anaconda version](https://anaconda.org/recess/stanscofi/badges/version.svg)](https://anaconda.org/recess/stanscofi) [![Zenodo version](https://zenodo.org/badge/DOI/10.5281/zenodo.8038847.svg)](https://doi.org/10.5281/zenodo.8038847) ![GitHub](https://img.shields.io/github/license/recess-eu-project/stanscofi.svg) [![Build Status](https://github.com/recess-eu-project/stanscofi/actions/workflows/post-push-test.yml/badge.svg)](https://github.com/recess-eu-project/stanscofi/actions/workflows/post-push-test.yml) [![Codecov](https://codecov.io/github/recess-eu-project/stanscofi/coverage.svg?branch=master)](https://codecov.io/github/recess-eu-project/stanscofi?branch=master) [![Codefactor](https://www.codefactor.io/repository/github/recess-eu-project/stanscofi/badge?style=plastic)](https://www.codefactor.io/repository/github/recess-eu-project/stanscofi)
 
 ## Statement of need 
 
 As of 2022, current drug development pipelines last around 10 years, costing $2billion in average, while drug commercialization failure rates go up to 90%. These issues can be mitigated by drug repurposing, where chemical compounds are screened for new therapeutic indications in a systematic fashion. In prior works, this approach has been implemented through collaborative filtering. This semi-supervised learning framework leverages known drug-disease matchings in order to recommend new ones.
 
 The **stanscofi** package comprises method-agnostic training, validation, preprocessing and visualization procedures on several published drug repurposing datasets. The proper implementation of these steps is crucial in order to avoid data leakage, *i*.*e*., the model is learnt over information that should be unavailable at prediction time. Indeed, data leakage is the source of a major reproducibility crisis in machine learning. This will be avoided by building training and validation sets which are weakly correlated with respect to the drug and disease feature vectors. The main performance metric will be the area under the curve (AUC), which estimates the diagnostic ability of a recommender system better than accuracy in imbalanced datasets.
 
@@ -50,15 +50,15 @@
 
 Once installed, to import **stanscofi** into your Python code
 
 ```
 import stanscofi
 ```
 
-Please check out notebook *Introduction to stanscofi.ipynb*. All functions are documented, so one can check out the inputs and outputs of a function func by typing
+Please check out notebook *Introduction to stanscofi.ipynb*. Documentation about **stanscofi** can be found at [this page](https://recess-eu-project.github.io/stanscofi/). All functions are documented, so one can check out the inputs and outputs of a function func by typing
 
 ```
 help(func)
 ```
 
 To mesure your environmental impact when using this package (in terms of carbon emissions), please run the following command
```

### Comparing `stanscofi-1.1.0/README.md` & `stanscofi-2.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ![funding logo](https://raw.githubusercontent.com/RECeSS-EU-Project/RECeSS-EU-Project.github.io/main/assets/images/header%2BEU_rescale.jpg)
 
 # STANdard for drug Screening by COllaborative FIltering (stanscofi) Python Package
 
 This repository is a part of the EU-funded [RECeSS project](https://recess-eu-project.github.io) (#101102016), and hosts the code for the open-source Python package *stanscofi* for the development of collaborative filtering-based drug repurposing algorithms.
 
-[![Python Version](https://img.shields.io/badge/python-3.8%7C3.9%7C3.10-pink)](https://badge.fury.io/py/stanscofi) [![PyPI version](https://img.shields.io/pypi/v/stanscofi.svg)](https://badge.fury.io/py/stanscofi) [![Anaconda version](https://anaconda.org/recess/stanscofi/badges/version.svg)](https://anaconda.org/recess/stanscofi) [![Zenodo version](https://zenodo.org/badge/DOI/10.5281/zenodo.8038847.svg)](https://doi.org/10.5281/zenodo.8038847) ![GitHub](https://img.shields.io/github/license/recess-eu-project/stanscofi.svg) [![Build Status](https://github.com/recess-eu-project/stanscofi/actions/workflows/post-push-test.yml/badge.svg)](https://github.com/recess-eu-project/stanscofi/actions/workflows/post-push-test.yml) [![Codecov](https://codecov.io/github/recess-eu-project/stanscofi/coverage.svg?branch=master)](https://codecov.io/github/recess-eu-project/stanscofi?branch=master) [![Codefactor](https://www.codefactor.io/repository/github/recess-eu-project/stanscofi/badge?style=plastic)](https://www.codefactor.io/repository/github/recess-eu-project/stanscofi)
+[![Python Version](https://img.shields.io/badge/python-3.8%7C3.9-pink)](https://badge.fury.io/py/stanscofi) [![PyPI version](https://img.shields.io/pypi/v/stanscofi.svg)](https://badge.fury.io/py/stanscofi) [![Anaconda version](https://anaconda.org/recess/stanscofi/badges/version.svg)](https://anaconda.org/recess/stanscofi) [![Zenodo version](https://zenodo.org/badge/DOI/10.5281/zenodo.8038847.svg)](https://doi.org/10.5281/zenodo.8038847) ![GitHub](https://img.shields.io/github/license/recess-eu-project/stanscofi.svg) [![Build Status](https://github.com/recess-eu-project/stanscofi/actions/workflows/post-push-test.yml/badge.svg)](https://github.com/recess-eu-project/stanscofi/actions/workflows/post-push-test.yml) [![Codecov](https://codecov.io/github/recess-eu-project/stanscofi/coverage.svg?branch=master)](https://codecov.io/github/recess-eu-project/stanscofi?branch=master) [![Codefactor](https://www.codefactor.io/repository/github/recess-eu-project/stanscofi/badge?style=plastic)](https://www.codefactor.io/repository/github/recess-eu-project/stanscofi)
 
 ## Statement of need 
 
 As of 2022, current drug development pipelines last around 10 years, costing $2billion in average, while drug commercialization failure rates go up to 90%. These issues can be mitigated by drug repurposing, where chemical compounds are screened for new therapeutic indications in a systematic fashion. In prior works, this approach has been implemented through collaborative filtering. This semi-supervised learning framework leverages known drug-disease matchings in order to recommend new ones.
 
 The **stanscofi** package comprises method-agnostic training, validation, preprocessing and visualization procedures on several published drug repurposing datasets. The proper implementation of these steps is crucial in order to avoid data leakage, *i*.*e*., the model is learnt over information that should be unavailable at prediction time. Indeed, data leakage is the source of a major reproducibility crisis in machine learning. This will be avoided by building training and validation sets which are weakly correlated with respect to the drug and disease feature vectors. The main performance metric will be the area under the curve (AUC), which estimates the diagnostic ability of a recommender system better than accuracy in imbalanced datasets.
 
@@ -36,15 +36,15 @@
 
 Once installed, to import **stanscofi** into your Python code
 
 ```
 import stanscofi
 ```
 
-Please check out notebook *Introduction to stanscofi.ipynb*. All functions are documented, so one can check out the inputs and outputs of a function func by typing
+Please check out notebook *Introduction to stanscofi.ipynb*. Documentation about **stanscofi** can be found at [this page](https://recess-eu-project.github.io/stanscofi/). All functions are documented, so one can check out the inputs and outputs of a function func by typing
 
 ```
 help(func)
 ```
 
 To mesure your environmental impact when using this package (in terms of carbon emissions), please run the following command
```

### Comparing `stanscofi-1.1.0/setup.py` & `stanscofi-2.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 NAME = "stanscofi"
-VERSION = "1.1.0"
+VERSION = "2.0.0"
 
 setup(name=NAME,
     version=VERSION,
     author="Clémence Réda",
     author_email="recess-project@proton.me",
     url="https://github.com/RECeSS-EU-Project/stanscofi",
     license_files = ('LICENSE'),
@@ -29,11 +29,13 @@
         "scipy>=1.5.4",
         "matplotlib>=3.3.2",
         "threadpoolctl>=3.1.0",
         "joblib>=1.0.1",
         "tqdm>=4.58.0",
         "codecarbon>=2.2.2",
         "seaborn>=0.11.0",
+        "cute-ranking>=0.0.3",
         "umap-learn>=0.5.3",
+        "fastcluster>=1.2.6",
     ],
     entry_points={},
 )
```

### Comparing `stanscofi-1.1.0/src/stanscofi/datasets.py` & `stanscofi-2.0.0/src/stanscofi/datasets.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #coding: utf-8
 
 import pandas as pd
 import numpy as np
+from scipy.sparse import coo_array, csr_array
 import seaborn as sns
 
 import matplotlib.pyplot as plt
 import matplotlib.lines as mlines
 
 from sklearn.decomposition import PCA
 import warnings
 with warnings.catch_warnings():
     warnings.filterwarnings("ignore", message=".*he 'nopython' keyword argument was not supplied to the 'numba.jit' decorator.*")
     import umap
 
-import stanscofi.utils
-import stanscofi.preprocessing
+from .preprocessing import meanimputation_standardize
 
 def generate_dummy_dataset(npositive, nnegative, nfeatures, mean, std, random_state=12454):
     '''
     Creates a dummy dataset where the positive and negative (item, user) pairs are arbitrarily similar. 
 
     Each of the nfeatures features for (item, user) pair feature vectors associated with positive ratings are drawn from a Gaussian distribution of mean mean and standard deviation std, whereas those for negative ratings are drawn from from a Gaussian distribution of mean -mean and standard deviation std. User and item feature matrices of shape (nfeatures//2, npositive+nnegative) are generated, which are the concatenation of npositive positive and nnegative negative pair feature vectors generated from Gaussian distributions. Thus there are npositive^2 positive ratings (each "positive" user with a "positive" item), nnegative^2 negative ratings (idem), and the remainder is unknown (that is, (npositive+nnegative)^2-npositive^2-nnegative^2 ratings).
 
@@ -35,15 +35,15 @@
     mean : float
         mean of generating Gaussian distributions
     std : float
         standard deviation of generating Gaussian distributions
 
     Returns
     ----------
-    ratings_mat : array-like of shape (n_items, n_users)
+    ratings : array-like of shape (n_items, n_users)
         a matrix which contains values in {-1, 0, 1} describing the known and unknown user-item matchings
     users : array-like of shape (n_item_features, n_items)
         a list of the item feature names in the order of column indices in ratings_mat
     items : array-like of shape (n_user_features, n_users)
         a list of the item feature names in the order of column indices in ratings_mat
     '''
     assert nfeatures%2==0
@@ -51,166 +51,215 @@
     ## Generate feature matrices
     nusers = nitems = npositive+nnegative
     positive = np.random.normal(mean,std,size=(nfeatures,npositive))
     negative = np.random.normal(-mean,std,size=(nfeatures,nnegative))
     users = np.concatenate((positive, negative), axis=1)[:nfeatures//2,:]
     items = np.concatenate((positive, negative), axis=1)[nfeatures//2:,:]
     ## Generate ratings
-    ratings = np.zeros((nitems*nusers, 3))
-    ids = np.argwhere(np.ones((nitems, nusers)))
-    ratings[:,0] = ids[:,0]
-    ratings[:,1] = ids[:,1]
-    positive = (ratings[:,0]<npositive)&(ratings[:,1]<npositive)
-    negative_u = (ratings[:,0]>=npositive)&(ratings[:,0]<nnegative+npositive+1)
-    negative_i = (ratings[:,1]>=npositive)&(ratings[:,1]<nnegative+npositive+1)
-    ratings[positive,2] = 1
-    ratings[negative_u&negative_i,2] = -1
-    ratings = pd.DataFrame(ratings, columns=["user","item","rating"], index=range(ratings.shape[0]))
+    ratings = np.zeros((nitems, nusers))
+    ratings[:npositive,:npositive] = 1
+    ratings[npositive:,npositive:] = -1
     ## Input to stanscofi
-    ratings_mat = stanscofi.utils.ratings2matrix(ratings, user_col="user", item_col="item", rating_col="rating")
-    users = pd.DataFrame(users, index=range(nfeatures//2), columns=range(nusers))
-    items = pd.DataFrame(items, index=range(nfeatures//2), columns=range(nitems))
-    return {"ratings_mat": ratings_mat, "users": users, "items": items}
+    return {"ratings": coo_array(ratings), "users": users, "items": items}
 
 class Dataset(object):
     '''
-    A class used to encode a drug repurposing dataset
+    A class used to encode a drug repurposing dataset (items are drugs, users are diseases)
 
     ...
 
     Parameters
     ----------
-    ratings_mat : array-like of shape (n_items, n_users)
-        a matrix which contains values in {-1, 0, 1} describing the known and unknown user-item matchings
-    users : array-like of shape (n_item_features, n_items)
-        a list of the item feature names in the order of column indices in ratings_mat
-    items : array-like of shape (n_user_features, n_users)
-        a list of the item feature names in the order of column indices in ratings_mat
-    same_item_user_features : bool
-        a list of the item feature names in the order of column indices in ratings_mat
+    ratings : array-like of shape (n_items, n_users)
+        an array which contains values in {-1, 0, 1, np.nan} describing the negative, unlabelled, positive, unavailable user-item matchings
+    items : array-like of shape (n_item_features, n_items)
+        an array which contains the item feature vectors
+    users : array-like of shape (n_user_features, n_users)
+        an array which contains the user feature vectors
+    same_item_user_features : bool (default: False)
+        whether the item and user features are the same (optional)
     name : str
-        the name of the dataset (if it exists)
-    folds : array-like of shape (n_ratings, 3)
-        a matrix which contains the user indices (column 1), the item indices (column 2) and the class for the corresponding (user, item) pair (value in {-1, 0, 1} in column 3) (if the dataset is masked, see below)
+        name of the dataset (optional)
 
     Attributes
     ----------
     name : str
-        the name of the dataset (if it exists)
-    ratings_mat : array-like of shape (n_items, n_users)
-        a matrix which contains values in {-1, 0, 1} describing the known and unknown user-item matchings
-    users : array-like of shape (n_item_features, n_items)
-        a list of the item feature names in the order of column indices in ratings_mat
-    items : array-like of shape (n_user_features, n_users)
-        a list of the item feature names in the order of column indices in ratings_mat
+        name of the dataset 
+    ratings : COO-array of shape (n_items, n_users)
+        an array which contains values in {-1, 0, 1} describing the negative, unlabelled/unavailable, positive user-item matchings
+    folds : COO-array of shape (n_items, n_users)
+        an array which contains values in {0, 1} describing the unavailable and available user-item matchings in ratings
+    items : COO-array of shape (n_item_features, n_items)
+        an array which contains the user feature vectors (NaN for missing features)
+    users : COO-array of shape (n_user_features, n_users)
+        an array which contains the item feature vectors (NaN for missing features)
     item_list : list of str
         a list of the item names in the order of row indices in ratings_mat
     user_list : list of str
-        a list of the item names in the order of column indices in ratings_mat
+        a list of the user names in the order of column indices in ratings_mat
     item_features : list of str
         a list of the item feature names in the order of column indices in ratings_mat
     user_features : list of str
-        a list of the item feature names in the order of column indices in ratings_mat
-    ratings : array-like of shape (n_ratings, 3)
-        a list of the item feature names in the order of column indices in ratings_mat
+        a list of the user feature names in the order of column indices in ratings_mat
     same_item_user_features : bool
-        a list of the item feature names in the order of column indices in ratings_mat
+        whether the item and user features are the same
+    nusers : int
+        number of users
+    nitems : int
+        number of items
+    nuser_features : int
+        number of user features
+    nitem_features : int
+        number of item features
 
     Methods
     -------
-    __init__(ratings_mat=None, users=None, items=None, same_item_user_features=False, name="dataset")
+    __init__(ratings=None, users=None, items=None, same_item_user_features=False, name="dataset")
         Initialize the Dataset object and creates all attributes
     summary(sep="-"*70)
         Prints out the characteristics of the drug repurposing dataset
     visualize(withzeros=False, X=None, y=None, figsize=(5,5), fontsize=20, dimred_args={}, predictions=None, use_ratings=False, random_state=1234, show_errors=False, verbose=False)
         Plots datapoints in the dataset annotated by the ground truth or predicted ratings
-    get_folds(folds, subset_name="subset")
+    subset(folds, subset_name="subset")
         Creates a subset of the dataset based on the folds given as input
-    mask_dataset(folds, subset_name="dataset")
-        Creates a masked dataset where only some of the ratings are known
     '''
-    def __init__(self, ratings_mat=None, users=None, items=None, same_item_user_features=False, name="dataset", folds=None):
+    def __init__(self, ratings=None, users=None, items=None, same_item_user_features=False, name="dataset"):
         '''
         Creates an instance of stanscofi.Dataset
 
         ...
 
         Parameters
         ----------
-        ratings_mat : array-like of shape (n_items, n_users)
-            a matrix which contains values in {-1, 0, 1} describing the known and unknown user-item matchings
-        users : array-like of shape (n_item_features, n_items)
-            a list of the item feature names in the order of column indices in ratings_mat
-        items : array-like of shape (n_user_features, n_users)
-            a list of the item feature names in the order of column indices in ratings_mat
-        same_item_user_features : bool
-            a list of the item feature names in the order of column indices in ratings_mat
+        ratings : array-like of shape (n_items, n_users)
+            an array which contains values in {-1, 0, 1, np.nan} describing the negative, unlabelled, positive, unavailable user-item matchings
+        items : array-like of shape (n_item_features, n_items)
+            an array which contains the item feature vectors
+        users : array-like of shape (n_user_features, n_users)
+            an array which contains the user feature vectors
+        same_item_user_features : bool (default: False)
+            whether the item and user features are the same (optional)
         name : str
-            the name of the dataset (if it exists)
+            name of the dataset (optional)
         '''
-        assert ratings_mat is not None
-        assert users is not None
-        assert items is not None
-        self.item_list = list(ratings_mat.index)
-        self.user_list = list(ratings_mat.columns)
-        users = users[self.user_list]
-        items = items[self.item_list]
-        if (same_item_user_features):
-            features = list(set(list(users.index)).intersection(set(list(items.index))))
+        assert ratings is not None
+        assert users is not None and users.shape[1]==ratings.shape[1]
+        assert items is not None and items.shape[1]==ratings.shape[0]
+        ## get metadata
+        if (str(type(ratings))=="<class 'pandas.core.frame.DataFrame'>"):
+            self.item_list = [str(x) for x in ratings.index]
+            self.user_list = [str(x) for x in ratings.columns]
+            ratings_ = ratings.values
+        else:
+            self.item_list = [str(x) for x in range(ratings.shape[0])]
+            self.user_list = [str(x) for x in range(ratings.shape[1])]
+            if (str(type(ratings))=="<class 'scipy.sparse._arrays.coo_array'>"):
+                ratings_ = ratings.toarray()
+            else:
+                ratings_ = ratings.copy()
+            ratings_ = ratings_.copy()
+        if (str(type(users))=="<class 'pandas.core.frame.DataFrame'>"):
+            users = users[self.user_list]
+            self.user_features = [str(x) for x in users.index]
+            users_ = users.values
+        else:
+            self.user_features = [str(x) for x in range(users.shape[0])]
+            users_ = users.copy()
+        if (str(type(items))=="<class 'pandas.core.frame.DataFrame'>"):
+            items = items[self.item_list]
+            self.item_features = [str(x) for x in items.index]
+            items_ = items.values
+        else:
+            self.item_features = [str(x) for x in range(items.shape[0])]
+            items_ = items.copy()
+        self.same_item_user_features = same_item_user_features
+        if (self.same_item_user_features):
+            features = list(set(self.item_features).intersection(set(self.user_features)))
             assert len(features)>0
             self.user_features = features
             self.item_features = features
             users = users.loc[features]
             items = items.loc[features]
-        else:
-            self.user_features = list(users.index)
-            self.item_features = list(items.index)
-        self.ratings_mat = ratings_mat.values
-        self.ratings = stanscofi.utils.matrix2ratings(ratings_mat, user_col="ind_id", item_col="drug_id", rating_col="rating").values
-        assert all([a in users.columns for a in self.ratings[:,0]])
-        assert all([a in items.columns for a in self.ratings[:,1]])
-        self.ratings[:,0] = [self.user_list.index(x) for x in self.ratings[:,0]] 
-        self.ratings[:,1] = [self.item_list.index(x) for x in self.ratings[:,1]] 
-        self.users = users.values
-        self.items = items.values
+        ## format
         self.name = name
-        self.same_item_user_features = same_item_user_features
-        self.folds = folds
+        self.ratings = coo_array(np.nan_to_num(ratings_, copy=True, nan=0))
+        ids = np.argwhere(~np.isnan(ratings_))
+        row = ids[:,0].ravel()
+        col = ids[:,1].ravel()
+        data = [1]*ids.shape[0]
+        self.folds = coo_array((data, (row, col)), shape=ratings_.shape)
+        self.users = coo_array(users_)
+        self.items = coo_array(items_)
+        self.nusers = self.users.shape[1]
+        self.nitems = self.items.shape[1]
+        self.nuser_features = self.users.shape[0]
+        self.nitem_features = self.items.shape[0]
 
     def summary(self, sep="-"*70):
         '''
-        Prints out a summary of the contents of a stanscofi.Dataset: the number of items, users, the number of positive, negative, unknown matchings, the sparsity number, and the shape and percentage of missing values in the item and user feature matrices
+        Prints out a summary of the contents of a stanscofi.Dataset: the number of items, users, the number of positive, negative, unlabeled, unavailable matchings, the sparsity number, and the shape and percentage of missing values in the item and user feature matrices
 
         ...
 
         Parameters
         ----------
         sep : str
             separator for pretty printing
+        ...
+
+        Returns
+        ----------
+        ndrugs : int
+            number of drugs
+        ndiseases : int
+            number of diseases
+        ndrugs_known : int
+            number of drugs with at least one known (positive or negative) rating
+        ndiseases_known : int
+            number of diseases with at least one known (positive or negative) rating
+        npositive : int
+            number of positive ratings
+        nnegative : int
+            number of negative ratings
+        nunlabeled_unavailable : int
+            number of unlabeled or unavailable ratings
+        nunavailable : int
+            number of unavailable ratings
+        sparsity : float
+            percentage of known ratings
+        sparsity_known : float
+            percentage of known ratings among drugs and diseases with at least one known rating
+        ndrug_features : int
+            number of drug features
+        missing_drug_features : float
+            percentage of missing drug feature values
+        ndisease_features : int
+            number of disease features
+        missing_disease_features : float
+            percentage of missing disease feature values
         '''
-        A = pd.DataFrame(self.ratings_mat, index=self.item_list, columns=self.user_list)
         print(sep)
-        print("* Matching matrix:")
-        ratings = pd.DataFrame(self.ratings, index=range(self.ratings.shape[0]), columns=["user", "item", "rating"])
-        ratings2 = ratings.copy()
-        ratings2["item"] = ratings2["item"].astype(str)
-        args = [len(np.unique(ratings2["item"])), len(np.unique(ratings2["user"]))]
-        args += [ratings2.loc[ratings2["rating"]==v].shape[0] for v in [1,-1]]
-        args += [np.prod(A.shape)-args[2]-args[3],(args[2]+args[3])*100/np.prod(A.shape)]
-        dataset_str = "Ratings: %d drugs\t%d diseases involved in at least one known matching\n%d positive, %d negative, %d unknown matchings\nSparsity for drugs/diseases involved in at least one known matching: %.2f perc."
-        print(dataset_str % tuple(args))
+        print("* Rating matrix: %d drugs x %d diseases" % (self.nitems, self.nusers))
+        restricted_ratings = self.ratings.toarray()[np.abs(self.ratings).sum(axis=1)>0,:]
+        restricted_ratings = restricted_ratings[:,np.abs(restricted_ratings).sum(axis=0)>0]
+        print("Including %d drugs and %d diseases involved in at least one positive/negative rating" % restricted_ratings.shape)
+        print("%d positive, %d negative, %d unlabeled (including %d unavailable) drug-disease ratings" % ((self.ratings==1).sum(), (self.ratings==-1).sum(), np.prod(self.ratings.shape)-self.ratings.getnnz(), np.prod(self.folds.shape)-self.folds.getnnz()))
+        print("Sparsity: %.2f percent (on drugs/diseases with at least one known rating %.2f)" % ((self.ratings!=0).mean()*100, (restricted_ratings!=0).mean()*100))
         print(sep[:len(sep)//2])
         print("* Feature matrices:")
         if (self.items.shape[0]>0):
-            print("Total #Drugs: %d\t#Drug features: %d\tPerc. Missing features: %d" % (self.items.shape[1], self.items.shape[0], np.sum(np.isnan(self.items))*100/(self.items.shape[0]*self.items.shape[1])))
+            print("#Drug features: %d\tTotal #Drugs: %d" % (self.items.shape))
+            print("Missing features: %.2f percent" % (np.isnan(self.items.toarray()).mean()*100))
         if (self.users.shape[0]>0):
-            print("Total #Diseases: %d\t#Disease features: %d\tPerc. Missing features: %d" % (self.users.shape[1], self.users.shape[0], np.sum(np.isnan(self.users))*100/(self.users.shape[0]*self.users.shape[1])))
+            print("#Disease features: %d\tTotal #Disease: %d" % (self.users.shape))
+            print("Missing features: %.2f percent" % (np.isnan(self.users.toarray()).mean()*100))
         if (self.users.shape[0]+self.items.shape[0]==0):
             print("No feature matrices.")
         print(sep+"\n")
+        return self.nitems, self.nusers, restricted_ratings.shape[0], restricted_ratings.shape[1], (self.ratings==1).sum(), (self.ratings==-1).sum(), np.prod(self.ratings.shape)-self.ratings.getnnz(), np.prod(self.folds.shape)-self.folds.getnnz(), (self.ratings!=0).mean()*100, (restricted_ratings!=0).mean()*100, self.items.shape[0], np.isnan(self.items.toarray()).mean()*100, self.users.shape[0], np.isnan(self.users.toarray()).mean()*100
 
     def visualize(self, withzeros=False, X=None, y=None, metric="euclidean", figsize=(5,5), fontsize=20, dimred_args={}, predictions=None, use_ratings=False, random_state=1234, show_errors=False, verbose=False):
         '''
         Plots a representation of the datapoints in a stanscofi.Dataset which is annotated either by the ground truth labels or the predicted labels. The representation is the plot of the datapoints according to the first two Principal Components, or the first two dimensions in UMAP, if the feature matrices can be converted into a (n_ratings, n_features) shaped matrix where n_features>1, else it plots a heatmap with the values in the matrix for each rating pair. 
 
         In the legend, ground truth labels are denoted with brackets: e.g., [0] (unknown), [1] (positive) and [-1] (negative); predicted ratings are denoted by "pos" (positive) and "neg" (negative); correct (resp., incorrect) predictions are denoted by "correct", resp. "error"
 
@@ -241,72 +290,73 @@
         show_errors : bool
             boolean to assess whether to color according to the error in class prediction; if show_errors=False, then either the ground truth or the predicted class labels will be used to color the datapoints; otherwise, the points will be restricted to the set of known matchings (even if withzeros=True) and colored according to the identity between the ground truth and the predicted labels for each (user, item) pair
         verbose : bool
             prints out information at each step
         '''
         assert fontsize > 0
         assert random_state >= 0
-        nvalues = np.prod(self.ratings_mat.shape)
+        nvalues = self.folds.data.shape[0]
         assert (X is None and y is None) or ((X.shape[0]==y.shape[0]==nvalues))
-        assert predictions is None or ((predictions.shape[1]==3) and (predictions.shape[0]==nvalues))
+        assert predictions is None or (predictions.data.shape[0]==nvalues)
         if (self.users.shape[0]==0 or self.items.shape[0]==0):
             if (verbose):
                 print("<datasets.visualize> Can't plot (no item/user feature matrix).")
             return None
-        assert predictions is None or (((predictions[:,-1]==1)|(predictions[:,-1]==-1)).all())
+        assert predictions is None or (((predictions.toarray()==1)|(predictions.toarray()==-1)|(predictions.toarray()==0)).all())
         if (X is None and y is None):
             if (verbose):
                 print("<datasets.visualize> Imputation of missing values by average row-value, standard scaling")
             subselect_size = max(2,min(int(5e7)//nvalues+1, nvalues))
+            subselect_size = min(subselect_size, min(self.users.shape[0],self.items.shape[0]))
             ## Preprocessed (item, user) pair feature matrix and corresponding outcome vector
-            X, y, _, _ = stanscofi.preprocessing.meanimputation_standardize(self, subset=min(subselect_size, min(self.users.shape[0],self.items.shape[0])), inf=2, verbose=verbose)
+            X, y, _, _ = meanimputation_standardize(self, subset=subselect_size, inf=2, verbose=verbose)
             use_inputX=False
         else:
             predictions = None
             show_errors = False
             use_inputX=True
-        markers = np.argwhere(np.ones(self.ratings_mat.shape))
+        markers = np.column_stack((self.folds.row, self.folds.col))
         ## True (known and unknown) ratings for all items and users in the dataset
         ## item i, user u, rating r
         markers = np.concatenate((markers, y.reshape(-1,1)), axis=1)
         if ((use_ratings) and (not use_inputX)):
             predictions = markers
         ## 1. predictions=None: Plots datapoints according to ground truth annotations
         if (predictions is None):
             show_errors = False
             ## item i, user u, rating r, scatter style (color + marker shape)
             all_pairs = np.array([[{-1:"r.", 1:"g.", 0:"y."}[k]] for i,j,k in markers.tolist()])
             all_pairs = np.concatenate((markers, all_pairs), axis=1)
             assert all_pairs.shape[1]==4 and all_pairs.shape[0]==nvalues
         else:
-            predictions = predictions.astype(int)
             ## 2. predictions!=None: Plots datapoints according to predicted annotations
             if (not use_ratings):
-                classes = dict(zip([(i,j) for i,j in predictions[:,:2].tolist()], predictions[:,2].flatten()))
-                all_pairs = np.array([[classes[(j,i)]] for i, j in markers[:,:2].tolist()])
+                classes = dict(zip([(i,j) for i,j in zip(self.folds.row, self.folds.col)], predictions.data))
+                all_pairs = np.array([[classes.get((i,j), 0)] for i, j in markers[:,:2].astype(int).tolist()])
                 all_pairs = np.concatenate((markers, all_pairs), axis=1)
             else:
                 all_pairs = np.concatenate((markers, markers[:,2]), axis=1)
             ## 2.a. predictions!=None: Only for datapoints with known ratings
             if (show_errors):
                 values = np.array([[{0:"r", 1:"g", -1:"y"}[int(true==pred)-int(true==0)]+{-1:"v", 1:"+", 0:"."}[true]] for [i,j,true,pred] in all_pairs.tolist()])
                 ## Predicted ratings for all known pairs of items and users in the dataset
                 ## item i, user u, rating r, scatter style (color + marker shape)
-                all_pairs = np.concatenate((all_pairs[:,[0,1,3]],values), axis=1, dtype=object)
+                all_pairs = np.array(np.concatenate((all_pairs[:,[0,1,3]], values), axis=1), dtype=object)
                 all_pairs = all_pairs[y!=0,:]
                 X = X[y!=0,:]
+                y = y[y!=0]
                 assert all_pairs.shape[1]==4
             ## 2.b. predictions!=None: For all datapoints
             else:
                 values = np.array([[{-1:"r", 1:"g", 0:"y"}[pred]+{-1:"v", 1:"+", 0:"."}[true]] for [i,j,true,pred] in all_pairs.tolist()])
                 ## Predicted ratings for all known pairs of items and users in the dataset
                 ## item i, user u, rating r, scatter style (color + marker shape)
-                all_pairs = np.concatenate((all_pairs[:,[0,1,3]],values), axis=1, dtype=object)
+                all_pairs = np.array(np.concatenate((all_pairs[:,[0,1,3]], values), axis=1), dtype=object)
                 assert all_pairs.shape[1]==4 and all_pairs.shape[0]==X.shape[0]
-        all_pairs[:,:-1] = all_pairs[:,:-1].astype(int)
+        all_pairs[:,:-1] = all_pairs[:,:-1].astype(float).astype(int)
         if (verbose):
             print("<datasets.visualize> Reducing dimension and plotting matrix X of size %d x %d" % X.shape)
         dimred_args.update({"n_components":min(2,X.shape[1]), "random_state":random_state})
         use_pca = ("n_neighbors" not in dimred_args)
         if (use_pca):
             with np.errstate(invalid="ignore"): # for NaN or 0 variance matrices
                 pca = PCA(**dimred_args)
@@ -356,92 +406,61 @@
             plt.ylabel(("PC2 ("+str(int(var12[1]))+"%)" if (use_pca) else "Dim2") if (not np.isnan(var12[1])) else "C2", fontsize=fontsize)
             plt.xlabel((("PC1 ("+str(int(var12[0]))+"%)" if (use_pca) else "Dim1")) if (not np.isnan(var12[0])) else "C1", fontsize=fontsize)
             plt.title("on %d features" % X.shape[1], fontsize=fontsize//2)
             plt.legend(handles=handles, fontsize=fontsize, loc='upper right', bbox_to_anchor=(1.6,0.9))
             plt.show()
         elif ((dimred_X!=0).any()):
             ## Prints a heatmap according to values in X
-            X_heatmap = X.reshape(self.ratings_mat.shape)
-            annot = self.ratings_mat.copy().astype(str)
+            X_reshape_folds = coo_array((X.ravel(), (self.folds.row, self.folds.col)), 
+                            shape=self.folds.shape)
+            X_heatmap = X_reshape_folds.toarray()
+            annot = self.ratings.toarray().astype(int).astype(str)
             annot[annot=="0"] = "" #unknown
             annot[annot=="1"] = "+"  #positive
             annot[annot=="-1"] = "*"  #negative
+            keep_ids_y = np.abs(X_heatmap).sum(axis=1)>0 
+            keep_ids_x = np.abs(X_heatmap).sum(axis=0)>0 
+            X_heatmap = X_heatmap[keep_ids_y,:][:,keep_ids_x]
+            annot = annot[keep_ids_y,:][:,keep_ids_x]
             h = sns.clustermap(X_heatmap, method='average', cmap="viridis", metric=metric, annot=annot, fmt="s", figsize=figsize)
             h.ax_heatmap.set_xlabel("Disease", fontsize=fontsize) 
             h.ax_heatmap.set_ylabel("Drug", fontsize=fontsize)
             h.ax_heatmap.set_xticklabels([])
             h.ax_heatmap.set_yticklabels([]) 
             handles = [mlines.Line2D([], [], color="black", marker=k) for k in ["+", "*"] if (k in annot)]
             h.ax_heatmap.legend(handles, ["Positive", "Negative"], fontsize=fontsize, loc='upper right', bbox_to_anchor=(1.6,0.9))
             plt.show()
         else:
             if (verbose):
                 print("<stanscofi.dataset.visualize> Matrix is empty, can't plot!")
         return None
 
-    def get_folds(self, folds, subset_name="subset"):
+    def subset(self, folds, subset_name="subset"):
         '''
         Obtains a subset of a stanscofi.Dataset based on a set of user and item indices
 
         ...
 
         Parameters
         ----------
-        folds : array-like of shape (n_ratings, 3)
-            a matrix which contains the user indices (column 1), the item indices (column 2) and the class for the corresponding (user, item) pair (value in {-1, 0, 1} in column 3). /!\ the ratings in the last column overrides values in dataset.ratings_mat
+        folds : COO-array of shape (n_items, n_users)
+            an array which contains values in {0, 1} describing the unavailable and available user-item matchings in ratings
         subset_name : str
             name of the newly created stanscofi.Dataset
 
         Returns
-        subset : stanscofi.Dataset
-            dataset corresponding to the folds in input
         ----------
-        '''
-        if (len(folds)==0):
-            raise ValueError("Fold is empty!")
-        assert folds.shape[1]==3
-        assert np.max(folds[:,0])<=self.ratings_mat.shape[1]
-        assert np.max(folds[:,1])<=self.ratings_mat.shape[0]
-        assert ((folds[:,-1]==1)|(folds[:,-1]==-1)|(folds[:,-1]==0)).all()
-        ratings = pd.DataFrame(folds, index=range(folds.shape[0]), columns=["user","item","rating"])
-        ratings["user"] = [self.user_list[x] for x in ratings["user"]]
-        ratings["item"] = [self.item_list[x] for x in ratings["item"]]
-        user_lst = np.unique(folds[:,0]).tolist() ## order of unique
-        item_lst = np.unique(folds[:,1]).tolist() ## order of unique
-        A = stanscofi.utils.ratings2matrix(ratings, user_col="user", item_col="item", rating_col="rating")
-        P = pd.DataFrame(self.users[:,user_lst], index=self.user_features, 
-                columns=[self.user_list[i] for i in user_lst])
-        S = pd.DataFrame(self.items[:,item_lst], index=self.item_features, 
-                columns=[self.item_list[i] for i in item_lst])
-        return Dataset(A, P, S, name=subset_name, same_item_user_features=self.same_item_user_features)
-
-    def mask_dataset(self, folds, subset_name="dataset"):
-        '''
-        Obtains a copy of a stanscofi.Dataset based on a set of user and item indices where some values in the initial ratings matrix are masked with 0's. Contrary to get_folds, the shapes of the user and item feature matrices are preserved, as well as ratings_mat. Some values (not in folds) are masked with 0's in the ratings_mat matrix.
-
-        ...
-
-        Parameters
-        ----------
-        folds : array-like of shape (n_ratings, 3)
-            a matrix which contains the user indices (column 1), the item indices (column 2) and the class for the corresponding (user, item) pair (value in {-1, 0, 1} in column 3). /!\ the ratings in the last column DO NOT override values in dataset.ratings_mat
-        subset_name : str
-            name of the newly created stanscofi.Dataset
-
-        Returns
         subset : stanscofi.Dataset
-            dataset where ratings values outside of the folds in input are masked
-        ----------
+            dataset corresponding to the folds in input
         '''
-        if (len(folds)==0):
+        if (np.prod(folds.shape)==0):
             raise ValueError("Fold is empty!")
-        assert folds.shape[1]==3
-        assert np.max(folds[:,0])<=self.ratings_mat.shape[1]
-        assert np.max(folds[:,1])<=self.ratings_mat.shape[0]
-        assert ((folds[:,-1]==1)|(folds[:,-1]==-1)|(folds[:,-1]==0)).all()
-        P = pd.DataFrame(self.users, index=self.user_features, columns=self.user_list)
-        S = pd.DataFrame(self.items, index=self.item_features, columns=self.item_list)
-        A = pd.DataFrame(self.ratings_mat, index=self.item_list, columns=self.user_list)
-        y = np.zeros(self.ratings_mat.shape)
-        y[folds[:,1],folds[:,0]] = folds[:,2]
-        y = pd.DataFrame(y, index=A.index, columns=A.columns)
-        return Dataset(ratings_mat=y, users=P, items=S, name=subset_name, same_item_user_features=self.same_item_user_features, folds=folds)
+        assert folds.shape==self.folds.shape
+        #data = self.ratings.toarray()[folds.row, folds.col].ravel()
+        sfolds = np.asarray(folds.toarray(), dtype=float)
+        sfolds[sfolds==0] = np.nan
+        ratings = self.ratings.toarray() * sfolds
+        ratings = pd.DataFrame(ratings, index=self.item_list, columns=self.user_list)
+        users = pd.DataFrame(self.users.toarray(), index=self.user_features, columns=self.user_list)
+        items = pd.DataFrame(self.items.toarray(), index=self.item_features, columns=self.item_list)
+        subset =  Dataset(ratings=ratings, users=users, items=items, same_item_user_features=self.same_item_user_features, name=subset_name)
+        return subset
```

### Comparing `stanscofi-1.1.0/src/stanscofi/models.py` & `stanscofi-2.0.0/src/stanscofi/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,107 +1,18 @@
 #coding: utf-8
 
 import numpy as np
+import random
 import pandas as pd
+from scipy.sparse import coo_array, csr_array
 
 from sklearn.decomposition import NMF as NonNegMatFact
 from sklearn.linear_model import LogisticRegression as Logit
 
-import stanscofi.preprocessing
-
-###############################################################################################################
-###################
-# Utils           #
-###################
-
-def scores2ratings(df, user_col="user", item_col="item", rating_col="rating"):
-    '''
-    Converts a matrix of scores into a list of scores
-
-    ...
-
-    Parameters
-    ----------
-    df : pandas.DataFrame of shape (n_items, n_users)
-        the matrix of scores
-    user_col : str
-        column denoting users
-    item_col : str
-        column denoting items
-    rating_col : str
-        column denoting ratings in {-1, 0, 1}
-
-    Returns
-    ----------
-    ratings : pandas.DataFrame of shape (n_ratings, 3)
-        the list of scores where the first column correspond to users, second to items, third to scores
-    '''
-    grid = np.argwhere(np.ones(df.shape))
-    res_df = pd.DataFrame([], index=range(grid.shape[0]))
-    res_df[user_col] = [df.columns[x] for x in list(grid[:, 1].flatten())]
-    res_df[item_col] = [df.index[x] for x in list(grid[:, 0].flatten())]
-    res_df[rating_col] = [df.values[i,j] for i,j in grid.tolist()]
-    return res_df[[user_col, item_col, rating_col]]
-
-def create_scores(preds, dataset):
-    '''
-    Converts a score vector or a score value into a list of scores
-
-    ...
-
-    Parameters
-    ----------
-    preds : int or float or array-like of shape (n_ratings, )
-        the matrix of scores
-    dataset : stanscofi.datasets.Dataset
-        dataset to apply the scores to
-
-    Returns
-    ----------
-    scores : array-like of shape (n_ratings, 3)
-        the list of scores where the first column correspond to users, second to items, third to scores
-    '''
-    assert str(type(preds)) in ["<class 'float'>", "<class 'int'>"] or len(preds.shape)==1 or preds.shape[1]==1
-    ids = np.argwhere(np.ones(dataset.ratings_mat.shape))
-    assert str(type(preds)) in ["<class 'float'>", "<class 'int'>"] or preds.shape[0]==ids.shape[0]
-    scores = np.zeros((ids.shape[0], 3))
-    scores[:,0] = ids[:,1] 
-    scores[:,1] = ids[:,0] 
-    scores[:,2] = np.ravel(preds)
-    return scores
-
-def create_overscores(preds, dataset):
-    '''
-    Converts a sublist of scores into a list of scores on the full dataset
-
-    ...
-
-    Parameters
-    ----------
-    preds : array-like of shape (n_ratings, 3)
-        the list of scores where the first column correspond to users, second to items, third to scores, where ratings are a subset of all possible ratings in the input dataset
-    dataset : stanscofi.datasets.Dataset
-        over-dataset which was used
-
-    Returns
-    ----------
-    scores : array-like of shape (n_ratings, 3)
-        the list of scores where the first column correspond to users, second to items, third to scores on all possible pairs in the dataset
-    '''
-    assert preds.shape[1]==3
-    assert np.max(preds[:,0])<=np.max(dataset.ratings_mat.shape[1])
-    assert np.max(preds[:,1])<=np.max(dataset.ratings_mat.shape[0])
-    ids = np.argwhere(np.ones(dataset.ratings_mat.shape))
-    scores = np.zeros((ids.shape[0], 3))
-    scores[:,0] = ids[:,1]
-    scores[:,1] = ids[:,0]
-    in_preds = [((preds[:,0]==i)&(preds[:,1]==j)).any() for i,j in ids[:,:2].tolist()]
-    assert sum(in_preds)==preds.shape[0]
-    scores[in_preds,2] = preds[:,2]
-    return scores
+from .preprocessing import preprocessing_XY
 
 ###############################################################################################################
 ###################
 # Basic model     #
 ###################
 
 class BasicModel(object):
@@ -109,228 +20,260 @@
     A class used to encode a drug repurposing model
 
     ...
 
     Parameters
     ----------
     params : dict
-        dictionary which contains method-wise parameters plus a key called "decision_threshold" with a float value which determines the decision threshold to label a positive class
+        dictionary which contains method-wise parameters
 
     Attributes
     ----------
     name : str
         the name of the model
     model : depends on the implemented method
         may contain an instance of a class of sklearn classifiers
-    decision_threshold : float
-        decision threshold to label a positive class
     ...
         other attributes might be present depending on the type of model
 
     Methods
     -------
     __init__(params)
-        Initialize the model with preselected parameters
-    to_picklable()
-        Outputs a dictionary which contains all attributes of the model
-    from_picklable(picklable)
-        Sets all parameters in the model according to dictionary picklable
-    predict(test_dataset)
+        Initializes the model with preselected parameters
+    fit(train_dataset, seed=1234)
+        Preprocesses and fits the model 
+    predict_proba(test_dataset)
         Outputs properly formatted predictions of the fitted model on test_dataset
-    classify(scores)
-        Applies the following decision rule: if score<self.decision_threshold, then return -1, otherwise return 1
+    predict(scores)
+        Applies the following decision rule: if score<threshold, then return the negative label, otherwise return the positive label
+    recommend_k_pairs(dataset, k=1, threshold=None)
+        Outputs the top-k (item, user) candidates (or candidates which score is higher than a threshold) in the input dataset
     print_scores(scores)
         Prints out information about scores
     print_classification(predictions)
         Prints out information about predicted labels
-    preprocessing(train_dataset)
-        Preprocess the input dataset into something that is an input to the self.model.fit if it exists (not implemented in BasicModel)
-    fit(train_dataset)
-        Preprocess and fit the model (not implemented in BasicModel)
-    model_predict(test_dataset)
-        Outputs predictions of the fitted model on test_dataset (not implemented in BasicModel)
+    preprocessing(train_dataset) [not implemented in BasicModel]
+        Preprocess the input dataset into something that is an input to the self.model_fit if it exists
+    model_fit(train_dataset) [not implemented in BasicModel]
+        Fits the model on train_dataset
+    model_predict_proba(test_dataset) [not implemented in BasicModel]
+        Outputs predictions of the fitted model on test_dataset
     '''
     def __init__(self, params):
         '''
         Creates an instance of stanscofi.BasicModel
 
         ...
 
         Parameters
         ----------
         params : dict
-            dictionary which contains method-wise parameters plus a key called "decision_threshold" with a float value which determines the decision threshold to label a positive class
+            dictionary which contains method-wise parameters
         '''
         self.name = "Model"
-        self.model = None
-        assert "decision_threshold" in params
-        self.decision_threshold = params["decision_threshold"]
+        for param in params:
+            setattr(self, param, params[param])
 
-    def to_picklable(self):
+    def fit(self, train_dataset, seed=1234):
         '''
-        Gets a serializable version of the model
+        Fitting the model on the training dataset.
+
+        Not implemented in the BasicModel class.
 
         ...
 
-        Returns
+        Parameters
         ----------
-        picklable : dict
-            dictionary which contains all attributes of the model
+        train_dataset : stanscofi.Dataset
+            training dataset on which the model should fit
+        seed : int (default: 1234)
+            random seed
         '''
-        objs = [x for x in dir(self.model) 
-		if (x[0]!="_" and x[-1]!="_" and str(type(x))!="<class 'method'>")
-        ]
-        picklable = {}
-        for a in objs:
-            picklable.setdefault(a, eval("self.model."+a))
-        picklable.setdefault("decision_threshold", self.decision_threshold)
-        return picklable
+        np.random.seed(seed)
+        random.seed(seed)
+        self.model_fit(*self.preprocessing(train_dataset, is_training=True))
 
-    def from_picklable(self, picklable):
+    def predict_proba(self, test_dataset, default_zero_val=1e-31):
         '''
-        Reinitializes a model based on its serializable version
+        Outputs properly formatted scores (not necessarily in [0,1]!) from the fitted model on test_dataset. Internally calls model_predict() then reformats the scores
 
         ...
 
         Parameters
         ----------
-        picklable : dict
-            dictionary which contains all attributes of the model
+        test_dataset : stanscofi.Dataset
+            dataset on which predictions should be made
+
+        Returns
+        ----------
+        scores : COO-array of shape (n_items, n_users)
+            sparse matrix in COOrdinate format, with nonzero values corresponding to predictions on available pairs in the dataset
         '''
-        for a in picklable:
-            if (str(type(picklable[a]))!="<class 'method'>"):
-                setattr(self.model, a, picklable[a])
+        scores = self.model_predict_proba(*self.preprocessing(test_dataset, is_training=False))
+        if ((scores!=0).any()):
+            default_val = min(default_zero_val, np.min(scores[scores!=0])/2)
+        else:
+            default_val = default_zero_val
+        #print(("folds",test_dataset.folds.data.shape[0]))
+        if (scores.shape==test_dataset.folds.shape):
+            scores[(scores==0)&(test_dataset.folds.toarray()==1)] = default_val ## avoid removing these zeroes
+            scores = coo_array(scores)
+            scores = scores*test_dataset.folds
+            #print(("scores",scores.data.shape[0]))
+            return coo_array(scores)
+        assert scores.shape[0]==test_dataset.folds.data.shape[0]
+        scores[(scores==0)&(test_dataset.folds.data==1)] = default_val ## avoid removing these zeroes 
+        scores_arr = coo_array((scores, (test_dataset.folds.row, test_dataset.folds.col)), shape=test_dataset.folds.shape)
+        #print(("scores",scores.data.shape[0]))
+        return scores_arr
 
-    def predict(self, test_dataset):
+    def predict(self, scores, threshold=0.5):
         '''
-        Outputs properly formatted predictions of the fitted model on test_dataset. Internally calls model_predict() then reformats the predictions
+        Outputs class labels based on the scores, using the following formula
+            prediction = -1 if (score<threshold) else 1
 
         ...
 
         Parameters
         ----------
-        test_dataset : stanscofi.Dataset
-            dataset on which predictions should be made
+        scores : COO-array of shape (n_items, n_users)
+            sparse matrix in COOrdinate format
+        threshold : float
+            the threshold of classification into the positive class
 
         Returns
         ----------
-        scores : array-like of shape (n_ratings, 3)
-            the list of scores where the first column correspond to users, second to items, third to scores
+        predictions : COO-array of shape (n_items, n_users)
+            sparse matrix in COOrdinate format with values in {-1,1}
         '''
-        preds = self.model_predict(test_dataset)
-        if (preds.shape==test_dataset.ratings_mat.shape):
-            scores_mat = pd.DataFrame(preds, index=test_dataset.item_list, columns=test_dataset.user_list)
-            ratings = scores2ratings(scores_mat, user_col="user", item_col="item", rating_col="rating")
-            ratings["user"] = [test_dataset.user_list.index(x) for x in ratings["user"]]
-            ratings["item"] = [test_dataset.item_list.index(x) for x in ratings["item"]]
-            scores = ratings[["user","item","rating"]].values
-        else:
-            scores = preds
-        return scores
+        #print(("scores-preds",scores.data.shape[0]))
+        preds = coo_array((scores.toarray()!=0).astype(int)*((-1)**(scores.toarray()<=threshold)))
+        #print(('preds',preds.data.shape[0]))
+        return preds
 
-    def classify(self, scores):
+    def recommend_k_pairs(self, dataset, k=1, threshold=None):
         '''
-        Outputs class labels based on the scores, using the following formula
-            prediction = -1 if (score<self.decision_threshold) else 1
+        Outputs the top-k (item, user) candidates (or candidates which score is higher than a threshold) in the input dataset
 
         ...
 
         Parameters
         ----------
-        scores : array-like of shape (n_ratings, 3)
-            the list of scores where the first column correspond to users, second to items, third to scores
+        dataset : stanscofi.Dataset
+            dataset on which predictions should be made
+        k : int or None (default: 1)
+            number of pair candidates to return (with ties)
+        threshold : float or None (default: 0)
+            threshold on candidate scores. If k is not None, k best candidates are returned independently of the value of threshold
+        ...
 
-        Returns
+        Parameters
         ----------
-        predictions : array-like of shape (n_ratings, 3)
-            the list of scores where the first column correspond to users, second to items, third to ratings
+        candidates : list of tuples of size 3
+            list of (item, user, score) candidates (by name as present in the dataset)
         '''
-        predictions = scores.copy()
-        predictions[:,2] = (-1)**(predictions[:,2]<self.decision_threshold)
-        return predictions.astype(int)
+        assert (k is None) or (k > 0)
+        scores = self.predict_proba(dataset)
+        if (k is not None):
+            vals = scores
+            kth_best = np.unique([scores.toarray()[a] for a in np.argsort(-scores)])[k]
+            ids_list = np.argwhere(scores==kth_best).tolist()
+        else:
+            assert threshold is not None
+            vals = (scores>=threshold)*scores
+            k = len(vals.data)
+            ids_list = np.dstack(np.unravel_index((-vals.toarray()).ravel().argsort(), scores.toarray().shape))[0][:k,:].tolist()
+        candidates = [[dataset.item_list[i], dataset.user_list[j], scores.toarray()[i,j]] for i,j in ids_list]
+        return candidates
 
     def print_scores(self, scores):
         '''
         Prints out information about the scores
 
         ...
 
         Parameters
         ----------
-        scores : array-like of shape (n_ratings, 3)
-            the list of scores where the first column correspond to users, second to items, third to scores
+        scores : COO-array
+            sparse matrix in COOrdinate format
         '''
-        Nitems, Nusers = len(np.unique(scores[:, 1].tolist())), len(np.unique(scores[:, 0].tolist()))
         print("* Scores")
-        print("%d unique items, %d unique users" % (Nitems, Nusers))
-        print("Scores: Min: %f\tMean: %f\tMedian: %f\tMax: %f\tStd: %f\n" % tuple([f(scores[:, 2]) for f in [np.min,np.mean,np.median,np.max,np.std]]))
+        print("%d unique items, %d unique users" % (len(np.unique(scores.row)), len(np.unique(scores.col))))
+        print("Scores: Min: %f\tMean: %f\tMedian: %f\tMax: %f\tStd: %f\n" % tuple([f(scores.data) for f in [np.min,np.mean,np.median,np.max,np.std]]))
 
     def print_classification(self, predictions):
         '''
         Prints out information about the predicted classes
 
         ...
 
         Parameters
         ----------
-        predictions : array-like of shape (n_ratings, 3)
-            the list of scores where the first column correspond to users, second to items, third to ratings
+        predictions : COO-array
+            sparse matrix in COOrdinate format
         '''
-        Nitems, Nusers = len(np.unique(predictions[:, 1].tolist())), len(np.unique(predictions[:, 0].tolist()))
         print("* Classification")
-        print("%d unique items, %d unique users" % (Nitems, Nusers))
-        print("Positive class: %d, Negative class: %d\n" % (np.sum(predictions[:,2]==1), np.sum(predictions[:,2]==-1)))
+        print("%d unique items, %d unique users" % (len(np.unique(predictions.row)), len(np.unique(predictions.col))))
+        print("Positive class: %d, Negative class: %d\n" % ((csr_array(predictions)==1).sum(), (csr_array(predictions)==-1).sum()))
 
-    def preprocessing(self, dataset):
+    def preprocessing(self, dataset, is_training=True):
         '''
         Preprocessing step, which converts elements of a dataset (ratings matrix, user feature matrix, item feature matrix) into appropriate inputs to the classifier (e.g., X feature matrix for each (user, item) pair, y response vector).
 
-        Not implemented in the BasicModel class.
+        <Not implemented in the BasicModel class.>
 
         ...
 
         Parameters
         ----------
         dataset : stanscofi.Dataset
             dataset to convert
+        is_training : bool
+            is the preprocessing prior to training (true) or testing (false)?
 
         Returns
         ----------
         ... : ...
             appropriate inputs to the classifier (vary across algorithms)
         '''
         raise NotImplemented
 
-    def fit(self, train_dataset):
+    def model_fit(self):
         '''
         Fitting the model on the training dataset.
 
-        Not implemented in the BasicModel class.
+        <Not implemented in the BasicModel class.>
 
         ...
 
         Parameters
         ----------
-        train_dataset : stanscofi.Dataset
-            training dataset on which the model should fit
+        ... : ...
+            appropriate inputs to the classifier (vary across algorithms)
         '''
         raise NotImplemented
 
-    def model_predict(self, test_dataset):
+    def model_predict_proba(self):
         '''
         Making predictions using the model on the testing dataset.
 
-        Not implemented in the BasicModel class.
+        <Not implemented in the BasicModel class.>
 
         ...
 
         Parameters
         ----------
-        test_dataset : stanscofi.Dataset
-            testing dataset on which the model should be validated
+        ... : ...
+            appropriate inputs to the classifier (vary across algorithms)
+        ...
+
+        Returns
+        ----------
+        scores : array_like of shape (n_items, n_users)
+            prediction values by the model
         '''
         raise NotImplemented
 
 ###############################################################################################################
 ###################
 # NMF             #
 ###################
@@ -340,93 +283,99 @@
     Non-negative Matrix Factorization (calls sklearn.decomposition.NMF internally). It uses the very same parameters as sklearn.decomposition.NMF, so please refer to help(sklearn.decomposition.NMF).
 
     ...
 
     Parameters
     ----------
     params : dict
-        dictionary which contains sklearn.decomposition.NMF parameters plus a key called "decision_threshold" with a float value which determines the decision threshold to label a positive class
+        dictionary which contains sklearn.decomposition.NMF parameters
 
     Attributes
     ----------
     Same as BasicModel class
 
     Methods
     -------
     Same as BasicModel class
     preprocessing(train_dataset)
-        Preprocess the input dataset into something that is an input to the self.model.fit if it exists
-    fit(train_dataset)
-        Preprocess and fit the model
-    model_predict(test_dataset)
+        Preprocesses the input dataset into something that is an input to fit
+    model_fit(train_dataset)
+        Preprocesses and fits the model
+    model_predict_proba(test_dataset)
         Outputs predictions of the fitted model on test_dataset
     '''
     def __init__(self, params):
         '''
         Creates an instance of stanscofi.NMF
 
         ...
 
         Parameters
         ----------
         params : dict
-            dictionary which contains sklearn.decomposition.NMF parameters plus a key called "decision_threshold" with a float value which determines the decision threshold to label a positive class
+            dictionary which contains sklearn.decomposition.NMF parameters
         '''
         super(NMF, self).__init__(params)
         self.name = "NMF"
-        self.model = NonNegMatFact(**{p: params[p] for p in params if (p!="decision_threshold")})
+        self.estimator = NonNegMatFact(**params)
 
-    def preprocessing(self, dataset):
+    def preprocessing(self, dataset, is_training=True):
         '''
         Preprocessing step, which converts elements of a dataset (ratings matrix, user feature matrix, item feature matrix) into appropriate inputs to the NMF classifier.
 
         ...
 
         Parameters
         ----------
         dataset : stanscofi.Dataset
             dataset to convert
+        is_training : bool
+            is the preprocessing prior to training (true) or testing (false)?
 
         Returns
         ----------
+        args : contains
         A : array-like of shape (n_users, n_items)
-            transposed translated association matrix so that all its values are non-negative
+            contains the transposed translated association matrix so that all its values are non-negative
         '''
-        A = dataset.ratings_mat.copy()
-        A -= np.min(A)
-        return A.T
+        mat = np.nan_to_num(dataset.ratings.toarray(), copy=True, nan=0.)
+        A = mat-np.min(mat)
+        return [A.T]
     
-    def fit(self, train_dataset):
+    def model_fit(self, input):
         '''
-        Fitting the NMF model on the training dataset.
+        Fitting the NMF model on the preprocessed training dataset.
 
         ...
 
         Parameters
         ----------
-        train_dataset : stanscofi.Dataset
-            training dataset on which the model should fit
+        input : array-like of shape (n_samples,n_features)
+            training data
         '''
-        inp = self.preprocessing(train_dataset)
-        self.model.fit(inp)
+        self.estimator.fit(input)
     
-    def model_predict(self, test_dataset):
+    def model_predict_proba(self, input):
         '''
         Making predictions using the NMF model on the testing dataset.
 
         ...
 
         Parameters
         ----------
-        test_dataset : stanscofi.Dataset
-            testing dataset on which the model should be validated
+        input : array-like of shape (n_samples,n_features)
+            testing data
+        ...
+
+        Returns
+        ----------
+        result : array-like of shape (n_samples,n_features)
         '''
-        inp = self.preprocessing(test_dataset)
-        W = self.model.fit_transform(inp)
-        return W.dot(self.model.components_).T
+        W = self.estimator.fit_transform(input)
+        return W.dot(self.estimator.components_).T
 
 ###############################################################################################################
 #########################
 # Logistic regression   #
 #########################
 
 class LogisticRegression(BasicModel):
@@ -434,96 +383,93 @@
     Logistic Regression (calls sklearn.linear_model.LogisticRegression internally). It uses the very same parameters as sklearn.linear_model.LogisticRegression, so please refer to help(sklearn.linear_model.LogisticRegression).
 
     ...
 
     Parameters
     ----------
     params : dict
-        dictionary which contains sklearn.linear_model.LogisticRegression parameters plus a key called "decision_threshold" with a float value which determines the decision threshold to label a positive class, plus a key called "preprocessing" which determines which preprocessing function (in stanscofi.preprocessing) should be applied to data, plus a key called "subset" which gives the maximum number of features to consider in the model (those features will be the Top-subset in terms of variance across samples)
+        dictionary which contains sklearn.linear_model.LogisticRegression parameters, plus a key called "preprocessing" which determines which preprocessing function (in stanscofi.preprocessing) should be applied to data, plus a key called "subset" which gives the maximum number of features to consider in the model (those features will be the Top-subset in terms of variance across samples)
 
     Attributes
     ----------
     Same as BasicModel class
 
     Methods
     -------
     Same as BasicModel class
     preprocessing(train_dataset)
-        Preprocess the input dataset into something that is an input to the self.model.fit if it exists
-    fit(train_dataset)
-        Preprocess and fit the model
-    model_predict(test_dataset)
+        Preprocesses the input dataset into something that is an input to fit
+    model_fit(train_dataset)
+        Preprocesses and fits the model
+    model_predict_proba(test_dataset)
         Outputs predictions of the fitted model on test_dataset
     '''
     def __init__(self, params):
         '''
         Creates an instance of stanscofi.LogisticRegression
 
         ...
 
         Parameters
         ----------
         params : dict
-            dictionary which contains sklearn.linear_model.LogisticRegression parameters plus a key called "decision_threshold" with a float value which determines the decision threshold to label a positive class, plus a key called "preprocessing" which determines which preprocessing function (in stanscofi.preprocessing) should be applied to data, plus a key called "subset" which gives the maximum number of features to consider in the model (those features will be the Top-subset in terms of variance across samples)
+            dictionary which contains sklearn.linear_model.LogisticRegression parameters, plus a key called "preprocessing_str" which determines which preprocessing function (in stanscofi.preprocessing) should be applied to data, plus a key called "subset" which gives the maximum number of features to consider in the model (those features will be the Top-subset in terms of variance across samples)
         '''
         super(LogisticRegression, self).__init__(params)
-        self.name = "LogisticRegression"
-        self.scalerP, self.scalerS = None, None
-        self.model = Logit(**{p: params[p] for p in params if (p not in ["decision_threshold", "preprocessing", "subset"])})
-        self.preprocessing_str = params["preprocessing"]
         assert self.preprocessing_str in ["Perlman_procedure", "meanimputation_standardize", "same_feature_preprocessing"]
-        self.subset = params["subset"]
-        self.filter = None
+        self.name = "LogisticRegression"
+        self.scalerP, self.scalerS, self.filter = None, None, None
+        self.estimator = Logit(**{p: params[p] for p in params if (p not in ["preprocessing_str", "subset"])})
 
-    def preprocessing(self, dataset):
+    def preprocessing(self, dataset, is_training=True):
         '''
         Preprocessing step, which converts elements of a dataset (ratings matrix, user feature matrix, item feature matrix) into appropriate inputs to the Logistic Regression classifier. 
 
         ...
 
         Parameters
         ----------
         dataset : stanscofi.Dataset
             dataset to convert
+        is_training : bool
+            is the preprocessing prior to training (true) or testing (false)?
 
         Returns
         ----------
+        args : contains
         X : array-like of shape (n_ratings, n_pair_features)
             (user, item) feature matrix (the actual contents of the matrix depends on parameters "preprocessing" and "subset" given as input
         y : array-like of shape (n_ratings, )
             response vector for each (user, item) pair
         '''
-        X, y, scalerS, scalerP, filter_ = stanscofi.preprocessing.preprocessing_routine(dataset, self.preprocessing_str, subset_=self.subset, filter_=self.filter, scalerS=self.scalerS, scalerP=self.scalerP, inf=2, njobs=1)
-        self.filter = filter_
-        self.scalerS = scalerS
-        self.scalerP = scalerP
-        return X, y
+        X, y, scalerS, scalerP, filter_ = preprocessing_XY(dataset, self.preprocessing_str, subset_=self.subset, filter_=self.filter, scalerS=self.scalerS, scalerP=self.scalerP, inf=2, njobs=1)
+        self.filter, self.scalerS, self.scalerP = filter_, scalerS, scalerP
+        return [X, y] if (is_training) else [X]
     
-    def fit(self, train_dataset):
+    def model_fit(self, X, y):
         '''
         Fitting the Logistic Regression model on the training dataset.
 
         ...
 
         Parameters
         ----------
-        train_dataset : stanscofi.Dataset
-            training dataset on which the model should fit
+        X : array-like of shape (n_ratings, n_pair_features)
+            (user, item) feature matrix (the actual contents of the matrix depends on parameters "preprocessing" and "subset" given as input
+        y : array-like of shape (n_ratings, )
+            response vector for each (user, item) pair
         '''
-        X, y = self.preprocessing(train_dataset)
-        self.model.fit(X, y)
+        self.estimator.fit(X, y)
     
-    def model_predict(self, test_dataset):
+    def model_predict_proba(self, X):
         '''
         Making predictions using the Logistic Regression model on the testing dataset.
 
         ...
 
         Parameters
         ----------
-        test_dataset : stanscofi.Dataset
-            testing dataset on which the model should be validated
+        X : array-like of shape (n_ratings, n_pair_features)
+            (user, item) feature matrix (the actual contents of the matrix depends on parameters "preprocessing" and "subset" given as input
         '''
-        X, _ = self.preprocessing(test_dataset)
-        preds = self.model.predict_proba(X).max(axis=1)
-        scores = create_scores(preds, test_dataset)
+        scores = self.estimator.predict_proba(X)[:,1] ## scores for the positive class
         return scores
```

### Comparing `stanscofi-1.1.0/src/stanscofi/preprocessing.py` & `stanscofi-2.0.0/src/stanscofi/preprocessing.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,75 +1,79 @@
 #coding:utf-8
 
 import numpy as np
-
 from joblib import Parallel, delayed
 from tqdm import tqdm
 
 from sklearn.preprocessing import StandardScaler
 from sklearn.impute import SimpleImputer
 
-def preprocessing_routine(dataset, preprocessing_str, subset_=None, filter_=None, scalerS=None, scalerP=None, inf=2, njobs=1):
+def preprocessing_XY(dataset, preprocessing_str, operator="*", sep_feature="-", subset_=None, filter_=None, scalerS=None, scalerP=None, inf=2, njobs=1):
     '''
     Converts a score vector or a score value into a list of scores
 
     ...
 
     Parameters
     ----------
     dataset : stanscofi.datasets.Dataset
         dataset to preprocess
     preprocessing_str : str
-        type of preprocessing: in ["Perlman_procedure","meanimputation_standardize","same_feature_preprocessing"]. see notebook for further details
+        type of preprocessing: in ["Perlman_procedure","meanimputation_standardize","same_feature_preprocessing"]. 
     subset_ : None or int
         Number of features to restrict the dataset to (Top-subset_ features in terms of cross-sample variance) /!\ across user and item features if preprocessing_str!="meanimputation_standardize" otherwise 2*subset_ features are preserved (subset_ for item features, subset_ for user features)
+    operator : None or str
+        arithmetric operation to apply, ex. "+", "*"
+    sep_feature : str
+        separator between feature type and element in the feature matrices in dataset
     filter_ : None or list
         list of feature indices to keep (of length subset_) (overrides the subset_ parameter if both are fed)
     scalerS : None or stanscofi.models.CustomScaler instance
         scaler for items; the scaler fitted on item feature vectors
     scalerP : None or stanscofi.models.CustomScaler instance
         scaler for users; the scaler fitted on user feature vectors
     inf : float or int
         placeholder value for infinity values (positive : +inf, negative : -inf)
     njobs : int
         number of jobs to run in parallel (njobs > 0) for the Perlman procedure
 
     Returns
     ----------
-    X : array-like of shape (n_items x n_users, n_item_features+n_user_features)
+    X : array-like of shape (n_folds, n_features)
         the feature matrix
-    y : array-like of shape (n_items x n_users, )
+    y : array-like of shape (n_folds, )
         the response/outcome vector
     scalerS : None or stanscofi.models.CustomScaler instance
         scaler for items; if the input value was None, returns the scaler fitted on item feature vectors
     scalerP : None or stanscofi.models.CustomScaler instance
         scaler for users; if the input value was None, returns the scaler fitted on user feature vectors
     filter_ : None or list
         list of feature indices to keep (of length subset_)
     '''
     assert njobs>0
     assert preprocessing_str in ["Perlman_procedure","meanimputation_standardize","same_feature_preprocessing"]
     if (preprocessing_str == "Perlman_procedure"):
-        X, y = eval(preprocessing_str)(dataset, njobs=njobs, sep_feature="-", missing=-666, verbose=False)
+        X, y = eval(preprocessing_str)(dataset, njobs=njobs, sep_feature=sep_feature, missing=-666, verbose=False)
         scalerS, scalerP = None, None
     if (preprocessing_str == "meanimputation_standardize"):
         X, y, scalerS, scalerP = eval(preprocessing_str)(dataset, subset=subset_, scalerS=scalerS, scalerP=scalerP, inf=inf, verbose=False)
     if (preprocessing_str == "same_feature_preprocessing"):
-        X, y = eval(preprocessing_str)(dataset)
+        X, y = eval(preprocessing_str)(dataset, operator)
         scalerS, scalerP = None, None
     if (preprocessing_str != "meanimputation_standardize"):
         if ((subset_ is not None) or (filter_ is not None)):
             if ((subset_ is not None) and (filter_ is None)):
                 with np.errstate(over="ignore"):
                     x_vars = [np.nanvar(X[:,i]) if (np.sum(~np.isnan(X[:,i]))>0) else 0 for i in range(X.shape[1])]
                     x_vars = [x if (not np.isnan(x) and not np.isinf(x)) else 0 for x in x_vars]
                     x_ids_vars = np.argsort(x_vars).tolist()
                     features = x_ids_vars[-subset_:]
                     filter_ = features
             X = X[:,filter_]
+    assert X.shape[0]==y.shape[0]==dataset.folds.data.shape[0]
     return X, y, scalerS, scalerP, filter_
 
 class CustomScaler(object):
     '''
     A class used to encode a simple preprocessing pipeline for feature matrices. Does mean imputation for features, feature filtering, correction of infinity errors and standardization
 
     ...
@@ -180,65 +184,62 @@
     scalerP : None or sklearn.preprocessing.StandardScaler instance
         scaler for users
     verbose : bool
         prints out information
 
     Returns
     ----------
-    X : array-like of shape (n_items x n_users, n_item_features+n_user_features)
+    X : array-like of shape (n_folds, n_item_features+n_user_features)
         the feature matrix
-    y : array-like of shape (n_items x n_users, )
+    y : array-like of shape (n_folds, )
         the response/outcome vector
     scalerS : None or stanscofi.models.CustomScaler instance
         scaler for items; if the input value was None, returns the scaler fitted on item feature vectors
     scalerP : None or stanscofi.models.CustomScaler instance
         scaler for users; if the input value was None, returns the scaler fitted on user feature vectors
     '''
-    y = np.ravel(dataset.ratings_mat.flatten())
+    y = dataset.ratings.toarray()[dataset.folds.row,dataset.folds.col].ravel()
     if (scalerS is None):
         scalerS = CustomScaler(posinf=inf, neginf=-inf)
     if (verbose):
         print("<preprocessing.meanimputation_standardize> Preprocessing of item feature matrix...")
-    S_ = scalerS.fit_transform(dataset.items.T.copy(), subset=subset, verbose=verbose) ## items x features=subset
+    S_ = scalerS.fit_transform(dataset.items.toarray().T, subset=subset, verbose=verbose) ## items x features=subset
     if (scalerP is None):
         scalerP = CustomScaler(posinf=inf, neginf=-inf)
     if (verbose):
         print("<preprocessing.meanimputation_standardize> Preprocessing of user feature matrix...")
-    P_ = scalerP.fit_transform(dataset.users.T.copy(), subset=subset, verbose=verbose) ## users x features=subset
-    ids = np.argwhere(np.ones(dataset.ratings_mat.shape)) 
-    SS = np.concatenate(tuple([S_[i,:].reshape(-1,1) for i, _ in ids.tolist()]), axis=1) ## (item, user) pairs x features
-    PP = np.concatenate(tuple([P_[j,:].reshape(-1,1) for _, j in ids.tolist()]), axis=1) ## (item, user) pairs x features
-    X = np.concatenate((SS, PP), axis=0).T ## (item, user) pairs x item/user features
+    P_ = scalerP.fit_transform(dataset.users.toarray().T, subset=subset, verbose=verbose) ## users x features=subset
+    X = np.column_stack((S_[dataset.folds.row,:], P_[dataset.folds.col,:])) ## (item, user) pairs x (item + user features)
     return X, y, scalerS, scalerP
 
-def same_feature_preprocessing(dataset):
+def same_feature_preprocessing(dataset, operator):
     '''
-    If the users and items have the same features in the dataset, then a simple way to combine the user and item feature matrices is to multiply the feature vectors coefficient per coefficient.
+    If the users and items have the same features in the dataset, then a simple way to combine the user and item feature matrices is to apply an element-wise arithmetic operator (*, +, etc.) to the feature vectors coefficient per coefficient.
 
     ...
 
     Parameters
     ----------
     dataset : stanscofi.Dataset
-        dataset which should be transformed, with n_items items (with n_item_features features) and n_users users (with n_user_features features) where n_item_features==n_user_features and dataset.same_item_user_features==True, and missing values are denoted by 0 or numpy.nan
+        dataset which should be transformed, where n_item_features==n_user_features and dataset.same_item_user_features==True
+    operator : str
+        arithmetric operation to apply, ex. "+", "*"
 
     Returns
     ----------
-    X : array-like of shape (n_items x n_users, n_item_features+n_user_features)
+    X : array-like of shape (n_folds, n_features)
         the feature matrix
-    y : array-like of shape (n_items x n_users, )
+    y : array-like of shape (n_folds, )
         the response/outcome vector
     '''
-    assert dataset.same_item_user_features==True
-    y = np.ravel(dataset.ratings_mat.flatten())
-    S_, P_ = dataset.items.T.copy(), dataset.users.T.copy()
-    P_[np.isnan(P_)] = 0
-    S_[np.isnan(S_)] = 0
-    ids = np.argwhere(np.ones(dataset.ratings_mat.shape)) # (item, user) pairs
-    X = np.concatenate(tuple([np.multiply(S_[i, :], P_[j, :]).reshape(-1,1) for i, j in ids.tolist()]), axis=1).T ## pairs x features
+    assert dataset.same_item_user_features
+    y = dataset.ratings.toarray()[dataset.folds.row,dataset.folds.col].ravel()
+    S_, P_ = [np.nan_to_num(x.toarray().T, copy=True, nan=0.) for x in [dataset.items, dataset.users]]
+    S_, P_ = S_[dataset.folds.row,:], P_[dataset.folds.col,:]
+    X = eval("S_ %s P_" % operator) ## (item, user) pairs x (item + user features)
     return X, y
 
 ## https://stackoverflow.com/questions/11144513/cartesian-product-of-x-and-y-array-points-into-single-array-of-2d-points
 def cartesian_product_transpose(*arrays):
     broadcastable = np.ix_(*arrays)
     broadcasted = np.broadcast_arrays(*broadcastable)
     rows, cols = np.prod(broadcasted[0].shape), len(broadcasted)
@@ -246,40 +247,40 @@
     out = np.empty(rows * cols, dtype=dtype)
     start, end = 0, rows
     for a in broadcasted:
         out[start:end] = a.reshape(-1)
         start, end = end, end + rows
     return out.reshape(cols, rows).T
 
-def Perlman_procedure(dataset, njobs=1, sep_feature="-", missing=-666, inf=2, verbose=False):
+def Perlman_procedure(dataset, njobs=1, sep_feature=None, missing=-666, inf=2, verbose=False):
     '''
     Method for combining (several) item and user similarity matrices (reference DOI: 10.1089/cmb.2010.0213). Instead of concatenating item and user features for a given pair, resulting in a vector of size (n_items x n_item_matrices)+(n_users x n_user_matrices), compute a single score per pair of (item_matrix, user_matrix) for each (item, user) pair, resulting in a vector of size (n_item_matrices) x (n_user_matrices).
 
     The score for any item i, user u, item-item similarity fi and user-user similarity fu is
     score_{fi,fu}(i,u) = max { sqrt(fi(dr, dr') x fu(di', di))  | (i',u')!=(i,u), fi(dr, dr')!=NaN, fu(di', di)!=NaN, rating(i',u')!=0 }
 
     Then the final feature matrix is X = (X_{i,j})_{i,j} for i a (item, user) pair and j a (item similarity, user similarity) pair
 
     ...
 
     Parameters
     ----------
     dataset : stanscofi.Dataset
         dataset which should be transformed, with n_items items (with n_item_features features) and n_users users (with n_user_features features) with the following attributes
-            ratings_mat : array-like of shape (n_ratings, 3)
-                a matrix which contains the user indices (column 1), the item indices (column 2) and the class for the corresponding (user, item) pair (value in {-1, 0, 1} in column 3), where 0 stands for unknown class, -1 for negative and 1 for positive classes
-            users : array-like of shape (n_diseases x n_disease_features, n_diseases)
-                concatenation of n_disease_features drug similarity matrices of shape (n_diseases, n_diseases), where values in user_features are denoted by "<feature><sep_feature><disease>" and missing values are denoted by numpy.nan; if the prefix in "<feature><sep_feature>" is missing, it is assumed that users is a single similarity matrix (n_user_matrices=1)
-            items : array-like of shape (n_drugs x n_drug_features, n_drugs)
+            ratings : COO-array of shape (n_items, n_users)
+                an array which contains values in {-1, 0, 1} describing the negative, unlabelled/unavailable, positive user-item matchings
+            items : COO-array of shape (n_item_features, n_items)
                 concatenation of n_drug_features drug similarity matrices of shape (n_drugs, n_drugs), where values in item_features are denoted by "<feature><sep_feature><drug>" and missing values are denoted by numpy.nan; if the prefix in "<feature><sep_feature>" is missing, it is assumed that items is a single similarity matrix (n_item_matrices=1)
+            users : COO-array of shape (n_user_features, n_users)
+                concatenation of n_disease_features drug similarity matrices of shape (n_diseases, n_diseases), where values in user_features are denoted by "<feature><sep_feature><disease>" and missing values are denoted by numpy.nan; if the prefix in "<feature><sep_feature>" is missing, it is assumed that users is a single similarity matrix (n_user_matrices=1)
         NaN values are replaced by 0, whereas infinite values are replaced by inf (parameter below).
     njobs : int
         number of jobs to run in parallel
-    sep_feature : str
-        separator between feature type and element in the feature matrices in dataset
+    sep_feature : str or None
+        separator between feature type and element in the feature matrices in dataset. None if there is one single feature type expected
     missing : int
         placeholder value that should be different from any feature name
     inf : int
         Value that replaces infinite values in the dataset (inf for +infinity, -inf for -infinity)
     verbose : bool
         prints out information
 
@@ -287,45 +288,46 @@
     ----------
     X : array-like of shape (n_items x n_users, n_item_features x n_user_features)
         the feature matrix
     y : array-like of shape (n_items x n_users, )
         the response/outcome vector 
     '''
     assert njobs > 0
-    is_user = sum([int(sep_feature in str(x)) for x in dataset.user_features])
-    is_item = sum([int(sep_feature in str(x)) for x in dataset.item_features])
-    assert is_user in [0, dataset.users.shape[0]]
-    assert is_item in [0, dataset.items.shape[0]]
-    A, P, S = dataset.ratings_mat.copy(), dataset.users.copy(), dataset.items.copy()
-    np.nan_to_num(P, copy=False, nan=0, posinf=inf, neginf=-inf)
-    np.nan_to_num(S, copy=False, nan=0, posinf=inf, neginf=-inf)
+    if (sep_feature is not None):
+        is_user = sum([int(sep_feature in str(x)) for x in dataset.user_features])
+        is_item = sum([int(sep_feature in str(x)) for x in dataset.item_features])
+    else:
+        is_user, is_item = 0, 0
+    if ((is_user not in [0, dataset.users.shape[0]]) or (is_item not in [0, dataset.items.shape[0]])):
+        print("Ensure that sep_feature(=\"%s\") is set to the correct value. If there is only one type of feature, set this parameter to None." % str(sep_feature))
+        assert is_user in [0, dataset.users.shape[0]]
+        assert is_item in [0, dataset.items.shape[0]]
+    y = dataset.ratings.toarray()[dataset.folds.row,dataset.folds.col].ravel()
+    P, S = [np.nan_to_num(x.toarray(), copy=True, nan=0, posinf=inf, neginf=-inf) for x in [dataset.users, dataset.items]]
     ## Ensure positive values in P and S
-    P = P-np.tile(np.nanmin(P, axis=1), (P.shape[1], 1)).T
-    S = S-np.tile(np.nanmin(S, axis=1), (S.shape[1], 1)).T
-    y = np.ravel(A.flatten())
-    ## All item,user pairs (items x users)
-    ids = np.argwhere(np.ones(A.shape)) 
+    P, S = [x-np.tile(np.nanmin(x, axis=1), (x.shape[1], 1)).T for x in [P, S]]
     ## All types of features (length=#features)
     nuser_features = np.array([missing]*len(dataset.user_features) if (is_user==0) else [x.split(sep_feature)[0] for x in dataset.user_features])
     nitem_features = np.array([missing]*len(dataset.item_features) if (is_item==0) else [x.split(sep_feature)[0] for x in dataset.item_features])
     ## All item/user corresponding to each type of feature (length=#features)
     ## In subset datasets some features might relate to absent diseases/drugs
     nuser_nms = np.array([dataset.user_list.index(x) if (x in dataset.user_list) else missing for x in (dataset.user_features if (is_user==0) else [y.split(sep_feature)[1] for y in dataset.user_features])])
     nitem_nms = np.array([dataset.item_list.index(x) if (x in dataset.item_list) else missing for x in (dataset.item_features if (is_item==0) else [y.split(sep_feature)[1] for y in dataset.item_features])])
     Nuf, Nif = len(set(nuser_features)), len(set(nitem_features))
     if (verbose):
         print("<preprocessing.Perlman_procedure> %d item similarities, %d user similarities" % (Nuf, Nif))
-    X = np.zeros((ids.shape[0], Nuf*Nif)) ## (item, user) pairs x feature type
-    if (verbose):
-        print("<preprocessing.Perlman_procedure> For %d ratings pairs, identified %d features" % X.shape)
     item_feature_mask = {fi: (nitem_features==fi).astype(int) for fi in set(nitem_features)}
-    item_mask = [S[:,i] * (nitem_nms!=i).astype(int) for i in range(A.shape[0])]
+    item_mask = [S[:,i] * (nitem_nms!=i).astype(int) for i in range(dataset.nitems)]
     user_feature_mask = {fu: (nuser_features==fu).astype(int) for fu in set(nuser_features)}
-    user_mask = [P[:,u] * (nuser_nms!=u).astype(int) for u in range(A.shape[1])]
-    known = np.array([0 if ((nitem_nms[i]==missing) or (nuser_nms[u]==missing)) else int(A[nitem_nms[i],nuser_nms[u]]!=0) for i in range(S.shape[0]) for u in range(P.shape[0])])
+    user_mask = [P[:,u] * (nuser_nms!=u).astype(int) for u in range(dataset.nusers)]
+    known = np.array([0 if ((nitem_nms[i]==missing) or (nuser_nms[u]==missing)) else int(dataset.ratings.toarray()[nitem_nms[i],nuser_nms[u]]!=0) for i in range(S.shape[0]) for u in range(P.shape[0])])
+    ## All item,user pairs (items x users)
+    ids = np.array([dataset.folds.row, dataset.folds.col]).T
+    if (verbose):
+        print("<preprocessing.Perlman_procedure> For %d ratings pairs, identified %d features" % (ids.shape[0], Nuf*Nif))
     features = [[a,b] for a in set(nitem_features) for b in set(nuser_features)]
     def single_run(fi, fu, known, item_feature_mask, item_mask, user_feature_mask, user_mask, ids):
         if (verbose):
             print("<preprocessing.Perlman_procedure> Considering item feature '%s' and user feature '%s' (%d jobs)" % (str(fi) if (fi!=missing) else "{1}", str(fu) if (fu!=missing) else "{1}", njobs))
         vals = [None]*ids.shape[0]
         for ii, [i, u] in enumerate(ids.tolist()):
             item_mat = item_feature_mask[fi] * item_mask[i]
@@ -333,9 +335,9 @@
             all_sim = np.prod(cartesian_product_transpose(item_mat, user_mat), axis=1)
             vals[ii] = np.max(np.multiply(all_sim, known))
         return vals
     if (njobs==1):
         vals = [single_run(fi, fu, known, item_feature_mask, item_mask, user_feature_mask, user_mask, ids) for [fi, fu] in tqdm(features)]
     else:
         vals = Parallel(n_jobs=min(njobs, len(features)), backend='loky')(delayed(single_run)(fi, fu, known, item_feature_mask, item_mask, user_feature_mask, user_mask, ids) for [fi, fu] in tqdm(features))
-    X = np.array(vals).T
-    return np.sqrt(X), y
+    X = np.sqrt(np.array(vals).T)
+    return X, y
```

### Comparing `stanscofi-1.1.0/src/stanscofi/training_testing.py` & `stanscofi-2.0.0/src/stanscofi/training_testing.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,118 +1,183 @@
 #coding: utf-8
 
 import pandas as pd
+import random
 import numpy as np
 from copy import deepcopy
 from joblib import Parallel, delayed
 from tqdm import tqdm
+from scipy.sparse import coo_array
 
 from scipy.cluster.hierarchy import linkage, fcluster
 from scipy.spatial.distance import squareform
 from sklearn.metrics import pairwise_distances
-from sklearn.model_selection import StratifiedKFold
+from sklearn.model_selection import StratifiedKFold, train_test_split
 
-import stanscofi.validation
+from .validation import compute_metrics, plot_metrics, metrics_list
 
-##############################
-# Weak correlation splitting #
-##############################
+#######################################
+# Weak correlation / random splitting #
+#######################################
+
+def indices_to_folds(indices, indices_array, shape):
+    '''
+    Converts indices of datapoints into folds as defined in stanscofi
+
+    ...
+
+    Parameters
+    ----------
+    indices : array-like of size (n_selected_ratings, )
+        flat indices of selected datapoints
+    indices_array : array-like of size (n_total_ratings, 2)
+        corresponding row and column indices of datapoints
+    shape : tuple of integers of size 2
+        total numbers of rows and columns
+
+    Returns
+    ----------
+    folds : COO-array of shape shape
+        folds which can be fed to other functions in stanscofi, e.g., dataset.subset(folds)
+    '''
+    row = indices_array[indices,0].ravel()
+    col = indices_array[indices,1].ravel()
+    data = np.ones(indices.shape[0])
+    return coo_array((data, (row, col)), shape=shape)
+
+def random_simple_split(dataset, test_size, metric="cosine", random_state=1234):
+    '''
+    Splits the data into training and testing datasets randomly.
+
+    ...
+
+    Parameters
+    ----------
+    dataset : stanscofi.Dataset
+        dataset to split
+    test_size : float
+        value between 0 and 1 (strictly) which indicates the maximum percentage of initial data (positive and negative ratings) being assigned to the test dataset
+    metric : str
+        metric to consider to assess distance between training and testing sets. Should belong to [‘cityblock’, ‘cosine’, ‘euclidean’, ‘l1’, ‘l2’, ‘manhattan’, ‘braycurtis’, ‘canberra’, ‘chebyshev’, ‘correlation’, ‘dice’, ‘hamming’, ‘jaccard’, ‘kulsinski’, ‘mahalanobis’, ‘minkowski’, ‘rogerstanimoto’, ‘russellrao’, ‘seuclidean’, ‘sokalmichener’, ‘sokalsneath’, ‘sqeuclidean’, ‘yule’]
+    random_state : int
+        random seed 
+
+    Returns
+    ----------
+    cv_folds : list of COO-array of shape (n_items, n_users)
+        list of arrays which contain values in {0, 1} describing the unavailable and available user-item matchings in the training (resp. testing) set
+    dist_train_test, dist_train, dist_test : float
+        minimum nonzero distance between an element in the training and in the testing sets, resp. inside the training set, resp. inside the testing set
+    '''
+    X = np.column_stack((dataset.folds.row, dataset.folds.col)) ## indices for available ratings
+    y = dataset.ratings.toarray()[dataset.folds.row,dataset.folds.col].ravel() ## values for available ratings
+    train_set, test_set,_,_ = train_test_split(X, y, test_size=test_size, random_state=random_state, shuffle=True, stratify=y)
+    cv_folds = tuple([
+                coo_array((np.ones(x.shape[0]), (x[:,0].ravel(), x[:,1].ravel())), 
+                        shape=dataset.folds.shape) for x in [train_set, test_set]
+    ])
+    item_matrix = np.nan_to_num(dataset.items.toarray(), copy=True, nan=0)
+    dist = pairwise_distances(item_matrix.T, metric=metric)
+    items_train, item_test = [np.unique(cv_folds[i].row) for i in [0,1]]
+    dist_lst = (
+        np.ma.masked_equal(dist[items_train,:][:,item_test], 0.0, copy=True).min(), 
+        np.ma.masked_equal(dist[items_train,:][:,items_train], 0.0, copy=True).min(), 
+        np.ma.masked_equal(dist[item_test,:][:,item_test], 0.0, copy=True).min()
+    )
+    return cv_folds, dist_lst
 
-def print_folds(folds, dataset, fold_name="Fold"):
+def random_cv_split(dataset, cv_generator, metric="cosine"):
     '''
-    Prints out information about a folds: number of unique drugs resp., diseases, number of considered ratings, proportion of positive and negative ratings
+    Splits the data into training and testing datasets randomly for cross-validation.
 
     ...
 
     Parameters
     ----------
-    folds : array-like of shape (n_ratings, 3)
-        a matrix which contains the user indices (column 1), the item indices (column 2) and the class for the corresponding (user, item) pair (value in {-1, 0, 1} in column 3)
     dataset : stanscofi.Dataset
-        dataset which can be subsetted by folds
-    fold_name : str
-        name given to the fold
-    '''
-    if (len(folds)==0):
-        print("<training_testing.print_folds> Fold is empty.")
-        return None
-    assert folds.shape[1]==3
-    assert np.max(folds[:,0])<=dataset.ratings_mat.shape[1]
-    assert np.max(folds[:,1])<=dataset.ratings_mat.shape[0]
-    assert ((folds[:,-1]==1)|(folds[:,-1]==-1)|(folds[:,-1]==0)).all()
-    name, ndrugs, ndiseases = [fold_name]+[np.unique(folds[:,x]).shape[0] for x in [1,0]]
-    nratings, percratings = [folds.shape[0], folds.shape[0]*100/dataset.ratings.shape[0]]
-    args = [name, ndrugs, ndiseases, nratings, percratings]
-    print("\n<training_testing.print_folds> %s: %d unique drugs and %d unique diseases and %d ratings (%.2f perc.)" % tuple(args))
-    counts = [ndrugs*ndiseases-folds.shape[0]]+[np.sum(folds[:,-1]==v) for v in [1,-1]]
-    print(pd.DataFrame(counts, index=[0,1,-1], columns=["counts"]).T)
+        dataset to split
+    cv_generator : scikit-learn cross-validation index generator
+        e.g. StratifiedKFold, KFold
+    metric : str
+        metric to consider to assess distance between training and testing sets. Should belong to [‘cityblock’, ‘cosine’, ‘euclidean’, ‘l1’, ‘l2’, ‘manhattan’, ‘braycurtis’, ‘canberra’, ‘chebyshev’, ‘correlation’, ‘dice’, ‘hamming’, ‘jaccard’, ‘kulsinski’, ‘mahalanobis’, ‘minkowski’, ‘rogerstanimoto’, ‘russellrao’, ‘seuclidean’, ‘sokalmichener’, ‘sokalsneath’, ‘sqeuclidean’, ‘yule’]
 
-def traintest_validation_split(dataset, test_size, early_stop=None, metric="cosine", disjoint_users=False, random_state=1234, verbose=False, print_dists=False):
+    Returns
+    ----------
+    cv_folds : list of size nsplits of COO-array of shape (n_items, n_users)
+        list of arrays which contain values in {0, 1} describing the unavailable and available user-item matchings in the training (resp. testing) set
+    dist_lst : list of size nsplits of tuples of float of size 3
+        for each fold, minimum nonzero distance between an element in the training and in the testing sets, resp. inside the training set, resp. inside the testing set
+    '''
+    X = np.column_stack((dataset.folds.row, dataset.folds.col)) ## indices for available ratings
+    y = dataset.ratings.toarray()[dataset.folds.row,dataset.folds.col].ravel() ## values for available ratings
+    cv_folds = [
+        (
+            indices_to_folds(train_index, X, dataset.folds.shape), 
+            indices_to_folds(test_index, X, dataset.folds.shape)
+        ) for train_index, test_index in cv_generator.split(X, y)]
+    item_matrix = np.nan_to_num(dataset.items.toarray(), copy=True, nan=0)
+    dist = pairwise_distances(item_matrix.T, metric=metric)
+    dist_lst = [(
+        np.ma.masked_equal(dist[np.unique(train_folds.row),:][:,np.unique(test_folds.row)], 0.0, copy=True).min(), 
+        np.ma.masked_equal(dist[np.unique(train_folds.row),:][:,np.unique(train_folds.row)], 0.0, copy=True).min(), 
+        np.ma.masked_equal(dist[np.unique(test_folds.row),:][:,np.unique(test_folds.row)], 0.0, copy=True).min()
+    ) for train_folds, test_folds in cv_folds]
+    return cv_folds, dist_lst
+
+def weakly_correlated_split(dataset, test_size, early_stop=None, metric="cosine", random_state=1234, verbose=False):
     '''
-    Splits the data into training and testing datasets with a low correlation
+    Splits the data into training and testing datasets with a low correlation among items, by applying a hierarchical clustering on the item feature matrix. NaNs in the item feature matrix are converted to 0. 
 
     ...
 
     Parameters
     ----------
     dataset : stanscofi.Dataset
         dataset to split
     test_size : float
-        value between 0 and 1 (strictly) which indicates the maximum percentage of initial data (known ratings) being assigned to the test dataset
+        value between 0 and 1 (strictly) which indicates the maximum percentage of initial data (positive and negative ratings) being assigned to the test dataset
     early_stop : int or None
         positive integer, which stops the cluster number search after 3 tries yielding the same number; note that if early_stop is not None, then the property on test_size will not necessarily hold anymore
     metric : str
         metric to consider to perform hierarchical clustering on the dataset. Should belong to [‘cityblock’, ‘cosine’, ‘euclidean’, ‘l1’, ‘l2’, ‘manhattan’, ‘braycurtis’, ‘canberra’, ‘chebyshev’, ‘correlation’, ‘dice’, ‘hamming’, ‘jaccard’, ‘kulsinski’, ‘mahalanobis’, ‘minkowski’, ‘rogerstanimoto’, ‘russellrao’, ‘seuclidean’, ‘sokalmichener’, ‘sokalsneath’, ‘sqeuclidean’, ‘yule’]
-    disjoint_users : bool
-        whether to split the data in four sets such that two of these sets have a disjoint set of diseases, that is,
-        if disjoint_users=False (default): Splits the initial dataset into two parts with the following properties
-            - The sets of users in both parts are disjoint
-            - The sets of items in training+testing sets and validation sets are weakly correlated
-              (by applying a hierarchical clustering on the item feature matrix, NaN are converted to 0)
-        if disjoint_users=True: Splits the initial dataset into four parts with the following properties
-            - The sets of users in train_folds and test_folds, resp. val_folds and supp_folds, 
-              resp. val_folds and train_folds, resp. test_folds and supp_folds are disjoint
-            - The sets of items are weakly correlated between
-               train_folds and test_folds/val_folds, test_folds and train_folds/supp_folds
-               and disjoint train_folds and test_folds, resp. val_folds and supp_folds, 
-              resp. val_folds and test_folds, resp. train_folds and supp_folds
-              (by applying a hierarchical clustering on the item feature matrix, NaN are converted to 0)
     random_state : int
         random seed 
     verbose : bool
         prints out information
-    print_dists : bool
-        prints distances between returned folds
 
     Returns
     ----------
-    train_folds, test_folds, val_folds, supp_folds : array-like of shape (n_ratings, 3)
-        a matrix which contains the user indices (column 1), the item indices (column 2) and the class for the corresponding (user, item) pair (value in {-1, 0, 1} in column 3)
+    train_folds, test_folds : COO-array of shape (n_items, n_users)
+        an array which contains values in {0, 1} describing the unavailable and available user-item matchings in the training (resp. testing) set
+    dist_train_test, dist_train, dist_test : float
+        minimum nonzero distance between an element in the training and in the testing sets, resp. inside the training set, resp. inside the testing set
     '''
     assert random_state > 0
     assert (early_stop is None) or (early_stop > 0)
     assert test_size > 0 and test_size < 1
     assert metric in ["cityblock", "cosine", "euclidean", "l1", "l2", "manhattan", "braycurtis", "canberra", "chebyshev", "correlation", "dice", "hamming", "jaccard", "kulsinski", "mahalanobis", "minkowski", "rogerstanimoto", "russellrao", "seuclidean", "sokalmichener", "sokalsneath", "sqeuclidean", "yule"]
     np.random.seed(random_state)
-    item_matrix = np.nan_to_num(dataset.items, copy=True)
-    ratings = dataset.ratings.copy()
-    train_nset = int((1-test_size)*ratings.shape[0])
-
-    dist = pairwise_distances(item_matrix.T,metric=metric)
-    dist_ = squareform(dist, checks=False)
-    Z = linkage(dist_, "average")
+    random.seed(random_state) 
+
+    item_matrix = np.nan_to_num(dataset.items.toarray(), copy=True, nan=0)
+    train_nset = int((1-test_size)*dataset.folds.data.shape[0])
+
+    dist = pairwise_distances(item_matrix.T, metric=metric)
+    Z = linkage(squareform(dist, checks=False), "average")
     select_nc, n_cluster_train = None, None
     l_nc, u_nc = 2, item_matrix.shape[1]
     count_sim, oldclnb = 0, None
     ## bisection to find the appropriate number of clusters, and where to split the data
     while (l_nc<u_nc):
         nc = (l_nc+u_nc)//2
         clusters = fcluster(Z, nc, criterion='maxclust', depth=2, R=None, monocrit=None)
-        nratings_train = {ratings[np.array([clusters[x]<=c for x in ratings[:,1].astype(int).tolist()]),:].shape[0]:c for c in range(1,len(np.unique(clusters))+1)}
+        nratings_train = {len([x for x in dataset.folds.row if (clusters[x]<=c)]):c for c in range(1,len(np.unique(clusters))+1)}
         select_clust = np.max([k if (k<=train_nset) else -1 for k in nratings_train])
+        #print("#training=%d\t#clust=%d\t#clusters=%d" % (train_nset, select_clust, nratings_train[select_clust]))
+        #print(np.max([k if (k<select_clust) else -1 for k in nratings_train]), select_clust, np.min([k if (k>select_clust) else len(dataset.folds.row) for k in nratings_train]))
         cluster_size = nratings_train.get(select_clust, -1)
         if (verbose):
             print("<training_testing.traintest_validation_split> Find #clusters=%d in [%d, %d] (%d ~ %d?)" % (nc, l_nc, u_nc, select_clust, train_nset))
         if (select_clust==train_nset):
             break
         if (select_clust==oldclnb):
             count_sim += 1
@@ -122,179 +187,139 @@
             oldclnb = select_clust
         if (select_clust<train_nset):
             l_nc = nc+1
         else:
             u_nc = nc
     select_nc = nc
     cluster_size = cluster_size
-    #select_nc, cluster_size = 2, 0 ## reproduce an old behavior which did not take into account the test_size parameter
+    ## reproduces an old behavior which did not take into account the test_size parameter and maximizes the distance between training and testing sets
+    #select_nc, cluster_size = 2, 0 
     item_labels = (fcluster(Z, select_nc, criterion='maxclust', depth=2, R=None, monocrit=None)>cluster_size+1).astype(int)+1
 
-    item_cluster = np.array([item_labels[item] for item in ratings[:,1].astype(int).tolist()])
-    train_set = ratings[item_cluster==1,:]
-    test_set = ratings[item_cluster==2,:]
-
-    f = lambda x : np.min(x[x!=0]) if (x[x!=0].shape[0]>0) else 0
-    get_dist = lambda s1, s2 : f(dist[np.unique(s1[:,1]).tolist(),:][:,np.unique(s2[:,1]).tolist()])
-
-    if (not disjoint_users):
-
-        if (print_dists): 
-            print("<training_testing.traintest_validation_split> The sets of items/drugs in the training/testing datasets are disjoint.")
-            print("<training_testing.traintest_validation_split> The sets of users/diseases in the training/testing datasets are *not* disjoint.")
-            print("<training_testing.traintest_validation_split> Distances:")
-            cols = ["Train set","Test set"]
-            sets = [train_set, test_set]
-            dists = pd.DataFrame([[get_dist(c1,c2) for c1 in sets] for c2 in sets], index=cols, columns=cols)
-            print(dists)
-
-        return train_set.astype(int), test_set.astype(int), np.array([]), np.array([])
-
-    user_cluster = np.array([np.sum(np.unique(item_cluster[ratings[ratings[:,0]==x,1].astype(int).tolist()])) for x in ratings[:,0].astype(int).tolist()])
-    train_set = ratings[user_cluster==1,:]
-    test_set = ratings[user_cluster==2,:]
-    validation_set = ratings[user_cluster==3,:]
-
-    ## Greedy approach to avoid computational explosion
-    ## Assign disease to the set for which the similarity with the newly added drugs is highest
-    val_users = np.unique(validation_set[:,0]).flatten().tolist()
-    val1_set = np.array([])
-    val2_set = np.array([])
-    get_subset = lambda cl : validation_set[(validation_set[:,0].flatten()==val_user)&(item_cluster[validation_set[:,1].flatten().tolist()]==cl),:]
-    for val_user in val_users:
-        valcl1, valcl2 = get_subset(1), get_subset(2)
-        #assert validation_set[validation_set[:,0].flatten()==val_user,:].shape[0]==np.sum([X.shape[0] for X in [valcl1,valcl2]])
-        train_set_ = np.concatenate((train_set, valcl1), axis=0)
-        test_set_ = np.concatenate((test_set, valcl2), axis=0)
-        #assert train_set.shape[0]+test_set.shape[0]+validation_set[validation_set[:,0].flatten()==val_user,:].shape[0]==np.sum([X.shape[0] for X in [train_set_,test_set_]])
-        dist_train = get_dist(train_set_, test_set)
-        dist_test = get_dist(train_set, test_set_)
-        #print((dist_test, dist_train, test_set.shape[0], valcl2.shape[0], train_set.shape[0], valcl1.shape[0]))
-        if (np.isclose(dist_test,dist_train)): # if equality
-                weights = [x.shape[0]/(train_set.shape[0]+test_set.shape[0]) for x in [train_set, test_set]]
-                dist_test += np.random.choice([-1,1], p=weights, size=1)
-        if (dist_test<dist_train):
-                test_set = np.copy(test_set_)
-                if (len(val1_set)==0):
-                    val1_set = np.copy(valcl1)
-                else:
-                    val1_set = np.concatenate((val1_set,valcl1), axis=0)
-        else:
-                train_set = np.copy(train_set_)
-                if (len(val2_set)==0):
-                    val2_set = np.copy(valcl2)
-                else:
-                    val2_set = np.concatenate((val2_set,valcl2), axis=0)
-
-    if (print_dists): 
-        print("<training_testing.traintest_validation_split> The sets of items/drugs in the training/testing datasets, in the validation/supplementary datasets, in the validation/testing and in the supplementary/training datasets are disjoint.")
-        print("<training_testing.traintest_validation_split> The sets of items/drugs in the training/testing datasets, in the validation/supplementary datasets, in the validation/training and in the supplementary/testing datasets are disjoint.")
-        print("<training_testing.traintest_validation_split> Distances")
-        cols = ["Train set","Test set","Val set","Supp set"]
-        sets = [train_set, test_set, val1_set, val2_set]
-        dists = pd.DataFrame([[np.nan if ((len(c1)==0) or (len(c2)==0)) else get_dist(c1,c2) for c1 in sets] for c2 in sets], index=cols, columns=cols)
-        print(dists)
+    ## COO-array of shape (n_items, n_users)
+    train_folds = dataset.folds.toarray()
+    train_folds[item_labels==2,:] = 0
+    test_folds = dataset.folds.toarray()-train_folds
+
+    dist_lst = (
+        np.ma.masked_equal(dist[item_labels==1,:][:,item_labels==2], 0.0, copy=True).min(), 
+        np.ma.masked_equal(dist[item_labels==1,:][:,item_labels==1], 0.0, copy=True).min(), 
+        np.ma.masked_equal(dist[item_labels==2,:][:,item_labels==2], 0.0, copy=True).min()
+    )
 
-    return train_set.astype(int), test_set.astype(int), val1_set.astype(int), val2_set.astype(int)
+    return (coo_array(train_folds), coo_array(test_folds)), dist_lst
 
 ##############################
 # Common training procedure  #
 ##############################
 
-def cv_training(template, params, train_dataset, is_masked=False, metric="AUC", beta=1, njobs=1, nsplits=5, random_state=1234, show_plots=True, verbose=False):
+def cv_training(template, params, train_dataset, nsplits, metric, k=1, beta=1, threshold=0, test_size=0.2, dist_type="cosine", cv_type=["random","weakly_correlated"][0], early_stop=2, njobs=1, random_state=1234, show_plots=False, verbose=False):
     '''
-    Trains a model on a dataset using cross-validation using sklearn.model_selection.StratifiedKFold
+    Trains a model on a dataset using cross-validation and custom metrics using sklearn.model_selection.StratifiedKFold
 
     ...
 
     Parameters
     ----------
     template : stanscofi.BasicModel or subclass
         type of model to train
     params : dict
         dictionary of parameters to initialize the model
     train_dataset : stanscofi.Dataset
         dataset to train upon
-    metric : str
-        metric to optimize the model upon. Should belong to ["AUC", "F_%.1f" % <beta>] where <beta> is a parameter of cv_training
-    beta : float
-        beta for the computation of a F_beta score
-    njobs : int
-        number of jobs to run in parallel. Should be lower than nsplits-1
     nsplits : int
         number of cross-validation steps
-    random_state : int
+    metric : str 
+        metric to optimize the model upon. Implemented metrics are in validation.py
+    k : int (default: 1)
+        Argument of the metric to optimize. Implemented metrics are in validation.py
+    beta : float (default: 1)
+        Argument of the metric to optimize. Implemented metrics are in validation.py
+    threshold : float (default: 0)
+        decision threshold
+    test_size : float (default: 0.2)
+        percentage of testing set (if cv_type="weakly_correlated")
+    dist_type : str (default: "cosine")
+        type of metric for splitting (if cv_type="weakly_correlated")
+    cv_type : str (default: "random")
+        type of split to apply to the dataset. Can either be "random" or "weakly_correlated"
+    early_stop : int or None
+        positive integer, which stops the cluster number search after 3 tries yielding the same number; note that if early_stop is not None, then the property on test_size will not necessarily hold anymore
+    njobs : int (default: 1)
+        number of jobs to run in parallel. Should be lower than nsplits-1
+    random_state : int (default: 1234)
         random seed
-    show_plots : bool
+    show_plots : bool (default: False)
         shows the validation plots at each cross-validation step
-    verbose : bool
+    verbose : bool (default: False)
         prints out information
 
     Returns
     ----------
-    best_estimator : dict
+    results : dict
         a dictionary which contains 
-            "test_"+metric : float
-                the best metric obtained across all validations on the testing set
-            "train_"+metric : float
-                the metric obtained on the training set in the best cross-validation step
-            "model_params" : dict
-                the parameters of the best performing model
-            "cv_folds" : tuple of array-like of shape (n_ratings, 3)
-                the corresponding training and testing folds for the best cross-validation step, where a fold is a matrix which contains the user indices (column 1), the item indices (column 2) and the class for the corresponding (user, item) pair (value in {-1, 0, 1} in column 3)
+            "models" : list of subinstances of stanscofi.models.BasicModel of length nsplits
+                all trained models
+            "train_metric" : list of floats of length nsplits
+                all metrics on training sets
+            "test_metric" : list of floats of length nsplits
+                all metrics on testing sets
+            "cv_folds" : list of COO-array of shape (n_items, n_users) of length nsplits
+                the training and testing folds for each split
     '''
-    assert beta > 0
+    assert cv_type in ["random", "weakly_correlated"]
     assert random_state > 0
+    assert test_size >0 and test_size<1
     assert nsplits > 1
-    assert metric in ["AUC", "F_%.1f" % beta]
     assert njobs in range(nsplits)
-    cv_generator = StratifiedKFold(n_splits=nsplits, shuffle=True, random_state=random_state)
-    Nitems, Nusers = len(np.unique(train_dataset.ratings[:,0])), len(np.unique(train_dataset.ratings[:,1]))
-    grid = np.indices((Nitems,Nusers))
-    full_list = np.zeros((Nitems*Nusers, 3))
-    full_list[:,0] = grid[0].flatten()
-    full_list[:,1] = grid[1].flatten()
-    full_list[:,2] = [train_dataset.ratings_mat[j,i] for i,j in full_list[:,:2].astype(int).tolist()]
-    full_list = full_list.astype(int)
-    cv_folds = cv_generator.split(full_list[:,:2], np.ravel(full_list[:,2]))
-    best_estimator, best_metric = {}, -float("inf")
-    def single_run(ncv, tfolds, sfolds, full_list):
-        if (verbose):
-            print("Crossvalidation step #%d/%d" % (ncv+1,nsplits))
+    assert metric in metrics_list
+
+    np.random.seed(random_state)
+    random.seed(random_state)
+    parallel = Parallel(n_jobs=njobs, verbose=verbose)
+
+    if (cv_type=="random"):
+        cv_generator = StratifiedKFold(n_splits=nsplits, shuffle=True, random_state=random_state)
+        cv_folds, _ = random_cv_split(train_dataset, cv_generator)
+    else:
+        seeds = np.random.choice(range(int(1e8)), size=nsplits)
+        cv_folds = [weakly_correlated_split(train_dataset, test_size, metric=dist_type, early_stop=early_stop, random_state=sd)[0] for sd in seeds]
+
+    def single_run(ncv, template, params, metric, tfolds, sfolds):
         model = template(params)
-        if (is_masked):
-            tdataset = train_dataset.mask_dataset(full_list[tfolds,:])
-            sdataset = train_dataset.mask_dataset(full_list[sfolds,:])            
-        else:
-            tdataset = train_dataset.get_folds(full_list[tfolds,:])
-            sdataset = train_dataset.get_folds(full_list[sfolds,:])
-        model.fit(tdataset)
-        scores_train = model.predict(tdataset)
-        predictions_train = model.classify(scores_train)
-        metrics_train, _ = stanscofi.validation.compute_metrics(scores_train, predictions_train, tdataset, beta=beta, verbose=verbose)
-        scores_test = model.predict(sdataset)
-        predictions_test = model.classify(scores_test)
-        metrics_test, plot_args = stanscofi.validation.compute_metrics(scores_test, predictions_test, sdataset, beta=beta, verbose=verbose)
+        tdataset = train_dataset.subset(tfolds)
+        sdataset = train_dataset.subset(sfolds)
+        model.fit(tdataset, seed=1234)
+        scores_train = model.predict_proba(tdataset)
+        predictions_train = model.predict(scores_train, threshold)
+        #print((tdataset.folds.data.shape[0], predictions_train.data.shape[0], scores_train.data.shape[0]))
+        metrics_train, _ = compute_metrics(scores_train, predictions_train, tdataset, metrics=[metric], verbose=verbose)
+        scores_test = model.predict_proba(sdataset)
+        predictions_test = model.predict(scores_test, threshold)
+        #print((sdataset.folds.data.shape[0], predictions_test.data.shape[0], scores_test.data.shape[0]))
+        metrics_test, plot_args = compute_metrics(scores_test, predictions_test, sdataset, metrics=[metric], k=k, beta=beta, verbose=verbose)
         if (show_plots):
-            stanscofi.validation.plot_metrics(**plot_args, figsize=(10,10), model_name="%s on %s (cv%d)\n" % (model.name, train_dataset.name, ncv+1))
-        return metrics_train.loc[metric][metrics_train.columns[0]], metrics_test.loc[metric][metrics_test.columns[0]], [tfolds, sfolds], params
-    if (njobs==1):
-        metrics_list = [single_run(ncv, tfolds, sfolds, full_list) for ncv, [tfolds, sfolds] in tqdm(enumerate(cv_folds))]
-    else:
-        metrics_list = Parallel(n_jobs=njobs, backend='loky')(delayed(single_run)(ncv, tfolds, sfolds, full_list) for ncv, [tfolds, sfolds] in tqdm(enumerate(cv_folds)))
-    metric_test = [m for _, m, _, _ in metrics_list]
-    best_id = np.argmax(metric_test)
-    best_metric = metric_test[best_id]
-    best_train_metric = metrics_list[best_id][0]
-    best_model = metrics_list[best_id][3]
-    best_folds = [full_list[ids,:] for ids in metrics_list[best_id][2]]
-    best_estimator = {"test_"+metric: best_metric, "train_"+metric: best_train_metric, "model_params": best_model, "cv_folds": best_folds}
-    return best_estimator
+            plot_metrics(**plot_args, figsize=(10,10), model_name="%s on %s (cv%d)\n" % (model.name, train_dataset.name, ncv+1))
+        metric_train, metric_test = metrics_train.loc[metric][metrics_train.columns[0]], metrics_test.loc[metric][metrics_test.columns[0]]
+        if (verbose):
+            print("Crossvalidation step #%d/%d (train %s %f, test %s %f)" % (ncv+1,nsplits,metric,metric_train,metric,metric_test))
+        return model, metric_train, metric_test
+
+    results = parallel(
+        delayed(single_run)(
+            ncv, deepcopy(template), params, metric, tfolds, sfolds
+        ) for ncv, (tfolds, sfolds) in enumerate(cv_folds)
+    )
+    return {"models": [r[0] for r in results], "train_metric": [r[1] for r in results], "test_metric": [r[2] for r in results], "cv_folds": cv_folds}
 
-def grid_search(search_params, template, params, train_dataset, is_masked=False, metric="AUC", njobs=1, nsplits=5, random_state=1234, show_plots=True, verbose=False):
+##############################
+# Hyperparameter search      #
+##############################
+
+def grid_search(search_params, template, params, train_dataset, nsplits, metric, k=1, beta=1, threshold=0, test_size=0.2, dist_type="cosine", cv_type=["random","weakly_correlated"][0], early_stop=2, njobs=1, random_state=1234, show_plots=False, verbose=False):
     '''
     Grid-search over hyperparameters, iteratively optimizing over one parameter at a time, and internally calling cv_training.
 
     ...
 
     Parameters
     ----------
@@ -302,51 +327,58 @@
         a dictionary which contains as keys the hyperparameter names and as values the corresponding intervals to explore during the grid-search
     template : stanscofi.BasicModel or subclass
         type of model to train
     params : dict
         dictionary of parameters to initialize the model
     train_dataset : stanscofi.Dataset
         dataset to train upon
-    metric : str
-        metric to optimize the model upon. Should belong to ["AUC", "F_%.1f" % <beta>] where <beta> is a parameter of cv_training
-    beta : float
-        beta for the computation of a F_beta score
-    njobs : int
+    metric : str 
+        metric to optimize the model upon. Implemented metrics are in validation.py
+    k : int (default: 1)
+        Argument of the metric to optimize. Implemented metrics are in validation.py
+    beta : float (default: 1)
+        Argument of the metric to optimize. Implemented metrics are in validation.py
+    threshold : float (default: 0)
+        decision threshold
+    test_size : float (default: 0.2)
+        percentage of testing set (if cv_type="weakly_correlated")
+    dist_type : str (default: "cosine")
+        type of metric for splitting (if cv_type="weakly_correlated")
+    cv_type : str (default: "random")
+        type of split to apply to the dataset. Can either be "random" or "weakly_correlated"
+    njobs : int (default: 1)
         number of jobs to run in parallel. Should be lower than nsplits-1
-    nsplits : int
-        number of cross-validation steps
-    random_state : int
+    random_state : int (default: 1234)
         random seed
-    show_plots : bool
+    show_plots : bool (default: False)
         shows the validation plots at each cross-validation step
-    verbose : bool
+    verbose : bool (default: False)
         prints out information
 
     Returns
     ----------
     best_params : dict
         a dictionary which contains as keys the hyperparameter names and as values the best values obtained across all grid-search steps
-    best_estimator : dict
+    best_model : subinstance of stanscofi.models.BasicModel
+        the best trained model associated with the best parameters
+    metrics : dict        
         a dictionary which contains 
-            "test_"+metric : float
-                the best metric obtained across all validations on the testing set
-            "train_"+metric : float
-                the metric obtained on the training set in the best cross-validation step
-            "model_params" : dict
-                the parameters of the best performing model
-            "cv_folds" : tuple of array-like of shape (n_ratings, 3)
-                the corresponding training and testing folds for the best cross-validation step, where a fold is a matrix which contains the user indices (column 1), the item indices (column 2) and the class for the corresponding (user, item) pair (value in {-1, 0, 1} in column 3)
+            "train_metric" : float 
+                the metric on the training set on the best crossvalidation split for the best set of parameters
+            "test_metric" : float
+                the metric on the testing set on the best crossvalidation split for the best set of parameters
     '''
-    best_params, best_model, best_metric = {}, None, -float("inf")
+    best_params, best_model, best_test_metric, best_train_metric = {}, None, -float("inf"), 0
     for param in search_params:
         for param_val in search_params[param]:
             params_ = params.copy()
             params_.update(best_params)
             params_.update({param: param_val})
-            best_estimator = cv_training(template, params_, train_dataset, is_masked=is_masked, metric=metric, njobs=njobs, nsplits=nsplits, random_state=random_state, show_plots=show_plots, verbose=verbose)
+            results = cv_training(template, params, train_dataset, nsplits, metric=metric, threshold=threshold, test_size=test_size, dist_type=dist_type, cv_type=cv_type, early_stop=early_stop, njobs=njobs, random_state=random_state, show_plots=show_plots, verbose=verbose)
             if (verbose):
-                print("<training_testing.grid_search> [%s=%s] %s on Test %f (Train %f)" % (param, str(param_val), metric, best_estimator["test_"+metric], best_estimator["train_"+metric]))
-            if (best_estimator["test_"+metric]>best_metric):
+                print("<training_testing.grid_search> [%s=%s] best %s on Test %f (Train %f)" % (param, str(param_val), metric, np.max(results["test_metric"]), results["train_metric"][np.argmax(results["test_metric"])]))
+            if (np.max(results["test_metric"])>best_test_metric):
                 best_params.update(params_)
-                best_model = deepcopy(best_estimator)
-                best_metric = best_estimator["test_"+metric]
-    return best_params, best_model
+                best_model = deepcopy(results["models"][np.argmax(results["test_metric"])])
+                best_test_metric = np.max(results["test_metric"])
+                best_train_metric = results["train_metric"][np.argmax(results["test_metric"])]
+    return best_params, best_model, {"test_metric": best_test_metric, "train_metric": best_train_metric}
```

### Comparing `stanscofi-1.1.0/src/stanscofi/utils.py` & `stanscofi-2.0.0/src/stanscofi/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,15 @@
         the name of the dataset to load. Should belong to the following list: ["Gottlieb", "DNdataset", "Cdataset", "LRSSL", "PREDICT_Gottlieb", "TRANSCRIPT", "PREDICT"]
     save_folder : str
         the path to the folder where dataset-related files are or will be stored
 
     Returns
     -------
     dataset_di : dictionary
-        a dictionary where key "ratings_mat" contains the drug-disease matching pandas.DataFrame of shape (n_drugs, n_diseases) (where missing values are denoted by 0), key "users" correspond to the disease pandas.DataFrame of shape (n_disease_features, n_diseases), and "items" correspond to the drug feature pandas.DataFrame of shape (n_drug_features, n_drugs)
+        a dictionary where key "ratings" contains the drug-disease matching pandas.DataFrame of shape (n_drugs, n_diseases) (where missing values are denoted by 0), key "users" correspond to the disease pandas.DataFrame of shape (n_disease_features, n_diseases), and "items" correspond to the drug feature pandas.DataFrame of shape (n_drug_features, n_drugs)
     '''
     assert model_name in ["Gottlieb", "Cdataset_Aonly", "indep", "Fdataset", "DNdataset", "Cdataset", "TRANSCRIPT", "PREDICT", "LRSSL", "LRSSL2", "PREDICT_Gottlieb", "TRANSCRIPT_v1", "PREDICT_v1"]
     if (model_name == "LRSSL"):
         url_lrssl = "https://raw.githubusercontent.com/LiangXujun/LRSSL/master/"
         lrssl_dataset_path = save_folder+"LRSSL/"
         fnames = {
             "A": "drug_dis_mat.txt", "P": "disease_similarity.txt", "S1": "drug_from_drugbank_without_ind_dommat.txt",
@@ -315,30 +315,32 @@
             print("Warning: this dataset has no drug/disease names!")
         path = drrs_dataset_path+model_name+"s/"
         fnames = {"S": "DrugSim.txt", "P": "DiseaseSim.txt", "A": "DiDrA.txt"}
         A, P, S = [pd.read_csv(path+fnames[k], sep="\t", header=None) for k in ["A", "P", "S"]]
         A = A.T
         if (model_name in ["Cdataset", "Fdataset"]):
             model_name2 = "Cdataset_Aonly" if (model_name=="Cdataset") else "Gottlieb"
-            A_dataset = load_dataset(model_name2, save_folder=save_folder)["ratings_mat"]
+            A_dataset = load_dataset(model_name2, save_folder=save_folder)["ratings"]
             drug_names = list(A_dataset.index)
             disease_names = list(A_dataset.columns)
             A.index = drug_names
             S.index = drug_names
             S.columns = drug_names
             A.columns = disease_names
             P.index = disease_names
             P.columns = disease_names
     A = A.fillna(0).astype(int)
     P = P.astype(float)
     S = S.astype(float)
+    S.columns = list(map(str,S.columns))
+    P.columns = list(map(str,P.columns))
     assert A.shape[0] == S.shape[1]
     assert A.shape[1] == P.shape[1]
     assert all([a in [-1, 0, 1] for a in np.unique(A).tolist()])
-    return {"ratings_mat": A, "users": P, "items": S}
+    return {"ratings": A, "users": P, "items": S}
 
 #############################
 ## MERGING RATINGS         ##
 #############################
 
 def merge_ratings(rating_dfs, user_col, item_col, rating_col):
     '''
```

### Comparing `stanscofi-1.1.0/src/stanscofi/validation.py` & `stanscofi-2.0.0/src/stanscofi/validation.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,109 +1,157 @@
 #coding: utf-8
 
-from sklearn.metrics import roc_auc_score as AUC
-from sklearn.metrics import fbeta_score
 from sklearn.metrics import precision_recall_curve as PRC
 from sklearn.metrics import roc_curve as ROC
 
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 from copy import deepcopy
 
-def compute_metrics(scores, predictions, test_dataset, beta=1, ignore_zeroes=False, verbose=False):
+###################################
+## LIST OF AVAILABLE METRICS     ##
+###################################
+from cute_ranking.core import mean_reciprocal_rank, r_precision, precision_at_k, recall_at_k, f1_score_at_k, average_precision, mean_average_precision, dcg_at_k, ndcg_at_k, mean_rank, hit_rate_at_k
+from sklearn.metrics import roc_auc_score, fbeta_score
+from scipy.stats import kendalltau, spearmanr
+
+def ERR(y_true, y_pred, max=10, max_grade=2):
+    '''
+        source: https://raw.githubusercontent.com/skondo/evaluation_measures/master/evaluations_measures.py
+    '''
+    max=10
+    max_grade=2
+    ranking = y_true[np.argsort(-y_pred)]
+    if max is None:
+        max = len(ranking)
+    ranking = ranking[:min(len(ranking), max)]
+    ranking = map(float, ranking)
+    result = 0.0
+    prob_step_down = 1.0 
+    for rank, rel in enumerate(ranking):
+        rank += 1
+        utility = (pow(2, rel) - 1) / pow(2, max_grade)
+        result += prob_step_down * utility / rank
+        prob_step_down *= (1 - utility)  
+    return result
+AUC = lambda y_true, y_pred, k, u1 : roc_auc_score(y_true, y_pred, average="weighted")
+Fscore = lambda y_true, y_pred, u, beta : fbeta_score(y_true, y_pred, beta=beta, average="weighted")
+def TAU(y_true, y_pred, u, u1):
+    if (len(np.unique(y_pred))==1):
+        return 0
+    res = kendalltau(y_true, y_pred)
+    return res.correlation
+def Rscore(y_true, y_pred, u, u1):
+    if (len(np.unique(y_pred))==1):
+        return 0
+    res = spearmanr(y_true, y_pred)
+    return res.correlation
+MRR = lambda y_true, y_pred, u, u1 : mean_reciprocal_rank([y_true[np.argsort(-y_pred)]])
+RP = lambda y_true, y_pred, u, u1 : r_precision(y_true[np.argsort(-y_pred)])
+PrecisionK = lambda y_true, y_pred, k, u1 : precision_at_k(y_true[np.argsort(-y_pred)], k)
+RecallK = lambda y_true, y_pred, k, u1 : recall_at_k(y_true[np.argsort(-y_pred)], np.sum(y_true>0), k=k)
+def F1K(y_true, y_pred, k, u1):
+    rec = recall_at_k(y_true[np.argsort(-y_pred)], np.sum(y_true>0), k)
+    prec = precision_at_k(y_true[np.argsort(-y_pred)], k)
+    if (rec+prec==0):
+        return 0
+    return f1_score_at_k(y_true[np.argsort(-y_pred)], np.sum(y_true>0), k=k)
+AP = lambda y_true, y_pred, u, u1 : average_precision(y_true[np.argsort(-y_pred)])
+MAP = lambda y_true, y_pred, u, u1 : mean_average_precision([y_true[np.argsort(-y_pred)]])
+DCGk = lambda y_true, y_pred, k, u1 : dcg_at_k(y_true[np.argsort(-y_pred)], k)
+NDCGk = lambda y_true, y_pred, k, u1 : ndcg_at_k(y_true[np.argsort(-y_pred)], k)
+MeanRank = lambda y_true, y_pred, k, u1 : mean_rank([y_true[np.argsort(-y_pred)]])
+HRk = lambda y_true, y_pred, k, u1 : hit_rate_at_k([y_true[np.argsort(-y_pred)]], k)
+metrics_list = ["AUC", "Fscore", "TAU", "Rscore", "MRR", "RP", "PrecisionK", "RecallK", "F1K", "AP", "MAP", "DCGk", "NDCGk", "MeanRank", "HRk", "ERR"]
+
+###################################
+## COMPUTATION OF METRICS        ##
+###################################
+
+def compute_metrics(scores, predictions, dataset, metrics, k=1, beta=1, verbose=False):
     '''
-    Computes validation metrics for a given set of scores and predictions w.r.t. a dataset
+    Computes *user-wise* validation metrics for a given set of scores and predictions w.r.t. a dataset
 
     ...
 
     Parameters
     ----------
-    scores : array-like of shape (n_ratings, 3)
-        a matrix which contains the user indices (column 1), the item indices (column 2) and the score for the corresponding (user, item) pair (float value in column 3)
-    predictions : array-like of shape (n_ratings, 3)
-        a matrix which contains the user indices (column 1), the item indices (column 2) and the class for the corresponding (user, item) pair (value in {-1, 0, 1} in column 3)
-    test_dataset : stanscofi.Dataset
-        the validation dataset on which the metrics should be computed
-    beta : float
-        a positive number for the computation of the F-beta metric
-    ignore_zeroes : bool
-        how to deal with more than two class labels; if ignore_zeroes=True, then pairs which are assigned 0 are not taken into account when computing the metric {{-1},{1}}; otherwise, zeroes are considered negative, and the validation metrics are computed {{-1,0},{1}}
+    scores : COO-array of shape (n_items, n_users)
+        sparse matrix in COOrdinate format
+    predictions : COO-array of shape (n_items, n_users)
+        sparse matrix in COOrdinate format with values in {-1,1}
+    dataset : stanscofi.Dataset
+        dataset on which the metrics should be computed
+    metrics : lst of str
+        list of metrics which should be computed
+    k : int (default: 1)
+        Argument of the metric to optimize. Implemented metrics are in validation.py
+    beta : float (default: 1)
+        Argument of the metric to optimize. Implemented metrics are in validation.py
     verbose : bool
         prints out information about ignored users for the computation of validation metrics, that is, users which pairs are only associated to a single class (i.e., all pairs with this users are either assigned 0, -1 or 1)
 
     Returns
     -------
-    metrics : pandas.DataFrame of shape (2, 2)
-        table of metrics: AUC, F_beta score in rows, average and standard deviation across users in columns
+    metrics : pandas.DataFrame of shape (len(metrics), 2)
+        table of metrics: metrics in rows, average and standard deviation across users in columns
     plots_args : dict
-        dictionary of arguments to feed to the plot_metrics function
+        dictionary of arguments to feed to the plot_metrics function to plot the Precision-Recall and the Receiver Operating Chracteristic (ROC) curves
     '''
-    assert scores.shape[1]==3
-    assert predictions.shape[1]==3
-    assert predictions.shape[0]==scores.shape[0]
-    assert beta>0
-    y_true_all = np.array([test_dataset.ratings_mat[j,i] for i,j in scores[:,:2].astype(int).tolist()])
-    y_pred_all = predictions[:,2].flatten()
-    if (test_dataset.folds is not None):
-        ids = np.argwhere(np.ones(test_dataset.ratings_mat.shape))
-        folds_ids = [((test_dataset.folds[:,0]==i)&(test_dataset.folds[:,1]==j)).any() for i,j in ids[:,:2].tolist()]
-        y_true_all = y_true_all[folds_ids]
-        y_pred_all = y_pred_all[folds_ids]
-        scores_ = scores[folds_ids,:]
-        assert y_true_all.shape[0] == test_dataset.folds.shape[0]
-        assert y_pred_all.shape[0] == test_dataset.folds.shape[0]
-    else:
-        scores_ = deepcopy(scores)
-    if (not ignore_zeroes):
-        predictions_ = deepcopy(predictions)
-        y_true = (y_true_all>0).astype(int) 
-        y_pred = (y_pred_all>0).astype(int)
-    else:
-        ids = np.argwhere(y_true_all!=0)
-        scores_ = scores[ids.flatten().tolist(),:]
-        predictions_ = predictions[ids,:]
-        y_true = (y_true_all[ids]>0).astype(int)
-        y_pred = (y_pred_all[ids]>0).astype(int)
-    assert y_true.shape[0]==y_pred.shape[0]==scores_.shape[0]
-    assert all([x in [-1,0,1] for x in np.unique(y_true).flatten()])
+    metrics_list = ["AUC", "Fscore", "TAU", "Rscore", "MRR", "RP", "PrecisionK", "RecallK", "F1K", "AP", "MAP", "DCGk", "NDCGk", "MeanRank", "HRk", "ERR"]
+    assert predictions.shape==scores.shape==dataset.folds.shape
+    assert all([metric in metrics_list for metric in metrics])
+    y_true_all = dataset.ratings.toarray()[dataset.folds.row,dataset.folds.col].ravel() 
+    y_pred_all = predictions.data.ravel()
+    scores_all = scores.data.ravel()
+    assert y_true_all.shape==y_pred_all.shape==scores_all.shape
     ## Compute average metric per user
-    user_ids = np.unique(scores_[:,0].flatten()).astype(int).tolist()
+    user_ids = np.unique(dataset.folds.col)
     n_ignored = 0
     aucs, tprs, recs, fscores = [], [], [], []
     base_fpr = np.linspace(0, 1, 101)
     base_pres = np.linspace(0, 1, 101)
+    metrics_list = {metric: [] for metric in metrics}
     for user_id in user_ids:
-        user_ids_i = np.argwhere(scores_[:,0].flatten()==user_id)
+        user_ids_i = np.argwhere(dataset.folds.col==user_id)
         if (len(user_ids_i)==0):
             n_ignored += 1
             continue
-        user_truth = y_true[user_ids_i].reshape(1, -1)
-        user_pred = y_pred[user_ids_i].reshape(1, -1)
-        if (len(np.unique(user_truth))==2):
-            fpr, tpr, _ = ROC(user_truth.flatten(), user_pred.flatten())
-            pres, rec, _ = PRC(user_truth.flatten(), user_pred.flatten())
-            aucs.append(AUC(user_truth.flatten(), user_pred.flatten()))
-            fscores.append(fbeta_score(user_truth.flatten(), user_pred.flatten(), beta=beta))
+        user_truth = y_true_all[user_ids_i]
+        user_pred = y_pred_all[user_ids_i]
+        if ((len(np.unique(user_truth))==2) and (1 in user_truth)):
+            fpr, tpr, _ = ROC(user_truth, user_pred, pos_label=1.)
+            pres, rec, _ = PRC(user_truth, user_pred)
+            aucs.append(roc_auc_score(user_truth, user_pred, average="weighted"))
+            fscores.append(fbeta_score(user_truth, user_pred, beta=beta, average="weighted"))
             tpr = np.interp(base_fpr, fpr, tpr)
             tpr[0] = 0.0
             tprs.append(tpr)
             rec = np.interp(base_pres, pres, rec)
             recs.append(rec)
+            for metric in metrics:
+                #print(metric)
+                value = eval(metric)(user_truth.ravel(), user_pred.ravel(), k, beta)
+                metrics_list.update({metric: metrics_list[metric]+[value]})
         else:
             n_ignored += 1
     if (verbose and n_ignored>0):
         print("<validation.compute_metrics> Computed on #users=%d, %d ignored (%2.f perc)" % (len(user_ids), n_ignored, 100*n_ignored/len(user_ids)))
     if (len(aucs)==0 or len(fscores)==0):
-        metrics = pd.DataFrame([], index=["AUC", "F_%.1f" % beta], 
-		columns=["Avg. across users", "Std"])
+        metrics = pd.DataFrame([], index=metrics, 
+		columns=["Average", "StandardDeviation"])
         return metrics, {}
-    metrics = pd.DataFrame([[f(x) for f in [np.mean, np.std]] for x in [aucs, fscores]], index=["AUC", "F_%.1f" % beta], 
-		columns=["Avg. across users", "Std"])
-    return metrics, {"y_true": y_true, "y_pred": y_pred, "scores": scores_[:,2].flatten(), "predictions": y_pred_all, "ground_truth": y_true_all, "aucs": aucs, "fscores": fscores, "tprs": np.array(tprs), "recs": np.array(recs)}
+    metrics = pd.DataFrame([[f(metrics_list[m]) for f in [np.mean, np.std]] for m in metrics_list], index=metrics, columns=["Average", "StandardDeviation"])
+    metrics = pd.concat((metrics, pd.DataFrame([[k,beta]], index=["arguments (k, beta)"], columns=metrics.columns)), axis=0)
+    return metrics, {"y_true": (y_true_all>0).astype(int), "y_pred": (y_pred_all>0).astype(int), "scores": scores_all, "predictions": y_pred_all, "ground_truth": y_true_all, "aucs": aucs, "fscores": fscores, "tprs": np.array(tprs), "recs": np.array(recs)}
+
+###################################
+## PLOTS                         ##
+###################################
 
 def plot_metrics(y_true=None, y_pred=None, scores=None, ground_truth=None, predictions=None, aucs=None, fscores=None, tprs=None, recs=None, figsize=(16,5), model_name="Model"):
     '''
     Plots the ROC curve, the Precision-Recall curve, the boxplot of predicted scores and the piechart of classes associated to the predictions y_pred in input w.r.t. ground truth y_true
 
     ...
```

### Comparing `stanscofi-1.1.0/src/stanscofi.egg-info/PKG-INFO` & `stanscofi-2.0.0/src/stanscofi.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stanscofi
-Version: 1.1.0
+Version: 2.0.0
 Summary: Package for STANdard drug Screening by COllaborative FIltering. Performs benchmarks against datasets and SotA algorithms, and implements training, validation and testing procedures.
 Home-page: https://github.com/RECeSS-EU-Project/stanscofi
 Author: Clémence Réda
 Author-email: recess-project@proton.me
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -14,15 +14,15 @@
 
 ![funding logo](https://raw.githubusercontent.com/RECeSS-EU-Project/RECeSS-EU-Project.github.io/main/assets/images/header%2BEU_rescale.jpg)
 
 # STANdard for drug Screening by COllaborative FIltering (stanscofi) Python Package
 
 This repository is a part of the EU-funded [RECeSS project](https://recess-eu-project.github.io) (#101102016), and hosts the code for the open-source Python package *stanscofi* for the development of collaborative filtering-based drug repurposing algorithms.
 
-[![Python Version](https://img.shields.io/badge/python-3.8%7C3.9%7C3.10-pink)](https://badge.fury.io/py/stanscofi) [![PyPI version](https://img.shields.io/pypi/v/stanscofi.svg)](https://badge.fury.io/py/stanscofi) [![Anaconda version](https://anaconda.org/recess/stanscofi/badges/version.svg)](https://anaconda.org/recess/stanscofi) [![Zenodo version](https://zenodo.org/badge/DOI/10.5281/zenodo.8038847.svg)](https://doi.org/10.5281/zenodo.8038847) ![GitHub](https://img.shields.io/github/license/recess-eu-project/stanscofi.svg) [![Build Status](https://github.com/recess-eu-project/stanscofi/actions/workflows/post-push-test.yml/badge.svg)](https://github.com/recess-eu-project/stanscofi/actions/workflows/post-push-test.yml) [![Codecov](https://codecov.io/github/recess-eu-project/stanscofi/coverage.svg?branch=master)](https://codecov.io/github/recess-eu-project/stanscofi?branch=master) [![Codefactor](https://www.codefactor.io/repository/github/recess-eu-project/stanscofi/badge?style=plastic)](https://www.codefactor.io/repository/github/recess-eu-project/stanscofi)
+[![Python Version](https://img.shields.io/badge/python-3.8%7C3.9-pink)](https://badge.fury.io/py/stanscofi) [![PyPI version](https://img.shields.io/pypi/v/stanscofi.svg)](https://badge.fury.io/py/stanscofi) [![Anaconda version](https://anaconda.org/recess/stanscofi/badges/version.svg)](https://anaconda.org/recess/stanscofi) [![Zenodo version](https://zenodo.org/badge/DOI/10.5281/zenodo.8038847.svg)](https://doi.org/10.5281/zenodo.8038847) ![GitHub](https://img.shields.io/github/license/recess-eu-project/stanscofi.svg) [![Build Status](https://github.com/recess-eu-project/stanscofi/actions/workflows/post-push-test.yml/badge.svg)](https://github.com/recess-eu-project/stanscofi/actions/workflows/post-push-test.yml) [![Codecov](https://codecov.io/github/recess-eu-project/stanscofi/coverage.svg?branch=master)](https://codecov.io/github/recess-eu-project/stanscofi?branch=master) [![Codefactor](https://www.codefactor.io/repository/github/recess-eu-project/stanscofi/badge?style=plastic)](https://www.codefactor.io/repository/github/recess-eu-project/stanscofi)
 
 ## Statement of need 
 
 As of 2022, current drug development pipelines last around 10 years, costing $2billion in average, while drug commercialization failure rates go up to 90%. These issues can be mitigated by drug repurposing, where chemical compounds are screened for new therapeutic indications in a systematic fashion. In prior works, this approach has been implemented through collaborative filtering. This semi-supervised learning framework leverages known drug-disease matchings in order to recommend new ones.
 
 The **stanscofi** package comprises method-agnostic training, validation, preprocessing and visualization procedures on several published drug repurposing datasets. The proper implementation of these steps is crucial in order to avoid data leakage, *i*.*e*., the model is learnt over information that should be unavailable at prediction time. Indeed, data leakage is the source of a major reproducibility crisis in machine learning. This will be avoided by building training and validation sets which are weakly correlated with respect to the drug and disease feature vectors. The main performance metric will be the area under the curve (AUC), which estimates the diagnostic ability of a recommender system better than accuracy in imbalanced datasets.
 
@@ -50,15 +50,15 @@
 
 Once installed, to import **stanscofi** into your Python code
 
 ```
 import stanscofi
 ```
 
-Please check out notebook *Introduction to stanscofi.ipynb*. All functions are documented, so one can check out the inputs and outputs of a function func by typing
+Please check out notebook *Introduction to stanscofi.ipynb*. Documentation about **stanscofi** can be found at [this page](https://recess-eu-project.github.io/stanscofi/). All functions are documented, so one can check out the inputs and outputs of a function func by typing
 
 ```
 help(func)
 ```
 
 To mesure your environmental impact when using this package (in terms of carbon emissions), please run the following command
```

