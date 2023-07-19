# Comparing `tmp/bnlearn-0.8.0.tar.gz` & `tmp/bnlearn-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bnlearn-0.8.0.tar", last modified: Wed May 17 11:02:38 2023, max compression
+gzip compressed data, was "bnlearn-0.8.1.tar", last modified: Wed Jul 19 07:12:08 2023, max compression
```

## Comparing `bnlearn-0.8.0.tar` & `bnlearn-0.8.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 11:02:38.010879 bnlearn-0.8.0/
--rw-rw-rw-   0        0        0     1231 2022-05-09 18:05:29.000000 bnlearn-0.8.0/LICENSE
--rw-rw-rw-   0        0        0      643 2022-05-09 18:05:29.000000 bnlearn-0.8.0/MANIFEST.in
--rw-rw-rw-   0        0        0    12268 2023-05-17 11:02:37.996634 bnlearn-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0    11621 2023-03-27 17:45:39.000000 bnlearn-0.8.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 11:02:37.870445 bnlearn-0.8.0/bnlearn/
--rw-rw-rw-   0        0        0     4477 2023-05-17 11:01:32.000000 bnlearn-0.8.0/bnlearn/__init__.py
--rw-rw-rw-   0        0        0    69616 2023-05-17 11:00:22.000000 bnlearn-0.8.0/bnlearn/bnlearn.py
--rw-rw-rw-   0        0        0     1745 2022-05-09 18:05:29.000000 bnlearn-0.8.0/bnlearn/confmatrix.py
-drwxrwxrwx   0        0        0        0 2023-05-17 11:02:37.928915 bnlearn-0.8.0/bnlearn/data/
--rw-rw-rw-   0        0        0        0 2022-05-09 18:05:29.000000 bnlearn-0.8.0/bnlearn/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 11:02:37.948190 bnlearn-0.8.0/bnlearn/discretize/
--rw-rw-rw-   0        0        0        0 2023-04-29 10:59:05.000000 bnlearn-0.8.0/bnlearn/discretize/__init__.py
--rw-rw-rw-   0        0        0     3410 2023-05-16 18:28:43.000000 bnlearn-0.8.0/bnlearn/discretize/discretize.py
--rw-rw-rw-   0        0        0    19168 2023-05-16 18:32:33.000000 bnlearn-0.8.0/bnlearn/discretize/learn_discrete_bayes_net.py
--rw-rw-rw-   0        0        0    45280 2023-05-16 21:41:39.000000 bnlearn-0.8.0/bnlearn/examples.py
--rw-rw-rw-   0        0        0     1330 2023-05-12 07:28:50.000000 bnlearn-0.8.0/bnlearn/examples_discretize.py
--rw-rw-rw-   0        0        0     3555 2023-04-01 15:11:24.000000 bnlearn-0.8.0/bnlearn/inference.py
--rw-rw-rw-   0        0        0    16904 2023-04-01 12:44:53.000000 bnlearn-0.8.0/bnlearn/network.py
--rw-rw-rw-   0        0        0     7419 2023-04-29 10:55:11.000000 bnlearn-0.8.0/bnlearn/parameter_learning.py
--rw-rw-rw-   0        0        0    25079 2023-05-09 15:43:00.000000 bnlearn-0.8.0/bnlearn/structure_learning.py
-drwxrwxrwx   0        0        0        0 2023-05-17 11:02:37.953589 bnlearn-0.8.0/bnlearn/tests/
--rw-rw-rw-   0        0        0        0 2022-11-30 17:18:09.000000 bnlearn-0.8.0/bnlearn/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 11:02:37.995637 bnlearn-0.8.0/bnlearn/tests/discretize/
--rw-rw-rw-   0        0        0        0 2023-04-29 10:59:05.000000 bnlearn-0.8.0/bnlearn/tests/discretize/__init__.py
--rw-rw-rw-   0        0        0     2293 2023-04-29 10:59:05.000000 bnlearn-0.8.0/bnlearn/tests/discretize/test_discretize.py
--rw-rw-rw-   0        0        0     9366 2023-05-12 07:28:13.000000 bnlearn-0.8.0/bnlearn/tests/discretize/test_learn_discrete_bayes_net.py
--rw-rw-rw-   0        0        0    13506 2023-05-14 19:03:35.000000 bnlearn-0.8.0/bnlearn/tests/test_bnlearn.py
--rw-rw-rw-   0        0        0     8222 2022-11-30 17:18:09.000000 bnlearn-0.8.0/bnlearn/tests/test_structure_learning.py
-drwxrwxrwx   0        0        0        0 2023-05-17 11:02:37.926635 bnlearn-0.8.0/bnlearn.egg-info/
--rw-rw-rw-   0        0        0    12268 2023-05-17 11:02:37.000000 bnlearn-0.8.0/bnlearn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      776 2023-05-17 11:02:37.000000 bnlearn-0.8.0/bnlearn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 11:02:37.000000 bnlearn-0.8.0/bnlearn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      204 2023-05-17 11:02:37.000000 bnlearn-0.8.0/bnlearn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-17 11:02:37.000000 bnlearn-0.8.0/bnlearn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 11:02:38.011879 bnlearn-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0     2071 2023-05-16 15:14:21.000000 bnlearn-0.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 07:12:08.141652 bnlearn-0.8.1/
+-rw-rw-rw-   0        0        0     1231 2022-05-09 18:05:29.000000 bnlearn-0.8.1/LICENSE
+-rw-rw-rw-   0        0        0      643 2022-05-09 18:05:29.000000 bnlearn-0.8.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    12276 2023-07-19 07:12:08.139623 bnlearn-0.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0    11670 2023-06-13 21:59:12.000000 bnlearn-0.8.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-19 07:12:08.071832 bnlearn-0.8.1/bnlearn/
+-rw-rw-rw-   0        0        0     4477 2023-07-19 07:11:51.000000 bnlearn-0.8.1/bnlearn/__init__.py
+-rw-rw-rw-   0        0        0    70897 2023-07-19 07:08:39.000000 bnlearn-0.8.1/bnlearn/bnlearn.py
+-rw-rw-rw-   0        0        0     1745 2022-05-09 18:05:29.000000 bnlearn-0.8.1/bnlearn/confmatrix.py
+drwxrwxrwx   0        0        0        0 2023-07-19 07:12:08.112021 bnlearn-0.8.1/bnlearn/data/
+-rw-rw-rw-   0        0        0        0 2022-05-09 18:05:29.000000 bnlearn-0.8.1/bnlearn/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 07:12:08.116680 bnlearn-0.8.1/bnlearn/discretize/
+-rw-rw-rw-   0        0        0        0 2023-04-29 10:59:05.000000 bnlearn-0.8.1/bnlearn/discretize/__init__.py
+-rw-rw-rw-   0        0        0     3837 2023-06-13 20:28:20.000000 bnlearn-0.8.1/bnlearn/discretize/discretize.py
+-rw-rw-rw-   0        0        0    19168 2023-05-16 18:32:33.000000 bnlearn-0.8.1/bnlearn/discretize/learn_discrete_bayes_net.py
+-rw-rw-rw-   0        0        0    45300 2023-06-12 07:48:11.000000 bnlearn-0.8.1/bnlearn/examples.py
+-rw-rw-rw-   0        0        0     1330 2023-05-12 07:28:50.000000 bnlearn-0.8.1/bnlearn/examples_discretize.py
+-rw-rw-rw-   0        0        0     4847 2023-06-13 21:56:47.000000 bnlearn-0.8.1/bnlearn/inference.py
+-rw-rw-rw-   0        0        0    16904 2023-04-01 12:44:53.000000 bnlearn-0.8.1/bnlearn/network.py
+-rw-rw-rw-   0        0        0     7419 2023-04-29 10:55:11.000000 bnlearn-0.8.1/bnlearn/parameter_learning.py
+-rw-rw-rw-   0        0        0    27145 2023-06-14 20:00:44.000000 bnlearn-0.8.1/bnlearn/structure_learning.py
+drwxrwxrwx   0        0        0        0 2023-07-19 07:12:08.122326 bnlearn-0.8.1/bnlearn/tests/
+-rw-rw-rw-   0        0        0        0 2022-11-30 17:18:09.000000 bnlearn-0.8.1/bnlearn/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 07:12:08.137741 bnlearn-0.8.1/bnlearn/tests/discretize/
+-rw-rw-rw-   0        0        0        0 2023-04-29 10:59:05.000000 bnlearn-0.8.1/bnlearn/tests/discretize/__init__.py
+-rw-rw-rw-   0        0        0     2293 2023-04-29 10:59:05.000000 bnlearn-0.8.1/bnlearn/tests/discretize/test_discretize.py
+-rw-rw-rw-   0        0        0     9366 2023-05-12 07:28:13.000000 bnlearn-0.8.1/bnlearn/tests/discretize/test_learn_discrete_bayes_net.py
+-rw-rw-rw-   0        0        0    13436 2023-06-14 20:08:24.000000 bnlearn-0.8.1/bnlearn/tests/test_bnlearn.py
+-rw-rw-rw-   0        0        0     8222 2022-11-30 17:18:09.000000 bnlearn-0.8.1/bnlearn/tests/test_structure_learning.py
+drwxrwxrwx   0        0        0        0 2023-07-19 07:12:08.109733 bnlearn-0.8.1/bnlearn.egg-info/
+-rw-rw-rw-   0        0        0    12276 2023-07-19 07:12:07.000000 bnlearn-0.8.1/bnlearn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      776 2023-07-19 07:12:07.000000 bnlearn-0.8.1/bnlearn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 07:12:07.000000 bnlearn-0.8.1/bnlearn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      204 2023-07-19 07:12:07.000000 bnlearn-0.8.1/bnlearn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-19 07:12:07.000000 bnlearn-0.8.1/bnlearn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-19 07:12:08.142801 bnlearn-0.8.1/setup.cfg
+-rw-rw-rw-   0        0        0     2071 2023-05-16 15:14:21.000000 bnlearn-0.8.1/setup.py
```

### Comparing `bnlearn-0.8.0/LICENSE` & `bnlearn-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.0/MANIFEST.in` & `bnlearn-0.8.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.0/PKG-INFO` & `bnlearn-0.8.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: bnlearn
-Version: 0.8.0
-Summary: Python package for learning the graphical structure of Bayesian networks, parameter learning, inference and sampling methods.
-Home-page: https://erdogant.github.io/bnlearn
-Author: Erdogan Taskesen
-Author-email: erdogant@gmail.com
-License: UNKNOWN
-Download-URL: https://github.com/erdogant/bnlearn/archive/0.8.0.tar.gz
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # bnlearn - Library for Bayesian network learning and inference
 
 [![Python](https://img.shields.io/pypi/pyversions/bnlearn)](https://img.shields.io/pypi/pyversions/bnlearn)
 [![PyPI Version](https://img.shields.io/pypi/v/bnlearn)](https://pypi.org/project/bnlearn/)
 ![GitHub Repo stars](https://img.shields.io/github/stars/erdogant/bnlearn)
 [![License](https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/erdogant/bnlearn/blob/master/LICENSE)
 [![Forks](https://img.shields.io/github/forks/erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/network)
@@ -143,15 +126,15 @@
 * loading bif files
 * conversion of directed to undirected graphs
 
 
 # 
 
 ### Method overview
-Learning a Bayesian network can be split into the underneath problems which are all implemented in this package:
+Learning a Bayesian network can be split into the underneath problems which are all implemented in this package for both discrete, continous and mixed data sets:
 
 * **Structure learning**: Given the data: Estimate a DAG that captures the dependencies between the variables.
    * There are multiple manners to perform structure learning.
       * Exhaustivesearch
       * Hillclimbsearch
       * NaiveBayes
       * TreeSearch
@@ -326,9 +309,7 @@
 Please cite ``bnlearn`` in your publications if this is useful for your research. See column right for citation information.
 
 ### Maintainer
 * Erdogan Taskesen, github: [erdogant](https://github.com/erdogant)
 * Contributions are welcome.
 * If you wish to buy me a <a href="https://erdogant.github.io/donate/?currency=USD&amount=5">Coffee</a> for this work, it is very appreciated :)
 
-
-
```

#### html2text {}

```diff
@@ -1,25 +1,17 @@
-Metadata-Version: 2.1 Name: bnlearn Version: 0.8.0 Summary: Python package for
-learning the graphical structure of Bayesian networks, parameter learning,
-inference and sampling methods. Home-page: https://erdogant.github.io/bnlearn
-Author: Erdogan Taskesen Author-email: erdogant@gmail.com License: UNKNOWN
-Download-URL: https://github.com/erdogant/bnlearn/archive/0.8.0.tar.gz
-Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Requires-Python: >=3 Description-Content-Type: text/markdown
-License-File: LICENSE # bnlearn - Library for Bayesian network learning and
-inference [![Python](https://img.shields.io/pypi/pyversions/bnlearn)](https://
-img.shields.io/pypi/pyversions/bnlearn) [![PyPI Version](https://
-img.shields.io/pypi/v/bnlearn)](https://pypi.org/project/bnlearn/) ![GitHub
-Repo stars](https://img.shields.io/github/stars/erdogant/bnlearn) [![License]
-(https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/
-erdogant/bnlearn/blob/master/LICENSE) [![Forks](https://img.shields.io/github/
-forks/erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/network) [!
-[Open Issues](https://img.shields.io/github/issues/erdogant/bnlearn.svg)]
-(https://github.com/erdogant/bnlearn/issues) [![Project Status](http://
+# bnlearn - Library for Bayesian network learning and inference [![Python]
+(https://img.shields.io/pypi/pyversions/bnlearn)](https://img.shields.io/pypi/
+pyversions/bnlearn) [![PyPI Version](https://img.shields.io/pypi/v/bnlearn)]
+(https://pypi.org/project/bnlearn/) ![GitHub Repo stars](https://
+img.shields.io/github/stars/erdogant/bnlearn) [![License](https://
+img.shields.io/badge/license-MIT-green.svg)](https://github.com/erdogant/
+bnlearn/blob/master/LICENSE) [![Forks](https://img.shields.io/github/forks/
+erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/network) [![Open
+Issues](https://img.shields.io/github/issues/erdogant/bnlearn.svg)](https://
+github.com/erdogant/bnlearn/issues) [![Project Status](http://
 www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/
 #active) [![Downloads](https://pepy.tech/badge/bnlearn/month)](https://
 pepy.tech/project/bnlearn/) [![Downloads](https://pepy.tech/badge/bnlearn)]
 (https://pepy.tech/project/bnlearn) [![DOI](https://zenodo.org/badge/
 231263493.svg)](https://zenodo.org/badge/latestdoi/231263493) [![Docs](https://
 img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/bnlearn/)
 [![Medium](https://img.shields.io/badge/Medium-Blog-black)](https://
@@ -59,51 +51,52 @@
 # Plot graph bn.plot() # To make the directed grapyh undirected
 bn.to_undirected() # Convert to one-hot datamatrix bn.df2onehot() # Derive the
 topological ordering of the (entire) graph bn.topological_sort() # See below
 for the exact working of the functions ``` ##### The following methods are also
 included: * inference * sampling * comparing two networks * loading bif files *
 conversion of directed to undirected graphs # ### Method overview Learning a
 Bayesian network can be split into the underneath problems which are all
-implemented in this package: * **Structure learning**: Given the data: Estimate
-a DAG that captures the dependencies between the variables. * There are
-multiple manners to perform structure learning. * Exhaustivesearch *
-Hillclimbsearch * NaiveBayes * TreeSearch * Chow-liu * Tree-augmented Naive
-Bayes (TAN) * **Parameter learning**: Given the data and DAG: Estimate the
-(conditional) probability distributions of the individual variables. *
-**Inference**: Given the learned model: Determine the exact probability values
-for your queries. # ### Examples A structured overview of all examples are now
-available on the [documentation pages](https://erdogant.github.io/bnlearn/).
-##### Structure learning * [Example: Learn structure on the Sprinkler dataset
-based on a simple dataframe](https://erdogant.github.io/bnlearn/pages/html/
-Examples.html#example-1) * [Example: Comparison method and scoring types types
-for structure learning](https://erdogant.github.io/bnlearn/pages/html/
-Examples.html#example-2) * [Example: Learn structure on more complex dataset
-(Asia)](https://erdogant.github.io/bnlearn/pages/html/Examples.html#example-3)
-##### Parameter learning * [Example: Parameter learning using a DAG and
-dataframe](https://erdogant.github.io/bnlearn/pages/html/
-Examples.html#parameter-learning) ##### Inferences * [Example: Make predictions
-on a dataframe using inference](https://erdogant.github.io/bnlearn/pages/html/
-Predict.html) ##### Sampling * [Example: Sampling to create datasets](https://
-erdogant.github.io/bnlearn/pages/html/Sampling%20and%20datasets.html) #####
-Complete examples * [Example: Create a Bayesian Network, learn its parameters
-from data and perform the inference](https://erdogant.github.io/bnlearn/pages/
-html/Examples.html#create-a-bayesian-network-learn-its-parameters-from-data-
-and-perform-the-inference) * [Example: Use case in the medical domain](https://
-erdogant.github.io/bnlearn/pages/html/UseCases.html) * [Example: Use case
-Titanic](https://erdogant.github.io/bnlearn/pages/html/UseCases.html#) #####
-Plotting * [Example: Interactive plotting](https://erdogant.github.io/bnlearn/
-pages/html/Plot.html#) * [Example: Static plotting](https://erdogant.github.io/
-bnlearn/pages/html/Plot.html#static-plot) * [Example: Comparison of two
-networks](https://erdogant.github.io/bnlearn/pages/html/Plot.html#comparison-
-of-two-networks) ##### Various * [Example: Saving and loading of bnlearn
-models](https://erdogant.github.io/bnlearn/pages/html/
-saving%20and%20loading.html) * [Example: Data conversions such as creating
-sparse datamatrix from source-target and weights](https://erdogant.github.io/
-bnlearn/pages/html/dataframe%20conversions.html?highlight=target#) * [Example:
-Load DAG from BIF files](https://erdogant.github.io/bnlearn/pages/html/
+implemented in this package for both discrete, continous and mixed data sets: *
+**Structure learning**: Given the data: Estimate a DAG that captures the
+dependencies between the variables. * There are multiple manners to perform
+structure learning. * Exhaustivesearch * Hillclimbsearch * NaiveBayes *
+TreeSearch * Chow-liu * Tree-augmented Naive Bayes (TAN) * **Parameter
+learning**: Given the data and DAG: Estimate the (conditional) probability
+distributions of the individual variables. * **Inference**: Given the learned
+model: Determine the exact probability values for your queries. # ### Examples
+A structured overview of all examples are now available on the [documentation
+pages](https://erdogant.github.io/bnlearn/). ##### Structure learning *
+[Example: Learn structure on the Sprinkler dataset based on a simple dataframe]
+(https://erdogant.github.io/bnlearn/pages/html/Examples.html#example-1) *
+[Example: Comparison method and scoring types types for structure learning]
+(https://erdogant.github.io/bnlearn/pages/html/Examples.html#example-2) *
+[Example: Learn structure on more complex dataset (Asia)](https://
+erdogant.github.io/bnlearn/pages/html/Examples.html#example-3) ##### Parameter
+learning * [Example: Parameter learning using a DAG and dataframe](https://
+erdogant.github.io/bnlearn/pages/html/Examples.html#parameter-learning) #####
+Inferences * [Example: Make predictions on a dataframe using inference](https:/
+/erdogant.github.io/bnlearn/pages/html/Predict.html) ##### Sampling * [Example:
+Sampling to create datasets](https://erdogant.github.io/bnlearn/pages/html/
+Sampling%20and%20datasets.html) ##### Complete examples * [Example: Create a
+Bayesian Network, learn its parameters from data and perform the inference]
+(https://erdogant.github.io/bnlearn/pages/html/Examples.html#create-a-bayesian-
+network-learn-its-parameters-from-data-and-perform-the-inference) * [Example:
+Use case in the medical domain](https://erdogant.github.io/bnlearn/pages/html/
+UseCases.html) * [Example: Use case Titanic](https://erdogant.github.io/
+bnlearn/pages/html/UseCases.html#) ##### Plotting * [Example: Interactive
+plotting](https://erdogant.github.io/bnlearn/pages/html/Plot.html#) * [Example:
+Static plotting](https://erdogant.github.io/bnlearn/pages/html/
+Plot.html#static-plot) * [Example: Comparison of two networks](https://
+erdogant.github.io/bnlearn/pages/html/Plot.html#comparison-of-two-networks)
+##### Various * [Example: Saving and loading of bnlearn models](https://
+erdogant.github.io/bnlearn/pages/html/saving%20and%20loading.html) * [Example:
+Data conversions such as creating sparse datamatrix from source-target and
+weights](https://erdogant.github.io/bnlearn/pages/html/
+dataframe%20conversions.html?highlight=target#) * [Example: Load DAG from BIF
+files](https://erdogant.github.io/bnlearn/pages/html/
 Examples.html?highlight=comparison#import-from-bif) # ### Various basic
 examples ```python import bnlearn as bn # Example dataframe sprinkler_data.csv
 can be loaded with: df = bn.import_example() # df = pd.read_csv
 ('sprinkler_data.csv') ``` ##### df looks like this ```python Cloudy Sprinkler
 Rain Wet_Grass 0 0 1 0 1 1 1 1 1 1 2 1 0 1 1 3 0 0 1 1 4 1 0 1 1 .. ... ... ...
 ... 995 0 0 0 0 996 1 0 0 0 997 0 0 1 0 998 1 1 0 1 999 1 0 1 1 ``` ```python
 model = bn.structure_learning.fit(df) # Compute edge strength with the
```

### Comparing `bnlearn-0.8.0/README.md` & `bnlearn-0.8.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: bnlearn
+Version: 0.8.1
+Summary: Python package for learning the graphical structure of Bayesian networks, parameter learning, inference and sampling methods.
+Home-page: https://erdogant.github.io/bnlearn
+Download-URL: https://github.com/erdogant/bnlearn/archive/0.8.1.tar.gz
+Author: Erdogan Taskesen
+Author-email: erdogant@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # bnlearn - Library for Bayesian network learning and inference
 
 [![Python](https://img.shields.io/pypi/pyversions/bnlearn)](https://img.shields.io/pypi/pyversions/bnlearn)
 [![PyPI Version](https://img.shields.io/pypi/v/bnlearn)](https://pypi.org/project/bnlearn/)
 ![GitHub Repo stars](https://img.shields.io/github/stars/erdogant/bnlearn)
 [![License](https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/erdogant/bnlearn/blob/master/LICENSE)
 [![Forks](https://img.shields.io/github/forks/erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/network)
@@ -126,15 +141,15 @@
 * loading bif files
 * conversion of directed to undirected graphs
 
 
 # 
 
 ### Method overview
-Learning a Bayesian network can be split into the underneath problems which are all implemented in this package:
+Learning a Bayesian network can be split into the underneath problems which are all implemented in this package for both discrete, continous and mixed data sets:
 
 * **Structure learning**: Given the data: Estimate a DAG that captures the dependencies between the variables.
    * There are multiple manners to perform structure learning.
       * Exhaustivesearch
       * Hillclimbsearch
       * NaiveBayes
       * TreeSearch
```

#### html2text {}

```diff
@@ -1,9 +1,17 @@
-# bnlearn - Library for Bayesian network learning and inference [![Python]
-(https://img.shields.io/pypi/pyversions/bnlearn)](https://img.shields.io/pypi/
+Metadata-Version: 2.1 Name: bnlearn Version: 0.8.1 Summary: Python package for
+learning the graphical structure of Bayesian networks, parameter learning,
+inference and sampling methods. Home-page: https://erdogant.github.io/bnlearn
+Download-URL: https://github.com/erdogant/bnlearn/archive/0.8.1.tar.gz Author:
+Erdogan Taskesen Author-email: erdogant@gmail.com Classifier: Programming
+Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent Requires-Python: >=3
+Description-Content-Type: text/markdown License-File: LICENSE # bnlearn -
+Library for Bayesian network learning and inference [![Python](https://
+img.shields.io/pypi/pyversions/bnlearn)](https://img.shields.io/pypi/
 pyversions/bnlearn) [![PyPI Version](https://img.shields.io/pypi/v/bnlearn)]
 (https://pypi.org/project/bnlearn/) ![GitHub Repo stars](https://
 img.shields.io/github/stars/erdogant/bnlearn) [![License](https://
 img.shields.io/badge/license-MIT-green.svg)](https://github.com/erdogant/
 bnlearn/blob/master/LICENSE) [![Forks](https://img.shields.io/github/forks/
 erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/network) [![Open
 Issues](https://img.shields.io/github/issues/erdogant/bnlearn.svg)](https://
@@ -51,51 +59,52 @@
 # Plot graph bn.plot() # To make the directed grapyh undirected
 bn.to_undirected() # Convert to one-hot datamatrix bn.df2onehot() # Derive the
 topological ordering of the (entire) graph bn.topological_sort() # See below
 for the exact working of the functions ``` ##### The following methods are also
 included: * inference * sampling * comparing two networks * loading bif files *
 conversion of directed to undirected graphs # ### Method overview Learning a
 Bayesian network can be split into the underneath problems which are all
-implemented in this package: * **Structure learning**: Given the data: Estimate
-a DAG that captures the dependencies between the variables. * There are
-multiple manners to perform structure learning. * Exhaustivesearch *
-Hillclimbsearch * NaiveBayes * TreeSearch * Chow-liu * Tree-augmented Naive
-Bayes (TAN) * **Parameter learning**: Given the data and DAG: Estimate the
-(conditional) probability distributions of the individual variables. *
-**Inference**: Given the learned model: Determine the exact probability values
-for your queries. # ### Examples A structured overview of all examples are now
-available on the [documentation pages](https://erdogant.github.io/bnlearn/).
-##### Structure learning * [Example: Learn structure on the Sprinkler dataset
-based on a simple dataframe](https://erdogant.github.io/bnlearn/pages/html/
-Examples.html#example-1) * [Example: Comparison method and scoring types types
-for structure learning](https://erdogant.github.io/bnlearn/pages/html/
-Examples.html#example-2) * [Example: Learn structure on more complex dataset
-(Asia)](https://erdogant.github.io/bnlearn/pages/html/Examples.html#example-3)
-##### Parameter learning * [Example: Parameter learning using a DAG and
-dataframe](https://erdogant.github.io/bnlearn/pages/html/
-Examples.html#parameter-learning) ##### Inferences * [Example: Make predictions
-on a dataframe using inference](https://erdogant.github.io/bnlearn/pages/html/
-Predict.html) ##### Sampling * [Example: Sampling to create datasets](https://
-erdogant.github.io/bnlearn/pages/html/Sampling%20and%20datasets.html) #####
-Complete examples * [Example: Create a Bayesian Network, learn its parameters
-from data and perform the inference](https://erdogant.github.io/bnlearn/pages/
-html/Examples.html#create-a-bayesian-network-learn-its-parameters-from-data-
-and-perform-the-inference) * [Example: Use case in the medical domain](https://
-erdogant.github.io/bnlearn/pages/html/UseCases.html) * [Example: Use case
-Titanic](https://erdogant.github.io/bnlearn/pages/html/UseCases.html#) #####
-Plotting * [Example: Interactive plotting](https://erdogant.github.io/bnlearn/
-pages/html/Plot.html#) * [Example: Static plotting](https://erdogant.github.io/
-bnlearn/pages/html/Plot.html#static-plot) * [Example: Comparison of two
-networks](https://erdogant.github.io/bnlearn/pages/html/Plot.html#comparison-
-of-two-networks) ##### Various * [Example: Saving and loading of bnlearn
-models](https://erdogant.github.io/bnlearn/pages/html/
-saving%20and%20loading.html) * [Example: Data conversions such as creating
-sparse datamatrix from source-target and weights](https://erdogant.github.io/
-bnlearn/pages/html/dataframe%20conversions.html?highlight=target#) * [Example:
-Load DAG from BIF files](https://erdogant.github.io/bnlearn/pages/html/
+implemented in this package for both discrete, continous and mixed data sets: *
+**Structure learning**: Given the data: Estimate a DAG that captures the
+dependencies between the variables. * There are multiple manners to perform
+structure learning. * Exhaustivesearch * Hillclimbsearch * NaiveBayes *
+TreeSearch * Chow-liu * Tree-augmented Naive Bayes (TAN) * **Parameter
+learning**: Given the data and DAG: Estimate the (conditional) probability
+distributions of the individual variables. * **Inference**: Given the learned
+model: Determine the exact probability values for your queries. # ### Examples
+A structured overview of all examples are now available on the [documentation
+pages](https://erdogant.github.io/bnlearn/). ##### Structure learning *
+[Example: Learn structure on the Sprinkler dataset based on a simple dataframe]
+(https://erdogant.github.io/bnlearn/pages/html/Examples.html#example-1) *
+[Example: Comparison method and scoring types types for structure learning]
+(https://erdogant.github.io/bnlearn/pages/html/Examples.html#example-2) *
+[Example: Learn structure on more complex dataset (Asia)](https://
+erdogant.github.io/bnlearn/pages/html/Examples.html#example-3) ##### Parameter
+learning * [Example: Parameter learning using a DAG and dataframe](https://
+erdogant.github.io/bnlearn/pages/html/Examples.html#parameter-learning) #####
+Inferences * [Example: Make predictions on a dataframe using inference](https:/
+/erdogant.github.io/bnlearn/pages/html/Predict.html) ##### Sampling * [Example:
+Sampling to create datasets](https://erdogant.github.io/bnlearn/pages/html/
+Sampling%20and%20datasets.html) ##### Complete examples * [Example: Create a
+Bayesian Network, learn its parameters from data and perform the inference]
+(https://erdogant.github.io/bnlearn/pages/html/Examples.html#create-a-bayesian-
+network-learn-its-parameters-from-data-and-perform-the-inference) * [Example:
+Use case in the medical domain](https://erdogant.github.io/bnlearn/pages/html/
+UseCases.html) * [Example: Use case Titanic](https://erdogant.github.io/
+bnlearn/pages/html/UseCases.html#) ##### Plotting * [Example: Interactive
+plotting](https://erdogant.github.io/bnlearn/pages/html/Plot.html#) * [Example:
+Static plotting](https://erdogant.github.io/bnlearn/pages/html/
+Plot.html#static-plot) * [Example: Comparison of two networks](https://
+erdogant.github.io/bnlearn/pages/html/Plot.html#comparison-of-two-networks)
+##### Various * [Example: Saving and loading of bnlearn models](https://
+erdogant.github.io/bnlearn/pages/html/saving%20and%20loading.html) * [Example:
+Data conversions such as creating sparse datamatrix from source-target and
+weights](https://erdogant.github.io/bnlearn/pages/html/
+dataframe%20conversions.html?highlight=target#) * [Example: Load DAG from BIF
+files](https://erdogant.github.io/bnlearn/pages/html/
 Examples.html?highlight=comparison#import-from-bif) # ### Various basic
 examples ```python import bnlearn as bn # Example dataframe sprinkler_data.csv
 can be loaded with: df = bn.import_example() # df = pd.read_csv
 ('sprinkler_data.csv') ``` ##### df looks like this ```python Cloudy Sprinkler
 Rain Wet_Grass 0 0 1 0 1 1 1 1 1 1 2 1 0 1 1 3 0 0 1 1 4 1 0 1 1 .. ... ... ...
 ... 995 0 0 0 0 996 1 0 0 0 997 0 0 1 0 998 1 1 0 1 999 1 0 1 1 ``` ```python
 model = bn.structure_learning.fit(df) # Compute edge strength with the
```

### Comparing `bnlearn-0.8.0/bnlearn/__init__.py` & `bnlearn-0.8.1/bnlearn/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 import bnlearn.network as network
 import bnlearn.confmatrix as confmatrix
 from bnlearn.discretize.discretize import discretize, discretize_value
 from packaging import version
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '0.8.0'
+__version__ = '0.8.1'
 
 import pgmpy
 # Check version pgmpy
 if version.parse(pgmpy.__version__) < version.parse("0.1.18"):
     raise ImportError('[bnlearn] >Error: This release requires pgmpy to be version >= 0.1.18. Try to: <pip install -U pgmpy>=0.1.18>')
 
 # Version check
```

### Comparing `bnlearn-0.8.0/bnlearn/bnlearn.py` & `bnlearn-0.8.1/bnlearn/bnlearn.py`

 * *Files 1% similar despite different names*

```diff
@@ -618,30 +618,39 @@
 
         return model
 
     except AttributeError:
         raise AttributeError('[bnlearn] >First get states of variables, edges, parents and network names')
 
 
-def query2df(query, variables=None, verbose=3):
+def query2df(query, variables=None, groupby=None, verbose=3):
     """Convert query from inference model to a dataframe.
 
     Parameters
     ----------
     query : Object from the inference model.
         Convert query object to a dataframe.
     variables : list
         Order or select variables.
+    groupby: list of strings (default: None)
+        The query is grouped on the variable name by taking the maximum P value for each catagory.
 
     Returns
     -------
     df : pd.DataFrame()
         Dataframe with inferences.
 
     """
+    if ((groupby is not None) and np.any(np.isin(groupby, variables))):
+        # Needs to be set to true.
+        groupby = list(np.array(groupby)[np.isin(groupby, variables)])
+    else:
+        if verbose>=2: print('[bnlearn] >Warning: variable(s) [%s] does not exists in DAG.' %(groupby))
+        groupby=None
+
     states = []
     getP = []
     for value_index, prob in enumerate(itertools.product(*[range(card) for card in query.cardinality])):
         states.append(prob)
         getP.append(query.values.ravel()[value_index])
 
     df = pd.DataFrame(data=states, columns=query.scope())
@@ -653,21 +662,27 @@
 
     # Order or filter on input variables
     if variables is not None:
         # Add Pvalue column
         variables = variables + ['p']
         df = df[variables]
 
+    # groupby
+    if groupby is not None:
+        df = df.groupby(groupby).apply(lambda x: x.loc[x['p'].idxmax()])
+        df.reset_index(drop=True, inplace=True)
+
     # Print table to screen
     if verbose>=3:
         print('[bnlearn] >Data is stored in [query.df]')
         print(tabulate(df, tablefmt="grid", headers="keys"))
 
     return df
 
+
 # %% Model Sprinkler
 def _DAG_sprinkler(CPD=True):
     """Create DAG-model for the sprinkler example.
 
     Parameters
     ----------
     CPD : bool, optional
@@ -915,15 +930,15 @@
 
 
 # %% PLOT
 def plot(model,
          pos=None,
          scale=1,
          interactive=False,
-         title='bnlearn_causal_network',
+         title='bnlearn Directed Acyclic Graph (DAG)',
          node_color=None,
          node_size=None,
          node_properties=None,
          edge_properties=None,
          params_interactive={'minmax_distance': [100, 250], 'figsize': (1500, 800), 'notebook': False, 'font_color': 'node_color', 'bgcolor': '#ffffff', 'show_slider': True, 'filepath': None},
          params_static={'minscale': 1, 'maxscale': 10, 'figsize': (15, 10), 'width': None, 'height': None, 'font_size': 14, 'font_family': 'sans-serif', 'alpha': 0.8, 'node_shape': 'o', 'layout': 'spring_layout', 'font_color': '#000000', 'facecolor': 'white', 'edge_alpha': 0.8, 'arrowstyle': '-|>', 'arrowsize': 30, 'visible': True},
          verbose=3):
@@ -1052,17 +1067,25 @@
             tooltip = []
             for node in nodelist:
                 tip = model["model"].get_cpds(node)
                 if tip is None: tip = node
                 tooltip.append(tip)
 
         # Make interactive plot
-        fig = _plot_interactive(params_interactive, nodelist, node_colors, node_sizes, edgelist, edge_colors, edge_weights, title, tooltip, verbose=verbose)
+        fig = _plot_interactive(params_interactive,
+                                nodelist,
+                                node_colors,
+                                node_sizes,
+                                edgelist,
+                                edge_colors,
+                                edge_weights,
+                                title,
+                                tooltip,
+                                verbose=verbose)
     else:
-
         # Bayesian model
         if ('bayes' in str(type(bnmodel)).lower()) or ('pgmpy' in str(type(bnmodel)).lower()):
             if verbose>=3: print('[bnlearn] >Plot based on Bayesian model')
             # positions for all nodes
             G = nx.DiGraph(model['adjmat'])
             pos = bnlearn.network.graphlayout(G, pos=pos, scale=scale, layout=params_static['layout'], verbose=verbose)
         elif 'networkx' in str(type(bnmodel)):
@@ -1072,29 +1095,40 @@
         else:
             if verbose>=3: print('[bnlearn] >Plot based on adjacency matrix')
             G = bnlearn.network.adjmat2graph(model['adjmat'])
             # Get positions
             pos = bnlearn.network.graphlayout(G, pos=pos, scale=scale, layout=params_static['layout'], verbose=verbose)
 
         # Make static plot
-        fig = _plot_static(model, params_static, nodelist, node_colors, node_sizes, G, pos, edge_colors, edge_weights, visible=params_static['visible'])
+        fig = _plot_static(model,
+                           params_static,
+                           nodelist,
+                           node_colors,
+                           node_sizes,
+                           G,
+                           pos,
+                           edge_colors,
+                           edge_weights,
+                           visible=params_static['visible'],
+                           title=title,
+                           )
 
     # Store
     out['fig']=fig
     out['ax']=fig  # Should be removed in later releases
     out['pos']=pos
     out['G']=G
     out['node_properties']=node_properties
     out['edge_properties']=edge_properties
     return out
 
 
 # %% Plot interactive
 # def _plot_static(model, params_static, nodelist, node_colors, node_sizes, title, verbose=3):
-def _plot_static(model, params_static, nodelist, node_colors, node_sizes, G, pos, edge_colors, edge_weights, visible=True):
+def _plot_static(model, params_static, nodelist, node_colors, node_sizes, G, pos, edge_colors, edge_weights, title, visible=True):
     # Bootup figure
     fig = plt.figure(figsize=params_static['figsize'], facecolor=params_static['facecolor'], dpi=100)
     fig.set_visible(visible)
     # nodes
     nx.draw_networkx_nodes(G, pos, nodelist=nodelist, node_size=node_sizes, alpha=params_static['alpha'], node_color=node_colors, node_shape=params_static['node_shape'])
     # edges
     # nx.draw_networkx_edges(G, pos, arrowstyle='-|>', arrowsize=30, edge_color=edge_color, width=edge_weights)
@@ -1102,16 +1136,16 @@
     # Labels
     nx.draw_networkx_labels(G, pos, font_size=params_static['font_size'], font_family=params_static['font_family'], font_color=params_static['font_color'])
     # Plot text of the weights
     # nx.draw_networkx_edge_labels(G, pos, edge_labels=nx.get_edge_attributes(G, 'weight'), font_color=params_static['font_color'])
     # Making figure nice
     # fig = plt.gca()
     # fig.set_axis_off()
-    if visible:
-        plt.show()
+    plt.title(title)
+    if visible: plt.show()
     # Return
     return fig
 
 
 # %% Plot interactive
 def _plot_interactive(params_interactive, nodelist, node_colors, node_sizes, edgelist, edge_colors, edge_weights, title, tooltip, verbose=3):
     # Try to import d3blocks
@@ -1326,15 +1360,15 @@
     >>> import bnlearn as bn
     >>> model = bn.import_DAG('sprinkler')
     >>> fig = bn.plot(model)
 
     """
     out = {}
     model = None
-    filepath= filepath.lower()
+    # filepath= filepath.lower()
     if verbose>=3: print('[bnlearn] >Import <%s>' %(filepath))
     # Get the data properties
     dataproperties = dz.get_dataproperties(filepath)
     # Get path to data
     # PATH_TO_DATA = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'data')
     PATH_TO_DATA = dataproperties['curpath']
 
@@ -1709,19 +1743,17 @@
 
     from sklearn.preprocessing import MinMaxScaler
     weights = MinMaxScaler(feature_range=(minscale, maxscale)).fit_transform(weights).flatten()
     return(weights)
 
 
 # %% Compute structure scores.
-def structure_scores(model, df, scoring_method=['k2', 'bds', 'bic', 'bdeu'], verbose=3, **kwargs):
+def structure_scores(model, df, scoring_method=['k2', 'bic', 'bdeu', 'bds'], verbose=3, **kwargs):
     """Compute structure scores.
 
-    Description
-    -----------
     Each model can be scored based on its structure. However, the score doesn't have very straight forward
     interpretebility but can be used to compare different models. A higher score represents a better fit.
     This method only needs the model structure to compute the score. The structure score functionality
     can be found here: :func:`bnlearn.bnlearn.structure_scores`.
 
     Parameters
     ----------
@@ -1780,15 +1812,15 @@
     # Compute structure scores
     if model is not None:
         for s in scoring_method:
             try:
                 scores[s] = structure_score(model, df, scoring_method=s)
             except:
                 if verbose>=2 and show_message:
-                    print('[bnlearn] >Skipping computing structure score for [%s].' %(s))
+                    print('[bnlearn] >WARNING> Skipping computing structure score for [%s].' %(s))
                     show_message=False
     # Return
     return scores
 
 
 # %%
 # def set_logger(verbose: [str, int] = 'info'):
```

### Comparing `bnlearn-0.8.0/bnlearn/confmatrix.py` & `bnlearn-0.8.1/bnlearn/confmatrix.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.0/bnlearn/discretize/discretize.py` & `bnlearn-0.8.1/bnlearn/discretize/discretize.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 
     Returns
     -------
     pandas DataFrame
         The discretized DataFrame where every continuous column is converted
         into categories.
     """
+    # Convert columns that are object into numerical
+    data = _convert_non_numerical_columns(data, verbose=verbose)
     nodes = list(data.columns)
     graph = _bayes_net_graph(nodes, edges)
     continuous_index = [nodes.index(c) for c in continuous_columns]
 
     data_disc, continuous_edges = discretize_all(
         data,
         graph,
@@ -53,16 +55,24 @@
 
         # TODO Let discretize_all return values starting from zero instead of from one
         data_disc[col] = pd.Categorical.from_codes(data_disc[col] - 1, dtype=dtype)
 
     return data_disc
 
 
+def _convert_non_numerical_columns(df: pd.DataFrame, verbose=3) -> pd.DataFrame:
+    for column in df.columns:
+        if not pd.api.types.is_numeric_dtype(df[column]):
+            df[column] = pd.Categorical(df[column])
+            df[column] = df[column].cat.codes
+
+    return df
+
 def _bayes_net_graph(nodes: List[str], edges: List[Tuple[str, str]]):
-    """
+    """Bayes net graph.
     >>> nodes = ['A', 'B', 'C', 'D']
     >>> edges = [('A', 'B'), ('A', 'C'), ('B', 'D'), ('C', 'D')]
     >>> _bayes_net_graph(nodes, edges)
     [0, (0, 1), (0, 2), (2, 1, 3)]
     """
     sources_and_target = [[target] for target in range(len(nodes))]
```

### Comparing `bnlearn-0.8.0/bnlearn/discretize/learn_discrete_bayes_net.py` & `bnlearn-0.8.1/bnlearn/discretize/learn_discrete_bayes_net.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.0/bnlearn/examples.py` & `bnlearn-0.8.1/bnlearn/examples.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,14 @@
 # Make plot
 bn.plot(model_mle)
 bn.plot(model_mle, interactive=True)
 # bn.independence_test(model, df)
 
 print(model_mle["model"].get_cpds("mpg"))
 
-
 print("Weight categories: ", df_disc["weight"].dtype.categories)
 evidence = {"weight": bn.discretize_value(df_disc["weight"], 3000.0)}
 print(evidence)
 print(bn.inference.fit(model_mle, variables=["mpg"], evidence=evidence, verbose=0))
 
 
 
@@ -311,15 +310,15 @@
 import bnlearn as bn
 df = bn.import_example('random_discrete')
 # Structure learning
 model = bn.structure_learning.fit(df, methodtype='nb', root_node="B", verbose=4, n_jobs=1)
 model = bn.structure_learning.fit(df, methodtype='hc', verbose=4, n_jobs=1)
 model = bn.structure_learning.fit(df, methodtype='cs', verbose=4, n_jobs=1)
 model = bn.structure_learning.fit(df, methodtype='cl', verbose=4, n_jobs=1)
-model = bn.structure_learning.fit(df, methodtype='tan', class_node="A", verbose=4, n_jobs=1)
+model = bn.structure_learning.fit(df, methodtype='tan', class_node="B", verbose=4, n_jobs=1)
 model = bn.structure_learning.fit(df, methodtype='ex', verbose=4, n_jobs=1)
 model = bn.independence_test(model, df, prune=True)
 # Plot
 bn.plot(model)
 
 
 # %%
@@ -1207,14 +1206,15 @@
 print(q1)
 print(q1.df)
 print(q2)
 print(q2.df)
 
 
 # %% Example with mixed dataset: titanic case
+import bnlearn as bn
 # Load example mixed dataset
 df_raw = bn.import_example(data='titanic')
 # Convert to onehot
 dfhot, dfnum = bn.df2onehot(df_raw)
 
 dfnum.loc[0:50, 'Survived'] = 2
 # Structure learning
```

### Comparing `bnlearn-0.8.0/bnlearn/examples_discretize.py` & `bnlearn-0.8.1/bnlearn/examples_discretize.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.0/bnlearn/network.py` & `bnlearn-0.8.1/bnlearn/network.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.0/bnlearn/parameter_learning.py` & `bnlearn-0.8.1/bnlearn/parameter_learning.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.0/bnlearn/structure_learning.py` & `bnlearn-0.8.1/bnlearn/structure_learning.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,30 +8,44 @@
 
 
 # %% Libraries
 import pandas as pd
 import numpy as np
 import matplotlib.pyplot as plt
 
-from pgmpy.estimators import BDeuScore, K2Score, BicScore
 from pgmpy.estimators import ExhaustiveSearch, HillClimbSearch, TreeSearch
 from pgmpy.models import NaiveBayes
 
 import pgmpy
 from packaging import version
 if version.parse(pgmpy.__version__)>=version.parse("0.1.13"):
     from pgmpy.estimators import PC as ConstraintBasedEstimator
 else:
     from pgmpy.estimators import ConstraintBasedEstimator
 
 import bnlearn
 
 
 # %% Structure Learning
-def fit(df, methodtype='hc', scoretype='bic', black_list=None, white_list=None, bw_list_method=None, max_indegree=None, tabu_length=100, epsilon=1e-4, max_iter=1e6, root_node=None, class_node=None, fixed_edges=None, return_all_dags=False, n_jobs=-1, verbose=3):
+def fit(df,
+        methodtype='hc',
+        scoretype='bic',
+        black_list=None,
+        white_list=None,
+        bw_list_method=None,
+        max_indegree=None,
+        tabu_length=100,
+        epsilon=1e-4,
+        max_iter=1e6,
+        root_node=None,
+        class_node=None,
+        fixed_edges=None,
+        return_all_dags=False,
+        n_jobs=-1,
+        verbose=3):
     """Structure learning fit model.
 
     Search strategies for structure learning
     The search space of DAGs is super-exponential in the number of variables and the above scoring functions allow for local maxima.
 
     To learn model structure (a DAG) from a data set, there are three broad techniques:
         1. Score-based structure learning (BIC/BDeu/K2 score; exhaustive search, hill climb/tabu search)
@@ -47,29 +61,37 @@
     Score-based Structure Learning.
     This approach construes model selection as an optimization task. It has two building blocks:
     A scoring function sD:->R that maps models to a numerical score, based on how well they fit to a given data set D.
     A search strategy to traverse the search space of possible models M and select a model with optimal score.
     Commonly used scoring functions to measure the fit between model and data are Bayesian Dirichlet scores such as BDeu or K2 and the Bayesian Information Criterion (BIC, also called MDL).
     BDeu is dependent on an equivalent sample size.
 
+    The BDs score is determined by adjusting certain settings based on the size of the dataset and the observed
+    variable counts. This adjustment involves using a value called "equivalent sample size" divided by the number of
+    parent configurations with observed variable counts. The score-method evaluates how effectively a model can describe the provided dataset.
+
     Parameters
     ----------
     df : pd.DataFrame()
         Input dataframe.
     methodtype : str, (default : 'hc')
         String Search strategy for structure_learning.
         'hc' or 'hillclimbsearch' (default)
         'ex' or 'exhaustivesearch'
         'cs' or 'constraintsearch'
         'cl' or 'chow-liu' (requires setting root_node parameter)
         'nb' or 'naivebayes' (requires <root_node>)
         'tan' (requires <root_node> and <class_node> parameter)
     scoretype : str, (default : 'bic')
         Scoring function for the search spaces.
-        'bic', 'k2', 'bdeu'
+            * 'bic'
+            * 'k2'
+            * 'bdeu'
+            * 'bds'
+            * 'aic'
     black_list : List or None, (default : None)
         List of edges are black listed.
         In case of filtering on nodes, the nodes black listed nodes are removed from the dataframe. The resulting model will not contain any nodes that are in black_list.
     white_list : List or None, (default : None)
         List of edges are white listed.
         In case of filtering on nodes, the search is limited to those edges. The resulting model will then only contain nodes that are in white_list.
         Works only in case of methodtype='hc' See also paramter: `bw_list_method`
@@ -92,15 +114,20 @@
     return_all_dags : Bool, (default: False)
         Return all possible DAGs. Only in case methodtype='exhaustivesearch'
     verbose : int, (default : 3)
         0: None, 1: Error,  2: Warning, 3: Info (default), 4: Debug, 5: Trace
 
     Returns
     -------
-    dict with model.
+    dict with keys:
+        'model' : pgmpy model
+        'model_edges' : Edges
+        'adjmat' : Adjacency matrix
+        'config' : Configurations
+        'structure_scores' : Structure scores (the lower the better)
 
     Examples
     --------
     >>> # Import bnlearn
     >>> import bnlearn as bn
     >>>
     >>> # Load DAG
@@ -120,14 +147,18 @@
     >>>
     >>> # Plot based on structure learning of sampled data
     >>> bn.plot(model_sl, pos=G['pos'])
     >>>
     >>> # Compare networks and make plot
     >>> bn.compare_networks(model, model_sl, pos=G['pos'])
 
+    References
+    ----------
+        * [1] Scutari, Marco. An Empirical-Bayes Score for Discrete Bayesian Networks. Journal of Machine Learning Research, 2016, pp. 438–48
+
     """
     out = []
     # Set config
     config = {'method': methodtype, 'scoring': scoretype, 'black_list': black_list, 'white_list': white_list, 'bw_list_method': bw_list_method, 'max_indegree': max_indegree, 'tabu_length': tabu_length, 'epsilon': epsilon, 'max_iter': max_iter, 'root_node': root_node, 'class_node': class_node, 'fixed_edges': fixed_edges, 'return_all_dags': return_all_dags, 'n_jobs': n_jobs, 'verbose': verbose}
     # Make some checks
     config = _make_checks(df, config, verbose=verbose)
     # Make sure columns are of type string
@@ -194,15 +225,15 @@
     # return
     return out
 
 
 # %% Make Checks
 def _make_checks(df, config, verbose=3):
     assert isinstance(pd.DataFrame(), type(df)), 'df must be of type pd.DataFrame()'
-    if not np.isin(config['scoring'], ['bic', 'k2', 'bdeu']): raise Exception('"scoretype=%s" is invalid.' %(config['scoring']))
+    if not np.isin(config['scoring'], ['bic', 'k2', 'bdeu', 'bds', 'aic']): raise Exception('"scoretype=%s" is invalid.' %(config['scoring']))
     if not np.isin(config['method'], ['naivebayes', 'nb', 'tan', 'cl', 'chow-liu', 'hc', 'ex', 'cs', 'exhaustivesearch', 'hillclimbsearch', 'constraintsearch']): raise Exception('"methodtype=%s" is invalid.' %(config['method']))
 
     if isinstance(config['white_list'], str):
         config['white_list'] = [config['white_list']]
     if isinstance(config['black_list'], str):
         config['black_list'] = [config['black_list']]
 
@@ -488,27 +519,59 @@
             out['scores'].append(score)
             out['dag'].append(dag)
             # print(score, dag.edges())
 
         plt.plot(out['scores'])
         plt.show()
 
-    return(out)
+    return out
 
 
 # %% Set scoring type
-def _SetScoringType(df, scoretype, verbose=3):
+def _SetScoringType(df, scoretype, verbose=3, **kwargs):
+    """Set scoring function.
+
+    Parameters
+    ----------
+    df : pandas DataFrame object
+        dataframe object where each column represents one variable.
+        (If some values in the data are missing the data cells should be set to `numpy.NaN`.
+        Note that pandas converts each column containing `numpy.NaN`s to dtype `float`.)
+    scoretype : string
+        Name of the scoring type method.
+            * bic
+            * k2
+            * bdue
+            * bds
+            * aic
+    verbose : int, (default : 3)
+        0:None, 1:Error, 2:Warning, 3:Info (default), 4:Debug, 5:Trace
+
+    Returns
+    -------
+    scoring method initialized with parameters.
+
+    References
+    ----------
+        * [1] Scutari, Marco. An Empirical-Bayes Score for Discrete Bayesian Networks. Journal of Machine Learning Research, 2016, pp. 438–48
+
+    """
     if verbose>=3: print('[bnlearn] >Set scoring type at [%s]' %(scoretype))
 
     if scoretype=='bic':
-        scoring_method = BicScore(df)
+        scoring_method = pgmpy.estimators.BicScore(df)
     elif scoretype=='k2':
-        scoring_method = K2Score(df)
+        scoring_method = pgmpy.estimators.K2Score(df)
     elif scoretype=='bdeu':
-        scoring_method = BDeuScore(df, equivalent_sample_size=5)
+        scoring_method = pgmpy.estimators.BDeuScore(df, equivalent_sample_size=5)
+    elif scoretype=='bds':
+        scoring_method = pgmpy.estimators.BDsScore(df, equivalent_sample_size=5)
+    elif scoretype=='aic':
+        scoring_method = pgmpy.estimators.AICScore(df)
+
 
     return(scoring_method)
 
 
 # %%
 def _is_independent(model, X, Y, Zs=[], significance_level=0.05):
     return model.test_conditional_independence(X, Y, Zs)[1] >= significance_level
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bnlearn-0.8.0/bnlearn/tests/discretize/test_discretize.py` & `bnlearn-0.8.1/bnlearn/tests/discretize/test_discretize.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.0/bnlearn/tests/discretize/test_learn_discrete_bayes_net.py` & `bnlearn-0.8.1/bnlearn/tests/discretize/test_learn_discrete_bayes_net.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.0/bnlearn/tests/test_bnlearn.py` & `bnlearn-0.8.1/bnlearn/tests/test_bnlearn.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,16 +128,15 @@
     model = bn.import_DAG('sprinkler', CPD=False)
     model_update = bn.parameter_learning.fit(model, df)
     assert [*model_update.keys()] == ['model', 'adjmat', 'config', 'model_edges', 'structure_scores', 'independence_test']
 
 
 def test_inference():
     DAG = bn.import_DAG('sprinkler')
-    q1 = bn.inference.fit(DAG, variables=['Wet_Grass'], evidence={'Rain': 1, 'Sprinkler': 0, 'Cloudy': 1}, to_df=False,
-                          verbose=0)
+    q1 = bn.inference.fit(DAG, variables=['Wet_Grass'], evidence={'Rain': 1, 'Sprinkler': 0, 'Cloudy': 1}, to_df=False, verbose=0)
     assert 'pgmpy.factors.discrete.DiscreteFactor.DiscreteFactor' in str(type(q1))
     assert q1.df is None
     q1 = bn.inference.fit(DAG, variables=['Wet_Grass'], evidence={'Rain': 1, 'Sprinkler': 0, 'Cloudy': 1}, to_df=True,
                           verbose=0)
     assert q1.df is not None
 
 
@@ -324,18 +323,17 @@
              ('Cloudy', 'Rain'),
              ('Sprinkler', 'Wet_Grass'),
              ('Rain', 'Wet_Grass')]
 
     # Make the actual Bayesian DAG
     DAG = bn.make_DAG(edges)
     model = bn.parameter_learning.fit(DAG, df)
-    assert [*model['structure_scores'].keys()] == ['k2', 'bds', 'bic', 'bdeu']
-    assert [*model['structure_scores'].values()] == [-1952.7499005180116, -1961.36196289961, -1953.219110059786,
-                                                     -1954.4304910940107]
+    assert set([*model['structure_scores'].keys()]) == {'bdeu', 'bds', 'bic', 'k2'}
+    assert [*model['structure_scores'].values()] == [-1952.7499005180116, -1953.219110059786, -1954.4304910940107, -1961.36196289961]
     # Print CPDs
     CPD = bn.print_CPD(model)
     bn.check_model(CPD)
     bn.check_model(model)
 
     df = bn.import_example('asia')
     model = bn.structure_learning.fit(df)
-    assert [*model['structure_scores'].keys()] == ['k2', 'bds', 'bic', 'bdeu']
+    assert set([*model['structure_scores'].keys()]) ==  {'bdeu', 'bds', 'bic', 'k2'}
```

### Comparing `bnlearn-0.8.0/bnlearn/tests/test_structure_learning.py` & `bnlearn-0.8.1/bnlearn/tests/test_structure_learning.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.0/bnlearn.egg-info/PKG-INFO` & `bnlearn-0.8.1/bnlearn.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: bnlearn
-Version: 0.8.0
+Version: 0.8.1
 Summary: Python package for learning the graphical structure of Bayesian networks, parameter learning, inference and sampling methods.
 Home-page: https://erdogant.github.io/bnlearn
+Download-URL: https://github.com/erdogant/bnlearn/archive/0.8.1.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
-License: UNKNOWN
-Download-URL: https://github.com/erdogant/bnlearn/archive/0.8.0.tar.gz
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -143,15 +141,15 @@
 * loading bif files
 * conversion of directed to undirected graphs
 
 
 # 
 
 ### Method overview
-Learning a Bayesian network can be split into the underneath problems which are all implemented in this package:
+Learning a Bayesian network can be split into the underneath problems which are all implemented in this package for both discrete, continous and mixed data sets:
 
 * **Structure learning**: Given the data: Estimate a DAG that captures the dependencies between the variables.
    * There are multiple manners to perform structure learning.
       * Exhaustivesearch
       * Hillclimbsearch
       * NaiveBayes
       * TreeSearch
@@ -326,9 +324,7 @@
 Please cite ``bnlearn`` in your publications if this is useful for your research. See column right for citation information.
 
 ### Maintainer
 * Erdogan Taskesen, github: [erdogant](https://github.com/erdogant)
 * Contributions are welcome.
 * If you wish to buy me a <a href="https://erdogant.github.io/donate/?currency=USD&amount=5">Coffee</a> for this work, it is very appreciated :)
 
-
-
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1 Name: bnlearn Version: 0.8.0 Summary: Python package for
+Metadata-Version: 2.1 Name: bnlearn Version: 0.8.1 Summary: Python package for
 learning the graphical structure of Bayesian networks, parameter learning,
 inference and sampling methods. Home-page: https://erdogant.github.io/bnlearn
-Author: Erdogan Taskesen Author-email: erdogant@gmail.com License: UNKNOWN
-Download-URL: https://github.com/erdogant/bnlearn/archive/0.8.0.tar.gz
-Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Requires-Python: >=3 Description-Content-Type: text/markdown
-License-File: LICENSE # bnlearn - Library for Bayesian network learning and
-inference [![Python](https://img.shields.io/pypi/pyversions/bnlearn)](https://
-img.shields.io/pypi/pyversions/bnlearn) [![PyPI Version](https://
-img.shields.io/pypi/v/bnlearn)](https://pypi.org/project/bnlearn/) ![GitHub
-Repo stars](https://img.shields.io/github/stars/erdogant/bnlearn) [![License]
-(https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/
-erdogant/bnlearn/blob/master/LICENSE) [![Forks](https://img.shields.io/github/
-forks/erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/network) [!
-[Open Issues](https://img.shields.io/github/issues/erdogant/bnlearn.svg)]
-(https://github.com/erdogant/bnlearn/issues) [![Project Status](http://
+Download-URL: https://github.com/erdogant/bnlearn/archive/0.8.1.tar.gz Author:
+Erdogan Taskesen Author-email: erdogant@gmail.com Classifier: Programming
+Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent Requires-Python: >=3
+Description-Content-Type: text/markdown License-File: LICENSE # bnlearn -
+Library for Bayesian network learning and inference [![Python](https://
+img.shields.io/pypi/pyversions/bnlearn)](https://img.shields.io/pypi/
+pyversions/bnlearn) [![PyPI Version](https://img.shields.io/pypi/v/bnlearn)]
+(https://pypi.org/project/bnlearn/) ![GitHub Repo stars](https://
+img.shields.io/github/stars/erdogant/bnlearn) [![License](https://
+img.shields.io/badge/license-MIT-green.svg)](https://github.com/erdogant/
+bnlearn/blob/master/LICENSE) [![Forks](https://img.shields.io/github/forks/
+erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/network) [![Open
+Issues](https://img.shields.io/github/issues/erdogant/bnlearn.svg)](https://
+github.com/erdogant/bnlearn/issues) [![Project Status](http://
 www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/
 #active) [![Downloads](https://pepy.tech/badge/bnlearn/month)](https://
 pepy.tech/project/bnlearn/) [![Downloads](https://pepy.tech/badge/bnlearn)]
 (https://pepy.tech/project/bnlearn) [![DOI](https://zenodo.org/badge/
 231263493.svg)](https://zenodo.org/badge/latestdoi/231263493) [![Docs](https://
 img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/bnlearn/)
 [![Medium](https://img.shields.io/badge/Medium-Blog-black)](https://
@@ -59,51 +59,52 @@
 # Plot graph bn.plot() # To make the directed grapyh undirected
 bn.to_undirected() # Convert to one-hot datamatrix bn.df2onehot() # Derive the
 topological ordering of the (entire) graph bn.topological_sort() # See below
 for the exact working of the functions ``` ##### The following methods are also
 included: * inference * sampling * comparing two networks * loading bif files *
 conversion of directed to undirected graphs # ### Method overview Learning a
 Bayesian network can be split into the underneath problems which are all
-implemented in this package: * **Structure learning**: Given the data: Estimate
-a DAG that captures the dependencies between the variables. * There are
-multiple manners to perform structure learning. * Exhaustivesearch *
-Hillclimbsearch * NaiveBayes * TreeSearch * Chow-liu * Tree-augmented Naive
-Bayes (TAN) * **Parameter learning**: Given the data and DAG: Estimate the
-(conditional) probability distributions of the individual variables. *
-**Inference**: Given the learned model: Determine the exact probability values
-for your queries. # ### Examples A structured overview of all examples are now
-available on the [documentation pages](https://erdogant.github.io/bnlearn/).
-##### Structure learning * [Example: Learn structure on the Sprinkler dataset
-based on a simple dataframe](https://erdogant.github.io/bnlearn/pages/html/
-Examples.html#example-1) * [Example: Comparison method and scoring types types
-for structure learning](https://erdogant.github.io/bnlearn/pages/html/
-Examples.html#example-2) * [Example: Learn structure on more complex dataset
-(Asia)](https://erdogant.github.io/bnlearn/pages/html/Examples.html#example-3)
-##### Parameter learning * [Example: Parameter learning using a DAG and
-dataframe](https://erdogant.github.io/bnlearn/pages/html/
-Examples.html#parameter-learning) ##### Inferences * [Example: Make predictions
-on a dataframe using inference](https://erdogant.github.io/bnlearn/pages/html/
-Predict.html) ##### Sampling * [Example: Sampling to create datasets](https://
-erdogant.github.io/bnlearn/pages/html/Sampling%20and%20datasets.html) #####
-Complete examples * [Example: Create a Bayesian Network, learn its parameters
-from data and perform the inference](https://erdogant.github.io/bnlearn/pages/
-html/Examples.html#create-a-bayesian-network-learn-its-parameters-from-data-
-and-perform-the-inference) * [Example: Use case in the medical domain](https://
-erdogant.github.io/bnlearn/pages/html/UseCases.html) * [Example: Use case
-Titanic](https://erdogant.github.io/bnlearn/pages/html/UseCases.html#) #####
-Plotting * [Example: Interactive plotting](https://erdogant.github.io/bnlearn/
-pages/html/Plot.html#) * [Example: Static plotting](https://erdogant.github.io/
-bnlearn/pages/html/Plot.html#static-plot) * [Example: Comparison of two
-networks](https://erdogant.github.io/bnlearn/pages/html/Plot.html#comparison-
-of-two-networks) ##### Various * [Example: Saving and loading of bnlearn
-models](https://erdogant.github.io/bnlearn/pages/html/
-saving%20and%20loading.html) * [Example: Data conversions such as creating
-sparse datamatrix from source-target and weights](https://erdogant.github.io/
-bnlearn/pages/html/dataframe%20conversions.html?highlight=target#) * [Example:
-Load DAG from BIF files](https://erdogant.github.io/bnlearn/pages/html/
+implemented in this package for both discrete, continous and mixed data sets: *
+**Structure learning**: Given the data: Estimate a DAG that captures the
+dependencies between the variables. * There are multiple manners to perform
+structure learning. * Exhaustivesearch * Hillclimbsearch * NaiveBayes *
+TreeSearch * Chow-liu * Tree-augmented Naive Bayes (TAN) * **Parameter
+learning**: Given the data and DAG: Estimate the (conditional) probability
+distributions of the individual variables. * **Inference**: Given the learned
+model: Determine the exact probability values for your queries. # ### Examples
+A structured overview of all examples are now available on the [documentation
+pages](https://erdogant.github.io/bnlearn/). ##### Structure learning *
+[Example: Learn structure on the Sprinkler dataset based on a simple dataframe]
+(https://erdogant.github.io/bnlearn/pages/html/Examples.html#example-1) *
+[Example: Comparison method and scoring types types for structure learning]
+(https://erdogant.github.io/bnlearn/pages/html/Examples.html#example-2) *
+[Example: Learn structure on more complex dataset (Asia)](https://
+erdogant.github.io/bnlearn/pages/html/Examples.html#example-3) ##### Parameter
+learning * [Example: Parameter learning using a DAG and dataframe](https://
+erdogant.github.io/bnlearn/pages/html/Examples.html#parameter-learning) #####
+Inferences * [Example: Make predictions on a dataframe using inference](https:/
+/erdogant.github.io/bnlearn/pages/html/Predict.html) ##### Sampling * [Example:
+Sampling to create datasets](https://erdogant.github.io/bnlearn/pages/html/
+Sampling%20and%20datasets.html) ##### Complete examples * [Example: Create a
+Bayesian Network, learn its parameters from data and perform the inference]
+(https://erdogant.github.io/bnlearn/pages/html/Examples.html#create-a-bayesian-
+network-learn-its-parameters-from-data-and-perform-the-inference) * [Example:
+Use case in the medical domain](https://erdogant.github.io/bnlearn/pages/html/
+UseCases.html) * [Example: Use case Titanic](https://erdogant.github.io/
+bnlearn/pages/html/UseCases.html#) ##### Plotting * [Example: Interactive
+plotting](https://erdogant.github.io/bnlearn/pages/html/Plot.html#) * [Example:
+Static plotting](https://erdogant.github.io/bnlearn/pages/html/
+Plot.html#static-plot) * [Example: Comparison of two networks](https://
+erdogant.github.io/bnlearn/pages/html/Plot.html#comparison-of-two-networks)
+##### Various * [Example: Saving and loading of bnlearn models](https://
+erdogant.github.io/bnlearn/pages/html/saving%20and%20loading.html) * [Example:
+Data conversions such as creating sparse datamatrix from source-target and
+weights](https://erdogant.github.io/bnlearn/pages/html/
+dataframe%20conversions.html?highlight=target#) * [Example: Load DAG from BIF
+files](https://erdogant.github.io/bnlearn/pages/html/
 Examples.html?highlight=comparison#import-from-bif) # ### Various basic
 examples ```python import bnlearn as bn # Example dataframe sprinkler_data.csv
 can be loaded with: df = bn.import_example() # df = pd.read_csv
 ('sprinkler_data.csv') ``` ##### df looks like this ```python Cloudy Sprinkler
 Rain Wet_Grass 0 0 1 0 1 1 1 1 1 1 2 1 0 1 1 3 0 0 1 1 4 1 0 1 1 .. ... ... ...
 ... 995 0 0 0 0 996 1 0 0 0 997 0 0 1 0 998 1 1 0 1 999 1 0 1 1 ``` ```python
 model = bn.structure_learning.fit(df) # Compute edge strength with the
```

### Comparing `bnlearn-0.8.0/bnlearn.egg-info/SOURCES.txt` & `bnlearn-0.8.1/bnlearn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.0/setup.py` & `bnlearn-0.8.1/setup.py`

 * *Files identical despite different names*

