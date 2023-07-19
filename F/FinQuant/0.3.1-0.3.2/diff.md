# Comparing `tmp/FinQuant-0.3.1.tar.gz` & `tmp/FinQuant-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FinQuant-0.3.1.tar", last modified: Sun Jul 16 10:15:15 2023, max compression
+gzip compressed data, was "FinQuant-0.3.2.tar", last modified: Wed Jul 19 11:29:29 2023, max compression
```

## Comparing `FinQuant-0.3.1.tar` & `FinQuant-0.3.2.tar`

### file list

```diff
@@ -1,38 +1,34 @@
-drwxrwxrwx   0 frank     (1000) frank     (1000)        0 2023-07-16 10:15:16.333624 FinQuant-0.3.1/
-drwxrwxrwx   0 frank     (1000) frank     (1000)        0 2023-07-16 10:15:16.088626 FinQuant-0.3.1/FinQuant.egg-info/
--rwxrwxrwx   0 frank     (1000) frank     (1000)    14840 2023-07-16 10:15:15.000000 FinQuant-0.3.1/FinQuant.egg-info/PKG-INFO
--rwxrwxrwx   0 frank     (1000) frank     (1000)      821 2023-07-16 10:15:15.000000 FinQuant-0.3.1/FinQuant.egg-info/SOURCES.txt
--rwxrwxrwx   0 frank     (1000) frank     (1000)        1 2023-07-16 10:15:15.000000 FinQuant-0.3.1/FinQuant.egg-info/dependency_links.txt
--rwxrwxrwx   0 frank     (1000) frank     (1000)      229 2023-07-16 10:15:15.000000 FinQuant-0.3.1/FinQuant.egg-info/requires.txt
--rwxrwxrwx   0 frank     (1000) frank     (1000)        9 2023-07-16 10:15:15.000000 FinQuant-0.3.1/FinQuant.egg-info/top_level.txt
--rwxrwxrwx   0 frank     (1000) frank     (1000)     1059 2023-07-15 13:11:58.000000 FinQuant-0.3.1/LICENSE.txt
--rwxrwxrwx   0 frank     (1000) frank     (1000)    14840 2023-07-16 10:15:16.334127 FinQuant-0.3.1/PKG-INFO
--rwxrwxrwx   0 frank     (1000) frank     (1000)    13659 2023-07-15 16:53:23.000000 FinQuant-0.3.1/README.md
-drwxrwxrwx   0 frank     (1000) frank     (1000)        0 2023-07-16 10:15:16.194124 FinQuant-0.3.1/finquant/
--rwxrwxrwx   0 frank     (1000) frank     (1000)        0 2023-07-15 13:12:00.000000 FinQuant-0.3.1/finquant/__init__.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)     2766 2023-07-16 10:13:37.000000 FinQuant-0.3.1/finquant/asset_test.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)    16730 2023-07-15 16:53:23.000000 FinQuant-0.3.1/finquant/efficient_frontier.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)     3133 2023-07-15 16:53:23.000000 FinQuant-0.3.1/finquant/market.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)     1993 2023-07-15 16:53:23.000000 FinQuant-0.3.1/finquant/minimise_fun.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)    11041 2023-07-15 16:53:23.000000 FinQuant-0.3.1/finquant/monte_carlo.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)     7485 2023-07-15 16:53:23.000000 FinQuant-0.3.1/finquant/moving_average.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)    46879 2023-07-16 10:12:50.000000 FinQuant-0.3.1/finquant/portfolio.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)     3936 2023-07-15 16:53:23.000000 FinQuant-0.3.1/finquant/quants.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)     2219 2023-07-15 16:53:23.000000 FinQuant-0.3.1/finquant/returns.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)     4840 2023-07-15 16:53:23.000000 FinQuant-0.3.1/finquant/stock.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)      301 2023-07-15 16:53:23.000000 FinQuant-0.3.1/pyproject.toml
--rwxrwxrwx   0 frank     (1000) frank     (1000)      106 2023-07-16 10:15:16.337624 FinQuant-0.3.1/setup.cfg
--rwxrwxrwx   0 frank     (1000) frank     (1000)     2200 2023-07-15 16:53:23.000000 FinQuant-0.3.1/setup.py
-drwxrwxrwx   0 frank     (1000) frank     (1000)        0 2023-07-16 10:15:16.321626 FinQuant-0.3.1/tests/
--rwxrwxrwx   0 frank     (1000) frank     (1000)     8254 2023-07-16 10:13:40.000000 FinQuant-0.3.1/tests/test_Example-Analysis.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)     3160 2023-07-16 10:13:40.000000 FinQuant-0.3.1/tests/test_Example-Build-Portfolio-from-file.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)     5489 2023-07-16 10:13:40.000000 FinQuant-0.3.1/tests/test_Example-Build-Portfolio-from-web.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)     6919 2023-07-16 10:13:40.000000 FinQuant-0.3.1/tests/test_Example-Optimisation.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)      212 2023-07-15 13:12:01.000000 FinQuant-0.3.1/tests/test_efficient_frontier.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)     1007 2023-07-15 16:53:23.000000 FinQuant-0.3.1/tests/test_market.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)     6283 2023-07-15 16:53:23.000000 FinQuant-0.3.1/tests/test_moving_average.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)      212 2023-07-15 13:12:01.000000 FinQuant-0.3.1/tests/test_optimisation.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)    15920 2023-07-15 16:53:23.000000 FinQuant-0.3.1/tests/test_portfolio.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)     1278 2023-07-15 16:53:23.000000 FinQuant-0.3.1/tests/test_quants.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)     2244 2023-07-15 16:53:23.000000 FinQuant-0.3.1/tests/test_returns.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)     1928 2023-07-15 16:53:23.000000 FinQuant-0.3.1/tests/test_stock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:29:29.239527 FinQuant-0.3.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:29:29.235527 FinQuant-0.3.2/FinQuant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14840 2023-07-19 11:29:29.000000 FinQuant-0.3.2/FinQuant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-19 11:29:29.000000 FinQuant-0.3.2/FinQuant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 11:29:29.000000 FinQuant-0.3.2/FinQuant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-19 11:29:29.000000 FinQuant-0.3.2/FinQuant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-19 11:29:29.000000 FinQuant-0.3.2/FinQuant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-19 11:28:51.000000 FinQuant-0.3.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14840 2023-07-19 11:29:29.239527 FinQuant-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13659 2023-07-19 11:28:51.000000 FinQuant-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:29:29.239527 FinQuant-0.3.2/finquant/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 11:28:51.000000 FinQuant-0.3.2/finquant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-07-19 11:28:51.000000 FinQuant-0.3.2/finquant/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16730 2023-07-19 11:28:51.000000 FinQuant-0.3.2/finquant/efficient_frontier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-19 11:28:51.000000 FinQuant-0.3.2/finquant/market.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-19 11:28:51.000000 FinQuant-0.3.2/finquant/minimise_fun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-07-19 11:28:51.000000 FinQuant-0.3.2/finquant/monte_carlo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-07-19 11:28:51.000000 FinQuant-0.3.2/finquant/moving_average.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46879 2023-07-19 11:28:51.000000 FinQuant-0.3.2/finquant/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-07-19 11:28:51.000000 FinQuant-0.3.2/finquant/quants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-19 11:28:51.000000 FinQuant-0.3.2/finquant/returns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-07-19 11:28:51.000000 FinQuant-0.3.2/finquant/stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-19 11:28:51.000000 FinQuant-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-19 11:29:29.239527 FinQuant-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-19 11:28:51.000000 FinQuant-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:29:29.239527 FinQuant-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-19 11:28:51.000000 FinQuant-0.3.2/tests/test_efficient_frontier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-19 11:28:51.000000 FinQuant-0.3.2/tests/test_market.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-07-19 11:28:51.000000 FinQuant-0.3.2/tests/test_moving_average.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-19 11:28:51.000000 FinQuant-0.3.2/tests/test_optimisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15920 2023-07-19 11:28:51.000000 FinQuant-0.3.2/tests/test_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-19 11:28:51.000000 FinQuant-0.3.2/tests/test_quants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-19 11:28:51.000000 FinQuant-0.3.2/tests/test_returns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-07-19 11:28:51.000000 FinQuant-0.3.2/tests/test_stock.py
```

### Comparing `FinQuant-0.3.1/FinQuant.egg-info/PKG-INFO` & `FinQuant-0.3.2/FinQuant.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: FinQuant
-Version: 0.3.1
+Version: 0.3.2
 Summary: A program for financial portfolio management, analysis and optimisation
 Home-page: https://github.com/fmilthaler/FinQuant
-Download-URL: https://github.com/fmilthaler/FinQuant/archive/v0.3.1.tar.gz
+Download-URL: https://github.com/fmilthaler/FinQuant/archive/v0.3.2.tar.gz
 Author: Frank Milthaler
 Author-email: f.milthaler@gmail.com
 License: MIT
 Project-URL: Documentation, https://finquant.readthedocs.io
 Keywords: finance,portfolio,investment,numerical,optimisation,monte carlo,efficient frontier,quantitative,quant
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
@@ -32,15 +32,15 @@
 </p>
 
 <p align="center">
   <a href="https://GitHub.com/fmilthaler/FinQuant/stargazers/">
     <img src="https://img.shields.io/github/stars/fmilthaler/FinQuant.svg?style=social&label=Star" alt='pypi'>
   </a>
   <a href="https://pypi.org/project/FinQuant">
-    <img src="https://img.shields.io/badge/pypi-v0.3.0-brightgreen.svg?style=popout" alt='pypi'>
+    <img src="https://img.shields.io/badge/pypi-v0.3.2-brightgreen.svg?style=popout" alt='pypi'>
   </a>
   <a href="https://github.com/fmilthaler/FinQuant">
     <img src="https://github.com/fmilthaler/finquant/actions/workflows/pytest.yml/badge.svg?branch=master" alt='GitHub Actions'>
   </a>
   <a href="http://finquant.readthedocs.io/">
     <img src="https://img.shields.io/readthedocs/finquant.svg?style=popout" alt="docs">
   </a>
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: FinQuant Version: 0.3.1 Summary: A program for
+Metadata-Version: 2.1 Name: FinQuant Version: 0.3.2 Summary: A program for
 financial portfolio management, analysis and optimisation Home-page: https://
 github.com/fmilthaler/FinQuant Download-URL: https://github.com/fmilthaler/
-FinQuant/archive/v0.3.1.tar.gz Author: Frank Milthaler Author-email:
+FinQuant/archive/v0.3.2.tar.gz Author: Frank Milthaler Author-email:
 f.milthaler@gmail.com License: MIT Project-URL: Documentation, https://
 finquant.readthedocs.io Keywords:
 finance,portfolio,investment,numerical,optimisation,monte carlo,efficient
 frontier,quantitative,quant Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education Classifier: Intended Audience ::
 Financial and Insurance Industry Classifier: Intended Audience :: Other
 Audience Classifier: Intended Audience :: Science/Research Classifier:
```

### Comparing `FinQuant-0.3.1/FinQuant.egg-info/SOURCES.txt` & `FinQuant-0.3.2/FinQuant.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -5,28 +5,24 @@
 setup.py
 FinQuant.egg-info/PKG-INFO
 FinQuant.egg-info/SOURCES.txt
 FinQuant.egg-info/dependency_links.txt
 FinQuant.egg-info/requires.txt
 FinQuant.egg-info/top_level.txt
 finquant/__init__.py
-finquant/asset_test.py
+finquant/asset.py
 finquant/efficient_frontier.py
 finquant/market.py
 finquant/minimise_fun.py
 finquant/monte_carlo.py
 finquant/moving_average.py
 finquant/portfolio.py
 finquant/quants.py
 finquant/returns.py
 finquant/stock.py
-tests/test_Example-Analysis.py
-tests/test_Example-Build-Portfolio-from-file.py
-tests/test_Example-Build-Portfolio-from-web.py
-tests/test_Example-Optimisation.py
 tests/test_efficient_frontier.py
 tests/test_market.py
 tests/test_moving_average.py
 tests/test_optimisation.py
 tests/test_portfolio.py
 tests/test_quants.py
 tests/test_returns.py
```

### Comparing `FinQuant-0.3.1/LICENSE.txt` & `FinQuant-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `FinQuant-0.3.1/PKG-INFO` & `FinQuant-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: FinQuant
-Version: 0.3.1
+Version: 0.3.2
 Summary: A program for financial portfolio management, analysis and optimisation
 Home-page: https://github.com/fmilthaler/FinQuant
-Download-URL: https://github.com/fmilthaler/FinQuant/archive/v0.3.1.tar.gz
+Download-URL: https://github.com/fmilthaler/FinQuant/archive/v0.3.2.tar.gz
 Author: Frank Milthaler
 Author-email: f.milthaler@gmail.com
 License: MIT
 Project-URL: Documentation, https://finquant.readthedocs.io
 Keywords: finance,portfolio,investment,numerical,optimisation,monte carlo,efficient frontier,quantitative,quant
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
@@ -32,15 +32,15 @@
 </p>
 
 <p align="center">
   <a href="https://GitHub.com/fmilthaler/FinQuant/stargazers/">
     <img src="https://img.shields.io/github/stars/fmilthaler/FinQuant.svg?style=social&label=Star" alt='pypi'>
   </a>
   <a href="https://pypi.org/project/FinQuant">
-    <img src="https://img.shields.io/badge/pypi-v0.3.0-brightgreen.svg?style=popout" alt='pypi'>
+    <img src="https://img.shields.io/badge/pypi-v0.3.2-brightgreen.svg?style=popout" alt='pypi'>
   </a>
   <a href="https://github.com/fmilthaler/FinQuant">
     <img src="https://github.com/fmilthaler/finquant/actions/workflows/pytest.yml/badge.svg?branch=master" alt='GitHub Actions'>
   </a>
   <a href="http://finquant.readthedocs.io/">
     <img src="https://img.shields.io/readthedocs/finquant.svg?style=popout" alt="docs">
   </a>
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: FinQuant Version: 0.3.1 Summary: A program for
+Metadata-Version: 2.1 Name: FinQuant Version: 0.3.2 Summary: A program for
 financial portfolio management, analysis and optimisation Home-page: https://
 github.com/fmilthaler/FinQuant Download-URL: https://github.com/fmilthaler/
-FinQuant/archive/v0.3.1.tar.gz Author: Frank Milthaler Author-email:
+FinQuant/archive/v0.3.2.tar.gz Author: Frank Milthaler Author-email:
 f.milthaler@gmail.com License: MIT Project-URL: Documentation, https://
 finquant.readthedocs.io Keywords:
 finance,portfolio,investment,numerical,optimisation,monte carlo,efficient
 frontier,quantitative,quant Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education Classifier: Intended Audience ::
 Financial and Insurance Industry Classifier: Intended Audience :: Other
 Audience Classifier: Intended Audience :: Science/Research Classifier:
```

### Comparing `FinQuant-0.3.1/README.md` & `FinQuant-0.3.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 </p>
 
 <p align="center">
   <a href="https://GitHub.com/fmilthaler/FinQuant/stargazers/">
     <img src="https://img.shields.io/github/stars/fmilthaler/FinQuant.svg?style=social&label=Star" alt='pypi'>
   </a>
   <a href="https://pypi.org/project/FinQuant">
-    <img src="https://img.shields.io/badge/pypi-v0.3.0-brightgreen.svg?style=popout" alt='pypi'>
+    <img src="https://img.shields.io/badge/pypi-v0.3.2-brightgreen.svg?style=popout" alt='pypi'>
   </a>
   <a href="https://github.com/fmilthaler/FinQuant">
     <img src="https://github.com/fmilthaler/finquant/actions/workflows/pytest.yml/badge.svg?branch=master" alt='GitHub Actions'>
   </a>
   <a href="http://finquant.readthedocs.io/">
     <img src="https://img.shields.io/readthedocs/finquant.svg?style=popout" alt="docs">
   </a>
```

### Comparing `FinQuant-0.3.1/finquant/efficient_frontier.py` & `FinQuant-0.3.2/finquant/efficient_frontier.py`

 * *Files identical despite different names*

### Comparing `FinQuant-0.3.1/finquant/minimise_fun.py` & `FinQuant-0.3.2/finquant/minimise_fun.py`

 * *Files identical despite different names*

### Comparing `FinQuant-0.3.1/finquant/monte_carlo.py` & `FinQuant-0.3.2/finquant/monte_carlo.py`

 * *Files identical despite different names*

### Comparing `FinQuant-0.3.1/finquant/moving_average.py` & `FinQuant-0.3.2/finquant/moving_average.py`

 * *Files identical despite different names*

### Comparing `FinQuant-0.3.1/finquant/portfolio.py` & `FinQuant-0.3.2/finquant/portfolio.py`

 * *Files identical despite different names*

### Comparing `FinQuant-0.3.1/finquant/quants.py` & `FinQuant-0.3.2/finquant/quants.py`

 * *Files identical despite different names*

### Comparing `FinQuant-0.3.1/finquant/returns.py` & `FinQuant-0.3.2/finquant/returns.py`

 * *Files identical despite different names*

### Comparing `FinQuant-0.3.1/finquant/stock.py` & `FinQuant-0.3.2/finquant/stock.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,108 +1,75 @@
-""" This module provides a public class ``Stock`` that holds and calculates quantities of a single stock.
-Instances of this class are used in the ``Portfolio`` class (provided in ``finquant.portfolio``).   
-Every time a new instance of ``Stock`` is added to ``Portfolio``, the quantities of the portfolio are updated.  
+"""
+This module provides a public class ``Stock`` that represents a single stock or fund.
+Instances of this class are used within the ``Portfolio`` class (provided in ``finquant.portfolio``).
+
+The ``Stock`` class is designed to hold and calculate quantities related to a single stock or fund.
+To initialize an instance of ``Stock``, it requires the following information:
+
+    - ``investmentinfo``: Information about the stock or fund provided as a ``pandas.DataFrame``.
+        The required column labels are ``Name`` and ``Allocation`` for the stock/fund name and allocation,
+        respectively. However, the DataFrame can contain more information beyond these columns,
+        such as year, strategy, currency (CCY), etc.
+
+    - ``data``: Historical price data for the stock or fund provided as a ``pandas.DataFrame``.
+        The data must contain `<stock_name> - Adj. Close`, which represents the closing price used to
+        compute the return on investment. The DataFrame can contain additional columns as well.
+
+The ``Stock`` class computes various quantities related to the stock or fund, such as expected return,
+volatility, skewness, and kurtosis. It also provides functionality to calculate the beta parameter
+of the stock using the CAPM (Capital Asset Pricing Model).
+
+The ``Stock`` class inherits from the ``Asset`` class in ``finquant.asset``, which provides common
+functionality and attributes for financial assets.
+
 """
 
 import numpy as np
 import pandas as pd
-
+from finquant.asset import Asset
 from finquant.returns import daily_returns, historical_mean_return
 
 
-class Stock:
-    """Object that contains information about a stock/fund.
-    To initialise the object, it requires a name, information about
-    the stock/fund given as one of the following data structures:
-
-    - ``pandas.Series``
-    - ``pandas.DataFrame``
-
-    The investment information can contain as little information as its name,
-    and the amount invested in it, the column labels must be ``Name`` and ``Allocation``
-    respectively, but it can also contain more information, such as
-
-    - Year
-    - Strategy
-    - CCY
-    - etc.
-
-    It also requires either data, e.g. daily closing prices as a
-    ``pandas.DataFrame`` or ``pandas.Series``.
-    ``data`` must be given as a ``pandas.DataFrame``, and at least one data column
-    is required to containing the closing price, hence it is required to
-    contain one column label ``<stock_name> - Adj. Close`` which is used to
-    compute the return of investment. However, ``data`` can contain more
-    data in additional columns.
+class Stock(Asset):
+    """Class that contains information about a stock/fund.
+
+    :param investmentinfo: Investment information for the stock as a ``pandas.DataFrame``.
+    :param data: Historical price data for the stock as a ``pandas.DataFrame``.
+
+    The ``Stock`` class extends the ``Asset`` class and represents a specific type of asset,
+    namely a stock within a portfolio.
+    It requires investment information and historical price data for the stock to initialize an instance.
+
+    In addition to the attributes inherited from the ``Asset`` class, the ``Stock`` class provides
+    a method to compute the beta parameter specific to stocks in a portfolio when compared to
+    the market index.
+
     """
 
-    def __init__(self, investmentinfo: pd.DataFrame, data: pd.Series):
+
+    def __init__(self, investmentinfo: pd.DataFrame, data: pd.Series) -> None:
         """
         :Input:
          :investmentinfo: ``pandas.DataFrame`` of investment information
-         :data: ``pandas.DataFrame`` of stock price
+         :data: ``pandas.Series`` of stock price
         """
         self.name = investmentinfo.Name
         self.investmentinfo = investmentinfo
-        self.data = data
-        # compute expected return and volatility of stock
-        self.expected_return = self.comp_expected_return()
-        self.volatility = self.comp_volatility()
-        self.skew = self._comp_skew()
-        self.kurtosis = self._comp_kurtosis()
+        super().__init__(data, self.name, asset_type="Stock")
         # beta parameter of stock (CAPM)
         self.beta = None
 
-    # functions to compute quantities
-    def comp_daily_returns(self):
-        """Computes the daily returns (percentage change).
-        See ``finquant.returns.daily_returns``.
-        """
-        return daily_returns(self.data)
-
-    def comp_expected_return(self, freq=252):
-        """Computes the Expected Return of the stock.
-
-        :Input:
-         :freq: ``int`` (default: ``252``), number of trading days, default
-             value corresponds to trading days in a year
-
-        :Output:
-         :expected_return: Expected Return of stock.
-        """
-        return historical_mean_return(self.data, freq=freq)
-
-    def comp_volatility(self, freq=252):
-        """Computes the Volatility of the stock.
-
-        :Input:
-         :freq: ``int`` (default: ``252``), number of trading days, default
-             value corresponds to trading days in a year
-
-        :Output:
-         :volatility: Volatility of stock.
-        """
-        return self.comp_daily_returns().std() * np.sqrt(freq)
-
-    def _comp_skew(self):
-        """Computes and returns the skewness of the stock."""
-        return self.data.skew()
-
-    def _comp_kurtosis(self):
-        """Computes and returns the Kurtosis of the stock."""
-        return self.data.kurt()
-
     def comp_beta(self, market_daily_returns: pd.Series) -> float:
         """Compute and return the Beta parameter of the stock.
 
         :Input:
          :market_daily_returns: ``pd.Series``, daily returns of the market
 
         :Output:
-         :sharpe: ``float``, the Beta parameter of the stock
+         :beta: ``float``, the Beta parameter of the stock
         """
         cov_mat = np.cov(
             self.comp_daily_returns(),
             market_daily_returns.to_frame()[market_daily_returns.name],
         )
 
         beta = cov_mat[0, 1] / cov_mat[1, 1]
@@ -112,22 +79,18 @@
     def properties(self):
         """Nicely prints out the properties of the stock: Expected Return,
         Volatility, Skewness, Kurtosis as well as the ``Allocation`` (and other
         information provided in investmentinfo.)
         """
         # nicely printing out information and quantities of the stock
         string = "-" * 50
-        string += f"\nStock: {self.name}"
+        string += f"\n{self.asset_type}: {self.name}"
         string += f"\nExpected Return: {self.expected_return:0.3f}"
         string += f"\nVolatility: {self.volatility:0.3f}"
         string += f"\nSkewness: {self.skew:0.5f}"
         string += f"\nKurtosis: {self.kurtosis:0.5f}"
+        if self.beta is not None:
+            string += f"\n{self.asset_type} Beta: {self.beta:0.3f}"
         string += "\nInformation:"
         string += "\n" + str(self.investmentinfo.to_frame().transpose())
-        string += "\n"
-        string += "-" * 50
-        print(string)
-
-    def __str__(self):
-        # print short description
-        string = "Contains information about " + str(self.name) + "."
-        return string
+        string += "\n" + "-" * 50
+        print(string)
```

### Comparing `FinQuant-0.3.1/setup.py` & `FinQuant-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `FinQuant-0.3.1/tests/test_market.py` & `FinQuant-0.3.2/tests/test_market.py`

 * *Files identical despite different names*

### Comparing `FinQuant-0.3.1/tests/test_moving_average.py` & `FinQuant-0.3.2/tests/test_moving_average.py`

 * *Files identical despite different names*

### Comparing `FinQuant-0.3.1/tests/test_portfolio.py` & `FinQuant-0.3.2/tests/test_portfolio.py`

 * *Files identical despite different names*

### Comparing `FinQuant-0.3.1/tests/test_quants.py` & `FinQuant-0.3.2/tests/test_quants.py`

 * *Files identical despite different names*

### Comparing `FinQuant-0.3.1/tests/test_returns.py` & `FinQuant-0.3.2/tests/test_returns.py`

 * *Files identical despite different names*

### Comparing `FinQuant-0.3.1/tests/test_stock.py` & `FinQuant-0.3.2/tests/test_stock.py`

 * *Files identical despite different names*

