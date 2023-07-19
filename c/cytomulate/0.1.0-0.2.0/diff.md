# Comparing `tmp/cytomulate-0.1.0.tar.gz` & `tmp/cytomulate-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cytomulate-0.1.0.tar", last modified: Sat Sep 10 20:30:40 2022, max compression
+gzip compressed data, was "cytomulate-0.2.0.tar", last modified: Wed Jul 19 01:30:35 2023, max compression
```

## Comparing `cytomulate-0.1.0.tar` & `cytomulate-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 yuqiuyang   (501) staff       (20)        0 2022-09-10 20:30:40.754904 cytomulate-0.1.0/
--rw-r--r--   0 yuqiuyang   (501) staff       (20)     8023 2022-09-10 20:30:40.754515 cytomulate-0.1.0/PKG-INFO
--rwxr-xr-x   0 yuqiuyang   (501) staff       (20)     6329 2022-09-10 20:21:16.000000 cytomulate-0.1.0/README.md
-drwxr-xr-x   0 yuqiuyang   (501) staff       (20)        0 2022-09-10 20:30:40.748475 cytomulate-0.1.0/cytomulate/
--rwxr-xr-x   0 yuqiuyang   (501) staff       (20)      264 2022-09-10 20:21:16.000000 cytomulate-0.1.0/cytomulate/__init__.py
--rwxr-xr-x   0 yuqiuyang   (501) staff       (20)     7212 2022-08-27 03:06:34.000000 cytomulate-0.1.0/cytomulate/__main__.py
--rw-r--r--   0 yuqiuyang   (501) staff       (20)     5051 2022-05-31 23:19:59.000000 cytomulate-0.1.0/cytomulate/cell_graph_general.py
--rw-r--r--   0 yuqiuyang   (501) staff       (20)     1814 2022-05-31 17:52:16.000000 cytomulate-0.1.0/cytomulate/cell_type_general.py
-drwxr-xr-x   0 yuqiuyang   (501) staff       (20)        0 2022-09-10 20:30:40.751597 cytomulate-0.1.0/cytomulate/creation/
--rw-r--r--   0 yuqiuyang   (501) staff       (20)        0 2022-03-01 17:27:53.000000 cytomulate-0.1.0/cytomulate/creation/__init__.py
--rw-r--r--   0 yuqiuyang   (501) staff       (20)     2527 2022-05-19 03:53:14.000000 cytomulate-0.1.0/cytomulate/creation/cell_graph.py
--rw-r--r--   0 yuqiuyang   (501) staff       (20)     8081 2022-08-27 03:06:34.000000 cytomulate-0.1.0/cytomulate/creation/cell_type.py
--rw-r--r--   0 yuqiuyang   (501) staff       (20)     3723 2022-05-31 23:33:06.000000 cytomulate-0.1.0/cytomulate/creation/cytof_data.py
--rw-r--r--   0 yuqiuyang   (501) staff       (20)    22345 2022-08-27 03:06:34.000000 cytomulate-0.1.0/cytomulate/cytof_data_general.py
-drwxr-xr-x   0 yuqiuyang   (501) staff       (20)        0 2022-09-10 20:30:40.753589 cytomulate-0.1.0/cytomulate/emulation/
--rw-r--r--   0 yuqiuyang   (501) staff       (20)        0 2022-03-01 17:27:53.000000 cytomulate-0.1.0/cytomulate/emulation/__init__.py
--rw-r--r--   0 yuqiuyang   (501) staff       (20)     3448 2022-05-21 21:02:42.000000 cytomulate-0.1.0/cytomulate/emulation/cell_graph.py
--rw-r--r--   0 yuqiuyang   (501) staff       (20)     2727 2022-05-19 03:53:14.000000 cytomulate-0.1.0/cytomulate/emulation/cell_type.py
--rw-r--r--   0 yuqiuyang   (501) staff       (20)     4502 2022-05-31 23:31:38.000000 cytomulate-0.1.0/cytomulate/emulation/cytof_data.py
--rw-r--r--   0 yuqiuyang   (501) staff       (20)     7548 2022-08-27 03:06:34.000000 cytomulate-0.1.0/cytomulate/utilities.py
-drwxr-xr-x   0 yuqiuyang   (501) staff       (20)        0 2022-09-10 20:30:40.750159 cytomulate-0.1.0/cytomulate.egg-info/
--rw-r--r--   0 yuqiuyang   (501) staff       (20)     8023 2022-09-10 20:30:40.000000 cytomulate-0.1.0/cytomulate.egg-info/PKG-INFO
--rw-r--r--   0 yuqiuyang   (501) staff       (20)      625 2022-09-10 20:30:40.000000 cytomulate-0.1.0/cytomulate.egg-info/SOURCES.txt
--rw-r--r--   0 yuqiuyang   (501) staff       (20)        1 2022-09-10 20:30:40.000000 cytomulate-0.1.0/cytomulate.egg-info/dependency_links.txt
--rw-r--r--   0 yuqiuyang   (501) staff       (20)       50 2022-09-10 20:30:40.000000 cytomulate-0.1.0/cytomulate.egg-info/requires.txt
--rw-r--r--   0 yuqiuyang   (501) staff       (20)       11 2022-09-10 20:30:40.000000 cytomulate-0.1.0/cytomulate.egg-info/top_level.txt
--rw-r--r--   0 yuqiuyang   (501) staff       (20)       38 2022-09-10 20:30:40.755014 cytomulate-0.1.0/setup.cfg
--rw-r--r--   0 yuqiuyang   (501) staff       (20)     2451 2022-09-10 20:21:16.000000 cytomulate-0.1.0/setup.py
+drwxr-xr-x   0 yuqiuyang   (501) staff       (20)        0 2023-07-19 01:30:35.833045 cytomulate-0.2.0/
+-rw-r--r--   0 yuqiuyang   (501) staff       (20)     1088 2023-07-13 02:03:31.000000 cytomulate-0.2.0/LICENSE.txt
+-rw-r--r--   0 yuqiuyang   (501) staff       (20)     8000 2023-07-19 01:30:35.832563 cytomulate-0.2.0/PKG-INFO
+-rwxr-xr-x   0 yuqiuyang   (501) staff       (20)     7506 2023-07-19 00:23:23.000000 cytomulate-0.2.0/README.md
+drwxr-xr-x   0 yuqiuyang   (501) staff       (20)        0 2023-07-19 01:30:35.824151 cytomulate-0.2.0/cytomulate/
+-rwxr-xr-x   0 yuqiuyang   (501) staff       (20)      264 2023-07-19 00:23:23.000000 cytomulate-0.2.0/cytomulate/__init__.py
+-rwxr-xr-x   0 yuqiuyang   (501) staff       (20)     7212 2022-08-27 03:06:34.000000 cytomulate-0.2.0/cytomulate/__main__.py
+-rw-r--r--   0 yuqiuyang   (501) staff       (20)     5123 2023-07-13 02:03:31.000000 cytomulate-0.2.0/cytomulate/cell_graph_general.py
+-rw-r--r--   0 yuqiuyang   (501) staff       (20)     2695 2023-07-19 00:23:23.000000 cytomulate-0.2.0/cytomulate/cell_type_general.py
+drwxr-xr-x   0 yuqiuyang   (501) staff       (20)        0 2023-07-19 01:30:35.830046 cytomulate-0.2.0/cytomulate/creation/
+-rw-r--r--   0 yuqiuyang   (501) staff       (20)        0 2022-03-01 17:27:53.000000 cytomulate-0.2.0/cytomulate/creation/__init__.py
+-rw-r--r--   0 yuqiuyang   (501) staff       (20)     2527 2022-05-19 03:53:14.000000 cytomulate-0.2.0/cytomulate/creation/cell_graph.py
+-rw-r--r--   0 yuqiuyang   (501) staff       (20)     8081 2022-08-27 03:06:34.000000 cytomulate-0.2.0/cytomulate/creation/cell_type.py
+-rw-r--r--   0 yuqiuyang   (501) staff       (20)     5271 2023-07-13 02:03:31.000000 cytomulate-0.2.0/cytomulate/creation/cytof_data.py
+-rw-r--r--   0 yuqiuyang   (501) staff       (20)    23402 2023-07-13 02:03:31.000000 cytomulate-0.2.0/cytomulate/cytof_data_general.py
+drwxr-xr-x   0 yuqiuyang   (501) staff       (20)        0 2023-07-19 01:30:35.832025 cytomulate-0.2.0/cytomulate/emulation/
+-rw-r--r--   0 yuqiuyang   (501) staff       (20)        0 2022-03-01 17:27:53.000000 cytomulate-0.2.0/cytomulate/emulation/__init__.py
+-rw-r--r--   0 yuqiuyang   (501) staff       (20)     3448 2022-05-21 21:02:42.000000 cytomulate-0.2.0/cytomulate/emulation/cell_graph.py
+-rw-r--r--   0 yuqiuyang   (501) staff       (20)     2853 2023-07-19 00:23:23.000000 cytomulate-0.2.0/cytomulate/emulation/cell_type.py
+-rw-r--r--   0 yuqiuyang   (501) staff       (20)     6852 2023-07-13 02:03:31.000000 cytomulate-0.2.0/cytomulate/emulation/cytof_data.py
+-rw-r--r--   0 yuqiuyang   (501) staff       (20)     9229 2023-07-19 00:23:23.000000 cytomulate-0.2.0/cytomulate/utilities.py
+drwxr-xr-x   0 yuqiuyang   (501) staff       (20)        0 2023-07-19 01:30:35.827770 cytomulate-0.2.0/cytomulate.egg-info/
+-rw-r--r--   0 yuqiuyang   (501) staff       (20)     8000 2023-07-19 01:30:35.000000 cytomulate-0.2.0/cytomulate.egg-info/PKG-INFO
+-rw-r--r--   0 yuqiuyang   (501) staff       (20)      637 2023-07-19 01:30:35.000000 cytomulate-0.2.0/cytomulate.egg-info/SOURCES.txt
+-rw-r--r--   0 yuqiuyang   (501) staff       (20)        1 2023-07-19 01:30:35.000000 cytomulate-0.2.0/cytomulate.egg-info/dependency_links.txt
+-rw-r--r--   0 yuqiuyang   (501) staff       (20)       50 2023-07-19 01:30:35.000000 cytomulate-0.2.0/cytomulate.egg-info/requires.txt
+-rw-r--r--   0 yuqiuyang   (501) staff       (20)       11 2023-07-19 01:30:35.000000 cytomulate-0.2.0/cytomulate.egg-info/top_level.txt
+-rw-r--r--   0 yuqiuyang   (501) staff       (20)       38 2023-07-19 01:30:35.833196 cytomulate-0.2.0/setup.cfg
+-rw-r--r--   0 yuqiuyang   (501) staff       (20)     2451 2023-07-19 00:23:23.000000 cytomulate-0.2.0/setup.py
```

### Comparing `cytomulate-0.1.0/PKG-INFO` & `cytomulate-0.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,160 +1,175 @@
 Metadata-Version: 2.1
 Name: cytomulate
-Version: 0.1.0
+Version: 0.2.0
 Summary: Accurate and Efficient Simulation of CyTOF data
-Home-page: UNKNOWN
 Author: Yuqiu Yang, Kevin Wang, Tao Wang, Sherry Wang
 Author-email: yuqiuy@smu.edu, kevinwang@smu.edu, Tao.Wang@UTSouthwestern.edu, swang@smu.edu
-License: UNKNOWN
-Description: ![Logo](/assets/cytomulate.jpg)
-        
-        # cytomulate
-        > A simulation package for Cytometry by Time-of-Flight (CyTOF)
-        
-        [![forthebadge](https://forthebadge.com/images/badges/open-source.svg)](https://forthebadge.com)
-        [![forthebadge](https://forthebadge.com/images/badges/made-with-python.svg)](https://forthebadge.com)
-        
-        | Branch | Release | CI/CD | Documentation | Code Coverage |
-        | --- | --- | --- | --- | --- |
-        | main | ![Badge1](https://img.shields.io/badge/Version-v0.1.0-success) | ![Tests](https://github.com/kevin931/cytomulate/actions/workflows/ci.yml/badge.svg?branch=main) | [![Documentation Status](https://readthedocs.org/projects/cytomulate/badge/?version=dev)](https://cytomulate.readthedocs.io/en/main/?badge=main) |  [![codecov](https://codecov.io/gh/kevin931/cytomulate/branch/dev/graph/badge.svg?token=F5H0QTXGMR)](https://codecov.io/gh/kevin931/cytomulate) |
-        | dev | ![Badge1](https://img.shields.io/badge/Version-v0.1.0-success) |![Tests](https://github.com/kevin931/cytomulate/actions/workflows/ci.yml/badge.svg?branch=dev) | [![Documentation Status](https://readthedocs.org/projects/cytomulate/badge/?version=dev)](https://cytomulate.readthedocs.io/en/dev/?badge=dev) | [![codecov](https://codecov.io/gh/kevin931/cytomulate/branch/dev/graph/badge.svg?token=F5H0QTXGMR)](https://codecov.io/gh/kevin931/cytomulate) |
-        
-        
-        ## Installation
-        
-        You can easily install ``cytomulate`` from either ``PyPI`` or ``conda``. For the former, use the following command:
-        
-        ```shell
-        pip install cytomulate
-        
-        ```
-        
-        Or if you are using a conda environment, you can use the following command:
-        
-        ```shell
-        conda install -c normalizingflow cytomulate
-        
-        ```
-        If you wish to use ``PyCytoData``, you can install separately with more instructions [here](https://cytomulate.readthedocs.io/en/dev/installation.html).
-        
-        ## Examples
-        
-        We have two modes: **Creation Mode** and **Emulation Mode**. The former is probabilistic-model based simulation without the need of datasets; the latter is based on existing datasets to match as much of the existing features as possible. Here, we give two quick examples of how they work.
-        
-        
-        ### Creation Mode
-        
-        To create your datasets, you can run the following:
-        
-        ```python
-        >>> from cytomulate import CreationCytofData
-        >>> cytof_data = CreationCytofData()
-        >>> cytof_data.initialize_cell_types()
-        >>> expression_matrices, labels, _, _ = cytof_data.sample(n_samples = 1000)
-        ```
-        The ``expression_matrices`` is a dictionary that contains the expression matrix from each sample. Correspondingly, ``labels`` is a dictionary that contains their cell types.
-        
-        
-        ### Emulation Mode
-        
-        This is a little bit more involved because we need existing data! If you already have your data, congratulations, you are good to go! For this demonstration, we use ``PyCytoData`` to load some example datasets instead (Of course, you will need to install [PyCytoData](https://pycytodata.readthedocs.io/en/latest/index.html) first if you wish to use it):
-        
-        ```python
-        >>> from cytomulate import EmulationCytoData
-        >>> from PyCytoData import DataLoader
-        
-        >>> exprs = DataLoader.load_dataset(dataset="levine13")
-        >>> exprs.preprocess(arcsinh=True)
-        >>> cytof_data = EmulationCytofData()
-        >>> cytof_data.initialize_cell_types(expression_matrix=exprs.expression_matrix,
-        ...                                  labels=exprs.cell_types)
-        >>> expression_matrices, labels, _, _ = cytof_data.sample(n_samples = 1000)
-        ```
-        This is it!
-        
-        ### Working with PyCytoData
-        
-        ![PyCytoData](/assets/pycytodata.jpg)
-        
-        We're fully compatible with ``PyCytoData``! As you've seen above, you can use ``PyCytoData`` to download datasets! If you're familiar with that interface and in love with its easy workflow, you can have ``cytomulate`` output a ``PyCytoData`` object as well:
-        
-        ```python
-        >>> from cytomulate import CreationCytofData
-        >>> cytof_data = CreationCytofData()
-        >>> cytof_data.initialize_cell_types()
-        >>> simulation_data = cytof_data.sample_to_pycytodata(n_samples = 1000)
-        ```
-        This will allow you to use all the downstream capabilities of ``PyCytoData``.
-        
-        ### Command-Line Interface (CLI)
-        
-        If you prefer to use cytomulate from the command-line, you've got that option as well! One **caveat** is that this mode requires ``PyCytoData`` to be installed. To run the Creation Mode, you can do:
-        
-        ```shell
-        python -m cytomulate \
-        	--creation \
-        	--n_cells 1000 \
-        	-o <your_dir_here>
-        ```
-        
-        To run the emulation mode, you can run the following:
-        
-        ```shell
-        python -m cytomulate \
-        	--emulation \
-        	--n_cells 1000 \
-        	-o <your_dir_here> \
-        	--exprs <you_path_to_exprssion_matrix> \
-        	--cell_types <you_path_to_cell_types>
-        ```
-        Of course, we have much more customization options! For more details, read our [tutorial here](https://cytomulate.readthedocs.io/en/dev/tutorial/cli.html).
-        
-        ## Documentation
-        
-        For more detailed documentation on ``cytomulate``, please visit our [website](https://cytomulate.readthedocs.io/)! You will find detailed tutorials,
-        guidelines, development guides, etc.
-        
-        Our documentation is built automatically on the cloud! If you wish to build locally, check our detailed guide [here](https://cytomulate.readthedocs.io/en/latest/change/build.html)!
-        
-        ## Latest Release: v0.1.0
-        
-        Our **FIRST OFFICIAL RELEASE** is here! From now on, all our releases will be supported with our standard support cycle. Here you will find our release notes.
-        
-        ### Changes and New Features
-        
-        - Added Command-Line Interface with support for complex simulations
-        - Improved docstrings
-        - Improved documentations with tutorials
-        
-        ### From Pre-release
-        
-        These are listed for documetation reasons for the first official release.
-        
-        - Support for ``Emulation Mode`` and ``Creation Mode``
-        - Support for complex simulations
-        - Availability on ``PyPI`` and ``conda``
-        
-        
-        ## References
-        
-        If you are cytomulating in your workflow, citing [our paper](https://doi.org/10.1101/2022.06.14.496200) is appreciated:
-        
-        ```
-        @article {Yang2022.06.14.496200,
-        	author = {Yang, Yuqiu and Wang, Kaiwen and Lu, Zeyu and Wang, Tao and Wang, Xinlei},
-        	title = {Cytomulate: Accurate and Efficient Simulation of CyTOF data},
-        	elocation-id = {2022.06.14.496200},
-        	year = {2022},
-        	doi = {10.1101/2022.06.14.496200},
-        	publisher = {Cold Spring Harbor Laboratory},
-        	URL = {https://www.biorxiv.org/content/early/2022/06/16/2022.06.14.496200},
-        	eprint = {https://www.biorxiv.org/content/early/2022/06/16/2022.06.14.496200.full.pdf},
-        	journal = {bioRxiv}
-        }
-        ```
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+![Logo](/assets/cytomulate.jpg)
+
+# cytomulate
+> A simulation package for Cytometry by Time-of-Flight (CyTOF)
+
+[![forthebadge](https://forthebadge.com/images/badges/open-source.svg)](https://forthebadge.com)
+[![forthebadge](https://forthebadge.com/images/badges/made-with-python.svg)](https://forthebadge.com)
+
+| Branch | Release | CI/CD | Documentation | Code Coverage |
+| --- | --- | --- | --- | --- |
+| main | ![Badge1](https://img.shields.io/badge/Version-v0.2.0-success) | ![Tests](https://github.com/kevin931/cytomulate/actions/workflows/ci.yml/badge.svg?branch=main) | [![Documentation Status](https://readthedocs.org/projects/cytomulate/badge/?version=dev)](https://cytomulate.readthedocs.io/en/main/?badge=main) |  [![codecov](https://codecov.io/gh/kevin931/cytomulate/branch/dev/graph/badge.svg?token=F5H0QTXGMR)](https://codecov.io/gh/kevin931/cytomulate) |
+| dev | ![Badge1](https://img.shields.io/badge/Version-v0.2.0-success) |![Tests](https://github.com/kevin931/cytomulate/actions/workflows/ci.yml/badge.svg?branch=dev) | [![Documentation Status](https://readthedocs.org/projects/cytomulate/badge/?version=dev)](https://cytomulate.readthedocs.io/en/dev/?badge=dev) | [![codecov](https://codecov.io/gh/kevin931/cytomulate/branch/dev/graph/badge.svg?token=F5H0QTXGMR)](https://codecov.io/gh/kevin931/cytomulate) |
+
+
+## Installation
+
+You can easily install ``cytomulate`` from either ``PyPI`` or ``conda``. For the former, use the following command:
+
+```shell
+pip install cytomulate
+
+```
+
+Or if you are using a conda environment, you can use the following command:
+
+```shell
+conda install -c normalizingflow cytomulate
+
+```
+If you wish to use ``PyCytoData``, you can install separately with more instructions [here](https://cytomulate.readthedocs.io/en/dev/installation.html).
+
+### Dependencies
+
+Good news: we didn't have to write `cytomulate` from scratch in assembly language! This means that we will need dependencies to install it. Below is a list of packages that you will need:
+
+- numpy
+- scipy
+- scikit-learn
+- networkx
+- matplotlib
+- tqdm
+
+Most of these are pretty standard! And even better news: the installation instructions should automatically handle all the dependency issues. If you have a problem with installation, let us know and we're happy to help!
+
+While the above are all core dependencies, we highly highly highly highly highly recommend `PyCytoData` as well! You can get all the benefits of an integrated pipeline! But of course, for those of you who don't fancy more dependencies, we understand as well!
+
+
+## Examples
+
+We have two modes: **Creation Mode** and **Emulation Mode**. The former is probabilistic-model based simulation without the need of datasets; the latter is based on existing datasets to match as much of the existing features as possible. Here, we give two quick examples of how they work.
+
+
+### Creation Mode
+
+To create your datasets, you can run the following:
+
+```python
+>>> from cytomulate import CreationCytofData
+>>> cytof_data = CreationCytofData()
+>>> cytof_data.initialize_cell_types()
+>>> expression_matrices, labels, _, _ = cytof_data.sample(n_samples = 1000)
+```
+The ``expression_matrices`` is a dictionary that contains the expression matrix from each sample. Correspondingly, ``labels`` is a dictionary that contains their cell types.
+
+
+### Emulation Mode
+
+This is a little bit more involved because we need existing data! If you already have your data, congratulations, you are good to go! For this demonstration, we use ``PyCytoData`` to load some example datasets instead (Of course, you will need to install [PyCytoData](https://pycytodata.readthedocs.io/en/latest/index.html) first if you wish to use it):
+
+```python
+>>> from cytomulate import EmulationCytoData
+>>> from PyCytoData import DataLoader
+
+>>> exprs = DataLoader.load_dataset(dataset="levine13")
+>>> exprs.preprocess(arcsinh=True)
+>>> cytof_data = EmulationCytofData()
+>>> cytof_data.initialize_cell_types(expression_matrix=exprs.expression_matrix,
+...                                  labels=exprs.cell_types)
+>>> expression_matrices, labels, _, _ = cytof_data.sample(n_samples = 1000)
+```
+This is it!
+
+### Working with PyCytoData
+
+![PyCytoData](/assets/pycytodata.jpg)
+
+We're fully compatible with ``PyCytoData``! As you've seen above, you can use ``PyCytoData`` to download datasets! If you're familiar with that interface and in love with its easy workflow, you can have ``cytomulate`` output a ``PyCytoData`` object as well:
+
+```python
+>>> from cytomulate import CreationCytofData
+>>> cytof_data = CreationCytofData()
+>>> cytof_data.initialize_cell_types()
+>>> simulation_data = cytof_data.sample_to_pycytodata(n_samples = 1000)
+```
+This will allow you to use all the downstream capabilities of ``PyCytoData``.
+
+### Command-Line Interface (CLI)
+
+If you prefer to use cytomulate from the command-line, you've got that option as well! One **caveat** is that this mode requires ``PyCytoData`` to be installed. To run the Creation Mode, you can do:
+
+```shell
+python -m cytomulate \
+	--creation \
+	--n_cells 1000 \
+	-o <your_dir_here>
+```
+
+To run the emulation mode, you can run the following:
+
+```shell
+python -m cytomulate \
+	--emulation \
+	--n_cells 1000 \
+	-o <your_dir_here> \
+	--exprs <you_path_to_exprssion_matrix> \
+	--cell_types <you_path_to_cell_types>
+```
+Of course, we have much more customization options! For more details, read our [tutorial here](https://cytomulate.readthedocs.io/en/dev/tutorial/cli.html).
+
+## Documentation
+
+For more detailed documentation on ``cytomulate``, please visit our [website](https://cytomulate.readthedocs.io/)! You will find detailed tutorials,
+guidelines, development guides, etc.
+
+Our documentation is built automatically on the cloud! If you wish to build locally, check our detailed guide [here](https://cytomulate.readthedocs.io/en/latest/change/build.html)!
+
+## Latest Release: v0.2.0
+
+Welcome to Cytomulate v0.2.0! Hooray! We are not only bringing documentation enhancements, but we
+are also introducing a new feature for more accurate simulations!
+
+### Changes and New Features
+- The `utilities.univariate_noise_model()` method:
+    - Added `half_normal` option to the `noise_distribution` parameter
+    - Changed the default `noise_distribution` to `uniform` (This is a **breaking change** because of the benefits to simulated results).
+    - A warning is given when no user-specified `noise_distribution` is supplied to warn the breaking change
+- Added the `utilities.estimate_noise_model()` method to estimate the noise present in the data
+- Added a built-in estimation procedure to match the amount of zeroes observed in the dataset
+
+### Improvements
+- Added 4 more detailed tutorials on `our documentation website <https://cytomulate.readthedocs.io>`_
+- Improved docstrings with more details on key parameters
+- Updated the lastest references and links
+
+
+## References
+
+If you are cytomulating in your workflow, citing [our paper](https://doi.org/10.1101/2022.06.14.496200) is appreciated:
+
+```
+@article {Yang2022.06.14.496200,
+	author = {Yang, Yuqiu and Wang, Kaiwen and Lu, Zeyu and Wang, Tao and Wang, Xinlei},
+	title = {Cytomulate: Accurate and Efficient Simulation of CyTOF data},
+	elocation-id = {2022.06.14.496200},
+	year = {2022},
+	doi = {10.1101/2022.06.14.496200},
+	publisher = {Cold Spring Harbor Laboratory},
+	URL = {https://www.biorxiv.org/content/early/2022/06/16/2022.06.14.496200},
+	eprint = {https://www.biorxiv.org/content/early/2022/06/16/2022.06.14.496200.full.pdf},
+	journal = {bioRxiv}
+}
+```
```

### Comparing `cytomulate-0.1.0/README.md` & `cytomulate-0.2.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 > A simulation package for Cytometry by Time-of-Flight (CyTOF)
 
 [![forthebadge](https://forthebadge.com/images/badges/open-source.svg)](https://forthebadge.com)
 [![forthebadge](https://forthebadge.com/images/badges/made-with-python.svg)](https://forthebadge.com)
 
 | Branch | Release | CI/CD | Documentation | Code Coverage |
 | --- | --- | --- | --- | --- |
-| main | ![Badge1](https://img.shields.io/badge/Version-v0.1.0-success) | ![Tests](https://github.com/kevin931/cytomulate/actions/workflows/ci.yml/badge.svg?branch=main) | [![Documentation Status](https://readthedocs.org/projects/cytomulate/badge/?version=dev)](https://cytomulate.readthedocs.io/en/main/?badge=main) |  [![codecov](https://codecov.io/gh/kevin931/cytomulate/branch/dev/graph/badge.svg?token=F5H0QTXGMR)](https://codecov.io/gh/kevin931/cytomulate) |
-| dev | ![Badge1](https://img.shields.io/badge/Version-v0.1.0-success) |![Tests](https://github.com/kevin931/cytomulate/actions/workflows/ci.yml/badge.svg?branch=dev) | [![Documentation Status](https://readthedocs.org/projects/cytomulate/badge/?version=dev)](https://cytomulate.readthedocs.io/en/dev/?badge=dev) | [![codecov](https://codecov.io/gh/kevin931/cytomulate/branch/dev/graph/badge.svg?token=F5H0QTXGMR)](https://codecov.io/gh/kevin931/cytomulate) |
+| main | ![Badge1](https://img.shields.io/badge/Version-v0.2.0-success) | ![Tests](https://github.com/kevin931/cytomulate/actions/workflows/ci.yml/badge.svg?branch=main) | [![Documentation Status](https://readthedocs.org/projects/cytomulate/badge/?version=dev)](https://cytomulate.readthedocs.io/en/main/?badge=main) |  [![codecov](https://codecov.io/gh/kevin931/cytomulate/branch/dev/graph/badge.svg?token=F5H0QTXGMR)](https://codecov.io/gh/kevin931/cytomulate) |
+| dev | ![Badge1](https://img.shields.io/badge/Version-v0.2.0-success) |![Tests](https://github.com/kevin931/cytomulate/actions/workflows/ci.yml/badge.svg?branch=dev) | [![Documentation Status](https://readthedocs.org/projects/cytomulate/badge/?version=dev)](https://cytomulate.readthedocs.io/en/dev/?badge=dev) | [![codecov](https://codecov.io/gh/kevin931/cytomulate/branch/dev/graph/badge.svg?token=F5H0QTXGMR)](https://codecov.io/gh/kevin931/cytomulate) |
 
 
 ## Installation
 
 You can easily install ``cytomulate`` from either ``PyPI`` or ``conda``. For the former, use the following command:
 
 ```shell
@@ -25,14 +25,30 @@
 
 ```shell
 conda install -c normalizingflow cytomulate
 
 ```
 If you wish to use ``PyCytoData``, you can install separately with more instructions [here](https://cytomulate.readthedocs.io/en/dev/installation.html).
 
+### Dependencies
+
+Good news: we didn't have to write `cytomulate` from scratch in assembly language! This means that we will need dependencies to install it. Below is a list of packages that you will need:
+
+- numpy
+- scipy
+- scikit-learn
+- networkx
+- matplotlib
+- tqdm
+
+Most of these are pretty standard! And even better news: the installation instructions should automatically handle all the dependency issues. If you have a problem with installation, let us know and we're happy to help!
+
+While the above are all core dependencies, we highly highly highly highly highly recommend `PyCytoData` as well! You can get all the benefits of an integrated pipeline! But of course, for those of you who don't fancy more dependencies, we understand as well!
+
+
 ## Examples
 
 We have two modes: **Creation Mode** and **Emulation Mode**. The former is probabilistic-model based simulation without the need of datasets; the latter is based on existing datasets to match as much of the existing features as possible. Here, we give two quick examples of how they work.
 
 
 ### Creation Mode
 
@@ -104,31 +120,31 @@
 ## Documentation
 
 For more detailed documentation on ``cytomulate``, please visit our [website](https://cytomulate.readthedocs.io/)! You will find detailed tutorials,
 guidelines, development guides, etc.
 
 Our documentation is built automatically on the cloud! If you wish to build locally, check our detailed guide [here](https://cytomulate.readthedocs.io/en/latest/change/build.html)!
 
-## Latest Release: v0.1.0
+## Latest Release: v0.2.0
 
-Our **FIRST OFFICIAL RELEASE** is here! From now on, all our releases will be supported with our standard support cycle. Here you will find our release notes.
+Welcome to Cytomulate v0.2.0! Hooray! We are not only bringing documentation enhancements, but we
+are also introducing a new feature for more accurate simulations!
 
 ### Changes and New Features
-
-- Added Command-Line Interface with support for complex simulations
-- Improved docstrings
-- Improved documentations with tutorials
-
-### From Pre-release
-
-These are listed for documetation reasons for the first official release.
-
-- Support for ``Emulation Mode`` and ``Creation Mode``
-- Support for complex simulations
-- Availability on ``PyPI`` and ``conda``
+- The `utilities.univariate_noise_model()` method:
+    - Added `half_normal` option to the `noise_distribution` parameter
+    - Changed the default `noise_distribution` to `uniform` (This is a **breaking change** because of the benefits to simulated results).
+    - A warning is given when no user-specified `noise_distribution` is supplied to warn the breaking change
+- Added the `utilities.estimate_noise_model()` method to estimate the noise present in the data
+- Added a built-in estimation procedure to match the amount of zeroes observed in the dataset
+
+### Improvements
+- Added 4 more detailed tutorials on `our documentation website <https://cytomulate.readthedocs.io>`_
+- Improved docstrings with more details on key parameters
+- Updated the lastest references and links
 
 
 ## References
 
 If you are cytomulating in your workflow, citing [our paper](https://doi.org/10.1101/2022.06.14.496200) is appreciated:
 
 ```
```

### Comparing `cytomulate-0.1.0/cytomulate/__main__.py` & `cytomulate-0.2.0/cytomulate/__main__.py`

 * *Files identical despite different names*

### Comparing `cytomulate-0.1.0/cytomulate/cell_graph_general.py` & `cytomulate-0.2.0/cytomulate/cell_graph_general.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,16 @@
         """Generate the actual differential paths
 
         Parameters
         ----------
         cell_types: dict
             A dictionary of CellType objects
         kwargs:
-            Extra parameters needed for non-default path generation algorithms
+            Extra parameters needed for non-default path generation algorithms, which
+            are passed to ``cytomulate.utilities.trajectories``.
         """
         edges = self.graph.edges
         for e in edges:
             from_label = e[0]
             to_label = e[1]
             end_values = cell_types[to_label].cell_mean - cell_types[from_label].cell_mean
             if self.n_markers <= 0:
```

### Comparing `cytomulate-0.1.0/cytomulate/cell_type_general.py` & `cytomulate-0.2.0/cytomulate/cell_type_general.py`

 * *Files 26% similar despite different names*

```diff
@@ -30,15 +30,17 @@
 
         # The actual cell type model
         self.model = None
 
         # cell_mean and cell_covariance are used during cell differentiation
         self.cell_mean = np.zeros(self.n_markers)
         self.cell_covariance = np.zeros((self.n_markers, self.n_markers))
-
+        # zero_probabilities is used for adjustment 
+        self.zero_probabilities = np.zeros(n_markers)
+        
     def sample_cell(self,
                     n_samples: int) -> Tuple[np.ndarray, np.ndarray]:
         """Draw random samples from the cell type model
 
         Parameters
         ----------
         n_samples: int
@@ -52,10 +54,25 @@
             An index array of positive values which
             will be used during the actual sample
             function in the CytofData object
                                 
         """
         X = np.zeros((n_samples, self.n_markers))
         X[:, :], _ = self.model.sample(n_samples)
-        expressed_index = (X > 0)
         X = np.clip(X, a_min=0, a_max=None)
+        for m in range(self.n_markers):
+            n_zero_exp = int((self.zero_probabilities[m]) * n_samples) 
+            n_zero_present = np.sum(X[:, m]<0.0001)
+            n_zero_needed = np.max([0, n_zero_exp-n_zero_present])
+            if n_zero_needed > 0:
+                non_zero_ind = np.where(X[:,m]>=0.0001)[0]
+                p = 1/(X[non_zero_ind, m])
+                p /= np.sum(p)
+                # if n_zero_needed is 0, this should yield 
+                # [] which when plugged into the next statement
+                # shall change nothing 
+                ind_to_zero = np.random.choice(non_zero_ind, size=n_zero_needed,
+                                                replace=False, p=p)
+                X[ind_to_zero, m] = 0
+                
+        expressed_index = (X > 0)
         return X, expressed_index
```

### Comparing `cytomulate-0.1.0/cytomulate/creation/cell_graph.py` & `cytomulate-0.2.0/cytomulate/creation/cell_graph.py`

 * *Files identical despite different names*

### Comparing `cytomulate-0.1.0/cytomulate/creation/cell_type.py` & `cytomulate-0.2.0/cytomulate/creation/cell_type.py`

 * *Files identical despite different names*

### Comparing `cytomulate-0.1.0/cytomulate/cytof_data_general.py` & `cytomulate-0.2.0/cytomulate/cytof_data_general.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,19 @@
     OPT_PCK["PyCytoData"] = False
 
 
 class GeneralCytofData:
     def __init__(self,
                  n_batches: int = 1,
                  background_noise_model: Optional[Union[Callable, dict]] = None) -> None:
-        """Initialize the GeneralCytofData object
+        """Initialize the GeneralCytofData object.
+        
+        This is the base class for `CreationCytofData` and `EmulationCytofData`, both of
+        which inherits most of the methods. This class provides functionalities including
+        sampling and complex simulations.
 
         Parameters
         ----------
         n_batches: int
             Number of batches
         background_noise_model: Callable or dict
             The probabilistic model used to generate noise. It should only have one input: size
@@ -49,20 +53,26 @@
         self.cell_type_ids_to_labels = {}
         self.cell_types = {}
 
         self.cell_graph = GeneralCellGraph()
 
     def generate_cell_abundances(self,
                                  is_random: bool = True) -> None:
-        """Generate cell abundances
+        """Generate cell abundances.
+        
+        This method generates the cell abundane for each batch. The probability
+        of each cell type can be either random or fixed with equal probabilities.
+        See `is_random` parameter for details.
 
         Parameters
         ----------
         is_random: bool
-            Whether the cell abundances should be randomly generated
+            Whether the cell abundances should be randomly generated. If
+            `True`, the abundance of each cell type is sampled from a dirichlet
+            distribution. If `False`, then all cell types an have equal probability. 
         """
         if is_random:
             # If randomly generate cell abundances,
             # we sample from a dirichlet(1)
             for b in range(self.n_batches):
                 self.cell_abundances[b] = {}
                 abundance = np.random.dirichlet(np.ones(len(self.cell_types)), size=1).reshape(-1)
@@ -214,21 +224,24 @@
 
         Parameters
         ----------
         n_samples: int
             Number of samples
         cell_abundances: dict or None
             A dictionary whose keys are the cell labels. The corresponding values should be
-            either the actual number of events for each cell type or the probability of each cell type
+            either the actual number of events for each cell type or the probability of each cell type.
+            If this is not provided, the one stored in the object will be used. Defaults to `None`.
         batch: int
-            The index of the batch for which we want to draw samples
+            The index of the batch for which we want to draw samples. Defaults to 0.
         beta_alpha: float or int
-            The alpha parameter of the beta distribution
+            The alpha parameter of the beta distribution, which should be contrained to the positive reals.
+            Defaults to 0.4.
         beta_beta: float or int
-            The beta parameter of the beta distribution
+            The beta parameter of the beta distribution, which should be contrained to the positive reals.
+            Defaults to 1.0.
 
         Returns
         -------
         expression_matrix: np.ndarray
             The expression matrix
         labels: np.ndarray
             The array of the corresponding cell type labels
@@ -351,17 +364,19 @@
             Number of samples for each batch. If an integer is provided, then it will be used for all batches
         cell_abundances: dict or None
             A nested dictionary whose keys are the batches. The corresponding values should be
             a dictionary mapping cell types to cell numbers or probabilities OR
             It can be a plain dictionary whose keys are the cell labels. The corresponding values should be
             either the actual number of events for each cell type or the probability of each cell type
         beta_alpha: float, int, or dict
-            The alpha parameters of the beta distribution
+            The alpha parameters of the beta distribution, which should be contrained to the positive reals.
+            Defaults to 0.4.
         beta_beta: float, int, or dict
-            The beta parameters of the beta distribution
+            The beta parameters of the beta distribution, which should be contrained to the positive reals.
+            Defaults to 0.4.
 
         Returns
         -------
         expression_matrices: dict
             The dictionary of expression matrices
         labels: dict
             The dictionary of arrays of the corresponding cell type labels
```

### Comparing `cytomulate-0.1.0/cytomulate/emulation/cell_graph.py` & `cytomulate-0.2.0/cytomulate/emulation/cell_graph.py`

 * *Files identical despite different names*

### Comparing `cytomulate-0.1.0/cytomulate/emulation/cell_type.py` & `cytomulate-0.2.0/cytomulate/emulation/cell_type.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,14 @@
         cell_id: int
             The id number assigned to the cell type
         n_markers: int
             Number of markers used in the experiment
         """
         super().__init__(label, cell_id, n_markers)
 
-
     def fit(self,
             data: np.ndarray,
             max_components: int,
             min_components: int,
             covariance_types: Union[list, tuple]) -> None:
         """Fit cell type models using the data provided
         
@@ -56,15 +55,18 @@
         # If the number of component the greater than the number of points
         # we will change them to the number of points
         min_components = np.min([min_components, n])
         max_components = np.min([max_components, n])
 
         self.cell_mean = np.mean(data, axis=0)
         self.cell_covariance = np.cov(data, rowvar=False)
-
+        
+        for m in range(self.n_markers):
+            self.zero_probabilities[m] = np.mean(data[:, m] < 0.0001)
+        
         # We use BIC (the smaller the better) to perform model selection
         smallest_bic = np.Inf
         current_bic = 0
         best_gm = None
         for n_components in range(min_components, max_components + 1):
             for cv_type in covariance_types:
                 gm = GaussianMixture(n_components=n_components,
```

### Comparing `cytomulate-0.1.0/cytomulate/utilities.py` & `cytomulate-0.2.0/cytomulate/utilities.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 # Math computation
 import numpy as np
 from numpy import random as rd
+from scipy.special import erfinv 
 
 # Polynomials and spline functions
 from numpy.polynomial import polynomial
 from scipy.interpolate import Akima1DInterpolator
 from scipy.interpolate import UnivariateSpline
 
+# Warnings
+import warnings
+
 # Typing
-from typing import Union, Optional, List, Tuple, Callable
+from typing import Union, Optional, List, Callable
 
 
 def spline_function(x: np.ndarray,
                     y: np.ndarray,
                     smoothing_factor: float = 0.5) -> Callable:
     """Generate a smoothing spline function
     
@@ -172,34 +176,76 @@
         trajectories_functions.append(spline_function(x, y, **kwargs))
     else:
         raise ValueError('Unknown type')
 
     return trajectories_functions
 
 
-def univariate_noise_model(noise_distribution: str = "normal",
+def univariate_noise_model(noise_distribution: Optional[str] = None,
                            **kwargs) -> Callable:
     """Generate a noise distribution
-    This is mainly used to generate background noise in the cytof_data object
+    This is mainly used to generate background noise in the cytof_data object.
+    
+    .. versionchanged:: 0.2.0 The default `noise_distribution` is changed to `uniform`. If no user-specified value is provided, a warning is given to inform users of the change.
+    .. versionadded:: 0.2.0 Added the `half_normal` option to the `noise_distribution` parameter.
     
     Parameters
     ----------
     noise_distribution: str
-        Either "normal" or "uniform"
+        Either "normal", "half_normal", or "uniform"
     kwargs:
         extra parameters needed for numpy.random.normal or numpy.random.uniform
 
     Returns
     -------
     model: Callable
         A RV generator that only takes size as its input
     """
-    if noise_distribution == "normal":
+    if noise_distribution is None:
+        warnings.warn("The default `noise_distribution` is now changed from `normal` to `uniform` as of v0.2.0. Please see the release notes for details.")
+        noise_distribution = "uniform"
+        
+    if noise_distribution == "half_normal":
+        def model(size):
+            return -np.abs(rd.normal(**kwargs, size=size))
+    elif noise_distribution == "normal":
         def model(size):
             return rd.normal(**kwargs, size=size)
     elif noise_distribution == "uniform":
         def model(size):
             return rd.uniform(**kwargs, size=size)
     else:
         raise ValueError('Unknown noise distribution')
     return model
 
+
+def estimate_noise_model(data: np.ndarray,
+                         noise_distribution: str = "uniform") -> Callable:
+    """Estimate the noise model from data
+    
+    .. versionadded:: 0.2.0
+
+    Parameters
+    ----------
+    data : np.ndarray
+        An array of expression matrix 
+    noise_distribution : str, optional
+        Either "half_normal" or "uniform", by default "uniform"
+
+    Returns
+    -------
+    Callable
+        A RV generator that only takes size as its input
+    """
+    para_dict = {"noise_distribution": noise_distribution}
+    if noise_distribution == "uniform":
+        min_val = np.min(data)
+        para_dict["low"] = min_val
+        para_dict["high"] = 0
+        
+    if noise_distribution == "half_normal":
+        m = np.median(data[np.where(data<=0)])
+        scale = np.abs(m/(np.sqrt(2)*erfinv(0.5)))
+        para_dict["loc"] = 0
+        para_dict["scale"] = scale
+    
+    return univariate_noise_model(**para_dict)
```

### Comparing `cytomulate-0.1.0/cytomulate.egg-info/PKG-INFO` & `cytomulate-0.2.0/cytomulate.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,160 +1,175 @@
 Metadata-Version: 2.1
 Name: cytomulate
-Version: 0.1.0
+Version: 0.2.0
 Summary: Accurate and Efficient Simulation of CyTOF data
-Home-page: UNKNOWN
 Author: Yuqiu Yang, Kevin Wang, Tao Wang, Sherry Wang
 Author-email: yuqiuy@smu.edu, kevinwang@smu.edu, Tao.Wang@UTSouthwestern.edu, swang@smu.edu
-License: UNKNOWN
-Description: ![Logo](/assets/cytomulate.jpg)
-        
-        # cytomulate
-        > A simulation package for Cytometry by Time-of-Flight (CyTOF)
-        
-        [![forthebadge](https://forthebadge.com/images/badges/open-source.svg)](https://forthebadge.com)
-        [![forthebadge](https://forthebadge.com/images/badges/made-with-python.svg)](https://forthebadge.com)
-        
-        | Branch | Release | CI/CD | Documentation | Code Coverage |
-        | --- | --- | --- | --- | --- |
-        | main | ![Badge1](https://img.shields.io/badge/Version-v0.1.0-success) | ![Tests](https://github.com/kevin931/cytomulate/actions/workflows/ci.yml/badge.svg?branch=main) | [![Documentation Status](https://readthedocs.org/projects/cytomulate/badge/?version=dev)](https://cytomulate.readthedocs.io/en/main/?badge=main) |  [![codecov](https://codecov.io/gh/kevin931/cytomulate/branch/dev/graph/badge.svg?token=F5H0QTXGMR)](https://codecov.io/gh/kevin931/cytomulate) |
-        | dev | ![Badge1](https://img.shields.io/badge/Version-v0.1.0-success) |![Tests](https://github.com/kevin931/cytomulate/actions/workflows/ci.yml/badge.svg?branch=dev) | [![Documentation Status](https://readthedocs.org/projects/cytomulate/badge/?version=dev)](https://cytomulate.readthedocs.io/en/dev/?badge=dev) | [![codecov](https://codecov.io/gh/kevin931/cytomulate/branch/dev/graph/badge.svg?token=F5H0QTXGMR)](https://codecov.io/gh/kevin931/cytomulate) |
-        
-        
-        ## Installation
-        
-        You can easily install ``cytomulate`` from either ``PyPI`` or ``conda``. For the former, use the following command:
-        
-        ```shell
-        pip install cytomulate
-        
-        ```
-        
-        Or if you are using a conda environment, you can use the following command:
-        
-        ```shell
-        conda install -c normalizingflow cytomulate
-        
-        ```
-        If you wish to use ``PyCytoData``, you can install separately with more instructions [here](https://cytomulate.readthedocs.io/en/dev/installation.html).
-        
-        ## Examples
-        
-        We have two modes: **Creation Mode** and **Emulation Mode**. The former is probabilistic-model based simulation without the need of datasets; the latter is based on existing datasets to match as much of the existing features as possible. Here, we give two quick examples of how they work.
-        
-        
-        ### Creation Mode
-        
-        To create your datasets, you can run the following:
-        
-        ```python
-        >>> from cytomulate import CreationCytofData
-        >>> cytof_data = CreationCytofData()
-        >>> cytof_data.initialize_cell_types()
-        >>> expression_matrices, labels, _, _ = cytof_data.sample(n_samples = 1000)
-        ```
-        The ``expression_matrices`` is a dictionary that contains the expression matrix from each sample. Correspondingly, ``labels`` is a dictionary that contains their cell types.
-        
-        
-        ### Emulation Mode
-        
-        This is a little bit more involved because we need existing data! If you already have your data, congratulations, you are good to go! For this demonstration, we use ``PyCytoData`` to load some example datasets instead (Of course, you will need to install [PyCytoData](https://pycytodata.readthedocs.io/en/latest/index.html) first if you wish to use it):
-        
-        ```python
-        >>> from cytomulate import EmulationCytoData
-        >>> from PyCytoData import DataLoader
-        
-        >>> exprs = DataLoader.load_dataset(dataset="levine13")
-        >>> exprs.preprocess(arcsinh=True)
-        >>> cytof_data = EmulationCytofData()
-        >>> cytof_data.initialize_cell_types(expression_matrix=exprs.expression_matrix,
-        ...                                  labels=exprs.cell_types)
-        >>> expression_matrices, labels, _, _ = cytof_data.sample(n_samples = 1000)
-        ```
-        This is it!
-        
-        ### Working with PyCytoData
-        
-        ![PyCytoData](/assets/pycytodata.jpg)
-        
-        We're fully compatible with ``PyCytoData``! As you've seen above, you can use ``PyCytoData`` to download datasets! If you're familiar with that interface and in love with its easy workflow, you can have ``cytomulate`` output a ``PyCytoData`` object as well:
-        
-        ```python
-        >>> from cytomulate import CreationCytofData
-        >>> cytof_data = CreationCytofData()
-        >>> cytof_data.initialize_cell_types()
-        >>> simulation_data = cytof_data.sample_to_pycytodata(n_samples = 1000)
-        ```
-        This will allow you to use all the downstream capabilities of ``PyCytoData``.
-        
-        ### Command-Line Interface (CLI)
-        
-        If you prefer to use cytomulate from the command-line, you've got that option as well! One **caveat** is that this mode requires ``PyCytoData`` to be installed. To run the Creation Mode, you can do:
-        
-        ```shell
-        python -m cytomulate \
-        	--creation \
-        	--n_cells 1000 \
-        	-o <your_dir_here>
-        ```
-        
-        To run the emulation mode, you can run the following:
-        
-        ```shell
-        python -m cytomulate \
-        	--emulation \
-        	--n_cells 1000 \
-        	-o <your_dir_here> \
-        	--exprs <you_path_to_exprssion_matrix> \
-        	--cell_types <you_path_to_cell_types>
-        ```
-        Of course, we have much more customization options! For more details, read our [tutorial here](https://cytomulate.readthedocs.io/en/dev/tutorial/cli.html).
-        
-        ## Documentation
-        
-        For more detailed documentation on ``cytomulate``, please visit our [website](https://cytomulate.readthedocs.io/)! You will find detailed tutorials,
-        guidelines, development guides, etc.
-        
-        Our documentation is built automatically on the cloud! If you wish to build locally, check our detailed guide [here](https://cytomulate.readthedocs.io/en/latest/change/build.html)!
-        
-        ## Latest Release: v0.1.0
-        
-        Our **FIRST OFFICIAL RELEASE** is here! From now on, all our releases will be supported with our standard support cycle. Here you will find our release notes.
-        
-        ### Changes and New Features
-        
-        - Added Command-Line Interface with support for complex simulations
-        - Improved docstrings
-        - Improved documentations with tutorials
-        
-        ### From Pre-release
-        
-        These are listed for documetation reasons for the first official release.
-        
-        - Support for ``Emulation Mode`` and ``Creation Mode``
-        - Support for complex simulations
-        - Availability on ``PyPI`` and ``conda``
-        
-        
-        ## References
-        
-        If you are cytomulating in your workflow, citing [our paper](https://doi.org/10.1101/2022.06.14.496200) is appreciated:
-        
-        ```
-        @article {Yang2022.06.14.496200,
-        	author = {Yang, Yuqiu and Wang, Kaiwen and Lu, Zeyu and Wang, Tao and Wang, Xinlei},
-        	title = {Cytomulate: Accurate and Efficient Simulation of CyTOF data},
-        	elocation-id = {2022.06.14.496200},
-        	year = {2022},
-        	doi = {10.1101/2022.06.14.496200},
-        	publisher = {Cold Spring Harbor Laboratory},
-        	URL = {https://www.biorxiv.org/content/early/2022/06/16/2022.06.14.496200},
-        	eprint = {https://www.biorxiv.org/content/early/2022/06/16/2022.06.14.496200.full.pdf},
-        	journal = {bioRxiv}
-        }
-        ```
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+![Logo](/assets/cytomulate.jpg)
+
+# cytomulate
+> A simulation package for Cytometry by Time-of-Flight (CyTOF)
+
+[![forthebadge](https://forthebadge.com/images/badges/open-source.svg)](https://forthebadge.com)
+[![forthebadge](https://forthebadge.com/images/badges/made-with-python.svg)](https://forthebadge.com)
+
+| Branch | Release | CI/CD | Documentation | Code Coverage |
+| --- | --- | --- | --- | --- |
+| main | ![Badge1](https://img.shields.io/badge/Version-v0.2.0-success) | ![Tests](https://github.com/kevin931/cytomulate/actions/workflows/ci.yml/badge.svg?branch=main) | [![Documentation Status](https://readthedocs.org/projects/cytomulate/badge/?version=dev)](https://cytomulate.readthedocs.io/en/main/?badge=main) |  [![codecov](https://codecov.io/gh/kevin931/cytomulate/branch/dev/graph/badge.svg?token=F5H0QTXGMR)](https://codecov.io/gh/kevin931/cytomulate) |
+| dev | ![Badge1](https://img.shields.io/badge/Version-v0.2.0-success) |![Tests](https://github.com/kevin931/cytomulate/actions/workflows/ci.yml/badge.svg?branch=dev) | [![Documentation Status](https://readthedocs.org/projects/cytomulate/badge/?version=dev)](https://cytomulate.readthedocs.io/en/dev/?badge=dev) | [![codecov](https://codecov.io/gh/kevin931/cytomulate/branch/dev/graph/badge.svg?token=F5H0QTXGMR)](https://codecov.io/gh/kevin931/cytomulate) |
+
+
+## Installation
+
+You can easily install ``cytomulate`` from either ``PyPI`` or ``conda``. For the former, use the following command:
+
+```shell
+pip install cytomulate
+
+```
+
+Or if you are using a conda environment, you can use the following command:
+
+```shell
+conda install -c normalizingflow cytomulate
+
+```
+If you wish to use ``PyCytoData``, you can install separately with more instructions [here](https://cytomulate.readthedocs.io/en/dev/installation.html).
+
+### Dependencies
+
+Good news: we didn't have to write `cytomulate` from scratch in assembly language! This means that we will need dependencies to install it. Below is a list of packages that you will need:
+
+- numpy
+- scipy
+- scikit-learn
+- networkx
+- matplotlib
+- tqdm
+
+Most of these are pretty standard! And even better news: the installation instructions should automatically handle all the dependency issues. If you have a problem with installation, let us know and we're happy to help!
+
+While the above are all core dependencies, we highly highly highly highly highly recommend `PyCytoData` as well! You can get all the benefits of an integrated pipeline! But of course, for those of you who don't fancy more dependencies, we understand as well!
+
+
+## Examples
+
+We have two modes: **Creation Mode** and **Emulation Mode**. The former is probabilistic-model based simulation without the need of datasets; the latter is based on existing datasets to match as much of the existing features as possible. Here, we give two quick examples of how they work.
+
+
+### Creation Mode
+
+To create your datasets, you can run the following:
+
+```python
+>>> from cytomulate import CreationCytofData
+>>> cytof_data = CreationCytofData()
+>>> cytof_data.initialize_cell_types()
+>>> expression_matrices, labels, _, _ = cytof_data.sample(n_samples = 1000)
+```
+The ``expression_matrices`` is a dictionary that contains the expression matrix from each sample. Correspondingly, ``labels`` is a dictionary that contains their cell types.
+
+
+### Emulation Mode
+
+This is a little bit more involved because we need existing data! If you already have your data, congratulations, you are good to go! For this demonstration, we use ``PyCytoData`` to load some example datasets instead (Of course, you will need to install [PyCytoData](https://pycytodata.readthedocs.io/en/latest/index.html) first if you wish to use it):
+
+```python
+>>> from cytomulate import EmulationCytoData
+>>> from PyCytoData import DataLoader
+
+>>> exprs = DataLoader.load_dataset(dataset="levine13")
+>>> exprs.preprocess(arcsinh=True)
+>>> cytof_data = EmulationCytofData()
+>>> cytof_data.initialize_cell_types(expression_matrix=exprs.expression_matrix,
+...                                  labels=exprs.cell_types)
+>>> expression_matrices, labels, _, _ = cytof_data.sample(n_samples = 1000)
+```
+This is it!
+
+### Working with PyCytoData
+
+![PyCytoData](/assets/pycytodata.jpg)
+
+We're fully compatible with ``PyCytoData``! As you've seen above, you can use ``PyCytoData`` to download datasets! If you're familiar with that interface and in love with its easy workflow, you can have ``cytomulate`` output a ``PyCytoData`` object as well:
+
+```python
+>>> from cytomulate import CreationCytofData
+>>> cytof_data = CreationCytofData()
+>>> cytof_data.initialize_cell_types()
+>>> simulation_data = cytof_data.sample_to_pycytodata(n_samples = 1000)
+```
+This will allow you to use all the downstream capabilities of ``PyCytoData``.
+
+### Command-Line Interface (CLI)
+
+If you prefer to use cytomulate from the command-line, you've got that option as well! One **caveat** is that this mode requires ``PyCytoData`` to be installed. To run the Creation Mode, you can do:
+
+```shell
+python -m cytomulate \
+	--creation \
+	--n_cells 1000 \
+	-o <your_dir_here>
+```
+
+To run the emulation mode, you can run the following:
+
+```shell
+python -m cytomulate \
+	--emulation \
+	--n_cells 1000 \
+	-o <your_dir_here> \
+	--exprs <you_path_to_exprssion_matrix> \
+	--cell_types <you_path_to_cell_types>
+```
+Of course, we have much more customization options! For more details, read our [tutorial here](https://cytomulate.readthedocs.io/en/dev/tutorial/cli.html).
+
+## Documentation
+
+For more detailed documentation on ``cytomulate``, please visit our [website](https://cytomulate.readthedocs.io/)! You will find detailed tutorials,
+guidelines, development guides, etc.
+
+Our documentation is built automatically on the cloud! If you wish to build locally, check our detailed guide [here](https://cytomulate.readthedocs.io/en/latest/change/build.html)!
+
+## Latest Release: v0.2.0
+
+Welcome to Cytomulate v0.2.0! Hooray! We are not only bringing documentation enhancements, but we
+are also introducing a new feature for more accurate simulations!
+
+### Changes and New Features
+- The `utilities.univariate_noise_model()` method:
+    - Added `half_normal` option to the `noise_distribution` parameter
+    - Changed the default `noise_distribution` to `uniform` (This is a **breaking change** because of the benefits to simulated results).
+    - A warning is given when no user-specified `noise_distribution` is supplied to warn the breaking change
+- Added the `utilities.estimate_noise_model()` method to estimate the noise present in the data
+- Added a built-in estimation procedure to match the amount of zeroes observed in the dataset
+
+### Improvements
+- Added 4 more detailed tutorials on `our documentation website <https://cytomulate.readthedocs.io>`_
+- Improved docstrings with more details on key parameters
+- Updated the lastest references and links
+
+
+## References
+
+If you are cytomulating in your workflow, citing [our paper](https://doi.org/10.1101/2022.06.14.496200) is appreciated:
+
+```
+@article {Yang2022.06.14.496200,
+	author = {Yang, Yuqiu and Wang, Kaiwen and Lu, Zeyu and Wang, Tao and Wang, Xinlei},
+	title = {Cytomulate: Accurate and Efficient Simulation of CyTOF data},
+	elocation-id = {2022.06.14.496200},
+	year = {2022},
+	doi = {10.1101/2022.06.14.496200},
+	publisher = {Cold Spring Harbor Laboratory},
+	URL = {https://www.biorxiv.org/content/early/2022/06/16/2022.06.14.496200},
+	eprint = {https://www.biorxiv.org/content/early/2022/06/16/2022.06.14.496200.full.pdf},
+	journal = {bioRxiv}
+}
+```
```

### Comparing `cytomulate-0.1.0/cytomulate.egg-info/SOURCES.txt` & `cytomulate-0.2.0/cytomulate.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.txt
 README.md
 setup.py
 cytomulate/__init__.py
 cytomulate/__main__.py
 cytomulate/cell_graph_general.py
 cytomulate/cell_type_general.py
 cytomulate/cytof_data_general.py
```

### Comparing `cytomulate-0.1.0/setup.py` & `cytomulate-0.2.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 import sys
 import os
 import shutil
 import distutils.cmd
 
-VERSION = "0.1.0"
+VERSION = "0.2.0"
 
 class PypiCommand(distutils.cmd.Command):
     
     description = "Build and upload for PyPI."
     user_options = []
     
     def initialize_options(self):
```

