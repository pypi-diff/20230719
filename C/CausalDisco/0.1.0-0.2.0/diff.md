# Comparing `tmp/causaldisco-0.1.0.tar.gz` & `tmp/causaldisco-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "causaldisco-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "causaldisco-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `causaldisco-0.1.0.tar` & `causaldisco-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0        0 2023-07-11 08:50:38.782313 causaldisco-0.1.0/CausalDisco/__init__.py
--rw-r--r--   0        0        0     2167 2023-07-11 08:50:38.782313 causaldisco-0.1.0/CausalDisco/analytics.py
--rw-r--r--   0        0        0     1960 2023-07-11 08:50:38.786313 causaldisco-0.1.0/CausalDisco/baselines.py
--rw-r--r--   0        0        0     1020 2023-07-11 08:50:38.786313 causaldisco-0.1.0/README.md
--rw-r--r--   0        0        0      767 2023-07-11 08:50:38.786313 causaldisco-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1647 1970-01-01 00:00:00.000000 causaldisco-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-19 14:56:51.107361 causaldisco-0.2.0/CausalDisco/__init__.py
+-rw-r--r--   0        0        0     2638 2023-07-19 14:56:51.107361 causaldisco-0.2.0/CausalDisco/analytics.py
+-rw-r--r--   0        0        0     1766 2023-07-19 14:56:51.107361 causaldisco-0.2.0/CausalDisco/baselines.py
+-rw-r--r--   0        0        0        0 2023-07-19 14:56:51.107361 causaldisco-0.2.0/CausalDisco/tests/__init__.py
+-rw-r--r--   0        0        0     2833 2023-07-19 14:56:51.107361 causaldisco-0.2.0/CausalDisco/tests/tests.py
+-rw-r--r--   0        0        0     3265 2023-07-19 14:56:51.107361 causaldisco-0.2.0/README.md
+-rw-r--r--   0        0        0      778 2023-07-19 14:56:51.111361 causaldisco-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3913 1970-01-01 00:00:00.000000 causaldisco-0.2.0/PKG-INFO
```

### Comparing `causaldisco-0.1.0/CausalDisco/baselines.py` & `causaldisco-0.2.0/CausalDisco/baselines.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,66 +1,67 @@
 import numpy as np
 from sklearn.linear_model import LinearRegression, LassoLarsIC
+from CausalDisco.analytics import r2coeff
 
 
 def sort_regress(X, scores):
-    """ 
-    Regress each variable onto all predecessors in the ordering incurred by the criterion.
+    """
+    Regress each variable onto all predecessors in
+    the ordering implied by the scores.
     Args:
         X: (n x d) matrix
-        ordering: (n) vector 
+        scores: (d) vector
     Returns:
-        causal structure matrix with coefficients.
+        Candidate causal structure matrix with coefficients
     """
     LR = LinearRegression()
     LL = LassoLarsIC(criterion='bic')
     d = X.shape[1]
     W = np.zeros((d, d))
     ordering = np.argsort(scores)
-    
+
     # backward regression
     for k in range(1, d):
         cov = ordering[:k]
         target = ordering[k]
         LR.fit(X[:, cov], X[:, target].ravel())
         weight = np.abs(LR.coef_)
         LL.fit(X[:, cov] * weight, X[:, target].ravel())
         W[cov, target] = LL.coef_ * weight
     return W
 
 
+def random_sort_regress(X, seed=None):
+    """
+    Perform sort_regress using a random order.
+    Args:
+        X: n x d data,
+        seed (optional): int
+    Returns:
+        Candidate causal structure matrix with coefficients.
+    """
+    if seed is None:
+        seed = np.random.randint(0, np.iinfo('int').max)
+    rng = np.random.default_rng(seed)
+    return sort_regress(X, rng.permutation(X.shape[1]))
+
+
 def var_sort_regress(X):
-    """ 
+    """
     Perform sort_regress using variances as ordering criterion.
     Args:
         X: n x d data,
     Returns:
-        causal structure matrix with coefficients.
+        Candidate causal structure matrix with coefficients.
     """
     return sort_regress(X, np.var(X, axis=0))
 
 
 def r2_sort_regress(X):
-    """ 
-    Perform sort_regress using R^2 as ordering criterion. R^2 are computed using partial correlations obtained through matrix inversion.
+    """
+    Perform sort_regress using R^2 as ordering criterion.
     Args:
         X: n x d data,
     Returns:
-        causal structure matrix with coefficients.
+        Candidate causal structure matrix with coefficients.
     """
-    return sort_regress(X, 1 - np.diag(1/np.linalg.inv(np.corrcoef(X.T))))
-
-
-if __name__ == "__main__":
-    d = 10
-    W = np.diag(np.ones(d-1), 1)
-    print(f'True\n{W}')
-    X = np.random.randn(10000, d).dot(np.linalg.inv(np.eye(d) - W))
-    X_std = (X - np.mean(X, axis=0))/np.std(X, axis=0)
-
-    print('--- varSortnRegress ---')
-    print(f'Recovered:\n{1.0*(var_sort_regress(X)!=0)}')
-    print(f'Recovered standardized:\n{1.0*(var_sort_regress(X_std)!=0)}')
-
-    print('--- r2SortnRegress ---')
-    print(f'Recovered:\n{1.0*(r2_sort_regress(X)!=0)}')
-    print(f'Recovered standardized:\n{1.0*(r2_sort_regress(X_std)!=0)}')
+    return sort_regress(X, r2coeff(X.T))
```

### Comparing `causaldisco-0.1.0/pyproject.toml` & `causaldisco-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "CausalDisco"
 description = """Baseline algorithms and analytics tools for Causal Discovery."""
 authors = [
-    {name = "Alexander G. Reisach"}, 
+    {name = "Alexander G. Reisach"},
     {name = "Sebastian Weichwald"},
 ]
 license = {text = "BSD 3-Clause License"}
 keywords = [
   "causality",
   "causal discovery",
 ]
@@ -21,10 +21,11 @@
   "Topic :: Scientific/Engineering :: Artificial Intelligence",
   "License :: OSI Approved :: BSD License",
   "Intended Audience :: Science/Research",
 ]
 dependencies = [
   "numpy",
   "scikit-learn",
+  "scipy",
 ]
 readme = "README.md"
-version = "0.1.0"
+version = "0.2.0"
```

