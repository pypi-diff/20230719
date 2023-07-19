# Comparing `tmp/psychoanalyze-0.6.2.tar.gz` & `tmp/psychoanalyze-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychoanalyze-0.6.2.tar", max compression
+gzip compressed data, was "psychoanalyze-0.6.3.tar", max compression
```

## Comparing `psychoanalyze-0.6.2.tar` & `psychoanalyze-0.6.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    35149 2023-07-16 03:40:00.954832 psychoanalyze-0.6.2/LICENSE
--rw-r--r--   0        0        0     1105 2023-07-16 03:40:00.954832 psychoanalyze-0.6.2/README.md
--rw-r--r--   0        0        0     1357 2023-07-16 03:43:03.128028 psychoanalyze-0.6.2/psychoanalyze/__init__.py
--rw-r--r--   0        0        0      756 2023-07-16 03:40:01.050833 psychoanalyze-0.6.2/psychoanalyze/analysis/__init__.py
--rw-r--r--   0        0        0     1288 2023-07-16 03:40:01.050833 psychoanalyze-0.6.2/psychoanalyze/analysis/bayes.py
--rw-r--r--   0        0        0     1120 2023-07-16 03:40:01.050833 psychoanalyze-0.6.2/psychoanalyze/analysis/ecdf.py
--rw-r--r--   0        0        0     2302 2023-07-16 03:40:01.050833 psychoanalyze-0.6.2/psychoanalyze/analysis/strength_duration.py
--rw-r--r--   0        0        0     2373 2023-07-16 03:40:01.050833 psychoanalyze-0.6.2/psychoanalyze/analysis/weber.py
--rw-r--r--   0        0        0     1153 2023-07-16 03:40:01.050833 psychoanalyze-0.6.2/psychoanalyze/data/__init__.py
--rw-r--r--   0        0        0     7140 2023-07-16 03:40:01.050833 psychoanalyze-0.6.2/psychoanalyze/data/blocks.py
--rw-r--r--   0        0        0     7225 2023-07-16 03:40:01.050833 psychoanalyze-0.6.2/psychoanalyze/data/points.py
--rw-r--r--   0        0        0     2868 2023-07-16 03:40:01.050833 psychoanalyze-0.6.2/psychoanalyze/data/sessions.py
--rw-r--r--   0        0        0      841 2023-07-16 03:40:01.050833 psychoanalyze-0.6.2/psychoanalyze/data/stimulus.py
--rw-r--r--   0        0        0     1678 2023-07-16 03:40:01.050833 psychoanalyze-0.6.2/psychoanalyze/data/subjects.py
--rw-r--r--   0        0        0     5206 2023-07-16 03:40:01.050833 psychoanalyze-0.6.2/psychoanalyze/data/trials.py
--rw-r--r--   0        0        0     3002 2023-07-16 03:40:01.050833 psychoanalyze-0.6.2/psychoanalyze/data/types.py
--rw-r--r--   0        0        0     1589 2023-07-16 03:40:01.050833 psychoanalyze-0.6.2/psychoanalyze/plot.py
--rw-r--r--   0        0        0     1518 2023-07-16 03:40:01.050833 psychoanalyze-0.6.2/psychoanalyze/sigmoids.py
--rw-r--r--   0        0        0     1919 2023-07-16 03:43:03.128028 psychoanalyze-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     2748 1970-01-01 00:00:00.000000 psychoanalyze-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-10-04 02:36:06.350931 psychoanalyze-0.6.3/LICENSE
+-rw-r--r--   0        0        0     1105 2023-07-10 23:11:08.910130 psychoanalyze-0.6.3/README.md
+-rw-r--r--   0        0        0     1357 2023-07-10 06:32:31.020291 psychoanalyze-0.6.3/psychoanalyze/__init__.py
+-rw-r--r--   0        0        0      756 2023-07-10 06:35:55.935533 psychoanalyze-0.6.3/psychoanalyze/analysis/__init__.py
+-rw-r--r--   0        0        0     1288 2023-07-10 06:35:48.275360 psychoanalyze-0.6.3/psychoanalyze/analysis/bayes.py
+-rw-r--r--   0        0        0     1120 2023-07-10 06:35:38.831225 psychoanalyze-0.6.3/psychoanalyze/analysis/ecdf.py
+-rw-r--r--   0        0        0     2302 2023-07-10 23:10:13.757714 psychoanalyze-0.6.3/psychoanalyze/analysis/strength_duration.py
+-rw-r--r--   0        0        0     2373 2023-07-10 06:35:32.351775 psychoanalyze-0.6.3/psychoanalyze/analysis/weber.py
+-rw-r--r--   0        0        0     1153 2023-07-15 09:38:33.343476 psychoanalyze-0.6.3/psychoanalyze/data/__init__.py
+-rw-r--r--   0        0        0     5715 2023-07-19 06:34:50.450027 psychoanalyze-0.6.3/psychoanalyze/data/blocks.py
+-rw-r--r--   0        0        0     7245 2023-07-19 04:42:14.885318 psychoanalyze-0.6.3/psychoanalyze/data/points.py
+-rw-r--r--   0        0        0     2868 2023-07-10 06:35:10.993442 psychoanalyze-0.6.3/psychoanalyze/data/sessions.py
+-rw-r--r--   0        0        0      841 2023-07-10 06:35:04.783422 psychoanalyze-0.6.3/psychoanalyze/data/stimulus.py
+-rw-r--r--   0        0        0     1678 2023-07-10 06:34:48.603492 psychoanalyze-0.6.3/psychoanalyze/data/subjects.py
+-rw-r--r--   0        0        0     5206 2023-07-14 06:02:28.786486 psychoanalyze-0.6.3/psychoanalyze/data/trials.py
+-rw-r--r--   0        0        0     3002 2023-07-16 02:29:21.297443 psychoanalyze-0.6.3/psychoanalyze/data/types.py
+-rw-r--r--   0        0        0     1589 2023-07-10 06:34:59.633459 psychoanalyze-0.6.3/psychoanalyze/plot.py
+-rw-r--r--   0        0        0     1518 2023-07-10 06:34:24.801696 psychoanalyze-0.6.3/psychoanalyze/sigmoids.py
+-rw-r--r--   0        0        0     1954 2023-07-19 07:08:51.735566 psychoanalyze-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     2804 1970-01-01 00:00:00.000000 psychoanalyze-0.6.3/PKG-INFO
```

### Comparing `psychoanalyze-0.6.2/LICENSE` & `psychoanalyze-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.6.2/README.md` & `psychoanalyze-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.6.2/psychoanalyze/__init__.py` & `psychoanalyze-0.6.3/psychoanalyze/__init__.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.6.2/psychoanalyze/analysis/__init__.py` & `psychoanalyze-0.6.3/psychoanalyze/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.6.2/psychoanalyze/analysis/bayes.py` & `psychoanalyze-0.6.3/psychoanalyze/analysis/bayes.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.6.2/psychoanalyze/analysis/ecdf.py` & `psychoanalyze-0.6.3/psychoanalyze/analysis/ecdf.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.6.2/psychoanalyze/analysis/strength_duration.py` & `psychoanalyze-0.6.3/psychoanalyze/analysis/strength_duration.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.6.2/psychoanalyze/analysis/weber.py` & `psychoanalyze-0.6.3/psychoanalyze/analysis/weber.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.6.2/psychoanalyze/data/__init__.py` & `psychoanalyze-0.6.3/psychoanalyze/data/__init__.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.6.2/psychoanalyze/data/blocks.py` & `psychoanalyze-0.6.3/psychoanalyze/data/blocks.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 """
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 import plotly.express as px
 import plotly.graph_objects as go
-from scipy.special import expit, logit
+from scipy.special import expit
 from scipy.stats import logistic as scipy_logistic
 from sklearn.linear_model import LogisticRegression
 
 from psychoanalyze.data import (
     points,
     sessions,
     stimulus,
@@ -112,45 +112,23 @@
     summary = (
         data.index.get_level_values("Subject").value_counts().rename("Total Blocks")
     )
     summary.index.name = "Subject"
     return summary
 
 
-def model_predictions(
-    intensity_choices: list[float],
-    k: float,
-    x_0: float = 0.0,
-) -> pd.Series:
-    """Calculate psi for array of x values. Possible duplicate."""
-    return pd.Series(
-        [1 / (1 + np.exp(-k * (x - x_0))) for x in intensity_choices],
-        index=intensity_choices,
-        name="Hit Rate",
-    )
-
-
-def make_predictions(fit: pd.Series, intensity_choices: list[float]) -> pd.Series:
-    """Get psi value for array of x values."""
-    return pd.Series(
-        fit.predict_proba(pd.DataFrame({"Intensity": intensity_choices}))[:, 1],
-        name="Hit Rate",
-        index=pd.Index(intensity_choices, name="Intensity"),
-    )
-
-
-def get_fit(trials: pd.DataFrame) -> pd.Series:
-    """Get parameter fits for given trial data."""
-    fit = LogisticRegression().fit(trials[["Intensity"]], trials["Result"])
-    return pd.Series(
-        {
-            "slope": fit.coef_[0][0],
-            "intercept": fit.intercept_[0],
-        },
-    )
+def fit(trials: pd.DataFrame) -> pd.Series:
+    """Fit logistic regression to trial data."""
+    fit = LogisticRegression().fit(
+        trials[["Intensity"]],
+        trials["Result"],
+    )
+    intercept = fit.intercept_[0]
+    slope = fit.coef_[0][0]
+    return pd.Series({"intercept": intercept, "slope": slope})
 
 
 def generate_trials(n_trials: int, model_params: dict[str, float]) -> pd.DataFrame:
     """Generate trials for block-level context."""
     return trials.moc_sample(n_trials, model_params)
 
 
@@ -194,30 +172,7 @@
         rows,  # row eg 'p[1]:p[8]'
         ["5%", "50%", "95%"],  # col
     ]
     param_fits = transform_errors(param_fits)
     param_fits = param_fits.rename(columns={"50%": y})
     param_fits.index = x
     return param_fits
-
-
-def logistic(params: dict[str, float]) -> pd.DataFrame:
-    """Generate logistic function from parameters."""
-    x = np.linspace(
-        scipy_logistic.ppf(0.01, loc=params["x_0"], scale=params["k"]),
-        scipy_logistic.ppf(0.99, loc=params["x_0"], scale=params["k"]),
-        100,
-    )
-    # ) * scipy_logistic.cdf(x, params["Threshold"], params["Slope"])
-    y = scipy_logistic.cdf(x, params["x_0"], params["k"])
-    index = pd.Index(x, name="Intensity")
-    logistic_points = pd.Series(
-        y,
-        index=index,
-        name="Hit Rate",
-    )
-    logit_hit_rate = pd.Series(
-        logit(logistic_points),
-        index=logistic_points.index,
-        name="logit(Hit Rate)",
-    )
-    return pd.concat([logistic_points, logit_hit_rate], axis=1)
```

### Comparing `psychoanalyze-0.6.2/psychoanalyze/data/points.py` & `psychoanalyze-0.6.3/psychoanalyze/data/points.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 import cmdstanpy as stan
 import numpy as np
 import pandas as pd
 import plotly.express as px
 from dash import dash_table
 from pandera import check_io, check_output
 from plotly import graph_objects as go
-from scipy.special import logit
+from scipy.special import expit, logit
 from scipy.stats import logistic
 
 from psychoanalyze.data import trials as pa_trials
 from psychoanalyze.data import types
 
 index_levels = ["Amp1", "Width1", "Freq1", "Dur1"]
 
@@ -190,27 +190,28 @@
     x: pd.Index,
     params: dict[str, float],
 ) -> pd.Series:
     """Calculate psi for an array of intensity levels x."""
     return pd.Series(
         params["gamma"]
         + (1 - params["gamma"] - params["lambda"])
-        / (1 + np.exp(-params["k"] * (x - params["x_0"]))),
+        * expit(params["x_0"] + params["k"] * x),
         index=x,
         name="p(x)",
     )
 
 
 def plot(points: pd.DataFrame, y: str) -> go.Figure:
     """Plot the psychometric function."""
     return px.scatter(
         points.reset_index(),
         x="Intensity",
         y=y,
         size="n",
+        color="Block",
         template="plotly_white",
     )
 
 
 def hit_rate(df: pd.DataFrame) -> pd.Series:
     """Calculate hit rate from hits and number of trials."""
     return pd.Series(df["Hits"] / df["n"], name="Hit Rate")
```

### Comparing `psychoanalyze-0.6.2/psychoanalyze/data/sessions.py` & `psychoanalyze-0.6.3/psychoanalyze/data/sessions.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.6.2/psychoanalyze/data/stimulus.py` & `psychoanalyze-0.6.3/psychoanalyze/data/stimulus.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.6.2/psychoanalyze/data/subjects.py` & `psychoanalyze-0.6.3/psychoanalyze/data/subjects.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.6.2/psychoanalyze/data/trials.py` & `psychoanalyze-0.6.3/psychoanalyze/data/trials.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.6.2/psychoanalyze/data/types.py` & `psychoanalyze-0.6.3/psychoanalyze/data/types.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.6.2/psychoanalyze/plot.py` & `psychoanalyze-0.6.3/psychoanalyze/plot.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.6.2/psychoanalyze/sigmoids.py` & `psychoanalyze-0.6.3/psychoanalyze/sigmoids.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.6.2/pyproject.toml` & `psychoanalyze-0.6.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "psychoanalyze"
-version = "0.6.2"
+version = "0.6.3"
 description = "A Pythonic analysis package for psychophysics data"
 authors = ["Ty Schlichenmeyer <t.schlic@wustl.edu>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "3.11.4"
@@ -33,14 +33,15 @@
 ruff = "^0.0.276"
 black = "^23.3.0"
 ipykernel = "^6.24.0"
 ipywidgets = "^8.0.7"
 kaleido = "0.2.1"
 pyarrow = "^12.0.1"
 types-pytz = "^2023.3.0.0"
+python-semantic-release = "^8.0.2"
 
 [tool.poetry.scripts]
 psychoanalyze = "psychoanalyze.__main__:main"
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `psychoanalyze-0.6.2/PKG-INFO` & `psychoanalyze-0.6.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychoanalyze
-Version: 0.6.2
+Version: 0.6.3
 Summary: A Pythonic analysis package for psychophysics data
 License: GPL-3.0-or-later
 Author: Ty Schlichenmeyer
 Author-email: t.schlic@wustl.edu
 Requires-Python: ==3.11.4
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
@@ -26,14 +26,15 @@
 Requires-Dist: numpy (>=1.25.0,<2.0.0)
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
 Requires-Dist: pandas-stubs (>=2.0.2.230605,<3.0.0.0)
 Requires-Dist: pandera[mypy] (>=0.15.1,<0.16.0)
 Requires-Dist: pyarrow (>=12.0.1,<13.0.0)
 Requires-Dist: pytest (>=7.3.2,<8.0.0)
 Requires-Dist: pytest-mock (>=3.11.1,<4.0.0)
+Requires-Dist: python-semantic-release (>=8.0.2,<9.0.0)
 Requires-Dist: ruff (>=0.0.276,<0.0.277)
 Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: statsmodels (>=0.14.0,<0.15.0)
 Requires-Dist: tuna (>=0.5.11,<0.6.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Requires-Dist: types-pytz (>=2023.3.0.0,<2024.0.0.0)
```

