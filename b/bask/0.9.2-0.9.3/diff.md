# Comparing `tmp/bask-0.9.2.tar.gz` & `tmp/bask-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bask-0.9.2.tar", last modified: Mon Sep 14 20:59:18 2020, max compression
+gzip compressed data, was "bask-0.9.3.tar", last modified: Mon Sep 14 21:01:52 2020, max compression
```

## Comparing `bask-0.9.2.tar` & `bask-0.9.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      592 2020-09-14 20:55:25.917535 bask-0.9.2/LICENSE
--rw-r--r--   0        0        0     2099 2020-09-14 20:55:25.917535 bask-0.9.2/README.rst
--rw-r--r--   0        0        0      571 2020-09-14 20:55:25.917535 bask-0.9.2/bask/__init__.py
--rw-r--r--   0        0        0    11111 2020-09-14 20:55:25.921533 bask-0.9.2/bask/acquisition.py
--rw-r--r--   0        0        0    29658 2020-09-14 20:55:25.921533 bask-0.9.2/bask/bayesgpr.py
--rw-r--r--   0        0        0      373 2020-09-14 20:55:25.921533 bask-0.9.2/bask/cli.py
--rw-r--r--   0        0        0    25994 2020-09-14 20:55:25.921533 bask-0.9.2/bask/optimizer.py
--rw-r--r--   0        0        0     1767 2020-09-14 20:55:25.921533 bask-0.9.2/bask/priors.py
--rw-r--r--   0        0        0    18102 2020-09-14 20:55:25.921533 bask-0.9.2/bask/searchcv.py
--rw-r--r--   0        0        0     7915 2020-09-14 20:55:25.921533 bask-0.9.2/bask/utils.py
--rw-r--r--   0        0        0     1796 2020-09-14 20:55:25.925531 bask-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     3368 2020-09-14 20:59:18.211925 bask-0.9.2/setup.py
--rw-r--r--   0        0        0     3771 2020-09-14 20:59:18.212366 bask-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0      592 2020-09-14 20:58:03.926459 bask-0.9.3/LICENSE
+-rw-r--r--   0        0        0     2099 2020-09-14 20:58:03.926459 bask-0.9.3/README.rst
+-rw-r--r--   0        0        0      571 2020-09-14 20:58:03.926459 bask-0.9.3/bask/__init__.py
+-rw-r--r--   0        0        0    11111 2020-09-14 20:58:03.926459 bask-0.9.3/bask/acquisition.py
+-rw-r--r--   0        0        0    29658 2020-09-14 20:58:03.926459 bask-0.9.3/bask/bayesgpr.py
+-rw-r--r--   0        0        0      373 2020-09-14 20:58:03.926459 bask-0.9.3/bask/cli.py
+-rw-r--r--   0        0        0    25994 2020-09-14 20:58:03.926459 bask-0.9.3/bask/optimizer.py
+-rw-r--r--   0        0        0     1767 2020-09-14 20:58:03.926459 bask-0.9.3/bask/priors.py
+-rw-r--r--   0        0        0    18102 2020-09-14 20:58:03.926459 bask-0.9.3/bask/searchcv.py
+-rw-r--r--   0        0        0     7915 2020-09-14 20:58:03.926459 bask-0.9.3/bask/utils.py
+-rw-r--r--   0        0        0     1796 2020-09-14 20:58:03.934463 bask-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     3368 2020-09-14 21:01:52.105527 bask-0.9.3/setup.py
+-rw-r--r--   0        0        0     3771 2020-09-14 21:01:52.105980 bask-0.9.3/PKG-INFO
```

### Comparing `bask-0.9.2/LICENSE` & `bask-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bask-0.9.2/README.rst` & `bask-0.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `bask-0.9.2/bask/__init__.py` & `bask-0.9.3/bask/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for Bayes-skopt."""
 
 __author__ = """Karlson Pfannschmidt"""
 __email__ = "kiudee@mail.upb.de"
-__version__ = "0.9.2"
+__version__ = "0.9.3"
 
 from .acquisition import *
 from .bayesgpr import BayesGPR
 from .optimizer import Optimizer
 from .searchcv import BayesSearchCV
 from .utils import guess_priors
```

### Comparing `bask-0.9.2/bask/acquisition.py` & `bask-0.9.3/bask/acquisition.py`

 * *Files identical despite different names*

### Comparing `bask-0.9.2/bask/bayesgpr.py` & `bask-0.9.3/bask/bayesgpr.py`

 * *Files 0% similar despite different names*

```diff
@@ -447,16 +447,16 @@
         # We are only able to guess priors now, since BayesGPR can add
         # another WhiteKernel, when noise is set to "gaussian":
         if priors is None:
             priors = guess_priors(self.kernel_)
 
         if warp_priors is None:
             warp_priors = (
-                st.norm(loc=0.0, scale=0.5).logpdf,
-                st.norm(loc=0.0, scale=0.5).logpdf,
+                st.norm(loc=0.0, scale=0.3).logpdf,
+                st.norm(loc=0.0, scale=0.3).logpdf,
             )
 
         # Update data, if available:
         if X is not None:
             if self.normalize_y:
                 self.y_train_mean_ = np.mean(y, axis=0)
                 y = y - self.y_train_mean_
```

### Comparing `bask-0.9.2/bask/optimizer.py` & `bask-0.9.3/bask/optimizer.py`

 * *Files identical despite different names*

### Comparing `bask-0.9.2/bask/priors.py` & `bask-0.9.3/bask/priors.py`

 * *Files identical despite different names*

### Comparing `bask-0.9.2/bask/searchcv.py` & `bask-0.9.3/bask/searchcv.py`

 * *Files identical despite different names*

### Comparing `bask-0.9.2/bask/utils.py` & `bask-0.9.3/bask/utils.py`

 * *Files identical despite different names*

### Comparing `bask-0.9.2/pyproject.toml` & `bask-0.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bask"
-version = "0.9.2"
+version = "0.9.3"
 description = "A fully Bayesian implementation of sequential model-based optimization"
 authors = ["Karlson Pfannschmidt <kiudee@mail.upb.de>"]
 license = "Apache-2.0"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
```

### Comparing `bask-0.9.2/setup.py` & `bask-0.9.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
           'nbsphinx-link>=1.3.0,<2.0.0']}
 
 entry_points = \
 {'console_scripts': ['bask = bask.cli:main']}
 
 setup_kwargs = {
     'name': 'bask',
-    'version': '0.9.2',
+    'version': '0.9.3',
     'description': 'A fully Bayesian implementation of sequential model-based optimization',
     'long_description': '\n\n\n.. image:: https://github.com/kiudee/bayes-skopt/raw/master/docs/images/header.png\n   :width: 800 px\n   :alt: Bayes-skopt header\n   :align: center\n\n===========\nBayes-skopt\n===========\n\n.. image:: https://mybinder.org/badge_logo.svg\n        :target: https://mybinder.org/v2/gh/kiudee/bayes-skopt/master?filepath=examples\n\n.. image:: https://img.shields.io/pypi/v/bask.svg\n        :target: https://pypi.python.org/pypi/bask\n\n.. image:: https://img.shields.io/travis/kiudee/bayes-skopt.svg\n        :target: https://travis-ci.org/kiudee/bayes-skopt\n\n.. image:: https://readthedocs.org/projects/bayes-skopt/badge/?version=latest\n        :target: https://bayes-skopt.readthedocs.io/en/latest/?badge=latest\n        :alt: Documentation Status\n\nA fully Bayesian implementation of sequential model-based optimization\n\n\n* Free software: Apache Software License 2.0\n* Documentation: https://bayes-skopt.readthedocs.io.\n* Built on top of the excellent `Scikit-Optimize (skopt) <https://github.com/scikit-optimize/scikit-optimize>`__.\n\n\nFeatures\n--------\n\n- A **fully Bayesian** variant of the ``GaussianProcessRegressor``.\n- State of the art information-theoretic acquisition functions, such as the\n  `Max-value entropy search <https://arxiv.org/abs/1703.01968>`__ or\n  `Predictive variance reduction search <https://bayesopt.github.io/papers/2017/13.pdf>`__, for even faster\n  convergence in simple regret.\n- Familiar `Optimizer` interface known from Scikit-Optimize.\n\nInstallation\n------------\n\nTo install the latest stable release it is best to install the version on PyPI::\n\n   pip install bask\n\nThe latest development version of Bayes-skopt can be installed from Github as follows::\n\n   pip install git+https://github.com/kiudee/bayes-skopt\n\nAnother option is to clone the repository and install Bayes-skopt using::\n\n   poetry install\n\nCredits\n-------\n\nThis package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.\n\n.. _Cookiecutter: https://github.com/audreyr/cookiecutter\n.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage\n',
     'author': 'Karlson Pfannschmidt',
     'author_email': 'kiudee@mail.upb.de',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/kiudee/bayes-skopt',
```

### Comparing `bask-0.9.2/PKG-INFO` & `bask-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bask
-Version: 0.9.2
+Version: 0.9.3
 Summary: A fully Bayesian implementation of sequential model-based optimization
 Home-page: https://github.com/kiudee/bayes-skopt
 License: Apache-2.0
 Keywords: optimization,bayesian,hyperparameters,robust
 Author: Karlson Pfannschmidt
 Author-email: kiudee@mail.upb.de
 Requires-Python: >=3.7,<4.0
```

