# Comparing `tmp/chess-tuning-tools-0.9.3.tar.gz` & `tmp/chess_tuning_tools-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess-tuning-tools-0.9.3.tar", max compression
+gzip compressed data, was "chess_tuning_tools-0.9.4.tar", max compression
```

## Comparing `chess-tuning-tools-0.9.3.tar` & `chess_tuning_tools-0.9.4.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0      592 2022-04-02 11:41:21.645157 chess-tuning-tools-0.9.3/LICENSE
--rw-r--r--   0        0        0     2135 2022-04-02 11:41:21.645157 chess-tuning-tools-0.9.3/README.rst
--rw-r--r--   0        0        0     1929 2022-04-02 11:41:21.649157 chess-tuning-tools-0.9.3/pyproject.toml
--rw-r--r--   0        0        0     1056 2022-04-02 11:41:21.649157 chess-tuning-tools-0.9.3/tune/__init__.py
--rw-r--r--   0        0        0    18485 2022-04-02 11:41:21.653157 chess-tuning-tools-0.9.3/tune/cli.py
--rw-r--r--   0        0        0      124 2022-04-02 11:41:21.653157 chess-tuning-tools-0.9.3/tune/db_workers/__init__.py
--rw-r--r--   0        0        0      186 2022-04-02 11:41:21.653157 chess-tuning-tools-0.9.3/tune/db_workers/dbmodels/__init__.py
--rw-r--r--   0        0        0      180 2022-04-02 11:41:21.653157 chess-tuning-tools-0.9.3/tune/db_workers/dbmodels/base_model.py
--rw-r--r--   0        0        0     5907 2022-04-02 11:41:21.653157 chess-tuning-tools-0.9.3/tune/db_workers/dbmodels/models.py
--rw-r--r--   0        0        0    15804 2022-04-02 11:41:21.653157 chess-tuning-tools-0.9.3/tune/db_workers/tuning_client.py
--rw-r--r--   0        0        0    17494 2022-04-02 11:41:21.653157 chess-tuning-tools-0.9.3/tune/db_workers/tuning_server.py
--rw-r--r--   0        0        0     4021 2022-04-02 11:41:21.653157 chess-tuning-tools-0.9.3/tune/db_workers/utils.py
--rw-r--r--   0        0        0     8998 2022-04-02 11:41:21.653157 chess-tuning-tools-0.9.3/tune/io.py
--rw-r--r--   0        0        0    42643 2022-04-02 11:41:21.653157 chess-tuning-tools-0.9.3/tune/local.py
--rw-r--r--   0        0        0    27523 2022-04-02 11:41:21.653157 chess-tuning-tools-0.9.3/tune/plots.py
--rw-r--r--   0        0        0     4785 2022-04-02 11:41:21.653157 chess-tuning-tools-0.9.3/tune/priors.py
--rw-r--r--   0        0        0     2739 2022-04-02 11:41:21.653157 chess-tuning-tools-0.9.3/tune/summary.py
--rw-r--r--   0        0        0     5364 2022-04-02 11:41:21.653157 chess-tuning-tools-0.9.3/tune/utils.py
--rw-r--r--   0        0        0     3535 2022-04-02 11:51:44.008942 chess-tuning-tools-0.9.3/setup.py
--rw-r--r--   0        0        0     3973 2022-04-02 11:51:44.009593 chess-tuning-tools-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0      592 2023-07-19 11:34:31.348552 chess_tuning_tools-0.9.4/LICENSE
+-rw-r--r--   0        0        0     2135 2023-07-19 11:34:31.348552 chess_tuning_tools-0.9.4/README.rst
+-rw-r--r--   0        0        0     1858 2023-07-19 11:34:31.352552 chess_tuning_tools-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0     1056 2023-07-19 11:34:31.356552 chess_tuning_tools-0.9.4/tune/__init__.py
+-rw-r--r--   0        0        0    18500 2023-07-19 11:34:31.356552 chess_tuning_tools-0.9.4/tune/cli.py
+-rw-r--r--   0        0        0      124 2023-07-19 11:34:31.356552 chess_tuning_tools-0.9.4/tune/db_workers/__init__.py
+-rw-r--r--   0        0        0      186 2023-07-19 11:34:31.356552 chess_tuning_tools-0.9.4/tune/db_workers/dbmodels/__init__.py
+-rw-r--r--   0        0        0      180 2023-07-19 11:34:31.356552 chess_tuning_tools-0.9.4/tune/db_workers/dbmodels/base_model.py
+-rw-r--r--   0        0        0     5906 2023-07-19 11:34:31.356552 chess_tuning_tools-0.9.4/tune/db_workers/dbmodels/models.py
+-rw-r--r--   0        0        0    15852 2023-07-19 11:34:31.356552 chess_tuning_tools-0.9.4/tune/db_workers/tuning_client.py
+-rw-r--r--   0        0        0    17488 2023-07-19 11:34:31.356552 chess_tuning_tools-0.9.4/tune/db_workers/tuning_server.py
+-rw-r--r--   0        0        0     4019 2023-07-19 11:34:31.356552 chess_tuning_tools-0.9.4/tune/db_workers/utils.py
+-rw-r--r--   0        0        0     8997 2023-07-19 11:34:31.356552 chess_tuning_tools-0.9.4/tune/io.py
+-rw-r--r--   0        0        0    42654 2023-07-19 11:34:31.356552 chess_tuning_tools-0.9.4/tune/local.py
+-rw-r--r--   0        0        0    27559 2023-07-19 11:34:31.356552 chess_tuning_tools-0.9.4/tune/plots.py
+-rw-r--r--   0        0        0     4785 2023-07-19 11:34:31.356552 chess_tuning_tools-0.9.4/tune/priors.py
+-rw-r--r--   0        0        0     2739 2023-07-19 11:34:31.356552 chess_tuning_tools-0.9.4/tune/summary.py
+-rw-r--r--   0        0        0     5407 2023-07-19 11:34:31.356552 chess_tuning_tools-0.9.4/tune/utils.py
+-rw-r--r--   0        0        0     3726 1970-01-01 00:00:00.000000 chess_tuning_tools-0.9.4/PKG-INFO
```

### Comparing `chess-tuning-tools-0.9.3/LICENSE` & `chess_tuning_tools-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `chess-tuning-tools-0.9.3/README.rst` & `chess_tuning_tools-0.9.4/README.rst`

 * *Files identical despite different names*

### Comparing `chess-tuning-tools-0.9.3/pyproject.toml` & `chess_tuning_tools-0.9.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chess-tuning-tools"
-version = "0.9.3"
+version = "0.9.4"
 description = "A collection of tools for local and distributed tuning of chess engines."
 authors = ["Karlson Pfannschmidt <kiudee@mail.upb.de>"]
 license = "Apache-2.0"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Natural Language :: English"
@@ -14,24 +14,23 @@
 keywords = ["chess", "tuning", "optimization", "engine"]
 documentation = "https://chess-tuning-tools.readthedocs.io"
 packages = [
     {include = "tune"}
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
-bask = ">=0.9.3,<1.0.0"
-Click = ">=7.1.2,<=8.0.4"
-numpy = ">=1.19.1"
+python = "~3.8"
+bask = ">=0.9.3"
+Click = ">=7.1.2,"
+numpy = ">=1.19.1,<1.24"
 scipy = ">=1.5.2"
 scikit-optimize = "^0.8"
 atomicwrites = ">=1.4.0"
 scikit-learn = ">=0.22,<0.24"
 dill = ">=0.3.4"
-importlib_metadata = {version = ">=1.4", python = "~3.7"}
 joblib = {version = ">=0.16.0", optional = true}
 psycopg2 = {version = ">=2.8.5", optional = true}
 sqlalchemy = {version = ">=1.3.18", optional = true}
 pandas = {version = ">=1.1.0", optional = true}
 Sphinx = {version = ">=3", optional = true}
 sphinx-book-theme = {version = ">=0.0.35", optional = true}
 myst-nb = {version = ">=0.9", optional = true}
@@ -42,23 +41,23 @@
 
 [tool.poetry.dev-dependencies]
 pytest = ">=6.0.1,<8"
 pip = ">=21.1.2"
 wheel = ">=0.34.2,<0.37"
 flake8 = ">=3.8.3"
 Sphinx = ">=3"
-black = "^19.10b0"
+black = "~22"
 pre-commit = ">=2.6.0"
 isort = "^5.3.2"
 flake8-bugbear = ">=20.1.4"
 sphinx-book-theme = ">=0.0.35"
 myst-nb = ">=0.9"
 sphinx-autobuild = ">=0.7.1"
-nox = ">=2021.6.12"
-nox-poetry = ">=0.8.6"
+nox = ">=2023.4.22"
+nox-poetry = ">=1.0.3"
 mypy = ">=0.910"
 
 [tool.poetry.scripts]
 tune = "tune.cli:cli"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/kiudee/chess-tuning-tools/issues"
```

### Comparing `chess-tuning-tools-0.9.3/tune/__init__.py` & `chess_tuning_tools-0.9.4/tune/__init__.py`

 * *Files identical despite different names*

### Comparing `chess-tuning-tools-0.9.3/tune/cli.py` & `chess_tuning_tools-0.9.4/tune/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     logfile,
     terminate_after,
     run_only_once,
     skip_benchmark,
     clientconfig,
     dbconfig,
 ):
-    """ Run the client to generate games for distributed tuning.
+    """Run the client to generate games for distributed tuning.
 
     In order to connect to the database you need to provide a valid DBCONFIG
     json file. It contains the necessary parameters to connect to the database
     where it can fetch jobs and store results.
     """
     log_level = logging.DEBUG if verbose else logging.INFO
     logging.basicConfig(
@@ -414,15 +414,17 @@
         fast_resume=fast_resume,
         model_path=model_path,
         gp_initial_burnin=settings.get("gp_initial_burnin", gp_initial_burnin),
         gp_initial_samples=settings.get("gp_initial_samples", gp_initial_samples),
         gp_priors=gp_priors,
     )
     extra_points = load_points_to_evaluate(
-        space=opt.space, csv_file=evaluate_points, rounds=settings.get("rounds", 10),
+        space=opt.space,
+        csv_file=evaluate_points,
+        rounds=settings.get("rounds", 10),
     )
     root_logger.debug(
         f"Loaded {len(extra_points)} extra points to evaluate: {extra_points}"
     )
 
     # Main optimization loop:
     while True:
```

### Comparing `chess-tuning-tools-0.9.3/tune/db_workers/dbmodels/models.py` & `chess_tuning_tools-0.9.4/tune/db_workers/dbmodels/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,14 +146,13 @@
             return (
                 f"<Result (job_id={self.job_id}, tc_id={self.tc_id},"
                 f" ww={self.ww_count}, wd={self.wd_count},"
                 f" wl={self.wl_count}, dd={self.dd_count},"
                 f" dl={self.dl_count}, ll={self.ll_count})>"
             )
 
-
 except ImportError:
     SqlTune = None
     SqlJob = None
     SqlUCIParam = None
     SqlTimeControl = None
     SqlResult = None
```

### Comparing `chess-tuning-tools-0.9.3/tune/db_workers/tuning_client.py` & `chess_tuning_tools-0.9.4/tune/db_workers/tuning_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -356,15 +356,17 @@
                         )
                     else:
                         self.logger.debug(
                             f"Initial benchmark results: lc0: {self.lc0_benchmark} "
                             f"nps, sf: {self.sf_benchmark} nps"
                         )
                     time_control = self.adjust_time_control(
-                        orig_tc, float(job.engine1_nps), float(job.engine2_nps),
+                        orig_tc,
+                        float(job.engine1_nps),
+                        float(job.engine2_nps),
                     )
                     self.logger.debug(
                         f"Adjusted time control from {orig_tc} to {time_control}"
                     )
 
                 # 3. Run experiment (and block)
                 self.logger.info(f"Running match with time control\n{time_control}")
```

### Comparing `chess-tuning-tools-0.9.3/tune/db_workers/tuning_server.py` & `chess_tuning_tools-0.9.4/tune/db_workers/tuning_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,17 +181,17 @@
         self.tunecfg = self.experiment["tuner"]
         self.parameters = list(self.tunecfg["parameters"].keys())
         self.dimensions = self.parse_dimensions(self.tunecfg["parameters"])
         self.space = normalize_dimensions(self.dimensions)
         self.priors = self.parse_priors(self.tunecfg["priors"])
 
         self.kernel = ConstantKernel(
-            constant_value=self.tunecfg.get("variance_value", 0.1 ** 2),
+            constant_value=self.tunecfg.get("variance_value", 0.1**2),
             constant_value_bounds=tuple(
-                self.tunecfg.get("variance_bounds", (0.01 ** 2, 0.5 ** 2))
+                self.tunecfg.get("variance_bounds", (0.01**2, 0.5**2))
             ),
         ) * Matern(
             length_scale=self.tunecfg.get("length_scale_value", 0.3),
             length_scale_bounds=tuple(
                 self.tunecfg.get("length_scale_bounds", (0.2, 0.8))
             ),
             nu=2.5,
```

### Comparing `chess-tuning-tools-0.9.3/tune/db_workers/utils.py` & `chess_tuning_tools-0.9.4/tune/db_workers/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
 def penta_to_score(draw_rate, counts, prior_games=10, prior_elo=0):
     prior = prior_games * prior_from_drawrate(prior_elo, draw_rate)
     probabilities = (counts + prior) / (counts.sum() + prior.sum())
     s01 = score_in_01(probabilities)
     score = (
         np.sqrt(2)
         * (s01 - 0.5)
-        / (probabilities.dot(np.power(np.linspace(0, 2, 5), 2)) - 4 * s01 ** 2)
+        / (probabilities.dot(np.power(np.linspace(0, 2, 5), 2)) - 4 * s01**2)
     )
     return score
 
 
 def simple_penta_to_score(draw_rate, counts, prior_games=10, prior_elo=0):
     prior = prior_games * prior_from_drawrate(prior_elo, draw_rate)
     probabilities = (counts + prior) / (counts.sum() + prior.sum())
```

### Comparing `chess-tuning-tools-0.9.3/tune/io.py` & `chess_tuning_tools-0.9.4/tune/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
                     "or list.".format(param_str)
                 )
 
     return dict(zip(j.keys(), dimensions))
 
 
 def load_tuning_config(json_dict):
-    """ Load the provided tuning configuration and split it up.
+    """Load the provided tuning configuration and split it up.
 
     Parameters
     ----------
     json_dict : dict
         Dictionary containing the engines, their fixed parameters, the tunable
         parameter ranges and other settings used during tuning.
```

### Comparing `chess-tuning-tools-0.9.3/tune/local.py` & `chess_tuning_tools-0.9.4/tune/local.py`

 * *Files 0% similar despite different names*

```diff
@@ -526,15 +526,15 @@
 
 def print_results(
     optimizer: Optimizer,
     result_object: OptimizeResult,
     parameter_names: Sequence[str],
     confidence: float = 0.9,
 ) -> Tuple[np.ndarray, float, float]:
-    """ Log the current results of the optimizer.
+    """Log the current results of the optimizer.
 
     Parameters
     ----------
     optimizer : bask.Optimizer
         Fitted Optimizer object.
     result_object : scipy.optimize.OptimizeResult
         Result object containing the data and the last fitted model.
@@ -913,15 +913,17 @@
         if popen.stdout is not None:
             for line in iter(popen.stdout.readline, ""):
                 yield line
         else:
             raise ValueError("No stdout found.")
 
 
-def is_debug_log(cutechess_line: str,) -> bool:
+def is_debug_log(
+    cutechess_line: str,
+) -> bool:
     """Check if the provided cutechess log line is a debug mode line.
 
     Parameters
     ----------
     cutechess_line : str
         One line from a cutechess log.
 
@@ -931,15 +933,17 @@
         True, if the given line is a debug mode line, False otherwise.
     """
     if re.match(r"[0-9]+ [<>]", cutechess_line) is not None:
         return True
     return False
 
 
-def check_log_for_errors(cutechess_output: List[str],) -> None:
+def check_log_for_errors(
+    cutechess_output: List[str],
+) -> None:
     """Parse the log output produced by cutechess-cli and scan for important errors.
 
     Parameters
     ----------
     cutechess_output : list of str
         String containing the log output produced by cutechess-cli.
     """
```

### Comparing `chess-tuning-tools-0.9.3/tune/plots.py` & `chess_tuning_tools-0.9.4/tune/plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -523,15 +523,18 @@
     n_colors = len(colors)
     if fig is None:
         plt.style.use("dark_background")
         n_cols = int(np.floor(np.sqrt(n_parameters)))
         n_rows = int(np.ceil(n_parameters / n_cols))
         figsize = (n_cols * plot_width, aspect_ratio * plot_width * n_rows)
         fig, ax = plt.subplots(
-            figsize=figsize, nrows=n_rows, ncols=n_cols, sharex=True,
+            figsize=figsize,
+            nrows=n_rows,
+            ncols=n_cols,
+            sharex=True,
         )
 
         margin_left = 1.0
         margin_right = 0.1
         margin_bottom = 0.5
         margin_top = 0.4
         wspace = 1
```

### Comparing `chess-tuning-tools-0.9.3/tune/priors.py` & `chess_tuning_tools-0.9.4/tune/priors.py`

 * *Files identical despite different names*

### Comparing `chess-tuning-tools-0.9.3/tune/summary.py` & `chess_tuning_tools-0.9.4/tune/summary.py`

 * *Files identical despite different names*

### Comparing `chess-tuning-tools-0.9.3/tune/utils.py` & `chess_tuning_tools-0.9.4/tune/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "TimeControl",
     "TimeControlBag",
     "latest_iterations",
 ]
 
 
 def expected_ucb(res, n_random_starts=100, alpha=1.96, random_state=None):
-    """ Compute the expected (pessimistic) optimum of the optimization result.
+    """Compute the expected (pessimistic) optimum of the optimization result.
 
     This will compute `gp_mean + alpha * gp_se` and find the optimum of that function.
 
     Parameters
     ----------
     * `res`  [`OptimizeResult`, scipy object]:
         The optimization result returned by a `bask` minimizer.
@@ -66,23 +66,29 @@
 
 def parse_timecontrol(tc_string):
     if "+" in tc_string:
         return tuple([Decimal(x) for x in tc_string.split("+")])
     return (Decimal(tc_string),)
 
 
-TC = namedtuple("TimeControl", ["time", "increment"],)
+TC = namedtuple(
+    "TimeControl",
+    ["time", "increment"],
+)
 
 
 class TimeControl(TC):
     @classmethod
     def from_string(cls, tc_string):
         tc = parse_timecontrol(tc_string)
         inc = Decimal("0.0") if len(tc) == 1 else tc[1]
-        return cls(time=Decimal(tc[0]), increment=inc,)
+        return cls(
+            time=Decimal(tc[0]),
+            increment=inc,
+        )
 
     def __str__(self):
         if abs(self.increment) < 1e-10:
             return f"{self.time}"
         return f"{self.time}+{self.increment}"
```

### Comparing `chess-tuning-tools-0.9.3/PKG-INFO` & `chess_tuning_tools-0.9.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,40 @@
 Metadata-Version: 2.1
 Name: chess-tuning-tools
-Version: 0.9.3
+Version: 0.9.4
 Summary: A collection of tools for local and distributed tuning of chess engines.
 Home-page: https://github.com/kiudee/chess-tuning-tools
 License: Apache-2.0
 Keywords: chess,tuning,optimization,engine
 Author: Karlson Pfannschmidt
 Author-email: kiudee@mail.upb.de
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<3.9
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: dist
 Provides-Extra: docs
-Requires-Dist: Click (>=7.1.2,<=8.0.4)
-Requires-Dist: Sphinx (>=3); extra == "docs"
+Requires-Dist: Click (>=7.1.2)
+Requires-Dist: Sphinx (>=3) ; extra == "docs"
 Requires-Dist: atomicwrites (>=1.4.0)
-Requires-Dist: bask (>=0.9.3,<1.0.0)
+Requires-Dist: bask (>=0.9.3)
 Requires-Dist: dill (>=0.3.4)
-Requires-Dist: importlib_metadata (>=1.4); python_version >= "3.7" and python_version < "3.8"
-Requires-Dist: joblib (>=0.16.0); extra == "dist"
-Requires-Dist: myst-nb (>=0.9); extra == "docs"
-Requires-Dist: numpy (>=1.19.1)
-Requires-Dist: pandas (>=1.1.0); extra == "dist"
-Requires-Dist: psycopg2 (>=2.8.5); extra == "dist"
+Requires-Dist: joblib (>=0.16.0) ; extra == "dist"
+Requires-Dist: myst-nb (>=0.9) ; extra == "docs"
+Requires-Dist: numpy (>=1.19.1,<1.24)
+Requires-Dist: pandas (>=1.1.0) ; extra == "dist"
+Requires-Dist: psycopg2 (>=2.8.5) ; extra == "dist"
 Requires-Dist: scikit-learn (>=0.22,<0.24)
 Requires-Dist: scikit-optimize (>=0.8,<0.9)
 Requires-Dist: scipy (>=1.5.2)
-Requires-Dist: sphinx-book-theme (>=0.0.35); extra == "docs"
-Requires-Dist: sqlalchemy (>=1.3.18); extra == "dist"
+Requires-Dist: sphinx-book-theme (>=0.0.35) ; extra == "docs"
+Requires-Dist: sqlalchemy (>=1.3.18) ; extra == "dist"
 Project-URL: Bug Tracker, https://github.com/kiudee/chess-tuning-tools/issues
 Project-URL: Documentation, https://chess-tuning-tools.readthedocs.io
 Project-URL: Repository, https://github.com/kiudee/chess-tuning-tools
 Description-Content-Type: text/x-rst
 
 
 .. image:: https://raw.githubusercontent.com/kiudee/chess-tuning-tools/master/docs/_static/CTT-Plots.png
```

