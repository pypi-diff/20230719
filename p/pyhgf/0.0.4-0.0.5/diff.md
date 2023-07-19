# Comparing `tmp/pyhgf-0.0.4.tar.gz` & `tmp/pyhgf-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhgf-0.0.4.tar", last modified: Tue Apr 18 16:32:25 2023, max compression
+gzip compressed data, was "pyhgf-0.0.5.tar", last modified: Wed Jul 19 13:06:04 2023, max compression
```

## Comparing `pyhgf-0.0.4.tar` & `pyhgf-0.0.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:32:25.313437 pyhgf-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    34493 2023-04-18 16:32:14.000000 pyhgf-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-18 16:32:14.000000 pyhgf-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-04-18 16:32:25.313437 pyhgf-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-04-18 16:32:14.000000 pyhgf-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:32:25.309437 pyhgf-0.0.4/pyhgf/
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-18 16:32:14.000000 pyhgf-0.0.4/pyhgf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12219 2023-04-18 16:32:14.000000 pyhgf-0.0.4/pyhgf/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)    13268 2023-04-18 16:32:14.000000 pyhgf-0.0.4/pyhgf/continuous.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:32:25.309437 pyhgf-0.0.4/pyhgf/data/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-18 16:32:14.000000 pyhgf-0.0.4/pyhgf/data/binary_input.dat
--rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-04-18 16:32:14.000000 pyhgf-0.0.4/pyhgf/data/usdchf.dat
--rw-r--r--   0 runner    (1001) docker     (123)    20862 2023-04-18 16:32:14.000000 pyhgf-0.0.4/pyhgf/distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)    24111 2023-04-18 16:32:14.000000 pyhgf-0.0.4/pyhgf/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10413 2023-04-18 16:32:14.000000 pyhgf-0.0.4/pyhgf/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-04-18 16:32:14.000000 pyhgf-0.0.4/pyhgf/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-18 16:32:14.000000 pyhgf-0.0.4/pyhgf/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-18 16:32:14.000000 pyhgf-0.0.4/pyhgf/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:32:25.309437 pyhgf-0.0.4/pyhgf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-04-18 16:32:25.000000 pyhgf-0.0.4/pyhgf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-18 16:32:25.000000 pyhgf-0.0.4/pyhgf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 16:32:25.000000 pyhgf-0.0.4/pyhgf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-18 16:32:25.000000 pyhgf-0.0.4/pyhgf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-18 16:32:25.000000 pyhgf-0.0.4/pyhgf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 16:32:25.313437 pyhgf-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-18 16:32:14.000000 pyhgf-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:32:25.309437 pyhgf-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-04-18 16:32:14.000000 pyhgf-0.0.4/tests/test_binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-04-18 16:32:14.000000 pyhgf-0.0.4/tests/test_continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)    12394 2023-04-18 16:32:14.000000 pyhgf-0.0.4/tests/test_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-04-18 16:32:14.000000 pyhgf-0.0.4/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-18 16:32:14.000000 pyhgf-0.0.4/tests/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-18 16:32:14.000000 pyhgf-0.0.4/tests/test_structure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:06:04.537768 pyhgf-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    34493 2023-07-19 13:05:51.000000 pyhgf-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-19 13:05:51.000000 pyhgf-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-07-19 13:06:04.537768 pyhgf-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7043 2023-07-19 13:05:51.000000 pyhgf-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:06:04.533768 pyhgf-0.0.5/pyhgf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-19 13:05:52.000000 pyhgf-0.0.5/pyhgf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12762 2023-07-19 13:05:52.000000 pyhgf-0.0.5/pyhgf/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16891 2023-07-19 13:05:52.000000 pyhgf-0.0.5/pyhgf/continuous.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:06:04.533768 pyhgf-0.0.5/pyhgf/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-19 13:05:52.000000 pyhgf-0.0.5/pyhgf/data/binary_input.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-07-19 13:05:52.000000 pyhgf-0.0.5/pyhgf/data/usdchf.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    21572 2023-07-19 13:05:52.000000 pyhgf-0.0.5/pyhgf/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33021 2023-07-19 13:05:52.000000 pyhgf-0.0.5/pyhgf/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10389 2023-07-19 13:05:52.000000 pyhgf-0.0.5/pyhgf/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-07-19 13:05:52.000000 pyhgf-0.0.5/pyhgf/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-07-19 13:05:52.000000 pyhgf-0.0.5/pyhgf/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-19 13:05:52.000000 pyhgf-0.0.5/pyhgf/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:06:04.533768 pyhgf-0.0.5/pyhgf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-07-19 13:06:04.000000 pyhgf-0.0.5/pyhgf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-19 13:06:04.000000 pyhgf-0.0.5/pyhgf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 13:06:04.000000 pyhgf-0.0.5/pyhgf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-19 13:06:04.000000 pyhgf-0.0.5/pyhgf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-19 13:06:04.000000 pyhgf-0.0.5/pyhgf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 13:06:04.537768 pyhgf-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-19 13:05:52.000000 pyhgf-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:06:04.537768 pyhgf-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-07-19 13:05:52.000000 pyhgf-0.0.5/tests/test_binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9361 2023-07-19 13:05:52.000000 pyhgf-0.0.5/tests/test_continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12315 2023-07-19 13:05:52.000000 pyhgf-0.0.5/tests/test_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-07-19 13:05:52.000000 pyhgf-0.0.5/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-07-19 13:05:52.000000 pyhgf-0.0.5/tests/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-07-19 13:05:52.000000 pyhgf-0.0.5/tests/test_structure.py
```

### Comparing `pyhgf-0.0.4/LICENSE` & `pyhgf-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhgf-0.0.4/PKG-INFO` & `pyhgf-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhgf
-Version: 0.0.4
+Version: 0.0.5
 Summary: The generalized, nodalized HGF for predictive coding.
 Author: ILAB
 Author-email: nicolas.legrand@cas.au.dk
 Maintainer: Nicolas Legrand
 Maintainer-email: nicolas.legrand@cas.au.dk
 License: GPL-3.0
 Description-Content-Type: text/markdown
@@ -12,60 +12,60 @@
 
 <img src="docs/source/images/logo.svg" align="center" alt="hgf" VSPACE=30>
 
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit) [![license](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://github.com/ilabcode/pyhgf/blob/master/LICENSE) [![codecov](https://codecov.io/gh/ilabcode/pyhgf/branch/master/graph/badge.svg)](https://codecov.io/gh/ilabcode/pyhgf) [![black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/) [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/) [![pip](https://badge.fury.io/py/pyhgf.svg)](https://badge.fury.io/py/pyhgf)
 
 # The multilevel, generalized and nodalized Hierarchical Gaussian Filter for predictive coding
 
-pyhgf is a Python library that implements the generalized, nodalized and multilevel Hierarchical Gaussian Filters for predictive coding written on top of [JAX](https://jax.readthedocs.io/en/latest/jax.html). The library can create and manipulate graph neural networks that perform beliefs update throught the diffusion of precision-weighted prediction errors under new observations. The core functions are derivable, JIT-able, and are designed to interface smoothly with other libraries in the JAX ecosystem for Bayesian inference.
+pyhgf is a Python library that implements the generalized, nodalized and multilevel Hierarchical Gaussian Filters for predictive coding written on top of [JAX](https://jax.readthedocs.io/en/latest/jax.html). The library can create and manipulate graph neural networks that perform belief update through the diffusion of precision-weighted prediction errors under new observations. The core functions are derivable, JIT-able, and are designed to interface smoothly with other libraries in the JAX ecosystem for Bayesian inference.
 
 * 🎓 [What is a Hierarchical Gaussian Filter?](https://ilabcode.github.io/pyhgf/theory.html)  
 * 📖 [API Documentation](https://ilabcode.github.io/pyhgf/)  
 * ✏️ [Tutorials and examples](https://ilabcode.github.io/pyhgf/tutorials.html)  
 
 ## Getting started
 
 ### Installation
 
-The last official release can be download from PIP:
+The last official release can be downloaded from PIP:
 
 `pip install pyhgf`
 
 The current version under development can be installed from the master branch of the GitHub folder:
 
 `pip install “git+https://github.com/ilabcode/pyhgf.git”`
 
 ### How does it works?
 
 The nodalized Hierarchical Gaussian Filter consists of a network of probabilistic nodes hierarchically structured where each node can inherit its value and volatility sufficient statistics from other parents node. The presentation of a new observation at the lower level of the hierarchy (i.e. the input node) triggers a recursive update of the nodes' belief through the bottom-up propagation of precision-weighted prediction error.
 
 More generally, pyhgf operates on graph neural networks that can be defined and updated through the following variables:
 
 * The node parameters (dictionary) that store each node's parameters (value, precision, learning rates, volatility coupling, ...).
-* The node structure (tuple) that list, for each node, the indexes of the value and volatility parents.
+* The node structure (tuple) that lists, for each node, the indexes of the value and volatility parents.
 * A set of update functions that operate on any of the 3 other variables, starting from a target node.
 * An update sequence (tuple) that define the order in which the update functions are called, and the target node.
 
-![png](./docs/source/images/graph_network.png)
+![png](./docs/source/images/graph_networks.svg)
 
 Value parent and volatility parent are nodes themself. Any node can be a value and/or volatility parent for other nodes and have multiple value and/or volatility parents. A filtering structure consists of nodes embedding other nodes hierarchically. Nodes are parametrized by their sufficient statistic and parents. The transformations between nodes can be linear, non-linear, or any function (thus a *generalization* of the HGF).
 
-The resulting probabilistic network operates as a filter towards new observation. If a decision function (taking the whole model as a parameter) is also defined, behaviours can be triggered accordingly. By comparing those behaviours with actual outcomes, a surprise function can be optimized over the range of parameters of interest.
+The resulting probabilistic network operates as a filter toward new observation. If a decision function (taking the whole model as a parameter) is also defined, behaviors can be triggered accordingly. By comparing those behaviors with actual outcomes, a surprise function can be optimized over the range of parameters of interest.
 
 ### The Hierarchical Gaussian Filter
 
 The Hierarchical Gaussian Filter for binary and continuous inputs as it was described in Mathys et al. (2011, 2014), and later implemented in the Matlab Tapas toolbox (Frässle et al. 2021), can be seen as a special case of this node structure such as:
 
 ![Figure2](./docs/source/images/hgf.png)
 
 The pyhgf package includes pre-implemented standard HGF models that can be used together with other neural network libraries of Bayesian inference tools. It is also possible for the user to build custom network structures that would match specific needs.
 
 ### Model fitting
 
-Here we demonstrate how to fit a two-level binary Hierarchical Gaussian filter. The input time series are binary outcome from Iglesias et al. (2013).
+Here we demonstrate how to fit a two-level binary Hierarchical Gaussian filter. The input time series are the binary outcomes from Iglesias et al. (2013).
 
 ```python
 from pyhgf.model import HGF
 from pyhgf import load_data
 
 # Load time series example data
 timeserie = load_data("binary")
@@ -95,15 +95,15 @@
 `Add 320 new binary observations.`  
 `Model's surprise = 203.29249572753906`
 
 ![png](./docs/source/images/trajectories.png)
 
 # Acknoledgements
 
-This implementation of the Hierarchical Gaussian Filter was largely inspired by the original [Matlab version](https://translationalneuromodeling.github.io/tapas). A Julia implementation of the generalised, nodalised and multilevel HGF is also available [here](https://github.com/ilabcode/HGF.jl).
+This implementation of the Hierarchical Gaussian Filter was largely inspired by the original [Matlab version](https://translationalneuromodeling.github.io/tapas). A Julia implementation of the generalized, nodalised and multilevel HGF is also available [here](https://github.com/ilabcode/HGF.jl).
 
 ## References
 
 1. Mathys, C. (2011). A Bayesian foundation for individual learning under uncertainty. In Frontiers in Human Neuroscience (Vol. 5). Frontiers Media SA. https://doi.org/10.3389/fnhum.2011.00039
 2. Mathys, C. D., Lomakina, E. I., Daunizeau, J., Iglesias, S., Brodersen, K. H., Friston, K. J., & Stephan, K. E. (2014). Uncertainty in perception and the hierarchical Gaussian filter. Frontiers in Human Neuroscience, 8. https://doi.org/10.3389/fnhum.2014.00825
 3. Powers, A. R., Mathys, C., & Corlett, P. R. (2017). Pavlovian conditioning-induced hallucinations result from overweighting of perceptual priors. Science (New York, N.Y.), 357(6351), 596–600. https://doi.org/10.1126/science.aan3458
 4. Frässle, S., Aponte, E. A., Bollmann, S., Brodersen, K. H., Do, C. T., Harrison, O. K., Harrison, S. J., Heinzle, J., Iglesias, S., Kasper, L., Lomakina, E. I., Mathys, C., Müller-Schrader, M., Pereira, I., Petzschner, F. H., Raman, S., Schöbi, D., Toussaint, B., Weber, L. A., … Stephan, K. E. (2021). TAPAS: An Open-Source Software Package for Translational Neuromodeling and Computational Psychiatry. In Frontiers in Psychiatry (Vol. 12). Frontiers Media SA. https://doi.org/10.3389/fpsyt.2021.680811
```

### Comparing `pyhgf-0.0.4/README.md` & `pyhgf-0.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 <img src="docs/source/images/logo.svg" align="center" alt="hgf" VSPACE=30>
 
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit) [![license](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://github.com/ilabcode/pyhgf/blob/master/LICENSE) [![codecov](https://codecov.io/gh/ilabcode/pyhgf/branch/master/graph/badge.svg)](https://codecov.io/gh/ilabcode/pyhgf) [![black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/) [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/) [![pip](https://badge.fury.io/py/pyhgf.svg)](https://badge.fury.io/py/pyhgf)
 
 # The multilevel, generalized and nodalized Hierarchical Gaussian Filter for predictive coding
 
-pyhgf is a Python library that implements the generalized, nodalized and multilevel Hierarchical Gaussian Filters for predictive coding written on top of [JAX](https://jax.readthedocs.io/en/latest/jax.html). The library can create and manipulate graph neural networks that perform beliefs update throught the diffusion of precision-weighted prediction errors under new observations. The core functions are derivable, JIT-able, and are designed to interface smoothly with other libraries in the JAX ecosystem for Bayesian inference.
+pyhgf is a Python library that implements the generalized, nodalized and multilevel Hierarchical Gaussian Filters for predictive coding written on top of [JAX](https://jax.readthedocs.io/en/latest/jax.html). The library can create and manipulate graph neural networks that perform belief update through the diffusion of precision-weighted prediction errors under new observations. The core functions are derivable, JIT-able, and are designed to interface smoothly with other libraries in the JAX ecosystem for Bayesian inference.
 
 * 🎓 [What is a Hierarchical Gaussian Filter?](https://ilabcode.github.io/pyhgf/theory.html)  
 * 📖 [API Documentation](https://ilabcode.github.io/pyhgf/)  
 * ✏️ [Tutorials and examples](https://ilabcode.github.io/pyhgf/tutorials.html)  
 
 ## Getting started
 
 ### Installation
 
-The last official release can be download from PIP:
+The last official release can be downloaded from PIP:
 
 `pip install pyhgf`
 
 The current version under development can be installed from the master branch of the GitHub folder:
 
 `pip install “git+https://github.com/ilabcode/pyhgf.git”`
 
 ### How does it works?
 
 The nodalized Hierarchical Gaussian Filter consists of a network of probabilistic nodes hierarchically structured where each node can inherit its value and volatility sufficient statistics from other parents node. The presentation of a new observation at the lower level of the hierarchy (i.e. the input node) triggers a recursive update of the nodes' belief through the bottom-up propagation of precision-weighted prediction error.
 
 More generally, pyhgf operates on graph neural networks that can be defined and updated through the following variables:
 
 * The node parameters (dictionary) that store each node's parameters (value, precision, learning rates, volatility coupling, ...).
-* The node structure (tuple) that list, for each node, the indexes of the value and volatility parents.
+* The node structure (tuple) that lists, for each node, the indexes of the value and volatility parents.
 * A set of update functions that operate on any of the 3 other variables, starting from a target node.
 * An update sequence (tuple) that define the order in which the update functions are called, and the target node.
 
-![png](./docs/source/images/graph_network.png)
+![png](./docs/source/images/graph_networks.svg)
 
 Value parent and volatility parent are nodes themself. Any node can be a value and/or volatility parent for other nodes and have multiple value and/or volatility parents. A filtering structure consists of nodes embedding other nodes hierarchically. Nodes are parametrized by their sufficient statistic and parents. The transformations between nodes can be linear, non-linear, or any function (thus a *generalization* of the HGF).
 
-The resulting probabilistic network operates as a filter towards new observation. If a decision function (taking the whole model as a parameter) is also defined, behaviours can be triggered accordingly. By comparing those behaviours with actual outcomes, a surprise function can be optimized over the range of parameters of interest.
+The resulting probabilistic network operates as a filter toward new observation. If a decision function (taking the whole model as a parameter) is also defined, behaviors can be triggered accordingly. By comparing those behaviors with actual outcomes, a surprise function can be optimized over the range of parameters of interest.
 
 ### The Hierarchical Gaussian Filter
 
 The Hierarchical Gaussian Filter for binary and continuous inputs as it was described in Mathys et al. (2011, 2014), and later implemented in the Matlab Tapas toolbox (Frässle et al. 2021), can be seen as a special case of this node structure such as:
 
 ![Figure2](./docs/source/images/hgf.png)
 
 The pyhgf package includes pre-implemented standard HGF models that can be used together with other neural network libraries of Bayesian inference tools. It is also possible for the user to build custom network structures that would match specific needs.
 
 ### Model fitting
 
-Here we demonstrate how to fit a two-level binary Hierarchical Gaussian filter. The input time series are binary outcome from Iglesias et al. (2013).
+Here we demonstrate how to fit a two-level binary Hierarchical Gaussian filter. The input time series are the binary outcomes from Iglesias et al. (2013).
 
 ```python
 from pyhgf.model import HGF
 from pyhgf import load_data
 
 # Load time series example data
 timeserie = load_data("binary")
@@ -83,15 +83,15 @@
 `Add 320 new binary observations.`  
 `Model's surprise = 203.29249572753906`
 
 ![png](./docs/source/images/trajectories.png)
 
 # Acknoledgements
 
-This implementation of the Hierarchical Gaussian Filter was largely inspired by the original [Matlab version](https://translationalneuromodeling.github.io/tapas). A Julia implementation of the generalised, nodalised and multilevel HGF is also available [here](https://github.com/ilabcode/HGF.jl).
+This implementation of the Hierarchical Gaussian Filter was largely inspired by the original [Matlab version](https://translationalneuromodeling.github.io/tapas). A Julia implementation of the generalized, nodalised and multilevel HGF is also available [here](https://github.com/ilabcode/HGF.jl).
 
 ## References
 
 1. Mathys, C. (2011). A Bayesian foundation for individual learning under uncertainty. In Frontiers in Human Neuroscience (Vol. 5). Frontiers Media SA. https://doi.org/10.3389/fnhum.2011.00039
 2. Mathys, C. D., Lomakina, E. I., Daunizeau, J., Iglesias, S., Brodersen, K. H., Friston, K. J., & Stephan, K. E. (2014). Uncertainty in perception and the hierarchical Gaussian filter. Frontiers in Human Neuroscience, 8. https://doi.org/10.3389/fnhum.2014.00825
 3. Powers, A. R., Mathys, C., & Corlett, P. R. (2017). Pavlovian conditioning-induced hallucinations result from overweighting of perceptual priors. Science (New York, N.Y.), 357(6351), 596–600. https://doi.org/10.1126/science.aan3458
 4. Frässle, S., Aponte, E. A., Bollmann, S., Brodersen, K. H., Do, C. T., Harrison, O. K., Harrison, S. J., Heinzle, J., Iglesias, S., Kasper, L., Lomakina, E. I., Mathys, C., Müller-Schrader, M., Pereira, I., Petzschner, F. H., Raman, S., Schöbi, D., Toussaint, B., Weber, L. A., … Stephan, K. E. (2021). TAPAS: An Open-Source Software Package for Translational Neuromodeling and Computational Psychiatry. In Frontiers in Psychiatry (Vol. 12). Frontiers Media SA. https://doi.org/10.3389/fpsyt.2021.680811
```

### Comparing `pyhgf-0.0.4/pyhgf/__init__.py` & `pyhgf-0.0.5/pyhgf/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Author: Nicolas Legrand <nicolas.legrand@cas.au.dk>
 
 import pkg_resources  # type: ignore
 from numpy import loadtxt
 
-__version__ = "0.0.4"
+__version__ = "0.0.5"
 
 
 def load_data(dataset: str):
     """Load dataset for continuous or binary HGF.
 
     Parameters
     ----------
```

### Comparing `pyhgf-0.0.4/pyhgf/binary.py` & `pyhgf-0.0.5/pyhgf/binary.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Author: Nicolas Legrand <nicolas.legrand@cas.au.dk>
 
 from functools import partial
 from typing import Dict, Union
 
 import jax.numpy as jnp
-from jax import Array, jit
+from jax import jit
 from jax.lax import cond
 from jax.typing import ArrayLike
 
 from pyhgf.typing import NodeStructure
 
 
 @partial(jit, static_argnames=("node_structure", "node_idx"))
@@ -20,44 +20,50 @@
     **args
 ) -> Dict:
     """Update the value and volatility parents of a binary node.
 
     If the parents have value and/or volatility parents, they will be updated
     recursively.
 
-    Updating the node's parents is a two step process:
+    Updating the node's parents is a two-step process:
         1. Update value parent(s) and their parents (if provided).
         2. Update volatility parent(s) and their parents (if provided).
 
     Then returns the new node tuple `(parameters, value_parents, volatility_parents)`.
 
     Parameters
     ----------
     parameters_structure :
         The structure of nodes' parameters. Each parameter is a dictionary with the
         following parameters: `"pihat", "pi", "muhat", "mu", "nu", "psis", "omega"` for
         continuous nodes.
     .. note::
-        `"psis"` is the value coupling strength. It should have same length than the
+        `"psis"` is the value coupling strength. It should have the same length as the
         volatility parents' indexes. `"kappas"` is the volatility coupling strength.
-        It should have same length than the volatility parents' indexes.
+        It should have the same length as the volatility parents' indexes.
     time_step :
         Interval between the previous time point and the current time point.
     node_idx :
-        Pointer to the node that need to be updated. After continuous update, the
+        Pointer to the node that needs to be updated. After continuous updates, the
         parameters of value and volatility parents (if any) will be different.
     node_structure :
-        Tuple of :py:class:`pyhgf.typing.Indexes` with same length than number of node.
+        Tuple of :py:class:`pyhgf.typing.Indexes` with the same length as node number.
         For each node, the index list value and volatility parents.
 
     Returns
     -------
     parameters_structure :
         The updated node structure.
 
+    References
+    ----------
+    .. [1] Weber, L. A., Waade, P. T., Legrand, N., Møller, A. H., Stephan, K. E., &
+       Mathys, C. (2023). The generalized Hierarchical Gaussian Filter (Version 1).
+       arXiv. https://doi.org/10.48550/ARXIV.2305.10937
+
     """
     # using the current node index, unwrap parameters and parents
     node_parameters = parameters_structure[node_idx]
     value_parents_idx = node_structure[node_idx].value_parents
     volatility_parents_idx = node_structure[node_idx].volatility_parents
 
     # Return here if no parents node are provided
@@ -139,48 +145,54 @@
     time_step: float,
     node_idx: int,
     node_structure: NodeStructure,
     value: float,
 ) -> Dict:
     """Update the input node structure given one observation.
 
-    This function is the entry level of the model fitting. It update the partents of
+    This function is the entry-level of the model fitting. It updates the parents of
     the input node and then call :py:func:`pyhgf.binary.binary_node_update` to update
     the rest of the node structure.
 
     Parameters
     ----------
     value :
         The new observed value.
     time_step :
-        Interval between the previous time point and the current time point.
+        The interval between the previous time point and the current time point.
     parameters_structure :
         The structure of nodes' parameters. Each parameter is a dictionary with the
         following parameters: `"pihat", "pi", "muhat", "mu", "nu", "psis", "omega"` for
         continuous nodes.
     .. note::
-        `"psis"` is the value coupling strength. It should have same length than the
+        `"psis"` is the value coupling strength. It should have the same length as the
         volatility parents' indexes. `"kappas"` is the volatility coupling strength.
-        It should have same length than the volatility parents' indexes.
+        It should have the same length as the volatility parents' indexes.
     node_structure :
-        Tuple of :py:class:`pyhgf.typing.Indexes` with same length than number of node.
+        Tuple of :py:class:`pyhgf.typing.Indexes` with the same length as node number.
         For each node, the index list value and volatility parents.
     node_idx :
-        Pointer to the node that need to be updated. After continuous update, the
+        Pointer to the node that needs to be updated. After continuous updates, the
         parameters of value and volatility parents (if any) will be different.
 
     Returns
     -------
     parameters_structure :
         The updated parameters structure.
 
     See Also
     --------
     update_continuous_parents, update_continuous_input_parents
 
+    References
+    ----------
+    .. [1] Weber, L. A., Waade, P. T., Legrand, N., Møller, A. H., Stephan, K. E., &
+       Mathys, C. (2023). The generalized Hierarchical Gaussian Filter (Version 1).
+       arXiv. https://doi.org/10.48550/ARXIV.2305.10937
+
     """
     # using the current node index, unwrap parameters and parents
     input_node_parameters = parameters_structure[node_idx]
     value_parents_idx = node_structure[node_idx].value_parents
     volatility_parents_idx = node_structure[node_idx].volatility_parents
 
     if (value_parents_idx is None) and (volatility_parents_idx is None):
@@ -206,15 +218,15 @@
         # 1.1 Compute new_muhat from continuous node parent (x2)
 
         # 1.1.1 get rho from the value parent of the binary node (x2)
         driftrate = parameters_structure[va_pa_value_parents_idx[0]]["rho"]
 
         # TODO: this will be decided once we figure out the multi parents/children
         # # 1.1.2 Look at the (optional) va_pa's value parents (x3)
-        # # and update the driftrate accordingly
+        # # and update the drift rate accordingly
         # if va_pa_value_parents[0][1] is not None:
         #     for va_pa_va_pa in va_pa_value_parents[0][1]:
         #         # For each x2's value parents (optional)
         #         _psi = va_pa_value_parents[0][0]["psis"]
         #         _mu = va_pa_va_pa[0]["mu"]
         #         driftrate += _psi * _mu
 
@@ -248,35 +260,35 @@
     parameters_structure[node_idx]["surprise"] = surprise
     parameters_structure[node_idx]["time_step"] = time_step
     parameters_structure[node_idx]["value"] = value
 
     return parameters_structure
 
 
-def gaussian_density(x: ArrayLike, mu: ArrayLike, pi: ArrayLike):
+def gaussian_density(x: ArrayLike, mu: ArrayLike, pi: ArrayLike) -> ArrayLike:
     """Gaussian density as defined by mean and precision."""
     return (
         pi
         / jnp.sqrt(2 * jnp.pi)
         * jnp.exp(jnp.subtract(0, pi) / 2 * (jnp.subtract(x, mu)) ** 2)
     )
 
 
 def sgm(
     x,
     lower_bound: Union[ArrayLike, float] = 0.0,
     upper_bound: Union[ArrayLike, float] = 1.0,
-) -> Array:
+) -> ArrayLike:
     """Logistic sigmoid function."""
     return jnp.subtract(upper_bound, lower_bound) / (1 + jnp.exp(-x)) + lower_bound
 
 
 def binary_surprise(
     x: Union[float, ArrayLike], muhat: Union[float, ArrayLike]
-) -> Array:
+) -> ArrayLike:
     r"""Surprise at a binary outcome.
 
     The surprise ellicited by a binary observation :math:`x` mean :math:`\hat{\mu}`
     and expected probability :math:`\hat{\pi}` is given by:
 
     .. math::
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyhgf-0.0.4/pyhgf/continuous.py` & `pyhgf-0.0.5/pyhgf/continuous.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,53 +14,62 @@
 def continuous_node_update(
     parameters_structure: Dict,
     time_step: float,
     node_idx: int,
     node_structure: NodeStructure,
     **args
 ) -> Dict:
-    """Update the value and volatility parents of a continuous node.
+    """Update the value and volatility parent(s) of a continuous node.
 
-    If the parents have value and/or volatility parents, they will be updated
-    recursively.
+    Updating the node's parents is a two-step process:
+    1. Update value parent(s).
+    2. Update volatility parent(s).
+
+    If a value/volatility parent has multiple children, all the children will update
+    the parent together, therefor this function should only be called once per group
+    of child nodes. The method :py:meth:`pyhgf.model.HGF.get_update_sequence`
+    ensures that this function is only called once all the children have been
+    updated.
 
-    Updating the node's parents is a two step process:
-    1. Update value parent(s) and their parents (if provided).
-    2. Update volatility parent(s) and their parents (if provided).
-
-    Then returns the new node structure.
+    Then returns the structure of the new parameters.
 
     Parameters
     ----------
     parameters_structure :
         The structure of nodes' parameters. Each parameter is a dictionary with the
         following parameters: `"pihat", "pi", "muhat", "mu", "nu", "psis", "omega"` for
         continuous nodes.
     .. note::
-        `"psis"` is the value coupling strength. It should have same length than the
+        `"psis"` is the value coupling strength. It should have the same length as the
         volatility parents' indexes. `"kappas"` is the volatility coupling strength.
-        It should have same length than the volatility parents' indexes.
+        It should have the same length as the volatility parents' indexes.
     time_step :
-        Interval between the previous time point and the current time point.
+        The interval between the previous time point and the current time point.
     node_idx :
-        Pointer to the node that need to be updated. After continuous update, the
+        Pointer to the node that needs to be updated. After continuous updates, the
         parameters of value and volatility parents (if any) will be different.
     node_structure :
-        Tuple of :py:class:`pyhgf.typing.Indexes` with same length than number of node.
+        Tuple of :py:class:`pyhgf.typing.Indexes` with the same length as node number.
         For each node, the index list value and volatility parents.
 
     Returns
     -------
     parameters_structure :
-        The updated node structure.
+        The updated parameters structure.
 
     See Also
     --------
     update_continuous_input_parents, update_binary_input_parents
 
+    References
+    ----------
+    .. [1] Weber, L. A., Waade, P. T., Legrand, N., Møller, A. H., Stephan, K. E., &
+       Mathys, C. (2023). The generalized Hierarchical Gaussian Filter (Version 1).
+       arXiv. https://doi.org/10.48550/ARXIV.2305.10937
+
     """
     # using the current node index, unwrap parameters and parents
     node_parameters = parameters_structure[node_idx]
     value_parents_idx = node_structure[node_idx].value_parents
     volatility_parents_idx = node_structure[node_idx].volatility_parents
 
     # return here if no parents node are provided
@@ -69,59 +78,120 @@
 
     pihat = node_parameters["pihat"]
 
     #######################################
     # Update the continuous value parents #
     #######################################
     if value_parents_idx is not None:
-        vape = node_parameters["mu"] - node_parameters["muhat"]
         psis = node_parameters["psis"]
 
         for va_pa_idx, psi in zip(value_parents_idx, psis):
-            # unpack the current parent's parameters with value and volatility parents
-            va_pa_node_parameters = parameters_structure[va_pa_idx]
-            va_pa_value_parents_idx = node_structure[va_pa_idx].value_parents
-            va_pa_volatility_parents_idx = node_structure[va_pa_idx].volatility_parents
-
-            # Compute new value for nu and pihat
-            logvol = va_pa_node_parameters["omega"]
-
-            # Look at the (optional) va_pa's volatility parents
-            # and update logvol accordingly
-            if va_pa_volatility_parents_idx is not None:
-                for va_pa_vo_pa, k in zip(
-                    va_pa_volatility_parents_idx, va_pa_node_parameters["kappas"]
-                ):
-                    logvol += k * parameters_structure[va_pa_vo_pa]["mu"]
-
-            # Estimate new_nu
-            nu = time_step * jnp.exp(logvol)
-            new_nu = jnp.where(nu > 1e-128, nu, jnp.nan)
-
-            pihat_pa, nu_pa = [1 / (1 / va_pa_node_parameters["pi"] + new_nu), new_nu]
-            pi_pa = pihat_pa + psi**2 * pihat
-
-            # Compute new muhat
-            driftrate = va_pa_node_parameters["rho"]
-
-            # Look at the (optional) va_pa's value parents
-            # and update driftrate accordingly
-            if va_pa_value_parents_idx is not None:
-                for va_pa_va_pa in va_pa_value_parents_idx:
-                    driftrate += psi * va_pa_va_pa["mu"]
-
-            muhat_pa = va_pa_node_parameters["mu"] + time_step * driftrate
-            mu_pa = muhat_pa + psi * pihat / pi_pa * vape
-
-            # Update this parent's parameters
-            parameters_structure[va_pa_idx]["pihat"] = pihat_pa
-            parameters_structure[va_pa_idx]["pi"] = pi_pa
-            parameters_structure[va_pa_idx]["muhat"] = muhat_pa
-            parameters_structure[va_pa_idx]["mu"] = mu_pa
-            parameters_structure[va_pa_idx]["nu"] = nu_pa
+            # if this child is the last one relative to this parent's family, all the
+            # child will update the parent at once, otherwise just pass and wait
+            if node_structure[va_pa_idx].value_children[-1] == node_idx:
+                # unpack the parent's parameters with the value and volatility parents
+                va_pa_node_parameters = parameters_structure[va_pa_idx]
+                va_pa_value_parents_idx = node_structure[va_pa_idx].value_parents
+                va_pa_volatility_parents_idx = node_structure[
+                    va_pa_idx
+                ].volatility_parents
+
+                # Compute new value for nu and pihat
+                logvol = va_pa_node_parameters["omega"]
+
+                # Look at the (optional) va_pa's volatility parents
+                # and update logvol accordingly
+                if va_pa_volatility_parents_idx is not None:
+                    for va_pa_vo_pa, k in zip(
+                        va_pa_volatility_parents_idx, va_pa_node_parameters["kappas"]
+                    ):
+                        logvol += k * parameters_structure[va_pa_vo_pa]["mu"]
+
+                # Estimate new_nu
+                nu = time_step * jnp.exp(logvol)
+                new_nu = jnp.where(nu > 1e-128, nu, jnp.nan)
+
+                pihat_pa, nu_pa = [
+                    1 / (1 / va_pa_node_parameters["pi"] + new_nu),
+                    new_nu,
+                ]
+
+                # gather precision updates from other nodes if the parent has many
+                # children - this part corresponds to the sum of children required for
+                # the multi-children situations
+                pi_children = 0.0
+                for child_idx in node_structure[va_pa_idx].value_children:
+                    # this part finds which psi corresponds to this value parent
+                    # in a JAX-compatible way
+                    psi_child = jnp.where(
+                        jnp.isin(
+                            va_pa_idx,
+                            jnp.array(node_structure[child_idx].value_parents),
+                        ),
+                        jnp.sum(
+                            jnp.equal(
+                                jnp.array(node_structure[child_idx].value_parents),
+                                va_pa_idx,
+                            )
+                            * jnp.array(parameters_structure[child_idx]["psis"])
+                        ),
+                        jnp.nan,
+                    )
+                    pihat_child = parameters_structure[child_idx]["pihat"]
+                    pi_children += psi_child**2 * pihat_child
+
+                pi_pa = pihat_pa + pi_children
+
+                # Compute new muhat
+                driftrate = va_pa_node_parameters["rho"]
+
+                # Look at the (optional) va_pa's value parents
+                # and update drift rate accordingly
+                if va_pa_value_parents_idx is not None:
+                    for va_pa_va_pa in va_pa_value_parents_idx:
+                        driftrate += psi * va_pa_va_pa["mu"]
+
+                muhat_pa = va_pa_node_parameters["mu"] + time_step * driftrate
+
+                # gather PE updates from other nodes if the parent has many children
+                # this part corresponds to the sum of children required for the
+                # multi-children situations
+                pe_children = 0.0
+                for child_idx in node_structure[va_pa_idx].value_children:
+                    # this part finds which psi corresponds to this value parent
+                    # in a JAX-compatible way
+                    psi_child = jnp.where(
+                        jnp.isin(
+                            va_pa_idx,
+                            jnp.array(node_structure[child_idx].value_parents),
+                        ),
+                        jnp.sum(
+                            jnp.equal(
+                                jnp.array(node_structure[child_idx].value_parents),
+                                va_pa_idx,
+                            )
+                            * jnp.array(parameters_structure[child_idx]["psis"])
+                        ),
+                        jnp.nan,
+                    )
+                    vape_child = (
+                        parameters_structure[child_idx]["mu"]
+                        - parameters_structure[child_idx]["muhat"]
+                    )
+                    pihat_child = parameters_structure[child_idx]["pihat"]
+                    pe_children += (psi_child * pihat_child * vape_child) / pi_pa
+
+                mu_pa = muhat_pa + pe_children
+
+                # Update this parent's parameters
+                parameters_structure[va_pa_idx]["pihat"] = pihat_pa
+                parameters_structure[va_pa_idx]["pi"] = pi_pa
+                parameters_structure[va_pa_idx]["muhat"] = muhat_pa
+                parameters_structure[va_pa_idx]["mu"] = mu_pa
+                parameters_structure[va_pa_idx]["nu"] = nu_pa
 
     #############################
     # Update volatility parents #
     #############################
     if volatility_parents_idx is not None:
         nu = node_parameters["nu"]
         kappas = node_parameters["kappas"]
@@ -157,15 +227,15 @@
             )
             pi_pa = jnp.where(pi_pa <= 0, jnp.nan, pi_pa)
 
             # Compute new muhat
             driftrate = vo_pa_node_parameters["rho"]
 
             # Look at the (optional) va_pa's value parents
-            # and update driftrate accordingly
+            # and update drift rate accordingly
             if vo_pa_value_parents_idx is not None:
                 for vo_pa_va_pa in vo_pa_value_parents_idx:
                     driftrate += psi * parameters_structure[vo_pa_va_pa]["mu"]
 
             muhat_pa = vo_pa_node_parameters["mu"] + time_step * driftrate
             mu_pa = muhat_pa + 0.5 * kappa * nu * pihat / pi_pa * vope
 
@@ -185,48 +255,53 @@
     time_step: float,
     node_idx: int,
     node_structure: NodeStructure,
     value: float,
 ) -> Dict:
     """Update the input node structure.
 
-    This function is the entry level of the model fitting. It update the partents of
-    the input node and then call :py:func:`pyhgf.jax.continuous_node_update` recursively
-    to update the rest of the node structure.
+    This function is the entry-level of the structure updates. It updates the parent
+    of the input node.
 
     Parameters
     ----------
     value :
         The new observed value.
     time_step :
-        Interval between the previous time point and the current time point.
+        The interval between the previous time point and the current time point.
     parameters_structure :
         The structure of nodes' parameters. Each parameter is a dictionary with the
         following parameters: `"pihat", "pi", "muhat", "mu", "nu", "psis", "omega"` for
         continuous nodes.
     .. note::
-        `"psis"` is the value coupling strength. It should have same length than the
+        `"psis"` is the value coupling strength. It should have the same length as the
         volatility parents' indexes. `"kappas"` is the volatility coupling strength.
-        It should have same length than the volatility parents' indexes.
+        It should have the same length as the volatility parents' indexes.
     node_structure :
         Tuple of :py:class:`pyhgf.typing.Indexes` with same length than number of node.
         For each node, the index list value and volatility parents.
     node_idx :
-        Pointer to the node that need to be updated. After continuous update, the
+        Pointer to the node that needs to be updated. After continuous updates, the
         parameters of value and volatility parents (if any) will be different.
 
     Returns
     -------
     parameters_structure :
         The updated parameters structure.
 
     See Also
     --------
     continuous_node_update, update_binary_input_parents
 
+    References
+    ----------
+    .. [1] Weber, L. A., Waade, P. T., Legrand, N., Møller, A. H., Stephan, K. E., &
+       Mathys, C. (2023). The generalized Hierarchical Gaussian Filter (Version 1).
+       arXiv. https://doi.org/10.48550/ARXIV.2305.10937
+
     """
     # using the current node index, unwrap parameters and parents
     input_node_parameters = parameters_structure[node_idx]
     value_parents_idx = node_structure[node_idx].value_parents
     volatility_parents_idx = node_structure[node_idx].volatility_parents
 
     lognoise = input_node_parameters["omega"]
@@ -274,19 +349,19 @@
         ]
         pi_va_pa = pihat_va_pa + pihat
 
         # Compute new muhat
         driftrate = va_pa_node_parameters["rho"]
 
         # Look at the (optional) va_pa's value parents
-        # and update driftrate accordingly
+        # and update drift rate accordingly
         if va_pa_value_parents_idx is not None:
             for va_pa_va_pa in va_pa_value_parents_idx:
                 driftrate += (
-                    va_pa_node_parameters["psis"]
+                    va_pa_node_parameters["psis"][0]
                     * parameters_structure[va_pa_va_pa]["mu"]
                 )
 
         muhat_va_pa = va_pa_node_parameters["mu"] + time_step * driftrate
         vape = value - muhat_va_pa
         mu_va_pa = muhat_va_pa + pihat / pi_va_pa * vape
 
@@ -307,15 +382,15 @@
 def gaussian_surprise(
     x: Union[float, ArrayLike],
     muhat: Union[float, ArrayLike],
     pihat: Union[float, ArrayLike],
 ) -> Array:
     r"""Surprise at an outcome under a Gaussian prediction.
 
-    The surprise ellicited by an observation :math:`x` under a Gaussian distribution
+    The surprise elicited by an observation :math:`x` under a Gaussian distribution
     with expected mean :math:`\hat{\mu}` and expected precision :math:`\hat{\pi}` is
     given by:
 
     .. math::
 
        \frac{1}{2} \log(2 \pi) - \log(\hat{\pi}) + \hat{\pi}\sqrt{x - \hat{\mu}}
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyhgf-0.0.4/pyhgf/data/usdchf.dat` & `pyhgf-0.0.5/pyhgf/data/usdchf.dat`

 * *Files identical despite different names*

### Comparing `pyhgf-0.0.4/pyhgf/distribution.py` & `pyhgf-0.0.5/pyhgf/distribution.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,16 +29,16 @@
     mu_3: Union[np.ndarray, ArrayLike, float],
     kappa_1: Union[np.ndarray, ArrayLike, float],
     kappa_2: Union[np.ndarray, ArrayLike, float],
     input_data: List[np.ndarray],
     response_function: Callable,
     model_type: str,
     n_levels: int,
-    response_function_parameters: Tuple = (),
-    time: Optional[List] = None,
+    response_function_parameters: Optional[List[Optional[Tuple]]] = None,
+    time_steps: Optional[List] = None,
 ) -> float:
     r"""Log probability from HGF model(s) given input data and parameter(s).
 
     This function support broadcasting along the first axis:
     - If the input data contains many time series, the function will automatically
     create the corresponding number of HGF models and fit them separately.
     - If a single input data is provided but some parameters have array-like inputs, the
@@ -60,76 +60,78 @@
         The :math:`\omega` parameter, or *evolution rate*, at the second level of the
         HGF. This parameter represents the tonic part of the variance (the part that is
         not inherited from parents nodes).
     omega_3 :
         The :math:`\omega` parameter, or *evolution rate*, at the third level of the
         HGF. This parameter represents the tonic part of the variance (the part that is
         not inherited from parents nodes). The value of this parameter will be ignored
-        when using a 2-levels HGF (`n_levels=2`).
+        when using a two-level HGF (`n_levels=2`).
     omega_input :
         Represent the noise associated with the input observation.
     rho_1 :
         The :math:`\rho` parameter at the first level of the HGF. This parameter
         represents the drift of the random walk.
     rho_2 :
         The :math:`\rho` parameter at the second level of the HGF. This parameter
         represents the drift of the random walk.
     rho_3 :
         The :math:`\rho` parameter at the first level of the HGF. This parameter
         represents the drift of the random walk. The value of this parameter will be
-        ignored when using a 2-levels HGF (`n_levels=2`).
+        ignored when using a two-level HGF (`n_levels=2`).
     pi_1 :
         The :math:`\pi` parameter, or *precision*, at the first level of the HGF.
     pi_2 :
         The :math:`\pi` parameter, or *precision*, at the second level of the HGF.
     pi_3 :
         The :math:`\pi` parameter, or *precision*, at the third level of the HGF. The
-        value of this parameter will be ignored when using a 2-levels HGF
+        value of this parameter will be ignored when using a two-level HGF
         (`n_levels=2`).
     mu_1 :
         The :math:`\mu` parameter, or *mean*, at the first level of the HGF.
     mu_2 :
         The :math:`\mu` parameter, or *mean*, at the second level of the HGF.
     mu_3 :
         The :math:`\mu` parameter, or *mean*, at the third level of the HGF. The value
-        of this parameter will be ignored when using a 2-levels HGF (`n_levels=2`).
+        of this parameter will be ignored when using a two-level HGF (`n_levels=2`).
     kappa_1 :
         The value of the :math:`\\kappa` parameter at the first level of the HGF. Kappa
         represents the phasic part of the variance (the part that is affected by the
-        parents nodes) and will defines the strenght of the connection between the node
+        parent nodes) and will define the strength of the connection between the node
         and the parent node. Often fixed to `1`.
     kappa_2 :
         The value of the :math:`\\kappa` parameter at the second level of the HGF. Kappa
         represents the phasic part of the variance (the part that is affected by the
-        parents nodes) and will defines the strenght of the connection between the node
+        parent nodes) and will define the strength of the connection between the node
         and the parent node. Often fixed to `1`. The value of this parameter will be
-        ignored when using a 2-levels HGF (`n_levels=2`).
+        ignored when using a two-level HGF (`n_levels=2`).
     input_data :
         List of input data. When `n` models should be fitted, the list contains `n` 1d
         Numpy arrays. By default, the associated time vector is the integers vector
         starting at `0`. A different time vector can be passed to the `time` argument.
     response_function :
         The response function to use to compute the model surprise.
     model_type :
         The model type to use (can be "continuous" or "binary").
     n_levels :
         The number of hierarchies in the perceptual model (can be `2` or `3`). If
-        `None`, the nodes hierarchy is not created and might be provided afterward
+        `None`, the nodes hierarchy is not created and might be provided afterwards
         using :py:meth:`pyhgf.model.HGF.add_nodes`.
     response_function_parameters :
-        Additional parameters to the response function.
-    time :
+        A list of tuples with the same length as the number of models. Each tuple
+        contains additional data and parameters that can be accessible to the response
+        functions.
+    time_steps :
         List of 1d Numpy arrays containing the time vectors for each input time series.
-        If one of the list item is `None`, or if `None` is provided instead, the time
-        vector will defaults to integers vector starting at 0.
+        If one of the list items is `None`, or if `None` is provided instead, the time
+        vector will default to the unit vector.
 
     Returns
     -------
     log_prob :
-        The sum of the log-probabilities (or negative surprise).
+        The sum of the log probabilities (or negative surprise).
 
     """
     # number of models
     n = len(input_data)
 
     # Broadcast inputs to an array with length n>=1
     (
@@ -164,20 +166,23 @@
         mu_2,
         mu_3,
         kappa_1,
         kappa_2,
         jnp.zeros(n),
     )
 
+    if response_function_parameters is None:
+        response_function_parameters = [None] * n
+
     # if no time vectors provided, set it to None (will defaults to integers vectors)
     # otherwise check consistency with the input data
-    if time is None:
-        time = [None] * n
+    if time_steps is None:
+        time_steps = [None] * n
     else:
-        assert len(time) == n
+        assert len(time_steps) == n
 
     surprise = 0.0
 
     # Fitting n HGF models to the n datasets
     for i in range(n):
         # Format HGF parameters
         initial_mu: Dict = {
@@ -209,69 +214,71 @@
                 model_type=model_type,
                 n_levels=n_levels,
                 eta0=0.0,
                 eta1=1.0,
                 pihat=jnp.inf,
                 verbose=False,
             )
-            .input_data(input_data=input_data[i], time=time[i])
+            .input_data(input_data=input_data[i], time_steps=time_steps[i])
             .surprise(
                 response_function=response_function,
-                response_function_parameters=response_function_parameters,
+                response_function_parameters=response_function_parameters[i],
             )
         )
 
     # Return the sum of the log probabilities (negative surprise)
     return -surprise
 
 
 class HGFLogpGradOp(Op):
     """Gradient Op for the HGF distribution."""
 
     def __init__(
         self,
         input_data: List = [],
-        time: Optional[List] = None,
+        time_steps: Optional[List] = None,
         model_type: str = "continous",
         n_levels: int = 2,
         response_function: Optional[Callable] = None,
-        response_function_parameters: Tuple = (),
+        response_function_parameters: Optional[List[Optional[Tuple]]] = None,
     ):
         """Initialize function.
 
         Parameters
         ----------
         input_data :
             List of input data. When `n` models should be fitted, the list contains `n`
-            1d Numpy arrays. By default, the associated time vector is the integers
-            vector starting at `0`. A different time vector can be passed to the `time`
-            argument.
-        time :
-            List of 1d Numpy arrays containing the time vectors for each input time
-            series. If one of the list item is `None`, or if `None` is provided instead,
-            the time vector will defaults to integers vector starting at 0.
+            1d Numpy arrays. By default, the associated time_steps vector is the unit
+            vector. A different time vector can be passed to the `time_steps` argument.
+        time_steps :
+            List of 1d Numpy arrays containing the time_steps vectors for each input
+            time series. If one of the list items is `None`, or if `None` is provided
+            instead, the time_steps vector will default to an integers vector starting
+            at 0.
         model_type :
             The model type to use (can be "continuous" or "binary").
         n_levels :
             The number of hierarchies in the perceptual model (can be `2` or `3`). If
             `None`, the nodes hierarchy is not created and might be provided afterward
             using `add_nodes()`.
         response_function :
             The response function to use to compute the model surprise.
         response_function_parameters :
-            Additional parameters to the response function.
+            A list of tuples with the same length as the number of models. Each tuple
+            contains additional data and parameters that can be accessible to the
+            response functions.
 
         """
         self.grad_logp = jit(
             grad(
                 Partial(
                     hgf_logp,
                     n_levels=n_levels,
                     input_data=input_data,
-                    time=time,
+                    time_steps=time_steps,
                     response_function=response_function,
                     model_type=model_type,
                     response_function_parameters=response_function_parameters,
                 ),
                 argnums=[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14],
             )
         )
@@ -374,24 +381,24 @@
     >>> from pyhgf.response import total_gaussian_surprise
 
     Create the data (value and time vectors)
 
     >>> timeserie = load_data("continuous")
 
     We create the PyMC distribution here, specifying the type of model and response
-    function we want to use (i.e simple gaussian surprise).
+    function we want to use (i.e. simple Gaussian surprise).
 
     >>> hgf_logp_op = HGFDistribution(
     >>>     n_levels=2,
     >>>     input_data=timeserie,
     >>>     response_function=total_gaussian_surprise,
     >>> )
 
     Create the PyMC model
-    Here we are fixing all the paramters to arbitrary values and sampling the
+    Here we are fixing all the parameters to arbitrary values and sampling the
     posterior probability density of Omega in the second level, using a normal
     distribution as prior : ω_2 ~ N(-11, 2).
 
     >>> with pm.Model() as model:
     >>>     ω_2 = pm.Normal("ω_2", -11.0, 2)
     >>>     pm.Potential(
     >>>         "hhgf_loglike",
@@ -422,62 +429,64 @@
     ===  =======  =====  =======  =======  =====  =====  ====  ====  =
 
     """
 
     def __init__(
         self,
         input_data: List[np.ndarray] = [],
-        time: Optional[List] = None,
+        time_steps: Optional[List] = None,
         model_type: str = "continuous",
         n_levels: int = 2,
         response_function: Optional[Callable] = None,
-        response_function_parameters: Tuple = (),
+        response_function_parameters: Optional[List[Optional[Tuple]]] = None,
     ):
         """Distribution initialization.
 
         Parameters
         ----------
         input_data :
             List of input data. When `n` models should be fitted, the list contains `n`
-            1d Numpy arrays. By default, the associated time vector is the integers
-            vector starting at `0`. A different time vector can be passed to the `time`
-            argument.
-        time :
-            List of 1d Numpy arrays containing the time vectors for each input time
-            series. If one of the list item is `None`, or if `None` is provided instead,
-            the time vector will defaults to integers vector starting at 0.
+            1d Numpy arrays. By default, the associated time vector is the unit
+            vector starting at `0`. A different time_steps vector can be passed to
+            the `time_steps` argument.
+        time_steps :
+            List of 1d Numpy arrays containing the time_steps vectors for each input
+            time series. If one of the list items is `None`, or if `None` is provided
+            instead, the time vector will default to an integers vector starting at 0.
         model_type :
             The model type to use (can be "continuous" or "binary").
         n_levels :
             The number of hierarchies in the perceptual model (can be `2` or `3`). If
-            `None`, the nodes hierarchy is not created and might be provided afterward
+            `None`, the nodes hierarchy is not created and might be provided afterwards
             using `add_nodes()`.
         response_function :
             The response function to use to compute the model surprise.
         response_function_parameters :
-            Additional parameters to the response function.
+            A list of tuples with the same length as the number of models. Each tuple
+            contains additional data and parameters that can be accessible to the
+            response functions.
 
         """
         # The value function
         self.hgf_logp = jit(
             Partial(
                 hgf_logp,
                 n_levels=n_levels,
                 input_data=input_data,
-                time=time,
+                time_steps=time_steps,
                 response_function=response_function,
                 model_type=model_type,
                 response_function_parameters=response_function_parameters,
             ),
         )
 
         # The gradient function
         self.hgf_logp_grad_op = HGFLogpGradOp(
             input_data=input_data,
-            time=time,
+            time_steps=time_steps,
             model_type=model_type,
             n_levels=n_levels,
             response_function=response_function,
             response_function_parameters=response_function_parameters,
         )
 
     def make_node(
@@ -512,15 +521,15 @@
             pt.as_tensor_variable(pi_3),
             pt.as_tensor_variable(mu_1),
             pt.as_tensor_variable(mu_2),
             pt.as_tensor_variable(mu_3),
             pt.as_tensor_variable(kappa_1),
             pt.as_tensor_variable(kappa_2),
         ]
-        # Define the type of the output returned by the wrapped JAX function
+        # Define the type of output returned by the wrapped JAX function
         outputs = [pt.dscalar()]
         return Apply(self, inputs, outputs)
 
     def perform(self, node, inputs, outputs):
         """Run the function forward."""
         result = self.hgf_logp(*inputs)
         outputs[0][0] = np.asarray(result, dtype=node.outputs[0].dtype)
@@ -541,15 +550,15 @@
             grad_mu_1,
             grad_mu_2,
             grad_mu_3,
             grad_kappa_1,
             grad_kappa_2,
         ) = self.hgf_logp_grad_op(*inputs)
         # If there are inputs for which the gradients will never be needed or cannot
-        # be computed, `aesara.gradient.grad_not_implemented` should  be used as the
+        # be computed, `pytensor.gradient.grad_not_implemented` should  be used as the
         # output gradient for that input.
         output_gradient = output_gradients[0]
         return [
             output_gradient * grad_omega_1,
             output_gradient * grad_omega_2,
             output_gradient * grad_omega_3,
             output_gradient * grad_omega_input,
```

### Comparing `pyhgf-0.0.4/pyhgf/model.py` & `pyhgf-0.0.5/pyhgf/model.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,60 +2,60 @@
 
 from math import log
 from typing import Callable, Dict, List, Optional, Tuple, Union
 
 import jax.numpy as jnp
 import numpy as np
 import pandas as pd
-from jax.lax import scan
+from jax.lax import scan, switch
 from jax.tree_util import Partial
 from jax.typing import ArrayLike
 
 from pyhgf.binary import binary_input_update, binary_node_update
 from pyhgf.continuous import (
     continuous_input_update,
     continuous_node_update,
     gaussian_surprise,
 )
 from pyhgf.plots import plot_correlations, plot_network, plot_trajectories
 from pyhgf.response import first_level_binary_surprise, first_level_gaussian_surprise
-from pyhgf.structure import loop_inputs
-from pyhgf.typing import Indexes, InputIndexes, NodeStructure
+from pyhgf.structure import beliefs_propagation
+from pyhgf.typing import Indexes, InputIndexes, NodeStructure, UpdateSequence
 
 
 class HGF(object):
     r"""The two-level and three-level Hierarchical Gaussian Filters (HGF).
 
-    This class use pre-made nodes structures that corresponds to the most widely used
+    This class uses pre-made nodes structures that correspond to the most widely used
     HGF. The inputs can be continuous or binary.
 
     Attributes
     ----------
     input_nodes_idx :
-        Indexes of the input nodes. Defaults to `(0,)` if the network only has one input
-        node.
+        Indexes of the input nodes with input types
+        :py:class:`pyhgf.typing.InputIndexes`. The default input node is `0` if the
+        network only has one input node.
     model_type :
         The model implemented (can be `"continuous"`, `"binary"` or `"custom"`).
     n_levels :
         The number of hierarchies in the model, including the input vector. Cannot be
         less than 2.
     node_structure :
         A tuple of :py:class:`pyhgf.typing.Indexes` representing the nodes hierarchy.
     node_trajectories :
-        The parameter structure that incluse the consecutive updates at each new
-        observation.
+        The dynamic of the node's beliefs after updating.
     parameters_structure :
         The structure of nodes' parameters. Each parameter is a dictionary with the
         following parameters: `"pihat", "pi", "muhat", "mu", "nu", "psis", "omega"` for
         continuous nodes.
     .. note::
-        `"psis"` is the value coupling strength. It should have same length than the
+        `"psis"` is the value coupling strength. It should have the same length as the
         volatility parents' indexes.
-        `"kappas"` is the volatility coupling strength. It should have same length
-        than the volatility parents' indexes.
+        `"kappas"` is the volatility coupling strength. It should have the same length
+        as the volatility parents' indexes.
     verbose : bool
         Verbosity level.
 
     """
 
     def __init__(
         self,
@@ -95,60 +95,61 @@
         eta0 :
             The first categorical value of the binary node. Defaults to `0.0`. Only
             relevant if `model_type="binary"`.
         eta1 :
             The second categorical value of the binary node. Defaults to `0.0`. Only
             relevant if `model_type="binary"`.
         initial_mu :
-            Dictionary containing the initial values for the :math:`\\mu` parameter at
+            A dictionary containing the initial values for the :math:`\\mu` parameter at
             different levels of the hierarchy. Defaults set to `0.0` at all levels.
         initial_pi :
-            Dictionary containing the initial values for the :math:`\\pi` parameter at
+            A dictionary containing the initial values for the :math:`\\pi` parameter at
             different levels of the hierarchy. Pis values encode the precision of the
-            values at each level (Var = 1/pi) Defaults set to `1.0` at all levels.
+            values at each level (Var = 1/pi) Defaults are set to `1.0` at all levels.
         kappas :
-            Dictionary containing the initial values for the :math:`\\kappa` parameter
+            A dictionary containing the initial values for the :math:`\\kappa` parameter
             at different levels of the hierarchy. Kappa represents the phasic part of
-            the variance (the part that is affected by the parents nodes) and will
-            defines the strenght of the connection between the node and the parent
-            node. Often fixed to `1`. Defaults set to `1` at all levels.
+            the variance (the part that is affected by the parent nodes) and will
+            define the strength of the connection between the node and the parent
+            node. Often fixed to `1`. Defaults are set to `1` at all levels.
         model_type : str
             The model type to use (can be `"continuous"` or `"binary"`).
         n_levels :
             The number of hierarchies in the perceptual model (can be `2` or `3`). If
             `None`, the nodes hierarchy is not created and might be provided afterward
             using `add_nodes()`. Defaults to `2` for a 2-level HGF.
         omega :
-            Dictionary containing the initial values for the :math:`\\omega` parameter
+            A dictionary containing the initial values for the :math:`\\omega` parameter
             at different levels of the hierarchy. :math:`\\omega` represents the tonic
             part of the variance (the part that is not affected by the parent node).
-            Defaults set to `-3.0` at all levels. This parameter is only required for
-            Gaussian Random Walk nodes.
+            Defaults are set to `-3.0` at all levels. This parameter is only required
+            for Gaussian Random Walk nodes.
         omega_input :
             Default value sets to `log(1e-4)`. Represents the noise associated with
             the input.
         pihat :
             The precision of the binary input node. Default to `jnp.inf`. Only relevant
             if `model_type="binary"`.
         rho :
-            Dictionary containing the initial values for the :math:`\\rho` parameter at
-            different levels of the hierarchy. Rho represents the drift of the random
+            A dictionary containing the initial values for the :math:`\\rho` parameter
+            at different levels of the hierarchy. Rho represents the drift of the random
             walk. This parameter is only required for Gaussian Random Walk nodes.
             Defaults set all entries to `0` according to the number of required levels.
         verbose :
-            Verbosity of the methods for model creation and fitting. Defaults to `True`.
+            The verbosity of the methods for model creation and fitting. Defaults to
+            `True`.
 
         """
         self.model_type = model_type
         self.verbose = verbose
         self.n_levels = n_levels
         self.node_structure: NodeStructure
         self.node_trajectories: Dict
         self.parameters_structure: Dict
-        self.input_nodes_idx: Tuple[InputIndexes, ...]
+        self.update_sequence: Optional[UpdateSequence] = None
 
         if model_type in ["continuous", "binary"]:
             if self.verbose:
                 print(
                     (
                         f"Creating a {self.model_type} Hierarchical Gaussian Filter "
                         f"with {self.n_levels} levels."
@@ -212,53 +213,139 @@
 
             # get the update sequence from structure
             self.update_sequence = self.get_update_sequence()
 
     def input_data(
         self,
         input_data: np.ndarray,
-        time: Optional[np.ndarray] = None,
+        time_steps: Optional[np.ndarray] = None,
     ):
         """Add new observations.
 
         Parameters
         ----------
         input_data :
-            The new observations.
-        time :
-            Time vector (optional). If `None`, the time vector will defaults to
-            `np.arange(0, len(input_data))`.
+            2d array of new observations (time x features).
+        time_steps :
+            Time vector (optional). If `None`, the time vector will default to
+            `np.ones(len(input_data))`. This vector is automatically transformed
+            into a time steps vector.
 
         """
         if self.verbose:
-            print((f"Add {len(input_data)} new {self.model_type} observations."))
-        if time is None:
-            time = np.ones(len(input_data), dtype=int)  # time step vector
+            print((f"Adding {len(input_data)} new observations."))
+        if time_steps is None:
+            time_steps = np.ones(len(input_data))  # time steps vector
+        if self.update_sequence is None:
+            self.update_sequence = self.get_update_sequence()
 
         # create the function that will be scaned
         scan_fn = Partial(
-            loop_inputs,
+            beliefs_propagation,
             update_sequence=self.update_sequence,
             node_structure=self.node_structure,
+            input_nodes_idx=self.input_nodes_idx.idx,
         )
 
-        # create the input array (data, time)
-        data = jnp.array([input_data, time], dtype=float).T
+        # concatenate data and time
+        time_steps = time_steps[..., jnp.newaxis]
+        if input_data.ndim == 1:
+            input_data = input_data[..., jnp.newaxis]
+
+        data = jnp.concatenate((input_data, time_steps), dtype=float, axis=1)
 
         # Run the entire for loop
         # this is where the model loop over the input time series
         # at each input the node structure is traversed and beliefs are updated
         # using precision-weighted prediction errors
         _, node_trajectories = scan(scan_fn, self.parameters_structure, data)
 
         # the node structure at each value update
         self.node_trajectories = node_trajectories
 
         return self
 
+    def input_custom_sequence(
+        self,
+        update_branches: Tuple[UpdateSequence],
+        branches_idx: np.array,
+        input_data: np.ndarray,
+        time_steps: Optional[np.ndarray] = None,
+    ):
+        """Add new observations with custom update sequences.
+
+        This method should be used when the update sequence should be adapted to the
+        input data. (e.g. in the case of missing/null observations that should not
+        trigger node update).
+
+        .. note::
+           When the dynamic adaptation of the update sequence is not required, it is
+           recommended to use :py:meth:`pyhgf.model.HGF.input_data` instead as this
+           might result in performance improvement.
+
+        Parameters
+        ----------
+        update_branches :
+            A tuple of UpdateSequence listing the possible update sequences.
+        branches_idx :
+            The branches indexes (integers). Should have the same length as the input
+            data.
+        input_data :
+            2d array of new observations (time x features).
+        time_steps :
+            Time vector (optional). If `None`, the time vector will default to
+            `np.ones(len(input_data))`. This vector is automatically transformed
+            into a time steps vector.
+
+        """
+        if self.verbose:
+            print((f"Adding {len(input_data)} new observations."))
+        if time_steps is None:
+            time_steps = np.ones(len(input_data))  # time steps vector
+
+        # concatenate data and time
+        time_steps = time_steps[..., jnp.newaxis]
+        if input_data.ndim == 1:
+            input_data = input_data[..., jnp.newaxis]
+        data = jnp.concatenate((input_data, time_steps), dtype=float, axis=1)
+
+        # create the update functions that will be scanned
+        branches_fn = [
+            Partial(
+                beliefs_propagation,
+                update_sequence=seq,
+                node_structure=self.node_structure,
+                input_nodes_idx=self.input_nodes_idx.idx,
+            )
+            for seq in update_branches
+        ]
+
+        # create the function that will be scanned
+        def switching_propagation(parameters_structure, scan_input):
+            data, idx = scan_input
+            return switch(idx, branches_fn, parameters_structure, data)
+
+        # wrap the inputs
+        scan_input = data, branches_idx
+
+        # scan over the input data and apply the switching belief propagation functions
+        _, node_trajectories = scan(
+            switching_propagation, self.parameters_structure, scan_input
+        )
+
+        # the node structure at each value update
+        self.node_trajectories = node_trajectories
+
+        # because some of the input node might not have been updated, here we manually
+        # insert the input data to the input node (without triggering updates)
+        for idx, inp in zip(self.input_nodes_idx.idx, range(input_data.shape[1])):
+            self.node_trajectories[idx]["value"] = input_data[:, inp]
+
+        return self
+
     def plot_trajectories(self, **kwargs):
         """Plot the parameters trajectories."""
         return plot_trajectories(hgf=self, **kwargs)
 
     def plot_correlations(self):
         """Plot the heatmap of cross-trajectories correlation."""
         return plot_correlations(hgf=self)
@@ -277,23 +364,23 @@
         The surprise depends on the input data, the model parameters, the response
         function and its additional parameters(optional).
 
         Parameters
         ----------
         response_function :
             The response function to use to compute the model surprise. If `None`
-            (default), return the sum of gaussian surprise if `model_type=="continuous"`
+            (default), return the sum of Gaussian surprise if `model_type=="continuous"`
             or the sum of the binary surprise if `model_type=="binary"`.
         response_function_parameters :
-            Additional parameters to the response function (optional) .
+            Additional parameters to the response function (optional).
 
         Returns
         -------
         surprise :
-            The model surprise given the input data and the response function.
+            The model's surprise given the input data and the response function.
 
         """
         if response_function is None:
             response_function = (
                 first_level_gaussian_surprise
                 if self.model_type == "continuous"
                 else first_level_binary_surprise
@@ -306,50 +393,60 @@
 
     def to_pandas(self) -> pd.DataFrame:
         """Export the nodes trajectories and surprise as a Pandas data frame.
 
         Returns
         -------
         structure_df :
-            Pandas data frame with the time series of the sufficient statistics and
-            surprise of each node in the structure.
+            Pandas data frame with the time series of sufficient statistics and
+            the surprise of each node in the structure.
 
         """
-        # input parameters
+        # get time and time steps from the first input node
         structure_df = pd.DataFrame(
             {
-                "time_steps": self.node_trajectories[0]["time_step"],
-                "time": jnp.cumsum(self.node_trajectories[0]["time_step"]),
-                "observation": self.node_trajectories[0]["value"],
+                "time_steps": self.node_trajectories[self.input_nodes_idx.idx[0]][
+                    "time_step"
+                ],
+                "time": jnp.cumsum(
+                    self.node_trajectories[self.input_nodes_idx.idx[0]]["time_step"]
+                ),
             }
         )
 
+        # add the observations from input nodes
+        for inpt in self.input_nodes_idx.idx:
+            structure_df[f"observation_input_{inpt}"] = self.node_trajectories[inpt][
+                "value"
+            ]
+
         # loop over nodes and store sufficient statistics with surprise
         for i in range(1, len(self.node_trajectories)):
-            structure_df[f"x_{i}_mu"] = self.node_trajectories[i]["mu"]
-            structure_df[f"x_{i}_pi"] = self.node_trajectories[i]["pi"]
-            structure_df[f"x_{i}_muhat"] = self.node_trajectories[i]["muhat"]
-            structure_df[f"x_{i}_pihat"] = self.node_trajectories[i]["pihat"]
-            if (i == 1) & (self.model_type == "continuous"):
-                surprise = gaussian_surprise(
-                    x=self.node_trajectories[0]["value"][1:],
-                    muhat=self.node_trajectories[i]["muhat"][:-1],
-                    pihat=self.node_trajectories[i]["pihat"][:-1],
-                )
-            else:
-                surprise = gaussian_surprise(
-                    x=self.node_trajectories[i]["mu"][1:],
-                    muhat=self.node_trajectories[i]["muhat"][:-1],
-                    pihat=self.node_trajectories[i]["pihat"][:-1],
+            if i not in self.input_nodes_idx.idx:
+                structure_df[f"x_{i}_mu"] = self.node_trajectories[i]["mu"]
+                structure_df[f"x_{i}_pi"] = self.node_trajectories[i]["pi"]
+                structure_df[f"x_{i}_muhat"] = self.node_trajectories[i]["muhat"]
+                structure_df[f"x_{i}_pihat"] = self.node_trajectories[i]["pihat"]
+                if (i == 1) & (self.model_type == "continuous"):
+                    surprise = gaussian_surprise(
+                        x=self.node_trajectories[0]["value"][1:],
+                        muhat=self.node_trajectories[i]["muhat"][:-1],
+                        pihat=self.node_trajectories[i]["pihat"][:-1],
+                    )
+                else:
+                    surprise = gaussian_surprise(
+                        x=self.node_trajectories[i]["mu"][1:],
+                        muhat=self.node_trajectories[i]["muhat"][:-1],
+                        pihat=self.node_trajectories[i]["pihat"][:-1],
+                    )
+                # fill with nans when the model cannot fit
+                surprise = jnp.where(
+                    jnp.isnan(self.node_trajectories[i]["mu"][1:]), jnp.nan, surprise
                 )
-            # fill with nans when the model cannot fit
-            surprise = jnp.where(
-                jnp.isnan(self.node_trajectories[i]["mu"][1:]), jnp.nan, surprise
-            )
-            structure_df[f"x_{i}_surprise"] = np.insert(surprise, 0, np.nan)
+                structure_df[f"x_{i}_surprise"] = np.insert(surprise, 0, np.nan)
 
         # compute the global surprise over all node
         structure_df["surprise"] = structure_df.iloc[
             :, structure_df.columns.str.contains("_surprise")
         ].sum(axis=1, min_count=1)
 
         return structure_df
@@ -397,64 +494,75 @@
                 "surprise": jnp.nan,
                 "time_step": jnp.nan,
                 "value": jnp.nan,
             }
         if input_idx == 0:
             # this is the first node, create the node structure
             self.parameters_structure = {input_idx: input_node_parameters}
-            self.node_structure = (Indexes(None, None),)
-            self.input_nodes_idx = (InputIndexes(input_idx, kind),)
+            self.node_structure = (Indexes(None, None, None, None),)
+            self.input_nodes_idx = InputIndexes((input_idx,), (kind,))
         else:
             # update the node structure
             self.parameters_structure[input_idx] = input_node_parameters
-            self.node_structure += (Indexes(None, None),)
-            self.input_nodes_idx += (InputIndexes(input_idx, kind),)
+            self.node_structure += (Indexes(None, None, None, None),)
+
+            # add information about the new input node in the indexes
+            new_idx = self.input_nodes_idx.idx
+            new_idx += (input_idx,)
+            new_kind = self.input_nodes_idx.kind
+            new_kind += (kind,)
+            self.input_nodes_idx = InputIndexes(new_idx, new_kind)
+
         return self
 
     def add_value_parent(
         self,
         children_idxs: List,
         value_coupling: Union[float, np.ndarray, ArrayLike] = 1.0,
         mu: Union[float, np.ndarray, ArrayLike] = 0.0,
-        mu_hat: Union[float, np.ndarray, ArrayLike] = jnp.nan,
+        mu_hat: Union[float, np.ndarray, ArrayLike] = 0.0,
         pi: Union[float, np.ndarray, ArrayLike] = 1.0,
-        pi_hat: Union[float, np.ndarray, ArrayLike] = jnp.nan,
+        pi_hat: Union[float, np.ndarray, ArrayLike] = 1.0,
         kappas: Optional[Tuple] = None,
         nu: Union[float, np.ndarray, ArrayLike] = jnp.nan,
         psis: Optional[Tuple] = None,
-        omega: Union[float, np.ndarray, ArrayLike] = jnp.nan,
+        omega: Union[float, np.ndarray, ArrayLike] = -4.0,
         rho: Union[float, np.ndarray, ArrayLike] = 0.0,
     ):
-        """Add a value parent to node.
+        """Add a value parent to a given set of nodes.
 
         Parameters
         ----------
         children_idxs :
             The child(s) node index(es).
         value_coupling :
             The value_coupling between the child and parent node. This is will be
             appended to the `psis` parameters in the child node.
         mu :
-            Mean.
+            The mean of the Gaussian distribution.
         mu_hat :
-            Expected mean.
+            The expected mean of the Gaussian distribution for the next observation.
         pi :
-            Precision.
+            The precision of the Gaussian distribution (inverse variance).
         pi_hat :
-            Expected precision.
+            The expected precision of the Gaussian distribution (inverse variance) for
+            the next observation.
         kappas :
-            Phasic part of the variance.
+            The phasic part of the variance (the part that is inherited from volatility
+            parents).
         nu :
             Stochasticity coupling.
         psis :
-            Value coupling.
+            The value coupling with other value parents (defaults to `None` when the
+            node is created as no parents are defined yet).
         omega :
-            Tonic part of the variance.
+            The tonic part of the variance (the variance that is not inherited from
+            volatility parent(s)).
         rho :
-            Drift of the random walk.
+            The drift of the random walk. Defaults to `0.0` (no drift).
 
         """
         # how many nodes in structure
         n_nodes = len(self.node_structure)
         parent_idx = n_nodes  # append a new parent in the structure
 
         # parent's parameter
@@ -467,15 +575,15 @@
             "nu": nu,
             "psis": psis,
             "omega": omega,
             "rho": rho,
         }
 
         # add a new node to connection structure with no parents
-        self.node_structure += (Indexes(None, None),)
+        self.node_structure += (Indexes(None, None, tuple(children_idxs), None),)
 
         # add a new parameters to parameters structure
         self.parameters_structure[parent_idx] = node_parameters
 
         # convert the structure to a list to modify it
         structure_as_list: List[Indexes] = list(self.node_structure)
 
@@ -483,73 +591,82 @@
             # add this node as parent and set value coupling
             if structure_as_list[idx].value_parents is not None:
                 # append new index
                 new_value_parents_idx = structure_as_list[idx].value_parents + (
                     parent_idx,
                 )
                 structure_as_list[idx] = Indexes(
-                    new_value_parents_idx, structure_as_list[idx].volatility_parents
+                    new_value_parents_idx,
+                    structure_as_list[idx].volatility_parents,
+                    structure_as_list[idx].value_children,
+                    structure_as_list[idx].volatility_children,
                 )
                 # set the value coupling strength
                 self.parameters_structure[idx]["psis"] += (value_coupling,)
             else:
                 # append new index
                 new_value_parents_idx = (parent_idx,)
                 structure_as_list[idx] = Indexes(
-                    new_value_parents_idx, structure_as_list[idx].volatility_parents
+                    new_value_parents_idx,
+                    structure_as_list[idx].volatility_parents,
+                    structure_as_list[idx].value_children,
+                    structure_as_list[idx].volatility_children,
                 )
                 # set the value coupling strength
                 self.parameters_structure[idx]["psis"] = (value_coupling,)
 
         # convert the list back to a tuple
         self.node_structure = tuple(structure_as_list)
 
         return self
 
     def add_volatility_parent(
         self,
         children_idxs: List,
         volatility_coupling: Union[float, np.ndarray, ArrayLike] = 1.0,
         mu: Union[float, np.ndarray, ArrayLike] = 0.0,
-        mu_hat: Union[float, np.ndarray, ArrayLike] = jnp.nan,
+        mu_hat: Union[float, np.ndarray, ArrayLike] = 0.0,
         pi: Union[float, np.ndarray, ArrayLike] = 1.0,
-        pi_hat: Union[float, np.ndarray, ArrayLike] = jnp.nan,
+        pi_hat: Union[float, np.ndarray, ArrayLike] = 1.0,
         kappas: Optional[Tuple] = None,
         nu: Union[float, np.ndarray, ArrayLike] = jnp.nan,
         psis: Optional[Tuple] = None,
-        omega: Union[float, np.ndarray, ArrayLike] = jnp.nan,
+        omega: Union[float, np.ndarray, ArrayLike] = -4.0,
         rho: Union[float, np.ndarray, ArrayLike] = 0.0,
     ):
-        """Add a volatility parent to node.
+        """Add a volatility parent to a given set of nodes.
 
         Parameters
         ----------
         children_idxs :
             The child(s) node index(es).
         volatility_coupling :
-            The volatility coupling between the child and parent node. This is will be
+            The volatility coupling between the child and parent node. This will be
             appended to the `kappas` parameters in the child node.
         mu :
-            Mean.
+            The mean of the Gaussian distribution.
         mu_hat :
-            Expected mean.
+            The expected mean of the Gaussian distribution for the next observation.
         pi :
-            Precision.
+            The precision of the Gaussian distribution (inverse variance).
         pi_hat :
-            Expected precision.
+            The expected precision of the Gaussian distribution (inverse variance) for
+            the next observation.
         kappas :
             Phasic part of the variance.
         nu :
             Stochasticity coupling.
         psis :
-            Value coupling.
+            The value coupling with other value parents (defaults to `None` when the
+            node is created as no parents are defined yet).
         omega :
-            Tonic part of the variance.
+            The tonic part of the variance (the variance that is not inherited from
+            volatility parent(s)).
         rho :
-            Drift of the random walk.
+            The drift of the random walk. Defaults to `0.0` (no drift).
 
         """
         # how many nodes in structure
         n_nodes = len(self.node_structure)
         parent_idx = n_nodes  # append a new parent in the structure
 
         # parent's parameter
@@ -561,92 +678,153 @@
             "kappas": kappas,
             "nu": nu,
             "psis": psis,
             "omega": omega,
             "rho": rho,
         }
 
-        # add a new node to connection structure with no parents
-        self.node_structure += (Indexes(None, None),)
+        # add a new node to the connection structure with no parents
+        self.node_structure += (Indexes(None, None, None, tuple(children_idxs)),)
 
-        # add a new parameters to parameters structure
+        # add a new parameter to the parameters structure
         self.parameters_structure[parent_idx] = node_parameters
 
         # convert the structure to a list to modify it
         structure_as_list: List[Indexes] = list(self.node_structure)
 
         for idx in children_idxs:
-            # add this node as parent and set value coupling
+            # add this node as a parent and set value coupling
             if structure_as_list[idx].volatility_parents is not None:
                 # append new index
                 new_volatility_parents_idx = structure_as_list[
                     idx
                 ].volatility_parents + (parent_idx,)
                 structure_as_list[idx] = Indexes(
-                    structure_as_list[idx].value_parents, new_volatility_parents_idx
+                    structure_as_list[idx].value_parents,
+                    new_volatility_parents_idx,
+                    structure_as_list[idx].value_children,
+                    structure_as_list[idx].volatility_children,
                 )
                 # set the value coupling strength
                 self.parameters_structure[idx]["kappas"] += (volatility_coupling,)
             else:
                 # append new index
                 new_volatility_parents_idx = (parent_idx,)
                 structure_as_list[idx] = Indexes(
-                    structure_as_list[idx].value_parents, new_volatility_parents_idx
+                    structure_as_list[idx].value_parents,
+                    new_volatility_parents_idx,
+                    structure_as_list[idx].value_children,
+                    structure_as_list[idx].volatility_children,
                 )
                 # set the value coupling strength
                 self.parameters_structure[idx]["kappas"] = (volatility_coupling,)
 
         # convert the list back to a tuple
         self.node_structure = tuple(structure_as_list)
 
         return self
 
     def get_update_sequence(
-        self, node_idx: int = 0, update_sequence: Tuple = ()
+        self, node_idxs: Tuple[int, ...] = (0,), update_sequence: Tuple = ()
     ) -> Tuple:
-        """Get update sequence from the nodes' connections structure.
+        """Automated creation of the update sequence from the network's structure.
+
+        The function ensures that the following rules apply:
+        1. all children have been updated before propagating to the parent(s) node.
+        2. the update function of an input node is chosen based on the node's type
+        (`"continuous"` or `"binary"`).
+        3. the update function of the parent of an input node is chosen based on the
+        node's type (`"continuous"` or `"binary"`).
 
         Parameters
         ----------
-        node_idx :
-            The index of the current node.
+        node_idxs :
+            The indexes of the current node(s) that should be evaluated. By default
+            (`None`), the function will start with the list of input nodes.
         update_sequence :
-            The current update sequence. This is used for recursive evaluation.
+            The current state of the update sequence (for recursive evaluation).
 
         Returns
         -------
         update_sequence :
             The update sequence.
 
         """
-        # get the parents indexes
-        value_parent_idx = self.node_structure[node_idx].value_parents
-        volatility_parent_idx = self.node_structure[node_idx].volatility_parents
-
-        # select the update function
-        if node_idx == 0:
-            if self.model_type == "binary":
-                update_fn = binary_input_update
-            elif self.model_type == "continuous":
-                update_fn = continuous_input_update
-        elif (node_idx == 1) & (self.model_type == "binary"):
-            update_fn = binary_node_update
-        else:
+        if len(update_sequence) == 0:
+            node_idxs = self.input_nodes_idx.idx
+
+        for node_idx in node_idxs:
+            # if the node has no parent, exit here
+            if (self.node_structure[node_idx].value_parents is None) & (
+                self.node_structure[node_idx].volatility_parents is None
+            ):
+                continue
+
+            # select the update function
+            # --------------------------
+
+            # case 1 - default to a continuous node
             update_fn = continuous_node_update
 
-        # create a new sequence step and add it to the list
-        new_sequence = node_idx, update_fn
-        update_sequence += (new_sequence,)
-
-        # search recursively for the nex update steps
-        if value_parent_idx is not None:
-            for idx in value_parent_idx:
-                update_sequence = self.get_update_sequence(
-                    node_idx=idx, update_sequence=update_sequence
-                )
-        if volatility_parent_idx is not None:
-            for idx in volatility_parent_idx:
-                update_sequence = self.get_update_sequence(
-                    node_idx=idx, update_sequence=update_sequence
-                )
+            # case 2 - this is an input node
+            if node_idx in self.input_nodes_idx.idx:
+                model_kind = [
+                    kind_
+                    for kind_, idx_ in zip(
+                        self.input_nodes_idx.kind, self.input_nodes_idx.idx
+                    )
+                    if idx_ == node_idx
+                ][0]
+                if model_kind == "binary":
+                    update_fn = binary_input_update
+                elif model_kind == "continuous":
+                    update_fn = continuous_input_update
+
+            # case 3 - this is the value parent of at least one binary input node
+            if self.node_structure[node_idx].value_children is not None:
+                value_children_idx = self.node_structure[node_idx].value_children
+                for child_idx in value_children_idx:  # type: ignore
+                    if child_idx in self.input_nodes_idx.idx:
+                        model_kind = [
+                            kind_
+                            for kind_, idx_ in zip(
+                                self.input_nodes_idx.kind, self.input_nodes_idx.idx
+                            )
+                            if idx_ == child_idx
+                        ][0]
+                        if model_kind == "binary":
+                            update_fn = binary_node_update
+
+            # create a new sequence step and add it to the list
+            new_sequence = node_idx, update_fn
+            update_sequence += (new_sequence,)
+
+            # search recursively for the next update steps - make sure that all the
+            # children have been updated before updating the parent(s)
+            # ---------------------------------------------------------------------
+
+            # loop over all possible dependencies (e.g. value, volatility coupling)
+            parents = self.node_structure[node_idx][:2]
+            for parent_types in parents:
+                if parent_types is not None:
+                    for idx in parent_types:
+                        # get the list of all the children in the parent's family
+                        children_idxs = []
+                        if self.node_structure[idx].value_children is not None:
+                            children_idxs.extend(
+                                [*self.node_structure[idx].value_children]
+                            )
+                        if self.node_structure[idx].volatility_children is not None:
+                            children_idxs.extend(
+                                [*self.node_structure[idx].volatility_children]
+                            )
+
+                        if len(children_idxs) > 0:
+                            # only call the update on the parent(s) if the current node
+                            # is the last on the children's list (meaning that all the
+                            # other nodes have been updated)
+                            if children_idxs[-1] == node_idx:
+                                update_sequence = self.get_update_sequence(
+                                    node_idxs=(idx,), update_sequence=update_sequence
+                                )
 
         return update_sequence
```

### Comparing `pyhgf-0.0.4/pyhgf/plots.py` & `pyhgf-0.0.5/pyhgf/plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,27 +26,27 @@
 
     This function will plot :math:`\hat{mu}`, :math:`\¨hat{pi}` (converted into standard
     deviation) and the surprise at each level of the node structure.
 
     Parameters
     ----------
     hgf :
-        Instance of the HGF model.
+        An instance of the HGF model.
     ci :
-        Show the uncertainty aroud the values estimates (standard deviation).
+        Show the uncertainty around the values estimates (standard deviation).
     surprise :
-        If `True` plot each node's surprise together witt the sufficient statistics.
+        If `True` plot each node's surprise together with sufficient statistics.
         If `False`, only the input node's surprise is depicted.
     figsize :
         The width and height of the figure. Defaults to `(18, 9)` for a 2-levels model,
         or to `(18, 12)` for a 3-levels model.
     axs :
-        A list of Matplotlib axes instance where to draw the trajectories. This should
-        correspond to the number of nodes in the structure. Default is `None` (create a
-        new figure).
+        A list of Matplotlib axes instances where to draw the trajectories. This should
+        correspond to the number of nodes in the structure. The default is `None`
+        (create a new figure).
 
     Returns
     -------
     axs :
         The Matplotlib axes instances where to plot the trajectories.
 
     Examples
@@ -117,36 +117,36 @@
         _, axs = plt.subplots(nrows=n_nodes + 1, figsize=figsize, sharex=True)
 
     # input node
     # ----------
     if hgf.model_type == "continuous":
         axs[n_nodes - 1].scatter(
             trajectories_df.time,
-            trajectories_df.observation,
+            trajectories_df.observation_input_0,
             s=3,
             label="Input",
             color="#2a2a2a",
             zorder=10,
             alpha=0.5,
         )
     elif hgf.model_type == "binary":
         axs[n_nodes - 1].scatter(
             x=trajectories_df.time,
-            y=trajectories_df.observation,
+            y=trajectories_df.observation_input_0,
             label="Input",
             color="#4c72b0",
             alpha=0.4,
             edgecolors="k",
             zorder=10,
         )
 
-    # loop over the node idexes
-    # -------------------------
+    # loop over the node indexes
+    # --------------------------
     for i in range(1, n_nodes + 1):
-        # use different colors for each nodes
+        # use different colors for each node
         color = next(palette)
 
         # which ax instance to use
         ax_i = n_nodes - i
 
         # extract the sufficient statistics from the data frame
         mu = trajectories_df[f"x_{i}_muhat"]
@@ -235,27 +235,27 @@
 
 def plot_correlations(hgf: "HGF") -> Axes:
     """Plot the heatmap correlation of the sufficient statistics trajectories.
 
     Parameters
     ----------
     hgf :
-        Instance of the HGF model.
+        An instance of the HGF model.
 
     Returns
     -------
     axs :
-        The Matplotlib ax instance containing the heatmap of parameters trajectories
+        The Matplotlib axe instance containing the heatmap of parameters trajectories
         correlation.
 
     """
     trajectories_df = hgf.to_pandas()
     trajectories_df = pd.concat(
         [
-            trajectories_df[["time", "observation", "surprise"]],
+            trajectories_df[["time", "observation_input_0", "surprise"]],
             trajectories_df.filter(regex="hat"),
         ],
         axis=1,
     )
 
     # rename columns with LateX expressions
     trajectories_df.columns = [
@@ -284,15 +284,15 @@
 
 def plot_network(hgf: "HGF") -> "Source":
     """Visualization of node network using GraphViz.
 
     Parameters
     ----------
     hgf :
-        Instance of the HGF model containing a node structure.
+        An instance of the HGF model containing a node structure.
 
     Notes
     -----
     This function requires [Graphviz](https://github.com/xflr6/graphviz) to be
     installed to work correctly.
 
     """
@@ -307,44 +307,42 @@
         )
 
     graphviz_structure = graphviz.Digraph("hgf-nodes", comment="Nodes structure")
 
     graphviz_structure.attr("node", shape="circle")
 
     # set input nodes
-    list_of_input_idx = []
-    for input_node in hgf.input_nodes_idx:
-        list_of_input_idx.append(input_node.idx)
+    for idx, kind in zip(hgf.input_nodes_idx.idx, hgf.input_nodes_idx.kind):
         graphviz_structure.node(
-            f"x_{input_node.idx}",
-            label=f"{input_node.kind.capitalize()[0]}I - {input_node.idx}",
+            f"x_{idx}",
+            label=f"{kind.capitalize()[0]}I - {idx}",
             style="filled",
             shape="octagon",
         )
 
     # create the rest of nodes
     for i in range(len(hgf.node_structure)):
         # only if node is not an input node
-        if i not in list_of_input_idx:
+        if i not in hgf.input_nodes_idx.idx:
             graphviz_structure.node(f"x_{i}", label=str(i), shape="circle")
 
     # connect value parents
-    for i, idx in enumerate(hgf.node_structure):
-        value_parents = idx.value_parents
+    for i, index in enumerate(hgf.node_structure):
+        value_parents = index.value_parents
 
         if value_parents is not None:
             for value_parents_idx in value_parents:
                 graphviz_structure.edge(
                     f"x_{value_parents_idx}",
                     f"x_{i}",
                 )
 
     # connect volatility parents
-    for i, idx in enumerate(hgf.node_structure):
-        volatility_parents = idx.volatility_parents
+    for i, index in enumerate(hgf.node_structure):
+        volatility_parents = index.volatility_parents
 
         if volatility_parents is not None:
             for volatility_parents_idx in volatility_parents:
                 graphviz_structure.edge(
                     f"x_{volatility_parents_idx}",
                     f"x_{i}",
                     color="gray",
```

### Comparing `pyhgf-0.0.4/pyhgf/response.py` & `pyhgf-0.0.5/pyhgf/response.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,26 +17,26 @@
       The Gaussian surprise at the first level is the default method to compute surprise
       for continuous models. The function returns `jnp.inf` if the model could not fit
       at a given time point.
 
     Parameters
     ----------
     hgf :
-        Instance of the HGF model.
+        An instance of the HGF model.
     response_function_parameters :
         No additional parameters are required to compute the Gaussian surprise.
 
     Returns
     -------
     surprise :
-        The model surprise given the input data.
+        The model's surprise given the input data.
 
     """
     # compute the sum of Gaussian surprise at the first level
-    # the input value at time t is compared to the gaussian prediction at t-1
+    # the input value at time t is compared to the Gaussian prediction at t-1
     surprise = jnp.sum(
         gaussian_surprise(
             x=hgf.node_trajectories[0]["value"][1:],
             muhat=hgf.node_trajectories[1]["muhat"][:-1],
             pihat=hgf.node_trajectories[1]["pihat"][:-1],
         )
     )
@@ -44,54 +44,52 @@
     # Return an infinite surprise if the model could not fit at any point
     return jnp.where(
         jnp.any(jnp.isnan(hgf.node_trajectories[1]["mu"])), jnp.inf, surprise
     )
 
 
 def total_gaussian_surprise(hgf: "HGF", response_function_parameters=None):
-    """Sum of the Gaussian surprise across probabilistic network.
+    """Sum of the Gaussian surprise across the probabilistic network.
 
     .. note::
       The function returns `jnp.inf` if the model could not fit at a given time point.
 
     Parameters
     ----------
     hgf :
-        Instance of the HGF model.
+        An instance of the HGF model.
     response_function_parameters :
         No additional parameters are required to compute the Gaussian surprise.
 
     Returns
     -------
     surprise :
-        The model surprise given the input data.
+        The model's surprise given the input data.
 
     """
-    # compute the sum of Gaussian surprise across every nodes
+    # compute the sum of Gaussian surprise across every node
     surprise = 0.0
 
     # first we start with nodes that are value parents to input nodes
-    input_idx_list = []
     input_parents_list = []
-    for inp in hgf.input_nodes_idx:
-        input_idx_list.append(inp.idx)
-        va_pa = hgf.node_structure[inp.idx].value_parents[0]  # type: ignore
+    for idx in hgf.input_nodes_idx.idx:
+        va_pa = hgf.node_structure[idx].value_parents[0]  # type: ignore
         input_parents_list.append(va_pa)
         surprise += jnp.sum(
             gaussian_surprise(
-                x=hgf.node_trajectories[inp.idx]["value"][1:],
+                x=hgf.node_trajectories[idx]["value"][1:],
                 muhat=hgf.node_trajectories[va_pa]["muhat"][:-1],
                 pihat=hgf.node_trajectories[va_pa]["pihat"][:-1],
             )
         )
 
     # then we do the same for every node that is not an input node
     # and not the parent of an input node
     for i in range(len(hgf.node_structure)):
-        if (i not in input_idx_list) and (i not in input_parents_list):
+        if (i not in hgf.input_nodes_idx.idx) and (i not in input_parents_list):
             surprise += jnp.sum(
                 gaussian_surprise(
                     x=hgf.node_trajectories[i]["mu"][1:],
                     muhat=hgf.node_trajectories[i]["muhat"][:-1],
                     pihat=hgf.node_trajectories[i]["pihat"][:-1],
                 )
             )
@@ -109,22 +107,22 @@
       The binary surprise is the default method to compute surprise when
       `model_type=="binary"`, therefore this method will only return the sum of
       valid time points, and `jnp.inf` if the model could not fit.
 
     Parameters
     ----------
     hgf :
-        Instance of the HGF model.
+        An instance of the HGF model.
     response_function_parameters :
         No additional parameters are required to compute the binary surprise.
 
     Returns
     -------
     surprise :
-        The model surprise given the input data.
+        The model's surprise given the input data.
 
     """
     # Return an infinite surprise if the model cannot fit
     this_surprise = jnp.where(
         jnp.isnan(hgf.node_trajectories[0]["surprise"]),
         jnp.inf,
         hgf.node_trajectories[0]["surprise"],
```

### Comparing `pyhgf-0.0.4/pyhgf.egg-info/PKG-INFO` & `pyhgf-0.0.5/pyhgf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhgf
-Version: 0.0.4
+Version: 0.0.5
 Summary: The generalized, nodalized HGF for predictive coding.
 Author: ILAB
 Author-email: nicolas.legrand@cas.au.dk
 Maintainer: Nicolas Legrand
 Maintainer-email: nicolas.legrand@cas.au.dk
 License: GPL-3.0
 Description-Content-Type: text/markdown
@@ -12,60 +12,60 @@
 
 <img src="docs/source/images/logo.svg" align="center" alt="hgf" VSPACE=30>
 
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit) [![license](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://github.com/ilabcode/pyhgf/blob/master/LICENSE) [![codecov](https://codecov.io/gh/ilabcode/pyhgf/branch/master/graph/badge.svg)](https://codecov.io/gh/ilabcode/pyhgf) [![black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/) [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/) [![pip](https://badge.fury.io/py/pyhgf.svg)](https://badge.fury.io/py/pyhgf)
 
 # The multilevel, generalized and nodalized Hierarchical Gaussian Filter for predictive coding
 
-pyhgf is a Python library that implements the generalized, nodalized and multilevel Hierarchical Gaussian Filters for predictive coding written on top of [JAX](https://jax.readthedocs.io/en/latest/jax.html). The library can create and manipulate graph neural networks that perform beliefs update throught the diffusion of precision-weighted prediction errors under new observations. The core functions are derivable, JIT-able, and are designed to interface smoothly with other libraries in the JAX ecosystem for Bayesian inference.
+pyhgf is a Python library that implements the generalized, nodalized and multilevel Hierarchical Gaussian Filters for predictive coding written on top of [JAX](https://jax.readthedocs.io/en/latest/jax.html). The library can create and manipulate graph neural networks that perform belief update through the diffusion of precision-weighted prediction errors under new observations. The core functions are derivable, JIT-able, and are designed to interface smoothly with other libraries in the JAX ecosystem for Bayesian inference.
 
 * 🎓 [What is a Hierarchical Gaussian Filter?](https://ilabcode.github.io/pyhgf/theory.html)  
 * 📖 [API Documentation](https://ilabcode.github.io/pyhgf/)  
 * ✏️ [Tutorials and examples](https://ilabcode.github.io/pyhgf/tutorials.html)  
 
 ## Getting started
 
 ### Installation
 
-The last official release can be download from PIP:
+The last official release can be downloaded from PIP:
 
 `pip install pyhgf`
 
 The current version under development can be installed from the master branch of the GitHub folder:
 
 `pip install “git+https://github.com/ilabcode/pyhgf.git”`
 
 ### How does it works?
 
 The nodalized Hierarchical Gaussian Filter consists of a network of probabilistic nodes hierarchically structured where each node can inherit its value and volatility sufficient statistics from other parents node. The presentation of a new observation at the lower level of the hierarchy (i.e. the input node) triggers a recursive update of the nodes' belief through the bottom-up propagation of precision-weighted prediction error.
 
 More generally, pyhgf operates on graph neural networks that can be defined and updated through the following variables:
 
 * The node parameters (dictionary) that store each node's parameters (value, precision, learning rates, volatility coupling, ...).
-* The node structure (tuple) that list, for each node, the indexes of the value and volatility parents.
+* The node structure (tuple) that lists, for each node, the indexes of the value and volatility parents.
 * A set of update functions that operate on any of the 3 other variables, starting from a target node.
 * An update sequence (tuple) that define the order in which the update functions are called, and the target node.
 
-![png](./docs/source/images/graph_network.png)
+![png](./docs/source/images/graph_networks.svg)
 
 Value parent and volatility parent are nodes themself. Any node can be a value and/or volatility parent for other nodes and have multiple value and/or volatility parents. A filtering structure consists of nodes embedding other nodes hierarchically. Nodes are parametrized by their sufficient statistic and parents. The transformations between nodes can be linear, non-linear, or any function (thus a *generalization* of the HGF).
 
-The resulting probabilistic network operates as a filter towards new observation. If a decision function (taking the whole model as a parameter) is also defined, behaviours can be triggered accordingly. By comparing those behaviours with actual outcomes, a surprise function can be optimized over the range of parameters of interest.
+The resulting probabilistic network operates as a filter toward new observation. If a decision function (taking the whole model as a parameter) is also defined, behaviors can be triggered accordingly. By comparing those behaviors with actual outcomes, a surprise function can be optimized over the range of parameters of interest.
 
 ### The Hierarchical Gaussian Filter
 
 The Hierarchical Gaussian Filter for binary and continuous inputs as it was described in Mathys et al. (2011, 2014), and later implemented in the Matlab Tapas toolbox (Frässle et al. 2021), can be seen as a special case of this node structure such as:
 
 ![Figure2](./docs/source/images/hgf.png)
 
 The pyhgf package includes pre-implemented standard HGF models that can be used together with other neural network libraries of Bayesian inference tools. It is also possible for the user to build custom network structures that would match specific needs.
 
 ### Model fitting
 
-Here we demonstrate how to fit a two-level binary Hierarchical Gaussian filter. The input time series are binary outcome from Iglesias et al. (2013).
+Here we demonstrate how to fit a two-level binary Hierarchical Gaussian filter. The input time series are the binary outcomes from Iglesias et al. (2013).
 
 ```python
 from pyhgf.model import HGF
 from pyhgf import load_data
 
 # Load time series example data
 timeserie = load_data("binary")
@@ -95,15 +95,15 @@
 `Add 320 new binary observations.`  
 `Model's surprise = 203.29249572753906`
 
 ![png](./docs/source/images/trajectories.png)
 
 # Acknoledgements
 
-This implementation of the Hierarchical Gaussian Filter was largely inspired by the original [Matlab version](https://translationalneuromodeling.github.io/tapas). A Julia implementation of the generalised, nodalised and multilevel HGF is also available [here](https://github.com/ilabcode/HGF.jl).
+This implementation of the Hierarchical Gaussian Filter was largely inspired by the original [Matlab version](https://translationalneuromodeling.github.io/tapas). A Julia implementation of the generalized, nodalised and multilevel HGF is also available [here](https://github.com/ilabcode/HGF.jl).
 
 ## References
 
 1. Mathys, C. (2011). A Bayesian foundation for individual learning under uncertainty. In Frontiers in Human Neuroscience (Vol. 5). Frontiers Media SA. https://doi.org/10.3389/fnhum.2011.00039
 2. Mathys, C. D., Lomakina, E. I., Daunizeau, J., Iglesias, S., Brodersen, K. H., Friston, K. J., & Stephan, K. E. (2014). Uncertainty in perception and the hierarchical Gaussian filter. Frontiers in Human Neuroscience, 8. https://doi.org/10.3389/fnhum.2014.00825
 3. Powers, A. R., Mathys, C., & Corlett, P. R. (2017). Pavlovian conditioning-induced hallucinations result from overweighting of perceptual priors. Science (New York, N.Y.), 357(6351), 596–600. https://doi.org/10.1126/science.aan3458
 4. Frässle, S., Aponte, E. A., Bollmann, S., Brodersen, K. H., Do, C. T., Harrison, O. K., Harrison, S. J., Heinzle, J., Iglesias, S., Kasper, L., Lomakina, E. I., Mathys, C., Müller-Schrader, M., Pereira, I., Petzschner, F. H., Raman, S., Schöbi, D., Toussaint, B., Weber, L. A., … Stephan, K. E. (2021). TAPAS: An Open-Source Software Package for Translational Neuromodeling and Computational Psychiatry. In Frontiers in Psychiatry (Vol. 12). Frontiers Media SA. https://doi.org/10.3389/fpsyt.2021.680811
```

### Comparing `pyhgf-0.0.4/pyhgf.egg-info/SOURCES.txt` & `pyhgf-0.0.5/pyhgf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhgf-0.0.4/setup.py` & `pyhgf-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `pyhgf-0.0.4/tests/test_distribution.py` & `pyhgf-0.0.5/tests/test_distribution.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,36 +8,34 @@
 import numpy as np
 import pymc as pm
 from jax import grad, jit
 from jax.tree_util import Partial
 
 from pyhgf import load_data
 from pyhgf.distribution import HGFDistribution, HGFLogpGradOp, hgf_logp
-from pyhgf.response import first_level_gaussian_surprise, first_level_binary_surprise
+from pyhgf.response import first_level_binary_surprise, first_level_gaussian_surprise
 
 
 class TestDistribution(TestCase):
-
     def test_hgf_logp(self):
-
         ##################
         # Continuous HGF #
         ##################
 
         # Create the data (value and time vectors)
         timeserie = load_data("continuous")
         jax_logp = jit(
             Partial(
                 hgf_logp,
                 n_levels=2,
                 input_data=[timeserie],
                 response_function=first_level_gaussian_surprise,
                 model_type="continuous",
                 response_function_parameters=None,
-                time=None
+                time_steps=None,
             )
         )
 
         logp = jax_logp(
             omega_1=-3.0,
             omega_2=-3.0,
             omega_3=jnp.nan,
@@ -89,15 +87,14 @@
             mu_3=jnp.nan,
             kappa_1=jnp.array(1.0),
             kappa_2=jnp.nan,
         )
         assert jnp.isclose(logp, -215.58821)
 
     def test_grad_logp(self):
-
         ##################
         # Continuous HGF #
         ##################
 
         # Create the data (value and time vectors)
         timeserie = load_data("continuous")
         grad_logp = jit(
@@ -152,15 +149,15 @@
 
         ##############
         # Binary HGF #
         ##############
 
         # Create the data (value and time vectors)
         timeserie = load_data("binary")
-        
+
         grad_logp = jit(
             grad(
                 Partial(
                     hgf_logp,
                     n_levels=2,
                     input_data=[timeserie],
                     response_function=first_level_binary_surprise,
@@ -184,29 +181,29 @@
             pi_3,
             mu_1,
             mu_2,
             mu_3,
             kappa_1,
             kappa_2,
         ) = grad_logp(
-                np.array(0.0),
-                np.array(-2.0),
-                np.array(0.0),
-                np.array(0.0),
-                np.array(0.0),
-                np.array(0.0),
-                np.array(0.0),
-                np.array(0.0),
-                np.array(1e4),
-                np.array(0.0),
-                np.array(0.0),
-                np.array(0.5),
-                np.array(0.0),
-                np.array(1.0),
-                np.array(1.0),
+            np.array(0.0),
+            np.array(-2.0),
+            np.array(0.0),
+            np.array(0.0),
+            np.array(0.0),
+            np.array(0.0),
+            np.array(0.0),
+            np.array(0.0),
+            np.array(1e4),
+            np.array(0.0),
+            np.array(0.0),
+            np.array(0.5),
+            np.array(0.0),
+            np.array(1.0),
+            np.array(1.0),
         )
 
         assert jnp.isclose(omega_2, -3.4070916)
 
     def test_aesara_logp(self):
         """Test the aesara hgf_logp op."""
 
@@ -308,16 +305,15 @@
             pi_2=1e1,
             mu_1=timeserie[0],
             mu_2=0.0,
             kappa_1=1.0,
         )[0].eval()
 
         assert jnp.isclose(omega_1, -6.8397017)
-        
-        
+
         ##############
         # Binary HGF #
         ##############
 
         # Create the data (value and time vectors)
         timeserie = load_data("binary")
 
@@ -358,15 +354,14 @@
             n_levels=2,
             input_data=[timeserie],
             response_function=first_level_gaussian_surprise,
             response_function_parameters=(np.array(1), 1),
         )
 
         with pm.Model() as model:
-
             omega_2 = pm.Uniform("omega_2", -10, 0)
 
             pm.Potential(
                 "hhgf_loglike",
                 hgf_logp_op(
                     omega_1=np.array(0.0),
                     omega_2=omega_2,
@@ -392,15 +387,15 @@
         assert pointslogs["omega_2"] == -1.39
         assert pointslogs["hhgf_loglike"] == 1088.4
 
         with model:
             idata = pm.sample(chains=2, cores=1, tune=1000)
 
         assert -8.5 < az.summary(idata)["mean"].values[0] < -8.0
-        assert az.summary(idata)["r_hat"].values[0] == 1
+        assert az.summary(idata)["r_hat"].values[0] <= 1.02
 
         ##########
         # Binary #
         ##########
 
         # Create the data (value and time vectors)
         timeserie = load_data("binary")
@@ -410,15 +405,14 @@
             model_type="binary",
             input_data=[timeserie],
             response_function=first_level_binary_surprise,
             response_function_parameters=(np.array(1), 1),
         )
 
         with pm.Model() as model:
-
             omega_2 = pm.Normal("omega_2", -11.0, 2)
 
             pm.Potential(
                 "hhgf_loglike",
                 hgf_logp_op(
                     omega_1=np.inf,
                     omega_2=omega_2,
@@ -445,9 +439,10 @@
         assert pointslogs["hhgf_loglike"] == -231.19
 
         with model:
             idata = pm.sample(chains=2, cores=1, tune=1000)
 
         assert -4 < round(az.summary(idata)["mean"].values[0]) < -2
 
+
 if __name__ == "__main__":
     unittest.main(argv=["first-arg-is-ignored"], exit=False)
```

### Comparing `pyhgf-0.0.4/tests/test_model.py` & `pyhgf-0.0.5/tests/test_model.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # Author: Nicolas Legrand <nicolas.legrand@cas.au.dk>
 
 import unittest
 from unittest import TestCase
 
 import jax.numpy as jnp
+import numpy as np
 
 from pyhgf import load_data
 from pyhgf.model import HGF
 from pyhgf.response import total_gaussian_surprise
 
+
 class Testmodel(TestCase):
     def test_HGF(self):
         """Test the model class"""
 
         ##############
         # Continuous #
         ##############
@@ -25,18 +27,20 @@
             model_type="continuous",
             initial_mu={"1": timeserie[0], "2": 0.0},
             initial_pi={"1": 1e4, "2": 1e1},
             omega={"1": -3.0, "2": -3.0},
             rho={"1": 0.0, "2": 0.0},
             kappas={"1": 1.0},
         )
-        
+
         two_level_continuous_hgf.input_data(input_data=timeserie)
 
-        surprise = two_level_continuous_hgf.surprise()  # Sum the surprise for this model
+        surprise = (
+            two_level_continuous_hgf.surprise()
+        )  # Sum the surprise for this model
         assert jnp.isclose(surprise, -676.51306)
         assert len(two_level_continuous_hgf.node_trajectories[1]["mu"]) == 614
 
         # three-level
         # -----------
         three_level_continuous_hgf = HGF(
             n_levels=3,
@@ -61,43 +65,72 @@
         timeseries = load_data("binary")
 
         # two-level
         # ---------
         two_level_binary_hgf = HGF(
             n_levels=2,
             model_type="binary",
-            initial_mu={"1": .0, "2": .5},
-            initial_pi={"1": .0, "2": 1e4},
+            initial_mu={"1": 0.0, "2": 0.5},
+            initial_pi={"1": 0.0, "2": 1e4},
             omega={"1": None, "2": -6.0},
             rho={"1": None, "2": 0.0},
             kappas={"1": None},
             eta0=0.0,
             eta1=1.0,
-            pihat = jnp.inf,
+            pihat=jnp.inf,
         )
 
         # Provide new observations
         two_level_binary_hgf = two_level_binary_hgf.input_data(timeseries)
         surprise = two_level_binary_hgf.surprise()
         assert jnp.isclose(surprise, 215.58821)
 
         # three-level
         # -----------
         three_level_binary_hgf = HGF(
             n_levels=3,
             model_type="binary",
-            initial_mu={"1": .0, "2": .5, "3": 0.},
-            initial_pi={"1": .0, "2": 1e4, "3": 1e1},
+            initial_mu={"1": 0.0, "2": 0.5, "3": 0.0},
+            initial_pi={"1": 0.0, "2": 1e4, "3": 1e1},
             omega={"1": None, "2": -6.0, "3": -2.0},
             rho={"1": None, "2": 0.0, "3": 0.0},
             kappas={"1": None, "2": 1.0},
             eta0=0.0,
             eta1=1.0,
             pihat=jnp.inf,
         )
         three_level_binary_hgf.input_data(input_data=timeseries)
         surprise = three_level_binary_hgf.surprise()
         assert jnp.isclose(surprise, 215.59067)
 
+        ############################
+        # dynamic update sequences #
+        ############################
+
+        three_level_binary_hgf = HGF(
+            n_levels=3,
+            model_type="binary",
+            initial_mu={"1": 0.0, "2": 0.5, "3": 0.0},
+            initial_pi={"1": 0.0, "2": 1e4, "3": 1e1},
+            omega={"1": None, "2": -6.0, "3": -2.0},
+            rho={"1": None, "2": 0.0, "3": 0.0},
+            kappas={"1": None, "2": 1.0},
+            eta0=0.0,
+            eta1=1.0,
+            pihat=jnp.inf,
+        )
+
+        # create a custom update series
+        update_sequence1 = three_level_binary_hgf.get_update_sequence()
+        update_sequence2 = update_sequence1[:2]
+        update_branches = (update_sequence1, update_sequence2)
+        branches_idx = np.random.binomial(n=1, p=0.5, size=len(timeseries))
+
+        three_level_binary_hgf.input_custom_sequence(
+            update_branches=update_branches,
+            branches_idx=branches_idx,
+            input_data=timeseries,
+        )
+
 
 if __name__ == "__main__":
     unittest.main(argv=["first-arg-is-ignored"], exit=False)
```

### Comparing `pyhgf-0.0.4/tests/test_plots.py` & `pyhgf-0.0.5/tests/test_plots.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 import jax.numpy as jnp
 
 from pyhgf import load_data
 from pyhgf.model import HGF
 
 
 class Testplots(TestCase):
-
     def test_plotting_functions(self):
-
         # Read USD-CHF data
         timeserie = load_data("continuous")
 
         ##############
         # Continuous #
         # ------------
 
@@ -66,46 +64,46 @@
 
         # Read binary input
         timeserie = load_data("binary")
 
         two_level_binary_hgf = HGF(
             n_levels=2,
             model_type="binary",
-            initial_mu={"1": .0, "2": .5},
-            initial_pi={"1": .0, "2": 1e4},
+            initial_mu={"1": 0.0, "2": 0.5},
+            initial_pi={"1": 0.0, "2": 1e4},
             omega={"1": None, "2": -6.0},
             rho={"1": None, "2": 0.0},
             kappas={"1": None},
             eta0=0.0,
             eta1=1.0,
-            pihat = jnp.inf,
+            pihat=jnp.inf,
         ).input_data(timeserie)
-        
+
         # plot trajectories
         two_level_binary_hgf.plot_trajectories()
 
         # plot correlations
         two_level_binary_hgf.plot_correlations()
 
         # plot node structures
         two_level_binary_hgf.plot_network()
 
         three_level_binary_hgf = HGF(
             n_levels=3,
             model_type="binary",
-            initial_mu={"1": .0, "2": .5, "3": 0.},
-            initial_pi={"1": .0, "2": 1e4, "3": 1e1},
+            initial_mu={"1": 0.0, "2": 0.5, "3": 0.0},
+            initial_pi={"1": 0.0, "2": 1e4, "3": 1e1},
             omega={"1": None, "2": -6.0, "3": -2.0},
             rho={"1": None, "2": 0.0, "3": 0.0},
             kappas={"1": None, "2": 1.0},
             eta0=0.0,
             eta1=1.0,
-            pihat = jnp.inf,
+            pihat=jnp.inf,
         ).input_data(timeserie)
-        
+
         # plot trajectories
         three_level_binary_hgf.plot_trajectories()
 
         # plot correlations
         three_level_binary_hgf.plot_correlations()
 
         # plot node structures
```

