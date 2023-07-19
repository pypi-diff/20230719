# Comparing `tmp/qubolite-0.8.1.tar.gz` & `tmp/qubolite-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qubolite-0.8.1.tar", last modified: Fri Jul 14 09:33:44 2023, max compression
+gzip compressed data, was "qubolite-0.8.2.tar", last modified: Wed Jul 19 14:25:06 2023, max compression
```

## Comparing `qubolite-0.8.1.tar` & `qubolite-0.8.2.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 smuecke   (1000) smuecke   (1000)        0 2023-07-14 09:33:44.595992 qubolite-0.8.1/
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)     5369 2023-07-14 09:33:44.595992 qubolite-0.8.1/PKG-INFO
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)     4795 2023-07-14 09:31:22.000000 qubolite-0.8.1/README.md
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)      907 2023-07-14 09:30:45.000000 qubolite-0.8.1/pyproject.toml
-drwxr-xr-x   0 smuecke   (1000) smuecke   (1000)        0 2023-07-14 09:33:44.595992 qubolite-0.8.1/qubolite/
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)      205 2023-07-12 14:20:19.000000 qubolite-0.8.1/qubolite/__init__.py
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)     5873 2023-07-12 14:20:19.000000 qubolite-0.8.1/qubolite/_c_utils.c
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)    10472 2023-07-12 14:20:19.000000 qubolite-0.8.1/qubolite/_heuristics.py
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)     2487 2023-07-12 14:20:19.000000 qubolite-0.8.1/qubolite/_misc.py
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)     6139 2023-07-14 08:43:25.000000 qubolite-0.8.1/qubolite/bitvec.py
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)     4689 2023-07-14 08:43:25.000000 qubolite-0.8.1/qubolite/bounds.py
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)     9413 2023-07-12 14:20:19.000000 qubolite-0.8.1/qubolite/compression.py
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)     8161 2023-07-14 08:43:25.000000 qubolite-0.8.1/qubolite/embedding.py
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)    22037 2023-07-14 09:14:59.000000 qubolite-0.8.1/qubolite/qubo.py
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)    11257 2023-07-12 14:20:19.000000 qubolite-0.8.1/qubolite/sampling.py
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)     6590 2023-07-14 08:43:25.000000 qubolite-0.8.1/qubolite/solving.py
-drwxr-xr-x   0 smuecke   (1000) smuecke   (1000)        0 2023-07-14 09:33:44.595992 qubolite-0.8.1/qubolite.egg-info/
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)     5369 2023-07-14 09:33:44.000000 qubolite-0.8.1/qubolite.egg-info/PKG-INFO
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)      417 2023-07-14 09:33:44.000000 qubolite-0.8.1/qubolite.egg-info/SOURCES.txt
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)        1 2023-07-14 09:33:44.000000 qubolite-0.8.1/qubolite.egg-info/dependency_links.txt
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)      185 2023-07-14 09:33:44.000000 qubolite-0.8.1/qubolite.egg-info/requires.txt
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)       18 2023-07-14 09:33:44.000000 qubolite-0.8.1/qubolite.egg-info/top_level.txt
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)       38 2023-07-14 09:33:44.595992 qubolite-0.8.1/setup.cfg
--rwxr-xr-x   0 smuecke   (1000) smuecke   (1000)      836 2023-07-12 13:34:37.000000 qubolite-0.8.1/setup.py
+drwxr-xr-x   0 smuecke   (1000) smuecke   (1000)        0 2023-07-19 14:25:06.158911 qubolite-0.8.2/
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)     1070 2023-07-19 14:19:32.000000 qubolite-0.8.2/LICENSE
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)     7948 2023-07-19 14:25:06.158911 qubolite-0.8.2/PKG-INFO
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)     5944 2023-07-19 14:20:09.000000 qubolite-0.8.2/README.md
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)     1215 2023-07-19 14:20:09.000000 qubolite-0.8.2/pyproject.toml
+drwxr-xr-x   0 smuecke   (1000) smuecke   (1000)        0 2023-07-19 14:25:06.158911 qubolite-0.8.2/qubolite/
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)      167 2023-07-19 14:20:09.000000 qubolite-0.8.2/qubolite/__init__.py
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)     5873 2023-07-12 14:20:19.000000 qubolite-0.8.2/qubolite/_c_utils.c
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)    10472 2023-07-12 14:20:19.000000 qubolite-0.8.2/qubolite/_heuristics.py
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)     1828 2023-07-19 14:20:09.000000 qubolite-0.8.2/qubolite/_misc.py
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)     8264 2023-07-19 14:20:09.000000 qubolite-0.8.2/qubolite/bitvec.py
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)     4689 2023-07-14 08:43:25.000000 qubolite-0.8.2/qubolite/bounds.py
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)     9413 2023-07-12 14:20:19.000000 qubolite-0.8.2/qubolite/compression.py
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)     8314 2023-07-19 14:20:09.000000 qubolite-0.8.2/qubolite/embedding.py
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)    26507 2023-07-19 14:20:09.000000 qubolite-0.8.2/qubolite/qubo.py
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)    11256 2023-07-19 14:20:09.000000 qubolite-0.8.2/qubolite/sampling.py
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)    11376 2023-07-19 14:21:47.000000 qubolite-0.8.2/qubolite/solving.py
+drwxr-xr-x   0 smuecke   (1000) smuecke   (1000)        0 2023-07-19 14:25:06.158911 qubolite-0.8.2/qubolite.egg-info/
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)     7948 2023-07-19 14:25:06.000000 qubolite-0.8.2/qubolite.egg-info/PKG-INFO
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)      425 2023-07-19 14:25:06.000000 qubolite-0.8.2/qubolite.egg-info/SOURCES.txt
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)        1 2023-07-19 14:25:06.000000 qubolite-0.8.2/qubolite.egg-info/dependency_links.txt
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)      185 2023-07-19 14:25:06.000000 qubolite-0.8.2/qubolite.egg-info/requires.txt
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)       18 2023-07-19 14:25:06.000000 qubolite-0.8.2/qubolite.egg-info/top_level.txt
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)       38 2023-07-19 14:25:06.158911 qubolite-0.8.2/setup.cfg
+-rwxr-xr-x   0 smuecke   (1000) smuecke   (1000)      836 2023-07-12 13:34:37.000000 qubolite-0.8.2/setup.py
```

### Comparing `qubolite-0.8.1/PKG-INFO` & `qubolite-0.8.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: qubolite
-Version: 0.8.1
-Summary: Toolbox for quadratic binary optimization
-Author-email: Sascha Mücke <sascha.muecke@tu-dortmund.de>, Thore Gerlach <thore.gerlach@iais.fraunhofer.de>
-Project-URL: Homepage, https://github.com/smuecke/qubolite
-Project-URL: Documentation, https://smuecke.github.io/qubolite
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: roof_dual
-Provides-Extra: kendall_tau
-Provides-Extra: embedding
-Provides-Extra: compression
-Provides-Extra: all
-
 # qubolite
 
 A light-weight toolbox for working with QUBO instances in NumPy.
 
 
 <img src="qubolite.png"  width="100" height="100">
 
@@ -115,7 +99,30 @@
     * **0.6.7** moved `brute_force` to new sub-module `solving`; added some approximate solving methods
     * **0.6.8** added `bitvec` sub-module; `dynamic_range` now uses bits by default, changed `bits=False` to `decibel=False`; removed scipy from requirements
     * **0.6.9** new, more memory-efficient save format
     * **0.6.10** fixed requirements in `setup.py`; fixed size estimation in `qubo.save()`
 * **0.7** Added more efficient brute-force implementation using C extension; added optional dependencies for calculating bounds and ordering distance
 * **0.8** New embeddings, new solving methods; switched to NumPy random generators from `RandomState`; added parameter compression for dynamic range reduction; Added documentation
     * **0.8.1** some fixes to documentation
+    * **0.8.2** implemented `qubo.dx2()`; added several new solving heuristics
+
+## License
+
+Copyright (c) 2023 Sascha Mücke
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `qubolite-0.8.1/pyproject.toml` & `qubolite-0.8.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -3,24 +3,30 @@
     "setuptools>=61.0",
     "numpy>=1.23.5"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qubolite"
-version = "0.8.1"
+version = "0.8.2"
 authors = [
     { name = "Sascha Mücke", email="sascha.muecke@tu-dortmund.de" },
     { name = "Thore Gerlach", email="thore.gerlach@iais.fraunhofer.de" }
 ]
 description = "Toolbox for quadratic binary optimization"
+license = {file = "LICENSE"}
 readme = "README.md"
+#repository = "https://github.com/smuecke/qubolite"
+#documentation = "https://smuecke.github.io/qubolite/api.html"
+keywords = ["qubo", "optimization", "quantum", "annealing"]
 requires-python = ">=3.8"
 classifiers = [
-    "Programming Language :: Python :: 3"
+    "Programming Language :: Python :: 3",
+    "Topic :: Scientific/Engineering :: Mathematics",
+    "Topic :: Scientific/Engineering :: Physics"
 ]
 dependencies = [
     "numpy>=1.23.5"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/smuecke/qubolite"
```

### Comparing `qubolite-0.8.1/qubolite/_c_utils.c` & `qubolite-0.8.2/qubolite/_c_utils.c`

 * *Files identical despite different names*

### Comparing `qubolite-0.8.1/qubolite/_heuristics.py` & `qubolite-0.8.2/qubolite/_heuristics.py`

 * *Files identical despite different names*

### Comparing `qubolite-0.8.1/qubolite/bitvec.py` & `qubolite-0.8.2/qubolite/bitvec.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import re
 
 import numpy as np
 from numpy.typing import ArrayLike
 
+from ._misc import get_random_state
+
 
 def all_bitvectors(n: int):
     """Generate all bit vectors of size ``n`` in lexicographical order, starting from all zeros.
     The least significant bit is at index 0. Note that always the same array object is yielded,
     so to persist the bit vectors you need to make copies.
 
     Args:
@@ -47,14 +49,38 @@
 
     Returns:
         numpy.ndarray: Array of shape ``(2**n, n)``
     """
     return np.arange(1<<n)[:, np.newaxis] & (1<<np.arange(n)) > 0
 
 
+def random(n: int, size=None, random_state=None):
+    """Create an array containing random bit vectors.
+
+    Args:
+        n (int): Number of bits per bit vector.
+        size (int | tuple, optional): Number of bit vectors to sample, or tuple
+            representing a shape. Defaults to None, which returns a single bit
+            vector (shape ``(n,)``).
+        random_state (optional): A numerical or lexical seed, or a NumPy random
+            generator. Defaults to None.
+
+    Returns:
+        numpy.ndarray: Random bit vector(s).
+    """
+    size = () if size is None else size
+    try:
+        shape = (*size, n)
+    except TypeError:
+        # `size` must be an integer
+        shape = (size, n)
+    rng = get_random_state(random_state)
+    return (rng.random(shape) < 0.5).astype(np.float64)
+
+
 def from_string(string: str):
     """Convert a string consisting of ``0`` and ``1`` to a bit vector.
 
     Args:
         string (str): Binary string.
 
     Returns:
@@ -196,7 +222,46 @@
         else:
             ix = int(token.strip('[!]'))
             if token[1] == '!': # inverse reference
                 x[:,i] = 1-x[:,ix]
             else:
                 x[:,i] = x[:,ix]
     return x
+
+
+# Manipulate Bit Vectors
+# ======================
+
+def flip_index(x, index, in_place=False):
+    """Flips the values of a given bit vector at the specified index or indices.
+
+    Args:
+        x (numpy.ndarray): Bit vector(s).
+        index (int | list | numpy.ndarray): Index or list of indices where to
+            flip the binary values.
+        in_place (bool, optional): If ``True``, modify the bit vector in place.
+            The return value will be a reference to the input array. Defaults to
+            False.
+
+    Returns:
+        numpy.ndarray: Bit vector(s) with the indices flipped at the specified
+            positions. If ``in_place=True``, this will be a reference to the
+            input array, otherwise a copy.
+
+    Examples:
+        The following inverts the first and last bits of all given bitvectors:
+
+        >>> x = from_expression('**10')
+        >>> x
+        array([[0., 0., 1., 0.],
+               [1., 0., 1., 0.],
+               [0., 1., 1., 0.],
+               [1., 1., 1., 0.]])
+        >>> flip_index(x, [0, -1])
+        array([[1., 0., 1., 1.],
+               [0., 0., 1., 1.],
+               [1., 1., 1., 1.],
+               [0., 1., 1., 1.]])
+    """
+    x_ = x if in_place else x.copy()
+    x_[..., index] = 1-x_[..., index]
+    return x_
```

### Comparing `qubolite-0.8.1/qubolite/bounds.py` & `qubolite-0.8.2/qubolite/bounds.py`

 * *Files identical despite different names*

### Comparing `qubolite-0.8.1/qubolite/compression.py` & `qubolite-0.8.2/qubolite/compression.py`

 * *Files identical despite different names*

### Comparing `qubolite-0.8.1/qubolite/embedding.py` & `qubolite-0.8.2/qubolite/embedding.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,15 +133,16 @@
     Args:
         values (numpy.ndarray | list): Values of which to find a subset.
             The resulting QUBO instance will have size ``len(values)``.
         target (int | float): Target value which the subset must add up to.
     """
     def __init__(self, values, target):
         self.__values = np.asarray(values)
-        self.__Q = self.__from_data(self.__values, target)
+        self.__target = target
+        self.__Q = self.__from_data(values, target)
 
     @property
     def qubo(self):
         return self.__Q
 
     @property
     def data(self):
@@ -155,18 +156,21 @@
         q = np.triu(q + np.tril(q, -1).T)
         return qubo(q)
 
     def map_solution(self, x):
         return self.__values[x.astype(bool)]
 
     @classmethod
-    def random(cls, n: int, low=0, high=10, summands=None, random_state=None):
+    def random(cls, n: int, low=-100, high=100,
+               summands=None, random_state=None):
         npr = get_random_state(random_state)
-        values = npr.uniform(low, high, size=n)
-        k = np.arange(2, n + 1) if summands is None else summands
+        values = np.zeros(n)
+        while np.any(np.isclose(values, 0)):
+            values = npr.uniform(low, high, size=n).round(2)
+        k = round(npr.triangular(0.1*n, 0.5*n, 0.9*n)) if summands is None else summands
         subset = npr.permutation(n) < k
         target = values[subset].sum()
         return cls(values, target)
 
 
 class Max2Sat(qubo_embedding):
     """Maximum Satisfyability problem with clauses of size 2.
```

### Comparing `qubolite-0.8.1/qubolite/qubo.py` & `qubolite-0.8.2/qubolite/qubo.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import struct
-from functools import reduce
 
 import numpy as np
+from numpy import newaxis as na
 
 from .bitvec  import all_bitvectors, all_bitvectors_array
-from ._misc    import get_random_state, is_triu, warn_size
+from ._misc   import get_random_state, is_triu, warn_size
 from _c_utils import brute_force as _brute_force_c
 
 def is_qubo_like(arr):
-    """Check if given array defines a QUBO instance, i.e.,
-    if the array is 2-dimensional and square.
+    """Check if given array defines a QUBO instance, i.e., if the array is
+    2-dimensional and square.
 
     Args:
         arr (numpy.ndarray): Input array.
 
     Returns:
         bool: ``True`` iff the input array defines a QUBO instance.
     """
@@ -21,16 +21,16 @@
         u, v = arr.shape[-2:]
         return u == v
     else:
         return False
 
 
 def to_triu_form(arr):
-    """Convert an array defining a QUBO instance to an
-    upper triangle matrix, if necessary.
+    """Convert an array defining a QUBO instance to an upper triangle matrix, if
+    necessary.
 
     Args:
         arr (numpy.ndarray): Input array.
 
     Returns:
         numpy.ndarray: Upper triangular matrix.
     """
@@ -48,27 +48,27 @@
         v = obj
     return v
 
 
 class qubo:
     """
     Standard class for QUBO instances.
-    This is mainly a wrapper around an upper triangular NumPy matrix with
-    lots of helpful methods. The passed array must be of the shape ``(n, n)``
-    for any positive ``n``. The linear coefficients lie along the diagonal.
-    A non-triangular matrix will be converted, i.e., the lower triangle will
-    be transposed and added to the upper triangle.
+    This is mainly a wrapper around an upper triangular NumPy matrix with lots
+    of helpful methods. The passed array must be of the shape ``(n, n)`` for any
+    positive ``n``. The linear coefficients lie along the diagonal. A
+    non-triangular matrix will be converted, i.e., the lower triangle will be
+    transposed and added to the upper triangle.
 
     Args:
         m (np.ndarray): Array containing the QUBO parameters.
 
     Examples:
-        If you have linear and quadratic coefficients in separate arrays,
-        e.g., ``lin`` with shape ``(n,)`` and ``qua`` with shape ``(n, n)``,
-        they can be combined to a ``qubo`` instance through ``qubo(np.diag(lin) + qua)``.
+        If you have linear and quadratic coefficients in separate arrays, e.g.,
+        ``lin`` with shape ``(n,)`` and ``qua`` with shape ``(n, n)``, they can
+        be combined to a ``qubo`` instance through ``qubo(np.diag(lin) + qua)``.
     """
 
     def __init__(self, m: np.ndarray):
         """
         Creates a ``qubo`` instance from a given NumPy array.
         
         """
@@ -79,18 +79,19 @@
     def __repr__(self):
         return 'qubo'+self.m.__repr__().lstrip('array')
 
     def __call__(self, x: np.ndarray):
         """Calculate the QUBO energy value for a given bit vector.
 
         Args:
-            x (numpy.ndarray): Bit vector of shape ``(n,)``, or multiple bit vectors ``(m, n)``.
+            x (numpy.ndarray): Bit vector of shape ``(n,)``, or multiple bit
+                vectors ``(m, n)``.
 
         Returns:
-            float or numpy.ndarray: QUBO energy value, or array ``(m,)`` of energy values.
+            float or numpy.ndarray of shape ``(m,)`` containing energy values.
         """
         return np.sum(np.dot(x, self.m)*x, axis=-1)
 
     def __getitem__(self, k):
         try:
             i, j = sorted(k)
             return self.m.__getitem__((i, j))
@@ -114,27 +115,34 @@
 
         Returns:
             qubo: Copy of this QUBO instance.
         """
         return qubo(self.m.copy())
 
     @classmethod
-    def random(cls, n: int, distr='normal', density=1.0, random_state=None, **kwargs):
-        """Create a QUBO instance with parameters sampled from a random distribution.
+    def random(cls, n: int,
+               distr='normal',
+               density=1.0,
+               random_state=None,
+               **kwargs):
+        """Create a QUBO instance with parameters sampled from a random
+        distribution.
 
         Args:
             n (int): QUBO size
-            distr (str, optional): Distribution from which the parameters are sampled.
-                Possible values are 'normal', 'uniform' and 'triangular'.
-                Additional keyword arguments will be passed to the corresponding
-                methods from ``numpy.random``. Defaults to 'normal'.
+            distr (str, optional): Distribution from which the parameters are
+                sampled. Possible values are ``'normal'``, ``'uniform'`` and
+                ``'triangular'``. Additional keyword arguments will be passed to
+                the corresponding methods from ``numpy.random``. Defaults to
+                ``'normal'``.
             density (float, optional): Expected density of the parameter matrix.
                 Each parameter is set to 0 with probability ``1-density``.
                 Defaults to 1.0.
-            random_state (optional): A numerical or lexical seed, or a NumPy random generator. Defaults to None.
+            random_state (optional): A numerical or lexical seed, or a NumPy
+                random generator. Defaults to None.
 
         Raises:
             ValueError: Raised if the ``distr`` argument is unknown.
 
         Returns:
             qubo: Random QUBO instance
         """
@@ -164,15 +172,16 @@
 
     def save(self, path: str, atol=1e-16):
         """Save the QUBO instance to disk.
         If the file exists, it will be overwritten.
         
         Args:
             path (str): Target file path.
-            atol (float, optional): Parameters with absolute value below this value will be treated as 0. Defaults to 1e-16.
+            atol (float, optional): Parameters with absolute value below this
+                value will be treated as 0. Defaults to 1e-16.
         """
         f = open(path, 'wb')
         f.write(struct.pack('<4s', b'QUBO')) # magic string
         f.write(struct.pack('<I', self.n)) # QUBO size
         # determine mode
         #  0x00: save flattened parameter array
         #  0x01: save index-value pairs
@@ -227,20 +236,20 @@
 
     def to_dict(self, names=None, double_indices=True, atol=1e-16):
         """Create a dictionary mapping variable indices to QUBO parameters.
         Contains entries only for non-zero parameters.
         
         Args:
             names (dict, optional): Dictionary mapping variables indices
-                (counting from 0) to names. By default, just the integer
-                indices are used.
-            double_indices (bool, optional): If ``True``, use ``(i, i)`` as
-                the key for diagonal entries, otherwise ``(i,)``. Defaults to True.
-            atol (float, optional): Parameters with absolute value below
-                this value will be treated as 0. Defaults to 1e-16.
+                (counting from 0) to names. By default, just the integer indices
+                are used.
+            double_indices (bool, optional): If ``True``, use ``(i, i)`` as the
+                key for diagonal entries, otherwise ``(i,)``. Defaults to True.
+            atol (float, optional): Parameters with absolute value below this
+                value will be treated as 0. Defaults to 1e-16.
             
         Returns:
             dict: Dictionary containing QUBO parameters.
 
         Examples:
             >>> Q = qubo.random(4, density=0.25).round(1)
             >>> Q
@@ -260,36 +269,37 @@
                     qubo_dict[(names[i],)] = self.m[i, i]
                 else:
                     qubo_dict[(names[i], names[j])] = self.m[i, j]
         return qubo_dict
 
     @classmethod
     def from_dict(cls, qubo_dict, n=None, relabel=True):
-        """Create QUBO instance from a dictionary mapping variable indices
-        to QUBO parameters. Note that, by default, unused variables are eliminated,
-        e.g., the dictionary ``{(0,): 2, (100,): -3}`` yields a QUBO instance
-        of size n=2. If you want to use the dictionary keys as variable indices
+        """Create QUBO instance from a dictionary mapping variable indices to
+        QUBO parameters. Note that, by default, unused variables are eliminated,
+        e.g., the dictionary ``{(0,): 2, (100,): -3}`` yields a QUBO instance of
+        size n=2. If you want to use the dictionary keys as variable indices
         as-is, set ``relabel=False``.
 
         Args:
             qubo_dict (dict): Dictionary mapping indices to QUBO parameters.
             n (int, optional): Specifies QUBO size. If None, the size is derived
                 from the number of variable names.
-            relabel (bool, optional): Indicate whether the variables should
-                be used as indices as-is, instead of removing unused variables.
+            relabel (bool, optional): Indicate whether the variables should be
+                used as indices as-is, instead of removing unused variables.
                 This works only for integer keys.
 
         Returns:
             qubo: QUBO instance with parameters taken from dictionary.
-            dict: Dictionary mapping the names of the variables used in
-                the input dictionary to the indices of the QUBO instance.
-                If ``relabel=False``, this dictionary will be an identity map.
+            dict: Dictionary mapping the names of the variables used in the
+                input dictionary to the indices of the QUBO instance. If
+                ``relabel=False``, this dictionary will be an identity map.
         """
         if relabel:
-            names = { k: i for i, k in enumerate(sorted(set().union(*qubo_dict.keys()))) }
+            key_set = set().union(*qubo_dict.keys())
+            names = { k: i for i, k in enumerate(sorted(key_set)) }
         else:
             names = { i: i for i in set().union(*qubo_dict.keys()) }
 
         n = max(names.values())+1 if n is None else n
         m = np.zeros((n, n))
         for k, v in qubo_dict.items():
             try:
@@ -300,36 +310,94 @@
                     i, = k
                     m[names[i], names[i]] += v
                 except ValueError:
                     pass
         m = np.triu(m + np.tril(m, -1).T)
         return cls(m), { i: k for k, i in names.items() }
 
+    def to_ising(self, offset=0.0):
+        """Convert this QUBO instance to an Ising model with variables
+        :math:`\\boldsymbol s\\in\\lbrace -1,+1\\rbrace` instead of
+        :math:`\\boldsymbol x\\in\\lbrace 0,1\\rbrace`.
+
+        Args:
+            offset (float, optional): Constant offset value added to the energy.
+                Defaults to 0.0.
+
+        Returns:
+            Tuple containing
+
+            - linear coefficients (*external field*) with shape ``(n,)``
+            - quadratic coefficients (*interactions*) with shape ``(n, n)``
+            - new offset (float)
+        """
+        m_ = self.m + self.m.T
+        lin = 0.25*m_.sum(0)
+        qua = 0.25*np.triu(self.m, 1)
+        c = 0.25*(self.m.sum()+np.diag(self.m).sum())+offset
+        return lin, qua, c
+
     @classmethod
     def from_ising(cls, linear, quadratic, offset=0.0):
+        """Create QUBO instance from Ising model parameters. In an Ising model,
+        the binary variables :math:`\\boldsymbol x\\in\\lbrace 0,1,\\rbrace` are
+        replaced with *bipolar* variables
+        :math:`\\boldsymbol s\\in\\lbrace -1,+1\\rbrace`. The two models are
+        computationally equivalent and can be converted into each other by
+        variable substitution :math:`\\boldsymbol s\\mapsto 2\\boldsymbol x+1`.
+
+        Args:
+            linear (list | numpy.ndarray): Linear coefficients, often denoted by
+                :math:`\\boldsymbol h`; also called *external field* in physics.
+            quadratic (list | numpy.ndarray): Quadratic coefficients, often
+                denoted by :math:`\\boldsymbol J`; also called *interactions* in
+                physics. If ``linear`` has shape ``(n,)``, this array must have
+                shape ``(n, n)``.
+            offset (float, optional): Constant offset added to the energy value.
+                Defaults to ``0.0``.
+
+        Returns:
+            Tuple containing ``qubo`` instance and a new offset value (float).
+        """
         lin = np.asarray(linear)
         qua = np.asarray(quadratic)
         n, = lin.shape
         assert qua.shape == (n, n), '`linear` and `quadratic` must have shapes (n,) and (n, n)'
-        qua_symm = np.tril(qua, -1).T + np.triu(qua, 1) + qua
-        m  = 2*np.diag(qua.sum(0)+lin)
-        m -= 4*np.triu(qua_symm, 1)
-        return cls(m)
+        qua_symm = qua + qua.T
+        qua_symm[np.diag_indices_from(qua)] = 0
+        m  = 2*np.diag(lin-qua_symm.sum(0))
+        m += 4*np.triu(qua_symm, 1)
+        c = qua.sum()-lin.sum()+offset
+        return cls(m), c
+
+    def unique_parameters(self):
+        """Return the unique parameter values of this QUBO instance.
 
+        Returns:
+            numpy.ndarray: Array containing the unique parameter values, sorted
+                in ascending order.
+        """
+        mask = np.triu_indices_from(self.m)
+        return np.unique(self.m[mask])
 
     def spectral_gap(self, return_optimum=False):
-        """Calculate the spectral gap of this QUBO instance.
-        Here, this is defined as the difference between the lowest and second-to lowest QUBO energy value across all bit vectors.
-        Note that the QUBO instance must be solved for calculating this value, therefore only QUBOs of sizes up to about 30 are feasible in practice.
+        """Calculate the spectral gap of this QUBO instance. Here, this is
+        defined as the difference between the lowest and second-to lowest QUBO
+        energy value across all bit vectors. Note that the QUBO instance must be
+        solved for calculating this value, therefore only QUBOs of sizes up to
+        about 30 are feasible in practice.
         
         Args:
-            return_optimum (bool, optional): If ``True``, returns the minimizing bit vector of this QUBO instance (which is calculated anyway). Defaults to False.
+            return_optimum (bool, optional): If ``True``, returns the minimizing
+            bit vector of this QUBO instance (which is calculated anyway).
+            Defaults to False.
 
         Raises:
-            ValueError: Raised if this QUBO instance is too large to be solved by brute force on the given system.
+            ValueError: Raised if this QUBO instance is too large to be solved
+            by brute force on the given system.
 
         Returns:
             sgap (float): Spectral gap.
             x (numpy.ndarray, optional): Minimizing bit vector.
         """
         warn_size(self.n, limit=25)
         try:
@@ -339,78 +407,109 @@
         sgap = v1-v0
         if return_optimum:
             return sgap, x
         else:
             return sgap
 
     def clamp(self, partial_assignment=None):
-        """Create QUBO instance equivalent to this but with a subset
-        of variables fixed (_clamped_) to constant values.
+        """Create QUBO instance equivalent to this but with a subset of
+        variables fixed (_clamped_) to constant values.
 
         Args:
-            partial_assignment (dict, optional): Dictionary mapping
-                variable indices (counting from 0) to constant values
-                0 or 1. Defaults to None, which does nothing and
-                returns a copy of this QUBO instance.
+            partial_assignment (dict, optional): Dictionary mapping variable
+                indices (counting from 0) to constant values 0 or 1. Defaults to
+                None, which does nothing and returns a copy of this QUBO
+                instance.
 
         Returns:
             qubo: Clamped QUBO instance.
-            const (float): Constant offset value, which must be added to the QUBO energy to obtain the original energy.
-            free (list): List of indices which the variable indices of the new QUBO instance correspond to (i.e., those indices that were not clamped).
+            const (float): Constant offset value, which must be added to the
+                QUBO energy to obtain the original energy.
+            free (list): List of indices which the variable indices of the new
+                QUBO instance correspond to (i.e., those indices that were not
+                clamped).
         """
         if partial_assignment is None:
             return self.copy(), 0, set(range(self.n))
         ones = list(sorted({i for i, b in partial_assignment.items() if b == 1}))
         free = list(sorted(set(range(self.n)).difference(partial_assignment.keys())))
         R = self.m.copy()
         const = R[ones, :][:, ones].sum()
         for i in free:
             R[i, i] += sum(R[l, i] if l<i else R[i, l] for l in ones)
         return qubo(R[free,:][:,free]), const, free
 
     def dx(self, x: np.ndarray):
-        """Discrete derivative w.r.t. ``x``.
-        The element at index ``i`` gives the QUBO energy change upon flipping the value of ``x[i]``.
-        
+        """Discrete derivative w.r.t. ``x``: The element at index ``i`` gives
+        the QUBO energy change upon flipping the value of ``x[i]``.
+
         Args:
-            x (np.ndarray): Bit vector w.r.t. which the discrete derivative is calculated. Can be an array of multiple bit vectors.
+            x (np.ndarray): Bit vector w.r.t. which the discrete derivative is
+                calculated. Can be an array of multiple bit vectors.
 
         Returns:
-            numpy.ndarray: Vector of discrete derivatives of this QUBO instance w.r.t. ``x``.
+            numpy.ndarray: Vector of discrete derivatives of this QUBO instance
+                w.r.t. ``x``.
         """
-        # 1st discrete derivatice
         m_  = np.triu(self.m, 1)
         m_ += m_.T
         sign = 1-2*x
         return sign*(np.diag(self.m)+(m_ @ x.T).T)
+        
+
+    def dx2(self, x: np.ndarray):
+        """2nd discrete derivative w.r.t. ``x``: Returns a matrix where the
+        element at index ``(i, j)`` gives the QUBO energy change upon flipping
+        both ``x[i]`` and ``x[j]`` simultaneously. The 1st discrete derivative
+        is along the diagonal.
+
+        Args:
+            x (np.ndarray): Bit vector w.r.t. which the discrete derivative is
+                calculated. Must have shape ``(n,)``.
+
+        Returns:
+            numpy.ndarray: Array of shape ``(n, n)`` containing the 2nd discrete
+                derivatives of this QUBO instance w.r.t. ``x``.
+
+        Examples:
+            Let ``Δ = Q.dx2(x)``, then ``Δ[i, j]`` is the same as
+            ``Q(flip_index(x, [i, j])) - Q(x)`` (see :func:`qubolite.bitvec.flip_index`).
+        """
+        dx = self.dx(x) # (m, n)
+        s = 2*x-1       # (m, n)
+        S = s[..., na] * s[..., na, :] * self.m
+        D = dx[..., na] + dx[..., na, :]
+        return np.triu(D+S, 1) + dx[..., na] * np.eye(self.n)
 
     def dynamic_range(self, decibel=False):
-        """Calculate the dynamic range (DR) of the QUBO parameters,
-        i.e., the logarithmic ratio between the largest and the smallest difference between all pairs of unique parameter values.
+        """Calculate the dynamic range (DR) of the QUBO parameters, i.e., the
+        logarithmic ratio between the largest and the smallest difference
+        between all pairs of unique parameter values.
 
         Args:
-            decibel (bool, optional): If ``True``, outputs the DR in the unit decibels. Defaults to False, which outputs the DR in bits.
+            decibel (bool, optional): If ``True``, outputs the DR in the unit
+                decibels. Defaults to False, which outputs the DR in bits.
 
         Returns:
             float: Dynamic range value.
         """
-        params = np.sort(np.unique(np.r_[self.m[np.triu_indices_from(self.m)], 0]))
+        params = np.unique(self.m) # <- doing this includes 0; result is sorted
         max_diff = params[-1]-params[0]
         min_diff = np.min(params[1:]-params[:-1])
         r = max_diff/min_diff
         return 20*np.log10(r) if decibel else np.log2(r)
 
     def absmax(self):
         """Returns the largest parameter by absolute value.
         This is equivalent to the infinity norm of the QUBO matrix.
 
         Returns:
             float: largest parameter by absolute value.
         """
-        return np.max(np.abs(self.m))
+        return np.max(np.abs(self.unique_parameters()))
 
     def round(self, *args):
         """Rounds the QUBO parameters to the nearest integers.
 
         Returns:
             qubo: QUBO instance with rounded parameters.
         """
@@ -425,106 +524,127 @@
         Returns:
             qubo: QUBO instance with scaled parameters.
         """
         return qubo(self.m*factor)
 
     def as_int(self, bits=32):
         """Scales and rounds the QUBO parameters to fit a given number of bits.
-        The number format is assumed to be signed integer, therefore ``b`` bits yields a value range of ``-2**(b-1)`` to ``2**(b-1)-1``.
+        The number format is assumed to be signed integer, therefore ``b`` bits
+        yields a value range of ``-2**(b-1)`` to ``2**(b-1)-1``.
 
         Args:
-            bits (int, optional): Number of bits to represent the parameters. Defaults to 32.
+            bits (int, optional): Number of bits to represent the parameters.
+                Defaults to 32.
 
         Returns:
             qubo: QUBO instance with scaled and rounded parameters.
         """
         p_min, p_max = self.m.min(), self.m.max()
         if np.abs(p_min) < np.abs(p_max):
             factor = ((2**(bits-1))-1)/np.abs(p_max)
         else:
             factor = (2**(bits-1))/np.abs(p_min)
         return qubo((self.m*factor).round())
 
     def partition_function(self, log=False, temp=1.0, fast=True):
-        """Calculate the partition function of the Ising model induced by this QUBO instance.
-        That is, return the sum of ``exp(-Q(x)/temp)`` over all bit vectors ``x``.
-        Note that this is infeasibly slow for QUBO sizes much larger than 20.
-
-        Args:
-            log (bool, optional): Return the natural log of the partition function instead. Defaults to False.
-            temp (float, optional): Temperature parameter of the Gibbs distribution. Defaults to 1.0.
-            fast (bool, optional): Internally create array of all bit vectors. This is faster, but requiers memory space exponential in the QUBO size. Defaults to True.
+        """Calculate the partition function of the Ising model induced by this
+        QUBO instance. That is, return the sum of ``exp(-Q(x)/temp)`` over all
+        bit vectors ``x``. Note that this is infeasibly slow for QUBO sizes much
+        larger than 20.
+
+        Args:
+            log (bool, optional): Return the natural log of the partition
+                function instead. Defaults to False.
+            temp (float, optional): Temperature parameter of the Gibbs
+                distribution. Defaults to 1.0.
+            fast (bool, optional): Internally create array of all bit vectors.
+                This is faster, but requiers memory space exponential in the
+                QUBO size. Defaults to True.
 
         Returns:
-            float: Value of the partition function, or the log partition function if ``log=True``.
+            float: Value of the partition function, or the log partition
+                function if ``log=True``.
         """
         Z = self.probabilities(temp=temp, unnormalized=True, fast=fast).sum()
         return np.log(Z) if log else Z
 
     def probabilities(self, temp=1.0, out=None, unnormalized=False, fast=True):
-        """Compute the complete vector of probabilities for observing a vector ``x`` under the Gibbs distribution induced by this QUBO instance.
-        The entries of the resulting array are sorted in lexicographic order by bit vector, e.g. for size 3: ``[000, 100, 010, 110, 001, 101, 011, 111]``.
-        Note that this method requires memory space exponential in QUBO size, which quickly becomes infeasible, depending on your system.
-        If ``n`` is the QUBO size, the output will have size ``2**n``.
+        """Compute the complete vector of probabilities for observing a vector
+        ``x`` under the Gibbs distribution induced by this QUBO instance. The
+        entries of the resulting array are sorted in lexicographic order by bit
+        vector, e.g. for size 3: ``[000, 100, 010, 110, 001, 101, 011, 111]``.
+        Note that this method requires memory space exponential in QUBO size,
+        which quickly becomes infeasible, depending on your system. If ``n`` is
+        the QUBO size, the output will have size ``2**n``.
         
         Args:
-            temp (float, optional): Temperature parameter of the Gibbs distribution. Defaults to 1.0.
-            out (numpy.ndarray, optional): Array to write the probabilities to. Defaults to None, which creates a new array.
-            unnormalized (bool, optional): Return the unnormalized probabilities. Defaults to False.
-            fast (bool, optional): Internally create array of all bit vectors. This is faster, but requiers memory space exponential in the QUBO size. Defaults to True.
+            temp (float, optional): Temperature parameter of the Gibbs
+                distribution. Defaults to 1.0.
+            out (numpy.ndarray, optional): Array to write the probabilities to.
+                Defaults to None, which creates a new array.
+            unnormalized (bool, optional): Return the unnormalized
+                probabilities. Defaults to False.
+            fast (bool, optional): Internally create array of all bit vectors.
+                This is faster, but requiers memory space exponential in the
+                QUBO size. Defaults to True.
 
         Returns:
             numpy.ndarray: Array containing probabilities.
         """
         if out is None:
             out = np.empty(1<<self.n)
         else:
             assert out.shape == (1<<self.n,), f'out array has wrong shape, ({1<<self.n},) expected'
         if fast:
-            # builds the entire (2**n, n)-array of n-bit vectors
+            # builds the entire (2**n, n) array of n-bit vectors
             X = all_bitvectors_array(self.n)
             out[...] = np.exp(-self(X)/temp)
         else:
             # uses less memory, but much slower
             warn_size(self.n, limit=20)
             for i, x in enumerate(all_bitvectors(self.n)):
                 out[i] = np.exp(-self(x)/temp)
         if unnormalized:
             return out
         return out/out.sum()
 
     def pairwise_marginals(self, temp=1.0, fast=True):
-        """Compute the marginal probabilities for each variable pair to assume the value (1, 1) under the Gibbs distribution induced by this QUBO instance.
-        Note that this operation's runtime is exponential in QUBO size.
+        """Compute the marginal probabilities for each variable pair to assume
+        the value (1, 1) under the Gibbs distribution induced by this QUBO
+        instance. Note that this operation's runtime is exponential in QUBO
+        size.
 
         Args:
-            temp (float, optional): Temperature parameter of the Gibbs distribution. Defaults to 1.0.
-            fast (bool, optional): Internally create array of all bit vectors. This is faster, but requiers memory space exponential in the QUBO size. Defaults to True.
+            temp (float, optional): Temperature parameter of the Gibbs
+                distribution. Defaults to 1.0.
+            fast (bool, optional): Internally create array of all bit vectors.
+                This is faster, but requiers memory space exponential in the
+                QUBO size. Defaults to True.
 
         Returns:
             numpy.ndarray: Upper triangular matrix of probabilities.
         """
         warn_size(self.n, limit=20)
         probs = self.probabilities(temp=temp, fast=fast)
         marginals = np.zeros((self.n, self.n))
         for x, p in zip(all_bitvectors(self.n), probs):
             suff_stat = np.outer(x, x)
             marginals += p*suff_stat
         return np.triu(marginals)
 
     def to_posiform(self):
         """Compute the unique posiform representation of this QUBO instance,
-        using the approach described in section 2.1 of [1].
-        The result is a tuple of an array ``P`` of shape ``(2, n, n)``, where ``n`` is the QUBO size,
-        and a constant offset value. All entries of the array are positive.
-        ``P[0]`` contains the coefficients for the literals ``Xi*Xj``, and ``Xi`` on the diagonal, while
-        ``P[1]`` contains the coefficients for ``Xi*!Xj`` (``!`` denoting negation), and ``!Xi`` on the diagonal.
-        See the paper for further infos.
-
-        [1] https://www.researchgate.net/publication/238379061_Preprocessing_of_unconstrained_quadratic_binary_optimization
+        using the approach described in section 2.1 of
+        `[1] <https://www.researchgate.net/publication/238379061_Preprocessing_of_unconstrained_quadratic_binary_optimization>`__.
+        The result is a tuple of an array ``P`` of shape ``(2, n, n)``, where
+        ``n`` is the QUBO size, and a constant offset value. All entries of the
+        array are positive. ``P[0]`` contains the coefficients for the literals
+        ``Xi*Xj``, and ``Xi`` on the diagonal, while ``P[1]`` contains the
+        coefficients for ``Xi*!Xj`` (``!`` denoting negation), and ``!Xi`` on
+        the diagonal. See the paper for further infos.
 
         Returns:
             numpy.ndarray: Posiform coefficients (see above)
             float: Constant offset value
         """
         posiform = np.zeros((2, self.n, self.n))
         # posiform[0] contains terms xi* xj, and  xi on diagonal
@@ -538,10 +658,25 @@
         posiform[0][diag_ix] = lin + qua_neg.sum(1)
         lin_ = posiform[0][diag_ix].copy()  # =: c'
         lin_neg = np.minimum(lin_, 0)
         posiform[1][diag_ix] = -lin_neg
         posiform[0][diag_ix] = np.maximum(lin_, 0)
         const = lin_neg.sum()
         return posiform, const
+    
 
-    def to_ising(self):
-        return NotImplemented
+def ordering_distance(Q1, Q2, X=None):
+    try:
+        from scipy.stats import kendalltau
+    except ImportError as e:
+        raise ImportError(
+            "scipy needs to be installed prior to running qubolite.ordering_distance(). You "
+            "can install scipy with:\n'pip install scipy'"
+        ) from e
+    assert Q1.n == Q2.n, 'QUBO instances must have the same dimension'
+    warn_size(Q1.n, limit=22)
+    if X is None:
+        X = all_bitvectors_array(Q1.n)
+    rnk1 = np.argsort(np.argsort(Q1(X)))
+    rnk2 = np.argsort(np.argsort(Q2(X)))
+    tau, _ = kendalltau(rnk1, rnk2)
+    return (1-tau)/2
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `qubolite-0.8.1/qubolite/sampling.py` & `qubolite-0.8.2/qubolite/sampling.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import struct
 from collections import Counter, defaultdict
 from functools   import cached_property
 
 import numpy as np
 
+from ._misc  import get_random_state, set_suffix
 from .bitvec import all_bitvectors_array, from_string, to_string
-from ._misc   import get_random_state, set_suffix
 
 
 class BinarySample:
     """Class for representing samples of binary vectors,
     e.g., measurements of a qubit system.
 
     Args:
@@ -106,22 +106,22 @@
 
     @cached_property
     def suff_stat(self):
         X = self.raw
         return np.triu(X.T @ X)
 
     def hellinger_distance(self, other):
-        """`Hellinger distance <https://en.wikipedia.org/wiki/Hellinger_distance#Discrete_distributions>`__ between this sample and another.
-        The Hellinger distance between two discrete probability
-        distributions :math:`p` and :math:`q` is defined as
+        """`Hellinger distance <https://en.wikipedia.org/wiki/Hellinger_distance#Discrete_distributions>`__
+        between this sample and another. The Hellinger distance between two
+        discrete probability distributions :math:`p` and :math:`q` is defined as
         
         :math:`\\frac{1}{\\sqrt{2}}\\sqrt{\\sum_{x\\in\\lbrace 0,1\\rbrace^n}(\\sqrt{p(x)}-\\sqrt{q(x)})^2}`.
         
-        In contrast to KL divergence, Hellinger distance is an
-        actual distance, in that it is symmetrical.
+        In contrast to KL divergence, Hellinger distance is an actual distance,
+        in that it is symmetrical.
 
         Args:
             other (BinarySample): Binary sample to compare against.
 
         Returns:
             float: Hellinger distance between the two samples.
         """
```

### Comparing `qubolite-0.8.1/qubolite/solving.py` & `qubolite-0.8.2/qubolite/solving.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import numpy as np
 
-from ._misc import get_random_state, warn_size
-from .qubo import qubo
+from ._misc   import get_random_state, warn_size
+from .bitvec  import flip_index
+from .qubo    import qubo
 from _c_utils import brute_force as _brute_force_c
 
 
 def brute_force(Q: qubo):
-    """Solve QUBO instance exactly by brute force.
-    Note that this method is infeasible for instances
-    with a size beyond around 30.
+    """Solve QUBO instance exactly by brute force. Note that this method is
+    infeasible for instances with a size beyond around 30.
 
     Args:
         Q (qubo): QUBO instance to solve.
 
     Raises:
-        ValueError: Raised if the QUBO size is too large to be brute-forced on the present system.
+        ValueError: Raised if the QUBO size is too large to be brute-forced on
+            the present system.
 
     Returns:
-        A tuple containing the minimizing vector (numpy.ndarray) and the minimal energy (float).
+        A tuple containing the minimizing vector (numpy.ndarray) and the minimal
+        energy (float).
     """
     warn_size(Q.n, limit=30)
     try:
         x, v, _ = _brute_force_c(Q.m)
     except TypeError:
         raise ValueError(f'n is too large to brute-force on this system')
     return x, v
@@ -30,37 +32,45 @@
 def simulated_annealing(Q: qubo,
                         schedule='2+',
                         halftime=0.25,
                         steps=100_000,
                         init_temp=None,
                         n_parallel=10,
                         random_state=None):
-    """Performs simulated annealing to approximate the minimizing
-    vector and minimal energy of a given QUBO instance.
+    """Performs simulated annealing to approximate the minimizing vector and
+    minimal energy of a given QUBO instance.
 
     Args:
         Q (qubo): QUBO instance.
-        schedule (str, optional): The annealing schedule to employ.
-            Possible values are: ``2+`` (quadratic additive), ``2*`` (quadratic multiplicative),
-            ``e+`` (exponential additive) and ``e*`` (exponential multiplicative).
-            See `here <http://what-when-how.com/artificial-intelligence/a-comparison-of-cooling-schedules-for-simulated-annealing-artificial-intelligence/>`__  for further infos. Defaults to '2+'.
-        halftime (float, optional): For multiplicative schedules only:
-            The percentage of steps after which the temperature is halved. Defaults to 0.25.
-        steps (int, optional): Number of annealing steps to perform. Defaults to 100_000.
-        init_temp (float, optional): Initial temperature. Defaults to None, which estimates an initial temperature.
-        n_parallel (int, optional): Number of random initial solutions to anneal simultaneously. Defaults to 10.
-        random_state (optional): A numerical or lexical seed, or a NumPy random generator. Defaults to None.
+        schedule (str, optional): The annealing schedule to employ. Possible
+            values are: ``2+`` (quadratic additive), ``2*`` (quadratic
+            multiplicative), ``e+`` (exponential additive) and ``e*``
+            (exponential multiplicative). See
+            `here <http://what-when-how.com/artificial-intelligence/a-comparison-of-cooling-schedules-for-simulated-annealing-artificial-intelligence/>`__ 
+            for further infos. Defaults to '2+'.
+        halftime (float, optional): For multiplicative schedules only: The
+            percentage of steps after which the temperature is halved. Defaults
+            to 0.25.
+        steps (int, optional): Number of annealing steps to perform. Defaults to
+            100_000.
+        init_temp (float, optional): Initial temperature. Defaults to None,
+            which estimates an initial temperature.
+        n_parallel (int, optional): Number of random initial solutions to anneal
+            simultaneously. Defaults to 10.
+        random_state (optional): A numerical or lexical seed, or a NumPy random
+            generator. Defaults to None.
 
     Raises:
         ValueError: Raised if the specificed schedule is unknown.
 
     Returns:
-        A tuple ``(x, y)`` containing the solution bit vectors and their respective energies.
-        The shape of ``x`` is ``(n_parallel, n)``, where ``n`` is the QUBO size; the shape of ``y``
-        is ``(n_parallel,)``. Bit vector ``x[i]`` has energy ``y[i]`` for each ``i``.
+        A tuple ``(x, y)`` containing the solution bit vectors and their
+        respective energies. The shape of ``x`` is ``(n_parallel, n)``, where
+        ``n`` is the QUBO size; the shape of ``y`` is ``(n_parallel,)``. Bit
+        vector ``x[i]`` has energy ``y[i]`` for each ``i``.
     """
     npr = get_random_state(random_state)
     if init_temp is None:
         # estimate initial temperature
         EΔy, k = 0, 0
         for _ in range(1000):
             x = npr.random(Q.n) < 0.5
@@ -71,22 +81,21 @@
         EΔy /= k
         initial_acc_prob = 0.99
         init_temp = -EΔy / np.log(initial_acc_prob)
         print(f'Init. temp. automatically set to {init_temp:.4f}')
 
     # setup cooling schedule
     if schedule == 'e+':
-        temps = init_temp / (
-                    1 + np.exp(2 * np.log(init_temp) * (np.linspace(0, 1, steps + 1) - 0.5)))
+        temps = init_temp/(1+np.exp(2*np.log(init_temp)*(np.linspace(0, 1, steps+1)-0.5)))
     elif schedule == '2+':
-        temps = init_temp * (1 - np.linspace(0, 1, steps + 1)) ** 2
+        temps = init_temp*(1-np.linspace(0, 1, steps+1))**2
     elif schedule == 'e*':
-        temps = init_temp * (0.5 ** (1 / halftime)) ** np.arange(0, 1, steps + 1)
+        temps = init_temp*(0.5**(1/halftime))**np.arange(0, 1, steps+1)
     elif schedule == '2*':
-        temps = init_temp / (1 + (1 / (halftime ** 2)) * np.linspace(0, 1, steps + 1) ** 2)
+        temps = init_temp/(1+(1/(halftime**2))*np.linspace(0, 1, steps+1)**2)
     else:
         raise ValueError('Unknown schedule; must be one of {e*, 2*, e+, 2+}.')
 
     x = (npr.random((n_parallel, Q.n)) < 0.5).astype(np.float64)
     y = Q(x)
     for temp in temps:
         z = npr.random((n_parallel, Q.n)) < (1 / Q.n)
@@ -98,58 +107,159 @@
         y = y + Δy * a
 
     srt = np.argsort(y)
     return x[srt, :], y[srt]
 
 
 def local_descent(Q: qubo, x=None, random_state=None):
-    """Starting from a given bit vector, find improvements in the
-    1-neighborhood and follow them until a local optimum is found.
-    If no initial vector is specified, a random vector is sampled.
-    At each step, the method greedily flips the bit that yields
-    greatest energy improvement.
+    """Starting from a given bit vector, find improvements in the 1-neighborhood
+    and follow them until a local optimum is found. If no initial vector is
+    specified, a random vector is sampled. At each step, the method greedily
+    flips the bit that yields the greatest energy improvement.
 
     Args:
         Q (qubo): QUBO instance.
         x (numpy.ndarray, optional): Initial bit vector. Defaults to None.
-        random_state (optional): A numerical or lexical seed, or a NumPy random generator. Defaults to None.
+        random_state (optional): A numerical or lexical seed, or a NumPy random
+            generator. Defaults to None.
 
     Returns:
-        A tuple containing the minimizing vector (numpy.ndarray) and the minimal energy (float).
+        A tuple containing the bit vector (numpy.ndarray) with lowest energy
+        found, and its energy (float).
     """
     if x is None:
         rng = get_random_state(random_state)
         x_ = rng.random(Q.n) < 0.5
     else:
         x_ = x.copy()
-    Δx = Q.dx(x_)
-    am = np.argmin(Δx)
-    while Δx[am] < 0:
-        x_[am] = 1 - x_[am]
+    while True:
         Δx = Q.dx(x_)
         am = np.argmin(Δx)
+        if Δx[am] >= 0:
+            break
+        x_[am] = 1 - x_[am]
     return x_, Q(x_)
 
 
+def local2_descent(Q: qubo, x=None, random_state=None):
+    """Starting from a given bit vector, find improvements in the 2-neighborhood
+    and follow them until a local optimum is found. If no initial vector is
+    specified, a random vector is sampled. At each step, the method greedily
+    flips up to two bits that yield the greatest energy improvement.
+
+    Args:
+        Q (qubo): QUBO instance.
+        x (numpy.ndarray, optional): Initial bit vector. Defaults to None.
+        random_state (optional): A numerical or lexical seed, or a NumPy random
+            generator. Defaults to None.
+
+    Returns:
+        A tuple containing the bit vector (numpy.ndarray) with lowest energy
+        found, and its energy (float).
+    """
+    if x is None:
+        rng = get_random_state(random_state)
+        x_ = rng.random(Q.n) < 0.5
+    else:
+        x_ = x.copy()
+    Δx = Q.dx2(x_) # (n, n) matrix
+    i, j = np.unravel_index(np.argmin(Δx), Δx.shape)
+    while True:
+        Δx = Q.dx2(x_)
+        i, j = np.unravel_index(np.argmin(Δx), Δx.shape)
+        if Δx[i, j] >= 0:
+            break
+        flip_index(x_, [i, j], in_place=True)
+    return x_, Q(x_)
+
+
+def local_descent_search(Q: qubo, steps=1000, random_state=None):
+    """Perform local descent in a multistart fashion and return the lowest
+    observed bit vector. Use the 1-neighborhood as search radius.
+
+    Args:
+        Q (qubo): QUBO instance.
+        steps (int, optional): Number of multistarts. Defaults to 1000.
+        random_state (optional): A numerical or lexical seed, or a NumPy random
+            generator. Defaults to None.
+
+    Returns:
+        A tuple containing the bit vector (numpy.ndarray) with lowest energy
+        found, and its energy (float).
+    """
+    rng = get_random_state(random_state)
+    x_min = np.empty(Q.n)
+    y_min = np.infty
+    x = np.empty(Q.n)
+    for _ in range(steps):
+        x[:] = rng.random(Q.n) < 0.5
+        while True:
+            Δx = Q.dx(x) # (n,) vector
+            am = np.argmin(Δx, axis=-1)
+            if Δx[am] >= 0:
+                break
+            x[am] = 1 - x[am]
+        y = Q(x)
+        if y <= y_min:
+            x_min[:] = x
+            y_min = y
+    return x_min, y_min
+
+
+def local2_descent_search(Q: qubo, steps=1000, random_state=None):
+    """Perform local descent in a multistart fashion and return the lowest
+    observed bit vector. Use the 2-neighborhood as search radius.
+
+    Args:
+        Q (qubo): QUBO instance.
+        steps (int, optional): Number of multistarts. Defaults to 1000.
+        random_state (optional): A numerical or lexical seed, or a NumPy random
+            generator. Defaults to None.
+
+    Returns:
+        A tuple containing the bit vector (numpy.ndarray) with lowest energy
+        found, and its energy (float).
+    """
+    rng = get_random_state(random_state)
+    x_min = np.empty(Q.n)
+    y_min = np.infty
+    x = np.empty(Q.n)
+    for _ in range(steps):
+        x[:] = rng.random(Q.n) < 0.5
+        while True:
+            Δx = Q.dx2(x) # (n, n) matrix
+            i, j = np.unravel_index(np.argmin(Δx), Δx.shape)
+            if Δx[i, j] >= 0:
+                break
+            flip_index(x, [i, j], in_place=True)
+        y = Q(x)
+        if y <= y_min:
+            x_min[:] = x
+            y_min = y
+    return x_min, y_min
+
+
 def random_search(Q: qubo, steps=100_000, n_parallel=None, random_state=None):
-    """Perform a random search in the space of bit vectors and return
-    the lowest-energy solution found.
+    """Perform a random search in the space of bit vectors and return the
+    lowest-energy solution found.
 
     Args:
         Q (qubo): QUBO instance.
         steps (int, optional): Number of steps to perform. Defaults to 100_000.
-        n_parallel (int, optional): Number of random bit vectors to sample at a time.
-            This does *not* increase the number of bit vectors sampled in total
-            (specified by ``steps``), but makes the procedure faster by using NumPy
-            vectorization. Defaults to None, which chooses a value such that the
-            resulting bit vector array has about 32k elements.
-        random_state (optional): A numerical or lexical seed, or a NumPy random generator. Defaults to None.
+        n_parallel (int, optional): Number of random bit vectors to sample at a
+            time. This does *not* increase the number of bit vectors sampled in
+            total (specified by ``steps``), but makes the procedure faster by
+            using NumPy vectorization. Defaults to None, which chooses a value
+            such that the resulting bit vector array has about 32k elements.
+        random_state (optional): A numerical or lexical seed, or a NumPy random
+            generator. Defaults to None.
 
     Returns:
-        A tuple containing the minimizing vector (numpy.ndarray) and the minimal energy (float).
+        A tuple containing the bit vector (numpy.ndarray) with lowest energy
+        found, and its energy (float).
     """
     rng = get_random_state(random_state)
     if n_parallel is None:
         n_parallel = 32_000 // Q.n
     x_min = np.empty(Q.n)
     y_min = np.infty
     remaining = steps
@@ -161,7 +271,40 @@
         y[:] = Q(x)
         i_min = np.argmin(y)
         if y[i_min] < y_min:
             x_min[:] = x[i_min, :]
             y_min = y[i_min]
         remaining -= r
     return x_min, y_min
+
+
+def subspace_search(Q: qubo, steps=1000, random_state=None):
+    """Perform search heuristic where :math:`n-\\log_2(n)` randomly selected
+    variables are fixed and the remaining :math:`\\log_2(n)` bits are solved by
+    brute force. The current solution is updated with the optimal sub-vector
+    assignment, and the process is repeated.
+
+    Args:
+        Q (qubo): QUBO instance.
+        steps (int, optional): Number of repetitions. Defaults to 1000.
+        random_state (optional): A numerical or lexical seed, or a NumPy random
+            generator. Defaults to None.
+
+    Returns:
+        A tuple containing the minimizing vector (numpy.ndarray) and the minimal
+        energy (float).
+    """
+    rng = get_random_state(random_state)
+    log_n = int(np.log2(Q.n))
+    variables = np.arange(Q.n).astype(int)
+    # sample random initial solution
+    x = (rng.random(Q.n) < 0.5).astype(np.float64)
+    for _ in range(steps):
+        # fix random subset of n - log(n) variables
+        rng.shuffle(variables)
+        fixed = variables[:Q.n-log_n]
+        Q_sub, _, free = Q.clamp(dict(zip(fixed, x[fixed])))
+        # find optimum in subspace by brute force
+        x_sub_opt, *_ = _brute_force_c(Q_sub.m)
+        # set variables in current solution to subspace-optimal bits
+        x[free] = x_sub_opt
+    return x, Q(x)
```

### Comparing `qubolite-0.8.1/setup.py` & `qubolite-0.8.2/setup.py`

 * *Files identical despite different names*

