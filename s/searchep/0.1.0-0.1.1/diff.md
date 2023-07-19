# Comparing `tmp/searchep-0.1.0.tar.gz` & `tmp/searchep-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "searchep-0.1.0.tar", max compression
+gzip compressed data, was "searchep-0.1.1.tar", max compression
```

## Comparing `searchep-0.1.0.tar` & `searchep-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1078 2023-07-19 13:45:44.388586 searchep-0.1.0/LICENSE
--rw-r--r--   0        0        0      150 2023-06-14 11:34:33.019430 searchep-0.1.0/README.md
--rw-r--r--   0        0        0      904 2023-07-19 14:26:20.538720 searchep-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4233 2023-05-16 10:21:16.199866 searchep-0.1.0/searchep/GPFlow_model_class.py
--rw-r--r--   0        0        0      309 2023-05-16 10:21:16.199866 searchep-0.1.0/searchep/__init__.py
--rw-r--r--   0        0        0    33087 2023-07-05 10:41:08.706740 searchep-0.1.0/searchep/data.py
--rw-r--r--   0        0        0     3710 2023-06-21 08:48:52.165571 searchep-0.1.0/searchep/eval.py
--rw-r--r--   0        0        0     7754 2023-06-20 15:39:01.782165 searchep-0.1.0/searchep/gpr.py
--rw-r--r--   0        0        0     5147 2023-05-16 10:21:16.199866 searchep-0.1.0/searchep/main.py
--rw-r--r--   0        0        0     5526 2023-05-16 10:21:16.199866 searchep-0.1.0/searchep/matrix.py
--rw-r--r--   0        0        0    26230 2023-05-16 10:21:16.199866 searchep-0.1.0/searchep/plots.py
--rw-r--r--   0        0        0    19605 2023-05-16 10:21:16.203867 searchep-0.1.0/searchep/tests.py
--rw-r--r--   0        0        0     3757 2023-06-21 08:46:25.168869 searchep-0.1.0/searchep/training.py
--rw-r--r--   0        0        0      500 2023-05-16 10:21:16.203867 searchep-0.1.0/searchep/zero_search.py
--rw-r--r--   0        0        0     1310 1970-01-01 00:00:00.000000 searchep-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-07-19 13:45:44.388586 searchep-0.1.1/LICENSE
+-rw-r--r--   0        0        0      243 2023-07-19 15:13:38.676404 searchep-0.1.1/README.md
+-rw-r--r--   0        0        0      926 2023-07-19 15:26:09.499709 searchep-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4233 2023-05-16 10:21:16.199866 searchep-0.1.1/searchep/GPFlow_model_class.py
+-rw-r--r--   0        0        0      309 2023-05-16 10:21:16.199866 searchep-0.1.1/searchep/__init__.py
+-rw-r--r--   0        0        0    33087 2023-07-05 10:41:08.706740 searchep-0.1.1/searchep/data.py
+-rw-r--r--   0        0        0     3710 2023-06-21 08:48:52.165571 searchep-0.1.1/searchep/eval.py
+-rw-r--r--   0        0        0     7754 2023-06-20 15:39:01.782165 searchep-0.1.1/searchep/gpr.py
+-rw-r--r--   0        0        0     5147 2023-05-16 10:21:16.199866 searchep-0.1.1/searchep/main.py
+-rw-r--r--   0        0        0     5526 2023-05-16 10:21:16.199866 searchep-0.1.1/searchep/matrix.py
+-rw-r--r--   0        0        0    26230 2023-05-16 10:21:16.199866 searchep-0.1.1/searchep/plots.py
+-rw-r--r--   0        0        0    19605 2023-05-16 10:21:16.203867 searchep-0.1.1/searchep/tests.py
+-rw-r--r--   0        0        0     3757 2023-06-21 08:46:25.168869 searchep-0.1.1/searchep/training.py
+-rw-r--r--   0        0        0      500 2023-05-16 10:21:16.203867 searchep-0.1.1/searchep/zero_search.py
+-rw-r--r--   0        0        0     1403 1970-01-01 00:00:00.000000 searchep-0.1.1/PKG-INFO
```

### Comparing `searchep-0.1.0/LICENSE` & `searchep-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `searchep-0.1.0/pyproject.toml` & `searchep-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "searchep"
-version = "0.1.0"
+version = "0.1.1"
 description = "A module to search for exceptional points"
 authors = ["Patrick Egenlauf <patrick.egenlauf+searchep@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://search-for-eps.github.io/Search-for-EPs/"
 repository = "https://github.com/Search-for-EPs/Search-for-EPs"
 documentation = "https://search-for-eps.github.io/Search-for-EPs/"
 keywords = ["searchep", "EP", "search for EPs", "exceptional points", "stepwise grouping algorithm"]
 
 [tool.poetry.dependencies]
 python = ">= 3.9.2, < 3.11"
-jax = {extras = ["cpu"], version = "^0.3.13"}
-jaxlib = "^0.3.10"
+jax = {extras = ["cpu"], version = ">= 0.3.13, < 1.0.0"}
+jaxlib = ">= 0.3.10, < 1.0.0"
 numpy = "^1.21.6"
 gpflow = "^2.5.2"
 pandas = "^1.3.5"
 plotly = "^5.8.0"
 scipy = "^1.7.3"
 matplotlib = "^3.5.2"
 setuptools = ">= 52.0.0"
```

### Comparing `searchep-0.1.0/searchep/GPFlow_model_class.py` & `searchep-0.1.1/searchep/GPFlow_model_class.py`

 * *Files identical despite different names*

### Comparing `searchep-0.1.0/searchep/data.py` & `searchep-0.1.1/searchep/data.py`

 * *Files identical despite different names*

### Comparing `searchep-0.1.0/searchep/eval.py` & `searchep-0.1.1/searchep/eval.py`

 * *Files identical despite different names*

### Comparing `searchep-0.1.0/searchep/gpr.py` & `searchep-0.1.1/searchep/gpr.py`

 * *Files identical despite different names*

### Comparing `searchep-0.1.0/searchep/main.py` & `searchep-0.1.1/searchep/main.py`

 * *Files identical despite different names*

### Comparing `searchep-0.1.0/searchep/matrix.py` & `searchep-0.1.1/searchep/matrix.py`

 * *Files identical despite different names*

### Comparing `searchep-0.1.0/searchep/plots.py` & `searchep-0.1.1/searchep/plots.py`

 * *Files identical despite different names*

### Comparing `searchep-0.1.0/searchep/tests.py` & `searchep-0.1.1/searchep/tests.py`

 * *Files identical despite different names*

### Comparing `searchep-0.1.0/searchep/training.py` & `searchep-0.1.1/searchep/training.py`

 * *Files identical despite different names*

### Comparing `searchep-0.1.0/PKG-INFO` & `searchep-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: searchep
-Version: 0.1.0
+Version: 0.1.1
 Summary: A module to search for exceptional points
 Home-page: https://search-for-eps.github.io/Search-for-EPs/
 License: MIT
 Keywords: searchep,EP,search for EPs,exceptional points,stepwise grouping algorithm
 Author: Patrick Egenlauf
 Author-email: patrick.egenlauf+searchep@gmail.com
 Requires-Python: >=3.9.2,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: gpflow (>=2.5.2,<3.0.0)
-Requires-Dist: jax[cpu] (>=0.3.13,<0.4.0)
-Requires-Dist: jaxlib (>=0.3.10,<0.4.0)
+Requires-Dist: jax[cpu] (>=0.3.13,<1.0.0)
+Requires-Dist: jaxlib (>=0.3.10,<1.0.0)
 Requires-Dist: matplotlib (>=3.5.2,<4.0.0)
 Requires-Dist: numpy (>=1.21.6,<2.0.0)
 Requires-Dist: pandas (>=1.3.5,<2.0.0)
 Requires-Dist: plotly (>=5.8.0,<6.0.0)
 Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: scipy (>=1.7.3,<2.0.0)
 Requires-Dist: setuptools (>=52.0.0)
@@ -25,11 +25,18 @@
 Project-URL: Documentation, https://search-for-eps.github.io/Search-for-EPs/
 Project-URL: Repository, https://github.com/Search-for-EPs/Search-for-EPs
 Description-Content-Type: text/markdown
 
 # Search-for-EPs
 
 
+### Installation
+
+You can install this package via `pip`.   
+
+    pip install searchep    
+
+
 ### Documentation
 
 The [documentation](https://search-for-eps.github.io/Search-for-EPs/) contains more details about this package.
```

