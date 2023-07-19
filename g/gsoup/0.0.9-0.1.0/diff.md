# Comparing `tmp/gsoup-0.0.9.tar.gz` & `tmp/gsoup-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gsoup-0.0.9.tar", last modified: Mon Jun 26 08:01:06 2023, max compression
+gzip compressed data, was "gsoup-0.1.0.tar", last modified: Wed Jul 19 01:46:21 2023, max compression
```

## Comparing `gsoup-0.0.9.tar` & `gsoup-0.1.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 08:01:06.734643 gsoup-0.0.9/
--rw-rw-rw-   0        0        0     1088 2022-12-12 04:07:15.000000 gsoup-0.0.9/LICENSE
--rw-rw-rw-   0        0        0       47 2022-12-12 04:07:15.000000 gsoup-0.0.9/MANIFEST.in
--rw-rw-rw-   0        0        0     3037 2023-06-26 08:01:06.734643 gsoup-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     1202 2023-06-25 06:21:55.000000 gsoup-0.0.9/README.md
--rw-rw-rw-   0        0        0     1252 2023-06-26 07:58:21.000000 gsoup-0.0.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-26 08:01:06.734643 gsoup-0.0.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-26 08:01:06.680651 gsoup-0.0.9/src/
-drwxrwxrwx   0        0        0        0 2023-06-26 08:01:06.713699 gsoup-0.0.9/src/gsoup/
--rw-rw-rw-   0        0        0   343980 2022-12-12 04:07:15.000000 gsoup-0.0.9/src/gsoup/FreeMono.ttf
--rw-rw-rw-   0        0        0     2734 2023-06-26 07:58:21.000000 gsoup-0.0.9/src/gsoup/__init__.py
--rw-rw-rw-   0        0        0    25250 2023-06-26 07:42:32.000000 gsoup-0.0.9/src/gsoup/core.py
--rw-rw-rw-   0        0        0     7363 2023-06-26 07:38:01.000000 gsoup-0.0.9/src/gsoup/geometry_advanced.py
--rw-rw-rw-   0        0        0    14707 2023-06-25 06:21:55.000000 gsoup-0.0.9/src/gsoup/geometry_basic.py
--rw-rw-rw-   0        0        0    20248 2023-06-26 07:55:45.000000 gsoup-0.0.9/src/gsoup/gsoup_io.py
--rw-rw-rw-   0        0        0    24244 2023-06-25 06:21:55.000000 gsoup-0.0.9/src/gsoup/image.py
--rw-rw-rw-   0        0        0    19684 2023-06-25 06:21:55.000000 gsoup-0.0.9/src/gsoup/procam.py
--rw-rw-rw-   0        0        0     8189 2023-02-28 11:28:59.000000 gsoup-0.0.9/src/gsoup/sphere_trace.py
--rw-rw-rw-   0        0        0     9104 2023-02-16 04:29:03.000000 gsoup-0.0.9/src/gsoup/structures.py
--rw-rw-rw-   0        0        0     5691 2023-06-26 07:44:21.000000 gsoup-0.0.9/src/gsoup/transforms.py
--rw-rw-rw-   0        0        0    11926 2023-06-25 06:21:55.000000 gsoup-0.0.9/src/gsoup/video.py
--rw-rw-rw-   0        0        0     7409 2023-02-26 12:22:36.000000 gsoup-0.0.9/src/gsoup/viewer.py
--rw-rw-rw-   0        0        0     6542 2023-02-28 11:44:06.000000 gsoup-0.0.9/src/gsoup/viewer_drivers.py
-drwxrwxrwx   0        0        0        0 2023-06-26 08:01:06.732648 gsoup-0.0.9/src/gsoup.egg-info/
--rw-rw-rw-   0        0        0     3037 2023-06-26 08:01:06.000000 gsoup-0.0.9/src/gsoup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      552 2023-06-26 08:01:06.000000 gsoup-0.0.9/src/gsoup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 08:01:06.000000 gsoup-0.0.9/src/gsoup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2023-06-26 08:01:06.000000 gsoup-0.0.9/src/gsoup.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-26 08:01:06.000000 gsoup-0.0.9/src/gsoup.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-26 08:01:06.733675 gsoup-0.0.9/tests/
--rw-rw-rw-   0        0        0    16532 2023-06-26 07:54:08.000000 gsoup-0.0.9/tests/test_basic.py
+drwxrwxrwx   0        0        0        0 2023-07-19 01:46:21.664711 gsoup-0.1.0/
+-rw-rw-rw-   0        0        0     1088 2022-12-12 04:07:15.000000 gsoup-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0       47 2022-12-12 04:07:15.000000 gsoup-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3058 2023-07-19 01:46:21.664711 gsoup-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1202 2023-07-03 04:59:26.000000 gsoup-0.1.0/README.md
+-rw-rw-rw-   0        0        0     1273 2023-07-19 01:45:47.000000 gsoup-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-19 01:46:21.664711 gsoup-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-19 01:46:21.609951 gsoup-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-19 01:46:21.645760 gsoup-0.1.0/src/gsoup/
+-rw-rw-rw-   0        0        0   343980 2022-12-12 04:07:15.000000 gsoup-0.1.0/src/gsoup/FreeMono.ttf
+-rw-rw-rw-   0        0        0     2810 2023-07-19 01:45:47.000000 gsoup-0.1.0/src/gsoup/__init__.py
+-rw-rw-rw-   0        0        0     8544 2023-07-12 07:34:20.000000 gsoup-0.1.0/src/gsoup/core.py
+-rw-rw-rw-   0        0        0     7363 2023-06-26 07:38:01.000000 gsoup-0.1.0/src/gsoup/geometry_advanced.py
+-rw-rw-rw-   0        0        0    16437 2023-07-12 07:11:14.000000 gsoup-0.1.0/src/gsoup/geometry_basic.py
+-rw-rw-rw-   0        0        0    27225 2023-07-19 01:45:12.000000 gsoup-0.1.0/src/gsoup/gsoup_io.py
+-rw-rw-rw-   0        0        0    22495 2023-07-18 09:05:07.000000 gsoup-0.1.0/src/gsoup/image.py
+-rw-rw-rw-   0        0        0    29667 2023-07-18 09:31:33.000000 gsoup-0.1.0/src/gsoup/procam.py
+-rw-rw-rw-   0        0        0     8189 2023-02-28 11:28:59.000000 gsoup-0.1.0/src/gsoup/sphere_trace.py
+-rw-rw-rw-   0        0        0     9104 2023-02-16 04:29:03.000000 gsoup-0.1.0/src/gsoup/structures.py
+-rw-rw-rw-   0        0        0    24669 2023-07-12 09:34:46.000000 gsoup-0.1.0/src/gsoup/transforms.py
+-rw-rw-rw-   0        0        0    12467 2023-07-19 01:33:52.000000 gsoup-0.1.0/src/gsoup/video.py
+-rw-rw-rw-   0        0        0     7409 2023-02-26 12:22:36.000000 gsoup-0.1.0/src/gsoup/viewer.py
+-rw-rw-rw-   0        0        0    10213 2023-07-12 08:57:12.000000 gsoup-0.1.0/src/gsoup/viewer_drivers.py
+drwxrwxrwx   0        0        0        0 2023-07-19 01:46:21.662714 gsoup-0.1.0/src/gsoup.egg-info/
+-rw-rw-rw-   0        0        0     3058 2023-07-19 01:46:21.000000 gsoup-0.1.0/src/gsoup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      552 2023-07-19 01:46:21.000000 gsoup-0.1.0/src/gsoup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 01:46:21.000000 gsoup-0.1.0/src/gsoup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      119 2023-07-19 01:46:21.000000 gsoup-0.1.0/src/gsoup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-19 01:46:21.000000 gsoup-0.1.0/src/gsoup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-19 01:46:21.662714 gsoup-0.1.0/tests/
+-rw-rw-rw-   0        0        0    19942 2023-07-19 01:39:10.000000 gsoup-0.1.0/tests/test_basic.py
```

### Comparing `gsoup-0.0.9/LICENSE` & `gsoup-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gsoup-0.0.9/PKG-INFO` & `gsoup-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gsoup
-Version: 0.0.9
+Version: 0.1.0
 Summary: A geoemtry & graphics library with focus on clarity rather than performance.
 Author-email: Yotam Erel <erelyotam@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Yotam Erel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,14 +30,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: build
 Provides-Extra: dev
+Provides-Extra: vis
 License-File: LICENSE
 
 # gsoup
 
 ## In a nutshell
 A python library implementing various geometry / graphics algorithms, with focus on clarity rather than performance.
```

### Comparing `gsoup-0.0.9/README.md` & `gsoup-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `gsoup-0.0.9/pyproject.toml` & `gsoup-0.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gsoup"
-version = "0.0.9"
+version = "0.1.0"
 description = "A geoemtry & graphics library with focus on clarity rather than performance."
 readme = "README.md"
 authors = [{ name = "Yotam Erel", email = "erelyotam@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -24,20 +24,21 @@
     "opencv-python",
 ]
 requires-python = ">=3.7"
 
 [project.optional-dependencies]
 build = ["build", "twine"]
 dev = ["bumpver", "pytest"]
+vis = ["polyscope"]
 
 [project.urls]
 Homepage = "https://github.com/yoterel/gsoup"
 
 [tool.bumpver]
-current_version = "0.0.9"
+current_version = "0.1.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `gsoup-0.0.9/src/gsoup/FreeMono.ttf` & `gsoup-0.1.0/src/gsoup/FreeMono.ttf`

 * *Files identical despite different names*

### Comparing `gsoup-0.0.9/src/gsoup/__init__.py` & `gsoup-0.1.0/src/gsoup/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,58 +1,62 @@
-__version__ = "0.0.9"
+__version__ = "0.1.0"
 
 from .core import (
     is_np,
-    broadcast_batch,
     to_hom,
     homogenize,
-    look_at_torch,
-    look_at_np,
     compose_rt,
     to_44,
     to_34,
     to_np,
     to_numpy,
     to_torch,
     to_8b,
     to_float,
+    broadcast_batch,
     map_range,
     map_to_01,
+    swap_columns
+)
+
+from .transforms import (
+    rotx,
+    roty,
+    rotz,
+    translate,
+    scale,
+    rotate,
+    look_at_torch,
+    look_at_np,
     create_random_cameras_on_unit_sphere,
-    random_vectors_on_sphere,
-    random_affine,
-    random_perspective,
     opengl_c2w_to_opencv_c2w,
     opencv_c2w_to_opengl_c2w,
     opencv_intrinsics_from_opengl_project,
     opengl_project_from_opencv_intrinsics,
     perspective_projection,
+    pixels_in_world_space,
+    find_rigid_transform,
+    find_affine_transformation,
+    decompose_affine,
+    random_vectors_on_sphere,
+    random_affine,
+    random_perspective,
+    random_qvec,
     vec2skew,
     batch_vec2skew,
     rotvec2mat,
     batch_rotvec2mat,
-    random_qvec,
     qvec2mat,
     batch_qvec2mat,
     mat2qvec,
     batch_mat2qvec,
 )
-
-from .transforms import (
-    rotx,
-    roty,
-    rotz,
-    translate,
-    scale,
-    rotate,
-    find_rigid_transform,
-    find_affine_transformation,
-    decompose_affine,
-)
 from .geometry_basic import (
+    is_inside_triangle,
+    ray_ray_intersection,
     duplicate_faces,
     remove_duplicate_faces,
     get_aspect_ratio,
     normalize_vertices,
     clean_infinite_vertices,
     calc_edges,
     calc_face_normals,
@@ -74,35 +78,33 @@
 from .gsoup_io import (
     write_to_json,
     save_image,
     save_images,
     save_animation,
     save_mesh,
     save_meshes,
-    save_obj,
     load_image,
     load_images,
-    load_obj,
     load_mesh,
+    save_pointcloud,
+    save_pointclouds
 )
 
 from .image import (
     alpha_compose,
     draw_text_on_image,
     draw_gizmo_on_image,
     merge_figures_with_line,
     generate_checkerboard,
     generate_voronoi_diagram,
     generate_gray_gradient,
     generate_dot_pattern,
     generate_stripe_pattern,
     generate_concentric_circles,
     generate_lollipop_pattern,
-    interpolate_single_channel,
-    interpolate_multi_channel,
     image_grid,
     resize_images_naive,
     adjust_contrast_brightness,
     change_brightness,
     linear_to_srgb,
     srgb_to_linear,
     pad_to_res,
@@ -126,14 +128,15 @@
 )
 
 from .procam import (
     warp_image,
     calibrate_procam,
     compute_backward_map,
     naive_color_compensate,
+    reconstruct_pointcloud,
     GrayCode
 )
 
 from .sphere_trace import (
     generate_rays,
     render
 )
```

### Comparing `gsoup-0.0.9/src/gsoup/core.py` & `gsoup-0.1.0/src/gsoup/transforms.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,133 +1,191 @@
-import torch
 import numpy as np
-from PIL import Image
-
-def is_np(x):
-    """
-    checks if x is a numpy array or torch tensor (will raise an error if x is neither)
-    :param x: object to check
-    :return: True if x is a numpy array, False if x is a torch tensor
-    """
-    if type(x) == np.ndarray:
-        return True
-    elif type(x) == torch.Tensor:
-        return False
-    else:
-        raise ValueError("input must be torch.Tensor or np.ndarray")
+from .core import to_44, compose_rt, normalize, broadcast_batch, is_np
+import torch
 
-def to_hom(x):
+def sincos(a, degrees=True):
     """
-    converts a vector to homogeneous coordinates
-    :param x: nxc numpy array
-    :return: nxc+1 numpy array
-    """
-    if is_np(x):
-        if x.ndim == 1:
-            return np.concatenate((x, np.array([1], dtype=x.dtype)))
-        else:
-            return np.concatenate((x, np.ones((x.shape[0], 1), dtype=x.dtype)), axis=-1)
-    else:
-        if x.ndim == 1:
-            return torch.cat((x, torch.ones(1, device=x.device)))
-        else:
-            return torch.cat((x, torch.ones(x.shape[0], 1, device=x.device)), dim=-1)
+    sin and cos of an angle
+    :param a: angle
+    :param degrees: if True, a is in degrees
+    """
+    if degrees:
+        a = np.deg2rad(a)
+    return np.sin(a), np.cos(a)
+
+def translate(t):
+    """
+    creates a translation matrix from a translation vector
+    :param t: translation vector or batch of translation vectors
+    :return: 4x4 translation matrix
+    """
+    if t.shape[-1] != 3:
+        raise ValueError("translation vector must be 3d")
+    if t.ndim == 1:
+        t = t[None, :]
+    mat = np.concatenate((np.eye(3)[None, :, :], t[:, :, None]), axis=-1)
+    return to_44(mat)
+
+def scale(s):
+    """
+    creates a scaling matrix from a scaling vector
+    :param s: scaling vector or batch of scaling vectors
+    :return: nx4x4 scaling matrix
+    """
+    if s.shape[-1] != 3:
+        raise ValueError("translation vector must be 3d")
+    if s.ndim == 1:
+        s = s[None, :]
+    mat = np.diag(s)
+    return to_44(mat)
+
+def rotate(a, r):
+    """
+    creates a rotation matrix from an angle a and an axis of rotation r
+    """
+    s, c = sincos(a)
+    r = normalize(r)
+    nc = 1 - c
+    x, y, z = r
+    return np.array([[x*x*nc +   c, x*y*nc - z*s, x*z*nc + y*s, 0],
+                      [y*x*nc + z*s, y*y*nc +   c, y*z*nc - x*s, 0],
+                      [x*z*nc - y*s, y*z*nc + x*s, z*z*nc +   c, 0],
+                      [           0,            0,            0, 1]])
+def rotx(a, degrees=True):
+    """
+    creates a homogeneous 3D rotation matrix around the x axis
+    a: angle
+    degrees: if True, a is in degrees, else radians
+    """
+    s, c = sincos(a, degrees)
+    return np.array([[1,0,0,0],
+                      [0,c,-s,0],
+                      [0,s,c,0],
+                      [0,0,0,1]])
 
-def homogenize(x, keepdim=False):
+def roty(a, degrees=True):
     """
-    normalizes a homogeneous vector by dividing by the last coordinate
-    :param x: nx3 numpy array
-    :return: nx4 numpy array
-    """
-    x = (x / x[..., -1:])
-    if not keepdim:
-        x = x[..., :-1]
-    return x
-
-def normalize(x, eps=1e-7):
-
-    if is_np(x):
-        return x / (np.linalg.norm(x, axis=-1, keepdims=True) + eps)
-    else:
-        return x / (torch.norm(x, dim=-1, keepdim=True) + eps)
-
+    creates a homogeneous 3D rotation matrix around the y axis
+    a: angle
+    degrees: if True, a is in degrees, else radians
+    """
+    s, c = sincos(a, degrees)
+    return np.array([[c,0,s,0],
+                      [0,1,0,0],
+                      [-s,0,c,0],
+                      [0,0,0,1]])
 
-def broadcast_batch(*args):
+def rotz(a, degrees=True):
     """
-    broadcast a list of arrays to the same shape on the batch dimension
-    assumes first dimension is batch unless ndim = 1 for all inputs (but then does not broadcast)
-    :param args: list of arrays
-    :return: list of arrays with the same shape
-    """
-    shapes = [a.shape for a in args]
-    ndims = np.array([a.ndim for a in args])
-    new_args = []
-    if (ndims <= 1).all():
-        for a in args:
-            new_args.append(a[None, :])
-        return new_args
-    elif ndims.min() == 1:
-        raise ValueError("cannot broadcast 1d and nd arrays")
-    else:
-        batch_dim = np.array([s[0] for s in shapes]).max()
-        for i, a in enumerate(args):
-            if a.shape[0] == batch_dim:
-                new_args.append(a)
-            else:
-                new_args.append(np.broadcast_to(a, (batch_dim, *a.shape[1:])))
-    return new_args
+    creates a homogeneous 3D rotation matrix around the z axis
+    a: angle
+    degrees: if True, a is in degrees, else radians
+    """
+    s, c = sincos(a, degrees)
+    return np.array([[c,-s,0,0],
+                      [s,c,0,0],
+                      [0,0,1,0],
+                      [0,0,0,1]])
 
-def compose_rt(R: np.array, t: np.array, square=False):
+def find_rigid_transform(A, B):
     """
-    composes a n x 3 x 4 numpy array from rotation and translation.
-    will broadcast upon batch dimension if necessary.
-    :param R: nx3x3 numpy array
-    :param t: nx3 numpy array
-    :param square: if True, output will be 4x4, otherwise 3x4
-    :return: n x 3 x 4 composition of the rotation and translation
-    """
-    RR, tt = broadcast_batch(R, t)
-    Rt = np.concatenate((RR, tt[:, :, None]), axis=-1)
-    if square:
-        Rt = to_44(Rt)
-    return Rt
-
-def to_44(mat):
-    """
-    converts a 3x4 to a 4x4 matrix by concatenating 0 0 0 1
-    :param mat: dimsx3x4 numpy array (dims can be any number of dims including 0)
-    :return: dimsx4x4 numpy array
-    """
-    if mat.shape[-2:] == (4, 4):
-        return mat
-    if mat.shape[-2:] != (3, 4):
-        raise ValueError("mat must be 3x4")
-    if is_np(mat):
-        to_cat = np.broadcast_to(np.array([0, 0, 0, 1]), (*mat.shape[:-2], 1, 4))
-        new_mat = np.concatenate((mat, to_cat), axis=-2)
-    else:
-        to_cat = torch.zeros((*mat.shape[:-2], 1, 4), dtype=mat.dtype, device=mat.device)
-        to_cat[..., -1] = 1
-        new_mat = torch.cat((mat, to_cat), dim=-2)
-    return new_mat
-
-def to_34(mat: np.array):
-    """
-    converts a 4x4 to a 3x4 matrix by removeing the last row
-    :param mat: 4x4 numpy array
-    :return: 3x4 numpy array
-    """
-    if mat.ndim == 3:
-        if mat.shape[1:] != (4, 4):
-            raise ValueError("mat must be 4x4")
-        return mat[:, :-1, :]
-    else:
-        if mat.shape != (4, 4):
-            raise ValueError("mat must be 4x4")
-        return mat[:-1, :]
+    finds best 3d rigid transformation between pc a and pc b (in the least squares sense) based on "Least-Squares Rigid Motion Using SVD"
+    :param A: point cloud a
+    :param B: point cloud b
+    :return: W such that W@A = B
+    """
+    centroid_A = np.mean(A, axis=0)
+    centroid_B = np.mean(B, axis=0)
+
+    A_mean = A - centroid_A
+    B_mean = B - centroid_B
+
+    H = A_mean.T @ B_mean
+    U, S, Vt = np.linalg.svd(H)
+
+    flip = np.linalg.det(Vt.T @ U.T)
+    ones = np.identity(len(Vt))
+    ones[-1, -1] = flip
+    R = Vt.T @ ones @ U.T
+    t = centroid_B - R @ centroid_A
+    return compose_rt(R[None, :], t[None, :], square=True)
+
+def find_affine_transformation(A, B):
+    """
+    finds best 3d affine transformation between pc a and pc b (in the least squares sense)
+    :param A: point cloud a
+    :param B: point cloud b
+    :return: W such that W@A = B
+    """
+    # assemble A matrix for least squares
+    assert len(A) >= 4
+    new_A = np.c_[A, np.ones(len(A))]
+    new_A = np.repeat(np.tile(new_A, (1, 3)), 3, axis=0)
+    # now A is 3nx12
+    # zero columns depending on index of point
+    new_A[::3, 4:] = 0
+    new_A[1::3, :4] = 0
+    new_A[1::3, 8:] = 0
+    new_A[2::3, :8] = 0
+    new_B = B.flatten()
+    if len(A) == 4:
+        #solve linear system
+        W = np.linalg.inv(new_A) @ new_B
+    else:
+        W = np.linalg.lstsq(new_A, new_B, rcond=None)[0]
+    return to_44(W.reshape(3, 4))
+
+def decompose_affine(A44):
+    """
+    Decompose 4x4 homogenous affine matrix into parts.
+    The parts are translations, rotations, zooms, shears.
+    Returns
+    -------
+    T : array, shape (3,)
+       Translation vector
+    R : array shape (3,3)
+        rotation matrix
+    Z : array, shape (3,)
+       scale vector.  May have one negative zoom to prevent need for negative
+       determinant R matrix above
+    S : array, shape (3,)
+       Shear vector, such that shears fill upper triangle above
+       diagonal to form shear matrix (type ``striu``).
+    Implementation of "Decomposing a matrix into simple transformations".
+    """
+    A44 = np.asarray(A44)
+    T = A44[:-1,-1]
+    RZS = A44[:-1,:-1]
+    # compute scales and shears
+    M0, M1, M2 = np.array(RZS).T
+    # extract x scale and normalize
+    sx = np.sqrt(np.sum(M0**2))
+    M0 /= sx
+    # orthogonalize M1 with respect to M0
+    sx_sxy = np.dot(M0, M1)
+    M1 -= sx_sxy * M0
+    # extract y scale and normalize
+    sy = np.sqrt(np.sum(M1**2))
+    M1 /= sy
+    sxy = sx_sxy / sx
+    # orthogonalize M2 with respect to M0 and M1
+    sx_sxz = np.dot(M0, M2)
+    sy_syz = np.dot(M1, M2)
+    M2 -= (sx_sxz * M0 + sy_syz * M1)
+    # extract z scale and normalize
+    sz = np.sqrt(np.sum(M2**2))
+    M2 /= sz
+    sxz = sx_sxz / sx
+    syz = sy_syz / sy
+    # Reconstruct rotation matrix, ensure positive determinant
+    Rmat = np.array([M0, M1, M2]).T
+    if np.linalg.det(Rmat) < 0:
+        sx *= -1
+        Rmat[:,0] *= -1
+    return T, Rmat, np.array([sx, sy, sz]), np.array([sxy, sxz, syz])
 
 def look_at_np(eye, at, up, opengl=False):
     """
     returns a batch of look_at transforms 4x4 (camera->world, the inverse of a ModelView matrix)
     will broadcast upon batch dimension if necessary.
     :param eye: n x 3 from vectors in world space
     :param at: n x 3 at vector in world space
@@ -272,36 +330,45 @@
     cx = width / 2
     cy = height / 2
     opencv_mtx = np.array([[fx, 0.0, cx],
                            [0.0, fy, cy],
                            [0.0, 0.0, 1]])
     return opencv_mtx
 
-def opengl_c2w_to_opencv_c2w(opengl_transforms):
+def opengl_c2w_to_opencv_c2w(opengl_transforms, is_column_major=False):
     """
     given a modelview matrix (World space->Eye/Camera/View space) where z is backward and y is up,
     converts its coordinate system to opencv convention (z forward, y down)
     :param opengl_transforms: 4x4 modelview matrix or batch of 4x4 modelview matrices
+    :param is_column_major: whether the input matrix is column major or row major
     :return: 4x4 modelview matrix in opencv convention
     """
     if opengl_transforms.ndim == 2:
         my_transforms = opengl_transforms[None, ...]
     else:
         my_transforms = opengl_transforms
     if my_transforms.shape[1:] != (4, 4):
         raise ValueError("transform must be 4x4 or batch of 4x4")
-    my_transforms[:, :, 1] *= -1
-    my_transforms[:, :, 2] *= -1
+    if is_column_major:
+        if is_np(my_transforms):
+            my_transforms = my_transforms.transpose(0, 2, 1)
+        else:
+            my_transforms = my_transforms.permute(0, 2, 1)
+        my_transforms[:, 1, :] *= -1
+        my_transforms[:, 2, :] *= -1
+    else:
+        my_transforms[:, :, 1] *= -1
+        my_transforms[:, :, 2] *= -1
     return my_transforms.reshape(opengl_transforms.shape)
 
-def opencv_c2w_to_opengl_c2w(opencv_transform):
+def opencv_c2w_to_opengl_c2w(opencv_transform, to_column_major=False):
     """
     converts coordinates of "vision" (opencv) to OpenGL coordinates by flipping y and z axes
     """
-    return opengl_c2w_to_opencv_c2w(opencv_transform)
+    return opengl_c2w_to_opencv_c2w(opencv_transform, to_column_major)
 
 def create_random_cameras_on_unit_sphere(n_cams, radius, normal=None, opengl=False, device="cpu"):
     """
     creates a batch of world2view ("ModelView" matrix) and view2clip ("Projection" matrix) transforms on a unit sphere looking at the center
     :param n_cams: number of cameras
     :param radius: radius of the sphere
     :param normal: if provided, only the hemisphere in the direction of the normal is sampled
@@ -327,130 +394,96 @@
     v2w = matrices  # c2w
     w2v = torch.inverse(v2w)
     v2c = perspective_projection()
     v2c = np.tile(v2c[None, :], (n_cams, 1, 1))
     v2c = torch.tensor(v2c, dtype=torch.float32, device=device)
     return w2v, v2c
 
-def to_np(arr: torch.Tensor):
-    """
-    converts a tensor to numpy array
-    :param arr: tensor
-    :return: numpy array
-    """
-    if type(arr) == torch.Tensor:
-        return arr.detach().cpu().numpy()
-    elif type(arr) == np.ndarray:
-        return arr
-    elif type(arr) == Image.Image:
-        return np.array(arr)
-    return arr.detach().cpu().numpy()
-
-def to_numpy(arr: torch.Tensor):
-    """
-    converts a tensor to numpy array
-    :param arr: tensor
-    :return: numpy array
-    """
-    return to_np(arr)
-
-def to_torch(arr: np.array, device="cpu", dtype=None):
-    """
-    converts a numpy array to a torch tensor
-    :param arr: numpy array
-    :param dtype: dtype of the tensor
-    :param device: device to put the tensor on
-    :return: torch tensor
+def pixels_in_world_space(camera_wh, K, Rt):
     """
-    if dtype is None:
-        return torch.tensor(arr, device=device)
-    else:
-        return torch.tensor(arr, dtype=dtype, device=device)
+    computes pinhole camera pixel locations in world space
+    :param camera_wh: resolution (width, height) as a tuple
+    :param K: the camera instrinsics matrix 3x3
+    :param Rt: the camera to world matrix 4x4
+    :return: np array n x 3 for pixels locations (in world space)
+    """
+    x, y = np.meshgrid(np.arange(camera_wh[0], dtype=np.float32),
+                       np.arange(camera_wh[1], dtype=np.float32), indexing='xy')
+    x = x.reshape(-1)[:, None]
+    y = y.reshape(-1)[:, None]
+    ones = np.ones(len(x))[:, None]
+    pixels_image = np.concatenate((x, y, ones), axis=-1)
+    pixels_camera = np.linalg.inv(K) @ pixels_image.T
+    pixels_camera_hom = np.concatenate((pixels_camera.T, np.ones(len(pixels_camera.T))[:, None]), axis=-1)
+    pixels_world = Rt @ pixels_camera_hom.T
+    pc = pixels_world.T[:, :3]
+    return pc
 
-def to_8b(x, clip=True):
+def random_qvec(n: int):
     """
-    convert an array (float, double) array to 8 bit
-    :param x: array
-    :param clip: if True, clips values to [0,1]
-    :return: 8 bit array
-    """
-    if is_np(x):
-        if x.dtype == np.float32 or x.dtype == np.float64:
-            if clip:
-                x = np.clip(x, 0, 1)
-            return (255 * x).round().astype(np.uint8)
-        elif x.dtype == bool:
-            return x.astype(np.uint8) * 255
-        elif x.dtype == np.uint8:
-            return x
-    else:
-        if x.dtype == torch.float32 or x.dtype == torch.float64:
-            if clip:
-                x = torch.clamp(x, 0, 1)
-            return (255 * x).round().type(torch.uint8)
-        elif x.dtype == torch.bool:
-            return x.type(torch.uint8) * 255
-        elif x.dtype == torch.uint8:
-            return x
-
-def to_float(x, clip=True):
-    """
-    convert a 8bit or bool array to float
-    :param x: array
-    :param clip: if True, clips values to [0,1]
-    :return: float array
-    """
-    if is_np(x):
-        if x.dtype == np.uint8:
-            return x.astype(np.float32) / 255
-        elif x.dtype == np.float32:
-            if clip:
-                x = np.clip(x, 0, 1)
-            return x
-        elif x.dtype == bool:
-            return x.astype(np.float32)
-        else:
-            raise ValueError("unsupported dtype")
-    else:
-        if x.dtype == torch.uint8:
-            return x.to(torch.float32) / 255
-        elif x.dtype == torch.float32:
-            if clip:
-                x = torch.clamp(x, 0, 1)
-            return x
-        elif x.dtype == torch.bool:
-            return x.to(torch.float32)
-        else:
-            raise ValueError("unsupported dtype")
+    generate random quaternions representing rotations
+    :param n: Number of quaternions in a batch to return.
+    :return: Quaternions as tensor of shape (N, 4).
+    """
+    o = np.random.randn(n, 4)
+    s = (o * o).sum(1)
+    denom = np.copysign(np.sqrt(s), o[:, 0])[:, None]
+    o = o / denom
+    return o
 
-def to_PIL(x: np.array):
+def random_affine(ang_range=20.0, trans_range=10.0, scale=2.0):
     """
-    convert a numpy float array to a PIL image
+    generates a random 2D affine transformation matrix
     """
-    if x.ndim == 3:
-        return Image.fromarray(to_8b(x))
-    elif x.ndim == 2:
-        return Image.fromarray(to_8b(x[:, :, None]), mode="L")
-    else:
-        raise ValueError("unsupported array dimensions")
+    R = np.eye(3)
+    ang_rot = np.random.uniform(ang_range)-ang_range/2
+    tx = trans_range*np.random.uniform()-trans_range/2
+    ty = trans_range*np.random.uniform()-trans_range/2
+    sx = np.random.rand() * scale
+    sy = np.random.rand() * scale
+    R[0, 0] = np.cos(ang_rot * np.pi / 180)
+    R[0, 1] = -np.sin(ang_rot * np.pi / 180)
+    R[1, 0] = np.sin(ang_rot * np.pi / 180)
+    R[1, 1] = np.cos(ang_rot * np.pi / 180)
+    T = np.eye(3)
+    T[0, 2] = tx
+    T[1, 2] = ty
+    S = np.eye(3)
+    S[0, 0] = sx
+    S[1, 1] = sy
+    H = T @ S @ R
+    return H
 
-def map_range(x, out_min, out_max):
+def random_perspective():
     """
-    given an input and a range, maps it to a new range
+    generates a random 2D perspective transformation matrix
     """
-    if type(x) == np.ndarray:
-        return np.clip((x-x.min()) * (out_max-out_min) / (x.max()-x.min()) + out_min, out_min, out_max)
-    elif type(x) == torch.Tensor:
-        return torch.clamp((x-x.min()) * (out_max-out_min) / (x.max()-x.min()) + out_min, out_min, out_max)
-    else:
-        raise ValueError("unsupported type")
-
-def map_to_01(x):
-    return map_range(x, 0, 1)
+    P = random_affine()
+    P[2, 0] = np.random.rand() / 100
+    P[2, 1] = np.random.rand() / 100
+    return P
 
+def random_vectors_on_sphere(n, normal=None, device="cpu"):
+    """
+    create a batch of uniformly distributed random unit vectors on a sphere
+    note: if normal is provided, returns random unit vectors on the hemisphere around the normal, but isn't uniform anymore.
+    :param n: number of vectors
+    :param normal: normals to orient the hemisphere (,3) or (n,3)
+    :param device: device to put the tensors on
+    :return: tensor of shape (n, 3)
+    """
+    locs = torch.randn((n, 3), device=device)
+    locs = torch.nn.functional.normalize(locs, dim=1, eps=1e-6)
+    if normal is not None:
+        if normal.ndim == 1:
+            normal = normal[None, :]
+        normal = torch.nn.functional.normalize(normal, dim=-1, eps=1e-6)
+        dot_product = (locs[:, None, :] @ normal[:, :, None]).squeeze()
+        locs[dot_product < 0] *= -1
+    return locs
 
 def vec2skew(v):
     """
     returns the skew operator matrix given a vector
     :param v:  (3, ) torch tensor
     :return:   (3, 3)
     """
@@ -500,77 +533,14 @@
     # ortho = torch.cross(rotvec, up)
     # ortho = ortho / ortho.norm(keepdim=True)
     # angle1 = torch.arccos(ortho.dot(r @ ortho))
     angle2 = torch.arccos((torch.trace(r) - 1) / 2)
     raise NotImplementedError("please verify this function implementation before usage")
     return rotvec * angle2
 
-def random_qvec(n: int):
-    """
-    generate random quaternions representing rotations
-    :param n: Number of quaternions in a batch to return.
-    :return: Quaternions as tensor of shape (N, 4).
-    """
-    o = np.random.randn(n, 4)
-    s = (o * o).sum(1)
-    denom = np.copysign(np.sqrt(s), o[:, 0])[:, None]
-    o = o / denom
-    return o
-
-def random_affine(ang_range=20.0, trans_range=10.0, scale=2.0):
-    """
-    generates a random 2D affine transformation matrix
-    """
-    R = np.eye(3)
-    ang_rot = np.random.uniform(ang_range)-ang_range/2
-    tx = trans_range*np.random.uniform()-trans_range/2
-    ty = trans_range*np.random.uniform()-trans_range/2
-    sx = np.random.rand() * scale
-    sy = np.random.rand() * scale
-    R[0, 0] = np.cos(ang_rot * np.pi / 180)
-    R[0, 1] = -np.sin(ang_rot * np.pi / 180)
-    R[1, 0] = np.sin(ang_rot * np.pi / 180)
-    R[1, 1] = np.cos(ang_rot * np.pi / 180)
-    T = np.eye(3)
-    T[0, 2] = tx
-    T[1, 2] = ty
-    S = np.eye(3)
-    S[0, 0] = sx
-    S[1, 1] = sy
-    H = T @ S @ R
-    return H
-
-def random_perspective():
-    """
-    generates a random 2D perspective transformation matrix
-    """
-    P = random_affine()
-    P[2, 0] = np.random.rand() / 100
-    P[2, 1] = np.random.rand() / 100
-    return P
-
-def random_vectors_on_sphere(n, normal=None, device="cpu"):
-    """
-    create a batch of uniformly distributed random unit vectors on a sphere
-    note: if normal is provided, returns random unit vectors on the hemisphere around the normal, but isn't uniform anymore.
-    :param n: number of vectors
-    :param normal: normals to orient the hemisphere (,3) or (n,3)
-    :param device: device to put the tensors on
-    :return: tensor of shape (n, 3)
-    """
-    locs = torch.randn((n, 3), device=device)
-    locs = torch.nn.functional.normalize(locs, dim=1, eps=1e-6)
-    if normal is not None:
-        if normal.ndim == 1:
-            normal = normal[None, :]
-        normal = torch.nn.functional.normalize(normal, dim=-1, eps=1e-6)
-        dot_product = (locs[:, None, :] @ normal[:, :, None]).squeeze()
-        locs[dot_product < 0] *= -1
-    return locs
-
 def qvec2mat(qvec):
     """
     Converts a quaternion to a rotation matrix
     :param qvec: tensor of size 4 where real part is first (a + bi + cj + dk) => (a, b, c, d)
     :return: rotation matrix 3x3
     """
     return batch_qvec2mat(qvec[None, :])[0]
```

### Comparing `gsoup-0.0.9/src/gsoup/geometry_advanced.py` & `gsoup-0.1.0/src/gsoup/geometry_advanced.py`

 * *Files identical despite different names*

### Comparing `gsoup-0.0.9/src/gsoup/geometry_basic.py` & `gsoup-0.1.0/src/gsoup/geometry_basic.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,33 @@
 import torch
 import numpy as np
-from .core import is_np
+from .core import is_np, broadcast_batch
 
+def edge_function(v0, v1, p):
+    """
+    returns the "edge function" which equals half the area of the traingle formed by v0, v1 and p
+    :param v0: first vertex of the triangle (3,)
+    :param v1: second vertex of the triangle (3,)
+    :param p: point to check (3,) or batch of points to check (B, 3)
+    """
+    return np.cross(v1 - v0, p - v0)
+
+def is_inside_triangle(p, v0, v1, v2):
+    """
+    checks if a point is inside a triangle
+    :param p: point or batch of points to check (3,)
+    :param v0: first vertex of the triangle (3,)
+    :param v1: second vertex of the triangle (3,)
+    :param v2: third vertex of the triangle (3,)
+    """
+    a = np.all(edge_function(v0, v1, p) >= 0, axis=-1)
+    b = np.all(edge_function(v1, v2, p) >= 0, axis=-1)
+    c = np.all(edge_function(v2, v0, p) >= 0, axis=-1)
+    return a & b & c
+    
 def duplicate_faces(f):
     """
     duplicates *every* face in the mesh, with flipped orientation (and appends it to the end of the tensor)
     note: will transfer to CPU if necessary with current implementation
     :param f: faces of the mesh (Nx3)
     :return: faces of the mesh with duplicated faces
     """
@@ -237,34 +259,50 @@
     ratioA = np.sin((1 - t) * halfTheta) / sinHalfTheta
     ratioB = np.sin(t * halfTheta) / sinHalfTheta
     qm = qa*ratioA + qb*ratioB
     return qm
 
 def ray_ray_intersection(oa, da, ob, db):
     """
-    returns point closest to both rays of form o+t*d,
-    and a weight factor that goes to 0 if the lines are parallel
-    :param oa:
-    :param da:
-    :param ob:
-    :param db:
-    :return:
-    """
-    da = da / np.linalg.norm(da)
-    db = db / np.linalg.norm(db)
+    returns points closest to each corresponding ray of form o+t*d in t he bundle
+    :param oa: origin of ray a (b x 3)
+    :param da: direction of ray a (b x 3)
+    :param ob: origin of ray b (b x 3)
+    :param db: direction of ray b (b x 3)
+    :return: points closest to each ray (b x 3) and a weight factor that goes to 0 if the lines are parallel
+    """
+    batched_input = True
+    if oa.ndim == 1:
+        oa = oa[None, :]
+        batched_input = False
+    if da.ndim == 1:
+        da = da[None, :]
+        batched_input = False
+    if ob.ndim == 1:
+        ob = ob[None, :]
+        batched_input = False
+    if db.ndim == 1:
+        db = db[None, :]
+        batched_input = False
+    oa, ob, da, db = broadcast_batch(oa, ob, da, db)
+    da = da / np.linalg.norm(da, axis=1, keepdims=True)
+    db = db / np.linalg.norm(db, axis=1, keepdims=True)
     c = np.cross(da, db)
-    denom = np.linalg.norm(c) ** 2
+    denom = np.linalg.norm(c, axis=-1) ** 2
     t = ob - oa
-    ta = np.linalg.det([t, db, c]) / (denom + 1e-10)
-    tb = np.linalg.det([t, da, c]) / (denom + 1e-10)
-    if ta < 0:
-        ta = 0
-    if tb < 0:
-        tb = 0
-    return (oa + ta * da + ob + tb * db) * 0.5, denom
+    stackedb = np.concatenate([t[:, None, :], db[:, None, :], c[:, None, :]], axis=1)
+    stackeda = np.concatenate([t[:, None, :], da[:, None, :], c[:, None, :]], axis=1)
+    ta = np.linalg.det(stackedb) / (denom + 1e-10)
+    tb = np.linalg.det(stackeda) / (denom + 1e-10)
+    ta[ta < 0] = 0
+    tb[tb < 0] = 0
+    points = (oa + ta[:, None] * da + ob + tb[:, None] * db) * 0.5
+    if not batched_input:
+        points = points[0]
+    return points, denom
 
 def get_center_of_attention(c2w):
     """
     find a central point of a batch of c2w transforms 4x4 they are all looking at.
     note: point is weighted by distance between lines.
     :param camera_poses: n x 4 x 4 np array of c2w matrices
     :return: the center of attention in 3d world coordinates
```

### Comparing `gsoup-0.0.9/src/gsoup/image.py` & `gsoup-0.1.0/src/gsoup/image.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import numpy as np
 import torch
 from PIL import Image, ImageDraw, ImageFont
 from scipy import interpolate, spatial
-from .core import to_8b, to_float, to_hom, homogenize, broadcast_batch, is_np, to_torch
+from .core import to_8b, to_float, to_hom, homogenize, broadcast_batch, is_np, to_torch, to_np
 from .structures import get_gizmo_coords
-from .gsoup_io import save_image
 
 def alpha_compose(images, backgrounds=None, bg_color=None):
     """
     composes a single or batch of RGBA images into a single or batch of RGB images.
+    if backgrounds is provided, will blend them with the images, otherwise will blend with bg_color.
     if no backgrounds or bg_color is provided, the background is assumed to be black.
     :param image: b x H x W x 4 or H x W x 4
     :param background: b x H x W x 3 or H x W x 3
     :param bg_color: 3 or b x 3 float32 array
     :return: b x H x W x 3 or H x W x 3
     """
     if images.ndim != 3 and images.ndim != 4:
@@ -47,14 +47,15 @@
     :param text_per_image: b x 1 numpy array of strings
     :param fill_white: if True, text is white, otherwise black
     :return: new (b x H x W x 3) numpy array with text written
     """
     is_numpy = is_np(images)
     if not is_numpy:
         device = images.device
+        images = to_np(images)
     is_float = images.dtype == np.float32
     if is_float:
         images = to_8b(images)
     rgbs = [Image.fromarray(x) for x in images]
     font = ImageFont.truetype("./FreeMono.ttf", 48)
     if fill_white:
         fill = "white"
@@ -268,24 +269,23 @@
         x0 = spacing_x * i
         y0 = spacing_y * i
         img1.ellipse([x0, y0, width - x0, height - y0], fill=tuple(np.random.randint(0, 255, size=(3,))))
     if dst is not None:
         img.save(str(dst))
     return np.array(img)
 
-def generate_gray_gradient(height, width, grayscale=False, vertical=True, flip=False, bins=10, dst=None):
+def generate_gray_gradient(height, width, grayscale=False, vertical=True, flip=False, bins=10):
     """
     generate a gray gradient image HxWx3
     :param height: height of the image
     :param width: width of the image
     :param grayscale: if True, the image is grayscale
     :param vertical: if True, the gradient is vertical
     :param flip: if True, the gradient is flipped
     :param bins: number of bins
-    :param dst: if not None, the image is written to this path
     :return: (H x W x 3) numpy array
     """
     bins = np.clip(bins, 1, 256)
     colors = np.linspace(0, 255, num=bins).astype(np.uint8)
     if vertical:
         n_bins = height // bins
         up_to_max_intensity = colors.repeat(n_bins)[:height]
@@ -306,63 +306,16 @@
         else:
             channel = up_to_max_intensity
         img = channel[None, :].repeat(height, axis=0)
         if flip:
             img = np.flip(img, axis=1)
     if not grayscale:
         img = img[:, :, None].repeat(3, axis=-1)
-    if dst is not None:
-        save_image(img, dst)
     return img
 
-def interpolate_single_channel(image: np.ndarray, mask: np.ndarray, method: str = "linear", fill_value: int = 0):
-    """
-    :param image: (H x W) numpy array
-    :param mask: (H x W) boolean numpy array, True indicates missing values
-    :param method: interpolation method, one of
-        'nearest', 'linear', 'cubic'.
-    :param fill_value: which value to use for filling up data outside the
-        convex hull of known pixel values.
-        Default is 0, Has no effect for 'nearest'.
-    :return: the image with missing values interpolated
-    """
-    h, w = image.shape[:2]
-    xx, yy = np.meshgrid(np.arange(w), np.arange(h))
-
-    known_x = xx[~mask]
-    known_y = yy[~mask]
-    known_v = image[~mask]
-    missing_x = xx[mask]
-    missing_y = yy[mask]
-
-    interp_values = interpolate.griddata(
-        (known_x, known_y), known_v, (missing_x, missing_y),
-        method=method, fill_value=fill_value
-    )
-
-    interp_image = image.copy()
-    interp_image[missing_y, missing_x] = interp_values
-
-    return interp_image
-
-def interpolate_multi_channel(image: np.ndarray, mask: np.ndarray):
-    """
-    given a multi channel image and a mask, interpolate the values where mask is true (per channel interpolation)
-    :param image: (H x W x C) numpy array
-    :param mask: (H x W) numpy array
-    :return: (H x W x C) numpy array
-    """
-    if image.ndim != 3:
-        raise ValueError("image must have atleast 1 channel")
-    interpolated = np.zeros_like(image)
-    for channel in range(image.shape[-1]):
-        interpolated_channel = interpolate_single_channel(image[:, :, channel], mask)
-        interpolated[:, :, channel] = interpolated_channel
-    return interpolated
-
 def image_grid(images, rows, cols):
     """
     :param images: list of images
     :param rows: number of rows
     :param cols: number of cols
     :return: grid image
     """
```

### Comparing `gsoup-0.0.9/src/gsoup/procam.py` & `gsoup-0.1.0/src/gsoup/procam.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import numpy as np
-import torch
 import cv2
 from .gsoup_io import save_image, save_images, load_images, load_image
-from .core import to_8b
-from .image import interpolate_multi_channel, change_brightness
+from .transforms import compose_rt
+from .core import to_8b, to_hom, swap_columns
+from .image import change_brightness
+from .geometry_basic import ray_ray_intersection
 from pathlib import Path
 from scipy.interpolate import LinearNDInterpolator
 
-def warp_image(backward_map, desired_image, cam_wh=None, output_path=None):
+def warp_image(backward_map, desired_image, cam_wh=None, mode="xy", output_path=None):
     """
     given a 2D dense map of corresponding pixels between projector and camera, computes a warped image such that if projected, the desired image appears when observed using camera
     :param backward_map: 2D dense mapping between pixels from projector 2 camera (proj_h x proj_w x 2) uint32
     :param desired_image: path to desired image from camera, or float np array channels last (cam_h x cam_w x 3) uint8
     :param cam_wh: device1 (width, height) as tuple, if not supplied assumes desired_image is in the correct dimensions in relation to backward_map
+    :param mode: "xy" or "ij" depending on the last channel of backward_map
     :param output_path: path to save warped image to
     :return: warped image (proj_h x proj_w x 3) uint8
     """
     if backward_map.ndim != 3:
         raise ValueError("backward_map must be 3D")
     if backward_map.shape[-1] != 2:
         raise ValueError("backward_map must have shape (cam_h, cam_w, 2)")
@@ -24,42 +26,59 @@
         if desired_image.ndim != 3:
             raise ValueError("desired_image must be 3D")
     else:
         if cam_wh is not None:
             desired_image = load_image(desired_image, resize_wh=cam_wh)
         else:
             desired_image = load_image(desired_image)
-    warpped = desired_image[(backward_map[..., 0], backward_map[..., 1])]
+    if mode == "xy":
+        warpped = desired_image[(backward_map[..., 1], backward_map[..., 0])]
+    elif mode == "ij":
+        warpped = desired_image[(backward_map[..., 0], backward_map[..., 1])]
+    else:
+        raise ValueError("mode must be 'xy' or 'ij'")
     if output_path is not None:
         output_path = Path(output_path)
         output_path.parent.mkdir(parents=True, exist_ok=True)
         save_image(warpped, output_path)
     return warpped
 
-def compute_backward_map(proj_wh, forward_map, foreground, output_dir=None, debug=False): 
+def compute_backward_map(proj_wh, forward_map, foreground, mode="ij", interpolate=True, output_dir=None, debug=False): 
     """
-    computes the inverse map of forward_map by piece-wise interpolating a triangulated version of it.
+    computes the inverse map of forward_map by piece-wise interpolating a triangulated version of it (see GrayCode.decode to understand forward_map)
     :param proj_wh: projector (width, height) as a tuple
     :param forward_map: forward map as a numpy array of shape (height, width, 2) of type int32
+    :param foreground: a boolean mask of shape (height, width) where True indicates a valid pixel in forward_map
+    :param interpolate: if False, output will not be interpolated (will have holes...)
+    :param mode: the last channel order of forward_map. either "xy" (width first) or "ij" (height first).
     :param output_dir: directory to save the inverse map to
-    :param debug: if True, saves a visualization of the inverse map to output_dir
-    :return: inverse map as a numpy array of shape (projector_height, projector_width, 2) of type int32
+    :param debug: if True, saves a visualization of the backward map to output_dir (R=X, G=Y, B=0) where X increases from left to right and Y increases from top to bottom
+    :return: backward map as a numpy array of shape (projector_height, projector_width, 2) of type int32, last channel encodes (height, width).
     """   
     if output_dir is not None:
         output_dir = Path(output_dir)
         output_dir.mkdir(parents=True, exist_ok=True)
-    data = np.argwhere(foreground)
+    data = np.argwhere(foreground)  # always ij
     points = forward_map[foreground]
-    interp = LinearNDInterpolator(points, data, fill_value=0.0)
-    X, Y = np.meshgrid(np.arange(proj_wh[1]), np.arange(proj_wh[0]))
-    result = interp(X, Y).transpose(1, 0, 2)  # eww
+    if interpolate:
+        interp = LinearNDInterpolator(points, data, fill_value=0.0)
+        X, Y = np.meshgrid(np.arange(proj_wh[0]), np.arange(proj_wh[1]))
+        result = interp(X, Y).transpose(1, 0, 2)  # eww
+    else:
+        sparse_map = np.zeros((proj_wh[1], proj_wh[0], 2), dtype=np.uint32)
+        if mode == "xy":
+            sparse_map[(points[:, 1]), (points[:, 0])] = data
+        elif mode == "ij":
+            sparse_map[(points[:, 0]), (points[:, 1])] = data
+        result = sparse_map
     if output_dir:
         np.save(Path(output_dir, "backward_map.npy"), result)
         if debug:
             result_normalized = result / np.array([forward_map.shape[0], forward_map.shape[1]])
+            result_normalized[..., [0, 1]] = result_normalized[..., [1, 0]]
             result_normalized_8b = to_8b(result_normalized)
             result_normalized_8b_3c = np.concatenate((result_normalized_8b, np.zeros_like(result_normalized_8b[..., :1])), axis=-1)
             save_image(result_normalized_8b_3c, Path(output_dir, "backward_map.png"))
     return result.round().astype(np.uint32)
 
 def naive_color_compensate(target_image, all_white_image, all_black_image, cam_width, cam_height, brightness_decrease=-127, projector_gamma=2.2, output_path=None, debug=False):
     """
@@ -88,42 +107,60 @@
     compensated = np.power(compensated, (1/projector_gamma))
     compensated = np.nan_to_num(compensated, nan=0.0, posinf=0.0, neginf=0.0)
     compensated = np.clip(compensated, 0, 1)
     if output_path:
         save_image(compensated, output_path)
     return compensated
 
-def calibrate_procam(proj_height, proj_width, graycode_step, capture_dir, 
+def calibrate_procam(proj_wh, capture_dir, 
                      chess_vert=10, chess_hori=7,
-                     black_thr=40, chess_block_size=10.0, verbose=True):
+                     bg_threshold=10, chess_block_size=10.0, projector_orientation="from_above", verbose=True,
+                     output_dir=None, debug=False):
     """
     calibrates a projection-camera pair using local homographies
     based on "Simple, accurate, and robust projector-camera calibration."
-    :param proj_height projector pixel height
-    :param proj_width projector pixel width
+    note1: the calibration poses some reasonable constraints on the projector-camera pair:
+    1) projector is assumed to have no distortion, and a square pixel aspect ratio.
+    2) camera is assumed to have a square pixel aspect ratio, and principle axis is assumed to be the center of the image.
+    3) both elements are assumed to have no tangential distortion.
+    note2: recommendations for calibration:
+    1) use a chessboard with as many blocks as possible, but make sure the chessboard is fully visible in the camera image and in focus.
+    2) capture sessions should span the whole image plane, and should be as diverse as possible in terms of poses (tilt the checkerboard !)
+    3) when tilting the checkerboard, do not tilt it too much or the projector pixels will get smeared and the gray code decoding will produce large errors.
+    4) place the checkeboard only in the working zone of the projector, i.e. the area where the projector is in focus.
+    5) make sure the full dynamic range of the camera is used, i.e. the blackest black and whitest white should be visible in the captured images.
+    6) attach the checkerboard to a flat surface, make sure the final pattern is as flat as possible. any bending will cause large errors.
+    7) capture as many sessions as possible, if a session is not good (use debug=True to check), discard it.
+    8) the RMS is only a rough estimate of the calibration quality, but if it is below 1, the calibration should be good enough (units are pixels).
+    :param proj_wh projector resolution (width, height) as a tuple
     :param chess_vert number of cross points of chessboard in vertical direction (not including the border, i.e. internal corners)
     :param chess_hori number of cross points of chessboard in horizontal direction (not including the border, i.e. internal corners)
-    :param graycode_step factor used to downsample the graycode images (see generate_gray_code)
     :param capture_dir directory containing the captured images when gray code patterns were projected, assumes structure as follows:
         capture_dir
             - folder1
                 - 0000.png
                 - 0001.png
                 - ...
             - folder2
                 - 0000.png
                 - ...
-    :param black_thr threshold for detecting black pixels in the chessboard
+    :param bg_threshold threshold for detecting foreground
     :param chess_block_size size of blocks of chessboard in real world in any unit of measurement (will only effect the translation componenet between camera and projector)
+    :param projector_orientation -  effects initial guess for projector principal point.
+                                    can be "from_above" or "from_below", or "none".
     :param verbose if true, will print out the calibration results
-    :return camera intrinsics, camera extrinsics, projector intrinsics, projector extrinsics, cam_proj_rmat, cam_proj_tvec
+    :param output_dir will save debug results to this directory
+    :param debug if true, will save debug info into output_dir
+    :return camera intrinsics (3x3),
+            camera distortion parameters (5x1),
+            projector intrinsics (3x3),
+            projector distortion parameters (5x1),
+            proj_transform (4x4), a projector to camera transformation matrix (to get p2w, you should invert this matrix and multiply from the left with the camera to world matrix)
     """
-    proj_shape = (proj_height, proj_width)
     chess_shape = (chess_vert, chess_hori)
-    gc_step = graycode_step
     capture_dir = Path(capture_dir)
     if not capture_dir.exists():
         raise FileNotFoundError("capture_dir was not found")
     dirnames = sorted(capture_dir.glob('*'))
     if len(dirnames) == 0:
         raise FileNotFoundError("capture_dir contains no subfolders")
     used_dirnames = []
@@ -134,27 +171,31 @@
             continue
         used_dirnames.append(str(dname))
         gc_fname_lists.append([str(x) for x in gc_fnames])
     dirnames = used_dirnames
     objps = np.zeros((chess_shape[0]*chess_shape[1], 3), np.float32)
     objps[:, :2] = chess_block_size * np.mgrid[0:chess_shape[0], 0:chess_shape[1]].T.reshape(-1, 2)
     graycode = GrayCode()
-    patterns = graycode.encode((proj_shape[1], proj_shape[0]))
-    cam_shape = load_image(gc_fname_lists[0][0], as_grayscale=True).shape
-    patch_size_half = int(np.ceil(cam_shape[1] / 180))
+    patterns = graycode.encode(proj_wh)
+    cam_shape = load_image(gc_fname_lists[0][0], as_grayscale=True).shape[::-1]  # width, height
+    patch_size_half = int(np.ceil(cam_shape[0] / 180))  # some magic number for patch size
     cam_corners_list = []
     cam_objps_list = []
     cam_corners_list2 = []
     proj_objps_list = []
     proj_corners_list = []
     for dname, gc_filenames in zip(dirnames, gc_fname_lists):
+        if verbose:
+            print("processing: {}".format(dname))
         if len(gc_filenames) != len(patterns):
             raise ValueError("invalid number of images in " + dname)
         imgs = load_images(gc_filenames, as_grayscale=True)[..., None]
-        forwardmap, fg = graycode.decode(imgs, (proj_shape[1], proj_shape[0]), mode="ij")
+        forwardmap, fg = graycode.decode(imgs, proj_wh, mode="xy",
+                                         bg_threshold=bg_threshold,
+                                         output_dir=output_dir, debug=debug)
         black_img = imgs[-1]
         white_img = imgs[-2]
         imgs = imgs[:-2]
         res, cam_corners = cv2.findChessboardCorners(white_img, chess_shape)
         if not res:
             raise RuntimeError("chessboard was not found in {}".format(gc_filenames[-2]))
         cam_objps_list.append(objps)
@@ -168,20 +209,18 @@
             src_points = []
             dst_points = []
             # todo: vectorize these loops
             for dx in range(-patch_size_half, patch_size_half + 1):
                 for dy in range(-patch_size_half, patch_size_half + 1):
                     x = c_x + dx
                     y = c_y + dy
-                    if int(white_img[y, x]) - int(black_img[y, x]) <= black_thr:
-                        continue
                     if fg[y, x]:
-                        proj_pix = forwardmap[y, x]  # backward map ?
+                        proj_pix = forwardmap[y, x]
                         src_points.append((x, y))
-                        dst_points.append(gc_step*np.array(proj_pix))
+                        dst_points.append(np.array(proj_pix))
             if len(src_points) < patch_size_half**2:
                 if verbose:
                     print('corner {}, {} was skiped because too few decoded pixels found (check your images and thresholds)'.format(c_x, c_y))
                 continue
             h_mat, inliers = cv2.findHomography(
                 np.array(src_points), np.array(dst_points))
             point = h_mat@np.array([corner[0][0], corner[0][1], 1]).transpose()
@@ -190,43 +229,128 @@
             proj_corners.append([point_pix])
             cam_corners2.append(corner)
         if len(proj_corners) < 3:
             raise RuntimeError("too few corners were found in {} (less than 3)".format(dname))
         proj_objps_list.append(np.float32(proj_objps))
         proj_corners_list.append(np.float32(proj_corners))
         cam_corners_list2.append(np.float32(cam_corners2))
-
+    if verbose:
+        print("total correspondence points: {}".format(sum([len(x) for x in proj_corners_list])))
     # Initial solution of camera's intrinsic parameters
+    # camera_intrinsics_init = np.array([[np.mean(cam_shape), 0, cam_shape[0]/2], [0, np.mean(cam_shape), cam_shape[1]/2], [0, 0, 1]])
     ret, cam_int, cam_dist, cam_rvecs, cam_tvecs = cv2.calibrateCamera(
-        cam_objps_list, cam_corners_list, cam_shape, None, None, None, None)
+        cam_objps_list, cam_corners_list, cam_shape, None , None, None, None,  # camera_intrinsics_init
+        cv2.CALIB_FIX_ASPECT_RATIO  + cv2.CALIB_FIX_PRINCIPAL_POINT)  # + cv2.CALIB_ZERO_TANGENT_DIST  # cv2.CALIB_USE_INTRINSIC_GUESS
     if verbose:
-        print('Initial camera intrinsic parameters: {}'.format(cam_int))
-        print('Initial camera distortion parameters: {}'.format(cam_dist))
-        print('Initial camera RMS: {}'.format(ret))
+        print('Camera calib. intrinsic parameters: {}'.format(cam_int))
+        print('Camera calib. distortion parameters: {}'.format(cam_dist))
+        print('Camera calib. reprojection error: {}'.format(ret))
 
     # Initial solution of projector's parameters
+    if projector_orientation == "none":
+        cy_correction = 0
+    elif projector_orientation == "from_below":
+        cy_correction = proj_wh[1] / 4
+    elif projector_orientation == "from_above":
+        cy_correction = - proj_wh[1] / 4
+    else:
+        raise ValueError("invalid projector_orientation")
+    projector_intrinsics_init = np.array([[np.mean(proj_wh), 0, proj_wh[0]/2], [0, np.mean(proj_wh), cy_correction + proj_wh[1]/2], [0, 0, 1]])
+    projector_ditortion_init = np.zeros((5, 1))
     ret, proj_int, proj_dist, proj_rvecs, proj_tvecs = cv2.calibrateCamera(
-        proj_objps_list, proj_corners_list, proj_shape, None, None, None, None)
+        proj_objps_list, proj_corners_list, proj_wh, projector_intrinsics_init, projector_ditortion_init, None, None,
+        cv2.CALIB_USE_INTRINSIC_GUESS + cv2.CALIB_FIX_ASPECT_RATIO + cv2.CALIB_ZERO_TANGENT_DIST + cv2.CALIB_FIX_K1 + cv2.CALIB_FIX_K2 + cv2.CALIB_FIX_K3)
+    
     if verbose:
-        print('Initial projector intrinsic parameters: {}'.format(proj_int))
-        print('Initial projector distortion parameters: {}'.format(proj_dist))
-        print('Initial projector RMS: {}'.format(ret))
+        print('Projector calib. intrinsic parameters: {}'.format(proj_int))
+        print('Projector calib. distortion parameters: {}'.format(proj_dist))
+        print('Projector calib. reprojection error: {}'.format(ret))
 
     # Stereo calibration for final solution
     ret, cam_int, cam_dist, proj_int, proj_dist, cam_proj_rmat, cam_proj_tvec, E, F = cv2.stereoCalibrate(
         proj_objps_list, cam_corners_list2, proj_corners_list, cam_int, cam_dist, proj_int, proj_dist, None)
     
+    proj_transform = compose_rt(cam_proj_rmat[None, ...], cam_proj_tvec[None, :, 0], square=True)[0]
     if verbose:
-        print('RMS: {}'.format(ret))
-        print('Camera intrinsic parameters: {}'.format(cam_int))
-        print('Camera distortion parameters: {}'.format(cam_dist))
-        print('Projector intrinsic parameters: {}'.format(proj_int))
-        print('Projector distortion parameters: {}'.format(proj_dist))
-        print('Rotation matrix / translation vector from camera to projector (cam2proj transform): {}, {}'.format(cam_proj_rmat, cam_proj_tvec))
-    return cam_int, cam_dist, proj_int, proj_dist, cam_proj_rmat, cam_proj_tvec
+        print('Stereo reprojection error: {}'.format(ret))
+        print('Stereo camera intrinsic parameters: {}'.format(cam_int))
+        print('Stereo camera distortion parameters: {}'.format(cam_dist))
+        print('Stereo projector intrinsic parameters: {}'.format(proj_int))
+        print('Stereo projector distortion parameters: {}'.format(proj_dist))
+        print('Stereo projector2camera transform): {}'.format(proj_transform))
+    if debug:
+        # computes a histogram of camera reprojection errors, and not just average error
+        cam_corners = np.array(cam_corners_list).squeeze()
+        proj_corners = np.array(proj_corners_list).squeeze()
+        obj_corners = np.array(cam_objps_list).squeeze()
+        all_projected_cam_corners = []
+        all_projected_proj_corners = []
+        for i in range(len(cam_corners)):
+            projected_cam_points, _ = cv2.projectPoints(obj_corners[i], cam_rvecs[i], cam_tvecs[i], cam_int, cam_dist)
+            all_projected_cam_corners.append(projected_cam_points)
+            projected_proj_points, _ = cv2.projectPoints(obj_corners[i], proj_rvecs[i], proj_tvecs[i], proj_int, proj_dist)
+            all_projected_proj_corners.append(projected_proj_points)
+        all_projected_cam_corners = np.array(all_projected_cam_corners).squeeze()
+        cam_norms = np.linalg.norm(cam_corners - all_projected_cam_corners, axis=-1)
+        cam_per_session_error = cam_norms.mean(axis=-1)
+        worst_to_best_cam_session_ids = np.argsort(cam_per_session_error)[::-1]
+        worst_to_best_cam_errors = cam_per_session_error[worst_to_best_cam_session_ids]
+        print("worst to best sessions ids for camera reprojection error: {}".format(worst_to_best_cam_session_ids))
+        print("and their associated errors: {}".format(worst_to_best_cam_errors))
+        cam_hist = np.histogram(cam_norms)
+        print('camera reprojection error histogram: {} (should be similar to gaussian around 0)'.format(cam_hist))
+        all_projected_proj_corners = np.array(all_projected_proj_corners).squeeze()
+        proj_norms = np.linalg.norm(proj_corners - all_projected_proj_corners, axis=-1)
+        per_session_projector_error = proj_norms.mean(axis=-1)
+        worst_to_best_proj_session_ids = np.argsort(per_session_projector_error)[::-1]
+        worst_to_best_proj_errors = per_session_projector_error[worst_to_best_proj_session_ids]
+        print("worst to best sessions ids for camera reprojection error: {}".format(worst_to_best_proj_session_ids))
+        print("and their associated errors: {}".format(worst_to_best_proj_errors))
+        proj_hist = np.histogram(proj_norms)
+        print('projector reprojection error histogram: {} (should be similar to gaussian around 0)'.format(proj_hist))
+    return cam_int, cam_dist, proj_int, proj_dist, proj_transform
+
+def reconstruct_pointcloud(forward_map, fg, cam_transform, proj_transform, cam_int, cam_dist, proj_int, mode="xy", color_image=None, debug=False):
+    """
+    given a dense pixel correspondence map between a camera and a projector, and calibration results, reconstructs a 3D point cloud of the scene.
+    :param forward_map: a dense pixel correspondence map between a camera and a projector (see GrayCode.decode)
+    :param fg: a foreground mask of the scene (see GrayCode.decode)
+    :param cam_transform: a 4x4 transformation matrix of the camera (cam to world)
+    :param proj_transform: a 4x4 transformation matrix of the projector (proj to world)
+    :param cam_int: camera's intrinsic parameters
+    :param cam_dist: camera's distortion parameters
+    :param proj_int: projector's intrinsic parameters
+    :param mode: "xy" or "ij" which is the ordering of the last channel of the forward map (see GrayCode.decode)
+    :param color_image: RGB image with the same spatial size as forwardmap. if supplied will return a colored point cloud (Nx6).
+    :param debug: if True, will return debug information
+    :return: a 3D point cloud of the scene (Nx3)
+    """
+    cam_pixels = swap_columns(np.argwhere(fg), 0, 1)
+    cam_origins = cam_transform[None, :3, -1]
+    cam_directions = (cam_transform[:3, :3] @ (np.linalg.inv(cam_int) @ to_hom(cam_pixels).T)).T
+    cam_directions = cam_directions / np.linalg.norm(cam_directions, axis=-1, keepdims=True)
+    # todo: account for distortion if supplied
+    # undistorted_cam_points =  cv2.undistortPoints(cam_points, cam_int, cam_dist, P=proj_transform[0]).squeeze()  # equivalent to not setting P and doing K @ points outside
+    if mode == "xy":
+        projector_pixels = forward_map[fg]
+    elif mode == "ij":
+        projector_pixels = swap_columns(forward_map[fg], 0 , 1)
+    else:
+        raise ValueError("mode must be either 'xy' or 'ij'")
+    projector_origins = proj_transform[None, :3, -1]
+    projector_directions = (proj_transform[:3, :3] @ (np.linalg.inv(proj_int) @ to_hom(projector_pixels).T)).T
+    projector_directions = projector_directions / np.linalg.norm(projector_directions, axis=-1, keepdims=True)
+    points, weight_factor = ray_ray_intersection(cam_origins, cam_directions, projector_origins, projector_directions)
+    if color_image is not None:
+        colors = color_image[fg] if mode == "xy" else color_image[swap_columns(fg, 0, 1)]
+        points = np.concatenate([points, colors], axis=-1)
+    if debug:
+        return points, weight_factor, cam_origins, cam_directions, projector_origins, projector_directions, cam_pixels, projector_pixels
+    else:
+        return points
 
 class GrayCode:
     """
     a class that handles encoding and decoding graycode patterns
     """
     def encode1d(self, length):
         total_images = len(bin(length-1)[2:])
@@ -257,59 +381,59 @@
         all_images = np.concatenate((codes_width_2d, codes_height_2d), axis=0)
         if flipped_patterns:
             all_images = np.concatenate((all_images, 255-codes_width_2d), axis=0)
             all_images = np.concatenate((all_images, 255-codes_height_2d), axis=0)
         all_images = np.concatenate((all_images, img_white, img_black), axis=0)
         return all_images[..., None]
     
-    def binarize(self, captures, flipped_patterns=True, bg_threshold=5, bin_threshold=5):
+    def binarize(self, captures, flipped_patterns=True, bg_threshold=10):
         """
         binarize a batch of images
         :param captures: a 4D numpy array of shape (n, height, width, 1) of captured images
         :param flipped_patterns: if true, patterns also contain their flipped version for better binarization
-        :param bg_threshold: a threshold used for background detection using the all-white and all-black captures
-        :param bin_threshold: a threshold used for binarization between the flipped and non-flipped patterns
+        :param bg_threshold: if the difference between the pixel in the white&black images is greater than this, pixel is foreground
         :return: a 4D numpy binary array for decoding (total_images, height, width, 1) where total_images is the number of gray code patterns
         and a binary foreground mask (height, width, 1)
         """
-        captures, bw = captures[:-2], captures[-2:]
-        foreground = np.abs(bw[0].astype(np.int32) - bw[1].astype(np.int32)) > bg_threshold
-        # img_bin = np.zeros_like(captures, dtype=np.uint8)
+        if not -255 <= bg_threshold <= 255:
+            raise ValueError('bg_threshold must be between -255 and 255')
+        patterns, bw = captures[:-2], captures[-2:]
+        foreground = bw[0].astype(np.int32) - bw[1].astype(np.int32) > bg_threshold
         if flipped_patterns:
-            captures, flipped = captures[:len(captures)//2], captures[len(captures)//2:]
-            valid = np.abs(captures.astype(np.int32) - flipped.astype(np.int32)) > bin_threshold
-            binary = captures > flipped
-            foreground = foreground & np.all(valid, axis=0)  # do not use pixels that do not meet threshold in any of the images
-        else:  # slightly naive threhsolding
-            threhold = 0.5*(bw[1] + bw[0])
-            binary = captures >= threhold
+            orig, flipped = patterns[:len(patterns)//2], patterns[len(patterns)//2:]
+            # valid = (orig.astype(np.int32) - flipped.astype(np.int32)) > bin_threshold
+            binary = orig > flipped
+            # foreground = foreground & np.all(valid, axis=0)  # only pixels that are valid in all images are foreground
+        else:  # slightly more naive thresholding
+            binary = patterns >= 0.5*(bw[1] + bw[0])
         return binary, foreground
 
     def decode1d(self, gc_imgs):
         # gray code to binary
         n, h, w = gc_imgs.shape
         binary_imgs = gc_imgs.copy()
         for i in range(1, n):  # xor with previous image except MSB
             binary_imgs[i, :, :] = np.bitwise_xor(binary_imgs[i, :, :], binary_imgs[i-1, :, :])
         # decode binary
         cofficient = np.fromfunction(lambda i,y,x: 2**(n-1-i), (n,h,w), dtype=int)
         img_index = np.sum(binary_imgs * cofficient, axis=0)
         return img_index
 
     def decode(self, captures, proj_wh,
-               flipped_patterns=True, bg_threshold=10, bin_threshold=30,
-               mode="xy", output_dir=None, debug=False):
+               flipped_patterns=True, bg_threshold=10,
+               mode="ij", output_dir=None, debug=False):
         """
         decodes a batch of images encoded with gray code
-        :param captures: a 4D numpy array of shape (n, height, width, c) of captured images
+        :param captures: a 4D numpy array of shape (n, height, width, c) of captured images (camera resolution is inferred from this)
         :param flipped_patterns: if true, patterns also contain their flipped version for better binarization
-        :param bg_threshold: a threshold used for background detection using teh all-white and all-black captures
-        :param bin_threshold: a threshold used for binarization
-        :param mode: "xy" or "ij" decides the order of last dimension coordinates (ij -> height first, xy -> width first)
-        :return: a 2D numpy array of shape (height, width, 2) specifying the coordinates of decoded result, and foreground mask (height, width)
+        :param bg_threshold: a threshold used for background detection using the all-white and all-black captures
+        :param mode: "xy" or "ij" decides the order of last dimension coordinates in the output (ij -> height first, xy -> width first)
+        :param output_dir: if not None, saves the decoded images to this directory
+        :param debug: if True, visualizes the map in an image using the red and green channels where R=X, G=Y, B=0, X increases from left to right, Y increases from top to bottom
+        :return: a 2D numpy array of shape (height, width, 2) mapping from camera pixels to projector pixels, and a foreground mask (height, width)
         """
         if captures.ndim != 4:
             raise ValueError("captures must be a 4D numpy array")
         if captures.dtype != np.uint8:
             raise ValueError("captures must be uint8")
         if output_dir is not None:
             output_dir = Path(output_dir)
@@ -318,30 +442,35 @@
         b = b - 2 # dont count white and black images
         if flipped_patterns:
             b = b // 2  # dont count flipped patterns
         encoded = self.encode(proj_wh, flipped_patterns)  # sanity: encode with same arguments to verify enough captures are present
         if len(encoded) != len(captures):
             raise ValueError("captures must have length of {}".format(len(encoded)))
         if c != 1:  # naively convert to grayscale
-            captures = captures.mean(axis=-1, keepdims=True).astype(np.uint8)
-        imgs_binary, fg = self.binarize(captures, flipped_patterns, bg_threshold, bin_threshold)
+            captures = captures.mean(axis=-1, keepdims=True).round().astype(np.uint8)
+        imgs_binary, fg = self.binarize(captures, flipped_patterns, bg_threshold)
         imgs_binary = imgs_binary[:, :, :, 0]
         fg = fg[:, :, 0]
         x = self.decode1d(imgs_binary[:b // 2])
         y = self.decode1d(imgs_binary[b // 2:])
         if mode == "ij":
             forward_map = np.concatenate((y[..., None], x[..., None]), axis=-1)
         elif mode == "xy":
             forward_map = np.concatenate((x[..., None], y[..., None]), axis=-1)
         else:
             raise ValueError("mode must be 'ij' or 'xy'")
         if output_dir is not None:
             np.save(Path(output_dir, "forward_map.npy"), forward_map)
             if debug:
                 save_images(imgs_binary[..., None], Path(output_dir, "imgs_binary"))
+                save_image(fg, Path(output_dir, "foreground.png"))
                 composed = forward_map * fg[..., None]
-                composed_normalized = composed / np.array([proj_wh[1], proj_wh[0]])
+                if mode == "ij":
+                    composed_normalized = composed / np.array([proj_wh[1], proj_wh[0]])
+                    composed_normalized[..., [0, 1]] = composed_normalized[..., [1, 0]]
+                elif mode == "xy":
+                    composed_normalized = composed / np.array([proj_wh[0], proj_wh[1]])
                 composed_normalized_8b = to_8b(composed_normalized)
                 composed_normalized_8b_3c = np.concatenate((composed_normalized_8b, np.zeros_like(composed_normalized_8b[..., :1])), axis=-1)
                 save_image(composed_normalized_8b_3c, Path(output_dir, "forward_map.png"))
         return forward_map, fg
```

### Comparing `gsoup-0.0.9/src/gsoup/sphere_trace.py` & `gsoup-0.1.0/src/gsoup/sphere_trace.py`

 * *Files identical despite different names*

### Comparing `gsoup-0.0.9/src/gsoup/structures.py` & `gsoup-0.1.0/src/gsoup/structures.py`

 * *Files identical despite different names*

### Comparing `gsoup-0.0.9/src/gsoup/video.py` & `gsoup-0.1.0/src/gsoup/video.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,16 +32,18 @@
             # do something
             print(fps())
     """
     def __init__(self,avarageof=50):
         self.frametimestamps = collections.deque(maxlen=avarageof)
     def __call__(self):
         self.frametimestamps.append(time.time())
-        if(len(self.frametimestamps) > 1):
-            return len(self.frametimestamps)/(self.frametimestamps[-1]-self.frametimestamps[0])
+        nominator = len(self.frametimestamps)
+        denominator = self.frametimestamps[-1] - self.frametimestamps[0]
+        if(len(self.frametimestamps) > 1) and (denominator != 0):
+            return nominator / denominator
         else:
             return 0.0
 
 def get_video_info(video_path):
     """
     returns basic video info
     :param video_path: path to video
@@ -85,15 +87,15 @@
         .input(str(video_path))
         .output('pipe:', format='rawvideo', pix_fmt='rgb24')
         .run(capture_stdout=True, quiet=not verbose)
     )
     video = np.frombuffer(out, np.uint8).reshape([-1, h, w, 3])
     return video
 
-def save_video(frames, output_path, fps, lossy=False, verbose=False):
+def save_video(frames, output_path, fps, lossy=True, verbose=False):
     """
     saves a video from a t x h x w x 3 numpy tensor
     :param frames: (t x h x w x 3) numpy array or directory path containing images of same format and resolution
     :param output_path: path to save video to
     :param fps: frames per second of output video
     :param lossy: if True, use lossy compression (default: False, but then only .avi is supported)
     """
@@ -130,35 +132,37 @@
         if len(files) == 0:
             raise FileNotFoundError("No images found in directory: {}".format(frames))
         extensions = []
         for file in files:
             extensions.append(file.suffix)
         if len(set(extensions)) > 1:
             raise ValueError("All images in directory must have same extension")
-        glob_pattern = str(frames) + "/*" + extensions[0]
+        with open("ffmpeg_input.txt", "wb") as outfile:
+            for filename in files:
+                mystr = "file '{}'\n".format(str(filename.resolve()).replace("\\", "/"))
+                outfile.write(mystr.encode())
+        stdin_stream = None
+        stdout_stream = subprocess.PIPE if not verbose else None
+        stderr_stream = subprocess.PIPE if not verbose else None
         if lossy:
-            (
-                ffmpeg
-                .input(glob_pattern, pattern_type='glob', framerate=fps)
-                .output(str(output_path))
-                .run(quiet=not verbose)
-            )
+            # (
+            args = ["ffmpeg", "-y", "-f", "concat", "-safe", "0", "-i", "ffmpeg_input.txt", "-framerate", str(fps), str(output_path)]
         else:
             if output_path.suffix == ".avi":
                 pix_fmt = "bgr24"
             else:
                 # todo: figure out lossless pixel formats for other containers
                 raise ValueError("Lossless video only supported for .avi container")
-            (
-                ffmpeg
-                .input(glob_pattern, pattern_type='glob', pix_fmt='rgb24', r=fps)
-                .output(str(output_path), vcodec='rawvideo', pix_fmt=pix_fmt)
-                .overwrite_output()
-                .run(quiet=not verbose)
-            )
+            args = ["ffmpeg", "-y", "-f", "concat", "-safe", "0", "-i", "ffmpeg_input.txt", "-framerate", str(fps), "-pix_fmt", pix_fmt, "-vcodec", "rawvideo", str(output_path)]
+        proc = subprocess.Popen(args, stdin=stdin_stream, stdout=stdout_stream, stderr=stderr_stream)
+        out, err = proc.communicate(input)
+        retcode = proc.poll()
+        if retcode:
+            raise ValueError('ffmpeg', out, err)
+        Path("ffmpeg_input.txt").unlink()
     else:
         raise ValueError("frames must be numpy array or path to directory of images")
 
 def reverse_video(video_path, output_path=None, verbose=False):
     """
     reverses a video and possibly saves it to disk
     :param video_path: path to video
@@ -199,15 +203,15 @@
     creates a folder of images from a video
     """
     dst = Path(dst)
     dst.mkdir(parents=True, exist_ok=True)
     (
         ffmpeg
         .input(str(src))
-        .output(str(dst / '%d.png'), vcodec='png', format='image2')
+        .output(str(dst / '%04d.png'), vcodec='png', format='image2')
         .overwrite_output()
         .run(quiet=not verbose)
     )
 
 def slice_from_video(src, every_n_frames=2, start_frame=0, end_frame=None, verbose=False):
     """
     slices a video into frames
```

### Comparing `gsoup-0.0.9/src/gsoup/viewer.py` & `gsoup-0.1.0/src/gsoup/viewer.py`

 * *Files identical despite different names*

### Comparing `gsoup-0.0.9/src/gsoup/viewer_drivers.py` & `gsoup-0.1.0/src/gsoup/viewer_drivers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 from gsoup.viewer import gviewer
-from gsoup import structures
+from gsoup import structures, pixels_in_world_space, to_hom, ray_ray_intersection, swap_columns, reconstruct_pointcloud, load_image
 
 """
 a few example functions for using the viewer
 """
 
 #### globals 
 ui_float = 0.0
@@ -136,8 +136,57 @@
         v_tot, e_tot, c_tot = gviewer.register_camera("cameras", camera_poses, edge_rad, group_cameras)
     if meshes is not None:
         for i, mesh in enumerate(meshes):
             gviewer.register_mesh("mesh_{}".format(i), mesh[0], mesh[1], transparency=0.5)
     if pointclouds is not None:
         for i, pointcloud in enumerate(pointclouds):
             gviewer.register_pointcloud("pc_{}".format(i), pointcloud, radius=1e-4)
+    gviewer.show()
+
+def calibration_static_view(camera_pose, projector_pose, camera_wh, projector_wh, camera_intrinsics=None, camera_distortion=None, projector_intrinsics=None, forward_map=None, fg=None, mode="xy"):
+    """
+    visualizes a procam pair reconstruction
+    :param camera_pose: (4, 4) np array of camera to world transform
+    :param projector_pose: (4, 4) np array of projector to world transform
+    :param camera_wh: (2,) np array of camera resolution
+    :param projector_wh: (2,) np array of projector resolution
+    :param camera_intrinsics: (3, 3) np array of camera intrinsics
+    :param camera_distortion: (5,) np array of camera distortion
+    :param projector_intrinsics: (3, 3) np array of projector intrinsics
+    :param forward_map: (h, w, 2) np array of projector to camera mapping
+    :param fg: (h, w, 3) np array of projector fg
+    :param mode: "xy" or "ij" for forward map last channel encoding
+    """
+    gviewer.init(height=1024, width=1024)
+    gviewer.ps.set_up_dir("z_up")
+    edge_rad = 0.0005
+    v_aabb, e_aabb, c_aabb = structures.get_aabb_coords()
+    aabb_network = gviewer.ps.register_curve_network("aabb", v_aabb, e_aabb, radius=edge_rad)
+    aabb_network.add_color_quantity("color", c_aabb, defined_on='edges', enabled=True)
+    v_gizmo, e_gizmo, c_gizmo = structures.get_gizmo_coords(0.1)
+    gizmo_network = gviewer.ps.register_curve_network("gizmo", v_gizmo, e_gizmo, radius=edge_rad)
+    gizmo_network.add_color_quantity("color", c_gizmo, defined_on='edges', enabled=True)
+    coa = np.zeros((1, 3))
+    gviewer.register_pointcloud("center_of_world", coa, c=np.array([1., 1., 1.])[None, :], radius=0.005, mode="sphere")
+    v_tot, e_tot, c_tot = gviewer.register_camera("camera", camera_pose[None, ...], edge_rad, True)
+    v_tot, e_tot, c_tot = gviewer.register_camera("projector", projector_pose[None, ...], edge_rad, True)
+    camera_pixels = pixels_in_world_space(camera_wh, camera_intrinsics, camera_pose)
+    projector_pixels = pixels_in_world_space(projector_wh, projector_intrinsics, projector_pose)
+    # camera_screen_pc = gviewer.register_pointcloud("camera_screen", camera_pixels, radius=0.0002)
+    # projector_screen_pc = gviewer.register_pointcloud("projector_screen", projector_pixels, radius=0.0002)
+    points, weight_factor, \
+    cam_origins, cam_directions, \
+    projector_origins, projector_directions, \
+    cam_pixels, projector_pixels = reconstruct_pointcloud(forward_map, fg,
+                                                          camera_pose, projector_pose,
+                                                          camera_intrinsics, camera_distortion, projector_intrinsics,
+                                                          mode=mode, color_image=load_image("D:/src/gsoup/tests/tests_resource/correspondence/0025.png")[..., :3], debug=True)
+    reconst = gviewer.register_pointcloud("reconstruction", points[:, :3], c=points[:, 3:], radius=0.0002)
+    t = np.linspace(0, 3, 50)
+    cam_ray_points = cam_origins[0] + t[:, None]*cam_directions[0][None, :]
+    cam_ray = gviewer.ps.register_curve_network("cam_ray", cam_ray_points, "line", radius=0.0002)
+    proj_ray_points = projector_origins[0] + t[:, None]*projector_directions[0][None, :]
+    proj_ray = gviewer.ps.register_curve_network("proj_ray", proj_ray_points, "line", radius=0.0002)
+    ray_intersection = points[0:1, :3]
+    gviewer.register_pointcloud("ray_intersection", ray_intersection, c=np.array([1., 1., 1.])[None, :], radius=0.0005, mode="sphere")
+    ###
     gviewer.show()
```

### Comparing `gsoup-0.0.9/src/gsoup.egg-info/PKG-INFO` & `gsoup-0.1.0/src/gsoup.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gsoup
-Version: 0.0.9
+Version: 0.1.0
 Summary: A geoemtry & graphics library with focus on clarity rather than performance.
 Author-email: Yotam Erel <erelyotam@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Yotam Erel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,14 +30,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: build
 Provides-Extra: dev
+Provides-Extra: vis
 License-File: LICENSE
 
 # gsoup
 
 ## In a nutshell
 A python library implementing various geometry / graphics algorithms, with focus on clarity rather than performance.
```

### Comparing `gsoup-0.0.9/src/gsoup.egg-info/SOURCES.txt` & `gsoup-0.1.0/src/gsoup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gsoup-0.0.9/tests/test_basic.py` & `gsoup-0.1.0/tests/test_basic.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import pytest
 import numpy as np
 import torch
 import gsoup
 from pathlib import Path
+from gsoup.viewer_drivers import calibration_static_view
+
 
 def test_type_conversions():
     test_numpy_bool = np.array([1, 0, 0, 1], dtype=bool)
     test_torch_bool = gsoup.to_torch(test_numpy_bool)
 
     test_float_from_bool = gsoup.to_float(test_numpy_bool)
     assert test_float_from_bool.dtype == np.float32
@@ -157,24 +159,28 @@
 
     v = torch.rand(100, 3) * 100
     v_normalized = gsoup.normalize_vertices(v)
     assert (v_normalized < 1.0).all()
 
 def test_structures():
     v, f = gsoup.structures.cube()
-    gsoup.save_obj(v, f, "resource/cube.obj")
-    v1, f1 = gsoup.load_obj("resource/cube.obj")
+    gsoup.save_mesh(v, f, "resource/cube.obj")
+    v1, f1 = gsoup.load_mesh("resource/cube.obj")
     assert np.allclose(v, v1)
     assert np.allclose(f, f1)
     v, f = gsoup.structures.icosehedron()
     gsoup.save_mesh(v, f, "resource/ico.obj")
-    v1, f1 = gsoup.load_obj("resource/ico.obj")
+    gsoup.save_mesh(v, f, "resource/ico.ply")
+    gsoup.save_mesh(v, f, "resource/ico_vcolor.ply", vertex_colors=np.random.randint(0, 255, size=v.shape).astype(np.uint8))
+    gsoup.save_mesh(v, f, "resource/ico_fcolor.ply", face_colors=np.random.randint(0, 255, size=f.shape).astype(np.uint8))
+    gsoup.save_pointcloud(v, "resource/ico_pc.ply")
+    v1, f1 = gsoup.load_mesh("resource/ico.obj")
     assert np.allclose(v, v1)
     assert np.allclose(f, f1)
-    v, f = gsoup.load_obj("resource/cube.obj")
+    v, f = gsoup.load_mesh("resource/cube.obj")
     assert v.shape[0] == 8
     assert f.shape[0] == 12
 
 def test_image():
     checkboard = gsoup.generate_checkerboard(512, 512, 8)
     gsoup.save_image(checkboard, "resource/checkboard.png")
     checkboard_RGBA = np.tile(checkboard, (1, 1, 4))
@@ -196,53 +202,53 @@
     assert lollipop_cropped_square.shape == (1, 512, 512, 3)
     lollipop_srgb = gsoup.linear_to_srgb(lollipop)
     lollipop_linear = gsoup.srgb_to_linear(lollipop_srgb)
     assert np.allclose(lollipop, lollipop_linear)
     gsoup.generate_concentric_circles(256, 512, dst=Path("resource/circles.png"))
     gsoup.generate_stripe_pattern(256, 512, direction="both", dst=Path("resource/stripe.png"))
     gsoup.generate_dot_pattern(512, 256, dst=Path("resource/dots.png"))
-    gray1 = gsoup.generate_gray_gradient(256, 256, grayscale=True, dst=Path("resource/gg_vert.png"))
+    gray1 = gsoup.generate_gray_gradient(256, 256, grayscale=True)
     assert gray1.shape == (256, 256)
     assert len(np.unique(gray1)) == 10
     assert gray1.max() == 255
-    gray2 = gsoup.generate_gray_gradient(50, 800, vertical=False, dst=Path("resource/gg_horiz.png"))
+    gray2 = gsoup.generate_gray_gradient(50, 800, vertical=False)
     assert gray2.shape == (50, 800, 3)
     assert gray2.max() == 255
-    gray3 = gsoup.generate_gray_gradient(256, 256, bins=-65, dst=Path("resource/gg_bin_min.png"))
+    gray3 = gsoup.generate_gray_gradient(256, 256, bins=-65)
     assert gray3.max() == 0
-    gray4 = gsoup.generate_gray_gradient(256, 256, bins=300, dst=Path("resource/gg_bin_max.png"))
+    gray4 = gsoup.generate_gray_gradient(256, 256, bins=300)
     assert gray4.max() == 255
-    gray5 = gsoup.generate_gray_gradient(1080, 1920, bins=300, dst=Path("resource/gg_highres.png"))
+    gray5 = gsoup.generate_gray_gradient(1080, 1920, bins=300)
     assert gray5.shape == (1080, 1920, 3)
     assert gray5.max() == 255
     dst = Path("resource/voronoi.png")
     gsoup.generate_voronoi_diagram(512, 512, 1000, dst=dst)
     img = gsoup.load_image(dst)
     assert img.shape == (512, 512, 3)
     assert img.dtype == np.uint8
     img = gsoup.load_image(dst, as_grayscale=True)
     assert img.shape == (512, 512)
     assert img.dtype == np.uint8
-    img = gsoup.load_image(dst, to_float=True)
+    img = gsoup.load_image(dst, float=True)
     assert img.shape == (512, 512, 3)
     assert img.dtype == np.float32
     assert (img>=0.0).all()
     assert (img<=1.0).all()
     img = gsoup.load_image(dst, channels_last=False)
     assert img.shape == (3, 512, 512)
-    img = gsoup.load_image(dst, to_float=True, as_grayscale=True)
+    img = gsoup.load_image(dst, float=True, as_grayscale=True)
     assert img.shape == (512, 512)
     assert img.dtype == np.float32
     assert (img>=0.0).all()
     assert (img<=1.0).all()
     img = gsoup.load_image(dst, channels_last=False, as_grayscale=True)
     assert img.shape == (512, 512)
-    img = gsoup.load_images(dst)
+    img = gsoup.load_images([dst])
     assert img.shape == (1, 512, 512, 3)
-    img = gsoup.load_images(dst, as_grayscale=True)
+    img = gsoup.load_images([dst], as_grayscale=True)
     assert img.shape == (1, 512, 512)
     img = gsoup.load_images([dst])
     assert img.shape == (1, 512, 512, 3)
     img = gsoup.load_images([dst, dst, dst, dst])
     assert img.shape == (4, 512, 512, 3)
     resized_img = gsoup.resize_images_naive(img, 256, 256, mode="mean")
     assert resized_img.shape == (4, 256, 256, 3)
@@ -255,83 +261,128 @@
     assert grid.shape == (512, 512, 3)
     img = gsoup.load_images([dst, dst, dst, dst], as_grayscale=True)
     assert img.shape == (4, 512, 512)
     img = gsoup.load_images([dst, dst, dst, dst], as_grayscale=True, channels_last=False)
     assert img.shape == (4, 512, 512)
     img = gsoup.load_images([dst, dst, dst, dst], resize_wh=(128, 128))
     assert img.shape == (4, 128, 128, 3)
-    img, paths = gsoup.load_images([dst, dst, dst, dst], resize_wh=(128, 256), as_grayscale=True, channels_last=False, return_paths=True, to_float=True, to_torch=True)
+    img, paths = gsoup.load_images([dst, dst, dst, dst], resize_wh=(128, 256), as_grayscale=True, channels_last=False, return_paths=True, float=True, to_torch=True)
     assert len(paths) == 4
     assert img.dtype == torch.float32
     assert img.shape == (4, 256, 128)
 
 def test_video():
-    # import os
-    # FFMPEG_DIR = os.path.join("/usr/bin")
-    # os.environ['PATH'] = FFMPEG_DIR + ":" + os.environ['PATH']
+    import platform
+    import os
+    if platform.system() == "Windows":
+        FFMPEG_DIR = os.path.join("D:/tools/ffmpeg-5.1-essentials_build/bin")
+        os.environ['PATH'] = FFMPEG_DIR + ";" + os.environ['PATH']
+    else:
+        FFMPEG_DIR = os.path.join("/usr/bin")
+        os.environ['PATH'] = FFMPEG_DIR + ":" + os.environ['PATH']
     frame_number = 100
-    images = np.random.randint(0, 255, (frame_number, 512, 512, 3), dtype=np.uint8)
+    h = 128
+    w = 128
+    # images = np.random.randint(0, 255, (frame_number, 512, 512, 3), dtype=np.uint8)
+    images = np.array([gsoup.generate_concentric_circles(h, w, n=5) for i in range(100)])
     # im1 = gsoup.generate_voronoi_diagram(512, 512, 1000)
     # im2 = gsoup.generate_voronoi_diagram(512, 512, 1000)
     # im1s = np.tile(im1[None, ...], (10, 1, 1, 1))
     # im2s = np.tile(im2[None, ...], (10, 1, 1, 1))
     # images = np.vstack([im1s, im2s])
-    dst = Path("resource/noise.avi")
-    gsoup.save_video(images, dst, fps=10)
-    gsoup.save_video(images, Path("resource/noise_lossy.avi"), lossy=True, fps=10)
-    reader = gsoup.VideoReader(dst, h=512, w=512)
+    gsoup.save_video(images, Path("resource/lossless_video.avi"), lossy=False, fps=10)
+    gsoup.save_video(images, Path("resource/lossy_video.avi"), lossy=True, fps=10)
+    reader = gsoup.VideoReader(Path("resource/lossless_video.avi"), h=h, w=w)
     fps = gsoup.FPS()
     for i, frame in enumerate(reader):
         print("{}: {}, fps: {}".format(i, frame.shape, fps()))
         assert np.all(frame == images[i])
-    video_frames = gsoup.load_video(dst)
-    assert video_frames.shape == (frame_number, 512, 512, 3)
+    video_frames = gsoup.load_video(Path("resource/lossless_video.avi"))
+    assert video_frames.shape == (frame_number, h, w, 3)
     assert np.all(video_frames == images)
-    video_frames_reversed = gsoup.reverse_video(dst)
+    video_frames_reversed = gsoup.reverse_video(Path("resource/lossless_video.avi"))
     assert (video_frames_reversed[-1] == video_frames[0]).all()
-    sliced_frames = gsoup.slice_from_video(dst, every_n_frames=2, start_frame=0, end_frame=6)
+    sliced_frames = gsoup.slice_from_video(Path("resource/lossless_video.avi"), every_n_frames=2, start_frame=0, end_frame=6)
     assert (sliced_frames == video_frames[:7:2, :, :, :]).all()
-    gsoup.video_to_images(dst, Path("resource/noise"))
-    gsoup.save_video(Path("resource/noise"), Path("resource/noise2.avi"), fps=10)
-    gsoup.save_video(Path("resource/noise"), Path("resource/noise_lossy2.avi"), lossy=True, fps=10)
-    discrete_images = gsoup.load_images(Path("resource/noise"))
-    assert discrete_images.shape == (frame_number, 512, 512, 3)
-    timestamps = gsoup.get_frame_timestamps(dst)
+    gsoup.video_to_images(Path("resource/lossless_video.avi"), Path("resource/ffmpeg_reconstructed_images"))
+    gsoup.save_video(Path("resource/ffmpeg_reconstructed_images"), Path("resource/reconst_lossy.avi"), fps=10, lossy=True)
+    gsoup.save_video(Path("resource/ffmpeg_reconstructed_images"), Path("resource/reconst_lossless.avi"), fps=10, lossy=False)
+    discrete_images = gsoup.load_images(Path("resource/ffmpeg_reconstructed_images"))
+    assert discrete_images.shape == (frame_number, h, w, 3)
+    timestamps = gsoup.get_frame_timestamps(Path("resource/lossless_video.avi"))
     assert timestamps[0] == 0
 
 def test_procam():
     gray = gsoup.GrayCode()
     patterns = gray.encode((128, 128))
+    mode = "ij"
     forward_map, fg = gray.decode(patterns, (128, 128),
-                                  output_dir=Path("resource/pix2pix"), mode="ij", debug=True)
+                                  output_dir=Path("resource/pix2pix"), mode=mode, debug=True)
     backward_map = gsoup.compute_backward_map((128, 128), forward_map, fg,
                                               output_dir=Path("resource/pix2pix"), debug=True)
     desired = gsoup.generate_lollipop_pattern(128, 128)
-    # desired = gsoup.to_float(desired)
-    warp_image = gsoup.warp_image(backward_map, desired, cam_wh=(forward_map.shape[1], forward_map.shape[0]),
+    warp_image = gsoup.warp_image(backward_map, desired, cam_wh=(forward_map.shape[1], forward_map.shape[0]), mode=mode,
                                   output_path=Path("resource/warp.png"))
     assert warp_image.shape == (128, 128, 3)
     assert warp_image.dtype == np.uint8
-    assert np.mean(np.abs(desired - warp_image)) < 10  # surely an identity corrospondence & warp can't be too bad
-    calibration_dir = Path("resource/calibration")
-    calibration_dir.mkdir(exist_ok=True, parents=True)
-    checkerboard = gsoup.to_float(gsoup.generate_checkerboard(128, 128, 16))
+    assert np.mean(np.abs(desired - warp_image)) < 10  # identity correspondence & warp should be very similar
+    # calibration_dir = Path("resource/calibration")
+    # calibration_dir.mkdir(exist_ok=True, parents=True)
+    checkerboard = gsoup.generate_checkerboard(128, 128, 16)
     # T = gsoup.random_perspective()
     # T_opencv = T[:2, :]
     # img_transformed = cv2.warpPerspective(checkerboard, T, (128, 128))
-    captures = np.bitwise_and(patterns==255, checkerboard[None, ...]==1.0)
-    gsoup.save_images(captures, Path(calibration_dir, "0"))
-    gsoup.save_images(captures, Path(calibration_dir, "1"))
+    # captures = np.bitwise_and(patterns==255, checkerboard[None, ...]==1.0)
+    # gsoup.save_images(captures, Path(calibration_dir, "0"))
+    # gsoup.save_images(captures, Path(calibration_dir, "1"))
+    gsoup.save_image(checkerboard, Path("resource/checkerboard.png"))
+    #############
+    # patterns = gray.encode((800, 800))
+    patterns = gsoup.load_images(Path("tests/tests_resource/correspondence"))
+    cam_wh = (patterns[0].shape[1], patterns[0].shape[0])
+    proj_wh = (800, 800)
+    forward_map, fg = gray.decode(patterns, (800, 800), output_dir="resource/forward", debug=True, mode=mode)
+    backward_map = gsoup.compute_backward_map((800, 800), forward_map, fg, mode=mode, output_dir="resource/backward_not_interp", debug=True, interpolate=False)
+    backward_map = gsoup.compute_backward_map((800, 800), forward_map, fg, mode=mode, output_dir="resource/backward_interp", debug=True, interpolate=True)
+    desired = gsoup.generate_lollipop_pattern(800, 800)
+    warp_image = gsoup.warp_image(backward_map, desired, cam_wh=cam_wh, mode=mode,
+                                  output_path=Path("resource/debug/warp.png"))
+    blend_to_cv = np.array([[1.0, 0, 0, 0],
+                            [0, -1, 0, 0],
+                            [0, 0, -1, 0],
+                            [0, 0, 0, 1]])
+    cam_transform = np.array([[0, 0, 1, 1], [1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 0, 1.0]])
+    cam_transform = cam_transform @ blend_to_cv
+    ### gt ###
+    # cam_int = np.array([[800, 0, 400.0], [0.0, 800, 400], [0, 0, 1]])
+    # proj_int = np.array([[800, 0, 400.0], [0.0, 800, 400], [0, 0, 1]])
+    # proj_transform = np.array([[-0.12403473, -0.23891242,  0.96308672,  0.8 ],
+    #                             [ 0.99227786, -0.02986405,  0.12038584,  0.1],
+    #                             [ 0.        ,  0.97058171,  0.24077168,  0.2],
+    #                             [ 0.        ,  0.        ,  0.        ,  1. ]])
+    # proj_transform = proj_transform @ blend_to_cv
+    # cam_dist = None
+    ### end gt ###
+    ### calib ###
     cam_int, cam_dist,\
     proj_int, proj_dist,\
-    cam_proj_rmat, cam_proj_tvec = gsoup.calibrate_procam(128, 128, 1, calibration_dir, chess_vert=7, chess_hori=7)
+    proj_transform = gsoup.calibrate_procam((800, 800), Path("tests/tests_resource/calibration"),
+                                            chess_vert=9, chess_hori=9,
+                                            chess_block_size=0.032, output_dir="resource/calibration",
+                                            projector_orientation="none", debug=True)
+    proj_transform = cam_transform @ np.linalg.inv(proj_transform)  # c2w @ p2c = p2w
+    ### end calib ###
+    # calibration_static_view(cam_transform, proj_transform, (800, 800), (800, 800), cam_int, cam_dist, proj_int, forward_map, fg, mode)
+    pc = gsoup.reconstruct_pointcloud(forward_map, fg, cam_transform, proj_transform, cam_int, cam_dist, proj_int, mode=mode)
+    gsoup.save_pointcloud(pc, "resource/points.ply")
 
 def test_sphere_tracer():
     image_size = 512
-    device = "cuda:0"
+    # device = "cuda:0"
+    device = "cpu"
     w2v, v2c = gsoup.create_random_cameras_on_unit_sphere(5, 1.0, opengl=True, device=device)
     ray_origins, ray_directions = gsoup.generate_rays(w2v, v2c[0], image_size, image_size, device=device)
     sdf = gsoup.structures.sphere_sdf(0.25)
     images = []
     for o, d in zip(ray_origins, ray_directions):
         result = gsoup.render(sdf, o.view(-1, 3), d.view(-1, 3))
         images.append(result.view(image_size, image_size, 4))
```

