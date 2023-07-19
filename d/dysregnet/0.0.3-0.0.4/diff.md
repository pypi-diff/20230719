# Comparing `tmp/dysregnet-0.0.3.tar.gz` & `tmp/dysregnet-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dysregnet-0.0.3.tar", last modified: Tue May 17 16:17:13 2022, max compression
+gzip compressed data, was "dysregnet-0.0.4.tar", last modified: Wed Jul 19 14:03:46 2023, max compression
```

## Comparing `dysregnet-0.0.3.tar` & `dysregnet-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 16:17:13.573511 dysregnet-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-05-17 16:16:59.000000 dysregnet-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5616 2022-05-17 16:17:13.573511 dysregnet-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4947 2022-05-17 16:16:59.000000 dysregnet-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 16:17:13.573511 dysregnet-0.0.3/dysregnet/
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-05-17 16:16:59.000000 dysregnet-0.0.3/dysregnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6705 2022-05-17 16:16:59.000000 dysregnet-0.0.3/dysregnet/dysregnet.py
--rw-r--r--   0 runner    (1001) docker     (121)     5931 2022-05-17 16:16:59.000000 dysregnet-0.0.3/dysregnet/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 16:17:13.573511 dysregnet-0.0.3/dysregnet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5616 2022-05-17 16:17:13.000000 dysregnet-0.0.3/dysregnet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      258 2022-05-17 16:17:13.000000 dysregnet-0.0.3/dysregnet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-17 16:17:13.000000 dysregnet-0.0.3/dysregnet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-05-17 16:17:13.000000 dysregnet-0.0.3/dysregnet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-05-17 16:17:13.000000 dysregnet-0.0.3/dysregnet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-17 16:17:13.573511 dysregnet-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1183 2022-05-17 16:16:59.000000 dysregnet-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:03:46.704052 dysregnet-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-19 14:03:34.000000 dysregnet-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-07-19 14:03:46.704052 dysregnet-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-07-19 14:03:34.000000 dysregnet-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 14:03:46.704052 dysregnet-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-19 14:03:34.000000 dysregnet-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:03:46.704052 dysregnet-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:03:46.704052 dysregnet-0.0.4/src/dysregnet/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-19 14:03:34.000000 dysregnet-0.0.4/src/dysregnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6741 2023-07-19 14:03:34.000000 dysregnet-0.0.4/src/dysregnet/dysregnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-07-19 14:03:34.000000 dysregnet-0.0.4/src/dysregnet/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:03:46.704052 dysregnet-0.0.4/src/dysregnet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-07-19 14:03:46.000000 dysregnet-0.0.4/src/dysregnet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-19 14:03:46.000000 dysregnet-0.0.4/src/dysregnet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 14:03:46.000000 dysregnet-0.0.4/src/dysregnet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-19 14:03:46.000000 dysregnet-0.0.4/src/dysregnet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-19 14:03:46.000000 dysregnet-0.0.4/src/dysregnet.egg-info/top_level.txt
```

### Comparing `dysregnet-0.0.3/LICENSE` & `dysregnet-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dysregnet-0.0.3/PKG-INFO` & `dysregnet-0.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,8 @@
-Metadata-Version: 2.1
-Name: dysregnet
-Version: 0.0.3
-Summary: DysRegNet
-Home-page: https://github.com/biomedbigdata/DysRegNet_package
-Author: Zakaria Louadi, olga lazareva
-Author-email: zakaria.louadi@tum.de, olga.lazareva@tum.de
-License: GPLv3
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
+[![PyPI version](https://badge.fury.io/py/dysregnet.svg)](https://badge.fury.io/py/dysregnet)
 
 # DysRegNet package
 
 
 DysRegNet, is a  method for inferring patient-specific regulatory alterations (dysregulations) from gene expression profiles. DysRegNet uses linear models to account for confounders and residual-derived z-scores to assess significance.
 
 
@@ -75,15 +59,15 @@
 
 - normaltest: Boolean. If True, Run a normality test for residuals "scipy.stats.normaltest". If residuals are not normal, the edge will not be considered in the analysis. 
 
 - normaltest_alpha: p-value threshold for normaltest (if True).
 
 - R2_threshold: R-squared (R2) threshold from 0 to 1 (optional).  If the fit is weaker, the edge will not be considered in the analysis. 
 
-- direction_condition: Boolean. If True: only include dysregulation that are relevalant for the interactions (down regulation of an activation or up regulation of a supressions). Please check the paper for more details.
+- direction_condition: Boolean. If True: only include dysregulation that are relevant for the interactions (down regulation of an activation or up regulation of a supressions). Please check the paper for more details.
 
 
 ## Get Started
 
 
 Please note, that the functions are annotated with dockstrings for more details.
 
@@ -128,14 +112,17 @@
 # results table
 data.get_results()
 
 # or a binary result
 
 data.get_results_binary()
 
+# get R2 values, coefficients, and coefficient p-values for all models/edges
+data.get_model_stats()
+
 ```
 
 The expected run time for the installation and running the demo dataset on a "normal" desktop computer is around 3~5 minutes.
 
 
 
 ## The output
@@ -149,17 +136,17 @@
 
 ## Example
 
 A simple example for running DysRegNet:
 ([Notebook](https://github.com/biomedbigdata/DysRegNet_package/blob/main/test.ipynb)/[Google Colab](https://colab.research.google.com/github/biomedbigdata/DysRegNet_package/blob/main/test.ipynb)).
 
 
-If you want to eun the exact demo. You will need to download the demo dataset and extract the files into test dataset/
+You will need to download the demo dataset and extract the files into test dataset/
 
-Link: https://figshare.com/ndownloader/files/35142652
+Link for the demo dataset: https://figshare.com/ndownloader/files/35142652
 
 
 
 ## Cite
 
 "DysRegNet: Patient-specific and confounder-aware dysregulated network inference"
 Olga Lazareva*, Zakaria Louadi*, Johannes Kersting, Jan Baumbach, David B. Blumenthal, Markus List. bioRxiv 2022.04.29.490015; doi: https://doi.org/10.1101/2022.04.29.490015. * equal first-authors
```

### Comparing `dysregnet-0.0.3/README.md` & `dysregnet-0.0.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+Metadata-Version: 2.1
+Name: dysregnet
+Version: 0.0.4
+Summary: DysRegNet
+Home-page: https://github.com/biomedbigdata/DysRegNet_package
+Author: Zakaria Louadi, Olga Lazareva, Johannes Kersting
+Author-email: zakaria.louadi@tum.de, olga.lazareva@tum.de, johannes.kersting@tum.de
+License: GPLv3
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![PyPI version](https://badge.fury.io/py/dysregnet.svg)](https://badge.fury.io/py/dysregnet)
+
 # DysRegNet package
 
 
 DysRegNet, is a  method for inferring patient-specific regulatory alterations (dysregulations) from gene expression profiles. DysRegNet uses linear models to account for confounders and residual-derived z-scores to assess significance.
 
 
 ## Installation
@@ -57,15 +77,15 @@
 
 - normaltest: Boolean. If True, Run a normality test for residuals "scipy.stats.normaltest". If residuals are not normal, the edge will not be considered in the analysis. 
 
 - normaltest_alpha: p-value threshold for normaltest (if True).
 
 - R2_threshold: R-squared (R2) threshold from 0 to 1 (optional).  If the fit is weaker, the edge will not be considered in the analysis. 
 
-- direction_condition: Boolean. If True: only include dysregulation that are relevalant for the interactions (down regulation of an activation or up regulation of a supressions). Please check the paper for more details.
+- direction_condition: Boolean. If True: only include dysregulation that are relevant for the interactions (down regulation of an activation or up regulation of a supressions). Please check the paper for more details.
 
 
 ## Get Started
 
 
 Please note, that the functions are annotated with dockstrings for more details.
 
@@ -110,14 +130,17 @@
 # results table
 data.get_results()
 
 # or a binary result
 
 data.get_results_binary()
 
+# get R2 values, coefficients, and coefficient p-values for all models/edges
+data.get_model_stats()
+
 ```
 
 The expected run time for the installation and running the demo dataset on a "normal" desktop computer is around 3~5 minutes.
 
 
 
 ## The output
@@ -131,17 +154,17 @@
 
 ## Example
 
 A simple example for running DysRegNet:
 ([Notebook](https://github.com/biomedbigdata/DysRegNet_package/blob/main/test.ipynb)/[Google Colab](https://colab.research.google.com/github/biomedbigdata/DysRegNet_package/blob/main/test.ipynb)).
 
 
-If you want to eun the exact demo. You will need to download the demo dataset and extract the files into test dataset/
+You will need to download the demo dataset and extract the files into test dataset/
 
-Link: https://figshare.com/ndownloader/files/35142652
+Link for the demo dataset: https://figshare.com/ndownloader/files/35142652
 
 
 
 ## Cite
 
 "DysRegNet: Patient-specific and confounder-aware dysregulated network inference"
 Olga Lazareva*, Zakaria Louadi*, Johannes Kersting, Jan Baumbach, David B. Blumenthal, Markus List. bioRxiv 2022.04.29.490015; doi: https://doi.org/10.1101/2022.04.29.490015. * equal first-authors
```

### Comparing `dysregnet-0.0.3/dysregnet/dysregnet.py` & `dysregnet-0.0.4/src/dysregnet/dysregnet.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,15 +53,15 @@
                     CatCov: List of strings.
                             List of categorical variable names. They should match the name of their columns in meta Dataframe.
 
                     ConCov: List of strings.
                             List of continuous covariates. They should match the name of their columns in meta Dataframe.
 
 
-                    zscoring: boolean, default: True 
+                    zscoring: boolean, default: False 
                          zscoring of expression data (if needed).
 
                     bonferroni_alpha: Float
                             P value threshold for multiple testing correction
 
                     normaltest: Bool
                             If True. Run a normality test for residuals "scipy.stats.normaltest". If residuals are not normal, the edge will not be considered in the analysis. 
@@ -134,32 +134,35 @@
                     self.GRN=GRN[GRN.iloc[:,0].isin(GRN_genes) ]
                     self.GRN=self.GRN[ self.GRN.iloc[:,1].isin(GRN_genes) ].drop_duplicates()
 
 
                     self.cov_df,self.expr, self.control, self.case = functions.process_data(self)
 
 
-                    self.results=functions.dyregnet_model(self)
+                    self.results, self.model_stats = functions.dyregnet_model(self)
                 
 
                 
                 
         def get_results(self):
             return  self.results
 
         
         
         
         def get_results_binary(self):
                 res_binary=self.results.copy()
-                res_binary=res_binary.set_index('patient id')
                 res_binary = res_binary.where(res_binary==0, other=1)
                 
                 return res_binary
 
+    
+        def get_model_stats(self):
+            return self.model_stats
+
```

### Comparing `dysregnet-0.0.3/dysregnet.egg-info/PKG-INFO` & `dysregnet-0.0.4/src/dysregnet.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: dysregnet
-Version: 0.0.3
+Version: 0.0.4
 Summary: DysRegNet
 Home-page: https://github.com/biomedbigdata/DysRegNet_package
-Author: Zakaria Louadi, olga lazareva
-Author-email: zakaria.louadi@tum.de, olga.lazareva@tum.de
+Author: Zakaria Louadi, Olga Lazareva, Johannes Kersting
+Author-email: zakaria.louadi@tum.de, olga.lazareva@tum.de, johannes.kersting@tum.de
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![PyPI version](https://badge.fury.io/py/dysregnet.svg)](https://badge.fury.io/py/dysregnet)
+
 # DysRegNet package
 
 
 DysRegNet, is a  method for inferring patient-specific regulatory alterations (dysregulations) from gene expression profiles. DysRegNet uses linear models to account for confounders and residual-derived z-scores to assess significance.
 
 
 ## Installation
@@ -75,15 +77,15 @@
 
 - normaltest: Boolean. If True, Run a normality test for residuals "scipy.stats.normaltest". If residuals are not normal, the edge will not be considered in the analysis. 
 
 - normaltest_alpha: p-value threshold for normaltest (if True).
 
 - R2_threshold: R-squared (R2) threshold from 0 to 1 (optional).  If the fit is weaker, the edge will not be considered in the analysis. 
 
-- direction_condition: Boolean. If True: only include dysregulation that are relevalant for the interactions (down regulation of an activation or up regulation of a supressions). Please check the paper for more details.
+- direction_condition: Boolean. If True: only include dysregulation that are relevant for the interactions (down regulation of an activation or up regulation of a supressions). Please check the paper for more details.
 
 
 ## Get Started
 
 
 Please note, that the functions are annotated with dockstrings for more details.
 
@@ -128,14 +130,17 @@
 # results table
 data.get_results()
 
 # or a binary result
 
 data.get_results_binary()
 
+# get R2 values, coefficients, and coefficient p-values for all models/edges
+data.get_model_stats()
+
 ```
 
 The expected run time for the installation and running the demo dataset on a "normal" desktop computer is around 3~5 minutes.
 
 
 
 ## The output
@@ -149,17 +154,17 @@
 
 ## Example
 
 A simple example for running DysRegNet:
 ([Notebook](https://github.com/biomedbigdata/DysRegNet_package/blob/main/test.ipynb)/[Google Colab](https://colab.research.google.com/github/biomedbigdata/DysRegNet_package/blob/main/test.ipynb)).
 
 
-If you want to eun the exact demo. You will need to download the demo dataset and extract the files into test dataset/
+You will need to download the demo dataset and extract the files into test dataset/
 
-Link: https://figshare.com/ndownloader/files/35142652
+Link for the demo dataset: https://figshare.com/ndownloader/files/35142652
 
 
 
 ## Cite
 
 "DysRegNet: Patient-specific and confounder-aware dysregulated network inference"
 Olga Lazareva*, Zakaria Louadi*, Johannes Kersting, Jan Baumbach, David B. Blumenthal, Markus List. bioRxiv 2022.04.29.490015; doi: https://doi.org/10.1101/2022.04.29.490015. * equal first-authors
```

### Comparing `dysregnet-0.0.3/setup.py` & `dysregnet-0.0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,37 +7,38 @@
 
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 
 setup(name='dysregnet',
-      version='0.0.3',
+      version='0.0.4',
       description='DysRegNet',
       long_description=README,
       long_description_content_type="text/markdown",
       url='https://github.com/biomedbigdata/DysRegNet_package',
-      author='Zakaria Louadi, olga lazareva',
-      author_email='zakaria.louadi@tum.de, olga.lazareva@tum.de',
+      author='Zakaria Louadi, Olga Lazareva, Johannes Kersting',
+      author_email='zakaria.louadi@tum.de, olga.lazareva@tum.de, johannes.kersting@tum.de',
       license='GPLv3',
       classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
       ],
-      packages=find_packages(),
+      package_dir = {'': 'src'},
+      packages=['dysregnet'],
       include_package_data=True,
       python_requires='>=3.7',
       install_requires=[
         'pandas',
         'numpy>= 1.19',
         'scipy',
         'statsmodels',
         'tqdm',
-        'sklearn', 
+        'scikit-learn', 
 
     ],
 
 )
```

