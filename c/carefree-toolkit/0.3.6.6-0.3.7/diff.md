# Comparing `tmp/carefree-toolkit-0.3.6.6.tar.gz` & `tmp/carefree-toolkit-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carefree-toolkit-0.3.6.6.tar", last modified: Tue Jun 27 15:22:14 2023, max compression
+gzip compressed data, was "carefree-toolkit-0.3.7.tar", last modified: Wed Jul 19 01:29:31 2023, max compression
```

## Comparing `carefree-toolkit-0.3.6.6.tar` & `carefree-toolkit-0.3.7.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 15:22:14.398146 carefree-toolkit-0.3.6.6/
--rw-rw-rw-   0        0        0     1090 2023-01-17 02:58:51.000000 carefree-toolkit-0.3.6.6/LICENSE
--rw-rw-rw-   0        0        0     9010 2023-06-27 15:22:14.397149 carefree-toolkit-0.3.6.6/PKG-INFO
--rw-rw-rw-   0        0        0     8579 2023-01-17 02:58:51.000000 carefree-toolkit-0.3.6.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 15:22:14.388178 carefree-toolkit-0.3.6.6/carefree_toolkit.egg-info/
--rw-rw-rw-   0        0        0     9010 2023-06-27 15:22:14.000000 carefree-toolkit-0.3.6.6/carefree_toolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      463 2023-06-27 15:22:14.000000 carefree-toolkit-0.3.6.6/carefree_toolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 15:22:14.000000 carefree-toolkit-0.3.6.6/carefree_toolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-06-27 15:22:14.000000 carefree-toolkit-0.3.6.6/carefree_toolkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-27 15:22:14.000000 carefree-toolkit-0.3.6.6/carefree_toolkit.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-27 15:22:14.395155 carefree-toolkit-0.3.6.6/cftool/
--rw-rw-rw-   0        0        0        0 2023-01-17 02:58:51.000000 carefree-toolkit-0.3.6.6/cftool/__init__.py
--rw-rw-rw-   0        0        0    22677 2023-03-28 02:09:10.000000 carefree-toolkit-0.3.6.6/cftool/array.py
--rw-rw-rw-   0        0        0       58 2023-05-17 12:47:47.000000 carefree-toolkit-0.3.6.6/cftool/constants.py
--rw-rw-rw-   0        0        0    10833 2023-06-27 13:19:40.000000 carefree-toolkit-0.3.6.6/cftool/cv.py
--rw-rw-rw-   0        0        0    17757 2023-06-27 12:49:06.000000 carefree-toolkit-0.3.6.6/cftool/data_structures.py
-drwxrwxrwx   0        0        0        0 2023-06-27 15:22:14.396189 carefree-toolkit-0.3.6.6/cftool/dist/
--rw-rw-rw-   0        0        0       28 2023-03-05 03:09:06.000000 carefree-toolkit-0.3.6.6/cftool/dist/__init__.py
--rw-rw-rw-   0        0        0    21842 2023-01-17 02:58:51.000000 carefree-toolkit-0.3.6.6/cftool/dist/core.py
--rw-rw-rw-   0        0        0     9983 2023-05-31 06:56:25.000000 carefree-toolkit-0.3.6.6/cftool/geometry.py
--rw-rw-rw-   0        0        0    25320 2023-01-17 02:58:51.000000 carefree-toolkit-0.3.6.6/cftool/manage.py
--rw-rw-rw-   0        0        0    85225 2023-06-17 13:29:03.000000 carefree-toolkit-0.3.6.6/cftool/misc.py
--rw-rw-rw-   0        0        0     6451 2023-03-21 11:08:09.000000 carefree-toolkit-0.3.6.6/cftool/pipeline.py
--rw-rw-rw-   0        0        0     1085 2023-06-27 13:01:32.000000 carefree-toolkit-0.3.6.6/cftool/types.py
--rw-rw-rw-   0        0        0     2237 2023-05-17 12:54:11.000000 carefree-toolkit-0.3.6.6/cftool/web.py
--rw-rw-rw-   0        0        0       42 2023-06-27 15:22:14.398146 carefree-toolkit-0.3.6.6/setup.cfg
--rw-rw-rw-   0        0        0      905 2023-06-27 15:21:39.000000 carefree-toolkit-0.3.6.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 01:29:31.559593 carefree-toolkit-0.3.7/
+-rw-rw-rw-   0        0        0     1090 2019-09-25 20:51:10.000000 carefree-toolkit-0.3.7/LICENSE
+-rw-rw-rw-   0        0        0     9006 2023-07-19 01:29:31.556598 carefree-toolkit-0.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0     8579 2022-06-27 01:36:51.000000 carefree-toolkit-0.3.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-19 01:29:31.498629 carefree-toolkit-0.3.7/carefree_toolkit.egg-info/
+-rw-rw-rw-   0        0        0     9006 2023-07-19 01:29:31.000000 carefree-toolkit-0.3.7/carefree_toolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      478 2023-07-19 01:29:31.000000 carefree-toolkit-0.3.7/carefree_toolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 01:29:31.000000 carefree-toolkit-0.3.7/carefree_toolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-07-19 01:29:31.000000 carefree-toolkit-0.3.7/carefree_toolkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-19 01:29:31.000000 carefree-toolkit-0.3.7/carefree_toolkit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-19 01:29:31.545982 carefree-toolkit-0.3.7/cftool/
+-rw-rw-rw-   0        0        0        0 2020-11-05 10:59:33.000000 carefree-toolkit-0.3.7/cftool/__init__.py
+-rw-rw-rw-   0        0        0    22677 2023-04-03 14:14:29.000000 carefree-toolkit-0.3.7/cftool/array.py
+-rw-rw-rw-   0        0        0       58 2023-05-18 01:18:59.000000 carefree-toolkit-0.3.7/cftool/constants.py
+-rw-rw-rw-   0        0        0    10836 2023-07-14 15:32:08.000000 carefree-toolkit-0.3.7/cftool/cv.py
+-rw-rw-rw-   0        0        0    17806 2023-06-30 01:15:17.000000 carefree-toolkit-0.3.7/cftool/data_structures.py
+drwxrwxrwx   0        0        0        0 2023-07-19 01:29:31.551967 carefree-toolkit-0.3.7/cftool/dist/
+-rw-rw-rw-   0        0        0       28 2023-04-03 14:14:29.000000 carefree-toolkit-0.3.7/cftool/dist/__init__.py
+-rw-rw-rw-   0        0        0    21842 2022-08-08 17:03:13.000000 carefree-toolkit-0.3.7/cftool/dist/core.py
+-rw-rw-rw-   0        0        0    12264 2023-07-16 15:56:00.000000 carefree-toolkit-0.3.7/cftool/geometry.py
+-rw-rw-rw-   0        0        0    25320 2022-08-08 17:03:13.000000 carefree-toolkit-0.3.7/cftool/manage.py
+-rw-rw-rw-   0        0        0    85225 2023-06-17 17:02:41.000000 carefree-toolkit-0.3.7/cftool/misc.py
+-rw-rw-rw-   0        0        0     6292 2023-07-16 15:56:36.000000 carefree-toolkit-0.3.7/cftool/noli.py
+-rw-rw-rw-   0        0        0     6451 2023-04-03 14:14:29.000000 carefree-toolkit-0.3.7/cftool/pipeline.py
+-rw-rw-rw-   0        0        0     1085 2023-06-30 01:15:17.000000 carefree-toolkit-0.3.7/cftool/types.py
+-rw-rw-rw-   0        0        0     2237 2023-05-18 01:18:59.000000 carefree-toolkit-0.3.7/cftool/web.py
+-rw-rw-rw-   0        0        0       42 2023-07-19 01:29:31.560592 carefree-toolkit-0.3.7/setup.cfg
+-rw-rw-rw-   0        0        0      903 2023-07-19 01:29:11.000000 carefree-toolkit-0.3.7/setup.py
```

### Comparing `carefree-toolkit-0.3.6.6/LICENSE` & `carefree-toolkit-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `carefree-toolkit-0.3.6.6/PKG-INFO` & `carefree-toolkit-0.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: carefree-toolkit
-Version: 0.3.6.6
+Version: 0.3.7
 Summary: Some commonly used functions and modules
 Home-page: https://github.com/carefree0910/carefree-toolkit
-Download-URL: https://github.com/carefree0910/carefree-toolkit/archive/v0.3.6.6.tar.gz
+Download-URL: https://github.com/carefree0910/carefree-toolkit/archive/v0.3.7.tar.gz
 Author: carefree0910
 Author-email: syameimaru.saki@gmail.com
 Keywords: python numpy data-science
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # carefree-toolkit
```

### Comparing `carefree-toolkit-0.3.6.6/README.md` & `carefree-toolkit-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `carefree-toolkit-0.3.6.6/carefree_toolkit.egg-info/PKG-INFO` & `carefree-toolkit-0.3.7/carefree_toolkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: carefree-toolkit
-Version: 0.3.6.6
+Version: 0.3.7
 Summary: Some commonly used functions and modules
 Home-page: https://github.com/carefree0910/carefree-toolkit
-Download-URL: https://github.com/carefree0910/carefree-toolkit/archive/v0.3.6.6.tar.gz
+Download-URL: https://github.com/carefree0910/carefree-toolkit/archive/v0.3.7.tar.gz
 Author: carefree0910
 Author-email: syameimaru.saki@gmail.com
 Keywords: python numpy data-science
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # carefree-toolkit
```

### Comparing `carefree-toolkit-0.3.6.6/cftool/array.py` & `carefree-toolkit-0.3.7/cftool/array.py`

 * *Files identical despite different names*

### Comparing `carefree-toolkit-0.3.6.6/cftool/cv.py` & `carefree-toolkit-0.3.7/cftool/cv.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,32 +98,33 @@
     *,
     anchor: Optional[int],
     to_gray: bool = False,
     to_mask: bool = False,
     resample: Any = Image.LANCZOS,
     normalize: bool = True,
     padding_mode: Optional[str] = None,
+    padding_mask: Optional[TImage] = None,
     padding_kwargs: Optional[Dict[str, Any]] = None,
     to_torch_fmt: bool = True,
 ) -> ReadImageResponse:
     if Image is None:
         raise ValueError("`pillow` is needed for `read_image`")
     if isinstance(image, str):
         image = Image.open(image)
     alpha = None
     original = image
     if image.mode == "RGBA":
-        alpha = image.split()[3]
+        alpha = padding_mask = image.split()[3]
     if not to_mask and not to_gray:
-        if alpha is None or padding_mode is None:
+        if padding_mask is None or padding_mode is None:
             image = to_rgb(image)
         else:
             padding = Padding.make(padding_mode, {})
             padding_kw = shallow_copy_dict(padding_kwargs or {})
-            padding_kw.update(dict(image=image, alpha=alpha))
+            padding_kw.update(dict(image=image, alpha=padding_mask))
             image = safe_execute(padding.pad, padding_kw)
     else:
         if to_mask and to_gray:
             raise ValueError("`to_mask` & `to_gray` should not be True simultaneously")
         if to_mask and image.mode == "RGBA":
             image = alpha
         else:
@@ -318,16 +319,15 @@
         *,
         radius: int = 5,
         **kwargs: Any,
     ) -> Image.Image:
         if cv2 is None:
             raise ValueError("`cv2` is needed for `CV2NS`")
         img_arr = np.array(image.convert("RGB"))[..., ::-1]
-        mask_arr = np.array(alpha)
-        rs = cv2.inpaint(img_arr, 255 - mask_arr, radius, cv2.INPAINT_NS)
+        rs = cv2.inpaint(img_arr, np.array(alpha), radius, cv2.INPAINT_NS)
         return Image.fromarray(rs[..., ::-1])
 
 
 @Padding.register("cv2_telea")
 class CV2Telea(Padding):
     def pad(
         self,
@@ -336,10 +336,9 @@
         *,
         radius: int = 5,
         **kwargs: Any,
     ) -> Image.Image:
         if cv2 is None:
             raise ValueError("`cv2` is needed for `CV2Telea`")
         img_arr = np.array(image.convert("RGB"))[..., ::-1]
-        mask_arr = np.array(alpha)
-        rs = cv2.inpaint(img_arr, 255 - mask_arr, radius, cv2.INPAINT_TELEA)
+        rs = cv2.inpaint(img_arr, np.array(alpha), radius, cv2.INPAINT_TELEA)
         return Image.fromarray(rs[..., ::-1])
```

### Comparing `carefree-toolkit-0.3.6.6/cftool/data_structures.py` & `carefree-toolkit-0.3.7/cftool/data_structures.py`

 * *Files 1% similar despite different names*

```diff
@@ -342,14 +342,17 @@
         ),
     )
     data: Dict[str, Any] = Field(..., description="Algorithm's data")
 
     def to_item(self) -> Item["WorkNode"]:
         return Item(self.key, self)
 
+    class Config:
+        smart_union = True
+
 
 class ToposortResult(NamedTuple):
     in_edges: Dict[str, Set[str]]
     hierarchy: List[List[Item[WorkNode]]]
     edge_labels: Dict[Tuple[str, str], str]
```

### Comparing `carefree-toolkit-0.3.6.6/cftool/dist/core.py` & `carefree-toolkit-0.3.7/cftool/dist/core.py`

 * *Files identical despite different names*

### Comparing `carefree-toolkit-0.3.6.6/cftool/geometry.py` & `carefree-toolkit-0.3.7/cftool/geometry.py`

 * *Files 20% similar despite different names*

```diff
@@ -270,14 +270,72 @@
 
     # top -> right -> bottom -> left
     @property
     def edges(self) -> List[Line]:
         corners = self.corner_points
         return [Line(corner, corners[(i + 1) % 4]) for i, corner in enumerate(corners)]
 
+    @property
+    def css_property(self) -> str:
+        return f"matrix({self.a},{self.b},{self.c},{self.d},{self.e},{self.f})"
+
+    def scale(
+        self,
+        scale: float,
+        scale_y: Optional[float] = None,
+        center: Optional[Point] = None,
+    ) -> "Matrix2D":
+        if scale_y is None:
+            scale_y = scale
+        if center is None:
+            return Matrix2D(
+                a=self.a * scale,
+                b=self.b * scale,
+                c=self.c * scale_y,
+                d=self.d * scale_y,
+                e=self.e,
+                f=self.f,
+            )
+        return Matrix2D.scale_matrix(scale, scale_y, center=center) @ self
+
+    def scale_to(
+        self,
+        scale: float,
+        scale_y: Optional[float] = None,
+        center: Optional[Point] = None,
+    ) -> "Matrix2D":
+        if scale_y is None:
+            scale_y = scale
+        w, h = self.wh
+        return self.scale(scale / w, scale_y / h, center=center)
+
+    def flip(
+        self,
+        flip_x: bool,
+        flip_y: bool,
+        center: Optional[Point] = None,
+    ) -> "Matrix2D":
+        return Matrix2D.flip_matrix(flip_x, flip_y, center) @ self
+
+    def rotate(self, theta: float, center: Optional[Point] = None) -> "Matrix2D":
+        if math.isclose(theta, 0.0):
+            return self.copy()
+        return Matrix2D.rotation_matrix(theta, center) @ self
+
+    def rotate_to(self, theta: float, center: Optional[Point] = None) -> "Matrix2D":
+        return self.rotate(theta - self.theta, center)
+
+    def move(self, point: Point) -> "Matrix2D":
+        a, b, c, d, e, f = self.tuple
+        return Matrix2D(a, b, c, d, point.x + e, point.y + f)
+
+    def move_to(self, point: Point) -> "Matrix2D":
+        a, b, c, d, _, _ = self.tuple
+        return Matrix2D(a, b, c, d, point.x, point.y)
+
     def decompose(self) -> Matrix2DProperties:
         w, h = self.wh
         a, b, c, d, e, f = self.tuple
         return Matrix2DProperties(
             x=e,
             y=f,
             w=w,
@@ -328,14 +386,29 @@
         )
 
     @classmethod
     def move_matrix(cls, x: float, y: float) -> "Matrix2D":
         return cls(a=1, b=0, c=0, d=1, e=x, f=y)
 
     @classmethod
+    def flip_matrix(
+        self,
+        flip_x: bool,
+        flip_y: bool,
+        center: Optional[Point] = None,
+    ) -> "Matrix2D":
+        fx = -1 if flip_x else 1
+        fy = -1 if flip_y else 1
+        return Matrix2D.scale_matrix(fx, fy, center)
+
+    @classmethod
+    def identical(cls) -> "Matrix2D":
+        return cls(a=1, b=0, c=0, d=1, e=0, f=0)
+
+    @classmethod
     def from_properties(cls, properties: Matrix2DProperties) -> "Matrix2D":
         return (
             cls.move_matrix(properties.x, properties.y)
             @ cls.rotation_matrix(properties.theta)
             @ cls.scale_matrix(properties.w, properties.h)
             @ cls.skew_matrix(properties.skew_x, properties.skew_y)
         )
```

### Comparing `carefree-toolkit-0.3.6.6/cftool/manage.py` & `carefree-toolkit-0.3.7/cftool/manage.py`

 * *Files identical despite different names*

### Comparing `carefree-toolkit-0.3.6.6/cftool/misc.py` & `carefree-toolkit-0.3.7/cftool/misc.py`

 * *Files identical despite different names*

### Comparing `carefree-toolkit-0.3.6.6/cftool/pipeline.py` & `carefree-toolkit-0.3.7/cftool/pipeline.py`

 * *Files identical despite different names*

### Comparing `carefree-toolkit-0.3.6.6/cftool/types.py` & `carefree-toolkit-0.3.7/cftool/types.py`

 * *Files identical despite different names*

### Comparing `carefree-toolkit-0.3.6.6/cftool/web.py` & `carefree-toolkit-0.3.7/cftool/web.py`

 * *Files identical despite different names*

### Comparing `carefree-toolkit-0.3.6.6/setup.py` & `carefree-toolkit-0.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 from setuptools import find_packages
 
 
-VERSION = "0.3.6.6"
+VERSION = "0.3.7"
 
 DESCRIPTION = "Some commonly used functions and modules"
 with open("README.md") as f:
     LONG_DESCRIPTION = f.read()
 
 INSTALL_REQUIRES = [
     "dill",
```

