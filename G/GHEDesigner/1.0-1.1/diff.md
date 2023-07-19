# Comparing `tmp/GHEDesigner-1.0.tar.gz` & `tmp/GHEDesigner-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GHEDesigner-1.0.tar", last modified: Fri Mar 24 20:25:26 2023, max compression
+gzip compressed data, was "GHEDesigner-1.1.tar", last modified: Wed Jul 19 15:35:51 2023, max compression
```

## Comparing `GHEDesigner-1.0.tar` & `GHEDesigner-1.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-24 20:25:26.695057 GHEDesigner-1.0/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-24 20:25:26.691057 GHEDesigner-1.0/GHEDesigner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    13020 2023-03-24 20:25:26.000000 GHEDesigner-1.0/GHEDesigner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      861 2023-03-24 20:25:26.000000 GHEDesigner-1.0/GHEDesigner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-24 20:25:26.000000 GHEDesigner-1.0/GHEDesigner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       74 2023-03-24 20:25:26.000000 GHEDesigner-1.0/GHEDesigner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-03-24 20:25:26.000000 GHEDesigner-1.0/GHEDesigner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-03-24 20:25:26.000000 GHEDesigner-1.0/GHEDesigner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2104 2023-03-24 20:25:21.000000 GHEDesigner-1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    13020 2023-03-24 20:25:26.695057 GHEDesigner-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    10924 2023-03-24 20:25:21.000000 GHEDesigner-1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-24 20:25:26.695057 GHEDesigner-1.0/ghedesigner/
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-03-24 20:25:21.000000 GHEDesigner-1.0/ghedesigner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      330 2023-03-24 20:25:21.000000 GHEDesigner-1.0/ghedesigner/borehole.py
--rw-r--r--   0 runner    (1001) docker     (122)    21430 2023-03-24 20:25:21.000000 GHEDesigner-1.0/ghedesigner/borehole_heat_exchangers.py
--rw-r--r--   0 runner    (1001) docker     (122)      108 2023-03-24 20:25:21.000000 GHEDesigner-1.0/ghedesigner/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     4378 2023-03-24 20:25:21.000000 GHEDesigner-1.0/ghedesigner/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (122)    13507 2023-03-24 20:25:21.000000 GHEDesigner-1.0/ghedesigner/design.py
--rw-r--r--   0 runner    (1001) docker     (122)    13776 2023-03-24 20:25:21.000000 GHEDesigner-1.0/ghedesigner/domains.py
--rw-r--r--   0 runner    (1001) docker     (122)      724 2023-03-24 20:25:21.000000 GHEDesigner-1.0/ghedesigner/enums.py
--rw-r--r--   0 runner    (1001) docker     (122)     2814 2023-03-24 20:25:21.000000 GHEDesigner-1.0/ghedesigner/feature_recognition.py
--rw-r--r--   0 runner    (1001) docker     (122)     5235 2023-03-24 20:25:21.000000 GHEDesigner-1.0/ghedesigner/geometry.py
--rw-r--r--   0 runner    (1001) docker     (122)    13593 2023-03-24 20:25:21.000000 GHEDesigner-1.0/ghedesigner/gfunction.py
--rw-r--r--   0 runner    (1001) docker     (122)    14187 2023-03-24 20:25:21.000000 GHEDesigner-1.0/ghedesigner/ground_heat_exchangers.py
--rw-r--r--   0 runner    (1001) docker     (122)    34420 2023-03-24 20:25:21.000000 GHEDesigner-1.0/ghedesigner/ground_loads.py
--rw-r--r--   0 runner    (1001) docker     (122)    38537 2023-03-24 20:25:21.000000 GHEDesigner-1.0/ghedesigner/manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     4595 2023-03-24 20:25:21.000000 GHEDesigner-1.0/ghedesigner/media.py
--rw-r--r--   0 runner    (1001) docker     (122)    33796 2023-03-24 20:25:21.000000 GHEDesigner-1.0/ghedesigner/output.py
--rw-r--r--   0 runner    (1001) docker     (122)    18134 2023-03-24 20:25:21.000000 GHEDesigner-1.0/ghedesigner/radial_numerical_borehole.py
--rw-r--r--   0 runner    (1001) docker     (122)    32742 2023-03-24 20:25:21.000000 GHEDesigner-1.0/ghedesigner/rowwise.py
--rw-r--r--   0 runner    (1001) docker     (122)    35429 2023-03-24 20:25:21.000000 GHEDesigner-1.0/ghedesigner/search_routines.py
--rw-r--r--   0 runner    (1001) docker     (122)     6839 2023-03-24 20:25:21.000000 GHEDesigner-1.0/ghedesigner/shape.py
--rw-r--r--   0 runner    (1001) docker     (122)     1483 2023-03-24 20:25:21.000000 GHEDesigner-1.0/ghedesigner/simulation.py
--rw-r--r--   0 runner    (1001) docker     (122)     2722 2023-03-24 20:25:21.000000 GHEDesigner-1.0/ghedesigner/utilities.py
--rw-r--r--   0 runner    (1001) docker     (122)     5417 2023-03-24 20:25:21.000000 GHEDesigner-1.0/ghedesigner/validate.py
--rw-r--r--   0 runner    (1001) docker     (122)      229 2023-03-24 20:25:26.695057 GHEDesigner-1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1400 2023-03-24 20:25:21.000000 GHEDesigner-1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 15:35:51.104897 GHEDesigner-1.1/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 15:35:51.100897 GHEDesigner-1.1/GHEDesigner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    13868 2023-07-19 15:35:50.000000 GHEDesigner-1.1/GHEDesigner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      861 2023-07-19 15:35:50.000000 GHEDesigner-1.1/GHEDesigner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-19 15:35:50.000000 GHEDesigner-1.1/GHEDesigner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       74 2023-07-19 15:35:50.000000 GHEDesigner-1.1/GHEDesigner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-07-19 15:35:50.000000 GHEDesigner-1.1/GHEDesigner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-07-19 15:35:50.000000 GHEDesigner-1.1/GHEDesigner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2104 2023-07-19 15:35:47.000000 GHEDesigner-1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    13868 2023-07-19 15:35:51.104897 GHEDesigner-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    11641 2023-07-19 15:35:47.000000 GHEDesigner-1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 15:35:51.104897 GHEDesigner-1.1/ghedesigner/
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-07-19 15:35:47.000000 GHEDesigner-1.1/ghedesigner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      330 2023-07-19 15:35:47.000000 GHEDesigner-1.1/ghedesigner/borehole.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21430 2023-07-19 15:35:47.000000 GHEDesigner-1.1/ghedesigner/borehole_heat_exchangers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      108 2023-07-19 15:35:47.000000 GHEDesigner-1.1/ghedesigner/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4378 2023-07-19 15:35:47.000000 GHEDesigner-1.1/ghedesigner/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13507 2023-07-19 15:35:47.000000 GHEDesigner-1.1/ghedesigner/design.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13758 2023-07-19 15:35:47.000000 GHEDesigner-1.1/ghedesigner/domains.py
+-rw-r--r--   0 runner    (1001) docker     (122)      724 2023-07-19 15:35:47.000000 GHEDesigner-1.1/ghedesigner/enums.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2154 2023-07-19 15:35:47.000000 GHEDesigner-1.1/ghedesigner/feature_recognition.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5235 2023-07-19 15:35:47.000000 GHEDesigner-1.1/ghedesigner/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13593 2023-07-19 15:35:47.000000 GHEDesigner-1.1/ghedesigner/gfunction.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14420 2023-07-19 15:35:47.000000 GHEDesigner-1.1/ghedesigner/ground_heat_exchangers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34420 2023-07-19 15:35:47.000000 GHEDesigner-1.1/ghedesigner/ground_loads.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38537 2023-07-19 15:35:47.000000 GHEDesigner-1.1/ghedesigner/manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4595 2023-07-19 15:35:47.000000 GHEDesigner-1.1/ghedesigner/media.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33898 2023-07-19 15:35:47.000000 GHEDesigner-1.1/ghedesigner/output.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15065 2023-07-19 15:35:47.000000 GHEDesigner-1.1/ghedesigner/radial_numerical_borehole.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32742 2023-07-19 15:35:47.000000 GHEDesigner-1.1/ghedesigner/rowwise.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35429 2023-07-19 15:35:47.000000 GHEDesigner-1.1/ghedesigner/search_routines.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8864 2023-07-19 15:35:47.000000 GHEDesigner-1.1/ghedesigner/shape.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1483 2023-07-19 15:35:47.000000 GHEDesigner-1.1/ghedesigner/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2722 2023-07-19 15:35:47.000000 GHEDesigner-1.1/ghedesigner/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5417 2023-07-19 15:35:47.000000 GHEDesigner-1.1/ghedesigner/validate.py
+-rw-r--r--   0 runner    (1001) docker     (122)      229 2023-07-19 15:35:51.104897 GHEDesigner-1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1415 2023-07-19 15:35:47.000000 GHEDesigner-1.1/setup.py
```

### Comparing `GHEDesigner-1.0/GHEDesigner.egg-info/PKG-INFO` & `GHEDesigner-1.1/GHEDesigner.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,30 @@
 Metadata-Version: 2.1
 Name: GHEDesigner
-Version: 1.0
+Version: 1.1
 Summary: A ground heat exchanger design tool with the capability to select and size flexibly configured borehole fields that are customized for specific building and property constraints.
 Home-page: https://github.com/BETSRG/GHEDesigner
 Author: Jeffrey D. Spitler
 Author-email: spitler@okstate.edu
 License: BSD-3
 Description: # GHEDesigner - A Flexible and Automatic Ground Heat Exchanger Design Tool
         
+        ![PyPI](https://img.shields.io/pypi/v/ghedesigner)
+        ![PyPI - Downloads](https://img.shields.io/pypi/dm/ghedesigner?label=PyPI%20Downloads)
+        ![Python Versions](https://img.shields.io/pypi/pyversions/ghedesigner)
+        [![Flake8](https://github.com/BETSRG/GHEDesigner/actions/workflows/flake8.yml/badge.svg)](https://github.com/BETSRG/GHEDesigner/actions/workflows/flake8.yml)
+        [![Tests](https://github.com/BETSRG/GHEDesigner/actions/workflows/tests.yml/badge.svg)](https://github.com/BETSRG/GHEDesigner/actions/workflows/tests.yml)
+        
+        ## Documentation
+        [![Documentation Status](https://readthedocs.org/projects/ghedesigner/badge/?version=latest)](https://ghedesigner.readthedocs.io/en/latest/?badge=latest)
+        
+        Project documentation is hosted on [ReadTheDocs](https://ghedesigner.readthedocs.io/en/latest/)
+        
+        ## Introduction
+        
         GHEDesigner is a Python package for designing ground heat exchangers (GHE) used with ground source heat pump (GSHP)
         systems. Compared to currently available tools such
         as [GLHEPRO](https://betsrg.org/ground-loop-heat-exchanger-design-software), GHEDesigner:
         
         - is flexible. It can synthesize borehole fields that are custom fit to the user's property description,
         - implements the RowWise algorithm ([Spitler, et al. 2022a](https://doi.org/10.22488/okstate.22.000016)) for
           automatically placing and sizing boreholes in any land area with complex geometry,
@@ -98,15 +111,14 @@
         
         GHEDesigner is supported for Python versions >= 3.8, and is tested with Python 3.8 and 3.9. GHEDesigner is dependent on
         the following packages:
         
         - [click][#click] (>=8.1.3)
         - [jsonschema][#jsonschema] (>=4.17.3)
         - [numpy][#numpy] (>=1.24.2)
-        - [opencv-python][#opencv] (==4.7.0.68)
         - [pygfunction][#pygfunction] (>=2.2.2)
         - [scipy][#scipy] (>=1.10.0)
         
         ## Quick Start
         
         **Users** - Install `GHEDesigner` via the package installer for Python ([pip][#pip]):
         
@@ -169,16 +181,14 @@
         
         [#pygfunction]: https://github.com/MassimoCimmino/pygfunction
         
         [#numpy]: https://numpy.org/doc/stable/
         
         [#scipy]: https://docs.scipy.org/doc/scipy/
         
-        [#opencv]: https://pypi.org/project/opencv-python/
-        
         [#click]: https://click.palletsprojects.com/en/8.1.x/
         
         [#jsonschema]: https://pypi.org/project/jsonschema/
         
         [#pip]: https://pip.pypa.io/en/latest/
         
         [#create]: https://github.com/betsrg/ghedesigner/issues/new
@@ -188,9 +198,10 @@
         [#closed]: https://github.com/betsrg/ghedesigner/issues?q=is%3Aissue+is%3Aclosed
         
 Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `GHEDesigner-1.0/GHEDesigner.egg-info/SOURCES.txt` & `GHEDesigner-1.1/GHEDesigner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GHEDesigner-1.0/LICENSE` & `GHEDesigner-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `GHEDesigner-1.0/PKG-INFO` & `GHEDesigner-1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,30 @@
 Metadata-Version: 2.1
 Name: GHEDesigner
-Version: 1.0
+Version: 1.1
 Summary: A ground heat exchanger design tool with the capability to select and size flexibly configured borehole fields that are customized for specific building and property constraints.
 Home-page: https://github.com/BETSRG/GHEDesigner
 Author: Jeffrey D. Spitler
 Author-email: spitler@okstate.edu
 License: BSD-3
 Description: # GHEDesigner - A Flexible and Automatic Ground Heat Exchanger Design Tool
         
+        ![PyPI](https://img.shields.io/pypi/v/ghedesigner)
+        ![PyPI - Downloads](https://img.shields.io/pypi/dm/ghedesigner?label=PyPI%20Downloads)
+        ![Python Versions](https://img.shields.io/pypi/pyversions/ghedesigner)
+        [![Flake8](https://github.com/BETSRG/GHEDesigner/actions/workflows/flake8.yml/badge.svg)](https://github.com/BETSRG/GHEDesigner/actions/workflows/flake8.yml)
+        [![Tests](https://github.com/BETSRG/GHEDesigner/actions/workflows/tests.yml/badge.svg)](https://github.com/BETSRG/GHEDesigner/actions/workflows/tests.yml)
+        
+        ## Documentation
+        [![Documentation Status](https://readthedocs.org/projects/ghedesigner/badge/?version=latest)](https://ghedesigner.readthedocs.io/en/latest/?badge=latest)
+        
+        Project documentation is hosted on [ReadTheDocs](https://ghedesigner.readthedocs.io/en/latest/)
+        
+        ## Introduction
+        
         GHEDesigner is a Python package for designing ground heat exchangers (GHE) used with ground source heat pump (GSHP)
         systems. Compared to currently available tools such
         as [GLHEPRO](https://betsrg.org/ground-loop-heat-exchanger-design-software), GHEDesigner:
         
         - is flexible. It can synthesize borehole fields that are custom fit to the user's property description,
         - implements the RowWise algorithm ([Spitler, et al. 2022a](https://doi.org/10.22488/okstate.22.000016)) for
           automatically placing and sizing boreholes in any land area with complex geometry,
@@ -98,15 +111,14 @@
         
         GHEDesigner is supported for Python versions >= 3.8, and is tested with Python 3.8 and 3.9. GHEDesigner is dependent on
         the following packages:
         
         - [click][#click] (>=8.1.3)
         - [jsonschema][#jsonschema] (>=4.17.3)
         - [numpy][#numpy] (>=1.24.2)
-        - [opencv-python][#opencv] (==4.7.0.68)
         - [pygfunction][#pygfunction] (>=2.2.2)
         - [scipy][#scipy] (>=1.10.0)
         
         ## Quick Start
         
         **Users** - Install `GHEDesigner` via the package installer for Python ([pip][#pip]):
         
@@ -169,16 +181,14 @@
         
         [#pygfunction]: https://github.com/MassimoCimmino/pygfunction
         
         [#numpy]: https://numpy.org/doc/stable/
         
         [#scipy]: https://docs.scipy.org/doc/scipy/
         
-        [#opencv]: https://pypi.org/project/opencv-python/
-        
         [#click]: https://click.palletsprojects.com/en/8.1.x/
         
         [#jsonschema]: https://pypi.org/project/jsonschema/
         
         [#pip]: https://pip.pypa.io/en/latest/
         
         [#create]: https://github.com/betsrg/ghedesigner/issues/new
@@ -188,9 +198,10 @@
         [#closed]: https://github.com/betsrg/ghedesigner/issues?q=is%3Aissue+is%3Aclosed
         
 Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `GHEDesigner-1.0/README.md` & `GHEDesigner-1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,22 @@
 # GHEDesigner - A Flexible and Automatic Ground Heat Exchanger Design Tool
 
+![PyPI](https://img.shields.io/pypi/v/ghedesigner)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/ghedesigner?label=PyPI%20Downloads)
+![Python Versions](https://img.shields.io/pypi/pyversions/ghedesigner)
+[![Flake8](https://github.com/BETSRG/GHEDesigner/actions/workflows/flake8.yml/badge.svg)](https://github.com/BETSRG/GHEDesigner/actions/workflows/flake8.yml)
+[![Tests](https://github.com/BETSRG/GHEDesigner/actions/workflows/tests.yml/badge.svg)](https://github.com/BETSRG/GHEDesigner/actions/workflows/tests.yml)
+
+## Documentation
+[![Documentation Status](https://readthedocs.org/projects/ghedesigner/badge/?version=latest)](https://ghedesigner.readthedocs.io/en/latest/?badge=latest)
+
+Project documentation is hosted on [ReadTheDocs](https://ghedesigner.readthedocs.io/en/latest/)
+
+## Introduction
+
 GHEDesigner is a Python package for designing ground heat exchangers (GHE) used with ground source heat pump (GSHP)
 systems. Compared to currently available tools such
 as [GLHEPRO](https://betsrg.org/ground-loop-heat-exchanger-design-software), GHEDesigner:
 
 - is flexible. It can synthesize borehole fields that are custom fit to the user's property description,
 - implements the RowWise algorithm ([Spitler, et al. 2022a](https://doi.org/10.22488/okstate.22.000016)) for
   automatically placing and sizing boreholes in any land area with complex geometry,
@@ -90,15 +103,14 @@
 
 GHEDesigner is supported for Python versions >= 3.8, and is tested with Python 3.8 and 3.9. GHEDesigner is dependent on
 the following packages:
 
 - [click][#click] (>=8.1.3)
 - [jsonschema][#jsonschema] (>=4.17.3)
 - [numpy][#numpy] (>=1.24.2)
-- [opencv-python][#opencv] (==4.7.0.68)
 - [pygfunction][#pygfunction] (>=2.2.2)
 - [scipy][#scipy] (>=1.10.0)
 
 ## Quick Start
 
 **Users** - Install `GHEDesigner` via the package installer for Python ([pip][#pip]):
 
@@ -161,16 +173,14 @@
 
 [#pygfunction]: https://github.com/MassimoCimmino/pygfunction
 
 [#numpy]: https://numpy.org/doc/stable/
 
 [#scipy]: https://docs.scipy.org/doc/scipy/
 
-[#opencv]: https://pypi.org/project/opencv-python/
-
 [#click]: https://click.palletsprojects.com/en/8.1.x/
 
 [#jsonschema]: https://pypi.org/project/jsonschema/
 
 [#pip]: https://pip.pypa.io/en/latest/
 
 [#create]: https://github.com/betsrg/ghedesigner/issues/new
```

### Comparing `GHEDesigner-1.0/ghedesigner/borehole_heat_exchangers.py` & `GHEDesigner-1.1/ghedesigner/borehole_heat_exchangers.py`

 * *Files identical despite different names*

### Comparing `GHEDesigner-1.0/ghedesigner/coordinates.py` & `GHEDesigner-1.1/ghedesigner/coordinates.py`

 * *Files identical despite different names*

### Comparing `GHEDesigner-1.0/ghedesigner/design.py` & `GHEDesigner-1.1/ghedesigner/design.py`

 * *Files identical despite different names*

### Comparing `GHEDesigner-1.0/ghedesigner/domains.py` & `GHEDesigner-1.1/ghedesigner/domains.py`

 * *Files 0% similar despite different names*

```diff
@@ -373,20 +373,20 @@
 
     coordinates_domain_nested_cutout = []
 
     for domain in coordinates_domain_nested:
         new_coordinates_domain = []
         for coordinates in domain:
             # Remove boreholes outside of property
-            new_coordinates = remove_cutout(coordinates, boundary=property_boundary, remove_inside=False)
+            new_coordinates = remove_cutout(coordinates, property_boundary, remove_inside=False)
             # Remove boreholes inside of building
             if len(new_coordinates) == 0:
                 continue
             for no_go_zone in no_go_boundaries:
-                new_coordinates = remove_cutout(new_coordinates, boundary=no_go_zone, remove_inside=True,
+                new_coordinates = remove_cutout(new_coordinates, no_go_zone, remove_inside=True,
                                                 keep_contour=False)
             new_coordinates_domain.append(new_coordinates)
         coordinates_domain_nested_cutout.append(new_coordinates_domain)
 
     coordinates_domain_nested_cutout_reordered = []
     field_descriptors_reordered = []
     for idx, domain in enumerate(coordinates_domain_nested_cutout):
```

### Comparing `GHEDesigner-1.0/ghedesigner/enums.py` & `GHEDesigner-1.1/ghedesigner/enums.py`

 * *Files identical despite different names*

### Comparing `GHEDesigner-1.0/ghedesigner/feature_recognition.py` & `GHEDesigner-1.1/ghedesigner/feature_recognition.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,30 @@
-import cv2
-import numpy as np
+from ghedesigner.shape import point_polygon_check
 
 
-def scale_coordinates(coordinates, scale):
-    new_coordinates = []
-    for x, y in coordinates:
-        x *= scale
-        y *= scale
-        new_coordinates.append((x, y))
-    return new_coordinates
-
-
-def remove_cutout(coordinates, boundary=None, remove_inside=True, keep_contour=True):
-    if boundary is None:
-        boundary = []
-
-    # cv2.pointPolygonTest only takes integers, so we scale by 10000 and then
-    # scale back to keep precision
-    scale = 10000.0
-    coordinates = scale_coordinates(coordinates, scale)
-    boundary = scale_coordinates(boundary, scale)
-
-    _boundary = np.array(boundary, dtype=np.uint64)
-
-    # https://stackoverflow.com/a/50670359/11637415
-    # Positive - point is inside the contour
-    # Negative - point is outside the contour
-    # Zero - point is on the contour
-
+def remove_cutout(coordinates, boundary, remove_inside=True, keep_contour=True):
     inside_points_idx = []
     outside_points_idx = []
     boundary_points_idx = []
+
+    inside = 1
+    outside = -1
+    on_edge = 0
+
     for idx, coordinate in enumerate(coordinates):
         coordinate = coordinates[idx]
-        dist = cv2.pointPolygonTest(_boundary, coordinate, False)
-        if dist > 0.0:
+        ret = point_polygon_check(boundary, coordinate)
+        if ret == inside:
             inside_points_idx.append(idx)
-        elif dist < 0.0:
+        elif ret == outside:
             outside_points_idx.append(idx)
-        elif dist == 0.0:
+        elif ret == on_edge:
             boundary_points_idx.append(idx)
+        else:
+            raise ValueError("Something bad happened")
 
     new_coordinates = []
     for idx, _ in enumerate(coordinates):
         # if we want to remove inside points and keep contour points
         if remove_inside and keep_contour:
             if idx in inside_points_idx:
                 continue
@@ -64,16 +45,14 @@
         # if we want to keep outside points and keep contour points
         else:
             if idx in outside_points_idx:
                 continue
             else:
                 new_coordinates.append(coordinates[idx])
 
-    new_coordinates = scale_coordinates(new_coordinates, 1 / scale)
-
     return new_coordinates
 
 
 def determine_largest_rectangle(property_boundary):
     x_max = 0
     y_max = 0
     for x, y in property_boundary:
```

### Comparing `GHEDesigner-1.0/ghedesigner/geometry.py` & `GHEDesigner-1.1/ghedesigner/geometry.py`

 * *Files identical despite different names*

### Comparing `GHEDesigner-1.0/ghedesigner/gfunction.py` & `GHEDesigner-1.1/ghedesigner/gfunction.py`

 * *Files identical despite different names*

### Comparing `GHEDesigner-1.0/ghedesigner/ground_heat_exchangers.py` & `GHEDesigner-1.1/ghedesigner/ground_heat_exchangers.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,22 @@
         g = self.combine_sts_lts(
             self.gFunction.log_time,
             g_function_corrected,
             self.radial_numerical.lntts.tolist(),
             self.radial_numerical.g.tolist(),
         )
 
-        return g
+        g_bhw = self.combine_sts_lts(
+            self.gFunction.log_time,
+            g_function_corrected,
+            self.radial_numerical.lntts.tolist(),
+            self.radial_numerical.g_bhw.tolist(),
+        )
+
+        return g, g_bhw
 
     def cost(self, max_eft, min_eft):
         delta_t_max = max_eft - self.sim_params.max_EFT_allowable
         delta_t_min = self.sim_params.min_EFT_allowable - min_eft
 
         t_excess = max([delta_t_max, delta_t_min])
         return t_excess
@@ -267,15 +274,15 @@
             t_excess = self.cost(max_hp_eft, min_hp_eft)
             results['excess_fluid_temperature'] = {'value': t_excess, 'units': 'C'}
         results['peak_load_analysis'] = self.hybrid_load.as_dict()
 
         g_function = dict()
         g_function['coordinates (x[m], y[m])'] = [(x, y) for x, y in self.gFunction.bore_locations]  # TODO: Verify form
         b_over_h = self.B_spacing / self.bhe.b.H
-        g = self.grab_g_function(b_over_h)
+        g, _ = self.grab_g_function(b_over_h)
         total_g_values = g.x.size
         number_lts_g_values = 27
         number_sts_g_values = 50
         sts_step_size = floor((total_g_values - number_lts_g_values) / number_sts_g_values)
         lntts = []
         g_values = []
         for idx in range(0, (total_g_values - number_lts_g_values), sts_step_size):
@@ -299,15 +306,15 @@
 
         # Solve for equivalent single U-tube
         self.bhe_eq = self.bhe.to_single()
         # Update short time step object with equivalent single u-tube
         self.radial_numerical.calc_sts_g_functions(self.bhe_eq)
         # Combine the short and long-term g-functions. The long term g-function
         # is interpolated for specific B/H and rb/H values.
-        g = self.grab_g_function(b_over_h)
+        g, _ = self.grab_g_function(b_over_h)
 
         if method == TimestepType.HYBRID:
             q_dot = self.hybrid_load.load[2:] * 1000.0  # convert to Watts
             time_values = self.hybrid_load.hour[2:]  # convert to seconds
             self.times = time_values
             self.loading = q_dot
```

### Comparing `GHEDesigner-1.0/ghedesigner/ground_loads.py` & `GHEDesigner-1.1/ghedesigner/ground_loads.py`

 * *Files identical despite different names*

### Comparing `GHEDesigner-1.0/ghedesigner/manager.py` & `GHEDesigner-1.1/ghedesigner/manager.py`

 * *Files identical despite different names*

### Comparing `GHEDesigner-1.0/ghedesigner/media.py` & `GHEDesigner-1.1/ghedesigner/media.py`

 * *Files identical despite different names*

### Comparing `GHEDesigner-1.0/ghedesigner/output.py` & `GHEDesigner-1.1/ghedesigner/output.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,20 +132,25 @@
         for hour, hour_load in enumerate(hourly_loadings):
             month, day_in_month, hour_in_day = self.ghe_time_convert(hour)
             csv_array.append([month, day_in_month, hour_in_day, hour, hour_load])
         return csv_array
 
     @staticmethod
     def get_g_function_data(design):
-        csv_array = [["ln(t/ts)", f"H:{design.ghe.bhe.b.H:0.2f}"]]
-        ghe_gf_adjusted = design.ghe.grab_g_function(design.ghe.B_spacing / float(design.ghe.bhe.b.H))
-        gfunction_log_vals = ghe_gf_adjusted.x
-        gfunction_g_vals = ghe_gf_adjusted.y
-        for log_val, g_val in zip(gfunction_log_vals, gfunction_g_vals):
-            csv_array.append([log_val, g_val])
+        title = f"H:{design.ghe.bhe.b.H:0.2f}"
+        csv_array = [["ln(t/ts)", f"{title}", f"{title}_bhw"]]
+        gf_adjusted, gf_bhw_adjusted = design.ghe.grab_g_function(design.ghe.B_spacing / float(design.ghe.bhe.b.H))
+
+        gf_log_vals = gf_adjusted.x
+        gf_g_vals = gf_adjusted.y
+
+        gf_bhw_g_vals = gf_bhw_adjusted.y
+
+        for log_val, g_val, g_bhw_val in zip(gf_log_vals, gf_g_vals, gf_bhw_g_vals):
+            csv_array.append([log_val, g_val, g_bhw_val])
         return csv_array
 
     @staticmethod
     def get_timestep_str(load_method: TimestepType):
         if load_method == TimestepType.HYBRID:
             return TimestepType.HYBRID.name
         if load_method == TimestepType.HOURLY:
```

### Comparing `GHEDesigner-1.0/ghedesigner/radial_numerical_borehole.py` & `GHEDesigner-1.1/ghedesigner/radial_numerical_borehole.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,68 +1,54 @@
+from enum import auto, IntEnum
 from math import exp, log, pi, sqrt
 
 import numpy as np
 from scipy.interpolate import interp1d
 from scipy.linalg.lapack import dgtsv
 
 from ghedesigner.borehole_heat_exchangers import SingleUTube
 from ghedesigner.constants import TWO_PI
 
 
-class RadialCellType(object):
-    FLUID = 1
-    CONVECTION = 2
-    PIPE = 3
-    GROUT = 4
-    SOIL = 5
+class CellProps(IntEnum):
+    R_IN = 0
+    R_CENTER = auto()
+    R_OUT = auto()
+    K = auto()
+    RHO_CP = auto()
+    TEMP = auto()
+    VOL = auto()
 
 
 class RadialNumericalBH(object):
     """
     X. Xu and Jeffrey D. Spitler. 2006. 'Modeling of Vertical Ground Loop Heat
     Exchangers with Variable Convective Resistance and Thermal Mass of the
     Fluid.' in Proceedings of the 10th International Conference on Thermal
     Energy Storage-EcoStock. Pomona, NJ, May 31-June 2.
     """
 
-    def __init__(
-            self,
-            single_u_tube: SingleUTube,
-            ground_init_temp: float = 20.0,
-            data_type: np.dtype = np.double,
-    ):
+    def __init__(self, single_u_tube: SingleUTube):
         self.single_u_tube = single_u_tube
-        self.dtype = data_type
-
-        self.cell_inputs = {
-            "type": 0,
-            "inner-radius": 1,
-            "center-radius": 2,
-            "outer-radius": 3,
-            "thickness": 4,
-            "conductivity": 5,
-            "heat-capacity": 6,
-            "initial-temperature": 7,
-            "volume": 8,
-        }
 
         # "The one dimensional model has a fluid core, an equivalent convective
         # resistance layer, a tube layer, a grout layer and is surrounded by the
         # ground."
 
         # cell numbers
         self.num_fluid_cells = 3
         self.num_conv_cells = 1
         self.num_pipe_cells = 4
         self.num_grout_cells = 27
         self.num_soil_cells = 500
 
-        self.num_cells = \
-            self.num_fluid_cells + self.num_conv_cells + self.num_fluid_cells + self.num_grout_cells + \
-            self.num_soil_cells + 1
+        self.num_cells = self.num_fluid_cells + self.num_conv_cells + self.num_fluid_cells
+        self.num_cells += self.num_grout_cells + self.num_soil_cells + 1
+
+        self.bh_wall_idx = self.num_fluid_cells + self.num_conv_cells + self.num_pipe_cells + self.num_grout_cells
 
         # Geometry and grid procedure
 
         # far-field radius is set to 10m; the soil region is represented by
         # 500 cells
         far_field_radius = 10  # soil radius (in meters)
         self.r_far_field = far_field_radius - single_u_tube.b.r_b
@@ -87,19 +73,20 @@
         self.thickness_soil = (self.r_far_field - self.r_borehole) / self.num_soil_cells
         self.thickness_grout = (self.r_borehole - self.r_out_tube) / self.num_grout_cells
         # pipe thickness is equivalent to original tube thickness
         self.thickness_conv = (self.r_in_tube - self.r_in_convection) / self.num_conv_cells
         self.thickness_fluid = (self.r_in_convection - self.r_fluid) / self.num_fluid_cells
 
         # other
-        self.init_temp = ground_init_temp
+        self.init_temp = 20
 
         # other
-        self.g = np.array([], dtype=self.dtype)
-        self.lntts = np.array([], dtype=self.dtype)
+        self.g = np.array([], dtype=np.double)
+        self.g_bhw = np.array([], dtype=np.double)
+        self.lntts = np.array([], dtype=np.double)
         self.c_0 = TWO_PI * single_u_tube.soil.k
         soil_diffusivity = single_u_tube.k_s / single_u_tube.soil.rhoCp
         self.t_s = single_u_tube.b.H ** 2 / (9 * soil_diffusivity)
         # default is at least 49 hours, or up to -8.6 log time
         self.calc_time_in_sec = max([self.t_s * exp(-8.6), 49.0 * 3600.0])
         self.g_sts = None
 
@@ -122,333 +109,272 @@
         num_grout_cells = self.num_grout_cells
         num_soil_cells = self.num_soil_cells
 
         cell_summation = 0
 
         # load fluid cells
         for idx in range(cell_summation, num_fluid_cells + cell_summation):
-            cell_type = RadialCellType.FLUID
-            thickness = self.thickness_fluid
-            center_radius = self.r_fluid + idx * thickness
+            center_radius = self.r_fluid + idx * self.thickness_fluid
 
             if idx == 0:
                 inner_radius = center_radius
             else:
-                inner_radius = center_radius - thickness / 2.0
+                inner_radius = center_radius - self.thickness_fluid / 2.0
 
-            outer_radius = center_radius + thickness / 2.0
+            outer_radius = center_radius + self.thickness_fluid / 2.0
 
             # The equivalent thermal mass of the fluid can be calculated from
             # equation (2)
             # pi (r_in_conv ** 2 - r_f **2) C_eq_f = 2pi r_p_in**2 * C_f
             rho_cp_eq = (2.0
                          * (self.single_u_tube.pipe.r_in ** 2)
                          * self.single_u_tube.fluid.rhoCp
                          ) / ((self.r_in_convection ** 2) - (self.r_fluid ** 2))
 
             k_eq = rho_cp_eq / self.single_u_tube.fluid.cp
 
             volume = pi * (outer_radius ** 2 - inner_radius ** 2)
             radial_cell[:, idx] = np.array(
                 [
-                    cell_type,
                     inner_radius,
                     center_radius,
                     outer_radius,
-                    thickness,
                     k_eq,
                     rho_cp_eq,
                     self.init_temp,
                     volume,
                 ],
-                dtype=self.dtype,
+                dtype=np.double,
             )
         cell_summation += num_fluid_cells
 
         # TODO: verify whether errors are possible here and raise exception if needed
         # assert cell_summation == num_fluid_cells
 
         # load convection cells
         for idx in range(cell_summation, num_conv_cells + cell_summation):
             j = idx - cell_summation
-            cell_type = RadialCellType.CONVECTION
-            thickness = self.thickness_conv
-            inner_radius = self.r_in_convection + j * thickness
-            center_radius = inner_radius + thickness / 2.0
-            outer_radius = inner_radius + thickness
+            inner_radius = self.r_in_convection + j * self.thickness_conv
+            center_radius = inner_radius + self.thickness_conv / 2.0
+            outer_radius = inner_radius + self.thickness_conv
             k_eq = log(self.r_in_tube / self.r_in_convection) / (TWO_PI * resist_f_eq)
             rho_cp = 1.0
             volume = pi * (outer_radius ** 2 - inner_radius ** 2)
             radial_cell[:, idx] = np.array(
                 [
-                    cell_type,
                     inner_radius,
                     center_radius,
                     outer_radius,
-                    thickness,
                     k_eq,
                     rho_cp,
                     self.init_temp,
                     volume,
                 ],
-                dtype=self.dtype,
+                dtype=np.double,
             )
         cell_summation += num_conv_cells
 
         # TODO: verify whether errors are possible here and raise exception if needed
         # assert cell_summation == (num_fluid_cells + num_conv_cells)
 
         # load pipe cells
         for idx in range(cell_summation, num_pipe_cells + cell_summation):
             j = idx - cell_summation
-            cell_type = RadialCellType.PIPE
-            thickness = self.thickness_pipe
-            inner_radius = self.r_in_tube + j * thickness
-            center_radius = inner_radius + thickness / 2.0
-            outer_radius = inner_radius + thickness
+            inner_radius = self.r_in_tube + j * self.thickness_pipe
+            center_radius = inner_radius + self.thickness_pipe / 2.0
+            outer_radius = inner_radius + self.thickness_pipe
             conductivity = log(self.r_borehole / self.r_in_tube) / (TWO_PI * resist_p_eq)
             rho_cp = self.single_u_tube.pipe.rhoCp
             volume = pi * (outer_radius ** 2 - inner_radius ** 2)
             radial_cell[:, idx] = np.array(
                 [
-                    cell_type,
                     inner_radius,
                     center_radius,
                     outer_radius,
-                    thickness,
                     conductivity,
                     rho_cp,
                     self.init_temp,
                     volume,
                 ],
-                dtype=self.dtype,
+                dtype=np.double,
             )
         cell_summation += num_pipe_cells
 
         # TODO: verify whether errors are possible here and raise exception if needed
         # assert cell_summation == (num_fluid_cells + num_conv_cells + num_pipe_cells)
 
         # load grout cells
         for idx in range(cell_summation, num_grout_cells + cell_summation):
             j = idx - cell_summation
-            cell_type = RadialCellType.GROUT
-            thickness = self.thickness_grout
-            inner_radius = self.r_out_tube + j * thickness
-            center_radius = inner_radius + thickness / 2.0
-            outer_radius = inner_radius + thickness
+            inner_radius = self.r_out_tube + j * self.thickness_grout
+            center_radius = inner_radius + self.thickness_grout / 2.0
+            outer_radius = inner_radius + self.thickness_grout
             conductivity = log(self.r_borehole / self.r_in_tube) / (TWO_PI * resist_tg_eq)
             rho_cp = self.single_u_tube.grout.rhoCp
             volume = pi * (outer_radius ** 2 - inner_radius ** 2)
             radial_cell[:, idx] = np.array(
                 [
-                    cell_type,
                     inner_radius,
                     center_radius,
                     outer_radius,
-                    thickness,
                     conductivity,
                     rho_cp,
                     self.init_temp,
                     volume,
                 ],
-                dtype=self.dtype,
+                dtype=np.double,
             )
         cell_summation += num_grout_cells
 
         # TODO: verify whether errors are possible here and raise exception if needed
         # assert cell_summation == (num_fluid_cells + num_conv_cells + num_pipe_cells + num_grout_cells)
 
         # load soil cells
         for idx in range(cell_summation, num_soil_cells + cell_summation):
             j = idx - cell_summation
-            cell_type = RadialCellType.SOIL
-            thickness = self.thickness_soil
-            inner_radius = self.r_borehole + j * thickness
-            center_radius = inner_radius + thickness / 2.0
-            outer_radius = inner_radius + thickness
+            inner_radius = self.r_borehole + j * self.thickness_soil
+            center_radius = inner_radius + self.thickness_soil / 2.0
+            outer_radius = inner_radius + self.thickness_soil
             conductivity = self.single_u_tube.soil.k
             rho_cp = self.single_u_tube.soil.rhoCp
             volume = pi * (outer_radius ** 2 - inner_radius ** 2)
             radial_cell[:, idx] = np.array(
                 [
-                    cell_type,
                     inner_radius,
                     center_radius,
                     outer_radius,
-                    thickness,
                     conductivity,
                     rho_cp,
                     self.init_temp,
                     volume,
                 ],
-                dtype=self.dtype,
+                dtype=np.double,
             )
         cell_summation += num_soil_cells
 
-    def calc_sts_g_functions(self, single_u_tube, final_time=None, calculate_at_bh_wall=False) -> tuple:
+    def calc_sts_g_functions(self, single_u_tube, final_time=None) -> tuple:
 
         self.partial_init(single_u_tube)
 
         resist_bh_effective = self.single_u_tube.calc_effective_borehole_resistance()
 
         resist_f_eq = self.single_u_tube.R_f / 2.0
         resist_p_eq = self.single_u_tube.R_p / 2.0
         resist_tg_eq = resist_bh_effective - resist_f_eq
 
         # Pass radial cell by reference and fill here so that it can be
         # destroyed when this method returns
-        radial_cell = np.zeros(
-            shape=(len(self.cell_inputs), self.num_cells), dtype=self.dtype
-        )
+        radial_cell = np.zeros(shape=(len(CellProps), self.num_cells), dtype=np.double)
         self.fill_radial_cell(radial_cell, resist_p_eq, resist_f_eq, resist_tg_eq)
 
         if final_time is None:
             final_time = self.calc_time_in_sec
 
         g = []
+        g_bhw = []
         lntts = []
 
         _dl = np.zeros(self.num_cells - 1)
         _d = np.zeros(self.num_cells)
         _du = np.zeros(self.num_cells - 1)
         _b = np.zeros(self.num_cells)
 
         heat_flux = 1.0
         init_temp = self.init_temp
 
         time = 1e-12 - 120
         time_step = 120
 
-        # type_idx = self.cell_inputs["type"]
-        r_in_idx = self.cell_inputs["inner-radius"]
-        r_center_idx = self.cell_inputs["center-radius"]
-        r_out_idx = self.cell_inputs["outer-radius"]
-        # thickness_idx = self.cell_inputs["thickness"]
-        k_idx = self.cell_inputs["conductivity"]
-        rho_cp_idx = self.cell_inputs["heat-capacity"]
-        temperature_idx = self.cell_inputs["initial-temperature"]
-        previous_temperature_idx = self.cell_inputs["initial-temperature"]
-        volume_idx = self.cell_inputs["volume"]
-
-        _fe_1 = np.zeros(shape=(self.num_cells - 2), dtype=self.dtype)
+        _fe_1 = np.zeros(shape=(self.num_cells - 2), dtype=np.double)
         _fe_2 = np.zeros_like(_fe_1)
         _ae = np.zeros_like(_fe_2)
         _fw_1 = np.zeros_like(_ae)
         _fw_2 = np.zeros_like(_fw_1)
         _aw = np.zeros_like(_fw_2)
         _ad = np.zeros_like(_aw)
 
         _west_cell = radial_cell[:, 0: self.num_cells - 2]
         _center_cell = radial_cell[:, 1: self.num_cells - 1]
         _east_cell = radial_cell[:, 2: self.num_cells - 0]
 
-        fe_1 = log(radial_cell[r_out_idx, 0] / radial_cell[r_center_idx, 0]) / (TWO_PI * radial_cell[k_idx, 0])
-        fe_2 = log(radial_cell[r_center_idx, 1] / radial_cell[r_in_idx, 1]) / (TWO_PI * radial_cell[k_idx, 1])
+        fe_1 = log(radial_cell[CellProps.R_OUT, 0] / radial_cell[CellProps.R_CENTER, 0])
+        fe_1 /= (TWO_PI * radial_cell[CellProps.K, 0])
+
+        fe_2 = log(radial_cell[CellProps.R_CENTER, 1] / radial_cell[CellProps.R_IN, 1])
+        fe_2 /= (TWO_PI * radial_cell[CellProps.K, 1])
+
         ae = 1 / (fe_1 + fe_2)
-        ad = radial_cell[rho_cp_idx, 0] * radial_cell[volume_idx, 0] / time_step
+        ad = radial_cell[CellProps.RHO_CP, 0] * radial_cell[CellProps.VOL, 0] / time_step
         _d[0] = -ae / ad - 1
         _du[0] = ae / ad
 
         def fill_f1(fx_1, cell):
-            fx_1[:] = np.log(cell[r_out_idx, :] / cell[r_center_idx, :]) / (TWO_PI * cell[k_idx, :])
+            fx_1[:] = np.log(cell[CellProps.R_OUT, :] / cell[CellProps.R_CENTER, :]) / (TWO_PI * cell[CellProps.K, :])
 
         def fill_f2(fx_2, cell):
-            fx_2[:] = np.log(cell[r_center_idx, :] / cell[r_in_idx, :]) / (TWO_PI * cell[k_idx, :])
+            fx_2[:] = np.log(cell[CellProps.R_CENTER, :] / cell[CellProps.R_IN, :]) / (TWO_PI * cell[CellProps.K, :])
 
         fill_f1(_fe_1, _center_cell)
         fill_f2(_fe_2, _east_cell)
         _ae[:] = 1.0 / (_fe_1 + _fe_2)
 
         fill_f1(_fw_1, _west_cell)
         fill_f2(_fw_2, _center_cell)
         _aw[:] = -1.0 / (_fw_1 + _fw_2)
 
-        _ad[:] = (_center_cell[rho_cp_idx, :] * _center_cell[volume_idx, :] / time_step)
+        _ad[:] = (_center_cell[CellProps.RHO_CP, :] * _center_cell[CellProps.VOL, :] / time_step)
         _dl[0: self.num_cells - 2] = -_aw / _ad
         _d[1: self.num_cells - 1] = _aw / _ad - _ae / _ad - 1.0
         _du[1: self.num_cells - 1] = _ae / _ad
 
         while True:
 
             time += time_step
 
             # For the idx == 0 case:
 
-            _b[0] = -radial_cell[previous_temperature_idx, 0] - heat_flux / ad
+            _b[0] = -radial_cell[CellProps.TEMP, 0] - heat_flux / ad
 
             # For the idx == n-1 case
 
             _dl[self.num_cells - 2] = 0.0
             _d[self.num_cells - 1] = 1.0
-            _b[self.num_cells - 1] = radial_cell[previous_temperature_idx, self.num_cells - 1]
+            _b[self.num_cells - 1] = radial_cell[CellProps.TEMP, self.num_cells - 1]
 
             # Now handle the 1 to n-2 cases with numpy slicing and vectorization
-            _b[1: self.num_cells - 1] = -radial_cell[previous_temperature_idx, 1: self.num_cells - 1]
+            _b[1: self.num_cells - 1] = -radial_cell[CellProps.TEMP, 1: self.num_cells - 1]
 
             # Tri-diagonal matrix solver
             # High level interface to LAPACK routine
             # https://docs.scipy.org/doc/scipy/reference/generated/scipy.linalg.lapack.dgtsv.html#scipy.linalg.lapack.dgtsv
             dgtsv(_dl, _d, _du, _b, overwrite_b=1)  # TODO: Do we really need lapack just to do a TDMA solution?
 
-            radial_cell[previous_temperature_idx, :] = _b
-            radial_cell[temperature_idx, :] = _b
+            radial_cell[CellProps.TEMP, :] = _b
 
-            if calculate_at_bh_wall:
-                raise ValueError(
-                    "This portion of the code does not currently run with this "
-                    "vectorized radial numerical implementation."
-                )
-                # bh_wall_temp = 0
-                #
-                # # calculate bh wall temp
-                # for idx, _ in enumerate(self.cells):
-                #     west_cell = self.cells[idx]
-                #     east_cell = self.cells[idx + 1]
-                #
-                #     if (
-                #         west_cell.type == RadialCellType.GROUT
-                #         and east_cell.type == RadialCellType.SOIL
-                #     ):
-                #         west_conductance_num = 2 * pi * west_cell.conductivity
-                #         west_conductance_den = log(
-                #             west_cell.outer_radius / west_cell.inner_radius
-                #         )
-                #         west_conductance = west_conductance_num / west_conductance_den
-                #
-                #         east_conductance_num = 2 * pi * east_cell.conductivity
-                #         east_conductance_den = log(
-                #             east_cell.center_radius / west_cell.inner_radius
-                #         )
-                #         east_conductance = east_conductance_num / east_conductance_den
-                #
-                #         bh_wall_temp_num_1 = west_conductance * west_cell.temperature
-                #         bh_wall_temp_num_2 = east_conductance * east_cell.temperature
-                #         bh_wall_temp_num = bh_wall_temp_num_1 + bh_wall_temp_num_2
-                #         bh_wall_temp_den = west_conductance + east_conductance
-                #         bh_wall_temp = bh_wall_temp_num / bh_wall_temp_den
-                #
-                #         break
-                #
-                # g.append(self.c_0 * ((bh_wall_temp - init_temp) / heat_flux))
-            else:
-                g.append(
-                    self.c_0
-                    * ((radial_cell[temperature_idx, 0] - init_temp) / heat_flux - resist_bh_effective)
-                )
+            # compute standard g-functions
+            g.append(self.c_0 * ((radial_cell[CellProps.TEMP, 0] - init_temp) / heat_flux - resist_bh_effective))
+
+            # compute g-functions at bh wall
+            bh_wall_temp = radial_cell[CellProps.TEMP, self.bh_wall_idx]
+            g_bhw.append(self.c_0 * ((bh_wall_temp - init_temp) / heat_flux))
 
             lntts.append(log(time / self.t_s))
 
             if time >= final_time - time_step:
                 break
 
         # quickly chop down the total values to a more manageable set
         num_intervals = 30
-        g_sts_temp = interp1d(lntts, g)
+        g_tmp = interp1d(lntts, g)
         uniform_lntts_vals = np.linspace(lntts[0], lntts[-1], num_intervals)
-        uniform_g_vals = g_sts_temp(uniform_lntts_vals)
+        uniform_g_vals = g_tmp(uniform_lntts_vals)
+
+        g_bhw_tmp = interp1d(lntts, g_bhw)
+        uniform_g_bhw_vals = g_bhw_tmp(uniform_lntts_vals)
 
         # set the final arrays and interpolator objects
         self.lntts = np.array(uniform_lntts_vals)
         self.g = np.array(uniform_g_vals)
+        self.g_bhw = np.array(uniform_g_bhw_vals)
         self.g_sts = interp1d(self.lntts, self.g)
 
         return self.lntts, self.g
```

### Comparing `GHEDesigner-1.0/ghedesigner/rowwise.py` & `GHEDesigner-1.1/ghedesigner/rowwise.py`

 * *Files identical despite different names*

### Comparing `GHEDesigner-1.0/ghedesigner/search_routines.py` & `GHEDesigner-1.1/ghedesigner/search_routines.py`

 * *Files identical despite different names*

### Comparing `GHEDesigner-1.0/ghedesigner/shape.py` & `GHEDesigner-1.1/ghedesigner/shape.py`

 * *Files 14% similar despite different names*

```diff
@@ -211,7 +211,74 @@
             # return [[x11,y11],[x12,y12]]
             return []
         else:
             return []
     rx = (c2 - c1) / (a1 - a2)
     ry = a1 * (c2 - c1) / (a1 - a2) + c1
     return [[rx, ry]]
+
+
+def point_polygon_check(contour, point):
+    """
+    Mimics pointPolygonTest from OpenCV-Python
+
+    Adapted from the methods outlined in the links below.
+    https://stackoverflow.com/a/63436180/5965685
+    https://stackoverflow.com/a/17693146/5965685
+
+    :param contour: list of tuples containing (x, y) contour boundary points
+    :param point: tuple containing the (x, y) point to test
+
+    :returns: -1 if outside, 0 if on edge, 1 if inside
+    :rtype: int
+    """
+
+    # check if on edge
+    # use Pythagoras to check whether the distance between the test point
+    # and the line vertices add to the distance between the line vertices
+    # if they are within tolerance, the point is co-linear
+    # if not, it is off the line
+
+    def distance(pt_1, pt_2) -> float:
+        return sqrt((pt_1[0] - pt_2[0]) ** 2 + (pt_1[1] - pt_2[1]) ** 2)
+
+    on_edge_tolerance = 0.001
+
+    for idx, vertex in enumerate(contour):
+        v1 = contour[idx - 1]
+        v2 = vertex
+        test_dist = distance(v1, point) + distance(v2, point)
+        v12_dist = distance(v1, v2)
+
+        if abs(test_dist - v12_dist) < on_edge_tolerance:
+            return 0
+
+    # if made it to here, not on edge and check if inside/outside
+    def between(p, a, b) -> bool:
+        return ((p >= a) and (p <= b)) or ((p <= a) and (p >= b))
+
+    inside = True
+    px = point[0]
+    py = point[1]
+
+    for idx, vertex in enumerate(contour):
+        v1 = contour[idx - 1]
+        v2 = vertex
+        v1x = v1[0]
+        v1y = v1[1]
+        v2x = v2[0]
+        v2y = v2[1]
+
+        if between(py, v1y, v2y):  # points inside vertical range
+            if ((py == v1y) and (v2y >= v1y)) or ((py == v2y) and (v1y >= v2y)):
+                continue
+
+            # calc cross product `PA X PB`, P lays on left side of AB if c > 0
+            c = (v1x - px) * (v2y - py) - (v2x - px) * (v1y - py)
+
+            if c == 0:
+                return 0
+
+            if (v1y < v2y) == (c > 0):
+                inside = not inside
+
+    return -1 if inside else 1
```

### Comparing `GHEDesigner-1.0/ghedesigner/simulation.py` & `GHEDesigner-1.1/ghedesigner/simulation.py`

 * *Files identical despite different names*

### Comparing `GHEDesigner-1.0/ghedesigner/utilities.py` & `GHEDesigner-1.1/ghedesigner/utilities.py`

 * *Files identical despite different names*

### Comparing `GHEDesigner-1.0/ghedesigner/validate.py` & `GHEDesigner-1.1/ghedesigner/validate.py`

 * *Files identical despite different names*

### Comparing `GHEDesigner-1.0/setup.py` & `GHEDesigner-1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 setup(
     name='GHEDesigner',
     install_requires=[
         'click>=8.1.3',
         'jsonschema>=4.17.3',
         'numpy>=1.24.2',
-        'opencv-python==4.7.0.68',
         'pygfunction>=2.2.2',
         'scipy>=1.10.0'
     ],
     url='https://github.com/BETSRG/GHEDesigner',
     description=short_description,
     license='BSD-3',
     long_description=readme_contents,
@@ -36,10 +35,11 @@
         'console_scripts': ['ghedesigner=ghedesigner.manager:run_manager_from_cli']
     },
     python_requires='>=3.8',
     classifiers=[
         'Topic :: Scientific/Engineering',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10'
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11'
     ]
 )
```

