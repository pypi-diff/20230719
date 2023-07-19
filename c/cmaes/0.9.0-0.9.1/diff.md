# Comparing `tmp/cmaes-0.9.0.tar.gz` & `tmp/cmaes-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmaes-0.9.0.tar", last modified: Tue Nov  8 07:21:59 2022, max compression
+gzip compressed data, was "cmaes-0.9.1.tar", last modified: Fri Jan  6 06:04:30 2023, max compression
```

## Comparing `cmaes-0.9.0.tar` & `cmaes-0.9.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 07:21:59.848804 cmaes-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-11-08 07:21:48.000000 cmaes-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    17118 2022-11-08 07:21:59.848804 cmaes-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    16008 2022-11-08 07:21:48.000000 cmaes-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 07:21:59.848804 cmaes-0.9.0/cmaes/
--rw-r--r--   0 runner    (1001) docker     (121)      175 2022-11-08 07:21:48.000000 cmaes-0.9.0/cmaes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14637 2022-11-08 07:21:48.000000 cmaes-0.9.0/cmaes/_cma.py
--rw-r--r--   0 runner    (1001) docker     (121)    24004 2022-11-08 07:21:48.000000 cmaes-0.9.0/cmaes/_cmawm.py
--rw-r--r--   0 runner    (1001) docker     (121)    11960 2022-11-08 07:21:48.000000 cmaes-0.9.0/cmaes/_sepcma.py
--rw-r--r--   0 runner    (1001) docker     (121)     1001 2022-11-08 07:21:48.000000 cmaes-0.9.0/cmaes/_stats.py
--rw-r--r--   0 runner    (1001) docker     (121)     2479 2022-11-08 07:21:48.000000 cmaes-0.9.0/cmaes/_warm_start.py
--rw-r--r--   0 runner    (1001) docker     (121)      211 2022-11-08 07:21:48.000000 cmaes-0.9.0/cmaes/cma.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 07:21:59.848804 cmaes-0.9.0/cmaes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    17118 2022-11-08 07:21:59.000000 cmaes-0.9.0/cmaes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      295 2022-11-08 07:21:59.000000 cmaes-0.9.0/cmaes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-08 07:21:59.000000 cmaes-0.9.0/cmaes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-11-08 07:21:59.000000 cmaes-0.9.0/cmaes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-11-08 07:21:59.000000 cmaes-0.9.0/cmaes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1431 2022-11-08 07:21:59.848804 cmaes-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-11-08 07:21:48.000000 cmaes-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 06:04:30.770602 cmaes-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-01-06 06:04:20.000000 cmaes-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18314 2023-01-06 06:04:30.770602 cmaes-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16018 2023-01-06 06:04:20.000000 cmaes-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 06:04:30.766602 cmaes-0.9.1/cmaes/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-01-06 06:04:20.000000 cmaes-0.9.1/cmaes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14675 2023-01-06 06:04:20.000000 cmaes-0.9.1/cmaes/_cma.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13077 2023-01-06 06:04:20.000000 cmaes-0.9.1/cmaes/_cmawm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12016 2023-01-06 06:04:20.000000 cmaes-0.9.1/cmaes/_sepcma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-01-06 06:04:20.000000 cmaes-0.9.1/cmaes/_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-01-06 06:04:20.000000 cmaes-0.9.1/cmaes/_warm_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-01-06 06:04:20.000000 cmaes-0.9.1/cmaes/cma.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 06:04:30.770602 cmaes-0.9.1/cmaes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18314 2023-01-06 06:04:30.000000 cmaes-0.9.1/cmaes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-01-06 06:04:30.000000 cmaes-0.9.1/cmaes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-06 06:04:30.000000 cmaes-0.9.1/cmaes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-06 06:04:30.000000 cmaes-0.9.1/cmaes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-06 06:04:30.000000 cmaes-0.9.1/cmaes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-01-06 06:04:20.000000 cmaes-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-01-06 06:04:30.770602 cmaes-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-01-06 06:04:20.000000 cmaes-0.9.1/setup.py
```

### Comparing `cmaes-0.9.0/LICENSE` & `cmaes-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cmaes-0.9.0/PKG-INFO` & `cmaes-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,49 @@
 Metadata-Version: 2.1
 Name: cmaes
-Version: 0.9.0
+Version: 0.9.1
 Summary: Lightweight Covariance Matrix Adaptation Evolution Strategy (CMA-ES) implementation for Python 3.
-Home-page: https://github.com/CyberAgent/cmaes
-Author: Masashi Shibata
-Author-email: m.shibata1020@gmail.com
-Maintainer: Masahiro Nomura
-Maintainer-email: nomura_masahiro@cyberagent.co.jp
+Author-email: Masashi Shibata <m.shibata1020@gmail.com>
+Maintainer-email: Masahiro Nomura <nomura_masahiro@cyberagent.co.jp>
 License: MIT License
+        
+        Copyright (c) 2020-2021 CyberAgent, Inc.
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/CyberAgentAILab/cmaes
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Intended Audience :: Science/Research
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: cmawm
 License-File: LICENSE
 
 # CMA-ES
 
 [![Software License](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square)](./LICENSE) [![PyPI - Downloads](https://img.shields.io/pypi/dw/cmaes)](https://pypistats.org/packages/cmaes)
@@ -38,15 +56,15 @@
 * **2022/05/13** The paper, ["CMA-ES with Margin: Lower-Bounding Marginal Probability for Mixed-Integer Black-Box Optimization"](https://arxiv.org/abs/2205.13482) written by Hamano, Saito, [@nomuramasahir0](https://github.com/nomuramasahir0) (the maintainer of this library), and Shirakawa, has been nominated as best paper at GECCO'22 ENUM track.
 * **2021/03/10** ["Introduction to CMA-ES sampler"](https://medium.com/optuna/introduction-to-cma-es-sampler-ee68194c8f88) is published at Optuna Medium Blog. This article explains when and how to make the best use out of CMA-ES sampler. Please check it out!
 * **2021/02/02** The paper ["Warm Starting CMA-ES for Hyperparameter Optimization"](https://arxiv.org/abs/2012.06932) written by [@nomuramasahir0](https://github.com/nomuramasahir0), the maintainer of this library, is accepted at AAAI 2021 :tada:
 * **2020/07/29** Optuna's built-in CMA-ES sampler which uses this library under the hood is stabled at Optuna v2.0. Please check out the [v2.0 release blog](https://medium.com/optuna/optuna-v2-3165e3f1fc2).
 
 ## Installation
 
-Supported Python versions are 3.6 or later.
+Supported Python versions are 3.7 or later.
 
 ```
 $ pip install cmaes
 ```
 
 Or you can install via [conda-forge](https://anaconda.org/conda-forge/cmaes).
 
@@ -76,15 +94,15 @@
             solutions.append((x, value))
             print(f"#{generation} {value} (x1={x[0]}, x2 = {x[1]})")
         optimizer.tell(solutions)
 ```
 
 And you can use this library via [Optuna](https://github.com/optuna/optuna) [2], an automatic hyperparameter optimization framework.
 Optuna's built-in CMA-ES sampler which uses this library under the hood is available from [v1.3.0](https://github.com/optuna/optuna/releases/tag/v1.3.0) and stabled at [v2.0.0](https://github.com/optuna/optuna/releases/tag/v2.2.0).
-See [the documentation](https://optuna.readthedocs.io/en/stable/reference/samplers.html#optuna.samplers.CmaEsSampler) or [v2.0 release blog](https://medium.com/optuna/optuna-v2-3165e3f1fc2) for more details.
+See [the documentation](https://optuna.readthedocs.io/en/stable/reference/samplers/generated/optuna.samplers.CmaEsSampler.html) or [v2.0 release blog](https://medium.com/optuna/optuna-v2-3165e3f1fc2) for more details.
 
 ```python
 import optuna
 
 def objective(trial: optuna.Trial):
     x1 = trial.suggest_uniform("x1", -4, 4)
     x2 = trial.suggest_uniform("x2", -4, 4)
```

### Comparing `cmaes-0.9.0/README.md` & `cmaes-0.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 * **2022/05/13** The paper, ["CMA-ES with Margin: Lower-Bounding Marginal Probability for Mixed-Integer Black-Box Optimization"](https://arxiv.org/abs/2205.13482) written by Hamano, Saito, [@nomuramasahir0](https://github.com/nomuramasahir0) (the maintainer of this library), and Shirakawa, has been nominated as best paper at GECCO'22 ENUM track.
 * **2021/03/10** ["Introduction to CMA-ES sampler"](https://medium.com/optuna/introduction-to-cma-es-sampler-ee68194c8f88) is published at Optuna Medium Blog. This article explains when and how to make the best use out of CMA-ES sampler. Please check it out!
 * **2021/02/02** The paper ["Warm Starting CMA-ES for Hyperparameter Optimization"](https://arxiv.org/abs/2012.06932) written by [@nomuramasahir0](https://github.com/nomuramasahir0), the maintainer of this library, is accepted at AAAI 2021 :tada:
 * **2020/07/29** Optuna's built-in CMA-ES sampler which uses this library under the hood is stabled at Optuna v2.0. Please check out the [v2.0 release blog](https://medium.com/optuna/optuna-v2-3165e3f1fc2).
 
 ## Installation
 
-Supported Python versions are 3.6 or later.
+Supported Python versions are 3.7 or later.
 
 ```
 $ pip install cmaes
 ```
 
 Or you can install via [conda-forge](https://anaconda.org/conda-forge/cmaes).
 
@@ -48,15 +48,15 @@
             solutions.append((x, value))
             print(f"#{generation} {value} (x1={x[0]}, x2 = {x[1]})")
         optimizer.tell(solutions)
 ```
 
 And you can use this library via [Optuna](https://github.com/optuna/optuna) [2], an automatic hyperparameter optimization framework.
 Optuna's built-in CMA-ES sampler which uses this library under the hood is available from [v1.3.0](https://github.com/optuna/optuna/releases/tag/v1.3.0) and stabled at [v2.0.0](https://github.com/optuna/optuna/releases/tag/v2.2.0).
-See [the documentation](https://optuna.readthedocs.io/en/stable/reference/samplers.html#optuna.samplers.CmaEsSampler) or [v2.0 release blog](https://medium.com/optuna/optuna-v2-3165e3f1fc2) for more details.
+See [the documentation](https://optuna.readthedocs.io/en/stable/reference/samplers/generated/optuna.samplers.CmaEsSampler.html) or [v2.0 release blog](https://medium.com/optuna/optuna-v2-3165e3f1fc2) for more details.
 
 ```python
 import optuna
 
 def objective(trial: optuna.Trial):
     x1 = trial.suggest_uniform("x1", -4, 4)
     x2 = trial.suggest_uniform("x2", -4, 4)
```

### Comparing `cmaes-0.9.0/cmaes/_cma.py` & `cmaes-0.9.1/cmaes/_cma.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
+from __future__ import annotations
+
 import math
 import numpy as np
 
 from typing import Any
 from typing import cast
-from typing import Dict
-from typing import List
 from typing import Optional
-from typing import Tuple
 
 
 _EPS = 1e-8
 _MEAN_MAX = 1e32
 _SIGMA_MAX = 1e32
 
 
@@ -192,28 +191,28 @@
         self._tolxup = 1e4
         self._tolfun = 1e-12
         self._tolconditioncov = 1e14
 
         self._funhist_term = 10 + math.ceil(30 * n_dim / population_size)
         self._funhist_values = np.empty(self._funhist_term * 2)
 
-    def __getstate__(self) -> Dict[str, Any]:
+    def __getstate__(self) -> dict[str, Any]:
         attrs = {}
         for name in self.__dict__:
             # Remove _rng in pickle serialized object.
             if name == "_rng":
                 continue
             if name == "_C":
                 sym1d = _compress_symmetric(self._C)
                 attrs["_c_1d"] = sym1d
                 continue
             attrs[name] = getattr(self, name)
         return attrs
 
-    def __setstate__(self, state: Dict[str, Any]) -> None:
+    def __setstate__(self, state: dict[str, Any]) -> None:
         state["_C"] = _decompress_symmetric(state["_c_1d"])
         del state["_c_1d"]
         self.__dict__.update(state)
         # Set _rng for unpickled object.
         setattr(self, "_rng", np.random.RandomState())
 
     @property
@@ -228,14 +227,17 @@
 
     @property
     def generation(self) -> int:
         """Generation number which is monotonically incremented
         when multi-variate gaussian distribution is updated."""
         return self._g
 
+    def reseed_rng(self, seed: int) -> None:
+        self._rng.seed(seed)
+
     def set_bounds(self, bounds: Optional[np.ndarray]) -> None:
         """Update boundary constraints"""
         assert bounds is None or _is_valid_bounds(bounds, self._mean), "invalid bounds"
         self._bounds = bounds
 
     def ask(self) -> np.ndarray:
         """Sample a parameter"""
@@ -243,15 +245,15 @@
             x = self._sample_solution()
             if self._is_feasible(x):
                 return x
         x = self._sample_solution()
         x = self._repair_infeasible_params(x)
         return x
 
-    def _eigen_decomposition(self) -> Tuple[np.ndarray, np.ndarray]:
+    def _eigen_decomposition(self) -> tuple[np.ndarray, np.ndarray]:
         if self._B is not None and self._D is not None:
             return self._B, self._D
 
         self._C = (self._C + self._C.T) / 2
         D2, B = np.linalg.eigh(self._C)
         D = np.sqrt(np.where(D2 < 0, _EPS, D2))
         self._C = np.dot(np.dot(B, np.diag(D**2)), B.T)
@@ -279,15 +281,15 @@
             return param
 
         # clip with lower and upper bound.
         param = np.where(param < self._bounds[:, 0], self._bounds[:, 0], param)
         param = np.where(param > self._bounds[:, 1], self._bounds[:, 1], param)
         return param
 
-    def tell(self, solutions: List[Tuple[np.ndarray, float]]) -> None:
+    def tell(self, solutions: list[tuple[np.ndarray, float]]) -> None:
         """Tell evaluation values"""
 
         assert len(solutions) == self._popsize, "Must tell popsize-length solutions."
         for s in solutions:
             assert np.all(
                 np.abs(s[0]) < _MEAN_MAX
             ), f"Abs of all param values must be less than {_MEAN_MAX} to avoid overflow errors"
```

### Comparing `cmaes-0.9.0/cmaes/_sepcma.py` & `cmaes-0.9.1/cmaes/_sepcma.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
+from __future__ import annotations
+
 import math
 import numpy as np
 
-from typing import Any, cast
-from typing import Dict
-from typing import List
+from typing import Any
+from typing import cast
 from typing import Optional
-from typing import Tuple
 
 
 _EPS = 1e-8
 _MEAN_MAX = 1e32
 _SIGMA_MAX = 1e32
 
 
@@ -173,24 +173,27 @@
 
     @property
     def generation(self) -> int:
         """Generation number which is monotonically incremented
         when multi-variate gaussian distribution is updated."""
         return self._g
 
-    def __getstate__(self) -> Dict[str, Any]:
+    def reseed_rng(self, seed: int) -> None:
+        self._rng.seed(seed)
+
+    def __getstate__(self) -> dict[str, Any]:
         attrs = {}
         for name in self.__dict__:
             # Remove _rng in pickle serialized object.
             if name == "_rng":
                 continue
             attrs[name] = getattr(self, name)
         return attrs
 
-    def __setstate__(self, state: Dict[str, Any]) -> None:
+    def __setstate__(self, state: dict[str, Any]) -> None:
         self.__dict__.update(state)
         # Set _rng for unpickled object.
         setattr(self, "_rng", np.random.RandomState())
 
     def set_bounds(self, bounds: Optional[np.ndarray]) -> None:
         """Update boundary constraints"""
         assert bounds is None or _is_valid_bounds(bounds, self._mean), "invalid bounds"
@@ -232,15 +235,15 @@
             return param
 
         # clip with lower and upper bound.
         param = np.where(param < self._bounds[:, 0], self._bounds[:, 0], param)
         param = np.where(param > self._bounds[:, 1], self._bounds[:, 1], param)
         return param
 
-    def tell(self, solutions: List[Tuple[np.ndarray, float]]) -> None:
+    def tell(self, solutions: list[tuple[np.ndarray, float]]) -> None:
         """Tell evaluation values"""
 
         assert len(solutions) == self._popsize, "Must tell popsize-length solutions."
         for s in solutions:
             assert np.all(
                 np.abs(s[0]) < _MEAN_MAX
             ), f"Abs of all param values must be less than {_MEAN_MAX} to avoid overflow errors"
```

### Comparing `cmaes-0.9.0/cmaes/_stats.py` & `cmaes-0.9.1/cmaes/_stats.py`

 * *Files identical despite different names*

### Comparing `cmaes-0.9.0/cmaes/_warm_start.py` & `cmaes-0.9.1/cmaes/_warm_start.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
+from __future__ import annotations
+
 import math
 import numpy as np
 
-from typing import Tuple, List
-
 
 def get_warm_start_mgd(
-    source_solutions: List[Tuple[np.ndarray, float]],
+    source_solutions: list[tuple[np.ndarray, float]],
     gamma: float = 0.1,
     alpha: float = 0.1,
-) -> Tuple[np.ndarray, float, np.ndarray]:
+) -> tuple[np.ndarray, float, np.ndarray]:
     """Estimates a promising distribution of the source task, then
     returns a multivariate gaussian distribution (the mean vector
     and the covariance matrix) used for initialization of the CMA-ES.
 
     Args:
         source_solutions:
             List of solutions (parameter, value) on a source task.
```

### Comparing `cmaes-0.9.0/cmaes.egg-info/PKG-INFO` & `cmaes-0.9.1/cmaes.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,49 @@
 Metadata-Version: 2.1
 Name: cmaes
-Version: 0.9.0
+Version: 0.9.1
 Summary: Lightweight Covariance Matrix Adaptation Evolution Strategy (CMA-ES) implementation for Python 3.
-Home-page: https://github.com/CyberAgent/cmaes
-Author: Masashi Shibata
-Author-email: m.shibata1020@gmail.com
-Maintainer: Masahiro Nomura
-Maintainer-email: nomura_masahiro@cyberagent.co.jp
+Author-email: Masashi Shibata <m.shibata1020@gmail.com>
+Maintainer-email: Masahiro Nomura <nomura_masahiro@cyberagent.co.jp>
 License: MIT License
+        
+        Copyright (c) 2020-2021 CyberAgent, Inc.
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/CyberAgentAILab/cmaes
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Intended Audience :: Science/Research
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: cmawm
 License-File: LICENSE
 
 # CMA-ES
 
 [![Software License](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square)](./LICENSE) [![PyPI - Downloads](https://img.shields.io/pypi/dw/cmaes)](https://pypistats.org/packages/cmaes)
@@ -38,15 +56,15 @@
 * **2022/05/13** The paper, ["CMA-ES with Margin: Lower-Bounding Marginal Probability for Mixed-Integer Black-Box Optimization"](https://arxiv.org/abs/2205.13482) written by Hamano, Saito, [@nomuramasahir0](https://github.com/nomuramasahir0) (the maintainer of this library), and Shirakawa, has been nominated as best paper at GECCO'22 ENUM track.
 * **2021/03/10** ["Introduction to CMA-ES sampler"](https://medium.com/optuna/introduction-to-cma-es-sampler-ee68194c8f88) is published at Optuna Medium Blog. This article explains when and how to make the best use out of CMA-ES sampler. Please check it out!
 * **2021/02/02** The paper ["Warm Starting CMA-ES for Hyperparameter Optimization"](https://arxiv.org/abs/2012.06932) written by [@nomuramasahir0](https://github.com/nomuramasahir0), the maintainer of this library, is accepted at AAAI 2021 :tada:
 * **2020/07/29** Optuna's built-in CMA-ES sampler which uses this library under the hood is stabled at Optuna v2.0. Please check out the [v2.0 release blog](https://medium.com/optuna/optuna-v2-3165e3f1fc2).
 
 ## Installation
 
-Supported Python versions are 3.6 or later.
+Supported Python versions are 3.7 or later.
 
 ```
 $ pip install cmaes
 ```
 
 Or you can install via [conda-forge](https://anaconda.org/conda-forge/cmaes).
 
@@ -76,15 +94,15 @@
             solutions.append((x, value))
             print(f"#{generation} {value} (x1={x[0]}, x2 = {x[1]})")
         optimizer.tell(solutions)
 ```
 
 And you can use this library via [Optuna](https://github.com/optuna/optuna) [2], an automatic hyperparameter optimization framework.
 Optuna's built-in CMA-ES sampler which uses this library under the hood is available from [v1.3.0](https://github.com/optuna/optuna/releases/tag/v1.3.0) and stabled at [v2.0.0](https://github.com/optuna/optuna/releases/tag/v2.2.0).
-See [the documentation](https://optuna.readthedocs.io/en/stable/reference/samplers.html#optuna.samplers.CmaEsSampler) or [v2.0 release blog](https://medium.com/optuna/optuna-v2-3165e3f1fc2) for more details.
+See [the documentation](https://optuna.readthedocs.io/en/stable/reference/samplers/generated/optuna.samplers.CmaEsSampler.html) or [v2.0 release blog](https://medium.com/optuna/optuna-v2-3165e3f1fc2) for more details.
 
 ```python
 import optuna
 
 def objective(trial: optuna.Trial):
     x1 = trial.suggest_uniform("x1", -4, 4)
     x2 = trial.suggest_uniform("x2", -4, 4)
```

