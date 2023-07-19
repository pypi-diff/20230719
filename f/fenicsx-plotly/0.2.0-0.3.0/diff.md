# Comparing `tmp/fenicsx_plotly-0.2.0.tar.gz` & `tmp/fenicsx_plotly-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenicsx_plotly-0.2.0.tar", last modified: Thu Dec 29 17:10:43 2022, max compression
+gzip compressed data, was "fenicsx_plotly-0.3.0.tar", last modified: Wed Jul 19 06:54:15 2023, max compression
```

## Comparing `fenicsx_plotly-0.2.0.tar` & `fenicsx_plotly-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 17:10:43.705441 fenicsx_plotly-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2022-12-29 17:10:28.000000 fenicsx_plotly-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2022-12-29 17:10:43.705441 fenicsx_plotly-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2022-12-29 17:10:28.000000 fenicsx_plotly-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      961 2022-12-29 17:10:28.000000 fenicsx_plotly-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-29 17:10:43.705441 fenicsx_plotly-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 17:10:43.701441 fenicsx_plotly-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 17:10:43.705441 fenicsx_plotly-0.2.0/src/fenicsx_plotly/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2022-12-29 17:10:28.000000 fenicsx_plotly-0.2.0/src/fenicsx_plotly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16628 2022-12-29 17:10:28.000000 fenicsx_plotly-0.2.0/src/fenicsx_plotly/_fenicsx_plotly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 17:10:43.705441 fenicsx_plotly-0.2.0/src/fenicsx_plotly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2022-12-29 17:10:43.000000 fenicsx_plotly-0.2.0/src/fenicsx_plotly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      310 2022-12-29 17:10:43.000000 fenicsx_plotly-0.2.0/src/fenicsx_plotly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-29 17:10:43.000000 fenicsx_plotly-0.2.0/src/fenicsx_plotly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2022-12-29 17:10:43.000000 fenicsx_plotly-0.2.0/src/fenicsx_plotly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2022-12-29 17:10:43.000000 fenicsx_plotly-0.2.0/src/fenicsx_plotly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 06:54:15.090276 fenicsx_plotly-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-19 06:53:57.000000 fenicsx_plotly-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-07-19 06:54:15.090276 fenicsx_plotly-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-19 06:53:57.000000 fenicsx_plotly-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-19 06:53:57.000000 fenicsx_plotly-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 06:54:15.090276 fenicsx_plotly-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 06:54:15.086275 fenicsx_plotly-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 06:54:15.090276 fenicsx_plotly-0.3.0/src/fenicsx_plotly/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-19 06:53:57.000000 fenicsx_plotly-0.3.0/src/fenicsx_plotly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16091 2023-07-19 06:53:57.000000 fenicsx_plotly-0.3.0/src/fenicsx_plotly/_fenicsx_plotly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 06:54:15.090276 fenicsx_plotly-0.3.0/src/fenicsx_plotly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-07-19 06:54:15.000000 fenicsx_plotly-0.3.0/src/fenicsx_plotly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-19 06:54:15.000000 fenicsx_plotly-0.3.0/src/fenicsx_plotly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 06:54:15.000000 fenicsx_plotly-0.3.0/src/fenicsx_plotly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-19 06:54:15.000000 fenicsx_plotly-0.3.0/src/fenicsx_plotly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-19 06:54:15.000000 fenicsx_plotly-0.3.0/src/fenicsx_plotly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 06:54:15.090276 fenicsx_plotly-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-07-19 06:53:57.000000 fenicsx_plotly-0.3.0/tests/test_fenicsx_plotly.py
```

### Comparing `fenicsx_plotly-0.2.0/LICENSE` & `fenicsx_plotly-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fenicsx_plotly-0.2.0/PKG-INFO` & `fenicsx_plotly-0.3.0/src/fenicsx_plotly.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: fenicsx_plotly
-Version: 0.2.0
+Name: fenicsx-plotly
+Version: 0.3.0
 Summary: Lightweight library for plotting FEniCS x objects using plotly
 Author-email: Henrik Finsberg <henriknf@simula.no>
 License: Copyright 2022 Henrik Finsberg
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -21,14 +21,15 @@
 [![MIT](https://img.shields.io/github/license/finsberg/fenicsx-plotly)](https://github.com/finsberg/fenicsx-plotly/blob/main/LICENSE)
 [![PyPI version](https://badge.fury.io/py/fenicsx-plotly.svg)](https://pypi.org/project/fenicsx-plotly/)
 [![Test package](https://github.com/finsberg/fenicsx-plotly/actions/workflows/test_package_coverage.yml/badge.svg)](https://github.com/finsberg/fenicsx-plotly/actions/workflows/test_package_coverage.yml)
 [![Pre-commit](https://github.com/finsberg/fenicsx-plotly/actions/workflows/pre-commit.yml/badge.svg)](https://github.com/finsberg/fenicsx-plotly/actions/workflows/pre-commit.yml)
 [![Deploy static content to Pages](https://github.com/finsberg/fenicsx-plotly/actions/workflows/build_docs.yml/badge.svg)](https://github.com/finsberg/fenicsx-plotly/actions/workflows/build_docs.yml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Create and publish a Docker image](https://github.com/finsberg/fenicsx-plotly/actions/workflows/docker-image.yml/badge.svg)](https://github.com/finsberg/fenicsx-plotly/pkgs/container/fenicsx-plotly)
+[![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/finsberg/a7290de789564f03eb6b1ee122fce423/raw/fenicsx-plotly-coverage.json)](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/finsberg/a7290de789564f03eb6b1ee122fce423/raw/fenicsx-plotly-coverage.json)
 
 # fenicsx-plotly
 
 `fenicsx-plotly` is package for plotting FEniCSx objects using plotly. It is a successor of [`fenics-plotly`](https://github.com/finsberg/pulse).
 
 * Documentation: https://finsberg.github.io/fenicsx-plotly/
 * Source code: https://github.com/finsberg/fenicsx-plotly
@@ -37,15 +38,15 @@
 
 To install `fenicsx-plotly` you need to first [install FEniCSx](https://github.com/FEniCS/dolfinx#installation). Next you can install `fenicsx-plotly` via pip
 ```
 python3 -m pip install fenicsx-plotly
 ```
 We also provide a pre-built docker image with FEniCSx and `fenicsx-plotly` installed. You pull this image using the command
 ```
-docker pull ghcr.io/finsberg/fenicsx-plotly:v0.2.0
+docker pull ghcr.io/finsberg/fenicsx-plotly:v0.3.0
 ```
 
 ## Simple Example
 ```python
 import dolfinx
 from mpi4py import MPI
 from fenicsx_plotly import plot
```

### Comparing `fenicsx_plotly-0.2.0/README.md` & `fenicsx_plotly-0.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [![MIT](https://img.shields.io/github/license/finsberg/fenicsx-plotly)](https://github.com/finsberg/fenicsx-plotly/blob/main/LICENSE)
 [![PyPI version](https://badge.fury.io/py/fenicsx-plotly.svg)](https://pypi.org/project/fenicsx-plotly/)
 [![Test package](https://github.com/finsberg/fenicsx-plotly/actions/workflows/test_package_coverage.yml/badge.svg)](https://github.com/finsberg/fenicsx-plotly/actions/workflows/test_package_coverage.yml)
 [![Pre-commit](https://github.com/finsberg/fenicsx-plotly/actions/workflows/pre-commit.yml/badge.svg)](https://github.com/finsberg/fenicsx-plotly/actions/workflows/pre-commit.yml)
 [![Deploy static content to Pages](https://github.com/finsberg/fenicsx-plotly/actions/workflows/build_docs.yml/badge.svg)](https://github.com/finsberg/fenicsx-plotly/actions/workflows/build_docs.yml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Create and publish a Docker image](https://github.com/finsberg/fenicsx-plotly/actions/workflows/docker-image.yml/badge.svg)](https://github.com/finsberg/fenicsx-plotly/pkgs/container/fenicsx-plotly)
+[![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/finsberg/a7290de789564f03eb6b1ee122fce423/raw/fenicsx-plotly-coverage.json)](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/finsberg/a7290de789564f03eb6b1ee122fce423/raw/fenicsx-plotly-coverage.json)
 
 # fenicsx-plotly
 
 `fenicsx-plotly` is package for plotting FEniCSx objects using plotly. It is a successor of [`fenics-plotly`](https://github.com/finsberg/pulse).
 
 * Documentation: https://finsberg.github.io/fenicsx-plotly/
 * Source code: https://github.com/finsberg/fenicsx-plotly
@@ -17,15 +18,15 @@
 
 To install `fenicsx-plotly` you need to first [install FEniCSx](https://github.com/FEniCS/dolfinx#installation). Next you can install `fenicsx-plotly` via pip
 ```
 python3 -m pip install fenicsx-plotly
 ```
 We also provide a pre-built docker image with FEniCSx and `fenicsx-plotly` installed. You pull this image using the command
 ```
-docker pull ghcr.io/finsberg/fenicsx-plotly:v0.2.0
+docker pull ghcr.io/finsberg/fenicsx-plotly:v0.3.0
 ```
 
 ## Simple Example
 ```python
 import dolfinx
 from mpi4py import MPI
 from fenicsx_plotly import plot
```

### Comparing `fenicsx_plotly-0.2.0/src/fenicsx_plotly/_fenicsx_plotly.py` & `fenicsx_plotly-0.3.0/src/fenicsx_plotly/_fenicsx_plotly.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import typing
 from pathlib import Path
 
 import dolfinx
 import numpy as np
+import numpy.typing as npt
 import plotly
 import plotly.graph_objects as go
 import plotly.io as pio
 import ufl
 from plotly.basedatatypes import BaseTraceType as _BaseTraceType
 
 try:
@@ -60,15 +61,15 @@
     }
     if save_config is not None:
         config.update(save_config)
 
     plotly.offline.plot(fig, filename=fname.as_posix(), auto_open=False, config=config)
 
 
-def _get_triangles(mesh: dolfinx.mesh.Mesh) -> np.ndarray[int]:
+def _get_triangles(mesh: dolfinx.mesh.Mesh) -> npt.NDArray[np.int32]:
     faces = dolfinx.mesh.locate_entities(
         mesh,
         2,
         lambda x: np.full(x.shape[1], True, dtype=bool),
     )
 
     mesh.topology.create_connectivity(2, 0)
@@ -79,15 +80,18 @@
         # FIXME: Should be possible to do this vectorized!
         triangle[:, face] = conn.links(face)
 
     return triangle
 
 
 def _surface_plot_mesh(
-    mesh: dolfinx.mesh.Mesh, color: str = "gray", opacity: float = 1.0, **kwargs
+    mesh: dolfinx.mesh.Mesh,
+    color: str = "gray",
+    opacity: float = 1.0,
+    **kwargs,
 ):
     coord = mesh.geometry.x
     triangle = _get_triangles(mesh)
     if len(coord[0, :]) == 2:
         coord = np.c_[coord, np.zeros(len(coord[:, 0]))]
 
     surface = go.Mesh3d(
@@ -104,19 +108,15 @@
     )
 
     return surface
 
 
 def _get_cells(mesh: dolfinx.mesh.Mesh) -> np.ndarray:
     dm = mesh.geometry.dofmap
-    cells = np.zeros((dm.num_nodes, len(dm.links(0))), dtype=np.int32)
-    # FIXME: Should be possible to vectorize this
-    for node in range(dm.num_nodes):
-        cells[node, :] = dm.links(node)
-    return cells
+    return dm.T
 
 
 def _wireframe_plot_mesh(mesh: dolfinx.mesh.Mesh, **kwargs) -> go.Scatter3d:
     coord = mesh.geometry.x
 
     if len(coord[0, :]) == 2:
         coord = np.c_[coord, np.zeros(len(coord[:, 0]))]
@@ -142,15 +142,17 @@
         hoverinfo="none",
     )
 
     return lines
 
 
 def _plot_dofs(
-    functionspace: dolfinx.fem.FunctionSpace, size: int, **kwargs
+    functionspace: dolfinx.fem.FunctionSpace,
+    size: int,
+    **kwargs,
 ) -> go.Scatter3d:
     dofs_coord = functionspace.tabulate_dof_coordinates()
     if len(dofs_coord[0, :]) == 2:
         dofs_coord = np.c_[dofs_coord, np.zeros(len(dofs_coord[:, 0]))]
 
     points = go.Scatter3d(
         x=dofs_coord[:, 0],
@@ -161,15 +163,14 @@
         marker=dict(size=size),
     )
 
     return points
 
 
 def _get_vertex_values(function: dolfinx.fem.Function) -> np.ndarray:
-
     fs = function.function_space
     mesh = fs.mesh
     shape = function.ufl_shape
 
     if len(shape) == 0:  # FiniteElement
         el = fs.ufl_element()
         # TODO: Ask Jørgen if there is a better way
@@ -236,15 +237,19 @@
         showscale=showscale,
     )
 
     return surface
 
 
 def _scatter_plot_function(
-    function: dolfinx.fem.Function, colorscale, showscale=True, size=10, **kwargs
+    function: dolfinx.fem.Function,
+    colorscale,
+    showscale=True,
+    size=10,
+    **kwargs,
 ) -> go.Scatter3d:
     dofs_coord = function.function_space.tabulate_dof_coordinates()
     if len(dofs_coord[0, :]) == 2:
         dofs_coord = np.c_[dofs_coord, np.zeros(len(dofs_coord[:, 0]))]
 
     mesh = function.function_space.mesh
     val = function.x.array
@@ -270,15 +275,14 @@
 def _cone_plot(
     function: dolfinx.fem.Function,
     size: int = 10,
     showscale: bool = True,
     normalize: bool = False,
     **kwargs,
 ) -> go.Cone:
-
     mesh = function.function_space.mesh
     points = mesh.geometry.x
     vectors = _get_vertex_values(function)
 
     if len(points[0, :]) == 2:
         points = np.c_[points, np.zeros(len(points[:, 0]))]
 
@@ -312,42 +316,44 @@
 
     data.append(_wireframe_plot_mesh(obj))
 
     return data
 
 
 def _handle_function_space(
-    obj: dolfinx.fem.FunctionSpace, **kwargs
+    obj: dolfinx.fem.FunctionSpace,
+    **kwargs,
 ) -> list[_BaseTraceType]:
     data = []
     points = _plot_dofs(obj, **kwargs)
     data.append(points)
 
     if kwargs.get("wireframe", True):
         lines = _wireframe_plot_mesh(obj.mesh, **kwargs)
         data.append(lines)
     return data
 
 
 def _handle_scalar_function(
-    obj: dolfinx.fem.Function, scatter: bool = False, **kwargs
+    obj: dolfinx.fem.Function,
+    scatter: bool = False,
+    **kwargs,
 ) -> _BaseTraceType:
     if scatter:
         surface = _scatter_plot_function(obj, **kwargs)
     else:
         surface = _surface_plot_function(obj, **kwargs)
     return surface
 
 
 def _handle_vector_function(
     obj: dolfinx.fem.Function,
     component: typing.Optional[str] = None,
     **kwargs,
 ) -> _BaseTraceType:
-
     fs = obj.function_space
 
     if component is None:
         return _cone_plot(obj, **kwargs)
 
     elif component == "magnitude":
         V, _ = obj.function_space.sub(0).collapse()
@@ -388,21 +394,27 @@
         lines = _wireframe_plot_mesh(obj.function_space.mesh)
         data.append(lines)
 
     return data
 
 
 def _handle_meshtags(
-    obj: dolfinx.mesh.MeshTagsMetaClass, colorscale: str = "inferno", **kwargs
+    obj: dolfinx.mesh.MeshTags,
+    colorscale: str = "inferno",
+    **kwargs,
 ) -> list[_BaseTraceType]:
-
     data = []
     if obj.dim != 2:
         raise NotImplementedError("Plotting of MeshTags is only supported for facets")
-    mesh = obj.mesh
+    mesh = kwargs.get("mesh")
+    if mesh is None:
+        raise RuntimeError(
+            "Please provide mesh as a keyword argument when plotting MeshTags",
+        )
+
     # array = meshfunc.array()
     coord = mesh.geometry.x
     if len(coord[0, :]) == 2:
         coord = np.c_[coord, np.zeros(len(coord[:, 0]))]
 
     triangle = _get_triangles(mesh)
     array = np.zeros(triangle.shape[1])
@@ -433,47 +445,30 @@
         lines = _wireframe_plot_mesh(mesh)
         data.append(lines)
 
     return data
 
 
 def _plot_dirichlet_bc(
-    obj: dolfinx.fem.bcs.DirichletBCMetaClass,
+    obj: dolfinx.fem.bcs.DirichletBC,
     size: int = 10,
     colorscale: str = "inferno",
     **kwargs,
 ) -> list[_BaseTraceType]:
-    if obj.function_space.element.num_sub_elements > 0:
-        raise NotImplementedError(
-            "Can plot dirichlet BC for finite elements (not vector elements)",
-        )
-    dofs = obj.function_space.tabulate_dof_coordinates()
-    if len(dofs[0, :]) == 2:
-        dofs = np.c_[dofs, np.zeros(len(dofs[:, 0]))]
-    indices, _ = obj.dof_indices()
-
-    coords = dofs[indices]
-    vals = obj.value.x.array[indices]
-
-    return go.Scatter3d(
-        x=coords[:, 0],
-        y=coords[:, 1],
-        z=coords[:, 2],
-        mode="markers",
-        marker=dict(
-            size=size,
-            color=vals,
-            colorscale=colorscale,
-            colorbar=dict(thickness=20),
-        ),
+    return _scatter_plot_function(
+        function=obj.g,
+        size=size,
+        colorscale=colorscale,
+        **kwargs,
     )
 
 
 def _handle_dirichlet_bc(
-    obj: dolfinx.fem.bcs.DirichletBCMetaClass, **kwargs
+    obj: dolfinx.fem.bcs.DirichletBC,
+    **kwargs,
 ) -> list[_BaseTraceType]:
     data = []
     points = _plot_dirichlet_bc(obj, **kwargs)
     data.append(points)
 
     lines = _wireframe_plot_mesh(obj.function_space.mesh, **kwargs)
     data.append(lines)
@@ -509,14 +504,15 @@
     size_frame: typing.Optional[typing.Tuple[int, int]] = None,
     background: typing.Tuple[int, int, int] = (242, 242, 242),
     normalize: bool = False,
     component: typing.Optional[str] = None,
     showscale: bool = True,
     show: bool = True,
     filename: typing.Optional[str] = None,
+    **kwargs,
 ) -> FEniCSPlotFig:
     """Plot FEniCSx object
 
     Parameters
     ----------
     obj : Mesh, Function. FunctionSpace, MeshFunction, DirichletBC
         FEniCSx object to be plotted
@@ -559,21 +555,21 @@
 
     if isinstance(obj, dolfinx.mesh.Mesh):
         handle = _handle_mesh
 
     elif isinstance(obj, dolfinx.fem.Function):
         handle = _handle_function
 
-    elif isinstance(obj, dolfinx.mesh.MeshTagsMetaClass):
+    elif isinstance(obj, dolfinx.mesh.MeshTags):
         handle = _handle_meshtags
 
     elif isinstance(obj, dolfinx.fem.FunctionSpace):
         handle = _handle_function_space
 
-    elif isinstance(obj, dolfinx.fem.bcs.DirichletBCMetaClass):
+    elif isinstance(obj, dolfinx.fem.bcs.DirichletBC):
         handle = _handle_dirichlet_bc
 
     else:
         raise TypeError(f"Cannot plot object of type {type(obj)}")
 
     data = handle(
         obj,
@@ -585,14 +581,15 @@
         component=component,
         opacity=opacity,
         show_grid=show_grid,
         color=color,
         wireframe=wireframe,
         showscale=showscale,
         name=name,
+        **kwargs,
     )
 
     layout = go.Layout(
         scene_xaxis_visible=show_grid,
         scene_yaxis_visible=show_grid,
         scene_zaxis_visible=show_grid,
         paper_bgcolor="rgb" + str(background),
```

### Comparing `fenicsx_plotly-0.2.0/src/fenicsx_plotly.egg-info/PKG-INFO` & `fenicsx_plotly-0.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: fenicsx-plotly
-Version: 0.2.0
+Name: fenicsx_plotly
+Version: 0.3.0
 Summary: Lightweight library for plotting FEniCS x objects using plotly
 Author-email: Henrik Finsberg <henriknf@simula.no>
 License: Copyright 2022 Henrik Finsberg
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -21,14 +21,15 @@
 [![MIT](https://img.shields.io/github/license/finsberg/fenicsx-plotly)](https://github.com/finsberg/fenicsx-plotly/blob/main/LICENSE)
 [![PyPI version](https://badge.fury.io/py/fenicsx-plotly.svg)](https://pypi.org/project/fenicsx-plotly/)
 [![Test package](https://github.com/finsberg/fenicsx-plotly/actions/workflows/test_package_coverage.yml/badge.svg)](https://github.com/finsberg/fenicsx-plotly/actions/workflows/test_package_coverage.yml)
 [![Pre-commit](https://github.com/finsberg/fenicsx-plotly/actions/workflows/pre-commit.yml/badge.svg)](https://github.com/finsberg/fenicsx-plotly/actions/workflows/pre-commit.yml)
 [![Deploy static content to Pages](https://github.com/finsberg/fenicsx-plotly/actions/workflows/build_docs.yml/badge.svg)](https://github.com/finsberg/fenicsx-plotly/actions/workflows/build_docs.yml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Create and publish a Docker image](https://github.com/finsberg/fenicsx-plotly/actions/workflows/docker-image.yml/badge.svg)](https://github.com/finsberg/fenicsx-plotly/pkgs/container/fenicsx-plotly)
+[![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/finsberg/a7290de789564f03eb6b1ee122fce423/raw/fenicsx-plotly-coverage.json)](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/finsberg/a7290de789564f03eb6b1ee122fce423/raw/fenicsx-plotly-coverage.json)
 
 # fenicsx-plotly
 
 `fenicsx-plotly` is package for plotting FEniCSx objects using plotly. It is a successor of [`fenics-plotly`](https://github.com/finsberg/pulse).
 
 * Documentation: https://finsberg.github.io/fenicsx-plotly/
 * Source code: https://github.com/finsberg/fenicsx-plotly
@@ -37,15 +38,15 @@
 
 To install `fenicsx-plotly` you need to first [install FEniCSx](https://github.com/FEniCS/dolfinx#installation). Next you can install `fenicsx-plotly` via pip
 ```
 python3 -m pip install fenicsx-plotly
 ```
 We also provide a pre-built docker image with FEniCSx and `fenicsx-plotly` installed. You pull this image using the command
 ```
-docker pull ghcr.io/finsberg/fenicsx-plotly:v0.2.0
+docker pull ghcr.io/finsberg/fenicsx-plotly:v0.3.0
 ```
 
 ## Simple Example
 ```python
 import dolfinx
 from mpi4py import MPI
 from fenicsx_plotly import plot
```

