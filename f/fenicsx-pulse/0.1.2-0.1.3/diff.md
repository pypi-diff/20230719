# Comparing `tmp/fenicsx-pulse-0.1.2.tar.gz` & `tmp/fenicsx-pulse-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenicsx-pulse-0.1.2.tar", last modified: Sat Jan  7 07:33:59 2023, max compression
+gzip compressed data, was "fenicsx-pulse-0.1.3.tar", last modified: Wed Jul 19 14:45:15 2023, max compression
```

## Comparing `fenicsx-pulse-0.1.2.tar` & `fenicsx-pulse-0.1.3.tar`

### file list

```diff
@@ -1,30 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 07:33:59.145778 fenicsx-pulse-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-01-07 07:33:43.000000 fenicsx-pulse-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-01-07 07:33:59.145778 fenicsx-pulse-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-01-07 07:33:43.000000 fenicsx-pulse-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-01-07 07:33:43.000000 fenicsx-pulse-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-07 07:33:59.145778 fenicsx-pulse-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 07:33:59.141778 fenicsx-pulse-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 07:33:59.145778 fenicsx-pulse-0.1.2/src/fenicsx_pulse/
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-01-07 07:33:43.000000 fenicsx-pulse-0.1.2/src/fenicsx_pulse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-07 07:33:43.000000 fenicsx-pulse-0.1.2/src/fenicsx_pulse/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-01-07 07:33:43.000000 fenicsx-pulse-0.1.2/src/fenicsx_pulse/active_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-01-07 07:33:43.000000 fenicsx-pulse-0.1.2/src/fenicsx_pulse/active_stress.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-01-07 07:33:43.000000 fenicsx-pulse-0.1.2/src/fenicsx_pulse/boundary_conditions.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-01-07 07:33:43.000000 fenicsx-pulse-0.1.2/src/fenicsx_pulse/cardiac_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-01-07 07:33:43.000000 fenicsx-pulse-0.1.2/src/fenicsx_pulse/compressibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-01-07 07:33:43.000000 fenicsx-pulse-0.1.2/src/fenicsx_pulse/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-01-07 07:33:43.000000 fenicsx-pulse-0.1.2/src/fenicsx_pulse/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-01-07 07:33:43.000000 fenicsx-pulse-0.1.2/src/fenicsx_pulse/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-01-07 07:33:43.000000 fenicsx-pulse-0.1.2/src/fenicsx_pulse/holzapfelogden.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-01-07 07:33:43.000000 fenicsx-pulse-0.1.2/src/fenicsx_pulse/invariants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-01-07 07:33:43.000000 fenicsx-pulse-0.1.2/src/fenicsx_pulse/kinematics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-01-07 07:33:43.000000 fenicsx-pulse-0.1.2/src/fenicsx_pulse/linear_elastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-01-07 07:33:43.000000 fenicsx-pulse-0.1.2/src/fenicsx_pulse/material_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-01-07 07:33:43.000000 fenicsx-pulse-0.1.2/src/fenicsx_pulse/mechanicsproblem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 07:33:59.145778 fenicsx-pulse-0.1.2/src/fenicsx_pulse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-01-07 07:33:59.000000 fenicsx-pulse-0.1.2/src/fenicsx_pulse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-01-07 07:33:59.000000 fenicsx-pulse-0.1.2/src/fenicsx_pulse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-07 07:33:59.000000 fenicsx-pulse-0.1.2/src/fenicsx_pulse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-01-07 07:33:59.000000 fenicsx-pulse-0.1.2/src/fenicsx_pulse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-07 07:33:59.000000 fenicsx-pulse-0.1.2/src/fenicsx_pulse.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:45:15.687528 fenicsx-pulse-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-19 14:45:00.000000 fenicsx-pulse-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-07-19 14:45:15.687528 fenicsx-pulse-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-07-19 14:45:00.000000 fenicsx-pulse-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-19 14:45:00.000000 fenicsx-pulse-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 14:45:15.687528 fenicsx-pulse-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:45:15.683528 fenicsx-pulse-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:45:15.687528 fenicsx-pulse-0.1.3/src/fenicsx_pulse/
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-19 14:45:00.000000 fenicsx-pulse-0.1.3/src/fenicsx_pulse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-19 14:45:00.000000 fenicsx-pulse-0.1.3/src/fenicsx_pulse/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-19 14:45:00.000000 fenicsx-pulse-0.1.3/src/fenicsx_pulse/active_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-19 14:45:00.000000 fenicsx-pulse-0.1.3/src/fenicsx_pulse/active_stress.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-19 14:45:00.000000 fenicsx-pulse-0.1.3/src/fenicsx_pulse/boundary_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-19 14:45:00.000000 fenicsx-pulse-0.1.3/src/fenicsx_pulse/cardiac_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-19 14:45:00.000000 fenicsx-pulse-0.1.3/src/fenicsx_pulse/compressibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-07-19 14:45:00.000000 fenicsx-pulse-0.1.3/src/fenicsx_pulse/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-19 14:45:00.000000 fenicsx-pulse-0.1.3/src/fenicsx_pulse/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-07-19 14:45:00.000000 fenicsx-pulse-0.1.3/src/fenicsx_pulse/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-07-19 14:45:00.000000 fenicsx-pulse-0.1.3/src/fenicsx_pulse/holzapfelogden.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-19 14:45:00.000000 fenicsx-pulse-0.1.3/src/fenicsx_pulse/invariants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-07-19 14:45:00.000000 fenicsx-pulse-0.1.3/src/fenicsx_pulse/kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-19 14:45:00.000000 fenicsx-pulse-0.1.3/src/fenicsx_pulse/linear_elastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-19 14:45:00.000000 fenicsx-pulse-0.1.3/src/fenicsx_pulse/material_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-07-19 14:45:00.000000 fenicsx-pulse-0.1.3/src/fenicsx_pulse/mechanicsproblem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:45:15.687528 fenicsx-pulse-0.1.3/src/fenicsx_pulse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-07-19 14:45:15.000000 fenicsx-pulse-0.1.3/src/fenicsx_pulse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-19 14:45:15.000000 fenicsx-pulse-0.1.3/src/fenicsx_pulse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 14:45:15.000000 fenicsx-pulse-0.1.3/src/fenicsx_pulse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-19 14:45:15.000000 fenicsx-pulse-0.1.3/src/fenicsx_pulse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-19 14:45:15.000000 fenicsx-pulse-0.1.3/src/fenicsx_pulse.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:45:15.687528 fenicsx-pulse-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-19 14:45:00.000000 fenicsx-pulse-0.1.3/tests/test_active_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-19 14:45:00.000000 fenicsx-pulse-0.1.3/tests/test_cardiac_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-19 14:45:00.000000 fenicsx-pulse-0.1.3/tests/test_compressibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-19 14:45:00.000000 fenicsx-pulse-0.1.3/tests/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-07-19 14:45:00.000000 fenicsx-pulse-0.1.3/tests/test_invariants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-07-19 14:45:00.000000 fenicsx-pulse-0.1.3/tests/test_kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-07-19 14:45:00.000000 fenicsx-pulse-0.1.3/tests/test_material_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-07-19 14:45:00.000000 fenicsx-pulse-0.1.3/tests/test_mechanicsproblem.py
```

### Comparing `fenicsx-pulse-0.1.2/LICENSE` & `fenicsx-pulse-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fenicsx-pulse-0.1.2/PKG-INFO` & `fenicsx-pulse-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenicsx-pulse
-Version: 0.1.2
+Version: 0.1.3
 Summary: Next generation cardiac mechanics solver based on FEniCSx
 Author-email: Henrik Finsberg <henriknf@simula.no>
 License: Copyright 2022 Henrik Finsberg
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -22,15 +22,15 @@
 [![MIT](https://img.shields.io/github/license/finsberg/fenicsx-pulse)](https://github.com/finsberg/fenicsx-pulse/blob/main/LICENSE)
 [![PyPI version](https://badge.fury.io/py/fenicsx-pulse.svg)](https://pypi.org/project/fenicsx_pulse/)
 [![Test package](https://github.com/finsberg/fenicsx-pulse/actions/workflows/test_package_coverage.yml/badge.svg)](https://github.com/finsberg/fenicsx-pulse/actions/workflows/test_package_coverage.yml)
 [![Pre-commit](https://github.com/finsberg/fenicsx-pulse/actions/workflows/pre-commit.yml/badge.svg)](https://github.com/finsberg/fenicsx-pulse/actions/workflows/pre-commit.yml)
 [![Deploy static content to Pages](https://github.com/finsberg/fenicsx-pulse/actions/workflows/build_docs.yml/badge.svg)](https://github.com/finsberg/fenicsx-pulse/actions/workflows/build_docs.yml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Create and publish a Docker image](https://github.com/finsberg/fenicsx-pulse/actions/workflows/docker-image.yml/badge.svg)](https://github.com/finsberg/fenicsx-pulse/pkgs/container/fenicsx_pulse)
-
+[![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/finsberg/a7290de789564f03eb6b1ee122fce423/raw/fenicsx-pulse-coverage.json)](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/finsberg/a7290de789564f03eb6b1ee122fce423/raw/fenicsx-pulse-coverage.json)
 
 # fenicsx-pulse
 
 `fenicsx-pulse` is a cardiac mechanics solver based on FEniCSx. It is a successor of [`pulse`](https://github.com/finsberg/pulse) which is a cardiac mechanics solver based on FEniCS.
 
 ---
 
@@ -49,15 +49,15 @@
 
 To install `fenicsx_pulse` you need to first [install FEniCSx](https://github.com/FEniCS/dolfinx#installation). Next you can install `fenicsx_pulse` via pip
 ```
 python3 -m pip install fenicsx-pulse
 ```
 We also provide a pre-built docker image with FEniCSx and `fenicsx_pulse` installed. You pull this image using the command
 ```
-docker pull ghcr.io/finsberg/fenicsx-pulse:v0.1.2
+docker pull ghcr.io/finsberg/fenicsx-pulse:v0.1.3
 ```
 
 ## Simple Example
 
 ```python
 import dolfinx
 import numpy as np
@@ -135,9 +135,8 @@
 xdmf.write_mesh(mesh)
 xdmf.write_function(u, 0.0)
 xdmf.write_function(p, 0.0)
 ```
 
 
 ## Contributing
-
-TBW
+See https://finsberg.github.io/fenicsx-pulse/CONTRIBUTING.html
```

### Comparing `fenicsx-pulse-0.1.2/README.md` & `fenicsx-pulse-0.1.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [![MIT](https://img.shields.io/github/license/finsberg/fenicsx-pulse)](https://github.com/finsberg/fenicsx-pulse/blob/main/LICENSE)
 [![PyPI version](https://badge.fury.io/py/fenicsx-pulse.svg)](https://pypi.org/project/fenicsx_pulse/)
 [![Test package](https://github.com/finsberg/fenicsx-pulse/actions/workflows/test_package_coverage.yml/badge.svg)](https://github.com/finsberg/fenicsx-pulse/actions/workflows/test_package_coverage.yml)
 [![Pre-commit](https://github.com/finsberg/fenicsx-pulse/actions/workflows/pre-commit.yml/badge.svg)](https://github.com/finsberg/fenicsx-pulse/actions/workflows/pre-commit.yml)
 [![Deploy static content to Pages](https://github.com/finsberg/fenicsx-pulse/actions/workflows/build_docs.yml/badge.svg)](https://github.com/finsberg/fenicsx-pulse/actions/workflows/build_docs.yml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Create and publish a Docker image](https://github.com/finsberg/fenicsx-pulse/actions/workflows/docker-image.yml/badge.svg)](https://github.com/finsberg/fenicsx-pulse/pkgs/container/fenicsx_pulse)
-
+[![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/finsberg/a7290de789564f03eb6b1ee122fce423/raw/fenicsx-pulse-coverage.json)](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/finsberg/a7290de789564f03eb6b1ee122fce423/raw/fenicsx-pulse-coverage.json)
 
 # fenicsx-pulse
 
 `fenicsx-pulse` is a cardiac mechanics solver based on FEniCSx. It is a successor of [`pulse`](https://github.com/finsberg/pulse) which is a cardiac mechanics solver based on FEniCS.
 
 ---
 
@@ -28,15 +28,15 @@
 
 To install `fenicsx_pulse` you need to first [install FEniCSx](https://github.com/FEniCS/dolfinx#installation). Next you can install `fenicsx_pulse` via pip
 ```
 python3 -m pip install fenicsx-pulse
 ```
 We also provide a pre-built docker image with FEniCSx and `fenicsx_pulse` installed. You pull this image using the command
 ```
-docker pull ghcr.io/finsberg/fenicsx-pulse:v0.1.2
+docker pull ghcr.io/finsberg/fenicsx-pulse:v0.1.3
 ```
 
 ## Simple Example
 
 ```python
 import dolfinx
 import numpy as np
@@ -114,9 +114,8 @@
 xdmf.write_mesh(mesh)
 xdmf.write_function(u, 0.0)
 xdmf.write_function(p, 0.0)
 ```
 
 
 ## Contributing
-
-TBW
+See https://finsberg.github.io/fenicsx-pulse/CONTRIBUTING.html
```

### Comparing `fenicsx-pulse-0.1.2/src/fenicsx_pulse/__init__.py` & `fenicsx-pulse-0.1.3/src/fenicsx_pulse/__init__.py`

 * *Files identical despite different names*

### Comparing `fenicsx-pulse-0.1.2/src/fenicsx_pulse/active_model.py` & `fenicsx-pulse-0.1.3/src/fenicsx_pulse/active_model.py`

 * *Files identical despite different names*

### Comparing `fenicsx-pulse-0.1.2/src/fenicsx_pulse/active_stress.py` & `fenicsx-pulse-0.1.3/src/fenicsx_pulse/active_stress.py`

 * *Files identical despite different names*

### Comparing `fenicsx-pulse-0.1.2/src/fenicsx_pulse/boundary_conditions.py` & `fenicsx-pulse-0.1.3/src/fenicsx_pulse/boundary_conditions.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,14 @@
 
 
 class BoundaryConditions(typing.NamedTuple):
     neumann: typing.Sequence[NeumannBC] = ()
     dirichlet: typing.Sequence[
         typing.Callable[
             [dolfinx.fem.FunctionSpace],
-            typing.Sequence[dolfinx.fem.bcs.DirichletBCMetaClass],
+            typing.Sequence[dolfinx.fem.bcs.DirichletBC],
         ]
     ] = ()
     robin: typing.Sequence[RobinBC] = ()
     body_force: typing.Sequence[
         float | dolfinx.fem.Constant | dolfinx.fem.Function
     ] = ()
```

### Comparing `fenicsx-pulse-0.1.2/src/fenicsx_pulse/cardiac_model.py` & `fenicsx-pulse-0.1.3/src/fenicsx_pulse/cardiac_model.py`

 * *Files identical despite different names*

### Comparing `fenicsx-pulse-0.1.2/src/fenicsx_pulse/compressibility.py` & `fenicsx-pulse-0.1.3/src/fenicsx_pulse/compressibility.py`

 * *Files identical despite different names*

### Comparing `fenicsx-pulse-0.1.2/src/fenicsx_pulse/exceptions.py` & `fenicsx-pulse-0.1.3/src/fenicsx_pulse/exceptions.py`

 * *Files identical despite different names*

### Comparing `fenicsx-pulse-0.1.2/src/fenicsx_pulse/geometry.py` & `fenicsx-pulse-0.1.3/src/fenicsx_pulse/geometry.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,42 +2,43 @@
 from dataclasses import dataclass
 from dataclasses import field
 from pathlib import Path
 from typing import NamedTuple
 
 import dolfinx
 import numpy as np
+import numpy.typing as npt
 import ufl
 
 from . import exceptions
 
 
 class Marker(NamedTuple):
     marker: int
     dim: int
-    locator: typing.Callable[[np.ndarray[np.float64]], bool]
+    locator: typing.Callable[[npt.NDArray[np.float64]], bool]
 
 
 @dataclass(slots=True)
 class Geometry:
     mesh: dolfinx.mesh.Mesh
     boundaries: typing.Sequence[Marker] = ()
     metadata: dict[str, typing.Any] = field(default_factory=dict)
-    _facet_indices: np.ndarray[np.int32] = field(init=False, repr=False)
-    _facet_markers: np.ndarray[np.int32] = field(init=False, repr=False)
-    _sorted_facets: np.ndarray[np.int32] = field(init=False, repr=False)
-    facet_tags: dolfinx.mesh.MeshTagsMetaClass = field(init=False, repr=False)
+    _facet_indices: npt.NDArray[np.int32] = field(init=False, repr=False)
+    _facet_markers: npt.NDArray[np.int32] = field(init=False, repr=False)
+    _sorted_facets: npt.NDArray[np.int32] = field(init=False, repr=False)
+    facet_tags: dolfinx.mesh.MeshTags = field(init=False, repr=False)
     dx: ufl.Measure = field(init=False, repr=False)
     ds: ufl.Measure = field(init=False, repr=False)
 
     def __post_init__(self) -> None:
         facet_indices, facet_markers = [], []
 
         # TODO: Handle when dim is not 2
-        for (marker, dim, locator) in self.boundaries:
+        for marker, dim, locator in self.boundaries:
             facets = dolfinx.mesh.locate_entities(self.mesh, dim, locator)
             facet_indices.append(facets)
             facet_markers.append(np.full_like(facets, marker))
 
         hstack = lambda x: np.array(x) if len(x) == 0 else np.hstack(x).astype(np.int32)
         self._facet_indices = hstack(facet_indices)
         self._facet_markers = hstack(facet_markers)
@@ -74,21 +75,22 @@
     def dim(self) -> int:
         return self.mesh.topology.dim
 
     def dump_mesh_tags(self, fname: str) -> None:
         if self.facet_tags.values.size == 0:
             raise exceptions.MeshTagNotFoundError
         self.mesh.topology.create_connectivity(self.facet_dimension, self.dim)
+
         with dolfinx.io.XDMFFile(
             self.mesh.comm,
             Path(fname).with_suffix(".xdmf"),
             "w",
         ) as xdmf:
             xdmf.write_mesh(self.mesh)
-            xdmf.write_meshtags(self.facet_tags)
+            xdmf.write_meshtags(self.facet_tags, x=self.mesh.geometry)
 
     @property
     def markers(self) -> tuple[int, ...]:
         return tuple(x[0] for x in self.boundaries)
 
     @property
     def facet_normal(self) -> ufl.FacetNormal:
```

### Comparing `fenicsx-pulse-0.1.2/src/fenicsx_pulse/holzapfelogden.py` & `fenicsx-pulse-0.1.3/src/fenicsx_pulse/holzapfelogden.py`

 * *Files identical despite different names*

### Comparing `fenicsx-pulse-0.1.2/src/fenicsx_pulse/invariants.py` & `fenicsx-pulse-0.1.3/src/fenicsx_pulse/invariants.py`

 * *Files identical despite different names*

### Comparing `fenicsx-pulse-0.1.2/src/fenicsx_pulse/kinematics.py` & `fenicsx-pulse-0.1.3/src/fenicsx_pulse/kinematics.py`

 * *Files identical despite different names*

### Comparing `fenicsx-pulse-0.1.2/src/fenicsx_pulse/linear_elastic.py` & `fenicsx-pulse-0.1.3/src/fenicsx_pulse/linear_elastic.py`

 * *Files identical despite different names*

### Comparing `fenicsx-pulse-0.1.2/src/fenicsx_pulse/material_model.py` & `fenicsx-pulse-0.1.3/src/fenicsx_pulse/material_model.py`

 * *Files identical despite different names*

### Comparing `fenicsx-pulse-0.1.2/src/fenicsx_pulse/mechanicsproblem.py` & `fenicsx-pulse-0.1.3/src/fenicsx_pulse/mechanicsproblem.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import typing
 from dataclasses import dataclass
 from dataclasses import field
 
-import dolfinx
+import dolfinx.fem.petsc
+import dolfinx.nls.petsc
 import ufl
 
 from . import kinematics
 from .boundary_conditions import BoundaryConditions
 from .cardiac_model import CardiacModel
 from .geometry import Geometry
 
@@ -18,15 +19,15 @@
     bcs: BoundaryConditions = field(default_factory=BoundaryConditions)
     _problem: dolfinx.fem.petsc.NonlinearProblem = field(init=False, repr=False)
     _solver: dolfinx.fem.petsc.NonlinearProblem = field(init=False, repr=False)
     state_space: dolfinx.fem.FunctionSpace = field(init=False, repr=False)
     state: dolfinx.fem.Function = field(init=False, repr=False)
     test_state: dolfinx.fem.Function = field(init=False, repr=False)
     _virtual_work: ufl.form.Form = field(init=False, repr=False)
-    _dirichlet_bc: typing.Sequence[dolfinx.fem.bcs.DirichletBCMetaClass] = field(
+    _dirichlet_bc: typing.Sequence[dolfinx.fem.bcs.DirichletBC] = field(
         init=False,
         repr=False,
     )
 
     def __post_init__(self):
         self._init_space()
         self._init_form()
@@ -71,15 +72,14 @@
         )
         # TODO: Make it possible for the user to set this
         self._solver.atol = 1e-8
         self._solver.rtol = 1e-8
         self._solver.convergence_criterion = "incremental"
 
     def _external_work(self, u, v):
-
         F = kinematics.DeformationGradient(u)
 
         N = self.geometry.facet_normal
         ds = self.geometry.ds
         dx = self.geometry.dx
 
         external_work = []
@@ -99,20 +99,18 @@
         if len(external_work) > 0:
             return sum(external_work)
 
         return None
 
     def _set_dirichlet_bc(self) -> None:
         for dirichlet_bc in self.bcs.dirichlet:
-
             if callable(dirichlet_bc):
                 try:
                     self._dirichlet_bc = dirichlet_bc(self.state_space)
                 except Exception as ex:
                     print(ex)
                     raise ex
             else:
-
                 raise NotImplementedError
 
     def solve(self):
         return self._solver.solve(self.state)
```

### Comparing `fenicsx-pulse-0.1.2/src/fenicsx_pulse.egg-info/PKG-INFO` & `fenicsx-pulse-0.1.3/src/fenicsx_pulse.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenicsx-pulse
-Version: 0.1.2
+Version: 0.1.3
 Summary: Next generation cardiac mechanics solver based on FEniCSx
 Author-email: Henrik Finsberg <henriknf@simula.no>
 License: Copyright 2022 Henrik Finsberg
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -22,15 +22,15 @@
 [![MIT](https://img.shields.io/github/license/finsberg/fenicsx-pulse)](https://github.com/finsberg/fenicsx-pulse/blob/main/LICENSE)
 [![PyPI version](https://badge.fury.io/py/fenicsx-pulse.svg)](https://pypi.org/project/fenicsx_pulse/)
 [![Test package](https://github.com/finsberg/fenicsx-pulse/actions/workflows/test_package_coverage.yml/badge.svg)](https://github.com/finsberg/fenicsx-pulse/actions/workflows/test_package_coverage.yml)
 [![Pre-commit](https://github.com/finsberg/fenicsx-pulse/actions/workflows/pre-commit.yml/badge.svg)](https://github.com/finsberg/fenicsx-pulse/actions/workflows/pre-commit.yml)
 [![Deploy static content to Pages](https://github.com/finsberg/fenicsx-pulse/actions/workflows/build_docs.yml/badge.svg)](https://github.com/finsberg/fenicsx-pulse/actions/workflows/build_docs.yml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Create and publish a Docker image](https://github.com/finsberg/fenicsx-pulse/actions/workflows/docker-image.yml/badge.svg)](https://github.com/finsberg/fenicsx-pulse/pkgs/container/fenicsx_pulse)
-
+[![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/finsberg/a7290de789564f03eb6b1ee122fce423/raw/fenicsx-pulse-coverage.json)](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/finsberg/a7290de789564f03eb6b1ee122fce423/raw/fenicsx-pulse-coverage.json)
 
 # fenicsx-pulse
 
 `fenicsx-pulse` is a cardiac mechanics solver based on FEniCSx. It is a successor of [`pulse`](https://github.com/finsberg/pulse) which is a cardiac mechanics solver based on FEniCS.
 
 ---
 
@@ -49,15 +49,15 @@
 
 To install `fenicsx_pulse` you need to first [install FEniCSx](https://github.com/FEniCS/dolfinx#installation). Next you can install `fenicsx_pulse` via pip
 ```
 python3 -m pip install fenicsx-pulse
 ```
 We also provide a pre-built docker image with FEniCSx and `fenicsx_pulse` installed. You pull this image using the command
 ```
-docker pull ghcr.io/finsberg/fenicsx-pulse:v0.1.2
+docker pull ghcr.io/finsberg/fenicsx-pulse:v0.1.3
 ```
 
 ## Simple Example
 
 ```python
 import dolfinx
 import numpy as np
@@ -135,9 +135,8 @@
 xdmf.write_mesh(mesh)
 xdmf.write_function(u, 0.0)
 xdmf.write_function(p, 0.0)
 ```
 
 
 ## Contributing
-
-TBW
+See https://finsberg.github.io/fenicsx-pulse/CONTRIBUTING.html
```

