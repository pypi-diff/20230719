# Comparing `tmp/deepof-0.5.0.tar.gz` & `tmp/deepof-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepof-0.5.0.tar", last modified: Tue Jul 18 15:13:31 2023, max compression
+gzip compressed data, was "deepof-0.5.1.tar", last modified: Wed Jul 19 13:52:20 2023, max compression
```

## Comparing `deepof-0.5.0.tar` & `deepof-0.5.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 lucas_miranda (1672059496) 75350028        0 2023-07-18 15:13:31.592716 deepof-0.5.0/
--rw-r--r--   0 lucas_miranda (1672059496) 75350028     1070 2022-08-29 09:41:22.000000 deepof-0.5.0/LICENSE
--rw-r--r--   0 lucas_miranda (1672059496) 75350028       77 2023-03-30 11:55:09.000000 deepof-0.5.0/MANIFEST.in
--rw-r--r--   0 lucas_miranda (1672059496) 75350028     9242 2023-07-18 15:13:31.588278 deepof-0.5.0/PKG-INFO
--rw-r--r--   0 lucas_miranda (1672059496) 75350028     8735 2023-07-18 14:36:16.000000 deepof-0.5.0/README.md
-drwxr-xr-x   0 lucas_miranda (1672059496) 75350028        0 2023-07-18 15:13:31.556982 deepof-0.5.0/deepof/
--rw-r--r--   0 lucas_miranda (1672059496) 75350028     6148 2023-03-09 17:44:01.000000 deepof-0.5.0/deepof/.DS_Store
--rw-r--r--   0 lucas_miranda (1672059496) 75350028       38 2022-08-29 09:41:22.000000 deepof-0.5.0/deepof/__init__.py
-drwxr-xr-x   0 lucas_miranda (1672059496) 75350028        0 2023-07-18 15:13:31.578890 deepof-0.5.0/deepof/__pycache__/
--rw-r--r--   0 lucas_miranda (1672059496) 75350028      104 2023-03-30 11:25:12.000000 deepof-0.5.0/deepof/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 lucas_miranda (1672059496) 75350028      153 2023-05-08 08:17:29.000000 deepof-0.5.0/deepof/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 lucas_miranda (1672059496) 75350028    23441 2023-07-18 14:18:37.000000 deepof-0.5.0/deepof/__pycache__/annotation_utils.cpython-39.pyc
--rw-r--r--   0 lucas_miranda (1672059496) 75350028    71735 2023-07-18 13:42:27.000000 deepof-0.5.0/deepof/__pycache__/data.cpython-39.pyc
--rw-r--r--   0 lucas_miranda (1672059496) 75350028     9319 2023-05-20 09:16:02.000000 deepof-0.5.0/deepof/__pycache__/deepof_train_embeddings.cpython-39.pyc
--rw-r--r--   0 lucas_miranda (1672059496) 75350028     8804 2023-04-26 16:06:24.000000 deepof-0.5.0/deepof/__pycache__/hypermodels.cpython-36.pyc
--rw-r--r--   0 lucas_miranda (1672059496) 75350028     6353 2023-05-08 08:17:38.000000 deepof-0.5.0/deepof/__pycache__/hypermodels.cpython-39.pyc
--rw-r--r--   0 lucas_miranda (1672059496) 75350028    14803 2023-04-26 16:06:24.000000 deepof-0.5.0/deepof/__pycache__/model_utils.cpython-36.pyc
--rw-r--r--   0 lucas_miranda (1672059496) 75350028    48088 2023-05-20 09:15:55.000000 deepof-0.5.0/deepof/__pycache__/model_utils.cpython-39.pyc
--rw-r--r--   0 lucas_miranda (1672059496) 75350028     9325 2023-04-26 16:06:24.000000 deepof-0.5.0/deepof/__pycache__/models.cpython-36.pyc
--rw-r--r--   0 lucas_miranda (1672059496) 75350028    49614 2023-05-15 14:00:18.000000 deepof-0.5.0/deepof/__pycache__/models.cpython-39.pyc
--rw-r--r--   0 lucas_miranda (1672059496) 75350028    26124 2023-03-30 11:25:12.000000 deepof-0.5.0/deepof/__pycache__/pose_utils.cpython-39.pyc
--rw-r--r--   0 lucas_miranda (1672059496) 75350028    39780 2023-07-18 13:48:24.000000 deepof-0.5.0/deepof/__pycache__/post_hoc.cpython-39.pyc
--rw-r--r--   0 lucas_miranda (1672059496) 75350028    26524 2023-03-30 11:25:12.000000 deepof-0.5.0/deepof/__pycache__/preprocess.cpython-36.pyc
--rw-r--r--   0 lucas_miranda (1672059496) 75350028    37167 2023-04-26 16:06:24.000000 deepof-0.5.0/deepof/__pycache__/utils.cpython-36.pyc
--rw-r--r--   0 lucas_miranda (1672059496) 75350028    50786 2023-07-17 16:40:48.000000 deepof-0.5.0/deepof/__pycache__/utils.cpython-39.pyc
--rw-r--r--   0 lucas_miranda (1672059496) 75350028     4586 2023-04-26 16:06:24.000000 deepof-0.5.0/deepof/__pycache__/visuals.cpython-36.pyc
--rw-r--r--   0 lucas_miranda (1672059496) 75350028    69714 2023-07-17 16:03:09.000000 deepof-0.5.0/deepof/__pycache__/visuals.cpython-39.pyc
--rw-r--r--   0 lucas_miranda (1672059496) 75350028    28990 2023-07-18 14:18:30.000000 deepof-0.5.0/deepof/annotation_utils.py
--rw-r--r--   0 lucas_miranda (1672059496) 75350028    97568 2023-07-18 13:42:26.000000 deepof-0.5.0/deepof/data.py
--rw-r--r--   0 lucas_miranda (1672059496) 75350028    15220 2023-05-20 00:53:20.000000 deepof-0.5.0/deepof/deepof_train_embeddings.py
--rw-r--r--   0 lucas_miranda (1672059496) 75350028     8274 2023-04-26 16:00:17.000000 deepof-0.5.0/deepof/hypermodels.py
--rw-r--r--   0 lucas_miranda (1672059496) 75350028    61556 2023-05-20 00:53:20.000000 deepof-0.5.0/deepof/model_utils.py
--rw-r--r--   0 lucas_miranda (1672059496) 75350028    78665 2023-05-15 09:53:25.000000 deepof-0.5.0/deepof/models.py
--rw-r--r--   0 lucas_miranda (1672059496) 75350028    49384 2023-07-18 13:48:06.000000 deepof-0.5.0/deepof/post_hoc.py
-drwxr-xr-x   0 lucas_miranda (1672059496) 75350028        0 2023-07-18 15:13:31.579985 deepof-0.5.0/deepof/trained_models/
--rw-r--r--   0 lucas_miranda (1672059496) 75350028        0 2022-08-29 09:41:22.000000 deepof-0.5.0/deepof/trained_models/.gitkeep
-drwxr-xr-x   0 lucas_miranda (1672059496) 75350028        0 2023-07-18 15:13:31.580192 deepof-0.5.0/deepof/trained_models/deepof_supervised/
--rw-r--r--   0 lucas_miranda (1672059496) 75350028 10139395 2023-03-30 11:55:02.000000 deepof-0.5.0/deepof/trained_models/deepof_supervised/deepof_supervised_huddle_estimator.pkl
--rw-r--r--   0 lucas_miranda (1672059496) 75350028    63431 2023-07-17 16:40:32.000000 deepof-0.5.0/deepof/utils.py
--rw-r--r--   0 lucas_miranda (1672059496) 75350028   100866 2023-07-05 11:18:17.000000 deepof-0.5.0/deepof/visuals.py
-drwxr-xr-x   0 lucas_miranda (1672059496) 75350028        0 2023-07-18 15:13:31.563598 deepof-0.5.0/deepof.egg-info/
--rw-r--r--   0 lucas_miranda (1672059496) 75350028     9242 2023-07-18 15:13:31.000000 deepof-0.5.0/deepof.egg-info/PKG-INFO
--rw-r--r--   0 lucas_miranda (1672059496) 75350028     1337 2023-07-18 15:13:31.000000 deepof-0.5.0/deepof.egg-info/SOURCES.txt
--rw-r--r--   0 lucas_miranda (1672059496) 75350028        1 2023-07-18 15:13:31.000000 deepof-0.5.0/deepof.egg-info/dependency_links.txt
--rw-r--r--   0 lucas_miranda (1672059496) 75350028      839 2023-07-18 15:13:31.000000 deepof-0.5.0/deepof.egg-info/requires.txt
--rw-r--r--   0 lucas_miranda (1672059496) 75350028        7 2023-07-18 15:13:31.000000 deepof-0.5.0/deepof.egg-info/top_level.txt
--rw-r--r--   0 lucas_miranda (1672059496) 75350028      949 2023-07-18 14:34:05.000000 deepof-0.5.0/requirements.txt
--rw-r--r--   0 lucas_miranda (1672059496) 75350028       38 2023-07-18 15:13:31.592763 deepof-0.5.0/setup.cfg
--rw-r--r--   0 lucas_miranda (1672059496) 75350028     1019 2023-07-18 14:31:43.000000 deepof-0.5.0/setup.py
+drwxr-xr-x   0 lucas_miranda (1672059496) 75350028        0 2023-07-19 13:52:20.940521 deepof-0.5.1/
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028     1070 2022-08-29 09:41:22.000000 deepof-0.5.1/LICENSE
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028       77 2023-03-30 11:55:09.000000 deepof-0.5.1/MANIFEST.in
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    10178 2023-07-19 13:52:20.940181 deepof-0.5.1/PKG-INFO
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028     9671 2023-07-19 08:27:52.000000 deepof-0.5.1/README.md
+drwxr-xr-x   0 lucas_miranda (1672059496) 75350028        0 2023-07-19 13:52:20.875550 deepof-0.5.1/deepof/
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028     6148 2023-03-09 17:44:01.000000 deepof-0.5.1/deepof/.DS_Store
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028       38 2022-08-29 09:41:22.000000 deepof-0.5.1/deepof/__init__.py
+drwxr-xr-x   0 lucas_miranda (1672059496) 75350028        0 2023-07-19 13:52:20.927480 deepof-0.5.1/deepof/__pycache__/
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028      104 2023-03-30 11:25:12.000000 deepof-0.5.1/deepof/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028      153 2023-05-08 08:17:29.000000 deepof-0.5.1/deepof/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    23815 2023-07-19 13:03:41.000000 deepof-0.5.1/deepof/__pycache__/annotation_utils.cpython-39.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    71870 2023-07-19 13:41:52.000000 deepof-0.5.1/deepof/__pycache__/data.cpython-39.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028     9319 2023-05-20 09:16:02.000000 deepof-0.5.1/deepof/__pycache__/deepof_train_embeddings.cpython-39.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028     8804 2023-04-26 16:06:24.000000 deepof-0.5.1/deepof/__pycache__/hypermodels.cpython-36.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028     6353 2023-05-08 08:17:38.000000 deepof-0.5.1/deepof/__pycache__/hypermodels.cpython-39.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    14803 2023-04-26 16:06:24.000000 deepof-0.5.1/deepof/__pycache__/model_utils.cpython-36.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    48088 2023-05-20 09:15:55.000000 deepof-0.5.1/deepof/__pycache__/model_utils.cpython-39.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028     9325 2023-04-26 16:06:24.000000 deepof-0.5.1/deepof/__pycache__/models.cpython-36.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    49614 2023-05-15 14:00:18.000000 deepof-0.5.1/deepof/__pycache__/models.cpython-39.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    26124 2023-03-30 11:25:12.000000 deepof-0.5.1/deepof/__pycache__/pose_utils.cpython-39.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    39780 2023-07-18 13:48:24.000000 deepof-0.5.1/deepof/__pycache__/post_hoc.cpython-39.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    26524 2023-03-30 11:25:12.000000 deepof-0.5.1/deepof/__pycache__/preprocess.cpython-36.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    37167 2023-04-26 16:06:24.000000 deepof-0.5.1/deepof/__pycache__/utils.cpython-36.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    50786 2023-07-17 16:40:48.000000 deepof-0.5.1/deepof/__pycache__/utils.cpython-39.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028     4586 2023-04-26 16:06:24.000000 deepof-0.5.1/deepof/__pycache__/visuals.cpython-36.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    69714 2023-07-17 16:03:09.000000 deepof-0.5.1/deepof/__pycache__/visuals.cpython-39.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    29130 2023-07-19 11:18:09.000000 deepof-0.5.1/deepof/annotation_utils.py
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    97765 2023-07-19 13:46:02.000000 deepof-0.5.1/deepof/data.py
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    15220 2023-05-20 00:53:20.000000 deepof-0.5.1/deepof/deepof_train_embeddings.py
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028     8274 2023-04-26 16:00:17.000000 deepof-0.5.1/deepof/hypermodels.py
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    61556 2023-05-20 00:53:20.000000 deepof-0.5.1/deepof/model_utils.py
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    78665 2023-05-15 09:53:25.000000 deepof-0.5.1/deepof/models.py
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    49384 2023-07-18 13:48:06.000000 deepof-0.5.1/deepof/post_hoc.py
+drwxr-xr-x   0 lucas_miranda (1672059496) 75350028        0 2023-07-19 13:52:20.928557 deepof-0.5.1/deepof/trained_models/
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028        0 2022-08-29 09:41:22.000000 deepof-0.5.1/deepof/trained_models/.gitkeep
+drwxr-xr-x   0 lucas_miranda (1672059496) 75350028        0 2023-07-19 13:52:20.928696 deepof-0.5.1/deepof/trained_models/deepof_supervised/
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028 10139395 2023-03-30 11:55:02.000000 deepof-0.5.1/deepof/trained_models/deepof_supervised/deepof_supervised_huddle_estimator.pkl
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    63431 2023-07-17 16:40:32.000000 deepof-0.5.1/deepof/utils.py
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028   100866 2023-07-05 11:18:17.000000 deepof-0.5.1/deepof/visuals.py
+drwxr-xr-x   0 lucas_miranda (1672059496) 75350028        0 2023-07-19 13:52:20.877950 deepof-0.5.1/deepof.egg-info/
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    10178 2023-07-19 13:52:20.000000 deepof-0.5.1/deepof.egg-info/PKG-INFO
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028     1337 2023-07-19 13:52:20.000000 deepof-0.5.1/deepof.egg-info/SOURCES.txt
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028        1 2023-07-19 13:52:20.000000 deepof-0.5.1/deepof.egg-info/dependency_links.txt
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028      839 2023-07-19 13:52:20.000000 deepof-0.5.1/deepof.egg-info/requires.txt
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028        7 2023-07-19 13:52:20.000000 deepof-0.5.1/deepof.egg-info/top_level.txt
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028      949 2023-07-18 14:34:05.000000 deepof-0.5.1/requirements.txt
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028       38 2023-07-19 13:52:20.940622 deepof-0.5.1/setup.cfg
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028     1019 2023-07-19 08:27:52.000000 deepof-0.5.1/setup.py
```

### Comparing `deepof-0.5.0/LICENSE` & `deepof-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deepof-0.5.0/PKG-INFO` & `deepof-0.5.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,12 @@
-Metadata-Version: 2.1
-Name: deepof
-Version: 0.5.0
-Summary: A suite for postprocessing time-series extracted from videos of freely moving rodents using DeepLabCut
-Home-page: https://gitlab.mpcdf.mpg.de/lucasmir/deepof/
-Author: Lucas Miranda
-Author-email: lucas_miranda@psych.mpg.de
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Requires-Python: >3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![Pipeline](https://gitlab.mpcdf.mpg.de/lucasmir/deepof/badges/master/pipeline.svg)](https://gitlab.mpcdf.mpg.de/lucasmir/deepof/-/pipelines)
 [![Coverage](https://gitlab.mpcdf.mpg.de/lucasmir/deepof/badges/master/coverage.svg)](https://coverage.readthedocs.io/en/coverage-5.3/)
 [![Documentation Status](https://readthedocs.org/projects/deepof/badge/?version=latest)](https://deepof.readthedocs.io/en/latest)
 [![CodeFactor](https://www.codefactor.io/repository/github/lucasmiranda42/deepof/badge)](https://www.codefactor.io/repository/github/lucasmiranda42/deepof)
-[![Version](https://img.shields.io/badge/release-v0.5.0-informational)](https://pypi.org/project/deepof/)
+[![Version](https://img.shields.io/badge/release-v0.5.1-informational)](https://pypi.org/project/deepof/)
 [![MLFPM](https://img.shields.io/badge/funding-MLFPM-informational)](https://mlfpm.eu/)
 [![Black](https://img.shields.io/badge/code%20style-black-black)](https://github.com/psf/black)
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.05394/status.svg)](https://doi.org/10.21105/joss.05394)
 
 <br>
 
 <div align="center">
@@ -155,14 +141,31 @@
     volume = {8},
     url = {https://joss.theoj.org/papers/10.21105/joss.05394},
     doi = {10.21105/JOSS.05394},
     issn = {2475-9066}
 }
 ```
 
+```bibtex
+@article{DeepOF:NCOMMS,
+  doi = {10.1038/s41467-023-40040-3},
+  url = {https://doi.org/10.1038/s41467-023-40040-3},
+  year = {2023},
+  month = jul,
+  publisher = {Springer Science and Business Media {LLC}},
+  volume = {14},
+  number = {1},
+  author = {Joeri Bordes and Lucas Miranda and Maya Reinhardt and Sowmya Narayan and Jakob Hartmann and Emily L. Newman and Lea Maria Brix and Lotte van Doeselaar and Clara Engelhardt and Larissa Dillmann and Shiladitya Mitra and Kerry J. Ressler and Benno P\"{u}tz and Felix Agakov and Bertram M\"{u}ller-Myhsok and Mathias V. Schmidt},
+  title = {Automatically annotated motion tracking identifies a distinct social behavioral profile following chronic social defeat stress},
+  journal = {Nature Communications}
+}
+```
+
+All data and code used to generate the results in the NCOMMS paper are available [here](https://datashare.mpcdf.mpg.de/s/3ETwBe1CKk09c9x) (password: *DeepOF2023*).
+
 ---
 ### Issues
 
 If you encounter any problems while using this package, please open an issue in the [issue tracker](https://github.com/mlfpm/deepof/issues).
 
 ---
 ### Contributions
```

### Comparing `deepof-0.5.0/README.md` & `deepof-0.5.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,26 @@
+Metadata-Version: 2.1
+Name: deepof
+Version: 0.5.1
+Summary: A suite for postprocessing time-series extracted from videos of freely moving rodents using DeepLabCut
+Home-page: https://gitlab.mpcdf.mpg.de/lucasmir/deepof/
+Author: Lucas Miranda
+Author-email: lucas_miranda@psych.mpg.de
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Requires-Python: >3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![Pipeline](https://gitlab.mpcdf.mpg.de/lucasmir/deepof/badges/master/pipeline.svg)](https://gitlab.mpcdf.mpg.de/lucasmir/deepof/-/pipelines)
 [![Coverage](https://gitlab.mpcdf.mpg.de/lucasmir/deepof/badges/master/coverage.svg)](https://coverage.readthedocs.io/en/coverage-5.3/)
 [![Documentation Status](https://readthedocs.org/projects/deepof/badge/?version=latest)](https://deepof.readthedocs.io/en/latest)
 [![CodeFactor](https://www.codefactor.io/repository/github/lucasmiranda42/deepof/badge)](https://www.codefactor.io/repository/github/lucasmiranda42/deepof)
-[![Version](https://img.shields.io/badge/release-v0.5.0-informational)](https://pypi.org/project/deepof/)
+[![Version](https://img.shields.io/badge/release-v0.5.1-informational)](https://pypi.org/project/deepof/)
 [![MLFPM](https://img.shields.io/badge/funding-MLFPM-informational)](https://mlfpm.eu/)
 [![Black](https://img.shields.io/badge/code%20style-black-black)](https://github.com/psf/black)
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.05394/status.svg)](https://doi.org/10.21105/joss.05394)
 
 <br>
 
 <div align="center">
@@ -141,14 +155,31 @@
     volume = {8},
     url = {https://joss.theoj.org/papers/10.21105/joss.05394},
     doi = {10.21105/JOSS.05394},
     issn = {2475-9066}
 }
 ```
 
+```bibtex
+@article{DeepOF:NCOMMS,
+  doi = {10.1038/s41467-023-40040-3},
+  url = {https://doi.org/10.1038/s41467-023-40040-3},
+  year = {2023},
+  month = jul,
+  publisher = {Springer Science and Business Media {LLC}},
+  volume = {14},
+  number = {1},
+  author = {Joeri Bordes and Lucas Miranda and Maya Reinhardt and Sowmya Narayan and Jakob Hartmann and Emily L. Newman and Lea Maria Brix and Lotte van Doeselaar and Clara Engelhardt and Larissa Dillmann and Shiladitya Mitra and Kerry J. Ressler and Benno P\"{u}tz and Felix Agakov and Bertram M\"{u}ller-Myhsok and Mathias V. Schmidt},
+  title = {Automatically annotated motion tracking identifies a distinct social behavioral profile following chronic social defeat stress},
+  journal = {Nature Communications}
+}
+```
+
+All data and code used to generate the results in the NCOMMS paper are available [here](https://datashare.mpcdf.mpg.de/s/3ETwBe1CKk09c9x) (password: *DeepOF2023*).
+
 ---
 ### Issues
 
 If you encounter any problems while using this package, please open an issue in the [issue tracker](https://github.com/mlfpm/deepof/issues).
 
 ---
 ### Contributions
```

### Comparing `deepof-0.5.0/deepof/.DS_Store` & `deepof-0.5.1/deepof/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepof-0.5.0/deepof/__pycache__/annotation_utils.cpython-39.pyc` & `deepof-0.5.1/deepof/__pycache__/annotation_utils.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Jul 18 14:18:30 2023 UTC, .py size: 28990 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 369f b664 3e71 0000  a.......6..d>q..
+00000000: 610d 0d0a 0000 0000 71c6 b764 ca71 0000  a.......q..d.q..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000c 0000 0040 0000 0073 7a02 0000 6400  .....@...sz...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 6d06 5a06 6d07 5a07 0100 6401  m.Z.m.Z.m.Z...d.
 00000060: 6404 6c08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0c 5a0c 0100 6401 6405 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
@@ -135,21 +135,21 @@
 00000860: 2863 6c6f 7365 5f73 696e 676c 655f 636f  (close_single_co
 00000870: 6e74 6163 742e 3c6c 6f63 616c 733e 2e3c  ntact.<locals>.<
 00000880: 6c69 7374 636f 6d70 3e72 0100 0000 2907  listcomp>r....).
 00000890: da0a 6973 696e 7374 616e 6365 da03 7374  ..isinstance..st
 000008a0: 7272 1c00 0000 721d 0000 0072 1e00 0000  rr....r....r....
 000008b0: da04 6c69 7374 da03 616e 7929 0772 1100  ..list..any).r..
 000008c0: 0000 7212 0000 0072 1300 0000 7214 0000  ..r....r....r...
-000008d0: 0072 1500 0000 7216 0000 00da 0d63 6c6f  .r....r......clo
+000008d0: 0072 1500 0000 7216 0000 005a 0d63 6c6f  .r....r....Z.clo
 000008e0: 7365 5f63 6f6e 7461 6374 7222 0000 0072  se_contactr"...r
 000008f0: 2100 0000 7223 0000 00da 1463 6c6f 7365  !...r#.....close
 00000900: 5f73 696e 676c 655f 636f 6e74 6163 7420  _single_contact 
 00000910: 0000 0073 1e00 0000 0016 0402 0a02 1e01  ...s............
 00000920: 02fe 0202 02fe 0604 0a01 0401 1204 02fc  ................
-00000930: 0406 02f9 060a 722a 0000 0046 290a 7211  ......r*...F).r.
+00000930: 0406 02f9 060a 7229 0000 0046 290a 7211  ......r)...F).r.
 00000940: 0000 00da 056c 6566 7431 da05 6c65 6674  .....left1..left
 00000950: 32da 0672 6967 6874 31da 0672 6967 6874  2..right1..right
 00000960: 3272 1400 0000 7215 0000 0072 1600 0000  2r....r....r....
 00000970: da03 7265 7672 1700 0000 6309 0000 0000  ..revr....c.....
 00000980: 0000 0000 0000 000a 0000 0005 0000 0043  ...............C
 00000990: 0000 0073 aa00 0000 7c08 7256 7400 6a01  ...s....|.rVt.j.
 000009a0: 6a02 7c00 7c03 1900 7c00 7c02 1900 1800  j.|.|...|.|.....
@@ -216,24 +216,24 @@
 00000d70: 2069 6620 7468 6520 6469 7374 616e 6365   if the distance
 00000d80: 2062 6574 7765 656e 2074 6865 2074 776f   between the two
 00000d90: 2073 7065 6369 6669 6564 2070 6f69 6e74   specified point
 00000da0: 7320 6973 206c 6573 7320 7468 616e 2074  s is less than t
 00000db0: 6f6c 2c20 4661 6c73 6520 6f74 6865 7277  ol, False otherw
 00000dc0: 6973 650a 0a20 2020 2072 1800 0000 7219  ise..    r....r.
 00000dd0: 0000 0072 1b00 0000 290a 7211 0000 0072  ...r....).r....r
-00000de0: 2b00 0000 722c 0000 0072 2d00 0000 722e  +...r,...r-...r.
+00000de0: 2a00 0000 722b 0000 0072 2c00 0000 722d  *...r+...r,...r-
 00000df0: 0000 0072 1400 0000 7215 0000 0072 1600  ...r....r....r..
-00000e00: 0000 722f 0000 00da 0e64 6f75 626c 655f  ..r/.....double_
+00000e00: 0000 722e 0000 005a 0e64 6f75 626c 655f  ..r....Z.double_
 00000e10: 636f 6e74 6163 7472 2200 0000 7222 0000  contactr"...r"..
 00000e20: 0072 2300 0000 da14 636c 6f73 655f 646f  .r#.....close_do
 00000e30: 7562 6c65 5f63 6f6e 7461 6374 4b00 0000  uble_contactK...
 00000e40: 7330 0000 0000 1c04 021e 0102 ff02 0202  s0..............
 00000e50: fe02 041e 0102 ff02 0202 fe02 fb06 0c1e  ................
 00000e60: 0102 ff02 0202 fe02 041e 0102 ff02 0202  ................
-00000e70: fe02 fb04 0a72 3100 0000 6303 0000 0000  .....r1...c.....
+00000e70: fe02 fb04 0a72 2f00 0000 6303 0000 0000  .....r/...c.....
 00000e80: 0000 0000 0000 0009 0000 0004 0000 0043  ...............C
 00000e90: 0000 0073 6800 0000 7c00 5c02 7d03 7d04  ...sh...|.\.}.}.
 00000ea0: 7c01 5c02 7d05 7d06 7c03 7400 a001 7c02  |.\.}.}.|.t...|.
 00000eb0: a101 7c05 7c03 1800 1400 1700 7400 a002  ..|.|.......t...
 00000ec0: 7c02 a101 7c06 7c04 1800 1400 1800 7d07  |...|.|.......}.
 00000ed0: 7c04 7400 a002 7c02 a101 7c05 7c03 1800  |.t...|...|.|...
 00000ee0: 1400 1700 7400 a001 7c02 a101 7c06 7c04  ....t...|...|.|.
@@ -246,15 +246,15 @@
 00000f50: 6572 2061 2070 6976 6f74 2e29 0372 1c00  er a pivot.).r..
 00000f60: 0000 da03 636f 73da 0373 696e 2909 da06  ....cos..sin)...
 00000f70: 6f72 6967 696e da05 706f 696e 74da 0361  origin..point..a
 00000f80: 6e67 da02 6f78 da02 6f79 da02 7078 da02  ng..ox..oy..px..
 00000f90: 7079 da02 7178 da02 7179 7222 0000 0072  py..qx..qyr"...r
 00000fa0: 2200 0000 7223 0000 00da 0672 6f74 6174  "...r#.....rotat
 00000fb0: 6580 0000 0073 0a00 0000 0002 0801 0802  e....s..........
-00000fc0: 2801 2801 723d 0000 00e7 0000 0000 0000  (.(.r=..........
+00000fc0: 2801 2801 723b 0000 00e7 0000 0000 0000  (.(.r;..........
 00000fd0: 0000 6306 0000 0000 0000 0000 0000 0008  ..c.............
 00000fe0: 0000 0006 0000 0043 0000 0073 6600 0000  .......C...sf...
 00000ff0: 7400 7c02 7c00 7c01 6602 7401 a002 7c04  t.|.|.|.f.t...|.
 00001000: a101 8303 5c02 7d00 7d01 7c00 7c02 6401  ....\.}.}.|.|.d.
 00001010: 1900 1800 6402 1300 7c03 6401 1900 7c05  ....d...|.d...|.
 00001020: 1700 6402 1300 1b00 7d06 7c01 7c02 6403  ..d.....}.|.|.d.
 00001030: 1900 1800 6402 1300 7c03 6403 1900 7c05  ....d...|.d...|.
@@ -269,23 +269,23 @@
 000010c0: 2061 7265 206f 7574 7369 6465 2074 6865   are outside the
 000010d0: 2065 6c6c 6970 7365 2064 656e 6f74 6564   ellipse denoted
 000010e0: 2062 7920 655f 6365 6e74 6572 2c20 655f   by e_center, e_
 000010f0: 6178 6573 2061 6e64 2065 5f61 6e67 6c65  axes and e_angle
 00001100: 2c20 7769 7468 2061 2063 6572 7461 696e  , with a certain
 00001110: 2074 6872 6573 686f 6c64 0a0a 2020 2020   threshold..    
 00001120: 7201 0000 00e9 0200 0000 7218 0000 0029  r.........r....)
-00001130: 0372 3d00 0000 721c 0000 00da 0772 6164  .r=...r......rad
+00001130: 0372 3b00 0000 721c 0000 00da 0772 6164  .r;...r......rad
 00001140: 6961 6e73 2908 da01 78da 0179 da08 655f  ians)...x..y..e_
 00001150: 6365 6e74 6572 da06 655f 6178 6573 da07  center..e_axes..
 00001160: 655f 616e 676c 65da 0974 6872 6573 686f  e_angle..thresho
-00001170: 6c64 da06 7465 726d 5f78 da06 7465 726d  ld..term_x..term
+00001170: 6c64 5a06 7465 726d 5f78 5a06 7465 726d  ldZ.term_xZ.term
 00001180: 5f79 7222 0000 0072 2200 0000 7223 0000  _yr"...r"...r#..
 00001190: 00da 0f6f 7574 7369 6465 5f65 6c6c 6970  ...outside_ellip
 000011a0: 7365 8a00 0000 7308 0000 0000 071a 0220  se....s........ 
-000011b0: 0120 0172 4900 0000 2907 da0a 6172 656e  . .rI...)...aren
+000011b0: 0120 0172 4500 0000 2907 da0a 6172 656e  . .rE...)...aren
 000011c0: 615f 7479 7065 da05 6172 656e 61da 0870  a_type..arena..p
 000011d0: 6f73 5f64 6963 7472 1400 0000 da04 6e6f  os_dictr......no
 000011e0: 7365 da0d 6365 6e74 6572 6564 5f64 6174  se..centered_dat
 000011f0: 6172 1700 0000 6306 0000 0000 0000 0000  ar....c.........
 00001200: 0000 000a 0000 0008 0000 0003 0000 0073  ...............s
 00001210: 9200 0000 7c02 7c04 1900 7d04 7c00 a000  ....|.|...}.|...
 00001220: 6401 a101 725e 7c05 7220 7401 a002 6402  d...r^|.r t...d.
@@ -335,53 +335,53 @@
 000014e0: 2063 6c69 6d62 696e 6720 286e 702e 6172   climbing (np.ar
 000014f0: 7261 7929 3a20 626f 6f6c 6561 6e20 6172  ray): boolean ar
 00001500: 7261 792e 2054 7275 6520 6966 2073 656c  ray. True if sel
 00001510: 6563 7465 6420 616e 696d 616c 2069 7320  ected animal is 
 00001520: 636c 696d 6269 6e67 2074 6865 2077 616c  climbing the wal
 00001530: 6c73 206f 6620 7468 6520 6172 656e 610a  ls of the arena.
 00001540: 0a20 2020 20da 0863 6972 6375 6c61 7272  .    ..circularr
-00001550: 3f00 0000 7201 0000 0072 1800 0000 7241  ?...r....r....rA
-00001560: 0000 0072 4200 0000 a906 7241 0000 0072  ...rB.....rA...r
-00001570: 4200 0000 7243 0000 0072 4400 0000 7245  B...rC...rD...rE
-00001580: 0000 0072 4600 0000 da07 706f 6c79 676f  ...rF.....polygo
+00001550: 3d00 0000 7201 0000 0072 1800 0000 723f  =...r....r....r?
+00001560: 0000 0072 4000 0000 a906 723f 0000 0072  ...r@.....r?...r
+00001570: 4000 0000 7241 0000 0072 4200 0000 7243  @...rA...rB...rC
+00001580: 0000 0072 4400 0000 da07 706f 6c79 676f  ...rD.....polygo
 00001590: 6e63 0100 0000 0000 0000 0000 0000 0200  nc..............
 000015a0: 0000 0600 0000 1300 0000 7326 0000 0067  ..........s&...g
 000015b0: 007c 005d 1e7d 0174 0088 0083 01a0 0188  .|.].}.t........
 000015c0: 01a1 01a0 0274 037c 0183 01a1 010c 0091  .....t.|........
 000015d0: 0271 0453 0072 2200 0000 a904 720a 0000  .q.S.r".....r...
 000015e0: 00da 0662 7566 6665 72da 0863 6f6e 7461  ...buffer..conta
 000015f0: 696e 7372 0900 0000 a902 721f 0000 00da  insr......r.....
-00001600: 016e a902 724b 0000 0072 1400 0000 7222  .n..rK...r....r"
+00001600: 016e a902 7247 0000 0072 1400 0000 7222  .n..rG...r....r"
 00001610: 0000 0072 2300 0000 7224 0000 00c0 0000  ...r#...r$......
 00001620: 00f3 0000 0000 7a1e 636c 696d 625f 7761  ......z.climb_wa
 00001630: 6c6c 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  ll.<locals>.<lis
 00001640: 7463 6f6d 703e 7a62 5375 7070 6f72 7465  tcomp>zbSupporte
 00001650: 6420 7661 6c75 6573 2066 6f72 2061 7265  d values for are
 00001660: 6e61 5f74 7970 6520 6172 6520 5b27 706f  na_type are ['po
 00001670: 6c79 676f 6e61 6c2d 6d61 6e75 616c 272c  lygonal-manual',
 00001680: 2027 6369 7263 756c 6172 2d6d 616e 7561   'circular-manua
 00001690: 6c27 2c20 2763 6972 6375 6c61 722d 6175  l', 'circular-au
 000016a0: 746f 6465 7465 6374 275d a907 da0a 7374  todetect']....st
 000016b0: 6172 7473 7769 7468 721c 0000 00da 057a  artswithr......z
-000016c0: 6572 6f73 da05 6172 7261 7972 4900 0000  eros..arrayrI...
+000016c0: 6572 6f73 da05 6172 7261 7972 4500 0000  eros..arrayrE...
 000016d0: da06 7661 6c75 6573 da13 4e6f 7449 6d70  ..values..NotImp
 000016e0: 6c65 6d65 6e74 6564 4572 726f 7229 0a72  lementedError).r
-000016f0: 4a00 0000 724b 0000 0072 4c00 0000 7214  J...rK...rL...r.
-00001700: 0000 0072 4d00 0000 724e 0000 00da 0663  ...rM...rN.....c
+000016f0: 4600 0000 7247 0000 0072 4800 0000 7214  F...rG...rH...r.
+00001700: 0000 0072 4900 0000 724a 0000 00da 0663  ...rI...rJ.....c
 00001710: 656e 7465 72da 0461 7865 73da 0561 6e67  enter..axes..ang
 00001720: 6c65 da08 636c 696d 6269 6e67 7222 0000  le..climbingr"..
-00001730: 0072 5700 0000 7223 0000 00da 0a63 6c69  .rW...r#.....cli
+00001730: 0072 5300 0000 7223 0000 00da 0a63 6c69  .rS...r#.....cli
 00001740: 6d62 5f77 616c 6c98 0000 0073 2a00 0000  mb_wall....s*...
 00001750: 0016 0802 0a01 1c01 0801 0801 0201 0601  ................
 00001760: 0601 0201 0201 0401 02fa 0809 0a02 0401  ................
-00001770: 14ff 0605 0201 02ff 0404 7263 0000 0072  ..........rc...r
-00001780: 4b00 0000 da00 290a da0c 7370 6565 645f  K.....)...speed_
-00001790: 6466 7261 6d65 724a 0000 0072 4b00 0000  dframerJ...rK...
-000017a0: 724c 0000 0072 1400 0000 da09 746f 6c5f  rL...r......tol_
-000017b0: 7370 6565 6472 4d00 0000 724e 0000 00da  speedrM...rN....
+00001770: 14ff 0605 0201 02ff 0404 725f 0000 0072  ..........r_...r
+00001780: 4700 0000 da00 290a da0c 7370 6565 645f  G.....)...speed_
+00001790: 6466 7261 6d65 7246 0000 0072 4700 0000  dframerF...rG...
+000017a0: 7248 0000 0072 1400 0000 da09 746f 6c5f  rH...r......tol_
+000017b0: 7370 6565 6472 4900 0000 724a 0000 00da  speedrI...rJ....
 000017c0: 0873 5f6f 626a 6563 74da 0961 6e69 6d61  .s_object..anima
 000017d0: 6c5f 6964 630a 0000 0000 0000 0000 0000  l_idc...........
 000017e0: 0012 0000 0008 0000 0003 0000 0073 0a01  .............s..
 000017f0: 0000 7c03 7c06 1900 6401 0200 7d06 7d0a  ..|.|...d...}.}.
 00001800: 7c09 6402 6b03 721e 7c09 6403 3700 7d09  |.d.k.r.|.d.7.}.
 00001810: 7c08 6404 6b02 72ea 7c01 a000 6405 a101  |.d.k.r.|...d...
 00001820: 729c 7c07 723e 7401 a002 6406 a101 6e0c  r.|.r>t...d...n.
@@ -455,52 +455,52 @@
 00001c60: 7572 6e73 3a0a 2020 2020 2020 2020 736e  urns:.        sn
 00001c70: 6966 6669 6e67 2028 6e70 2e61 7272 6179  iffing (np.array
 00001c80: 293a 2062 6f6f 6c65 616e 2061 7272 6179  ): boolean array
 00001c90: 2e20 5472 7565 2069 6620 7365 6c65 6374  . True if select
 00001ca0: 6564 2061 6e69 6d61 6c20 6973 2073 6e69  ed animal is sni
 00001cb0: 6666 696e 6720 7468 6520 7365 6c65 6374  ffing the select
 00001cc0: 6564 206f 626a 6563 740a 0a20 2020 2054  ed object..    T
-00001cd0: 7264 0000 00da 015f 724b 0000 0072 4f00  rd....._rK...rO.
-00001ce0: 0000 723f 0000 0072 0100 0000 7218 0000  ..r?...r....r...
-00001cf0: 0072 4100 0000 7242 0000 0072 5000 0000  .rA...rB...rP...
-00001d00: 7251 0000 0063 0100 0000 0000 0000 0000  rQ...c..........
+00001cd0: 7260 0000 00da 015f 7247 0000 0072 4b00  r`....._rG...rK.
+00001ce0: 0000 723d 0000 0072 0100 0000 7218 0000  ..r=...r....r...
+00001cf0: 0072 3f00 0000 7240 0000 0072 4c00 0000  .r?...r@...rL...
+00001d00: 724d 0000 0063 0100 0000 0000 0000 0000  rM...c..........
 00001d10: 0000 0200 0000 0600 0000 1300 0000 7328  ..............s(
 00001d20: 0000 0067 007c 005d 207d 0174 0088 0083  ...g.|.] }.t....
 00001d30: 01a0 0188 010b 00a1 01a0 0274 037c 0183  ...........t.|..
 00001d40: 01a1 010c 0091 0271 0453 0072 2200 0000  .......q.S.r"...
-00001d50: 7252 0000 0072 5500 0000 7257 0000 0072  rR...rU...rW...r
+00001d50: 724e 0000 0072 5100 0000 7253 0000 0072  rN...rQ...rS...r
 00001d60: 2200 0000 7223 0000 0072 2400 0000 0801  "...r#...r$.....
 00001d70: 0000 7304 0000 0006 0202 ff7a 2073 6e69  ..s........z sni
 00001d80: 6666 5f6f 626a 6563 742e 3c6c 6f63 616c  ff_object.<local
 00001d90: 733e 2e3c 6c69 7374 636f 6d70 3e63 0100  s>.<listcomp>c..
 00001da0: 0000 0000 0000 0000 0000 0200 0000 0600  ................
 00001db0: 0000 1300 0000 7326 0000 0067 007c 005d  ......s&...g.|.]
 00001dc0: 1e7d 0174 0088 0083 01a0 0188 01a1 01a0  .}.t............
 00001dd0: 0274 037c 0183 01a1 010c 0091 0271 0453  .t.|.........q.S
-00001de0: 0072 2200 0000 7252 0000 0072 5500 0000  .r"...rR...rU...
-00001df0: 7257 0000 0072 2200 0000 7223 0000 0072  rW...r"...r#...r
-00001e00: 2400 0000 0e01 0000 7258 0000 00da 0643  $.......rX.....C
-00001e10: 656e 7465 7272 5900 0000 2912 7265 0000  enterrY...).re..
-00001e20: 0072 4a00 0000 724b 0000 0072 4c00 0000  .rJ...rK...rL...
-00001e30: 7214 0000 0072 6600 0000 724d 0000 0072  r....rf...rM...r
-00001e40: 4e00 0000 7267 0000 0072 6800 0000 da06  N...rg...rh.....
-00001e50: 6e6f 7369 6e67 725f 0000 0072 6000 0000  nosingr_...r`...
-00001e60: 7261 0000 00da 0a6e 6f73 696e 675f 6d69  ra.....nosing_mi
-00001e70: 6eda 0a6e 6f73 696e 675f 6d61 78da 0573  n..nosing_max..s
+00001de0: 0072 2200 0000 724e 0000 0072 5100 0000  .r"...rN...rQ...
+00001df0: 7253 0000 0072 2200 0000 7223 0000 0072  rS...r"...r#...r
+00001e00: 2400 0000 0e01 0000 7254 0000 00da 0643  $.......rT.....C
+00001e10: 656e 7465 7272 5500 0000 2912 7261 0000  enterrU...).ra..
+00001e20: 0072 4600 0000 7247 0000 0072 4800 0000  .rF...rG...rH...
+00001e30: 7214 0000 0072 6200 0000 7249 0000 0072  r....rb...rI...r
+00001e40: 4a00 0000 7263 0000 0072 6400 0000 5a06  J...rc...rd...Z.
+00001e50: 6e6f 7369 6e67 725b 0000 0072 5c00 0000  nosingr[...r\...
+00001e60: 725d 0000 005a 0a6e 6f73 696e 675f 6d69  r]...Z.nosing_mi
+00001e70: 6e5a 0a6e 6f73 696e 675f 6d61 78da 0573  nZ.nosing_max..s
 00001e80: 7065 6564 da08 736e 6966 6669 6e67 7222  peed..sniffingr"
-00001e90: 0000 0072 5700 0000 7223 0000 00da 0c73  ...rW...r#.....s
+00001e90: 0000 0072 5300 0000 7223 0000 00da 0c73  ...rS...r#.....s
 00001ea0: 6e69 6666 5f6f 626a 6563 74cb 0000 0073  niff_object....s
 00001eb0: 4c00 0000 001e 0e02 0801 0802 0801 0a01  L...............
 00001ec0: 1c01 0801 0802 0201 0601 0601 0201 0201  ................
 00001ed0: 0401 04fa 0608 0201 0601 0601 0201 0201  ................
 00001ee0: 0401 02fa 0809 0a02 0401 0c02 04fe 04ff  ................
 00001ef0: 0406 0401 14ff 0405 0c03 0402 1001 0802  ................
-00001f00: 7270 0000 0029 04da 0858 5f68 7564 646c  rp...)...X_huddl
+00001f00: 7269 0000 0029 04da 0858 5f68 7564 646c  ri...)...X_huddl
 00001f10: 65da 1068 7564 646c 655f 6573 7469 6d61  e..huddle_estima
-00001f20: 746f 7272 6800 0000 7217 0000 0063 0300  torrh...r....c..
+00001f20: 746f 7272 6400 0000 7217 0000 0063 0300  torrd...r....c..
 00001f30: 0000 0000 0000 0000 0000 0600 0000 1c00  ................
 00001f40: 0000 4300 0000 7366 0100 0064 01a0 007c  ..C...sf...d...|
 00001f50: 027c 02a1 0264 02a0 007c 027c 02a1 0264  .|...d...|.|...d
 00001f60: 03a0 007c 027c 02a1 0264 04a0 007c 027c  ...|.|...d...|.|
 00001f70: 02a1 0264 05a0 007c 027c 02a1 0264 06a0  ...d...|.|...d..
 00001f80: 007c 027c 02a1 0264 07a0 007c 027c 02a1  .|.|...d...|.|..
 00001f90: 0264 08a0 007c 027c 02a1 0264 09a0 007c  .d...|.|...d...|
@@ -602,29 +602,29 @@
 00002590: 7219 0000 0029 0eda 0666 6f72 6d61 74da  r....)...format.
 000025a0: 084b 6579 4572 726f 72da 0877 6172 6e69  .KeyError..warni
 000025b0: 6e67 73da 0477 6172 6e72 1c00 0000 da04  ngs..warnr......
 000025c0: 6675 6c6c da05 7368 6170 65da 036e 616e  full..shape..nan
 000025d0: da05 6973 6e61 6eda 046d 6561 6eda 0770  ..isnan..mean..p
 000025e0: 7265 6469 6374 720b 0000 00da 0d66 6974  redictr......fit
 000025f0: 5f74 7261 6e73 666f 726d da0a 6e61 6e5f  _transform..nan_
-00002600: 746f 5f6e 756d 2906 7271 0000 0072 7200  to_num).rq...rr.
-00002610: 0000 7268 0000 00da 1172 6571 7569 7265  ..rh.....require
+00002600: 746f 5f6e 756d 2906 726a 0000 0072 6b00  to_num).rj...rk.
+00002610: 0000 7264 0000 005a 1172 6571 7569 7265  ..rd...Z.require
 00002620: 645f 6665 6174 7572 6573 da06 585f 6d61  d_features..X_ma
-00002630: 736b da08 795f 6875 6464 6c65 7222 0000  sk..y_huddler"..
+00002630: 736b 5a08 795f 6875 6464 6c65 7222 0000  skZ.y_huddler"..
 00002640: 0072 2200 0000 7223 0000 00da 0668 7564  .r"...r#.....hud
 00002650: 646c 651d 0100 0073 5000 0000 0012 0a01  dle....sP.......
 00002660: 0a01 0a01 0a01 0a01 0a01 0a01 0a01 0a01  ................
 00002670: 0a01 0a01 0801 0801 0801 0801 0801 0801  ................
 00002680: 0801 0801 0801 0801 0801 0801 0801 0801  ................
 00002690: 08e6 041c 0201 0c01 0e02 0401 02ff 0404  ................
-000026a0: 1a03 1601 0401 10ff 0403 0a01 7282 0000  ............r...
-000026b0: 0029 0572 6500 0000 da11 6c69 6b65 6c69  .).re.....likeli
-000026c0: 686f 6f64 5f64 6672 616d 6572 6600 0000  hood_dframerf...
+000026a0: 1a03 1601 0401 10ff 0403 0a01 7279 0000  ............ry..
+000026b0: 0029 0572 6100 0000 da11 6c69 6b65 6c69  .).ra.....likeli
+000026c0: 686f 6f64 5f64 6672 616d 6572 6200 0000  hood_dframerb...
 000026d0: da0e 746f 6c5f 6c69 6b65 6c69 686f 6f64  ..tol_likelihood
-000026e0: 7268 0000 0063 0500 0000 0000 0000 0000  rh...c..........
+000026e0: 7264 0000 0063 0500 0000 0000 0000 0000  rd...c..........
 000026f0: 0000 0900 0000 0400 0000 4300 0000 7358  ..........C...sX
 00002700: 0000 007c 0464 016b 0372 107c 0464 0237  ...|.d.k.r.|.d.7
 00002710: 007d 047c 007c 0464 0317 0019 007c 026b  .}.|.|.d.....|.k
 00002720: 007d 057c 007c 0464 0317 0019 007c 007c  .}.|.|.d.....|.|
 00002730: 0464 0417 0019 006b 007d 067c 017c 0464  .d.....k.}.|.|.d
 00002740: 0417 0019 007c 036b 047d 077c 057c 0740  .....|.k.}.|.|.@
 00002750: 007c 0640 007d 087c 0853 0029 0561 2602  .|.@.}.|.S.).a&.
@@ -658,24 +658,24 @@
 00002910: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
 00002920: 2020 206c 6f6f 6b61 726f 756e 6420 286e     lookaround (n
 00002930: 702e 6172 7261 7929 3a20 5472 7565 2069  p.array): True i
 00002940: 6620 7468 6520 616e 696d 616c 2069 7320  f the animal is 
 00002950: 7374 616e 6469 6e67 2073 7469 6c6c 2061  standing still a
 00002960: 6e64 206c 6f6f 6b69 6e67 2061 726f 756e  nd looking aroun
 00002970: 642c 2046 616c 7365 206f 7468 6572 7769  d, False otherwi
-00002980: 7365 0a0a 2020 2020 7264 0000 0072 6900  se..    rd...ri.
-00002990: 0000 726a 0000 00da 044e 6f73 6572 2200  ..rj.....Noser".
-000029a0: 0000 2909 7265 0000 0072 8300 0000 7266  ..).re...r....rf
-000029b0: 0000 0072 8400 0000 7268 0000 0072 6e00  ...r....rh...rn.
-000029c0: 0000 da0a 6e6f 7365 5f73 7065 6564 da0f  ....nose_speed..
+00002980: 7365 0a0a 2020 2020 7260 0000 0072 6500  se..    r`...re.
+00002990: 0000 7266 0000 00da 044e 6f73 6572 2200  ..rf.....Noser".
+000029a0: 0000 2909 7261 0000 0072 7a00 0000 7262  ..).ra...rz...rb
+000029b0: 0000 0072 7b00 0000 7264 0000 0072 6700  ...r{...rd...rg.
+000029c0: 0000 5a0a 6e6f 7365 5f73 7065 6564 da0f  ..Z.nose_speed..
 000029d0: 6e6f 7365 5f6c 696b 656c 6968 6f6f 64da  nose_likelihood.
 000029e0: 0a6c 6f6f 6b61 726f 756e 6472 2200 0000  .lookaroundr"...
 000029f0: 7222 0000 0072 2300 0000 da0b 6c6f 6f6b  r"...r#.....look
 00002a00: 5f61 726f 756e 645d 0100 0073 0e00 0000  _around]...s....
-00002a10: 0013 0801 0802 1001 1801 1002 0c02 7289  ..............r.
+00002a10: 0013 0801 0802 1001 1801 1002 0c02 727f  ..............r.
 00002a20: 0000 00e9 1400 0000 2907 da0f 6469 7374  ........)...dist
 00002a30: 616e 6365 5f64 6672 616d 65da 0f70 6f73  ance_dframe..pos
 00002a40: 6974 696f 6e5f 6466 7261 6d65 da08 666f  ition_dframe..fo
 00002a50: 6c6c 6f77 6572 da08 666f 6c6c 6f77 6564  llower..followed
 00002a60: da06 6672 616d 6573 7214 0000 0072 1700  ..framesr....r..
 00002a70: 0000 6306 0000 0000 0000 0000 0000 000a  ..c.............
 00002a80: 0000 0007 0000 0003 0000 0073 d200 0000  ...........s....
@@ -745,46 +745,46 @@
 00002e80: 6c73 6520 6f74 6865 7277 6973 650a 0a20  lse otherwise.. 
 00002e90: 2020 2063 0100 0000 0000 0000 0000 0000     c............
 00002ea0: 0200 0000 0600 0000 1300 0000 7320 0000  ............s ..
 00002eb0: 0069 007c 005d 187d 017c 0188 0188 0064  .i.|.].}.|.....d
 00002ec0: 0017 0019 00a0 007c 01a1 0193 0271 0453  .......|.....q.S
 00002ed0: 0029 01da 0a5f 5461 696c 5f62 6173 6529  .)..._Tail_base)
 00002ee0: 01da 0573 6869 6674 a902 721f 0000 00da  ...shift..r.....
-00002ef0: 0169 2902 728e 0000 0072 8c00 0000 7222  .i).r....r....r"
+00002ef0: 0169 2902 7284 0000 0072 8200 0000 7222  .i).r....r....r"
 00002f00: 0000 0072 2300 0000 da0a 3c64 6963 7463  ...r#.....<dictc
 00002f10: 6f6d 703e 9501 0000 7302 0000 0006 017a  omp>....s......z
 00002f20: 2266 6f6c 6c6f 7769 6e67 5f70 6174 682e  "following_path.
 00002f30: 3c6c 6f63 616c 733e 2e3c 6469 6374 636f  <locals>.<dictco
 00002f40: 6d70 3e63 0100 0000 0000 0000 0000 0000  mp>c............
 00002f50: 0200 0000 0700 0000 1300 0000 732e 0000  ............s...
 00002f60: 0069 007c 005d 267d 017c 0174 006a 016a  .i.|.]&}.|.t.j.j
 00002f70: 0288 0188 0064 0017 0019 0088 027c 0119  .....d.......|..
 00002f80: 0018 0064 0164 028d 0293 0271 0453 0029  ...d.d.....q.S.)
 00002f90: 03da 055f 4e6f 7365 7218 0000 0072 1900  ..._Noser....r..
-00002fa0: 0000 721b 0000 0072 9200 0000 2903 728d  ..r....r....).r.
-00002fb0: 0000 0072 8c00 0000 da0a 7368 6966 745f  ...r......shift_
-00002fc0: 6469 6374 7222 0000 0072 2300 0000 7294  dictr"...r#...r.
+00002fa0: 0000 721b 0000 0072 8800 0000 2903 7283  ..r....r....).r.
+00002fb0: 0000 0072 8200 0000 da0a 7368 6966 745f  ...r......shift_
+00002fc0: 6469 6374 7222 0000 0072 2300 0000 728a  dictr"...r#...r.
 00002fd0: 0000 0099 0100 0073 0800 0000 0604 02fd  .......s........
-00002fe0: 0801 14ff 7295 0000 0072 9000 0000 7218  ....r....r....r.
+00002fe0: 0801 14ff 728b 0000 0072 8600 0000 7218  ....r....r....r.
 00002ff0: 0000 0072 1900 0000 7201 0000 0029 09da  ...r....r....)..
 00003000: 0572 616e 6765 da02 7064 da09 4461 7461  .range..pd..Data
 00003010: 4672 616d 65da 0574 7570 6c65 da06 736f  Frame..tuple..so
-00003020: 7274 6564 721c 0000 00da 0361 6c6c 725c  rtedr......allr\
-00003030: 0000 00da 036d 696e 290a 728b 0000 0072  .....min).r....r
-00003040: 8c00 0000 728d 0000 0072 8e00 0000 728f  ....r....r....r.
-00003050: 0000 0072 1400 0000 da07 6469 7374 5f64  ...r......dist_d
-00003060: 66da 0d72 6967 6874 5f6f 7269 656e 7431  f..right_orient1
-00003070: da0d 7269 6768 745f 6f72 6965 6e74 32da  ..right_orient2.
-00003080: 0666 6f6c 6c6f 7772 2200 0000 2904 728e  .followr"...).r.
-00003090: 0000 0072 8d00 0000 728c 0000 0072 9600  ...r....r....r..
+00003020: 7274 6564 721c 0000 00da 0361 6c6c 7258  rtedr......allrX
+00003030: 0000 00da 036d 696e 290a 7281 0000 0072  .....min).r....r
+00003040: 8200 0000 7283 0000 0072 8400 0000 7285  ....r....r....r.
+00003050: 0000 0072 1400 0000 5a07 6469 7374 5f64  ...r....Z.dist_d
+00003060: 665a 0d72 6967 6874 5f6f 7269 656e 7431  fZ.right_orient1
+00003070: 5a0d 7269 6768 745f 6f72 6965 6e74 32da  Z.right_orient2.
+00003080: 0666 6f6c 6c6f 7772 2200 0000 2904 7284  .followr"...).r.
+00003090: 0000 0072 8300 0000 7282 0000 0072 8c00  ...r....r....r..
 000030a0: 0000 7223 0000 00da 0e66 6f6c 6c6f 7769  ..r#.....followi
 000030b0: 6e67 5f70 6174 687c 0100 0073 2c00 0000  ng_path|...s,...
 000030c0: 0019 0c01 06ff 0603 0401 0e04 06fc 04ff  ................
 000030d0: 040b 1a01 0201 16ff 02ff 02ff 0208 1a01  ................
-000030e0: 1aff 02ff 0206 0401 1cff 0604 72a2 0000  ............r...
+000030e0: 1aff 02ff 0206 0401 1cff 0604 7295 0000  ............r...
 000030f0: 00e9 0a00 0000 2904 da10 6265 6861 7669  ......)...behavi
 00003100: 6f75 725f 6466 7261 6d65 da0b 7769 6e64  our_dframe..wind
 00003110: 6f77 5f73 697a 65da 0773 7465 7070 6564  ow_size..stepped
 00003120: 7217 0000 0063 0300 0000 0000 0000 0000  r....c..........
 00003130: 0000 0600 0000 0400 0000 4300 0000 7366  ..........C...sf
 00003140: 0000 0064 0164 0284 007c 006a 0044 0083  ...d.d...|.j.D..
 00003150: 017d 037c 006a 017c 0364 0364 048d 02a0  .}.|.j.|.d.d....
@@ -825,32 +825,32 @@
 00003380: 2062 6568 6176 696f 7572 2070 6572 2069   behaviour per i
 00003390: 6e73 7461 6e63 6520 6f66 2074 6865 2073  nstance of the s
 000033a0: 6c69 6469 6e67 2077 696e 646f 770a 0a20  liding window.. 
 000033b0: 2020 2063 0100 0000 0000 0000 0000 0000     c............
 000033c0: 0200 0000 0500 0000 5300 0000 731c 0000  ........S...s...
 000033d0: 0067 007c 005d 147d 0164 007c 01a0 00a1  .g.|.].}.d.|....
 000033e0: 0076 0072 047c 0191 0271 0453 0029 0172  .v.r.|...q.S.).r
-000033f0: 6e00 0000 2901 da05 6c6f 7765 7229 0272  n...)...lower).r
+000033f0: 6700 0000 2901 da05 6c6f 7765 72a9 0272  g...)...lower..r
 00003400: 1f00 0000 da03 636f 6c72 2200 0000 7222  ......colr"...r"
 00003410: 0000 0072 2300 0000 7224 0000 00c4 0100  ...r#...r$......
-00003420: 0072 5800 0000 7a21 6d61 785f 6265 6861  .rX...z!max_beha
+00003420: 0072 5400 0000 7a21 6d61 785f 6265 6861  .rT...z!max_beha
 00003430: 7669 6f75 722e 3c6c 6f63 616c 733e 2e3c  viour.<locals>.<
 00003440: 6c69 7374 636f 6d70 3e72 1800 0000 7219  listcomp>r....r.
-00003450: 0000 0054 2901 725f 0000 004e 2909 da07  ...T).r_...N)...
+00003450: 0000 0054 2901 725b 0000 004e 2909 da07  ...T).r[...N)...
 00003460: 636f 6c75 6d6e 73da 0464 726f 70da 0661  columns..drop..a
 00003470: 7374 7970 65da 0566 6c6f 6174 da07 726f  stype..float..ro
 00003480: 6c6c 696e 67da 0373 756d da06 6964 786d  lling..sum..idxm
-00003490: 6178 721c 0000 0072 5c00 0000 2906 72a4  axr....r\...).r.
-000034a0: 0000 0072 a500 0000 72a6 0000 00da 0673  ...r....r......s
-000034b0: 7065 6564 73da 0977 696e 5f61 7272 6179  peeds..win_array
-000034c0: da09 6d61 785f 6172 7261 7972 2200 0000  ..max_arrayr"...
+00003490: 6178 721c 0000 0072 5800 0000 2906 7297  axr....rX...).r.
+000034a0: 0000 0072 9800 0000 7299 0000 00da 0673  ...r....r......s
+000034b0: 7065 6564 735a 0977 696e 5f61 7272 6179  peedsZ.win_array
+000034c0: 5a09 6d61 785f 6172 7261 7972 2200 0000  Z.max_arrayr"...
 000034d0: 7222 0000 0072 2300 0000 da0d 6d61 785f  r"...r#.....max_
 000034e0: 6265 6861 7669 6f75 72b6 0100 0073 0e00  behaviour....s..
 000034f0: 0000 000e 1002 1401 1201 0401 0e01 1402  ................
-00003500: 72b3 0000 0029 02da 0768 7061 7261 6d73  r....)...hparams
+00003500: 72a5 0000 0029 02da 0768 7061 7261 6d73  r....)...hparams
 00003510: 7217 0000 0063 0100 0000 0000 0000 0000  r....c..........
 00003520: 0000 0400 0000 0900 0000 4300 0000 7334  ..........C...s4
 00003530: 0000 0064 0164 0264 0364 0464 0264 0164  ...d.d.d.d.d.d.d
 00003540: 0564 0664 079c 087d 017c 00a0 00a1 0044  .d.d...}.|.....D
 00003550: 005d 105c 027d 027d 037c 037c 017c 023c  .].\.}.}.|.|.|.<
 00003560: 0071 1e7c 0153 0029 0861 2d01 0000 5265  .q.|.S.).a-...Re
 00003570: 7475 726e 2074 6865 206d 6f73 7420 6672  turn the most fr
@@ -868,29 +868,29 @@
 00003630: 2064 6963 7469 6f6e 6172 7920 7769 7468   dictionary with
 00003640: 206f 7665 7277 7269 7474 656e 2070 6172   overwritten par
 00003650: 616d 6574 6572 732e 2054 686f 7365 206e  ameters. Those n
 00003660: 6f74 2073 7065 6369 6669 6564 2069 6e20  ot specified in 
 00003670: 7468 6520 696e 7075 7420 7265 7461 696e  the input retain
 00003680: 2074 6865 6972 2064 6566 6175 6c74 2076   their default v
 00003690: 616c 7565 730a 0a20 2020 20e9 0500 0000  alues..    .....
-000036a0: 72a3 0000 00e9 1900 0000 e92d 0000 0072  r..........-...r
-000036b0: 3f00 0000 6733 3333 3333 33eb 3f29 08da  ?...g333333.?)..
+000036a0: 7296 0000 00e9 1900 0000 e92d 0000 0072  r..........-...r
+000036b0: 3d00 0000 6733 3333 3333 33eb 3f29 085a  =...g333333.?).Z
 000036c0: 0b73 7065 6564 5f70 6175 7365 da09 636c  .speed_pause..cl
 000036d0: 696d 625f 746f 6cda 1163 6c6f 7365 5f63  imb_tol..close_c
 000036e0: 6f6e 7461 6374 5f74 6f6c da10 7369 6465  ontact_tol..side
 000036f0: 5f63 6f6e 7461 6374 5f74 6f6c da0d 666f  _contact_tol..fo
 00003700: 6c6c 6f77 5f66 7261 6d65 73da 0a66 6f6c  llow_frames..fol
 00003710: 6c6f 775f 746f 6cda 0c68 7564 646c 655f  low_tol..huddle_
-00003720: 7370 6565 6472 8700 0000 2901 da05 6974  speedr....)...it
-00003730: 656d 7329 0472 b400 0000 da08 6465 6661  ems).r......defa
+00003720: 7370 6565 6472 7d00 0000 2901 da05 6974  speedr}...)...it
+00003730: 656d 7329 0472 a600 0000 da08 6465 6661  ems).r......defa
 00003740: 756c 7473 da01 6bda 0176 7222 0000 0072  ults..k..vr"...r
 00003750: 2200 0000 7223 0000 00da 0f67 6574 5f68  "...r#.....get_h
 00003760: 7061 7261 6d65 7465 7273 d001 0000 7318  parameters....s.
 00003770: 0000 0000 0b02 0102 0102 0102 0102 0102  ................
-00003780: 0102 0102 f806 0b10 010a 0272 c300 0000  ...........r....
+00003780: 0102 0102 f806 0b10 010a 0272 b400 0000  ...........r....
 00003790: 2901 da07 636f 726e 6572 7363 0300 0000  )...cornersc....
 000037a0: 0000 0000 0000 0000 0600 0000 0700 0000  ................
 000037b0: 4300 0000 738c 0000 0074 007c 0064 0114  C...s....t.|.d..
 000037c0: 0064 021b 0083 0174 007c 0164 031b 0083  .d.....t.|.d....
 000037d0: 0166 0274 007c 0064 0414 0064 021b 0083  .f.t.|.d...d....
 000037e0: 0174 007c 0164 031b 0083 0166 0274 007c  .t.|.d.....f.t.|
 000037f0: 0064 0114 0064 021b 0083 0174 007c 0164  .d...d.....t.|.d
@@ -919,28 +919,28 @@
 00003960: 6469 6374 696f 6e61 7279 2077 6974 6820  dictionary with 
 00003970: 6f76 6572 7772 6974 656e 2070 6172 616d  overwriten param
 00003980: 6574 6572 732e 2054 686f 7365 206e 6f74  eters. Those not
 00003990: 2073 7065 6369 6669 6564 2069 6e20 7468   specified in th
 000039a0: 6520 696e 7075 7420 7265 7461 696e 2074  e input retain t
 000039b0: 6865 6972 2064 6566 6175 6c74 2076 616c  heir default val
 000039c0: 7565 730a 0a20 2020 2067 3333 3333 3333  ues..    g333333
-000039d0: d33f 72a3 0000 0067 cdcc cccc cccc f03f  .?r....g.......?
-000039e0: 6700 0000 0000 001a 4072 8a00 0000 6733  g.......@r....g3
-000039f0: 3333 3333 3319 4029 04da 0864 6f77 6e6c  33333.@)...downl
-00003a00: 6566 74da 0964 6f77 6e72 6967 6874 da06  eft..downright..
-00003a10: 7570 6c65 6674 da07 7570 7269 6768 7429  upleft..upright)
-00003a20: 02da 0369 6e74 72bf 0000 0029 06da 0177  ...intr....)...w
-00003a30: da01 6872 c400 0000 72c0 0000 0072 c100  ..hr....r....r..
-00003a40: 0000 72c2 0000 0072 2200 0000 7222 0000  ..r....r"...r"..
+000039d0: d33f 7296 0000 0067 cdcc cccc cccc f03f  .?r....g.......?
+000039e0: 6700 0000 0000 001a 4072 8000 0000 6733  g.......@r....g3
+000039f0: 3333 3333 3319 4029 045a 0864 6f77 6e6c  33333.@).Z.downl
+00003a00: 6566 745a 0964 6f77 6e72 6967 6874 5a06  eftZ.downrightZ.
+00003a10: 7570 6c65 6674 5a07 7570 7269 6768 7429  upleftZ.upright)
+00003a20: 02da 0369 6e74 72b0 0000 0029 06da 0177  ...intr....)...w
+00003a30: da01 6872 b500 0000 72b1 0000 0072 b200  ..hr....r....r..
+00003a40: 0000 72b3 0000 0072 2200 0000 7222 0000  ..r....r"...r"..
 00003a50: 0072 2300 0000 da0d 6672 616d 655f 636f  .r#.....frame_co
 00003a60: 726e 6572 73ec 0100 0073 1000 0000 000d  rners....s......
-00003a70: 1a01 1a01 1a01 1afc 0607 1001 0a02 72cc  ..............r.
+00003a70: 1a01 1a01 1a01 1afc 0607 1001 0a02 72b9  ..............r.
 00003a80: 0000 0029 0ada 0c63 6f6f 7264 5f6f 626a  ...)...coord_obj
 00003a90: 6563 74da 0a72 6177 5f63 6f6f 7264 73da  ect..raw_coords.
-00003aa0: 0663 6f6f 7264 73da 0564 6973 7473 72b0  .coords..distsr.
+00003aa0: 0663 6f6f 7264 73da 0564 6973 7473 72a4  .coords..distsr.
 00003ab0: 0000 00da 0d66 756c 6c5f 6665 6174 7572  .....full_featur
 00003ac0: 6573 da05 7669 6465 6fda 1274 7261 696e  es..video..train
 00003ad0: 6564 5f6d 6f64 656c 5f70 6174 68da 0670  ed_model_path..p
 00003ae0: 6172 616d 7372 1700 0000 6309 0000 0000  aramsr....c.....
 00003af0: 0000 0000 0000 001a 0000 000e 0000 0003  ................
 00003b00: 0000 0073 7204 0000 7400 7401 6a02 a003  ...sr...t.t.j...
 00003b10: 7c07 6401 6402 a103 6403 8302 8f1a 7d09  |.d.d...d.....}.
@@ -1081,386 +1081,409 @@
 00004380: 616d 6529 3a20 7461 626c 6520 7769 7468  ame): table with
 00004390: 2074 7261 6974 7320 6173 2063 6f6c 756d   traits as colum
 000043a0: 6e73 2061 6e64 2066 7261 6d65 7320 6173  ns and frames as
 000043b0: 2072 6f77 732e 2045 6163 6820 7661 6c75   rows. Each valu
 000043c0: 6520 6973 2061 2062 6f6f 6c65 616e 2069  e is a boolean i
 000043d0: 6e64 6963 6174 696e 6720 7472 6169 7420  ndicating trait 
 000043e0: 6465 7465 6374 696f 6e20 6174 2061 2067  detection at a g
-000043f0: 6976 656e 2074 696d 650a 0a20 2020 20da  iven time..    .
+000043f0: 6976 656e 2074 696d 650a 0a20 2020 205a  iven time..    Z
 00004400: 1164 6565 706f 665f 7375 7065 7276 6973  .deepof_supervis
 00004410: 6564 7a26 6465 6570 6f66 5f73 7570 6572  edz&deepof_super
 00004420: 7669 7365 645f 6875 6464 6c65 5f65 7374  vised_huddle_est
 00004430: 696d 6174 6f72 2e70 6b6c da02 7262 4e72  imator.pkl..rbNr
-00004440: 1800 0000 7269 0000 0072 6400 0000 7a08  ....ri...rd...z.
+00004440: 1800 0000 7265 0000 0072 6000 0000 7a08  ....re...r`...z.
 00004450: 282e 2a3f 2944 4c43 7201 0000 0054 2901  (.*?)DLCr....T).
-00004460: 72aa 0000 00e9 ffff ffff e9fe ffff ff29  r..............)
+00004460: 729e 0000 00e9 ffff ffff e9fe ffff ff29  r..............)
 00004470: 09da 084c 6566 745f 6561 72da 0952 6967  ...Left_ear..Rig
 00004480: 6874 5f65 6172 da07 5370 696e 655f 3172  ht_ear..Spine_1r
-00004490: 6a00 0000 da07 5370 696e 655f 32da 094c  j.....Spine_2..L
+00004490: 6600 0000 da07 5370 696e 655f 32da 094c  f.....Spine_2..L
 000044a0: 6566 745f 6668 6970 da0a 5269 6768 745f  eft_fhip..Right_
 000044b0: 6668 6970 da09 4c65 6674 5f62 6869 70da  fhip..Left_bhip.
 000044c0: 0a52 6967 6874 5f62 6869 7063 0100 0000  .Right_bhipc....
-000044d0: 0000 0000 0000 0000 0200 0000 0400 0000  ................
-000044e0: 1300 0000 731a 0000 0067 007c 005d 127d  ....s....g.|.].}
-000044f0: 017c 0188 006a 0076 0072 047c 0191 0271  .|...j.v.r.|...q
-00004500: 0453 0072 2200 0000 a901 72a9 0000 0029  .S.r".....r....)
-00004510: 0272 1f00 0000 da09 626f 6479 5f70 6172  .r......body_par
-00004520: 7429 0172 cf00 0000 7222 0000 0072 2300  t).r....r"...r#.
-00004530: 0000 7224 0000 0057 0200 0072 5800 0000  ..r$...W...rX...
-00004540: 7a26 7375 7065 7276 6973 6564 5f74 6167  z&supervised_tag
-00004550: 6769 6e67 2e3c 6c6f 6361 6c73 3e2e 3c6c  ging.<locals>.<l
-00004560: 6973 7463 6f6d 703e 2902 da0b 696e 7465  istcomp>)...inte
-00004570: 7261 6374 6f72 73da 0662 7061 7274 7363  ractors..bpartsc
-00004580: 0200 0000 0000 0000 0000 0000 0400 0000  ................
-00004590: 0900 0000 1300 0000 73b6 0000 007a 1488  ........s....z..
-000045a0: 0064 0119 007c 0164 0119 0017 007d 0257  .d...|.d.....}.W
-000045b0: 006e 2804 0074 0079 3c01 0001 0001 0087  .n(..t.y<.......
-000045c0: 0066 0164 0264 0384 087c 0164 0119 0044  .f.d.d...|.d...D
-000045d0: 0083 017d 0259 006e 0230 007a 1488 0064  ...}.Y.n.0.z...d
-000045e0: 0419 007c 0164 0519 0017 007d 0357 006e  ...|.d.....}.W.n
-000045f0: 2804 0074 0079 7a01 0001 0001 0087 0066  (..t.yz........f
-00004600: 0164 0664 0384 087c 0164 0519 0044 0083  .d.d...|.d...D..
-00004610: 017d 0359 006e 0230 0074 016a 02a0 0374  .}.Y.n.0.t.j...t
-00004620: 0488 0674 057c 0274 0683 0273 947c 026e  ...t.|.t...s.|.n
-00004630: 027c 0374 057c 0274 0683 0273 a47c 036e  .|.t.|.t...s.|.n
-00004640: 027c 0288 0564 0719 0088 0288 0483 06a1  .|...d..........
-00004650: 0153 0029 087a 4252 6574 7572 6e20 6120  .S.).zBReturn a 
-00004660: 736d 6f6f 7468 2062 6f6f 6c65 616e 2061  smooth boolean a
-00004670: 7272 6179 2077 6974 6820 3174 6f31 2063  rray with 1to1 c
-00004680: 6f6e 7461 6374 7320 6265 7477 6565 6e20  ontacts between 
-00004690: 7477 6f20 6d69 6365 2e72 0100 0000 6301  two mice.r....c.
-000046a0: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-000046b0: 0000 0013 0000 0073 1c00 0000 6700 7c00  .......s....g.|.
-000046c0: 5d14 7d01 8800 6400 1900 6401 1700 7c01  ].}...d...d...|.
-000046d0: 1700 9102 7104 5300 2902 7201 0000 0072  ....q.S.).r....r
-000046e0: 6900 0000 7222 0000 00a9 0272 1f00 0000  i...r".....r....
-000046f0: da06 7375 6666 6978 a901 72e3 0000 0072  ..suffix..r....r
-00004700: 2200 0000 7223 0000 0072 2400 0000 6002  "...r#...r$...`.
-00004710: 0000 7258 0000 007a 4073 7570 6572 7669  ..rX...z@supervi
-00004720: 7365 645f 7461 6767 696e 672e 3c6c 6f63  sed_tagging.<loc
-00004730: 616c 733e 2e6f 6e65 6279 6f6e 655f 636f  als>.onebyone_co
-00004740: 6e74 6163 742e 3c6c 6f63 616c 733e 2e3c  ntact.<locals>.<
-00004750: 6c69 7374 636f 6d70 3e72 1800 0000 72d7  listcomp>r....r.
-00004760: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00004770: 0200 0000 0400 0000 1300 0000 731c 0000  ............s...
-00004780: 0067 007c 005d 147d 0188 0064 0019 0064  .g.|.].}...d...d
-00004790: 0117 007c 0117 0091 0271 0453 0029 0272  ...|.....q.S.).r
-000047a0: 1800 0000 7269 0000 0072 2200 0000 72e5  ....ri...r"...r.
-000047b0: 0000 0072 e700 0000 7222 0000 0072 2300  ...r....r"...r#.
-000047c0: 0000 7224 0000 0065 0200 0072 5800 0000  ..r$...e...rX...
-000047d0: 72ba 0000 0029 07da 0954 7970 6545 7272  r....)...TypeErr
-000047e0: 6f72 da06 6465 6570 6f66 da05 7574 696c  or..deepof..util
-000047f0: 73da 1473 6d6f 6f74 685f 626f 6f6c 6561  s..smooth_boolea
-00004800: 6e5f 6172 7261 7972 2a00 0000 7225 0000  n_arrayr*...r%..
-00004810: 0072 2700 0000 2904 72e3 0000 0072 e400  .r'...).r....r..
-00004820: 0000 7212 0000 0072 1300 0000 a906 da0a  ..r....r........
-00004830: 616e 696d 616c 5f69 6473 7215 0000 00da  animal_idsr.....
-00004840: 0c61 7265 6e61 5f70 6172 616d 7372 1600  .arena_paramsr..
-00004850: 0000 72d4 0000 0072 ce00 0000 72e7 0000  ..r....r....r...
-00004860: 0072 2300 0000 da10 6f6e 6562 796f 6e65  .r#.....onebyone
-00004870: 5f63 6f6e 7461 6374 5902 0000 7324 0000  _contactY...s$..
-00004880: 0000 0402 0114 010c 011c 0202 0114 010c  ................
-00004890: 011c 0206 0102 0102 0110 0110 0106 0102  ................
-000048a0: 0102 fa02 ff7a 2c73 7570 6572 7669 7365  .....z,supervise
-000048b0: 645f 7461 6767 696e 672e 3c6c 6f63 616c  d_tagging.<local
-000048c0: 733e 2e6f 6e65 6279 6f6e 655f 636f 6e74  s>.onebyone_cont
-000048d0: 6163 74a9 0272 e300 0000 722f 0000 0063  act..r....r/...c
-000048e0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-000048f0: 0d00 0000 1300 0000 7346 0000 0074 006a  ........sF...t.j
-00004900: 01a0 0274 0388 057c 0064 0119 0064 0217  ...t...|.d...d..
-00004910: 007c 0064 0119 0064 0317 007c 0064 0419  .|.d...d...|.d..
-00004920: 0064 0217 007c 0064 0419 0064 0317 0088  .d...|.d...d....
-00004930: 0464 0519 007c 0188 0188 0364 068d 09a1  .d...|.....d....
-00004940: 0153 0029 077a 4a52 6574 7572 6e20 6120  .S.).zJReturn a 
-00004950: 736d 6f6f 7468 2062 6f6f 6c65 616e 2061  smooth boolean a
-00004960: 7272 6179 2077 6974 6820 7369 6465 2062  rray with side b
-00004970: 7920 7369 6465 2063 6f6e 7461 6374 7320  y side contacts 
-00004980: 6265 7477 6565 6e20 7477 6f20 6d69 6365  between two mice
-00004990: 2e72 0100 0000 7295 0000 0072 9000 0000  .r....r....r....
-000049a0: 7218 0000 0072 bb00 0000 2903 722f 0000  r....r....).r/..
-000049b0: 0072 1500 0000 7216 0000 0029 0472 e900  .r....r....).r..
-000049c0: 0000 72ea 0000 0072 eb00 0000 7231 0000  ..r....r....r1..
-000049d0: 0072 f000 0000 72ec 0000 0072 2200 0000  .r....r....r"...
-000049e0: 7223 0000 00da 1074 776f 6279 7477 6f5f  r#.....twobytwo_
-000049f0: 636f 6e74 6163 7472 0200 0073 1a00 0000  contactr...s....
-00004a00: 0003 0601 0201 0201 0a01 0a01 0a01 0a01  ................
-00004a10: 0601 0201 0201 02f7 04ff 7a2c 7375 7065  ..........z,supe
-00004a20: 7276 6973 6564 5f74 6167 6769 6e67 2e3c  rvised_tagging.<
-00004a30: 6c6f 6361 6c73 3e2e 7477 6f62 7974 776f  locals>.twobytwo
-00004a40: 5f63 6f6e 7461 6374 6303 0000 0000 0000  _contactc.......
-00004a50: 0000 0000 0006 0000 0006 0000 0013 0000  ................
-00004a60: 0073 5c00 0000 6700 6401 a201 7d03 8701  .s\...g.d...}...
-00004a70: 6601 6402 6403 8408 7c03 4400 8301 7d03  f.d.d...|.D...}.
-00004a80: 8801 8700 8702 6602 6404 6403 8408 7c03  ......f.d.d...|.
-00004a90: 4400 8301 1900 7d04 7400 6a01 7c04 6405  D.....}.t.j.|.d.
-00004aa0: 6406 8502 1900 6405 6407 8d02 7d05 7400  d.....d.d...}.t.
-00004ab0: 6a02 7c05 6408 7400 6a03 6408 6407 8d04  j.|.d.t.j.d.d...
-00004ac0: 5300 2909 7a24 5265 7475 726e 2074 6865  S.).z$Return the
-00004ad0: 206f 7665 7261 6c6c 2073 7065 6564 206f   overall speed o
-00004ae0: 6620 6120 6d6f 7573 652e 290b 726a 0000  f a mouse.).rj..
-00004af0: 0072 db00 0000 72dc 0000 0072 8500 0000  .r....r....r....
-00004b00: 72d9 0000 0072 da00 0000 72dd 0000 0072  r....r....r....r
-00004b10: de00 0000 72df 0000 0072 e000 0000 da09  ....r....r......
-00004b20: 5461 696c 5f62 6173 6563 0100 0000 0000  Tail_basec......
-00004b30: 0000 0000 0000 0200 0000 0400 0000 1300  ................
-00004b40: 0000 731a 0000 0067 007c 005d 127d 017c  ..s....g.|.].}.|
-00004b50: 0188 006a 0076 0072 047c 0191 0271 0453  ...j.v.r.|...q.S
-00004b60: 0072 2200 0000 72e1 0000 00a9 0272 1f00  .r"...r......r..
-00004b70: 0000 da05 6270 6172 7429 01da 0a6f 7672  ....bpart)...ovr
-00004b80: 5f73 7065 6564 7372 2200 0000 7223 0000  _speedsr"...r#..
-00004b90: 0072 2400 0000 9202 0000 7258 0000 007a  .r$.......rX...z
-00004ba0: 3d73 7570 6572 7669 7365 645f 7461 6767  =supervised_tagg
-00004bb0: 696e 672e 3c6c 6f63 616c 733e 2e6f 7665  ing.<locals>.ove
-00004bc0: 7261 6c6c 5f73 7065 6564 2e3c 6c6f 6361  rall_speed.<loca
-00004bd0: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 6301  ls>.<listcomp>c.
-00004be0: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00004bf0: 0000 0013 0000 0073 1800 0000 6700 7c00  .......s....g.|.
-00004c00: 5d10 7d01 8800 8801 1700 7c01 1700 9102  ].}.......|.....
-00004c10: 7104 5300 7222 0000 0072 2200 0000 72f3  q.S.r"...r"...r.
-00004c20: 0000 0029 02da 035f 6964 da05 7563 6f6e  ...)..._id..ucon
-00004c30: 6472 2200 0000 7223 0000 0072 2400 0000  dr"...r#...r$...
-00004c40: 9302 0000 7258 0000 0072 1800 0000 4e72  ....rX...r....Nr
-00004c50: 1900 0000 7201 0000 0029 0472 1c00 0000  ....r....).r....
-00004c60: da09 6e61 6e6d 6564 6961 6eda 0669 6e73  ..nanmedian..ins
-00004c70: 6572 7472 7900 0000 2906 72f5 0000 0072  ertry...).r....r
-00004c80: f600 0000 72f7 0000 0072 e400 0000 725c  ....r....r....r\
-00004c90: 0000 00da 0961 7667 5f73 7065 6564 7222  .....avg_speedr"
-00004ca0: 0000 0029 0372 f600 0000 72f5 0000 0072  ...).r....r....r
-00004cb0: f700 0000 7223 0000 00da 0d6f 7665 7261  ....r#.....overa
-00004cc0: 6c6c 5f73 7065 6564 8302 0000 730a 0000  ll_speed....s...
-00004cd0: 0000 0208 0d12 0118 0116 017a 2973 7570  ...........z)sup
-00004ce0: 6572 7669 7365 645f 7461 6767 696e 672e  ervised_tagging.
-00004cf0: 3c6c 6f63 616c 733e 2e6f 7665 7261 6c6c  <locals>.overall
-00004d00: 5f73 7065 6564 723f 0000 0072 9500 0000  _speedr?...r....
-00004d10: da0a 5f6e 6f73 6532 6e6f 7365 46da 0b5f  .._nose2noseF.._
-00004d20: 7369 6465 6279 7369 6465 da0b 5f73 6964  sidebyside.._sid
-00004d30: 6572 6573 6964 6572 9000 0000 da0a 5f6e  eresider......_n
-00004d40: 6f73 6532 7461 696c da0a 5f6e 6f73 6532  ose2tail.._nose2
-00004d50: 626f 6479 72bc 0000 0072 bd00 0000 2904  bodyr....r....).
-00004d60: 728d 0000 0072 8e00 0000 728f 0000 0072  r....r....r....r
-00004d70: 1400 0000 da0a 5f66 6f6c 6c6f 7769 6e67  ......_following
-00004d80: 72b9 0000 0072 8500 0000 7262 0000 0072  r....r....rb...r
-00004d90: be00 0000 724b 0000 0029 0272 6700 0000  ....rK...).rg...
-00004da0: 7268 0000 0072 6f00 0000 2902 7272 0000  rh...ro...).rr..
-00004db0: 0072 6800 0000 7282 0000 0072 8700 0000  .rh...r....r....
-00004dc0: 2901 7268 0000 0072 8800 0000 726e 0000  ).rh...r....rn..
-00004dd0: 0029 26da 046f 7065 6eda 026f 73da 0470  .)&..open..os..p
-00004de0: 6174 68da 046a 6f69 6eda 0670 6963 6b6c  ath..join..pickl
-00004df0: 65da 046c 6f61 6472 2700 0000 da07 5f74  e..loadr'....._t
-00004e00: 6162 6c65 73da 046b 6579 73da 075f 7669  ables..keys.._vi
-00004e10: 6465 6f73 da05 696e 6465 78da 0d5f 6172  deos..index.._ar
-00004e20: 656e 615f 7061 7261 6d73 da06 5f61 7265  ena_params.._are
-00004e30: 6e61 da0b 5f61 6e69 6d61 6c5f 6964 73da  na.._animal_ids.
-00004e40: 036c 656e da02 7265 da07 6669 6e64 616c  .len..re..findal
-00004e50: 6cda 0a49 6e64 6578 4572 726f 72da 0b72  l..IndexError..r
-00004e60: 6573 6574 5f69 6e64 6578 da0b 6765 745f  eset_index..get_
-00004e70: 7175 616c 6974 79da 075f 7363 616c 6573  quality.._scales
-00004e80: 7206 0000 00da 0462 6f6f 6c72 0d00 0000  r......boolr....
-00004e90: 72e9 0000 0072 ea00 0000 72eb 0000 0072  r....r....r....r
-00004ea0: a200 0000 7274 0000 0072 6300 0000 7270  ....rt...rc...rp
-00004eb0: 0000 0072 8200 0000 7289 0000 0072 9800  ...r....r....r..
-00004ec0: 0000 7299 0000 00da 0666 696c 6c6e 6172  ..r......fillnar
-00004ed0: ab00 0000 72ac 0000 0029 1a72 cd00 0000  ....r....).r....
-00004ee0: 72ce 0000 0072 cf00 0000 72d0 0000 0072  r....r....r....r
-00004ef0: b000 0000 72d1 0000 0072 d200 0000 72d3  ....r....r....r.
-00004f00: 0000 0072 d400 0000 da03 6573 7472 7200  ...r......estrr.
-00004f10: 0000 da06 7472 6163 6b73 da09 7669 645f  ....tracks..vid_
-00004f20: 696e 6465 7872 4a00 0000 da09 756e 6465  indexrJ.....unde
-00004f30: 7263 6f6e 64da 0876 6964 5f6e 616d 65da  rcond..vid_name.
-00004f40: 0b6c 696b 656c 6968 6f6f 6473 da08 7461  .likelihoods..ta
-00004f50: 675f 6469 6374 da09 6d61 696e 5f62 6f64  g_dict..main_bod
-00004f60: 7972 ef00 0000 72f1 0000 0072 fb00 0000  yr....r....r....
-00004f70: da0c 616e 696d 616c 5f70 6169 7273 da0b  ..animal_pairs..
-00004f80: 616e 696d 616c 5f70 6169 7272 f600 0000  animal_pairr....
-00004f90: da06 7461 675f 6466 7222 0000 0029 0772  ..tag_dfr"...).r
-00004fa0: ed00 0000 7215 0000 0072 ee00 0000 7216  ....r....r....r.
-00004fb0: 0000 0072 cf00 0000 72d4 0000 0072 ce00  ...r....r....r..
-00004fc0: 0000 7223 0000 00da 1273 7570 6572 7669  ..r#.....supervi
-00004fd0: 7365 645f 7461 6767 696e 6706 0200 0073  sed_tagging....s
-00004fe0: 0001 0000 001f 0201 0601 0201 0201 02fd  ................
-00004ff0: 0205 02fa 0407 0201 2803 0e01 0c02 0a01  ........(.......
-00005000: 0602 0601 1402 0201 1801 0c01 0e02 1001  ................
-00005010: 1001 1003 1001 1401 0e01 0e03 0403 080b  ................
-00005020: 1202 1e19 1e11 0815 0e02 0e02 0a02 0201  ................
-00005030: 06ff 1e06 0afe 0201 16ff 0206 0afe 0201  ................
-00005040: 16ff 0204 0201 08ff 1e03 0201 08ff 1e03  ................
-00005050: 0201 08ff 1e03 0201 08ff 1e04 0203 0601  ................
-00005060: 0201 0201 0201 0601 0601 0601 06fa 04ff  ................
-00005070: 02fe 0201 16ff 020f 0601 0201 0201 0201  ................
-00005080: 0601 0601 0601 06fa 04ff 02fe 0201 16ff  ................
-00005090: 060c 0e01 0a02 0801 0601 0201 0201 0201  ................
-000050a0: 0201 0601 0afb 02ff 1009 0601 0201 0201  ................
-000050b0: 0201 0201 0201 0601 0601 0a01 0201 02f7  ................
-000050c0: 04ff 100d 0601 0201 1801 0201 06fd 04ff  ................
-000050d0: 1007 0201 0201 0201 0601 0601 02fb 1209  ................
-000050e0: 1c02 1602 7223 0100 0072 9c00 0000 7218  ....r#...r....r.
-000050f0: 0000 0029 07da 0b63 6f6f 7264 696e 6174  ...)...coordinat
-00005100: 6573 721e 0100 00da 0c76 6964 656f 5f6f  esr......video_o
-00005110: 7574 7075 74da 0b66 7261 6d65 5f6c 696d  utput..frame_lim
-00005120: 6974 da05 6465 6275 67da 066e 5f6a 6f62  it..debug..n_job
-00005130: 7372 d400 0000 6307 0000 0000 0000 0000  sr....c.........
-00005140: 0000 0008 0000 0008 0000 0003 0000 0073  ...............s
-00005150: a400 0000 8700 8701 8702 8704 8705 8706  ................
-00005160: 6606 6401 6402 8408 8903 7400 7c02 7401  f.d.d.....t.|.t.
-00005170: 8302 7226 7c02 7d07 6e20 7c02 6403 6b02  ..r&|.}.n |.d.k.
-00005180: 723e 7401 8800 6a02 a003 a100 8301 7d07  r>t...j.......}.
-00005190: 6e08 7404 6404 8301 8201 7405 7406 7c07  n.t.d.....t.t.|.
-000051a0: 8301 6405 8d01 8905 7407 6406 7c05 6407  ..d.....t.d.|.d.
-000051b0: 8d02 8f28 0100 7408 8300 8703 6601 6408  ...(..t.....f.d.
-000051c0: 6409 8408 7c07 4400 8301 8301 0100 5700  d...|.D.......W.
-000051d0: 640a 0400 0400 8303 0100 6e10 3100 738e  d.........n.1.s.
-000051e0: 3000 0100 0100 0100 5900 0100 8805 a009  0.......Y.......
-000051f0: a100 0100 640a 5300 290b 61a7 0200 004f  ....d.S.).a....O
-00005200: 7574 7075 7420 616e 6e6f 7461 7465 6420  utput annotated 
-00005210: 7669 6465 6f73 2e0a 0a20 2020 2041 7267  videos...    Arg
-00005220: 733a 0a20 2020 2020 2020 2063 6f6f 7264  s:.        coord
-00005230: 696e 6174 6573 3a20 436f 6f72 6469 6e61  inates: Coordina
-00005240: 7465 7320 6f62 6a65 6374 2e0a 2020 2020  tes object..    
-00005250: 2020 2020 7461 675f 6469 6374 3a20 4469      tag_dict: Di
-00005260: 6374 696f 6e61 7279 2077 6974 6820 7375  ctionary with su
-00005270: 7065 7276 6973 6564 2061 6e6e 6f74 6174  pervised annotat
-00005280: 696f 6e73 2074 6f20 7265 6e64 6572 206f  ions to render o
-00005290: 6e20 7468 6520 7669 6465 6f2e 0a20 2020  n the video..   
-000052a0: 2020 2020 2076 6964 656f 5f6f 7574 7075       video_outpu
-000052b0: 743a 204c 6973 7420 7769 7468 2074 6865  t: List with the
-000052c0: 206e 616d 6573 206f 6620 7468 6520 7669   names of the vi
-000052d0: 6465 6f73 2074 6f20 7265 6e64 6572 2c20  deos to render, 
-000052e0: 6f72 2027 616c 6c27 2028 6465 6661 756c  or 'all' (defaul
-000052f0: 7429 2074 6f20 7265 6e64 6572 2061 6c6c  t) to render all
-00005300: 2076 6964 656f 732e 0a20 2020 2020 2020   videos..       
-00005310: 2066 7261 6d65 5f6c 696d 6974 3a20 4e75   frame_limit: Nu
-00005320: 6d62 6572 206f 6620 6672 616d 6573 2074  mber of frames t
-00005330: 6f20 7265 6e64 6572 2070 6572 206f 7574  o render per out
-00005340: 7075 7420 7669 6465 6f2e 2049 6620 4e6f  put video. If No
-00005350: 6e65 2c20 616c 6c20 6672 616d 6573 2061  ne, all frames a
-00005360: 7265 2072 656e 6465 7265 642e 0a20 2020  re rendered..   
-00005370: 2020 2020 2064 6562 7567 3a20 4966 2054       debug: If T
-00005380: 7275 652c 2064 6562 7567 6769 6e67 2069  rue, debugging i
-00005390: 6e66 6f72 6d61 7469 6f6e 2c20 7375 6368  nformation, such
-000053a0: 2061 7320 6172 656e 6120 6669 7473 2061   as arena fits a
-000053b0: 6e64 2070 726f 6365 7373 6564 2074 7261  nd processed tra
-000053c0: 636b 6c65 7473 2c20 6172 6520 6469 7370  cklets, are disp
-000053d0: 6c61 7965 642e 0a20 2020 2020 2020 206e  layed..        n
-000053e0: 5f6a 6f62 733a 204e 756d 6265 7220 6f66  _jobs: Number of
-000053f0: 206a 6f62 7320 746f 2072 756e 2069 6e20   jobs to run in 
-00005400: 7061 7261 6c6c 656c 2e0a 2020 2020 2020  parallel..      
-00005410: 2020 7061 7261 6d73 2028 6469 6374 293a    params (dict):
-00005420: 2064 6963 7469 6f6e 6172 7920 746f 206f   dictionary to o
-00005430: 7665 7277 7269 7465 2074 6865 2064 6566  verwrite the def
-00005440: 6175 6c74 2076 616c 7565 7320 6f66 2074  ault values of t
-00005450: 6865 2068 7970 6572 7061 7261 6d65 7465  he hyperparamete
-00005460: 7273 206f 6620 7468 6520 6675 6e63 7469  rs of the functi
-00005470: 6f6e 7320 7468 6174 2074 6865 2073 7570  ons that the sup
-00005480: 6572 7669 7365 6420 706f 7365 2065 7374  ervised pose est
-00005490: 696d 6174 696f 6e20 7574 696c 697a 6573  imation utilizes
-000054a0: 2e0a 2020 2020 6301 0000 0000 0000 0000  ..    c.........
-000054b0: 0000 0001 0000 0008 0000 0013 0000 0073  ...............s
-000054c0: 3a00 0000 7400 6a01 6a02 8800 8805 7c00  :...t.j.j.....|.
-000054d0: 1900 7403 8800 6a04 a005 a100 8301 a006  ..t...j.........
-000054e0: 7c00 a101 8801 8802 8803 6401 8d06 0100  |.........d.....
-000054f0: 8804 a007 6402 a101 0100 6403 5300 2904  ....d.....d.S.).
-00005500: 7a52 4f75 7470 7574 2061 2073 696e 676c  zROutput a singl
-00005510: 6520 616e 6e6f 7461 7465 6420 7669 6465  e annotated vide
-00005520: 6f2e 2045 6e63 6c6f 7365 6420 696e 2061  o. Enclosed in a
-00005530: 2066 756e 6374 696f 6e20 746f 2065 6e61   function to ena
-00005540: 626c 6520 7061 7261 6c6c 656c 697a 6174  ble parallelizat
-00005550: 696f 6e2e 2905 721e 0100 0072 1a01 0000  ion.).r....r....
-00005560: 7227 0100 0072 2601 0000 72d4 0000 0072  r'...r&...r....r
-00005570: 1800 0000 4e29 0872 e900 0000 da07 7669  ....N).r......vi
-00005580: 7375 616c 73da 0e61 6e6e 6f74 6174 655f  suals..annotate_
-00005590: 7669 6465 6f72 2700 0000 7208 0100 0072  videor'...r....r
-000055a0: 0901 0000 720b 0100 00da 0675 7064 6174  ....r......updat
-000055b0: 6529 01da 0369 6478 2906 7224 0100 0072  e)...idx).r$...r
-000055c0: 2701 0000 7226 0100 0072 d400 0000 da04  '...r&...r......
-000055d0: 7062 6172 721e 0100 0072 2200 0000 7223  pbarr....r"...r#
-000055e0: 0000 00da 0c6f 7574 7075 745f 7669 6465  .....output_vide
-000055f0: 6f17 0300 0073 1200 0000 0002 0601 0201  o....s..........
-00005600: 0601 1201 0201 0201 02fa 0608 7a29 7461  ............z)ta
-00005610: 6767 6564 5f76 6964 656f 5f6f 7574 7075  gged_video_outpu
-00005620: 742e 3c6c 6f63 616c 733e 2e6f 7574 7075  t.<locals>.outpu
-00005630: 745f 7669 6465 6f72 9c00 0000 7a52 5669  t_videor....zRVi
-00005640: 6465 6f20 6f75 7470 7574 206d 7573 7420  deo output must 
-00005650: 6265 2065 6974 6865 7220 2761 6c6c 2720  be either 'all' 
-00005660: 6f72 2061 206c 6973 7420 7769 7468 2074  or a list with t
-00005670: 6865 206e 616d 6573 206f 6620 7468 6520  he names of the 
-00005680: 7669 6465 6f73 2074 6f20 7265 6e64 6572  videos to render
-00005690: 2901 da05 746f 7461 6cda 0974 6872 6561  )...total..threa
-000056a0: 6469 6e67 2901 7228 0100 0063 0100 0000  ding).r(...c....
-000056b0: 0000 0000 0000 0000 0200 0000 0300 0000  ................
-000056c0: 3300 0000 731a 0000 007c 005d 127d 0174  3...s....|.].}.t
-000056d0: 0088 0083 017c 0183 0156 0001 0071 0264  .....|...V...q.d
-000056e0: 0053 0029 014e 2901 7202 0000 0029 0272  .S.).N).r....).r
-000056f0: 1f00 0000 da03 6b65 7929 0172 2e01 0000  ......key).r....
-00005700: 7222 0000 0072 2300 0000 da09 3c67 656e  r"...r#.....<gen
-00005710: 6578 7072 3e2e 0300 0072 5800 0000 7a26  expr>....rX...z&
-00005720: 7461 6767 6564 5f76 6964 656f 5f6f 7574  tagged_video_out
-00005730: 7075 742e 3c6c 6f63 616c 733e 2e3c 6765  put.<locals>.<ge
-00005740: 6e65 7870 723e 4e29 0a72 2500 0000 7227  nexpr>N).r%...r'
-00005750: 0000 0072 0801 0000 7209 0100 00da 0e41  ...r....r......A
-00005760: 7474 7269 6275 7465 4572 726f 7272 0c00  ttributeErrorr..
-00005770: 0000 720f 0100 0072 0400 0000 7203 0000  ..r....r....r...
-00005780: 00da 0563 6c6f 7365 2908 7224 0100 0072  ...close).r$...r
-00005790: 1e01 0000 7225 0100 0072 2601 0000 7227  ....r%...r&...r'
-000057a0: 0100 0072 2801 0000 72d4 0000 00da 0876  ...r(...r......v
-000057b0: 6964 5f69 6478 7372 2200 0000 2907 7224  id_idxsr"...).r$
-000057c0: 0100 0072 2701 0000 7226 0100 0072 2e01  ...r'...r&...r..
-000057d0: 0000 72d4 0000 0072 2d01 0000 721e 0100  ..r....r-...r...
-000057e0: 0072 2300 0000 da13 7461 6767 6564 5f76  .r#.....tagged_v
-000057f0: 6964 656f 5f6f 7574 7075 7402 0300 0073  ideo_output....s
-00005800: 1800 0000 0015 160c 0a01 0601 0801 1002  ................
-00005810: 0201 02ff 0404 0e01 0e01 3601 7236 0100  ..........6.r6..
-00005820: 00da 085f 5f6d 6169 6e5f 5fda 0669 676e  ...__main__..ign
-00005830: 6f72 657a 1941 6c6c 2d4e 614e 2073 6c69  orez.All-NaN sli
-00005840: 6365 2065 6e63 6f75 6e74 6572 6564 2901  ce encountered).
-00005850: da07 6d65 7373 6167 6529 0146 2901 723e  ..message).F).r>
-00005860: 0000 0029 0146 2903 4672 4b00 0000 7264  ...).F).FrK...rd
-00005870: 0000 0029 0172 6400 0000 2901 7264 0000  ...).rd...).rd..
-00005880: 0029 0272 8a00 0000 7201 0000 0029 0272  .).r....r....).r
-00005890: a300 0000 4629 0572 9c00 0000 4e46 7218  ....F).r....NFr.
-000058a0: 0000 004e 293e da07 5f5f 646f 635f 5f72  ...N)>..__doc__r
-000058b0: 0301 0000 7206 0100 0072 7500 0000 da06  ....r....ru.....
-000058c0: 6a6f 626c 6962 7202 0000 0072 0300 0000  joblibr....r....
-000058d0: 7204 0000 00da 0674 7970 696e 6772 0500  r......typingr..
-000058e0: 0000 7206 0000 0072 0700 0000 7208 0000  ..r....r....r...
-000058f0: 00da 1073 6861 7065 6c79 2e67 656f 6d65  ...shapely.geome
-00005900: 7472 7972 0900 0000 720a 0000 00da 1573  tryr....r......s
-00005910: 6b6c 6561 726e 2e70 7265 7072 6f63 6573  klearn.preproces
-00005920: 7369 6e67 720b 0000 0072 0c00 0000 da09  singr....r......
-00005930: 6974 6572 746f 6f6c 7372 0d00 0000 da03  itertoolsr......
-00005940: 6376 32da 056e 756d 7079 721c 0000 00da  cv2..numpyr.....
-00005950: 0670 616e 6461 7372 9800 0000 da05 7265  .pandasr......re
-00005960: 6765 7872 1001 0000 da10 736b 6c65 6172  gexr......sklear
-00005970: 6e2e 7069 7065 6c69 6e65 da07 736b 6c65  n.pipeline..skle
-00005980: 6172 6eda 0c64 6565 706f 662e 7574 696c  arn..deepof.util
-00005990: 7372 e900 0000 da0f 6465 6570 6f66 2e70  sr......deepof.p
-000059a0: 6f73 745f 686f 63da 0770 726f 6a65 6374  ost_hoc..project
-000059b0: 7224 0100 00da 0a74 6162 6c65 5f64 6963  r$.....table_dic
-000059c0: 7472 9900 0000 7226 0000 0072 ac00 0000  tr....r&...r....
-000059d0: 72c9 0000 0072 5c00 0000 722a 0000 0072  r....r\...r*...r
-000059e0: 1601 0000 7231 0000 0072 3d00 0000 7249  ....r1...r=...rI
-000059f0: 0000 0072 6300 0000 7270 0000 00da 076e  ...rc...rp.....n
-00005a00: 6461 7272 6179 da08 7069 7065 6c69 6e65  darray..pipeline
-00005a10: da08 5069 7065 6c69 6e65 7282 0000 0072  ..Pipeliner....r
-00005a20: 8900 0000 72a2 0000 0072 b300 0000 da04  ....r....r......
-00005a30: 6469 6374 72c3 0000 0072 cc00 0000 7223  dictr....r....r#
-00005a40: 0100 0072 3601 0000 da08 5f5f 6e61 6d65  ...r6.....__name
-00005a50: 5f5f da0e 6669 6c74 6572 7761 726e 696e  __..filterwarnin
-00005a60: 6773 7222 0000 0072 2200 0000 7222 0000  gsr"...r"...r"..
-00005a70: 0072 2300 0000 da08 3c6d 6f64 756c 653e  .r#.....<module>
-00005a80: 0500 0000 7308 0100 0004 0208 0108 0108  ....s...........
-00005a90: 0114 0118 0110 010c 010c 010c 0208 0108  ................
-00005aa0: 0108 0108 0108 0208 0108 030a 010a 010a  ................
-00005ab0: 0404 0102 0102 0102 0102 0102 0104 f90c  ................
-00005ac0: 3400 f702 0104 0102 0102 0102 0102 0102  4...............
-00005ad0: 0102 0102 0102 0104 f60c 3508 0a0a 1400  ..........5.....
-00005ae0: fa02 0102 0104 0104 0102 0102 0102 0104  ................
-00005af0: f90c 3b00 0100 0100 f602 0104 0102 0104  ..;.............
-00005b00: 0104 0102 0102 0102 0102 0102 0102 f60c  ................
-00005b10: 5500 fd02 0104 0106 0102 0104 fc0c 4500  U.............E.
-00005b20: fb02 0104 0104 0102 0102 0102 fb0c 2400  ..............$.
-00005b30: 0100 fa02 0104 0104 0102 0102 0102 0102  ................
-00005b40: 0104 f90c 3b00 ff02 0108 0104 fe0c 1a14  ....;...........
-00005b50: 1c12 2202 0102 f702 0102 0102 0102 0102  ..".............
-00005b60: 0102 0102 0102 0102 0102 0104 f60c 7f00  ................
-00005b70: 7f00 0100 0100 0100 0100 0100 f902 0102  ................
-00005b80: 0102 010e 0102 0102 0102 0102 f90c 300a  ..............0.
-00005b90: 02                                       .
+000044d0: 0000 0000 0000 0000 0100 0000 0600 0000  ................
+000044e0: 1300 0000 7328 0000 0067 007c 005d 2089  ....s(...g.|.] .
+000044f0: 0074 0087 0066 0164 0064 0184 0888 016a  .t...f.d.d.....j
+00004500: 0144 0083 0183 0172 0488 0091 0271 0453  .D.....r.....q.S
+00004510: 0029 0263 0100 0000 0000 0000 0000 0000  .).c............
+00004520: 0200 0000 0400 0000 3300 0000 731a 0000  ........3...s...
+00004530: 007c 005d 127d 0188 007c 0164 0019 0076  .|.].}...|.d...v
+00004540: 0056 0001 0071 0264 0153 0029 0272 0100  .V...q.d.S.).r..
+00004550: 0000 4e72 2200 0000 729b 0000 00a9 015a  ..Nr"...r......Z
+00004560: 0962 6f64 795f 7061 7274 7222 0000 0072  .body_partr"...r
+00004570: 2300 0000 da09 3c67 656e 6578 7072 3e5a  #.....<genexpr>Z
+00004580: 0200 0072 5400 0000 7a30 7375 7065 7276  ...rT...z0superv
+00004590: 6973 6564 5f74 6167 6769 6e67 2e3c 6c6f  ised_tagging.<lo
+000045a0: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
+000045b0: 2e3c 6765 6e65 7870 723e a902 7228 0000  .<genexpr>..r(..
+000045c0: 0072 9d00 0000 a901 721f 0000 0029 0172  .r......r....).r
+000045d0: bc00 0000 72cd 0000 0072 2300 0000 7224  ....r....r#...r$
+000045e0: 0000 0057 0200 0073 0600 0000 0602 0201  ...W...s........
+000045f0: 18fe 7a26 7375 7065 7276 6973 6564 5f74  ..z&supervised_t
+00004600: 6167 6769 6e67 2e3c 6c6f 6361 6c73 3e2e  agging.<locals>.
+00004610: 3c6c 6973 7463 6f6d 703e 2902 da0b 696e  <listcomp>)...in
+00004620: 7465 7261 6374 6f72 73da 0662 7061 7274  teractors..bpart
+00004630: 7363 0200 0000 0000 0000 0000 0000 0400  sc..............
+00004640: 0000 0900 0000 1300 0000 73b6 0000 007a  ..........s....z
+00004650: 1488 0064 0119 007c 0164 0119 0017 007d  ...d...|.d.....}
+00004660: 0257 006e 2804 0074 0079 3c01 0001 0001  .W.n(..t.y<.....
+00004670: 0087 0066 0164 0264 0384 087c 0164 0119  ...f.d.d...|.d..
+00004680: 0044 0083 017d 0259 006e 0230 007a 1488  .D...}.Y.n.0.z..
+00004690: 0064 0419 007c 0164 0519 0017 007d 0357  .d...|.d.....}.W
+000046a0: 006e 2804 0074 0079 7a01 0001 0001 0087  .n(..t.yz.......
+000046b0: 0066 0164 0664 0384 087c 0164 0519 0044  .f.d.d...|.d...D
+000046c0: 0083 017d 0359 006e 0230 0074 016a 02a0  ...}.Y.n.0.t.j..
+000046d0: 0374 0488 0674 057c 0274 0683 0273 947c  .t...t.|.t...s.|
+000046e0: 026e 027c 0374 057c 0274 0683 0273 a47c  .n.|.t.|.t...s.|
+000046f0: 036e 027c 0288 0564 0719 0088 0288 0483  .n.|...d........
+00004700: 06a1 0153 0029 087a 4252 6574 7572 6e20  ...S.).zBReturn 
+00004710: 6120 736d 6f6f 7468 2062 6f6f 6c65 616e  a smooth boolean
+00004720: 2061 7272 6179 2077 6974 6820 3174 6f31   array with 1to1
+00004730: 2063 6f6e 7461 6374 7320 6265 7477 6565   contacts betwee
+00004740: 6e20 7477 6f20 6d69 6365 2e72 0100 0000  n two mice.r....
+00004750: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00004760: 0004 0000 0013 0000 0073 1c00 0000 6700  .........s....g.
+00004770: 7c00 5d14 7d01 8800 6400 1900 6401 1700  |.].}...d...d...
+00004780: 7c01 1700 9102 7104 5300 2902 7201 0000  |.....q.S.).r...
+00004790: 0072 6500 0000 7222 0000 00a9 0272 1f00  .re...r".....r..
+000047a0: 0000 da06 7375 6666 6978 a901 72d1 0000  ....suffix..r...
+000047b0: 0072 2200 0000 7223 0000 0072 2400 0000  .r"...r#...r$...
+000047c0: 6402 0000 7254 0000 007a 4073 7570 6572  d...rT...z@super
+000047d0: 7669 7365 645f 7461 6767 696e 672e 3c6c  vised_tagging.<l
+000047e0: 6f63 616c 733e 2e6f 6e65 6279 6f6e 655f  ocals>.onebyone_
+000047f0: 636f 6e74 6163 742e 3c6c 6f63 616c 733e  contact.<locals>
+00004800: 2e3c 6c69 7374 636f 6d70 3e72 1800 0000  .<listcomp>r....
+00004810: 72c3 0000 0063 0100 0000 0000 0000 0000  r....c..........
+00004820: 0000 0200 0000 0400 0000 1300 0000 731c  ..............s.
+00004830: 0000 0067 007c 005d 147d 0188 0064 0019  ...g.|.].}...d..
+00004840: 0064 0117 007c 0117 0091 0271 0453 0029  .d...|.....q.S.)
+00004850: 0272 1800 0000 7265 0000 0072 2200 0000  .r....re...r"...
+00004860: 72d3 0000 0072 d500 0000 7222 0000 0072  r....r....r"...r
+00004870: 2300 0000 7224 0000 0069 0200 0072 5400  #...r$...i...rT.
+00004880: 0000 72ab 0000 0029 07da 0954 7970 6545  ..r....)...TypeE
+00004890: 7272 6f72 da06 6465 6570 6f66 da05 7574  rror..deepof..ut
+000048a0: 696c 73da 1473 6d6f 6f74 685f 626f 6f6c  ils..smooth_bool
+000048b0: 6561 6e5f 6172 7261 7972 2900 0000 7225  ean_arrayr)...r%
+000048c0: 0000 0072 2700 0000 2904 72d1 0000 0072  ...r'...).r....r
+000048d0: d200 0000 7212 0000 0072 1300 0000 a906  ....r....r......
+000048e0: da0a 616e 696d 616c 5f69 6473 7215 0000  ..animal_idsr...
+000048f0: 00da 0c61 7265 6e61 5f70 6172 616d 7372  ...arena_paramsr
+00004900: 1600 0000 72c1 0000 0072 bb00 0000 72d5  ....r....r....r.
+00004910: 0000 0072 2300 0000 da10 6f6e 6562 796f  ...r#.....onebyo
+00004920: 6e65 5f63 6f6e 7461 6374 5d02 0000 7324  ne_contact]...s$
+00004930: 0000 0000 0402 0114 010c 011c 0202 0114  ................
+00004940: 010c 011c 0206 0102 0102 0110 0110 0106  ................
+00004950: 0102 0102 fa02 ff7a 2c73 7570 6572 7669  .......z,supervi
+00004960: 7365 645f 7461 6767 696e 672e 3c6c 6f63  sed_tagging.<loc
+00004970: 616c 733e 2e6f 6e65 6279 6f6e 655f 636f  als>.onebyone_co
+00004980: 6e74 6163 74a9 0272 d100 0000 722e 0000  ntact..r....r...
+00004990: 0063 0200 0000 0000 0000 0000 0000 0200  .c..............
+000049a0: 0000 0d00 0000 1300 0000 7346 0000 0074  ..........sF...t
+000049b0: 006a 01a0 0274 0388 057c 0064 0119 0064  .j...t...|.d...d
+000049c0: 0217 007c 0064 0119 0064 0317 007c 0064  ...|.d...d...|.d
+000049d0: 0419 0064 0217 007c 0064 0419 0064 0317  ...d...|.d...d..
+000049e0: 0088 0464 0519 007c 0188 0188 0364 068d  ...d...|.....d..
+000049f0: 09a1 0153 0029 077a 4a52 6574 7572 6e20  ...S.).zJReturn 
+00004a00: 6120 736d 6f6f 7468 2062 6f6f 6c65 616e  a smooth boolean
+00004a10: 2061 7272 6179 2077 6974 6820 7369 6465   array with side
+00004a20: 2062 7920 7369 6465 2063 6f6e 7461 6374   by side contact
+00004a30: 7320 6265 7477 6565 6e20 7477 6f20 6d69  s between two mi
+00004a40: 6365 2e72 0100 0000 728b 0000 0072 8600  ce.r....r....r..
+00004a50: 0000 7218 0000 0072 ac00 0000 2903 722e  ..r....r....).r.
+00004a60: 0000 0072 1500 0000 7216 0000 0029 0472  ...r....r....).r
+00004a70: d700 0000 72d8 0000 0072 d900 0000 722f  ....r....r....r/
+00004a80: 0000 0072 de00 0000 72da 0000 0072 2200  ...r....r....r".
+00004a90: 0000 7223 0000 00da 1074 776f 6279 7477  ..r#.....twobytw
+00004aa0: 6f5f 636f 6e74 6163 7476 0200 0073 1a00  o_contactv...s..
+00004ab0: 0000 0003 0601 0201 0201 0a01 0a01 0a01  ................
+00004ac0: 0a01 0601 0201 0201 02f7 04ff 7a2c 7375  ............z,su
+00004ad0: 7065 7276 6973 6564 5f74 6167 6769 6e67  pervised_tagging
+00004ae0: 2e3c 6c6f 6361 6c73 3e2e 7477 6f62 7974  .<locals>.twobyt
+00004af0: 776f 5f63 6f6e 7461 6374 6303 0000 0000  wo_contactc.....
+00004b00: 0000 0000 0000 0006 0000 0006 0000 0013  ................
+00004b10: 0000 0073 5c00 0000 6700 6401 a201 7d03  ...s\...g.d...}.
+00004b20: 8701 6601 6402 6403 8408 7c03 4400 8301  ..f.d.d...|.D...
+00004b30: 7d03 8801 8700 8702 6602 6404 6403 8408  }.......f.d.d...
+00004b40: 7c03 4400 8301 1900 7d04 7400 6a01 7c04  |.D.....}.t.j.|.
+00004b50: 6405 6406 8502 1900 6405 6407 8d02 7d05  d.d.....d.d...}.
+00004b60: 7400 6a02 7c05 6408 7400 6a03 6408 6407  t.j.|.d.t.j.d.d.
+00004b70: 8d04 5300 2909 7a24 5265 7475 726e 2074  ..S.).z$Return t
+00004b80: 6865 206f 7665 7261 6c6c 2073 7065 6564  he overall speed
+00004b90: 206f 6620 6120 6d6f 7573 652e 290b 7266   of a mouse.).rf
+00004ba0: 0000 0072 c700 0000 72c8 0000 0072 7c00  ...r....r....r|.
+00004bb0: 0000 72c5 0000 0072 c600 0000 72c9 0000  ..r....r....r...
+00004bc0: 0072 ca00 0000 72cb 0000 0072 cc00 0000  .r....r....r....
+00004bd0: 5a09 5461 696c 5f62 6173 6563 0100 0000  Z.Tail_basec....
+00004be0: 0000 0000 0000 0000 0100 0000 0600 0000  ................
+00004bf0: 1300 0000 732c 0000 0067 007c 005d 2489  ....s,...g.|.]$.
+00004c00: 0088 0072 0474 0087 0066 0164 0064 0184  ...r.t...f.d.d..
+00004c10: 0888 016a 0144 0083 0183 0172 0488 0091  ...j.D.....r....
+00004c20: 0271 0453 0029 0263 0100 0000 0000 0000  .q.S.).c........
+00004c30: 0000 0000 0200 0000 0300 0000 3300 0000  ............3...
+00004c40: 7316 0000 007c 005d 0e7d 0188 007c 0176  s....|.].}...|.v
+00004c50: 0056 0001 0071 0264 0053 00a9 014e 7222  .V...q.d.S...Nr"
+00004c60: 0000 0072 9b00 0000 a901 da05 6270 6172  ...r........bpar
+00004c70: 7472 2200 0000 7223 0000 0072 ce00 0000  tr"...r#...r....
+00004c80: 9a02 0000 7254 0000 007a 4773 7570 6572  ....rT...zGsuper
+00004c90: 7669 7365 645f 7461 6767 696e 672e 3c6c  vised_tagging.<l
+00004ca0: 6f63 616c 733e 2e6f 7665 7261 6c6c 5f73  ocals>.overall_s
+00004cb0: 7065 6564 2e3c 6c6f 6361 6c73 3e2e 3c6c  peed.<locals>.<l
+00004cc0: 6973 7463 6f6d 703e 2e3c 6765 6e65 7870  istcomp>.<genexp
+00004cd0: 723e 72cf 0000 0072 d000 0000 2901 da0a  r>r....r....)...
+00004ce0: 6f76 725f 7370 6565 6473 72e1 0000 0072  ovr_speedsr....r
+00004cf0: 2300 0000 7224 0000 0096 0200 0073 0800  #...r$.......s..
+00004d00: 0000 0602 0201 0401 18fd 7a3d 7375 7065  ..........z=supe
+00004d10: 7276 6973 6564 5f74 6167 6769 6e67 2e3c  rvised_tagging.<
+00004d20: 6c6f 6361 6c73 3e2e 6f76 6572 616c 6c5f  locals>.overall_
+00004d30: 7370 6565 642e 3c6c 6f63 616c 733e 2e3c  speed.<locals>.<
+00004d40: 6c69 7374 636f 6d70 3e63 0100 0000 0000  listcomp>c......
+00004d50: 0000 0000 0000 0200 0000 0400 0000 1300  ................
+00004d60: 0000 7318 0000 0067 007c 005d 107d 0188  ..s....g.|.].}..
+00004d70: 0088 0117 007c 0117 0091 0271 0453 0072  .....|.....q.S.r
+00004d80: 2200 0000 7222 0000 0029 0272 1f00 0000  "...r"...).r....
+00004d90: 72e2 0000 0029 02da 035f 6964 da05 7563  r....)..._id..uc
+00004da0: 6f6e 6472 2200 0000 7223 0000 0072 2400  ondr"...r#...r$.
+00004db0: 0000 9c02 0000 7254 0000 0072 1800 0000  ......rT...r....
+00004dc0: 4e72 1900 0000 7201 0000 0029 0472 1c00  Nr....r....).r..
+00004dd0: 0000 da09 6e61 6e6d 6564 6961 6eda 0669  ....nanmedian..i
+00004de0: 6e73 6572 7472 7200 0000 2906 72e3 0000  nsertrr...).r...
+00004df0: 0072 e400 0000 72e5 0000 0072 d200 0000  .r....r....r....
+00004e00: 7258 0000 005a 0961 7667 5f73 7065 6564  rX...Z.avg_speed
+00004e10: 7222 0000 0029 0372 e400 0000 72e3 0000  r"...).r....r...
+00004e20: 0072 e500 0000 7223 0000 00da 0d6f 7665  .r....r#.....ove
+00004e30: 7261 6c6c 5f73 7065 6564 8702 0000 730e  rall_speed....s.
+00004e40: 0000 0000 0208 0d0a 0202 fe06 0618 0116  ................
+00004e50: 017a 2973 7570 6572 7669 7365 645f 7461  .z)supervised_ta
+00004e60: 6767 696e 672e 3c6c 6f63 616c 733e 2e6f  gging.<locals>.o
+00004e70: 7665 7261 6c6c 5f73 7065 6564 723d 0000  verall_speedr=..
+00004e80: 0072 8b00 0000 5a0a 5f6e 6f73 6532 6e6f  .r....Z._nose2no
+00004e90: 7365 465a 0b5f 7369 6465 6279 7369 6465  seFZ._sidebyside
+00004ea0: 5a0b 5f73 6964 6572 6573 6964 6572 8600  Z._sideresider..
+00004eb0: 0000 5a0a 5f6e 6f73 6532 7461 696c 5a0a  ..Z._nose2tailZ.
+00004ec0: 5f6e 6f73 6532 626f 6479 72ad 0000 0072  _nose2bodyr....r
+00004ed0: ae00 0000 2904 7283 0000 0072 8400 0000  ....).r....r....
+00004ee0: 7285 0000 0072 1400 0000 5a0a 5f66 6f6c  r....r....Z._fol
+00004ef0: 6c6f 7769 6e67 72aa 0000 0072 7c00 0000  lowingr....r|...
+00004f00: 725e 0000 0072 af00 0000 7247 0000 0029  r^...r....rG...)
+00004f10: 0272 6300 0000 7264 0000 0072 6800 0000  .rc...rd...rh...
+00004f20: 2902 726b 0000 0072 6400 0000 7279 0000  ).rk...rd...ry..
+00004f30: 0072 7d00 0000 2901 7264 0000 0072 7e00  .r}...).rd...r~.
+00004f40: 0000 7267 0000 0029 26da 046f 7065 6eda  ..rg...)&..open.
+00004f50: 026f 73da 0470 6174 68da 046a 6f69 6eda  .os..path..join.
+00004f60: 0670 6963 6b6c 65da 046c 6f61 6472 2700  .pickle..loadr'.
+00004f70: 0000 da07 5f74 6162 6c65 73da 046b 6579  ...._tables..key
+00004f80: 73da 075f 7669 6465 6f73 da05 696e 6465  s.._videos..inde
+00004f90: 78da 0d5f 6172 656e 615f 7061 7261 6d73  x.._arena_params
+00004fa0: da06 5f61 7265 6e61 da0b 5f61 6e69 6d61  .._arena.._anima
+00004fb0: 6c5f 6964 73da 036c 656e da02 7265 da07  l_ids..len..re..
+00004fc0: 6669 6e64 616c 6cda 0a49 6e64 6578 4572  findall..IndexEr
+00004fd0: 726f 72da 0b72 6573 6574 5f69 6e64 6578  ror..reset_index
+00004fe0: da0b 6765 745f 7175 616c 6974 79da 075f  ..get_quality.._
+00004ff0: 7363 616c 6573 7206 0000 00da 0462 6f6f  scalesr......boo
+00005000: 6c72 0d00 0000 72d7 0000 0072 d800 0000  lr....r....r....
+00005010: 72d9 0000 0072 9500 0000 726d 0000 0072  r....r....rm...r
+00005020: 5f00 0000 7269 0000 0072 7900 0000 727f  _...ri...ry...r.
+00005030: 0000 0072 8e00 0000 728f 0000 00da 0666  ...r....r......f
+00005040: 696c 6c6e 6172 9f00 0000 72a0 0000 0029  illnar....r....)
+00005050: 1a72 ba00 0000 72bb 0000 0072 bc00 0000  .r....r....r....
+00005060: 72bd 0000 0072 a400 0000 72be 0000 0072  r....r....r....r
+00005070: bf00 0000 72c0 0000 0072 c100 0000 da03  ....r....r......
+00005080: 6573 7472 6b00 0000 5a06 7472 6163 6b73  estrk...Z.tracks
+00005090: da09 7669 645f 696e 6465 7872 4600 0000  ..vid_indexrF...
+000050a0: 5a09 756e 6465 7263 6f6e 645a 0876 6964  Z.undercondZ.vid
+000050b0: 5f6e 616d 655a 0b6c 696b 656c 6968 6f6f  _nameZ.likelihoo
+000050c0: 6473 da08 7461 675f 6469 6374 5a09 6d61  ds..tag_dictZ.ma
+000050d0: 696e 5f62 6f64 7972 dd00 0000 72df 0000  in_bodyr....r...
+000050e0: 0072 e800 0000 5a0c 616e 696d 616c 5f70  .r....Z.animal_p
+000050f0: 6169 7273 5a0b 616e 696d 616c 5f70 6169  airsZ.animal_pai
+00005100: 7272 e400 0000 5a06 7461 675f 6466 7222  rr....Z.tag_dfr"
+00005110: 0000 0029 0772 db00 0000 7215 0000 0072  ...).r....r....r
+00005120: dc00 0000 7216 0000 0072 bc00 0000 72c1  ....r....r....r.
+00005130: 0000 0072 bb00 0000 7223 0000 00da 1273  ...r....r#.....s
+00005140: 7570 6572 7669 7365 645f 7461 6767 696e  upervised_taggin
+00005150: 6706 0200 0073 0401 0000 001f 0201 0601  g....s..........
+00005160: 0201 0201 02fd 0205 02fa 0407 0201 2803  ..............(.
+00005170: 0e01 0c02 0a01 0602 0601 1402 0201 1801  ................
+00005180: 0c01 0e02 1001 1001 1003 1001 1401 0e01  ................
+00005190: 0e03 0403 080b 0a02 02fe 0606 1e19 1e11  ................
+000051a0: 081a 0e02 0e02 0a02 0201 06ff 1e06 0afe  ................
+000051b0: 0201 16ff 0206 0afe 0201 16ff 0204 0201  ................
+000051c0: 08ff 1e03 0201 08ff 1e03 0201 08ff 1e03  ................
+000051d0: 0201 08ff 1e04 0203 0601 0201 0201 0201  ................
+000051e0: 0601 0601 0601 06fa 04ff 02fe 0201 16ff  ................
+000051f0: 020f 0601 0201 0201 0201 0601 0601 0601  ................
+00005200: 06fa 04ff 02fe 0201 16ff 060c 0e01 0a02  ................
+00005210: 0801 0601 0201 0201 0201 0201 0601 0afb  ................
+00005220: 02ff 1009 0601 0201 0201 0201 0201 0201  ................
+00005230: 0601 0601 0a01 0201 02f7 04ff 100d 0601  ................
+00005240: 0201 1801 0201 06fd 04ff 1007 0201 0201  ................
+00005250: 0201 0601 0601 02fb 1209 1c02 1602 7202  ..............r.
+00005260: 0100 0072 9200 0000 7218 0000 0029 07da  ...r....r....)..
+00005270: 0b63 6f6f 7264 696e 6174 6573 7201 0100  .coordinatesr...
+00005280: 00da 0c76 6964 656f 5f6f 7574 7075 74da  ...video_output.
+00005290: 0b66 7261 6d65 5f6c 696d 6974 da05 6465  .frame_limit..de
+000052a0: 6275 67da 066e 5f6a 6f62 7372 c100 0000  bug..n_jobsr....
+000052b0: 6307 0000 0000 0000 0000 0000 0008 0000  c...............
+000052c0: 0008 0000 0003 0000 0073 a400 0000 8700  .........s......
+000052d0: 8701 8702 8704 8705 8706 6606 6401 6402  ..........f.d.d.
+000052e0: 8408 8903 7400 7c02 7401 8302 7226 7c02  ....t.|.t...r&|.
+000052f0: 7d07 6e20 7c02 6403 6b02 723e 7401 8800  }.n |.d.k.r>t...
+00005300: 6a02 a003 a100 8301 7d07 6e08 7404 6404  j.......}.n.t.d.
+00005310: 8301 8201 7405 7406 7c07 8301 6405 8d01  ....t.t.|...d...
+00005320: 8905 7407 6406 7c05 6407 8d02 8f28 0100  ..t.d.|.d....(..
+00005330: 7408 8300 8703 6601 6408 6409 8408 7c07  t.....f.d.d...|.
+00005340: 4400 8301 8301 0100 5700 640a 0400 0400  D.......W.d.....
+00005350: 8303 0100 6e10 3100 738e 3000 0100 0100  ....n.1.s.0.....
+00005360: 0100 5900 0100 8805 a009 a100 0100 640a  ..Y...........d.
+00005370: 5300 290b 61a7 0200 004f 7574 7075 7420  S.).a....Output 
+00005380: 616e 6e6f 7461 7465 6420 7669 6465 6f73  annotated videos
+00005390: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
+000053a0: 2020 2020 2063 6f6f 7264 696e 6174 6573       coordinates
+000053b0: 3a20 436f 6f72 6469 6e61 7465 7320 6f62  : Coordinates ob
+000053c0: 6a65 6374 2e0a 2020 2020 2020 2020 7461  ject..        ta
+000053d0: 675f 6469 6374 3a20 4469 6374 696f 6e61  g_dict: Dictiona
+000053e0: 7279 2077 6974 6820 7375 7065 7276 6973  ry with supervis
+000053f0: 6564 2061 6e6e 6f74 6174 696f 6e73 2074  ed annotations t
+00005400: 6f20 7265 6e64 6572 206f 6e20 7468 6520  o render on the 
+00005410: 7669 6465 6f2e 0a20 2020 2020 2020 2076  video..        v
+00005420: 6964 656f 5f6f 7574 7075 743a 204c 6973  ideo_output: Lis
+00005430: 7420 7769 7468 2074 6865 206e 616d 6573  t with the names
+00005440: 206f 6620 7468 6520 7669 6465 6f73 2074   of the videos t
+00005450: 6f20 7265 6e64 6572 2c20 6f72 2027 616c  o render, or 'al
+00005460: 6c27 2028 6465 6661 756c 7429 2074 6f20  l' (default) to 
+00005470: 7265 6e64 6572 2061 6c6c 2076 6964 656f  render all video
+00005480: 732e 0a20 2020 2020 2020 2066 7261 6d65  s..        frame
+00005490: 5f6c 696d 6974 3a20 4e75 6d62 6572 206f  _limit: Number o
+000054a0: 6620 6672 616d 6573 2074 6f20 7265 6e64  f frames to rend
+000054b0: 6572 2070 6572 206f 7574 7075 7420 7669  er per output vi
+000054c0: 6465 6f2e 2049 6620 4e6f 6e65 2c20 616c  deo. If None, al
+000054d0: 6c20 6672 616d 6573 2061 7265 2072 656e  l frames are ren
+000054e0: 6465 7265 642e 0a20 2020 2020 2020 2064  dered..        d
+000054f0: 6562 7567 3a20 4966 2054 7275 652c 2064  ebug: If True, d
+00005500: 6562 7567 6769 6e67 2069 6e66 6f72 6d61  ebugging informa
+00005510: 7469 6f6e 2c20 7375 6368 2061 7320 6172  tion, such as ar
+00005520: 656e 6120 6669 7473 2061 6e64 2070 726f  ena fits and pro
+00005530: 6365 7373 6564 2074 7261 636b 6c65 7473  cessed tracklets
+00005540: 2c20 6172 6520 6469 7370 6c61 7965 642e  , are displayed.
+00005550: 0a20 2020 2020 2020 206e 5f6a 6f62 733a  .        n_jobs:
+00005560: 204e 756d 6265 7220 6f66 206a 6f62 7320   Number of jobs 
+00005570: 746f 2072 756e 2069 6e20 7061 7261 6c6c  to run in parall
+00005580: 656c 2e0a 2020 2020 2020 2020 7061 7261  el..        para
+00005590: 6d73 2028 6469 6374 293a 2064 6963 7469  ms (dict): dicti
+000055a0: 6f6e 6172 7920 746f 206f 7665 7277 7269  onary to overwri
+000055b0: 7465 2074 6865 2064 6566 6175 6c74 2076  te the default v
+000055c0: 616c 7565 7320 6f66 2074 6865 2068 7970  alues of the hyp
+000055d0: 6572 7061 7261 6d65 7465 7273 206f 6620  erparameters of 
+000055e0: 7468 6520 6675 6e63 7469 6f6e 7320 7468  the functions th
+000055f0: 6174 2074 6865 2073 7570 6572 7669 7365  at the supervise
+00005600: 6420 706f 7365 2065 7374 696d 6174 696f  d pose estimatio
+00005610: 6e20 7574 696c 697a 6573 2e0a 2020 2020  n utilizes..    
+00005620: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00005630: 0008 0000 0013 0000 0073 3a00 0000 7400  .........s:...t.
+00005640: 6a01 6a02 8800 8805 7c00 1900 7403 8800  j.j.....|...t...
+00005650: 6a04 a005 a100 8301 a006 7c00 a101 8801  j.........|.....
+00005660: 8802 8803 6401 8d06 0100 8804 a007 6402  ....d.........d.
+00005670: a101 0100 6403 5300 2904 7a52 4f75 7470  ....d.S.).zROutp
+00005680: 7574 2061 2073 696e 676c 6520 616e 6e6f  ut a single anno
+00005690: 7461 7465 6420 7669 6465 6f2e 2045 6e63  tated video. Enc
+000056a0: 6c6f 7365 6420 696e 2061 2066 756e 6374  losed in a funct
+000056b0: 696f 6e20 746f 2065 6e61 626c 6520 7061  ion to enable pa
+000056c0: 7261 6c6c 656c 697a 6174 696f 6e2e 2905  rallelization.).
+000056d0: 7201 0100 0072 0001 0000 7206 0100 0072  r....r....r....r
+000056e0: 0501 0000 72c1 0000 0072 1800 0000 4e29  ....r....r....N)
+000056f0: 0872 d700 0000 5a07 7669 7375 616c 735a  .r....Z.visualsZ
+00005700: 0e61 6e6e 6f74 6174 655f 7669 6465 6f72  .annotate_videor
+00005710: 2700 0000 72ef 0000 0072 f000 0000 72f2  '...r....r....r.
+00005720: 0000 00da 0675 7064 6174 6529 01da 0369  .....update)...i
+00005730: 6478 2906 7203 0100 0072 0601 0000 7205  dx).r....r....r.
+00005740: 0100 0072 c100 0000 da04 7062 6172 7201  ...r......pbarr.
+00005750: 0100 0072 2200 0000 7223 0000 00da 0c6f  ...r"...r#.....o
+00005760: 7574 7075 745f 7669 6465 6f20 0300 0073  utput_video ...s
+00005770: 1200 0000 0002 0601 0201 0601 1201 0201  ................
+00005780: 0201 02fa 0608 7a29 7461 6767 6564 5f76  ......z)tagged_v
+00005790: 6964 656f 5f6f 7574 7075 742e 3c6c 6f63  ideo_output.<loc
+000057a0: 616c 733e 2e6f 7574 7075 745f 7669 6465  als>.output_vide
+000057b0: 6f72 9200 0000 7a52 5669 6465 6f20 6f75  or....zRVideo ou
+000057c0: 7470 7574 206d 7573 7420 6265 2065 6974  tput must be eit
+000057d0: 6865 7220 2761 6c6c 2720 6f72 2061 206c  her 'all' or a l
+000057e0: 6973 7420 7769 7468 2074 6865 206e 616d  ist with the nam
+000057f0: 6573 206f 6620 7468 6520 7669 6465 6f73  es of the videos
+00005800: 2074 6f20 7265 6e64 6572 2901 da05 746f   to render)...to
+00005810: 7461 6cda 0974 6872 6561 6469 6e67 2901  tal..threading).
+00005820: 7207 0100 0063 0100 0000 0000 0000 0000  r....c..........
+00005830: 0000 0200 0000 0300 0000 3300 0000 731a  ..........3...s.
+00005840: 0000 007c 005d 127d 0174 0088 0083 017c  ...|.].}.t.....|
+00005850: 0183 0156 0001 0071 0264 0053 0072 e000  ...V...q.d.S.r..
+00005860: 0000 2901 7202 0000 0029 0272 1f00 0000  ..).r....).r....
+00005870: da03 6b65 7929 0172 0b01 0000 7222 0000  ..key).r....r"..
+00005880: 0072 2300 0000 72ce 0000 0037 0300 0072  .r#...r....7...r
+00005890: 5400 0000 7a26 7461 6767 6564 5f76 6964  T...z&tagged_vid
+000058a0: 656f 5f6f 7574 7075 742e 3c6c 6f63 616c  eo_output.<local
+000058b0: 733e 2e3c 6765 6e65 7870 723e 4e29 0a72  s>.<genexpr>N).r
+000058c0: 2500 0000 7227 0000 0072 ef00 0000 72f0  %...r'...r....r.
+000058d0: 0000 00da 0e41 7474 7269 6275 7465 4572  .....AttributeEr
+000058e0: 726f 7272 0c00 0000 72f6 0000 0072 0400  rorr....r....r..
+000058f0: 0000 7203 0000 00da 0563 6c6f 7365 2908  ..r......close).
+00005900: 7203 0100 0072 0101 0000 7204 0100 0072  r....r....r....r
+00005910: 0501 0000 7206 0100 0072 0701 0000 72c1  ....r....r....r.
+00005920: 0000 005a 0876 6964 5f69 6478 7372 2200  ...Z.vid_idxsr".
+00005930: 0000 2907 7203 0100 0072 0601 0000 7205  ..).r....r....r.
+00005940: 0100 0072 0b01 0000 72c1 0000 0072 0a01  ...r....r....r..
+00005950: 0000 7201 0100 0072 2300 0000 da13 7461  ..r....r#.....ta
+00005960: 6767 6564 5f76 6964 656f 5f6f 7574 7075  gged_video_outpu
+00005970: 740b 0300 0073 1800 0000 0015 160c 0a01  t....s..........
+00005980: 0601 0801 1002 0201 02ff 0404 0e01 0e01  ................
+00005990: 3601 7211 0100 00da 085f 5f6d 6169 6e5f  6.r......__main_
+000059a0: 5fda 0669 676e 6f72 657a 1941 6c6c 2d4e  _..ignorez.All-N
+000059b0: 614e 2073 6c69 6365 2065 6e63 6f75 6e74  aN slice encount
+000059c0: 6572 6564 2901 da07 6d65 7373 6167 6529  ered)...message)
+000059d0: 0146 2901 723c 0000 0029 0146 2903 4672  .F).r<...).F).Fr
+000059e0: 4700 0000 7260 0000 0029 0172 6000 0000  G...r`...).r`...
+000059f0: 2901 7260 0000 0029 0272 8000 0000 7201  ).r`...).r....r.
+00005a00: 0000 0029 0272 9600 0000 4629 0572 9200  ...).r....F).r..
+00005a10: 0000 4e46 7218 0000 004e 293e da07 5f5f  ..NFr....N)>..__
+00005a20: 646f 635f 5f72 ea00 0000 72ed 0000 0072  doc__r....r....r
+00005a30: 6e00 0000 da06 6a6f 626c 6962 7202 0000  n.....joblibr...
+00005a40: 0072 0300 0000 7204 0000 00da 0674 7970  .r....r......typ
+00005a50: 696e 6772 0500 0000 7206 0000 0072 0700  ingr....r....r..
+00005a60: 0000 7208 0000 00da 1073 6861 7065 6c79  ..r......shapely
+00005a70: 2e67 656f 6d65 7472 7972 0900 0000 720a  .geometryr....r.
+00005a80: 0000 00da 1573 6b6c 6561 726e 2e70 7265  .....sklearn.pre
+00005a90: 7072 6f63 6573 7369 6e67 720b 0000 0072  processingr....r
+00005aa0: 0c00 0000 da09 6974 6572 746f 6f6c 7372  ......itertoolsr
+00005ab0: 0d00 0000 da03 6376 32da 056e 756d 7079  ......cv2..numpy
+00005ac0: 721c 0000 00da 0670 616e 6461 7372 8e00  r......pandasr..
+00005ad0: 0000 da05 7265 6765 7872 f700 0000 da10  ....regexr......
+00005ae0: 736b 6c65 6172 6e2e 7069 7065 6c69 6e65  sklearn.pipeline
+00005af0: da07 736b 6c65 6172 6eda 0c64 6565 706f  ..sklearn..deepo
+00005b00: 662e 7574 696c 7372 d700 0000 da0f 6465  f.utilsr......de
+00005b10: 6570 6f66 2e70 6f73 745f 686f 63da 0770  epof.post_hoc..p
+00005b20: 726f 6a65 6374 7203 0100 00da 0a74 6162  rojectr......tab
+00005b30: 6c65 5f64 6963 7472 8f00 0000 7226 0000  le_dictr....r&..
+00005b40: 0072 a000 0000 72b6 0000 0072 5800 0000  .r....r....rX...
+00005b50: 7229 0000 0072 fd00 0000 722f 0000 0072  r)...r....r/...r
+00005b60: 3b00 0000 7245 0000 0072 5f00 0000 7269  ;...rE...r_...ri
+00005b70: 0000 00da 076e 6461 7272 6179 da08 7069  .....ndarray..pi
+00005b80: 7065 6c69 6e65 da08 5069 7065 6c69 6e65  peline..Pipeline
+00005b90: 7279 0000 0072 7f00 0000 7295 0000 0072  ry...r....r....r
+00005ba0: a500 0000 da04 6469 6374 72b4 0000 0072  ......dictr....r
+00005bb0: b900 0000 7202 0100 0072 1101 0000 da08  ....r....r......
+00005bc0: 5f5f 6e61 6d65 5f5f da0e 6669 6c74 6572  __name__..filter
+00005bd0: 7761 726e 696e 6773 7222 0000 0072 2200  warningsr"...r".
+00005be0: 0000 7222 0000 0072 2300 0000 da08 3c6d  ..r"...r#.....<m
+00005bf0: 6f64 756c 653e 0500 0000 7308 0100 0004  odule>....s.....
+00005c00: 0208 0108 0108 0114 0118 0110 010c 010c  ................
+00005c10: 010c 0208 0108 0108 0108 0108 0208 0108  ................
+00005c20: 030a 010a 010a 0404 0102 0102 0102 0102  ................
+00005c30: 0102 0104 f90c 3400 f702 0104 0102 0102  ......4.........
+00005c40: 0102 0102 0102 0102 0102 0102 0104 f60c  ................
+00005c50: 3508 0a0a 1400 fa02 0102 0104 0104 0102  5...............
+00005c60: 0102 0102 0104 f90c 3b00 0100 0100 f602  ........;.......
+00005c70: 0104 0102 0104 0104 0102 0102 0102 0102  ................
+00005c80: 0102 0102 f60c 5500 fd02 0104 0106 0102  ......U.........
+00005c90: 0104 fc0c 4500 fb02 0104 0104 0102 0102  ....E...........
+00005ca0: 0102 fb0c 2400 0100 fa02 0104 0104 0102  ....$...........
+00005cb0: 0102 0102 0102 0104 f90c 3b00 ff02 0108  ..........;.....
+00005cc0: 0104 fe0c 1a14 1c12 2202 0102 f702 0102  ........".......
+00005cd0: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00005ce0: 0104 f60c 7f00 7f00 0a00 0100 0100 0100  ................
+00005cf0: 0100 f902 0102 0102 010e 0102 0102 0102  ................
+00005d00: 0102 f90c 300a 02                        ....0..
```

### Comparing `deepof-0.5.0/deepof/__pycache__/data.cpython-39.pyc` & `deepof-0.5.1/deepof/__pycache__/data.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Jul 18 13:42:26 2023 UTC, .py size: 97568 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,4484 +1,4492 @@
-00000000: 610d 0d0a 0000 0000 c296 b664 207d 0100  a..........d }..
+00000000: 610d 0d0a 0000 0000 97e7 b764 e67d 0100  a..........d.}..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 ca01 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 d601 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6401 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6406 6c09 6d0a 5a0a 0100 6401  ..d.d.l.m.Z...d.
 00000070: 6407 6c0b 6d0c 5a0c 0100 6401 6408 6c0d  d.l.m.Z...d.d.l.
 00000080: 6d0e 5a0e 0100 6401 6409 6c0f 6d10 5a10  m.Z...d.d.l.m.Z.
-00000090: 6d11 5a11 6d12 5a12 6d13 5a13 0100 6401  m.Z.m.Z.m.Z...d.
-000000a0: 640a 6c14 6d14 5a14 0100 6401 640b 6c15  d.l.m.Z...d.d.l.
-000000b0: 6d15 5a15 0100 6401 640c 6c16 6d17 5a17  m.Z...d.d.l.m.Z.
-000000c0: 6d18 5a18 6d19 5a19 0100 6401 640d 6c16  m.Z.m.Z...d.d.l.
-000000d0: 6d1a 5a1a 6d1b 5a1b 6d1c 5a1c 6d17 5a17  m.Z.m.Z.m.Z.m.Z.
-000000e0: 0100 6401 640e 6c1d 5a1d 6401 640e 6c1e  ..d.d.l.Z.d.d.l.
-000000f0: 5a1e 6401 640e 6c1f 5a1f 6401 640e 6c20  Z.d.d.l.Z.d.d.l 
-00000100: 6d21 5a22 0100 6401 640e 6c23 5a24 6401  m!Z"..d.d.l#Z$d.
-00000110: 640e 6c25 5a26 6401 640e 6c27 5a27 6401  d.l%Z&d.d.l'Z'd.
-00000120: 640e 6c28 5a29 6401 640e 6c2a 5a2a 6401  d.l(Z)d.d.l*Z*d.
-00000130: 640e 6c2b 5a2b 6401 640e 6c2c 5a2c 6401  d.l+Z+d.d.l,Z,d.
-00000140: 640e 6c07 5a07 6401 640e 6c2d 5a2e 6401  d.l.Z.d.d.l-Z.d.
-00000150: 640e 6c2f 5a2f 6401 640e 6c30 5a30 6401  d.l/Z/d.d.l0Z0d.
-00000160: 640e 6c31 5a32 6401 640e 6c33 5a32 6401  d.l1Z2d.d.l3Z2d.
-00000170: 640e 6c34 5a32 6401 640e 6c35 5a32 6401  d.l4Z2d.d.l5Z2d.
-00000180: 640e 6c36 5a32 6518 640f 6517 8302 5a37  d.l6Z2e.d.e...Z7
-00000190: 6518 6410 6517 8302 5a38 6518 6411 6517  e.d.e...Z8e.d.e.
-000001a0: 8302 5a39 653a 6538 6412 9c02 6413 6414  ..Z9e:e8d...d.d.
-000001b0: 8404 5a3b 4700 6415 6416 8400 6416 8302  ..Z;G.d.d...d...
-000001c0: 5a3c 4700 6417 6418 8400 6418 8302 5a3d  Z<G.d.d...d...Z=
-000001d0: 4700 6419 641a 8400 641a 653e 8303 5a3f  G.d.d...d.e>..Z?
-000001e0: 6540 641b 6b02 9001 72c6 641c 6527 6a41  e@d.k...r.d.e'jA
-000001f0: 641d 3c00 640e 5300 291e 61c9 0200 0044  d.<.d.S.).a....D
-00000200: 6174 6120 7374 7275 6374 7572 6573 2066  ata structures f
-00000210: 6f72 2070 7265 7072 6f63 6573 7369 6e67  or preprocessing
-00000220: 2061 6e64 2077 7261 6e67 6c69 6e67 206f   and wrangling o
-00000230: 6620 444c 4320 6f75 7470 7574 2064 6174  f DLC output dat
-00000240: 612e 2054 6869 7320 6973 2074 6865 206d  a. This is the m
-00000250: 6169 6e20 6d6f 6475 6c65 2068 616e 646c  ain module handl
-00000260: 6564 2062 7920 7468 6520 7573 6572 2e0a  ed by the user..
-00000270: 0a54 6865 7265 2061 7265 2074 6872 6565  .There are three
-00000280: 206d 6169 6e20 6461 7461 2073 7472 7563   main data struc
-00000290: 7475 7265 7320 746f 2070 6179 2061 7474  tures to pay att
-000002a0: 656e 7469 6f6e 2074 6f3a 0a2d 203a 636c  ention to:.- :cl
-000002b0: 6173 733a 607e 6465 6570 6f66 2e64 6174  ass:`~deepof.dat
-000002c0: 612e 5072 6f6a 6563 7460 2c20 7768 6963  a.Project`, whic
-000002d0: 6820 7365 7276 6573 2061 7320 6120 636f  h serves as a co
-000002e0: 6e66 6967 7572 6174 696f 6e20 6875 6220  nfiguration hub 
-000002f0: 666f 7220 7468 6520 7768 6f6c 6520 7069  for the whole pi
-00000300: 7065 6c69 6e65 0a2d 203a 636c 6173 733a  peline.- :class:
-00000310: 607e 6465 6570 6f66 2e64 6174 612e 436f  `~deepof.data.Co
-00000320: 6f72 6469 6e61 7465 7360 2c20 7768 6963  ordinates`, whic
-00000330: 6820 6163 7473 2061 7320 616e 2069 6e74  h acts as an int
-00000340: 6572 6d65 6469 6172 7920 6265 7477 6565  ermediary betwee
-00000350: 6e20 7072 6f6a 6563 7420 636f 6e66 6967  n project config
-00000360: 7572 6174 696f 6e20 616e 6420 6461 7461  uration and data
-00000370: 2c20 616e 6420 636f 6e74 6169 6e73 0a61  , and contains.a
-00000380: 2070 6c65 7468 6f72 6120 6f66 2070 726f   plethora of pro
-00000390: 6365 7373 696e 6720 6d65 7468 6f64 7320  cessing methods 
-000003a0: 746f 2061 7070 6c79 2c20 616e 640a 2d20  to apply, and.- 
-000003b0: 3a63 6c61 7373 3a60 7e64 6565 706f 662e  :class:`~deepof.
-000003c0: 6461 7461 2e54 6162 6c65 4469 6374 602c  data.TableDict`,
-000003d0: 2077 6869 6368 2069 7320 7468 6520 6d61   which is the ma
-000003e0: 696e 2064 6174 6120 7374 7275 6374 7572  in data structur
-000003f0: 6520 746f 2073 746f 7265 2074 6865 2064  e to store the d
-00000400: 6174 612c 2068 6176 696e 6720 6578 7065  ata, having expe
-00000410: 7269 6d65 6e74 2049 4473 2061 7320 6b65  riment IDs as ke
-00000420: 7973 0a61 6e64 2070 726f 6365 7373 6564  ys.and processed
-00000430: 2074 696d 652d 7365 7269 6573 2061 7320   time-series as 
-00000440: 7661 6c75 6573 2069 6e20 6120 6469 6374  values in a dict
-00000450: 696f 6e61 7279 2d6c 696b 6520 6f62 6a65  ionary-like obje
-00000460: 6374 2e0a 0a46 6f72 2061 2064 6574 6169  ct...For a detai
-00000470: 6c65 6420 7475 746f 7269 616c 206f 6e20  led tutorial on 
-00000480: 686f 7720 746f 2075 7365 2074 6869 7320  how to use this 
-00000490: 6d6f 6475 6c65 2c20 7365 6520 7468 6520  module, see the 
-000004a0: 6164 7661 6e63 6564 2074 7574 6f72 6961  advanced tutoria
-000004b0: 6c73 2069 6e20 7468 6520 6d61 696e 2073  ls in the main s
-000004c0: 6563 7469 6f6e 2e0a e900 0000 0029 01da  ection.......)..
-000004d0: 0b64 6566 6175 6c74 6469 6374 2901 da11  .defaultdict)...
-000004e0: 7265 736f 7572 6365 5f66 696c 656e 616d  resource_filenam
-000004f0: 6529 01da 0750 6f6c 7967 6f6e 2901 da06  e)...Polygon)...
-00000500: 726d 7472 6565 2901 da11 7261 6e64 6f6d  rmtree)...random
-00000510: 5f70 726f 6a65 6374 696f 6e29 01da 094b  _projection)...K
-00000520: 6572 6e65 6c50 4341 2901 da04 5453 4e45  ernelPCA)...TSNE
-00000530: 2904 da0c 4d69 6e4d 6178 5363 616c 6572  )...MinMaxScaler
-00000540: da0e 5374 616e 6461 7264 5363 616c 6572  ..StandardScaler
-00000550: da0c 526f 6275 7374 5363 616c 6572 da0c  ..RobustScaler..
-00000560: 4c61 6265 6c45 6e63 6f64 6572 2901 da04  LabelEncoder)...
-00000570: 7469 6d65 2901 da04 7471 646d 2903 da03  time)...tqdm)...
-00000580: 416e 79da 074e 6577 5479 7065 da05 556e  Any..NewType..Un
-00000590: 696f 6e29 04da 0444 6963 74da 044c 6973  ion)...Dict..Lis
-000005a0: 74da 0554 7570 6c65 720f 0000 004e da0e  t..Tupler....N..
-000005b0: 6465 6570 6f66 5f70 726f 6a65 6374 da12  deepof_project..
-000005c0: 6465 6570 6f66 5f63 6f6f 7264 696e 6174  deepof_coordinat
-000005d0: 6573 da11 6465 6570 6f66 5f74 6162 6c65  es..deepof_table
-000005e0: 5f64 6963 7429 02da 0c70 726f 6a65 6374  _dict)...project
-000005f0: 5f70 6174 68da 0672 6574 7572 6e63 0100  _path..returnc..
-00000600: 0000 0000 0000 0000 0000 0300 0000 0800  ................
-00000610: 0000 4300 0000 7356 0000 0074 0074 016a  ..C...sV...t.t.j
-00000620: 02a0 037c 0064 0164 02a1 0364 0383 028f  ...|.d.d...d....
-00000630: 1a7d 0174 04a0 057c 01a1 017d 0257 0064  .}.t...|...}.W.d
-00000640: 0404 0004 0083 0301 006e 1031 0073 3630  .........n.1.s60
-00000650: 0001 0001 0001 0059 0001 0074 016a 02a0  .......Y...t.j..
-00000660: 067c 00a1 0164 0519 007c 025f 077c 0253  .|...d...|._.|.S
-00000670: 0029 067a a54c 6f61 6420 6120 7072 652d  .).z.Load a pre-
-00000680: 7361 7665 6420 7069 636b 6c65 6420 436f  saved pickled Co
-00000690: 6f72 6469 6e61 7465 7320 6f62 6a65 6374  ordinates object
-000006a0: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
-000006b0: 2020 2020 2070 726f 6a65 6374 5f70 6174       project_pat
-000006c0: 6820 2873 7472 293a 206e 616d 6520 6f66  h (str): name of
-000006d0: 2074 6865 2066 696c 6520 746f 206c 6f61   the file to loa
-000006e0: 642e 0a0a 2020 2020 5265 7475 726e 733a  d...    Returns:
-000006f0: 0a20 2020 2020 2020 2050 7265 2d72 756e  .        Pre-run
-00000700: 2063 6f6f 7264 696e 6174 6573 206f 626a   coordinates obj
-00000710: 6563 742e 0a0a 2020 2020 da0b 436f 6f72  ect...    ..Coor
-00000720: 6469 6e61 7465 737a 1664 6565 706f 665f  dinatesz.deepof_
-00000730: 636f 6f72 6469 6e61 7465 732e 706b 6cda  coordinates.pkl.
-00000740: 0272 624e 7201 0000 0029 08da 046f 7065  .rbNr....)...ope
-00000750: 6eda 026f 73da 0470 6174 68da 046a 6f69  n..os..path..joi
-00000760: 6eda 0670 6963 6b6c 65da 046c 6f61 64da  n..pickle..load.
-00000770: 0573 706c 6974 da0d 5f70 726f 6a65 6374  .split.._project
-00000780: 5f70 6174 6829 0372 1800 0000 da06 6861  _path).r......ha
-00000790: 6e64 6c65 da0b 636f 6f72 6469 6e61 7465  ndle..coordinate
-000007a0: 73a9 0072 2600 0000 fa3a 2f55 7365 7273  s..r&....:/Users
-000007b0: 2f6c 7563 6173 5f6d 6972 616e 6461 2f50  /lucas_miranda/P
-000007c0: 7963 6861 726d 5072 6f6a 6563 7473 2f64  ycharmProjects/d
-000007d0: 6565 706f 662f 6465 6570 6f66 2f64 6174  eepof/deepof/dat
-000007e0: 612e 7079 da0c 6c6f 6164 5f70 726f 6a65  a.py..load_proje
-000007f0: 6374 4100 0000 730e 0000 0000 0a02 0110  ctA...s.........
-00000800: ff04 0202 0128 0212 0172 2800 0000 6300  .....(...r(...c.
-00000810: 0000 0000 0000 0000 0000 0000 0000 0015  ................
-00000820: 0000 0040 0000 0073 5601 0000 6500 5a01  ...@...sV...e.Z.
-00000830: 6400 5a02 6401 5a03 6402 6403 6404 6405  d.Z.d.Z.d.d.d.d.
-00000840: 6504 6406 6701 8301 6402 6407 6408 6409  e.d.g...d.d.d.d.
-00000850: 640a 640b 640c 6505 6a06 a007 640d a101  d.d.d.e.j...d...
-00000860: 6402 6402 640e 640f 6410 640e 6613 6508  d.d.d.d.d.d.f.e.
-00000870: 6509 6509 650a 6508 650b 650a 650c 650c  e.e.e.e.e.e.e.e.
-00000880: 650d 6509 6509 6509 6509 6509 650d 6509  e.e.e.e.e.e.e.e.
-00000890: 6509 650c 6411 9c13 6412 6413 8405 5a0e  e.e.d...d.d...Z.
-000008a0: 6414 6415 8400 5a0f 6416 6417 8400 5a10  d.d...Z.d.d...Z.
-000008b0: 6418 6419 8400 5a11 6512 641a 641b 8400  d.d...Z.e.d.d...
-000008c0: 8301 5a13 6512 641c 641d 8400 8301 5a14  ..Z.e.d.d.....Z.
-000008d0: 6512 641e 641f 8400 8301 5a15 6434 6516  e.d.d.....Z.d4e.
-000008e0: 650a 6517 6a18 6421 9c03 6422 6423 8405  e.e.j.d!..d"d#..
-000008f0: 5a19 6435 650a 651a 6424 9c02 6425 6426  Z.d5e.e.d$..d%d&
-00000900: 8405 5a1b 6436 650b 650a 650b 6427 9c03  ..Z.d6e.e.e.d'..
-00000910: 6428 6429 8405 5a1c 6437 650b 650a 650b  d(d)..Z.d7e.e.e.
-00000920: 6427 9c03 642a 642b 8405 5a1d 6438 650b  d'..d*d+..Z.d8e.
-00000930: 650a 650b 6427 9c03 642c 642d 8405 5a1e  e.e.d'..d,d-..Z.
-00000940: 6439 650a 650a 651f 642e 9c03 642f 6430  d9e.e.e.d...d/d0
-00000950: 8405 5a20 6513 6a21 6431 641b 8400 8301  ..Z e.j!d1d.....
-00000960: 5a13 6514 6a21 6432 641d 8400 8301 5a14  Z.e.j!d2d.....Z.
-00000970: 6515 6a21 6433 641f 8400 8301 5a15 6402  e.j!d3d.....Z.d.
-00000980: 5300 293a da07 5072 6f6a 6563 747a 8843  S.):..Projectz.C
-00000990: 6c61 7373 2066 6f72 206c 6f61 6469 6e67  lass for loading
-000009a0: 2061 6e64 2070 7265 7072 6f63 6573 7369   and preprocessi
-000009b0: 6e67 2044 4c43 2064 6174 6120 6f66 2069  ng DLC data of i
-000009c0: 6e64 6976 6964 7561 6c20 616e 6420 6d75  ndividual and mu
-000009d0: 6c74 6970 6c65 2061 6e69 6d61 6c73 2e0a  ltiple animals..
-000009e0: 0a20 2020 2041 6c6c 206d 6169 6e20 636f  .    All main co
-000009f0: 6d70 7574 6174 696f 6e73 2061 7265 2068  mputations are h
-00000a00: 616e 646c 6564 2066 726f 6d20 6865 7265  andled from here
-00000a10: 2e0a 0a20 2020 204e 7a10 706f 6c79 676f  ...    Nz.polygo
-00000a20: 6e61 6c2d 6d61 6e75 616c da09 6465 6570  nal-manual..deep
-00000a30: 6f66 5f31 34e9 fa00 0000 da00 54e9 0500  of_14.......T...
-00000a40: 0000 e903 0000 0067 0000 0000 0000 e83f  .......g.......?
-00000a50: da0d 6d6f 7573 655f 746f 7076 6965 7772  ..mouse_topviewr
-00000a60: 1500 0000 da01 2ee9 0100 0000 da0a 6175  ..............au
-00000a70: 746f 6465 7465 6374 7a04 2e6d 7034 2913  todetectz..mp4).
-00000a80: da0a 616e 696d 616c 5f69 6473 da05 6172  ..animal_ids..ar
-00000a90: 656e 61da 0e62 6f64 7970 6172 745f 6772  ena..bodypart_gr
-00000aa0: 6170 68da 1b65 6e61 626c 655f 6974 6572  aph..enable_iter
-00000ab0: 6174 6976 655f 696d 7075 7461 7469 6f6e  ative_imputation
-00000ac0: da11 6578 636c 7564 655f 626f 6479 7061  ..exclude_bodypa
-00000ad0: 7274 73da 0e65 7870 5f63 6f6e 6469 7469  rts..exp_conditi
-00000ae0: 6f6e 73da 1469 6e74 6572 706f 6c61 7465  ons..interpolate
-00000af0: 5f6f 7574 6c69 6572 73da 1369 6e74 6572  _outliers..inter
-00000b00: 706f 6c61 7469 6f6e 5f6c 696d 6974 da11  polation_limit..
-00000b10: 696e 7465 7270 6f6c 6174 696f 6e5f 7374  interpolation_st
-00000b20: 64da 0e6c 696b 656c 6968 6f6f 645f 746f  d..likelihood_to
-00000b30: 6cda 056d 6f64 656c da0c 7072 6f6a 6563  l..model..projec
-00000b40: 745f 6e61 6d65 7218 0000 00da 0a76 6964  t_namer......vid
-00000b50: 656f 5f70 6174 68da 0a74 6162 6c65 5f70  eo_path..table_p
-00000b60: 6174 68da 0c73 6d6f 6f74 685f 616c 7068  ath..smooth_alph
-00000b70: 61da 0c74 6162 6c65 5f66 6f72 6d61 74da  a..table_format.
-00000b80: 0c76 6964 656f 5f66 6f72 6d61 74da 0b76  .video_format..v
-00000b90: 6964 656f 5f73 6361 6c65 6314 0000 0000  ideo_scalec.....
-00000ba0: 0000 0000 0000 0015 0000 0005 0000 0003  ................
-00000bb0: 0000 0073 5801 0000 7c0d 8800 5f00 7c0c  ...sX...|..._.|.
-00000bc0: 8800 5f01 7c0e 8800 5f02 7c0f 8800 5f03  .._.|..._.|..._.
-00000bd0: 7404 7405 6401 8302 8800 5f06 7c11 8800  t.t.d....._.|...
-00000be0: 5f07 8800 6a07 6402 6b02 726c 6403 6404  _...j.d.k.rld.d.
-00000bf0: 8400 7408 a009 8800 6a03 a101 4400 8301  ..t.....j...D...
-00000c00: 6405 1900 7d14 6406 7c14 7600 725e 6406  d...}.d.|.v.r^d.
-00000c10: 8800 5f07 6e0e 6407 7c14 7600 726c 6407  .._.n.d.|.v.rld.
-00000c20: 8800 5f07 740a 8701 6601 6408 6404 8408  .._.t...f.d.d...
-00000c30: 7408 a009 8800 6a02 a101 4400 8301 8301  t.....j...D.....
-00000c40: 8800 5f0b 740a 8700 6601 6409 6404 8408  .._.t...f.d.d...
-00000c50: 7408 a009 8800 6a03 a101 4400 8301 8301  t.....j...D.....
-00000c60: 8800 5f0c 740d 8800 6a0b 8301 740d 8800  .._.t...j...t...
-00000c70: 6a0c 8301 6b02 73c8 4a00 640a 8301 8201  j...k.s.J.d.....
-00000c80: 7c02 8800 5f0e 7c13 8800 5f0f 640b 8800  |..._.|..._.d...
-00000c90: 5f10 640c 8800 5f11 7c01 640b 7501 72ec  _.d..._.|.d.u.r.
-00000ca0: 7c01 6e04 640d 6701 8800 5f12 640c 8800  |.n.d.g..._.d...
-00000cb0: 5f13 7c03 8800 5f14 640b 8800 5f15 640e  _.|..._.d..._.d.
-00000cc0: 8800 5f16 640f 8800 5f17 7c06 8800 5f18  .._.d..._.|..._.
-00000cd0: 7c07 8800 5f19 7c08 8800 5f1a 7c09 8800  |..._.|..._.|...
-00000ce0: 5f1b 7c0a 8800 5f1c 7c0b 8800 5f1d 7c10  _.|..._.|..._.|.
-00000cf0: 8800 5f1e 640b 8800 5f1f 8801 8800 5f20  .._.d..._....._ 
-00000d00: 7c04 8800 5f21 7c05 8800 5f22 640b 5300  |..._!|..._"d.S.
-00000d10: 2910 611b 0800 0049 6e69 7469 616c 697a  ).a....Initializ
-00000d20: 6520 6120 5072 6f6a 6563 7420 6f62 6a65  e a Project obje
-00000d30: 6374 2e0a 0a20 2020 2020 2020 2041 7267  ct...        Arg
-00000d40: 733a 0a20 2020 2020 2020 2020 2020 2061  s:.            a
-00000d50: 6e69 6d61 6c5f 6964 7320 286c 6973 7429  nimal_ids (list)
-00000d60: 3a20 6c69 7374 206f 6620 616e 696d 616c  : list of animal
-00000d70: 2069 6473 2e0a 2020 2020 2020 2020 2020   ids..          
-00000d80: 2020 6172 656e 6120 2873 7472 293a 2061    arena (str): a
-00000d90: 7265 6e61 2074 7970 652e 2043 616e 2062  rena type. Can b
-00000da0: 6520 6f6e 6520 6f66 2022 6369 7263 756c  e one of "circul
-00000db0: 6172 2d61 7574 6f64 6574 6563 7422 2c20  ar-autodetect", 
-00000dc0: 2263 6972 6375 6c61 722d 6d61 6e75 616c  "circular-manual
-00000dd0: 222c 206f 7220 2270 6f6c 7967 6f6e 2d6d  ", or "polygon-m
-00000de0: 616e 7561 6c22 2e0a 2020 2020 2020 2020  anual"..        
-00000df0: 2020 2020 626f 6479 7061 7274 5f67 7261      bodypart_gra
-00000e00: 7068 2028 7374 7229 3a20 626f 6479 2070  ph (str): body p
-00000e10: 6172 7420 7363 6865 6d65 2074 6f20 7573  art scheme to us
-00000e20: 6520 666f 7220 7468 6520 616e 616c 7973  e for the analys
-00000e30: 6973 2e20 4465 6661 756c 7473 2074 6f20  is. Defaults to 
-00000e40: 4e6f 6e65 2c20 696e 2077 6869 6368 2063  None, in which c
-00000e50: 6173 6520 7468 6520 7072 6f67 7261 6d20  ase the program 
-00000e60: 7769 6c6c 2061 7474 656d 7074 2074 6f20  will attempt to 
-00000e70: 7365 6c65 6374 2069 7420 6175 746f 6d61  select it automa
-00000e80: 7469 6361 6c6c 7920 6261 7365 6420 6f6e  tically based on
-00000e90: 2074 6865 2061 7661 696c 6162 6c65 2062   the available b
-00000ea0: 6f64 7920 7061 7274 732e 0a20 2020 2020  ody parts..     
-00000eb0: 2020 2020 2020 2065 6e61 626c 655f 6974         enable_it
-00000ec0: 6572 6174 6976 655f 696d 7075 7461 7469  erative_imputati
-00000ed0: 6f6e 2028 626f 6f6c 293a 2077 6865 7468  on (bool): wheth
-00000ee0: 6572 2074 6f20 7573 6520 6974 6572 6174  er to use iterat
-00000ef0: 6976 6520 696d 7075 7461 7469 6f6e 2066  ive imputation f
-00000f00: 6f72 206f 6363 6c75 6465 6420 626f 6479  or occluded body
-00000f10: 2070 6172 7473 2e20 5265 636f 6d6d 656e   parts. Recommen
-00000f20: 6465 6420 6966 2073 6576 6572 616c 2061  ded if several a
-00000f30: 6e69 6d61 6c73 2061 7265 2070 7265 7365  nimals are prese
-00000f40: 6e74 2c20 6275 7420 736c 6f77 6572 2e0a  nt, but slower..
-00000f50: 2020 2020 2020 2020 2020 2020 6578 636c              excl
-00000f60: 7564 655f 626f 6479 7061 7274 7320 286c  ude_bodyparts (l
-00000f70: 6973 7429 3a20 6c69 7374 206f 6620 626f  ist): list of bo
-00000f80: 6479 7061 7274 7320 746f 2065 7863 6c75  dyparts to exclu
-00000f90: 6465 2066 726f 6d20 616e 616c 7973 6973  de from analysis
-00000fa0: 2e0a 2020 2020 2020 2020 2020 2020 6578  ..            ex
-00000fb0: 705f 636f 6e64 6974 696f 6e73 2028 6469  p_conditions (di
-00000fc0: 6374 293a 2064 6963 7469 6f6e 6172 7920  ct): dictionary 
-00000fd0: 7769 7468 2065 7870 6572 696d 656e 7420  with experiment 
-00000fe0: 4944 7320 6173 206b 6579 7320 616e 6420  IDs as keys and 
-00000ff0: 6578 7065 7269 6d65 6e74 616c 2063 6f6e  experimental con
-00001000: 6469 7469 6f6e 7320 6173 2076 616c 7565  ditions as value
-00001010: 732e 0a20 2020 2020 2020 2020 2020 2069  s..            i
-00001020: 6e74 6572 706f 6c61 7465 5f6f 7574 6c69  nterpolate_outli
-00001030: 6572 7320 2862 6f6f 6c29 3a20 7768 6574  ers (bool): whet
-00001040: 6865 7220 746f 2069 6e74 6572 706f 6c61  her to interpola
-00001050: 7465 206d 6973 7369 6e67 2064 6174 612e  te missing data.
-00001060: 0a20 2020 2020 2020 2020 2020 2069 6e74  .            int
-00001070: 6572 706f 6c61 7469 6f6e 5f6c 696d 6974  erpolation_limit
-00001080: 2028 696e 7429 3a20 6d61 7869 6d75 6d20   (int): maximum 
-00001090: 6e75 6d62 6572 206f 6620 6d69 7373 696e  number of missin
-000010a0: 6720 6672 616d 6573 2074 6f20 696e 7465  g frames to inte
-000010b0: 7270 6f6c 6174 652e 0a20 2020 2020 2020  rpolate..       
-000010c0: 2020 2020 2069 6e74 6572 706f 6c61 7469       interpolati
-000010d0: 6f6e 5f73 7464 2028 696e 7429 3a20 6d61  on_std (int): ma
-000010e0: 7869 6d75 6d20 6e75 6d62 6572 206f 6620  ximum number of 
-000010f0: 7374 616e 6461 7264 2064 6576 6961 7469  standard deviati
-00001100: 6f6e 7320 746f 2069 6e74 6572 706f 6c61  ons to interpola
-00001110: 7465 2e0a 2020 2020 2020 2020 2020 2020  te..            
-00001120: 6c69 6b65 6c69 686f 6f64 5f74 6f6c 2028  likelihood_tol (
-00001130: 666c 6f61 7429 3a20 6c69 6b65 6c69 686f  float): likeliho
-00001140: 6f64 2074 6872 6573 686f 6c64 2066 6f72  od threshold for
-00001150: 206f 7574 6c69 6572 2064 6574 6563 7469   outlier detecti
-00001160: 6f6e 2e0a 2020 2020 2020 2020 2020 2020  on..            
-00001170: 6d6f 6465 6c20 2873 7472 293a 206d 6f64  model (str): mod
-00001180: 656c 2074 6f20 7573 6520 666f 7220 706f  el to use for po
-00001190: 7365 2065 7374 696d 6174 696f 6e2e 2044  se estimation. D
-000011a0: 6566 6175 6c74 7320 746f 2027 6d6f 7573  efaults to 'mous
-000011b0: 655f 746f 7076 6965 7727 2028 6173 2064  e_topview' (as d
-000011c0: 6573 6372 6962 6564 2069 6e20 7468 6520  escribed in the 
-000011d0: 646f 6375 6d65 6e74 6174 696f 6e29 2e0a  documentation)..
-000011e0: 2020 2020 2020 2020 2020 2020 7072 6f6a              proj
-000011f0: 6563 745f 6e61 6d65 2028 7374 7229 3a20  ect_name (str): 
-00001200: 6e61 6d65 206f 6620 7468 6520 6375 7272  name of the curr
-00001210: 656e 7420 7072 6f6a 6563 742e 0a20 2020  ent project..   
-00001220: 2020 2020 2020 2020 2070 726f 6a65 6374           project
-00001230: 5f70 6174 6820 2873 7472 293a 2070 6174  _path (str): pat
-00001240: 6820 746f 2074 6865 2066 6f6c 6465 7220  h to the folder 
-00001250: 636f 6e74 6169 6e69 6e67 2074 6865 2044  containing the D
-00001260: 4c43 206f 7574 7075 7420 6461 7461 2e0a  LC output data..
-00001270: 2020 2020 2020 2020 2020 2020 7669 6465              vide
-00001280: 6f5f 7061 7468 2028 7374 7229 3a20 7061  o_path (str): pa
-00001290: 7468 2077 6865 7265 2074 6f20 6669 6e64  th where to find
-000012a0: 2074 6865 2076 6964 656f 7320 746f 2075   the videos to u
-000012b0: 7365 2e20 4966 206e 6f74 2073 7065 6369  se. If not speci
-000012c0: 6669 6564 2c20 6465 6570 6f66 2c20 6173  fied, deepof, as
-000012d0: 7375 6d65 7320 7468 6579 2061 7265 2069  sumes they are i
-000012e0: 6e20 796f 7572 2070 726f 6a65 6374 2070  n your project p
-000012f0: 6174 682e 0a20 2020 2020 2020 2020 2020  ath..           
-00001300: 2074 6162 6c65 5f70 6174 6820 2873 7472   table_path (str
-00001310: 293a 2070 6174 6820 7768 6572 6520 746f  ): path where to
-00001320: 2066 696e 6420 7468 6520 7472 6163 6b73   find the tracks
-00001330: 2074 6f20 7573 652e 2049 6620 6e6f 7420   to use. If not 
-00001340: 7370 6563 6966 6965 642c 2064 6565 706f  specified, deepo
-00001350: 662c 2061 7373 756d 6573 2074 6865 7920  f, assumes they 
-00001360: 6172 6520 696e 2079 6f75 7220 7072 6f6a  are in your proj
-00001370: 6563 7420 7061 7468 2e0a 2020 2020 2020  ect path..      
-00001380: 2020 2020 2020 736d 6f6f 7468 5f61 6c70        smooth_alp
-00001390: 6861 2028 666c 6f61 7429 3a20 736d 6f6f  ha (float): smoo
-000013a0: 7468 696e 6720 696e 7465 6e73 6974 792e  thing intensity.
-000013b0: 2054 6865 2068 6967 6865 7220 7468 6520   The higher the 
-000013c0: 7661 6c75 652c 2074 6865 206d 6f72 6520  value, the more 
-000013d0: 736d 6f6f 7468 696e 672e 0a20 2020 2020  smoothing..     
-000013e0: 2020 2020 2020 2074 6162 6c65 5f66 6f72         table_for
-000013f0: 6d61 7420 2873 7472 293a 2066 6f72 6d61  mat (str): forma
-00001400: 7420 6f66 2074 6865 2074 6162 6c65 2e20  t of the table. 
-00001410: 4465 6661 756c 7473 2074 6f20 2761 7574  Defaults to 'aut
-00001420: 6f64 6574 6563 7427 2c20 6275 7420 6361  odetect', but ca
-00001430: 6e20 6265 2073 6574 2074 6f20 2263 7376  n be set to "csv
-00001440: 2220 6f72 2022 6835 222e 0a20 2020 2020  " or "h5"..     
-00001450: 2020 2020 2020 2076 6964 656f 5f66 6f72         video_for
-00001460: 6d61 7420 2873 7472 293a 2076 6964 656f  mat (str): video
-00001470: 2066 6f72 6d61 742e 2044 6566 6175 6c74   format. Default
-00001480: 7320 746f 2027 2e6d 7034 272e 0a20 2020  s to '.mp4'..   
-00001490: 2020 2020 2020 2020 2076 6964 656f 5f73           video_s
-000014a0: 6361 6c65 2028 696e 7429 3a20 6469 616d  cale (int): diam
-000014b0: 6574 6572 206f 6620 7468 6520 6172 656e  eter of the aren
-000014c0: 6120 696e 206d 6d20 2869 6620 7468 6520  a in mm (if the 
-000014d0: 6172 656e 6120 6973 2072 6f75 6e64 2920  arena is round) 
-000014e0: 6f72 206c 656e 6774 6820 6f66 2074 6865  or length of the
-000014f0: 2066 6972 7374 2073 7065 6369 6669 6564   first specified
-00001500: 2061 7265 6e61 2073 6964 6520 2869 6620   arena side (if 
-00001510: 7468 6520 6172 656e 6120 6973 2070 6f6c  the arena is pol
-00001520: 7967 6f6e 616c 292e 0a0a 2020 2020 2020  ygonal)...      
-00001530: 2020 da0e 7472 6169 6e65 645f 6d6f 6465    ..trained_mode
-00001540: 6c73 7232 0000 0063 0100 0000 0000 0000  lsr2...c........
-00001550: 0000 0000 0200 0000 0500 0000 5300 0000  ............S...
-00001560: 731a 0000 0067 007c 005d 127d 017c 01a0  s....g.|.].}.|..
-00001570: 0064 00a1 0173 047c 0191 0271 0453 00a9  .d...s.|...q.S..
-00001580: 0172 3000 0000 a901 da0a 7374 6172 7473  .r0.......starts
-00001590: 7769 7468 a902 da02 2e30 da01 6972 2600  with.....0..ir&.
-000015a0: 0000 7226 0000 0072 2700 0000 da0a 3c6c  ..r&...r'.....<l
-000015b0: 6973 7463 6f6d 703e 9300 0000 f300 0000  istcomp>........
-000015c0: 007a 2450 726f 6a65 6374 2e5f 5f69 6e69  .z$Project.__ini
-000015d0: 745f 5f2e 3c6c 6f63 616c 733e 2e3c 6c69  t__.<locals>.<li
-000015e0: 7374 636f 6d70 3e72 0100 0000 fa03 2e68  stcomp>r.......h
-000015f0: 35fa 042e 6373 7663 0100 0000 0000 0000  5...csvc........
-00001600: 0000 0000 0200 0000 0500 0000 1300 0000  ................
-00001610: 7324 0000 0067 007c 005d 1c7d 017c 01a0  s$...g.|.].}.|..
-00001620: 0088 00a1 0172 047c 01a0 0164 00a1 0173  .....r.|...d...s
-00001630: 047c 0191 0271 0453 0072 4600 0000 a902  .|...q.S.rF.....
-00001640: da08 656e 6473 7769 7468 7248 0000 00a9  ..endswithrH....
-00001650: 0272 4a00 0000 da03 7669 6429 0172 4300  .rJ.....vid).rC.
-00001660: 0000 7226 0000 0072 2700 0000 724c 0000  ..r&...r'...rL..
-00001670: 0099 0000 0073 0600 0000 0602 0201 14fe  .....s..........
-00001680: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00001690: 0005 0000 0013 0000 0073 2600 0000 6700  .........s&...g.
-000016a0: 7c00 5d1e 7d01 7c01 a000 8800 6a01 a101  |.].}.|.....j...
-000016b0: 7204 7c01 a002 6400 a101 7304 7c01 9102  r.|...d...s.|...
-000016c0: 7104 5300 7246 0000 0029 0372 5100 0000  q.S.rF...).rQ...
-000016d0: 7242 0000 0072 4800 0000 2902 724a 0000  rB...rH...).rJ..
-000016e0: 00da 0374 6162 a901 da04 7365 6c66 7226  ...tab....selfr&
-000016f0: 0000 0072 2700 0000 724c 0000 00a0 0000  ...r'...rL......
-00001700: 0073 0600 0000 0602 0201 16fe 7a45 556e  .s..........zEUn
-00001710: 6571 7561 6c20 6e75 6d62 6572 206f 6620  equal number of 
-00001720: 7669 6465 6f73 2061 6e64 2074 6162 6c65  videos and table
-00001730: 732e 2050 6c65 6173 6520 6368 6563 6b20  s. Please check 
-00001740: 796f 7572 2066 696c 6520 7374 7275 6374  your file struct
-00001750: 7572 654e 5472 2c00 0000 da03 616c 6c46  ureNTr,.....allF
-00001760: 2923 7218 0000 0072 3e00 0000 723f 0000  )#r....r>...r?..
-00001770: 0072 4000 0000 7203 0000 00da 085f 5f6e  .r@...r......__n
-00001780: 616d 655f 5fda 0c74 7261 696e 6564 5f70  ame__..trained_p
-00001790: 6174 6872 4200 0000 721d 0000 00da 076c  athrB...r......l
-000017a0: 6973 7464 6972 da06 736f 7274 6564 da06  istdir..sorted..
-000017b0: 7669 6465 6f73 da06 7461 626c 6573 da03  videos..tables..
-000017c0: 6c65 6e72 3400 0000 da0a 6172 656e 615f  lenr4.....arena_
-000017d0: 6469 6d73 da11 656c 6c69 7073 655f 6465  dims..ellipse_de
-000017e0: 7465 6374 696f 6eda 0661 6e67 6c65 7372  tection..anglesr
-000017f0: 3300 0000 da05 6172 6561 7372 3500 0000  3.....areasr5...
-00001800: da0c 636f 6e6e 6563 7469 7669 7479 da09  ..connectivity..
-00001810: 6469 7374 616e 6365 73da 0365 676f 7238  distances..egor8
-00001820: 0000 0072 3900 0000 723a 0000 0072 3b00  ...r9...r:...r;.
-00001830: 0000 da14 6c69 6b65 6c69 686f 6f64 5f74  ....likelihood_t
-00001840: 6f6c 6572 616e 6365 723d 0000 0072 4100  olerancer=...rA.
-00001850: 0000 da0a 6672 616d 655f 7261 7465 7243  ....frame_raterC
-00001860: 0000 0072 3600 0000 7237 0000 0029 1572  ...r6...r7...).r
-00001870: 5600 0000 7233 0000 0072 3400 0000 7235  V...r3...r4...r5
-00001880: 0000 0072 3600 0000 7237 0000 0072 3800  ...r6...r7...r8.
-00001890: 0000 7239 0000 0072 3a00 0000 723b 0000  ..r9...r:...r;..
-000018a0: 0072 3c00 0000 723d 0000 0072 3e00 0000  .r<...r=...r>...
-000018b0: 7218 0000 0072 3f00 0000 7240 0000 0072  r....r?...r@...r
-000018c0: 4100 0000 7242 0000 0072 4300 0000 7244  A...rB...rC...rD
-000018d0: 0000 00da 0265 7872 2600 0000 2902 7256  .....exr&...).rV
-000018e0: 0000 0072 4300 0000 7227 0000 00da 085f  ...rC...r'....._
-000018f0: 5f69 6e69 745f 5f5b 0000 0073 6000 0000  _init__[...s`...
-00001900: 002f 0601 0601 0601 0601 0c03 0601 0a01  ./..............
-00001910: 1a01 0801 0801 0801 0601 0201 0a02 0afe  ................
-00001920: 04ff 0607 0201 0a02 0afe 04ff 0607 0a01  ................
-00001930: 04ff 0802 02fe 0405 0601 0601 0603 0601  ................
-00001940: 1401 0601 0601 0601 0601 0601 0601 0601  ................
-00001950: 0601 0601 0601 0601 0601 0601 0601 0601  ................
-00001960: 7a10 5072 6f6a 6563 742e 5f5f 696e 6974  z.Project.__init
-00001970: 5f5f 6301 0000 0000 0000 0000 0000 0001  __c.............
-00001980: 0000 0004 0000 0043 0000 0073 1000 0000  .......C...s....
-00001990: 6401 a000 7401 7c00 6a02 8301 a101 5300  d...t.|.j.....S.
-000019a0: a902 7a1b 5072 696e 7420 7468 6520 6f62  ..z.Print the ob
-000019b0: 6a65 6374 2074 6f20 7374 646f 7574 2e7a  ject to stdout.z
-000019c0: 1c64 6565 706f 6620 616e 616c 7973 6973  .deepof analysis
-000019d0: 206f 6620 7b7d 2076 6964 656f 73a9 03da   of {} videos...
-000019e0: 0666 6f72 6d61 7472 5e00 0000 725c 0000  .formatr^...r\..
-000019f0: 0072 5500 0000 7226 0000 0072 2600 0000  .rU...r&...r&...
-00001a00: 7227 0000 00da 075f 5f73 7472 5f5f c300  r'.....__str__..
-00001a10: 0000 7302 0000 0000 027a 0f50 726f 6a65  ..s......z.Proje
-00001a20: 6374 2e5f 5f73 7472 5f5f 6301 0000 0000  ct.__str__c.....
-00001a30: 0000 0000 0000 0001 0000 0004 0000 0043  ...............C
-00001a40: 0000 0073 1000 0000 6401 a000 7401 7c00  ...s....d...t.|.
-00001a50: 6a02 8301 a101 5300 726a 0000 0072 6b00  j.....S.rj...rk.
-00001a60: 0000 7255 0000 0072 2600 0000 7226 0000  ..rU...r&...r&..
-00001a70: 0072 2700 0000 da08 5f5f 7265 7072 5f5f  .r'.....__repr__
-00001a80: c700 0000 7302 0000 0000 027a 1050 726f  ....s......z.Pro
-00001a90: 6a65 6374 2e5f 5f72 6570 725f 5f63 0100  ject.__repr__c..
-00001aa0: 0000 0000 0000 0000 0000 0400 0000 0a00  ................
-00001ab0: 0000 0300 0000 73b4 0100 0074 006a 01a0  ......s....t.j..
-00001ac0: 0288 006a 0388 006a 04a1 027d 0174 0587  ...j...j...}.t..
-00001ad0: 0066 0164 0164 0284 0874 00a0 0688 006a  .f.d.d...t.....j
-00001ae0: 07a1 0144 0083 0183 0164 036b 0272 3c74  ...D.....d.k.r<t
-00001af0: 0864 0483 0182 0174 0587 0066 0164 0564  .d.....t...f.d.d
-00001b00: 0284 0874 00a0 0688 006a 09a1 0144 0083  ...t.....j...D..
-00001b10: 0183 0164 036b 0272 6674 0864 0683 0182  ...d.k.rft.d....
-00001b20: 0174 006a 01a0 0a7c 01a1 0190 0173 a874  .t.j...|.....s.t
-00001b30: 00a0 0b7c 01a1 0101 0074 00a0 0b74 006a  ...|.....t...t.j
-00001b40: 01a0 0288 006a 0388 006a 0464 07a1 03a1  .....j...j.d....
-00001b50: 0101 0074 00a0 0b74 006a 01a0 0288 006a  ...t...t.j.....j
-00001b60: 0388 006a 0464 08a1 03a1 0101 0074 00a0  ...j.d.......t..
-00001b70: 0b74 006a 01a0 0288 006a 0388 006a 0464  .t.j.....j...j.d
-00001b80: 09a1 03a1 0101 0074 00a0 0b74 006a 01a0  .......t...t.j..
-00001b90: 0288 006a 0388 006a 0464 0aa1 03a1 0101  ...j...j.d......
-00001ba0: 0074 00a0 0688 006a 07a1 0144 005d 3a7d  .t.....j...D.]:}
-00001bb0: 027c 02a0 0c88 006a 0da1 0172 f274 0ea0  .|.....j...r.t..
-00001bc0: 0f74 006a 01a0 0288 006a 077c 02a1 0274  .t.j.....j.|...t
-00001bd0: 006a 01a0 0288 006a 0388 006a 0464 077c  .j.....j...j.d.|
-00001be0: 02a1 04a1 0201 0071 f274 00a0 0688 006a  .......q.t.....j
-00001bf0: 09a1 0144 005d 3e7d 037c 03a0 0c88 006a  ...D.]>}.|.....j
-00001c00: 10a1 0190 0172 3a74 0ea0 0f74 006a 01a0  .....r:t...t.j..
-00001c10: 0288 006a 097c 03a1 0274 006a 01a0 0288  ...j.|...t.j....
-00001c20: 006a 0388 006a 0464 087c 03a1 04a1 0201  .j...j.d.|......
-00001c30: 0090 0171 3a74 006a 01a0 0288 006a 0388  ...q:t.j.....j..
-00001c40: 006a 0464 07a1 0388 005f 0774 006a 01a0  .j.d....._.t.j..
-00001c50: 0288 006a 0388 006a 0464 08a1 0388 005f  ...j...j.d....._
-00001c60: 096e 0874 1164 0b83 0182 0164 0c53 0029  .n.t.d.....d.S.)
-00001c70: 0d7a 3e43 7265 6174 6520 6120 7072 6f6a  .z>Create a proj
-00001c80: 6563 7420 6469 7265 6374 6f72 7920 7768  ect directory wh
-00001c90: 6572 6520 746f 2073 6176 6520 616c 6c20  ere to save all 
-00001ca0: 7072 6f64 7563 6564 2072 6573 756c 7473  produced results
-00001cb0: 2e63 0100 0000 0000 0000 0000 0000 0200  .c..............
-00001cc0: 0000 0500 0000 1300 0000 731c 0000 0067  ..........s....g
-00001cd0: 007c 005d 147d 017c 01a0 0088 006a 01a1  .|.].}.|.....j..
-00001ce0: 0172 047c 0191 0271 0453 0072 2600 0000  .r.|...q.S.r&...
-00001cf0: 2902 7251 0000 0072 4300 0000 7249 0000  ).rQ...rC...rI..
-00001d00: 0072 5500 0000 7226 0000 0072 2700 0000  .rU...r&...r'...
-00001d10: 724c 0000 00d2 0000 0073 0600 0000 0602  rL.......s......
-00001d20: 0201 0cfe 7a34 5072 6f6a 6563 742e 7365  ....z4Project.se
-00001d30: 745f 7570 5f70 726f 6a65 6374 5f64 6972  t_up_project_dir
-00001d40: 6563 746f 7279 2e3c 6c6f 6361 6c73 3e2e  ectory.<locals>.
-00001d50: 3c6c 6973 7463 6f6d 703e 7201 0000 007a  <listcomp>r....z
-00001d60: 3a54 6865 7265 2061 7265 206e 6f20 636f  :There are no co
-00001d70: 6d70 6174 6962 6c65 2076 6964 656f 7320  mpatible videos 
-00001d80: 696e 2074 6865 2073 7065 6369 6669 6564  in the specified
-00001d90: 2064 6972 6563 746f 7279 2e63 0100 0000   directory.c....
-00001da0: 0000 0000 0000 0000 0200 0000 0500 0000  ................
-00001db0: 1300 0000 731c 0000 0067 007c 005d 147d  ....s....g.|.].}
-00001dc0: 017c 01a0 0088 006a 01a1 0172 047c 0191  .|.....j...r.|..
-00001dd0: 0271 0453 0072 2600 0000 2902 7251 0000  .q.S.r&...).rQ..
-00001de0: 0072 4200 0000 7249 0000 0072 5500 0000  .rB...rI...rU...
-00001df0: 7226 0000 0072 2700 0000 724c 0000 00df  r&...r'...rL....
-00001e00: 0000 0073 0600 0000 0602 0201 0cfe 7a3a  ...s..........z:
-00001e10: 5468 6572 6520 6172 6520 6e6f 2063 6f6d  There are no com
-00001e20: 7061 7469 626c 6520 7472 6163 6b73 2069  patible tracks i
-00001e30: 6e20 7468 6520 7370 6563 6966 6965 6420  n the specified 
-00001e40: 6469 7265 6374 6f72 792e da06 5669 6465  directory...Vide
-00001e50: 6f73 da06 5461 626c 6573 721a 0000 00da  os..Tablesr.....
-00001e60: 0746 6967 7572 6573 7a3e 5072 6f6a 6563  .Figuresz>Projec
-00001e70: 7420 616c 7265 6164 7920 6578 6973 7473  t already exists
-00001e80: 2e20 4465 6c65 7465 2069 7420 6f72 2073  . Delete it or s
-00001e90: 7065 6369 6679 2061 2064 6966 6665 7265  pecify a differe
-00001ea0: 6e74 206e 616d 652e 4e29 1272 1d00 0000  nt name.N).r....
-00001eb0: 721e 0000 0072 1f00 0000 7218 0000 0072  r....r....r....r
-00001ec0: 3e00 0000 725e 0000 0072 5a00 0000 723f  >...r^...rZ...r?
-00001ed0: 0000 00da 1146 696c 654e 6f74 466f 756e  .....FileNotFoun
-00001ee0: 6445 7272 6f72 7240 0000 00da 0665 7869  dErrorr@.....exi
-00001ef0: 7374 73da 086d 616b 6564 6972 7372 5100  sts..makedirsrQ.
-00001f00: 0000 7243 0000 00da 0673 6875 7469 6cda  ..rC.....shutil.
-00001f10: 0563 6f70 7932 7242 0000 00da 074f 5345  .copy2rB.....OSE
-00001f20: 7272 6f72 2904 7256 0000 0072 1800 0000  rror).rV...r....
-00001f30: 7253 0000 0072 5400 0000 7226 0000 0072  rS...rT...r&...r
-00001f40: 5500 0000 7227 0000 00da 1873 6574 5f75  U...r'.....set_u
-00001f50: 705f 7072 6f6a 6563 745f 6469 7265 6374  p_project_direct
-00001f60: 6f72 79cb 0000 0073 7000 0000 0003 1203  ory....sp.......
-00001f70: 0201 0a02 0afe 04ff 0207 02f9 02ff 020a  ................
-00001f80: 0201 02ff 0404 0201 0a02 0afe 04ff 0207  ................
-00001f90: 02f9 02ff 020a 0201 02ff 0404 0e01 0a01  ................
-00001fa0: 1a01 1a01 0401 12ff 0403 1a03 1001 0c01  ................
-00001fb0: 0401 0e01 0601 0cff 02fe 0607 1001 0e01  ................
-00001fc0: 0401 0e01 0601 0cff 02fe 0808 0601 0aff  ................
-00001fd0: 0603 0601 0aff 0805 0201 02ff 7a20 5072  ............z Pr
-00001fe0: 6f6a 6563 742e 7365 745f 7570 5f70 726f  oject.set_up_pro
-00001ff0: 6a65 6374 5f64 6972 6563 746f 7279 6301  ject_directoryc.
-00002000: 0000 0000 0000 0000 0000 0001 0000 0001  ................
-00002010: 0000 0043 0000 0073 0600 0000 7c00 6a00  ...C...s....|.j.
-00002020: 5300 2901 7a53 4c69 7374 2e20 4966 206e  S.).zSList. If n
-00002030: 6f74 2027 616c 6c27 2c20 7365 7473 2074  ot 'all', sets t
-00002040: 6865 2062 6f64 7920 7061 7274 7320 616d  he body parts am
-00002050: 6f6e 6720 7768 6963 6820 7468 6520 6469  ong which the di
-00002060: 7374 616e 6365 7320 7769 6c6c 2062 6520  stances will be 
-00002070: 636f 6d70 7574 6564 2ea9 01da 0a5f 6469  computed....._di
-00002080: 7374 616e 6365 7372 5500 0000 7226 0000  stancesrU...r&..
-00002090: 0072 2600 0000 7227 0000 0072 6400 0000  .r&...r'...rd...
-000020a0: 1401 0000 7302 0000 0000 037a 1150 726f  ....s......z.Pro
-000020b0: 6a65 6374 2e64 6973 7461 6e63 6573 6301  ject.distancesc.
-000020c0: 0000 0000 0000 0000 0000 0001 0000 0001  ................
-000020d0: 0000 0043 0000 0073 0600 0000 7c00 6a00  ...C...s....|.j.
-000020e0: 5300 2901 7a6f 5374 7269 6e67 2c20 6e61  S.).zoString, na
-000020f0: 6d65 206f 6620 6120 626f 6479 2070 6172  me of a body par
-00002100: 742e 2049 6620 5472 7565 2c20 636f 6d70  t. If True, comp
-00002110: 7574 6573 206f 6e6c 7920 7468 6520 6469  utes only the di
-00002120: 7374 616e 6365 7320 6265 7477 6565 6e20  stances between 
-00002130: 7468 6520 7370 6563 6966 6965 6420 626f  the specified bo
-00002140: 6479 2070 6172 7420 616e 6420 7468 6520  dy part and the 
-00002150: 7265 7374 2ea9 01da 045f 6567 6f72 5500  rest....._egorU.
-00002160: 0000 7226 0000 0072 2600 0000 7227 0000  ..r&...r&...r'..
-00002170: 0072 6500 0000 1901 0000 7302 0000 0000  .re.......s.....
-00002180: 037a 0b50 726f 6a65 6374 2e65 676f 6301  .z.Project.egoc.
-00002190: 0000 0000 0000 0000 0000 0001 0000 0001  ................
-000021a0: 0000 0043 0000 0073 0600 0000 7c00 6a00  ...C...s....|.j.
-000021b0: 5300 2901 7a67 426f 6f6c 2e20 546f 6767  S.).zgBool. Togg
-000021c0: 6c65 7320 616e 676c 6520 636f 6d70 7574  les angle comput
-000021d0: 6174 696f 6e2e 2054 7275 6520 6279 2064  ation. True by d
-000021e0: 6566 6175 6c74 2e20 4966 2074 7572 6e65  efault. If turne
-000021f0: 6420 6f66 662c 2065 6e68 616e 6365 7320  d off, enhances 
-00002200: 7065 7266 6f72 6d61 6e63 6520 666f 7220  performance for 
-00002210: 6269 6720 6461 7461 7365 7473 2ea9 01da  big datasets....
-00002220: 075f 616e 676c 6573 7255 0000 0072 2600  ._anglesrU...r&.
-00002230: 0000 7226 0000 0072 2700 0000 7261 0000  ..r&...r'...ra..
-00002240: 001e 0100 0073 0200 0000 0003 7a0e 5072  .....s......z.Pr
-00002250: 6f6a 6563 742e 616e 676c 6573 4629 0372  oject.anglesF).r
-00002260: 5d00 0000 da07 7665 7262 6f73 6572 1900  ].....verboser..
-00002270: 0000 6303 0000 0000 0000 0000 0000 0003  ..c.............
-00002280: 0000 0008 0000 0043 0000 0073 2c00 0000  .......C...s,...
-00002290: 7c02 720c 7400 6401 8301 0100 7401 6a02  |.r.t.d.....t.j.
-000022a0: a003 7c00 6a04 7c00 6a05 7c00 6a06 7c00  ..|.j.|.j.|.j.|.
-000022b0: 6a07 7c01 7c00 6a08 a106 5300 2902 6139  j.|.|.j...S.).a9
-000022c0: 0100 0052 6574 7572 6e20 7468 6520 6172  ...Return the ar
-000022d0: 656e 6120 6173 2072 6563 6f67 6e69 7365  ena as recognise
-000022e0: 6420 6672 6f6d 2074 6865 2076 6964 656f  d from the video
-000022f0: 732e 0a0a 2020 2020 2020 2020 4172 6773  s...        Args
-00002300: 3a0a 2020 2020 2020 2020 2020 2020 7461  :.            ta
-00002310: 626c 6573 2028 6c69 7374 293a 206c 6973  bles (list): lis
-00002320: 7420 6f66 2063 6f6f 7264 696e 6174 6520  t of coordinate 
-00002330: 7461 626c 6573 0a20 2020 2020 2020 2020  tables.         
-00002340: 2020 2076 6572 626f 7365 2028 626f 6f6c     verbose (bool
-00002350: 293a 2069 6620 5472 7565 2c20 6c6f 6773  ): if True, logs
-00002360: 2074 6f20 636f 6e73 6f6c 650a 0a20 2020   to console..   
-00002370: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-00002380: 2020 2020 2020 2020 2020 6172 656e 6120            arena 
-00002390: 286e 702e 6e64 6172 7261 7929 3a20 6172  (np.ndarray): ar
-000023a0: 656e 6120 7061 7261 6d65 7465 7273 2c20  ena parameters, 
-000023b0: 6173 2072 6563 6f67 6e69 7365 6420 6672  as recognised fr
-000023c0: 6f6d 2074 6865 2076 6964 656f 732e 2054  om the videos. T
-000023d0: 6865 2073 6861 7065 2064 6570 656e 6473  he shape depends
-000023e0: 206f 6e20 7468 6520 6172 656e 6120 7479   on the arena ty
-000023f0: 7065 0a0a 2020 2020 2020 2020 7a12 4465  pe..        z.De
-00002400: 7465 6374 696e 6720 6172 656e 612e 2e2e  tecting arena...
-00002410: 2909 da05 7072 696e 74da 0664 6565 706f  )...print..deepo
-00002420: 66da 0575 7469 6c73 da0a 6765 745f 6172  f..utils..get_ar
-00002430: 656e 6173 7234 0000 0072 5f00 0000 7218  enasr4...r_...r.
-00002440: 0000 0072 3e00 0000 725c 0000 0029 0372  ...r>...r\...).r
-00002450: 5600 0000 725d 0000 0072 7f00 0000 7226  V...r]...r....r&
-00002460: 0000 0072 2600 0000 7227 0000 00da 0967  ...r&...r'.....g
-00002470: 6574 5f61 7265 6e61 2301 0000 7314 0000  et_arena#...s...
-00002480: 0000 0b04 0108 0206 0104 0104 0104 0104  ................
-00002490: 0102 0104 fa7a 1150 726f 6a65 6374 2e67  .....z.Project.g
-000024a0: 6574 5f61 7265 6e61 2902 727f 0000 0072  et_arena).r....r
-000024b0: 1900 0000 6302 0000 0000 0000 0000 0000  ....c...........
-000024c0: 000f 0000 0009 0000 0003 0000 0073 9604  .............s..
-000024d0: 0000 8801 6a00 6401 7601 7212 7401 6402  ....j.d.v.r.t.d.
-000024e0: 8301 8201 7c01 721e 7402 6403 8301 0100  ....|.r.t.d.....
-000024f0: 6900 7d02 8801 6a03 4400 5dba 8902 8801  i.}...j.D.].....
-00002500: 6a00 6404 6b02 7284 7404 6a05 7406 6a07  j.d.k.r.t.j.t.j.
-00002510: a008 8801 6a09 8802 a102 740a 6405 8d02  ....j.....t.d...
-00002520: 7d03 7c03 6a0b 6a0c 6406 6407 8d01 6a0b  }.|.j.j.d.d...j.
-00002530: 7d03 7c03 6a0d 6408 6409 6409 8502 6602  }.|.j.d.d.d...f.
-00002540: 1900 7c03 5f0e 7c03 6a0f 640a 6409 8502  ..|._.|.j.d.d...
-00002550: 1900 7d03 6e26 8801 6a00 640b 6b02 72aa  ..}.n&..j.d.k.r.
-00002560: 7404 6a10 7406 6a07 a008 8801 6a09 8802  t.j.t.j.....j...
-00002570: a102 640c 6406 640d 8d03 7d03 7a18 7411  ..d.d.d...}.z.t.
-00002580: 6a12 6a13 a014 640e 8802 a102 640c 1900  j.j...d.....d...
-00002590: 7d04 5700 6e16 0400 7415 79d8 0100 0100  }.W.n...t.y.....
-000025a0: 0100 8802 7d04 5900 6e02 3000 7c03 7c02  ....}.Y.n.0.|.|.
-000025b0: 7c04 3c00 7128 640f 7416 7c02 a017 a100  |.<.q(d.t.|.....
-000025c0: 8301 640c 1900 6a18 7600 9001 726e 7416  ..d...j.v...rnt.
-000025d0: 7416 7c02 a017 a100 8301 640c 1900 6a0d  t.|.......d...j.
-000025e0: 640f 6409 6409 8502 6602 1900 a019 a100  d.d.d...f.......
-000025f0: 8301 8801 5f1a 7c02 a01b a100 4400 5d40  ...._.|.....D.]@
-00002600: 5c02 7d05 8902 8802 6a0d 640f 1900 6410  \.}.....j.d...d.
-00002610: 1700 8802 6a0d 6411 1900 1700 7c02 7c05  ....j.d.....|.|.
-00002620: 1900 6a0d 6411 3c00 7c02 7c05 1900 6a1c  ..j.d.<.|.|...j.
-00002630: 640f 640c 6412 6413 8d03 0100 9001 712c  d.d.d.d.......q,
-00002640: 7c02 a01b a100 4400 5d56 5c02 7d05 8902  |.....D.]V\.}...
-00002650: 8802 a01d a100 7d06 7404 6a1e a01f 8702  ......}.t.j.....
-00002660: 6601 6414 6415 8408 7420 6416 8301 4400  f.d.d...t d...D.
-00002670: 8301 a101 7c06 5f0e 7c06 6a0f 6416 6409  ....|._.|.j.d.d.
-00002680: 8502 1900 a021 740a a101 7d06 7c06 6a0c  .....!t...}.|.j.
-00002690: 6412 6407 8d01 7c02 7c05 3c00 9001 7176  d.d...|.|.<...qv
-000026a0: 8701 6601 6417 6418 8408 8801 6a1a 4400  ..f.d.d.....j.D.
-000026b0: 8301 8900 8700 8701 6602 6419 6418 8408  ........f.d.d...
-000026c0: 8801 6a1a 4400 8301 8801 5f22 7423 8801  ..j.D....._"t#..
-000026d0: 6a1a 8301 640a 6b04 9002 7232 8801 6a24  j...d.k...r2..j$
-000026e0: 7425 641a 6701 8301 6b03 9002 7232 8701  t%d.g...k...r2..
-000026f0: 6601 641b 6415 8408 8801 6a1a 4400 8301  f.d.d.....j.D...
-00002700: 8801 5f24 8801 6a26 6409 7501 9002 7294  .._$..j&d.u...r.
-00002710: 7c02 a01b a100 4400 5d4c 5c02 7d05 8902  |.....D.]L\.}...
-00002720: 7404 6a27 641c 7404 6a28 8802 6a29 640c  t.j'd.t.j(..j)d.
-00002730: 1900 8801 6a26 1a00 641d 641e 8d02 8802  ....j&..d.d.....
-00002740: 6a29 640c 1900 640a 1700 641f 6420 8d04  j)d...d...d.d ..
-00002750: a02a 6421 6422 8400 a101 7c02 7c05 1900  .*d!d"....|.|...
-00002760: 5f18 9002 7146 742b 8300 7d07 7c02 a01b  _...qFt+..}.|...
-00002770: a100 4400 5d6c 5c02 7d05 8902 8802 6a2c  ..D.]l\.}.....j,
-00002780: 6423 6424 640a 6406 6425 8d04 7d08 8802  d#d$d.d.d%..}...
-00002790: 6a2c 6426 6424 640a 6406 6425 8d04 7d09  j,d&d$d.d.d%..}.
-000027a0: 8802 6a2c 6427 6424 640a 6412 6425 8d04  ..j,d'd$d.d.d%..
-000027b0: 7d0a 7404 6a2d 7c08 7c09 6702 640a 6428  }.t.j-|.|.g.d.d(
-000027c0: 8d02 6a2e 640a 6428 8d01 7c02 7c05 3c00  ..j.d.d(..|.|.<.
-000027d0: 7c0a a02f 6429 a101 7c07 7c05 3c00 9002  |../d)..|.|.<...
-000027e0: 71a2 7430 7c07 642a 8801 6a1a 642b 8d03  q.t0|.d*..j.d+..
-000027f0: 7d07 8801 6a31 9003 7292 7c01 9003 7236  }...j1..r.|...r6
-00002800: 7402 642c 8301 0100 7c02 a01b a100 4400  t.d,....|.....D.
-00002810: 5d52 5c02 7d05 8902 8802 6a18 7d0b 8802  ]R\.}.....j.}...
-00002820: 6a0e 7d0c 7404 a032 7411 6a12 6a33 7434  j.}.t..2t.j.j3t4
-00002830: a035 8802 a101 8801 6a31 642d 642e 8d03  .5......j1d-d...
-00002840: a101 6a0c 6412 6407 8d01 7d0d 7c0c 7c0d  ..j.d.d...}.|.|.
-00002850: 5f0e 7c0b 7c0d 5f18 7c0d 7c02 7c05 3c00  _.|.|._.|.|.|.<.
-00002860: 9003 713e 8801 6a24 7425 641a 6701 8301  ..q>..j$t%d.g...
-00002870: 6b03 9004 7208 7c02 a01b a100 4400 5d5a  k...r.|.....D.]Z
-00002880: 5c02 7d0e 8902 8802 6a1c 8801 6a24 640a  \.}.....j...j$d.
-00002890: 6411 642f 8d03 8903 8803 6a2e 640a 6412  d.d/......j.d.d.
-000028a0: 6413 8d02 0100 7404 6a1e a036 8703 6601  d.....t.j..6..f.
-000028b0: 6430 6415 8408 7420 6416 8301 4400 8301  d0d...t d...D...
-000028c0: a101 8803 5f0e 8803 6a2e 640a 6428 8d01  ...._...j.d.d(..
-000028d0: 7c02 7c0e 3c00 9003 71ac 8801 6a37 9004  |.|.<...q...j7..
-000028e0: 7258 7c01 9004 721e 7402 6431 8301 0100  rX|...r.t.d1....
-000028f0: 7c02 a01b a100 4400 5d30 5c02 7d0e 8902  |.....D.]0\.}...
-00002900: 7411 6a12 6a37 8802 7c07 7c0e 1900 8801  t.j.j7..|.|.....
-00002910: 6a38 6432 8801 6a39 8801 6a3a 6433 8d06  j8d2..j9..j:d3..
-00002920: 7c02 7c0e 3c00 9004 7126 8801 6a3b 9004  |.|.<...q&..j;..
-00002930: 727e 7c01 9004 726e 7402 6434 8301 0100  r~|...rnt.d4....
-00002940: 7411 6a12 a03c 8801 7c02 7c07 a103 7d02  t.j..<..|.|...}.
-00002950: 7411 6a12 a03d 8801 7c02 7c07 a103 7d02  t.j..=..|.|...}.
-00002960: 7c02 7c07 6602 5300 2935 6140 0100 004c  |.|.f.S.)5a@...L
-00002970: 6f61 6420 7669 6465 6f73 2061 6e64 2074  oad videos and t
-00002980: 6162 6c65 7320 696e 746f 2064 6963 7469  ables into dicti
-00002990: 6f6e 6172 6965 732e 0a0a 2020 2020 2020  onaries...      
-000029a0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-000029b0: 2020 2020 7665 7262 6f73 6520 2862 6f6f      verbose (boo
-000029c0: 6c29 3a20 4966 2054 7275 652c 2070 7269  l): If True, pri
-000029d0: 6e74 7320 7468 6520 7072 6f67 7265 7373  nts the progress
-000029e0: 206f 6620 6461 7461 206c 6f61 6469 6e67   of data loading
-000029f0: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-00002a00: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
-00002a10: 5475 706c 653a 2041 2074 7570 6c65 2063  Tuple: A tuple c
-00002a20: 6f6e 7461 696e 696e 6720 7468 6520 666f  ontaining the fo
-00002a30: 6c6c 6f77 696e 6720 6120 6469 6374 696f  llowing a dictio
-00002a40: 6e61 7279 2077 6974 6820 616c 6c20 6c6f  nary with all lo
-00002a50: 6164 6564 2074 6162 6c65 7320 7065 7220  aded tables per 
-00002a60: 6578 7065 7269 6d65 6e74 2c0a 2020 2020  experiment,.    
-00002a70: 2020 2020 2020 2020 616e 6420 616e 6f74          and anot
-00002a80: 6865 7220 6469 6374 696f 6e61 7279 2077  her dictionary w
-00002a90: 6974 6820 444c 4320 6461 7461 2071 7561  ith DLC data qua
-00002aa0: 6c69 7479 2e0a 0a20 2020 2020 2020 2029  lity...        )
-00002ab0: 0272 4e00 0000 724f 0000 007a 3154 7261  .rN...rO...z1Tra
-00002ac0: 636b 696e 6720 6669 6c65 7320 6d75 7374  cking files must
-00002ad0: 2062 6520 696e 2065 6974 6865 7220 6835   be in either h5
-00002ae0: 206f 7220 6373 7620 666f 726d 6174 7a17   or csv formatz.
-00002af0: 4c6f 6164 696e 6720 7472 616a 6563 746f  Loading trajecto
-00002b00: 7269 6573 2e2e 2e72 4e00 0000 a901 da05  ries...rN.......
-00002b10: 6474 7970 6546 2901 da04 6472 6f70 da06  dtypeF)...drop..
-00002b20: 7363 6f72 6572 4e72 3100 0000 724f 0000  scorerNr1...rO..
-00002b30: 0072 0100 0000 2902 da09 696e 6465 785f  .r....)...index_
-00002b40: 636f 6cda 0a6c 6f77 5f6d 656d 6f72 797a  col..low_memoryz
-00002b50: 0828 2e2a 3f29 444c 43da 0b69 6e64 6976  .(.*?)DLC..indiv
-00002b60: 6964 7561 6c73 da01 5fda 0962 6f64 7970  iduals.._..bodyp
-00002b70: 6172 7473 5429 02da 0461 7869 73da 0769  artsT)...axis..i
-00002b80: 6e70 6c61 6365 6301 0000 0000 0000 0000  nplacec.........
-00002b90: 0000 0002 0000 0004 0000 0013 0000 0073  ...............s
-00002ba0: 1600 0000 6700 7c00 5d0e 7d01 8800 6a00  ....g.|.].}...j.
-00002bb0: 7c01 1900 9102 7104 5300 7226 0000 00a9  |.....q.S.r&....
-00002bc0: 01da 0469 6c6f 6372 4900 0000 2901 7254  ...ilocrI...).rT
-00002bd0: 0000 0072 2600 0000 7227 0000 0072 4c00  ...r&...r'...rL.
-00002be0: 0000 7d01 0000 724d 0000 007a 2750 726f  ..}...rM...z'Pro
-00002bf0: 6a65 6374 2e6c 6f61 645f 7461 626c 6573  ject.load_tables
-00002c00: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
-00002c10: 6f6d 703e e902 0000 0063 0100 0000 0000  omp>.....c......
-00002c20: 0000 0000 0000 0200 0000 0800 0000 1300  ................
-00002c30: 0000 732a 0000 0069 007c 005d 227d 0164  ..s*...i.|.]"}.d
-00002c40: 00a0 007c 01a1 0174 016a 026a 037c 0188  ...|...t.j.j.|..
-00002c50: 006a 0488 006a 0564 018d 0393 0271 0453  .j...j.d.....q.S
-00002c60: 0029 027a 0f7b 7d6d 6f75 7365 5f74 6f70  .).z.{}mouse_top
-00002c70: 7669 6577 2902 7237 0000 00da 0c67 7261  view).r7.....gra
-00002c80: 7068 5f70 7265 7365 7429 0672 6c00 0000  ph_preset).rl...
-00002c90: 7281 0000 0072 8200 0000 da0d 636f 6e6e  r....r......conn
-00002ca0: 6563 745f 6d6f 7573 6572 3700 0000 7235  ect_mouser7...r5
-00002cb0: 0000 00a9 0272 4a00 0000 da03 6169 6472  .....rJ.....aidr
-00002cc0: 5500 0000 7226 0000 0072 2700 0000 da0a  U...r&...r'.....
-00002cd0: 3c64 6963 7463 6f6d 703e 8301 0000 730c  <dictcomp>....s.
-00002ce0: 0000 0006 0602 fb0e 0102 0104 0104 fd7a  ...............z
-00002cf0: 2750 726f 6a65 6374 2e6c 6f61 645f 7461  'Project.load_ta
-00002d00: 626c 6573 2e3c 6c6f 6361 6c73 3e2e 3c64  bles.<locals>.<d
-00002d10: 6963 7463 6f6d 703e 6301 0000 0000 0000  ictcomp>c.......
-00002d20: 0000 0000 0002 0000 0006 0000 0013 0000  ................
-00002d30: 0073 1c00 0000 6900 7c00 5d14 7d01 7c01  .s....i.|.].}.|.
-00002d40: 8800 7c01 8801 6a00 1700 1900 9302 7104  ..|...j.......q.
-00002d50: 5300 7226 0000 0029 0172 3d00 0000 7295  S.r&...).r=...r.
-00002d60: 0000 0029 02da 0a6d 6f64 656c 5f64 6963  ...)...model_dic
-00002d70: 7472 5600 0000 7226 0000 0072 2700 0000  trV...r&...r'...
-00002d80: 7297 0000 008b 0100 0073 0200 0000 0601  r........s......
-00002d90: 722c 0000 0063 0100 0000 0000 0000 0000  r,...c..........
-00002da0: 0000 0300 0000 0500 0000 1300 0000 7324  ..............s$
-00002db0: 0000 0067 007c 005d 1c7d 0188 006a 0044  ...g.|.].}...j.D
-00002dc0: 005d 107d 027c 0164 0017 007c 0217 0091  .].}.|.d...|....
-00002dd0: 0371 0e71 0453 00a9 0172 8c00 0000 2901  .q.q.S...r....).
-00002de0: 7237 0000 0029 0372 4a00 0000 7296 0000  r7...).rJ...r...
-00002df0: 00da 0262 7072 5500 0000 7226 0000 0072  ...bprU...r&...r
-00002e00: 2700 0000 724c 0000 0091 0100 0073 0600  '...rL.......s..
-00002e10: 0000 0602 0201 0afe 7a08 3030 3a30 303a  ........z.00:00:
-00002e20: 3030 da03 7365 6329 01da 0475 6e69 74da  00..sec)...unit.
-00002e30: 046c 6566 7429 02da 0770 6572 696f 6473  .left)...periods
-00002e40: da06 636c 6f73 6564 6301 0000 0000 0000  ..closedc.......
-00002e50: 0000 0000 0001 0000 0003 0000 0053 0000  .............S..
-00002e60: 0073 1000 0000 7400 7c00 8301 6401 6400  .s....t.|...d.d.
-00002e70: 8502 1900 5300 2902 4ee9 0700 0000 a901  ....S.).N.......
-00002e80: da03 7374 7229 01da 0174 7226 0000 0072  ..str)...tr&...r
-00002e90: 2600 0000 7227 0000 00da 083c 6c61 6d62  &...r'.....<lamb
-00002ea0: 6461 3e9f 0100 0072 4d00 0000 7a25 5072  da>....rM...z%Pr
-00002eb0: 6f6a 6563 742e 6c6f 6164 5f74 6162 6c65  oject.load_table
-00002ec0: 732e 3c6c 6f63 616c 733e 2e3c 6c61 6d62  s.<locals>.<lamb
-00002ed0: 6461 3eda 0178 da06 636f 6f72 6473 2903  da>..x..coords).
-00002ee0: da05 6c65 7665 6c72 8e00 0000 da0a 6472  ..levelr......dr
-00002ef0: 6f70 5f6c 6576 656c da01 79da 0a6c 696b  op_level..y..lik
-00002f00: 656c 6968 6f6f 64a9 0172 8e00 0000 e700  elihood..r......
-00002f10: 0000 0000 0000 00da 0771 7561 6c69 7479  .........quality
-00002f20: a902 da03 7479 7072 3300 0000 7a19 536d  ....typr3...z.Sm
-00002f30: 6f6f 7468 696e 6720 7472 616a 6563 746f  oothing trajecto
-00002f40: 7269 6573 2e2e 2ee9 0f00 0000 2902 da05  ries........)...
-00002f50: 616c 7068 61da 0877 5f6c 656e 6774 6829  alpha..w_length)
-00002f60: 0272 8e00 0000 72a7 0000 0063 0100 0000  .r....r....c....
-00002f70: 0000 0000 0000 0000 0100 0000 0800 0000  ................
-00002f80: 1300 0000 732c 0000 0067 007c 005d 2489  ....s,...g.|.]$.
-00002f90: 0074 0074 0174 0287 0066 0164 0064 0184  .t.t.t...f.d.d..
-00002fa0: 0888 016a 0344 0083 0183 0183 0183 0191  ...j.D..........
-00002fb0: 0271 0453 0029 0263 0100 0000 0000 0000  .q.S.).c........
-00002fc0: 0000 0000 0200 0000 0400 0000 1300 0000  ................
-00002fd0: 7314 0000 0067 007c 005d 0c7d 017c 0188  s....g.|.].}.|..
-00002fe0: 0019 0091 0271 0453 0072 2600 0000 7226  .....q.S.r&...r&
-00002ff0: 0000 0072 4900 0000 a901 da01 6a72 2600  ...rI.......jr&.
-00003000: 0000 7227 0000 0072 4c00 0000 c401 0000  ..r'...rL.......
-00003010: 724d 0000 007a 3250 726f 6a65 6374 2e6c  rM...z2Project.l
-00003020: 6f61 645f 7461 626c 6573 2e3c 6c6f 6361  oad_tables.<loca
-00003030: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 2e3c  ls>.<listcomp>.<
-00003040: 6c69 7374 636f 6d70 3e29 0472 5b00 0000  listcomp>).r[...
-00003050: da04 6c69 7374 da03 7365 74da 0763 6f6c  ..list..set..col
-00003060: 756d 6e73 2901 724a 0000 0029 01da 0474  umns).rJ...)...t
-00003070: 656d 7072 b300 0000 7227 0000 0072 4c00  empr....r'...rL.
-00003080: 0000 c401 0000 724d 0000 007a 1949 6e74  ......rM...z.Int
-00003090: 6572 706f 6c61 7469 6e67 206f 7574 6c69  erpolating outli
-000030a0: 6572 732e 2e2e da02 6f72 2904 7266 0000  ers.....or).rf..
-000030b0: 00da 046d 6f64 65da 056c 696d 6974 da05  ...mode..limit..
-000030c0: 6e5f 7374 647a 2c49 7465 7261 7469 7665  n_stdz,Iterative
-000030d0: 2069 6d70 7574 6174 696f 6e20 6f66 206f   imputation of o
-000030e0: 636c 7564 6564 2062 6f64 7970 6172 7473  cluded bodyparts
-000030f0: 2e2e 2e29 3e72 4200 0000 da13 4e6f 7449  ...)>rB.....NotI
-00003100: 6d70 6c65 6d65 6e74 6564 4572 726f 7272  mplementedErrorr
-00003110: 8000 0000 725d 0000 00da 0270 64da 0872  ....r].....pd..r
-00003120: 6561 645f 6864 6672 1d00 0000 721e 0000  ead_hdfr....r...
-00003130: 0072 1f00 0000 7240 0000 00da 0566 6c6f  .r....r@.....flo
-00003140: 6174 da01 54da 0b72 6573 6574 5f69 6e64  at..T..reset_ind
-00003150: 6578 da03 6c6f 6372 b700 0000 7291 0000  ex..locr....r...
-00003160: 00da 0872 6561 645f 6373 7672 8100 0000  ...read_csvr....
-00003170: 7282 0000 00da 0272 65da 0766 696e 6461  r......re..finda
-00003180: 6c6c da0a 496e 6465 7845 7272 6f72 72b5  ll..IndexErrorr.
-00003190: 0000 00da 0676 616c 7565 73da 0569 6e64  .....values..ind
-000031a0: 6578 da06 756e 6971 7565 7233 0000 00da  ex..uniquer3....
-000031b0: 0569 7465 6d73 7287 0000 00da 0463 6f70  .itemsr......cop
-000031c0: 79da 0a4d 756c 7469 496e 6465 78da 0b66  y..MultiIndex..f
-000031d0: 726f 6d5f 6172 7261 7973 da05 7261 6e67  rom_arrays..rang
-000031e0: 65da 0661 7374 7970 6572 6300 0000 725e  e..astyperc...r^
-000031f0: 0000 0072 3700 0000 da05 7475 706c 6572  ...r7.....tupler
-00003200: 6700 0000 da0f 7469 6d65 6465 6c74 615f  g.....timedelta_
-00003210: 7261 6e67 65da 0c74 6f5f 7469 6d65 6465  range..to_timede
-00003220: 6c74 61da 0573 6861 7065 da03 6d61 7072  lta..shape..mapr
-00003230: 0200 0000 da02 7873 da06 636f 6e63 6174  ......xs..concat
-00003240: da0a 736f 7274 5f69 6e64 6578 da06 6669  ..sort_index..fi
-00003250: 6c6c 6e61 da09 5461 626c 6544 6963 7472  llna..TableDictr
-00003260: 4100 0000 da09 4461 7461 4672 616d 65da  A.....DataFrame.
-00003270: 1673 6d6f 6f74 685f 6d75 6c74 5f74 7261  .smooth_mult_tra
-00003280: 6a65 6374 6f72 79da 026e 70da 0561 7272  jectory..np..arr
-00003290: 6179 da0c 6672 6f6d 5f70 726f 6475 6374  ay..from_product
-000032a0: 7239 0000 0072 6600 0000 723a 0000 0072  r9...rf...r:...r
-000032b0: 3b00 0000 7236 0000 00da 1469 7465 7261  ;...r6.....itera
-000032c0: 7469 7665 5f69 6d70 7574 6174 696f 6eda  tive_imputation.
-000032d0: 1373 6574 5f6d 6973 7369 6e67 5f61 6e69  .set_missing_ani
-000032e0: 6d61 6c73 290f 7256 0000 0072 7f00 0000  mals).rV...r....
-000032f0: da08 7461 625f 6469 6374 da0a 6c6f 6164  ..tab_dict..load
-00003300: 6564 5f74 6162 5a08 7461 625f 6e61 6d65  ed_tabZ.tab_name
-00003310: da03 6b65 79da 0874 6162 5f63 6f70 79da  ..key..tab_copy.
-00003320: 086c 696b 5f64 6963 7472 a500 0000 72a9  .lik_dictr....r.
-00003330: 0000 00da 036c 696b da07 6375 725f 6964  .....lik..cur_id
-00003340: 78da 0863 7572 5f63 6f6c 73da 0673 6d6f  x..cur_cols..smo
-00003350: 6f74 68da 016b 7226 0000 0029 0472 9800  oth..kr&...).r..
-00003360: 0000 7256 0000 0072 5400 0000 72b8 0000  ..rV...rT...r...
-00003370: 0072 2700 0000 da0b 6c6f 6164 5f74 6162  .r'.....load_tab
-00003380: 6c65 733a 0100 0073 de00 0000 000b 0a01  les:...s........
-00003390: 0201 02ff 0404 0401 0802 0401 0a02 0a02  ................
-000033a0: 0401 10ff 0605 1001 1401 1002 0a02 0401  ................
-000033b0: 0e01 0201 02fd 0607 0201 1801 0c01 0a02  ................
-000033c0: 0a03 1801 0201 20ff 0604 1003 16ff 0c03  ...... .........
-000033d0: 1803 1001 0802 0601 14ff 0603 1401 1403  ................
-000033e0: 0a06 04fa 0608 0c01 04ff 0805 2201 0a02  ............"...
-000033f0: 04fe 0807 0c01 1001 0401 0201 1801 0c01  ................
-00003400: 02fc 0605 06fb 0e07 0602 1001 1201 1201  ................
-00003410: 1202 1e01 1202 1002 0802 0601 0802 1001  ................
-00003420: 0601 0601 0401 0601 0eff 04ff 0404 02fc  ................
-00003430: 0605 0601 0601 0c02 1202 1001 1201 0e01  ................
-00003440: 0601 14ff 0603 1402 0802 0601 0802 1001  ................
-00003450: 0601 0201 0601 0401 0201 0401 04fa 0e09  ................
-00003460: 0802 0601 0802 1003 1002 7a13 5072 6f6a  ..........z.Proj
-00003470: 6563 742e 6c6f 6164 5f74 6162 6c65 7329  ect.load_tables)
-00003480: 0372 e200 0000 727f 0000 0072 1900 0000  .r....r....r....
-00003490: 6303 0000 0000 0000 0000 0000 0006 0000  c...............
-000034a0: 0006 0000 0003 0000 0073 1e01 0000 7c02  .........s....|.
-000034b0: 720c 7400 6401 8301 0100 8802 6a01 8900  r.t.d.......j...
-000034c0: 8800 6402 6b02 7236 8803 7402 8803 a003  ..d.k.r6..t.....
-000034d0: a100 8301 6403 1900 1900 6a04 6a05 6403  ....d.....j.j.d.
-000034e0: 1900 8900 8703 6601 6404 6405 8408 8800  ......f.d.d.....
-000034f0: 4400 8301 7350 4a00 6406 8301 8201 8802  D...sPJ.d.......
-00003500: 6a06 6407 6407 8502 6408 6407 8502 6602  j.d.d...d.d...f.
-00003510: 1900 8901 8701 6601 6409 640a 8408 7407  ......f.d.d...t.
-00003520: 8803 a008 a100 8301 4400 8301 7d03 7c03  ........D...}.|.
-00003530: a003 a100 4400 5d32 7d04 7c03 7c04 1900  ....D.]2}.|.|...
-00003540: 6a09 6407 6407 8502 8700 6601 640b 6405  j.d.d.....f.d.d.
-00003550: 8408 7c03 7c04 1900 6a04 4400 8301 6602  ..|.|...j.D...f.
-00003560: 1900 7c03 7c04 3c00 7188 8802 6a0a 72fa  ..|.|.<.q...j.r.
-00003570: 7c03 a008 a100 4400 5d2e 5c02 7d04 7d05  |.....D.].\.}.}.
-00003580: 7c05 6a09 6407 6407 8502 8702 6601 640c  |.j.d.d.....f.d.
-00003590: 6405 8408 7c05 6a04 4400 8301 6602 1900  d...|.j.D...f...
-000035a0: 7c03 7c04 3c00 71ca 7c03 a003 a100 4400  |.|.<.q.|.....D.
-000035b0: 5d16 7d04 8803 7c04 1900 6a0b 7c03 7c04  ].}...|...j.|.|.
-000035c0: 1900 5f0b 9001 7102 7c03 5300 290d 61c7  .._...q.|.S.).a.
-000035d0: 0100 0043 6f6d 7075 7465 2074 6865 2064  ...Compute the d
-000035e0: 6973 7461 6e63 6573 2062 6574 7765 656e  istances between
-000035f0: 2061 6c6c 2073 656c 6563 7465 6420 626f   all selected bo
-00003600: 6479 2070 6172 7473 206f 7665 7220 7469  dy parts over ti
-00003610: 6d65 2e20 4966 2065 676f 2069 7320 7072  me. If ego is pr
-00003620: 6f76 6964 6564 2c20 6974 206f 6e6c 7920  ovided, it only 
-00003630: 7265 7475 726e 7320 6469 7374 616e 6365  returns distance
-00003640: 7320 746f 2061 2073 7065 6369 6669 6564  s to a specified
-00003650: 2062 6f64 7970 6172 742e 0a0a 2020 2020   bodypart...    
-00003660: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-00003670: 2020 2020 2020 7461 625f 6469 6374 2028        tab_dict (
-00003680: 6469 6374 293a 2044 6963 7469 6f6e 6172  dict): Dictionar
-00003690: 7920 6f66 2070 616e 6461 7320 4461 7461  y of pandas Data
-000036a0: 4672 616d 6573 2063 6f6e 7461 696e 696e  Frames containin
-000036b0: 6720 7468 6520 7472 616a 6563 746f 7269  g the trajectori
-000036c0: 6573 206f 6620 616c 6c20 626f 6479 7061  es of all bodypa
-000036d0: 7274 732e 0a20 2020 2020 2020 2020 2020  rts..           
-000036e0: 2076 6572 626f 7365 2028 626f 6f6c 293a   verbose (bool):
-000036f0: 2049 6620 5472 7565 2c20 7072 696e 7473   If True, prints
-00003700: 2070 726f 6772 6573 732e 2044 6566 6175   progress. Defau
-00003710: 6c74 7320 746f 2054 7275 652e 0a0a 2020  lts to True...  
-00003720: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
-00003730: 2020 2020 2020 2020 2020 2064 6963 743a             dict:
-00003740: 2044 6963 7469 6f6e 6172 7920 6f66 2070   Dictionary of p
-00003750: 616e 6461 7320 4461 7461 4672 616d 6573  andas DataFrames
-00003760: 2063 6f6e 7461 696e 696e 6720 7468 6520   containing the 
-00003770: 6469 7374 616e 6365 7320 6265 7477 6565  distances betwee
-00003780: 6e20 616c 6c20 626f 6479 7061 7274 732e  n all bodyparts.
-00003790: 0a0a 2020 2020 2020 2020 7a16 436f 6d70  ..        z.Comp
-000037a0: 7574 696e 6720 6469 7374 616e 6365 732e  uting distances.
-000037b0: 2e2e 7257 0000 0072 0100 0000 6301 0000  ..rW...r....c...
-000037c0: 0000 0000 0000 0000 0002 0000 0006 0000  ................
-000037d0: 0013 0000 0073 2800 0000 6700 7c00 5d20  .....s(...g.|.] 
-000037e0: 7d01 7c01 7400 8800 a001 a100 8301 6400  }.|.t.........d.
-000037f0: 1900 6a02 6a03 6400 1900 7600 9102 7104  ..j.j.d...v...q.
-00003800: 5300 a901 7201 0000 0029 0472 b500 0000  S...r....).r....
-00003810: 72c8 0000 0072 b700 0000 da06 6c65 7665  r....r......leve
-00003820: 6c73 7249 0000 0029 0172 e200 0000 7226  lsrI...).r....r&
-00003830: 0000 0072 2700 0000 724c 0000 00f5 0100  ...r'...rL......
-00003840: 0073 0200 0000 0601 7a29 5072 6f6a 6563  .s......z)Projec
-00003850: 742e 6765 745f 6469 7374 616e 6365 732e  t.get_distances.
-00003860: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-00003870: 6d70 3e7a 2d4e 6f64 6573 2073 686f 756c  mp>z-Nodes shoul
-00003880: 6420 636f 7272 6573 706f 6e64 2074 6f20  d correspond to 
-00003890: 6578 6973 7465 6e74 2062 6f64 7970 6172  existent bodypar
-000038a0: 7473 4e72 9200 0000 6301 0000 0000 0000  tsNr....c.......
-000038b0: 0000 0000 0004 0000 000a 0000 0013 0000  ................
-000038c0: 0073 3600 0000 6900 7c00 5d2e 5c02 7d01  .s6...i.|.].\.}.
-000038d0: 5c02 7d02 7d03 7c02 7400 6a01 a002 7c03  \.}.}.|.t.j...|.
-000038e0: 8800 7c01 6400 6602 1900 8800 7c01 6401  ..|.d.f.....|.d.
-000038f0: 6602 1900 a103 9302 7104 5300 2902 7231  f.......q.S.).r1
-00003900: 0000 0072 0100 0000 2903 7281 0000 0072  ...r....).r....r
-00003910: 8200 0000 da0e 6270 6172 745f 6469 7374  ......bpart_dist
-00003920: 616e 6365 2904 724a 0000 0072 4b00 0000  ance).rJ...rK...
-00003930: 72e4 0000 0072 5400 0000 2901 da06 7363  r....rT...)...sc
-00003940: 616c 6573 7226 0000 0072 2700 0000 7297  alesr&...r'...r.
-00003950: 0000 00fb 0100 0073 0400 0000 0602 0aff  .......s........
-00003960: 7a29 5072 6f6a 6563 742e 6765 745f 6469  z)Project.get_di
-00003970: 7374 616e 6365 732e 3c6c 6f63 616c 733e  stances.<locals>
-00003980: 2e3c 6469 6374 636f 6d70 3e63 0100 0000  .<dictcomp>c....
-00003990: 0000 0000 0000 0000 0200 0000 0700 0000  ................
-000039a0: 1300 0000 7324 0000 0067 007c 005d 1c7d  ....s$...g.|.].}
-000039b0: 0174 00a0 0187 0066 0164 0064 0184 087c  .t.....f.d.d...|
-000039c0: 0144 0083 01a1 0191 0271 0453 0029 0263  .D.......q.S.).c
-000039d0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-000039e0: 0400 0000 1300 0000 7314 0000 0067 007c  ........s....g.|
-000039f0: 005d 0c7d 017c 0188 0076 0091 0271 0453  .].}.|...v...q.S
-00003a00: 0072 2600 0000 7226 0000 0072 4900 0000  .r&...r&...rI...
-00003a10: a901 da05 6e6f 6465 7372 2600 0000 7227  ....nodesr&...r'
-00003a20: 0000 0072 4c00 0000 0202 0000 724d 0000  ...rL.......rM..
-00003a30: 007a 3450 726f 6a65 6374 2e67 6574 5f64  .z4Project.get_d
-00003a40: 6973 7461 6e63 6573 2e3c 6c6f 6361 6c73  istances.<locals
-00003a50: 3e2e 3c6c 6973 7463 6f6d 703e 2e3c 6c69  >.<listcomp>.<li
-00003a60: 7374 636f 6d70 3e29 0272 dd00 0000 7257  stcomp>).r....rW
-00003a70: 0000 0029 0272 4a00 0000 72b4 0000 0072  ...).rJ...r....r
-00003a80: f100 0000 7226 0000 0072 2700 0000 724c  ....r&...r'...rL
-00003a90: 0000 0002 0200 0072 4d00 0000 6301 0000  .......rM...c...
-00003aa0: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-00003ab0: 0013 0000 0073 1a00 0000 6700 7c00 5d12  .....s....g.|.].
-00003ac0: 7d01 8800 6a00 7c01 7600 7204 7c01 9102  }...j.|.v.r.|...
-00003ad0: 7104 5300 7226 0000 0029 0172 6500 0000  q.S.r&...).re...
-00003ae0: 2902 724a 0000 00da 0464 6973 7472 5500  ).rJ.....distrU.
-00003af0: 0000 7226 0000 0072 2700 0000 724c 0000  ..r&...r'...rL..
-00003b00: 0008 0200 0072 4d00 0000 290c 7280 0000  .....rM...).r...
-00003b10: 0072 6400 0000 72b5 0000 00da 046b 6579  .rd...r......key
-00003b20: 7372 b700 0000 72ee 0000 0072 f000 0000  sr....r....r....
-00003b30: da09 656e 756d 6572 6174 6572 cb00 0000  ..enumerater....
-00003b40: 72c3 0000 0072 6500 0000 72c9 0000 0029  r....re...r....)
-00003b50: 0672 5600 0000 72e2 0000 0072 7f00 0000  .rV...r....r....
-00003b60: da0d 6469 7374 616e 6365 5f64 6963 7472  ..distance_dictr
-00003b70: e400 0000 da03 7661 6c72 2600 0000 2904  ......valr&...).
-00003b80: 72f2 0000 0072 f000 0000 7256 0000 0072  r....r....rV...r
-00003b90: e200 0000 7227 0000 00da 0d67 6574 5f64  ....r'.....get_d
-00003ba0: 6973 7461 6e63 6573 e301 0000 7334 0000  istances....s4..
-00003bb0: 0000 0b04 0108 0206 0108 011c 020a 0102  ................
-00003bc0: ff08 0202 fe04 0416 020a 020a fe06 050c  ................
-00003bd0: 0108 011e ff0a 0406 0110 0104 011a ff0a  ................
-00003be0: 050c 0114 027a 1550 726f 6a65 6374 2e67  .....z.Project.g
-00003bf0: 6574 5f64 6973 7461 6e63 6573 6303 0000  et_distancesc...
-00003c00: 0000 0000 0000 0000 000b 0000 000b 0000  ................
-00003c10: 0043 0000 0073 0201 0000 7c02 720c 7400  .C...s....|.r.t.
-00003c20: 6401 8301 0100 6700 7d03 7c00 6a01 4400  d.....g.}.|.j.D.
-00003c30: 5d1a 7d04 7c03 7402 6a03 a004 7c00 6a05  ].}.|.t.j...|.j.
-00003c40: 7c04 1900 a101 3700 7d03 7116 6402 6403  |.....7.}.q.d.d.
-00003c50: 8400 7c03 4400 8301 7d03 6900 7d05 7a80  ..|.D...}.i.}.z.
-00003c60: 7c01 a006 a100 4400 5d72 5c02 7d06 7d07  |.....D.]r\.}.}.
-00003c70: 6700 7d08 7c03 4400 5d4a 7d09 7407 a008  g.}.|.D.]J}.t...
-00003c80: 7402 6a03 a009 740a a00b 7c07 7c09 1900  t.j...t...|.|...
-00003c90: a101 a00c 6404 7c07 6a0d 6405 1900 6406  ....d.|.j.d...d.
-00003ca0: 6703 a101 a101 6a0e a101 7d0a 740f 7c09  g.....j...}.t.|.
-00003cb0: 8301 6701 7c0a 5f10 7c08 a011 7c0a a101  ..g.|._.|...|...
-00003cc0: 0100 715e 7407 6a12 7c08 6407 6408 8d02  ..q^t.j.|.d.d...
-00003cd0: 7d08 7c08 7c05 7c06 3c00 714e 5700 6e1a  }.|.|.|.<.qNW.n.
-00003ce0: 0400 7413 79de 0100 0100 0100 7413 6409  ..t.y.......t.d.
-00003cf0: 8301 8201 5900 6e02 3000 7c05 a014 a100  ....Y.n.0.|.....
-00003d00: 4400 5d14 7d06 7c01 7c06 1900 6a15 7c05  D.].}.|.|...j.|.
-00003d10: 7c06 1900 5f15 71e8 7c05 5300 290a 619b  |..._.q.|.S.).a.
-00003d20: 0100 0043 6f6d 7075 7465 2061 6c6c 2074  ...Compute all t
-00003d30: 6865 2061 6e67 6c65 7320 6265 7477 6565  he angles betwee
-00003d40: 6e20 6164 6a61 6365 6e74 2062 6f64 7970  n adjacent bodyp
-00003d50: 6172 7420 7472 696f 7320 7065 7220 7669  art trios per vi
-00003d60: 6465 6f20 616e 6420 7065 7220 6672 616d  deo and per fram
-00003d70: 6520 696e 2074 6865 2064 6174 612e 0a0a  e in the data...
-00003d80: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-00003d90: 2020 2020 2020 2020 2020 7461 625f 6469            tab_di
-00003da0: 6374 2028 6469 6374 293a 2044 6963 7469  ct (dict): Dicti
-00003db0: 6f6e 6172 7920 6f66 2070 616e 6461 7320  onary of pandas 
-00003dc0: 4461 7461 4672 616d 6573 2063 6f6e 7461  DataFrames conta
-00003dd0: 696e 696e 6720 7468 6520 7472 616a 6563  ining the trajec
-00003de0: 746f 7269 6573 206f 6620 616c 6c20 626f  tories of all bo
-00003df0: 6479 7061 7274 732e 0a20 2020 2020 2020  dyparts..       
-00003e00: 2020 2020 2076 6572 626f 7365 2028 626f       verbose (bo
-00003e10: 6f6c 293a 2049 6620 5472 7565 2c20 7072  ol): If True, pr
-00003e20: 696e 7473 2070 726f 6772 6573 732e 2044  ints progress. D
-00003e30: 6566 6175 6c74 7320 746f 2054 7275 652e  efaults to True.
-00003e40: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00003e50: 733a 0a20 2020 2020 2020 2020 2020 2064  s:.            d
-00003e60: 6963 743a 2044 6963 7469 6f6e 6172 7920  ict: Dictionary 
-00003e70: 6f66 2070 616e 6461 7320 4461 7461 4672  of pandas DataFr
-00003e80: 616d 6573 2063 6f6e 7461 696e 696e 6720  ames containing 
-00003e90: 7468 6520 6469 7374 616e 6365 7320 6265  the distances be
-00003ea0: 7477 6565 6e20 616c 6c20 626f 6479 7061  tween all bodypa
-00003eb0: 7274 732e 0a0a 2020 2020 2020 2020 7a13  rts...        z.
-00003ec0: 436f 6d70 7574 696e 6720 616e 676c 6573  Computing angles
-00003ed0: 2e2e 2e63 0100 0000 0000 0000 0000 0000  ...c............
-00003ee0: 0200 0000 0400 0000 5300 0000 731c 0000  ........S...s...
-00003ef0: 0067 007c 005d 147d 0174 007c 0183 0164  .g.|.].}.t.|...d
-00003f00: 006b 0272 047c 0191 0271 0453 0029 0172  .k.r.|...q.S.).r
-00003f10: 2e00 0000 2901 725e 0000 0072 4900 0000  ....).r^...rI...
-00003f20: 7226 0000 0072 2600 0000 7227 0000 0072  r&...r&...r'...r
-00003f30: 4c00 0000 2302 0000 724d 0000 007a 2650  L...#...rM...z&P
-00003f40: 726f 6a65 6374 2e67 6574 5f61 6e67 6c65  roject.get_angle
-00003f50: 732e 3c6c 6f63 616c 733e 2e3c 6c69 7374  s.<locals>.<list
-00003f60: 636f 6d70 3e72 2e00 0000 7201 0000 0072  comp>r....r....r
-00003f70: 9200 0000 7231 0000 0072 ab00 0000 7ad1  ....r1...r....z.
-00003f80: 4172 6520 796f 7520 7573 696e 6720 6120  Are you using a 
-00003f90: 6375 7374 6f6d 206c 6162 656c 6c69 6e67  custom labelling
-00003fa0: 2073 6368 656d 653f 204f 7574 2074 7574   scheme? Out tut
-00003fb0: 6f72 6961 6c73 206d 6179 2068 656c 7021  orials may help!
-00003fc0: 2049 6e20 6361 7365 2079 6f75 2772 6520   In case you're 
-00003fd0: 6e6f 742c 2061 7265 2074 6865 7265 206d  not, are there m
-00003fe0: 756c 7469 706c 6520 616e 696d 616c 7320  ultiple animals 
-00003ff0: 696e 2079 6f75 7220 7369 6e67 6c65 2d61  in your single-a
-00004000: 6e69 6d61 6c20 444c 4320 7669 6465 6f3f  nimal DLC video?
-00004010: 204d 616b 6520 7375 7265 2074 6f20 7365   Make sure to se
-00004020: 7420 7468 6520 616e 696d 616c 5f69 6473  t the animal_ids
-00004030: 2070 6172 616d 6574 6572 2069 6e20 6465   parameter in de
-00004040: 6570 6f66 2e64 6174 612e 5072 6f6a 6563  epof.data.Projec
-00004050: 7429 1672 8000 0000 7233 0000 0072 8100  t).r....r3...r..
-00004060: 0000 7282 0000 00da 1565 6e75 6d65 7261  ..r......enumera
-00004070: 7465 5f61 6c6c 5f62 7269 6467 6573 7263  te_all_bridgesrc
-00004080: 0000 0072 cb00 0000 72be 0000 0072 db00  ...r....r....r..
-00004090: 0000 da05 616e 676c 6572 dd00 0000 72de  ....angler....r.
-000040a0: 0000 00da 0772 6573 6861 7065 72d4 0000  .....reshaper...
-000040b0: 0072 c100 0000 72d1 0000 0072 b700 0000  .r....r....r....
-000040c0: da06 6170 7065 6e64 72d7 0000 00da 084b  ..appendr......K
-000040d0: 6579 4572 726f 7272 f400 0000 72c9 0000  eyErrorr....r...
-000040e0: 0029 0b72 5600 0000 72e2 0000 0072 7f00  .).rV...r....r..
-000040f0: 0000 da07 6272 6964 6765 7372 4b00 0000  ....bridgesrK...
-00004100: da0a 616e 676c 655f 6469 6374 72e4 0000  ..angle_dictr...
-00004110: 0072 5400 0000 da04 6461 7473 da06 636c  .rT.....dats..cl
-00004120: 6971 7565 da03 6461 7472 2600 0000 7226  ique..datr&...r&
-00004130: 0000 0072 2700 0000 da0a 6765 745f 616e  ...r'.....get_an
-00004140: 676c 6573 1102 0000 7336 0000 0000 0b04  gles....s6......
-00004150: 0108 0304 010a 0118 010e 0204 0102 0110  ................
-00004160: 0204 0108 0104 0106 011e ff04 ff04 060c  ................
-00004170: 010c 020e 020e 010c 0102 0102 ff0a 070c  ................
-00004180: 0112 027a 1250 726f 6a65 6374 2e67 6574  ...z.Project.get
-00004190: 5f61 6e67 6c65 7363 0300 0000 0000 0000  _anglesc........
-000041a0: 0000 0000 0800 0000 0900 0000 0300 0000  ................
-000041b0: 73f8 0000 007c 0272 0c74 0064 0183 0101  s....|.r.t.d....
-000041c0: 0069 007d 037a c47c 01a0 01a1 0044 005d  .i.}.z.|.....D.]
-000041d0: b65c 027d 047d 0574 02a0 03a1 007d 067c  .\.}.}.t.....}.|
-000041e0: 006a 0444 005d 9689 0088 0064 026b 0272  .j.D.].....d.k.r
-000041f0: 4064 0389 007c 056a 0564 0364 0385 0274  @d...|.j.d.d...t
-00004200: 066a 07a0 087c 056a 0988 00a1 0266 0219  .j...|.j.....f..
-00004210: 007d 077c 076a 0a87 0066 0164 0464 0584  .}.|.j...f.d.d..
-00004220: 0864 0664 078d 027d 0774 026a 037c 07a0  .d.d...}.t.j.|..
-00004230: 0ba1 007c 076a 0c67 0064 08a2 0164 098d  ...|.j.g.d...d..
-00004240: 03a0 0d64 0aa0 0e88 0064 0375 0172 9e88  ...d.....d.u.r..
-00004250: 006e 0264 0288 0064 0375 0172 ac64 0b6e  .n.d...d.u.r.d.n
-00004260: 0264 02a1 02a1 017d 0774 026a 0f7c 067c  .d.....}.t.j.|.|
-00004270: 0767 0264 0664 078d 027d 0671 307c 067c  .g.d.d...}.q0|.|
-00004280: 037c 043c 0071 1a57 006e 1e04 0074 1079  .|.<.q.W.n...t.y
-00004290: f201 0001 0001 0074 11a0 1264 0ca1 0101  .......t...d....
-000042a0: 0059 0064 0353 0030 007c 0353 0029 0d61  .Y.d.S.0.|.S.).a
-000042b0: 9301 0000 436f 6d70 7574 6520 616c 6c20  ....Compute all 
-000042c0: 7265 6c65 7661 6e74 2061 7265 6173 2028  relevant areas (
-000042d0: 6865 6164 2c20 746f 7273 6f2c 2062 6163  head, torso, bac
-000042e0: 6b29 2070 6572 2076 6964 656f 2061 6e64  k) per video and
-000042f0: 2070 6572 2066 7261 6d65 2069 6e20 7468   per frame in th
-00004300: 6520 6461 7461 2e0a 0a20 2020 2020 2020  e data...       
-00004310: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
-00004320: 2020 2074 6162 5f64 6963 7420 2864 6963     tab_dict (dic
-00004330: 7429 3a20 4469 6374 696f 6e61 7279 206f  t): Dictionary o
-00004340: 6620 7061 6e64 6173 2044 6174 6146 7261  f pandas DataFra
-00004350: 6d65 7320 636f 6e74 6169 6e69 6e67 2074  mes containing t
-00004360: 6865 2074 7261 6a65 6374 6f72 6965 7320  he trajectories 
-00004370: 6f66 2061 6c6c 2062 6f64 7970 6172 7473  of all bodyparts
-00004380: 2e0a 2020 2020 2020 2020 2020 2020 7665  ..            ve
-00004390: 7262 6f73 6520 2862 6f6f 6c29 3a20 4966  rbose (bool): If
-000043a0: 2054 7275 652c 2070 7269 6e74 7320 7072   True, prints pr
-000043b0: 6f67 7265 7373 2e20 4465 6661 756c 7473  ogress. Defaults
-000043c0: 2074 6f20 5472 7565 2e0a 0a20 2020 2020   to True...     
-000043d0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-000043e0: 2020 2020 2020 2020 6469 6374 3a20 4469          dict: Di
-000043f0: 6374 696f 6e61 7279 206f 6620 7061 6e64  ctionary of pand
-00004400: 6173 2044 6174 6146 7261 6d65 7320 636f  as DataFrames co
-00004410: 6e74 6169 6e69 6e67 2074 6865 2064 6973  ntaining the dis
-00004420: 7461 6e63 6573 2062 6574 7765 656e 2061  tances between a
-00004430: 6c6c 2062 6f64 7970 6172 7473 2e0a 0a20  ll bodyparts... 
-00004440: 2020 2020 2020 207a 1243 6f6d 7075 7469         z.Computi
-00004450: 6e67 2061 7265 6173 2e2e 2e72 2c00 0000  ng areas...r,...
-00004460: 4e63 0100 0000 0000 0000 0000 0000 0100  Nc..............
-00004470: 0000 0400 0000 1300 0000 7310 0000 0074  ..........s....t
-00004480: 006a 016a 027c 0088 0064 018d 0253 0029  .j.j.|...d...S.)
-00004490: 024e 2901 da09 616e 696d 616c 5f69 6429  .N)...animal_id)
-000044a0: 0372 8100 0000 7282 0000 00da 0d63 6f6d  .r....r......com
-000044b0: 7075 7465 5f61 7265 6173 a901 72a5 0000  pute_areas..r...
-000044c0: 00a9 0172 9600 0000 7226 0000 0072 2700  ...r....r&...r'.
-000044d0: 0000 72a4 0000 0063 0200 0072 4d00 0000  ..r....c...rM...
-000044e0: 7a23 5072 6f6a 6563 742e 6765 745f 6172  z#Project.get_ar
-000044f0: 6561 732e 3c6c 6f63 616c 733e 2e3c 6c61  eas.<locals>.<la
-00004500: 6d62 6461 3e72 3100 0000 72ab 0000 0029  mbda>r1...r....)
-00004510: 04da 0968 6561 645f 6172 6561 da0a 746f  ...head_area..to
-00004520: 7273 6f5f 6172 6561 da09 6261 636b 5f61  rso_area..back_a
-00004530: 7265 61da 0966 756c 6c5f 6172 6561 a902  rea..full_area..
-00004540: 72c9 0000 0072 b700 0000 7a04 7b7d 7b7d  r....r....z.{}{}
-00004550: 728c 0000 007a 8049 7420 7365 656d 7320  r....z.It seems 
-00004560: 796f 7527 7265 2075 7369 6e67 2061 2063  you're using a c
-00004570: 7573 746f 6d20 6c61 6265 6c6c 696e 6720  ustom labelling 
-00004580: 7363 6865 6d65 2077 6869 6368 2069 7320  scheme which is 
-00004590: 6d69 7373 696e 6720 6b65 7920 626f 6479  missing key body
-000045a0: 2070 6172 7473 2e20 596f 7520 6361 6e20   parts. You can 
-000045b0: 7072 6f63 6565 642c 2062 7574 206e 6f20  proceed, but no 
-000045c0: 6172 6561 7320 7769 6c6c 2062 6520 636f  areas will be co
-000045d0: 6d70 7574 6564 2e29 1372 8000 0000 72cb  mputed.).r....r.
-000045e0: 0000 0072 be00 0000 72db 0000 0072 3300  ...r....r....r3.
-000045f0: 0000 72c3 0000 0072 8100 0000 7282 0000  ..r....r....r...
-00004600: 00da 0e66 696c 7465 725f 636f 6c75 6d6e  ...filter_column
-00004610: 7372 b700 0000 da05 6170 706c 79da 0774  sr......apply..t
-00004620: 6f5f 6c69 7374 72c9 0000 00da 0a61 6464  o_listr......add
-00004630: 5f70 7265 6669 7872 6c00 0000 72d7 0000  _prefixrl...r...
-00004640: 0072 fd00 0000 da08 7761 726e 696e 6773  .r......warnings
-00004650: da04 7761 726e 2908 7256 0000 0072 e200  ..warn).rV...r..
-00004660: 0000 727f 0000 00da 0a61 7265 6173 5f64  ..r......areas_d
-00004670: 6963 7472 e400 0000 7254 0000 00da 0965  ictr....rT.....e
-00004680: 7870 5f74 6162 6c65 da0d 6375 7272 656e  xp_table..curren
-00004690: 745f 7461 626c 6572 2600 0000 7207 0100  t_tabler&...r...
-000046a0: 0072 2700 0000 da09 6765 745f 6172 6561  .r'.....get_area
-000046b0: 7344 0200 0073 4200 0000 000b 0401 0802  sD...sB.........
-000046c0: 0402 0201 1002 0802 0a02 0801 0403 0401  ................
-000046d0: 16ff 0403 0401 0cff 0603 0401 0601 0401  ................
-000046e0: 06fd 0605 0401 0e01 0efe 02fb 040b 1402  ................
-000046f0: 0e02 0c01 0401 02ff 0403 0802 7a11 5072  ............z.Pr
-00004700: 6f6a 6563 742e 6765 745f 6172 6561 7329  oject.get_areas)
-00004710: 0372 7f00 0000 da05 666f 7263 6572 1900  .r......forcer..
-00004720: 0000 6303 0000 0000 0000 0000 0000 0009  ..c.............
-00004730: 0000 0017 0000 0043 0000 0073 6e01 0000  .......C...sn...
-00004740: 7c01 720c 7400 6401 8301 0100 7c02 7240  |.r.t.d.....|.r@
-00004750: 7401 6a02 a003 7401 6a02 a004 7c00 6a05  t.j...t.j...|.j.
-00004760: 7c00 6a06 a102 a101 7240 7407 7401 6a02  |.j.....r@t.t.j.
-00004770: a004 7c00 6a05 7c00 6a06 a102 8301 0100  ..|.j.|.j.......
-00004780: 7c00 a008 a100 0100 7409 740a a00b 740c  |.......t.t...t.
-00004790: a00d 7401 6a02 a004 7c00 6a0e 7c00 6a0f  ..t.j...|.j.|.j.
-000047a0: 6402 1900 a102 a101 6a10 a101 8301 7c00  d.......j.....|.
-000047b0: 5f10 7c00 a011 7c01 a101 5c02 7d03 7d04  _.|...|...\.}.}.
-000047c0: 7c00 6a12 6403 7501 72a4 7c03 a013 a100  |.j.d.u.r.|.....
-000047d0: 7c00 6a12 a013 a100 6b02 73a4 4a00 6404  |.j.....k.s.J.d.
-000047e0: 8301 8201 6403 7d05 6403 7d06 6403 7d07  ....d.}.d.}.d.}.
-000047f0: 7c00 a014 7c03 7c01 a102 5c03 7c00 5f15  |...|.|...\.|._.
-00004800: 7c00 5f16 7c00 5f17 7c00 6a18 72da 7c00  |._.|._.|.j.r.|.
-00004810: a019 7c03 7c01 a102 7d05 7c00 6a1a 72ec  ..|.|...}.|.j.r.
-00004820: 7c00 a01b 7c03 7c01 a102 7d06 7c00 6a1c  |...|.|...}.|.j.
-00004830: 72fe 7c00 a01d 7c03 7c01 a102 7d07 741e  r.|...|.|...}.t.
-00004840: 7c00 6a05 7c00 6a06 7c06 7c00 6a1f 7c07  |.j.|.j.|.|.j.|.
-00004850: 7c00 6a20 7c00 6a21 7c00 6a22 7c05 7c00  |.j |.j!|.j"|.|.
-00004860: 6a23 7c00 6a24 7c00 6a10 7c00 6a12 7c00  j#|.j$|.j.|.j.|.
-00004870: 6a05 7c04 7c00 6a15 7c00 6a16 7c03 7c00  j.|.|.j.|.j.|.|.
-00004880: 6a25 7c00 6a0f 7c00 6a17 6405 8d15 7d08  j%|.j.|.j.d...}.
-00004890: 7c08 6a26 6406 6407 8d01 0100 7c01 9001  |.j&d.d.....|...
-000048a0: 726a 7400 6408 8301 0100 7c08 5300 2909  rjt.d.....|.S.).
-000048b0: 6130 0100 0047 656e 6572 6174 6520 6120  a0...Generate a 
-000048c0: 6465 6570 6f66 2e43 6f6f 7264 696e 6174  deepof.Coordinat
-000048d0: 6573 2064 6174 6173 6574 2075 7369 6e67  es dataset using
-000048e0: 2061 6c6c 2074 6865 206f 7074 696f 6e73   all the options
-000048f0: 2073 7065 6369 6669 6564 2064 7572 696e   specified durin
-00004900: 6720 696e 6974 6961 6c69 7a61 7469 6f6e  g initialization
-00004910: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
-00004920: 0a20 2020 2020 2020 2020 2020 2076 6572  .            ver
-00004930: 626f 7365 2028 626f 6f6c 293a 2049 6620  bose (bool): If 
-00004940: 5472 7565 2c20 7072 696e 7473 2070 726f  True, prints pro
-00004950: 6772 6573 732e 2044 6566 6175 6c74 7320  gress. Defaults 
-00004960: 746f 2054 7275 652e 0a0a 2020 2020 2020  to True...      
-00004970: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-00004980: 2020 2020 2020 2063 6f6f 7264 696e 6174         coordinat
-00004990: 6573 3a20 4465 6570 6f66 2e43 6f6f 7264  es: Deepof.Coord
-000049a0: 696e 6174 6573 206f 626a 6563 7420 636f  inates object co
-000049b0: 6e74 6169 6e69 6e67 2074 6865 2074 7261  ntaining the tra
-000049c0: 6a65 6374 6f72 6965 7320 6f66 2061 6c6c  jectories of all
-000049d0: 2062 6f64 7970 6172 7473 2e0a 0a20 2020   bodyparts...   
-000049e0: 2020 2020 207a 2153 6574 7469 6e67 2075       z!Setting u
-000049f0: 7020 7072 6f6a 6563 7420 6469 7265 6374  p project direct
-00004a00: 6f72 6965 732e 2e2e 7201 0000 004e 7a2f  ories...r....Nz/
-00004a10: 6578 7065 7269 6d65 6e74 616c 2049 4473  experimental IDs
-00004a20: 2069 6e20 6578 705f 636f 6e64 6974 696f   in exp_conditio
-00004a30: 6e73 2064 6f20 6e6f 7420 6d61 7463 6829  ns do not match)
-00004a40: 1572 1800 0000 723e 0000 0072 6100 0000  .r....r>...ra...
-00004a50: 7233 0000 0072 6200 0000 7234 0000 0072  r3...rb...r4...r
-00004a60: 5f00 0000 7235 0000 0072 6400 0000 7263  _...r5...rd...rc
-00004a70: 0000 00da 1265 7863 6c75 6465 645f 626f  .....excluded_bo
-00004a80: 6479 7061 7274 7372 6700 0000 7238 0000  dypartsrg...r8..
-00004a90: 0072 1e00 0000 72ad 0000 0072 f000 0000  .r....r....r....
-00004aa0: da0c 6172 656e 615f 7061 7261 6d73 725d  ..arena_paramsr]
-00004ab0: 0000 00da 1274 7261 696e 6564 5f6d 6f64  .....trained_mod
-00004ac0: 656c 5f70 6174 6872 5c00 0000 da10 7669  el_pathr\.....vi
-00004ad0: 6465 6f5f 7265 736f 6c75 7469 6f6e 46a9  deo_resolutionF.
-00004ae0: 01da 0974 696d 6573 7461 6d70 fa05 446f  ...timestamp..Do
-00004af0: 6e65 2129 2772 8000 0000 721d 0000 0072  ne!)'r....r....r
-00004b00: 1e00 0000 7273 0000 0072 1f00 0000 7218  ....rs...r....r.
-00004b10: 0000 0072 3e00 0000 7205 0000 0072 7800  ...r>...r....rx.
-00004b20: 0000 da03 696e 7472 dd00 0000 da05 726f  ....intr......ro
-00004b30: 756e 64da 0470 696d 73da 0d49 6d61 6765  und..pims..Image
-00004b40: 494f 5265 6164 6572 723f 0000 0072 5c00  IOReaderr?...r\.
-00004b50: 0000 7267 0000 0072 ec00 0000 7238 0000  ..rg...r....r8..
-00004b60: 0072 f400 0000 7284 0000 0072 f000 0000  .r....r....r....
-00004b70: 7219 0100 0072 1b01 0000 7264 0000 0072  r....r....rd...r
-00004b80: f800 0000 7261 0000 0072 0301 0000 7262  ....ra...r....rb
-00004b90: 0000 0072 1601 0000 721a 0000 0072 3300  ...r....r....r3.
-00004ba0: 0000 7234 0000 0072 5f00 0000 7235 0000  ..r4...r_...r5..
-00004bb0: 0072 6300 0000 7237 0000 0072 5900 0000  .rc...r7...rY...
-00004bc0: da04 7361 7665 2909 7256 0000 0072 7f00  ..save).rV...r..
-00004bd0: 0000 7217 0100 0072 5d00 0000 72ad 0000  ..r....r]...r...
-00004be0: 0072 6400 0000 7261 0000 0072 6200 0000  .rd...ra...rb...
-00004bf0: 72a6 0000 0072 2600 0000 7226 0000 0072  r....r&...r&...r
-00004c00: 2700 0000 da06 6372 6561 7465 7c02 0000  '.....create|...
-00004c10: 7372 0000 0000 0a04 0108 021e 0116 0208  sr..............
-00004c20: 0102 0104 0104 0114 ff04 ff02 ff06 080e  ................
-00004c30: 010a 0210 ff04 0202 fe04 0404 0104 0104  ................
-00004c40: 0304 0104 ff10 0406 010c 0206 010c 0206  ................
-00004c50: 010c 0202 0104 0104 0102 0104 0102 0104  ................
-00004c60: 0104 0104 0102 0104 0104 0104 0104 0104  ................
-00004c70: 0102 0104 0104 0102 0104 0104 0104 eb06  ................
-00004c80: 190c 0206 0108 027a 0e50 726f 6a65 6374  .......z.Project
-00004c90: 2e63 7265 6174 6563 0200 0000 0000 0000  .createc........
-00004ca0: 0000 0000 0200 0000 0200 0000 4300 0000  ............C...
-00004cb0: 730a 0000 007c 017c 005f 0064 0053 00a9  s....|.|._.d.S..
-00004cc0: 014e 7279 0000 00a9 0272 5600 0000 da05  .Nry.....rV.....
-00004cd0: 7661 6c75 6572 2600 0000 7226 0000 0072  valuer&...r&...r
-00004ce0: 2700 0000 7264 0000 00cd 0200 0073 0200  '...rd.......s..
-00004cf0: 0000 0002 6302 0000 0000 0000 0000 0000  ....c...........
-00004d00: 0002 0000 0002 0000 0043 0000 0073 0a00  .........C...s..
-00004d10: 0000 7c01 7c00 5f00 6400 5300 7225 0100  ..|.|._.d.S.r%..
-00004d20: 0072 7b00 0000 7226 0100 0072 2600 0000  .r{...r&...r&...
-00004d30: 7226 0000 0072 2700 0000 7265 0000 00d1  r&...r'...re....
-00004d40: 0200 0073 0200 0000 0002 6302 0000 0000  ...s......c.....
-00004d50: 0000 0000 0000 0002 0000 0002 0000 0043  ...............C
-00004d60: 0000 0073 0a00 0000 7c01 7c00 5f00 6400  ...s....|.|._.d.
-00004d70: 5300 7225 0100 0072 7d00 0000 7226 0100  S.r%...r}...r&..
-00004d80: 0072 2600 0000 7226 0000 0072 2700 0000  .r&...r&...r'...
-00004d90: 7261 0000 00d5 0200 0073 0200 0000 0002  ra.......s......
-00004da0: 2901 4629 0154 2901 5429 0154 2901 5429  ).F).T).T).T).T)
-00004db0: 0254 4629 2272 5800 0000 da0a 5f5f 6d6f  .TF)"rX.....__mo
-00004dc0: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-00004dd0: 6d65 5f5f da07 5f5f 646f 635f 5f72 d100  me__..__doc__r..
-00004de0: 0000 721d 0000 0072 1e00 0000 721f 0000  ..r....r....r...
-00004df0: 0072 1300 0000 72a2 0000 00da 0462 6f6f  .r....r......boo
-00004e00: 6cda 0464 6963 7472 1f01 0000 72c0 0000  l..dictr....r...
-00004e10: 0072 6900 0000 726d 0000 0072 6e00 0000  .ri...rm...rn...
-00004e20: 7278 0000 00da 0870 726f 7065 7274 7972  rx.....propertyr
-00004e30: 6400 0000 7265 0000 0072 6100 0000 72b5  d...re...ra...r.
-00004e40: 0000 0072 dd00 0000 72de 0000 0072 8400  ...r....r....r..
-00004e50: 0000 7214 0000 0072 ec00 0000 72f8 0000  ..r....r....r...
-00004e60: 0072 0301 0000 7216 0100 0072 2500 0000  .r....r....r%...
-00004e70: 7224 0100 00da 0673 6574 7465 7272 2600  r$.....setterr&.
-00004e80: 0000 7226 0000 0072 2600 0000 7227 0000  ..r&...r&...r'..
-00004e90: 0072 2900 0000 5400 0000 737e 0000 0008  .r)...T...s~....
-00004ea0: 0104 0802 0102 0102 0102 0108 0102 0102  ................
-00004eb0: 0102 0102 0102 0102 0102 010a 0102 0102  ................
-00004ec0: 0102 0102 0102 0102 ec02 0202 0102 0102  ................
-00004ed0: 0102 0102 0102 0102 0102 0102 0102 0102  ................
-00004ee0: 0102 0102 0102 0102 0102 0102 0102 0102  ................
-00004ef0: ec0c 6808 0408 0408 4902 010a 0402 010a  ..h.....I.......
-00004f00: 0402 010a 0416 1712 7f00 2a14 2e14 3314  ..........*...3.
-00004f10: 3814 5104 010a 0304 010a 0304 0172 2900  8.Q..........r).
-00004f20: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00004f30: 0000 001e 0000 0040 0000 0073 da01 0000  .......@...s....
-00004f40: 6500 5a01 6400 5a02 6401 5a03 6402 6504  e.Z.d.Z.d.Z.d.e.
-00004f50: 6403 6701 8301 6402 6402 6402 6402 6402  d.g...d.d.d.d.d.
-00004f60: 6607 6505 6505 6505 6506 6a07 6505 6505  f.e.e.e.e.j.e.e.
-00004f70: 6508 6506 6a09 650a 650b 6508 6505 650b  e.e.j.e.e.e.e.e.
-00004f80: 650b 6508 650b 6508 6508 650c 6a0d 650e  e.e.e.e.e.e.j.e.
-00004f90: 6508 6404 9c15 6405 6406 8405 5a0f 6407  e.d...d.d...Z.d.
-00004fa0: 6408 8400 5a10 6409 640a 8400 5a11 6442  d...Z.d.d...Z.dB
-00004fb0: 6505 6512 650a 6505 6512 6505 6512 6513  e.e.e.e.e.e.e.e.
-00004fc0: 6514 640e 9c09 640f 6410 8405 5a15 6443  e.d...d.d...Z.dC
-00004fd0: 650a 6505 6512 6512 6513 6514 6411 9c06  e.e.e.e.e.e.d...
-00004fe0: 6412 6413 8405 5a16 6444 6512 650a 6505  d.d...Z.dDe.e.e.
-00004ff0: 6512 6513 6514 6414 9c06 6415 6416 8405  e.e.e.d...d.d...
-00005000: 5a17 6445 650a 6505 6514 6418 9c03 6419  Z.dEe.e.e.d...d.
-00005010: 641a 8405 5a18 6446 6512 641b 9c01 641c  d...Z.dFe.d...d.
-00005020: 641d 8405 5a19 651a 641e 641f 8400 8301  d...Z.e.d.d.....
-00005030: 5a1b 6420 6421 8400 5a1c 6422 6423 8400  Z.d d!..Z.d"d#..
-00005040: 5a1d 651a 6424 6425 8400 8301 5a1e 6447  Z.e.d$d%....Z.dG
-00005050: 650e 6505 6512 6426 9c03 6427 6428 8405  e.e.e.d&..d'd(..
-00005060: 5a1f 6448 6505 6512 6429 9c02 642a 642b  Z.dHe.e.d)..d*d+
-00005070: 8405 5a20 6449 6505 6514 6505 6512 6505  ..Z dIe.e.e.e.e.
-00005080: 6512 6514 642c 9c07 642d 642e 8405 5a21  e.e.d,..d-d...Z!
-00005090: 6900 640b 6506 6a22 640b 642f 640b 6606  i.d.e.j"d.d/d.f.
-000050a0: 6513 6512 650a 6512 650a 6512 6514 6430  e.e.e.e.e.e.e.d0
-000050b0: 9c07 6431 6432 8405 5a23 644a 6524 6506  ..d1d2..Z#dJe$e.
-000050c0: 6a09 6506 6a09 6506 6a09 6506 6a09 6604  j.e.j.e.j.e.j.f.
-000050d0: 1900 6506 6a09 6505 6505 650a 650a 650a  ..e.j.e.e.e.e.e.
-000050e0: 6512 6512 650a 6525 6525 6505 6505 6525  e.e.e.e%e%e.e.e%
-000050f0: 6525 6505 6505 6512 6512 6505 650a 6505  e%e.e.e.e.e.e.e.
-00005100: 650a 6525 6512 6525 6524 643f 9c1c 6440  e.e%e.e%e$d?..d@
-00005110: 6441 8405 5a26 6402 5300 294b 721a 0000  dA..Z&d.S.)Kr...
-00005120: 007a 8443 6c61 7373 2066 6f72 2073 746f  .z.Class for sto
-00005130: 7269 6e67 2074 6865 2072 6573 756c 7473  ring the results
-00005140: 206f 6620 6120 7261 6e20 7072 6f6a 6563   of a ran projec
-00005150: 742e 204d 6574 686f 6473 2061 7265 206d  t. Methods are m
-00005160: 6f73 746c 7920 7365 7474 6572 7320 616e  ostly setters an
-00005170: 6420 6765 7474 6572 7320 696e 2063 6861  d getters in cha
-00005180: 7267 6520 6f66 2074 6964 7969 6e67 2075  rge of tidying u
-00005190: 7020 7468 6520 6765 6e65 7261 7465 6420  p the generated 
-000051a0: 7461 626c 6573 2e4e 722c 0000 0029 1572  tables.Nr,...).r
-000051b0: 1800 0000 723e 0000 0072 3400 0000 725f  ....r>...r4...r_
-000051c0: 0000 0072 3500 0000 721e 0000 0072 ad00  ...r5...r....r..
-000051d0: 0000 72f0 0000 0072 6700 0000 7219 0100  ..r....rg...r...
-000051e0: 0072 5d00 0000 721a 0100 0072 5c00 0000  .r]...r....r\...
-000051f0: 721b 0100 0072 6100 0000 7233 0000 0072  r....ra...r3...r
-00005200: 6200 0000 7264 0000 0072 6300 0000 7218  b...rd...rc...r.
-00005210: 0100 0072 3800 0000 6316 0000 0000 0000  ...r8...c.......
-00005220: 0000 0000 0016 0000 0002 0000 0043 0000  .............C..
-00005230: 0073 8200 0000 7c01 7c00 5f00 7c02 7c00  .s....|.|._.|.|.
-00005240: 5f01 7c10 7c00 5f02 7c03 7c00 5f03 7c0a  _.|.|._.|.|._.|.
-00005250: 7c00 5f04 7c04 7c00 5f05 7c05 7c00 5f06  |._.|.|._.|.|._.
-00005260: 7c14 7c00 5f07 7c15 7c00 5f08 7c09 7c00  |.|._.|.|._.|.|.
-00005270: 5f09 7c06 7c00 5f0a 7c07 7c00 5f0b 7c08  _.|.|._.|.|._.|.
-00005280: 7c00 5f0c 7c0b 7c00 5f0d 7c0c 7c00 5f0e  |._.|.|._.|.|._.
-00005290: 7c0d 7c00 5f0f 7c0e 7c00 5f10 7c0f 7c00  |.|._.|.|._.|.|.
-000052a0: 5f11 7c11 7c00 5f12 7c12 7c00 5f13 7c13  _.|.|._.|.|._.|.
-000052b0: 7c00 5f14 6401 5300 2902 6151 0900 0043  |._.d.S.).aQ...C
-000052c0: 6c61 7373 2066 6f72 2073 746f 7269 6e67  lass for storing
-000052d0: 2074 6865 2072 6573 756c 7473 206f 6620   the results of 
-000052e0: 6120 7261 6e20 7072 6f6a 6563 742e 204d  a ran project. M
-000052f0: 6574 686f 6473 2061 7265 206d 6f73 746c  ethods are mostl
-00005300: 7920 7365 7474 6572 7320 616e 6420 6765  y setters and ge
-00005310: 7474 6572 7320 696e 2063 6861 7267 6520  tters in charge 
-00005320: 6f66 2074 6964 7969 6e67 2075 7020 7468  of tidying up th
-00005330: 6520 6765 6e65 7261 7465 6420 7461 626c  e generated tabl
-00005340: 6573 2e0a 0a20 2020 2020 2020 2041 7267  es...        Arg
-00005350: 733a 0a20 2020 2020 2020 2020 2020 2070  s:.            p
-00005360: 726f 6a65 6374 5f6e 616d 6520 2873 7472  roject_name (str
-00005370: 293a 206e 616d 6520 6f66 2074 6865 2063  ): name of the c
-00005380: 7572 7265 6e74 2070 726f 6a65 6374 2e0a  urrent project..
-00005390: 2020 2020 2020 2020 2020 2020 7072 6f6a              proj
-000053a0: 6563 745f 7061 7468 2028 7374 7229 3a20  ect_path (str): 
-000053b0: 7061 7468 2074 6f20 7468 6520 666f 6c64  path to the fold
-000053c0: 6572 2063 6f6e 7461 696e 696e 6720 7468  er containing th
-000053d0: 6520 444c 4320 6f75 7470 7574 2064 6174  e DLC output dat
-000053e0: 612e 0a20 2020 2020 2020 2020 2020 2061  a..            a
-000053f0: 7265 6e61 2028 7374 7229 3a20 5479 7065  rena (str): Type
-00005400: 206f 6620 6172 656e 6120 7573 6564 2066   of arena used f
-00005410: 6f72 2074 6865 2065 7870 6572 696d 656e  or the experimen
-00005420: 742e 2053 6565 2064 6565 706f 662e 6461  t. See deepof.da
-00005430: 7461 2e50 726f 6a65 6374 2066 6f72 206d  ta.Project for m
-00005440: 6f72 6520 696e 666f 726d 6174 696f 6e2e  ore information.
-00005450: 0a20 2020 2020 2020 2020 2020 2061 7265  .            are
-00005460: 6e61 5f64 696d 7320 286e 702e 6172 7261  na_dims (np.arra
-00005470: 7929 3a20 4469 6d65 6e73 696f 6e73 206f  y): Dimensions o
-00005480: 6620 7468 6520 6172 656e 612e 2053 6565  f the arena. See
-00005490: 2064 6565 706f 662e 6461 7461 2e50 726f   deepof.data.Pro
-000054a0: 6a65 6374 2066 6f72 206d 6f72 6520 696e  ject for more in
-000054b0: 666f 726d 6174 696f 6e2e 0a20 2020 2020  formation..     
-000054c0: 2020 2020 2020 2062 6f64 7970 6172 745f         bodypart_
-000054d0: 6772 6170 6820 286e 782e 4772 6170 6829  graph (nx.Graph)
-000054e0: 3a20 4772 6170 6820 636f 6e74 6169 6e69  : Graph containi
-000054f0: 6e67 2074 6865 2062 6f64 7920 7061 7274  ng the body part
-00005500: 2063 6f6e 6e65 6374 6976 6974 792e 2053   connectivity. S
-00005510: 6565 2064 6565 706f 662e 6461 7461 2e50  ee deepof.data.P
-00005520: 726f 6a65 6374 2066 6f72 206d 6f72 6520  roject for more 
-00005530: 696e 666f 726d 6174 696f 6e2e 0a20 2020  information..   
-00005540: 2020 2020 2020 2020 2070 6174 6820 2873           path (s
-00005550: 7472 293a 2050 6174 6820 746f 2074 6865  tr): Path to the
-00005560: 2066 6f6c 6465 7220 636f 6e74 6169 6e69   folder containi
-00005570: 6e67 2074 6865 2072 6573 756c 7473 206f  ng the results o
-00005580: 6620 7468 6520 6578 7065 7269 6d65 6e74  f the experiment
-00005590: 2e0a 2020 2020 2020 2020 2020 2020 7175  ..            qu
-000055a0: 616c 6974 7920 2864 6963 7429 3a20 4469  ality (dict): Di
-000055b0: 6374 696f 6e61 7279 2063 6f6e 7461 696e  ctionary contain
-000055c0: 696e 6720 7468 6520 7175 616c 6974 7920  ing the quality 
-000055d0: 6f66 2074 6865 2065 7870 6572 696d 656e  of the experimen
-000055e0: 742e 2053 6565 2064 6565 706f 662e 6461  t. See deepof.da
-000055f0: 7461 2e50 726f 6a65 6374 2066 6f72 206d  ta.Project for m
-00005600: 6f72 6520 696e 666f 726d 6174 696f 6e2e  ore information.
-00005610: 0a20 2020 2020 2020 2020 2020 2073 6361  .            sca
-00005620: 6c65 7320 286e 702e 6e64 6172 7261 7929  les (np.ndarray)
-00005630: 3a20 5363 616c 6573 2075 7365 6420 666f  : Scales used fo
-00005640: 7220 7468 6520 6578 7065 7269 6d65 6e74  r the experiment
-00005650: 2e20 5365 6520 6465 6570 6f66 2e64 6174  . See deepof.dat
-00005660: 612e 5072 6f6a 6563 7420 666f 7220 6d6f  a.Project for mo
-00005670: 7265 2069 6e66 6f72 6d61 7469 6f6e 2e0a  re information..
-00005680: 2020 2020 2020 2020 2020 2020 6672 616d              fram
-00005690: 655f 7261 7465 2028 696e 7429 3a20 6672  e_rate (int): fr
-000056a0: 616d 6520 7261 7465 206f 6620 7468 6520  ame rate of the 
-000056b0: 7072 6f63 6573 7365 6420 7669 6465 6f73  processed videos
-000056c0: 2e0a 2020 2020 2020 2020 2020 2020 6172  ..            ar
-000056d0: 656e 615f 7061 7261 6d73 2028 4c69 7374  ena_params (List
-000056e0: 293a 204c 6973 7420 636f 6e74 6169 6e69  ): List containi
-000056f0: 6e67 2074 6865 2070 6172 616d 6574 6572  ng the parameter
-00005700: 7320 6f66 2074 6865 2061 7265 6e61 2e20  s of the arena. 
-00005710: 5365 6520 6465 6570 6f66 2e64 6174 612e  See deepof.data.
-00005720: 5072 6f6a 6563 7420 666f 7220 6d6f 7265  Project for more
-00005730: 2069 6e66 6f72 6d61 7469 6f6e 2e0a 2020   information..  
-00005740: 2020 2020 2020 2020 2020 7461 626c 6573            tables
-00005750: 2028 6469 6374 293a 2044 6963 7469 6f6e   (dict): Diction
-00005760: 6172 7920 636f 6e74 6169 6e69 6e67 2074  ary containing t
-00005770: 6865 2074 6162 6c65 7320 6f66 2074 6865  he tables of the
-00005780: 2065 7870 6572 696d 656e 742e 2053 6565   experiment. See
-00005790: 2064 6565 706f 662e 6461 7461 2e50 726f   deepof.data.Pro
-000057a0: 6a65 6374 2066 6f72 206d 6f72 6520 696e  ject for more in
-000057b0: 666f 726d 6174 696f 6e2e 0a20 2020 2020  formation..     
-000057c0: 2020 2020 2020 2074 7261 696e 6564 5f6d         trained_m
-000057d0: 6f64 656c 5f70 6174 6820 2873 7472 293a  odel_path (str):
-000057e0: 2050 6174 6820 746f 2074 6865 2074 7261   Path to the tra
-000057f0: 696e 6564 206d 6f64 656c 7320 7573 6564  ined models used
-00005800: 2066 6f72 2074 6865 2073 7570 6572 7669   for the supervi
-00005810: 7365 6420 7069 7065 6c69 6e65 2e20 466f  sed pipeline. Fo
-00005820: 7220 696e 7465 726e 616c 2075 7365 206f  r internal use o
-00005830: 6e6c 792e 0a20 2020 2020 2020 2020 2020  nly..           
-00005840: 2076 6964 656f 7320 284c 6973 7429 3a20   videos (List): 
-00005850: 4c69 7374 2063 6f6e 7461 696e 696e 6720  List containing 
-00005860: 7468 6520 7669 6465 6f73 2075 7365 6420  the videos used 
-00005870: 666f 7220 7468 6520 6578 7065 7269 6d65  for the experime
-00005880: 6e74 2e20 5365 6520 6465 6570 6f66 2e64  nt. See deepof.d
-00005890: 6174 612e 5072 6f6a 6563 7420 666f 7220  ata.Project for 
-000058a0: 6d6f 7265 2069 6e66 6f72 6d61 7469 6f6e  more information
-000058b0: 2e0a 2020 2020 2020 2020 2020 2020 7669  ..            vi
-000058c0: 6465 6f5f 7265 736f 6c75 7469 6f6e 2028  deo_resolution (
-000058d0: 4c69 7374 293a 204c 6973 7420 636f 6e74  List): List cont
-000058e0: 6169 6e69 6e67 2074 6865 2061 7574 6f6d  aining the autom
-000058f0: 6174 6963 616c 6c79 2064 6574 6563 7465  atically detecte
-00005900: 6420 7265 736f 6c75 7469 6f6e 206f 6620  d resolution of 
-00005910: 7468 6520 7669 6465 6f73 2075 7365 6420  the videos used 
-00005920: 666f 7220 7468 6520 6578 7065 7269 6d65  for the experime
-00005930: 6e74 2e0a 2020 2020 2020 2020 2020 2020  nt..            
-00005940: 616e 676c 6573 2028 6469 6374 293a 2044  angles (dict): D
-00005950: 6963 7469 6f6e 6172 7920 636f 6e74 6169  ictionary contai
-00005960: 6e69 6e67 2074 6865 2061 6e67 6c65 7320  ning the angles 
-00005970: 6f66 2074 6865 2065 7870 6572 696d 656e  of the experimen
-00005980: 742e 2053 6565 2064 6565 706f 662e 6461  t. See deepof.da
-00005990: 7461 2e50 726f 6a65 6374 2066 6f72 206d  ta.Project for m
-000059a0: 6f72 6520 696e 666f 726d 6174 696f 6e2e  ore information.
-000059b0: 0a20 2020 2020 2020 2020 2020 2061 6e69  .            ani
-000059c0: 6d61 6c5f 6964 7320 284c 6973 7429 3a20  mal_ids (List): 
-000059d0: 4c69 7374 2063 6f6e 7461 696e 696e 6720  List containing 
-000059e0: 7468 6520 616e 696d 616c 2049 4473 206f  the animal IDs o
-000059f0: 6620 7468 6520 6578 7065 7269 6d65 6e74  f the experiment
-00005a00: 2e20 5365 6520 6465 6570 6f66 2e64 6174  . See deepof.dat
-00005a10: 612e 5072 6f6a 6563 7420 666f 7220 6d6f  a.Project for mo
-00005a20: 7265 2069 6e66 6f72 6d61 7469 6f6e 2e0a  re information..
-00005a30: 2020 2020 2020 2020 2020 2020 6172 6561              area
-00005a40: 7320 2864 6963 7429 3a20 6469 6374 696f  s (dict): dictio
-00005a50: 6e61 7279 2077 6974 6820 6172 6561 7320  nary with areas 
-00005a60: 746f 2063 6f6d 7075 7465 2e20 4279 2064  to compute. By d
-00005a70: 6566 6175 6c74 2c20 6974 2069 6e63 6c75  efault, it inclu
-00005a80: 6465 7320 6865 6164 2c20 746f 7273 6f2c  des head, torso,
-00005a90: 2061 6e64 2062 6163 6b2e 0a20 2020 2020   and back..     
-00005aa0: 2020 2020 2020 2064 6973 7461 6e63 6573         distances
-00005ab0: 2028 6469 6374 293a 2044 6963 7469 6f6e   (dict): Diction
-00005ac0: 6172 7920 636f 6e74 6169 6e69 6e67 2074  ary containing t
-00005ad0: 6865 2064 6973 7461 6e63 6573 206f 6620  he distances of 
-00005ae0: 7468 6520 6578 7065 7269 6d65 6e74 2e20  the experiment. 
-00005af0: 5365 6520 6465 6570 6f66 2e64 6174 612e  See deepof.data.
-00005b00: 5072 6f6a 6563 7420 666f 7220 6d6f 7265  Project for more
-00005b10: 2069 6e66 6f72 6d61 7469 6f6e 2e0a 2020   information..  
-00005b20: 2020 2020 2020 2020 2020 6578 636c 7564            exclud
-00005b30: 6564 5f62 6f64 7970 6172 7473 2028 6c69  ed_bodyparts (li
-00005b40: 7374 293a 206c 6973 7420 6f66 2062 6f64  st): list of bod
-00005b50: 7970 6172 7473 2074 6f20 6578 636c 7564  yparts to exclud
-00005b60: 6520 6672 6f6d 2061 6e61 6c79 7369 732e  e from analysis.
-00005b70: 0a20 2020 2020 2020 2020 2020 2065 7870  .            exp
-00005b80: 5f63 6f6e 6469 7469 6f6e 7320 2864 6963  _conditions (dic
-00005b90: 7429 3a20 4469 6374 696f 6e61 7279 2063  t): Dictionary c
-00005ba0: 6f6e 7461 696e 696e 6720 7468 6520 6578  ontaining the ex
-00005bb0: 7065 7269 6d65 6e74 616c 2063 6f6e 6469  perimental condi
-00005bc0: 7469 6f6e 7320 6f66 2074 6865 2065 7870  tions of the exp
-00005bd0: 6572 696d 656e 742e 2053 6565 2064 6565  eriment. See dee
-00005be0: 706f 662e 6461 7461 2e50 726f 6a65 6374  pof.data.Project
-00005bf0: 2066 6f72 206d 6f72 6520 696e 666f 726d   for more inform
-00005c00: 6174 696f 6e2e 0a0a 2020 2020 2020 2020  ation...        
-00005c10: 4e29 1572 2300 0000 da0d 5f70 726f 6a65  N).r#....._proje
-00005c20: 6374 5f6e 616d 65da 0b5f 616e 696d 616c  ct_name.._animal
-00005c30: 5f69 6473 da06 5f61 7265 6e61 da0d 5f61  _ids.._arena.._a
-00005c40: 7265 6e61 5f70 6172 616d 73da 0b5f 6172  rena_params.._ar
-00005c50: 656e 615f 6469 6d73 da0f 5f62 6f64 7970  ena_dims.._bodyp
-00005c60: 6172 745f 6772 6170 68da 095f 6578 636c  art_graph.._excl
-00005c70: 7564 6564 da0f 5f65 7870 5f63 6f6e 6469  uded.._exp_condi
-00005c80: 7469 6f6e 73da 0b5f 6672 616d 655f 7261  tions.._frame_ra
-00005c90: 7465 da05 5f70 6174 68da 085f 7175 616c  te.._path.._qual
-00005ca0: 6974 79da 075f 7363 616c 6573 da07 5f74  ity.._scales.._t
-00005cb0: 6162 6c65 73da 135f 7472 6169 6e65 645f  ables.._trained_
-00005cc0: 6d6f 6465 6c5f 7061 7468 da07 5f76 6964  model_path.._vid
-00005cd0: 656f 73da 115f 7669 6465 6f5f 7265 736f  eos.._video_reso
-00005ce0: 6c75 7469 6f6e 727e 0000 00da 065f 6172  lutionr~....._ar
-00005cf0: 6561 7372 7a00 0000 da0d 5f63 6f6e 6e65  easrz....._conne
-00005d00: 6374 6976 6974 7929 1672 5600 0000 7218  ctivity).rV...r.
-00005d10: 0000 0072 3e00 0000 7234 0000 0072 5f00  ...r>...r4...r_.
-00005d20: 0000 7235 0000 0072 1e00 0000 72ad 0000  ..r5...r....r...
-00005d30: 0072 f000 0000 7267 0000 0072 1901 0000  .r....rg...r....
-00005d40: 725d 0000 0072 1a01 0000 725c 0000 0072  r]...r....r\...r
-00005d50: 1b01 0000 7261 0000 0072 3300 0000 7262  ....ra...r3...rb
-00005d60: 0000 0072 6400 0000 7263 0000 0072 1801  ...rd...rc...r..
-00005d70: 0000 7238 0000 0072 2600 0000 7226 0000  ..r8...r&...r&..
-00005d80: 0072 2700 0000 7269 0000 00dd 0200 0073  .r'...ri.......s
-00005d90: 2a00 0000 0031 0601 0601 0601 0601 0601  *....1..........
-00005da0: 0601 0601 0601 0601 0601 0601 0601 0601  ................
-00005db0: 0601 0601 0601 0601 0601 0601 0601 7a14  ..............z.
-00005dc0: 436f 6f72 6469 6e61 7465 732e 5f5f 696e  Coordinates.__in
-00005dd0: 6974 5f5f 6301 0000 0000 0000 0000 0000  it__c...........
-00005de0: 0001 0000 0004 0000 0043 0000 0073 1000  .........C...s..
-00005df0: 0000 6401 a000 7401 7c00 6a02 8301 a101  ..d...t.|.j.....
-00005e00: 5300 726a 0000 00a9 0372 6c00 0000 725e  S.rj.....rl...r^
-00005e10: 0000 0072 3d01 0000 7255 0000 0072 2600  ...r=...rU...r&.
-00005e20: 0000 7226 0000 0072 2700 0000 726d 0000  ..r&...r'...rm..
-00005e30: 0024 0300 0073 0200 0000 0002 7a13 436f  .$...s......z.Co
-00005e40: 6f72 6469 6e61 7465 732e 5f5f 7374 725f  ordinates.__str_
-00005e50: 5f63 0100 0000 0000 0000 0000 0000 0100  _c..............
-00005e60: 0000 0400 0000 4300 0000 7310 0000 0064  ......C...s....d
-00005e70: 01a0 0074 017c 006a 0283 01a1 0153 0072  ...t.|.j.....S.r
-00005e80: 6a00 0000 7241 0100 0072 5500 0000 7226  j...rA...rU...r&
-00005e90: 0000 0072 2600 0000 7227 0000 0072 6e00  ...r&...r'...rn.
-00005ea0: 0000 2803 0000 7302 0000 0000 027a 1443  ..(...s......z.C
-00005eb0: 6f6f 7264 696e 6174 6573 2e5f 5f72 6570  oordinates.__rep
-00005ec0: 725f 5f46 7201 0000 0054 2909 da06 6365  r__Fr....T)...ce
-00005ed0: 6e74 6572 da05 706f 6c61 72da 0573 7065  nter..polar..spe
-00005ee0: 6564 da05 616c 6967 6eda 0d61 6c69 676e  ed..align..align
-00005ef0: 5f69 6e70 6c61 6365 da0b 7365 6c65 6374  _inplace..select
-00005f00: 6564 5f69 64da 1070 726f 7061 6761 7465  ed_id..propagate
-00005f10: 5f6c 6162 656c 73da 1570 726f 7061 6761  _labels..propaga
-00005f20: 7465 5f61 6e6e 6f74 6174 696f 6e73 7219  te_annotationsr.
-00005f30: 0000 0063 0900 0000 0000 0000 0000 0000  ...c............
-00005f40: 1b00 0000 0d00 0000 0300 0000 73fe 0400  ............s...
-00005f50: 0074 006a 01a0 027c 006a 03a1 017d 0964  .t.j...|.j...}.d
-00005f60: 015c 027d 0a7d 0b7c 006a 047d 0c7c 0272  .\.}.}.|.j.}.|.r
-00005f70: 5a64 025c 027d 0a7d 0b74 006a 01a0 057c  Zd.\.}.}.t.j...|
-00005f80: 0ca1 01a0 06a1 007d 0c7c 09a0 07a1 0044  .......}.|.....D
-00005f90: 005d 185c 027d 0d7d 0e74 006a 01a0 087c  .].\.}.}.t.j...|
-00005fa0: 0ea1 017c 097c 0d3c 0071 4088 0264 036b  ...|.|.<.q@..d.k
-00005fb0: 0290 0172 0274 097c 09a0 07a1 0083 0144  ...r.t.|.......D
-00005fc0: 005d 8c5c 027d 0f5c 027d 0d7d 107c 106a  .].\.}.\.}.}.|.j
-00005fd0: 0a64 0464 0485 0274 0b64 0583 017c 0a67  .d.d...t.d...|.g
-00005fe0: 0166 0266 0219 007c 0c7c 0f19 0064 0619  .f.f...|.|...d..
-00005ff0: 0018 007c 106a 0a64 0464 0485 0274 0b64  ...|.j.d.d...t.d
-00006000: 0583 017c 0a67 0166 0266 023c 007c 106a  ...|.g.f.f.<.|.j
-00006010: 0a64 0464 0485 0274 0b64 0583 017c 0b67  .d.d...t.d...|.g
-00006020: 0166 0266 0219 007c 0c7c 0f19 0064 0719  .f.f...|.|...d..
-00006030: 0018 007c 106a 0a64 0464 0485 0274 0b64  ...|.j.d.d...t.d
-00006040: 0583 017c 0b67 0166 0266 023c 0071 7090  ...|.g.f.f.<.qp.
-00006050: 016e 2674 0c88 0274 0d83 0290 0272 2888  .n&t...t.....r(.
-00006060: 0264 036b 0390 0272 2874 097c 09a0 07a1  .d.k...r(t.|....
-00006070: 0083 0144 0090 015d 005c 027d 0f5c 027d  ...D...].\.}.\.}
-00006080: 0d7d 107c 006a 0e7d 117c 0664 0475 0190  .}.|.j.}.|.d.u..
-00006090: 0172 487c 0667 017d 117c 1144 005d d689  .rH|.g.}.|.D.]..
-000060a0: 007c 10a0 0f7c 106a 0a64 0464 0485 0287  .|...|.j.d.d....
-000060b0: 0066 0164 0864 0984 087c 106a 1044 0083  .f.d.d...|.j.D..
-000060c0: 0166 0219 006a 0a64 0464 0485 0274 0b64  .f...j.d.d...t.d
-000060d0: 0583 017c 0a67 0166 0266 0219 006a 117c  ...|.g.f.f...j.|
-000060e0: 1088 0088 0064 0a6b 0390 0172 a064 0b6e  .....d.k...r.d.n
-000060f0: 0264 0a17 0088 0217 0019 007c 0a19 0064  .d.........|...d
-00006100: 0664 0c8d 02a1 0101 007c 10a0 0f7c 106a  .d.......|...|.j
-00006110: 0a64 0464 0485 0287 0066 0164 0d64 0984  .d.d.....f.d.d..
-00006120: 087c 106a 1044 0083 0166 0219 006a 0a64  .|.j.D...f...j.d
-00006130: 0464 0485 0274 0b64 0583 017c 0b67 0166  .d...t.d...|.g.f
-00006140: 0266 0219 006a 117c 1088 0088 0064 0a6b  .f...j.|.....d.k
-00006150: 0390 0272 0864 0b6e 0264 0a17 0088 0217  ...r.d.n.d......
-00006160: 0019 007c 0b19 0064 0664 0c8d 02a1 0101  ...|...d.d......
-00006170: 0090 0171 4c90 0171 2488 0190 0372 ac74  ...qL..q$....r.t
-00006180: 1287 0266 0164 0e64 0f84 0874 137c 09a0  ...f.d.d...t.|..
-00006190: 14a1 0083 0164 0619 006a 106a 1564 0619  .....d...j.j.d..
-000061a0: 0044 0083 0183 0190 0273 624a 0064 1083  .D.......sbJ.d..
-000061b0: 0182 0174 1287 0166 0164 1164 0f84 0874  ...t...f.d.d...t
-000061c0: 137c 09a0 14a1 0083 0164 0619 006a 106a  .|.......d...j.j
-000061d0: 1564 0619 0044 0083 0183 0190 0273 964a  .d...D.......s.J
-000061e0: 0064 1283 0182 017c 09a0 07a1 0044 0090  .d.....|.....D..
-000061f0: 015d 0a5c 027d 0d7d 0e7c 0e6a 167d 1267  .].\.}.}.|.j.}.g
-00006200: 007d 1364 047d 147c 1144 005d d089 0087  .}.d.}.|.D.]....
-00006210: 0087 0166 0264 1364 0984 087c 0e6a 1044  ...f.d.d...|.j.D
-00006220: 0083 017d 1588 0088 0064 0a6b 0390 0272  ...}.....d.k...r
-00006230: e464 0b6e 0264 0a17 0088 0117 007c 0290  .d.n.d.......|..
-00006240: 0272 f664 146e 0264 0566 0288 0088 0064  .r.d.n.d.f.....d
-00006250: 0a6b 0390 0372 0a64 0b6e 0264 0a17 0088  .k...r.d.n.d....
-00006260: 0117 007c 0290 0372 1c64 156e 0264 1666  ...|...r.d.n.d.f
-00006270: 0267 027c 1517 007d 157c 0e7c 1519 007d  .g.|...}.|.|...}
-00006280: 167c 137c 1537 007d 137c 0590 0272 ba7c  .|.|.7.}.|...r.|
-00006290: 0290 0273 ba74 006a 016a 1774 18a0 197c  ...s.t.j.j.t...|
-000062a0: 16a1 0164 1764 188d 027d 1664 197c 1674  ...d.d...}.d.|.t
-000062b0: 18a0 1a7c 16a1 0164 1a6b 003c 0074 1ba0  ...|...d.k.<.t..
-000062c0: 1c7c 16a1 017d 1674 1b6a 1d7c 147c 1667  .|...}.t.j.|.|.g
-000062d0: 0264 0764 0c8d 027d 1490 0271 ba7c 127c  .d.d...}...q.|.|
-000062e0: 145f 1674 1b6a 1ea0 1f7c 13a1 017c 145f  ._.t.j...|...|._
-000062f0: 107c 147c 097c 0d3c 0090 0271 9e7c 0390  .|.|.|.<...q.|..
-00006300: 0372 e07c 09a0 07a1 0044 005d 245c 027d  .r.|.....D.]$\.}
-00006310: 0d7d 0e74 006a 016a 207c 0e7c 0388 0264  .}.t.j.j |.|...d
-00006320: 1b8d 037d 177c 177c 097c 0d3c 0090 0371  ...}.|.|.|.<...q
-00006330: ba7c 0664 0475 0190 0472 207c 09a0 07a1  .|.d.u...r |....
-00006340: 0044 005d 2c5c 027d 0d7d 187c 186a 0a64  .D.],\.}.}.|.j.d
-00006350: 0464 0485 0274 006a 01a0 217c 186a 107c  .d...t.j..!|.j.|
-00006360: 06a1 0266 0219 007c 097c 0d3c 0090 0371  ...f...|.|.<...q
-00006370: f274 006a 01a0 227c 007c 097c 00a0 23a1  .t.j.."|.|.|..#.
-00006380: 00a1 037d 097c 0890 0472 9074 137c 08a0  ...}.|...r.t.|..
-00006390: 14a1 0083 0164 0619 006a 107d 197c 09a0  .....d...j.}.|..
-000063a0: 07a1 0044 005d 3a5c 027d 0d7d 0e7c 1944  ...D.]:\.}.}.|.D
-000063b0: 005d 2a7d 1a7c 087c 0d19 006a 0a64 0464  .]*}.|.|...j.d.d
-000063c0: 0485 027c 1a66 0219 007c 0e6a 0a64 0464  ...|.f...|.j.d.d
-000063d0: 0485 027c 1a66 023c 0090 0471 6090 0471  ...|.f.<...q`..q
-000063e0: 547c 0790 0472 d67c 09a0 07a1 0044 005d  T|...r.|.....D.]
-000063f0: 365c 027d 0d7d 0e74 18a0 247c 006a 257c  6\.}.}.t..$|.j%|
-00006400: 0d19 007c 0719 006a 147c 0e6a 2664 0619  ...|...j.|.j&d..
-00006410: 00a1 027c 0e6a 0a64 0464 0485 0264 1c66  ...|.j.d.d...d.f
-00006420: 023c 0090 0471 9e74 277c 0964 1d7c 006a  .<...q.t'|.d.|.j
-00006430: 0e7c 006a 287c 006a 0488 027c 006a 297c  .|.j(|.j...|.j)|
-00006440: 027c 006a 257c 077c 0864 1e8d 0b53 0029  .|.j%|.|.d...S.)
-00006450: 1f61 8405 0000 5265 7475 726e 2061 2074  .a....Return a t
-00006460: 6162 6c65 5f64 6963 7420 6f62 6a65 6374  able_dict object
-00006470: 2077 6974 6820 7468 6520 636f 6f72 6469   with the coordi
-00006480: 6e61 7465 7320 6f66 2065 6163 6820 616e  nates of each an
-00006490: 696d 616c 2061 7320 7661 6c75 6573 2e0a  imal as values..
-000064a0: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
-000064b0: 2020 2020 2020 2020 2020 2063 656e 7465             cente
-000064c0: 7220 2873 7472 293a 204e 616d 6520 6f66  r (str): Name of
-000064d0: 2074 6865 2062 6f64 7920 7061 7274 2074   the body part t
-000064e0: 6f20 7768 6963 6820 7468 6520 706f 7369  o which the posi
-000064f0: 7469 6f6e 7320 7769 6c6c 2062 6520 6365  tions will be ce
-00006500: 6e74 6572 6564 2e20 4966 2066 616c 7365  ntered. If false
-00006510: 2c20 7468 6520 7261 7720 6461 7461 2069  , the raw data i
-00006520: 7320 7265 7475 726e 6564 3b20 6966 2027  s returned; if '
-00006530: 6172 656e 6127 2028 6465 6661 756c 7429  arena' (default)
-00006540: 2c20 636f 6f72 6469 6e61 7465 7320 6172  , coordinates ar
-00006550: 6520 6365 6e74 6572 6564 2069 6e20 7468  e centered in th
-00006560: 6520 7069 7463 680a 2020 2020 2020 2020  e pitch.        
-00006570: 2020 2020 706f 6c61 7220 2862 6f6f 6c29      polar (bool)
-00006580: 2053 7461 7465 7320 7768 6574 6865 7220   States whether 
-00006590: 7468 6520 636f 6f72 6469 6e61 7465 7320  the coordinates 
-000065a0: 7368 6f75 6c64 2062 6520 636f 6e76 6572  should be conver
-000065b0: 7465 6420 746f 2070 6f6c 6172 2076 616c  ted to polar val
-000065c0: 7565 732e 0a20 2020 2020 2020 2020 2020  ues..           
-000065d0: 2073 7065 6564 2028 696e 7429 3a20 5374   speed (int): St
-000065e0: 6174 6573 2074 6865 2064 6572 6976 6174  ates the derivat
-000065f0: 6976 6520 6f66 2074 6865 2070 6f73 6974  ive of the posit
-00006600: 696f 6e73 2074 6f20 7265 706f 7274 2e20  ions to report. 
-00006610: 5370 6565 6420 6973 2072 6574 7572 6e65  Speed is returne
-00006620: 6420 6966 2031 2c20 6163 6365 6c65 7261  d if 1, accelera
-00006630: 7469 6f6e 2069 6620 322c 206a 6572 6b20  tion if 2, jerk 
-00006640: 6966 2033 2c20 6574 632e 0a20 2020 2020  if 3, etc..     
-00006650: 2020 2020 2020 2061 6c69 676e 2028 7374         align (st
-00006660: 7229 3a20 5365 6c65 6374 7320 7468 6520  r): Selects the 
-00006670: 626f 6479 2070 6172 7420 746f 2077 6869  body part to whi
-00006680: 6368 206c 6174 6572 2070 726f 6365 7373  ch later process
-00006690: 6573 2077 696c 6c20 616c 6967 6e20 7468  es will align th
-000066a0: 6520 6672 616d 6573 2077 6974 6820 2873  e frames with (s
-000066b0: 6565 2070 7265 7072 6f63 6573 7320 696e  ee preprocess in
-000066c0: 2074 6162 6c65 5f64 6963 7420 646f 6375   table_dict docu
-000066d0: 6d65 6e74 6174 696f 6e29 2e0a 2020 2020  mentation)..    
-000066e0: 2020 2020 2020 2020 616c 6967 6e5f 696e          align_in
-000066f0: 706c 6163 6520 2862 6f6f 6c29 3a20 4f6e  place (bool): On
-00006700: 6c79 2076 616c 6964 2069 6620 616c 6967  ly valid if alig
-00006710: 6e20 6973 2073 6574 2e20 416c 6967 6e73  n is set. Aligns
-00006720: 2074 6865 2076 6563 746f 7220 7468 6174   the vector that
-00006730: 2067 6f65 7320 6672 6f6d 2074 6865 206f   goes from the o
-00006740: 7269 6769 6e20 746f 2074 6865 2073 656c  rigin to the sel
-00006750: 6563 7465 6420 626f 6479 2070 6172 7420  ected body part 
-00006760: 7769 7468 2074 6865 2079 2d61 7869 732c  with the y-axis,
-00006770: 2066 6f72 2061 6c6c 2074 696d 6570 6f69   for all timepoi
-00006780: 6e74 7320 2864 6566 6175 6c74 292e 0a20  nts (default).. 
-00006790: 2020 2020 2020 2020 2020 2073 656c 6563             selec
-000067a0: 7465 645f 6964 2028 7374 7229 3a20 5365  ted_id (str): Se
-000067b0: 6c65 6374 7320 6120 7369 6e67 6c65 2061  lects a single a
-000067c0: 6e69 6d61 6c20 6f6e 206d 756c 7469 2061  nimal on multi a
-000067d0: 6e69 6d61 6c20 7365 7474 696e 6773 2e20  nimal settings. 
-000067e0: 4465 6661 756c 7473 2074 6f20 4e6f 6e65  Defaults to None
-000067f0: 2028 616c 6c20 616e 696d 616c 7320 6172   (all animals ar
-00006800: 6520 7072 6f63 6573 7365 6429 2e0a 2020  e processed)..  
-00006810: 2020 2020 2020 2020 2020 7072 6f70 6167            propag
-00006820: 6174 655f 6c61 6265 6c73 2028 626f 6f6c  ate_labels (bool
-00006830: 293a 2049 6620 5472 7565 2c20 6164 6473  ): If True, adds
-00006840: 2061 6e20 6578 7472 6120 6665 6174 7572   an extra featur
-00006850: 6520 666f 7220 6561 6368 2076 6964 656f  e for each video
-00006860: 2063 6f6e 7461 696e 696e 6720 6974 7320   containing its 
-00006870: 7068 656e 6f74 7970 6963 206c 6162 656c  phenotypic label
-00006880: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
-00006890: 7061 6761 7465 5f61 6e6e 6f74 6174 696f  pagate_annotatio
-000068a0: 6e73 2028 6469 6374 293a 2049 6620 6120  ns (dict): If a 
-000068b0: 6469 6374 696f 6e61 7279 2069 7320 7072  dictionary is pr
-000068c0: 6f76 6964 6564 2c20 7375 7065 7276 6973  ovided, supervis
-000068d0: 6564 2061 6e6e 6f74 6174 696f 6e73 2061  ed annotations a
-000068e0: 7265 2070 726f 7061 6761 7465 6420 7468  re propagated th
-000068f0: 726f 7567 6820 7468 6520 7472 6169 6e69  rough the traini
-00006900: 6e67 2064 6174 6173 6574 2e20 5468 6973  ng dataset. This
-00006910: 2063 616e 2062 6520 7573 6564 2066 6f72   can be used for
-00006920: 2072 6567 756c 6172 6973 696e 6720 7468   regularising th
-00006930: 6520 6c61 7465 6e74 2073 7061 6365 2062  e latent space b
-00006940: 6173 6564 206f 6e20 616c 7265 6164 7920  ased on already 
-00006950: 6b6e 6f77 6e20 7472 6169 7473 2e0a 0a20  known traits... 
-00006960: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-00006970: 2020 2020 2020 2020 2020 2020 7461 626c              tabl
-00006980: 655f 6469 6374 3a20 4120 7461 626c 655f  e_dict: A table_
-00006990: 6469 6374 206f 626a 6563 7420 636f 6e74  dict object cont
-000069a0: 6169 6e69 6e67 2074 6865 2063 6f6f 7264  aining the coord
-000069b0: 696e 6174 6573 206f 6620 6561 6368 2061  inates of each a
-000069c0: 6e69 6d61 6c20 6173 2076 616c 7565 732e  nimal as values.
-000069d0: 0a0a 2020 2020 2020 2020 2902 72a5 0000  ..        ).r...
-000069e0: 0072 a900 0000 2902 da03 7268 6fda 0370  .r....)...rho..p
-000069f0: 6869 7234 0000 004e 72a5 0000 0072 0100  hir4...Nr....r..
-00006a00: 0000 7231 0000 0063 0100 0000 0000 0000  ..r1...c........
-00006a10: 0000 0000 0200 0000 0500 0000 1300 0000  ................
-00006a20: 731e 0000 0067 007c 005d 167d 017c 0164  s....g.|.].}.|.d
-00006a30: 0019 00a0 0088 00a1 0172 047c 0191 0271  .........r.|...q
-00006a40: 0453 0072 ed00 0000 7247 0000 0072 4900  .S.r....rG...rI.
-00006a50: 0000 7207 0100 0072 2600 0000 7227 0000  ..r....r&...r'..
-00006a60: 0072 4c00 0000 6903 0000 724d 0000 007a  .rL...i...rM...z
-00006a70: 2a43 6f6f 7264 696e 6174 6573 2e67 6574  *Coordinates.get
-00006a80: 5f63 6f6f 7264 732e 3c6c 6f63 616c 733e  _coords.<locals>
-00006a90: 2e3c 6c69 7374 636f 6d70 3e72 2c00 0000  .<listcomp>r,...
-00006aa0: 728c 0000 0072 ab00 0000 6301 0000 0000  r....r....c.....
-00006ab0: 0000 0000 0000 0002 0000 0005 0000 0013  ................
-00006ac0: 0000 0073 1e00 0000 6700 7c00 5d16 7d01  ...s....g.|.].}.
-00006ad0: 7c01 6400 1900 a000 8800 a101 7204 7c01  |.d.........r.|.
-00006ae0: 9102 7104 5300 72ed 0000 0072 4700 0000  ..q.S.r....rG...
-00006af0: 7249 0000 0072 0701 0000 7226 0000 0072  rI...r....r&...r
-00006b00: 2700 0000 724c 0000 0073 0300 0072 4d00  '...rL...s...rM.
-00006b10: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
-00006b20: 0000 0003 0000 0033 0000 0073 1600 0000  .......3...s....
-00006b30: 7c00 5d0e 7d01 8800 7c01 7600 5600 0100  |.].}...|.v.V...
-00006b40: 7102 6400 5300 7225 0100 0072 2600 0000  q.d.S.r%...r&...
-00006b50: a902 724a 0000 0072 9a00 0000 a901 7242  ..rJ...r......rB
-00006b60: 0100 0072 2600 0000 7227 0000 00da 093c  ...r&...r'.....<
-00006b70: 6765 6e65 7870 723e 7d03 0000 7302 0000  genexpr>}...s...
-00006b80: 0004 017a 2943 6f6f 7264 696e 6174 6573  ...z)Coordinates
-00006b90: 2e67 6574 5f63 6f6f 7264 732e 3c6c 6f63  .get_coords.<loc
-00006ba0: 616c 733e 2e3c 6765 6e65 7870 723e 7a3e  als>.<genexpr>z>
-00006bb0: 666f 7220 616c 6967 6e20 746f 2072 756e  for align to run
-00006bc0: 2c20 6365 6e74 6572 206d 7573 7420 6265  , center must be
-00006bd0: 2073 6574 2074 6f20 7468 6520 6e61 6d65   set to the name
-00006be0: 206f 6620 6120 626f 6479 7061 7274 6301   of a bodypartc.
-00006bf0: 0000 0000 0000 0000 0000 0002 0000 0003  ................
-00006c00: 0000 0033 0000 0073 1600 0000 7c00 5d0e  ...3...s....|.].
-00006c10: 7d01 8800 7c01 7600 5600 0100 7102 6400  }...|.v.V...q.d.
-00006c20: 5300 7225 0100 0072 2600 0000 724c 0100  S.r%...r&...rL..
-00006c30: 0029 0172 4501 0000 7226 0000 0072 2700  .).rE...r&...r'.
-00006c40: 0000 724e 0100 0080 0300 0073 0200 0000  ..rN.......s....
-00006c50: 0401 7a2b 616c 6967 6e20 6d75 7374 2062  ..z+align must b
-00006c60: 6520 7365 7420 746f 2074 6865 206e 616d  e set to the nam
-00006c70: 6520 6f66 2061 2062 6f64 7970 6172 7463  e of a bodypartc
-00006c80: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00006c90: 0500 0000 1300 0000 732c 0000 0067 007c  ........s,...g.|
-00006ca0: 005d 247d 017c 0164 0019 00a0 0088 01a1  .]$}.|.d........
-00006cb0: 0173 047c 0164 0019 00a0 0188 00a1 0172  .s.|.d.........r
-00006cc0: 047c 0191 0271 0453 0072 ed00 0000 7250  .|...q.S.r....rP
-00006cd0: 0000 0072 4900 0000 2902 7296 0000 0072  ...rI...).r....r
-00006ce0: 4501 0000 7226 0000 0072 2700 0000 724c  E...r&...r'...rL
-00006cf0: 0000 008c 0300 0073 0600 0000 0602 0201  .......s........
-00006d00: 1cfe 724b 0100 0072 4a01 0000 72a9 0000  ..rK...rJ...r...
-00006d10: 0072 5700 0000 2901 72ba 0000 0072 ac00  .rW...).r....r..
-00006d20: 0000 67f1 68e3 88b5 f8e4 3e29 02da 0564  ..g.h.....>)...d
-00006d30: 6572 6976 7242 0100 00da 0570 6865 6e6f  erivrB.....pheno
-00006d40: 72a6 0000 0029 0972 3300 0000 7234 0000  r....).r3...r4..
-00006d50: 0072 5f00 0000 7242 0100 0072 6300 0000  .r_...rB...rc...
-00006d60: 7243 0100 0072 3800 0000 7248 0100 0072  rC...r8...rH...r
-00006d70: 4901 0000 292a 7281 0000 0072 8200 0000  I...)*r....r....
-00006d80: da08 6465 6570 636f 7079 723b 0100 0072  ..deepcopyr;...r
-00006d90: 3a01 0000 da08 6270 3270 6f6c 6172 da08  :.....bp2polar..
-00006da0: 746f 5f6e 756d 7079 72cb 0000 00da 0974  to_numpyr......t
-00006db0: 6162 3270 6f6c 6172 72f5 0000 0072 c300  ab2polarr....r..
-00006dc0: 0000 da05 736c 6963 65da 0a69 7369 6e73  ....slice..isins
-00006dd0: 7461 6e63 6572 a200 0000 7230 0100 00da  tancer....r0....
-00006de0: 0675 7064 6174 6572 b700 0000 da08 7375  .updater......su
-00006df0: 6274 7261 6374 da03 616e 7972 b500 0000  btract..anyr....
-00006e00: 72c8 0000 0072 ee00 0000 72c9 0000 00da  r....r....r.....
-00006e10: 1261 6c69 676e 5f74 7261 6a65 6374 6f72  .align_trajector
-00006e20: 6965 7372 dd00 0000 72de 0000 00da 0361  iesr....r......a
-00006e30: 6273 72be 0000 0072 db00 0000 72d7 0000  bsr....r....r...
-00006e40: 0072 cd00 0000 da0b 6672 6f6d 5f74 7570  .r......from_tup
-00006e50: 6c65 73da 0d72 6f6c 6c69 6e67 5f73 7065  les..rolling_spe
-00006e60: 6564 720d 0100 0072 e100 0000 da0b 6765  edr....r......ge
-00006e70: 745f 7175 616c 6974 79da 0672 6570 6561  t_quality..repea
-00006e80: 7472 3601 0000 72d4 0000 0072 da00 0000  tr6...r....r....
-00006e90: 7231 0100 0072 4001 0000 291b 7256 0000  r1...r@...).rV..
-00006ea0: 0072 4201 0000 7243 0100 0072 4401 0000  .rB...rC...rD...
-00006eb0: 7245 0100 0072 4601 0000 7247 0100 0072  rE...rF...rG...r
-00006ec0: 4801 0000 7249 0100 00da 0474 6162 73da  H...rI.....tabs.
-00006ed0: 0763 6f6f 7264 5f31 da07 636f 6f72 645f  .coord_1..coord_
-00006ee0: 3272 f000 0000 72e4 0000 0072 5400 0000  2r....r....rT...
-00006ef0: 724b 0000 0072 2701 0000 7233 0000 00da  rK...r'...r3....
-00006f00: 0961 6c6c 5f69 6e64 6578 da0b 616c 6c5f  .all_index..all_
-00006f10: 636f 6c75 6d6e 73da 1361 6c69 676e 6564  columns..aligned
-00006f20: 5f63 6f6f 7264 696e 6174 6573 72b7 0000  _coordinatesr...
-00006f30: 00da 0f70 6172 7469 616c 5f61 6c69 676e  ...partial_align
-00006f40: 6564 da03 7665 6c72 f700 0000 da0b 616e  ed..velr......an
-00006f50: 6e6f 7461 7469 6f6e 73da 0361 6e6e 7226  notations..annr&
-00006f60: 0000 0029 0372 9600 0000 7245 0100 0072  ...).r....rE...r
-00006f70: 4201 0000 7227 0000 00da 0a67 6574 5f63  B...r'.....get_c
-00006f80: 6f6f 7264 732c 0300 0073 de00 0000 001b  oords,...s......
-00006f90: 0e01 0801 0602 0401 0801 1001 1001 1202  ................
-00006fa0: 0a02 1803 26ff 1a05 26ff 2004 1602 1a03  ....&...&. .....
-00006fb0: 0601 0a01 0602 0802 0401 2201 14ff 0403  ..........".....
-00006fc0: 2001 02fc 04ff 040a 0401 2201 14ff 0403   .........".....
-00006fd0: 2001 02fc 04ff 0c09 0602 0c01 16ff 0c02   ...............
-00006fe0: 02fe 0403 0c01 16ff 0c02 02fe 0404 1202  ................
-00006ff0: 0601 0401 0402 0802 0c02 04fe 0607 1801  ................
-00007000: 0cfe 0205 1801 0cfe 02fb 0209 02f7 040b  ................
-00007010: 0801 0802 0c01 0601 0aff 0603 1201 0a01  ................
-00007020: 0401 08ff 0a04 0601 0e01 0c02 0601 1001  ................
-00007030: 1201 0c03 0a01 1001 0401 16ff 0c05 1402  ................
-00007040: 0601 1202 1001 0801 2c02 0601 1001 0401  ........,.......
-00007050: 16ff 1604 0201 0201 0201 0401 0401 0401  ................
-00007060: 0201 0401 0201 0401 0201 02f5 7a16 436f  ............z.Co
-00007070: 6f72 6469 6e61 7465 732e 6765 745f 636f  ordinates.get_co
-00007080: 6f72 6473 2906 7244 0100 0072 4701 0000  ords).rD...rG...
-00007090: da0f 6669 6c74 6572 5f6f 6e5f 6772 6170  ..filter_on_grap
-000070a0: 6872 4801 0000 7249 0100 0072 1900 0000  hrH...rI...r....
-000070b0: 6306 0000 0000 0000 0000 0000 000d 0000  c...............
-000070c0: 000a 0000 0043 0000 0073 aa01 0000 7400  .....C...s....t.
-000070d0: 6a01 a002 7c00 6a03 a101 7d06 7c00 6a03  j...|.j...}.|.j.
-000070e0: 6401 7501 9001 729e 7c01 724e 7c06 a004  d.u...r.|.rN|...
-000070f0: a100 4400 5d26 5c02 7d07 7d08 7400 6a01  ..D.]&\.}.}.t.j.
-00007100: 6a05 7c08 7c01 6402 1700 6403 6404 8d03  j.|.|.d...d.d...
-00007110: 7d09 7c09 7c06 7c07 3c00 7126 7c02 6401  }.|.|.|.<.q&|.d.
-00007120: 7501 728a 7c06 a004 a100 4400 5d2a 5c02  u.r.|.....D.]*\.
-00007130: 7d07 7d0a 7c0a 6a06 6401 6401 8502 7400  }.}.|.j.d.d...t.
-00007140: 6a01 a007 7c0a 6a08 7c02 a102 6602 1900  j...|.j.|...f...
-00007150: 7c06 7c07 3c00 715e 7400 6a01 a009 7c00  |.|.<.q^t.j...|.
-00007160: 7c06 7c00 a00a a100 a103 7d06 7c04 72cc  |.|.......}.|.r.
-00007170: 7c06 a004 a100 4400 5d20 5c02 7d07 7d08  |.....D.] \.}.}.
-00007180: 7c00 6a0b 7c07 1900 7c08 6a06 6401 6401  |.j.|...|.j.d.d.
-00007190: 8502 6405 6602 3c00 71aa 7c05 9001 7224  ..d.f.<.q.|...r$
-000071a0: 740c 7c05 a00d a100 8301 6406 1900 6a08  t.|.......d...j.
-000071b0: 7d0b 7c06 a004 a100 4400 5d36 5c02 7d07  }.|.....D.]6\.}.
-000071c0: 7d08 7c0b 4400 5d28 7d0c 7c05 7c07 1900  }.|.D.](}.|.|...
-000071d0: 6a06 6401 6401 8502 7c0c 6602 1900 7c08  j.d.d...|.f...|.
-000071e0: 6a06 6401 6401 8502 7c0c 6602 3c00 71f8  j.d.d...|.f.<.q.
-000071f0: 71ec 7c03 9001 7282 7c06 a004 a100 4400  q.|...r.|.....D.
-00007200: 5d4e 5c02 7d07 7d08 7c08 6a06 6401 6401  ]N\.}.}.|.j.d.d.
-00007210: 8502 740c 740e 6407 6408 8400 7400 6a01  ..t.t.d.d...t.j.
-00007220: 6a0f 7c00 6a10 7c00 6a11 6409 8d02 6a12  j.|.j.|.j.d...j.
-00007230: 4400 8301 8301 740e 7c08 6a08 8301 4000  D.....t.|.j...@.
-00007240: 8301 6602 1900 7c06 7c07 3c00 9001 7132  ..f...|.|.<...q2
-00007250: 7413 7c06 7c00 6a10 7c00 6a14 7c00 6a0b  t.|.|.j.|.j.|.j.
-00007260: 7c04 7c05 6403 640a 8d07 5300 7415 640b  |.|.d.d...S.t.d.
-00007270: 8301 8201 6401 5300 290c 61d3 0200 0052  ....d.S.).a....R
-00007280: 6574 7572 6e20 6120 7461 626c 655f 6469  eturn a table_di
-00007290: 6374 206f 626a 6563 7420 7769 7468 2074  ct object with t
-000072a0: 6865 2064 6973 7461 6e63 6573 2062 6574  he distances bet
-000072b0: 7765 656e 2062 6f64 7920 7061 7274 7320  ween body parts 
-000072c0: 616e 696d 616c 2061 7320 7661 6c75 6573  animal as values
-000072d0: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
-000072e0: 0a20 2020 2020 2020 2020 2020 2073 7065  .            spe
-000072f0: 6564 2028 696e 7429 3a20 5468 6520 6465  ed (int): The de
-00007300: 7269 7661 7469 7665 2074 6f20 7573 6520  rivative to use 
-00007310: 666f 7220 7370 6565 642e 0a20 2020 2020  for speed..     
-00007320: 2020 2020 2020 2073 656c 6563 7465 645f         selected_
-00007330: 6964 2028 7374 7229 3a20 5468 6520 6964  id (str): The id
-00007340: 206f 6620 7468 6520 616e 696d 616c 2074   of the animal t
-00007350: 6f20 7365 6c65 6374 2e0a 2020 2020 2020  o select..      
-00007360: 2020 2020 2020 6669 6c74 6572 5f6f 6e5f        filter_on_
-00007370: 6772 6170 6820 2862 6f6f 6c29 3a20 4966  graph (bool): If
-00007380: 2054 7275 652c 206f 6e6c 7920 6469 7374   True, only dist
-00007390: 616e 6365 7320 6265 7477 6565 6e20 636f  ances between co
-000073a0: 6e6e 6563 7465 6420 6e6f 6465 7320 696e  nnected nodes in
-000073b0: 2074 6865 2044 6565 704f 4620 6772 6170   the DeepOF grap
-000073c0: 6820 7265 7072 6573 656e 7461 7469 6f6e  h representation
-000073d0: 7320 6172 6520 6b65 7074 2e20 4f74 6865  s are kept. Othe
-000073e0: 7277 6973 652c 2061 6c6c 2064 6973 7461  rwise, all dista
-000073f0: 6e63 6573 2062 6574 7765 656e 2062 6f64  nces between bod
-00007400: 7970 6172 7473 2061 7265 2072 6574 7572  yparts are retur
-00007410: 6e65 642e 0a20 2020 2020 2020 2020 2020  ned..           
-00007420: 2070 726f 7061 6761 7465 5f6c 6162 656c   propagate_label
-00007430: 7320 2862 6f6f 6c29 3a20 4966 2054 7275  s (bool): If Tru
-00007440: 652c 2074 6865 2070 6865 6e6f 2063 6f6c  e, the pheno col
-00007450: 756d 6e20 7769 6c6c 2062 6520 7072 6f70  umn will be prop
-00007460: 6167 6174 6564 2066 726f 6d20 7468 6520  agated from the 
-00007470: 6f72 6967 696e 616c 2064 6174 612e 0a20  original data.. 
-00007480: 2020 2020 2020 2020 2020 2070 726f 7061             propa
-00007490: 6761 7465 5f61 6e6e 6f74 6174 696f 6e73  gate_annotations
-000074a0: 2028 4469 6374 293a 2041 2064 6963 7469   (Dict): A dicti
-000074b0: 6f6e 6172 7920 6f66 2061 6e6e 6f74 6174  onary of annotat
-000074c0: 696f 6e73 2074 6f20 7072 6f70 6167 6174  ions to propagat
-000074d0: 652e 0a0a 2020 2020 2020 2020 5265 7475  e...        Retu
-000074e0: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
-000074f0: 2074 6162 6c65 5f64 6963 743a 2041 2074   table_dict: A t
-00007500: 6162 6c65 5f64 6963 7420 6f62 6a65 6374  able_dict object
-00007510: 2077 6974 6820 7468 6520 6469 7374 616e   with the distan
-00007520: 6365 7320 6265 7477 6565 6e20 626f 6479  ces between body
-00007530: 2070 6172 7473 2061 6e69 6d61 6c20 6173   parts animal as
-00007540: 2076 616c 7565 732e 0a0a 2020 2020 2020   values...      
-00007550: 2020 4e72 3100 0000 da05 6469 7374 73a9    Nr1.....dists.
-00007560: 0272 4f01 0000 72af 0000 0072 5001 0000  .rO...r....rP...
-00007570: 7201 0000 0063 0100 0000 0000 0000 0000  r....c..........
-00007580: 0000 0200 0000 0500 0000 5300 0000 7318  ..........S...s.
-00007590: 0000 0067 007c 005d 107d 0174 0074 017c  ...g.|.].}.t.t.|
-000075a0: 0183 0183 0191 0271 0453 0072 2600 0000  .......q.S.r&...
-000075b0: a902 72d1 0000 0072 5b00 0000 a902 724a  ..r....r[.....rJ
-000075c0: 0000 00da 0165 7226 0000 0072 2600 0000  .....er&...r&...
-000075d0: 7227 0000 0072 4c00 0000 1004 0000 7304  r'...rL.......s.
-000075e0: 0000 0006 0202 ff7a 2d43 6f6f 7264 696e  .......z-Coordin
-000075f0: 6174 6573 2e67 6574 5f64 6973 7461 6e63  ates.get_distanc
-00007600: 6573 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  es.<locals>.<lis
-00007610: 7463 6f6d 703e 2902 7233 0000 0072 9300  tcomp>).r3...r..
-00007620: 0000 a906 7233 0000 0072 6300 0000 7238  ....r3...rc...r8
-00007630: 0000 0072 4801 0000 7249 0100 0072 af00  ...rH...rI...r..
-00007640: 0000 7a3f 4469 7374 616e 6365 7320 6e6f  ..z?Distances no
-00007650: 7420 636f 6d70 7574 6564 2e20 5265 6164  t computed. Read
-00007660: 2074 6865 2064 6f63 756d 656e 7461 7469   the documentati
-00007670: 6f6e 2066 6f72 206d 6f72 6520 6465 7461  on for more deta
-00007680: 696c 7329 1672 8100 0000 7282 0000 0072  ils).r....r....r
-00007690: 5101 0000 727a 0000 0072 cb00 0000 725d  Q...rz...r....r]
-000076a0: 0100 0072 c300 0000 720d 0100 0072 b700  ...r....r....r..
-000076b0: 0000 72e1 0000 0072 5e01 0000 7236 0100  ..r....r^...r6..
-000076c0: 0072 b500 0000 72c8 0000 0072 b600 0000  .r....r....r....
-000076d0: 7294 0000 0072 3001 0000 7234 0100 00da  r....r0...r4....
-000076e0: 0565 6467 6573 72da 0000 0072 4001 0000  .edgesr....r@...
-000076f0: da0a 5661 6c75 6545 7272 6f72 290d 7256  ..ValueError).rV
-00007700: 0000 0072 4401 0000 7247 0100 0072 6b01  ...rD...rG...rk.
-00007710: 0000 7248 0100 0072 4901 0000 7260 0100  ..rH...rI...r`..
-00007720: 0072 e400 0000 7254 0000 0072 6701 0000  .r....rT...rg...
-00007730: 72f7 0000 0072 6801 0000 7269 0100 0072  r....rh...ri...r
-00007740: 2600 0000 7226 0000 0072 2700 0000 72f8  &...r&...r'...r.
-00007750: 0000 00d7 0300 0073 6400 0000 0015 0e02  .......sd.......
-00007760: 0c02 0401 1001 1601 0a02 0801 1001 0401  ................
-00007770: 16ff 0a05 1402 0401 1001 1a02 0601 1202  ................
-00007780: 1001 0801 2802 0602 1001 0401 0601 0201  ....(...........
-00007790: 0201 0602 0601 0401 04fe 06fe 04ff 0209  ................
-000077a0: 08f7 02ff 02ff 02ff 0c10 0201 0201 0401  ................
-000077b0: 0401 0401 0201 0201 02f9 060a 0201 02ff  ................
-000077c0: 7a19 436f 6f72 6469 6e61 7465 732e 6765  z.Coordinates.ge
-000077d0: 745f 6469 7374 616e 6365 7329 06da 0764  t_distances)...d
-000077e0: 6567 7265 6573 7244 0100 0072 4701 0000  egreesrD...rG...
-000077f0: 7248 0100 0072 4901 0000 7219 0000 0063  rH...rI...r....c
-00007800: 0600 0000 0000 0000 0000 0000 0d00 0000  ................
-00007810: 0900 0000 4300 0000 735a 0100 0074 006a  ....C...sZ...t.j
-00007820: 01a0 027c 006a 03a1 017d 067c 006a 0364  ...|.j...}.|.j.d
-00007830: 0175 0190 0172 4e7c 0172 3064 0264 0384  .u...rN|.r0d.d..
-00007840: 007c 06a0 04a1 0044 0083 017d 067c 0272  .|.....D...}.|.r
-00007850: 647c 06a0 04a1 0044 005d 265c 027d 077d  d|.....D.]&\.}.}
-00007860: 0874 006a 016a 057c 087c 0264 0417 0064  .t.j.j.|.|.d...d
-00007870: 0564 068d 037d 097c 097c 067c 073c 0071  .d...}.|.|.|.<.q
-00007880: 3c7c 0364 0175 0172 a07c 06a0 04a1 0044  <|.d.u.r.|.....D
-00007890: 005d 2a5c 027d 077d 0a7c 0a6a 0664 0164  .]*\.}.}.|.j.d.d
-000078a0: 0185 0274 006a 01a0 077c 0a6a 087c 03a1  ...t.j...|.j.|..
-000078b0: 0266 0219 007c 067c 073c 0071 7474 006a  .f...|.|.<.qtt.j
-000078c0: 01a0 097c 007c 067c 00a0 0aa1 00a1 037d  ...|.|.|.......}
-000078d0: 067c 0472 d87c 06a0 04a1 0044 005d 165c  .|.r.|.....D.].\
-000078e0: 027d 077d 087c 006a 0b7c 0719 007c 0864  .}.}.|.j.|...|.d
-000078f0: 073c 0071 c07c 0590 0172 3274 0c7c 05a0  .<.q.|...r2t.|..
-00007900: 0da1 0083 0164 0819 006a 087d 0b7c 06a0  .....d...j.}.|..
-00007910: 04a1 0044 005d 385c 027d 077d 087c 0b44  ...D.]8\.}.}.|.D
-00007920: 005d 2a7d 0c7c 057c 0719 006a 0664 0164  .]*}.|.|...j.d.d
-00007930: 0185 027c 0c66 0219 007c 086a 0664 0164  ...|.f...|.j.d.d
-00007940: 0185 027c 0c66 023c 0090 0171 0471 f874  ...|.f.<...q.q.t
-00007950: 0e7c 067c 006a 0f7c 006a 107c 006a 0b7c  .|.|.j.|.j.|.j.|
-00007960: 047c 0564 0564 098d 0753 0074 1164 0a83  .|.d.d...S.t.d..
-00007970: 0182 0164 0153 0029 0b61 8d02 0000 5265  ...d.S.).a....Re
-00007980: 7475 726e 2061 2074 6162 6c65 5f64 6963  turn a table_dic
-00007990: 7420 6f62 6a65 6374 2077 6974 6820 7468  t object with th
-000079a0: 6520 616e 676c 6573 2062 6574 7765 656e  e angles between
-000079b0: 2062 6f64 7920 7061 7274 7320 616e 696d   body parts anim
-000079c0: 616c 2061 7320 7661 6c75 6573 2e0a 0a20  al as values... 
-000079d0: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
-000079e0: 2020 2020 2020 2020 2064 6567 7265 6573           degrees
-000079f0: 2028 626f 6f6c 293a 2049 6620 5472 7565   (bool): If True
-00007a00: 2028 6465 6661 756c 7429 2c20 7468 6520   (default), the 
-00007a10: 616e 676c 6573 2077 696c 6c20 6265 2069  angles will be i
-00007a20: 6e20 6465 6772 6565 732e 204f 7468 6572  n degrees. Other
-00007a30: 7769 7365 2074 6865 7920 7769 6c6c 2062  wise they will b
-00007a40: 6520 636f 6e76 6572 7465 6420 746f 2072  e converted to r
-00007a50: 6164 6961 6e73 2e0a 2020 2020 2020 2020  adians..        
-00007a60: 2020 2020 7370 6565 6420 2869 6e74 293a      speed (int):
-00007a70: 2054 6865 2064 6572 6976 6174 6976 6520   The derivative 
-00007a80: 746f 2075 7365 2066 6f72 2073 7065 6564  to use for speed
-00007a90: 2e0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00007aa0: 6c65 6374 6564 5f69 6420 2873 7472 293a  lected_id (str):
-00007ab0: 2054 6865 2069 6420 6f66 2074 6865 2061   The id of the a
-00007ac0: 6e69 6d61 6c20 746f 2073 656c 6563 742e  nimal to select.
-00007ad0: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
-00007ae0: 7061 6761 7465 5f6c 6162 656c 7320 2862  pagate_labels (b
-00007af0: 6f6f 6c29 3a20 4966 2054 7275 652c 2074  ool): If True, t
-00007b00: 6865 2070 6865 6e6f 2063 6f6c 756d 6e20  he pheno column 
-00007b10: 7769 6c6c 2062 6520 7072 6f70 6167 6174  will be propagat
-00007b20: 6564 2066 726f 6d20 7468 6520 6f72 6967  ed from the orig
-00007b30: 696e 616c 2064 6174 612e 0a20 2020 2020  inal data..     
-00007b40: 2020 2020 2020 2070 726f 7061 6761 7465         propagate
-00007b50: 5f61 6e6e 6f74 6174 696f 6e73 2028 4469  _annotations (Di
-00007b60: 6374 293a 2041 2064 6963 7469 6f6e 6172  ct): A dictionar
-00007b70: 7920 6f66 2061 6e6e 6f74 6174 696f 6e73  y of annotations
-00007b80: 2074 6f20 7072 6f70 6167 6174 652e 0a0a   to propagate...
-00007b90: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-00007ba0: 0a20 2020 2020 2020 2020 2020 2074 6162  .            tab
-00007bb0: 6c65 5f64 6963 743a 2041 2074 6162 6c65  le_dict: A table
-00007bc0: 5f64 6963 7420 6f62 6a65 6374 2077 6974  _dict object wit
-00007bd0: 6820 7468 6520 616e 676c 6573 2062 6574  h the angles bet
-00007be0: 7765 656e 2062 6f64 7920 7061 7274 7320  ween body parts 
-00007bf0: 616e 696d 616c 2061 7320 7661 6c75 6573  animal as values
-00007c00: 2e0a 0a20 2020 2020 2020 204e 6301 0000  ...        Nc...
-00007c10: 0000 0000 0000 0000 0003 0000 0006 0000  ................
-00007c20: 0053 0000 0073 1c00 0000 6900 7c00 5d14  .S...s....i.|.].
-00007c30: 5c02 7d01 7d02 7c01 7400 a001 7c02 a101  \.}.}.|.t...|...
-00007c40: 9302 7104 5300 7226 0000 0029 0272 dd00  ..q.S.r&...).r..
-00007c50: 0000 7274 0100 0029 0372 4a00 0000 72e4  ..rt...).rJ...r.
-00007c60: 0000 0072 5400 0000 7226 0000 0072 2600  ...rT...r&...r&.
-00007c70: 0000 7227 0000 0072 9700 0000 4304 0000  ..r'...r....C...
-00007c80: 724d 0000 007a 2a43 6f6f 7264 696e 6174  rM...z*Coordinat
-00007c90: 6573 2e67 6574 5f61 6e67 6c65 732e 3c6c  es.get_angles.<l
-00007ca0: 6f63 616c 733e 2e3c 6469 6374 636f 6d70  ocals>.<dictcomp
-00007cb0: 3e72 3100 0000 7261 0000 0072 6d01 0000  >r1...ra...rm...
-00007cc0: 7250 0100 0072 0100 0000 7271 0100 007a  rP...r....rq...z
-00007cd0: 3c41 6e67 6c65 7320 6e6f 7420 636f 6d70  <Angles not comp
-00007ce0: 7574 6564 2e20 5265 6164 2074 6865 2064  uted. Read the d
-00007cf0: 6f63 756d 656e 7461 7469 6f6e 2066 6f72  ocumentation for
-00007d00: 206d 6f72 6520 6465 7461 696c 7329 1272   more details).r
-00007d10: 8100 0000 7282 0000 0072 5101 0000 727e  ....r....rQ...r~
-00007d20: 0000 0072 cb00 0000 725d 0100 0072 c300  ...r....r]...r..
-00007d30: 0000 720d 0100 0072 b700 0000 72e1 0000  ..r....r....r...
-00007d40: 0072 5e01 0000 7236 0100 0072 b500 0000  .r^...r6...r....
-00007d50: 72c8 0000 0072 da00 0000 7230 0100 0072  r....r....r0...r
-00007d60: 4001 0000 7273 0100 0029 0d72 5600 0000  @...rs...).rV...
-00007d70: 7274 0100 0072 4401 0000 7247 0100 0072  rt...rD...rG...r
-00007d80: 4801 0000 7249 0100 0072 6001 0000 72e4  H...rI...r`...r.
-00007d90: 0000 0072 5400 0000 7267 0100 0072 f700  ...rT...rg...r..
-00007da0: 0000 7268 0100 0072 6901 0000 7226 0000  ..rh...ri...r&..
-00007db0: 0072 2600 0000 7227 0000 0072 0301 0000  .r&...r'...r....
-00007dc0: 2a04 0000 7344 0000 0000 150e 020c 0104  *...sD..........
-00007dd0: 0112 0204 0110 0116 010a 0208 0110 0104  ................
-00007de0: 0116 ff0a 0514 0204 0110 0110 0206 0112  ................
-00007df0: 0210 0108 012a 0202 0102 0104 0104 0104  .....*..........
-00007e00: 0102 0102 0102 f906 0a02 0102 ff7a 1643  .............z.C
-00007e10: 6f6f 7264 696e 6174 6573 2e67 6574 5f61  oordinates.get_a
-00007e20: 6e67 6c65 7372 5700 0000 2903 7244 0100  nglesrW...).rD..
-00007e30: 0072 4701 0000 7219 0000 0063 0300 0000  .rG...r....c....
-00007e40: 0000 0000 0000 0000 0c00 0000 0800 0000  ................
-00007e50: 4300 0000 7306 0100 0074 006a 01a0 027c  C...s....t.j...|
-00007e60: 006a 03a1 017d 037c 006a 0364 0175 0172  .j...}.|.j.d.u.r
-00007e70: fa7c 0264 026b 0272 287c 006a 047d 046e  .|.d.k.r(|.j.}.n
-00007e80: 067c 0267 017d 047c 03a0 05a1 0044 005d  .|.g.}.|.....D.]
-00007e90: 5e5c 027d 057d 0674 06a0 07a1 007d 077c  ^\.}.}.t.....}.|
-00007ea0: 0444 005d 407d 087c 0864 036b 0272 5a64  .D.]@}.|.d.k.rZd
-00007eb0: 017d 087c 066a 0864 0164 0185 0274 006a  .}.|.j.d.d...t.j
-00007ec0: 01a0 097c 066a 0a7c 08a1 0266 0219 007d  ...|.j.|...f...}
-00007ed0: 0974 066a 0b7c 077c 0967 0264 0464 058d  .t.j.|.|.g.d.d..
-00007ee0: 027d 0771 4a7c 077c 037c 053c 0071 367c  .}.qJ|.|.|.<.q6|
-00007ef0: 0172 ca7c 03a0 05a1 0044 005d 265c 027d  .r.|.....D.]&\.}
-00007f00: 057d 0674 006a 016a 0c7c 067c 0164 0417  .}.t.j.j.|.|.d..
-00007f10: 0064 0664 078d 037d 0a7c 0a7c 037c 053c  .d.d...}.|.|.|.<
-00007f20: 0071 a274 006a 01a0 0d7c 007c 037c 00a0  .q.t.j...|.|.|..
-00007f30: 0ea1 00a1 037d 0374 0f7c 037c 006a 047c  .....}.t.|.|.j.|
-00007f40: 006a 1064 087c 006a 1164 098d 057d 0b7c  .j.d.|.j.d...}.|
-00007f50: 0b53 0074 1264 0a83 0182 0164 0153 0029  .S.t.d.....d.S.)
-00007f60: 0b61 e501 0000 5265 7475 726e 2061 2074  .a....Return a t
-00007f70: 6162 6c65 5f64 6963 7420 6f62 6a65 6374  able_dict object
-00007f80: 2077 6974 6820 616c 6c20 7265 6c65 7661   with all releva
-00007f90: 6e74 2061 7265 6173 2028 6865 6164 2c20  nt areas (head, 
-00007fa0: 746f 7273 6f2c 2062 6163 6b2c 2066 756c  torso, back, ful
-00007fb0: 6c29 2e20 556e 6c65 7373 2073 7065 6369  l). Unless speci
-00007fc0: 6669 6564 206f 7468 6572 7769 7365 2c20  fied otherwise, 
-00007fd0: 7468 6520 6172 6561 7320 6172 6520 636f  the areas are co
-00007fe0: 6d70 7574 6564 2066 6f72 2061 6c6c 2061  mputed for all a
-00007ff0: 6e69 6d61 6c73 2e0a 0a20 2020 2020 2020  nimals...       
-00008000: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
-00008010: 2020 2073 7065 6564 2028 696e 7429 3a20     speed (int): 
-00008020: 5468 6520 6465 7269 7661 7469 7665 2074  The derivative t
-00008030: 6f20 7573 6520 666f 7220 7370 6565 642e  o use for speed.
-00008040: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00008050: 6563 7465 645f 6964 2028 7374 7229 3a20  ected_id (str): 
-00008060: 5468 6520 6964 206f 6620 7468 6520 616e  The id of the an
-00008070: 696d 616c 2074 6f20 7365 6c65 6374 2e20  imal to select. 
-00008080: 2261 6c6c 2220 2864 6566 6175 6c74 2920  "all" (default) 
-00008090: 636f 6d70 7574 6573 2074 6865 2061 7265  computes the are
-000080a0: 6173 2066 6f72 2061 6c6c 2061 6e69 6d61  as for all anima
-000080b0: 6c73 2e20 4465 636c 6172 6564 2069 6e20  ls. Declared in 
-000080c0: 7365 6c66 2e5f 616e 696d 616c 5f69 6473  self._animal_ids
-000080d0: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-000080e0: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
-000080f0: 7461 626c 655f 6469 6374 3a20 4120 7461  table_dict: A ta
-00008100: 626c 655f 6469 6374 206f 626a 6563 7420  ble_dict object 
-00008110: 7769 7468 2074 6865 2061 7265 6173 206f  with the areas o
-00008120: 6620 7468 6520 626f 6479 2070 6172 7473  f the body parts
-00008130: 2061 6e69 6d61 6c20 6173 2076 616c 7565   animal as value
-00008140: 732e 0a20 2020 2020 2020 204e 7257 0000  s..        NrW..
-00008150: 0072 2c00 0000 7231 0000 0072 ab00 0000  .r,...r1...r....
-00008160: 7261 0000 0072 6d01 0000 7262 0000 0029  ra...rm...rb...)
-00008170: 0472 3300 0000 7263 0000 0072 af00 0000  .r3...rc...r....
-00008180: 7238 0000 007a 3b41 7265 6173 206e 6f74  r8...z;Areas not
-00008190: 2063 6f6d 7075 7465 642e 2052 6561 6420   computed. Read 
-000081a0: 7468 6520 646f 6375 6d65 6e74 6174 696f  the documentatio
-000081b0: 6e20 666f 7220 6d6f 7265 2064 6574 6169  n for more detai
-000081c0: 6c73 2913 7281 0000 0072 8200 0000 7251  ls).r....r....rQ
-000081d0: 0100 0072 3f01 0000 7230 0100 0072 cb00  ...r?...r0...r..
-000081e0: 0000 72be 0000 0072 db00 0000 72c3 0000  ..r....r....r...
-000081f0: 0072 0d01 0000 72b7 0000 0072 d700 0000  .r....r....r....
-00008200: 725d 0100 0072 e100 0000 725e 0100 0072  r]...r....r^...r
-00008210: da00 0000 7240 0100 0072 3601 0000 7273  ....r@...r6...rs
-00008220: 0100 0029 0c72 5600 0000 7244 0100 0072  ...).rV...rD...r
-00008230: 4701 0000 7260 0100 00da 0c73 656c 6563  G...r`.....selec
-00008240: 7465 645f 6964 7372 e400 0000 7254 0000  ted_idsr....rT..
-00008250: 0072 1401 0000 7296 0000 0072 1501 0000  .r....r....r....
-00008260: 7267 0100 0072 6200 0000 7226 0000 0072  rg...rb...r&...r
-00008270: 2600 0000 7227 0000 0072 1601 0000 6c04  &...r'...r....l.
-00008280: 0000 733e 0000 0000 0a0e 020a 0208 0108  ..s>............
-00008290: 0206 0210 0208 0208 0208 0104 0304 0116  ................
-000082a0: ff04 0314 020a 0204 0110 0116 010a 0314  ................
-000082b0: 0202 0102 0104 0104 0102 0104 fb06 0804  ................
-000082c0: 0202 0102 ff7a 1543 6f6f 7264 696e 6174  .....z.Coordinat
-000082d0: 6573 2e67 6574 5f61 7265 6173 2901 da04  es.get_areas)...
-000082e0: 706c 6179 6302 0000 0000 0000 0000 0000  playc...........
-000082f0: 0002 0000 0001 0000 0043 0000 0073 0e00  .........C...s..
-00008300: 0000 7c01 7208 7400 8201 7c00 6a01 5300  ..|.r.t...|.j.S.
-00008310: 2901 7a39 5265 7475 656e 7320 7468 6520  ).z9Retuens the 
-00008320: 7669 6465 6f73 2061 7373 6f63 6961 7465  videos associate
-00008330: 6420 7769 7468 2074 6865 2064 6174 6173  d with the datas
-00008340: 6574 2061 7320 6120 6c69 7374 2e29 0272  et as a list.).r
-00008350: bd00 0000 723d 0100 0029 0272 5600 0000  ....r=...).rV...
-00008360: 7276 0100 0072 2600 0000 7226 0000 0072  rv...r&...r&...r
-00008370: 2700 0000 da0a 6765 745f 7669 6465 6f73  '.....get_videos
-00008380: a604 0000 7306 0000 0000 0204 0104 027a  ....s..........z
-00008390: 1643 6f6f 7264 696e 6174 6573 2e67 6574  .Coordinates.get
-000083a0: 5f76 6964 656f 7363 0100 0000 0000 0000  _videosc........
-000083b0: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
-000083c0: 7306 0000 007c 006a 0053 0029 017a 4652  s....|.j.S.).zFR
-000083d0: 6574 7572 6e20 7468 6520 7374 6f72 6564  eturn the stored
-000083e0: 2064 6963 7469 6f6e 6172 7920 7769 7468   dictionary with
-000083f0: 2065 7870 6572 696d 656e 7461 6c20 636f   experimental co
-00008400: 6e64 6974 696f 6e73 2070 6572 2073 7562  nditions per sub
-00008410: 6a65 6374 2e29 0172 3601 0000 7255 0000  ject.).r6...rU..
-00008420: 0072 2600 0000 7226 0000 0072 2700 0000  .r&...r&...r'...
-00008430: da12 6765 745f 6578 705f 636f 6e64 6974  ..get_exp_condit
-00008440: 696f 6e73 ad04 0000 7302 0000 0000 037a  ions....s......z
-00008450: 1e43 6f6f 7264 696e 6174 6573 2e67 6574  .Coordinates.get
-00008460: 5f65 7870 5f63 6f6e 6469 7469 6f6e 7363  _exp_conditionsc
-00008470: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00008480: 0400 0000 0300 0000 7338 0000 0074 006a  ........s8...t.j
-00008490: 017c 0164 0164 028d 0289 0087 0066 0164  .|.d.d.......f.d
-000084a0: 0364 0484 0888 006a 0264 0564 0585 0264  .d.....j.d.d...d
-000084b0: 0166 0219 0044 0083 0189 0088 007c 005f  .f...D.......|._
-000084c0: 0364 0553 0029 067a a84c 6f61 6420 6578  .d.S.).z.Load ex
-000084d0: 7065 7269 6d65 6e74 616c 2063 6f6e 6469  perimental condi
-000084e0: 7469 6f6e 7320 6672 6f6d 2061 2077 6964  tions from a wid
-000084f0: 652d 666f 726d 6174 2063 7376 2074 6162  e-format csv tab
-00008500: 6c65 2e0a 0a20 2020 2020 2020 2041 7267  le...        Arg
-00008510: 733a 0a20 2020 2020 2020 2020 2020 2066  s:.            f
-00008520: 696c 6570 6174 6820 2873 7472 293a 2050  ilepath (str): P
-00008530: 6174 6820 746f 2074 6865 2066 696c 6520  ath to the file 
-00008540: 636f 6e74 6169 6e69 6e67 2074 6865 2065  containing the e
-00008550: 7870 6572 696d 656e 7461 6c20 636f 6e64  xperimental cond
-00008560: 6974 696f 6e73 2e0a 0a20 2020 2020 2020  itions...       
-00008570: 2072 0100 0000 2901 7289 0000 0063 0100   r....).r....c..
-00008580: 0000 0000 0000 0000 0000 0200 0000 0900  ................
-00008590: 0000 1300 0000 7348 0000 0069 007c 005d  ......sH...i.|.]
-000085a0: 407d 017c 0174 00a0 0188 006a 0288 006a  @}.|.t.....j...j
-000085b0: 0364 0064 0085 0264 0166 0219 007c 016b  .d.d...d.f...|.k
-000085c0: 0264 0064 0085 0266 0219 006a 0364 0164  .d.d...f...j.d.d
-000085d0: 0264 0085 0266 0219 00a1 016a 0493 0271  .d...f.....j...q
-000085e0: 0453 0029 034e 7201 0000 0072 3100 0000  .S.).Nr....r1...
-000085f0: 2905 72be 0000 0072 db00 0000 72c3 0000  ).r....r....r...
-00008600: 0072 9100 0000 72c1 0000 0029 0272 4a00  .r....r....).rJ.
-00008610: 0000 da06 6578 705f 6964 a901 7238 0000  ....exp_id..r8..
-00008620: 0072 2600 0000 7227 0000 0072 9700 0000  .r&...r'...r....
-00008630: ba04 0000 7308 0000 0006 0402 fd06 0130  ....s..........0
-00008640: ff7a 3343 6f6f 7264 696e 6174 6573 2e6c  .z3Coordinates.l
-00008650: 6f61 645f 6578 705f 636f 6e64 6974 696f  oad_exp_conditio
-00008660: 6e73 2e3c 6c6f 6361 6c73 3e2e 3c64 6963  ns.<locals>.<dic
-00008670: 7463 6f6d 703e 4e29 0472 be00 0000 72c4  tcomp>N).r....r.
-00008680: 0000 0072 9100 0000 7236 0100 0029 0272  ...r....r6...).r
-00008690: 5600 0000 da08 6669 6c65 7061 7468 7226  V.....filepathr&
-000086a0: 0000 0072 7a01 0000 7227 0000 00da 136c  ...rz...r'.....l
-000086b0: 6f61 645f 6578 705f 636f 6e64 6974 696f  oad_exp_conditio
-000086c0: 6e73 b204 0000 730a 0000 0000 070e 010a  ns....s.........
-000086d0: 0410 fc06 067a 1f43 6f6f 7264 696e 6174  .....z.Coordinat
-000086e0: 6573 2e6c 6f61 645f 6578 705f 636f 6e64  es.load_exp_cond
-000086f0: 6974 696f 6e73 6301 0000 0000 0000 0000  itionsc.........
-00008700: 0000 0001 0000 0005 0000 0043 0000 0073  ...........C...s
-00008710: 1200 0000 7400 7c00 6a01 6401 7c00 6a02  ....t.|.j.d.|.j.
-00008720: 6402 8d03 5300 2903 7a4d 5265 7472 6965  d...S.).zMRetrie
-00008730: 7665 2061 2064 6963 7469 6f6e 6172 7920  ve a dictionary 
-00008740: 7769 7468 2074 6865 2074 6167 6769 6e67  with the tagging
-00008750: 2071 7561 6c69 7479 2070 6572 2076 6964   quality per vid
-00008760: 656f 2c20 6173 2072 6570 6f72 7465 6420  eo, as reported 
-00008770: 6279 2044 4c43 2e72 ad00 0000 72ae 0000  by DLC.r....r...
-00008780: 0029 0372 da00 0000 7239 0100 0072 3001  .).r....r9...r0.
-00008790: 0000 7255 0000 0072 2600 0000 7226 0000  ..rU...r&...r&..
-000087a0: 0072 2700 0000 725e 0100 00c2 0400 0073  .r'...r^.......s
-000087b0: 0200 0000 0002 7a17 436f 6f72 6469 6e61  ......z.Coordina
-000087c0: 7465 732e 6765 745f 7175 616c 6974 7963  tes.get_qualityc
-000087d0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-000087e0: 0300 0000 4300 0000 7312 0000 007c 006a  ....C...s....|.j
-000087f0: 007c 006a 0167 017c 006a 0266 0353 0029  .|.j.g.|.j.f.S.)
-00008800: 017a 3d52 6574 7269 6576 6520 616c 6c20  .z=Retrieve all 
-00008810: 6176 6169 6c61 626c 6520 696e 666f 726d  available inform
-00008820: 6174 696f 6e20 6173 736f 6369 6174 6564  ation associated
-00008830: 2077 6974 6820 7468 6520 6172 656e 612e   with the arena.
-00008840: 2903 7231 0100 0072 3301 0000 723a 0100  ).r1...r3...r:..
-00008850: 0072 5500 0000 7226 0000 0072 2600 0000  .rU...r&...r&...
-00008860: 7227 0000 0072 8300 0000 c604 0000 7302  r'...r........s.
-00008870: 0000 0000 037a 1643 6f6f 7264 696e 6174  .....z.Coordinat
-00008880: 6573 2e67 6574 5f61 7265 6e61 7329 0372  es.get_arenas).r
-00008890: 5c00 0000 da0a 6172 656e 615f 7479 7065  \.....arena_type
-000088a0: 727f 0000 0063 0400 0000 0000 0000 0000  r....c..........
-000088b0: 0000 0d00 0000 0800 0000 4300 0000 7300  ..........C...s.
-000088c0: 0100 007c 0164 0175 0072 0e7c 006a 007d  ...|.d.u.r.|.j.}
-000088d0: 017c 0264 0175 0072 1c7c 006a 017d 0267  .|.d.u.r.|.j.}.g
-000088e0: 0067 0002 007d 047d 0574 027c 006a 0083  .g...}.}.t.|.j..
-000088f0: 0144 005d 2e5c 027d 067d 077c 0144 005d  .D.].\.}.}.|.D.]
-00008900: 207d 087c 087c 0776 0072 3c7c 04a0 037c   }.|.|.v.r<|...|
-00008910: 07a1 0101 007c 05a0 037c 06a1 0101 0071  .....|...|.....q
-00008920: 3c71 307c 0372 8874 0464 02a0 0574 067c  <q0|.r.t.d...t.|
-00008930: 0183 0174 067c 0183 0164 036b 0472 8064  ...t.|...d.k.r.d
-00008940: 046e 0264 05a1 0283 0101 0074 076a 086a  .n.d.......t.j.j
-00008950: 097c 027c 006a 0a7c 006a 0b7c 006a 0c7c  .|.|.j.|.j.|.j.|
-00008960: 006a 0d7c 0464 068d 065c 037d 097d 0a7d  .j.|.d...\.}.}.}
-00008970: 0b7c 0372 ba74 0464 0783 0101 0074 027c  .|.r.t.d.....t.|
-00008980: 0183 0144 005d 2c5c 027d 067d 0c7c 097c  ...D.],\.}.}.|.|
-00008990: 0619 007c 006a 0e7c 057c 0619 003c 007c  ...|.j.|.|...<.|
-000089a0: 0a7c 0619 007c 006a 0f7c 057c 0619 003c  .|...|.j.|.|...<
-000089b0: 0071 c27c 006a 1064 0864 098d 0101 0064  .q.|.j.d.d.....d
-000089c0: 0153 0029 0a61 b401 0000 5461 6720 7468  .S.).a....Tag th
-000089d0: 6520 6172 656e 6120 696e 2074 6865 2076  e arena in the v
-000089e0: 6964 656f 732e 0a0a 2020 2020 2020 2020  ideos...        
-000089f0: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-00008a00: 2020 7669 6465 6f73 2028 6c69 7374 293a    videos (list):
-00008a10: 2041 206c 6973 7420 6f66 2076 6964 656f   A list of video
-00008a20: 7320 746f 2072 6561 6e6e 6f74 6174 652e  s to reannotate.
-00008a30: 2049 6620 4e6f 6e65 2c20 616c 6c20 7669   If None, all vi
-00008a40: 6465 6f73 2061 7265 206c 6f61 6465 642e  deos are loaded.
-00008a50: 0a20 2020 2020 2020 2020 2020 2061 7265  .            are
-00008a60: 6e61 5f74 7970 6520 2873 7472 293a 2054  na_type (str): T
-00008a70: 6865 2074 7970 6520 6f66 2061 7265 6e61  he type of arena
-00008a80: 2074 6f20 7573 652e 204d 7573 7420 6265   to use. Must be
-00008a90: 206f 6e65 206f 6620 2270 6f6c 7967 6f6e   one of "polygon
-00008aa0: 616c 2d6d 616e 7561 6c22 2c20 2263 6972  al-manual", "cir
-00008ab0: 6375 6c61 722d 6d61 6e75 616c 222c 206f  cular-manual", o
-00008ac0: 7220 2263 6972 6375 6c61 722d 6175 746f  r "circular-auto
-00008ad0: 6465 7465 6374 222e 2049 6620 4e6f 6e65  detect". If None
-00008ae0: 2028 6465 6661 756c 7429 2c20 7468 6520   (default), the 
-00008af0: 6172 656e 6120 7479 7065 2073 7065 6369  arena type speci
-00008b00: 6669 6564 2077 6865 6e20 6372 6561 7469  fied when creati
-00008b10: 6e67 2074 6865 2070 726f 6a65 6374 2069  ng the project i
-00008b20: 7320 7573 6564 2e0a 2020 2020 2020 2020  s used..        
-00008b30: 2020 2020 7665 7262 6f73 6520 2862 6f6f      verbose (boo
-00008b40: 6c29 3a20 5768 6574 6865 7220 746f 2070  l): Whether to p
-00008b50: 7269 6e74 2074 6865 2070 726f 6772 6573  rint the progres
-00008b60: 7320 6f66 2074 6865 2061 6e6e 6f74 6174  s of the annotat
-00008b70: 696f 6e2e 0a0a 2020 2020 2020 2020 4e7a  ion...        Nz
-00008b80: 1245 6469 7469 6e67 207b 7d20 6172 656e  .Editing {} aren
-00008b90: 617b 7d72 3100 0000 da01 7372 2c00 0000  a{}r1.....sr,...
-00008ba0: 2906 7234 0000 0072 5f00 0000 7218 0000  ).r4...r_...r...
-00008bb0: 0072 3e00 0000 725d 0000 0072 5c00 0000  .r>...r]...r\...
-00008bc0: 721e 0100 0046 721c 0100 0029 1172 3d01  r....Fr....).r=.
-00008bd0: 0000 7231 0100 0072 f500 0000 72fc 0000  ..r1...r....r...
-00008be0: 0072 8000 0000 726c 0000 0072 5e00 0000  .r....rl...r^...
-00008bf0: 7281 0000 0072 8200 0000 7283 0000 0072  r....r....r....r
-00008c00: 3301 0000 7223 0000 0072 2f01 0000 723b  3...r#...r/...r;
-00008c10: 0100 0072 3a01 0000 7232 0100 0072 2301  ...r:...r2...r#.
-00008c20: 0000 290d 7256 0000 0072 5c00 0000 727d  ..).rV...r\...r}
-00008c30: 0100 0072 7f00 0000 da0e 7669 6465 6f73  ...r......videos
-00008c40: 5f72 656e 616d 6564 da08 7669 645f 6964  _renamed..vid_id
-00008c50: 6373 da07 7669 645f 6964 78da 0676 6964  cs..vid_idx..vid
-00008c60: 5f69 6eda 0776 6964 5f6f 7574 da0d 6564  _in..vid_out..ed
-00008c70: 6974 6564 5f73 6361 6c65 73da 1365 6469  ited_scales..edi
-00008c80: 7465 645f 6172 656e 615f 7061 7261 6d73  ted_arena_params
-00008c90: 728c 0000 0072 5300 0000 7226 0000 0072  r....rS...r&...r
-00008ca0: 2600 0000 7227 0000 00da 0b65 6469 745f  &...r'.....edit_
-00008cb0: 6172 656e 6173 cb04 0000 7338 0000 0000  arenas....s8....
-00008cc0: 0b08 0106 0108 0106 020a 0112 0108 0108  ................
-00008cd0: 010a 010e 0204 0102 011e ff04 0406 0102  ................
-00008ce0: 0104 0104 0104 0104 0102 fa0c 0904 0108  ................
-00008cf0: 0310 0112 0114 027a 1743 6f6f 7264 696e  .......z.Coordin
-00008d00: 6174 6573 2e65 6469 745f 6172 656e 6173  ates.edit_arenas
-00008d10: 2902 da08 6669 6c65 6e61 6d65 721d 0100  )...filenamer...
-00008d20: 0063 0300 0000 0000 0000 0000 0000 0500  .c..............
-00008d30: 0000 0900 0000 4300 0000 737e 0000 0064  ......C...s~...d
-00008d40: 01a0 0074 016a 02a0 037c 006a 047c 006a  ...t.j...|.j.|.j
-00008d50: 0564 027c 0164 0375 0172 207c 016e 0264  .d.|.d.u.r |.n.d
-00008d60: 04a1 047c 0272 3864 0574 0674 0783 0083  ...|.r8d.t.t....
-00008d70: 019b 009d 026e 0264 06a1 027d 0374 087c  .....n.d...}.t.|
-00008d80: 0364 0783 028f 227d 0474 096a 0a7c 007c  .d...."}.t.j.|.|
-00008d90: 0474 096a 0b64 088d 0301 0057 0064 0304  .t.j.d.....W.d..
-00008da0: 0004 0083 0301 006e 1031 0073 7030 0001  .......n.1.sp0..
-00008db0: 0001 0001 0059 0001 0064 0353 0029 0961  .....Y...d.S.).a
-00008dc0: 2601 0000 5361 7665 2074 6865 2063 7572  &...Save the cur
-00008dd0: 7265 6e74 2073 7461 7465 206f 6620 7468  rent state of th
-00008de0: 6520 436f 6f72 6469 6e61 7465 7320 6f62  e Coordinates ob
-00008df0: 6a65 6374 2074 6f20 6120 7069 636b 6c65  ject to a pickle
-00008e00: 6420 6669 6c65 2e0a 0a20 2020 2020 2020  d file...       
-00008e10: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
-00008e20: 2020 2066 696c 656e 616d 6520 2873 7472     filename (str
-00008e30: 293a 204e 616d 6520 6f66 2074 6865 2070  ): Name of the p
-00008e40: 6963 6b6c 6564 2066 696c 6520 746f 2073  ickled file to s
-00008e50: 746f 7265 2e20 4966 206e 6f20 6e61 6d65  tore. If no name
-00008e60: 2069 7320 7072 6f76 6964 6564 2c20 6120   is provided, a 
-00008e70: 6465 6661 756c 7420 6973 2075 7365 642e  default is used.
-00008e80: 0a20 2020 2020 2020 2020 2020 2074 696d  .            tim
-00008e90: 6573 7461 6d70 2028 626f 6f6c 293a 2057  estamp (bool): W
-00008ea0: 6865 7468 6572 2074 6f20 6170 7065 6e64  hether to append
-00008eb0: 2061 2074 696d 6520 7374 616d 7020 6174   a time stamp at
-00008ec0: 2074 6865 2065 6e64 206f 6620 7468 6520   the end of the 
-00008ed0: 6f75 7470 7574 2066 696c 6520 6e61 6d65  output file name
-00008ee0: 2e0a 2020 2020 2020 2020 7a08 7b7d 7b7d  ..        z.{}{}
-00008ef0: 2e70 6b6c 721a 0000 004e 7216 0000 0072  .pklr....Nr....r
-00008f00: 8c00 0000 722c 0000 00da 0277 6229 01da  ....r,.....wb)..
-00008f10: 0870 726f 746f 636f 6c29 0c72 6c00 0000  .protocol).rl...
-00008f20: 721d 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
-00008f30: 2300 0000 722f 0100 0072 1f01 0000 720d  #...r/...r....r.
-00008f40: 0000 0072 1c00 0000 7220 0000 00da 0464  ...r....r .....d
-00008f50: 756d 70da 1048 4947 4845 5354 5f50 524f  ump..HIGHEST_PRO
-00008f60: 544f 434f 4c29 0572 5600 0000 7287 0100  TOCOL).rV...r...
-00008f70: 0072 1d01 0000 da07 706b 6c5f 6f75 7472  .r......pkl_outr
-00008f80: 2400 0000 7226 0000 0072 2600 0000 7227  $...r&...r&...r'
-00008f90: 0000 0072 2301 0000 fa04 0000 7316 0000  ...r#.......s...
-00008fa0: 0000 0704 0106 0104 0104 0102 010e fc02  ................
-00008fb0: 0616 f904 0a0c 017a 1043 6f6f 7264 696e  .......z.Coordin
-00008fc0: 6174 6573 2e73 6176 6529 0772 0401 0000  ates.save).r....
-00008fd0: da14 7072 6563 6f6d 7075 7465 645f 7461  ..precomputed_ta
-00008fe0: 625f 6469 6374 7242 0100 0072 4301 0000  b_dictrB...rC...
-00008ff0: 7245 0100 00da 0a70 7265 7072 6f63 6573  rE.....preproces
-00009000: 7372 1900 0000 6307 0000 0000 0000 0000  sr....c.........
-00009010: 0000 001a 0000 0009 0000 000b 0000 0073  ...............s
-00009020: 9203 0000 8800 6a00 7c01 7c03 7c05 7c04  ......j.|.|.|.|.
-00009030: 6401 8d04 7d08 8800 6a00 7c01 6402 6403  d...}...j.|.d.d.
-00009040: 8d02 7d09 8800 6a01 7c01 6404 8d01 7d0a  ..}...j.|.d...}.
-00009050: 7c08 a002 7c09 7c0a a102 7d0b 7c02 6405  |...|.|...}.|.d.
-00009060: 7501 7244 7c02 7d0b 7403 6a04 6a05 7c01  u.rD|.}.t.j.j.|.
-00009070: 6405 7500 7258 8800 6a06 6e02 7c01 8800  d.u.rX..j.n.|...
-00009080: 6a06 6405 7501 728a 8800 6a06 6406 1900  j.d.u.r...j.d...
-00009090: 728a 7407 7408 8700 6601 6407 6408 8408  r.t.t...f.d.d...
-000090a0: 8800 6a09 4400 8301 8301 8301 6e04 8800  ..j.D.......n...
-000090b0: 6a09 8800 6a0a 6409 8d03 7d0c 7c0c 7c0b  j...j.d...}.|.|.
-000090c0: 5f0b 7407 7407 7c0a a00c a100 8301 6406  _.t.t.|.......d.
-000090d0: 1900 6a0d 8301 7d0d 740e a00f 640a 6408  ..j...}.t...d.d.
-000090e0: 8400 7407 7c0b a00c a100 8301 6406 1900  ..t.|.......d...
-000090f0: 6a0d 4400 8301 a101 7d0e 640b 6408 8400  j.D.....}.d.d...
-00009100: 7407 7c0c a010 a100 8301 4400 8301 640c  t.|.......D...d.
-00009110: 6408 8400 7407 7c0c a010 a100 8301 4400  d...t.|.......D.
-00009120: 8301 1700 7407 7c0c a010 a100 8301 1700  ....t.|.........
-00009130: 7d0f 6700 7d10 6700 7d11 7c0f 4400 5d2e  }.g.}.g.}.|.D.].
-00009140: 7d12 7411 7c0e 8301 4400 5d1e 5c02 7d13  }.t.|...D.].\.}.
-00009150: 7d14 7c12 7c14 6b02 9001 7226 7c10 a012  }.|.|.k...r&|...
-00009160: 7c13 a101 0100 9001 7126 9001 711a 6700  |.......q&..q.g.
-00009170: 7d15 640d 6408 8400 7407 7c0c 6a13 8301  }.d.d...t.|.j...
-00009180: 4400 8301 4400 5d5e 7d16 7411 7c0d 8301  D...D.]^}.t.|...
-00009190: 4400 5d1e 5c02 7d13 7d14 7c16 7c14 6b02  D.].\.}.}.|.|.k.
-000091a0: 9001 726e 7c11 a012 7c13 a101 0100 9001  ..rn|...|.......
-000091b0: 716e 7414 8800 6a06 8301 6402 6b04 9001  qnt...j...d.k...
-000091c0: 7262 7c15 a012 7414 7408 640e 6408 8400  rb|...t.t.d.d...
-000091d0: 7c16 4400 8301 8301 8301 6402 6b02 a101  |.D.......d.k...
-000091e0: 0100 9001 7162 7c06 9002 72ee 7c0b 6a15  ....qb|...r.|.j.
-000091f0: 6600 6900 7c07 a401 8e01 5c02 7d17 7d18  f.i.|.....\.}.}.
-00009200: 7c17 6406 1900 6405 6405 8502 6405 6405  |.d...d.d...d.d.
-00009210: 8502 7c0e a016 7c0d a101 0f00 6603 1900  ..|...|.....f...
-00009220: 6405 6405 8502 6405 6405 8502 7c10 6603  d.d...d.d...|.f.
-00009230: 1900 7c17 6406 1900 6405 6405 8502 6405  ..|.d...d.d...d.
-00009240: 6405 8502 7c0e a016 7c0d a101 6603 1900  d...|...|...f...
-00009250: 6405 6405 8502 6405 6405 8502 7c11 6603  d.d...d.d...|.f.
-00009260: 1900 7c17 6402 1900 6703 7d19 7a74 7c19  ..|.d...g.}.zt|.
-00009270: 7c17 640f 1900 6405 6405 8502 6405 6405  |.d...d.d...d.d.
-00009280: 8502 7c0e a016 7c0d a101 0f00 6603 1900  ..|...|.....f...
-00009290: 6405 6405 8502 6405 6405 8502 7c10 6603  d.d...d.d...|.f.
-000092a0: 1900 7c17 640f 1900 6405 6405 8502 6405  ..|.d...d.d...d.
-000092b0: 6405 8502 7c0e a016 7c0d a101 6603 1900  d...|...|...f...
-000092c0: 6405 6405 8502 6405 6405 8502 7c11 6603  d.d...d.d...|.f.
-000092d0: 1900 7c17 6410 1900 6703 3700 7d19 5700  ..|.d...g.7.}.W.
-000092e0: 6e2e 0400 7417 9002 79ea 0100 0100 0100  n...t...y.......
-000092f0: 7c19 7c17 640f 1900 7c17 640f 1900 7c17  |.|.d...|.d...|.
-00009300: 6410 1900 6703 3700 7d19 5900 6e02 3000  d...g.7.}.Y.n.0.
-00009310: 6e8a 7418 a019 7407 7c17 a00c a100 8301  n.t...t.|.......
-00009320: a101 7d17 7c17 6405 6405 8502 7c0e a016  ..}.|.d.d...|...
-00009330: 7c0d a101 0f00 6602 1900 6405 6405 8502  |.....f...d.d...
-00009340: 7c10 6602 1900 6a1a 7c17 6a1b 6406 1900  |.f...j.|.j.d...
-00009350: 7414 7c0c a010 a100 8301 6411 6703 6412  t.|.......d.g.d.
-00009360: 6413 8d02 7403 6a04 a01c 741d a01e 7c0c  d...t.j...t...|.
-00009370: a101 a01f a100 7c17 6405 6405 8502 7c0e  ......|.d.d...|.
-00009380: a016 7c0d a101 6602 1900 6405 6405 8502  ..|...f...d.d...
-00009390: 7c11 6602 1900 a102 6602 7d19 7420 7c19  |.f.....f.}.t |.
-000093a0: 8301 741d a021 7c0c a101 a01f a100 7c0b  ..t..!|.......|.
-000093b0: 7c18 6604 5300 2914 61ed 0300 0047 656e  |.f.S.).a....Gen
-000093c0: 6572 6174 6520 6120 6461 7461 7365 7420  erate a dataset 
-000093d0: 7769 7468 2061 6c6c 2073 7065 6369 6669  with all specifi
-000093e0: 6564 2066 6561 7475 7265 732e 0a0a 2020  ed features...  
-000093f0: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-00009400: 2020 2020 2020 2020 616e 696d 616c 5f69          animal_i
-00009410: 6420 2873 7472 293a 204e 616d 6520 6f66  d (str): Name of
-00009420: 2074 6865 2061 6e69 6d61 6c20 746f 2070   the animal to p
-00009430: 726f 6365 7373 2e20 4966 204e 6f6e 6520  rocess. If None 
-00009440: 2864 6566 6175 6c74 2920 616c 6c20 616e  (default) all an
-00009450: 696d 616c 7320 6172 6520 696e 636c 7564  imals are includ
-00009460: 6564 2069 6e20 6120 6d75 6c74 692d 616e  ed in a multi-an
-00009470: 696d 616c 2067 7261 7068 2e0a 2020 2020  imal graph..    
-00009480: 2020 2020 2020 2020 7072 6563 6f6d 7075          precompu
-00009490: 7465 645f 7461 625f 6469 6374 2028 7461  ted_tab_dict (ta
-000094a0: 626c 655f 6469 6374 293a 2074 6162 6c65  ble_dict): table
-000094b0: 5f64 6963 7420 6f62 6a65 6374 2066 6f72  _dict object for
-000094c0: 2066 7572 7468 6572 2067 7261 7068 2070   further graph p
-000094d0: 726f 6365 7373 696e 672e 204e 6f6e 6520  rocessing. None 
-000094e0: 2864 6566 6175 6c74 2920 6275 696c 6473  (default) builds
-000094f0: 2069 7420 6f6e 2074 6865 2073 706f 742e   it on the spot.
-00009500: 0a20 2020 2020 2020 2020 2020 2063 656e  .            cen
-00009510: 7465 7220 2873 7472 293a 204e 616d 6520  ter (str): Name 
-00009520: 6f66 2074 6865 2062 6f64 7920 7061 7274  of the body part
-00009530: 2074 6f20 7768 6963 6820 7468 6520 706f   to which the po
-00009540: 7369 7469 6f6e 7320 7769 6c6c 2062 6520  sitions will be 
-00009550: 6365 6e74 6572 6564 2e20 4966 2066 616c  centered. If fal
-00009560: 7365 2c20 7261 7720 6461 7461 2069 7320  se, raw data is 
-00009570: 7265 7475 726e 6564 3b20 6966 2027 6172  returned; if 'ar
-00009580: 656e 6127 2028 6465 6661 756c 7429 2c20  ena' (default), 
-00009590: 636f 6f72 6469 6e61 7465 7320 6172 6520  coordinates are 
-000095a0: 6365 6e74 6572 6564 206f 6e20 7468 6520  centered on the 
-000095b0: 7069 7463 682e 0a20 2020 2020 2020 2020  pitch..         
-000095c0: 2020 2070 6f6c 6172 2028 626f 6f6c 2920     polar (bool) 
-000095d0: 5374 6174 6573 2077 6865 7468 6572 2074  States whether t
-000095e0: 6865 2063 6f6f 7264 696e 6174 6573 2073  he coordinates s
-000095f0: 686f 756c 6420 6265 2063 6f6e 7665 7274  hould be convert
-00009600: 6564 2074 6f20 706f 6c61 7220 7661 6c75  ed to polar valu
-00009610: 6573 2e0a 2020 2020 2020 2020 2020 2020  es..            
-00009620: 616c 6967 6e20 2873 7472 293a 2053 656c  align (str): Sel
-00009630: 6563 7473 2074 6865 2062 6f64 7920 7061  ects the body pa
-00009640: 7274 2074 6f20 7768 6963 6820 6c61 7465  rt to which late
-00009650: 7220 7072 6f63 6573 7365 7320 7769 6c6c  r processes will
-00009660: 2061 6c69 676e 2074 6865 2066 7261 6d65   align the frame
-00009670: 7320 7769 7468 2028 7365 6520 7072 6570  s with (see prep
-00009680: 726f 6365 7373 2069 6e20 7461 626c 655f  rocess in table_
-00009690: 6469 6374 2064 6f63 756d 656e 7461 7469  dict documentati
-000096a0: 6f6e 292e 0a20 2020 2020 2020 2020 2020  on)..           
-000096b0: 2070 7265 7072 6f63 6573 7320 2862 6f6f   preprocess (boo
-000096c0: 6c29 3a20 7768 6574 6865 7220 746f 2070  l): whether to p
-000096d0: 7265 7072 6f63 6573 7320 7468 6520 6461  reprocess the da
-000096e0: 7461 2074 6f20 7061 7373 2074 6f20 6175  ta to pass to au
-000096f0: 746f 656e 636f 6465 7273 2e20 4966 2046  toencoders. If F
-00009700: 616c 7365 2c20 6e6f 6465 2066 6561 7475  alse, node featu
-00009710: 7265 7320 616e 6420 6469 7374 616e 6365  res and distance
-00009720: 2d77 6569 6768 7465 6420 6164 6a61 6365  -weighted adjace
-00009730: 6e63 7920 6d61 7472 6963 6573 206f 6e20  ncy matrices on 
-00009740: 7468 6520 7261 7720 6461 7461 2061 7265  the raw data are
-00009750: 2072 6574 7572 6e65 642e 0a0a 2020 2020   returned...    
-00009760: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-00009770: 2020 2020 2020 2020 206d 6572 6765 645f           merged_
-00009780: 6665 6174 7572 6573 3a20 4120 6772 6170  features: A grap
-00009790: 682d 6261 7365 6420 6461 7461 7365 742e  h-based dataset.
-000097a0: 0a0a 2020 2020 2020 2020 2904 7247 0100  ..        ).rG..
-000097b0: 0072 4201 0000 7245 0100 0072 4301 0000  .rB...rE...rC...
-000097c0: 7231 0000 0029 0272 4701 0000 7244 0100  r1...).rG...rD..
-000097d0: 0029 0172 4701 0000 4e72 0100 0000 6301  .).rG...Nr....c.
-000097e0: 0000 0000 0000 0000 0000 0002 0000 000a  ................
-000097f0: 0000 0013 0000 0073 3400 0000 6700 7c00  .......s4...g.|.
-00009800: 5d2c 7d01 7400 a001 6400 a002 7403 7400  ],}.t...d...t.t.
-00009810: 6a04 6401 6402 8400 8800 6a05 4400 8301  j.d.d.....j.D...
-00009820: 8302 a101 6403 7c01 a103 9102 7104 5300  ....d.|.....q.S.
-00009830: 2904 da01 7c63 0100 0000 0000 0000 0000  )...|c..........
-00009840: 0000 0200 0000 0400 0000 5300 0000 7314  ..........S...s.
-00009850: 0000 0067 007c 005d 0c7d 017c 0164 0017  ...g.|.].}.|.d..
-00009860: 0091 0271 0453 0072 9900 0000 7226 0000  ...q.S.r....r&..
-00009870: 0072 4900 0000 7226 0000 0072 2600 0000  .rI...r&...r&...
-00009880: 7227 0000 0072 4c00 0000 3c05 0000 724d  r'...rL...<...rM
-00009890: 0000 007a 3c43 6f6f 7264 696e 6174 6573  ...z<Coordinates
-000098a0: 2e67 6574 5f67 7261 7068 5f64 6174 6173  .get_graph_datas
-000098b0: 6574 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  et.<locals>.<lis
-000098c0: 7463 6f6d 703e 2e3c 6c69 7374 636f 6d70  tcomp>.<listcomp
-000098d0: 3e72 2c00 0000 2906 72c5 0000 00da 0373  >r,...).r......s
-000098e0: 7562 721f 0000 0072 d500 0000 da06 6573  ubr....r......es
-000098f0: 6361 7065 7230 0100 0072 4c01 0000 7255  caper0...rL...rU
-00009900: 0000 0072 2600 0000 7227 0000 0072 4c00  ...r&...r'...rL.
-00009910: 0000 3905 0000 7310 0000 0006 0802 f904  ..9...s.........
-00009920: 0104 0116 ff02 0302 0102 fb7a 3143 6f6f  ...........z1Coo
-00009930: 7264 696e 6174 6573 2e67 6574 5f67 7261  rdinates.get_gra
-00009940: 7068 5f64 6174 6173 6574 2e3c 6c6f 6361  ph_dataset.<loca
-00009950: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 2903  ls>.<listcomp>).
-00009960: 7233 0000 0072 3700 0000 7293 0000 0063  r3...r7...r....c
-00009970: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00009980: 0300 0000 5300 0000 7310 0000 0067 007c  ....S...s....g.|
-00009990: 005d 087d 017c 0191 0271 0453 0072 2600  .].}.|...q.S.r&.
-000099a0: 0000 7226 0000 0072 4900 0000 7226 0000  ..r&...rI...r&..
-000099b0: 0072 2600 0000 7227 0000 0072 4c00 0000  .r&...r'...rL...
-000099c0: 4d05 0000 724d 0000 0063 0100 0000 0000  M...rM...c......
-000099d0: 0000 0000 0000 0200 0000 0400 0000 5300  ..............S.
-000099e0: 0000 7314 0000 0067 007c 005d 0c7d 017c  ..s....g.|.].}.|
-000099f0: 0164 0066 0291 0271 0453 0072 0601 0000  .d.f...q.S.r....
-00009a00: 7226 0000 0072 4900 0000 7226 0000 0072  r&...rI...r&...r
-00009a10: 2600 0000 7227 0000 0072 4c00 0000 4f05  &...r'...rL...O.
-00009a20: 0000 724d 0000 0063 0100 0000 0000 0000  ..rM...c........
-00009a30: 0000 0000 0200 0000 0400 0000 5300 0000  ............S...
-00009a40: 7314 0000 0067 007c 005d 0c7d 017c 0164  s....g.|.].}.|.d
-00009a50: 0066 0291 0271 0453 0029 0172 a900 0000  .f...q.S.).r....
-00009a60: 7226 0000 0072 4900 0000 7226 0000 0072  r&...rI...r&...r
-00009a70: 2600 0000 7227 0000 0072 4c00 0000 5005  &...r'...rL...P.
-00009a80: 0000 724d 0000 0063 0100 0000 0000 0000  ..rM...c........
-00009a90: 0000 0000 0200 0000 0500 0000 5300 0000  ............S...
-00009aa0: 7318 0000 0067 007c 005d 107d 0174 0074  s....g.|.].}.t.t
-00009ab0: 017c 0183 0183 0191 0271 0453 0072 2600  .|.......q.S.r&.
-00009ac0: 0000 726e 0100 0072 6f01 0000 7226 0000  ..rn...ro...r&..
-00009ad0: 0072 2600 0000 7227 0000 0072 4c00 0000  .r&...r'...rL...
-00009ae0: 5d05 0000 724d 0000 0063 0100 0000 0000  ]...rM...c......
-00009af0: 0000 0000 0000 0200 0000 0500 0000 5300  ..............S.
-00009b00: 0000 731a 0000 0067 007c 005d 127d 017c  ..s....g.|.].}.|
-00009b10: 01a0 0064 00a1 0164 0119 0091 0271 0453  ...d...d.....q.S
-00009b20: 0029 0272 8c00 0000 7201 0000 0029 0172  .).r....r....).r
-00009b30: 2200 0000 2902 724a 0000 00da 046e 6f64  "...).rJ.....nod
-00009b40: 6572 2600 0000 7226 0000 0072 2700 0000  er&...r&...r'...
-00009b50: 724c 0000 0064 0500 0072 4d00 0000 7292  rL...d...rM...r.
-00009b60: 0000 0072 2e00 0000 e9ff ffff ffda 0146  ...r...........F
-00009b70: 2901 da05 6f72 6465 7229 2272 6a01 0000  )...order)"rj...
-00009b80: 72f8 0000 00da 056d 6572 6765 7281 0000  r......merger...
-00009b90: 0072 8200 0000 7294 0000 0072 3001 0000  .r....r....r0...
-00009ba0: 72b5 0000 0072 b600 0000 7235 0100 0072  r....r....r5...r
-00009bb0: 3401 0000 7240 0100 0072 c800 0000 72b7  4...r@...r....r.
-00009bc0: 0000 0072 be00 0000 da05 496e 6465 7872  ...r......Indexr
-00009bd0: f200 0000 72f5 0000 0072 fc00 0000 7272  ....r....r....rr
-00009be0: 0100 0072 5e00 0000 728e 0100 00da 0469  ...r^...r......i
-00009bf0: 7369 6e72 c700 0000 72dd 0000 00da 0b63  sinr....r......c
-00009c00: 6f6e 6361 7465 6e61 7465 72fb 0000 0072  oncatenater....r
-00009c10: d400 0000 da14 6564 6765 735f 746f 5f77  ......edges_to_w
-00009c20: 6569 7468 6564 5f61 646a da02 6e78 da0a  eithed_adj..nx..
-00009c30: 6164 6a5f 6d61 7472 6978 da07 746f 6465  adj_matrix..tode
-00009c40: 6e73 6572 d100 0000 da10 6164 6a61 6365  nser......adjace
-00009c50: 6e63 795f 6d61 7472 6978 291a 7256 0000  ncy_matrix).rV..
-00009c60: 0072 0401 0000 728d 0100 0072 4201 0000  .r....r....rB...
-00009c70: 7243 0100 0072 4501 0000 728e 0100 00da  rC...rE...r.....
-00009c80: 066b 7761 7267 7372 a600 0000 da06 7370  .kwargsr......sp
-00009c90: 6565 6473 726c 0100 0072 e200 0000 da05  eedsrl...r......
-00009ca0: 6772 6170 68da 1265 6467 655f 6665 6174  graph..edge_feat
-00009cb0: 7572 655f 6e61 6d65 73da 0d66 6561 7475  ure_names..featu
-00009cc0: 7265 5f6e 616d 6573 da12 6e6f 6465 5f66  re_names..node_f
-00009cd0: 6561 7475 7265 5f6e 616d 6573 da14 6e6f  eature_names..no
-00009ce0: 6465 5f73 6f72 7469 6e67 5f69 6e64 6963  de_sorting_indic
-00009cf0: 6573 da14 6564 6765 5f73 6f72 7469 6e67  es..edge_sorting
-00009d00: 5f69 6e64 6963 6573 da01 6e72 b400 0000  _indices..nr....
-00009d10: da01 66da 1469 6e6e 6572 5f6c 696e 6b5f  ..f..inner_link_
-00009d20: 626f 6f6c 5f6d 6173 6b72 7001 0000 da0d  bool_maskrp.....
-00009d30: 746f 5f70 7265 7072 6f63 6573 73da 0d67  to_preprocess..g
-00009d40: 6c6f 6261 6c5f 7363 616c 6572 da07 6461  lobal_scaler..da
-00009d50: 7461 7365 7472 2600 0000 7255 0000 0072  tasetr&...rU...r
-00009d60: 2700 0000 da11 6765 745f 6772 6170 685f  '.....get_graph_
-00009d70: 6461 7461 7365 740e 0500 0073 ae00 0000  dataset....s....
-00009d80: 0019 0401 08ff 0603 0e01 0c03 0c02 0801  ................
-00009d90: 0403 0601 1010 08f2 020e 08f2 0401 0201  ................
-00009da0: 0a08 04f8 04ff 02ff 040f 0402 04ec 0617  ................
-00009db0: 0601 1601 2202 1401 14ff 0202 0afe 02ff  ...."...........
-00009dc0: 0207 0401 0401 0801 1001 0a01 1202 0401  ................
-00009dd0: 1801 1001 0a01 0e02 1001 0401 18ff 0805  ................
-00009de0: 0601 1402 2001 10ff 0203 1e01 10ff 0203  .... ...........
-00009df0: 06f9 0409 0201 0201 2001 10ff 0203 1e01  ........ .......
-00009e00: 10ff 0203 06f9 0a09 0e01 2203 1204 1601  ..........".....
-00009e10: 0aff 0402 18fe 0403 0601 0c01 1401 0aff  ................
-00009e20: 02fe 02fc 040d 0601 0c01 0201 02fc 7a1d  ..............z.
-00009e30: 436f 6f72 6469 6e61 7465 732e 6765 745f  Coordinates.get_
-00009e40: 6772 6170 685f 6461 7461 7365 7472 3100  graph_datasetr1.
-00009e50: 0000 2907 da06 7061 7261 6d73 da0c 7669  ..)...params..vi
-00009e60: 6465 6f5f 6f75 7470 7574 da0b 6672 616d  deo_output..fram
-00009e70: 655f 6c69 6d69 74da 0564 6562 7567 da06  e_limit..debug..
-00009e80: 6e5f 6a6f 6273 7248 0100 0072 1900 0000  n_jobsrH...r....
-00009e90: 6307 0000 0000 0000 0000 0000 0013 0000  c...............
-00009ea0: 000c 0000 0003 0000 0073 dc01 0000 6900  .........s....i.
-00009eb0: 7d07 7400 6a01 a002 7c01 a101 7d01 8801  }.t.j...|...}...
-00009ec0: 6a03 6401 6402 8d01 7d08 7a12 8801 6a03  j.d.d...}.z...j.
-00009ed0: 6403 6404 6405 8d02 7d09 5700 6e20 0400  d.d.d...}.W.n ..
-00009ee0: 7404 794e 0100 0100 0100 8801 6a03 6403  t.yN........j.d.
-00009ef0: 6406 6405 8d02 7d09 5900 6e02 3000 8801  d.d...}.Y.n.0...
-00009f00: a005 a100 7d0a 8801 6a03 6407 6408 8d01  ....}...j.d.d...
-00009f10: 7d0b 7406 8801 6a07 8301 6407 6b01 7284  }.t...j...d.k.r.
-00009f20: 7400 6a08 6a09 8801 6409 640a 8d02 7d0c  t.j.j...d.d...}.
-00009f30: 6e14 8701 6601 640b 640c 8408 8801 6a07  n...f.d.d.....j.
-00009f40: 4400 8301 7d0c 740a 8801 6a0b a00c a100  D...}.t...j.....
-00009f50: 8301 4400 5d50 8900 7c08 8800 1900 6a0d  ..D.]P..|.....j.
-00009f60: 7d0d 7400 6a01 6a0e 8801 7c08 7c09 7c0a  }.t.j.j...|.|.|.
-00009f70: 7c0c 7c0b 8700 6601 640d 640e 8408 8801  |.|...f.d.d.....
-00009f80: 6a0f 4400 8301 640f 1900 8801 6a10 7c01  j.D...d.....j.|.
-00009f90: 6410 8d09 7d0e 7c0d 7c0e 5f0d 7c0e 7c07  d...}.|.|._.|.|.
-00009fa0: 8800 3c00 71a6 7c06 9001 7220 7c07 a011  ..<.q.|...r |...
-00009fb0: a100 4400 5d18 5c02 8900 7d0f 8801 6a12  ..D.].\...}...j.
-00009fc0: 8800 1900 7c0f 6411 3c00 9001 7106 7c02  ....|.d.<...q.|.
-00009fd0: 9001 7240 7400 6a01 6a13 8801 7c07 7c02  ..r@t.j.j...|.|.
-00009fe0: 7c03 7c04 7c05 7c01 6412 8d07 0100 7400  |.|.|.|.d.....t.
-00009ff0: 6a14 6a15 8801 7c07 8801 a016 a100 8801  j.j...|.........
-0000a000: 6a07 6413 6701 1700 6414 8d04 7d07 7400  j.d.g...d...}.t.
-0000a010: 6a14 a017 8801 a016 a100 a101 7d10 7c07  j...........}.|.
-0000a020: 4400 5d44 7d11 8801 6a07 4400 5d36 7d12  D.]D}...j.D.]6}.
-0000a030: 6407 7c10 7c11 1900 7c12 1900 6a18 1800  d.|.|...|...j...
-0000a040: 7c07 7c11 1900 6415 a019 7c12 9001 72ac  |.|...d...|...r.
-0000a050: 6416 a019 7c12 a101 6e02 6417 a101 3c00  d...|...n.d...<.
-0000a060: 9001 717e 9001 7174 741a 7c07 6413 8801  ..q~..qtt.|.d...
-0000a070: 6a07 8801 6a1b 8801 6a1c 8801 6a1d 8801  j...j...j...j...
-0000a080: 6a12 7c06 6418 8d08 5300 2919 61e3 0300  j.|.d...S.).a...
-0000a090: 0041 6e6e 6f74 6174 6573 2063 6f6f 7264  .Annotates coord
-0000a0a0: 696e 6174 6573 2077 6974 6820 6265 6861  inates with beha
-0000a0b0: 7669 6f72 616c 2074 7261 6974 7320 7573  vioral traits us
-0000a0c0: 696e 6720 6120 7375 7065 7276 6973 6564  ing a supervised
-0000a0d0: 2070 6970 656c 696e 652e 0a0a 2020 2020   pipeline...    
-0000a0e0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-0000a0f0: 2020 2020 2020 7061 7261 6d73 2028 4469        params (Di
-0000a100: 6374 293a 2041 2064 6963 7469 6f6e 6172  ct): A dictionar
-0000a110: 7920 7769 7468 2074 6865 2070 6172 616d  y with the param
-0000a120: 6574 6572 7320 746f 2075 7365 2066 6f72  eters to use for
-0000a130: 2074 6865 2070 6970 656c 696e 652e 2049   the pipeline. I
-0000a140: 6620 756e 7375 7265 2c20 6c65 6176 6520  f unsure, leave 
-0000a150: 656d 7074 792e 0a20 2020 2020 2020 2020  empty..         
-0000a160: 2020 2076 6964 656f 5f6f 7574 7075 7420     video_output 
-0000a170: 2862 6f6f 6c29 3a20 4974 206f 7574 7075  (bool): It outpu
-0000a180: 7473 2061 2066 756c 6c79 2061 6e6e 6f74  ts a fully annot
-0000a190: 6174 6564 2076 6964 656f 2066 6f72 2065  ated video for e
-0000a1a0: 6163 6820 6578 7065 7269 6d65 6e74 2069  ach experiment i
-0000a1b0: 6e64 6963 6174 6564 2069 6e20 6120 6c69  ndicated in a li
-0000a1c0: 7374 2e20 4966 2073 6574 2074 6f20 2261  st. If set to "a
-0000a1d0: 6c6c 222c 2069 7420 7769 6c6c 206f 7574  ll", it will out
-0000a1e0: 7075 7420 616c 6c20 7669 6465 6f73 2e20  put all videos. 
-0000a1f0: 4661 6c73 6520 6279 2064 6566 6175 6c74  False by default
-0000a200: 2e0a 2020 2020 2020 2020 2020 2020 6672  ..            fr
-0000a210: 616d 655f 6c69 6d69 7420 2869 6e74 293a  ame_limit (int):
-0000a220: 204f 6e6c 7920 6170 706c 6965 7320 6966   Only applies if
-0000a230: 2076 6964 656f 5f6f 7574 7075 7420 6973   video_output is
-0000a240: 206e 6f74 2046 616c 7365 2e20 496e 6469   not False. Indi
-0000a250: 6361 7465 7320 7468 6520 6d61 7869 6d75  cates the maximu
-0000a260: 6d20 6e75 6d62 6572 206f 6620 6672 616d  m number of fram
-0000a270: 6573 2070 6572 2076 6964 656f 2074 6f20  es per video to 
-0000a280: 6f75 7470 7574 2e0a 2020 2020 2020 2020  output..        
-0000a290: 2020 2020 6465 6275 6720 2862 6f6f 6c29      debug (bool)
-0000a2a0: 3a20 4f6e 6c79 2061 7070 6c69 6573 2069  : Only applies i
-0000a2b0: 6620 7669 6465 6f5f 6f75 7470 7574 2069  f video_output i
-0000a2c0: 7320 6e6f 7420 4661 6c73 652e 2049 6620  s not False. If 
-0000a2d0: 5472 7565 2c20 616c 6c20 7669 6465 6f73  True, all videos
-0000a2e0: 2077 696c 6c20 696e 636c 7564 6520 6465   will include de
-0000a2f0: 6275 6720 696e 666f 726d 6174 696f 6e2c  bug information,
-0000a300: 2073 7563 6820 6173 2074 6865 2064 6574   such as the det
-0000a310: 6563 7465 6420 6172 656e 6120 616e 6420  ected arena and 
-0000a320: 7468 6520 7072 6570 726f 6365 7373 6564  the preprocessed
-0000a330: 2074 7261 636b 696e 6720 7461 6773 2e0a   tracking tags..
-0000a340: 2020 2020 2020 2020 2020 2020 6e5f 6a6f              n_jo
-0000a350: 6273 2028 696e 7429 3a20 4e75 6d62 6572  bs (int): Number
-0000a360: 206f 6620 6a6f 6273 2074 6f20 7573 6520   of jobs to use 
-0000a370: 666f 7220 7061 7261 6c6c 656c 2070 726f  for parallel pro
-0000a380: 6365 7373 696e 672e 0a20 2020 2020 2020  cessing..       
-0000a390: 2020 2020 2070 726f 7061 6761 7465 5f6c       propagate_l
-0000a3a0: 6162 656c 7320 2862 6f6f 6c29 3a20 4966  abels (bool): If
-0000a3b0: 2054 7275 652c 2074 6865 2070 6865 6e6f   True, the pheno
-0000a3c0: 2063 6f6c 756d 6e20 7769 6c6c 2062 6520   column will be 
-0000a3d0: 7072 6f70 6167 6174 6564 2066 726f 6d20  propagated from 
-0000a3e0: 7468 6520 6f72 6967 696e 616c 2064 6174  the original dat
-0000a3f0: 612e 0a0a 2020 2020 2020 2020 5265 7475  a...        Retu
-0000a400: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
-0000a410: 2074 6162 6c65 5f64 6963 743a 2041 2074   table_dict: A t
-0000a420: 6162 6c65 5f64 6963 7420 6f62 6a65 6374  able_dict object
-0000a430: 2077 6974 6820 616c 6c20 7375 7065 7276   with all superv
-0000a440: 6973 6564 2061 6e6e 6f74 6174 696f 6e73  ised annotations
-0000a450: 2070 6572 2065 7870 6572 696d 656e 7420   per experiment 
-0000a460: 6173 2076 616c 7565 732e 0a0a 2020 2020  as values...    
-0000a470: 2020 2020 4e72 4d01 0000 da06 4365 6e74      NrM.....Cent
-0000a480: 6572 da07 5370 696e 655f 3129 0272 4201  er..Spine_1).rB.
-0000a490: 0000 7245 0100 00da 044e 6f73 6572 3100  ..rE.....Noser1.
-0000a4a0: 0000 2901 7244 0100 0046 2901 da0e 696e  ..).rD...F)...in
-0000a4b0: 636c 7564 655f 616e 676c 6573 6301 0000  clude_anglesc...
-0000a4c0: 0000 0000 0000 0000 0002 0000 0008 0000  ................
-0000a4d0: 0013 0000 0073 2000 0000 6900 7c00 5d18  .....s ...i.|.].
-0000a4e0: 7d01 7c01 7400 6a01 6a02 8800 7c01 6400  }.|.t.j.j...|.d.
-0000a4f0: 6401 8d03 9302 7104 5300 2902 4629 0272  d.....q.S.).F).r
-0000a500: 0401 0000 72b6 0100 0029 0372 8100 0000  ....r....).r....
-0000a510: da08 706f 7374 5f68 6f63 da30 616c 6967  ..post_hoc.0alig
-0000a520: 6e5f 6465 6570 6f66 5f6b 696e 656d 6174  n_deepof_kinemat
-0000a530: 6963 735f 7769 7468 5f75 6e73 7570 6572  ics_with_unsuper
-0000a540: 7669 7365 645f 6c61 6265 6c73 2902 724a  vised_labels).rJ
-0000a550: 0000 00da 035f 6964 7255 0000 0072 2600  ....._idrU...r&.
-0000a560: 0000 7227 0000 0072 9700 0000 c105 0000  ..r'...r........
-0000a570: 7308 0000 0006 0402 fd08 0106 ff7a 3543  s............z5C
-0000a580: 6f6f 7264 696e 6174 6573 2e73 7570 6572  oordinates.super
-0000a590: 7669 7365 645f 616e 6e6f 7461 7469 6f6e  vised_annotation
-0000a5a0: 2e3c 6c6f 6361 6c73 3e2e 3c64 6963 7463  .<locals>.<dictc
-0000a5b0: 6f6d 703e 6301 0000 0000 0000 0000 0000  omp>c...........
-0000a5c0: 0002 0000 0003 0000 0013 0000 0073 1400  .............s..
-0000a5d0: 0000 6700 7c00 5d0c 7d01 8800 7204 7c01  ..g.|.].}...r.|.
-0000a5e0: 9102 7104 5300 7226 0000 0072 2600 0000  ..q.S.r&...r&...
-0000a5f0: 7252 0000 0029 0172 e400 0000 7226 0000  rR...).r....r&..
-0000a600: 0072 2700 0000 724c 0000 00d4 0500 0072  .r'...rL.......r
-0000a610: 4d00 0000 7a35 436f 6f72 6469 6e61 7465  M...z5Coordinate
-0000a620: 732e 7375 7065 7276 6973 6564 5f61 6e6e  s.supervised_ann
-0000a630: 6f74 6174 696f 6e2e 3c6c 6f63 616c 733e  otation.<locals>
-0000a640: 2e3c 6c69 7374 636f 6d70 3e72 0100 0000  .<listcomp>r....
-0000a650: 2908 da0a 7261 775f 636f 6f72 6473 72a6  )...raw_coordsr.
-0000a660: 0000 0072 6c01 0000 da0d 6675 6c6c 5f66  ...rl.....full_f
-0000a670: 6561 7475 7265 7372 a001 0000 da05 7669  eaturesr......vi
-0000a680: 6465 6f72 1a01 0000 72ae 0100 0072 5001  deor....r....rP.
-0000a690: 0000 2905 72af 0100 0072 b001 0000 72b1  ..).r....r....r.
-0000a6a0: 0100 0072 b201 0000 72ae 0100 00da 0a73  ...r....r......s
-0000a6b0: 7570 6572 7669 7365 6429 0172 3300 0000  upervised).r3...
-0000a6c0: 7a09 7b7d 6d69 7373 696e 677a 037b 7d5f  z.{}missingz.{}_
-0000a6d0: 722c 0000 0029 0772 af00 0000 7233 0000  r,...).r....r3..
-0000a6e0: 0072 3400 0000 725f 0000 0072 6300 0000  .r4...r_...rc...
-0000a6f0: 7238 0000 0072 4801 0000 291e 7281 0000  r8...rH...).r...
-0000a700: 00da 1061 6e6e 6f74 6174 696f 6e5f 7574  ...annotation_ut
-0000a710: 696c 73da 0f67 6574 5f68 7061 7261 6d65  ils..get_hparame
-0000a720: 7465 7273 726a 0100 00da 0e41 7373 6572  tersrj.....Asser
-0000a730: 7469 6f6e 4572 726f 7272 f800 0000 725e  tionErrorr....r^
-0000a740: 0000 0072 3001 0000 72b7 0100 0072 b801  ...r0...r....r..
-0000a750: 0000 720e 0000 0072 3b01 0000 72f4 0000  ..r....r;...r...
-0000a760: 0072 c900 0000 da12 7375 7065 7276 6973  .r......supervis
-0000a770: 6564 5f74 6167 6769 6e67 723d 0100 0072  ed_taggingr=...r
-0000a780: 3c01 0000 72cb 0000 0072 3601 0000 da13  <...r....r6.....
-0000a790: 7461 6767 6564 5f76 6964 656f 5f6f 7574  tagged_video_out
-0000a7a0: 7075 7472 8200 0000 72e1 0000 0072 5e01  putr....r....r^.
-0000a7b0: 0000 da1c 636f 6d70 7574 655f 616e 696d  ....compute_anim
-0000a7c0: 616c 5f70 7265 7365 6e63 655f 6d61 736b  al_presence_mask
-0000a7d0: 72c8 0000 0072 6c00 0000 72da 0000 0072  r....rl...r....r
-0000a7e0: 3101 0000 7233 0100 0072 4001 0000 2913  1...r3...r@...).
-0000a7f0: 7256 0000 0072 ae01 0000 72af 0100 0072  rV...r....r....r
-0000a800: b001 0000 72b1 0100 0072 b201 0000 7248  ....r....r....rH
-0000a810: 0100 00da 0874 6167 5f64 6963 7472 ba01  .....tag_dictr..
-0000a820: 0000 72a6 0000 0072 6c01 0000 72a0 0100  ..r....rl...r...
-0000a830: 00da 0d66 6561 7475 7265 735f 6469 6374  ...features_dict
-0000a840: da09 7461 675f 696e 6465 78da 0f73 7570  ..tag_index..sup
-0000a850: 6572 7669 7365 645f 7461 6773 7254 0000  ervised_tagsrT..
-0000a860: 00da 0e70 7265 7365 6e63 655f 6d61 736b  ...presence_mask
-0000a870: 73da 0374 6167 da06 616e 696d 616c 7226  s..tag..animalr&
-0000a880: 0000 0029 0272 e400 0000 7256 0000 0072  ...).r....rV...r
-0000a890: 2700 0000 da15 7375 7065 7276 6973 6564  '.....supervised
-0000a8a0: 5f61 6e6e 6f74 6174 696f 6e98 0500 0073  _annotation....s
-0000a8b0: 8800 0000 0017 0401 0c01 0c02 0201 1201  ................
-0000a8c0: 0c01 1402 0801 0c01 0e02 0601 04ff 04ff  ................
-0000a8d0: 0406 0a04 04fc 0608 1203 0a01 0601 0201  ................
-0000a8e0: 0201 0201 0201 0201 0201 1601 0401 02f7  ................
-0000a8f0: 060b 0601 0a02 0601 1001 1202 0602 0601  ................
-0000a900: 0201 0201 0201 0201 0201 0201 02f9 060b  ................
-0000a910: 0601 0201 0201 0601 0afc 0608 1001 0801  ................
-0000a920: 0a03 10fe 0601 18ff 0a04 0201 0201 0201  ................
-0000a930: 0401 0401 0401 0401 0401 02f8 7a21 436f  ............z!Co
-0000a940: 6f72 6469 6e61 7465 732e 7375 7065 7276  ordinates.superv
-0000a950: 6973 6564 5f61 6e6e 6f74 6174 696f 6eda  ised_annotation.
-0000a960: 0456 6144 45da 0972 6563 7572 7265 6e74  .VaDE..recurrent
-0000a970: e940 0000 00e9 0400 0000 e996 0000 00e9  .@..............
-0000a980: 0a00 0000 72ac 0000 00e7 9a99 9999 9999  ....r...........
-0000a990: b93f da06 636f 7369 6e65 da03 6e63 65da  .?..cosine..nce.
-0000a9a0: 066c 696e 6561 7272 b000 0000 291c da13  .linearr....)...
-0000a9b0: 7072 6570 726f 6365 7373 6564 5f6f 626a  preprocessed_obj
-0000a9c0: 6563 7472 9e01 0000 da0f 656d 6265 6464  ectr......embedd
-0000a9d0: 696e 675f 6d6f 6465 6cda 0c65 6e63 6f64  ing_model..encod
-0000a9e0: 6572 5f74 7970 65da 0a62 6174 6368 5f73  er_type..batch_s
-0000a9f0: 697a 65da 0a6c 6174 656e 745f 6469 6dda  ize..latent_dim.
-0000aa00: 0665 706f 6368 73da 0b6c 6f67 5f68 6973  .epochs..log_his
-0000aa10: 746f 7279 da0b 6c6f 675f 6870 6172 616d  tory..log_hparam
-0000aa20: 73da 0c6e 5f63 6f6d 706f 6e65 6e74 73da  s..n_components.
-0000aa30: 0b6b 6d65 616e 735f 6c6f 7373 da0b 7465  .kmeans_loss..te
-0000aa40: 6d70 6572 6174 7572 65da 1f63 6f6e 7472  mperature..contr
-0000aa50: 6173 7469 7665 5f73 696d 696c 6172 6974  astive_similarit
-0000aa60: 795f 6675 6e63 7469 6f6e da19 636f 6e74  y_function..cont
-0000aa70: 7261 7374 6976 655f 6c6f 7373 5f66 756e  rastive_loss_fun
-0000aa80: 6374 696f 6eda 0462 6574 61da 0374 6175  ction..beta..tau
-0000aa90: da0b 6f75 7470 7574 5f70 6174 68da 0a70  ..output_path..p
-0000aaa0: 7265 7472 6169 6e65 64da 1073 6176 655f  retrained..save_
-0000aab0: 6368 6563 6b70 6f69 6e74 73da 0c73 6176  checkpoints..sav
-0000aac0: 655f 7765 6967 6874 73da 0a69 6e70 7574  e_weights..input
-0000aad0: 5f74 7970 65da 0372 756e da11 6b6c 5f61  _type..run..kl_a
-0000aae0: 6e6e 6561 6c69 6e67 5f6d 6f64 65da 096b  nnealing_mode..k
-0000aaf0: 6c5f 7761 726d 7570 da10 7265 675f 6361  l_warmup..reg_ca
-0000ab00: 745f 636c 7573 7465 7273 da09 7265 636c  t_clusters..recl
-0000ab10: 7573 7465 72da 1a69 6e74 6572 6163 7469  uster..interacti
-0000ab20: 6f6e 5f72 6567 756c 6172 697a 6174 696f  on_regularizatio
-0000ab30: 6e72 1900 0000 631c 0000 0000 0000 0000  nr....c.........
-0000ab40: 0000 001f 0000 001e 0000 000b 0000 0073  ...............s
-0000ab50: d400 0000 7c12 7254 7400 6a01 a002 7c00  ....|.rTt.j...|.
-0000ab60: 6a03 7c00 6a04 6401 6402 a104 7d1d 7400  j.|.j.d.d...}.t.
-0000ab70: 6a01 a002 7c1d 7405 7c12 7406 8302 7230  j...|.t.|.t...r0
-0000ab80: 7c12 6e20 8700 8701 8702 8703 6604 6403  |.n ........f.d.
-0000ab90: 6404 8408 7400 a007 7c1d a101 4400 8301  d...t...|...D...
-0000aba0: 6405 1900 a102 7d12 7a60 7408 6a09 6a0a  d.....}.z`t.j.j.
-0000abb0: 6600 7c01 7c02 8800 8801 7c05 8802 7c07  f.|.|.....|...|.
-0000abc0: 7c08 7c09 8803 7c0b 7c0c 7c0d 7c0e 7c0f  |.|...|.|.|.|.|.
-0000abd0: 7c10 7400 6a01 a002 7c00 6a03 7c00 6a04  |.t.j...|.j.|.j.
-0000abe0: 7c11 6401 a104 7c12 7c13 7c14 7c15 7c16  |.d...|.|.|.|.|.
-0000abf0: 7c17 7c18 7c19 7c1a 7c1b 6406 9c1b 7c1c  |.|.|.|.|.d...|.
-0000ac00: a401 8e01 7d1e 5700 6e1a 0400 740b 79ce  ....}.W.n...t.y.
-0000ac10: 0100 0100 0100 740c 6407 8301 8201 5900  ......t.d.....Y.
-0000ac20: 6e02 3000 7c1e 5300 2908 61f9 0d00 0041  n.0.|.S.).a....A
-0000ac30: 6e6e 6f74 6174 6573 2063 6f6f 7264 696e  nnotates coordin
-0000ac40: 6174 6573 2075 7369 6e67 2061 2064 6565  ates using a dee
-0000ac50: 7020 756e 7375 7065 7276 6973 6564 2061  p unsupervised a
-0000ac60: 7574 6f65 6e63 6f64 6572 2e0a 0a20 2020  utoencoder...   
-0000ac70: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
-0000ac80: 2020 2020 2020 2070 7265 7072 6f63 6573         preproces
-0000ac90: 7365 645f 6f62 6a65 6374 2028 7475 706c  sed_object (tupl
-0000aca0: 6529 3a20 5475 706c 6520 636f 6e74 6169  e): Tuple contai
-0000acb0: 6e69 6e67 2061 2070 7265 7072 6f63 6573  ning a preproces
-0000acc0: 7365 6420 6f62 6a65 6374 2028 585f 7472  sed object (X_tr
-0000acd0: 6169 6e2c 2079 5f74 7261 696e 2c20 585f  ain, y_train, X_
-0000ace0: 7465 7374 2c20 795f 7465 7374 292e 0a20  test, y_test).. 
-0000acf0: 2020 2020 2020 2020 2020 2061 646a 6163             adjac
-0000ad00: 656e 6379 5f6d 6174 7269 7820 286e 702e  ency_matrix (np.
-0000ad10: 6e64 6172 7261 7929 3a20 6164 6a61 6365  ndarray): adjace
-0000ad20: 6e63 7920 6d61 7472 6978 206f 6620 7468  ncy matrix of th
-0000ad30: 6520 636f 6e6e 6563 7469 7669 7479 2067  e connectivity g
-0000ad40: 7261 7068 2074 6f20 7573 652e 0a20 2020  raph to use..   
-0000ad50: 2020 2020 2020 2020 2065 6d62 6564 6469           embeddi
-0000ad60: 6e67 5f6d 6f64 656c 2028 7374 7229 3a20  ng_model (str): 
-0000ad70: 4e61 6d65 206f 6620 7468 6520 656d 6265  Name of the embe
-0000ad80: 6464 696e 6720 6d6f 6465 6c20 746f 2075  dding model to u
-0000ad90: 7365 2e20 4d75 7374 2062 6520 6f6e 6520  se. Must be one 
-0000ada0: 6f66 2056 5156 4145 2028 6465 6661 756c  of VQVAE (defaul
-0000adb0: 7429 2c20 5661 4445 2c20 6f72 2063 6f6e  t), VaDE, or con
-0000adc0: 7472 6173 7469 7665 2e0a 2020 2020 2020  trastive..      
-0000add0: 2020 2020 2020 656e 636f 6465 725f 7479        encoder_ty
-0000ade0: 7065 2028 7374 7229 3a20 456e 636f 6465  pe (str): Encode
-0000adf0: 7220 6172 6368 6974 6563 7475 7265 2074  r architecture t
-0000ae00: 6f20 7573 652e 204d 7573 7420 6265 206f  o use. Must be o
-0000ae10: 6e65 206f 6620 2272 6563 7572 7265 6e74  ne of "recurrent
-0000ae20: 222c 2022 5443 4e22 2c20 616e 6420 2274  ", "TCN", and "t
-0000ae30: 7261 6e73 666f 726d 6572 222e 0a20 2020  ransformer"..   
-0000ae40: 2020 2020 2020 2020 2062 6174 6368 5f73           batch_s
-0000ae50: 697a 6520 2869 6e74 293a 2042 6174 6368  ize (int): Batch
-0000ae60: 2073 697a 6520 666f 7220 7472 6169 6e69   size for traini
-0000ae70: 6e67 2e0a 2020 2020 2020 2020 2020 2020  ng..            
-0000ae80: 6c61 7465 6e74 5f64 696d 2028 696e 7429  latent_dim (int)
-0000ae90: 3a20 4469 6d65 6e74 696f 6e20 7369 7a65  : Dimention size
-0000aea0: 206f 6620 7468 6520 6c61 7465 6e74 2073   of the latent s
-0000aeb0: 7061 6365 2e0a 2020 2020 2020 2020 2020  pace..          
-0000aec0: 2020 6570 6f63 6873 2028 696e 7429 3a20    epochs (int): 
-0000aed0: 4d61 7869 6d75 6d20 6e75 6d62 6572 206f  Maximum number o
-0000aee0: 6620 6570 6f63 6873 2074 6f20 7472 6169  f epochs to trai
-0000aef0: 6e20 7468 6520 6d6f 6465 6c2e 2041 6374  n the model. Act
-0000af00: 7561 6c20 7472 6169 6e69 6e67 206d 6967  ual training mig
-0000af10: 6874 2062 6520 7368 6f72 7465 722c 2061  ht be shorter, a
-0000af20: 7320 7468 6520 6d6f 6465 6c20 7769 6c6c  s the model will
-0000af30: 2073 746f 7020 7472 6169 6e69 6e67 2077   stop training w
-0000af40: 6865 6e20 7661 6c69 6461 7469 6f6e 206c  hen validation l
-0000af50: 6f73 7320 7374 6f70 7320 6465 6372 6561  oss stops decrea
-0000af60: 7369 6e67 2e0a 2020 2020 2020 2020 2020  sing..          
-0000af70: 2020 6c6f 675f 6869 7374 6f72 7920 2862    log_history (b
-0000af80: 6f6f 6c29 3a20 5768 6574 6865 7220 746f  ool): Whether to
-0000af90: 206c 6f67 2074 6865 2068 6973 746f 7279   log the history
-0000afa0: 206f 6620 7468 6520 6d6f 6465 6c20 746f   of the model to
-0000afb0: 2054 656e 736f 7242 6f61 7264 2e0a 2020   TensorBoard..  
-0000afc0: 2020 2020 2020 2020 2020 6c6f 675f 6870            log_hp
-0000afd0: 6172 616d 7320 2862 6f6f 6c29 3a20 5768  arams (bool): Wh
-0000afe0: 6574 6865 7220 746f 206c 6f67 2074 6865  ether to log the
-0000aff0: 2068 7970 6572 7061 7261 6d65 7465 7273   hyperparameters
-0000b000: 206f 6620 7468 6520 6d6f 6465 6c20 746f   of the model to
-0000b010: 2054 656e 736f 7242 6f61 7264 2e0a 2020   TensorBoard..  
-0000b020: 2020 2020 2020 2020 2020 6e5f 636f 6d70            n_comp
-0000b030: 6f6e 656e 7473 2028 696e 7429 3a20 4e75  onents (int): Nu
-0000b040: 6d62 6572 206f 6620 6c61 7465 6e74 2063  mber of latent c
-0000b050: 6c75 7374 6572 7320 666f 7220 7468 6520  lusters for the 
-0000b060: 656d 6265 6464 696e 6720 6d6f 6465 6c20  embedding model 
-0000b070: 746f 2075 7365 2e0a 2020 2020 2020 2020  to use..        
-0000b080: 2020 2020 6b6d 6561 6e73 5f6c 6f73 7320      kmeans_loss 
-0000b090: 2866 6c6f 6174 293a 2057 6569 6768 7420  (float): Weight 
-0000b0a0: 6f66 2074 6865 2067 7261 6d20 6c6f 7373  of the gram loss
-0000b0b0: 2c20 7768 6963 6820 6164 6473 2061 2072  , which adds a r
-0000b0c0: 6567 756c 6172 697a 6174 696f 6e20 7465  egularization te
-0000b0d0: 726d 2074 6f20 5661 4445 2061 6e64 2056  rm to VaDE and V
-0000b0e0: 5156 4145 206d 6f64 656c 7320 7768 6963  QVAE models whic
-0000b0f0: 6820 7065 6e61 6c69 7a65 7320 7468 6520  h penalizes the 
-0000b100: 636f 7272 656c 6174 696f 6e20 6265 7477  correlation betw
-0000b110: 6565 6e20 7468 6520 6469 6d65 6e73 696f  een the dimensio
-0000b120: 6e73 2069 6e20 7468 6520 6c61 7465 6e74  ns in the latent
-0000b130: 2073 7061 6365 2e0a 2020 2020 2020 2020   space..        
-0000b140: 2020 2020 7465 6d70 6572 6174 7572 6520      temperature 
-0000b150: 2866 6c6f 6174 293a 2074 656d 7065 7261  (float): tempera
-0000b160: 7475 7265 2070 6172 616d 6574 6572 2066  ture parameter f
-0000b170: 6f72 2074 6865 2063 6f6e 7472 6173 7469  or the contrasti
-0000b180: 7665 206c 6f73 7320 6675 6e63 7469 6f6e  ve loss function
-0000b190: 732e 2048 6967 6865 7220 7661 6c75 6573  s. Higher values
-0000b1a0: 2070 7574 2068 6172 7368 6572 2070 656e   put harsher pen
-0000b1b0: 616c 7469 6573 206f 6e20 6e65 6761 7469  alties on negati
-0000b1c0: 7665 2070 6169 7220 7369 6d69 6c61 7269  ve pair similari
-0000b1d0: 7479 2e0a 2020 2020 2020 2020 2020 2020  ty..            
-0000b1e0: 636f 6e74 7261 7374 6976 655f 7369 6d69  contrastive_simi
-0000b1f0: 6c61 7269 7479 5f66 756e 6374 696f 6e20  larity_function 
-0000b200: 2873 7472 293a 2073 696d 696c 6172 6974  (str): similarit
-0000b210: 7920 6675 6e63 7469 6f6e 2062 6574 7765  y function betwe
-0000b220: 656e 2070 6f73 6974 6976 6520 616e 6420  en positive and 
-0000b230: 6e65 6761 7469 7665 2070 6169 7273 2e20  negative pairs. 
-0000b240: 4d75 7374 2062 6520 6f6e 6520 6f66 2027  Must be one of '
-0000b250: 636f 7369 6e65 2720 2864 6566 6175 6c74  cosine' (default
-0000b260: 292c 2027 6575 636c 6964 6561 6e27 2c20  ), 'euclidean', 
-0000b270: 2764 6f74 272c 2061 6e64 2027 6564 6974  'dot', and 'edit
-0000b280: 272e 0a20 2020 2020 2020 2020 2020 2063  '..            c
-0000b290: 6f6e 7472 6173 7469 7665 5f6c 6f73 735f  ontrastive_loss_
-0000b2a0: 6675 6e63 7469 6f6e 2028 7374 7229 3a20  function (str): 
-0000b2b0: 636f 6e74 7261 7374 6976 6520 6c6f 7373  contrastive loss
-0000b2c0: 2066 756e 6374 696f 6e2e 204d 7573 7420   function. Must 
-0000b2d0: 6265 206f 6e65 206f 6620 276e 6365 2720  be one of 'nce' 
-0000b2e0: 2864 6566 6175 6c74 292c 2027 6463 6c27  (default), 'dcl'
-0000b2f0: 2c20 2766 6327 2c20 616e 6420 2768 6172  , 'fc', and 'har
-0000b300: 645f 6463 6c27 2e20 5365 6520 7370 6563  d_dcl'. See spec
-0000b310: 6966 6963 2064 6f63 756d 656e 7461 7469  ific documentati
-0000b320: 6f6e 2066 6f72 2064 6574 6169 6c73 2e0a  on for details..
-0000b330: 2020 2020 2020 2020 2020 2020 6265 7461              beta
-0000b340: 2028 666c 6f61 7429 3a20 4265 7461 2028   (float): Beta (
-0000b350: 636f 6e63 656e 7472 6174 696f 6e29 2070  concentration) p
-0000b360: 6172 616d 6574 6572 2066 6f72 2074 6865  arameter for the
-0000b370: 2068 6172 645f 6463 6c20 636f 6e74 7261   hard_dcl contra
-0000b380: 7374 6976 6520 6c6f 7373 2e20 4869 6768  stive loss. High
-0000b390: 6572 2076 616c 7565 7320 6c65 6164 2074  er values lead t
-0000b3a0: 6f20 2768 6172 6465 7227 206e 6567 6174  o 'harder' negat
-0000b3b0: 6976 6520 7361 6d70 6c65 732e 0a20 2020  ive samples..   
-0000b3c0: 2020 2020 2020 2020 2074 6175 2028 666c           tau (fl
-0000b3d0: 6f61 7429 3a20 5461 7520 7061 7261 6d65  oat): Tau parame
-0000b3e0: 7465 7220 666f 7220 7468 6520 6463 6c20  ter for the dcl 
-0000b3f0: 616e 6420 6861 7264 5f64 636c 2063 6f6e  and hard_dcl con
-0000b400: 7472 6173 7469 7665 206c 6f73 7365 732c  trastive losses,
-0000b410: 2069 6e64 6963 6174 696e 6720 706f 7369   indicating posi
-0000b420: 7469 7665 2063 6c61 7373 2070 726f 6261  tive class proba
-0000b430: 6269 6c69 7479 2e0a 2020 2020 2020 2020  bility..        
-0000b440: 2020 2020 6f75 7470 7574 5f70 6174 6820      output_path 
-0000b450: 2873 7472 293a 2050 6174 6820 746f 2073  (str): Path to s
-0000b460: 6176 6520 7468 6520 7472 6169 6e65 6420  ave the trained 
-0000b470: 6d6f 6465 6c20 616e 6420 616c 6c20 6c6f  model and all lo
-0000b480: 6720 6669 6c65 732e 0a20 2020 2020 2020  g files..       
-0000b490: 2020 2020 2070 7265 7472 6169 6e65 6420       pretrained 
-0000b4a0: 2873 7472 293a 2057 6865 7468 6572 2074  (str): Whether t
-0000b4b0: 6f20 6c6f 6164 2061 2070 7265 7472 6169  o load a pretrai
-0000b4c0: 6e65 6420 6d6f 6465 6c2e 2049 6620 4661  ned model. If Fa
-0000b4d0: 6c73 652c 206d 6f64 656c 2069 7320 7472  lse, model is tr
-0000b4e0: 6169 6e65 6420 6672 6f6d 2073 6372 6174  ained from scrat
-0000b4f0: 6368 2e20 4966 206e 6f74 2c20 6d75 7374  ch. If not, must
-0000b500: 2062 6520 7468 6520 7061 7468 2074 6f20   be the path to 
-0000b510: 6120 7361 7665 6420 6d6f 6465 6c2e 0a20  a saved model.. 
-0000b520: 2020 2020 2020 2020 2020 2073 6176 655f             save_
-0000b530: 6368 6563 6b70 6f69 6e74 7320 2862 6f6f  checkpoints (boo
-0000b540: 6c29 3a20 5768 6574 6865 7220 746f 2073  l): Whether to s
-0000b550: 6176 6520 6368 6563 6b70 6f69 6e74 7320  ave checkpoints 
-0000b560: 6f66 2074 6865 206d 6f64 656c 2064 7572  of the model dur
-0000b570: 696e 6720 7472 6169 6e69 6e67 2e20 4465  ing training. De
-0000b580: 6661 756c 7473 2074 6f20 4661 6c73 652e  faults to False.
-0000b590: 0a20 2020 2020 2020 2020 2020 2073 6176  .            sav
-0000b5a0: 655f 7765 6967 6874 7320 2862 6f6f 6c29  e_weights (bool)
-0000b5b0: 3a20 5768 6574 6865 7220 746f 2073 6176  : Whether to sav
-0000b5c0: 6520 7468 6520 7765 6967 6874 7320 6f66  e the weights of
-0000b5d0: 2074 6865 206d 6f64 656c 2064 7572 696e   the model durin
-0000b5e0: 6720 7472 6169 6e69 6e67 2e20 4465 6661  g training. Defa
-0000b5f0: 756c 7473 2074 6f20 5472 7565 2e0a 2020  ults to True..  
-0000b600: 2020 2020 2020 2020 2020 696e 7075 745f            input_
-0000b610: 7479 7065 2028 7374 7229 3a20 5479 7065  type (str): Type
-0000b620: 206f 6620 7468 6520 7072 6570 726f 6365   of the preproce
-0000b630: 7373 6564 5f6f 626a 6563 7420 7061 7373  ssed_object pass
-0000b640: 6564 2061 7320 7468 6520 6669 7273 7420  ed as the first 
-0000b650: 7061 7261 6d65 7465 722e 2053 6565 2064  parameter. See d
-0000b660: 6565 706f 662e 6461 7461 2e54 6162 6c65  eepof.data.Table
-0000b670: 4469 6374 2066 6f72 206d 6f72 6520 6465  Dict for more de
-0000b680: 7461 696c 732e 0a20 2020 2020 2020 2020  tails..         
-0000b690: 2020 2072 756e 2028 696e 7429 3a20 5275     run (int): Ru
-0000b6a0: 6e20 6e75 6d62 6572 2066 6f72 2074 6865  n number for the
-0000b6b0: 206d 6f64 656c 2e20 5573 6564 2074 6f20   model. Used to 
-0000b6c0: 7361 7665 2074 6865 206d 6f64 656c 2061  save the model a
-0000b6d0: 6e64 206c 6f67 2066 696c 6573 2e20 4f70  nd log files. Op
-0000b6e0: 7469 6f6e 616c 2e0a 2020 2020 2020 2020  tional..        
-0000b6f0: 2020 2020 6b6c 5f61 6e6e 6561 6c69 6e67      kl_annealing
-0000b700: 5f6d 6f64 6520 2873 7472 293a 204d 6f64  _mode (str): Mod
-0000b710: 6520 6f66 2074 6865 204b 4c20 616e 6e65  e of the KL anne
-0000b720: 616c 696e 672e 204d 7573 7420 6265 206f  aling. Must be o
-0000b730: 6e65 206f 6620 226c 696e 6561 7222 2c20  ne of "linear", 
-0000b740: 6f72 2022 7369 676d 6f69 6422 2e0a 2020  or "sigmoid"..  
-0000b750: 2020 2020 2020 2020 2020 6b6c 5f77 6172            kl_war
-0000b760: 6d75 7020 2869 6e74 293a 204e 756d 6265  mup (int): Numbe
-0000b770: 7220 6f66 2065 706f 6368 7320 746f 2077  r of epochs to w
-0000b780: 6172 6d20 7570 2074 6865 204b 4c20 616e  arm up the KL an
-0000b790: 6e65 616c 696e 672e 0a20 2020 2020 2020  nealing..       
-0000b7a0: 2020 2020 2072 6567 5f63 6174 5f63 6c75       reg_cat_clu
-0000b7b0: 7374 6572 7320 2862 6f6f 6c29 3a20 7768  sters (bool): wh
-0000b7c0: 6574 6865 7220 746f 2070 656e 616c 697a  ether to penaliz
-0000b7d0: 6520 756e 6576 656e 2063 6c75 7374 6572  e uneven cluster
-0000b7e0: 206d 656d 6265 7273 6869 7020 696e 2074   membership in t
-0000b7f0: 6865 206c 6174 656e 7420 7370 6163 652c  he latent space,
-0000b800: 2062 7920 6d69 6e69 6d69 7a69 6e67 2074   by minimizing t
-0000b810: 6865 204b 4c20 6469 7665 7267 656e 6365  he KL divergence
-0000b820: 2062 6574 7765 656e 2063 6c75 7374 6572   between cluster
-0000b830: 206d 656d 6265 7273 6869 7020 616e 6420   membership and 
-0000b840: 6120 756e 6966 6f72 6d20 6361 7465 676f  a uniform catego
-0000b850: 7269 6361 6c20 6469 7374 7269 6275 7469  rical distributi
-0000b860: 6f6e 2e0a 2020 2020 2020 2020 2020 2020  on..            
-0000b870: 7265 636c 7573 7465 7220 2862 6f6f 6c29  recluster (bool)
-0000b880: 3a20 7768 6574 6865 7220 746f 2072 6563  : whether to rec
-0000b890: 6c75 7374 6572 2061 6674 6572 2074 7261  luster after tra
-0000b8a0: 696e 696e 6720 7573 696e 6720 6120 4761  ining using a Ga
-0000b8b0: 7573 7369 616e 204d 6978 7475 7265 204d  ussian Mixture M
-0000b8c0: 6f64 656c 2e20 4f6e 6c79 2076 616c 6964  odel. Only valid
-0000b8d0: 2066 6f72 2056 6144 452e 0a20 2020 2020   for VaDE..     
-0000b8e0: 2020 2020 2020 2069 6e74 6572 6163 7469         interacti
-0000b8f0: 6f6e 5f72 6567 756c 6172 697a 6174 696f  on_regularizatio
-0000b900: 6e20 2866 6c6f 6174 293a 2077 6569 6768  n (float): weigh
-0000b910: 7420 6f66 2074 6865 2069 6e74 6572 6163  t of the interac
-0000b920: 7469 6f6e 2072 6567 756c 6172 697a 6174  tion regularizat
-0000b930: 696f 6e20 7465 726d 2066 6f72 2061 6c6c  ion term for all
-0000b940: 2065 6e63 6f64 6572 732e 0a20 2020 2020   encoders..     
-0000b950: 2020 2020 2020 202a 2a6b 7761 7267 733a         **kwargs:
-0000b960: 2041 6464 6974 696f 6e61 6c20 6b65 7977   Additional keyw
-0000b970: 6f72 6420 6172 6775 6d65 6e74 7320 746f  ord arguments to
-0000b980: 2070 6173 7320 746f 2074 6865 206d 6f64   pass to the mod
-0000b990: 656c 2e0a 0a20 2020 2020 2020 2052 6574  el...        Ret
-0000b9a0: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
-0000b9b0: 2020 5475 706c 653a 2054 7570 6c65 2063    Tuple: Tuple c
-0000b9c0: 6f6e 7461 696e 696e 6720 616c 6c20 7472  ontaining all tr
-0000b9d0: 6169 6e65 6420 6d6f 6465 6c73 2e20 5365  ained models. Se
-0000b9e0: 6520 7370 6563 6966 6963 206d 6f64 656c  e specific model
-0000b9f0: 2064 6f63 756d 656e 7461 7469 6f6e 2075   documentation u
-0000ba00: 6e64 6572 2064 6565 706f 662e 6d6f 6465  nder deepof.mode
-0000ba10: 6c73 2066 6f72 2064 6574 6169 6c73 2e0a  ls for details..
-0000ba20: 2020 2020 2020 2020 da0e 5472 6169 6e65          ..Traine
-0000ba30: 645f 6d6f 6465 6c73 da0f 7472 6169 6e65  d_models..traine
-0000ba40: 645f 7765 6967 6874 7363 0100 0000 0000  d_weightsc......
-0000ba50: 0000 0000 0000 0200 0000 0500 0000 1300  ................
-0000ba60: 0000 7338 0000 0067 007c 005d 307d 0188  ..s8...g.|.]0}..
-0000ba70: 007c 0176 0072 0488 017c 0176 0072 0464  .|.v.r...|.v.r.d
-0000ba80: 00a0 0088 02a1 017c 0176 0072 0464 01a0  .......|.v.r.d..
-0000ba90: 0088 03a1 0172 047c 0191 0271 0453 0029  .....r.|...q.S.)
-0000baa0: 027a 0b65 6e63 6f64 696e 673d 7b7d 7a04  .z.encoding={}z.
-0000bab0: 6b3d 7b7d 2901 726c 0000 0029 0272 4a00  k={}).rl...).rJ.
-0000bac0: 0000 da01 77a9 0472 d701 0000 72d8 0100  ....w..r....r...
-0000bad0: 0072 da01 0000 72de 0100 0072 2600 0000  .r....r....r&...
-0000bae0: 7227 0000 0072 4c00 0000 5406 0000 730c  r'...rL...T...s.
-0000baf0: 0000 0006 0202 0108 0108 010e 010a fb7a  ...............z
-0000bb00: 3b43 6f6f 7264 696e 6174 6573 2e64 6565  ;Coordinates.dee
-0000bb10: 705f 756e 7375 7065 7276 6973 6564 5f65  p_unsupervised_e
-0000bb20: 6d62 6564 6469 6e67 2e3c 6c6f 6361 6c73  mbedding.<locals
-0000bb30: 3e2e 3c6c 6973 7463 6f6d 703e 7201 0000  >.<listcomp>r...
-0000bb40: 0029 1b72 d601 0000 729e 0100 0072 d701  .).r....r....r..
-0000bb50: 0000 72d8 0100 0072 d901 0000 72da 0100  ..r....r....r...
-0000bb60: 0072 db01 0000 72dc 0100 0072 dd01 0000  .r....r....r....
-0000bb70: 72de 0100 0072 df01 0000 72e0 0100 0072  r....r....r....r
-0000bb80: e101 0000 72e2 0100 0072 e301 0000 72e4  ....r....r....r.
-0000bb90: 0100 0072 e501 0000 72e6 0100 0072 e701  ...r....r....r..
-0000bba0: 0000 72e8 0100 0072 e901 0000 72ea 0100  ..r....r....r...
-0000bbb0: 0072 eb01 0000 72ec 0100 0072 ed01 0000  .r....r....r....
-0000bbc0: 72ee 0100 0072 ef01 0000 7a4f 4e6f 2070  r....r....zONo p
-0000bbd0: 7265 7472 6169 6e65 6420 6d6f 6465 6c20  retrained model 
-0000bbe0: 666f 756e 6420 666f 7220 7468 6520 6769  found for the gi
-0000bbf0: 7665 6e20 7061 7261 6d65 7465 7273 2e20  ven parameters. 
-0000bc00: 506c 6561 7365 2074 7261 696e 2061 206d  Please train a m
-0000bc10: 6f64 656c 2066 6972 7374 2e29 0d72 1d00  odel first.).r..
-0000bc20: 0000 721e 0000 0072 1f00 0000 7223 0000  ..r....r....r#..
-0000bc30: 0072 2f01 0000 7256 0100 0072 a200 0000  .r/...rV...r....
-0000bc40: 725a 0000 0072 8100 0000 da0b 6d6f 6465  rZ...r......mode
-0000bc50: 6c5f 7574 696c 73da 1765 6d62 6564 6469  l_utils..embeddi
-0000bc60: 6e67 5f6d 6f64 656c 5f66 6974 7469 6e67  ng_model_fitting
-0000bc70: 72c7 0000 0072 7301 0000 291f 7256 0000  r....rs...).rV..
-0000bc80: 0072 d601 0000 729e 0100 0072 d701 0000  .r....r....r....
-0000bc90: 72d8 0100 0072 d901 0000 72da 0100 0072  r....r....r....r
-0000bca0: db01 0000 72dc 0100 0072 dd01 0000 72de  ....r....r....r.
-0000bcb0: 0100 0072 df01 0000 72e0 0100 0072 e101  ...r....r....r..
-0000bcc0: 0000 72e2 0100 0072 e301 0000 72e4 0100  ..r....r....r...
-0000bcd0: 0072 e501 0000 72e6 0100 0072 e701 0000  .r....r....r....
-0000bce0: 72e8 0100 0072 e901 0000 72ea 0100 0072  r....r....r....r
-0000bcf0: eb01 0000 72ec 0100 0072 ed01 0000 72ee  ....r....r....r.
-0000bd00: 0100 0072 ef01 0000 729f 0100 00da 0f70  ...r....r......p
-0000bd10: 7265 7472 6169 6e65 645f 7061 7468 7245  retrained_pathrE
-0000bd20: 0000 0072 2600 0000 72f3 0100 0072 2700  ...r&...r....r'.
-0000bd30: 0000 da1b 6465 6570 5f75 6e73 7570 6572  ....deep_unsuper
-0000bd40: 7669 7365 645f 656d 6265 6464 696e 6706  vised_embedding.
-0000bd50: 0600 0073 7600 0000 0042 0401 0601 0401  ...sv....B......
-0000bd60: 0401 0201 02fc 0406 0601 0203 08ff 0602  ................
-0000bd70: 1002 08fe 0407 02f9 02fb 0410 0201 0801  ................
-0000bd80: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-0000bd90: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-0000bda0: 0601 0401 0401 0201 02fc 0206 0201 0201  ................
-0000bdb0: 0201 0201 0201 0201 0201 0201 0201 02e0  ................
-0000bdc0: 0421 02df 0a23 0c01 0201 02ff 0a05 7a27  .!...#........z'
-0000bdd0: 436f 6f72 6469 6e61 7465 732e 6465 6570  Coordinates.deep
-0000bde0: 5f75 6e73 7570 6572 7669 7365 645f 656d  _unsupervised_em
-0000bdf0: 6265 6464 696e 6729 0846 4672 0100 0000  bedding).FFr....
-0000be00: 4654 4e46 4629 0572 0100 0000 4e54 4646  FTNFF).r....NTFF
-0000be10: 2905 4672 0100 0000 4e46 4629 0272 0100  ).Fr....NFF).r..
-0000be20: 0000 7257 0000 0029 0146 2903 4e4e 5429  ..rW...).F).NNT)
-0000be30: 024e 5429 064e 4e46 464e 5429 1a4e 72cc  .NT).NNFFNT).Nr.
-0000be40: 0100 0072 cd01 0000 72ce 0100 0072 cf01  ...r....r....r..
-0000be50: 0000 72d0 0100 0054 4672 d101 0000 72ac  ..r....TFr....r.
-0000be60: 0000 0072 d201 0000 72d3 0100 0072 d401  ...r....r....r..
-0000be70: 0000 72d2 0100 0072 d201 0000 722c 0000  ..r....r....r,..
-0000be80: 0046 4654 4672 0100 0000 72d5 0100 0072  .FFTFr....r....r
-0000be90: b000 0000 72ac 0000 0046 72ac 0000 0029  ....r....Fr....)
-0000bea0: 2772 5800 0000 7228 0100 0072 2901 0000  'rX...r(...r)...
-0000beb0: 722a 0100 0072 d100 0000 72a2 0000 0072  r*...r....r....r
-0000bec0: dd00 0000 72de 0000 0072 2c01 0000 da07  ....r....r,.....
-0000bed0: 6e64 6172 7261 7972 1f01 0000 7213 0000  ndarrayr....r...
-0000bee0: 0072 9b01 0000 da05 4772 6170 6872 b500  .r......Graphr..
-0000bef0: 0000 7269 0000 0072 6d00 0000 726e 0000  ..ri...rm...rn..
-0000bf00: 0072 2b01 0000 7212 0000 00da 0a74 6162  .r+...r......tab
-0000bf10: 6c65 5f64 6963 7472 6a01 0000 72f8 0000  le_dictrj...r...
-0000bf20: 0072 0301 0000 7216 0100 0072 7701 0000  .r....r....rw...
-0000bf30: 722d 0100 0072 7801 0000 727c 0100 0072  r-...rx...r|...r
-0000bf40: 5e01 0000 7283 0000 0072 8601 0000 7223  ^...r....r....r#
-0000bf50: 0100 0072 ad01 0000 da03 696e 6672 cb01  ...r......infr..
-0000bf60: 0000 7214 0000 0072 c000 0000 72f7 0100  ..r....r....r...
-0000bf70: 0072 2600 0000 7226 0000 0072 2600 0000  .r&...r&...r&...
-0000bf80: 7227 0000 0072 1a00 0000 da02 0000 7366  r'...r........sf
-0000bf90: 0100 0008 0104 1202 0108 0102 0102 0102  ................
-0000bfa0: 0102 0102 ea02 0202 0102 0102 0104 0102  ................
-0000bfb0: 0102 0102 0104 0102 0102 0102 0102 0102  ................
-0000bfc0: 0102 0102 0102 0102 0102 0104 0102 0102  ................
-0000bfd0: ea0c 4708 0408 0600 0100 0100 0100 0100  ..G.............
-0000bfe0: 0100 0100 0100 f702 0202 0102 0102 0102  ................
-0000bff0: 0102 0102 0102 0102 0102 f60c 7f00 2e00  ................
-0000c000: 0100 0100 0100 0100 fa02 0202 0102 0102  ................
-0000c010: 0102 0102 0102 f90c 5500 0100 0100 0100  ........U.......
-0000c020: 0100 fa02 0202 0102 0102 0102 0102 0102  ................
-0000c030: f90c 4214 3a10 0702 010a 0408 1008 0402  ..B.:...........
-0000c040: 010a 0500 ff02 0106 ff0c 2f12 1600 0100  ........../.....
-0000c050: 0100 0100 0100 0100 f902 0202 0102 0102  ................
-0000c060: 0102 0102 0102 0202 f70c 7f00 0d02 0102  ................
-0000c070: 0104 0102 0102 0102 f902 0202 0102 0102  ................
-0000c080: 0102 0102 0102 0102 f80c 7100 0100 0100  ..........q.....
-0000c090: 0100 0100 0100 0100 0100 0100 0100 0100  ................
-0000c0a0: 0100 0100 0100 0100 0100 0100 0100 0100  ................
-0000c0b0: 0100 0100 0100 0100 0100 0100 0100 e402  ................
-0000c0c0: 0216 0104 0102 0102 0102 0102 0102 0102  ................
-0000c0d0: 0102 0102 0102 0102 0102 0102 0102 0102  ................
-0000c0e0: 0102 0102 0102 0102 0102 0102 0102 0102  ................
-0000c0f0: 0102 0102 0102 0202 e272 1a00 0000 6300  .........r....c.
-0000c100: 0000 0000 0000 0000 0000 0000 0000 000e  ................
-0000c110: 0000 0000 0000 0073 5c01 0000 6500 5a01  .......s\...e.Z.
-0000c120: 6400 5a02 6401 5a03 6402 6402 6504 6403  d.Z.d.Z.d.d.e.d.
-0000c130: 6701 8301 6402 6402 6402 6402 6404 6404  g...d.d.d.d.d.d.
-0000c140: 6609 6505 6506 6506 6507 6a08 6509 6506  f.e.e.e.e.j.e.e.
-0000c150: 650a 6a0b 650c 650d 650c 650e 6505 650c  e.j.e.e.e.e.e.e.
-0000c160: 6602 1900 6405 9c0b 8700 6601 6406 6407  f...d.....f.d.d.
-0000c170: 840d 5a0f 6510 6511 6408 9c02 6409 640a  ..Z.e.e.d...d.d.
-0000c180: 8404 5a12 650d 6511 640b 9c02 640c 640d  ..Z.e.e.d...d.d.
-0000c190: 8404 5a13 6507 6a14 640e 9c01 640f 6410  ..Z.e.j.d...d.d.
-0000c1a0: 8404 5a15 6430 6506 6516 6506 6517 6518  ..Z.d0e.e.e.e.e.
-0000c1b0: 6518 6602 1900 6412 9c04 6413 6414 8405  e.f...d...d.d...
-0000c1c0: 5a19 6431 6516 6506 6517 6518 6518 6602  Z.d1e.e.e.e.e.f.
-0000c1d0: 1900 6416 9c03 6417 6418 8405 5a1a 6432  ..d...d.d...Z.d2
-0000c1e0: 6516 6506 6517 6518 6518 6602 1900 6416  e.e.e.e.e.f...d.
-0000c1f0: 9c03 6419 641a 8405 5a1b 6433 6516 6517  ..d.d...Z.d3e.e.
-0000c200: 6518 6518 6602 1900 641b 9c02 641c 641d  e.e.f...d...d.d.
-0000c210: 8405 5a1c 6434 6506 6511 641e 9c02 641f  ..Z.d4e.e.d...d.
-0000c220: 6420 8405 5a1d 6404 6421 9c01 6422 6423  d ..Z.d.d!..d"d#
-0000c230: 8402 5a1e 6435 6511 6516 6504 6425 9c03  ..Z.d5e.e.e.d%..
-0000c240: 6426 6427 8405 5a1f 6436 6506 6516 6516  d&d'..Z.d6e.e.e.
-0000c250: 6506 6518 6516 6516 650c 650c 6516 650d  e.e.e.e.e.e.e.e.
-0000c260: 6507 6a14 642d 9c0c 642e 642f 8405 5a20  e.j.d-..d.d/..Z 
-0000c270: 8700 0400 5a21 5300 2937 72da 0000 007a  ....Z!S.)7r....z
-0000c280: e54d 6169 6e20 636c 6173 7320 666f 7220  .Main class for 
-0000c290: 7374 6f72 696e 6720 6120 7369 6e67 6c65  storing a single
-0000c2a0: 2064 6174 6173 6574 2061 7320 6120 6469   dataset as a di
-0000c2b0: 6374 696f 6e61 7279 2077 6974 6820 696e  ctionary with in
-0000c2c0: 6469 7669 6475 616c 7320 6173 206b 6579  dividuals as key
-0000c2d0: 7320 616e 6420 7061 6e64 6173 2e44 6174  s and pandas.Dat
-0000c2e0: 6146 7261 6d65 7320 6173 2076 616c 7565  aFrames as value
-0000c2f0: 732e 0a0a 2020 2020 496e 636c 7564 6573  s...    Includes
-0000c300: 206d 6574 686f 6473 2066 6f72 2067 656e   methods for gen
-0000c310: 6572 6174 696e 6720 7472 6169 6e69 6e67  erating training
-0000c320: 2061 6e64 2074 6573 7469 6e67 2064 6174   and testing dat
-0000c330: 6173 6574 7320 666f 7220 7468 6520 7375  asets for the su
-0000c340: 7065 7276 6973 6564 2061 6e64 2075 6e73  pervised and uns
-0000c350: 7570 6572 7669 7365 6420 6d6f 6465 6c73  upervised models
-0000c360: 2e0a 2020 2020 4e72 2c00 0000 4629 0b72  ..    Nr,...F).r
-0000c370: 6001 0000 72af 0000 0072 3400 0000 725f  `...r....r4...r_
-0000c380: 0000 0072 3300 0000 7242 0100 0072 6300  ...r3...rB...rc.
-0000c390: 0000 7243 0100 0072 3800 0000 7248 0100  ..rC...r8...rH..
-0000c3a0: 0072 4901 0000 630c 0000 0000 0000 0000  .rI...c.........
-0000c3b0: 0000 000c 0000 0003 0000 0003 0000 0073  ...............s
-0000c3c0: 4c00 0000 7400 8300 a001 7c01 a101 0100  L...t.....|.....
-0000c3d0: 7c02 7c00 5f02 7c06 7c00 5f03 7c07 7c00  |.|._.|.|._.|.|.
-0000c3e0: 5f04 7c08 7c00 5f05 7c03 7c00 5f06 7c04  _.|.|._.|.|._.|.
-0000c3f0: 7c00 5f07 7c05 7c00 5f08 7c09 7c00 5f09  |._.|.|._.|.|._.
-0000c400: 7c0a 7c00 5f0a 7c0b 7c00 5f0b 6401 5300  |.|._.|.|._.d.S.
-0000c410: 2902 61f6 0400 0053 746f 7265 2073 696e  ).a....Store sin
-0000c420: 676c 6520 6461 7461 7365 7473 2061 7320  gle datasets as 
-0000c430: 6469 6374 696f 6e61 7269 6573 2077 6974  dictionaries wit
-0000c440: 6820 696e 6469 7669 6475 616c 7320 6173  h individuals as
-0000c450: 206b 6579 7320 616e 6420 7061 6e64 6173   keys and pandas
-0000c460: 2e44 6174 6146 7261 6d65 7320 6173 2076  .DataFrames as v
-0000c470: 616c 7565 732e 0a0a 2020 2020 2020 2020  alues...        
-0000c480: 496e 636c 7564 6573 206d 6574 686f 6473  Includes methods
-0000c490: 2066 6f72 2067 656e 6572 6174 696e 6720   for generating 
-0000c4a0: 7472 6169 6e69 6e67 2061 6e64 2074 6573  training and tes
-0000c4b0: 7469 6e67 2064 6174 6173 6574 7320 666f  ting datasets fo
-0000c4c0: 7220 7468 6520 6175 746f 656e 636f 6465  r the autoencode
-0000c4d0: 7273 2e0a 0a20 2020 2020 2020 2041 7267  rs...        Arg
-0000c4e0: 733a 0a20 2020 2020 2020 2020 2020 2074  s:.            t
-0000c4f0: 6162 7320 2844 6963 7429 3a20 4469 6374  abs (Dict): Dict
-0000c500: 696f 6e61 7279 206f 6620 7061 6e64 6173  ionary of pandas
-0000c510: 2e44 6174 6146 7261 6d65 7320 7769 7468  .DataFrames with
-0000c520: 2069 6e64 6976 6964 7561 6c20 6578 7065   individual expe
-0000c530: 7269 6d65 6e74 7320 6173 206b 6579 732e  riments as keys.
-0000c540: 0a20 2020 2020 2020 2020 2020 2074 7970  .            typ
-0000c550: 2028 7374 7229 3a20 5479 7065 206f 6620   (str): Type of 
-0000c560: 7468 6520 6461 7461 7365 742e 2045 7861  the dataset. Exa
-0000c570: 6d70 6c65 7320 6172 6520 2263 6f6f 7264  mples are "coord
-0000c580: 7322 2c20 2264 6973 7473 222c 2061 6e64  s", "dists", and
-0000c590: 2022 616e 676c 6573 222e 2046 6f72 206c   "angles". For l
-0000c5a0: 6f67 6769 6e67 2070 7572 706f 7365 7320  ogging purposes 
-0000c5b0: 6f6e 6c79 2e0a 2020 2020 2020 2020 2020  only..          
-0000c5c0: 2020 6172 656e 6120 2873 7472 293a 2054    arena (str): T
-0000c5d0: 7970 6520 6f66 2074 6865 2061 7265 6e61  ype of the arena
-0000c5e0: 2e20 4d75 7374 2062 6520 6f6e 6520 6f66  . Must be one of
-0000c5f0: 2022 6369 7263 756c 6172 2d61 7574 6f64   "circular-autod
-0000c600: 6574 6563 7422 2c20 2263 6972 6375 6c61  etect", "circula
-0000c610: 722d 6d61 6e75 616c 222c 206f 7220 2270  r-manual", or "p
-0000c620: 6f6c 7967 6f6e 2d6d 616e 7561 6c22 2e20  olygon-manual". 
-0000c630: 4861 6e64 6c65 6420 696e 7465 726e 616c  Handled internal
-0000c640: 6c79 2e0a 2020 2020 2020 2020 2020 2020  ly..            
-0000c650: 6172 656e 615f 6469 6d73 2028 6e70 2e61  arena_dims (np.a
-0000c660: 7272 6179 293a 2044 696d 656e 7369 6f6e  rray): Dimension
-0000c670: 7320 6f66 2074 6865 2061 7265 6e61 2069  s of the arena i
-0000c680: 6e20 6d6d 2e0a 2020 2020 2020 2020 2020  n mm..          
-0000c690: 2020 616e 696d 616c 5f69 6473 2028 6c69    animal_ids (li
-0000c6a0: 7374 293a 206c 6973 7420 6f66 2061 6e69  st): list of ani
-0000c6b0: 6d61 6c20 6964 732e 0a20 2020 2020 2020  mal ids..       
-0000c6c0: 2020 2020 2063 656e 7465 7220 2873 7472       center (str
-0000c6d0: 293a 2054 7970 6520 6f66 2074 6865 2063  ): Type of the c
-0000c6e0: 656e 7465 722e 2048 616e 646c 6564 2069  enter. Handled i
-0000c6f0: 6e74 6572 6e61 6c6c 792e 0a20 2020 2020  nternally..     
-0000c700: 2020 2020 2020 2070 6f6c 6172 2028 626f         polar (bo
-0000c710: 6f6c 293a 2057 6865 7468 6572 2074 6865  ol): Whether the
-0000c720: 2064 6174 6173 6574 2069 7320 696e 2070   dataset is in p
-0000c730: 6f6c 6172 2063 6f6f 7264 696e 6174 6573  olar coordinates
-0000c740: 2e20 4861 6e64 6c65 6420 696e 7465 726e  . Handled intern
-0000c750: 616c 6c79 2e0a 2020 2020 2020 2020 2020  ally..          
-0000c760: 2020 6578 705f 636f 6e64 6974 696f 6e73    exp_conditions
-0000c770: 2028 6469 6374 293a 2064 6963 7469 6f6e   (dict): diction
-0000c780: 6172 7920 7769 7468 2065 7870 6572 696d  ary with experim
-0000c790: 656e 7420 4944 7320 6173 206b 6579 7320  ent IDs as keys 
-0000c7a0: 616e 6420 6578 7065 7269 6d65 6e74 616c  and experimental
-0000c7b0: 2063 6f6e 6469 7469 6f6e 7320 6173 2076   conditions as v
-0000c7c0: 616c 7565 732e 0a20 2020 2020 2020 2020  alues..         
-0000c7d0: 2020 2070 726f 7061 6761 7465 5f6c 6162     propagate_lab
-0000c7e0: 656c 7320 2862 6f6f 6c29 3a20 5768 6574  els (bool): Whet
-0000c7f0: 6865 7220 746f 2070 726f 7061 6761 7465  her to propagate
-0000c800: 2070 6865 6e6f 7479 7069 6320 6c61 6265   phenotypic labe
-0000c810: 6c73 2066 726f 6d20 7468 6520 6f72 6967  ls from the orig
-0000c820: 696e 616c 2065 7870 6572 696d 656e 7473  inal experiments
-0000c830: 2074 6f20 7468 6520 7472 616e 7366 6f72   to the transfor
-0000c840: 6d65 6420 6461 7461 7365 742e 0a20 2020  med dataset..   
-0000c850: 2020 2020 2020 2020 2070 726f 7061 6761           propaga
-0000c860: 7465 5f61 6e6e 6f74 6174 696f 6e73 2028  te_annotations (
-0000c870: 4469 6374 293a 2044 6963 7469 6f6e 6172  Dict): Dictionar
-0000c880: 7920 6f66 2061 6e6e 6f74 6174 696f 6e73  y of annotations
-0000c890: 2074 6f20 7072 6f70 6167 6174 652e 2049   to propagate. I
-0000c8a0: 6620 7072 6f76 6964 6564 2c20 7468 6520  f provided, the 
-0000c8b0: 7375 7065 7276 6973 6564 2061 6e6e 6f74  supervised annot
-0000c8c0: 6174 696f 6e73 206f 6620 7468 6520 696e  ations of the in
-0000c8d0: 6469 7669 6475 616c 2065 7870 6572 696d  dividual experim
-0000c8e0: 656e 7473 2061 7265 2070 726f 7061 6761  ents are propaga
-0000c8f0: 7465 6420 746f 2074 6865 2064 6174 6173  ted to the datas
-0000c900: 6574 2e0a 0a20 2020 2020 2020 204e 290c  et...        N).
-0000c910: da05 7375 7065 7272 6900 0000 da05 5f74  ..superri....._t
-0000c920: 7970 65da 075f 6365 6e74 6572 7240 0100  ype.._centerr@..
-0000c930: 00da 065f 706f 6c61 7272 3101 0000 7233  ..._polarr1...r3
-0000c940: 0100 0072 3001 0000 7236 0100 00da 115f  ...r0...r6....._
-0000c950: 7072 6f70 6167 6174 655f 6c61 6265 6c73  propagate_labels
-0000c960: da16 5f70 726f 7061 6761 7465 5f61 6e6e  .._propagate_ann
-0000c970: 6f74 6174 696f 6e73 290c 7256 0000 0072  otations).rV...r
-0000c980: 6001 0000 72af 0000 0072 3400 0000 725f  `...r....r4...r_
-0000c990: 0000 0072 3300 0000 7242 0100 0072 6300  ...r3...rB...rc.
-0000c9a0: 0000 7243 0100 0072 3800 0000 7248 0100  ..rC...r8...rH..
-0000c9b0: 0072 4901 0000 a901 da09 5f5f 636c 6173  .rI.......__clas
-0000c9c0: 735f 5f72 2600 0000 7227 0000 0072 6900  s__r&...r'...ri.
-0000c9d0: 0000 9206 0000 7316 0000 0000 1f0c 0106  ......s.........
-0000c9e0: 0106 0106 0106 0106 0106 0106 0106 0106  ................
-0000c9f0: 017a 1254 6162 6c65 4469 6374 2e5f 5f69  .z.TableDict.__i
-0000ca00: 6e69 745f 5f29 0272 f400 0000 7219 0000  nit__).r....r...
-0000ca10: 0063 0200 0000 0000 0000 0000 0000 0200  .c..............
-0000ca20: 0000 0800 0000 0300 0000 735c 0000 0074  ..........s\...t
-0000ca30: 006a 01a0 027c 00a1 0189 0174 03a0 0487  .j...|.....t....
-0000ca40: 0166 0164 0164 0284 0888 0044 0083 01a1  .f.d.d.....D....
-0000ca50: 0173 2c4a 0064 0383 0182 0174 0587 0066  .s,J.d.....t...f
-0000ca60: 0164 0464 0584 0888 01a0 06a1 0044 0083  .d.d.........D..
-0000ca70: 017c 006a 077c 006a 087c 006a 097c 006a  .|.j.|.j.|.j.|.j
-0000ca80: 0a7c 006a 0b64 068d 0653 0029 0761 6e01  .|.j.d...S.).an.
-0000ca90: 0000 5265 7475 726e 2061 2073 7562 7365  ..Return a subse
-0000caa0: 7420 6f66 2074 6865 206f 7269 6769 6e61  t of the origina
-0000cab0: 6c20 7461 626c 655f 6469 6374 206f 626a  l table_dict obj
-0000cac0: 6563 742c 2063 6f6e 7461 696e 696e 6720  ect, containing 
-0000cad0: 6f6e 6c79 2074 6865 2073 7065 6369 6669  only the specifi
-0000cae0: 6564 206b 6579 732e 0a0a 2020 2020 2020  ed keys...      
-0000caf0: 2020 5573 6566 756c 2c20 666f 7220 6578    Useful, for ex
-0000cb00: 616d 706c 652c 2074 6f20 7365 6c65 6374  ample, to select
-0000cb10: 2064 6174 6120 636f 6d69 6e67 2066 726f   data coming fro
-0000cb20: 6d20 7669 6465 6f73 206f 6620 6120 7370  m videos of a sp
-0000cb30: 6563 6966 6965 6420 636f 6e64 6974 696f  ecified conditio
-0000cb40: 6e2e 0a0a 2020 2020 2020 2020 4172 6773  n...        Args
-0000cb50: 3a0a 2020 2020 2020 2020 2020 2020 6b65  :.            ke
-0000cb60: 7973 2028 6c69 7374 293a 204c 6973 7420  ys (list): List 
-0000cb70: 6f66 206b 6579 7320 746f 206b 6565 702e  of keys to keep.
-0000cb80: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-0000cb90: 733a 0a20 2020 2020 2020 2020 2020 2054  s:.            T
-0000cba0: 6162 6c65 4469 6374 3a20 5375 6273 6574  ableDict: Subset
-0000cbb0: 206f 6620 7468 6520 6f72 6967 696e 616c   of the original
-0000cbc0: 2074 6162 6c65 5f64 6963 7420 6f62 6a65   table_dict obje
-0000cbd0: 6374 2c20 636f 6e74 6169 6e69 6e67 206f  ct, containing o
-0000cbe0: 6e6c 7920 7468 6520 7370 6563 6966 6965  nly the specifie
-0000cbf0: 6420 6b65 7973 2e0a 2020 2020 2020 2020  d keys..        
-0000cc00: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-0000cc10: 0005 0000 0013 0000 0073 1800 0000 6700  .........s....g.
-0000cc20: 7c00 5d10 7d01 7c01 8800 a000 a100 7600  |.].}.|.......v.
-0000cc30: 9102 7104 5300 7226 0000 00a9 0172 f400  ..q.S.r&.....r..
-0000cc40: 0000 2902 724a 0000 0072 eb00 0000 2901  ..).rJ...r....).
-0000cc50: da05 7461 626c 6572 2600 0000 7227 0000  ..tabler&...r'..
-0000cc60: 0072 4c00 0000 c906 0000 724d 0000 007a  .rL.......rM...z
-0000cc70: 2b54 6162 6c65 4469 6374 2e66 696c 7465  +TableDict.filte
-0000cc80: 725f 7669 6465 6f73 2e3c 6c6f 6361 6c73  r_videos.<locals
-0000cc90: 3e2e 3c6c 6973 7463 6f6d 703e 7a15 496e  >.<listcomp>z.In
-0000cca0: 7661 6c69 6420 6b65 7973 2073 656c 6563  valid keys selec
-0000ccb0: 7465 6463 0100 0000 0000 0000 0000 0000  tedc............
-0000ccc0: 0300 0000 0400 0000 1300 0000 731e 0000  ............s...
-0000ccd0: 0069 007c 005d 165c 027d 017d 027c 0188  .i.|.].\.}.}.|..
-0000cce0: 0076 0072 047c 017c 0293 0271 0453 0072  .v.r.|.|...q.S.r
-0000ccf0: 2600 0000 7226 0000 00a9 0372 4a00 0000  &...r&.....rJ...
-0000cd00: 72eb 0000 0072 2701 0000 7204 0200 0072  r....r'...r....r
-0000cd10: 2600 0000 7227 0000 0072 9700 0000 cc06  &...r'...r......
-0000cd20: 0000 724d 0000 007a 2b54 6162 6c65 4469  ..rM...z+TableDi
-0000cd30: 6374 2e66 696c 7465 725f 7669 6465 6f73  ct.filter_videos
-0000cd40: 2e3c 6c6f 6361 6c73 3e2e 3c64 6963 7463  .<locals>.<dictc
-0000cd50: 6f6d 703e a904 7263 0000 0072 4801 0000  omp>..rc...rH...
-0000cd60: 7249 0100 0072 3800 0000 290c 7281 0000  rI...r8...).r...
-0000cd70: 0072 8200 0000 7251 0100 0072 dd00 0000  .r....rQ...r....
-0000cd80: 7257 0000 0072 da00 0000 72cb 0000 0072  rW...r....r....r
-0000cd90: fd01 0000 7240 0100 0072 0002 0000 7201  ....r@...r....r.
-0000cda0: 0200 0072 3601 0000 2902 7256 0000 0072  ...r6...).rV...r
-0000cdb0: f400 0000 7226 0000 0029 0272 f400 0000  ....r&...).r....
-0000cdc0: 7205 0200 0072 2700 0000 da0d 6669 6c74  r....r'.....filt
-0000cdd0: 6572 5f76 6964 656f 73bd 0600 0073 1400  er_videos....s..
-0000cde0: 0000 000b 0c01 2002 0201 1401 0401 0401  ...... .........
-0000cdf0: 0401 0401 04fa 7a17 5461 626c 6544 6963  ......z.TableDic
-0000ce00: 742e 6669 6c74 6572 5f76 6964 656f 7329  t.filter_videos)
-0000ce10: 02da 0b65 7870 5f66 696c 7465 7273 7219  ...exp_filtersr.
-0000ce20: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
-0000ce30: 0300 0000 0a00 0000 0300 0000 736c 0000  ............sl..
-0000ce40: 0074 006a 01a0 0288 03a1 017d 027c 01a0  .t.j.......}.|..
-0000ce50: 03a1 0044 005d 525c 0289 0089 0187 0087  ...D.]R\........
-0000ce60: 0187 0366 0364 0164 0284 087c 02a0 03a1  ...f.d.d...|....
-0000ce70: 0044 0083 0189 0274 0488 0288 036a 0588  .D.....t.....j..
-0000ce80: 036a 0688 036a 0788 036a 0887 0266 0164  .j...j...j...f.d
-0000ce90: 0364 0284 0888 036a 09a0 03a1 0044 0083  .d.....j.....D..
-0000cea0: 0164 048d 067d 0271 147c 0253 0029 0561  .d...}.q.|.S.).a
-0000ceb0: 5c01 0000 5265 7475 726e 2061 2073 7562  \...Return a sub
-0000cec0: 7365 7420 6f66 2074 6865 206f 7269 6769  set of the origi
-0000ced0: 6e61 6c20 7461 626c 655f 6469 6374 206f  nal table_dict o
-0000cee0: 626a 6563 742c 2063 6f6e 7461 696e 696e  bject, containin
-0000cef0: 6720 6f6e 6c79 2076 6964 656f 7320 6265  g only videos be
-0000cf00: 6c6f 6e67 696e 6720 746f 2074 6865 2073  longing to the s
-0000cf10: 7065 6369 6669 6564 2065 7870 6572 696d  pecified experim
-0000cf20: 656e 7461 6c20 636f 6e64 6974 696f 6e2e  ental condition.
-0000cf30: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
-0000cf40: 2020 2020 2020 2020 2020 2020 6578 705f              exp_
-0000cf50: 6669 6c74 6572 7320 2864 6963 7429 3a20  filters (dict): 
-0000cf60: 6578 7065 7269 6d65 6e74 616c 2063 6f6e  experimental con
-0000cf70: 6469 7469 6f6e 7320 616e 6420 7661 6c75  ditions and valu
-0000cf80: 6573 2074 6f20 6669 6c74 6572 206f 6e2e  es to filter on.
-0000cf90: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-0000cfa0: 733a 0a20 2020 2020 2020 2020 2020 2054  s:.            T
-0000cfb0: 6162 6c65 4469 6374 3a20 5375 6273 6574  ableDict: Subset
-0000cfc0: 206f 6620 7468 6520 6f72 6967 696e 616c   of the original
-0000cfd0: 2074 6162 6c65 5f64 6963 7420 6f62 6a65   table_dict obje
-0000cfe0: 6374 2c20 636f 6e74 6169 6e69 6e67 206f  ct, containing o
-0000cff0: 6e6c 7920 7468 6520 7370 6563 6966 6965  nly the specifie
-0000d000: 6420 6b65 7973 2e0a 2020 2020 2020 2020  d keys..        
-0000d010: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
-0000d020: 0004 0000 0013 0000 0073 2a00 0000 6900  .........s*...i.
-0000d030: 7c00 5d22 5c02 7d01 7d02 8802 6a00 7c01  |.]"\.}.}...j.|.
-0000d040: 1900 8800 1900 6a01 8801 6b02 7204 7c01  ......j...k.r.|.
-0000d050: 7c02 9302 7104 5300 7226 0000 0029 0272  |...q.S.r&...).r
-0000d060: 3601 0000 72c8 0000 0072 0602 0000 2903  6...r....r....).
-0000d070: da0d 6578 705f 636f 6e64 6974 696f 6eda  ..exp_condition.
-0000d080: 0965 7870 5f76 616c 7565 7256 0000 0072  .exp_valuerV...r
-0000d090: 2600 0000 7227 0000 0072 9700 0000 e106  &...r'...r......
-0000d0a0: 0000 7306 0000 0006 0206 0114 fe7a 2e54  ..s..........z.T
-0000d0b0: 6162 6c65 4469 6374 2e66 696c 7465 725f  ableDict.filter_
-0000d0c0: 636f 6e64 6974 696f 6e2e 3c6c 6f63 616c  condition.<local
-0000d0d0: 733e 2e3c 6469 6374 636f 6d70 3e63 0100  s>.<dictcomp>c..
-0000d0e0: 0000 0000 0000 0000 0000 0300 0000 0500  ................
-0000d0f0: 0000 1300 0000 7322 0000 0069 007c 005d  ......s"...i.|.]
-0000d100: 1a5c 027d 017d 027c 0188 00a0 00a1 0076  .\.}.}.|.......v
-0000d110: 0072 047c 017c 0293 0271 0453 0072 2600  .r.|.|...q.S.r&.
-0000d120: 0000 7204 0200 0072 0602 0000 2901 da0e  ..r....r....)...
-0000d130: 6669 6c74 6572 6564 5f74 6162 6c65 7226  filtered_tabler&
-0000d140: 0000 0072 2700 0000 7297 0000 00ec 0600  ...r'...r.......
-0000d150: 0073 0600 0000 0602 0601 0cfe 7207 0200  .s..........r...
-0000d160: 0029 0a72 8100 0000 7282 0000 0072 5101  .).r....r....rQ.
-0000d170: 0000 72cb 0000 0072 da00 0000 72fd 0100  ..r....r....r...
-0000d180: 0072 4001 0000 7200 0200 0072 0102 0000  .r@...r....r....
-0000d190: 7236 0100 0029 0372 5600 0000 7209 0200  r6...).rV...r...
-0000d1a0: 0072 0502 0000 7226 0000 0029 0472 0a02  .r....r&...).r..
-0000d1b0: 0000 720b 0200 0072 0c02 0000 7256 0000  ..r....r....rV..
-0000d1c0: 0072 2700 0000 da10 6669 6c74 6572 5f63  .r'.....filter_c
-0000d1d0: 6f6e 6469 7469 6f6e d406 0000 7320 0000  ondition....s ..
-0000d1e0: 0000 090c 0210 020e 0206 fe06 0502 0102  ................
-0000d1f0: 0104 0104 0104 0104 010a 0208 fe04 fa08  ................
-0000d200: 0d7a 1a54 6162 6c65 4469 6374 2e66 696c  .z.TableDict.fil
-0000d210: 7465 725f 636f 6e64 6974 696f 6e29 0172  ter_condition).r
-0000d220: 1900 0000 6301 0000 0000 0000 0000 0000  ....c...........
-0000d230: 0003 0000 0005 0000 0043 0000 0073 6c00  .........C...sl.
-0000d240: 0000 6401 7d01 7c00 6a00 7234 6402 6403  ..d.}.|.j.r4d.d.
-0000d250: 8400 7c00 a001 a100 4400 8301 7d01 7402  ..|.....D...}.t.
-0000d260: a003 6404 6405 8400 7c01 a004 a100 4400  ..d.d...|.....D.
-0000d270: 8301 a101 7d01 6406 6403 8400 7c00 a001  ....}.d.d...|...
-0000d280: a100 4400 8301 7d02 7402 6a05 6407 6405  ..D...}.t.j.d.d.
-0000d290: 8400 7c02 a004 a100 4400 8301 6408 6409  ..|.....D...d.d.
-0000d2a0: 8d02 6a06 7d02 7c02 7c01 6602 5300 290a  ..j.}.|.|.f.S.).
-0000d2b0: 7a7c 5265 7475 726e 2061 206e 756d 7079  z|Return a numpy
-0000d2c0: 206e 6461 7272 6179 2066 726f 6d20 7468   ndarray from th
-0000d2d0: 6520 7072 6570 726f 6365 7373 696e 6720  e preprocessing 
-0000d2e0: 6f66 2074 6865 2074 6162 6c65 5f64 6963  of the table_dic
-0000d2f0: 7420 6f62 6a65 6374 2c20 7265 6164 7920  t object, ready 
-0000d300: 666f 7220 7072 6f6a 6563 7469 6f6e 2069  for projection i
-0000d310: 6e74 6f20 6120 6c6f 7765 7220 6469 6d65  nto a lower dime
-0000d320: 6e73 696f 6e61 6c20 7370 6163 652e 4e63  nsional space.Nc
-0000d330: 0100 0000 0000 0000 0000 0000 0300 0000  ................
-0000d340: 0500 0000 5300 0000 731c 0000 0069 007c  ....S...s....i.|
-0000d350: 005d 145c 027d 017d 027c 017c 026a 0064  .].\.}.}.|.|.j.d
-0000d360: 0019 0093 0271 0453 00a9 0129 0272 0100  .....q.S...).r..
-0000d370: 0000 7293 0100 0072 9000 0000 a903 724a  ..r....r......rJ
-0000d380: 0000 0072 eb00 0000 da01 7672 2600 0000  ...r......vr&...
-0000d390: 7226 0000 0072 2700 0000 7297 0000 00fb  r&...r'...r.....
-0000d3a0: 0600 0072 4d00 0000 7a31 5461 626c 6544  ...rM...z1TableD
-0000d3b0: 6963 742e 5f70 7265 7061 7265 5f70 726f  ict._prepare_pro
-0000d3c0: 6a65 6374 696f 6e2e 3c6c 6f63 616c 733e  jection.<locals>
-0000d3d0: 2e3c 6469 6374 636f 6d70 3e63 0100 0000  .<dictcomp>c....
-0000d3e0: 0000 0000 0000 0000 0200 0000 0300 0000  ................
-0000d3f0: 5300 0000 7310 0000 0067 007c 005d 087d  S...s....g.|.].}
-0000d400: 017c 0191 0271 0453 0072 2600 0000 7226  .|...q.S.r&...r&
-0000d410: 0000 0029 0272 4a00 0000 72f7 0000 0072  ...).rJ...r....r
-0000d420: 2600 0000 7226 0000 0072 2700 0000 724c  &...r&...r'...rL
-0000d430: 0000 00fc 0600 0072 4d00 0000 7a31 5461  .......rM...z1Ta
-0000d440: 626c 6544 6963 742e 5f70 7265 7061 7265  bleDict._prepare
-0000d450: 5f70 726f 6a65 6374 696f 6e2e 3c6c 6f63  _projection.<loc
-0000d460: 616c 733e 2e3c 6c69 7374 636f 6d70 3e63  als>.<listcomp>c
-0000d470: 0100 0000 0000 0000 0000 0000 0300 0000  ................
-0000d480: 0700 0000 5300 0000 7320 0000 0069 007c  ....S...s ...i.|
-0000d490: 005d 185c 027d 017d 027c 0174 006a 017c  .].\.}.}.|.t.j.|
-0000d4a0: 0264 0064 018d 0293 0271 0453 0029 0272  .d.d.....q.S.).r
-0000d4b0: 0100 0000 72ab 0000 0029 0272 dd00 0000  ....r....).r....
-0000d4c0: da04 6d65 616e 720f 0200 0072 2600 0000  ..meanr....r&...
-0000d4d0: 7226 0000 0072 2700 0000 7297 0000 00fe  r&...r'...r.....
-0000d4e0: 0600 0072 4d00 0000 6301 0000 0000 0000  ...rM...c.......
-0000d4f0: 0000 0000 0002 0000 0005 0000 0053 0000  .............S..
-0000d500: 0073 2400 0000 6700 7c00 5d1c 7d01 7400  .s$...g.|.].}.t.
-0000d510: a001 7c01 a101 6400 6400 8502 7400 6a02  ..|...d.d...t.j.
-0000d520: 6602 1900 9102 7104 5300 7225 0100 0029  f.....q.S.r%...)
-0000d530: 0372 dd00 0000 72de 0000 00da 076e 6577  .r....r......new
-0000d540: 6178 6973 2902 724a 0000 00da 0365 7870  axis).rJ.....exp
-0000d550: 7226 0000 0072 2600 0000 7227 0000 0072  r&...r&...r'...r
-0000d560: 4c00 0000 0007 0000 724d 0000 0072 3100  L.......rM...r1.
-0000d570: 0000 72ab 0000 0029 0772 0002 0000 72cb  ..r....).r....r.
-0000d580: 0000 0072 dd00 0000 72de 0000 0072 c800  ...r....r....r..
-0000d590: 0000 7299 0100 0072 c100 0000 2903 7256  ..r....r....).rV
-0000d5a0: 0000 00da 066c 6162 656c 73da 0158 7226  .....labels..Xr&
-0000d5b0: 0000 0072 2600 0000 7227 0000 00da 135f  ...r&...r'....._
-0000d5c0: 7072 6570 6172 655f 7072 6f6a 6563 7469  prepare_projecti
-0000d5d0: 6f6e f506 0000 7312 0000 0000 0204 0306  on....s.........
-0000d5e0: 0112 0118 0212 0104 0112 ff08 047a 1d54  .............z.T
-0000d5f0: 6162 6c65 4469 6374 2e5f 7072 6570 6172  ableDict._prepar
-0000d600: 655f 7072 6f6a 6563 7469 6f6e 7292 0000  e_projectionr...
-0000d610: 0029 04da 0f70 726f 6a65 6374 696f 6e5f  .)...projection_
-0000d620: 7479 7065 72de 0100 00da 066b 6572 6e65  typer......kerne
-0000d630: 6c72 1900 0000 6304 0000 0000 0000 0000  lr....c.........
-0000d640: 0000 0006 0000 0004 0000 0043 0000 0073  ...........C...s
-0000d650: 7000 0000 7c00 a000 a100 5c02 7d04 7d05  p...|.....\.}.}.
-0000d660: 7c01 6401 6b02 7222 7401 6a02 7c02 6402  |.d.k.r"t.j.|.d.
-0000d670: 8d01 7d01 6e2a 7c01 6403 6b02 7238 7403  ..}.n*|.d.k.r8t.
-0000d680: 7c02 7c03 6404 8d02 7d01 6e14 7c01 6405  |.|.d...}.n.|.d.
-0000d690: 6b02 724c 7404 6a05 7c02 6402 8d01 7d01  k.rLt.j.|.d...}.
-0000d6a0: 7c01 a006 7c04 a101 7d04 7c05 6406 7501  |...|...}.|.d.u.
-0000d6b0: 7268 7c04 7c05 7c01 6603 5300 7c04 7c01  rh|.|.|.f.S.|.|.
-0000d6c0: 6602 5300 2907 6156 0200 0052 6574 7572  f.S.).aV...Retur
-0000d6d0: 6e20 6120 7472 6169 6e69 6e67 2073 6574  n a training set
-0000d6e0: 2067 656e 6572 6174 6564 2066 726f 6d20   generated from 
-0000d6f0: 7468 6520 3244 206f 7269 6769 6e61 6c20  the 2D original 
-0000d700: 6461 7461 2028 7469 6d65 2078 2066 6561  data (time x fea
-0000d710: 7475 7265 7329 2061 6e64 2061 2073 7065  tures) and a spe
-0000d720: 6369 6669 6564 2070 726f 6a65 6374 696f  cified projectio
-0000d730: 6e20 746f 2061 6e20 6e5f 636f 6d70 6f6e  n to an n_compon
-0000d740: 656e 7473 2073 7061 6365 2e0a 0a20 2020  ents space...   
-0000d750: 2020 2020 2054 6865 2073 616d 706c 6520       The sample 
-0000d760: 7061 7261 6d65 7465 7220 616c 6c6f 7773  parameter allows
-0000d770: 2074 6865 2075 7365 7220 746f 2072 616e   the user to ran
-0000d780: 646f 6d6c 7920 7069 636b 2061 2073 7562  domly pick a sub
-0000d790: 7365 7420 6f66 2074 6865 2064 6174 6120  set of the data 
-0000d7a0: 666f 7220 7065 7266 6f72 6d61 6e63 6520  for performance 
-0000d7b0: 6f72 2076 6973 7561 6c69 7a61 7469 6f6e  or visualization
-0000d7c0: 2072 6561 736f 6e73 2e20 466f 7220 696e   reasons. For in
-0000d7d0: 7465 726e 616c 2075 7361 6765 206f 6e6c  ternal usage onl
-0000d7e0: 792e 0a0a 2020 2020 2020 2020 4172 6773  y...        Args
-0000d7f0: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
-0000d800: 6f6a 6563 7469 6f6e 5f74 7970 6520 2873  ojection_type (s
-0000d810: 7472 293a 2050 726f 6a65 6374 696f 6e20  tr): Projection 
-0000d820: 746f 2062 6520 7573 6564 2e0a 2020 2020  to be used..    
-0000d830: 2020 2020 2020 2020 6e5f 636f 6d70 6f6e          n_compon
-0000d840: 656e 7473 2028 696e 7429 3a20 4e75 6d62  ents (int): Numb
-0000d850: 6572 206f 6620 636f 6d70 6f6e 656e 7473  er of components
-0000d860: 2074 6f20 7072 6f6a 6563 7420 746f 2e0a   to project to..
-0000d870: 2020 2020 2020 2020 2020 2020 6b65 726e              kern
-0000d880: 656c 2028 7374 7229 3a20 4b65 726e 656c  el (str): Kernel
-0000d890: 2074 6f20 6265 2075 7365 6420 666f 7220   to be used for 
-0000d8a0: 7468 6520 7261 6e64 6f6d 2061 6e64 2050  the random and P
-0000d8b0: 4341 2061 6c67 6f72 6974 686d 732e 0a0a  CA algorithms...
-0000d8c0: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-0000d8d0: 0a20 2020 2020 2020 2020 2020 2074 7570  .            tup
-0000d8e0: 6c65 3a20 5475 706c 6520 636f 6e74 6169  le: Tuple contai
-0000d8f0: 6e69 6e67 2070 726f 6a65 6374 6564 2064  ning projected d
-0000d900: 6174 6120 616e 6420 7072 6f6a 6563 7469  ata and projecti
-0000d910: 6f6e 2074 7970 652e 0a20 2020 2020 2020  on type..       
-0000d920: 20da 0672 616e 646f 6da9 0172 de01 0000   ..random..r....
-0000d930: da03 7063 61a9 0272 de01 0000 7218 0200  ..pca..r....r...
-0000d940: 00da 0475 6d61 704e 2907 7216 0200 0072  ...umapN).r....r
-0000d950: 0600 0000 da18 4761 7573 7369 616e 5261  ......GaussianRa
-0000d960: 6e64 6f6d 5072 6f6a 6563 7469 6f6e 7207  ndomProjectionr.
-0000d970: 0000 0072 1d02 0000 da04 554d 4150 da0d  ...r......UMAP..
-0000d980: 6669 745f 7472 616e 7366 6f72 6d29 0672  fit_transform).r
-0000d990: 5600 0000 7217 0200 0072 de01 0000 7218  V...r....r....r.
-0000d9a0: 0200 0072 1502 0000 7214 0200 0072 2600  ...r....r....r&.
-0000d9b0: 0000 7226 0000 0072 2700 0000 da0b 5f70  ..r&...r'....._p
-0000d9c0: 726f 6a65 6374 696f 6e05 0700 0073 1a00  rojection....s..
-0000d9d0: 0000 0012 0c02 0801 0401 02ff 0803 0801  ................
-0000d9e0: 0e01 0801 0c02 0a02 0801 0a02 7a15 5461  ............z.Ta
-0000d9f0: 626c 6544 6963 742e 5f70 726f 6a65 6374  bleDict._project
-0000da00: 696f 6e72 d501 0000 2903 72de 0100 0072  ionr....).r....r
-0000da10: 1802 0000 7219 0000 0063 0300 0000 0000  ....r....c......
-0000da20: 0000 0000 0000 0300 0000 0500 0000 4300  ..............C.
-0000da30: 0000 7310 0000 007c 006a 0064 017c 017c  ..s....|.j.d.|.|
-0000da40: 0264 028d 0353 0029 0361 1702 0000 5265  .d...S.).a....Re
-0000da50: 7475 726e 2061 2074 7261 696e 696e 6720  turn a training 
-0000da60: 7365 7420 6765 6e65 7261 7465 6420 6672  set generated fr
-0000da70: 6f6d 2074 6865 2032 4420 6f72 6967 696e  om the 2D origin
-0000da80: 616c 2064 6174 6120 2874 696d 6520 7820  al data (time x 
-0000da90: 6665 6174 7572 6573 2920 616e 6420 6120  features) and a 
-0000daa0: 7261 6e64 6f6d 2070 726f 6a65 6374 696f  random projectio
-0000dab0: 6e20 746f 2061 206e 5f63 6f6d 706f 6e65  n to a n_compone
-0000dac0: 6e74 7320 7370 6163 652e 0a0a 2020 2020  nts space...    
-0000dad0: 2020 2020 5468 6520 7361 6d70 6c65 2070      The sample p
-0000dae0: 6172 616d 6574 6572 2061 6c6c 6f77 7320  arameter allows 
-0000daf0: 7468 6520 7573 6572 2074 6f20 7261 6e64  the user to rand
-0000db00: 6f6d 6c79 2070 6963 6b20 6120 7375 6273  omly pick a subs
-0000db10: 6574 206f 6620 7468 6520 6461 7461 2066  et of the data f
-0000db20: 6f72 0a20 2020 2020 2020 2070 6572 666f  or.        perfo
-0000db30: 726d 616e 6365 206f 7220 7669 7375 616c  rmance or visual
-0000db40: 697a 6174 696f 6e20 7265 6173 6f6e 732e  ization reasons.
-0000db50: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
-0000db60: 2020 2020 2020 2020 2020 2020 6e5f 636f              n_co
-0000db70: 6d70 6f6e 656e 7473 2028 696e 7429 3a20  mponents (int): 
-0000db80: 4e75 6d62 6572 206f 6620 636f 6d70 6f6e  Number of compon
-0000db90: 656e 7473 2074 6f20 7072 6f6a 6563 7420  ents to project 
-0000dba0: 746f 2e20 4465 6661 756c 7420 6973 2032  to. Default is 2
-0000dbb0: 2e0a 2020 2020 2020 2020 2020 2020 6b65  ..            ke
-0000dbc0: 726e 656c 2028 7374 7229 3a20 4b65 726e  rnel (str): Kern
-0000dbd0: 656c 2074 6f20 6265 2075 7365 6420 666f  el to be used fo
-0000dbe0: 7220 7072 6f6a 6563 7469 6f6e 732e 2044  r projections. D
-0000dbf0: 6566 6175 6c74 7320 746f 206c 696e 6561  efaults to linea
-0000dc00: 722e 0a0a 2020 2020 2020 2020 5265 7475  r...        Retu
-0000dc10: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
-0000dc20: 2074 7570 6c65 3a20 5475 706c 6520 636f   tuple: Tuple co
-0000dc30: 6e74 6169 6e69 6e67 2070 726f 6a65 6374  ntaining project
-0000dc40: 6564 2064 6174 6120 616e 6420 7072 6f6a  ed data and proj
-0000dc50: 6563 7469 6f6e 2074 7970 652e 0a20 2020  ection type..   
-0000dc60: 2020 2020 2072 1902 0000 721c 0200 00a9       r....r.....
-0000dc70: 0172 2102 0000 a903 7256 0000 0072 de01  .r!.....rV...r..
-0000dc80: 0000 7218 0200 0072 2600 0000 7226 0000  ..r....r&...r&..
-0000dc90: 0072 2700 0000 7206 0000 0029 0700 0073  .r'...r....)...s
-0000dca0: 0200 0000 000f 7a1b 5461 626c 6544 6963  ......z.TableDic
-0000dcb0: 742e 7261 6e64 6f6d 5f70 726f 6a65 6374  t.random_project
-0000dcc0: 696f 6e63 0300 0000 0000 0000 0000 0000  ionc............
-0000dcd0: 0300 0000 0500 0000 4300 0000 7310 0000  ........C...s...
-0000dce0: 007c 006a 0064 017c 017c 0264 028d 0353  .|.j.d.|.|.d...S
-0000dcf0: 0029 0361 1402 0000 5265 7475 726e 2061  .).a....Return a
-0000dd00: 2074 7261 696e 696e 6720 7365 7420 6765   training set ge
-0000dd10: 6e65 7261 7465 6420 6672 6f6d 2074 6865  nerated from the
-0000dd20: 2032 4420 6f72 6967 696e 616c 2064 6174   2D original dat
-0000dd30: 6120 2874 696d 6520 7820 6665 6174 7572  a (time x featur
-0000dd40: 6573 2920 616e 6420 6120 5043 4120 7072  es) and a PCA pr
-0000dd50: 6f6a 6563 7469 6f6e 2074 6f20 6120 6e5f  ojection to a n_
-0000dd60: 636f 6d70 6f6e 656e 7473 2073 7061 6365  components space
-0000dd70: 2e0a 0a20 2020 2020 2020 2054 6865 2073  ...        The s
-0000dd80: 616d 706c 6520 7061 7261 6d65 7465 7220  ample parameter 
-0000dd90: 616c 6c6f 7773 2074 6865 2075 7365 7220  allows the user 
-0000dda0: 746f 2072 616e 646f 6d6c 7920 7069 636b  to randomly pick
-0000ddb0: 2061 2073 7562 7365 7420 6f66 2074 6865   a subset of the
-0000ddc0: 2064 6174 6120 666f 720a 2020 2020 2020   data for.      
-0000ddd0: 2020 7065 7266 6f72 6d61 6e63 6520 6f72    performance or
-0000dde0: 2076 6973 7561 6c69 7a61 7469 6f6e 2072   visualization r
-0000ddf0: 6561 736f 6e73 2e0a 0a20 2020 2020 2020  easons...       
-0000de00: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
-0000de10: 2020 206e 5f63 6f6d 706f 6e65 6e74 7320     n_components 
-0000de20: 2869 6e74 293a 204e 756d 6265 7220 6f66  (int): Number of
-0000de30: 2063 6f6d 706f 6e65 6e74 7320 746f 2070   components to p
-0000de40: 726f 6a65 6374 2074 6f2e 2044 6566 6175  roject to. Defau
-0000de50: 6c74 2069 7320 322e 0a20 2020 2020 2020  lt is 2..       
-0000de60: 2020 2020 206b 6572 6e65 6c20 2873 7472       kernel (str
-0000de70: 293a 204b 6572 6e65 6c20 746f 2062 6520  ): Kernel to be 
-0000de80: 7573 6564 2066 6f72 2070 726f 6a65 6374  used for project
-0000de90: 696f 6e73 2e20 4465 6661 756c 7473 2074  ions. Defaults t
-0000dea0: 6f20 6c69 6e65 6172 2e0a 0a20 2020 2020  o linear...     
-0000deb0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-0000dec0: 2020 2020 2020 2020 7475 706c 653a 2054          tuple: T
-0000ded0: 7570 6c65 2063 6f6e 7461 696e 696e 6720  uple containing 
-0000dee0: 7072 6f6a 6563 7465 6420 6461 7461 2061  projected data a
-0000def0: 6e64 2070 726f 6a65 6374 696f 6e20 7479  nd projection ty
-0000df00: 7065 2e0a 2020 2020 2020 2020 721b 0200  pe..        r...
-0000df10: 0072 1c02 0000 7222 0200 0072 2302 0000  .r....r"...r#...
-0000df20: 7226 0000 0072 2600 0000 7227 0000 0072  r&...r&...r'...r
-0000df30: 1b02 0000 3a07 0000 7302 0000 0000 0d7a  ....:...s......z
-0000df40: 0d54 6162 6c65 4469 6374 2e70 6361 2902  .TableDict.pca).
-0000df50: 72de 0100 0072 1900 0000 6302 0000 0000  r....r....c.....
-0000df60: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
-0000df70: 0000 0073 0e00 0000 7c00 6a00 6401 7c01  ...s....|.j.d.|.
-0000df80: 6402 8d02 5300 2903 611f 0200 0052 6574  d...S.).a....Ret
-0000df90: 7572 6e20 6120 7472 6169 6e69 6e67 2073  urn a training s
-0000dfa0: 6574 2067 656e 6572 6174 6564 2066 726f  et generated fro
-0000dfb0: 6d20 7468 6520 3244 206f 7269 6769 6e61  m the 2D origina
-0000dfc0: 6c20 6461 7461 2028 7469 6d65 2078 2066  l data (time x f
-0000dfd0: 6561 7475 7265 7329 2061 6e64 2061 2050  eatures) and a P
-0000dfe0: 4341 2070 726f 6a65 6374 696f 6e20 746f  CA projection to
-0000dff0: 2061 206e 5f63 6f6d 706f 6e65 6e74 7320   a n_components 
-0000e000: 7370 6163 652e 0a0a 2020 2020 2020 2020  space...        
-0000e010: 5468 6520 7361 6d70 6c65 2070 6172 616d  The sample param
-0000e020: 6574 6572 2061 6c6c 6f77 7320 7468 6520  eter allows the 
-0000e030: 7573 6572 2074 6f20 7261 6e64 6f6d 6c79  user to randomly
-0000e040: 2070 6963 6b20 6120 7375 6273 6574 206f   pick a subset o
-0000e050: 6620 7468 6520 6461 7461 2066 6f72 0a20  f the data for. 
-0000e060: 2020 2020 2020 2070 6572 666f 726d 616e         performan
-0000e070: 6365 206f 7220 7669 7375 616c 697a 6174  ce or visualizat
-0000e080: 696f 6e20 7265 6173 6f6e 732e 0a0a 2020  ion reasons...  
-0000e090: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-0000e0a0: 2020 2020 2020 2020 6e5f 636f 6d70 6f6e          n_compon
-0000e0b0: 656e 7473 2028 696e 7429 3a20 4e75 6d62  ents (int): Numb
-0000e0c0: 6572 206f 6620 636f 6d70 6f6e 656e 7473  er of components
-0000e0d0: 2074 6f20 7072 6f6a 6563 7420 746f 2e20   to project to. 
-0000e0e0: 4465 6661 756c 7420 6973 2032 2e0a 2020  Default is 2..  
-0000e0f0: 2020 2020 2020 2020 2020 7065 7270 6c65            perple
-0000e100: 7869 7479 2028 696e 7429 3a20 5065 7270  xity (int): Perp
-0000e110: 6c65 7869 7479 2070 6172 616d 6574 6572  lexity parameter
-0000e120: 2066 6f72 2074 6865 2074 2d53 4e45 2061   for the t-SNE a
-0000e130: 6c67 6f72 6974 686d 2e20 4465 6661 756c  lgorithm. Defaul
-0000e140: 7420 6973 2033 302e 0a0a 2020 2020 2020  t is 30...      
-0000e150: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-0000e160: 2020 2020 2020 2074 7570 6c65 3a20 5475         tuple: Tu
-0000e170: 706c 6520 636f 6e74 6169 6e69 6e67 2070  ple containing p
-0000e180: 726f 6a65 6374 6564 2064 6174 6120 616e  rojected data an
-0000e190: 6420 7072 6f6a 6563 7469 6f6e 2074 7970  d projection typ
-0000e1a0: 652e 0a0a 2020 2020 2020 2020 721d 0200  e...        r...
-0000e1b0: 0072 1a02 0000 7222 0200 0029 0272 5600  .r....r"...).rV.
-0000e1c0: 0000 72de 0100 0072 2600 0000 7226 0000  ..r....r&...r&..
-0000e1d0: 0072 2700 0000 721d 0200 0049 0700 0073  .r'...r....I...s
-0000e1e0: 0800 0000 0011 0401 0201 02fe 7a0e 5461  ............z.Ta
-0000e1f0: 626c 6544 6963 742e 756d 6170 2902 7247  bleDict.umap).rG
-0000e200: 0100 0072 1900 0000 6302 0000 0000 0000  ...r....c.......
-0000e210: 0000 0000 0005 0000 0008 0000 0003 0000  ................
-0000e220: 0073 6e00 0000 7c00 a000 a100 7d02 7c02  .sn...|.....}.|.
-0000e230: a001 a100 4400 5d3e 5c02 7d03 7d04 7402  ....D.]>\.}.}.t.
-0000e240: 6a03 a004 7c04 6a05 7c01 a102 8900 7c04  j...|.j.|.....|.
-0000e250: 6a06 6401 6401 8502 8700 6601 6402 6403  j.d.d.....f.d.d.
-0000e260: 8408 7c04 6a05 4400 8301 6602 1900 7c02  ..|.j.D...f...|.
-0000e270: 7c03 3c00 7110 7407 7c02 7c00 6a08 7c00  |.<.q.t.|.|.j.|.
-0000e280: 6a09 7c00 6a0a 7c00 6a0b 7c00 6a0c 6404  j.|.j.|.j.|.j.d.
-0000e290: 8d06 5300 2905 6179 0100 0046 696c 7465  ..S.).ay...Filte
-0000e2a0: 7220 6120 5461 626c 6544 6963 7420 6f62  r a TableDict ob
-0000e2b0: 6a65 6374 2074 6f20 6b65 6570 206f 6e6c  ject to keep onl
-0000e2c0: 7920 7468 6f73 6520 636f 6c75 6d6e 7320  y those columns 
-0000e2d0: 7265 6c61 7465 6420 746f 2074 6865 2073  related to the s
-0000e2e0: 656c 6563 7465 6420 6964 2e0a 0a20 2020  elected id...   
-0000e2f0: 2020 2020 204c 6561 7665 206c 6162 656c       Leave label
-0000e300: 7320 756e 746f 7563 6865 6420 6966 2070  s untouched if p
-0000e310: 7265 7365 6e74 2e0a 0a20 2020 2020 2020  resent...       
-0000e320: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
-0000e330: 2020 2073 656c 6563 7465 645f 6964 2028     selected_id (
-0000e340: 7374 7229 3a20 7365 6c65 6374 2061 2073  str): select a s
-0000e350: 696e 676c 6520 616e 696d 616c 206f 6e20  ingle animal on 
-0000e360: 6d75 6c74 6920 616e 696d 616c 2073 6574  multi animal set
-0000e370: 7469 6e67 732e 2044 6566 6175 6c74 7320  tings. Defaults 
-0000e380: 746f 204e 6f6e 6520 2861 6c6c 2061 6e69  to None (all ani
-0000e390: 6d61 6c73 2061 7265 2070 726f 6365 7373  mals are process
-0000e3a0: 6564 292e 0a0a 2020 2020 2020 2020 5265  ed)...        Re
-0000e3b0: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
-0000e3c0: 2020 2074 6162 6c65 5f64 6963 743a 2046     table_dict: F
-0000e3d0: 696c 7465 7265 6420 5461 626c 6544 6963  iltered TableDic
-0000e3e0: 7420 6f62 6a65 6374 2c20 6b65 6570 696e  t object, keepin
-0000e3f0: 6720 6f6e 6c79 2074 6865 2073 656c 6563  g only the selec
-0000e400: 7465 6420 616e 696d 616c 2e0a 2020 2020  ted animal..    
-0000e410: 2020 2020 4e63 0100 0000 0000 0000 0000      Nc..........
-0000e420: 0000 0200 0000 0400 0000 1300 0000 7318  ..............s.
-0000e430: 0000 0067 007c 005d 107d 017c 0188 0076  ...g.|.].}.|...v
-0000e440: 0072 047c 0191 0271 0453 0072 2600 0000  .r.|...q.S.r&...
-0000e450: 7226 0000 0029 0272 4a00 0000 da03 6270  r&...).rJ.....bp
-0000e460: 61a9 01da 0f63 6f6c 756d 6e73 5f74 6f5f  a....columns_to_
-0000e470: 6b65 6570 7226 0000 0072 2700 0000 724c  keepr&...r'...rL
-0000e480: 0000 006e 0700 0072 4d00 0000 7a27 5461  ...n...rM...z'Ta
-0000e490: 626c 6544 6963 742e 6669 6c74 6572 5f69  bleDict.filter_i
-0000e4a0: 642e 3c6c 6f63 616c 733e 2e3c 6c69 7374  d.<locals>.<list
-0000e4b0: 636f 6d70 3e29 0572 af00 0000 7263 0000  comp>).r....rc..
-0000e4c0: 0072 4801 0000 7249 0100 0072 3800 0000  .rH...rI...r8...
-0000e4d0: 290d 72cc 0000 0072 cb00 0000 7281 0000  ).r....r....r...
-0000e4e0: 0072 8200 0000 720d 0100 0072 b700 0000  .r....r....r....
-0000e4f0: 72c3 0000 0072 da00 0000 72fd 0100 0072  r....r....r....r
-0000e500: 4001 0000 7200 0200 0072 0102 0000 7236  @...r....r....r6
-0000e510: 0100 0029 0572 5600 0000 7247 0100 0072  ...).rV...rG...r
-0000e520: 6001 0000 72e4 0000 0072 f700 0000 7226  `...r....r....r&
-0000e530: 0000 0072 2502 0000 7227 0000 00da 0966  ...r%...r'.....f
-0000e540: 696c 7465 725f 6964 5f07 0000 731c 0000  ilter_id_...s...
-0000e550: 0000 0b08 0110 0110 0104 011a ff0a 0402  ................
-0000e560: 0102 0104 0104 0104 0104 0104 fa7a 1354  .............z.T
-0000e570: 6162 6c65 4469 6374 2e66 696c 7465 725f  ableDict.filter_
-0000e580: 6964 a901 da0c 6967 6e6f 7265 5f69 6e64  id....ignore_ind
-0000e590: 6578 6301 0000 0000 0000 0001 0000 000d  exc.............
-0000e5a0: 0000 0007 0000 0007 0000 0073 2201 0000  ...........s"...
-0000e5b0: 7400 a001 7c00 a101 6701 7402 7c02 8301  t...|...g.t.|...
-0000e5c0: 1700 7d02 7403 7402 8301 7d03 7c02 4400  ..}.t.t...}.|.D.
-0000e5d0: 5d24 7d04 7c04 a004 a100 4400 5d16 5c02  ]$}.|.....D.].\.
-0000e5e0: 7d05 7d06 7c03 7c05 1900 a005 7c06 a101  }.}.|.|.....|...
-0000e5f0: 0100 712c 7120 7406 7c00 6a07 6701 6401  ..q,q t.|.j.g.d.
-0000e600: 6402 8400 7c02 4400 8301 1700 8301 7d07  d...|.D.......}.
-0000e610: 7408 8700 6601 6403 6404 8408 7c03 a004  t...f.d.d...|...
-0000e620: a100 4400 8301 6405 7c00 6a09 7c07 7c00  ..D...d.|.j.|.|.
-0000e630: 6a0a 6406 8d05 7d08 7c08 a004 a100 4400  j.d...}.|.....D.
-0000e640: 5d84 5c02 7d05 7d09 6407 6402 8400 7c09  ].\.}.}.d.d...|.
-0000e650: 6a0b 4400 8301 7d0a 740c 7c0a 8301 6408  j.D...}.t.|...d.
-0000e660: 6b04 7290 740c 7c0a 6408 1900 8301 6409  k.r.t.|.d.....d.
-0000e670: 6b02 72cc 7c0a 6408 1900 6e08 7c0a 6408  k.r.|.d...n.|.d.
-0000e680: 1900 6701 7d0b 7c09 6a0d 640a 640a 8502  ..g.}.|.j.d.d...
-0000e690: 7c0b 6602 1900 6a0e 640a 640a 8502 6408  |.f...j.d.d...d.
-0000e6a0: 6602 1900 7d0c 7c09 6a0f 7c0a 6409 640b  f...}.|.j.|.d.d.
-0000e6b0: 8d02 7c08 7c05 3c00 7c0c 7c08 7c05 1900  ..|.|.<.|.|.|...
-0000e6c0: 640c 3c00 7190 7c00 6a10 7c08 5f10 7c08  d.<.q.|.j.|._.|.
-0000e6d0: 5300 290d 61ac 0100 0054 616b 6520 6120  S.).a....Take a 
-0000e6e0: 6e75 6d62 6572 206f 6620 7461 626c 655f  number of table_
-0000e6f0: 6469 6374 206f 626a 6563 7473 2061 6e64  dict objects and
-0000e700: 206d 6572 6765 7320 7468 656d 2074 6f20   merges them to 
-0000e710: 7468 6520 6375 7272 656e 7420 6f6e 652e  the current one.
-0000e720: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-0000e730: 7320 6120 7461 626c 655f 6469 6374 206f  s a table_dict o
-0000e740: 626a 6563 7420 6f66 2074 7970 6520 276d  bject of type 'm
-0000e750: 6572 6765 6427 2e0a 2020 2020 2020 2020  erged'..        
-0000e760: 4f6e 6c79 2061 6e6e 6f74 6174 696f 6e73  Only annotations
-0000e770: 206f 6620 7468 6520 6669 7273 7420 7461   of the first ta
-0000e780: 626c 655f 6469 6374 206f 626a 6563 7420  ble_dict object 
-0000e790: 6172 6520 6b65 7074 2e0a 0a20 2020 2020  are kept...     
-0000e7a0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-0000e7b0: 2020 2020 202a 6172 6773 2028 7461 626c       *args (tabl
-0000e7c0: 655f 6469 6374 293a 2074 6162 6c65 5f64  e_dict): table_d
-0000e7d0: 6963 7420 6f62 6a65 6374 7320 746f 2062  ict objects to b
-0000e7e0: 6520 6d65 7267 6564 2e0a 2020 2020 2020  e merged..      
-0000e7f0: 2020 2020 2020 6967 6e6f 7265 5f69 6e64        ignore_ind
-0000e800: 6578 2028 626f 6f6c 293a 2069 676e 6f72  ex (bool): ignor
-0000e810: 6520 696e 6465 7820 7768 656e 206d 6572  e index when mer
-0000e820: 6769 6e67 2e20 4465 6661 756c 7473 2074  ging. Defaults t
-0000e830: 6f20 4661 6c73 652e 0a0a 2020 2020 2020  o False...      
-0000e840: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-0000e850: 2020 2020 2020 2074 6162 6c65 5f64 6963         table_dic
-0000e860: 743a 204d 6572 6765 6420 7461 626c 655f  t: Merged table_
-0000e870: 6469 6374 206f 626a 6563 742e 0a20 2020  dict object..   
-0000e880: 2020 2020 2063 0100 0000 0000 0000 0000       c..........
-0000e890: 0000 0200 0000 0300 0000 5300 0000 7312  ..........S...s.
-0000e8a0: 0000 0067 007c 005d 0a7d 017c 016a 0091  ...g.|.].}.|.j..
-0000e8b0: 0271 0453 0072 2600 0000 2901 7200 0200  .q.S.r&...).r...
-0000e8c0: 0029 0272 4a00 0000 da07 7461 6264 6963  .).rJ.....tabdic
-0000e8d0: 7472 2600 0000 7226 0000 0072 2700 0000  tr&...r&...r'...
-0000e8e0: 724c 0000 008e 0700 0072 4d00 0000 7a23  rL.......rM...z#
-0000e8f0: 5461 626c 6544 6963 742e 6d65 7267 652e  TableDict.merge.
-0000e900: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-0000e910: 6d70 3e63 0100 0000 0000 0000 0000 0000  mp>c............
-0000e920: 0300 0000 0900 0000 1300 0000 7324 0000  ............s$..
-0000e930: 0069 007c 005d 1c5c 027d 017d 027c 0174  .i.|.].\.}.}.|.t
-0000e940: 006a 017c 0264 0088 0064 0164 028d 0493  .j.|.d...d.d....
-0000e950: 0271 0453 0029 0372 3100 0000 da05 696e  .q.S.).r1.....in
-0000e960: 6e65 7229 0372 8e00 0000 7229 0200 0072  ner).r....r)...r
-0000e970: 1f00 0000 2902 72be 0000 0072 d700 0000  ....).r....r....
-0000e980: 2903 724a 0000 0072 e400 0000 72f7 0000  ).rJ...r....r...
-0000e990: 0072 2802 0000 7226 0000 0072 2700 0000  .r(...r&...r'...
-0000e9a0: 7297 0000 0092 0700 0073 0400 0000 0602  r........s......
-0000e9b0: 06ff 7a23 5461 626c 6544 6963 742e 6d65  ..z#TableDict.me
-0000e9c0: 7267 652e 3c6c 6f63 616c 733e 2e3c 6469  rge.<locals>.<di
-0000e9d0: 6374 636f 6d70 3eda 066d 6572 6765 6429  ctcomp>..merged)
-0000e9e0: 0472 af00 0000 7263 0000 0072 4801 0000  .r....rc...rH...
-0000e9f0: 7249 0100 0063 0100 0000 0000 0000 0000  rI...c..........
-0000ea00: 0000 0200 0000 0500 0000 5300 0000 731c  ..........S...s.
-0000ea10: 0000 0067 007c 005d 147d 0164 0074 007c  ...g.|.].}.d.t.|
-0000ea20: 0183 0176 0072 047c 0191 0271 0453 00a9  ...v.r.|...q.S..
-0000ea30: 0172 5001 0000 72a1 0000 00a9 0272 4a00  .rP...r......rJ.
-0000ea40: 0000 da03 636f 6c72 2600 0000 7226 0000  ....colr&...r&..
-0000ea50: 0072 2700 0000 724c 0000 009f 0700 0072  .r'...rL.......r
-0000ea60: 4d00 0000 7201 0000 0072 3100 0000 4e72  M...r....r1...Nr
-0000ea70: ab00 0000 7250 0100 0029 1172 cc00 0000  ....rP...).r....
-0000ea80: 7251 0100 0072 b500 0000 7202 0000 0072  rQ...r....r....r
-0000ea90: cb00 0000 72fc 0000 0072 5901 0000 7200  ....r....rY...r.
-0000eaa0: 0200 0072 da00 0000 7240 0100 0072 0102  ...r....r@...r..
-0000eab0: 0000 72b7 0000 0072 5e00 0000 72c3 0000  ..r....r^...r...
-0000eac0: 0072 9100 0000 7287 0000 0072 3001 0000  .r....r....r0...
-0000ead0: 290d 7256 0000 0072 2902 0000 da04 6172  ).rV...r).....ar
-0000eae0: 6773 da0b 6d65 7267 6564 5f64 6963 7472  gs..merged_dictr
-0000eaf0: 2a02 0000 72e4 0000 0072 f700 0000 7248  *...r....r....rH
-0000eb00: 0100 00da 0d6d 6572 6765 645f 7461 626c  .....merged_tabl
-0000eb10: 6573 7254 0000 00da 0a70 6865 6e6f 5f63  esrT.....pheno_c
-0000eb20: 6f6c 73da 0970 6865 6e6f 5f63 6f6c 7214  ols..pheno_colr.
-0000eb30: 0200 0072 2600 0000 7228 0200 0072 2700  ...r&...r(...r'.
-0000eb40: 0000 7296 0100 007a 0700 0073 3600 0000  ..r....z...s6...
-0000eb50: 000d 1401 0801 0801 1001 1202 0201 14ff  ................
-0000eb60: 0404 0201 0a02 06fe 0404 0201 0401 0201  ................
-0000eb70: 04f8 060c 1002 1001 0c03 20ff 0203 2002  .......... ... .
-0000eb80: 1201 0e03 0802 7a0f 5461 626c 6544 6963  ......z.TableDic
-0000eb90: 742e 6d65 7267 6572 0100 0000 2903 da12  t.merger....)...
-0000eba0: 6375 7272 656e 745f 7461 626c 655f 6469  current_table_di
-0000ebb0: 6374 da0b 7465 7374 5f76 6964 656f 7372  ct..test_videosr
-0000ebc0: 1900 0000 6303 0000 0000 0000 0000 0000  ....c...........
-0000ebd0: 000c 0000 0008 0000 0003 0000 0073 8c03  .............s..
-0000ebe0: 0000 7c01 a000 a100 8901 7401 6a02 6700  ..|.......t.j.g.
-0000ebf0: 7403 6401 8d02 7d03 7401 6a02 6402 6403  t.d...}.t.j.d.d.
-0000ec00: 8400 8801 4400 8301 7404 6401 8d02 8901  ....D...t.d.....
-0000ec10: 7c00 6a05 729a 7401 6a06 8801 6404 6405  |.j.r.t.j...d.d.
-0000ec20: 8d02 7d04 7407 7408 7c04 6406 6406 8502  ..}.t.t.|.d.d...
-0000ec30: 6407 6602 1900 8301 8301 4400 5d3c 8900  d.f.......D.]<..
-0000ec40: 7401 6a09 6a0a 8700 8701 6602 6408 6403  t.j.j.....f.d.d.
-0000ec50: 8408 740b 740c 8801 8301 8301 4400 8301  ..t.t.......D...
-0000ec60: 7c02 6409 640a 8d03 7d05 7401 a006 7c03  |.d.d...}.t...|.
-0000ec70: 7c05 6702 a101 7d03 715a 6e1a 7401 6a09  |.g...}.qZn.t.j.
-0000ec80: 6a0a 740b 740c 8801 8301 8301 7c02 6409  j.t.t.......|.d.
-0000ec90: 640a 8d03 7d03 7401 a002 6700 a101 7401  d...}.t...g...t.
-0000eca0: a002 6700 a101 7401 a002 6700 a101 0300  ..g...t...g.....
-0000ecb0: 0200 7d06 7d07 7d08 7c02 6404 6b04 9001  ..}.}.}.|.d.k...
-0000ecc0: 7246 7a28 7401 a006 8801 7c03 1900 a101  rFz(t.....|.....
-0000ecd0: 7d07 7401 a006 7401 6a0d 8801 7c03 6404  }.t...t.j...|.d.
-0000ece0: 6405 8d03 a101 7d09 5700 6e3a 0400 740e  d.....}.W.n:..t.
-0000ecf0: 9001 7942 0100 0100 0100 7401 6a02 6700  ..yB......t.j.g.
-0000ed00: 7403 6401 8d02 7d03 7401 a006 7408 8801  t.d...}.t...t...
-0000ed10: 8301 a101 7d09 740f a010 640b a101 0100  ....}.t...d.....
-0000ed20: 5900 6e02 3000 6e0e 7401 a006 7408 8801  Y.n.0.n.t...t...
-0000ed30: 8301 a101 7d09 7c00 6a05 9002 7228 7411  ....}.|.j...r(t.
-0000ed40: 8300 7d0a 7c09 6406 6406 8502 6406 6407  ..}.|.d.d...d.d.
-0000ed50: 8502 6602 1900 7c09 6406 6406 8502 6407  ..f...|.d.d...d.
-0000ed60: 6602 1900 6406 6406 8502 7401 6a12 6602  f...d.d...t.j.f.
-0000ed70: 1900 0200 7d09 7d06 7c0a a013 7c06 6406  ....}.}.|...|.d.
-0000ed80: 6406 8502 6404 6602 1900 a101 7c06 6406  d...d.f.....|.d.
-0000ed90: 6406 8502 6404 6602 3c00 7a5a 7c07 6406  d...d.f.<.zZ|.d.
-0000eda0: 6406 8502 6406 6407 8502 6602 1900 7c07  d...d.d...f...|.
-0000edb0: 6406 6406 8502 6407 6602 1900 6406 6406  d.d...d.f...d.d.
-0000edc0: 8502 7401 6a12 6602 1900 0200 7d07 7d08  ..t.j.f.....}.}.
-0000edd0: 7c0a a014 7c08 6406 6406 8502 6404 6602  |...|.d.d...d.f.
-0000ede0: 1900 a101 7c08 6406 6406 8502 6404 6602  ....|.d.d...d.f.
-0000edf0: 3c00 5700 6e14 0400 7415 9002 7926 0100  <.W.n...t...y&..
-0000ee00: 0100 0100 5900 6e02 3000 7c00 6a16 9003  ....Y.n.0.|.j...
-0000ee10: 7266 7408 7c00 6a16 a000 a100 8301 6404  rft.|.j.......d.
-0000ee20: 1900 6a17 640c 1900 7d0b 7a40 7c09 6406  ..j.d...}.z@|.d.
-0000ee30: 6406 8502 6406 7c0b 0b00 8502 6602 1900  d...d.|.....f...
-0000ee40: 7401 6a06 7c06 7c09 6406 6406 8502 7c0b  t.j.|.|.d.d...|.
-0000ee50: 0b00 6406 8502 6602 1900 6702 640c 6405  ..d...f...g.d.d.
-0000ee60: 8d02 0200 7d09 7d06 5700 6e42 0400 740e  ....}.}.W.nB..t.
-0000ee70: 9002 79ca 0100 0100 0100 7c09 6406 6406  ..y.......|.d.d.
-0000ee80: 8502 6406 7c0b 0b00 8502 6602 1900 7c09  ..d.|.....f...|.
-0000ee90: 6406 6406 8502 7c0b 0b00 6406 8502 6602  d.d...|...d...f.
-0000eea0: 1900 0200 7d09 7d06 5900 6e02 3000 7a84  ....}.}.Y.n.0.z.
-0000eeb0: 7a3c 7c07 6406 6406 8502 6406 7c0b 0b00  z<|.d.d...d.|...
-0000eec0: 8502 6602 1900 7401 a006 7c08 7c07 6406  ..f...t...|.|.d.
-0000eed0: 6406 8502 7c0b 0b00 6406 8502 6602 1900  d...|...d...f...
-0000eee0: 6702 a101 0200 7d07 7d08 5700 6e42 0400  g.....}.}.W.nB..
-0000eef0: 740e 9003 794c 0100 0100 0100 7c07 6406  t...yL......|.d.
-0000ef00: 6406 8502 6406 7c0b 0b00 8502 6602 1900  d...d.|.....f...
-0000ef10: 7c07 6406 6406 8502 7c0b 0b00 6406 8502  |.d.d...|...d...
-0000ef20: 6602 1900 0200 7d07 7d08 5900 6e02 3000  f.....}.}.Y.n.0.
-0000ef30: 5700 6e14 0400 7415 9003 7964 0100 0100  W.n...t...yd....
-0000ef40: 0100 5900 6e02 3000 7c09 a018 7419 a101  ..Y.n.0.|...t...
-0000ef50: 7c06 a018 7419 a101 7c07 a018 7419 a101  |...t...|...t...
-0000ef60: 7c08 a018 7419 a101 7c03 6605 5300 290d  |...t...|.f.S.).
-0000ef70: 61d4 0100 0047 656e 6572 6174 6520 7472  a....Generate tr
-0000ef80: 6169 6e69 6e67 2061 6e64 2074 6573 7420  aining and test 
-0000ef90: 7365 7473 2061 7320 6e75 6d70 792e 6172  sets as numpy.ar
-0000efa0: 7261 7920 6f62 6a65 6374 7320 666f 7220  ray objects for 
-0000efb0: 6d6f 6465 6c20 7472 6169 6e69 6e67 2e0a  model training..
-0000efc0: 0a20 2020 2020 2020 2049 6e74 656e 6465  .        Intende
-0000efd0: 6420 666f 7220 696e 7465 726e 616c 2075  d for internal u
-0000efe0: 7361 6765 206f 6e6c 792e 0a0a 2020 2020  sage only...    
-0000eff0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-0000f000: 2020 2020 2020 6375 7272 656e 745f 7461        current_ta
-0000f010: 626c 655f 6469 6374 2028 7461 626c 655f  ble_dict (table_
-0000f020: 6469 6374 293a 2074 6162 6c65 5f64 6963  dict): table_dic
-0000f030: 7420 6f62 6a65 6374 2063 6f6e 7461 696e  t object contain
-0000f040: 696e 6720 7468 6520 6461 7461 2074 6f20  ing the data to 
-0000f050: 6265 2075 7365 6420 666f 7220 7472 6169  be used for trai
-0000f060: 6e69 6e67 2e0a 2020 2020 2020 2020 2020  ning..          
-0000f070: 2020 7465 7374 5f76 6964 656f 7320 2869    test_videos (i
-0000f080: 6e74 293a 204e 756d 6265 7220 6f66 2076  nt): Number of v
-0000f090: 6964 656f 7320 746f 2062 6520 7573 6564  ideos to be used
-0000f0a0: 2066 6f72 2074 6573 7469 6e67 2e20 4465   for testing. De
-0000f0b0: 6661 756c 7473 2074 6f20 302e 0a0a 2020  faults to 0...  
-0000f0c0: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
-0000f0d0: 2020 2020 2020 2020 2020 2074 7570 6c65             tuple
-0000f0e0: 3a20 5475 706c 6520 636f 6e74 6169 6e69  : Tuple containi
-0000f0f0: 6e67 2074 7261 696e 696e 6720 6461 7461  ng training data
-0000f100: 2c20 7472 6169 6e69 6e67 206c 6162 656c  , training label
-0000f110: 7320 2869 6620 616e 7929 2c20 7465 7374  s (if any), test
-0000f120: 2064 6174 612c 2061 6e64 2074 6573 7420   data, and test 
-0000f130: 6c61 6265 6c73 2028 6966 2061 6e79 292e  labels (if any).
-0000f140: 0a20 2020 2020 2020 2072 8500 0000 6301  .        r....c.
-0000f150: 0000 0000 0000 0000 0000 0002 0000 0003  ................
-0000f160: 0000 0053 0000 0073 1200 0000 6700 7c00  ...S...s....g.|.
-0000f170: 5d0a 7d01 7c01 6a00 9102 7104 5300 7226  ].}.|.j...q.S.r&
-0000f180: 0000 0029 0172 c800 0000 2902 724a 0000  ...).r....).rJ..
-0000f190: 0072 1002 0000 7226 0000 0072 2600 0000  .r....r&...r&...
-0000f1a0: 7227 0000 0072 4c00 0000 c307 0000 724d  r'...rL.......rM
-0000f1b0: 0000 007a 2e54 6162 6c65 4469 6374 2e67  ...z.TableDict.g
-0000f1c0: 6574 5f74 7261 696e 696e 675f 7365 742e  et_training_set.
-0000f1d0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-0000f1e0: 6d70 3e72 0100 0000 72ab 0000 004e 7293  mp>r....r....Nr.
-0000f1f0: 0100 0063 0100 0000 0000 0000 0000 0000  ...c............
-0000f200: 0200 0000 0400 0000 1300 0000 7320 0000  ............s ..
-0000f210: 0067 007c 005d 187d 0188 017c 0119 0064  .g.|.].}...|...d
-0000f220: 0019 0088 006b 0272 047c 0191 0271 0453  .....k.r.|...q.S
-0000f230: 0072 0e02 0000 7226 0000 0072 4900 0000  .r....r&...rI...
-0000f240: a902 da05 6c61 6265 6cda 0872 6177 5f64  ....label..raw_d
-0000f250: 6174 6172 2600 0000 7227 0000 0072 4c00  atar&...r'...rL.
-0000f260: 0000 c907 0000 724d 0000 0046 a901 da07  ......rM...F....
-0000f270: 7265 706c 6163 657a 7943 6f75 6c64 206e  replacezyCould n
-0000f280: 6f74 2066 696e 6420 6d6f 7265 2074 6861  ot find more tha
-0000f290: 6e20 6f6e 6520 7361 6d70 6c65 2066 6f72  n one sample for
-0000f2a0: 2061 7420 6c65 6173 7420 6f6e 6520 636f   at least one co
-0000f2b0: 6e64 6974 696f 6e2e 2050 6172 7469 7469  ndition. Partiti
-0000f2c0: 6f6e 2062 6574 7765 656e 2074 7261 696e  on between train
-0000f2d0: 696e 6720 616e 6420 7465 7374 2073 6574  ing and test set
-0000f2e0: 2077 6173 206e 6f74 2070 6f73 7369 626c   was not possibl
-0000f2f0: 652e 7231 0000 0029 1a72 c800 0000 72dd  e.r1...).r....r.
-0000f300: 0000 0072 de00 0000 721f 0100 00da 066f  ...r....r......o
-0000f310: 626a 6563 7472 0002 0000 7299 0100 0072  bjectr....r....r
-0000f320: b600 0000 72b5 0000 0072 1902 0000 da06  ....r....r......
-0000f330: 6368 6f69 6365 72cf 0000 0072 5e00 0000  choicer....r^...
-0000f340: da06 6465 6c65 7465 7273 0100 0072 1101  ..deleters...r..
-0000f350: 0000 7212 0100 0072 0c00 0000 7212 0200  ..r....r....r...
-0000f360: 0072 2002 0000 da09 7472 616e 7366 6f72  .r .....transfor
-0000f370: 6d72 c700 0000 7201 0200 0072 d400 0000  mr....r....r....
-0000f380: 72d0 0000 0072 c000 0000 290c 7256 0000  r....r....).rV..
-0000f390: 0072 3502 0000 7236 0200 00da 0a74 6573  .r5...r6.....tes
-0000f3a0: 745f 696e 6465 78da 0a63 6f6e 6361 745f  t_index..concat_
-0000f3b0: 7261 77da 0b6c 6162 656c 5f69 6e64 6578  raw..label_index
-0000f3c0: da07 795f 7472 6169 6eda 0658 5f74 6573  ..y_train..X_tes
-0000f3d0: 74da 0679 5f74 6573 74da 0758 5f74 7261  t..y_test..X_tra
-0000f3e0: 696e da02 6c65 da07 6e5f 616e 6e6f 7472  in..le..n_annotr
-0000f3f0: 2600 0000 7237 0200 0072 2700 0000 da10  &...r7...r'.....
-0000f400: 6765 745f 7472 6169 6e69 6e67 5f73 6574  get_training_set
-0000f410: af07 0000 7376 0000 0000 0e08 040e 0218  ....sv..........
-0000f420: 0106 010e 021c 0106 011a 0102 0102 fd06  ................
-0000f430: 0512 0206 010e ff06 0422 010a 0102 010e  ........."......
-0000f440: 011a 010e 010e 010e 0104 0102 ff0c 060e  ................
-0000f450: 0208 0106 0134 0122 0102 0134 0126 010e  .....4."...4.&..
-0000f460: 0106 0208 0118 0202 0214 0122 fe0a 040e  ..........."....
-0000f470: 0134 0202 0102 0214 011e fe0a 040e 0138  .4.............8
-0000f480: 020e 0106 0308 0108 0108 0108 0102 fb7a  ...............z
-0000f490: 1a54 6162 6c65 4469 6374 2e67 6574 5f74  .TableDict.get_t
-0000f4a0: 7261 696e 696e 675f 7365 7472 d700 0000  raining_setr....
-0000f4b0: e919 0000 0072 3100 0000 da08 7374 616e  .....r1.....stan
-0000f4c0: 6461 7264 72d1 0100 0029 0cda 0a68 616e  dardr....)...han
-0000f4d0: 646c 655f 6964 73da 0b77 696e 646f 775f  dle_ids..window_
-0000f4e0: 7369 7a65 da0b 7769 6e64 6f77 5f73 7465  size..window_ste
-0000f4f0: 70da 0573 6361 6c65 da11 7072 6574 7261  p..scale..pretra
-0000f500: 696e 6564 5f73 6361 6c65 7272 3602 0000  ined_scalerr6...
-0000f510: 727f 0000 00da 0773 6875 6666 6c65 da13  r......shuffle..
-0000f520: 6669 6c74 6572 5f6c 6f77 5f76 6172 6961  filter_low_varia
-0000f530: 6e63 65da 1669 6e74 6572 706f 6c61 7465  nce..interpolate
-0000f540: 5f6e 6f72 6d61 6c69 7a65 64da 1270 7265  _normalized..pre
-0000f550: 636f 6d70 7574 6564 5f62 7265 616b 7372  computed_breaksr
-0000f560: 1900 0000 630d 0000 0000 0000 0000 0000  ....c...........
-0000f570: 0022 0000 000d 0000 0003 0000 0073 1407  ."...........s..
-0000f580: 0000 7400 a001 7c00 a101 7d0d 7c02 6401  ..t...|...}.|.d.
-0000f590: 7600 731a 4a00 6402 8301 8201 7c0a 727e  v.s.J.d.....|.r~
-0000f5a0: 7c0d a002 a100 4400 5d56 5c02 7d0e 7d0f  |.....D.]V\.}.}.
-0000f5b0: 7c0f 6a03 6403 6403 8502 7404 7405 a006  |.j.d.d...t.t...
-0000f5c0: 7c0f 6a07 6404 6405 8d01 7c0a 6b04 a101  |.j.d.d...|.k...
-0000f5d0: 6404 1900 8301 7404 7405 a006 6406 6407  d.....t.t...d.d.
-0000f5e0: 8400 7c0f 6a08 4400 8301 a101 6404 1900  ..|.j.D.....d...
-0000f5f0: 8301 1700 6602 1900 7c0d 7c0e 3c00 7126  ....f...|.|.<.q&
-0000f600: 7c05 9001 7298 7c08 7290 7409 6408 8301  |...r.|.r.t.d...
-0000f610: 0100 7c05 6409 7601 72a0 740a 640a 8301  ..|.d.v.r.t.d...
-0000f620: 8201 7c0d a002 a100 4400 5d42 5c02 7d0e  ..|.....D.]B\.}.
-0000f630: 7d0f 740b 6a0c 6a0d 7c00 7c0f 7c05 6403  }.t.j.j.|.|.|.d.
-0000f640: 640b 8d04 7d10 740e 6a0f 7c10 7c0f 6a08  d...}.t.j.|.|.j.
-0000f650: 7c0f 6a10 640c 8d03 6a11 640d 640e 8400  |.j.d...j.d.d...
-0000f660: 6404 6405 8d02 7c0d 7c0e 3c00 71a8 7c05  d.d...|.|.<.q.|.
-0000f670: 640f 6b02 72fc 7412 8300 7d11 6e18 7c05  d.k.r.t...}.n.|.
-0000f680: 6410 6b02 9001 720e 7413 8300 7d11 6e06  d.k...r.t...}.n.
-0000f690: 7414 8300 7d11 7c06 6403 7500 9001 7252  t...}.|.d.u...rR
-0000f6a0: 740e a015 7404 7c0d a016 a100 8301 a101  t...t.|.........
-0000f6b0: 7d12 7c11 a017 7c12 6a18 6403 6403 8502  }.|...|.j.d.d...
-0000f6c0: 7c12 6a19 741a 6b02 6602 1900 6a16 a101  |.j.t.k.f...j...
-0000f6d0: 0100 6e04 7c06 7d11 7c0d a002 a100 4400  ..n.|.}.|.....D.
-0000f6e0: 5d36 5c02 7d0e 7d0f 740b 6a0c 6a0d 7c00  ]6\.}.}.t.j.j.|.
-0000f6f0: 7c0f 7c05 7c11 640b 8d04 7d10 740e 6a0f  |.|.|.d...}.t.j.
-0000f700: 7c10 7c0f 6a08 7c0f 6a10 640c 8d03 7c0d  |.|.j.|.j.d...|.
-0000f710: 7c0e 3c00 9001 715e 6e04 6403 7d11 7c05  |.<...q^n.d.}.|.
-0000f720: 640f 6b02 9002 72c8 7c0b 9002 72c8 7400  d.k...r.|...r.t.
-0000f730: a001 7c0d a101 7d13 7c13 a002 a100 4400  ..|...}.|.....D.
-0000f740: 9001 5d02 5c02 7d0e 7d0f 7400 a001 7c0f  ..].\.}.}.t...|.
-0000f750: 6a16 a101 7d14 7a22 7405 6a1b 7c14 7c14  j...}.z"t.j.|.|.
-0000f760: 7c0b 6b04 3c00 7405 6a1b 7c14 7c14 7c0b  |.k.<.t.j.|.|.|.
-0000f770: 0b00 6b00 3c00 5700 6e9e 0400 741c 9002  ..k.<.W.n...t...
-0000f780: 7994 0100 0100 0100 7405 6a1b 7c14 7405  y.......t.j.|.t.
-0000f790: 6a1d 7c14 6403 6403 8502 6403 6411 8502  j.|.d.d...d.d...
-0000f7a0: 6602 1900 a01e 741a a101 7c0b 6b04 7405  f.....t...|.k.t.
-0000f7b0: a01f 6412 6701 7420 7c14 8301 1400 6701  ..d.g.t |.....g.
-0000f7c0: a101 6a21 6413 6405 8d03 3c00 7405 6a1b  ..j!d.d...<.t.j.
-0000f7d0: 7c14 7405 6a1d 7c14 6403 6403 8502 6403  |.t.j.|.d.d...d.
-0000f7e0: 6411 8502 6602 1900 a01e 741a a101 7c0b  d...f.....t...|.
-0000f7f0: 0b00 6b00 7405 a01f 6412 6701 7420 7c14  ..k.t...d.g.t |.
-0000f800: 8301 1400 6701 a101 6a21 6413 6405 8d03  ....g...j!d.d...
-0000f810: 3c00 5900 6e02 3000 740e 6a0f 7c14 7c0f  <.Y.n.0.t.j.|.|.
-0000f820: 6a10 7c0f 6a08 6414 8d03 a011 6415 640e  j.|.j.d.....d.d.
-0000f830: 8400 a101 6a22 6416 6417 8d01 7c13 7c0e  ....j"d.d...|.|.
-0000f840: 3c00 9001 71be 7c13 7d0d 7c00 a023 7c0d  <...q.|.}.|..#|.
-0000f850: 7c07 a102 5c05 7d15 7d16 7d17 7d18 8901  |...\.}.}.}.}...
-0000f860: 7c08 9002 72ec 7409 6418 8301 0100 740b  |...r.t.d.....t.
-0000f870: 6a0c 6a24 7c0d 7c15 8701 6601 6419 6407  j.j$|.|...f.d.d.
-0000f880: 8408 7425 7420 7c0d 8301 8301 4400 8301  ..t%t |.....D...
-0000f890: 7c01 7c03 7c04 7c0c 641a 8d07 5c02 7d15  |.|.|.|.d...\.}.
-0000f8a0: 7d19 7c08 6413 6b04 9003 7286 7c01 9003  }.|.d.k...r.|...
-0000f8b0: 7286 7405 6a26 7c15 6404 6b03 641b 6405  r.t.j&|.d.k.d.d.
-0000f8c0: 8d02 6a27 6413 6405 8d01 7d1a 7409 641c  ..j'd.d...}.t.d.
-0000f8d0: a028 7c1a a029 a100 7c1a a02a a100 a102  .(|..)..|..*....
-0000f8e0: 8301 0100 7409 641d a028 7c1a a02b a100  ....t.d..(|..+..
-0000f8f0: a101 8301 0100 7409 641e a028 7c1a a02c  ......t.d..(|..,
-0000f900: a100 a101 8301 0100 7c00 6a2d 9003 7396  ........|.j-..s.
-0000f910: 7c00 6a2e 9003 72f0 7c19 6403 7500 9003  |.j...r.|.d.u...
-0000f920: 72d6 740b 6a0c 6a24 7c0d 7c16 8701 6601  r.t.j.j$|.|...f.
-0000f930: 641f 6407 8408 7425 7420 7c0d 8301 8301  d.d...t%t |.....
-0000f940: 4400 8301 6412 7c03 7c04 7c0c 641a 8d07  D...d.|.|.|.d...
-0000f950: 5c02 7d16 7d1b 6e0e 740b 6a0c a02f 7c16  \.}.}.n.t.j../|.
-0000f960: 7c19 a102 7d16 7c16 6a29 6413 6405 8d01  |...}.|.j)d.d...
-0000f970: 7d16 7c07 9004 72c8 7420 8801 8301 6404  }.|...r.t ....d.
-0000f980: 6b04 9004 72c8 740b 6a0c 6a24 7c0d 7c17  k...r.t.j.j$|.|.
-0000f990: 8801 7c01 7c03 7c04 7c0c 641a 8d07 5c02  ..|.|.|.|.d...\.
-0000f9a0: 7d17 7d1c 7c00 6a2d 9004 7332 7c00 6a2e  }.}.|.j-..s2|.j.
-0000f9b0: 9004 728c 7c1c 6403 7500 9004 7272 740b  ..r.|.d.u...rrt.
-0000f9c0: 6a0c 6a24 7c0d 7c18 8701 6601 6420 6407  j.j$|.|...f.d d.
-0000f9d0: 8408 7425 7420 7c0d 8301 8301 4400 8301  ..t%t |.....D...
-0000f9e0: 6412 7c03 7c04 7c0c 641a 8d07 5c02 7d18  d.|.|.|.d...\.}.
-0000f9f0: 7d1b 6e1a 740b 6a0c a02f 7c18 7c1c a102  }.n.t.j../|.|...
-0000fa00: 7d18 7c18 6a29 6413 6405 8d01 7d18 7c09  }.|.j)d.d...}.|.
-0000fa10: 9004 72c8 7405 6a30 6a31 7c17 6a32 6404  ..r.t.j0j1|.j2d.
-0000fa20: 1900 7c17 6a32 6404 1900 6412 6421 8d03  ..|.j2d...d.d!..
-0000fa30: 7d1d 7c17 7c1d 1900 7d17 7c00 6a2d 9004  }.|.|...}.|.j-..
-0000fa40: 72c8 7c18 7c1d 1900 7d18 7c09 9005 7204  r.|.|...}.|...r.
-0000fa50: 7405 6a30 6a31 7c15 6a32 6404 1900 7c15  t.j0j1|.j2d...|.
-0000fa60: 6a32 6404 1900 6412 6421 8d03 7d1e 7c15  j2d...d.d!..}.|.
-0000fa70: 7c1e 1900 7d15 7c00 6a2d 9005 7204 7c16  |...}.|.j-..r.|.
-0000fa80: 7c1e 1900 7d16 7405 a01f 7c17 a101 7405  |...}.t...|...t.
-0000fa90: a01f 7c18 a101 0200 7d17 7d18 7c07 9005  ..|.....}.}.|...
-0000faa0: 72be 7c01 9005 72be 7420 7c17 6a32 8301  r.|...r.t |.j2..
-0000fab0: 6404 6b04 9005 72be 7c15 6a32 6413 1900  d.k...r.|.j2d...
-0000fac0: 7c17 6a32 6413 1900 6b03 9005 72be 7405  |.j2d...k...r.t.
-0000fad0: a033 7c15 6a32 6413 1900 7c17 6a32 6413  .3|.j2d...|.j2d.
-0000fae0: 1900 a102 7d1f 7c15 6a32 6413 1900 7c1f  ....}.|.j2d...|.
-0000faf0: 6b00 9005 729a 7405 6a34 7c15 6422 6404  k...r.t.j4|.d"d.
-0000fb00: 7c1f 7c15 6a32 6413 1900 1800 6602 6422  |.|.j2d.....f.d"
-0000fb10: 6603 6423 6424 8d03 7d15 6e24 7405 6a34  f.d#d$..}.n$t.j4
-0000fb20: 7c17 6422 6404 7c1f 7c17 6a32 6413 1900  |.d"d.|.|.j2d...
-0000fb30: 1800 6602 6422 6603 6423 6424 8d03 7d17  ..f.d"f.d#d$..}.
-0000fb40: 7c08 9005 72cc 7409 6425 8301 0100 7c16  |...r.t.d%....|.
-0000fb50: 6a32 6426 6b03 9006 720a 7c15 6a32 6404  j2d&k...r.|.j2d.
-0000fb60: 1900 7c16 6a32 6404 1900 6b02 9006 730a  ..|.j2d...k...s.
-0000fb70: 4a00 6427 a028 7c15 6a32 6404 1900 7c16  J.d'.(|.j2d...|.
-0000fb80: 6a32 6404 1900 a102 8301 8201 7c18 6a32  j2d.........|.j2
-0000fb90: 6426 6b03 9006 7234 7c17 6a32 6404 1900  d&k...r4|.j2d...
-0000fba0: 7c18 6a32 6404 1900 6b02 9006 7334 4a00  |.j2d...k...s4J.
-0000fbb0: 6428 8301 8201 7420 7c00 6a35 8301 6413  d(....t |.j5..d.
-0000fbc0: 6b04 9007 7204 7c02 6429 6b02 9007 7204  k...r.|.d)k...r.
-0000fbd0: 6700 6700 0200 7d20 7d21 7c00 6a35 4400  g.g...} }!|.j5D.
-0000fbe0: 5d82 8900 7c20 a01d 7c15 6403 6403 8502  ]...| ..|.d.d...
-0000fbf0: 6403 6403 8502 7405 a006 8700 6601 642a  d.d...t.....f.d*
-0000fc00: 6407 8408 7404 7c0d a016 a100 8301 6404  d...t.|.......d.
-0000fc10: 1900 6a08 4400 8301 a101 6603 1900 a101  ..j.D.....f.....
-0000fc20: 0100 7c21 a01d 7c17 6403 6403 8502 6403  ..|!..|.d.d...d.
-0000fc30: 6403 8502 7405 a006 8700 6601 642b 6407  d...t.....f.d+d.
-0000fc40: 8408 7404 7c0d a016 a100 8301 6404 1900  ..t.|.......d...
-0000fc50: 6a08 4400 8301 a101 6603 1900 a101 0100  j.D.....f.......
-0000fc60: 9006 715e 7405 a036 7405 a037 7c20 a101  ..q^t..6t..7| ..
-0000fc70: a101 7405 a036 7405 a037 7c21 a101 a101  ..t..6t..7|!....
-0000fc80: 0200 7d15 7d17 7c15 7c16 7c17 7c18 6604  ..}.}.|.|.|.|.f.
-0000fc90: 7c11 6602 5300 292c 6117 0c00 0050 7265  |.f.S.),a....Pre
-0000fca0: 7072 6f63 6573 7320 7468 6520 6c6f 6164  process the load
-0000fcb0: 6564 2064 6174 6173 6574 2062 6566 6f72  ed dataset befor
-0000fcc0: 6520 6665 6564 696e 6720 746f 2075 6e73  e feeding to uns
-0000fcd0: 7570 6572 7669 7365 6420 656d 6265 6464  upervised embedd
-0000fce0: 696e 6720 6d6f 6465 6c73 2e0a 0a20 2020  ing models...   
-0000fcf0: 2020 2020 2043 6170 6162 6c65 206f 6620       Capable of 
-0000fd00: 7265 7475 726e 696e 6720 7472 6169 6e69  returning traini
-0000fd10: 6e67 2061 6e64 2074 6573 7420 7365 7473  ng and test sets
-0000fd20: 2072 6561 6479 2066 6f72 206d 6f64 656c   ready for model
-0000fd30: 2074 7261 696e 696e 672e 0a0a 2020 2020   training...    
-0000fd40: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-0000fd50: 2020 2020 2020 6175 746f 6d61 7469 635f        automatic_
-0000fd60: 6368 616e 6765 706f 696e 7473 2028 7374  changepoints (st
-0000fd70: 7229 3a20 7370 6563 6966 6965 7320 7468  r): specifies th
-0000fd80: 6520 6368 616e 6765 706f 696e 7420 6465  e changepoint de
-0000fd90: 7465 6374 696f 6e20 6b65 726e 656c 2074  tection kernel t
-0000fda0: 6f20 7573 6520 746f 2072 7570 7475 7265  o use to rupture
-0000fdb0: 2074 6865 2064 6174 6120 6163 726f 7373   the data across
-0000fdc0: 2074 696d 6520 7573 696e 6720 5065 6c74   time using Pelt
-0000fdd0: 2e20 4361 6e20 6265 2073 6574 2074 6f20  . Can be set to 
-0000fde0: 2272 6266 2220 2864 6566 6175 6c74 292c  "rbf" (default),
-0000fdf0: 206f 7220 226c 696e 6561 7222 2e20 4966   or "linear". If
-0000fe00: 2046 616c 7365 2c20 6669 7865 642d 6c65   False, fixed-le
-0000fe10: 6e67 7468 2072 7570 7475 7265 7320 6172  ngth ruptures ar
-0000fe20: 6520 6170 7069 6c65 642e 0a20 2020 2020  e appiled..     
-0000fe30: 2020 2020 2020 2068 616e 646c 655f 6964         handle_id
-0000fe40: 7320 2873 7472 293a 2069 6e64 6963 6174  s (str): indicat
-0000fe50: 6573 2074 6865 2064 6566 6175 6c74 2061  es the default a
-0000fe60: 6374 696f 6e20 746f 2068 616e 646c 6520  ction to handle 
-0000fe70: 6d75 6c74 6970 6c65 2061 6e69 6d61 6c73  multiple animals
-0000fe80: 2069 6e20 7468 6520 5461 626c 6544 6963   in the TableDic
-0000fe90: 7420 6f62 6a65 6374 2e20 4d75 7374 2062  t object. Must b
-0000fea0: 6520 6f6e 6520 6f66 2022 636f 6e63 6174  e one of "concat
-0000feb0: 2220 2862 6f64 7920 7061 7274 7320 6672  " (body parts fr
-0000fec0: 6f6d 2064 6966 6665 7265 6e74 2061 6e69  om different ani
-0000fed0: 6d61 6c73 2061 7265 2074 7265 6174 6564  mals are treated
-0000fee0: 2061 7320 6665 6174 7572 6573 2920 616e   as features) an
-0000fef0: 6420 2273 706c 6974 2220 2864 6966 6665  d "split" (diffe
-0000ff00: 7265 6e74 2073 6c69 6469 6e67 2077 696e  rent sliding win
-0000ff10: 646f 7773 2061 7265 2063 7265 6174 6564  dows are created
-0000ff20: 2066 6f72 2065 6163 6820 616e 696d 616c   for each animal
-0000ff30: 292e 0a20 2020 2020 2020 2020 2020 2077  )..            w
-0000ff40: 696e 646f 775f 7369 7a65 2028 696e 7429  indow_size (int)
-0000ff50: 3a20 4d69 6e69 6d75 6d20 7369 7a65 206f  : Minimum size o
-0000ff60: 6620 7468 6520 6170 706c 6965 6420 7275  f the applied ru
-0000ff70: 7074 7572 6573 2e20 4966 2061 7574 6f6d  ptures. If autom
-0000ff80: 6174 6963 5f63 6861 6e67 6570 6f69 6e74  atic_changepoint
-0000ff90: 7320 6973 2046 616c 7365 2c20 7370 6563  s is False, spec
-0000ffa0: 6966 6965 7320 7468 6520 7369 7a65 206f  ifies the size o
-0000ffb0: 6620 7468 6520 736c 6964 696e 6720 7769  f the sliding wi
-0000ffc0: 6e64 6f77 2074 6f20 7061 7373 2074 6872  ndow to pass thr
-0000ffd0: 6f75 6768 2074 6865 2064 6174 6120 746f  ough the data to
-0000ffe0: 2067 656e 6572 6174 6520 7472 6169 6e69   generate traini
-0000fff0: 6e67 2069 6e73 7461 6e63 6573 2e0a 2020  ng instances..  
-00010000: 2020 2020 2020 2020 2020 7769 6e64 6f77            window
-00010010: 5f73 7465 7020 2869 6e74 293a 2053 7065  _step (int): Spe
-00010020: 6369 6669 6573 2074 6865 206d 696e 696d  cifies the minim
-00010030: 756d 206a 756d 7020 666f 7220 7468 6520  um jump for the 
-00010040: 7275 7074 7572 6520 616c 676f 7269 7468  rupture algorith
-00010050: 6d73 2e20 4966 2061 7574 6f6d 6174 6963  ms. If automatic
-00010060: 5f63 6861 6e67 6570 6f69 6e74 7320 6973  _changepoints is
-00010070: 2046 616c 7365 2c20 7370 6563 6966 6965   False, specifie
-00010080: 7320 7468 6520 7374 6570 2074 6f20 7461  s the step to ta
-00010090: 6b65 2077 6865 6e20 736c 6964 696e 6720  ke when sliding 
-000100a0: 7468 6520 6166 6f72 656d 656e 7469 6f6e  the aforemention
-000100b0: 6564 2077 696e 646f 772e 2049 6e20 7468  ed window. In th
-000100c0: 6973 2063 6173 652c 2061 2076 616c 7565  is case, a value
-000100d0: 206f 6620 3120 696e 6469 6361 7465 7320   of 1 indicates 
-000100e0: 6120 7472 7565 2073 6c69 6469 6e67 2077  a true sliding w
-000100f0: 696e 646f 772c 2061 6e64 2061 2076 616c  indow, and a val
-00010100: 7565 2065 7175 616c 2074 6f20 7769 6e64  ue equal to wind
-00010110: 6f77 5f73 697a 6520 7370 6c69 7473 2074  ow_size splits t
-00010120: 6865 2064 6174 6120 696e 746f 206e 6f6e  he data into non
-00010130: 2d6f 7665 726c 6170 7069 6e67 2063 6875  -overlapping chu
-00010140: 6e6b 732e 0a20 2020 2020 2020 2020 2020  nks..           
-00010150: 2073 6361 6c65 2028 7374 7229 3a20 4461   scale (str): Da
-00010160: 7461 2073 6361 6c69 6e67 206d 6574 686f  ta scaling metho
-00010170: 642e 204d 7573 7420 6265 206f 6e65 206f  d. Must be one o
-00010180: 6620 2773 7461 6e64 6172 6427 2c20 2772  f 'standard', 'r
-00010190: 6f62 7573 7427 2028 6465 6661 756c 743b  obust' (default;
-000101a0: 2072 6563 6f6d 6d65 6e64 6564 2920 616e   recommended) an
-000101b0: 6420 276d 696e 6d61 7827 2e0a 2020 2020  d 'minmax'..    
-000101c0: 2020 2020 2020 2020 7072 6574 7261 696e          pretrain
-000101d0: 6564 5f73 6361 6c65 7220 2841 6e79 293a  ed_scaler (Any):
-000101e0: 2050 7265 2d66 6974 2067 6c6f 6261 6c20   Pre-fit global 
-000101f0: 7363 616c 6572 2c20 7472 6169 6e65 6420  scaler, trained 
-00010200: 6f6e 2074 6865 2077 686f 6c65 2064 6174  on the whole dat
-00010210: 6173 6574 2e20 5573 6566 756c 2074 6f20  aset. Useful to 
-00010220: 7072 6f63 6573 7320 7369 6e67 6c65 2076  process single v
-00010230: 6964 656f 732e 0a20 2020 2020 2020 2020  ideos..         
-00010240: 2020 2074 6573 745f 7669 6465 6f73 2028     test_videos (
-00010250: 696e 7429 3a20 4e75 6d62 6572 206f 6620  int): Number of 
-00010260: 7669 6465 6f73 2074 6f20 7573 6520 666f  videos to use fo
-00010270: 7220 7465 7374 696e 672e 2049 6620 302c  r testing. If 0,
-00010280: 206e 6f20 7465 7374 2073 6574 2069 7320   no test set is 
-00010290: 6765 6e65 7261 7465 642e 0a20 2020 2020  generated..     
-000102a0: 2020 2020 2020 2076 6572 626f 7365 2028         verbose (
-000102b0: 696e 7429 3a20 5665 7262 6f73 6974 7920  int): Verbosity 
-000102c0: 6c65 7665 6c2e 2030 2028 6465 6661 756c  level. 0 (defaul
-000102d0: 7429 2069 7320 7369 6c65 6e74 2c20 3120  t) is silent, 1 
-000102e0: 7072 696e 7473 2070 726f 6772 6573 732c  prints progress,
-000102f0: 2032 2070 7269 6e74 7320 6465 6275 6720   2 prints debug 
-00010300: 696e 666f 726d 6174 696f 6e2e 0a20 2020  information..   
-00010310: 2020 2020 2020 2020 2073 6875 6666 6c65           shuffle
-00010320: 2028 626f 6f6c 293a 2057 6865 7468 6572   (bool): Whether
-00010330: 2074 6f20 7368 7566 666c 6520 7468 6520   to shuffle the 
-00010340: 6461 7461 2062 6566 6f72 6520 7072 6570  data before prep
-00010350: 726f 6365 7373 696e 672e 2044 6566 6175  rocessing. Defau
-00010360: 6c74 7320 746f 2046 616c 7365 2e0a 2020  lts to False..  
-00010370: 2020 2020 2020 2020 2020 6669 6c74 6572            filter
-00010380: 5f6c 6f77 5f76 6172 6961 6e63 6520 2866  _low_variance (f
-00010390: 6c6f 6174 293a 2072 656d 6f76 6520 6665  loat): remove fe
-000103a0: 6174 7572 6573 2077 6974 6820 7661 7269  atures with vari
-000103b0: 616e 6365 206c 6f77 6572 2074 6861 6e20  ance lower than 
-000103c0: 7468 6520 7370 6563 6966 6965 6420 7468  the specified th
-000103d0: 7265 7368 6f6c 642e 2055 7365 6675 6c20  reshold. Useful 
-000103e0: 746f 2067 6574 2072 6964 206f 6620 7468  to get rid of th
-000103f0: 6520 7820 6178 6973 206f 6620 7468 6520  e x axis of the 
-00010400: 626f 6479 2070 6172 7420 7573 6564 2066  body part used f
-00010410: 6f72 2061 6c69 676e 6d65 6e74 2028 7768  or alignment (wh
-00010420: 6963 6820 776f 756c 6420 696e 7472 6f64  ich would introd
-00010430: 7563 6520 6e6f 6973 6520 6166 7465 7220  uce noise after 
-00010440: 7374 616e 6461 7264 697a 6174 696f 6e29  standardization)
-00010450: 2e0a 2020 2020 2020 2020 2020 2020 696e  ..            in
-00010460: 7465 7270 6f6c 6174 655f 6e6f 726d 616c  terpolate_normal
-00010470: 697a 6564 2869 6e74 293a 2069 6620 6e6f  ized(int): if no
-00010480: 7420 302c 2069 7420 7370 6563 6966 6965  t 0, it specifie
-00010490: 7320 7468 6520 6e75 6d62 6572 206f 6620  s the number of 
-000104a0: 7374 616e 6461 7264 2064 6576 6961 7469  standard deviati
-000104b0: 6f6e 7320 6265 796f 6e64 2077 6869 6368  ons beyond which
-000104c0: 2076 616c 7565 7320 7769 6c6c 2062 6520   values will be 
-000104d0: 696e 7465 7270 6f6c 6174 6564 2061 6674  interpolated aft
-000104e0: 6572 206e 6f72 6d61 6c69 7a61 7469 6f6e  er normalization
-000104f0: 2e20 4f6e 6c79 2075 7365 6420 6966 2073  . Only used if s
-00010500: 6361 6c65 2069 7320 7365 7420 746f 2022  cale is set to "
-00010510: 7374 616e 6461 7264 222e 0a20 2020 2020  standard"..     
-00010520: 2020 2020 2020 2070 7265 636f 6d70 7574         precomput
-00010530: 6564 5f62 7265 616b 7320 2864 6963 7429  ed_breaks (dict)
-00010540: 3a20 4966 2070 726f 7669 6465 642c 2063  : If provided, c
-00010550: 6861 6e67 6570 6f69 6e74 2064 6574 6563  hangepoint detec
-00010560: 7469 6f6e 2069 7320 7072 6576 656e 7465  tion is prevente
-00010570: 642c 2061 6e64 2070 726f 7669 6465 6420  d, and provided 
-00010580: 6272 6561 6b73 2061 7265 2075 7365 6420  breaks are used 
-00010590: 696e 7374 6561 642e 0a0a 2020 2020 2020  instead...      
-000105a0: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-000105b0: 2020 2020 2020 2058 5f74 7261 696e 2028         X_train (
-000105c0: 6e70 2e6e 6461 7272 6179 293a 2033 4420  np.ndarray): 3D 
-000105d0: 6461 7461 7365 7420 7769 7468 2073 6861  dataset with sha
-000105e0: 7065 2028 696e 7374 616e 6365 732c 2073  pe (instances, s
-000105f0: 6c69 6469 6e67 5f77 696e 646f 775f 7369  liding_window_si
-00010600: 7a65 2c20 6665 6174 7572 6573 2920 6765  ze, features) ge
-00010610: 6e65 7261 7465 6420 6672 6f6d 2061 6c6c  nerated from all
-00010620: 2074 7261 696e 696e 6720 7669 6465 6f73   training videos
-00010630: 2e0a 2020 2020 2020 2020 2020 2020 795f  ..            y_
-00010640: 7472 6169 6e20 286e 702e 6e64 6172 7261  train (np.ndarra
-00010650: 7929 3a20 3344 2064 6174 6173 6574 2077  y): 3D dataset w
-00010660: 6974 6820 7368 6170 6520 2869 6e73 7461  ith shape (insta
-00010670: 6e63 6573 2c20 736c 6964 696e 675f 7769  nces, sliding_wi
-00010680: 6e64 6f77 5f73 697a 652c 206c 6162 656c  ndow_size, label
-00010690: 7329 2067 656e 6572 6174 6564 2066 726f  s) generated fro
-000106a0: 6d20 616c 6c20 7472 6169 6e69 6e67 2076  m all training v
-000106b0: 6964 656f 732e 204e 6f74 6520 7468 6174  ideos. Note that
-000106c0: 206e 6f20 6c61 6265 6c73 2061 7265 2075   no labels are u
-000106d0: 7365 2062 7920 6465 6661 756c 7420 696e  se by default in
-000106e0: 2074 6865 2066 756c 6c79 2075 6e73 7570   the fully unsup
-000106f0: 6572 7669 7365 6420 7069 7065 6c69 6e65  ervised pipeline
-00010700: 2028 696e 2077 6869 6368 2063 6173 6520   (in which case 
-00010710: 7468 6973 2069 7320 616e 2065 6d70 7479  this is an empty
-00010720: 2061 7272 6179 292e 0a20 2020 2020 2020   array)..       
-00010730: 2020 2020 2058 5f74 6573 7420 286e 702e       X_test (np.
-00010740: 6e64 6172 7261 7929 3a20 3344 2064 6174  ndarray): 3D dat
-00010750: 6173 6574 2077 6974 6820 7368 6170 6520  aset with shape 
-00010760: 2869 6e73 7461 6e63 6573 2c20 736c 6964  (instances, slid
-00010770: 696e 675f 7769 6e64 6f77 5f73 697a 652c  ing_window_size,
-00010780: 2066 6561 7475 7265 7329 2067 656e 6572   features) gener
-00010790: 6174 6564 2066 726f 6d20 616c 6c20 7465  ated from all te
-000107a0: 7374 2076 6964 656f 7320 2830 2062 7920  st videos (0 by 
-000107b0: 6465 6661 756c 7429 2e0a 2020 2020 2020  default)..      
-000107c0: 2020 2020 2020 795f 7465 7374 2028 6e70        y_test (np
-000107d0: 2e6e 6461 7272 6179 293a 2033 4420 6461  .ndarray): 3D da
-000107e0: 7461 7365 7420 7769 7468 2073 6861 7065  taset with shape
-000107f0: 2028 696e 7374 616e 6365 732c 2073 6c69   (instances, sli
-00010800: 6469 6e67 5f77 696e 646f 775f 7369 7a65  ding_window_size
-00010810: 2c20 6c61 6265 6c73 2920 6765 6e65 7261  , labels) genera
-00010820: 7465 6420 6672 6f6d 2061 6c6c 2074 6573  ted from all tes
-00010830: 7420 7669 6465 6f73 2e20 4e6f 7465 2074  t videos. Note t
-00010840: 6861 7420 6e6f 206c 6162 656c 7320 6172  hat no labels ar
-00010850: 6520 7573 6520 6279 2064 6566 6175 6c74  e use by default
-00010860: 2069 6e20 7468 6520 6675 6c6c 7920 756e   in the fully un
-00010870: 7375 7065 7276 6973 6564 2070 6970 656c  supervised pipel
-00010880: 696e 6520 2869 6e20 7768 6963 6820 6361  ine (in which ca
-00010890: 7365 2074 6869 7320 6973 2061 6e20 656d  se this is an em
-000108a0: 7074 7920 6172 7261 7929 2e0a 2020 2020  pty array)..    
-000108b0: 2020 2020 2902 72d7 0000 0072 2200 0000      ).r....r"...
-000108c0: 7a56 6861 6e64 6c65 2049 4473 2073 686f  zVhandle IDs sho
-000108d0: 756c 6420 6265 206f 6e65 206f 6620 2763  uld be one of 'c
-000108e0: 6f6e 6361 7427 2c20 616e 6420 2773 706c  oncat', and 'spl
-000108f0: 6974 272e 2053 6565 2064 6f63 756d 656e  it'. See documen
-00010900: 7461 7469 6f6e 2066 6f72 206d 6f72 6520  tation for more 
-00010910: 6465 7461 696c 732e 4e72 0100 0000 72ab  details.Nr....r.
-00010920: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00010930: 0200 0000 0500 0000 5300 0000 7318 0000  ........S...s...
-00010940: 0067 007c 005d 107d 0164 0074 007c 0183  .g.|.].}.d.t.|..
-00010950: 0176 0091 0271 0453 0072 2d02 0000 72a1  .v...q.S.r-...r.
-00010960: 0000 0072 2e02 0000 7226 0000 0072 2600  ...r....r&...r&.
-00010970: 0000 7227 0000 0072 4c00 0000 4408 0000  ..r'...rL...D...
-00010980: 724d 0000 007a 2854 6162 6c65 4469 6374  rM...z(TableDict
-00010990: 2e70 7265 7072 6f63 6573 732e 3c6c 6f63  .preprocess.<loc
-000109a0: 616c 733e 2e3c 6c69 7374 636f 6d70 3e7a  als>.<listcomp>z
-000109b0: 0f53 6361 6c69 6e67 2064 6174 612e 2e2e  .Scaling data...
-000109c0: 2903 da06 726f 6275 7374 724b 0200 00da  )...robustrK....
-000109d0: 066d 696e 6d61 787a 3849 6e76 616c 6964  .minmaxz8Invalid
-000109e0: 2073 6361 6c65 722e 2053 656c 6563 7420   scaler. Select 
-000109f0: 6f6e 6520 6f66 2073 7461 6e64 6172 642c  one of standard,
-00010a00: 206d 696e 6d61 7820 6f72 2072 6f62 7573   minmax or robus
-00010a10: 7429 0472 2500 0000 da0d 6665 6174 7572  t).r%.....featur
-00010a20: 655f 6172 7261 7972 4f02 0000 72ab 0100  e_arrayrO...r...
-00010a30: 0029 0272 b700 0000 72c9 0000 0063 0100  .).r....r....c..
-00010a40: 0000 0000 0000 0000 0000 0100 0000 0400  ................
-00010a50: 0000 5300 0000 730e 0000 0074 006a 017c  ..S...s....t.j.|
-00010a60: 0064 0164 028d 0253 00a9 034e da06 6967  .d.d...S...N..ig
-00010a70: 6e6f 7265 2901 da06 6572 726f 7273 a902  nore)...errors..
-00010a80: 72be 0000 00da 0a74 6f5f 6e75 6d65 7269  r......to_numeri
-00010a90: 6372 0601 0000 7226 0000 0072 2600 0000  cr....r&...r&...
-00010aa0: 7227 0000 0072 a400 0000 5e08 0000 724d  r'...r....^...rM
-00010ab0: 0000 007a 2654 6162 6c65 4469 6374 2e70  ...z&TableDict.p
-00010ac0: 7265 7072 6f63 6573 732e 3c6c 6f63 616c  reprocess.<local
-00010ad0: 733e 2e3c 6c61 6d62 6461 3e72 4b02 0000  s>.<lambda>rK...
-00010ae0: 7256 0200 0072 9301 0000 4672 3100 0000  rV...r....Fr1...
-00010af0: 720c 0100 0063 0100 0000 0000 0000 0000  r....c..........
-00010b00: 0000 0100 0000 0400 0000 5300 0000 730e  ..........S...s.
-00010b10: 0000 0074 006a 017c 0064 0164 028d 0253  ...t.j.|.d.d...S
-00010b20: 0072 5802 0000 725b 0200 0072 0601 0000  .rX...r[...r....
-00010b30: 7226 0000 0072 2600 0000 7227 0000 0072  r&...r&...r'...r
-00010b40: a400 0000 9f08 0000 724d 0000 00da 0462  ........rM.....b
-00010b50: 6f74 6829 01da 0f6c 696d 6974 5f64 6972  oth)...limit_dir
-00010b60: 6563 7469 6f6e 7a17 4272 6561 6b69 6e67  ectionz.Breaking
-00010b70: 2074 696d 6520 7365 7269 6573 2e2e 2e63   time series...c
-00010b80: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00010b90: 0400 0000 1300 0000 7318 0000 0067 007c  ........s....g.|
-00010ba0: 005d 107d 017c 0188 0076 0172 047c 0191  .].}.|...v.r.|..
-00010bb0: 0271 0453 0072 2600 0000 7226 0000 0072  .q.S.r&...r&...r
-00010bc0: 4900 0000 a901 7240 0200 0072 2600 0000  I.....r@...r&...
-00010bd0: 7227 0000 0072 4c00 0000 b108 0000 724d  r'...rL.......rM
-00010be0: 0000 0029 0772 fa01 0000 da0a 746f 5f72  ...).r......to_r
-00010bf0: 7570 7475 7265 da0f 7275 7074 7572 655f  upture..rupture_
-00010c00: 696e 6469 6365 73da 1661 7574 6f6d 6174  indices..automat
-00010c10: 6963 5f63 6861 6e67 6570 6f69 6e74 7372  ic_changepointsr
-00010c20: 4d02 0000 724e 0200 0072 5402 0000 7292  M...rN...rT...r.
-00010c30: 0000 007a 3261 7665 7261 6765 2072 7570  ...z2average rup
-00010c40: 7475 7265 206c 656e 6774 683a 207b 7d2c  ture length: {},
-00010c50: 2073 7461 6e64 6172 6420 6465 7669 6174   standard deviat
-00010c60: 696f 6e3a 207b 7d7a 1a6d 696e 696d 756d  ion: {}z.minimum
-00010c70: 2072 7570 7475 7265 206c 656e 6774 683a   rupture length:
-00010c80: 207b 7d7a 1a6d 6178 696d 756d 2072 7570   {}z.maximum rup
-00010c90: 7475 7265 206c 656e 6774 683a 207b 7d63  ture length: {}c
-00010ca0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00010cb0: 0400 0000 1300 0000 7318 0000 0067 007c  ........s....g.|
-00010cc0: 005d 107d 017c 0188 0076 0172 047c 0191  .].}.|...v.r.|..
-00010cd0: 0271 0453 0072 2600 0000 7226 0000 0072  .q.S.r&...r&...r
-00010ce0: 4900 0000 725f 0200 0072 2600 0000 7227  I...r_...r&...r'
-00010cf0: 0000 0072 4c00 0000 c908 0000 7302 0000  ...rL.......s...
-00010d00: 0006 0163 0100 0000 0000 0000 0000 0000  ...c............
-00010d10: 0200 0000 0400 0000 1300 0000 7318 0000  ............s...
-00010d20: 0067 007c 005d 107d 017c 0188 0076 0072  .g.|.].}.|...v.r
-00010d30: 047c 0191 0271 0453 0072 2600 0000 7226  .|...q.S.r&...r&
-00010d40: 0000 0072 4900 0000 725f 0200 0072 2600  ...rI...r_...r&.
-00010d50: 0000 7227 0000 0072 4c00 0000 e908 0000  ..r'...rL.......
-00010d60: 7302 0000 0006 0172 3a02 0000 2902 7201  s......r:...).r.
-00010d70: 0000 0072 0100 0000 72ac 0000 0029 01da  ...r....r....)..
-00010d80: 0f63 6f6e 7374 616e 745f 7661 6c75 6573  .constant_values
-00010d90: 721e 0100 0072 ed00 0000 7a3c 7472 6169  r....r....z<trai
-00010da0: 6e69 6e67 2073 6574 2028 7b7d 2920 616e  ning set ({}) an
-00010db0: 6420 6c61 6265 6c73 2028 7b7d 2920 646f  d labels ({}) do
-00010dc0: 206e 6f74 2068 6176 6520 7468 6520 7361   not have the sa
-00010dd0: 6d65 2073 6861 7065 7a32 7472 6169 6e69  me shapez2traini
-00010de0: 6e67 2073 6574 2061 6e64 206c 6162 656c  ng set and label
-00010df0: 7320 646f 206e 6f74 2068 6176 6520 7468  s do not have th
-00010e00: 6520 7361 6d65 2073 6861 7065 7222 0000  e same shaper"..
-00010e10: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
-00010e20: 0000 0500 0000 1300 0000 7326 0000 0067  ..........s&...g
-00010e30: 007c 005d 1e7d 0174 00a0 017c 0167 01a1  .|.].}.t...|.g..
-00010e40: 01a0 02a1 0064 0019 00a0 0388 00a1 0191  .....d..........
-00010e50: 0271 0453 0072 ed00 0000 a904 72dd 0000  .q.S.r......r...
-00010e60: 0072 de00 0000 da07 666c 6174 7465 6e72  .r......flattenr
-00010e70: 4800 0000 7249 0000 0072 0701 0000 7226  H...rI...r....r&
-00010e80: 0000 0072 2700 0000 724c 0000 0036 0900  ...r'...rL...6..
-00010e90: 0073 0400 0000 0602 02ff 6301 0000 0000  .s........c.....
-00010ea0: 0000 0000 0000 0002 0000 0005 0000 0013  ................
-00010eb0: 0000 0073 2600 0000 6700 7c00 5d1e 7d01  ...s&...g.|.].}.
-00010ec0: 7400 a001 7c01 6701 a101 a002 a100 6400  t...|.g.......d.
-00010ed0: 1900 a003 8800 a101 9102 7104 5300 72ed  ..........q.S.r.
-00010ee0: 0000 0072 6402 0000 7249 0000 0072 0701  ...rd...rI...r..
-00010ef0: 0000 7226 0000 0072 2700 0000 724c 0000  ..r&...r'...rL..
-00010f00: 0042 0900 0073 0400 0000 0602 02ff 2938  .B...s........)8
-00010f10: 72cc 0000 0072 5101 0000 72cb 0000 0072  r....rQ...r....r
-00010f20: 9100 0000 72b5 0000 0072 dd00 0000 da05  ....r....r......
-00010f30: 7768 6572 65da 0376 6172 72b7 0000 0072  where..varr....r
-00010f40: 8000 0000 7273 0100 0072 8100 0000 7282  ....rs...r....r.
-00010f50: 0000 00da 0b73 6361 6c65 5f74 6162 6c65  .....scale_table
-00010f60: 72be 0000 0072 db00 0000 72c9 0000 0072  r....r....r....r
-00010f70: 0e01 0000 720a 0000 0072 0900 0000 720b  ....r....r....r.
-00010f80: 0000 0072 d700 0000 72c8 0000 00da 0366  ...r....r......f
-00010f90: 6974 72c3 0000 00da 0664 7479 7065 7372  itr......dtypesr
-00010fa0: c000 0000 da03 6e61 6eda 0954 7970 6545  ......nan..TypeE
-00010fb0: 7272 6f72 72fc 0000 0072 d000 0000 72de  rrorr....r....r.
-00010fc0: 0000 0072 5e00 0000 72c1 0000 00da 0b69  ...r^...r......i
-00010fd0: 6e74 6572 706f 6c61 7465 7249 0200 00da  nterpolaterI....
-00010fe0: 1672 7570 7475 7265 5f70 6572 5f65 7870  .rupture_per_exp
-00010ff0: 6572 696d 656e 7472 cf00 0000 7257 0000  erimentr....rW..
-00011000: 00da 0373 756d 726c 0000 0072 1102 0000  ...sumrl...r....
-00011010: da03 7374 64da 036d 696e da03 6d61 7872  ..std..min..maxr
-00011020: 0002 0000 7201 0200 00da 1673 706c 6974  ....r......split
-00011030: 5f77 6974 685f 6272 6561 6b70 6f69 6e74  _with_breakpoint
-00011040: 7372 1902 0000 723d 0200 0072 d400 0000  sr....r=...r....
-00011050: da07 6d61 7869 6d75 6dda 0370 6164 7230  ..maximum..padr0
-00011060: 0100 00da 0773 7175 6565 7a65 7299 0100  .....squeezer...
-00011070: 0029 2272 5600 0000 7262 0200 0072 4c02  .)"rV...rb...rL.
-00011080: 0000 724d 0200 0072 4e02 0000 724f 0200  ..rM...rN...rO..
-00011090: 0072 5002 0000 7236 0200 0072 7f00 0000  .rP...r6...r....
-000110a0: 7251 0200 0072 5202 0000 7253 0200 0072  rQ...rR...rS...r
-000110b0: 5402 0000 da0a 7461 626c 655f 7465 6d70  T.....table_temp
-000110c0: 72e4 0000 0072 5400 0000 da0b 6375 7272  r....rT.....curr
-000110d0: 656e 745f 7461 6272 ab01 0000 da0b 636f  ent_tabr......co
-000110e0: 6e63 6174 5f64 6174 61da 0e74 6f5f 696e  ncat_data..to_in
-000110f0: 7465 7270 6f6c 6174 65da 0763 7572 5f74  terpolate..cur_t
-00011100: 6162 7246 0200 0072 4302 0000 7244 0200  abrF...rC...rD..
-00011110: 0072 4502 0000 da0c 7472 6169 6e5f 6272  .rE.....train_br
-00011120: 6561 6b73 da0b 7270 745f 6c65 6e67 7468  eaks..rpt_length
-00011130: 7372 8c00 0000 da0b 7465 7374 5f62 7265  sr......test_bre
-00011140: 616b 73da 0c73 6875 6666 6c65 5f74 6573  aks..shuffle_tes
-00011150: 74da 0d73 6875 6666 6c65 5f74 7261 696e  t..shuffle_train
-00011160: da0d 6d61 785f 7365 716c 656e 6774 68da  ..max_seqlength.
-00011170: 0d58 5f74 7261 696e 5f73 706c 6974 da0c  .X_train_split..
-00011180: 585f 7465 7374 5f73 706c 6974 7226 0000  X_test_splitr&..
-00011190: 0029 0272 9600 0000 7240 0200 0072 2700  .).r....r@...r'.
-000111a0: 0000 728e 0100 000d 0800 0073 cc01 0000  ..r........s....
-000111b0: 0029 0a02 0a03 02fd 0405 0403 1001 0401  .)..............
-000111c0: 0601 1c01 1cff 02ff 02ff 0a06 0601 0401  ................
-000111d0: 0802 0801 0201 02ff 0405 1002 0601 0201  ................
-000111e0: 0201 0201 02fc 0607 0401 0201 0401 04fd  ................
-000111f0: 0604 08fc 0c07 0801 0801 0a01 0802 0602  ................
-00011200: 0a01 1201 0401 18ff 0604 0402 1002 0601  ................
-00011210: 0201 0201 0201 02fc 0607 0401 0aff 1005  ................
-00011220: 0402 1003 0a01 1201 0c02 0201 0e01 1403  ................
-00011230: 0e08 04fa 0201 0401 1c01 1601 02fd 04ff  ................
-00011240: 020d 04fa 0201 0401 1e01 1601 02fd 04ff  ................
-00011250: 0809 1401 06ff 0402 02fe 04ff 0a06 0403  ................
-00011260: 0401 04ff 0e04 0601 0803 0601 0201 0201  ................
-00011270: 1801 0201 0201 0201 02f9 0a0b 1001 1a01  ................
-00011280: 0201 0401 0cff 02ff 0405 1201 1202 1002  ................
-00011290: 0a01 0601 0201 0201 0a01 0aff 0403 0201  ................
-000112a0: 0201 0201 02f7 0c0d 0e02 0c02 1403 0601  ................
-000112b0: 0201 0201 0201 0201 0201 0201 02f9 0a0a  ................
-000112c0: 1001 0a01 0601 0201 0201 0a01 0aff 0403  ................
-000112d0: 0201 0201 0201 02f7 0c0c 0e01 0c02 0601  ................
-000112e0: 0601 12ff 0603 0802 0801 0802 0601 0601  ................
-000112f0: 12ff 0603 0802 0801 0802 1605 02ff 0402  ................
-00011300: 02fe 0403 0cfd 0404 12fc 0406 1801 1001  ................
-00011310: 0401 0201 1601 02fd 0806 0401 0201 1601  ................
-00011320: 02fd 0606 0601 0802 0c02 12ff 0602 0401  ................
-00011330: 10ff 02fe 0405 0c02 12ff 0602 02fe 0405  ................
-00011340: 1a01 0a01 0a01 0401 0201 0601 0601 0401  ................
-00011350: 0a02 10fe 04ff 02fe 02ff 02ff 040c 0401  ................
-00011360: 0201 0601 0601 0401 0a02 10fe 04ff 02fe  ................
-00011370: 02ff 02ff 080d 1201 08ff 0804 7a14 5461  ............z.Ta
-00011380: 626c 6544 6963 742e 7072 6570 726f 6365  bleDict.preproce
-00011390: 7373 2902 7292 0000 004e 2902 7292 0000  ss).r....N).r...
-000113a0: 0072 d501 0000 2902 7292 0000 0072 d501  .r....).r....r..
-000113b0: 0000 2901 7292 0000 0029 014e 2901 7201  ..).r....).N).r.
-000113c0: 0000 0029 0c46 72d7 0000 0072 4a02 0000  ...).Fr....rJ...
-000113d0: 7231 0000 0072 4b02 0000 4e72 0100 0000  r1...rK...Nr....
-000113e0: 7201 0000 0046 4672 d101 0000 4e29 2272  r....FFr....N)"r
-000113f0: 5800 0000 7228 0100 0072 2901 0000 722a  X...r(...r)...r*
-00011400: 0100 0072 d100 0000 7212 0000 0072 a200  ...r....r....r..
-00011410: 0000 72dd 0000 0072 de00 0000 7213 0000  ..r....r....r...
-00011420: 0072 9b01 0000 72f9 0100 0072 2b01 0000  .r....r....r+...
-00011430: 722c 0100 0072 1100 0000 7269 0000 0072  r,...r....ri...r
-00011440: b500 0000 72fa 0100 0072 0802 0000 720d  ....r....r....r.
-00011450: 0200 0072 f801 0000 7216 0200 0072 1f01  ...r....r....r..
-00011460: 0000 7214 0000 0072 0f00 0000 7221 0200  ..r....r....r!..
-00011470: 0072 0600 0000 721b 0200 0072 1d02 0000  .r....r....r....
-00011480: 7227 0200 0072 9601 0000 7249 0200 0072  r'...r....rI...r
-00011490: 8e01 0000 da0d 5f5f 636c 6173 7363 656c  ......__classcel
-000114a0: 6c5f 5f72 2600 0000 7226 0000 0072 0202  l__r&...r&...r..
-000114b0: 0000 7227 0000 0072 da00 0000 8c06 0000  ..r'...r........
-000114c0: 739c 0000 0008 0104 0902 0102 0108 0102  s...............
-000114d0: 0102 0102 0102 0102 0102 f402 0202 0102  ................
-000114e0: 0102 0104 0102 0102 0104 0102 0102 0102  ................
-000114f0: 010a f410 2b10 1710 2110 1300 0100 fc02  ....+...!.......
-00011500: 0202 0102 0102 010a fb0c 2500 ff02 0104  ..........%.....
-00011510: 010a fe0c 111c 1100 fe02 0202 010a fd0c  ................
-00011520: 1612 1b0e 3600 ff02 0104 0102 fe0c 6000  ....6.........`.
-00011530: 0100 0100 0100 0100 0100 0100 0100 0100  ................
-00011540: 0100 0100 0100 f302 0302 0102 0102 0102  ................
-00011550: 0102 0102 0102 0102 0102 0102 0102 0104  ................
-00011560: f272 da00 0000 da08 5f5f 6d61 696e 5f5f  .r......__main__
-00011570: da01 32da 1454 465f 4350 505f 4d49 4e5f  ..2..TF_CPP_MIN_
-00011580: 4c4f 475f 4c45 5645 4c29 4272 2a01 0000  LOG_LEVEL)Br*...
-00011590: da0b 636f 6c6c 6563 7469 6f6e 7372 0200  ..collectionsr..
-000115a0: 0000 da0d 706b 675f 7265 736f 7572 6365  ....pkg_resource
-000115b0: 7372 0300 0000 da10 7368 6170 656c 792e  sr......shapely.
-000115c0: 6765 6f6d 6574 7279 7204 0000 0072 7500  geometryr....ru.
-000115d0: 0000 7205 0000 00da 0773 6b6c 6561 726e  ..r......sklearn
-000115e0: 7206 0000 00da 1573 6b6c 6561 726e 2e64  r......sklearn.d
-000115f0: 6563 6f6d 706f 7369 7469 6f6e 7207 0000  ecompositionr...
-00011600: 00da 1073 6b6c 6561 726e 2e6d 616e 6966  ...sklearn.manif
-00011610: 6f6c 6472 0800 0000 da15 736b 6c65 6172  oldr......sklear
-00011620: 6e2e 7072 6570 726f 6365 7373 696e 6772  n.preprocessingr
-00011630: 0900 0000 720a 0000 0072 0b00 0000 720c  ....r....r....r.
-00011640: 0000 0072 0d00 0000 720e 0000 00da 0674  ...r....r......t
-00011650: 7970 696e 6772 0f00 0000 7210 0000 0072  ypingr....r....r
-00011660: 1100 0000 7212 0000 0072 1300 0000 7214  ....r....r....r.
-00011670: 0000 0072 cc00 0000 da08 6461 7465 7469  ...r......dateti
-00011680: 6d65 da04 6d61 7468 da11 6d61 7470 6c6f  me..math..matplo
-00011690: 746c 6962 2e70 7970 6c6f 74da 0670 7970  tlib.pyplot..pyp
-000116a0: 6c6f 74da 0370 6c74 da08 6e65 7477 6f72  lot..plt..networ
-000116b0: 6b78 729b 0100 00da 056e 756d 7079 72dd  kxr......numpyr.
-000116c0: 0000 0072 1d00 0000 da06 7061 6e64 6173  ...r......pandas
-000116d0: 72be 0000 0072 2000 0000 7221 0100 0072  r....r ...r!...r
-000116e0: c500 0000 da0a 7465 6e73 6f72 666c 6f77  ......tensorflow
-000116f0: da02 7466 721d 0200 0072 1101 0000 da12  ..tfr....r......
-00011700: 6465 6570 6f66 2e6d 6f64 656c 5f75 7469  deepof.model_uti
-00011710: 6c73 7281 0000 00da 0d64 6565 706f 662e  lsr......deepof.
-00011720: 6d6f 6465 6c73 da17 6465 6570 6f66 2e61  models..deepof.a
-00011730: 6e6e 6f74 6174 696f 6e5f 7574 696c 73da  nnotation_utils.
-00011740: 0c64 6565 706f 662e 7574 696c 73da 0e64  .deepof.utils..d
-00011750: 6565 706f 662e 7669 7375 616c 73da 0770  eepof.visuals..p
-00011760: 726f 6a65 6374 7225 0000 0072 fa01 0000  rojectr%...r....
-00011770: 72a2 0000 0072 2800 0000 7229 0000 0072  r....r(...r)...r
-00011780: 1a00 0000 722c 0100 0072 da00 0000 7258  ....r,...r....rX
-00011790: 0000 00da 0765 6e76 6972 6f6e 7226 0000  .....environr&..
-000117a0: 0072 2600 0000 7226 0000 0072 2700 0000  .r&...r&...r'...
-000117b0: da08 3c6d 6f64 756c 653e 0100 0000 7374  ..<module>....st
-000117c0: 0000 0004 100c 010c 010c 010c 010c 010c  ................
-000117d0: 010c 0118 060c 010c 0114 0118 0108 0108  ................
-000117e0: 0108 010c 0108 0108 0108 0108 0108 0108  ................
-000117f0: 0108 0108 0108 0108 0108 0208 0108 0108  ................
-00011800: 0108 0108 030a 010a 010a 0610 130e 7f00  ................
-00011810: 7f00 7f00 7f00 7f00 0b0e 7f00 7f00 7f00  ................
-00011820: 7f00 7f00 7f00 7f00 3910 7f00 7f00 7f00  ........9.......
-00011830: 7f00 7f00 4a0a 02                        ....J..
+00000090: 0100 6401 640a 6c11 6d12 5a12 6d13 5a13  ..d.d.l.m.Z.m.Z.
+000000a0: 6d14 5a14 6d15 5a15 0100 6401 640b 6c16  m.Z.m.Z...d.d.l.
+000000b0: 6d16 5a16 0100 6401 640c 6c17 6d17 5a17  m.Z...d.d.l.m.Z.
+000000c0: 0100 6401 640d 6c18 6d19 5a19 6d1a 5a1a  ..d.d.l.m.Z.m.Z.
+000000d0: 6d1b 5a1b 0100 6401 640e 6c18 6d1c 5a1c  m.Z...d.d.l.m.Z.
+000000e0: 6d1d 5a1d 6d1e 5a1e 6d19 5a19 0100 6401  m.Z.m.Z.m.Z...d.
+000000f0: 640f 6c1f 5a1f 6401 640f 6c20 5a20 6401  d.l.Z.d.d.l Z d.
+00000100: 640f 6c21 5a21 6401 640f 6c22 6d23 5a24  d.l!Z!d.d.l"m#Z$
+00000110: 0100 6401 640f 6c25 5a26 6401 640f 6c27  ..d.d.l%Z&d.d.l'
+00000120: 5a28 6401 640f 6c29 5a29 6401 640f 6c2a  Z(d.d.l)Z)d.d.l*
+00000130: 5a2b 6401 640f 6c2c 5a2c 6401 640f 6c2d  Z+d.d.l,Z,d.d.l-
+00000140: 5a2d 6401 640f 6c2e 5a2e 6401 640f 6c09  Z-d.d.l.Z.d.d.l.
+00000150: 5a09 6401 640f 6c2f 5a30 6401 640f 6c31  Z.d.d.l/Z0d.d.l1
+00000160: 5a31 6401 640f 6c32 5a32 6401 640f 6c33  Z1d.d.l2Z2d.d.l3
+00000170: 5a34 6401 640f 6c35 5a34 6401 640f 6c36  Z4d.d.l5Z4d.d.l6
+00000180: 5a34 6401 640f 6c37 5a34 6401 640f 6c38  Z4d.d.l7Z4d.d.l8
+00000190: 5a34 651a 6410 6519 8302 5a39 651a 6411  Z4e.d.e...Z9e.d.
+000001a0: 6519 8302 5a3a 651a 6412 6519 8302 5a3b  e...Z:e.d.e...Z;
+000001b0: 653c 653a 6413 9c02 6414 6415 8404 5a3d  e<e:d...d.d...Z=
+000001c0: 4700 6416 6417 8400 6417 8302 5a3e 4700  G.d.d...d...Z>G.
+000001d0: 6418 6419 8400 6419 8302 5a3f 4700 641a  d.d...d...Z?G.d.
+000001e0: 641b 8400 641b 6540 8303 5a41 6542 641c  d...d.e@..ZAeBd.
+000001f0: 6b02 9001 72d2 641d 6529 6a43 641e 3c00  k...r.d.e)jCd.<.
+00000200: 640f 5300 291f 61c9 0200 0044 6174 6120  d.S.).a....Data 
+00000210: 7374 7275 6374 7572 6573 2066 6f72 2070  structures for p
+00000220: 7265 7072 6f63 6573 7369 6e67 2061 6e64  reprocessing and
+00000230: 2077 7261 6e67 6c69 6e67 206f 6620 444c   wrangling of DL
+00000240: 4320 6f75 7470 7574 2064 6174 612e 2054  C output data. T
+00000250: 6869 7320 6973 2074 6865 206d 6169 6e20  his is the main 
+00000260: 6d6f 6475 6c65 2068 616e 646c 6564 2062  module handled b
+00000270: 7920 7468 6520 7573 6572 2e0a 0a54 6865  y the user...The
+00000280: 7265 2061 7265 2074 6872 6565 206d 6169  re are three mai
+00000290: 6e20 6461 7461 2073 7472 7563 7475 7265  n data structure
+000002a0: 7320 746f 2070 6179 2061 7474 656e 7469  s to pay attenti
+000002b0: 6f6e 2074 6f3a 0a2d 203a 636c 6173 733a  on to:.- :class:
+000002c0: 607e 6465 6570 6f66 2e64 6174 612e 5072  `~deepof.data.Pr
+000002d0: 6f6a 6563 7460 2c20 7768 6963 6820 7365  oject`, which se
+000002e0: 7276 6573 2061 7320 6120 636f 6e66 6967  rves as a config
+000002f0: 7572 6174 696f 6e20 6875 6220 666f 7220  uration hub for 
+00000300: 7468 6520 7768 6f6c 6520 7069 7065 6c69  the whole pipeli
+00000310: 6e65 0a2d 203a 636c 6173 733a 607e 6465  ne.- :class:`~de
+00000320: 6570 6f66 2e64 6174 612e 436f 6f72 6469  epof.data.Coordi
+00000330: 6e61 7465 7360 2c20 7768 6963 6820 6163  nates`, which ac
+00000340: 7473 2061 7320 616e 2069 6e74 6572 6d65  ts as an interme
+00000350: 6469 6172 7920 6265 7477 6565 6e20 7072  diary between pr
+00000360: 6f6a 6563 7420 636f 6e66 6967 7572 6174  oject configurat
+00000370: 696f 6e20 616e 6420 6461 7461 2c20 616e  ion and data, an
+00000380: 6420 636f 6e74 6169 6e73 0a61 2070 6c65  d contains.a ple
+00000390: 7468 6f72 6120 6f66 2070 726f 6365 7373  thora of process
+000003a0: 696e 6720 6d65 7468 6f64 7320 746f 2061  ing methods to a
+000003b0: 7070 6c79 2c20 616e 640a 2d20 3a63 6c61  pply, and.- :cla
+000003c0: 7373 3a60 7e64 6565 706f 662e 6461 7461  ss:`~deepof.data
+000003d0: 2e54 6162 6c65 4469 6374 602c 2077 6869  .TableDict`, whi
+000003e0: 6368 2069 7320 7468 6520 6d61 696e 2064  ch is the main d
+000003f0: 6174 6120 7374 7275 6374 7572 6520 746f  ata structure to
+00000400: 2073 746f 7265 2074 6865 2064 6174 612c   store the data,
+00000410: 2068 6176 696e 6720 6578 7065 7269 6d65   having experime
+00000420: 6e74 2049 4473 2061 7320 6b65 7973 0a61  nt IDs as keys.a
+00000430: 6e64 2070 726f 6365 7373 6564 2074 696d  nd processed tim
+00000440: 652d 7365 7269 6573 2061 7320 7661 6c75  e-series as valu
+00000450: 6573 2069 6e20 6120 6469 6374 696f 6e61  es in a dictiona
+00000460: 7279 2d6c 696b 6520 6f62 6a65 6374 2e0a  ry-like object..
+00000470: 0a46 6f72 2061 2064 6574 6169 6c65 6420  .For a detailed 
+00000480: 7475 746f 7269 616c 206f 6e20 686f 7720  tutorial on how 
+00000490: 746f 2075 7365 2074 6869 7320 6d6f 6475  to use this modu
+000004a0: 6c65 2c20 7365 6520 7468 6520 6164 7661  le, see the adva
+000004b0: 6e63 6564 2074 7574 6f72 6961 6c73 2069  nced tutorials i
+000004c0: 6e20 7468 6520 6d61 696e 2073 6563 7469  n the main secti
+000004d0: 6f6e 2e0a e900 0000 0029 01da 0b64 6566  on.......)...def
+000004e0: 6175 6c74 6469 6374 2901 da11 6765 745f  aultdict)...get_
+000004f0: 636c 6f73 655f 6d61 7463 6865 7329 01da  close_matches)..
+00000500: 1172 6573 6f75 7263 655f 6669 6c65 6e61  .resource_filena
+00000510: 6d65 2901 da07 506f 6c79 676f 6e29 01da  me)...Polygon)..
+00000520: 0672 6d74 7265 6529 01da 1172 616e 646f  .rmtree)...rando
+00000530: 6d5f 7072 6f6a 6563 7469 6f6e 2901 da09  m_projection)...
+00000540: 4b65 726e 656c 5043 4129 01da 0454 534e  KernelPCA)...TSN
+00000550: 4529 04da 0c4d 696e 4d61 7853 6361 6c65  E)...MinMaxScale
+00000560: 72da 0e53 7461 6e64 6172 6453 6361 6c65  r..StandardScale
+00000570: 72da 0c52 6f62 7573 7453 6361 6c65 72da  r..RobustScaler.
+00000580: 0c4c 6162 656c 456e 636f 6465 7229 01da  .LabelEncoder)..
+00000590: 0474 696d 6529 01da 0474 7164 6d29 03da  .time)...tqdm)..
+000005a0: 0341 6e79 da07 4e65 7754 7970 65da 0555  .Any..NewType..U
+000005b0: 6e69 6f6e 2904 da04 4469 6374 da04 4c69  nion)...Dict..Li
+000005c0: 7374 da05 5475 706c 6572 1000 0000 4eda  st..Tupler....N.
+000005d0: 0e64 6565 706f 665f 7072 6f6a 6563 74da  .deepof_project.
+000005e0: 1264 6565 706f 665f 636f 6f72 6469 6e61  .deepof_coordina
+000005f0: 7465 73da 1164 6565 706f 665f 7461 626c  tes..deepof_tabl
+00000600: 655f 6469 6374 2902 da0c 7072 6f6a 6563  e_dict)...projec
+00000610: 745f 7061 7468 da06 7265 7475 726e 6301  t_path..returnc.
+00000620: 0000 0000 0000 0000 0000 0003 0000 0008  ................
+00000630: 0000 0043 0000 0073 5600 0000 7400 7401  ...C...sV...t.t.
+00000640: 6a02 a003 7c00 6401 6402 a103 6403 8302  j...|.d.d...d...
+00000650: 8f1a 7d01 7404 a005 7c01 a101 7d02 5700  ..}.t...|...}.W.
+00000660: 6404 0400 0400 8303 0100 6e10 3100 7336  d.........n.1.s6
+00000670: 3000 0100 0100 0100 5900 0100 7401 6a02  0.......Y...t.j.
+00000680: a006 7c00 a101 6405 1900 7c02 5f07 7c02  ..|...d...|._.|.
+00000690: 5300 2906 7aa5 4c6f 6164 2061 2070 7265  S.).z.Load a pre
+000006a0: 2d73 6176 6564 2070 6963 6b6c 6564 2043  -saved pickled C
+000006b0: 6f6f 7264 696e 6174 6573 206f 626a 6563  oordinates objec
+000006c0: 742e 0a0a 2020 2020 4172 6773 3a0a 2020  t...    Args:.  
+000006d0: 2020 2020 2020 7072 6f6a 6563 745f 7061        project_pa
+000006e0: 7468 2028 7374 7229 3a20 6e61 6d65 206f  th (str): name o
+000006f0: 6620 7468 6520 6669 6c65 2074 6f20 6c6f  f the file to lo
+00000700: 6164 2e0a 0a20 2020 2052 6574 7572 6e73  ad...    Returns
+00000710: 3a0a 2020 2020 2020 2020 5072 652d 7275  :.        Pre-ru
+00000720: 6e20 636f 6f72 6469 6e61 7465 7320 6f62  n coordinates ob
+00000730: 6a65 6374 2e0a 0a20 2020 20da 0b43 6f6f  ject...    ..Coo
+00000740: 7264 696e 6174 6573 7a16 6465 6570 6f66  rdinatesz.deepof
+00000750: 5f63 6f6f 7264 696e 6174 6573 2e70 6b6c  _coordinates.pkl
+00000760: da02 7262 4e72 0100 0000 2908 da04 6f70  ..rbNr....)...op
+00000770: 656e da02 6f73 da04 7061 7468 da04 6a6f  en..os..path..jo
+00000780: 696e da06 7069 636b 6c65 da04 6c6f 6164  in..pickle..load
+00000790: da05 7370 6c69 74da 0d5f 7072 6f6a 6563  ..split.._projec
+000007a0: 745f 7061 7468 2903 7219 0000 00da 0668  t_path).r......h
+000007b0: 616e 646c 65da 0b63 6f6f 7264 696e 6174  andle..coordinat
+000007c0: 6573 a900 7227 0000 00fa 3a2f 5573 6572  es..r'....:/User
+000007d0: 732f 6c75 6361 735f 6d69 7261 6e64 612f  s/lucas_miranda/
+000007e0: 5079 6368 6172 6d50 726f 6a65 6374 732f  PycharmProjects/
+000007f0: 6465 6570 6f66 2f64 6565 706f 662f 6461  deepof/deepof/da
+00000800: 7461 2e70 79da 0c6c 6f61 645f 7072 6f6a  ta.py..load_proj
+00000810: 6563 7442 0000 0073 0e00 0000 000a 0201  ectB...s........
+00000820: 10ff 0402 0201 2802 1201 7229 0000 0063  ......(...r)...c
+00000830: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000840: 1500 0000 4000 0000 7356 0100 0065 005a  ....@...sV...e.Z
+00000850: 0164 005a 0264 015a 0364 0264 0364 0464  .d.Z.d.Z.d.d.d.d
+00000860: 0565 0464 0667 0183 0164 0264 0764 0864  .e.d.g...d.d.d.d
+00000870: 0964 0a64 0b64 0c65 056a 06a0 0764 0da1  .d.d.d.e.j...d..
+00000880: 0164 0264 0264 0e64 0f64 1064 0e66 1365  .d.d.d.d.d.d.f.e
+00000890: 0865 0965 0965 0a65 0865 0b65 0a65 0c65  .e.e.e.e.e.e.e.e
+000008a0: 0c65 0d65 0965 0965 0965 0965 0965 0d65  .e.e.e.e.e.e.e.e
+000008b0: 0965 0965 0c64 119c 1364 1264 1384 055a  .e.e.d...d.d...Z
+000008c0: 0e64 1464 1584 005a 0f64 1664 1784 005a  .d.d...Z.d.d...Z
+000008d0: 1064 1864 1984 005a 1165 1264 1a64 1b84  .d.d...Z.e.d.d..
+000008e0: 0083 015a 1365 1264 1c64 1d84 0083 015a  ...Z.e.d.d.....Z
+000008f0: 1465 1264 1e64 1f84 0083 015a 1564 3465  .e.d.d.....Z.d4e
+00000900: 1665 0a65 176a 1864 219c 0364 2264 2384  .e.e.j.d!..d"d#.
+00000910: 055a 1964 3565 0a65 1a64 249c 0264 2564  .Z.d5e.e.d$..d%d
+00000920: 2684 055a 1b64 3665 0b65 0a65 0b64 279c  &..Z.d6e.e.e.d'.
+00000930: 0364 2864 2984 055a 1c64 3765 0b65 0a65  .d(d)..Z.d7e.e.e
+00000940: 0b64 279c 0364 2a64 2b84 055a 1d64 3865  .d'..d*d+..Z.d8e
+00000950: 0b65 0a65 0b64 279c 0364 2c64 2d84 055a  .e.e.d'..d,d-..Z
+00000960: 1e64 3965 0a65 0a65 1f64 2e9c 0364 2f64  .d9e.e.e.d...d/d
+00000970: 3084 055a 2065 136a 2164 3164 1b84 0083  0..Z e.j!d1d....
+00000980: 015a 1365 146a 2164 3264 1d84 0083 015a  .Z.e.j!d2d.....Z
+00000990: 1465 156a 2164 3364 1f84 0083 015a 1564  .e.j!d3d.....Z.d
+000009a0: 0253 0029 3ada 0750 726f 6a65 6374 7a88  .S.):..Projectz.
+000009b0: 436c 6173 7320 666f 7220 6c6f 6164 696e  Class for loadin
+000009c0: 6720 616e 6420 7072 6570 726f 6365 7373  g and preprocess
+000009d0: 696e 6720 444c 4320 6461 7461 206f 6620  ing DLC data of 
+000009e0: 696e 6469 7669 6475 616c 2061 6e64 206d  individual and m
+000009f0: 756c 7469 706c 6520 616e 696d 616c 732e  ultiple animals.
+00000a00: 0a0a 2020 2020 416c 6c20 6d61 696e 2063  ..    All main c
+00000a10: 6f6d 7075 7461 7469 6f6e 7320 6172 6520  omputations are 
+00000a20: 6861 6e64 6c65 6420 6672 6f6d 2068 6572  handled from her
+00000a30: 652e 0a0a 2020 2020 4e7a 1070 6f6c 7967  e...    Nz.polyg
+00000a40: 6f6e 616c 2d6d 616e 7561 6cda 0964 6565  onal-manual..dee
+00000a50: 706f 665f 3134 e9fa 0000 00da 0054 e905  pof_14.......T..
+00000a60: 0000 00e9 0300 0000 6700 0000 0000 00e8  ........g.......
+00000a70: 3fda 0d6d 6f75 7365 5f74 6f70 7669 6577  ?..mouse_topview
+00000a80: 7216 0000 00da 012e e901 0000 00da 0a61  r..............a
+00000a90: 7574 6f64 6574 6563 747a 042e 6d70 3429  utodetectz..mp4)
+00000aa0: 13da 0a61 6e69 6d61 6c5f 6964 73da 0561  ...animal_ids..a
+00000ab0: 7265 6e61 da0e 626f 6479 7061 7274 5f67  rena..bodypart_g
+00000ac0: 7261 7068 da1b 656e 6162 6c65 5f69 7465  raph..enable_ite
+00000ad0: 7261 7469 7665 5f69 6d70 7574 6174 696f  rative_imputatio
+00000ae0: 6eda 1165 7863 6c75 6465 5f62 6f64 7970  n..exclude_bodyp
+00000af0: 6172 7473 da0e 6578 705f 636f 6e64 6974  arts..exp_condit
+00000b00: 696f 6e73 da14 696e 7465 7270 6f6c 6174  ions..interpolat
+00000b10: 655f 6f75 746c 6965 7273 da13 696e 7465  e_outliers..inte
+00000b20: 7270 6f6c 6174 696f 6e5f 6c69 6d69 74da  rpolation_limit.
+00000b30: 1169 6e74 6572 706f 6c61 7469 6f6e 5f73  .interpolation_s
+00000b40: 7464 da0e 6c69 6b65 6c69 686f 6f64 5f74  td..likelihood_t
+00000b50: 6f6c da05 6d6f 6465 6cda 0c70 726f 6a65  ol..model..proje
+00000b60: 6374 5f6e 616d 6572 1900 0000 da0a 7669  ct_namer......vi
+00000b70: 6465 6f5f 7061 7468 da0a 7461 626c 655f  deo_path..table_
+00000b80: 7061 7468 da0c 736d 6f6f 7468 5f61 6c70  path..smooth_alp
+00000b90: 6861 da0c 7461 626c 655f 666f 726d 6174  ha..table_format
+00000ba0: da0c 7669 6465 6f5f 666f 726d 6174 da0b  ..video_format..
+00000bb0: 7669 6465 6f5f 7363 616c 6563 1400 0000  video_scalec....
+00000bc0: 0000 0000 0000 0000 1500 0000 0500 0000  ................
+00000bd0: 0300 0000 7358 0100 007c 0d88 005f 007c  ....sX...|..._.|
+00000be0: 0c88 005f 017c 0e88 005f 027c 0f88 005f  ..._.|..._.|..._
+00000bf0: 0374 0474 0564 0183 0288 005f 067c 1188  .t.t.d....._.|..
+00000c00: 005f 0788 006a 0764 026b 0272 6c64 0364  ._...j.d.k.rld.d
+00000c10: 0484 0074 08a0 0988 006a 03a1 0144 0083  ...t.....j...D..
+00000c20: 0164 0519 007d 1464 067c 1476 0072 5e64  .d...}.d.|.v.r^d
+00000c30: 0688 005f 076e 0e64 077c 1476 0072 6c64  ..._.n.d.|.v.rld
+00000c40: 0788 005f 0774 0a87 0166 0164 0864 0484  ..._.t...f.d.d..
+00000c50: 0874 08a0 0988 006a 02a1 0144 0083 0183  .t.....j...D....
+00000c60: 0188 005f 0b74 0a87 0066 0164 0964 0484  ..._.t...f.d.d..
+00000c70: 0874 08a0 0988 006a 03a1 0144 0083 0183  .t.....j...D....
+00000c80: 0188 005f 0c74 0d88 006a 0b83 0174 0d88  ..._.t...j...t..
+00000c90: 006a 0c83 016b 0273 c84a 0064 0a83 0182  .j...k.s.J.d....
+00000ca0: 017c 0288 005f 0e7c 1388 005f 0f64 0b88  .|..._.|..._.d..
+00000cb0: 005f 1064 0c88 005f 117c 0164 0b75 0172  ._.d..._.|.d.u.r
+00000cc0: ec7c 016e 0464 0d67 0188 005f 1264 0c88  .|.n.d.g..._.d..
+00000cd0: 005f 137c 0388 005f 1464 0b88 005f 1564  ._.|..._.d..._.d
+00000ce0: 0e88 005f 1664 0f88 005f 177c 0688 005f  ..._.d..._.|..._
+00000cf0: 187c 0788 005f 197c 0888 005f 1a7c 0988  .|..._.|..._.|..
+00000d00: 005f 1b7c 0a88 005f 1c7c 0b88 005f 1d7c  ._.|..._.|..._.|
+00000d10: 1088 005f 1e64 0b88 005f 1f88 0188 005f  ..._.d..._....._
+00000d20: 207c 0488 005f 217c 0588 005f 2264 0b53   |..._!|..._"d.S
+00000d30: 0029 1061 1b08 0000 496e 6974 6961 6c69  .).a....Initiali
+00000d40: 7a65 2061 2050 726f 6a65 6374 206f 626a  ze a Project obj
+00000d50: 6563 742e 0a0a 2020 2020 2020 2020 4172  ect...        Ar
+00000d60: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+00000d70: 616e 696d 616c 5f69 6473 2028 6c69 7374  animal_ids (list
+00000d80: 293a 206c 6973 7420 6f66 2061 6e69 6d61  ): list of anima
+00000d90: 6c20 6964 732e 0a20 2020 2020 2020 2020  l ids..         
+00000da0: 2020 2061 7265 6e61 2028 7374 7229 3a20     arena (str): 
+00000db0: 6172 656e 6120 7479 7065 2e20 4361 6e20  arena type. Can 
+00000dc0: 6265 206f 6e65 206f 6620 2263 6972 6375  be one of "circu
+00000dd0: 6c61 722d 6175 746f 6465 7465 6374 222c  lar-autodetect",
+00000de0: 2022 6369 7263 756c 6172 2d6d 616e 7561   "circular-manua
+00000df0: 6c22 2c20 6f72 2022 706f 6c79 676f 6e2d  l", or "polygon-
+00000e00: 6d61 6e75 616c 222e 0a20 2020 2020 2020  manual"..       
+00000e10: 2020 2020 2062 6f64 7970 6172 745f 6772       bodypart_gr
+00000e20: 6170 6820 2873 7472 293a 2062 6f64 7920  aph (str): body 
+00000e30: 7061 7274 2073 6368 656d 6520 746f 2075  part scheme to u
+00000e40: 7365 2066 6f72 2074 6865 2061 6e61 6c79  se for the analy
+00000e50: 7369 732e 2044 6566 6175 6c74 7320 746f  sis. Defaults to
+00000e60: 204e 6f6e 652c 2069 6e20 7768 6963 6820   None, in which 
+00000e70: 6361 7365 2074 6865 2070 726f 6772 616d  case the program
+00000e80: 2077 696c 6c20 6174 7465 6d70 7420 746f   will attempt to
+00000e90: 2073 656c 6563 7420 6974 2061 7574 6f6d   select it autom
+00000ea0: 6174 6963 616c 6c79 2062 6173 6564 206f  atically based o
+00000eb0: 6e20 7468 6520 6176 6169 6c61 626c 6520  n the available 
+00000ec0: 626f 6479 2070 6172 7473 2e0a 2020 2020  body parts..    
+00000ed0: 2020 2020 2020 2020 656e 6162 6c65 5f69          enable_i
+00000ee0: 7465 7261 7469 7665 5f69 6d70 7574 6174  terative_imputat
+00000ef0: 696f 6e20 2862 6f6f 6c29 3a20 7768 6574  ion (bool): whet
+00000f00: 6865 7220 746f 2075 7365 2069 7465 7261  her to use itera
+00000f10: 7469 7665 2069 6d70 7574 6174 696f 6e20  tive imputation 
+00000f20: 666f 7220 6f63 636c 7564 6564 2062 6f64  for occluded bod
+00000f30: 7920 7061 7274 732e 2052 6563 6f6d 6d65  y parts. Recomme
+00000f40: 6e64 6564 2069 6620 7365 7665 7261 6c20  nded if several 
+00000f50: 616e 696d 616c 7320 6172 6520 7072 6573  animals are pres
+00000f60: 656e 742c 2062 7574 2073 6c6f 7765 722e  ent, but slower.
+00000f70: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
+00000f80: 6c75 6465 5f62 6f64 7970 6172 7473 2028  lude_bodyparts (
+00000f90: 6c69 7374 293a 206c 6973 7420 6f66 2062  list): list of b
+00000fa0: 6f64 7970 6172 7473 2074 6f20 6578 636c  odyparts to excl
+00000fb0: 7564 6520 6672 6f6d 2061 6e61 6c79 7369  ude from analysi
+00000fc0: 732e 0a20 2020 2020 2020 2020 2020 2065  s..            e
+00000fd0: 7870 5f63 6f6e 6469 7469 6f6e 7320 2864  xp_conditions (d
+00000fe0: 6963 7429 3a20 6469 6374 696f 6e61 7279  ict): dictionary
+00000ff0: 2077 6974 6820 6578 7065 7269 6d65 6e74   with experiment
+00001000: 2049 4473 2061 7320 6b65 7973 2061 6e64   IDs as keys and
+00001010: 2065 7870 6572 696d 656e 7461 6c20 636f   experimental co
+00001020: 6e64 6974 696f 6e73 2061 7320 7661 6c75  nditions as valu
+00001030: 6573 2e0a 2020 2020 2020 2020 2020 2020  es..            
+00001040: 696e 7465 7270 6f6c 6174 655f 6f75 746c  interpolate_outl
+00001050: 6965 7273 2028 626f 6f6c 293a 2077 6865  iers (bool): whe
+00001060: 7468 6572 2074 6f20 696e 7465 7270 6f6c  ther to interpol
+00001070: 6174 6520 6d69 7373 696e 6720 6461 7461  ate missing data
+00001080: 2e0a 2020 2020 2020 2020 2020 2020 696e  ..            in
+00001090: 7465 7270 6f6c 6174 696f 6e5f 6c69 6d69  terpolation_limi
+000010a0: 7420 2869 6e74 293a 206d 6178 696d 756d  t (int): maximum
+000010b0: 206e 756d 6265 7220 6f66 206d 6973 7369   number of missi
+000010c0: 6e67 2066 7261 6d65 7320 746f 2069 6e74  ng frames to int
+000010d0: 6572 706f 6c61 7465 2e0a 2020 2020 2020  erpolate..      
+000010e0: 2020 2020 2020 696e 7465 7270 6f6c 6174        interpolat
+000010f0: 696f 6e5f 7374 6420 2869 6e74 293a 206d  ion_std (int): m
+00001100: 6178 696d 756d 206e 756d 6265 7220 6f66  aximum number of
+00001110: 2073 7461 6e64 6172 6420 6465 7669 6174   standard deviat
+00001120: 696f 6e73 2074 6f20 696e 7465 7270 6f6c  ions to interpol
+00001130: 6174 652e 0a20 2020 2020 2020 2020 2020  ate..           
+00001140: 206c 696b 656c 6968 6f6f 645f 746f 6c20   likelihood_tol 
+00001150: 2866 6c6f 6174 293a 206c 696b 656c 6968  (float): likelih
+00001160: 6f6f 6420 7468 7265 7368 6f6c 6420 666f  ood threshold fo
+00001170: 7220 6f75 746c 6965 7220 6465 7465 6374  r outlier detect
+00001180: 696f 6e2e 0a20 2020 2020 2020 2020 2020  ion..           
+00001190: 206d 6f64 656c 2028 7374 7229 3a20 6d6f   model (str): mo
+000011a0: 6465 6c20 746f 2075 7365 2066 6f72 2070  del to use for p
+000011b0: 6f73 6520 6573 7469 6d61 7469 6f6e 2e20  ose estimation. 
+000011c0: 4465 6661 756c 7473 2074 6f20 276d 6f75  Defaults to 'mou
+000011d0: 7365 5f74 6f70 7669 6577 2720 2861 7320  se_topview' (as 
+000011e0: 6465 7363 7269 6265 6420 696e 2074 6865  described in the
+000011f0: 2064 6f63 756d 656e 7461 7469 6f6e 292e   documentation).
+00001200: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
+00001210: 6a65 6374 5f6e 616d 6520 2873 7472 293a  ject_name (str):
+00001220: 206e 616d 6520 6f66 2074 6865 2063 7572   name of the cur
+00001230: 7265 6e74 2070 726f 6a65 6374 2e0a 2020  rent project..  
+00001240: 2020 2020 2020 2020 2020 7072 6f6a 6563            projec
+00001250: 745f 7061 7468 2028 7374 7229 3a20 7061  t_path (str): pa
+00001260: 7468 2074 6f20 7468 6520 666f 6c64 6572  th to the folder
+00001270: 2063 6f6e 7461 696e 696e 6720 7468 6520   containing the 
+00001280: 444c 4320 6f75 7470 7574 2064 6174 612e  DLC output data.
+00001290: 0a20 2020 2020 2020 2020 2020 2076 6964  .            vid
+000012a0: 656f 5f70 6174 6820 2873 7472 293a 2070  eo_path (str): p
+000012b0: 6174 6820 7768 6572 6520 746f 2066 696e  ath where to fin
+000012c0: 6420 7468 6520 7669 6465 6f73 2074 6f20  d the videos to 
+000012d0: 7573 652e 2049 6620 6e6f 7420 7370 6563  use. If not spec
+000012e0: 6966 6965 642c 2064 6565 706f 662c 2061  ified, deepof, a
+000012f0: 7373 756d 6573 2074 6865 7920 6172 6520  ssumes they are 
+00001300: 696e 2079 6f75 7220 7072 6f6a 6563 7420  in your project 
+00001310: 7061 7468 2e0a 2020 2020 2020 2020 2020  path..          
+00001320: 2020 7461 626c 655f 7061 7468 2028 7374    table_path (st
+00001330: 7229 3a20 7061 7468 2077 6865 7265 2074  r): path where t
+00001340: 6f20 6669 6e64 2074 6865 2074 7261 636b  o find the track
+00001350: 7320 746f 2075 7365 2e20 4966 206e 6f74  s to use. If not
+00001360: 2073 7065 6369 6669 6564 2c20 6465 6570   specified, deep
+00001370: 6f66 2c20 6173 7375 6d65 7320 7468 6579  of, assumes they
+00001380: 2061 7265 2069 6e20 796f 7572 2070 726f   are in your pro
+00001390: 6a65 6374 2070 6174 682e 0a20 2020 2020  ject path..     
+000013a0: 2020 2020 2020 2073 6d6f 6f74 685f 616c         smooth_al
+000013b0: 7068 6120 2866 6c6f 6174 293a 2073 6d6f  pha (float): smo
+000013c0: 6f74 6869 6e67 2069 6e74 656e 7369 7479  othing intensity
+000013d0: 2e20 5468 6520 6869 6768 6572 2074 6865  . The higher the
+000013e0: 2076 616c 7565 2c20 7468 6520 6d6f 7265   value, the more
+000013f0: 2073 6d6f 6f74 6869 6e67 2e0a 2020 2020   smoothing..    
+00001400: 2020 2020 2020 2020 7461 626c 655f 666f          table_fo
+00001410: 726d 6174 2028 7374 7229 3a20 666f 726d  rmat (str): form
+00001420: 6174 206f 6620 7468 6520 7461 626c 652e  at of the table.
+00001430: 2044 6566 6175 6c74 7320 746f 2027 6175   Defaults to 'au
+00001440: 746f 6465 7465 6374 272c 2062 7574 2063  todetect', but c
+00001450: 616e 2062 6520 7365 7420 746f 2022 6373  an be set to "cs
+00001460: 7622 206f 7220 2268 3522 2e0a 2020 2020  v" or "h5"..    
+00001470: 2020 2020 2020 2020 7669 6465 6f5f 666f          video_fo
+00001480: 726d 6174 2028 7374 7229 3a20 7669 6465  rmat (str): vide
+00001490: 6f20 666f 726d 6174 2e20 4465 6661 756c  o format. Defaul
+000014a0: 7473 2074 6f20 272e 6d70 3427 2e0a 2020  ts to '.mp4'..  
+000014b0: 2020 2020 2020 2020 2020 7669 6465 6f5f            video_
+000014c0: 7363 616c 6520 2869 6e74 293a 2064 6961  scale (int): dia
+000014d0: 6d65 7465 7220 6f66 2074 6865 2061 7265  meter of the are
+000014e0: 6e61 2069 6e20 6d6d 2028 6966 2074 6865  na in mm (if the
+000014f0: 2061 7265 6e61 2069 7320 726f 756e 6429   arena is round)
+00001500: 206f 7220 6c65 6e67 7468 206f 6620 7468   or length of th
+00001510: 6520 6669 7273 7420 7370 6563 6966 6965  e first specifie
+00001520: 6420 6172 656e 6120 7369 6465 2028 6966  d arena side (if
+00001530: 2074 6865 2061 7265 6e61 2069 7320 706f   the arena is po
+00001540: 6c79 676f 6e61 6c29 2e0a 0a20 2020 2020  lygonal)...     
+00001550: 2020 20da 0e74 7261 696e 6564 5f6d 6f64     ..trained_mod
+00001560: 656c 7372 3300 0000 6301 0000 0000 0000  elsr3...c.......
+00001570: 0000 0000 0002 0000 0005 0000 0053 0000  .............S..
+00001580: 0073 1a00 0000 6700 7c00 5d12 7d01 7c01  .s....g.|.].}.|.
+00001590: a000 6400 a101 7304 7c01 9102 7104 5300  ..d...s.|...q.S.
+000015a0: a901 7231 0000 00a9 01da 0a73 7461 7274  ..r1.......start
+000015b0: 7377 6974 68a9 02da 022e 30da 0169 7227  swith.....0..ir'
+000015c0: 0000 0072 2700 0000 7228 0000 00da 0a3c  ...r'...r(.....<
+000015d0: 6c69 7374 636f 6d70 3e94 0000 00f3 0000  listcomp>.......
+000015e0: 0000 7a24 5072 6f6a 6563 742e 5f5f 696e  ..z$Project.__in
+000015f0: 6974 5f5f 2e3c 6c6f 6361 6c73 3e2e 3c6c  it__.<locals>.<l
+00001600: 6973 7463 6f6d 703e 7201 0000 00fa 032e  istcomp>r.......
+00001610: 6835 fa04 2e63 7376 6301 0000 0000 0000  h5...csvc.......
+00001620: 0000 0000 0002 0000 0005 0000 0013 0000  ................
+00001630: 0073 2400 0000 6700 7c00 5d1c 7d01 7c01  .s$...g.|.].}.|.
+00001640: a000 8800 a101 7204 7c01 a001 6400 a101  ......r.|...d...
+00001650: 7304 7c01 9102 7104 5300 7247 0000 00a9  s.|...q.S.rG....
+00001660: 02da 0865 6e64 7377 6974 6872 4900 0000  ...endswithrI...
+00001670: a902 724b 0000 00da 0376 6964 2901 7244  ..rK.....vid).rD
+00001680: 0000 0072 2700 0000 7228 0000 0072 4d00  ...r'...r(...rM.
+00001690: 0000 9a00 0000 7306 0000 0006 0202 0114  ......s.........
+000016a0: fe63 0100 0000 0000 0000 0000 0000 0200  .c..............
+000016b0: 0000 0500 0000 1300 0000 7326 0000 0067  ..........s&...g
+000016c0: 007c 005d 1e7d 017c 01a0 0088 006a 01a1  .|.].}.|.....j..
+000016d0: 0172 047c 01a0 0264 00a1 0173 047c 0191  .r.|...d...s.|..
+000016e0: 0271 0453 0072 4700 0000 2903 7252 0000  .q.S.rG...).rR..
+000016f0: 0072 4300 0000 7249 0000 0029 0272 4b00  .rC...rI...).rK.
+00001700: 0000 da03 7461 62a9 01da 0473 656c 6672  ....tab....selfr
+00001710: 2700 0000 7228 0000 0072 4d00 0000 a100  '...r(...rM.....
+00001720: 0000 7306 0000 0006 0202 0116 fe7a 4555  ..s..........zEU
+00001730: 6e65 7175 616c 206e 756d 6265 7220 6f66  nequal number of
+00001740: 2076 6964 656f 7320 616e 6420 7461 626c   videos and tabl
+00001750: 6573 2e20 506c 6561 7365 2063 6865 636b  es. Please check
+00001760: 2079 6f75 7220 6669 6c65 2073 7472 7563   your file struc
+00001770: 7475 7265 4e54 722d 0000 00da 0361 6c6c  tureNTr-.....all
+00001780: 4629 2372 1900 0000 723f 0000 0072 4000  F)#r....r?...r@.
+00001790: 0000 7241 0000 0072 0400 0000 da08 5f5f  ..rA...r......__
+000017a0: 6e61 6d65 5f5f da0c 7472 6169 6e65 645f  name__..trained_
+000017b0: 7061 7468 7243 0000 0072 1e00 0000 da07  pathrC...r......
+000017c0: 6c69 7374 6469 72da 0673 6f72 7465 64da  listdir..sorted.
+000017d0: 0676 6964 656f 73da 0674 6162 6c65 73da  .videos..tables.
+000017e0: 036c 656e 7235 0000 00da 0a61 7265 6e61  .lenr5.....arena
+000017f0: 5f64 696d 73da 1165 6c6c 6970 7365 5f64  _dims..ellipse_d
+00001800: 6574 6563 7469 6f6e da06 616e 676c 6573  etection..angles
+00001810: 7234 0000 00da 0561 7265 6173 7236 0000  r4.....areasr6..
+00001820: 00da 0c63 6f6e 6e65 6374 6976 6974 79da  ...connectivity.
+00001830: 0964 6973 7461 6e63 6573 da03 6567 6f72  .distances..egor
+00001840: 3900 0000 723a 0000 0072 3b00 0000 723c  9...r:...r;...r<
+00001850: 0000 00da 146c 696b 656c 6968 6f6f 645f  .....likelihood_
+00001860: 746f 6c65 7261 6e63 6572 3e00 0000 7242  tolerancer>...rB
+00001870: 0000 00da 0a66 7261 6d65 5f72 6174 6572  .....frame_rater
+00001880: 4400 0000 7237 0000 0072 3800 0000 2915  D...r7...r8...).
+00001890: 7257 0000 0072 3400 0000 7235 0000 0072  rW...r4...r5...r
+000018a0: 3600 0000 7237 0000 0072 3800 0000 7239  6...r7...r8...r9
+000018b0: 0000 0072 3a00 0000 723b 0000 0072 3c00  ...r:...r;...r<.
+000018c0: 0000 723d 0000 0072 3e00 0000 723f 0000  ..r=...r>...r?..
+000018d0: 0072 1900 0000 7240 0000 0072 4100 0000  .r....r@...rA...
+000018e0: 7242 0000 0072 4300 0000 7244 0000 0072  rB...rC...rD...r
+000018f0: 4500 0000 da02 6578 7227 0000 0029 0272  E.....exr'...).r
+00001900: 5700 0000 7244 0000 0072 2800 0000 da08  W...rD...r(.....
+00001910: 5f5f 696e 6974 5f5f 5c00 0000 7360 0000  __init__\...s`..
+00001920: 0000 2f06 0106 0106 0106 010c 0306 010a  ../.............
+00001930: 011a 0108 0108 0108 0106 0102 010a 020a  ................
+00001940: fe04 ff06 0702 010a 020a fe04 ff06 070a  ................
+00001950: 0104 ff08 0202 fe04 0506 0106 0106 0306  ................
+00001960: 0114 0106 0106 0106 0106 0106 0106 0106  ................
+00001970: 0106 0106 0106 0106 0106 0106 0106 0106  ................
+00001980: 017a 1050 726f 6a65 6374 2e5f 5f69 6e69  .z.Project.__ini
+00001990: 745f 5f63 0100 0000 0000 0000 0000 0000  t__c............
+000019a0: 0100 0000 0400 0000 4300 0000 7310 0000  ........C...s...
+000019b0: 0064 01a0 0074 017c 006a 0283 01a1 0153  .d...t.|.j.....S
+000019c0: 00a9 027a 1b50 7269 6e74 2074 6865 206f  ...z.Print the o
+000019d0: 626a 6563 7420 746f 2073 7464 6f75 742e  bject to stdout.
+000019e0: 7a1c 6465 6570 6f66 2061 6e61 6c79 7369  z.deepof analysi
+000019f0: 7320 6f66 207b 7d20 7669 6465 6f73 a903  s of {} videos..
+00001a00: da06 666f 726d 6174 725f 0000 0072 5d00  ..formatr_...r].
+00001a10: 0000 7256 0000 0072 2700 0000 7227 0000  ..rV...r'...r'..
+00001a20: 0072 2800 0000 da07 5f5f 7374 725f 5fc4  .r(.....__str__.
+00001a30: 0000 0073 0200 0000 0002 7a0f 5072 6f6a  ...s......z.Proj
+00001a40: 6563 742e 5f5f 7374 725f 5f63 0100 0000  ect.__str__c....
+00001a50: 0000 0000 0000 0000 0100 0000 0400 0000  ................
+00001a60: 4300 0000 7310 0000 0064 01a0 0074 017c  C...s....d...t.|
+00001a70: 006a 0283 01a1 0153 0072 6b00 0000 726c  .j.....S.rk...rl
+00001a80: 0000 0072 5600 0000 7227 0000 0072 2700  ...rV...r'...r'.
+00001a90: 0000 7228 0000 00da 085f 5f72 6570 725f  ..r(.....__repr_
+00001aa0: 5fc8 0000 0073 0200 0000 0002 7a10 5072  _....s......z.Pr
+00001ab0: 6f6a 6563 742e 5f5f 7265 7072 5f5f 6301  oject.__repr__c.
+00001ac0: 0000 0000 0000 0000 0000 0004 0000 000a  ................
+00001ad0: 0000 0003 0000 0073 b401 0000 7400 6a01  .......s....t.j.
+00001ae0: a002 8800 6a03 8800 6a04 a102 7d01 7405  ....j...j...}.t.
+00001af0: 8700 6601 6401 6402 8408 7400 a006 8800  ..f.d.d...t.....
+00001b00: 6a07 a101 4400 8301 8301 6403 6b02 723c  j...D.....d.k.r<
+00001b10: 7408 6404 8301 8201 7405 8700 6601 6405  t.d.....t...f.d.
+00001b20: 6402 8408 7400 a006 8800 6a09 a101 4400  d...t.....j...D.
+00001b30: 8301 8301 6403 6b02 7266 7408 6406 8301  ....d.k.rft.d...
+00001b40: 8201 7400 6a01 a00a 7c01 a101 9001 73a8  ..t.j...|.....s.
+00001b50: 7400 a00b 7c01 a101 0100 7400 a00b 7400  t...|.....t...t.
+00001b60: 6a01 a002 8800 6a03 8800 6a04 6407 a103  j.....j...j.d...
+00001b70: a101 0100 7400 a00b 7400 6a01 a002 8800  ....t...t.j.....
+00001b80: 6a03 8800 6a04 6408 a103 a101 0100 7400  j...j.d.......t.
+00001b90: a00b 7400 6a01 a002 8800 6a03 8800 6a04  ..t.j.....j...j.
+00001ba0: 6409 a103 a101 0100 7400 a00b 7400 6a01  d.......t...t.j.
+00001bb0: a002 8800 6a03 8800 6a04 640a a103 a101  ....j...j.d.....
+00001bc0: 0100 7400 a006 8800 6a07 a101 4400 5d3a  ..t.....j...D.]:
+00001bd0: 7d02 7c02 a00c 8800 6a0d a101 72f2 740e  }.|.....j...r.t.
+00001be0: a00f 7400 6a01 a002 8800 6a07 7c02 a102  ..t.j.....j.|...
+00001bf0: 7400 6a01 a002 8800 6a03 8800 6a04 6407  t.j.....j...j.d.
+00001c00: 7c02 a104 a102 0100 71f2 7400 a006 8800  |.......q.t.....
+00001c10: 6a09 a101 4400 5d3e 7d03 7c03 a00c 8800  j...D.]>}.|.....
+00001c20: 6a10 a101 9001 723a 740e a00f 7400 6a01  j.....r:t...t.j.
+00001c30: a002 8800 6a09 7c03 a102 7400 6a01 a002  ....j.|...t.j...
+00001c40: 8800 6a03 8800 6a04 6408 7c03 a104 a102  ..j...j.d.|.....
+00001c50: 0100 9001 713a 7400 6a01 a002 8800 6a03  ....q:t.j.....j.
+00001c60: 8800 6a04 6407 a103 8800 5f07 7400 6a01  ..j.d....._.t.j.
+00001c70: a002 8800 6a03 8800 6a04 6408 a103 8800  ....j...j.d.....
+00001c80: 5f09 6e08 7411 640b 8301 8201 640c 5300  _.n.t.d.....d.S.
+00001c90: 290d 7a3e 4372 6561 7465 2061 2070 726f  ).z>Create a pro
+00001ca0: 6a65 6374 2064 6972 6563 746f 7279 2077  ject directory w
+00001cb0: 6865 7265 2074 6f20 7361 7665 2061 6c6c  here to save all
+00001cc0: 2070 726f 6475 6365 6420 7265 7375 6c74   produced result
+00001cd0: 732e 6301 0000 0000 0000 0000 0000 0002  s.c.............
+00001ce0: 0000 0005 0000 0013 0000 0073 1c00 0000  ...........s....
+00001cf0: 6700 7c00 5d14 7d01 7c01 a000 8800 6a01  g.|.].}.|.....j.
+00001d00: a101 7204 7c01 9102 7104 5300 7227 0000  ..r.|...q.S.r'..
+00001d10: 0029 0272 5200 0000 7244 0000 0072 4a00  .).rR...rD...rJ.
+00001d20: 0000 7256 0000 0072 2700 0000 7228 0000  ..rV...r'...r(..
+00001d30: 0072 4d00 0000 d300 0000 7306 0000 0006  .rM.......s.....
+00001d40: 0202 010c fe7a 3450 726f 6a65 6374 2e73  .....z4Project.s
+00001d50: 6574 5f75 705f 7072 6f6a 6563 745f 6469  et_up_project_di
+00001d60: 7265 6374 6f72 792e 3c6c 6f63 616c 733e  rectory.<locals>
+00001d70: 2e3c 6c69 7374 636f 6d70 3e72 0100 0000  .<listcomp>r....
+00001d80: 7a3a 5468 6572 6520 6172 6520 6e6f 2063  z:There are no c
+00001d90: 6f6d 7061 7469 626c 6520 7669 6465 6f73  ompatible videos
+00001da0: 2069 6e20 7468 6520 7370 6563 6966 6965   in the specifie
+00001db0: 6420 6469 7265 6374 6f72 792e 6301 0000  d directory.c...
+00001dc0: 0000 0000 0000 0000 0002 0000 0005 0000  ................
+00001dd0: 0013 0000 0073 1c00 0000 6700 7c00 5d14  .....s....g.|.].
+00001de0: 7d01 7c01 a000 8800 6a01 a101 7204 7c01  }.|.....j...r.|.
+00001df0: 9102 7104 5300 7227 0000 0029 0272 5200  ..q.S.r'...).rR.
+00001e00: 0000 7243 0000 0072 4a00 0000 7256 0000  ..rC...rJ...rV..
+00001e10: 0072 2700 0000 7228 0000 0072 4d00 0000  .r'...r(...rM...
+00001e20: e000 0000 7306 0000 0006 0202 010c fe7a  ....s..........z
+00001e30: 3a54 6865 7265 2061 7265 206e 6f20 636f  :There are no co
+00001e40: 6d70 6174 6962 6c65 2074 7261 636b 7320  mpatible tracks 
+00001e50: 696e 2074 6865 2073 7065 6369 6669 6564  in the specified
+00001e60: 2064 6972 6563 746f 7279 2eda 0656 6964   directory...Vid
+00001e70: 656f 73da 0654 6162 6c65 7372 1b00 0000  eos..Tablesr....
+00001e80: da07 4669 6775 7265 737a 3e50 726f 6a65  ..Figuresz>Proje
+00001e90: 6374 2061 6c72 6561 6479 2065 7869 7374  ct already exist
+00001ea0: 732e 2044 656c 6574 6520 6974 206f 7220  s. Delete it or 
+00001eb0: 7370 6563 6966 7920 6120 6469 6666 6572  specify a differ
+00001ec0: 656e 7420 6e61 6d65 2e4e 2912 721e 0000  ent name.N).r...
+00001ed0: 0072 1f00 0000 7220 0000 0072 1900 0000  .r....r ...r....
+00001ee0: 723f 0000 0072 5f00 0000 725b 0000 0072  r?...r_...r[...r
+00001ef0: 4000 0000 da11 4669 6c65 4e6f 7446 6f75  @.....FileNotFou
+00001f00: 6e64 4572 726f 7272 4100 0000 da06 6578  ndErrorrA.....ex
+00001f10: 6973 7473 da08 6d61 6b65 6469 7273 7252  ists..makedirsrR
+00001f20: 0000 0072 4400 0000 da06 7368 7574 696c  ...rD.....shutil
+00001f30: da05 636f 7079 3272 4300 0000 da07 4f53  ..copy2rC.....OS
+00001f40: 4572 726f 7229 0472 5700 0000 7219 0000  Error).rW...r...
+00001f50: 0072 5400 0000 7255 0000 0072 2700 0000  .rT...rU...r'...
+00001f60: 7256 0000 0072 2800 0000 da18 7365 745f  rV...r(.....set_
+00001f70: 7570 5f70 726f 6a65 6374 5f64 6972 6563  up_project_direc
+00001f80: 746f 7279 cc00 0000 7370 0000 0000 0312  tory....sp......
+00001f90: 0302 010a 020a fe04 ff02 0702 f902 ff02  ................
+00001fa0: 0a02 0102 ff04 0402 010a 020a fe04 ff02  ................
+00001fb0: 0702 f902 ff02 0a02 0102 ff04 040e 010a  ................
+00001fc0: 011a 011a 0104 0112 ff04 031a 0310 010c  ................
+00001fd0: 0104 010e 0106 010c ff02 fe06 0710 010e  ................
+00001fe0: 0104 010e 0106 010c ff02 fe08 0806 010a  ................
+00001ff0: ff06 0306 010a ff08 0502 0102 ff7a 2050  .............z P
+00002000: 726f 6a65 6374 2e73 6574 5f75 705f 7072  roject.set_up_pr
+00002010: 6f6a 6563 745f 6469 7265 6374 6f72 7963  oject_directoryc
+00002020: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00002030: 0100 0000 4300 0000 7306 0000 007c 006a  ....C...s....|.j
+00002040: 0053 0029 017a 534c 6973 742e 2049 6620  .S.).zSList. If 
+00002050: 6e6f 7420 2761 6c6c 272c 2073 6574 7320  not 'all', sets 
+00002060: 7468 6520 626f 6479 2070 6172 7473 2061  the body parts a
+00002070: 6d6f 6e67 2077 6869 6368 2074 6865 2064  mong which the d
+00002080: 6973 7461 6e63 6573 2077 696c 6c20 6265  istances will be
+00002090: 2063 6f6d 7075 7465 642e a901 da0a 5f64   computed....._d
+000020a0: 6973 7461 6e63 6573 7256 0000 0072 2700  istancesrV...r'.
+000020b0: 0000 7227 0000 0072 2800 0000 7265 0000  ..r'...r(...re..
+000020c0: 0015 0100 0073 0200 0000 0003 7a11 5072  .....s......z.Pr
+000020d0: 6f6a 6563 742e 6469 7374 616e 6365 7363  oject.distancesc
+000020e0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+000020f0: 0100 0000 4300 0000 7306 0000 007c 006a  ....C...s....|.j
+00002100: 0053 0029 017a 6f53 7472 696e 672c 206e  .S.).zoString, n
+00002110: 616d 6520 6f66 2061 2062 6f64 7920 7061  ame of a body pa
+00002120: 7274 2e20 4966 2054 7275 652c 2063 6f6d  rt. If True, com
+00002130: 7075 7465 7320 6f6e 6c79 2074 6865 2064  putes only the d
+00002140: 6973 7461 6e63 6573 2062 6574 7765 656e  istances between
+00002150: 2074 6865 2073 7065 6369 6669 6564 2062   the specified b
+00002160: 6f64 7920 7061 7274 2061 6e64 2074 6865  ody part and the
+00002170: 2072 6573 742e a901 da04 5f65 676f 7256   rest....._egorV
+00002180: 0000 0072 2700 0000 7227 0000 0072 2800  ...r'...r'...r(.
+00002190: 0000 7266 0000 001a 0100 0073 0200 0000  ..rf.......s....
+000021a0: 0003 7a0b 5072 6f6a 6563 742e 6567 6f63  ..z.Project.egoc
+000021b0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+000021c0: 0100 0000 4300 0000 7306 0000 007c 006a  ....C...s....|.j
+000021d0: 0053 0029 017a 6742 6f6f 6c2e 2054 6f67  .S.).zgBool. Tog
+000021e0: 676c 6573 2061 6e67 6c65 2063 6f6d 7075  gles angle compu
+000021f0: 7461 7469 6f6e 2e20 5472 7565 2062 7920  tation. True by 
+00002200: 6465 6661 756c 742e 2049 6620 7475 726e  default. If turn
+00002210: 6564 206f 6666 2c20 656e 6861 6e63 6573  ed off, enhances
+00002220: 2070 6572 666f 726d 616e 6365 2066 6f72   performance for
+00002230: 2062 6967 2064 6174 6173 6574 732e a901   big datasets...
+00002240: da07 5f61 6e67 6c65 7372 5600 0000 7227  .._anglesrV...r'
+00002250: 0000 0072 2700 0000 7228 0000 0072 6200  ...r'...r(...rb.
+00002260: 0000 1f01 0000 7302 0000 0000 037a 0e50  ......s......z.P
+00002270: 726f 6a65 6374 2e61 6e67 6c65 7346 2903  roject.anglesF).
+00002280: 725e 0000 00da 0776 6572 626f 7365 721a  r^.....verboser.
+00002290: 0000 0063 0300 0000 0000 0000 0000 0000  ...c............
+000022a0: 0300 0000 0800 0000 4300 0000 732c 0000  ........C...s,..
+000022b0: 007c 0272 0c74 0064 0183 0101 0074 016a  .|.r.t.d.....t.j
+000022c0: 02a0 037c 006a 047c 006a 057c 006a 067c  ...|.j.|.j.|.j.|
+000022d0: 006a 077c 017c 006a 08a1 0653 0029 0261  .j.|.|.j...S.).a
+000022e0: 3901 0000 5265 7475 726e 2074 6865 2061  9...Return the a
+000022f0: 7265 6e61 2061 7320 7265 636f 676e 6973  rena as recognis
+00002300: 6564 2066 726f 6d20 7468 6520 7669 6465  ed from the vide
+00002310: 6f73 2e0a 0a20 2020 2020 2020 2041 7267  os...        Arg
+00002320: 733a 0a20 2020 2020 2020 2020 2020 2074  s:.            t
+00002330: 6162 6c65 7320 286c 6973 7429 3a20 6c69  ables (list): li
+00002340: 7374 206f 6620 636f 6f72 6469 6e61 7465  st of coordinate
+00002350: 2074 6162 6c65 730a 2020 2020 2020 2020   tables.        
+00002360: 2020 2020 7665 7262 6f73 6520 2862 6f6f      verbose (boo
+00002370: 6c29 3a20 6966 2054 7275 652c 206c 6f67  l): if True, log
+00002380: 7320 746f 2063 6f6e 736f 6c65 0a0a 2020  s to console..  
+00002390: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
+000023a0: 2020 2020 2020 2020 2020 2061 7265 6e61             arena
+000023b0: 2028 6e70 2e6e 6461 7272 6179 293a 2061   (np.ndarray): a
+000023c0: 7265 6e61 2070 6172 616d 6574 6572 732c  rena parameters,
+000023d0: 2061 7320 7265 636f 676e 6973 6564 2066   as recognised f
+000023e0: 726f 6d20 7468 6520 7669 6465 6f73 2e20  rom the videos. 
+000023f0: 5468 6520 7368 6170 6520 6465 7065 6e64  The shape depend
+00002400: 7320 6f6e 2074 6865 2061 7265 6e61 2074  s on the arena t
+00002410: 7970 650a 0a20 2020 2020 2020 207a 1244  ype..        z.D
+00002420: 6574 6563 7469 6e67 2061 7265 6e61 2e2e  etecting arena..
+00002430: 2e29 09da 0570 7269 6e74 da06 6465 6570  .)...print..deep
+00002440: 6f66 da05 7574 696c 73da 0a67 6574 5f61  of..utils..get_a
+00002450: 7265 6e61 7372 3500 0000 7260 0000 0072  renasr5...r`...r
+00002460: 1900 0000 723f 0000 0072 5d00 0000 2903  ....r?...r]...).
+00002470: 7257 0000 0072 5e00 0000 7280 0000 0072  rW...r^...r....r
+00002480: 2700 0000 7227 0000 0072 2800 0000 da09  '...r'...r(.....
+00002490: 6765 745f 6172 656e 6124 0100 0073 1400  get_arena$...s..
+000024a0: 0000 000b 0401 0802 0601 0401 0401 0401  ................
+000024b0: 0401 0201 04fa 7a11 5072 6f6a 6563 742e  ......z.Project.
+000024c0: 6765 745f 6172 656e 6129 0272 8000 0000  get_arena).r....
+000024d0: 721a 0000 0063 0200 0000 0000 0000 0000  r....c..........
+000024e0: 0000 0f00 0000 0900 0000 0300 0000 7396  ..............s.
+000024f0: 0400 0088 016a 0064 0176 0172 1274 0164  .....j.d.v.r.t.d
+00002500: 0283 0182 017c 0172 1e74 0264 0383 0101  .....|.r.t.d....
+00002510: 0069 007d 0288 016a 0344 005d ba89 0288  .i.}...j.D.]....
+00002520: 016a 0064 046b 0272 8474 046a 0574 066a  .j.d.k.r.t.j.t.j
+00002530: 07a0 0888 016a 0988 02a1 0274 0a64 058d  .....j.....t.d..
+00002540: 027d 037c 036a 0b6a 0c64 0664 078d 016a  .}.|.j.j.d.d...j
+00002550: 0b7d 037c 036a 0d64 0864 0964 0985 0266  .}.|.j.d.d.d...f
+00002560: 0219 007c 035f 0e7c 036a 0f64 0a64 0985  ...|._.|.j.d.d..
+00002570: 0219 007d 036e 2688 016a 0064 0b6b 0272  ...}.n&..j.d.k.r
+00002580: aa74 046a 1074 066a 07a0 0888 016a 0988  .t.j.t.j.....j..
+00002590: 02a1 0264 0c64 0664 0d8d 037d 037a 1874  ...d.d.d...}.z.t
+000025a0: 116a 126a 13a0 1464 0e88 02a1 0264 0c19  .j.j...d.....d..
+000025b0: 007d 0457 006e 1604 0074 1579 d801 0001  .}.W.n...t.y....
+000025c0: 0001 0088 027d 0459 006e 0230 007c 037c  .....}.Y.n.0.|.|
+000025d0: 027c 043c 0071 2864 0f74 167c 02a0 17a1  .|.<.q(d.t.|....
+000025e0: 0083 0164 0c19 006a 1876 0090 0172 6e74  ...d...j.v...rnt
+000025f0: 1674 167c 02a0 17a1 0083 0164 0c19 006a  .t.|.......d...j
+00002600: 0d64 0f64 0964 0985 0266 0219 00a0 19a1  .d.d.d...f......
+00002610: 0083 0188 015f 1a7c 02a0 1ba1 0044 005d  ....._.|.....D.]
+00002620: 405c 027d 0589 0288 026a 0d64 0f19 0064  @\.}.....j.d...d
+00002630: 1017 0088 026a 0d64 1119 0017 007c 027c  .....j.d.....|.|
+00002640: 0519 006a 0d64 113c 007c 027c 0519 006a  ...j.d.<.|.|...j
+00002650: 1c64 0f64 0c64 1264 138d 0301 0090 0171  .d.d.d.d.......q
+00002660: 2c7c 02a0 1ba1 0044 005d 565c 027d 0589  ,|.....D.]V\.}..
+00002670: 0288 02a0 1da1 007d 0674 046a 1ea0 1f87  .......}.t.j....
+00002680: 0266 0164 1464 1584 0874 2064 1683 0144  .f.d.d...t d...D
+00002690: 0083 01a1 017c 065f 0e7c 066a 0f64 1664  .....|._.|.j.d.d
+000026a0: 0985 0219 00a0 2174 0aa1 017d 067c 066a  ......!t...}.|.j
+000026b0: 0c64 1264 078d 017c 027c 053c 0090 0171  .d.d...|.|.<...q
+000026c0: 7687 0166 0164 1764 1884 0888 016a 1a44  v..f.d.d.....j.D
+000026d0: 0083 0189 0087 0087 0166 0264 1964 1884  .........f.d.d..
+000026e0: 0888 016a 1a44 0083 0188 015f 2274 2388  ...j.D....._"t#.
+000026f0: 016a 1a83 0164 0a6b 0490 0272 3288 016a  .j...d.k...r2..j
+00002700: 2474 2564 1a67 0183 016b 0390 0272 3287  $t%d.g...k...r2.
+00002710: 0166 0164 1b64 1584 0888 016a 1a44 0083  .f.d.d.....j.D..
+00002720: 0188 015f 2488 016a 2664 0975 0190 0272  ..._$..j&d.u...r
+00002730: 947c 02a0 1ba1 0044 005d 4c5c 027d 0589  .|.....D.]L\.}..
+00002740: 0274 046a 2764 1c74 046a 2888 026a 2964  .t.j'd.t.j(..j)d
+00002750: 0c19 0088 016a 261a 0064 1d64 1e8d 0288  .....j&..d.d....
+00002760: 026a 2964 0c19 0064 0a17 0064 1f64 208d  .j)d...d...d.d .
+00002770: 04a0 2a64 2164 2284 00a1 017c 027c 0519  ..*d!d"....|.|..
+00002780: 005f 1890 0271 4674 2b83 007d 077c 02a0  ._...qFt+..}.|..
+00002790: 1ba1 0044 005d 6c5c 027d 0589 0288 026a  ...D.]l\.}.....j
+000027a0: 2c64 2364 2464 0a64 0664 258d 047d 0888  ,d#d$d.d.d%..}..
+000027b0: 026a 2c64 2664 2464 0a64 0664 258d 047d  .j,d&d$d.d.d%..}
+000027c0: 0988 026a 2c64 2764 2464 0a64 1264 258d  ...j,d'd$d.d.d%.
+000027d0: 047d 0a74 046a 2d7c 087c 0967 0264 0a64  .}.t.j-|.|.g.d.d
+000027e0: 288d 026a 2e64 0a64 288d 017c 027c 053c  (..j.d.d(..|.|.<
+000027f0: 007c 0aa0 2f64 29a1 017c 077c 053c 0090  .|../d)..|.|.<..
+00002800: 0271 a274 307c 0764 2a88 016a 1a64 2b8d  .q.t0|.d*..j.d+.
+00002810: 037d 0788 016a 3190 0372 927c 0190 0372  .}...j1..r.|...r
+00002820: 3674 0264 2c83 0101 007c 02a0 1ba1 0044  6t.d,....|.....D
+00002830: 005d 525c 027d 0589 0288 026a 187d 0b88  .]R\.}.....j.}..
+00002840: 026a 0e7d 0c74 04a0 3274 116a 126a 3374  .j.}.t..2t.j.j3t
+00002850: 34a0 3588 02a1 0188 016a 3164 2d64 2e8d  4.5......j1d-d..
+00002860: 03a1 016a 0c64 1264 078d 017d 0d7c 0c7c  ...j.d.d...}.|.|
+00002870: 0d5f 0e7c 0b7c 0d5f 187c 0d7c 027c 053c  ._.|.|._.|.|.|.<
+00002880: 0090 0371 3e88 016a 2474 2564 1a67 0183  ...q>..j$t%d.g..
+00002890: 016b 0390 0472 087c 02a0 1ba1 0044 005d  .k...r.|.....D.]
+000028a0: 5a5c 027d 0e89 0288 026a 1c88 016a 2464  Z\.}.....j...j$d
+000028b0: 0a64 1164 2f8d 0389 0388 036a 2e64 0a64  .d.d/......j.d.d
+000028c0: 1264 138d 0201 0074 046a 1ea0 3687 0366  .d.....t.j..6..f
+000028d0: 0164 3064 1584 0874 2064 1683 0144 0083  .d0d...t d...D..
+000028e0: 01a1 0188 035f 0e88 036a 2e64 0a64 288d  ....._...j.d.d(.
+000028f0: 017c 027c 0e3c 0090 0371 ac88 016a 3790  .|.|.<...q...j7.
+00002900: 0472 587c 0190 0472 1e74 0264 3183 0101  .rX|...r.t.d1...
+00002910: 007c 02a0 1ba1 0044 005d 305c 027d 0e89  .|.....D.]0\.}..
+00002920: 0274 116a 126a 3788 027c 077c 0e19 0088  .t.j.j7..|.|....
+00002930: 016a 3864 3288 016a 3988 016a 3a64 338d  .j8d2..j9..j:d3.
+00002940: 067c 027c 0e3c 0090 0471 2688 016a 3b90  .|.|.<...q&..j;.
+00002950: 0472 7e7c 0190 0472 6e74 0264 3483 0101  .r~|...rnt.d4...
+00002960: 0074 116a 12a0 3c88 017c 027c 07a1 037d  .t.j..<..|.|...}
+00002970: 0274 116a 12a0 3d88 017c 027c 07a1 037d  .t.j..=..|.|...}
+00002980: 027c 027c 0766 0253 0029 3561 4001 0000  .|.|.f.S.)5a@...
+00002990: 4c6f 6164 2076 6964 656f 7320 616e 6420  Load videos and 
+000029a0: 7461 626c 6573 2069 6e74 6f20 6469 6374  tables into dict
+000029b0: 696f 6e61 7269 6573 2e0a 0a20 2020 2020  ionaries...     
+000029c0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+000029d0: 2020 2020 2076 6572 626f 7365 2028 626f       verbose (bo
+000029e0: 6f6c 293a 2049 6620 5472 7565 2c20 7072  ol): If True, pr
+000029f0: 696e 7473 2074 6865 2070 726f 6772 6573  ints the progres
+00002a00: 7320 6f66 2064 6174 6120 6c6f 6164 696e  s of data loadin
+00002a10: 672e 0a0a 2020 2020 2020 2020 5265 7475  g...        Retu
+00002a20: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+00002a30: 2054 7570 6c65 3a20 4120 7475 706c 6520   Tuple: A tuple 
+00002a40: 636f 6e74 6169 6e69 6e67 2074 6865 2066  containing the f
+00002a50: 6f6c 6c6f 7769 6e67 2061 2064 6963 7469  ollowing a dicti
+00002a60: 6f6e 6172 7920 7769 7468 2061 6c6c 206c  onary with all l
+00002a70: 6f61 6465 6420 7461 626c 6573 2070 6572  oaded tables per
+00002a80: 2065 7870 6572 696d 656e 742c 0a20 2020   experiment,.   
+00002a90: 2020 2020 2020 2020 2061 6e64 2061 6e6f           and ano
+00002aa0: 7468 6572 2064 6963 7469 6f6e 6172 7920  ther dictionary 
+00002ab0: 7769 7468 2044 4c43 2064 6174 6120 7175  with DLC data qu
+00002ac0: 616c 6974 792e 0a0a 2020 2020 2020 2020  ality...        
+00002ad0: 2902 724f 0000 0072 5000 0000 7a31 5472  ).rO...rP...z1Tr
+00002ae0: 6163 6b69 6e67 2066 696c 6573 206d 7573  acking files mus
+00002af0: 7420 6265 2069 6e20 6569 7468 6572 2068  t be in either h
+00002b00: 3520 6f72 2063 7376 2066 6f72 6d61 747a  5 or csv formatz
+00002b10: 174c 6f61 6469 6e67 2074 7261 6a65 6374  .Loading traject
+00002b20: 6f72 6965 732e 2e2e 724f 0000 00a9 01da  ories...rO......
+00002b30: 0564 7479 7065 4629 01da 0464 726f 70da  .dtypeF)...drop.
+00002b40: 0673 636f 7265 724e 7232 0000 0072 5000  .scorerNr2...rP.
+00002b50: 0000 7201 0000 0029 02da 0969 6e64 6578  ..r....)...index
+00002b60: 5f63 6f6c da0a 6c6f 775f 6d65 6d6f 7279  _col..low_memory
+00002b70: 7a08 282e 2a3f 2944 4c43 da0b 696e 6469  z.(.*?)DLC..indi
+00002b80: 7669 6475 616c 73da 015f da09 626f 6479  viduals.._..body
+00002b90: 7061 7274 7354 2902 da04 6178 6973 da07  partsT)...axis..
+00002ba0: 696e 706c 6163 6563 0100 0000 0000 0000  inplacec........
+00002bb0: 0000 0000 0200 0000 0400 0000 1300 0000  ................
+00002bc0: 7316 0000 0067 007c 005d 0e7d 0188 006a  s....g.|.].}...j
+00002bd0: 007c 0119 0091 0271 0453 0072 2700 0000  .|.....q.S.r'...
+00002be0: a901 da04 696c 6f63 724a 0000 0029 0172  ....ilocrJ...).r
+00002bf0: 5500 0000 7227 0000 0072 2800 0000 724d  U...r'...r(...rM
+00002c00: 0000 007e 0100 0072 4e00 0000 7a27 5072  ...~...rN...z'Pr
+00002c10: 6f6a 6563 742e 6c6f 6164 5f74 6162 6c65  oject.load_table
+00002c20: 732e 3c6c 6f63 616c 733e 2e3c 6c69 7374  s.<locals>.<list
+00002c30: 636f 6d70 3ee9 0200 0000 6301 0000 0000  comp>.....c.....
+00002c40: 0000 0000 0000 0002 0000 0008 0000 0013  ................
+00002c50: 0000 0073 2a00 0000 6900 7c00 5d22 7d01  ...s*...i.|.]"}.
+00002c60: 6400 a000 7c01 a101 7401 6a02 6a03 7c01  d...|...t.j.j.|.
+00002c70: 8800 6a04 8800 6a05 6401 8d03 9302 7104  ..j...j.d.....q.
+00002c80: 5300 2902 7a0f 7b7d 6d6f 7573 655f 746f  S.).z.{}mouse_to
+00002c90: 7076 6965 7729 0272 3800 0000 da0c 6772  pview).r8.....gr
+00002ca0: 6170 685f 7072 6573 6574 2906 726d 0000  aph_preset).rm..
+00002cb0: 0072 8200 0000 7283 0000 00da 0d63 6f6e  .r....r......con
+00002cc0: 6e65 6374 5f6d 6f75 7365 7238 0000 0072  nect_mouser8...r
+00002cd0: 3600 0000 a902 724b 0000 00da 0361 6964  6.....rK.....aid
+00002ce0: 7256 0000 0072 2700 0000 7228 0000 00da  rV...r'...r(....
+00002cf0: 0a3c 6469 6374 636f 6d70 3e84 0100 0073  .<dictcomp>....s
+00002d00: 0c00 0000 0606 02fb 0e01 0201 0401 04fd  ................
+00002d10: 7a27 5072 6f6a 6563 742e 6c6f 6164 5f74  z'Project.load_t
+00002d20: 6162 6c65 732e 3c6c 6f63 616c 733e 2e3c  ables.<locals>.<
+00002d30: 6469 6374 636f 6d70 3e63 0100 0000 0000  dictcomp>c......
+00002d40: 0000 0000 0000 0200 0000 0600 0000 1300  ................
+00002d50: 0000 731c 0000 0069 007c 005d 147d 017c  ..s....i.|.].}.|
+00002d60: 0188 007c 0188 016a 0017 0019 0093 0271  ...|...j.......q
+00002d70: 0453 0072 2700 0000 2901 723e 0000 0072  .S.r'...).r>...r
+00002d80: 9600 0000 2902 da0a 6d6f 6465 6c5f 6469  ....)...model_di
+00002d90: 6374 7257 0000 0072 2700 0000 7228 0000  ctrW...r'...r(..
+00002da0: 0072 9800 0000 8c01 0000 7302 0000 0006  .r........s.....
+00002db0: 0172 2d00 0000 6301 0000 0000 0000 0000  .r-...c.........
+00002dc0: 0000 0003 0000 0005 0000 0013 0000 0073  ...............s
+00002dd0: 2400 0000 6700 7c00 5d1c 7d01 8800 6a00  $...g.|.].}...j.
+00002de0: 4400 5d10 7d02 7c01 6400 1700 7c02 1700  D.].}.|.d...|...
+00002df0: 9103 710e 7104 5300 a901 728d 0000 0029  ..q.q.S...r....)
+00002e00: 0172 3800 0000 2903 724b 0000 0072 9700  .r8...).rK...r..
+00002e10: 0000 da02 6270 7256 0000 0072 2700 0000  ....bprV...r'...
+00002e20: 7228 0000 0072 4d00 0000 9201 0000 7306  r(...rM.......s.
+00002e30: 0000 0006 0202 010a fe7a 0830 303a 3030  .........z.00:00
+00002e40: 3a30 30da 0373 6563 2901 da04 756e 6974  :00..sec)...unit
+00002e50: da04 6c65 6674 2902 da07 7065 7269 6f64  ..left)...period
+00002e60: 73da 0663 6c6f 7365 6463 0100 0000 0000  s..closedc......
+00002e70: 0000 0000 0000 0100 0000 0300 0000 5300  ..............S.
+00002e80: 0000 7310 0000 0074 007c 0083 0164 0164  ..s....t.|...d.d
+00002e90: 0085 0219 0053 0029 024e e907 0000 00a9  .....S.).N......
+00002ea0: 01da 0373 7472 2901 da01 7472 2700 0000  ...str)...tr'...
+00002eb0: 7227 0000 0072 2800 0000 da08 3c6c 616d  r'...r(.....<lam
+00002ec0: 6264 613e a001 0000 724e 0000 007a 2550  bda>....rN...z%P
+00002ed0: 726f 6a65 6374 2e6c 6f61 645f 7461 626c  roject.load_tabl
+00002ee0: 6573 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d  es.<locals>.<lam
+00002ef0: 6264 613e da01 78da 0663 6f6f 7264 7329  bda>..x..coords)
+00002f00: 03da 056c 6576 656c 728f 0000 00da 0a64  ...levelr......d
+00002f10: 726f 705f 6c65 7665 6cda 0179 da0a 6c69  rop_level..y..li
+00002f20: 6b65 6c69 686f 6f64 a901 728f 0000 00e7  kelihood..r.....
+00002f30: 0000 0000 0000 0000 da07 7175 616c 6974  ..........qualit
+00002f40: 79a9 02da 0374 7970 7234 0000 007a 1953  y....typr4...z.S
+00002f50: 6d6f 6f74 6869 6e67 2074 7261 6a65 6374  moothing traject
+00002f60: 6f72 6965 732e 2e2e e90f 0000 0029 02da  ories........)..
+00002f70: 0561 6c70 6861 da08 775f 6c65 6e67 7468  .alpha..w_length
+00002f80: 2902 728f 0000 0072 a800 0000 6301 0000  ).r....r....c...
+00002f90: 0000 0000 0000 0000 0001 0000 0008 0000  ................
+00002fa0: 0013 0000 0073 2c00 0000 6700 7c00 5d24  .....s,...g.|.]$
+00002fb0: 8900 7400 7401 7402 8700 6601 6400 6401  ..t.t.t...f.d.d.
+00002fc0: 8408 8801 6a03 4400 8301 8301 8301 8301  ....j.D.........
+00002fd0: 9102 7104 5300 2902 6301 0000 0000 0000  ..q.S.).c.......
+00002fe0: 0000 0000 0002 0000 0004 0000 0013 0000  ................
+00002ff0: 0073 1400 0000 6700 7c00 5d0c 7d01 7c01  .s....g.|.].}.|.
+00003000: 8800 1900 9102 7104 5300 7227 0000 0072  ......q.S.r'...r
+00003010: 2700 0000 724a 0000 00a9 01da 016a 7227  '...rJ.......jr'
+00003020: 0000 0072 2800 0000 724d 0000 00c5 0100  ...r(...rM......
+00003030: 0072 4e00 0000 7a32 5072 6f6a 6563 742e  .rN...z2Project.
+00003040: 6c6f 6164 5f74 6162 6c65 732e 3c6c 6f63  load_tables.<loc
+00003050: 616c 733e 2e3c 6c69 7374 636f 6d70 3e2e  als>.<listcomp>.
+00003060: 3c6c 6973 7463 6f6d 703e 2904 725c 0000  <listcomp>).r\..
+00003070: 00da 046c 6973 74da 0373 6574 da07 636f  ...list..set..co
+00003080: 6c75 6d6e 7329 0172 4b00 0000 2901 da04  lumns).rK...)...
+00003090: 7465 6d70 72b4 0000 0072 2800 0000 724d  tempr....r(...rM
+000030a0: 0000 00c5 0100 0072 4e00 0000 7a19 496e  .......rN...z.In
+000030b0: 7465 7270 6f6c 6174 696e 6720 6f75 746c  terpolating outl
+000030c0: 6965 7273 2e2e 2eda 026f 7229 0472 6700  iers.....or).rg.
+000030d0: 0000 da04 6d6f 6465 da05 6c69 6d69 74da  ....mode..limit.
+000030e0: 056e 5f73 7464 7a2c 4974 6572 6174 6976  .n_stdz,Iterativ
+000030f0: 6520 696d 7075 7461 7469 6f6e 206f 6620  e imputation of 
+00003100: 6f63 6c75 6465 6420 626f 6479 7061 7274  ocluded bodypart
+00003110: 732e 2e2e 293e 7243 0000 00da 134e 6f74  s...)>rC.....Not
+00003120: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
+00003130: 7281 0000 0072 5e00 0000 da02 7064 da08  r....r^.....pd..
+00003140: 7265 6164 5f68 6466 721e 0000 0072 1f00  read_hdfr....r..
+00003150: 0000 7220 0000 0072 4100 0000 da05 666c  ..r ...rA.....fl
+00003160: 6f61 74da 0154 da0b 7265 7365 745f 696e  oat..T..reset_in
+00003170: 6465 78da 036c 6f63 72b8 0000 0072 9200  dex..locr....r..
+00003180: 0000 da08 7265 6164 5f63 7376 7282 0000  ....read_csvr...
+00003190: 0072 8300 0000 da02 7265 da07 6669 6e64  .r......re..find
+000031a0: 616c 6cda 0a49 6e64 6578 4572 726f 7272  all..IndexErrorr
+000031b0: b600 0000 da06 7661 6c75 6573 da05 696e  ......values..in
+000031c0: 6465 78da 0675 6e69 7175 6572 3400 0000  dex..uniquer4...
+000031d0: da05 6974 656d 7372 8800 0000 da04 636f  ..itemsr......co
+000031e0: 7079 da0a 4d75 6c74 6949 6e64 6578 da0b  py..MultiIndex..
+000031f0: 6672 6f6d 5f61 7272 6179 73da 0572 616e  from_arrays..ran
+00003200: 6765 da06 6173 7479 7065 7264 0000 0072  ge..astyperd...r
+00003210: 5f00 0000 7238 0000 00da 0574 7570 6c65  _...r8.....tuple
+00003220: 7268 0000 00da 0f74 696d 6564 656c 7461  rh.....timedelta
+00003230: 5f72 616e 6765 da0c 746f 5f74 696d 6564  _range..to_timed
+00003240: 656c 7461 da05 7368 6170 65da 036d 6170  elta..shape..map
+00003250: 7202 0000 00da 0278 73da 0663 6f6e 6361  r......xs..conca
+00003260: 74da 0a73 6f72 745f 696e 6465 78da 0666  t..sort_index..f
+00003270: 696c 6c6e 61da 0954 6162 6c65 4469 6374  illna..TableDict
+00003280: 7242 0000 00da 0944 6174 6146 7261 6d65  rB.....DataFrame
+00003290: da16 736d 6f6f 7468 5f6d 756c 745f 7472  ..smooth_mult_tr
+000032a0: 616a 6563 746f 7279 da02 6e70 da05 6172  ajectory..np..ar
+000032b0: 7261 79da 0c66 726f 6d5f 7072 6f64 7563  ray..from_produc
+000032c0: 7472 3a00 0000 7267 0000 0072 3b00 0000  tr:...rg...r;...
+000032d0: 723c 0000 0072 3700 0000 da14 6974 6572  r<...r7.....iter
+000032e0: 6174 6976 655f 696d 7075 7461 7469 6f6e  ative_imputation
+000032f0: da13 7365 745f 6d69 7373 696e 675f 616e  ..set_missing_an
+00003300: 696d 616c 7329 0f72 5700 0000 7280 0000  imals).rW...r...
+00003310: 00da 0874 6162 5f64 6963 74da 0a6c 6f61  ...tab_dict..loa
+00003320: 6465 645f 7461 62da 0874 6162 5f6e 616d  ded_tab..tab_nam
+00003330: 65da 036b 6579 da08 7461 625f 636f 7079  e..key..tab_copy
+00003340: da08 6c69 6b5f 6469 6374 72a6 0000 0072  ..lik_dictr....r
+00003350: aa00 0000 da03 6c69 6bda 0763 7572 5f69  ......lik..cur_i
+00003360: 6478 da08 6375 725f 636f 6c73 da06 736d  dx..cur_cols..sm
+00003370: 6f6f 7468 da01 6b72 2700 0000 2904 7299  ooth..kr'...).r.
+00003380: 0000 0072 5700 0000 7255 0000 0072 b900  ...rW...rU...r..
+00003390: 0000 7228 0000 00da 0b6c 6f61 645f 7461  ..r(.....load_ta
+000033a0: 626c 6573 3b01 0000 73de 0000 0000 0b0a  bles;...s.......
+000033b0: 0102 0102 ff04 0404 0108 0204 010a 020a  ................
+000033c0: 0204 0110 ff06 0510 0114 0110 020a 0204  ................
+000033d0: 010e 0102 0102 fd06 0702 0118 010c 010a  ................
+000033e0: 020a 0318 0102 0120 ff06 0410 0316 ff0c  ....... ........
+000033f0: 0318 0310 0108 0206 0114 ff06 0314 0114  ................
+00003400: 030a 0604 fa06 080c 0104 ff08 0522 010a  ............."..
+00003410: 0204 fe08 070c 0110 0104 0102 0118 010c  ................
+00003420: 0102 fc06 0506 fb0e 0706 0210 0112 0112  ................
+00003430: 0112 021e 0112 0210 0208 0206 0108 0210  ................
+00003440: 0106 0106 0104 0106 010e ff04 ff04 0402  ................
+00003450: fc06 0506 0106 010c 0212 0210 0112 010e  ................
+00003460: 0106 0114 ff06 0314 0208 0206 0108 0210  ................
+00003470: 0106 0102 0106 0104 0102 0104 0104 fa0e  ................
+00003480: 0908 0206 0108 0210 0310 027a 1350 726f  ...........z.Pro
+00003490: 6a65 6374 2e6c 6f61 645f 7461 626c 6573  ject.load_tables
+000034a0: 2903 72e3 0000 0072 8000 0000 721a 0000  ).r....r....r...
+000034b0: 0063 0300 0000 0000 0000 0000 0000 0600  .c..............
+000034c0: 0000 0600 0000 0300 0000 731e 0100 007c  ..........s....|
+000034d0: 0272 0c74 0064 0183 0101 0088 026a 0189  .r.t.d.......j..
+000034e0: 0088 0064 026b 0272 3688 0374 0288 03a0  ...d.k.r6..t....
+000034f0: 03a1 0083 0164 0319 0019 006a 046a 0564  .....d.....j.j.d
+00003500: 0319 0089 0087 0366 0164 0464 0584 0888  .......f.d.d....
+00003510: 0044 0083 0173 504a 0064 0683 0182 0188  .D...sPJ.d......
+00003520: 026a 0664 0764 0785 0264 0864 0785 0266  .j.d.d...d.d...f
+00003530: 0219 0089 0187 0166 0164 0964 0a84 0874  .......f.d.d...t
+00003540: 0788 03a0 08a1 0083 0144 0083 017d 037c  .........D...}.|
+00003550: 03a0 03a1 0044 005d 327d 047c 037c 0419  .....D.]2}.|.|..
+00003560: 006a 0964 0764 0785 0287 0066 0164 0b64  .j.d.d.....f.d.d
+00003570: 0584 087c 037c 0419 006a 0444 0083 0166  ...|.|...j.D...f
+00003580: 0219 007c 037c 043c 0071 8888 026a 0a72  ...|.|.<.q...j.r
+00003590: fa7c 03a0 08a1 0044 005d 2e5c 027d 047d  .|.....D.].\.}.}
+000035a0: 057c 056a 0964 0764 0785 0287 0266 0164  .|.j.d.d.....f.d
+000035b0: 0c64 0584 087c 056a 0444 0083 0166 0219  .d...|.j.D...f..
+000035c0: 007c 037c 043c 0071 ca7c 03a0 03a1 0044  .|.|.<.q.|.....D
+000035d0: 005d 167d 0488 037c 0419 006a 0b7c 037c  .].}...|...j.|.|
+000035e0: 0419 005f 0b90 0171 027c 0353 0029 0d61  ..._...q.|.S.).a
+000035f0: c701 0000 436f 6d70 7574 6520 7468 6520  ....Compute the 
+00003600: 6469 7374 616e 6365 7320 6265 7477 6565  distances betwee
+00003610: 6e20 616c 6c20 7365 6c65 6374 6564 2062  n all selected b
+00003620: 6f64 7920 7061 7274 7320 6f76 6572 2074  ody parts over t
+00003630: 696d 652e 2049 6620 6567 6f20 6973 2070  ime. If ego is p
+00003640: 726f 7669 6465 642c 2069 7420 6f6e 6c79  rovided, it only
+00003650: 2072 6574 7572 6e73 2064 6973 7461 6e63   returns distanc
+00003660: 6573 2074 6f20 6120 7370 6563 6966 6965  es to a specifie
+00003670: 6420 626f 6479 7061 7274 2e0a 0a20 2020  d bodypart...   
+00003680: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+00003690: 2020 2020 2020 2074 6162 5f64 6963 7420         tab_dict 
+000036a0: 2864 6963 7429 3a20 4469 6374 696f 6e61  (dict): Dictiona
+000036b0: 7279 206f 6620 7061 6e64 6173 2044 6174  ry of pandas Dat
+000036c0: 6146 7261 6d65 7320 636f 6e74 6169 6e69  aFrames containi
+000036d0: 6e67 2074 6865 2074 7261 6a65 6374 6f72  ng the trajector
+000036e0: 6965 7320 6f66 2061 6c6c 2062 6f64 7970  ies of all bodyp
+000036f0: 6172 7473 2e0a 2020 2020 2020 2020 2020  arts..          
+00003700: 2020 7665 7262 6f73 6520 2862 6f6f 6c29    verbose (bool)
+00003710: 3a20 4966 2054 7275 652c 2070 7269 6e74  : If True, print
+00003720: 7320 7072 6f67 7265 7373 2e20 4465 6661  s progress. Defa
+00003730: 756c 7473 2074 6f20 5472 7565 2e0a 0a20  ults to True... 
+00003740: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
+00003750: 2020 2020 2020 2020 2020 2020 6469 6374              dict
+00003760: 3a20 4469 6374 696f 6e61 7279 206f 6620  : Dictionary of 
+00003770: 7061 6e64 6173 2044 6174 6146 7261 6d65  pandas DataFrame
+00003780: 7320 636f 6e74 6169 6e69 6e67 2074 6865  s containing the
+00003790: 2064 6973 7461 6e63 6573 2062 6574 7765   distances betwe
+000037a0: 656e 2061 6c6c 2062 6f64 7970 6172 7473  en all bodyparts
+000037b0: 2e0a 0a20 2020 2020 2020 207a 1643 6f6d  ...        z.Com
+000037c0: 7075 7469 6e67 2064 6973 7461 6e63 6573  puting distances
+000037d0: 2e2e 2e72 5800 0000 7201 0000 0063 0100  ...rX...r....c..
+000037e0: 0000 0000 0000 0000 0000 0200 0000 0600  ................
+000037f0: 0000 1300 0000 7328 0000 0067 007c 005d  ......s(...g.|.]
+00003800: 207d 017c 0174 0088 00a0 01a1 0083 0164   }.|.t.........d
+00003810: 0019 006a 026a 0364 0019 0076 0091 0271  ...j.j.d...v...q
+00003820: 0453 00a9 0172 0100 0000 2904 72b6 0000  .S...r....).r...
+00003830: 0072 c900 0000 72b8 0000 00da 066c 6576  .r....r......lev
+00003840: 656c 7372 4a00 0000 2901 72e3 0000 0072  elsrJ...).r....r
+00003850: 2700 0000 7228 0000 0072 4d00 0000 f601  '...r(...rM.....
+00003860: 0000 7302 0000 0006 017a 2950 726f 6a65  ..s......z)Proje
+00003870: 6374 2e67 6574 5f64 6973 7461 6e63 6573  ct.get_distances
+00003880: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
+00003890: 6f6d 703e 7a2d 4e6f 6465 7320 7368 6f75  omp>z-Nodes shou
+000038a0: 6c64 2063 6f72 7265 7370 6f6e 6420 746f  ld correspond to
+000038b0: 2065 7869 7374 656e 7420 626f 6479 7061   existent bodypa
+000038c0: 7274 734e 7293 0000 0063 0100 0000 0000  rtsNr....c......
+000038d0: 0000 0000 0000 0400 0000 0a00 0000 1300  ................
+000038e0: 0000 7336 0000 0069 007c 005d 2e5c 027d  ..s6...i.|.].\.}
+000038f0: 015c 027d 027d 037c 0274 006a 01a0 027c  .\.}.}.|.t.j...|
+00003900: 0388 007c 0164 0066 0219 0088 007c 0164  ...|.d.f.....|.d
+00003910: 0166 0219 00a1 0393 0271 0453 0029 0272  .f.......q.S.).r
+00003920: 3200 0000 7201 0000 0029 0372 8200 0000  2...r....).r....
+00003930: 7283 0000 00da 0e62 7061 7274 5f64 6973  r......bpart_dis
+00003940: 7461 6e63 6529 0472 4b00 0000 724c 0000  tance).rK...rL..
+00003950: 0072 e600 0000 7255 0000 0029 01da 0673  .r....rU...)...s
+00003960: 6361 6c65 7372 2700 0000 7228 0000 0072  calesr'...r(...r
+00003970: 9800 0000 fc01 0000 7304 0000 0006 020a  ........s.......
+00003980: ff7a 2950 726f 6a65 6374 2e67 6574 5f64  .z)Project.get_d
+00003990: 6973 7461 6e63 6573 2e3c 6c6f 6361 6c73  istances.<locals
+000039a0: 3e2e 3c64 6963 7463 6f6d 703e 6301 0000  >.<dictcomp>c...
+000039b0: 0000 0000 0000 0000 0002 0000 0007 0000  ................
+000039c0: 0013 0000 0073 2400 0000 6700 7c00 5d1c  .....s$...g.|.].
+000039d0: 7d01 7400 a001 8700 6601 6400 6401 8408  }.t.....f.d.d...
+000039e0: 7c01 4400 8301 a101 9102 7104 5300 2902  |.D.......q.S.).
+000039f0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00003a00: 0004 0000 0013 0000 0073 1400 0000 6700  .........s....g.
+00003a10: 7c00 5d0c 7d01 7c01 8800 7600 9102 7104  |.].}.|...v...q.
+00003a20: 5300 7227 0000 0072 2700 0000 724a 0000  S.r'...r'...rJ..
+00003a30: 00a9 01da 056e 6f64 6573 7227 0000 0072  .....nodesr'...r
+00003a40: 2800 0000 724d 0000 0003 0200 0072 4e00  (...rM.......rN.
+00003a50: 0000 7a34 5072 6f6a 6563 742e 6765 745f  ..z4Project.get_
+00003a60: 6469 7374 616e 6365 732e 3c6c 6f63 616c  distances.<local
+00003a70: 733e 2e3c 6c69 7374 636f 6d70 3e2e 3c6c  s>.<listcomp>.<l
+00003a80: 6973 7463 6f6d 703e 2902 72de 0000 0072  istcomp>).r....r
+00003a90: 5800 0000 2902 724b 0000 0072 b500 0000  X...).rK...r....
+00003aa0: 72f3 0000 0072 2700 0000 7228 0000 0072  r....r'...r(...r
+00003ab0: 4d00 0000 0302 0000 724e 0000 0063 0100  M.......rN...c..
+00003ac0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+00003ad0: 0000 1300 0000 731a 0000 0067 007c 005d  ......s....g.|.]
+00003ae0: 127d 0188 006a 007c 0176 0072 047c 0191  .}...j.|.v.r.|..
+00003af0: 0271 0453 0072 2700 0000 2901 7266 0000  .q.S.r'...).rf..
+00003b00: 0029 0272 4b00 0000 da04 6469 7374 7256  .).rK.....distrV
+00003b10: 0000 0072 2700 0000 7228 0000 0072 4d00  ...r'...r(...rM.
+00003b20: 0000 0902 0000 724e 0000 0029 0c72 8100  ......rN...).r..
+00003b30: 0000 7265 0000 0072 b600 0000 da04 6b65  ..re...r......ke
+00003b40: 7973 72b8 0000 0072 f000 0000 72f2 0000  ysr....r....r...
+00003b50: 00da 0965 6e75 6d65 7261 7465 72cc 0000  ...enumerater...
+00003b60: 0072 c400 0000 7266 0000 0072 ca00 0000  .r....rf...r....
+00003b70: 2906 7257 0000 0072 e300 0000 7280 0000  ).rW...r....r...
+00003b80: 00da 0d64 6973 7461 6e63 655f 6469 6374  ...distance_dict
+00003b90: 72e6 0000 00da 0376 616c 7227 0000 0029  r......valr'...)
+00003ba0: 0472 f400 0000 72f2 0000 0072 5700 0000  .r....r....rW...
+00003bb0: 72e3 0000 0072 2800 0000 da0d 6765 745f  r....r(.....get_
+00003bc0: 6469 7374 616e 6365 73e4 0100 0073 3400  distances....s4.
+00003bd0: 0000 000b 0401 0802 0601 0801 1c02 0a01  ................
+00003be0: 02ff 0802 02fe 0404 1602 0a02 0afe 0605  ................
+00003bf0: 0c01 0801 1eff 0a04 0601 1001 0401 1aff  ................
+00003c00: 0a05 0c01 1402 7a15 5072 6f6a 6563 742e  ......z.Project.
+00003c10: 6765 745f 6469 7374 616e 6365 7363 0300  get_distancesc..
+00003c20: 0000 0000 0000 0000 0000 0b00 0000 0b00  ................
+00003c30: 0000 4300 0000 7302 0100 007c 0272 0c74  ..C...s....|.r.t
+00003c40: 0064 0183 0101 0067 007d 037c 006a 0144  .d.....g.}.|.j.D
+00003c50: 005d 1a7d 047c 0374 026a 03a0 047c 006a  .].}.|.t.j...|.j
+00003c60: 057c 0419 00a1 0137 007d 0371 1664 0264  .|.....7.}.q.d.d
+00003c70: 0384 007c 0344 0083 017d 0369 007d 057a  ...|.D...}.i.}.z
+00003c80: 807c 01a0 06a1 0044 005d 725c 027d 067d  .|.....D.]r\.}.}
+00003c90: 0767 007d 087c 0344 005d 4a7d 0974 07a0  .g.}.|.D.]J}.t..
+00003ca0: 0874 026a 03a0 0974 0aa0 0b7c 077c 0919  .t.j...t...|.|..
+00003cb0: 00a1 01a0 0c64 047c 076a 0d64 0519 0064  .....d.|.j.d...d
+00003cc0: 0667 03a1 01a1 016a 0ea1 017d 0a74 0f7c  .g.....j...}.t.|
+00003cd0: 0983 0167 017c 0a5f 107c 08a0 117c 0aa1  ...g.|._.|...|..
+00003ce0: 0101 0071 5e74 076a 127c 0864 0764 088d  ...q^t.j.|.d.d..
+00003cf0: 027d 087c 087c 057c 063c 0071 4e57 006e  .}.|.|.|.<.qNW.n
+00003d00: 1a04 0074 1379 de01 0001 0001 0074 1364  ...t.y.......t.d
+00003d10: 0983 0182 0159 006e 0230 007c 05a0 14a1  .....Y.n.0.|....
+00003d20: 0044 005d 147d 067c 017c 0619 006a 157c  .D.].}.|.|...j.|
+00003d30: 057c 0619 005f 1571 e87c 0553 0029 0a61  .|..._.q.|.S.).a
+00003d40: 9b01 0000 436f 6d70 7574 6520 616c 6c20  ....Compute all 
+00003d50: 7468 6520 616e 676c 6573 2062 6574 7765  the angles betwe
+00003d60: 656e 2061 646a 6163 656e 7420 626f 6479  en adjacent body
+00003d70: 7061 7274 2074 7269 6f73 2070 6572 2076  part trios per v
+00003d80: 6964 656f 2061 6e64 2070 6572 2066 7261  ideo and per fra
+00003d90: 6d65 2069 6e20 7468 6520 6461 7461 2e0a  me in the data..
+00003da0: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
+00003db0: 2020 2020 2020 2020 2020 2074 6162 5f64             tab_d
+00003dc0: 6963 7420 2864 6963 7429 3a20 4469 6374  ict (dict): Dict
+00003dd0: 696f 6e61 7279 206f 6620 7061 6e64 6173  ionary of pandas
+00003de0: 2044 6174 6146 7261 6d65 7320 636f 6e74   DataFrames cont
+00003df0: 6169 6e69 6e67 2074 6865 2074 7261 6a65  aining the traje
+00003e00: 6374 6f72 6965 7320 6f66 2061 6c6c 2062  ctories of all b
+00003e10: 6f64 7970 6172 7473 2e0a 2020 2020 2020  odyparts..      
+00003e20: 2020 2020 2020 7665 7262 6f73 6520 2862        verbose (b
+00003e30: 6f6f 6c29 3a20 4966 2054 7275 652c 2070  ool): If True, p
+00003e40: 7269 6e74 7320 7072 6f67 7265 7373 2e20  rints progress. 
+00003e50: 4465 6661 756c 7473 2074 6f20 5472 7565  Defaults to True
+00003e60: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+00003e70: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+00003e80: 6469 6374 3a20 4469 6374 696f 6e61 7279  dict: Dictionary
+00003e90: 206f 6620 7061 6e64 6173 2044 6174 6146   of pandas DataF
+00003ea0: 7261 6d65 7320 636f 6e74 6169 6e69 6e67  rames containing
+00003eb0: 2074 6865 2064 6973 7461 6e63 6573 2062   the distances b
+00003ec0: 6574 7765 656e 2061 6c6c 2062 6f64 7970  etween all bodyp
+00003ed0: 6172 7473 2e0a 0a20 2020 2020 2020 207a  arts...        z
+00003ee0: 1343 6f6d 7075 7469 6e67 2061 6e67 6c65  .Computing angle
+00003ef0: 732e 2e2e 6301 0000 0000 0000 0000 0000  s...c...........
+00003f00: 0002 0000 0004 0000 0053 0000 0073 1c00  .........S...s..
+00003f10: 0000 6700 7c00 5d14 7d01 7400 7c01 8301  ..g.|.].}.t.|...
+00003f20: 6400 6b02 7204 7c01 9102 7104 5300 2901  d.k.r.|...q.S.).
+00003f30: 722f 0000 0029 0172 5f00 0000 724a 0000  r/...).r_...rJ..
+00003f40: 0072 2700 0000 7227 0000 0072 2800 0000  .r'...r'...r(...
+00003f50: 724d 0000 0024 0200 0072 4e00 0000 7a26  rM...$...rN...z&
+00003f60: 5072 6f6a 6563 742e 6765 745f 616e 676c  Project.get_angl
+00003f70: 6573 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  es.<locals>.<lis
+00003f80: 7463 6f6d 703e 722f 0000 0072 0100 0000  tcomp>r/...r....
+00003f90: 7293 0000 0072 3200 0000 72ac 0000 007a  r....r2...r....z
+00003fa0: d141 7265 2079 6f75 2075 7369 6e67 2061  .Are you using a
+00003fb0: 2063 7573 746f 6d20 6c61 6265 6c6c 696e   custom labellin
+00003fc0: 6720 7363 6865 6d65 3f20 4f75 7420 7475  g scheme? Out tu
+00003fd0: 746f 7269 616c 7320 6d61 7920 6865 6c70  torials may help
+00003fe0: 2120 496e 2063 6173 6520 796f 7527 7265  ! In case you're
+00003ff0: 206e 6f74 2c20 6172 6520 7468 6572 6520   not, are there 
+00004000: 6d75 6c74 6970 6c65 2061 6e69 6d61 6c73  multiple animals
+00004010: 2069 6e20 796f 7572 2073 696e 676c 652d   in your single-
+00004020: 616e 696d 616c 2044 4c43 2076 6964 656f  animal DLC video
+00004030: 3f20 4d61 6b65 2073 7572 6520 746f 2073  ? Make sure to s
+00004040: 6574 2074 6865 2061 6e69 6d61 6c5f 6964  et the animal_id
+00004050: 7320 7061 7261 6d65 7465 7220 696e 2064  s parameter in d
+00004060: 6565 706f 662e 6461 7461 2e50 726f 6a65  eepof.data.Proje
+00004070: 6374 2916 7281 0000 0072 3400 0000 7282  ct).r....r4...r.
+00004080: 0000 0072 8300 0000 da15 656e 756d 6572  ...r......enumer
+00004090: 6174 655f 616c 6c5f 6272 6964 6765 7372  ate_all_bridgesr
+000040a0: 6400 0000 72cc 0000 0072 bf00 0000 72dc  d...r....r....r.
+000040b0: 0000 00da 0561 6e67 6c65 72de 0000 0072  .....angler....r
+000040c0: df00 0000 da07 7265 7368 6170 6572 d500  ......reshaper..
+000040d0: 0000 72c2 0000 0072 d200 0000 72b8 0000  ..r....r....r...
+000040e0: 00da 0661 7070 656e 6472 d800 0000 da08  ...appendr......
+000040f0: 4b65 7945 7272 6f72 72f6 0000 0072 ca00  KeyErrorr....r..
+00004100: 0000 290b 7257 0000 0072 e300 0000 7280  ..).rW...r....r.
+00004110: 0000 00da 0762 7269 6467 6573 724c 0000  .....bridgesrL..
+00004120: 00da 0a61 6e67 6c65 5f64 6963 7472 e600  ...angle_dictr..
+00004130: 0000 7255 0000 00da 0464 6174 73da 0663  ..rU.....dats..c
+00004140: 6c69 7175 65da 0364 6174 7227 0000 0072  lique..datr'...r
+00004150: 2700 0000 7228 0000 00da 0a67 6574 5f61  '...r(.....get_a
+00004160: 6e67 6c65 7312 0200 0073 3600 0000 000b  ngles....s6.....
+00004170: 0401 0803 0401 0a01 1801 0e02 0401 0201  ................
+00004180: 1002 0401 0801 0401 0601 1eff 04ff 0406  ................
+00004190: 0c01 0c02 0e02 0e01 0c01 0201 02ff 0a07  ................
+000041a0: 0c01 1202 7a12 5072 6f6a 6563 742e 6765  ....z.Project.ge
+000041b0: 745f 616e 676c 6573 6303 0000 0000 0000  t_anglesc.......
+000041c0: 0000 0000 0008 0000 0009 0000 0003 0000  ................
+000041d0: 0073 f800 0000 7c02 720c 7400 6401 8301  .s....|.r.t.d...
+000041e0: 0100 6900 7d03 7ac4 7c01 a001 a100 4400  ..i.}.z.|.....D.
+000041f0: 5db6 5c02 7d04 7d05 7402 a003 a100 7d06  ].\.}.}.t.....}.
+00004200: 7c00 6a04 4400 5d96 8900 8800 6402 6b02  |.j.D.].....d.k.
+00004210: 7240 6403 8900 7c05 6a05 6403 6403 8502  r@d...|.j.d.d...
+00004220: 7406 6a07 a008 7c05 6a09 8800 a102 6602  t.j...|.j.....f.
+00004230: 1900 7d07 7c07 6a0a 8700 6601 6404 6405  ..}.|.j...f.d.d.
+00004240: 8408 6406 6407 8d02 7d07 7402 6a03 7c07  ..d.d...}.t.j.|.
+00004250: a00b a100 7c07 6a0c 6700 6408 a201 6409  ....|.j.g.d...d.
+00004260: 8d03 a00d 640a a00e 8800 6403 7501 729e  ....d.....d.u.r.
+00004270: 8800 6e02 6402 8800 6403 7501 72ac 640b  ..n.d...d.u.r.d.
+00004280: 6e02 6402 a102 a101 7d07 7402 6a0f 7c06  n.d.....}.t.j.|.
+00004290: 7c07 6702 6406 6407 8d02 7d06 7130 7c06  |.g.d.d...}.q0|.
+000042a0: 7c03 7c04 3c00 711a 5700 6e1e 0400 7410  |.|.<.q.W.n...t.
+000042b0: 79f2 0100 0100 0100 7411 a012 640c a101  y.......t...d...
+000042c0: 0100 5900 6403 5300 3000 7c03 5300 290d  ..Y.d.S.0.|.S.).
+000042d0: 6193 0100 0043 6f6d 7075 7465 2061 6c6c  a....Compute all
+000042e0: 2072 656c 6576 616e 7420 6172 6561 7320   relevant areas 
+000042f0: 2868 6561 642c 2074 6f72 736f 2c20 6261  (head, torso, ba
+00004300: 636b 2920 7065 7220 7669 6465 6f20 616e  ck) per video an
+00004310: 6420 7065 7220 6672 616d 6520 696e 2074  d per frame in t
+00004320: 6865 2064 6174 612e 0a0a 2020 2020 2020  he data...      
+00004330: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+00004340: 2020 2020 7461 625f 6469 6374 2028 6469      tab_dict (di
+00004350: 6374 293a 2044 6963 7469 6f6e 6172 7920  ct): Dictionary 
+00004360: 6f66 2070 616e 6461 7320 4461 7461 4672  of pandas DataFr
+00004370: 616d 6573 2063 6f6e 7461 696e 696e 6720  ames containing 
+00004380: 7468 6520 7472 616a 6563 746f 7269 6573  the trajectories
+00004390: 206f 6620 616c 6c20 626f 6479 7061 7274   of all bodypart
+000043a0: 732e 0a20 2020 2020 2020 2020 2020 2076  s..            v
+000043b0: 6572 626f 7365 2028 626f 6f6c 293a 2049  erbose (bool): I
+000043c0: 6620 5472 7565 2c20 7072 696e 7473 2070  f True, prints p
+000043d0: 726f 6772 6573 732e 2044 6566 6175 6c74  rogress. Default
+000043e0: 7320 746f 2054 7275 652e 0a0a 2020 2020  s to True...    
+000043f0: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+00004400: 2020 2020 2020 2020 2064 6963 743a 2044           dict: D
+00004410: 6963 7469 6f6e 6172 7920 6f66 2070 616e  ictionary of pan
+00004420: 6461 7320 4461 7461 4672 616d 6573 2063  das DataFrames c
+00004430: 6f6e 7461 696e 696e 6720 7468 6520 6469  ontaining the di
+00004440: 7374 616e 6365 7320 6265 7477 6565 6e20  stances between 
+00004450: 616c 6c20 626f 6479 7061 7274 732e 0a0a  all bodyparts...
+00004460: 2020 2020 2020 2020 7a12 436f 6d70 7574          z.Comput
+00004470: 696e 6720 6172 6561 732e 2e2e 722d 0000  ing areas...r-..
+00004480: 004e 6301 0000 0000 0000 0000 0000 0001  .Nc.............
+00004490: 0000 0004 0000 0013 0000 0073 1000 0000  ...........s....
+000044a0: 7400 6a01 6a02 7c00 8800 6401 8d02 5300  t.j.j.|...d...S.
+000044b0: 2902 4e29 01da 0961 6e69 6d61 6c5f 6964  ).N)...animal_id
+000044c0: 2903 7282 0000 0072 8300 0000 da0d 636f  ).r....r......co
+000044d0: 6d70 7574 655f 6172 6561 73a9 0172 a600  mpute_areas..r..
+000044e0: 0000 a901 7297 0000 0072 2700 0000 7228  ....r....r'...r(
+000044f0: 0000 0072 a500 0000 6402 0000 724e 0000  ...r....d...rN..
+00004500: 007a 2350 726f 6a65 6374 2e67 6574 5f61  .z#Project.get_a
+00004510: 7265 6173 2e3c 6c6f 6361 6c73 3e2e 3c6c  reas.<locals>.<l
+00004520: 616d 6264 613e 7232 0000 0072 ac00 0000  ambda>r2...r....
+00004530: 2904 da09 6865 6164 5f61 7265 61da 0a74  )...head_area..t
+00004540: 6f72 736f 5f61 7265 61da 0962 6163 6b5f  orso_area..back_
+00004550: 6172 6561 da09 6675 6c6c 5f61 7265 61a9  area..full_area.
+00004560: 0272 ca00 0000 72b8 0000 007a 047b 7d7b  .r....r....z.{}{
+00004570: 7d72 8d00 0000 7a80 4974 2073 6565 6d73  }r....z.It seems
+00004580: 2079 6f75 2772 6520 7573 696e 6720 6120   you're using a 
+00004590: 6375 7374 6f6d 206c 6162 656c 6c69 6e67  custom labelling
+000045a0: 2073 6368 656d 6520 7768 6963 6820 6973   scheme which is
+000045b0: 206d 6973 7369 6e67 206b 6579 2062 6f64   missing key bod
+000045c0: 7920 7061 7274 732e 2059 6f75 2063 616e  y parts. You can
+000045d0: 2070 726f 6365 6564 2c20 6275 7420 6e6f   proceed, but no
+000045e0: 2061 7265 6173 2077 696c 6c20 6265 2063   areas will be c
+000045f0: 6f6d 7075 7465 642e 2913 7281 0000 0072  omputed.).r....r
+00004600: cc00 0000 72bf 0000 0072 dc00 0000 7234  ....r....r....r4
+00004610: 0000 0072 c400 0000 7282 0000 0072 8300  ...r....r....r..
+00004620: 0000 da0e 6669 6c74 6572 5f63 6f6c 756d  ....filter_colum
+00004630: 6e73 72b8 0000 00da 0561 7070 6c79 da07  nsr......apply..
+00004640: 746f 5f6c 6973 7472 ca00 0000 da0a 6164  to_listr......ad
+00004650: 645f 7072 6566 6978 726d 0000 0072 d800  d_prefixrm...r..
+00004660: 0000 72ff 0000 00da 0877 6172 6e69 6e67  ..r......warning
+00004670: 73da 0477 6172 6e29 0872 5700 0000 72e3  s..warn).rW...r.
+00004680: 0000 0072 8000 0000 da0a 6172 6561 735f  ...r......areas_
+00004690: 6469 6374 72e6 0000 0072 5500 0000 da09  dictr....rU.....
+000046a0: 6578 705f 7461 626c 65da 0d63 7572 7265  exp_table..curre
+000046b0: 6e74 5f74 6162 6c65 7227 0000 0072 0901  nt_tabler'...r..
+000046c0: 0000 7228 0000 00da 0967 6574 5f61 7265  ..r(.....get_are
+000046d0: 6173 4502 0000 7342 0000 0000 0b04 0108  asE...sB........
+000046e0: 0204 0202 0110 0208 020a 0208 0104 0304  ................
+000046f0: 0116 ff04 0304 010c ff06 0304 0106 0104  ................
+00004700: 0106 fd06 0504 010e 010e fe02 fb04 0b14  ................
+00004710: 020e 020c 0104 0102 ff04 0308 027a 1150  .............z.P
+00004720: 726f 6a65 6374 2e67 6574 5f61 7265 6173  roject.get_areas
+00004730: 2903 7280 0000 00da 0566 6f72 6365 721a  ).r......forcer.
+00004740: 0000 0063 0300 0000 0000 0000 0000 0000  ...c............
+00004750: 0900 0000 1700 0000 4300 0000 736e 0100  ........C...sn..
+00004760: 007c 0172 0c74 0064 0183 0101 007c 0272  .|.r.t.d.....|.r
+00004770: 4074 016a 02a0 0374 016a 02a0 047c 006a  @t.j...t.j...|.j
+00004780: 057c 006a 06a1 02a1 0172 4074 0774 016a  .|.j.....r@t.t.j
+00004790: 02a0 047c 006a 057c 006a 06a1 0283 0101  ...|.j.|.j......
+000047a0: 007c 00a0 08a1 0001 0074 0974 0aa0 0b74  .|.......t.t...t
+000047b0: 0ca0 0d74 016a 02a0 047c 006a 0e7c 006a  ...t.j...|.j.|.j
+000047c0: 0f64 0219 00a1 02a1 016a 10a1 0183 017c  .d.......j.....|
+000047d0: 005f 107c 00a0 117c 01a1 015c 027d 037d  ._.|...|...\.}.}
+000047e0: 047c 006a 1264 0375 0172 a47c 03a0 13a1  .|.j.d.u.r.|....
+000047f0: 007c 006a 12a0 13a1 006b 0273 a44a 0064  .|.j.....k.s.J.d
+00004800: 0483 0182 0164 037d 0564 037d 0664 037d  .....d.}.d.}.d.}
+00004810: 077c 00a0 147c 037c 01a1 025c 037c 005f  .|...|.|...\.|._
+00004820: 157c 005f 167c 005f 177c 006a 1872 da7c  .|._.|._.|.j.r.|
+00004830: 00a0 197c 037c 01a1 027d 057c 006a 1a72  ...|.|...}.|.j.r
+00004840: ec7c 00a0 1b7c 037c 01a1 027d 067c 006a  .|...|.|...}.|.j
+00004850: 1c72 fe7c 00a0 1d7c 037c 01a1 027d 0774  .r.|...|.|...}.t
+00004860: 1e7c 006a 057c 006a 067c 067c 006a 1f7c  .|.j.|.j.|.|.j.|
+00004870: 077c 006a 207c 006a 217c 006a 227c 057c  .|.j |.j!|.j"|.|
+00004880: 006a 237c 006a 247c 006a 107c 006a 127c  .j#|.j$|.j.|.j.|
+00004890: 006a 057c 047c 006a 157c 006a 167c 037c  .j.|.|.j.|.j.|.|
+000048a0: 006a 257c 006a 0f7c 006a 1764 058d 157d  .j%|.j.|.j.d...}
+000048b0: 087c 086a 2664 0664 078d 0101 007c 0190  .|.j&d.d.....|..
+000048c0: 0172 6a74 0064 0883 0101 007c 0853 0029  .rjt.d.....|.S.)
+000048d0: 0961 3001 0000 4765 6e65 7261 7465 2061  .a0...Generate a
+000048e0: 2064 6565 706f 662e 436f 6f72 6469 6e61   deepof.Coordina
+000048f0: 7465 7320 6461 7461 7365 7420 7573 696e  tes dataset usin
+00004900: 6720 616c 6c20 7468 6520 6f70 7469 6f6e  g all the option
+00004910: 7320 7370 6563 6966 6965 6420 6475 7269  s specified duri
+00004920: 6e67 2069 6e69 7469 616c 697a 6174 696f  ng initializatio
+00004930: 6e2e 0a0a 2020 2020 2020 2020 4172 6773  n...        Args
+00004940: 3a0a 2020 2020 2020 2020 2020 2020 7665  :.            ve
+00004950: 7262 6f73 6520 2862 6f6f 6c29 3a20 4966  rbose (bool): If
+00004960: 2054 7275 652c 2070 7269 6e74 7320 7072   True, prints pr
+00004970: 6f67 7265 7373 2e20 4465 6661 756c 7473  ogress. Defaults
+00004980: 2074 6f20 5472 7565 2e0a 0a20 2020 2020   to True...     
+00004990: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+000049a0: 2020 2020 2020 2020 636f 6f72 6469 6e61          coordina
+000049b0: 7465 733a 2044 6565 706f 662e 436f 6f72  tes: Deepof.Coor
+000049c0: 6469 6e61 7465 7320 6f62 6a65 6374 2063  dinates object c
+000049d0: 6f6e 7461 696e 696e 6720 7468 6520 7472  ontaining the tr
+000049e0: 616a 6563 746f 7269 6573 206f 6620 616c  ajectories of al
+000049f0: 6c20 626f 6479 7061 7274 732e 0a0a 2020  l bodyparts...  
+00004a00: 2020 2020 2020 7a21 5365 7474 696e 6720        z!Setting 
+00004a10: 7570 2070 726f 6a65 6374 2064 6972 6563  up project direc
+00004a20: 746f 7269 6573 2e2e 2e72 0100 0000 4e7a  tories...r....Nz
+00004a30: 2f65 7870 6572 696d 656e 7461 6c20 4944  /experimental ID
+00004a40: 7320 696e 2065 7870 5f63 6f6e 6469 7469  s in exp_conditi
+00004a50: 6f6e 7320 646f 206e 6f74 206d 6174 6368  ons do not match
+00004a60: 2915 7219 0000 0072 3f00 0000 7262 0000  ).r....r?...rb..
+00004a70: 0072 3400 0000 7263 0000 0072 3500 0000  .r4...rc...r5...
+00004a80: 7260 0000 0072 3600 0000 7265 0000 0072  r`...r6...re...r
+00004a90: 6400 0000 da12 6578 636c 7564 6564 5f62  d.....excluded_b
+00004aa0: 6f64 7970 6172 7473 7268 0000 0072 3900  odypartsrh...r9.
+00004ab0: 0000 721f 0000 0072 ae00 0000 72f2 0000  ..r....r....r...
+00004ac0: 00da 0c61 7265 6e61 5f70 6172 616d 7372  ...arena_paramsr
+00004ad0: 5e00 0000 da12 7472 6169 6e65 645f 6d6f  ^.....trained_mo
+00004ae0: 6465 6c5f 7061 7468 725d 0000 00da 1076  del_pathr].....v
+00004af0: 6964 656f 5f72 6573 6f6c 7574 696f 6e46  ideo_resolutionF
+00004b00: a901 da09 7469 6d65 7374 616d 70fa 0544  ....timestamp..D
+00004b10: 6f6e 6521 2927 7281 0000 0072 1e00 0000  one!)'r....r....
+00004b20: 721f 0000 0072 7400 0000 7220 0000 0072  r....rt...r ...r
+00004b30: 1900 0000 723f 0000 0072 0600 0000 7279  ....r?...r....ry
+00004b40: 0000 00da 0369 6e74 72de 0000 00da 0572  .....intr......r
+00004b50: 6f75 6e64 da04 7069 6d73 da0d 496d 6167  ound..pims..Imag
+00004b60: 6549 4f52 6561 6465 7272 4000 0000 725d  eIOReaderr@...r]
+00004b70: 0000 0072 6800 0000 72ee 0000 0072 3900  ...rh...r....r9.
+00004b80: 0000 72f6 0000 0072 8500 0000 72f2 0000  ..r....r....r...
+00004b90: 0072 1b01 0000 721d 0100 0072 6500 0000  .r....r....re...
+00004ba0: 72fa 0000 0072 6200 0000 7205 0100 0072  r....rb...r....r
+00004bb0: 6300 0000 7218 0100 0072 1b00 0000 7234  c...r....r....r4
+00004bc0: 0000 0072 3500 0000 7260 0000 0072 3600  ...r5...r`...r6.
+00004bd0: 0000 7264 0000 0072 3800 0000 725a 0000  ..rd...r8...rZ..
+00004be0: 00da 0473 6176 6529 0972 5700 0000 7280  ...save).rW...r.
+00004bf0: 0000 0072 1901 0000 725e 0000 0072 ae00  ...r....r^...r..
+00004c00: 0000 7265 0000 0072 6200 0000 7263 0000  ..re...rb...rc..
+00004c10: 0072 a700 0000 7227 0000 0072 2700 0000  .r....r'...r'...
+00004c20: 7228 0000 00da 0663 7265 6174 657d 0200  r(.....create}..
+00004c30: 0073 7200 0000 000a 0401 0802 1e01 1602  .sr.............
+00004c40: 0801 0201 0401 0401 14ff 04ff 02ff 0608  ................
+00004c50: 0e01 0a02 10ff 0402 02fe 0404 0401 0401  ................
+00004c60: 0403 0401 04ff 1004 0601 0c02 0601 0c02  ................
+00004c70: 0601 0c02 0201 0401 0401 0201 0401 0201  ................
+00004c80: 0401 0401 0401 0201 0401 0401 0401 0401  ................
+00004c90: 0401 0201 0401 0401 0201 0401 0401 04eb  ................
+00004ca0: 0619 0c02 0601 0802 7a0e 5072 6f6a 6563  ........z.Projec
+00004cb0: 742e 6372 6561 7465 6302 0000 0000 0000  t.createc.......
+00004cc0: 0000 0000 0002 0000 0002 0000 0043 0000  .............C..
+00004cd0: 0073 0a00 0000 7c01 7c00 5f00 6400 5300  .s....|.|._.d.S.
+00004ce0: a901 4e72 7a00 0000 a902 7257 0000 00da  ..Nrz.....rW....
+00004cf0: 0576 616c 7565 7227 0000 0072 2700 0000  .valuer'...r'...
+00004d00: 7228 0000 0072 6500 0000 ce02 0000 7302  r(...re.......s.
+00004d10: 0000 0000 0263 0200 0000 0000 0000 0000  .....c..........
+00004d20: 0000 0200 0000 0200 0000 4300 0000 730a  ..........C...s.
+00004d30: 0000 007c 017c 005f 0064 0053 0072 2701  ...|.|._.d.S.r'.
+00004d40: 0000 727c 0000 0072 2801 0000 7227 0000  ..r|...r(...r'..
+00004d50: 0072 2700 0000 7228 0000 0072 6600 0000  .r'...r(...rf...
+00004d60: d202 0000 7302 0000 0000 0263 0200 0000  ....s......c....
+00004d70: 0000 0000 0000 0000 0200 0000 0200 0000  ................
+00004d80: 4300 0000 730a 0000 007c 017c 005f 0064  C...s....|.|._.d
+00004d90: 0053 0072 2701 0000 727e 0000 0072 2801  .S.r'...r~...r(.
+00004da0: 0000 7227 0000 0072 2700 0000 7228 0000  ..r'...r'...r(..
+00004db0: 0072 6200 0000 d602 0000 7302 0000 0000  .rb.......s.....
+00004dc0: 0229 0146 2901 5429 0154 2901 5429 0154  .).F).T).T).T).T
+00004dd0: 2902 5446 2922 7259 0000 00da 0a5f 5f6d  ).TF)"rY.....__m
+00004de0: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+00004df0: 616d 655f 5fda 075f 5f64 6f63 5f5f 72d2  ame__..__doc__r.
+00004e00: 0000 0072 1e00 0000 721f 0000 0072 2000  ...r....r....r .
+00004e10: 0000 7214 0000 0072 a300 0000 da04 626f  ..r....r......bo
+00004e20: 6f6c da04 6469 6374 7221 0100 0072 c100  ol..dictr!...r..
+00004e30: 0000 726a 0000 0072 6e00 0000 726f 0000  ..rj...rn...ro..
+00004e40: 0072 7900 0000 da08 7072 6f70 6572 7479  .ry.....property
+00004e50: 7265 0000 0072 6600 0000 7262 0000 0072  re...rf...rb...r
+00004e60: b600 0000 72de 0000 0072 df00 0000 7285  ....r....r....r.
+00004e70: 0000 0072 1500 0000 72ee 0000 0072 fa00  ...r....r....r..
+00004e80: 0000 7205 0100 0072 1801 0000 7226 0000  ..r....r....r&..
+00004e90: 0072 2601 0000 da06 7365 7474 6572 7227  .r&.....setterr'
+00004ea0: 0000 0072 2700 0000 7227 0000 0072 2800  ...r'...r'...r(.
+00004eb0: 0000 722a 0000 0055 0000 0073 7e00 0000  ..r*...U...s~...
+00004ec0: 0801 0408 0201 0201 0201 0201 0801 0201  ................
+00004ed0: 0201 0201 0201 0201 0201 0201 0a01 0201  ................
+00004ee0: 0201 0201 0201 0201 02ec 0202 0201 0201  ................
+00004ef0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00004f00: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00004f10: 02ec 0c68 0804 0804 0849 0201 0a04 0201  ...h.....I......
+00004f20: 0a04 0201 0a04 1617 127f 002a 142e 1433  ...........*...3
+00004f30: 1438 1451 0401 0a03 0401 0a03 0401 722a  .8.Q..........r*
+00004f40: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00004f50: 0000 0000 1e00 0000 4000 0000 73da 0100  ........@...s...
+00004f60: 0065 005a 0164 005a 0264 015a 0364 0265  .e.Z.d.Z.d.Z.d.e
+00004f70: 0464 0367 0183 0164 0264 0264 0264 0264  .d.g...d.d.d.d.d
+00004f80: 0266 0765 0565 0565 0565 066a 0765 0565  .f.e.e.e.e.j.e.e
+00004f90: 0565 0865 066a 0965 0a65 0b65 0865 0565  .e.e.j.e.e.e.e.e
+00004fa0: 0b65 0b65 0865 0b65 0865 0865 0c6a 0d65  .e.e.e.e.e.e.j.e
+00004fb0: 0e65 0864 049c 1564 0564 0684 055a 0f64  .e.d...d.d...Z.d
+00004fc0: 0764 0884 005a 1064 0964 0a84 005a 1164  .d...Z.d.d...Z.d
+00004fd0: 4265 0565 1265 0a65 0565 1265 0565 1265  Be.e.e.e.e.e.e.e
+00004fe0: 1365 1464 0e9c 0964 0f64 1084 055a 1564  .e.d...d.d...Z.d
+00004ff0: 4365 0a65 0565 1265 1265 1365 1464 119c  Ce.e.e.e.e.e.d..
+00005000: 0664 1264 1384 055a 1664 4465 1265 0a65  .d.d...Z.dDe.e.e
+00005010: 0565 1265 1365 1464 149c 0664 1564 1684  .e.e.e.d...d.d..
+00005020: 055a 1764 4565 0a65 0565 1464 189c 0364  .Z.dEe.e.e.d...d
+00005030: 1964 1a84 055a 1864 4665 1264 1b9c 0164  .d...Z.dFe.d...d
+00005040: 1c64 1d84 055a 1965 1a64 1e64 1f84 0083  .d...Z.e.d.d....
+00005050: 015a 1b64 2064 2184 005a 1c64 2264 2384  .Z.d d!..Z.d"d#.
+00005060: 005a 1d65 1a64 2464 2584 0083 015a 1e64  .Z.e.d$d%....Z.d
+00005070: 4765 0e65 0565 1264 269c 0364 2764 2884  Ge.e.e.d&..d'd(.
+00005080: 055a 1f64 4865 0565 1264 299c 0264 2a64  .Z.dHe.e.d)..d*d
+00005090: 2b84 055a 2064 4965 0565 1465 0565 1265  +..Z dIe.e.e.e.e
+000050a0: 0565 1265 1464 2c9c 0764 2d64 2e84 055a  .e.e.d,..d-d...Z
+000050b0: 2169 0064 0b65 066a 2264 0b64 2f64 0b66  !i.d.e.j"d.d/d.f
+000050c0: 0665 1365 1265 0a65 1265 0a65 1265 1464  .e.e.e.e.e.e.e.d
+000050d0: 309c 0764 3164 3284 055a 2364 4a65 2465  0..d1d2..Z#dJe$e
+000050e0: 066a 0965 066a 0965 066a 0965 066a 0966  .j.e.j.e.j.e.j.f
+000050f0: 0419 0065 066a 0965 0565 0565 0a65 0a65  ...e.j.e.e.e.e.e
+00005100: 0a65 1265 1265 0a65 2565 2565 0565 0565  .e.e.e.e%e%e.e.e
+00005110: 2565 2565 0565 0565 1265 1265 0565 0a65  %e%e.e.e.e.e.e.e
+00005120: 0565 0a65 2565 1265 2565 2464 3f9c 1c64  .e.e%e.e%e$d?..d
+00005130: 4064 4184 055a 2664 0253 0029 4b72 1b00  @dA..Z&d.S.)Kr..
+00005140: 0000 7a84 436c 6173 7320 666f 7220 7374  ..z.Class for st
+00005150: 6f72 696e 6720 7468 6520 7265 7375 6c74  oring the result
+00005160: 7320 6f66 2061 2072 616e 2070 726f 6a65  s of a ran proje
+00005170: 6374 2e20 4d65 7468 6f64 7320 6172 6520  ct. Methods are 
+00005180: 6d6f 7374 6c79 2073 6574 7465 7273 2061  mostly setters a
+00005190: 6e64 2067 6574 7465 7273 2069 6e20 6368  nd getters in ch
+000051a0: 6172 6765 206f 6620 7469 6479 696e 6720  arge of tidying 
+000051b0: 7570 2074 6865 2067 656e 6572 6174 6564  up the generated
+000051c0: 2074 6162 6c65 732e 4e72 2d00 0000 2915   tables.Nr-...).
+000051d0: 7219 0000 0072 3f00 0000 7235 0000 0072  r....r?...r5...r
+000051e0: 6000 0000 7236 0000 0072 1f00 0000 72ae  `...r6...r....r.
+000051f0: 0000 0072 f200 0000 7268 0000 0072 1b01  ...r....rh...r..
+00005200: 0000 725e 0000 0072 1c01 0000 725d 0000  ..r^...r....r]..
+00005210: 0072 1d01 0000 7262 0000 0072 3400 0000  .r....rb...r4...
+00005220: 7263 0000 0072 6500 0000 7264 0000 0072  rc...re...rd...r
+00005230: 1a01 0000 7239 0000 0063 1600 0000 0000  ....r9...c......
+00005240: 0000 0000 0000 1600 0000 0200 0000 4300  ..............C.
+00005250: 0000 7382 0000 007c 017c 005f 007c 027c  ..s....|.|._.|.|
+00005260: 005f 017c 107c 005f 027c 037c 005f 037c  ._.|.|._.|.|._.|
+00005270: 0a7c 005f 047c 047c 005f 057c 057c 005f  .|._.|.|._.|.|._
+00005280: 067c 147c 005f 077c 157c 005f 087c 097c  .|.|._.|.|._.|.|
+00005290: 005f 097c 067c 005f 0a7c 077c 005f 0b7c  ._.|.|._.|.|._.|
+000052a0: 087c 005f 0c7c 0b7c 005f 0d7c 0c7c 005f  .|._.|.|._.|.|._
+000052b0: 0e7c 0d7c 005f 0f7c 0e7c 005f 107c 0f7c  .|.|._.|.|._.|.|
+000052c0: 005f 117c 117c 005f 127c 127c 005f 137c  ._.|.|._.|.|._.|
+000052d0: 137c 005f 1464 0153 0029 0261 5109 0000  .|._.d.S.).aQ...
+000052e0: 436c 6173 7320 666f 7220 7374 6f72 696e  Class for storin
+000052f0: 6720 7468 6520 7265 7375 6c74 7320 6f66  g the results of
+00005300: 2061 2072 616e 2070 726f 6a65 6374 2e20   a ran project. 
+00005310: 4d65 7468 6f64 7320 6172 6520 6d6f 7374  Methods are most
+00005320: 6c79 2073 6574 7465 7273 2061 6e64 2067  ly setters and g
+00005330: 6574 7465 7273 2069 6e20 6368 6172 6765  etters in charge
+00005340: 206f 6620 7469 6479 696e 6720 7570 2074   of tidying up t
+00005350: 6865 2067 656e 6572 6174 6564 2074 6162  he generated tab
+00005360: 6c65 732e 0a0a 2020 2020 2020 2020 4172  les...        Ar
+00005370: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+00005380: 7072 6f6a 6563 745f 6e61 6d65 2028 7374  project_name (st
+00005390: 7229 3a20 6e61 6d65 206f 6620 7468 6520  r): name of the 
+000053a0: 6375 7272 656e 7420 7072 6f6a 6563 742e  current project.
+000053b0: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
+000053c0: 6a65 6374 5f70 6174 6820 2873 7472 293a  ject_path (str):
+000053d0: 2070 6174 6820 746f 2074 6865 2066 6f6c   path to the fol
+000053e0: 6465 7220 636f 6e74 6169 6e69 6e67 2074  der containing t
+000053f0: 6865 2044 4c43 206f 7574 7075 7420 6461  he DLC output da
+00005400: 7461 2e0a 2020 2020 2020 2020 2020 2020  ta..            
+00005410: 6172 656e 6120 2873 7472 293a 2054 7970  arena (str): Typ
+00005420: 6520 6f66 2061 7265 6e61 2075 7365 6420  e of arena used 
+00005430: 666f 7220 7468 6520 6578 7065 7269 6d65  for the experime
+00005440: 6e74 2e20 5365 6520 6465 6570 6f66 2e64  nt. See deepof.d
+00005450: 6174 612e 5072 6f6a 6563 7420 666f 7220  ata.Project for 
+00005460: 6d6f 7265 2069 6e66 6f72 6d61 7469 6f6e  more information
+00005470: 2e0a 2020 2020 2020 2020 2020 2020 6172  ..            ar
+00005480: 656e 615f 6469 6d73 2028 6e70 2e61 7272  ena_dims (np.arr
+00005490: 6179 293a 2044 696d 656e 7369 6f6e 7320  ay): Dimensions 
+000054a0: 6f66 2074 6865 2061 7265 6e61 2e20 5365  of the arena. Se
+000054b0: 6520 6465 6570 6f66 2e64 6174 612e 5072  e deepof.data.Pr
+000054c0: 6f6a 6563 7420 666f 7220 6d6f 7265 2069  oject for more i
+000054d0: 6e66 6f72 6d61 7469 6f6e 2e0a 2020 2020  nformation..    
+000054e0: 2020 2020 2020 2020 626f 6479 7061 7274          bodypart
+000054f0: 5f67 7261 7068 2028 6e78 2e47 7261 7068  _graph (nx.Graph
+00005500: 293a 2047 7261 7068 2063 6f6e 7461 696e  ): Graph contain
+00005510: 696e 6720 7468 6520 626f 6479 2070 6172  ing the body par
+00005520: 7420 636f 6e6e 6563 7469 7669 7479 2e20  t connectivity. 
+00005530: 5365 6520 6465 6570 6f66 2e64 6174 612e  See deepof.data.
+00005540: 5072 6f6a 6563 7420 666f 7220 6d6f 7265  Project for more
+00005550: 2069 6e66 6f72 6d61 7469 6f6e 2e0a 2020   information..  
+00005560: 2020 2020 2020 2020 2020 7061 7468 2028            path (
+00005570: 7374 7229 3a20 5061 7468 2074 6f20 7468  str): Path to th
+00005580: 6520 666f 6c64 6572 2063 6f6e 7461 696e  e folder contain
+00005590: 696e 6720 7468 6520 7265 7375 6c74 7320  ing the results 
+000055a0: 6f66 2074 6865 2065 7870 6572 696d 656e  of the experimen
+000055b0: 742e 0a20 2020 2020 2020 2020 2020 2071  t..            q
+000055c0: 7561 6c69 7479 2028 6469 6374 293a 2044  uality (dict): D
+000055d0: 6963 7469 6f6e 6172 7920 636f 6e74 6169  ictionary contai
+000055e0: 6e69 6e67 2074 6865 2071 7561 6c69 7479  ning the quality
+000055f0: 206f 6620 7468 6520 6578 7065 7269 6d65   of the experime
+00005600: 6e74 2e20 5365 6520 6465 6570 6f66 2e64  nt. See deepof.d
+00005610: 6174 612e 5072 6f6a 6563 7420 666f 7220  ata.Project for 
+00005620: 6d6f 7265 2069 6e66 6f72 6d61 7469 6f6e  more information
+00005630: 2e0a 2020 2020 2020 2020 2020 2020 7363  ..            sc
+00005640: 616c 6573 2028 6e70 2e6e 6461 7272 6179  ales (np.ndarray
+00005650: 293a 2053 6361 6c65 7320 7573 6564 2066  ): Scales used f
+00005660: 6f72 2074 6865 2065 7870 6572 696d 656e  or the experimen
+00005670: 742e 2053 6565 2064 6565 706f 662e 6461  t. See deepof.da
+00005680: 7461 2e50 726f 6a65 6374 2066 6f72 206d  ta.Project for m
+00005690: 6f72 6520 696e 666f 726d 6174 696f 6e2e  ore information.
+000056a0: 0a20 2020 2020 2020 2020 2020 2066 7261  .            fra
+000056b0: 6d65 5f72 6174 6520 2869 6e74 293a 2066  me_rate (int): f
+000056c0: 7261 6d65 2072 6174 6520 6f66 2074 6865  rame rate of the
+000056d0: 2070 726f 6365 7373 6564 2076 6964 656f   processed video
+000056e0: 732e 0a20 2020 2020 2020 2020 2020 2061  s..            a
+000056f0: 7265 6e61 5f70 6172 616d 7320 284c 6973  rena_params (Lis
+00005700: 7429 3a20 4c69 7374 2063 6f6e 7461 696e  t): List contain
+00005710: 696e 6720 7468 6520 7061 7261 6d65 7465  ing the paramete
+00005720: 7273 206f 6620 7468 6520 6172 656e 612e  rs of the arena.
+00005730: 2053 6565 2064 6565 706f 662e 6461 7461   See deepof.data
+00005740: 2e50 726f 6a65 6374 2066 6f72 206d 6f72  .Project for mor
+00005750: 6520 696e 666f 726d 6174 696f 6e2e 0a20  e information.. 
+00005760: 2020 2020 2020 2020 2020 2074 6162 6c65             table
+00005770: 7320 2864 6963 7429 3a20 4469 6374 696f  s (dict): Dictio
+00005780: 6e61 7279 2063 6f6e 7461 696e 696e 6720  nary containing 
+00005790: 7468 6520 7461 626c 6573 206f 6620 7468  the tables of th
+000057a0: 6520 6578 7065 7269 6d65 6e74 2e20 5365  e experiment. Se
+000057b0: 6520 6465 6570 6f66 2e64 6174 612e 5072  e deepof.data.Pr
+000057c0: 6f6a 6563 7420 666f 7220 6d6f 7265 2069  oject for more i
+000057d0: 6e66 6f72 6d61 7469 6f6e 2e0a 2020 2020  nformation..    
+000057e0: 2020 2020 2020 2020 7472 6169 6e65 645f          trained_
+000057f0: 6d6f 6465 6c5f 7061 7468 2028 7374 7229  model_path (str)
+00005800: 3a20 5061 7468 2074 6f20 7468 6520 7472  : Path to the tr
+00005810: 6169 6e65 6420 6d6f 6465 6c73 2075 7365  ained models use
+00005820: 6420 666f 7220 7468 6520 7375 7065 7276  d for the superv
+00005830: 6973 6564 2070 6970 656c 696e 652e 2046  ised pipeline. F
+00005840: 6f72 2069 6e74 6572 6e61 6c20 7573 6520  or internal use 
+00005850: 6f6e 6c79 2e0a 2020 2020 2020 2020 2020  only..          
+00005860: 2020 7669 6465 6f73 2028 4c69 7374 293a    videos (List):
+00005870: 204c 6973 7420 636f 6e74 6169 6e69 6e67   List containing
+00005880: 2074 6865 2076 6964 656f 7320 7573 6564   the videos used
+00005890: 2066 6f72 2074 6865 2065 7870 6572 696d   for the experim
+000058a0: 656e 742e 2053 6565 2064 6565 706f 662e  ent. See deepof.
+000058b0: 6461 7461 2e50 726f 6a65 6374 2066 6f72  data.Project for
+000058c0: 206d 6f72 6520 696e 666f 726d 6174 696f   more informatio
+000058d0: 6e2e 0a20 2020 2020 2020 2020 2020 2076  n..            v
+000058e0: 6964 656f 5f72 6573 6f6c 7574 696f 6e20  ideo_resolution 
+000058f0: 284c 6973 7429 3a20 4c69 7374 2063 6f6e  (List): List con
+00005900: 7461 696e 696e 6720 7468 6520 6175 746f  taining the auto
+00005910: 6d61 7469 6361 6c6c 7920 6465 7465 6374  matically detect
+00005920: 6564 2072 6573 6f6c 7574 696f 6e20 6f66  ed resolution of
+00005930: 2074 6865 2076 6964 656f 7320 7573 6564   the videos used
+00005940: 2066 6f72 2074 6865 2065 7870 6572 696d   for the experim
+00005950: 656e 742e 0a20 2020 2020 2020 2020 2020  ent..           
+00005960: 2061 6e67 6c65 7320 2864 6963 7429 3a20   angles (dict): 
+00005970: 4469 6374 696f 6e61 7279 2063 6f6e 7461  Dictionary conta
+00005980: 696e 696e 6720 7468 6520 616e 676c 6573  ining the angles
+00005990: 206f 6620 7468 6520 6578 7065 7269 6d65   of the experime
+000059a0: 6e74 2e20 5365 6520 6465 6570 6f66 2e64  nt. See deepof.d
+000059b0: 6174 612e 5072 6f6a 6563 7420 666f 7220  ata.Project for 
+000059c0: 6d6f 7265 2069 6e66 6f72 6d61 7469 6f6e  more information
+000059d0: 2e0a 2020 2020 2020 2020 2020 2020 616e  ..            an
+000059e0: 696d 616c 5f69 6473 2028 4c69 7374 293a  imal_ids (List):
+000059f0: 204c 6973 7420 636f 6e74 6169 6e69 6e67   List containing
+00005a00: 2074 6865 2061 6e69 6d61 6c20 4944 7320   the animal IDs 
+00005a10: 6f66 2074 6865 2065 7870 6572 696d 656e  of the experimen
+00005a20: 742e 2053 6565 2064 6565 706f 662e 6461  t. See deepof.da
+00005a30: 7461 2e50 726f 6a65 6374 2066 6f72 206d  ta.Project for m
+00005a40: 6f72 6520 696e 666f 726d 6174 696f 6e2e  ore information.
+00005a50: 0a20 2020 2020 2020 2020 2020 2061 7265  .            are
+00005a60: 6173 2028 6469 6374 293a 2064 6963 7469  as (dict): dicti
+00005a70: 6f6e 6172 7920 7769 7468 2061 7265 6173  onary with areas
+00005a80: 2074 6f20 636f 6d70 7574 652e 2042 7920   to compute. By 
+00005a90: 6465 6661 756c 742c 2069 7420 696e 636c  default, it incl
+00005aa0: 7564 6573 2068 6561 642c 2074 6f72 736f  udes head, torso
+00005ab0: 2c20 616e 6420 6261 636b 2e0a 2020 2020  , and back..    
+00005ac0: 2020 2020 2020 2020 6469 7374 616e 6365          distance
+00005ad0: 7320 2864 6963 7429 3a20 4469 6374 696f  s (dict): Dictio
+00005ae0: 6e61 7279 2063 6f6e 7461 696e 696e 6720  nary containing 
+00005af0: 7468 6520 6469 7374 616e 6365 7320 6f66  the distances of
+00005b00: 2074 6865 2065 7870 6572 696d 656e 742e   the experiment.
+00005b10: 2053 6565 2064 6565 706f 662e 6461 7461   See deepof.data
+00005b20: 2e50 726f 6a65 6374 2066 6f72 206d 6f72  .Project for mor
+00005b30: 6520 696e 666f 726d 6174 696f 6e2e 0a20  e information.. 
+00005b40: 2020 2020 2020 2020 2020 2065 7863 6c75             exclu
+00005b50: 6465 645f 626f 6479 7061 7274 7320 286c  ded_bodyparts (l
+00005b60: 6973 7429 3a20 6c69 7374 206f 6620 626f  ist): list of bo
+00005b70: 6479 7061 7274 7320 746f 2065 7863 6c75  dyparts to exclu
+00005b80: 6465 2066 726f 6d20 616e 616c 7973 6973  de from analysis
+00005b90: 2e0a 2020 2020 2020 2020 2020 2020 6578  ..            ex
+00005ba0: 705f 636f 6e64 6974 696f 6e73 2028 6469  p_conditions (di
+00005bb0: 6374 293a 2044 6963 7469 6f6e 6172 7920  ct): Dictionary 
+00005bc0: 636f 6e74 6169 6e69 6e67 2074 6865 2065  containing the e
+00005bd0: 7870 6572 696d 656e 7461 6c20 636f 6e64  xperimental cond
+00005be0: 6974 696f 6e73 206f 6620 7468 6520 6578  itions of the ex
+00005bf0: 7065 7269 6d65 6e74 2e20 5365 6520 6465  periment. See de
+00005c00: 6570 6f66 2e64 6174 612e 5072 6f6a 6563  epof.data.Projec
+00005c10: 7420 666f 7220 6d6f 7265 2069 6e66 6f72  t for more infor
+00005c20: 6d61 7469 6f6e 2e0a 0a20 2020 2020 2020  mation...       
+00005c30: 204e 2915 7224 0000 00da 0d5f 7072 6f6a   N).r$....._proj
+00005c40: 6563 745f 6e61 6d65 da0b 5f61 6e69 6d61  ect_name.._anima
+00005c50: 6c5f 6964 73da 065f 6172 656e 61da 0d5f  l_ids.._arena.._
+00005c60: 6172 656e 615f 7061 7261 6d73 da0b 5f61  arena_params.._a
+00005c70: 7265 6e61 5f64 696d 73da 0f5f 626f 6479  rena_dims.._body
+00005c80: 7061 7274 5f67 7261 7068 da09 5f65 7863  part_graph.._exc
+00005c90: 6c75 6465 64da 0f5f 6578 705f 636f 6e64  luded.._exp_cond
+00005ca0: 6974 696f 6e73 da0b 5f66 7261 6d65 5f72  itions.._frame_r
+00005cb0: 6174 65da 055f 7061 7468 da08 5f71 7561  ate.._path.._qua
+00005cc0: 6c69 7479 da07 5f73 6361 6c65 73da 075f  lity.._scales.._
+00005cd0: 7461 626c 6573 da13 5f74 7261 696e 6564  tables.._trained
+00005ce0: 5f6d 6f64 656c 5f70 6174 68da 075f 7669  _model_path.._vi
+00005cf0: 6465 6f73 da11 5f76 6964 656f 5f72 6573  deos.._video_res
+00005d00: 6f6c 7574 696f 6e72 7f00 0000 da06 5f61  olutionr......_a
+00005d10: 7265 6173 727b 0000 00da 0d5f 636f 6e6e  reasr{....._conn
+00005d20: 6563 7469 7669 7479 2916 7257 0000 0072  ectivity).rW...r
+00005d30: 1900 0000 723f 0000 0072 3500 0000 7260  ....r?...r5...r`
+00005d40: 0000 0072 3600 0000 721f 0000 0072 ae00  ...r6...r....r..
+00005d50: 0000 72f2 0000 0072 6800 0000 721b 0100  ..r....rh...r...
+00005d60: 0072 5e00 0000 721c 0100 0072 5d00 0000  .r^...r....r]...
+00005d70: 721d 0100 0072 6200 0000 7234 0000 0072  r....rb...r4...r
+00005d80: 6300 0000 7265 0000 0072 6400 0000 721a  c...re...rd...r.
+00005d90: 0100 0072 3900 0000 7227 0000 0072 2700  ...r9...r'...r'.
+00005da0: 0000 7228 0000 0072 6a00 0000 de02 0000  ..r(...rj.......
+00005db0: 732a 0000 0000 3106 0106 0106 0106 0106  s*....1.........
+00005dc0: 0106 0106 0106 0106 0106 0106 0106 0106  ................
+00005dd0: 0106 0106 0106 0106 0106 0106 0106 017a  ...............z
+00005de0: 1443 6f6f 7264 696e 6174 6573 2e5f 5f69  .Coordinates.__i
+00005df0: 6e69 745f 5f63 0100 0000 0000 0000 0000  nit__c..........
+00005e00: 0000 0100 0000 0400 0000 4300 0000 7310  ..........C...s.
+00005e10: 0000 0064 01a0 0074 017c 006a 0283 01a1  ...d...t.|.j....
+00005e20: 0153 0072 6b00 0000 a903 726d 0000 0072  .S.rk.....rm...r
+00005e30: 5f00 0000 723f 0100 0072 5600 0000 7227  _...r?...rV...r'
+00005e40: 0000 0072 2700 0000 7228 0000 0072 6e00  ...r'...r(...rn.
+00005e50: 0000 2503 0000 7302 0000 0000 027a 1343  ..%...s......z.C
+00005e60: 6f6f 7264 696e 6174 6573 2e5f 5f73 7472  oordinates.__str
+00005e70: 5f5f 6301 0000 0000 0000 0000 0000 0001  __c.............
+00005e80: 0000 0004 0000 0043 0000 0073 1000 0000  .......C...s....
+00005e90: 6401 a000 7401 7c00 6a02 8301 a101 5300  d...t.|.j.....S.
+00005ea0: 726b 0000 0072 4301 0000 7256 0000 0072  rk...rC...rV...r
+00005eb0: 2700 0000 7227 0000 0072 2800 0000 726f  '...r'...r(...ro
+00005ec0: 0000 0029 0300 0073 0200 0000 0002 7a14  ...)...s......z.
+00005ed0: 436f 6f72 6469 6e61 7465 732e 5f5f 7265  Coordinates.__re
+00005ee0: 7072 5f5f 4672 0100 0000 5429 09da 0663  pr__Fr....T)...c
+00005ef0: 656e 7465 72da 0570 6f6c 6172 da05 7370  enter..polar..sp
+00005f00: 6565 64da 0561 6c69 676e da0d 616c 6967  eed..align..alig
+00005f10: 6e5f 696e 706c 6163 65da 0b73 656c 6563  n_inplace..selec
+00005f20: 7465 645f 6964 da10 7072 6f70 6167 6174  ted_id..propagat
+00005f30: 655f 6c61 6265 6c73 da15 7072 6f70 6167  e_labels..propag
+00005f40: 6174 655f 616e 6e6f 7461 7469 6f6e 7372  ate_annotationsr
+00005f50: 1a00 0000 6309 0000 0000 0000 0000 0000  ....c...........
+00005f60: 001b 0000 000d 0000 0003 0000 0073 fe04  .............s..
+00005f70: 0000 7400 6a01 a002 7c00 6a03 a101 7d09  ..t.j...|.j...}.
+00005f80: 6401 5c02 7d0a 7d0b 7c00 6a04 7d0c 7c02  d.\.}.}.|.j.}.|.
+00005f90: 725a 6402 5c02 7d0a 7d0b 7400 6a01 a005  rZd.\.}.}.t.j...
+00005fa0: 7c0c a101 a006 a100 7d0c 7c09 a007 a100  |.......}.|.....
+00005fb0: 4400 5d18 5c02 7d0d 7d0e 7400 6a01 a008  D.].\.}.}.t.j...
+00005fc0: 7c0e a101 7c09 7c0d 3c00 7140 8802 6403  |...|.|.<.q@..d.
+00005fd0: 6b02 9001 7202 7409 7c09 a007 a100 8301  k...r.t.|.......
+00005fe0: 4400 5d8c 5c02 7d0f 5c02 7d0d 7d10 7c10  D.].\.}.\.}.}.|.
+00005ff0: 6a0a 6404 6404 8502 740b 6405 8301 7c0a  j.d.d...t.d...|.
+00006000: 6701 6602 6602 1900 7c0c 7c0f 1900 6406  g.f.f...|.|...d.
+00006010: 1900 1800 7c10 6a0a 6404 6404 8502 740b  ....|.j.d.d...t.
+00006020: 6405 8301 7c0a 6701 6602 6602 3c00 7c10  d...|.g.f.f.<.|.
+00006030: 6a0a 6404 6404 8502 740b 6405 8301 7c0b  j.d.d...t.d...|.
+00006040: 6701 6602 6602 1900 7c0c 7c0f 1900 6407  g.f.f...|.|...d.
+00006050: 1900 1800 7c10 6a0a 6404 6404 8502 740b  ....|.j.d.d...t.
+00006060: 6405 8301 7c0b 6701 6602 6602 3c00 7170  d...|.g.f.f.<.qp
+00006070: 9001 6e26 740c 8802 740d 8302 9002 7228  ..n&t...t.....r(
+00006080: 8802 6403 6b03 9002 7228 7409 7c09 a007  ..d.k...r(t.|...
+00006090: a100 8301 4400 9001 5d00 5c02 7d0f 5c02  ....D...].\.}.\.
+000060a0: 7d0d 7d10 7c00 6a0e 7d11 7c06 6404 7501  }.}.|.j.}.|.d.u.
+000060b0: 9001 7248 7c06 6701 7d11 7c11 4400 5dd6  ..rH|.g.}.|.D.].
+000060c0: 8900 7c10 a00f 7c10 6a0a 6404 6404 8502  ..|...|.j.d.d...
+000060d0: 8700 6601 6408 6409 8408 7c10 6a10 4400  ..f.d.d...|.j.D.
+000060e0: 8301 6602 1900 6a0a 6404 6404 8502 740b  ..f...j.d.d...t.
+000060f0: 6405 8301 7c0a 6701 6602 6602 1900 6a11  d...|.g.f.f...j.
+00006100: 7c10 8800 8800 640a 6b03 9001 72a0 640b  |.....d.k...r.d.
+00006110: 6e02 640a 1700 8802 1700 1900 7c0a 1900  n.d.........|...
+00006120: 6406 640c 8d02 a101 0100 7c10 a00f 7c10  d.d.......|...|.
+00006130: 6a0a 6404 6404 8502 8700 6601 640d 6409  j.d.d.....f.d.d.
+00006140: 8408 7c10 6a10 4400 8301 6602 1900 6a0a  ..|.j.D...f...j.
+00006150: 6404 6404 8502 740b 6405 8301 7c0b 6701  d.d...t.d...|.g.
+00006160: 6602 6602 1900 6a11 7c10 8800 8800 640a  f.f...j.|.....d.
+00006170: 6b03 9002 7208 640b 6e02 640a 1700 8802  k...r.d.n.d.....
+00006180: 1700 1900 7c0b 1900 6406 640c 8d02 a101  ....|...d.d.....
+00006190: 0100 9001 714c 9001 7124 8801 9003 72ac  ....qL..q$....r.
+000061a0: 7412 8702 6601 640e 640f 8408 7413 7c09  t...f.d.d...t.|.
+000061b0: a014 a100 8301 6406 1900 6a10 6a15 6406  ......d...j.j.d.
+000061c0: 1900 4400 8301 8301 9002 7362 4a00 6410  ..D.......sbJ.d.
+000061d0: 8301 8201 7412 8701 6601 6411 640f 8408  ....t...f.d.d...
+000061e0: 7413 7c09 a014 a100 8301 6406 1900 6a10  t.|.......d...j.
+000061f0: 6a15 6406 1900 4400 8301 8301 9002 7396  j.d...D.......s.
+00006200: 4a00 6412 8301 8201 7c09 a007 a100 4400  J.d.....|.....D.
+00006210: 9001 5d0a 5c02 7d0d 7d0e 7c0e 6a16 7d12  ..].\.}.}.|.j.}.
+00006220: 6700 7d13 6404 7d14 7c11 4400 5dd0 8900  g.}.d.}.|.D.]...
+00006230: 8700 8701 6602 6413 6409 8408 7c0e 6a10  ....f.d.d...|.j.
+00006240: 4400 8301 7d15 8800 8800 640a 6b03 9002  D...}.....d.k...
+00006250: 72e4 640b 6e02 640a 1700 8801 1700 7c02  r.d.n.d.......|.
+00006260: 9002 72f6 6414 6e02 6405 6602 8800 8800  ..r.d.n.d.f.....
+00006270: 640a 6b03 9003 720a 640b 6e02 640a 1700  d.k...r.d.n.d...
+00006280: 8801 1700 7c02 9003 721c 6415 6e02 6416  ....|...r.d.n.d.
+00006290: 6602 6702 7c15 1700 7d15 7c0e 7c15 1900  f.g.|...}.|.|...
+000062a0: 7d16 7c13 7c15 3700 7d13 7c05 9002 72ba  }.|.|.7.}.|...r.
+000062b0: 7c02 9002 73ba 7400 6a01 6a17 7418 a019  |...s.t.j.j.t...
+000062c0: 7c16 a101 6417 6418 8d02 7d16 6419 7c16  |...d.d...}.d.|.
+000062d0: 7418 a01a 7c16 a101 641a 6b00 3c00 741b  t...|...d.k.<.t.
+000062e0: a01c 7c16 a101 7d16 741b 6a1d 7c14 7c16  ..|...}.t.j.|.|.
+000062f0: 6702 6407 640c 8d02 7d14 9002 71ba 7c12  g.d.d...}...q.|.
+00006300: 7c14 5f16 741b 6a1e a01f 7c13 a101 7c14  |._.t.j...|...|.
+00006310: 5f10 7c14 7c09 7c0d 3c00 9002 719e 7c03  _.|.|.|.<...q.|.
+00006320: 9003 72e0 7c09 a007 a100 4400 5d24 5c02  ..r.|.....D.]$\.
+00006330: 7d0d 7d0e 7400 6a01 6a20 7c0e 7c03 8802  }.}.t.j.j |.|...
+00006340: 641b 8d03 7d17 7c17 7c09 7c0d 3c00 9003  d...}.|.|.|.<...
+00006350: 71ba 7c06 6404 7501 9004 7220 7c09 a007  q.|.d.u...r |...
+00006360: a100 4400 5d2c 5c02 7d0d 7d18 7c18 6a0a  ..D.],\.}.}.|.j.
+00006370: 6404 6404 8502 7400 6a01 a021 7c18 6a10  d.d...t.j..!|.j.
+00006380: 7c06 a102 6602 1900 7c09 7c0d 3c00 9003  |...f...|.|.<...
+00006390: 71f2 7400 6a01 a022 7c00 7c09 7c00 a023  q.t.j.."|.|.|..#
+000063a0: a100 a103 7d09 7c08 9004 7290 7413 7c08  ....}.|...r.t.|.
+000063b0: a014 a100 8301 6406 1900 6a10 7d19 7c09  ......d...j.}.|.
+000063c0: a007 a100 4400 5d3a 5c02 7d0d 7d0e 7c19  ....D.]:\.}.}.|.
+000063d0: 4400 5d2a 7d1a 7c08 7c0d 1900 6a0a 6404  D.]*}.|.|...j.d.
+000063e0: 6404 8502 7c1a 6602 1900 7c0e 6a0a 6404  d...|.f...|.j.d.
+000063f0: 6404 8502 7c1a 6602 3c00 9004 7160 9004  d...|.f.<...q`..
+00006400: 7154 7c07 9004 72d6 7c09 a007 a100 4400  qT|...r.|.....D.
+00006410: 5d36 5c02 7d0d 7d0e 7418 a024 7c00 6a25  ]6\.}.}.t..$|.j%
+00006420: 7c0d 1900 7c07 1900 6a14 7c0e 6a26 6406  |...|...j.|.j&d.
+00006430: 1900 a102 7c0e 6a0a 6404 6404 8502 641c  ....|.j.d.d...d.
+00006440: 6602 3c00 9004 719e 7427 7c09 641d 7c00  f.<...q.t'|.d.|.
+00006450: 6a0e 7c00 6a28 7c00 6a04 8802 7c00 6a29  j.|.j(|.j...|.j)
+00006460: 7c02 7c00 6a25 7c07 7c08 641e 8d0b 5300  |.|.j%|.|.d...S.
+00006470: 291f 6184 0500 0052 6574 7572 6e20 6120  ).a....Return a 
+00006480: 7461 626c 655f 6469 6374 206f 626a 6563  table_dict objec
+00006490: 7420 7769 7468 2074 6865 2063 6f6f 7264  t with the coord
+000064a0: 696e 6174 6573 206f 6620 6561 6368 2061  inates of each a
+000064b0: 6e69 6d61 6c20 6173 2076 616c 7565 732e  nimal as values.
+000064c0: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+000064d0: 2020 2020 2020 2020 2020 2020 6365 6e74              cent
+000064e0: 6572 2028 7374 7229 3a20 4e61 6d65 206f  er (str): Name o
+000064f0: 6620 7468 6520 626f 6479 2070 6172 7420  f the body part 
+00006500: 746f 2077 6869 6368 2074 6865 2070 6f73  to which the pos
+00006510: 6974 696f 6e73 2077 696c 6c20 6265 2063  itions will be c
+00006520: 656e 7465 7265 642e 2049 6620 6661 6c73  entered. If fals
+00006530: 652c 2074 6865 2072 6177 2064 6174 6120  e, the raw data 
+00006540: 6973 2072 6574 7572 6e65 643b 2069 6620  is returned; if 
+00006550: 2761 7265 6e61 2720 2864 6566 6175 6c74  'arena' (default
+00006560: 292c 2063 6f6f 7264 696e 6174 6573 2061  ), coordinates a
+00006570: 7265 2063 656e 7465 7265 6420 696e 2074  re centered in t
+00006580: 6865 2070 6974 6368 0a20 2020 2020 2020  he pitch.       
+00006590: 2020 2020 2070 6f6c 6172 2028 626f 6f6c       polar (bool
+000065a0: 2920 5374 6174 6573 2077 6865 7468 6572  ) States whether
+000065b0: 2074 6865 2063 6f6f 7264 696e 6174 6573   the coordinates
+000065c0: 2073 686f 756c 6420 6265 2063 6f6e 7665   should be conve
+000065d0: 7274 6564 2074 6f20 706f 6c61 7220 7661  rted to polar va
+000065e0: 6c75 6573 2e0a 2020 2020 2020 2020 2020  lues..          
+000065f0: 2020 7370 6565 6420 2869 6e74 293a 2053    speed (int): S
+00006600: 7461 7465 7320 7468 6520 6465 7269 7661  tates the deriva
+00006610: 7469 7665 206f 6620 7468 6520 706f 7369  tive of the posi
+00006620: 7469 6f6e 7320 746f 2072 6570 6f72 742e  tions to report.
+00006630: 2053 7065 6564 2069 7320 7265 7475 726e   Speed is return
+00006640: 6564 2069 6620 312c 2061 6363 656c 6572  ed if 1, acceler
+00006650: 6174 696f 6e20 6966 2032 2c20 6a65 726b  ation if 2, jerk
+00006660: 2069 6620 332c 2065 7463 2e0a 2020 2020   if 3, etc..    
+00006670: 2020 2020 2020 2020 616c 6967 6e20 2873          align (s
+00006680: 7472 293a 2053 656c 6563 7473 2074 6865  tr): Selects the
+00006690: 2062 6f64 7920 7061 7274 2074 6f20 7768   body part to wh
+000066a0: 6963 6820 6c61 7465 7220 7072 6f63 6573  ich later proces
+000066b0: 7365 7320 7769 6c6c 2061 6c69 676e 2074  ses will align t
+000066c0: 6865 2066 7261 6d65 7320 7769 7468 2028  he frames with (
+000066d0: 7365 6520 7072 6570 726f 6365 7373 2069  see preprocess i
+000066e0: 6e20 7461 626c 655f 6469 6374 2064 6f63  n table_dict doc
+000066f0: 756d 656e 7461 7469 6f6e 292e 0a20 2020  umentation)..   
+00006700: 2020 2020 2020 2020 2061 6c69 676e 5f69           align_i
+00006710: 6e70 6c61 6365 2028 626f 6f6c 293a 204f  nplace (bool): O
+00006720: 6e6c 7920 7661 6c69 6420 6966 2061 6c69  nly valid if ali
+00006730: 676e 2069 7320 7365 742e 2041 6c69 676e  gn is set. Align
+00006740: 7320 7468 6520 7665 6374 6f72 2074 6861  s the vector tha
+00006750: 7420 676f 6573 2066 726f 6d20 7468 6520  t goes from the 
+00006760: 6f72 6967 696e 2074 6f20 7468 6520 7365  origin to the se
+00006770: 6c65 6374 6564 2062 6f64 7920 7061 7274  lected body part
+00006780: 2077 6974 6820 7468 6520 792d 6178 6973   with the y-axis
+00006790: 2c20 666f 7220 616c 6c20 7469 6d65 706f  , for all timepo
+000067a0: 696e 7473 2028 6465 6661 756c 7429 2e0a  ints (default)..
+000067b0: 2020 2020 2020 2020 2020 2020 7365 6c65              sele
+000067c0: 6374 6564 5f69 6420 2873 7472 293a 2053  cted_id (str): S
+000067d0: 656c 6563 7473 2061 2073 696e 676c 6520  elects a single 
+000067e0: 616e 696d 616c 206f 6e20 6d75 6c74 6920  animal on multi 
+000067f0: 616e 696d 616c 2073 6574 7469 6e67 732e  animal settings.
+00006800: 2044 6566 6175 6c74 7320 746f 204e 6f6e   Defaults to Non
+00006810: 6520 2861 6c6c 2061 6e69 6d61 6c73 2061  e (all animals a
+00006820: 7265 2070 726f 6365 7373 6564 292e 0a20  re processed).. 
+00006830: 2020 2020 2020 2020 2020 2070 726f 7061             propa
+00006840: 6761 7465 5f6c 6162 656c 7320 2862 6f6f  gate_labels (boo
+00006850: 6c29 3a20 4966 2054 7275 652c 2061 6464  l): If True, add
+00006860: 7320 616e 2065 7874 7261 2066 6561 7475  s an extra featu
+00006870: 7265 2066 6f72 2065 6163 6820 7669 6465  re for each vide
+00006880: 6f20 636f 6e74 6169 6e69 6e67 2069 7473  o containing its
+00006890: 2070 6865 6e6f 7479 7069 6320 6c61 6265   phenotypic labe
+000068a0: 6c0a 2020 2020 2020 2020 2020 2020 7072  l.            pr
+000068b0: 6f70 6167 6174 655f 616e 6e6f 7461 7469  opagate_annotati
+000068c0: 6f6e 7320 2864 6963 7429 3a20 4966 2061  ons (dict): If a
+000068d0: 2064 6963 7469 6f6e 6172 7920 6973 2070   dictionary is p
+000068e0: 726f 7669 6465 642c 2073 7570 6572 7669  rovided, supervi
+000068f0: 7365 6420 616e 6e6f 7461 7469 6f6e 7320  sed annotations 
+00006900: 6172 6520 7072 6f70 6167 6174 6564 2074  are propagated t
+00006910: 6872 6f75 6768 2074 6865 2074 7261 696e  hrough the train
+00006920: 696e 6720 6461 7461 7365 742e 2054 6869  ing dataset. Thi
+00006930: 7320 6361 6e20 6265 2075 7365 6420 666f  s can be used fo
+00006940: 7220 7265 6775 6c61 7269 7369 6e67 2074  r regularising t
+00006950: 6865 206c 6174 656e 7420 7370 6163 6520  he latent space 
+00006960: 6261 7365 6420 6f6e 2061 6c72 6561 6479  based on already
+00006970: 206b 6e6f 776e 2074 7261 6974 732e 0a0a   known traits...
+00006980: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+00006990: 0a20 2020 2020 2020 2020 2020 2074 6162  .            tab
+000069a0: 6c65 5f64 6963 743a 2041 2074 6162 6c65  le_dict: A table
+000069b0: 5f64 6963 7420 6f62 6a65 6374 2063 6f6e  _dict object con
+000069c0: 7461 696e 696e 6720 7468 6520 636f 6f72  taining the coor
+000069d0: 6469 6e61 7465 7320 6f66 2065 6163 6820  dinates of each 
+000069e0: 616e 696d 616c 2061 7320 7661 6c75 6573  animal as values
+000069f0: 2e0a 0a20 2020 2020 2020 2029 0272 a600  ...        ).r..
+00006a00: 0000 72aa 0000 0029 02da 0372 686f da03  ..r....)...rho..
+00006a10: 7068 6972 3500 0000 4e72 a600 0000 7201  phir5...Nr....r.
+00006a20: 0000 0072 3200 0000 6301 0000 0000 0000  ...r2...c.......
+00006a30: 0000 0000 0002 0000 0005 0000 0013 0000  ................
+00006a40: 0073 1e00 0000 6700 7c00 5d16 7d01 7c01  .s....g.|.].}.|.
+00006a50: 6400 1900 a000 8800 a101 7204 7c01 9102  d.........r.|...
+00006a60: 7104 5300 72ef 0000 0072 4800 0000 724a  q.S.r....rH...rJ
+00006a70: 0000 0072 0901 0000 7227 0000 0072 2800  ...r....r'...r(.
+00006a80: 0000 724d 0000 006a 0300 0072 4e00 0000  ..rM...j...rN...
+00006a90: 7a2a 436f 6f72 6469 6e61 7465 732e 6765  z*Coordinates.ge
+00006aa0: 745f 636f 6f72 6473 2e3c 6c6f 6361 6c73  t_coords.<locals
+00006ab0: 3e2e 3c6c 6973 7463 6f6d 703e 722d 0000  >.<listcomp>r-..
+00006ac0: 0072 8d00 0000 72ac 0000 0063 0100 0000  .r....r....c....
+00006ad0: 0000 0000 0000 0000 0200 0000 0500 0000  ................
+00006ae0: 1300 0000 731e 0000 0067 007c 005d 167d  ....s....g.|.].}
+00006af0: 017c 0164 0019 00a0 0088 00a1 0172 047c  .|.d.........r.|
+00006b00: 0191 0271 0453 0072 ef00 0000 7248 0000  ...q.S.r....rH..
+00006b10: 0072 4a00 0000 7209 0100 0072 2700 0000  .rJ...r....r'...
+00006b20: 7228 0000 0072 4d00 0000 7403 0000 724e  r(...rM...t...rN
+00006b30: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00006b40: 0200 0000 0300 0000 3300 0000 7316 0000  ........3...s...
+00006b50: 007c 005d 0e7d 0188 007c 0176 0056 0001  .|.].}...|.v.V..
+00006b60: 0071 0264 0053 0072 2701 0000 7227 0000  .q.d.S.r'...r'..
+00006b70: 00a9 0272 4b00 0000 729b 0000 00a9 0172  ...rK...r......r
+00006b80: 4401 0000 7227 0000 0072 2800 0000 da09  D...r'...r(.....
+00006b90: 3c67 656e 6578 7072 3e7e 0300 0073 0200  <genexpr>~...s..
+00006ba0: 0000 0401 7a29 436f 6f72 6469 6e61 7465  ....z)Coordinate
+00006bb0: 732e 6765 745f 636f 6f72 6473 2e3c 6c6f  s.get_coords.<lo
+00006bc0: 6361 6c73 3e2e 3c67 656e 6578 7072 3e7a  cals>.<genexpr>z
+00006bd0: 3e66 6f72 2061 6c69 676e 2074 6f20 7275  >for align to ru
+00006be0: 6e2c 2063 656e 7465 7220 6d75 7374 2062  n, center must b
+00006bf0: 6520 7365 7420 746f 2074 6865 206e 616d  e set to the nam
+00006c00: 6520 6f66 2061 2062 6f64 7970 6172 7463  e of a bodypartc
+00006c10: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00006c20: 0300 0000 3300 0000 7316 0000 007c 005d  ....3...s....|.]
+00006c30: 0e7d 0188 007c 0176 0056 0001 0071 0264  .}...|.v.V...q.d
+00006c40: 0053 0072 2701 0000 7227 0000 0072 4e01  .S.r'...r'...rN.
+00006c50: 0000 2901 7247 0100 0072 2700 0000 7228  ..).rG...r'...r(
+00006c60: 0000 0072 5001 0000 8103 0000 7302 0000  ...rP.......s...
+00006c70: 0004 017a 2b61 6c69 676e 206d 7573 7420  ...z+align must 
+00006c80: 6265 2073 6574 2074 6f20 7468 6520 6e61  be set to the na
+00006c90: 6d65 206f 6620 6120 626f 6479 7061 7274  me of a bodypart
+00006ca0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00006cb0: 0005 0000 0013 0000 0073 2c00 0000 6700  .........s,...g.
+00006cc0: 7c00 5d24 7d01 7c01 6400 1900 a000 8801  |.]$}.|.d.......
+00006cd0: a101 7304 7c01 6400 1900 a001 8800 a101  ..s.|.d.........
+00006ce0: 7204 7c01 9102 7104 5300 72ef 0000 0072  r.|...q.S.r....r
+00006cf0: 5100 0000 724a 0000 0029 0272 9700 0000  Q...rJ...).r....
+00006d00: 7247 0100 0072 2700 0000 7228 0000 0072  rG...r'...r(...r
+00006d10: 4d00 0000 8d03 0000 7306 0000 0006 0202  M.......s.......
+00006d20: 011c fe72 4d01 0000 724c 0100 0072 aa00  ...rM...rL...r..
+00006d30: 0000 7258 0000 0029 0172 bb00 0000 72ad  ..rX...).r....r.
+00006d40: 0000 0067 f168 e388 b5f8 e43e 2902 da05  ...g.h.....>)...
+00006d50: 6465 7269 7672 4401 0000 da05 7068 656e  derivrD.....phen
+00006d60: 6f72 a700 0000 2909 7234 0000 0072 3500  or....).r4...r5.
+00006d70: 0000 7260 0000 0072 4401 0000 7264 0000  ..r`...rD...rd..
+00006d80: 0072 4501 0000 7239 0000 0072 4a01 0000  .rE...r9...rJ...
+00006d90: 724b 0100 0029 2a72 8200 0000 7283 0000  rK...)*r....r...
+00006da0: 00da 0864 6565 7063 6f70 7972 3d01 0000  ...deepcopyr=...
+00006db0: 723c 0100 00da 0862 7032 706f 6c61 72da  r<.....bp2polar.
+00006dc0: 0874 6f5f 6e75 6d70 7972 cc00 0000 da09  .to_numpyr......
+00006dd0: 7461 6232 706f 6c61 7272 f700 0000 72c4  tab2polarr....r.
+00006de0: 0000 00da 0573 6c69 6365 da0a 6973 696e  .....slice..isin
+00006df0: 7374 616e 6365 72a3 0000 0072 3201 0000  stancer....r2...
+00006e00: da06 7570 6461 7465 72b8 0000 00da 0873  ..updater......s
+00006e10: 7562 7472 6163 74da 0361 6e79 72b6 0000  ubtract..anyr...
+00006e20: 0072 c900 0000 72f0 0000 0072 ca00 0000  .r....r....r....
+00006e30: da12 616c 6967 6e5f 7472 616a 6563 746f  ..align_trajecto
+00006e40: 7269 6573 72de 0000 0072 df00 0000 da03  riesr....r......
+00006e50: 6162 7372 bf00 0000 72dc 0000 0072 d800  absr....r....r..
+00006e60: 0000 72ce 0000 00da 0b66 726f 6d5f 7475  ..r......from_tu
+00006e70: 706c 6573 da0d 726f 6c6c 696e 675f 7370  ples..rolling_sp
+00006e80: 6565 6472 0f01 0000 72e2 0000 00da 0b67  eedr....r......g
+00006e90: 6574 5f71 7561 6c69 7479 da06 7265 7065  et_quality..repe
+00006ea0: 6174 7238 0100 0072 d500 0000 72db 0000  atr8...r....r...
+00006eb0: 0072 3301 0000 7242 0100 0029 1b72 5700  .r3...rB...).rW.
+00006ec0: 0000 7244 0100 0072 4501 0000 7246 0100  ..rD...rE...rF..
+00006ed0: 0072 4701 0000 7248 0100 0072 4901 0000  .rG...rH...rI...
+00006ee0: 724a 0100 0072 4b01 0000 da04 7461 6273  rJ...rK.....tabs
+00006ef0: da07 636f 6f72 645f 31da 0763 6f6f 7264  ..coord_1..coord
+00006f00: 5f32 72f2 0000 0072 e600 0000 7255 0000  _2r....r....rU..
+00006f10: 0072 4c00 0000 7229 0100 0072 3400 0000  .rL...r)...r4...
+00006f20: da09 616c 6c5f 696e 6465 78da 0b61 6c6c  ..all_index..all
+00006f30: 5f63 6f6c 756d 6e73 da13 616c 6967 6e65  _columns..aligne
+00006f40: 645f 636f 6f72 6469 6e61 7465 7372 b800  d_coordinatesr..
+00006f50: 0000 da0f 7061 7274 6961 6c5f 616c 6967  ....partial_alig
+00006f60: 6e65 64da 0376 656c 72f9 0000 00da 0b61  ned..velr......a
+00006f70: 6e6e 6f74 6174 696f 6e73 da03 616e 6e72  nnotations..annr
+00006f80: 2700 0000 2903 7297 0000 0072 4701 0000  '...).r....rG...
+00006f90: 7244 0100 0072 2800 0000 da0a 6765 745f  rD...r(.....get_
+00006fa0: 636f 6f72 6473 2d03 0000 73de 0000 0000  coords-...s.....
+00006fb0: 1b0e 0108 0106 0204 0108 0110 0110 0112  ................
+00006fc0: 020a 0218 0326 ff1a 0526 ff20 0416 021a  .....&...&. ....
+00006fd0: 0306 010a 0106 0208 0204 0122 0114 ff04  ..........."....
+00006fe0: 0320 0102 fc04 ff04 0a04 0122 0114 ff04  . ........."....
+00006ff0: 0320 0102 fc04 ff0c 0906 020c 0116 ff0c  . ..............
+00007000: 0202 fe04 030c 0116 ff0c 0202 fe04 0412  ................
+00007010: 0206 0104 0104 0208 020c 0204 fe06 0718  ................
+00007020: 010c fe02 0518 010c fe02 fb02 0902 f704  ................
+00007030: 0b08 0108 020c 0106 010a ff06 0312 010a  ................
+00007040: 0104 0108 ff0a 0406 010e 010c 0206 0110  ................
+00007050: 0112 010c 030a 0110 0104 0116 ff0c 0514  ................
+00007060: 0206 0112 0210 0108 012c 0206 0110 0104  .........,......
+00007070: 0116 ff16 0402 0102 0102 0104 0104 0104  ................
+00007080: 0102 0104 0102 0104 0102 0102 f57a 1643  .............z.C
+00007090: 6f6f 7264 696e 6174 6573 2e67 6574 5f63  oordinates.get_c
+000070a0: 6f6f 7264 7329 0672 4601 0000 7249 0100  oords).rF...rI..
+000070b0: 00da 0f66 696c 7465 725f 6f6e 5f67 7261  ...filter_on_gra
+000070c0: 7068 724a 0100 0072 4b01 0000 721a 0000  phrJ...rK...r...
+000070d0: 0063 0600 0000 0000 0000 0000 0000 0d00  .c..............
+000070e0: 0000 0a00 0000 4300 0000 73aa 0100 0074  ......C...s....t
+000070f0: 006a 01a0 027c 006a 03a1 017d 067c 006a  .j...|.j...}.|.j
+00007100: 0364 0175 0190 0172 9e7c 0172 4e7c 06a0  .d.u...r.|.rN|..
+00007110: 04a1 0044 005d 265c 027d 077d 0874 006a  ...D.]&\.}.}.t.j
+00007120: 016a 057c 087c 0164 0217 0064 0364 048d  .j.|.|.d...d.d..
+00007130: 037d 097c 097c 067c 073c 0071 267c 0264  .}.|.|.|.<.q&|.d
+00007140: 0175 0172 8a7c 06a0 04a1 0044 005d 2a5c  .u.r.|.....D.]*\
+00007150: 027d 077d 0a7c 0a6a 0664 0164 0185 0274  .}.}.|.j.d.d...t
+00007160: 006a 01a0 077c 0a6a 087c 02a1 0266 0219  .j...|.j.|...f..
+00007170: 007c 067c 073c 0071 5e74 006a 01a0 097c  .|.|.<.q^t.j...|
+00007180: 007c 067c 00a0 0aa1 00a1 037d 067c 0472  .|.|.......}.|.r
+00007190: cc7c 06a0 04a1 0044 005d 205c 027d 077d  .|.....D.] \.}.}
+000071a0: 087c 006a 0b7c 0719 007c 086a 0664 0164  .|.j.|...|.j.d.d
+000071b0: 0185 0264 0566 023c 0071 aa7c 0590 0172  ...d.f.<.q.|...r
+000071c0: 2474 0c7c 05a0 0da1 0083 0164 0619 006a  $t.|.......d...j
+000071d0: 087d 0b7c 06a0 04a1 0044 005d 365c 027d  .}.|.....D.]6\.}
+000071e0: 077d 087c 0b44 005d 287d 0c7c 057c 0719  .}.|.D.](}.|.|..
+000071f0: 006a 0664 0164 0185 027c 0c66 0219 007c  .j.d.d...|.f...|
+00007200: 086a 0664 0164 0185 027c 0c66 023c 0071  .j.d.d...|.f.<.q
+00007210: f871 ec7c 0390 0172 827c 06a0 04a1 0044  .q.|...r.|.....D
+00007220: 005d 4e5c 027d 077d 087c 086a 0664 0164  .]N\.}.}.|.j.d.d
+00007230: 0185 0274 0c74 0e64 0764 0884 0074 006a  ...t.t.d.d...t.j
+00007240: 016a 0f7c 006a 107c 006a 1164 098d 026a  .j.|.j.|.j.d...j
+00007250: 1244 0083 0183 0174 0e7c 086a 0883 0140  .D.....t.|.j...@
+00007260: 0083 0166 0219 007c 067c 073c 0090 0171  ...f...|.|.<...q
+00007270: 3274 137c 067c 006a 107c 006a 147c 006a  2t.|.|.j.|.j.|.j
+00007280: 0b7c 047c 0564 0364 0a8d 0753 0074 1564  .|.|.d.d...S.t.d
+00007290: 0b83 0182 0164 0153 0029 0c61 d302 0000  .....d.S.).a....
+000072a0: 5265 7475 726e 2061 2074 6162 6c65 5f64  Return a table_d
+000072b0: 6963 7420 6f62 6a65 6374 2077 6974 6820  ict object with 
+000072c0: 7468 6520 6469 7374 616e 6365 7320 6265  the distances be
+000072d0: 7477 6565 6e20 626f 6479 2070 6172 7473  tween body parts
+000072e0: 2061 6e69 6d61 6c20 6173 2076 616c 7565   animal as value
+000072f0: 732e 0a0a 2020 2020 2020 2020 4172 6773  s...        Args
+00007300: 3a0a 2020 2020 2020 2020 2020 2020 7370  :.            sp
+00007310: 6565 6420 2869 6e74 293a 2054 6865 2064  eed (int): The d
+00007320: 6572 6976 6174 6976 6520 746f 2075 7365  erivative to use
+00007330: 2066 6f72 2073 7065 6564 2e0a 2020 2020   for speed..    
+00007340: 2020 2020 2020 2020 7365 6c65 6374 6564          selected
+00007350: 5f69 6420 2873 7472 293a 2054 6865 2069  _id (str): The i
+00007360: 6420 6f66 2074 6865 2061 6e69 6d61 6c20  d of the animal 
+00007370: 746f 2073 656c 6563 742e 0a20 2020 2020  to select..     
+00007380: 2020 2020 2020 2066 696c 7465 725f 6f6e         filter_on
+00007390: 5f67 7261 7068 2028 626f 6f6c 293a 2049  _graph (bool): I
+000073a0: 6620 5472 7565 2c20 6f6e 6c79 2064 6973  f True, only dis
+000073b0: 7461 6e63 6573 2062 6574 7765 656e 2063  tances between c
+000073c0: 6f6e 6e65 6374 6564 206e 6f64 6573 2069  onnected nodes i
+000073d0: 6e20 7468 6520 4465 6570 4f46 2067 7261  n the DeepOF gra
+000073e0: 7068 2072 6570 7265 7365 6e74 6174 696f  ph representatio
+000073f0: 6e73 2061 7265 206b 6570 742e 204f 7468  ns are kept. Oth
+00007400: 6572 7769 7365 2c20 616c 6c20 6469 7374  erwise, all dist
+00007410: 616e 6365 7320 6265 7477 6565 6e20 626f  ances between bo
+00007420: 6479 7061 7274 7320 6172 6520 7265 7475  dyparts are retu
+00007430: 726e 6564 2e0a 2020 2020 2020 2020 2020  rned..          
+00007440: 2020 7072 6f70 6167 6174 655f 6c61 6265    propagate_labe
+00007450: 6c73 2028 626f 6f6c 293a 2049 6620 5472  ls (bool): If Tr
+00007460: 7565 2c20 7468 6520 7068 656e 6f20 636f  ue, the pheno co
+00007470: 6c75 6d6e 2077 696c 6c20 6265 2070 726f  lumn will be pro
+00007480: 7061 6761 7465 6420 6672 6f6d 2074 6865  pagated from the
+00007490: 206f 7269 6769 6e61 6c20 6461 7461 2e0a   original data..
+000074a0: 2020 2020 2020 2020 2020 2020 7072 6f70              prop
+000074b0: 6167 6174 655f 616e 6e6f 7461 7469 6f6e  agate_annotation
+000074c0: 7320 2844 6963 7429 3a20 4120 6469 6374  s (Dict): A dict
+000074d0: 696f 6e61 7279 206f 6620 616e 6e6f 7461  ionary of annota
+000074e0: 7469 6f6e 7320 746f 2070 726f 7061 6761  tions to propaga
+000074f0: 7465 2e0a 0a20 2020 2020 2020 2052 6574  te...        Ret
+00007500: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
+00007510: 2020 7461 626c 655f 6469 6374 3a20 4120    table_dict: A 
+00007520: 7461 626c 655f 6469 6374 206f 626a 6563  table_dict objec
+00007530: 7420 7769 7468 2074 6865 2064 6973 7461  t with the dista
+00007540: 6e63 6573 2062 6574 7765 656e 2062 6f64  nces between bod
+00007550: 7920 7061 7274 7320 616e 696d 616c 2061  y parts animal a
+00007560: 7320 7661 6c75 6573 2e0a 0a20 2020 2020  s values...     
+00007570: 2020 204e 7232 0000 00da 0564 6973 7473     Nr2.....dists
+00007580: a902 7251 0100 0072 b000 0000 7252 0100  ..rQ...r....rR..
+00007590: 0072 0100 0000 6301 0000 0000 0000 0000  .r....c.........
+000075a0: 0000 0002 0000 0005 0000 0053 0000 0073  ...........S...s
+000075b0: 1800 0000 6700 7c00 5d10 7d01 7400 7401  ....g.|.].}.t.t.
+000075c0: 7c01 8301 8301 9102 7104 5300 7227 0000  |.......q.S.r'..
+000075d0: 00a9 0272 d200 0000 725c 0000 00a9 0272  ...r....r\.....r
+000075e0: 4b00 0000 da01 6572 2700 0000 7227 0000  K.....er'...r'..
+000075f0: 0072 2800 0000 724d 0000 0011 0400 0073  .r(...rM.......s
+00007600: 0400 0000 0602 02ff 7a2d 436f 6f72 6469  ........z-Coordi
+00007610: 6e61 7465 732e 6765 745f 6469 7374 616e  nates.get_distan
+00007620: 6365 732e 3c6c 6f63 616c 733e 2e3c 6c69  ces.<locals>.<li
+00007630: 7374 636f 6d70 3e29 0272 3400 0000 7294  stcomp>).r4...r.
+00007640: 0000 00a9 0672 3400 0000 7264 0000 0072  .....r4...rd...r
+00007650: 3900 0000 724a 0100 0072 4b01 0000 72b0  9...rJ...rK...r.
+00007660: 0000 007a 3f44 6973 7461 6e63 6573 206e  ...z?Distances n
+00007670: 6f74 2063 6f6d 7075 7465 642e 2052 6561  ot computed. Rea
+00007680: 6420 7468 6520 646f 6375 6d65 6e74 6174  d the documentat
+00007690: 696f 6e20 666f 7220 6d6f 7265 2064 6574  ion for more det
+000076a0: 6169 6c73 2916 7282 0000 0072 8300 0000  ails).r....r....
+000076b0: 7253 0100 0072 7b00 0000 72cc 0000 0072  rS...r{...r....r
+000076c0: 5f01 0000 72c4 0000 0072 0f01 0000 72b8  _...r....r....r.
+000076d0: 0000 0072 e200 0000 7260 0100 0072 3801  ...r....r`...r8.
+000076e0: 0000 72b6 0000 0072 c900 0000 72b7 0000  ..r....r....r...
+000076f0: 0072 9500 0000 7232 0100 0072 3601 0000  .r....r2...r6...
+00007700: da05 6564 6765 7372 db00 0000 7242 0100  ..edgesr....rB..
+00007710: 00da 0a56 616c 7565 4572 726f 7229 0d72  ...ValueError).r
+00007720: 5700 0000 7246 0100 0072 4901 0000 726d  W...rF...rI...rm
+00007730: 0100 0072 4a01 0000 724b 0100 0072 6201  ...rJ...rK...rb.
+00007740: 0000 72e6 0000 0072 5500 0000 7269 0100  ..r....rU...ri..
+00007750: 0072 f900 0000 726a 0100 0072 6b01 0000  .r....rj...rk...
+00007760: 7227 0000 0072 2700 0000 7228 0000 0072  r'...r'...r(...r
+00007770: fa00 0000 d803 0000 7364 0000 0000 150e  ........sd......
+00007780: 020c 0204 0110 0116 010a 0208 0110 0104  ................
+00007790: 0116 ff0a 0514 0204 0110 011a 0206 0112  ................
+000077a0: 0210 0108 0128 0206 0210 0104 0106 0102  .....(..........
+000077b0: 0102 0106 0206 0104 0104 fe06 fe04 ff02  ................
+000077c0: 0908 f702 ff02 ff02 ff0c 1002 0102 0104  ................
+000077d0: 0104 0104 0102 0102 0102 f906 0a02 0102  ................
+000077e0: ff7a 1943 6f6f 7264 696e 6174 6573 2e67  .z.Coordinates.g
+000077f0: 6574 5f64 6973 7461 6e63 6573 2906 da07  et_distances)...
+00007800: 6465 6772 6565 7372 4601 0000 7249 0100  degreesrF...rI..
+00007810: 0072 4a01 0000 724b 0100 0072 1a00 0000  .rJ...rK...r....
+00007820: 6306 0000 0000 0000 0000 0000 000d 0000  c...............
+00007830: 0009 0000 0043 0000 0073 5a01 0000 7400  .....C...sZ...t.
+00007840: 6a01 a002 7c00 6a03 a101 7d06 7c00 6a03  j...|.j...}.|.j.
+00007850: 6401 7501 9001 724e 7c01 7230 6402 6403  d.u...rN|.r0d.d.
+00007860: 8400 7c06 a004 a100 4400 8301 7d06 7c02  ..|.....D...}.|.
+00007870: 7264 7c06 a004 a100 4400 5d26 5c02 7d07  rd|.....D.]&\.}.
+00007880: 7d08 7400 6a01 6a05 7c08 7c02 6404 1700  }.t.j.j.|.|.d...
+00007890: 6405 6406 8d03 7d09 7c09 7c06 7c07 3c00  d.d...}.|.|.|.<.
+000078a0: 713c 7c03 6401 7501 72a0 7c06 a004 a100  q<|.d.u.r.|.....
+000078b0: 4400 5d2a 5c02 7d07 7d0a 7c0a 6a06 6401  D.]*\.}.}.|.j.d.
+000078c0: 6401 8502 7400 6a01 a007 7c0a 6a08 7c03  d...t.j...|.j.|.
+000078d0: a102 6602 1900 7c06 7c07 3c00 7174 7400  ..f...|.|.<.qtt.
+000078e0: 6a01 a009 7c00 7c06 7c00 a00a a100 a103  j...|.|.|.......
+000078f0: 7d06 7c04 72d8 7c06 a004 a100 4400 5d16  }.|.r.|.....D.].
+00007900: 5c02 7d07 7d08 7c00 6a0b 7c07 1900 7c08  \.}.}.|.j.|...|.
+00007910: 6407 3c00 71c0 7c05 9001 7232 740c 7c05  d.<.q.|...r2t.|.
+00007920: a00d a100 8301 6408 1900 6a08 7d0b 7c06  ......d...j.}.|.
+00007930: a004 a100 4400 5d38 5c02 7d07 7d08 7c0b  ....D.]8\.}.}.|.
+00007940: 4400 5d2a 7d0c 7c05 7c07 1900 6a06 6401  D.]*}.|.|...j.d.
+00007950: 6401 8502 7c0c 6602 1900 7c08 6a06 6401  d...|.f...|.j.d.
+00007960: 6401 8502 7c0c 6602 3c00 9001 7104 71f8  d...|.f.<...q.q.
+00007970: 740e 7c06 7c00 6a0f 7c00 6a10 7c00 6a0b  t.|.|.j.|.j.|.j.
+00007980: 7c04 7c05 6405 6409 8d07 5300 7411 640a  |.|.d.d...S.t.d.
+00007990: 8301 8201 6401 5300 290b 618d 0200 0052  ....d.S.).a....R
+000079a0: 6574 7572 6e20 6120 7461 626c 655f 6469  eturn a table_di
+000079b0: 6374 206f 626a 6563 7420 7769 7468 2074  ct object with t
+000079c0: 6865 2061 6e67 6c65 7320 6265 7477 6565  he angles betwee
+000079d0: 6e20 626f 6479 2070 6172 7473 2061 6e69  n body parts ani
+000079e0: 6d61 6c20 6173 2076 616c 7565 732e 0a0a  mal as values...
+000079f0: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+00007a00: 2020 2020 2020 2020 2020 6465 6772 6565            degree
+00007a10: 7320 2862 6f6f 6c29 3a20 4966 2054 7275  s (bool): If Tru
+00007a20: 6520 2864 6566 6175 6c74 292c 2074 6865  e (default), the
+00007a30: 2061 6e67 6c65 7320 7769 6c6c 2062 6520   angles will be 
+00007a40: 696e 2064 6567 7265 6573 2e20 4f74 6865  in degrees. Othe
+00007a50: 7277 6973 6520 7468 6579 2077 696c 6c20  rwise they will 
+00007a60: 6265 2063 6f6e 7665 7274 6564 2074 6f20  be converted to 
+00007a70: 7261 6469 616e 732e 0a20 2020 2020 2020  radians..       
+00007a80: 2020 2020 2073 7065 6564 2028 696e 7429       speed (int)
+00007a90: 3a20 5468 6520 6465 7269 7661 7469 7665  : The derivative
+00007aa0: 2074 6f20 7573 6520 666f 7220 7370 6565   to use for spee
+00007ab0: 642e 0a20 2020 2020 2020 2020 2020 2073  d..            s
+00007ac0: 656c 6563 7465 645f 6964 2028 7374 7229  elected_id (str)
+00007ad0: 3a20 5468 6520 6964 206f 6620 7468 6520  : The id of the 
+00007ae0: 616e 696d 616c 2074 6f20 7365 6c65 6374  animal to select
+00007af0: 2e0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
+00007b00: 6f70 6167 6174 655f 6c61 6265 6c73 2028  opagate_labels (
+00007b10: 626f 6f6c 293a 2049 6620 5472 7565 2c20  bool): If True, 
+00007b20: 7468 6520 7068 656e 6f20 636f 6c75 6d6e  the pheno column
+00007b30: 2077 696c 6c20 6265 2070 726f 7061 6761   will be propaga
+00007b40: 7465 6420 6672 6f6d 2074 6865 206f 7269  ted from the ori
+00007b50: 6769 6e61 6c20 6461 7461 2e0a 2020 2020  ginal data..    
+00007b60: 2020 2020 2020 2020 7072 6f70 6167 6174          propagat
+00007b70: 655f 616e 6e6f 7461 7469 6f6e 7320 2844  e_annotations (D
+00007b80: 6963 7429 3a20 4120 6469 6374 696f 6e61  ict): A dictiona
+00007b90: 7279 206f 6620 616e 6e6f 7461 7469 6f6e  ry of annotation
+00007ba0: 7320 746f 2070 726f 7061 6761 7465 2e0a  s to propagate..
+00007bb0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00007bc0: 3a0a 2020 2020 2020 2020 2020 2020 7461  :.            ta
+00007bd0: 626c 655f 6469 6374 3a20 4120 7461 626c  ble_dict: A tabl
+00007be0: 655f 6469 6374 206f 626a 6563 7420 7769  e_dict object wi
+00007bf0: 7468 2074 6865 2061 6e67 6c65 7320 6265  th the angles be
+00007c00: 7477 6565 6e20 626f 6479 2070 6172 7473  tween body parts
+00007c10: 2061 6e69 6d61 6c20 6173 2076 616c 7565   animal as value
+00007c20: 732e 0a0a 2020 2020 2020 2020 4e63 0100  s...        Nc..
+00007c30: 0000 0000 0000 0000 0000 0300 0000 0600  ................
+00007c40: 0000 5300 0000 731c 0000 0069 007c 005d  ..S...s....i.|.]
+00007c50: 145c 027d 017d 027c 0174 00a0 017c 02a1  .\.}.}.|.t...|..
+00007c60: 0193 0271 0453 0072 2700 0000 2902 72de  ...q.S.r'...).r.
+00007c70: 0000 0072 7601 0000 2903 724b 0000 0072  ...rv...).rK...r
+00007c80: e600 0000 7255 0000 0072 2700 0000 7227  ....rU...r'...r'
+00007c90: 0000 0072 2800 0000 7298 0000 0044 0400  ...r(...r....D..
+00007ca0: 0072 4e00 0000 7a2a 436f 6f72 6469 6e61  .rN...z*Coordina
+00007cb0: 7465 732e 6765 745f 616e 676c 6573 2e3c  tes.get_angles.<
+00007cc0: 6c6f 6361 6c73 3e2e 3c64 6963 7463 6f6d  locals>.<dictcom
+00007cd0: 703e 7232 0000 0072 6200 0000 726f 0100  p>r2...rb...ro..
+00007ce0: 0072 5201 0000 7201 0000 0072 7301 0000  .rR...r....rs...
+00007cf0: 7a3c 416e 676c 6573 206e 6f74 2063 6f6d  z<Angles not com
+00007d00: 7075 7465 642e 2052 6561 6420 7468 6520  puted. Read the 
+00007d10: 646f 6375 6d65 6e74 6174 696f 6e20 666f  documentation fo
+00007d20: 7220 6d6f 7265 2064 6574 6169 6c73 2912  r more details).
+00007d30: 7282 0000 0072 8300 0000 7253 0100 0072  r....r....rS...r
+00007d40: 7f00 0000 72cc 0000 0072 5f01 0000 72c4  ....r....r_...r.
+00007d50: 0000 0072 0f01 0000 72b8 0000 0072 e200  ...r....r....r..
+00007d60: 0000 7260 0100 0072 3801 0000 72b6 0000  ..r`...r8...r...
+00007d70: 0072 c900 0000 72db 0000 0072 3201 0000  .r....r....r2...
+00007d80: 7242 0100 0072 7501 0000 290d 7257 0000  rB...ru...).rW..
+00007d90: 0072 7601 0000 7246 0100 0072 4901 0000  .rv...rF...rI...
+00007da0: 724a 0100 0072 4b01 0000 7262 0100 0072  rJ...rK...rb...r
+00007db0: e600 0000 7255 0000 0072 6901 0000 72f9  ....rU...ri...r.
+00007dc0: 0000 0072 6a01 0000 726b 0100 0072 2700  ...rj...rk...r'.
+00007dd0: 0000 7227 0000 0072 2800 0000 7205 0100  ..r'...r(...r...
+00007de0: 002b 0400 0073 4400 0000 0015 0e02 0c01  .+...sD.........
+00007df0: 0401 1202 0401 1001 1601 0a02 0801 1001  ................
+00007e00: 0401 16ff 0a05 1402 0401 1001 1002 0601  ................
+00007e10: 1202 1001 0801 2a02 0201 0201 0401 0401  ......*.........
+00007e20: 0401 0201 0201 02f9 060a 0201 02ff 7a16  ..............z.
+00007e30: 436f 6f72 6469 6e61 7465 732e 6765 745f  Coordinates.get_
+00007e40: 616e 676c 6573 7258 0000 0029 0372 4601  anglesrX...).rF.
+00007e50: 0000 7249 0100 0072 1a00 0000 6303 0000  ..rI...r....c...
+00007e60: 0000 0000 0000 0000 000c 0000 0008 0000  ................
+00007e70: 0043 0000 0073 0601 0000 7400 6a01 a002  .C...s....t.j...
+00007e80: 7c00 6a03 a101 7d03 7c00 6a03 6401 7501  |.j...}.|.j.d.u.
+00007e90: 72fa 7c02 6402 6b02 7228 7c00 6a04 7d04  r.|.d.k.r(|.j.}.
+00007ea0: 6e06 7c02 6701 7d04 7c03 a005 a100 4400  n.|.g.}.|.....D.
+00007eb0: 5d5e 5c02 7d05 7d06 7406 a007 a100 7d07  ]^\.}.}.t.....}.
+00007ec0: 7c04 4400 5d40 7d08 7c08 6403 6b02 725a  |.D.]@}.|.d.k.rZ
+00007ed0: 6401 7d08 7c06 6a08 6401 6401 8502 7400  d.}.|.j.d.d...t.
+00007ee0: 6a01 a009 7c06 6a0a 7c08 a102 6602 1900  j...|.j.|...f...
+00007ef0: 7d09 7406 6a0b 7c07 7c09 6702 6404 6405  }.t.j.|.|.g.d.d.
+00007f00: 8d02 7d07 714a 7c07 7c03 7c05 3c00 7136  ..}.qJ|.|.|.<.q6
+00007f10: 7c01 72ca 7c03 a005 a100 4400 5d26 5c02  |.r.|.....D.]&\.
+00007f20: 7d05 7d06 7400 6a01 6a0c 7c06 7c01 6404  }.}.t.j.j.|.|.d.
+00007f30: 1700 6406 6407 8d03 7d0a 7c0a 7c03 7c05  ..d.d...}.|.|.|.
+00007f40: 3c00 71a2 7400 6a01 a00d 7c00 7c03 7c00  <.q.t.j...|.|.|.
+00007f50: a00e a100 a103 7d03 740f 7c03 7c00 6a04  ......}.t.|.|.j.
+00007f60: 7c00 6a10 6408 7c00 6a11 6409 8d05 7d0b  |.j.d.|.j.d...}.
+00007f70: 7c0b 5300 7412 640a 8301 8201 6401 5300  |.S.t.d.....d.S.
+00007f80: 290b 61e5 0100 0052 6574 7572 6e20 6120  ).a....Return a 
+00007f90: 7461 626c 655f 6469 6374 206f 626a 6563  table_dict objec
+00007fa0: 7420 7769 7468 2061 6c6c 2072 656c 6576  t with all relev
+00007fb0: 616e 7420 6172 6561 7320 2868 6561 642c  ant areas (head,
+00007fc0: 2074 6f72 736f 2c20 6261 636b 2c20 6675   torso, back, fu
+00007fd0: 6c6c 292e 2055 6e6c 6573 7320 7370 6563  ll). Unless spec
+00007fe0: 6966 6965 6420 6f74 6865 7277 6973 652c  ified otherwise,
+00007ff0: 2074 6865 2061 7265 6173 2061 7265 2063   the areas are c
+00008000: 6f6d 7075 7465 6420 666f 7220 616c 6c20  omputed for all 
+00008010: 616e 696d 616c 732e 0a0a 2020 2020 2020  animals...      
+00008020: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+00008030: 2020 2020 7370 6565 6420 2869 6e74 293a      speed (int):
+00008040: 2054 6865 2064 6572 6976 6174 6976 6520   The derivative 
+00008050: 746f 2075 7365 2066 6f72 2073 7065 6564  to use for speed
+00008060: 2e0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00008070: 6c65 6374 6564 5f69 6420 2873 7472 293a  lected_id (str):
+00008080: 2054 6865 2069 6420 6f66 2074 6865 2061   The id of the a
+00008090: 6e69 6d61 6c20 746f 2073 656c 6563 742e  nimal to select.
+000080a0: 2022 616c 6c22 2028 6465 6661 756c 7429   "all" (default)
+000080b0: 2063 6f6d 7075 7465 7320 7468 6520 6172   computes the ar
+000080c0: 6561 7320 666f 7220 616c 6c20 616e 696d  eas for all anim
+000080d0: 616c 732e 2044 6563 6c61 7265 6420 696e  als. Declared in
+000080e0: 2073 656c 662e 5f61 6e69 6d61 6c5f 6964   self._animal_id
+000080f0: 732e 0a0a 2020 2020 2020 2020 5265 7475  s...        Retu
+00008100: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+00008110: 2074 6162 6c65 5f64 6963 743a 2041 2074   table_dict: A t
+00008120: 6162 6c65 5f64 6963 7420 6f62 6a65 6374  able_dict object
+00008130: 2077 6974 6820 7468 6520 6172 6561 7320   with the areas 
+00008140: 6f66 2074 6865 2062 6f64 7920 7061 7274  of the body part
+00008150: 7320 616e 696d 616c 2061 7320 7661 6c75  s animal as valu
+00008160: 6573 2e0a 2020 2020 2020 2020 4e72 5800  es..        NrX.
+00008170: 0000 722d 0000 0072 3200 0000 72ac 0000  ..r-...r2...r...
+00008180: 0072 6200 0000 726f 0100 0072 6300 0000  .rb...ro...rc...
+00008190: 2904 7234 0000 0072 6400 0000 72b0 0000  ).r4...rd...r...
+000081a0: 0072 3900 0000 7a3b 4172 6561 7320 6e6f  .r9...z;Areas no
+000081b0: 7420 636f 6d70 7574 6564 2e20 5265 6164  t computed. Read
+000081c0: 2074 6865 2064 6f63 756d 656e 7461 7469   the documentati
+000081d0: 6f6e 2066 6f72 206d 6f72 6520 6465 7461  on for more deta
+000081e0: 696c 7329 1372 8200 0000 7283 0000 0072  ils).r....r....r
+000081f0: 5301 0000 7241 0100 0072 3201 0000 72cc  S...rA...r2...r.
+00008200: 0000 0072 bf00 0000 72dc 0000 0072 c400  ...r....r....r..
+00008210: 0000 720f 0100 0072 b800 0000 72d8 0000  ..r....r....r...
+00008220: 0072 5f01 0000 72e2 0000 0072 6001 0000  .r_...r....r`...
+00008230: 72db 0000 0072 4201 0000 7238 0100 0072  r....rB...r8...r
+00008240: 7501 0000 290c 7257 0000 0072 4601 0000  u...).rW...rF...
+00008250: 7249 0100 0072 6201 0000 da0c 7365 6c65  rI...rb.....sele
+00008260: 6374 6564 5f69 6473 72e6 0000 0072 5500  cted_idsr....rU.
+00008270: 0000 7216 0100 0072 9700 0000 7217 0100  ..r....r....r...
+00008280: 0072 6901 0000 7263 0000 0072 2700 0000  .ri...rc...r'...
+00008290: 7227 0000 0072 2800 0000 7218 0100 006d  r'...r(...r....m
+000082a0: 0400 0073 3e00 0000 000a 0e02 0a02 0801  ...s>...........
+000082b0: 0802 0602 1002 0802 0802 0801 0403 0401  ................
+000082c0: 16ff 0403 1402 0a02 0401 1001 1601 0a03  ................
+000082d0: 1402 0201 0201 0401 0401 0201 04fb 0608  ................
+000082e0: 0402 0201 02ff 7a15 436f 6f72 6469 6e61  ......z.Coordina
+000082f0: 7465 732e 6765 745f 6172 6561 7329 01da  tes.get_areas)..
+00008300: 0470 6c61 7963 0200 0000 0000 0000 0000  .playc..........
+00008310: 0000 0200 0000 0100 0000 4300 0000 730e  ..........C...s.
+00008320: 0000 007c 0172 0874 0082 017c 006a 0153  ...|.r.t...|.j.S
+00008330: 0029 017a 3952 6574 7565 6e73 2074 6865  .).z9Retuens the
+00008340: 2076 6964 656f 7320 6173 736f 6369 6174   videos associat
+00008350: 6564 2077 6974 6820 7468 6520 6461 7461  ed with the data
+00008360: 7365 7420 6173 2061 206c 6973 742e 2902  set as a list.).
+00008370: 72be 0000 0072 3f01 0000 2902 7257 0000  r....r?...).rW..
+00008380: 0072 7801 0000 7227 0000 0072 2700 0000  .rx...r'...r'...
+00008390: 7228 0000 00da 0a67 6574 5f76 6964 656f  r(.....get_video
+000083a0: 73a7 0400 0073 0600 0000 0002 0401 0402  s....s..........
+000083b0: 7a16 436f 6f72 6469 6e61 7465 732e 6765  z.Coordinates.ge
+000083c0: 745f 7669 6465 6f73 6301 0000 0000 0000  t_videosc.......
+000083d0: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
+000083e0: 0073 0600 0000 7c00 6a00 5300 2901 7a46  .s....|.j.S.).zF
+000083f0: 5265 7475 726e 2074 6865 2073 746f 7265  Return the store
+00008400: 6420 6469 6374 696f 6e61 7279 2077 6974  d dictionary wit
+00008410: 6820 6578 7065 7269 6d65 6e74 616c 2063  h experimental c
+00008420: 6f6e 6469 7469 6f6e 7320 7065 7220 7375  onditions per su
+00008430: 626a 6563 742e 2901 7238 0100 0072 5600  bject.).r8...rV.
+00008440: 0000 7227 0000 0072 2700 0000 7228 0000  ..r'...r'...r(..
+00008450: 00da 1267 6574 5f65 7870 5f63 6f6e 6469  ...get_exp_condi
+00008460: 7469 6f6e 73ae 0400 0073 0200 0000 0003  tions....s......
+00008470: 7a1e 436f 6f72 6469 6e61 7465 732e 6765  z.Coordinates.ge
+00008480: 745f 6578 705f 636f 6e64 6974 696f 6e73  t_exp_conditions
+00008490: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+000084a0: 0004 0000 0003 0000 0073 3800 0000 7400  .........s8...t.
+000084b0: 6a01 7c01 6401 6402 8d02 8900 8700 6601  j.|.d.d.......f.
+000084c0: 6403 6404 8408 8800 6a02 6405 6405 8502  d.d.....j.d.d...
+000084d0: 6401 6602 1900 4400 8301 8900 8800 7c00  d.f...D.......|.
+000084e0: 5f03 6405 5300 2906 7aa8 4c6f 6164 2065  _.d.S.).z.Load e
+000084f0: 7870 6572 696d 656e 7461 6c20 636f 6e64  xperimental cond
+00008500: 6974 696f 6e73 2066 726f 6d20 6120 7769  itions from a wi
+00008510: 6465 2d66 6f72 6d61 7420 6373 7620 7461  de-format csv ta
+00008520: 626c 652e 0a0a 2020 2020 2020 2020 4172  ble...        Ar
+00008530: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+00008540: 6669 6c65 7061 7468 2028 7374 7229 3a20  filepath (str): 
+00008550: 5061 7468 2074 6f20 7468 6520 6669 6c65  Path to the file
+00008560: 2063 6f6e 7461 696e 696e 6720 7468 6520   containing the 
+00008570: 6578 7065 7269 6d65 6e74 616c 2063 6f6e  experimental con
+00008580: 6469 7469 6f6e 732e 0a0a 2020 2020 2020  ditions...      
+00008590: 2020 7201 0000 0029 0172 8a00 0000 6301    r....).r....c.
+000085a0: 0000 0000 0000 0000 0000 0002 0000 0009  ................
+000085b0: 0000 0013 0000 0073 4800 0000 6900 7c00  .......sH...i.|.
+000085c0: 5d40 7d01 7c01 7400 a001 8800 6a02 8800  ]@}.|.t.....j...
+000085d0: 6a03 6400 6400 8502 6401 6602 1900 7c01  j.d.d...d.f...|.
+000085e0: 6b02 6400 6400 8502 6602 1900 6a03 6401  k.d.d...f...j.d.
+000085f0: 6402 6400 8502 6602 1900 a101 6a04 9302  d.d...f.....j...
+00008600: 7104 5300 2903 4e72 0100 0000 7232 0000  q.S.).Nr....r2..
+00008610: 0029 0572 bf00 0000 72dc 0000 0072 c400  .).r....r....r..
+00008620: 0000 7292 0000 0072 c200 0000 2902 724b  ..r....r....).rK
+00008630: 0000 00da 0665 7870 5f69 64a9 0172 3900  .....exp_id..r9.
+00008640: 0000 7227 0000 0072 2800 0000 7298 0000  ..r'...r(...r...
+00008650: 00bb 0400 0073 0800 0000 0604 02fd 0601  .....s..........
+00008660: 30ff 7a33 436f 6f72 6469 6e61 7465 732e  0.z3Coordinates.
+00008670: 6c6f 6164 5f65 7870 5f63 6f6e 6469 7469  load_exp_conditi
+00008680: 6f6e 732e 3c6c 6f63 616c 733e 2e3c 6469  ons.<locals>.<di
+00008690: 6374 636f 6d70 3e4e 2904 72bf 0000 0072  ctcomp>N).r....r
+000086a0: c500 0000 7292 0000 0072 3801 0000 2902  ....r....r8...).
+000086b0: 7257 0000 00da 0866 696c 6570 6174 6872  rW.....filepathr
+000086c0: 2700 0000 727c 0100 0072 2800 0000 da13  '...r|...r(.....
+000086d0: 6c6f 6164 5f65 7870 5f63 6f6e 6469 7469  load_exp_conditi
+000086e0: 6f6e 73b3 0400 0073 0a00 0000 0007 0e01  ons....s........
+000086f0: 0a04 10fc 0606 7a1f 436f 6f72 6469 6e61  ......z.Coordina
+00008700: 7465 732e 6c6f 6164 5f65 7870 5f63 6f6e  tes.load_exp_con
+00008710: 6469 7469 6f6e 7363 0100 0000 0000 0000  ditionsc........
+00008720: 0000 0000 0100 0000 0500 0000 4300 0000  ............C...
+00008730: 7312 0000 0074 007c 006a 0164 017c 006a  s....t.|.j.d.|.j
+00008740: 0264 028d 0353 0029 037a 4d52 6574 7269  .d...S.).zMRetri
+00008750: 6576 6520 6120 6469 6374 696f 6e61 7279  eve a dictionary
+00008760: 2077 6974 6820 7468 6520 7461 6767 696e   with the taggin
+00008770: 6720 7175 616c 6974 7920 7065 7220 7669  g quality per vi
+00008780: 6465 6f2c 2061 7320 7265 706f 7274 6564  deo, as reported
+00008790: 2062 7920 444c 432e 72ae 0000 0072 af00   by DLC.r....r..
+000087a0: 0000 2903 72db 0000 0072 3b01 0000 7232  ..).r....r;...r2
+000087b0: 0100 0072 5600 0000 7227 0000 0072 2700  ...rV...r'...r'.
+000087c0: 0000 7228 0000 0072 6001 0000 c304 0000  ..r(...r`.......
+000087d0: 7302 0000 0000 027a 1743 6f6f 7264 696e  s......z.Coordin
+000087e0: 6174 6573 2e67 6574 5f71 7561 6c69 7479  ates.get_quality
+000087f0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00008800: 0003 0000 0043 0000 0073 1200 0000 7c00  .....C...s....|.
+00008810: 6a00 7c00 6a01 6701 7c00 6a02 6603 5300  j.|.j.g.|.j.f.S.
+00008820: 2901 7a3d 5265 7472 6965 7665 2061 6c6c  ).z=Retrieve all
+00008830: 2061 7661 696c 6162 6c65 2069 6e66 6f72   available infor
+00008840: 6d61 7469 6f6e 2061 7373 6f63 6961 7465  mation associate
+00008850: 6420 7769 7468 2074 6865 2061 7265 6e61  d with the arena
+00008860: 2e29 0372 3301 0000 7235 0100 0072 3c01  .).r3...r5...r<.
+00008870: 0000 7256 0000 0072 2700 0000 7227 0000  ..rV...r'...r'..
+00008880: 0072 2800 0000 7284 0000 00c7 0400 0073  .r(...r........s
+00008890: 0200 0000 0003 7a16 436f 6f72 6469 6e61  ......z.Coordina
+000088a0: 7465 732e 6765 745f 6172 656e 6173 2903  tes.get_arenas).
+000088b0: 725d 0000 00da 0a61 7265 6e61 5f74 7970  r].....arena_typ
+000088c0: 6572 8000 0000 6304 0000 0000 0000 0000  er....c.........
+000088d0: 0000 000d 0000 0008 0000 0043 0000 0073  ...........C...s
+000088e0: 0001 0000 7c01 6401 7500 720e 7c00 6a00  ....|.d.u.r.|.j.
+000088f0: 7d01 7c02 6401 7500 721c 7c00 6a01 7d02  }.|.d.u.r.|.j.}.
+00008900: 6700 6700 0200 7d04 7d05 7402 7c00 6a00  g.g...}.}.t.|.j.
+00008910: 8301 4400 5d2e 5c02 7d06 7d07 7c01 4400  ..D.].\.}.}.|.D.
+00008920: 5d20 7d08 7c08 7c07 7600 723c 7c04 a003  ] }.|.|.v.r<|...
+00008930: 7c07 a101 0100 7c05 a003 7c06 a101 0100  |.....|...|.....
+00008940: 713c 7130 7c03 7288 7404 6402 a005 7406  q<q0|.r.t.d...t.
+00008950: 7c01 8301 7406 7c01 8301 6403 6b04 7280  |...t.|...d.k.r.
+00008960: 6404 6e02 6405 a102 8301 0100 7407 6a08  d.n.d.......t.j.
+00008970: 6a09 7c02 7c00 6a0a 7c00 6a0b 7c00 6a0c  j.|.|.j.|.j.|.j.
+00008980: 7c00 6a0d 7c04 6406 8d06 5c03 7d09 7d0a  |.j.|.d...\.}.}.
+00008990: 7d0b 7c03 72ba 7404 6407 8301 0100 7402  }.|.r.t.d.....t.
+000089a0: 7c01 8301 4400 5d2c 5c02 7d06 7d0c 7c09  |...D.],\.}.}.|.
+000089b0: 7c06 1900 7c00 6a0e 7c05 7c06 1900 3c00  |...|.j.|.|...<.
+000089c0: 7c0a 7c06 1900 7c00 6a0f 7c05 7c06 1900  |.|...|.j.|.|...
+000089d0: 3c00 71c2 7c00 6a10 6408 6409 8d01 0100  <.q.|.j.d.d.....
+000089e0: 6401 5300 290a 61b4 0100 0054 6167 2074  d.S.).a....Tag t
+000089f0: 6865 2061 7265 6e61 2069 6e20 7468 6520  he arena in the 
+00008a00: 7669 6465 6f73 2e0a 0a20 2020 2020 2020  videos...       
+00008a10: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+00008a20: 2020 2076 6964 656f 7320 286c 6973 7429     videos (list)
+00008a30: 3a20 4120 6c69 7374 206f 6620 7669 6465  : A list of vide
+00008a40: 6f73 2074 6f20 7265 616e 6e6f 7461 7465  os to reannotate
+00008a50: 2e20 4966 204e 6f6e 652c 2061 6c6c 2076  . If None, all v
+00008a60: 6964 656f 7320 6172 6520 6c6f 6164 6564  ideos are loaded
+00008a70: 2e0a 2020 2020 2020 2020 2020 2020 6172  ..            ar
+00008a80: 656e 615f 7479 7065 2028 7374 7229 3a20  ena_type (str): 
+00008a90: 5468 6520 7479 7065 206f 6620 6172 656e  The type of aren
+00008aa0: 6120 746f 2075 7365 2e20 4d75 7374 2062  a to use. Must b
+00008ab0: 6520 6f6e 6520 6f66 2022 706f 6c79 676f  e one of "polygo
+00008ac0: 6e61 6c2d 6d61 6e75 616c 222c 2022 6369  nal-manual", "ci
+00008ad0: 7263 756c 6172 2d6d 616e 7561 6c22 2c20  rcular-manual", 
+00008ae0: 6f72 2022 6369 7263 756c 6172 2d61 7574  or "circular-aut
+00008af0: 6f64 6574 6563 7422 2e20 4966 204e 6f6e  odetect". If Non
+00008b00: 6520 2864 6566 6175 6c74 292c 2074 6865  e (default), the
+00008b10: 2061 7265 6e61 2074 7970 6520 7370 6563   arena type spec
+00008b20: 6966 6965 6420 7768 656e 2063 7265 6174  ified when creat
+00008b30: 696e 6720 7468 6520 7072 6f6a 6563 7420  ing the project 
+00008b40: 6973 2075 7365 642e 0a20 2020 2020 2020  is used..       
+00008b50: 2020 2020 2076 6572 626f 7365 2028 626f       verbose (bo
+00008b60: 6f6c 293a 2057 6865 7468 6572 2074 6f20  ol): Whether to 
+00008b70: 7072 696e 7420 7468 6520 7072 6f67 7265  print the progre
+00008b80: 7373 206f 6620 7468 6520 616e 6e6f 7461  ss of the annota
+00008b90: 7469 6f6e 2e0a 0a20 2020 2020 2020 204e  tion...        N
+00008ba0: 7a12 4564 6974 696e 6720 7b7d 2061 7265  z.Editing {} are
+00008bb0: 6e61 7b7d 7232 0000 00da 0173 722d 0000  na{}r2.....sr-..
+00008bc0: 0029 0672 3500 0000 7260 0000 0072 1900  .).r5...r`...r..
+00008bd0: 0000 723f 0000 0072 5e00 0000 725d 0000  ..r?...r^...r]..
+00008be0: 0072 2001 0000 4672 1e01 0000 2911 723f  .r ...Fr....).r?
+00008bf0: 0100 0072 3301 0000 72f7 0000 0072 fe00  ...r3...r....r..
+00008c00: 0000 7281 0000 0072 6d00 0000 725f 0000  ..r....rm...r_..
+00008c10: 0072 8200 0000 7283 0000 0072 8400 0000  .r....r....r....
+00008c20: 7235 0100 0072 2400 0000 7231 0100 0072  r5...r$...r1...r
+00008c30: 3d01 0000 723c 0100 0072 3401 0000 7225  =...r<...r4...r%
+00008c40: 0100 0029 0d72 5700 0000 725d 0000 0072  ...).rW...r]...r
+00008c50: 7f01 0000 7280 0000 00da 0e76 6964 656f  ....r......video
+00008c60: 735f 7265 6e61 6d65 64da 0876 6964 5f69  s_renamed..vid_i
+00008c70: 6463 73da 0776 6964 5f69 6478 da06 7669  dcs..vid_idx..vi
+00008c80: 645f 696e da07 7669 645f 6f75 74da 0d65  d_in..vid_out..e
+00008c90: 6469 7465 645f 7363 616c 6573 da13 6564  dited_scales..ed
+00008ca0: 6974 6564 5f61 7265 6e61 5f70 6172 616d  ited_arena_param
+00008cb0: 7372 8d00 0000 7254 0000 0072 2700 0000  sr....rT...r'...
+00008cc0: 7227 0000 0072 2800 0000 da0b 6564 6974  r'...r(.....edit
+00008cd0: 5f61 7265 6e61 73cc 0400 0073 3800 0000  _arenas....s8...
+00008ce0: 000b 0801 0601 0801 0602 0a01 1201 0801  ................
+00008cf0: 0801 0a01 0e02 0401 0201 1eff 0404 0601  ................
+00008d00: 0201 0401 0401 0401 0401 02fa 0c09 0401  ................
+00008d10: 0803 1001 1201 1402 7a17 436f 6f72 6469  ........z.Coordi
+00008d20: 6e61 7465 732e 6564 6974 5f61 7265 6e61  nates.edit_arena
+00008d30: 7329 02da 0866 696c 656e 616d 6572 1f01  s)...filenamer..
+00008d40: 0000 6303 0000 0000 0000 0000 0000 0005  ..c.............
+00008d50: 0000 0009 0000 0043 0000 0073 7e00 0000  .......C...s~...
+00008d60: 6401 a000 7401 6a02 a003 7c00 6a04 7c00  d...t.j...|.j.|.
+00008d70: 6a05 6402 7c01 6403 7501 7220 7c01 6e02  j.d.|.d.u.r |.n.
+00008d80: 6404 a104 7c02 7238 6405 7406 7407 8300  d...|.r8d.t.t...
+00008d90: 8301 9b00 9d02 6e02 6406 a102 7d03 7408  ......n.d...}.t.
+00008da0: 7c03 6407 8302 8f22 7d04 7409 6a0a 7c00  |.d...."}.t.j.|.
+00008db0: 7c04 7409 6a0b 6408 8d03 0100 5700 6403  |.t.j.d.....W.d.
+00008dc0: 0400 0400 8303 0100 6e10 3100 7370 3000  ........n.1.sp0.
+00008dd0: 0100 0100 0100 5900 0100 6403 5300 2909  ......Y...d.S.).
+00008de0: 6126 0100 0053 6176 6520 7468 6520 6375  a&...Save the cu
+00008df0: 7272 656e 7420 7374 6174 6520 6f66 2074  rrent state of t
+00008e00: 6865 2043 6f6f 7264 696e 6174 6573 206f  he Coordinates o
+00008e10: 626a 6563 7420 746f 2061 2070 6963 6b6c  bject to a pickl
+00008e20: 6564 2066 696c 652e 0a0a 2020 2020 2020  ed file...      
+00008e30: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+00008e40: 2020 2020 6669 6c65 6e61 6d65 2028 7374      filename (st
+00008e50: 7229 3a20 4e61 6d65 206f 6620 7468 6520  r): Name of the 
+00008e60: 7069 636b 6c65 6420 6669 6c65 2074 6f20  pickled file to 
+00008e70: 7374 6f72 652e 2049 6620 6e6f 206e 616d  store. If no nam
+00008e80: 6520 6973 2070 726f 7669 6465 642c 2061  e is provided, a
+00008e90: 2064 6566 6175 6c74 2069 7320 7573 6564   default is used
+00008ea0: 2e0a 2020 2020 2020 2020 2020 2020 7469  ..            ti
+00008eb0: 6d65 7374 616d 7020 2862 6f6f 6c29 3a20  mestamp (bool): 
+00008ec0: 5768 6574 6865 7220 746f 2061 7070 656e  Whether to appen
+00008ed0: 6420 6120 7469 6d65 2073 7461 6d70 2061  d a time stamp a
+00008ee0: 7420 7468 6520 656e 6420 6f66 2074 6865  t the end of the
+00008ef0: 206f 7574 7075 7420 6669 6c65 206e 616d   output file nam
+00008f00: 652e 0a20 2020 2020 2020 207a 087b 7d7b  e..        z.{}{
+00008f10: 7d2e 706b 6c72 1b00 0000 4e72 1700 0000  }.pklr....Nr....
+00008f20: 728d 0000 0072 2d00 0000 da02 7762 2901  r....r-.....wb).
+00008f30: da08 7072 6f74 6f63 6f6c 290c 726d 0000  ..protocol).rm..
+00008f40: 0072 1e00 0000 721f 0000 0072 2000 0000  .r....r....r ...
+00008f50: 7224 0000 0072 3101 0000 7221 0100 0072  r$...r1...r!...r
+00008f60: 0e00 0000 721d 0000 0072 2100 0000 da04  ....r....r!.....
+00008f70: 6475 6d70 da10 4849 4748 4553 545f 5052  dump..HIGHEST_PR
+00008f80: 4f54 4f43 4f4c 2905 7257 0000 0072 8901  OTOCOL).rW...r..
+00008f90: 0000 721f 0100 00da 0770 6b6c 5f6f 7574  ..r......pkl_out
+00008fa0: 7225 0000 0072 2700 0000 7227 0000 0072  r%...r'...r'...r
+00008fb0: 2800 0000 7225 0100 00fb 0400 0073 1600  (...r%.......s..
+00008fc0: 0000 0007 0401 0601 0401 0401 0201 0efc  ................
+00008fd0: 0206 16f9 040a 0c01 7a10 436f 6f72 6469  ........z.Coordi
+00008fe0: 6e61 7465 732e 7361 7665 2907 7206 0100  nates.save).r...
+00008ff0: 00da 1470 7265 636f 6d70 7574 6564 5f74  ...precomputed_t
+00009000: 6162 5f64 6963 7472 4401 0000 7245 0100  ab_dictrD...rE..
+00009010: 0072 4701 0000 da0a 7072 6570 726f 6365  .rG.....preproce
+00009020: 7373 721a 0000 0063 0700 0000 0000 0000  ssr....c........
+00009030: 0000 0000 1a00 0000 0900 0000 0b00 0000  ................
+00009040: 7392 0300 0088 006a 007c 017c 037c 057c  s......j.|.|.|.|
+00009050: 0464 018d 047d 0888 006a 007c 0164 0264  .d...}...j.|.d.d
+00009060: 038d 027d 0988 006a 017c 0164 048d 017d  ...}...j.|.d...}
+00009070: 0a7c 08a0 027c 097c 0aa1 027d 0b7c 0264  .|...|.|...}.|.d
+00009080: 0575 0172 447c 027d 0b74 036a 046a 057c  .u.rD|.}.t.j.j.|
+00009090: 0164 0575 0072 5888 006a 066e 027c 0188  .d.u.rX..j.n.|..
+000090a0: 006a 0664 0575 0172 8a88 006a 0664 0619  .j.d.u.r...j.d..
+000090b0: 0072 8a74 0774 0887 0066 0164 0764 0884  .r.t.t...f.d.d..
+000090c0: 0888 006a 0944 0083 0183 0183 016e 0488  ...j.D.......n..
+000090d0: 006a 0988 006a 0a64 098d 037d 0c7c 0c7c  .j...j.d...}.|.|
+000090e0: 0b5f 0b74 0774 077c 0aa0 0ca1 0083 0164  ._.t.t.|.......d
+000090f0: 0619 006a 0d83 017d 0d74 0ea0 0f64 0a64  ...j...}.t...d.d
+00009100: 0884 0074 077c 0ba0 0ca1 0083 0164 0619  ...t.|.......d..
+00009110: 006a 0d44 0083 01a1 017d 0e64 0b64 0884  .j.D.....}.d.d..
+00009120: 0074 077c 0ca0 10a1 0083 0144 0083 0164  .t.|.......D...d
+00009130: 0c64 0884 0074 077c 0ca0 10a1 0083 0144  .d...t.|.......D
+00009140: 0083 0117 0074 077c 0ca0 10a1 0083 0117  .....t.|........
+00009150: 007d 0f67 007d 1067 007d 117c 0f44 005d  .}.g.}.g.}.|.D.]
+00009160: 2e7d 1274 117c 0e83 0144 005d 1e5c 027d  .}.t.|...D.].\.}
+00009170: 137d 147c 127c 146b 0290 0172 267c 10a0  .}.|.|.k...r&|..
+00009180: 127c 13a1 0101 0090 0171 2690 0171 1a67  .|.......q&..q.g
+00009190: 007d 1564 0d64 0884 0074 077c 0c6a 1383  .}.d.d...t.|.j..
+000091a0: 0144 0083 0144 005d 5e7d 1674 117c 0d83  .D...D.]^}.t.|..
+000091b0: 0144 005d 1e5c 027d 137d 147c 167c 146b  .D.].\.}.}.|.|.k
+000091c0: 0290 0172 6e7c 11a0 127c 13a1 0101 0090  ...rn|...|......
+000091d0: 0171 6e74 1488 006a 0683 0164 026b 0490  .qnt...j...d.k..
+000091e0: 0172 627c 15a0 1274 1474 0864 0e64 0884  .rb|...t.t.d.d..
+000091f0: 007c 1644 0083 0183 0183 0164 026b 02a1  .|.D.......d.k..
+00009200: 0101 0090 0171 627c 0690 0272 ee7c 0b6a  .....qb|...r.|.j
+00009210: 1566 0069 007c 07a4 018e 015c 027d 177d  .f.i.|.....\.}.}
+00009220: 187c 1764 0619 0064 0564 0585 0264 0564  .|.d...d.d...d.d
+00009230: 0585 027c 0ea0 167c 0da1 010f 0066 0319  ...|...|.....f..
+00009240: 0064 0564 0585 0264 0564 0585 027c 1066  .d.d...d.d...|.f
+00009250: 0319 007c 1764 0619 0064 0564 0585 0264  ...|.d...d.d...d
+00009260: 0564 0585 027c 0ea0 167c 0da1 0166 0319  .d...|...|...f..
+00009270: 0064 0564 0585 0264 0564 0585 027c 1166  .d.d...d.d...|.f
+00009280: 0319 007c 1764 0219 0067 037d 197a 747c  ...|.d...g.}.zt|
+00009290: 197c 1764 0f19 0064 0564 0585 0264 0564  .|.d...d.d...d.d
+000092a0: 0585 027c 0ea0 167c 0da1 010f 0066 0319  ...|...|.....f..
+000092b0: 0064 0564 0585 0264 0564 0585 027c 1066  .d.d...d.d...|.f
+000092c0: 0319 007c 1764 0f19 0064 0564 0585 0264  ...|.d...d.d...d
+000092d0: 0564 0585 027c 0ea0 167c 0da1 0166 0319  .d...|...|...f..
+000092e0: 0064 0564 0585 0264 0564 0585 027c 1166  .d.d...d.d...|.f
+000092f0: 0319 007c 1764 1019 0067 0337 007d 1957  ...|.d...g.7.}.W
+00009300: 006e 2e04 0074 1790 0279 ea01 0001 0001  .n...t...y......
+00009310: 007c 197c 1764 0f19 007c 1764 0f19 007c  .|.|.d...|.d...|
+00009320: 1764 1019 0067 0337 007d 1959 006e 0230  .d...g.7.}.Y.n.0
+00009330: 006e 8a74 18a0 1974 077c 17a0 0ca1 0083  .n.t...t.|......
+00009340: 01a1 017d 177c 1764 0564 0585 027c 0ea0  ...}.|.d.d...|..
+00009350: 167c 0da1 010f 0066 0219 0064 0564 0585  .|.....f...d.d..
+00009360: 027c 1066 0219 006a 1a7c 176a 1b64 0619  .|.f...j.|.j.d..
+00009370: 0074 147c 0ca0 10a1 0083 0164 1167 0364  .t.|.......d.g.d
+00009380: 1264 138d 0274 036a 04a0 1c74 1da0 1e7c  .d...t.j...t...|
+00009390: 0ca1 01a0 1fa1 007c 1764 0564 0585 027c  .......|.d.d...|
+000093a0: 0ea0 167c 0da1 0166 0219 0064 0564 0585  ...|...f...d.d..
+000093b0: 027c 1166 0219 00a1 0266 027d 1974 207c  .|.f.....f.}.t |
+000093c0: 1983 0174 1da0 217c 0ca1 01a0 1fa1 007c  ...t..!|.......|
+000093d0: 0b7c 1866 0453 0029 1461 ed03 0000 4765  .|.f.S.).a....Ge
+000093e0: 6e65 7261 7465 2061 2064 6174 6173 6574  nerate a dataset
+000093f0: 2077 6974 6820 616c 6c20 7370 6563 6966   with all specif
+00009400: 6965 6420 6665 6174 7572 6573 2e0a 0a20  ied features... 
+00009410: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+00009420: 2020 2020 2020 2020 2061 6e69 6d61 6c5f           animal_
+00009430: 6964 2028 7374 7229 3a20 4e61 6d65 206f  id (str): Name o
+00009440: 6620 7468 6520 616e 696d 616c 2074 6f20  f the animal to 
+00009450: 7072 6f63 6573 732e 2049 6620 4e6f 6e65  process. If None
+00009460: 2028 6465 6661 756c 7429 2061 6c6c 2061   (default) all a
+00009470: 6e69 6d61 6c73 2061 7265 2069 6e63 6c75  nimals are inclu
+00009480: 6465 6420 696e 2061 206d 756c 7469 2d61  ded in a multi-a
+00009490: 6e69 6d61 6c20 6772 6170 682e 0a20 2020  nimal graph..   
+000094a0: 2020 2020 2020 2020 2070 7265 636f 6d70           precomp
+000094b0: 7574 6564 5f74 6162 5f64 6963 7420 2874  uted_tab_dict (t
+000094c0: 6162 6c65 5f64 6963 7429 3a20 7461 626c  able_dict): tabl
+000094d0: 655f 6469 6374 206f 626a 6563 7420 666f  e_dict object fo
+000094e0: 7220 6675 7274 6865 7220 6772 6170 6820  r further graph 
+000094f0: 7072 6f63 6573 7369 6e67 2e20 4e6f 6e65  processing. None
+00009500: 2028 6465 6661 756c 7429 2062 7569 6c64   (default) build
+00009510: 7320 6974 206f 6e20 7468 6520 7370 6f74  s it on the spot
+00009520: 2e0a 2020 2020 2020 2020 2020 2020 6365  ..            ce
+00009530: 6e74 6572 2028 7374 7229 3a20 4e61 6d65  nter (str): Name
+00009540: 206f 6620 7468 6520 626f 6479 2070 6172   of the body par
+00009550: 7420 746f 2077 6869 6368 2074 6865 2070  t to which the p
+00009560: 6f73 6974 696f 6e73 2077 696c 6c20 6265  ositions will be
+00009570: 2063 656e 7465 7265 642e 2049 6620 6661   centered. If fa
+00009580: 6c73 652c 2072 6177 2064 6174 6120 6973  lse, raw data is
+00009590: 2072 6574 7572 6e65 643b 2069 6620 2761   returned; if 'a
+000095a0: 7265 6e61 2720 2864 6566 6175 6c74 292c  rena' (default),
+000095b0: 2063 6f6f 7264 696e 6174 6573 2061 7265   coordinates are
+000095c0: 2063 656e 7465 7265 6420 6f6e 2074 6865   centered on the
+000095d0: 2070 6974 6368 2e0a 2020 2020 2020 2020   pitch..        
+000095e0: 2020 2020 706f 6c61 7220 2862 6f6f 6c29      polar (bool)
+000095f0: 2053 7461 7465 7320 7768 6574 6865 7220   States whether 
+00009600: 7468 6520 636f 6f72 6469 6e61 7465 7320  the coordinates 
+00009610: 7368 6f75 6c64 2062 6520 636f 6e76 6572  should be conver
+00009620: 7465 6420 746f 2070 6f6c 6172 2076 616c  ted to polar val
+00009630: 7565 732e 0a20 2020 2020 2020 2020 2020  ues..           
+00009640: 2061 6c69 676e 2028 7374 7229 3a20 5365   align (str): Se
+00009650: 6c65 6374 7320 7468 6520 626f 6479 2070  lects the body p
+00009660: 6172 7420 746f 2077 6869 6368 206c 6174  art to which lat
+00009670: 6572 2070 726f 6365 7373 6573 2077 696c  er processes wil
+00009680: 6c20 616c 6967 6e20 7468 6520 6672 616d  l align the fram
+00009690: 6573 2077 6974 6820 2873 6565 2070 7265  es with (see pre
+000096a0: 7072 6f63 6573 7320 696e 2074 6162 6c65  process in table
+000096b0: 5f64 6963 7420 646f 6375 6d65 6e74 6174  _dict documentat
+000096c0: 696f 6e29 2e0a 2020 2020 2020 2020 2020  ion)..          
+000096d0: 2020 7072 6570 726f 6365 7373 2028 626f    preprocess (bo
+000096e0: 6f6c 293a 2077 6865 7468 6572 2074 6f20  ol): whether to 
+000096f0: 7072 6570 726f 6365 7373 2074 6865 2064  preprocess the d
+00009700: 6174 6120 746f 2070 6173 7320 746f 2061  ata to pass to a
+00009710: 7574 6f65 6e63 6f64 6572 732e 2049 6620  utoencoders. If 
+00009720: 4661 6c73 652c 206e 6f64 6520 6665 6174  False, node feat
+00009730: 7572 6573 2061 6e64 2064 6973 7461 6e63  ures and distanc
+00009740: 652d 7765 6967 6874 6564 2061 646a 6163  e-weighted adjac
+00009750: 656e 6379 206d 6174 7269 6365 7320 6f6e  ency matrices on
+00009760: 2074 6865 2072 6177 2064 6174 6120 6172   the raw data ar
+00009770: 6520 7265 7475 726e 6564 2e0a 0a20 2020  e returned...   
+00009780: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
+00009790: 2020 2020 2020 2020 2020 6d65 7267 6564            merged
+000097a0: 5f66 6561 7475 7265 733a 2041 2067 7261  _features: A gra
+000097b0: 7068 2d62 6173 6564 2064 6174 6173 6574  ph-based dataset
+000097c0: 2e0a 0a20 2020 2020 2020 2029 0472 4901  ...        ).rI.
+000097d0: 0000 7244 0100 0072 4701 0000 7245 0100  ..rD...rG...rE..
+000097e0: 0072 3200 0000 2902 7249 0100 0072 4601  .r2...).rI...rF.
+000097f0: 0000 2901 7249 0100 004e 7201 0000 0063  ..).rI...Nr....c
+00009800: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00009810: 0a00 0000 1300 0000 7334 0000 0067 007c  ........s4...g.|
+00009820: 005d 2c7d 0174 00a0 0164 00a0 0274 0374  .],}.t...d...t.t
+00009830: 006a 0464 0164 0284 0088 006a 0544 0083  .j.d.d.....j.D..
+00009840: 0183 02a1 0164 037c 01a1 0391 0271 0453  .....d.|.....q.S
+00009850: 0029 04da 017c 6301 0000 0000 0000 0000  .)...|c.........
+00009860: 0000 0002 0000 0004 0000 0053 0000 0073  ...........S...s
+00009870: 1400 0000 6700 7c00 5d0c 7d01 7c01 6400  ....g.|.].}.|.d.
+00009880: 1700 9102 7104 5300 729a 0000 0072 2700  ....q.S.r....r'.
+00009890: 0000 724a 0000 0072 2700 0000 7227 0000  ..rJ...r'...r'..
+000098a0: 0072 2800 0000 724d 0000 003d 0500 0072  .r(...rM...=...r
+000098b0: 4e00 0000 7a3c 436f 6f72 6469 6e61 7465  N...z<Coordinate
+000098c0: 732e 6765 745f 6772 6170 685f 6461 7461  s.get_graph_data
+000098d0: 7365 742e 3c6c 6f63 616c 733e 2e3c 6c69  set.<locals>.<li
+000098e0: 7374 636f 6d70 3e2e 3c6c 6973 7463 6f6d  stcomp>.<listcom
+000098f0: 703e 722d 0000 0029 0672 c600 0000 da03  p>r-...).r......
+00009900: 7375 6272 2000 0000 72d6 0000 00da 0665  subr ...r......e
+00009910: 7363 6170 6572 3201 0000 724e 0100 0072  scaper2...rN...r
+00009920: 5600 0000 7227 0000 0072 2800 0000 724d  V...r'...r(...rM
+00009930: 0000 003a 0500 0073 1000 0000 0608 02f9  ...:...s........
+00009940: 0401 0401 16ff 0203 0201 02fb 7a31 436f  ............z1Co
+00009950: 6f72 6469 6e61 7465 732e 6765 745f 6772  ordinates.get_gr
+00009960: 6170 685f 6461 7461 7365 742e 3c6c 6f63  aph_dataset.<loc
+00009970: 616c 733e 2e3c 6c69 7374 636f 6d70 3e29  als>.<listcomp>)
+00009980: 0372 3400 0000 7238 0000 0072 9400 0000  .r4...r8...r....
+00009990: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+000099a0: 0003 0000 0053 0000 0073 1000 0000 6700  .....S...s....g.
+000099b0: 7c00 5d08 7d01 7c01 9102 7104 5300 7227  |.].}.|...q.S.r'
+000099c0: 0000 0072 2700 0000 724a 0000 0072 2700  ...r'...rJ...r'.
+000099d0: 0000 7227 0000 0072 2800 0000 724d 0000  ..r'...r(...rM..
+000099e0: 004e 0500 0072 4e00 0000 6301 0000 0000  .N...rN...c.....
+000099f0: 0000 0000 0000 0002 0000 0004 0000 0053  ...............S
+00009a00: 0000 0073 1400 0000 6700 7c00 5d0c 7d01  ...s....g.|.].}.
+00009a10: 7c01 6400 6602 9102 7104 5300 7208 0100  |.d.f...q.S.r...
+00009a20: 0072 2700 0000 724a 0000 0072 2700 0000  .r'...rJ...r'...
+00009a30: 7227 0000 0072 2800 0000 724d 0000 0050  r'...r(...rM...P
+00009a40: 0500 0072 4e00 0000 6301 0000 0000 0000  ...rN...c.......
+00009a50: 0000 0000 0002 0000 0004 0000 0053 0000  .............S..
+00009a60: 0073 1400 0000 6700 7c00 5d0c 7d01 7c01  .s....g.|.].}.|.
+00009a70: 6400 6602 9102 7104 5300 2901 72aa 0000  d.f...q.S.).r...
+00009a80: 0072 2700 0000 724a 0000 0072 2700 0000  .r'...rJ...r'...
+00009a90: 7227 0000 0072 2800 0000 724d 0000 0051  r'...r(...rM...Q
+00009aa0: 0500 0072 4e00 0000 6301 0000 0000 0000  ...rN...c.......
+00009ab0: 0000 0000 0002 0000 0005 0000 0053 0000  .............S..
+00009ac0: 0073 1800 0000 6700 7c00 5d10 7d01 7400  .s....g.|.].}.t.
+00009ad0: 7401 7c01 8301 8301 9102 7104 5300 7227  t.|.......q.S.r'
+00009ae0: 0000 0072 7001 0000 7271 0100 0072 2700  ...rp...rq...r'.
+00009af0: 0000 7227 0000 0072 2800 0000 724d 0000  ..r'...r(...rM..
+00009b00: 005e 0500 0072 4e00 0000 6301 0000 0000  .^...rN...c.....
+00009b10: 0000 0000 0000 0002 0000 0005 0000 0053  ...............S
+00009b20: 0000 0073 1a00 0000 6700 7c00 5d12 7d01  ...s....g.|.].}.
+00009b30: 7c01 a000 6400 a101 6401 1900 9102 7104  |...d...d.....q.
+00009b40: 5300 2902 728d 0000 0072 0100 0000 2901  S.).r....r....).
+00009b50: 7223 0000 0029 0272 4b00 0000 da04 6e6f  r#...).rK.....no
+00009b60: 6465 7227 0000 0072 2700 0000 7228 0000  der'...r'...r(..
+00009b70: 0072 4d00 0000 6505 0000 724e 0000 0072  .rM...e...rN...r
+00009b80: 9300 0000 722f 0000 00e9 ffff ffff da01  ....r/..........
+00009b90: 4629 01da 056f 7264 6572 2922 726c 0100  F)...order)"rl..
+00009ba0: 0072 fa00 0000 da05 6d65 7267 6572 8200  .r......merger..
+00009bb0: 0000 7283 0000 0072 9500 0000 7232 0100  ..r....r....r2..
+00009bc0: 0072 b600 0000 72b7 0000 0072 3701 0000  .r....r....r7...
+00009bd0: 7236 0100 0072 4201 0000 72c9 0000 0072  r6...rB...r....r
+00009be0: b800 0000 72bf 0000 00da 0549 6e64 6578  ....r......Index
+00009bf0: 72f4 0000 0072 f700 0000 72fe 0000 0072  r....r....r....r
+00009c00: 7401 0000 725f 0000 0072 9001 0000 da04  t...r_...r......
+00009c10: 6973 696e 72c8 0000 0072 de00 0000 da0b  isinr....r......
+00009c20: 636f 6e63 6174 656e 6174 6572 fd00 0000  concatenater....
+00009c30: 72d5 0000 00da 1465 6467 6573 5f74 6f5f  r......edges_to_
+00009c40: 7765 6974 6865 645f 6164 6ada 026e 78da  weithed_adj..nx.
+00009c50: 0a61 646a 5f6d 6174 7269 78da 0774 6f64  .adj_matrix..tod
+00009c60: 656e 7365 72d2 0000 00da 1061 646a 6163  enser......adjac
+00009c70: 656e 6379 5f6d 6174 7269 7829 1a72 5700  ency_matrix).rW.
+00009c80: 0000 7206 0100 0072 8f01 0000 7244 0100  ..r....r....rD..
+00009c90: 0072 4501 0000 7247 0100 0072 9001 0000  .rE...rG...r....
+00009ca0: da06 6b77 6172 6773 72a7 0000 00da 0673  ..kwargsr......s
+00009cb0: 7065 6564 7372 6e01 0000 72e3 0000 00da  peedsrn...r.....
+00009cc0: 0567 7261 7068 da12 6564 6765 5f66 6561  .graph..edge_fea
+00009cd0: 7475 7265 5f6e 616d 6573 da0d 6665 6174  ture_names..feat
+00009ce0: 7572 655f 6e61 6d65 73da 126e 6f64 655f  ure_names..node_
+00009cf0: 6665 6174 7572 655f 6e61 6d65 73da 146e  feature_names..n
+00009d00: 6f64 655f 736f 7274 696e 675f 696e 6469  ode_sorting_indi
+00009d10: 6365 73da 1465 6467 655f 736f 7274 696e  ces..edge_sortin
+00009d20: 675f 696e 6469 6365 73da 016e 72b5 0000  g_indices..nr...
+00009d30: 00da 0166 da14 696e 6e65 725f 6c69 6e6b  ...f..inner_link
+00009d40: 5f62 6f6f 6c5f 6d61 736b 7272 0100 00da  _bool_maskrr....
+00009d50: 0d74 6f5f 7072 6570 726f 6365 7373 da0d  .to_preprocess..
+00009d60: 676c 6f62 616c 5f73 6361 6c65 72da 0764  global_scaler..d
+00009d70: 6174 6173 6574 7227 0000 0072 5600 0000  atasetr'...rV...
+00009d80: 7228 0000 00da 1167 6574 5f67 7261 7068  r(.....get_graph
+00009d90: 5f64 6174 6173 6574 0f05 0000 73ae 0000  _dataset....s...
+00009da0: 0000 1904 0108 ff06 030e 010c 030c 0208  ................
+00009db0: 0104 0306 0110 1008 f202 0e08 f204 0102  ................
+00009dc0: 010a 0804 f804 ff02 ff04 0f04 0204 ec06  ................
+00009dd0: 1706 0116 0122 0214 0114 ff02 020a fe02  ....."..........
+00009de0: ff02 0704 0104 0108 0110 010a 0112 0204  ................
+00009df0: 0118 0110 010a 010e 0210 0104 0118 ff08  ................
+00009e00: 0506 0114 0220 0110 ff02 031e 0110 ff02  ..... ..........
+00009e10: 0306 f904 0902 0102 0120 0110 ff02 031e  ......... ......
+00009e20: 0110 ff02 0306 f90a 090e 0122 0312 0416  ..........."....
+00009e30: 010a ff04 0218 fe04 0306 010c 0114 010a  ................
+00009e40: ff02 fe02 fc04 0d06 010c 0102 0102 fc7a  ...............z
+00009e50: 1d43 6f6f 7264 696e 6174 6573 2e67 6574  .Coordinates.get
+00009e60: 5f67 7261 7068 5f64 6174 6173 6574 7232  _graph_datasetr2
+00009e70: 0000 0029 07da 0670 6172 616d 73da 0c76  ...)...params..v
+00009e80: 6964 656f 5f6f 7574 7075 74da 0b66 7261  ideo_output..fra
+00009e90: 6d65 5f6c 696d 6974 da05 6465 6275 67da  me_limit..debug.
+00009ea0: 066e 5f6a 6f62 7372 4a01 0000 721a 0000  .n_jobsrJ...r...
+00009eb0: 0063 0700 0000 0000 0000 0000 0000 1300  .c..............
+00009ec0: 0000 0e00 0000 0300 0000 730a 0200 0069  ..........s....i
+00009ed0: 007d 0774 006a 01a0 027c 01a1 017d 0188  .}.t.j...|...}..
+00009ee0: 016a 0364 0164 028d 017d 087a 1288 016a  .j.d.d...}.z...j
+00009ef0: 0364 0364 0464 058d 027d 0957 006e 2004  .d.d.d...}.W.n .
+00009f00: 0074 0479 4e01 0001 0001 0088 016a 0364  .t.yN........j.d
+00009f10: 0364 0664 058d 027d 0959 006e 0230 0088  .d.d...}.Y.n.0..
+00009f20: 01a0 05a1 007d 0a88 016a 0364 0764 088d  .....}...j.d.d..
+00009f30: 017d 0b74 0688 016a 0783 0164 076b 0172  .}.t...j...d.k.r
+00009f40: 8474 006a 086a 0988 0164 0964 0a8d 027d  .t.j.j...d.d...}
+00009f50: 0c6e 1487 0166 0164 0b64 0c84 0888 016a  .n...f.d.d.....j
+00009f60: 0744 0083 017d 0c74 0a88 016a 0ba0 0ca1  .D...}.t...j....
+00009f70: 0083 0144 005d 7e89 007c 0888 0019 006a  ...D.]~..|.....j
+00009f80: 0d7d 0d74 0e88 0083 0101 0074 0e74 0f88  .}.t.......t.t..
+00009f90: 0088 016a 1064 0d64 0764 0e8d 0464 0f19  ...j.d.d.d...d..
+00009fa0: 0083 0101 0074 006a 016a 1188 017c 087c  .....t.j.j...|.|
+00009fb0: 097c 0a7c 0c7c 0b74 0f88 0087 0066 0164  .|.|.|.t.....f.d
+00009fc0: 1064 1184 0888 016a 1044 0083 0164 0d64  .d.....j.D...d.d
+00009fd0: 0764 0e8d 0464 0f19 0088 016a 127c 0164  .d...d.....j.|.d
+00009fe0: 128d 097d 0e7c 0d7c 0e5f 0d7c 0e7c 0788  ...}.|.|._.|.|..
+00009ff0: 003c 0071 a67c 0690 0172 4e7c 07a0 13a1  .<.q.|...rN|....
+0000a000: 0044 005d 185c 0289 007d 0f88 016a 1488  .D.].\...}...j..
+0000a010: 0019 007c 0f64 133c 0090 0171 347c 0290  ...|.d.<...q4|..
+0000a020: 0172 6e74 006a 016a 1588 017c 077c 027c  .rnt.j.j...|.|.|
+0000a030: 037c 047c 057c 0164 148d 0701 0074 006a  .|.|.|.d.....t.j
+0000a040: 166a 1788 017c 0788 01a0 18a1 0088 016a  .j...|.........j
+0000a050: 0764 1567 0117 0064 168d 047d 0774 006a  .d.g...d...}.t.j
+0000a060: 16a0 1988 01a0 18a1 00a1 017d 107c 0744  ...........}.|.D
+0000a070: 005d 447d 1188 016a 0744 005d 367d 1264  .]D}...j.D.]6}.d
+0000a080: 077c 107c 1119 007c 1219 006a 1a18 007c  .|.|...|...j...|
+0000a090: 077c 1119 0064 17a0 1b7c 1290 0172 da64  .|...d...|...r.d
+0000a0a0: 18a0 1b7c 12a1 016e 0264 19a1 013c 0090  ...|...n.d...<..
+0000a0b0: 0171 ac90 0171 a274 1c7c 0764 1588 016a  .q...q.t.|.d...j
+0000a0c0: 0788 016a 1d88 016a 1e88 016a 1f88 016a  ...j...j...j...j
+0000a0d0: 147c 0664 1a8d 0853 0029 1b61 e303 0000  .|.d...S.).a....
+0000a0e0: 416e 6e6f 7461 7465 7320 636f 6f72 6469  Annotates coordi
+0000a0f0: 6e61 7465 7320 7769 7468 2062 6568 6176  nates with behav
+0000a100: 696f 7261 6c20 7472 6169 7473 2075 7369  ioral traits usi
+0000a110: 6e67 2061 2073 7570 6572 7669 7365 6420  ng a supervised 
+0000a120: 7069 7065 6c69 6e65 2e0a 0a20 2020 2020  pipeline...     
+0000a130: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+0000a140: 2020 2020 2070 6172 616d 7320 2844 6963       params (Dic
+0000a150: 7429 3a20 4120 6469 6374 696f 6e61 7279  t): A dictionary
+0000a160: 2077 6974 6820 7468 6520 7061 7261 6d65   with the parame
+0000a170: 7465 7273 2074 6f20 7573 6520 666f 7220  ters to use for 
+0000a180: 7468 6520 7069 7065 6c69 6e65 2e20 4966  the pipeline. If
+0000a190: 2075 6e73 7572 652c 206c 6561 7665 2065   unsure, leave e
+0000a1a0: 6d70 7479 2e0a 2020 2020 2020 2020 2020  mpty..          
+0000a1b0: 2020 7669 6465 6f5f 6f75 7470 7574 2028    video_output (
+0000a1c0: 626f 6f6c 293a 2049 7420 6f75 7470 7574  bool): It output
+0000a1d0: 7320 6120 6675 6c6c 7920 616e 6e6f 7461  s a fully annota
+0000a1e0: 7465 6420 7669 6465 6f20 666f 7220 6561  ted video for ea
+0000a1f0: 6368 2065 7870 6572 696d 656e 7420 696e  ch experiment in
+0000a200: 6469 6361 7465 6420 696e 2061 206c 6973  dicated in a lis
+0000a210: 742e 2049 6620 7365 7420 746f 2022 616c  t. If set to "al
+0000a220: 6c22 2c20 6974 2077 696c 6c20 6f75 7470  l", it will outp
+0000a230: 7574 2061 6c6c 2076 6964 656f 732e 2046  ut all videos. F
+0000a240: 616c 7365 2062 7920 6465 6661 756c 742e  alse by default.
+0000a250: 0a20 2020 2020 2020 2020 2020 2066 7261  .            fra
+0000a260: 6d65 5f6c 696d 6974 2028 696e 7429 3a20  me_limit (int): 
+0000a270: 4f6e 6c79 2061 7070 6c69 6573 2069 6620  Only applies if 
+0000a280: 7669 6465 6f5f 6f75 7470 7574 2069 7320  video_output is 
+0000a290: 6e6f 7420 4661 6c73 652e 2049 6e64 6963  not False. Indic
+0000a2a0: 6174 6573 2074 6865 206d 6178 696d 756d  ates the maximum
+0000a2b0: 206e 756d 6265 7220 6f66 2066 7261 6d65   number of frame
+0000a2c0: 7320 7065 7220 7669 6465 6f20 746f 206f  s per video to o
+0000a2d0: 7574 7075 742e 0a20 2020 2020 2020 2020  utput..         
+0000a2e0: 2020 2064 6562 7567 2028 626f 6f6c 293a     debug (bool):
+0000a2f0: 204f 6e6c 7920 6170 706c 6965 7320 6966   Only applies if
+0000a300: 2076 6964 656f 5f6f 7574 7075 7420 6973   video_output is
+0000a310: 206e 6f74 2046 616c 7365 2e20 4966 2054   not False. If T
+0000a320: 7275 652c 2061 6c6c 2076 6964 656f 7320  rue, all videos 
+0000a330: 7769 6c6c 2069 6e63 6c75 6465 2064 6562  will include deb
+0000a340: 7567 2069 6e66 6f72 6d61 7469 6f6e 2c20  ug information, 
+0000a350: 7375 6368 2061 7320 7468 6520 6465 7465  such as the dete
+0000a360: 6374 6564 2061 7265 6e61 2061 6e64 2074  cted arena and t
+0000a370: 6865 2070 7265 7072 6f63 6573 7365 6420  he preprocessed 
+0000a380: 7472 6163 6b69 6e67 2074 6167 732e 0a20  tracking tags.. 
+0000a390: 2020 2020 2020 2020 2020 206e 5f6a 6f62             n_job
+0000a3a0: 7320 2869 6e74 293a 204e 756d 6265 7220  s (int): Number 
+0000a3b0: 6f66 206a 6f62 7320 746f 2075 7365 2066  of jobs to use f
+0000a3c0: 6f72 2070 6172 616c 6c65 6c20 7072 6f63  or parallel proc
+0000a3d0: 6573 7369 6e67 2e0a 2020 2020 2020 2020  essing..        
+0000a3e0: 2020 2020 7072 6f70 6167 6174 655f 6c61      propagate_la
+0000a3f0: 6265 6c73 2028 626f 6f6c 293a 2049 6620  bels (bool): If 
+0000a400: 5472 7565 2c20 7468 6520 7068 656e 6f20  True, the pheno 
+0000a410: 636f 6c75 6d6e 2077 696c 6c20 6265 2070  column will be p
+0000a420: 726f 7061 6761 7465 6420 6672 6f6d 2074  ropagated from t
+0000a430: 6865 206f 7269 6769 6e61 6c20 6461 7461  he original data
+0000a440: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+0000a450: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+0000a460: 7461 626c 655f 6469 6374 3a20 4120 7461  table_dict: A ta
+0000a470: 626c 655f 6469 6374 206f 626a 6563 7420  ble_dict object 
+0000a480: 7769 7468 2061 6c6c 2073 7570 6572 7669  with all supervi
+0000a490: 7365 6420 616e 6e6f 7461 7469 6f6e 7320  sed annotations 
+0000a4a0: 7065 7220 6578 7065 7269 6d65 6e74 2061  per experiment a
+0000a4b0: 7320 7661 6c75 6573 2e0a 0a20 2020 2020  s values...     
+0000a4c0: 2020 204e 724f 0100 00da 0643 656e 7465     NrO.....Cente
+0000a4d0: 72da 0753 7069 6e65 5f31 2902 7244 0100  r..Spine_1).rD..
+0000a4e0: 0072 4701 0000 da04 4e6f 7365 7232 0000  .rG.....Noser2..
+0000a4f0: 0029 0172 4601 0000 4629 01da 0e69 6e63  .).rF...F)...inc
+0000a500: 6c75 6465 5f61 6e67 6c65 7363 0100 0000  lude_anglesc....
+0000a510: 0000 0000 0000 0000 0200 0000 0800 0000  ................
+0000a520: 1300 0000 7320 0000 0069 007c 005d 187d  ....s ...i.|.].}
+0000a530: 017c 0174 006a 016a 0288 007c 0164 0064  .|.t.j.j...|.d.d
+0000a540: 018d 0393 0271 0453 0029 0246 2902 7206  .....q.S.).F).r.
+0000a550: 0100 0072 b801 0000 2903 7282 0000 00da  ...r....).r.....
+0000a560: 0870 6f73 745f 686f 63da 3061 6c69 676e  .post_hoc.0align
+0000a570: 5f64 6565 706f 665f 6b69 6e65 6d61 7469  _deepof_kinemati
+0000a580: 6373 5f77 6974 685f 756e 7375 7065 7276  cs_with_unsuperv
+0000a590: 6973 6564 5f6c 6162 656c 7329 0272 4b00  ised_labels).rK.
+0000a5a0: 0000 da03 5f69 6472 5600 0000 7227 0000  ...._idrV...r'..
+0000a5b0: 0072 2800 0000 7298 0000 00c2 0500 0073  .r(...r........s
+0000a5c0: 0800 0000 0604 02fd 0801 06ff 7a35 436f  ............z5Co
+0000a5d0: 6f72 6469 6e61 7465 732e 7375 7065 7276  ordinates.superv
+0000a5e0: 6973 6564 5f61 6e6e 6f74 6174 696f 6e2e  ised_annotation.
+0000a5f0: 3c6c 6f63 616c 733e 2e3c 6469 6374 636f  <locals>.<dictco
+0000a600: 6d70 3ee7 9a99 9999 9999 b93f 2902 da06  mp>........?)...
+0000a610: 6375 746f 6666 72a9 0100 0072 0100 0000  cutoffr....r....
+0000a620: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+0000a630: 0005 0000 0013 0000 0073 1a00 0000 6700  .........s....g.
+0000a640: 7c00 5d12 7d01 7c01 a000 8800 a101 7204  |.].}.|.......r.
+0000a650: 7c01 9102 7104 5300 7227 0000 0072 4800  |...q.S.r'...rH.
+0000a660: 0000 7253 0000 0029 0172 e600 0000 7227  ..rS...).r....r'
+0000a670: 0000 0072 2800 0000 724d 0000 00da 0500  ...r(...rM......
+0000a680: 0072 4e00 0000 7a35 436f 6f72 6469 6e61  .rN...z5Coordina
+0000a690: 7465 732e 7375 7065 7276 6973 6564 5f61  tes.supervised_a
+0000a6a0: 6e6e 6f74 6174 696f 6e2e 3c6c 6f63 616c  nnotation.<local
+0000a6b0: 733e 2e3c 6c69 7374 636f 6d70 3e29 08da  s>.<listcomp>)..
+0000a6c0: 0a72 6177 5f63 6f6f 7264 7372 a700 0000  .raw_coordsr....
+0000a6d0: 726e 0100 00da 0d66 756c 6c5f 6665 6174  rn.....full_feat
+0000a6e0: 7572 6573 72a2 0100 00da 0576 6964 656f  uresr......video
+0000a6f0: 721c 0100 0072 b001 0000 7252 0100 0029  r....r....rR...)
+0000a700: 0572 b101 0000 72b2 0100 0072 b301 0000  .r....r....r....
+0000a710: 72b4 0100 0072 b001 0000 da0a 7375 7065  r....r......supe
+0000a720: 7276 6973 6564 2901 7234 0000 007a 097b  rvised).r4...z.{
+0000a730: 7d6d 6973 7369 6e67 7a03 7b7d 5f72 2d00  }missingz.{}_r-.
+0000a740: 0000 2907 72b0 0000 0072 3400 0000 7235  ..).r....r4...r5
+0000a750: 0000 0072 6000 0000 7264 0000 0072 3900  ...r`...rd...r9.
+0000a760: 0000 724a 0100 0029 2072 8200 0000 da10  ..rJ...) r......
+0000a770: 616e 6e6f 7461 7469 6f6e 5f75 7469 6c73  annotation_utils
+0000a780: da0f 6765 745f 6870 6172 616d 6574 6572  ..get_hparameter
+0000a790: 7372 6c01 0000 da0e 4173 7365 7274 696f  srl.....Assertio
+0000a7a0: 6e45 7272 6f72 72fa 0000 0072 5f00 0000  nErrorr....r_...
+0000a7b0: 7232 0100 0072 b901 0000 72ba 0100 0072  r2...r....r....r
+0000a7c0: 0f00 0000 723d 0100 0072 f600 0000 72ca  ....r=...r....r.
+0000a7d0: 0000 0072 8100 0000 7203 0000 0072 3f01  ...r....r....r?.
+0000a7e0: 0000 da12 7375 7065 7276 6973 6564 5f74  ....supervised_t
+0000a7f0: 6167 6769 6e67 723e 0100 0072 cc00 0000  aggingr>...r....
+0000a800: 7238 0100 00da 1374 6167 6765 645f 7669  r8.....tagged_vi
+0000a810: 6465 6f5f 6f75 7470 7574 7283 0000 0072  deo_outputr....r
+0000a820: e200 0000 7260 0100 00da 1c63 6f6d 7075  ....r`.....compu
+0000a830: 7465 5f61 6e69 6d61 6c5f 7072 6573 656e  te_animal_presen
+0000a840: 6365 5f6d 6173 6b72 c900 0000 726d 0000  ce_maskr....rm..
+0000a850: 0072 db00 0000 7233 0100 0072 3501 0000  .r....r3...r5...
+0000a860: 7242 0100 0029 1372 5700 0000 72b0 0100  rB...).rW...r...
+0000a870: 0072 b101 0000 72b2 0100 0072 b301 0000  .r....r....r....
+0000a880: 72b4 0100 0072 4a01 0000 da08 7461 675f  r....rJ.....tag_
+0000a890: 6469 6374 72be 0100 0072 a700 0000 726e  dictr....r....rn
+0000a8a0: 0100 0072 a201 0000 da0d 6665 6174 7572  ...r......featur
+0000a8b0: 6573 5f64 6963 74da 0974 6167 5f69 6e64  es_dict..tag_ind
+0000a8c0: 6578 da0f 7375 7065 7276 6973 6564 5f74  ex..supervised_t
+0000a8d0: 6167 7372 5500 0000 da0e 7072 6573 656e  agsrU.....presen
+0000a8e0: 6365 5f6d 6173 6b73 da03 7461 67da 0661  ce_masks..tag..a
+0000a8f0: 6e69 6d61 6c72 2700 0000 2902 72e6 0000  nimalr'...).r...
+0000a900: 0072 5700 0000 7228 0000 00da 1573 7570  .rW...r(.....sup
+0000a910: 6572 7669 7365 645f 616e 6e6f 7461 7469  ervised_annotati
+0000a920: 6f6e 9905 0000 738c 0000 0000 1704 010c  on....s.........
+0000a930: 010c 0202 0112 010c 0114 0208 010c 010e  ................
+0000a940: 0206 0104 ff04 ff04 060a 0404 fc06 0812  ................
+0000a950: 040a 0208 011a 0206 0102 0102 0102 0102  ................
+0000a960: 0102 0102 0122 0104 0102 f706 0c06 010a  ....."..........
+0000a970: 0206 0110 0112 0206 0206 0102 0102 0102  ................
+0000a980: 0102 0102 0102 0102 f906 0b06 0102 0102  ................
+0000a990: 0106 010a fc06 0810 0108 010a 0310 fe06  ................
+0000a9a0: 0118 ff0a 0402 0102 0102 0104 0104 0104  ................
+0000a9b0: 0104 0104 0102 f87a 2143 6f6f 7264 696e  .......z!Coordin
+0000a9c0: 6174 6573 2e73 7570 6572 7669 7365 645f  ates.supervised_
+0000a9d0: 616e 6e6f 7461 7469 6f6e da04 5661 4445  annotation..VaDE
+0000a9e0: da09 7265 6375 7272 656e 74e9 4000 0000  ..recurrent.@...
+0000a9f0: e904 0000 00e9 9600 0000 e90a 0000 0072  ...............r
+0000aa00: ad00 0000 72bc 0100 00da 0663 6f73 696e  ....r......cosin
+0000aa10: 65da 036e 6365 da06 6c69 6e65 6172 72b1  e..nce..linearr.
+0000aa20: 0000 0029 1cda 1370 7265 7072 6f63 6573  ...)...preproces
+0000aa30: 7365 645f 6f62 6a65 6374 72a0 0100 00da  sed_objectr.....
+0000aa40: 0f65 6d62 6564 6469 6e67 5f6d 6f64 656c  .embedding_model
+0000aa50: da0c 656e 636f 6465 725f 7479 7065 da0a  ..encoder_type..
+0000aa60: 6261 7463 685f 7369 7a65 da0a 6c61 7465  batch_size..late
+0000aa70: 6e74 5f64 696d da06 6570 6f63 6873 da0b  nt_dim..epochs..
+0000aa80: 6c6f 675f 6869 7374 6f72 79da 0b6c 6f67  log_history..log
+0000aa90: 5f68 7061 7261 6d73 da0c 6e5f 636f 6d70  _hparams..n_comp
+0000aaa0: 6f6e 656e 7473 da0b 6b6d 6561 6e73 5f6c  onents..kmeans_l
+0000aab0: 6f73 73da 0b74 656d 7065 7261 7475 7265  oss..temperature
+0000aac0: da1f 636f 6e74 7261 7374 6976 655f 7369  ..contrastive_si
+0000aad0: 6d69 6c61 7269 7479 5f66 756e 6374 696f  milarity_functio
+0000aae0: 6eda 1963 6f6e 7472 6173 7469 7665 5f6c  n..contrastive_l
+0000aaf0: 6f73 735f 6675 6e63 7469 6f6e da04 6265  oss_function..be
+0000ab00: 7461 da03 7461 75da 0b6f 7574 7075 745f  ta..tau..output_
+0000ab10: 7061 7468 da0a 7072 6574 7261 696e 6564  path..pretrained
+0000ab20: da10 7361 7665 5f63 6865 636b 706f 696e  ..save_checkpoin
+0000ab30: 7473 da0c 7361 7665 5f77 6569 6768 7473  ts..save_weights
+0000ab40: da0a 696e 7075 745f 7479 7065 da03 7275  ..input_type..ru
+0000ab50: 6eda 116b 6c5f 616e 6e65 616c 696e 675f  n..kl_annealing_
+0000ab60: 6d6f 6465 da09 6b6c 5f77 6172 6d75 70da  mode..kl_warmup.
+0000ab70: 1072 6567 5f63 6174 5f63 6c75 7374 6572  .reg_cat_cluster
+0000ab80: 73da 0972 6563 6c75 7374 6572 da1a 696e  s..recluster..in
+0000ab90: 7465 7261 6374 696f 6e5f 7265 6775 6c61  teraction_regula
+0000aba0: 7269 7a61 7469 6f6e 721a 0000 0063 1c00  rizationr....c..
+0000abb0: 0000 0000 0000 0000 0000 1f00 0000 1e00  ................
+0000abc0: 0000 0b00 0000 73d4 0000 007c 1272 5474  ......s....|.rTt
+0000abd0: 006a 01a0 027c 006a 037c 006a 0464 0164  .j...|.j.|.j.d.d
+0000abe0: 02a1 047d 1d74 006a 01a0 027c 1d74 057c  ...}.t.j...|.t.|
+0000abf0: 1274 0683 0272 307c 126e 2087 0087 0187  .t...r0|.n .....
+0000ac00: 0287 0366 0464 0364 0484 0874 00a0 077c  ...f.d.d...t...|
+0000ac10: 1da1 0144 0083 0164 0519 00a1 027d 127a  ...D...d.....}.z
+0000ac20: 6074 086a 096a 0a66 007c 017c 0288 0088  `t.j.j.f.|.|....
+0000ac30: 017c 0588 027c 077c 087c 0988 037c 0b7c  .|...|.|.|...|.|
+0000ac40: 0c7c 0d7c 0e7c 0f7c 1074 006a 01a0 027c  .|.|.|.|.t.j...|
+0000ac50: 006a 037c 006a 047c 1164 01a1 047c 127c  .j.|.j.|.d...|.|
+0000ac60: 137c 147c 157c 167c 177c 187c 197c 1a7c  .|.|.|.|.|.|.|.|
+0000ac70: 1b64 069c 1b7c 1ca4 018e 017d 1e57 006e  .d...|.....}.W.n
+0000ac80: 1a04 0074 0b79 ce01 0001 0001 0074 0c64  ...t.y.......t.d
+0000ac90: 0783 0182 0159 006e 0230 007c 1e53 0029  .....Y.n.0.|.S.)
+0000aca0: 0861 f90d 0000 416e 6e6f 7461 7465 7320  .a....Annotates 
+0000acb0: 636f 6f72 6469 6e61 7465 7320 7573 696e  coordinates usin
+0000acc0: 6720 6120 6465 6570 2075 6e73 7570 6572  g a deep unsuper
+0000acd0: 7669 7365 6420 6175 746f 656e 636f 6465  vised autoencode
+0000ace0: 722e 0a0a 2020 2020 2020 2020 4172 6773  r...        Args
+0000acf0: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
+0000ad00: 6570 726f 6365 7373 6564 5f6f 626a 6563  eprocessed_objec
+0000ad10: 7420 2874 7570 6c65 293a 2054 7570 6c65  t (tuple): Tuple
+0000ad20: 2063 6f6e 7461 696e 696e 6720 6120 7072   containing a pr
+0000ad30: 6570 726f 6365 7373 6564 206f 626a 6563  eprocessed objec
+0000ad40: 7420 2858 5f74 7261 696e 2c20 795f 7472  t (X_train, y_tr
+0000ad50: 6169 6e2c 2058 5f74 6573 742c 2079 5f74  ain, X_test, y_t
+0000ad60: 6573 7429 2e0a 2020 2020 2020 2020 2020  est)..          
+0000ad70: 2020 6164 6a61 6365 6e63 795f 6d61 7472    adjacency_matr
+0000ad80: 6978 2028 6e70 2e6e 6461 7272 6179 293a  ix (np.ndarray):
+0000ad90: 2061 646a 6163 656e 6379 206d 6174 7269   adjacency matri
+0000ada0: 7820 6f66 2074 6865 2063 6f6e 6e65 6374  x of the connect
+0000adb0: 6976 6974 7920 6772 6170 6820 746f 2075  ivity graph to u
+0000adc0: 7365 2e0a 2020 2020 2020 2020 2020 2020  se..            
+0000add0: 656d 6265 6464 696e 675f 6d6f 6465 6c20  embedding_model 
+0000ade0: 2873 7472 293a 204e 616d 6520 6f66 2074  (str): Name of t
+0000adf0: 6865 2065 6d62 6564 6469 6e67 206d 6f64  he embedding mod
+0000ae00: 656c 2074 6f20 7573 652e 204d 7573 7420  el to use. Must 
+0000ae10: 6265 206f 6e65 206f 6620 5651 5641 4520  be one of VQVAE 
+0000ae20: 2864 6566 6175 6c74 292c 2056 6144 452c  (default), VaDE,
+0000ae30: 206f 7220 636f 6e74 7261 7374 6976 652e   or contrastive.
+0000ae40: 0a20 2020 2020 2020 2020 2020 2065 6e63  .            enc
+0000ae50: 6f64 6572 5f74 7970 6520 2873 7472 293a  oder_type (str):
+0000ae60: 2045 6e63 6f64 6572 2061 7263 6869 7465   Encoder archite
+0000ae70: 6374 7572 6520 746f 2075 7365 2e20 4d75  cture to use. Mu
+0000ae80: 7374 2062 6520 6f6e 6520 6f66 2022 7265  st be one of "re
+0000ae90: 6375 7272 656e 7422 2c20 2254 434e 222c  current", "TCN",
+0000aea0: 2061 6e64 2022 7472 616e 7366 6f72 6d65   and "transforme
+0000aeb0: 7222 2e0a 2020 2020 2020 2020 2020 2020  r"..            
+0000aec0: 6261 7463 685f 7369 7a65 2028 696e 7429  batch_size (int)
+0000aed0: 3a20 4261 7463 6820 7369 7a65 2066 6f72  : Batch size for
+0000aee0: 2074 7261 696e 696e 672e 0a20 2020 2020   training..     
+0000aef0: 2020 2020 2020 206c 6174 656e 745f 6469         latent_di
+0000af00: 6d20 2869 6e74 293a 2044 696d 656e 7469  m (int): Dimenti
+0000af10: 6f6e 2073 697a 6520 6f66 2074 6865 206c  on size of the l
+0000af20: 6174 656e 7420 7370 6163 652e 0a20 2020  atent space..   
+0000af30: 2020 2020 2020 2020 2065 706f 6368 7320           epochs 
+0000af40: 2869 6e74 293a 204d 6178 696d 756d 206e  (int): Maximum n
+0000af50: 756d 6265 7220 6f66 2065 706f 6368 7320  umber of epochs 
+0000af60: 746f 2074 7261 696e 2074 6865 206d 6f64  to train the mod
+0000af70: 656c 2e20 4163 7475 616c 2074 7261 696e  el. Actual train
+0000af80: 696e 6720 6d69 6768 7420 6265 2073 686f  ing might be sho
+0000af90: 7274 6572 2c20 6173 2074 6865 206d 6f64  rter, as the mod
+0000afa0: 656c 2077 696c 6c20 7374 6f70 2074 7261  el will stop tra
+0000afb0: 696e 696e 6720 7768 656e 2076 616c 6964  ining when valid
+0000afc0: 6174 696f 6e20 6c6f 7373 2073 746f 7073  ation loss stops
+0000afd0: 2064 6563 7265 6173 696e 672e 0a20 2020   decreasing..   
+0000afe0: 2020 2020 2020 2020 206c 6f67 5f68 6973           log_his
+0000aff0: 746f 7279 2028 626f 6f6c 293a 2057 6865  tory (bool): Whe
+0000b000: 7468 6572 2074 6f20 6c6f 6720 7468 6520  ther to log the 
+0000b010: 6869 7374 6f72 7920 6f66 2074 6865 206d  history of the m
+0000b020: 6f64 656c 2074 6f20 5465 6e73 6f72 426f  odel to TensorBo
+0000b030: 6172 642e 0a20 2020 2020 2020 2020 2020  ard..           
+0000b040: 206c 6f67 5f68 7061 7261 6d73 2028 626f   log_hparams (bo
+0000b050: 6f6c 293a 2057 6865 7468 6572 2074 6f20  ol): Whether to 
+0000b060: 6c6f 6720 7468 6520 6879 7065 7270 6172  log the hyperpar
+0000b070: 616d 6574 6572 7320 6f66 2074 6865 206d  ameters of the m
+0000b080: 6f64 656c 2074 6f20 5465 6e73 6f72 426f  odel to TensorBo
+0000b090: 6172 642e 0a20 2020 2020 2020 2020 2020  ard..           
+0000b0a0: 206e 5f63 6f6d 706f 6e65 6e74 7320 2869   n_components (i
+0000b0b0: 6e74 293a 204e 756d 6265 7220 6f66 206c  nt): Number of l
+0000b0c0: 6174 656e 7420 636c 7573 7465 7273 2066  atent clusters f
+0000b0d0: 6f72 2074 6865 2065 6d62 6564 6469 6e67  or the embedding
+0000b0e0: 206d 6f64 656c 2074 6f20 7573 652e 0a20   model to use.. 
+0000b0f0: 2020 2020 2020 2020 2020 206b 6d65 616e             kmean
+0000b100: 735f 6c6f 7373 2028 666c 6f61 7429 3a20  s_loss (float): 
+0000b110: 5765 6967 6874 206f 6620 7468 6520 6772  Weight of the gr
+0000b120: 616d 206c 6f73 732c 2077 6869 6368 2061  am loss, which a
+0000b130: 6464 7320 6120 7265 6775 6c61 7269 7a61  dds a regulariza
+0000b140: 7469 6f6e 2074 6572 6d20 746f 2056 6144  tion term to VaD
+0000b150: 4520 616e 6420 5651 5641 4520 6d6f 6465  E and VQVAE mode
+0000b160: 6c73 2077 6869 6368 2070 656e 616c 697a  ls which penaliz
+0000b170: 6573 2074 6865 2063 6f72 7265 6c61 7469  es the correlati
+0000b180: 6f6e 2062 6574 7765 656e 2074 6865 2064  on between the d
+0000b190: 696d 656e 7369 6f6e 7320 696e 2074 6865  imensions in the
+0000b1a0: 206c 6174 656e 7420 7370 6163 652e 0a20   latent space.. 
+0000b1b0: 2020 2020 2020 2020 2020 2074 656d 7065             tempe
+0000b1c0: 7261 7475 7265 2028 666c 6f61 7429 3a20  rature (float): 
+0000b1d0: 7465 6d70 6572 6174 7572 6520 7061 7261  temperature para
+0000b1e0: 6d65 7465 7220 666f 7220 7468 6520 636f  meter for the co
+0000b1f0: 6e74 7261 7374 6976 6520 6c6f 7373 2066  ntrastive loss f
+0000b200: 756e 6374 696f 6e73 2e20 4869 6768 6572  unctions. Higher
+0000b210: 2076 616c 7565 7320 7075 7420 6861 7273   values put hars
+0000b220: 6865 7220 7065 6e61 6c74 6965 7320 6f6e  her penalties on
+0000b230: 206e 6567 6174 6976 6520 7061 6972 2073   negative pair s
+0000b240: 696d 696c 6172 6974 792e 0a20 2020 2020  imilarity..     
+0000b250: 2020 2020 2020 2063 6f6e 7472 6173 7469         contrasti
+0000b260: 7665 5f73 696d 696c 6172 6974 795f 6675  ve_similarity_fu
+0000b270: 6e63 7469 6f6e 2028 7374 7229 3a20 7369  nction (str): si
+0000b280: 6d69 6c61 7269 7479 2066 756e 6374 696f  milarity functio
+0000b290: 6e20 6265 7477 6565 6e20 706f 7369 7469  n between positi
+0000b2a0: 7665 2061 6e64 206e 6567 6174 6976 6520  ve and negative 
+0000b2b0: 7061 6972 732e 204d 7573 7420 6265 206f  pairs. Must be o
+0000b2c0: 6e65 206f 6620 2763 6f73 696e 6527 2028  ne of 'cosine' (
+0000b2d0: 6465 6661 756c 7429 2c20 2765 7563 6c69  default), 'eucli
+0000b2e0: 6465 616e 272c 2027 646f 7427 2c20 616e  dean', 'dot', an
+0000b2f0: 6420 2765 6469 7427 2e0a 2020 2020 2020  d 'edit'..      
+0000b300: 2020 2020 2020 636f 6e74 7261 7374 6976        contrastiv
+0000b310: 655f 6c6f 7373 5f66 756e 6374 696f 6e20  e_loss_function 
+0000b320: 2873 7472 293a 2063 6f6e 7472 6173 7469  (str): contrasti
+0000b330: 7665 206c 6f73 7320 6675 6e63 7469 6f6e  ve loss function
+0000b340: 2e20 4d75 7374 2062 6520 6f6e 6520 6f66  . Must be one of
+0000b350: 2027 6e63 6527 2028 6465 6661 756c 7429   'nce' (default)
+0000b360: 2c20 2764 636c 272c 2027 6663 272c 2061  , 'dcl', 'fc', a
+0000b370: 6e64 2027 6861 7264 5f64 636c 272e 2053  nd 'hard_dcl'. S
+0000b380: 6565 2073 7065 6369 6669 6320 646f 6375  ee specific docu
+0000b390: 6d65 6e74 6174 696f 6e20 666f 7220 6465  mentation for de
+0000b3a0: 7461 696c 732e 0a20 2020 2020 2020 2020  tails..         
+0000b3b0: 2020 2062 6574 6120 2866 6c6f 6174 293a     beta (float):
+0000b3c0: 2042 6574 6120 2863 6f6e 6365 6e74 7261   Beta (concentra
+0000b3d0: 7469 6f6e 2920 7061 7261 6d65 7465 7220  tion) parameter 
+0000b3e0: 666f 7220 7468 6520 6861 7264 5f64 636c  for the hard_dcl
+0000b3f0: 2063 6f6e 7472 6173 7469 7665 206c 6f73   contrastive los
+0000b400: 732e 2048 6967 6865 7220 7661 6c75 6573  s. Higher values
+0000b410: 206c 6561 6420 746f 2027 6861 7264 6572   lead to 'harder
+0000b420: 2720 6e65 6761 7469 7665 2073 616d 706c  ' negative sampl
+0000b430: 6573 2e0a 2020 2020 2020 2020 2020 2020  es..            
+0000b440: 7461 7520 2866 6c6f 6174 293a 2054 6175  tau (float): Tau
+0000b450: 2070 6172 616d 6574 6572 2066 6f72 2074   parameter for t
+0000b460: 6865 2064 636c 2061 6e64 2068 6172 645f  he dcl and hard_
+0000b470: 6463 6c20 636f 6e74 7261 7374 6976 6520  dcl contrastive 
+0000b480: 6c6f 7373 6573 2c20 696e 6469 6361 7469  losses, indicati
+0000b490: 6e67 2070 6f73 6974 6976 6520 636c 6173  ng positive clas
+0000b4a0: 7320 7072 6f62 6162 696c 6974 792e 0a20  s probability.. 
+0000b4b0: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
+0000b4c0: 745f 7061 7468 2028 7374 7229 3a20 5061  t_path (str): Pa
+0000b4d0: 7468 2074 6f20 7361 7665 2074 6865 2074  th to save the t
+0000b4e0: 7261 696e 6564 206d 6f64 656c 2061 6e64  rained model and
+0000b4f0: 2061 6c6c 206c 6f67 2066 696c 6573 2e0a   all log files..
+0000b500: 2020 2020 2020 2020 2020 2020 7072 6574              pret
+0000b510: 7261 696e 6564 2028 7374 7229 3a20 5768  rained (str): Wh
+0000b520: 6574 6865 7220 746f 206c 6f61 6420 6120  ether to load a 
+0000b530: 7072 6574 7261 696e 6564 206d 6f64 656c  pretrained model
+0000b540: 2e20 4966 2046 616c 7365 2c20 6d6f 6465  . If False, mode
+0000b550: 6c20 6973 2074 7261 696e 6564 2066 726f  l is trained fro
+0000b560: 6d20 7363 7261 7463 682e 2049 6620 6e6f  m scratch. If no
+0000b570: 742c 206d 7573 7420 6265 2074 6865 2070  t, must be the p
+0000b580: 6174 6820 746f 2061 2073 6176 6564 206d  ath to a saved m
+0000b590: 6f64 656c 2e0a 2020 2020 2020 2020 2020  odel..          
+0000b5a0: 2020 7361 7665 5f63 6865 636b 706f 696e    save_checkpoin
+0000b5b0: 7473 2028 626f 6f6c 293a 2057 6865 7468  ts (bool): Wheth
+0000b5c0: 6572 2074 6f20 7361 7665 2063 6865 636b  er to save check
+0000b5d0: 706f 696e 7473 206f 6620 7468 6520 6d6f  points of the mo
+0000b5e0: 6465 6c20 6475 7269 6e67 2074 7261 696e  del during train
+0000b5f0: 696e 672e 2044 6566 6175 6c74 7320 746f  ing. Defaults to
+0000b600: 2046 616c 7365 2e0a 2020 2020 2020 2020   False..        
+0000b610: 2020 2020 7361 7665 5f77 6569 6768 7473      save_weights
+0000b620: 2028 626f 6f6c 293a 2057 6865 7468 6572   (bool): Whether
+0000b630: 2074 6f20 7361 7665 2074 6865 2077 6569   to save the wei
+0000b640: 6768 7473 206f 6620 7468 6520 6d6f 6465  ghts of the mode
+0000b650: 6c20 6475 7269 6e67 2074 7261 696e 696e  l during trainin
+0000b660: 672e 2044 6566 6175 6c74 7320 746f 2054  g. Defaults to T
+0000b670: 7275 652e 0a20 2020 2020 2020 2020 2020  rue..           
+0000b680: 2069 6e70 7574 5f74 7970 6520 2873 7472   input_type (str
+0000b690: 293a 2054 7970 6520 6f66 2074 6865 2070  ): Type of the p
+0000b6a0: 7265 7072 6f63 6573 7365 645f 6f62 6a65  reprocessed_obje
+0000b6b0: 6374 2070 6173 7365 6420 6173 2074 6865  ct passed as the
+0000b6c0: 2066 6972 7374 2070 6172 616d 6574 6572   first parameter
+0000b6d0: 2e20 5365 6520 6465 6570 6f66 2e64 6174  . See deepof.dat
+0000b6e0: 612e 5461 626c 6544 6963 7420 666f 7220  a.TableDict for 
+0000b6f0: 6d6f 7265 2064 6574 6169 6c73 2e0a 2020  more details..  
+0000b700: 2020 2020 2020 2020 2020 7275 6e20 2869            run (i
+0000b710: 6e74 293a 2052 756e 206e 756d 6265 7220  nt): Run number 
+0000b720: 666f 7220 7468 6520 6d6f 6465 6c2e 2055  for the model. U
+0000b730: 7365 6420 746f 2073 6176 6520 7468 6520  sed to save the 
+0000b740: 6d6f 6465 6c20 616e 6420 6c6f 6720 6669  model and log fi
+0000b750: 6c65 732e 204f 7074 696f 6e61 6c2e 0a20  les. Optional.. 
+0000b760: 2020 2020 2020 2020 2020 206b 6c5f 616e             kl_an
+0000b770: 6e65 616c 696e 675f 6d6f 6465 2028 7374  nealing_mode (st
+0000b780: 7229 3a20 4d6f 6465 206f 6620 7468 6520  r): Mode of the 
+0000b790: 4b4c 2061 6e6e 6561 6c69 6e67 2e20 4d75  KL annealing. Mu
+0000b7a0: 7374 2062 6520 6f6e 6520 6f66 2022 6c69  st be one of "li
+0000b7b0: 6e65 6172 222c 206f 7220 2273 6967 6d6f  near", or "sigmo
+0000b7c0: 6964 222e 0a20 2020 2020 2020 2020 2020  id"..           
+0000b7d0: 206b 6c5f 7761 726d 7570 2028 696e 7429   kl_warmup (int)
+0000b7e0: 3a20 4e75 6d62 6572 206f 6620 6570 6f63  : Number of epoc
+0000b7f0: 6873 2074 6f20 7761 726d 2075 7020 7468  hs to warm up th
+0000b800: 6520 4b4c 2061 6e6e 6561 6c69 6e67 2e0a  e KL annealing..
+0000b810: 2020 2020 2020 2020 2020 2020 7265 675f              reg_
+0000b820: 6361 745f 636c 7573 7465 7273 2028 626f  cat_clusters (bo
+0000b830: 6f6c 293a 2077 6865 7468 6572 2074 6f20  ol): whether to 
+0000b840: 7065 6e61 6c69 7a65 2075 6e65 7665 6e20  penalize uneven 
+0000b850: 636c 7573 7465 7220 6d65 6d62 6572 7368  cluster membersh
+0000b860: 6970 2069 6e20 7468 6520 6c61 7465 6e74  ip in the latent
+0000b870: 2073 7061 6365 2c20 6279 206d 696e 696d   space, by minim
+0000b880: 697a 696e 6720 7468 6520 4b4c 2064 6976  izing the KL div
+0000b890: 6572 6765 6e63 6520 6265 7477 6565 6e20  ergence between 
+0000b8a0: 636c 7573 7465 7220 6d65 6d62 6572 7368  cluster membersh
+0000b8b0: 6970 2061 6e64 2061 2075 6e69 666f 726d  ip and a uniform
+0000b8c0: 2063 6174 6567 6f72 6963 616c 2064 6973   categorical dis
+0000b8d0: 7472 6962 7574 696f 6e2e 0a20 2020 2020  tribution..     
+0000b8e0: 2020 2020 2020 2072 6563 6c75 7374 6572         recluster
+0000b8f0: 2028 626f 6f6c 293a 2077 6865 7468 6572   (bool): whether
+0000b900: 2074 6f20 7265 636c 7573 7465 7220 6166   to recluster af
+0000b910: 7465 7220 7472 6169 6e69 6e67 2075 7369  ter training usi
+0000b920: 6e67 2061 2047 6175 7373 6961 6e20 4d69  ng a Gaussian Mi
+0000b930: 7874 7572 6520 4d6f 6465 6c2e 204f 6e6c  xture Model. Onl
+0000b940: 7920 7661 6c69 6420 666f 7220 5661 4445  y valid for VaDE
+0000b950: 2e0a 2020 2020 2020 2020 2020 2020 696e  ..            in
+0000b960: 7465 7261 6374 696f 6e5f 7265 6775 6c61  teraction_regula
+0000b970: 7269 7a61 7469 6f6e 2028 666c 6f61 7429  rization (float)
+0000b980: 3a20 7765 6967 6874 206f 6620 7468 6520  : weight of the 
+0000b990: 696e 7465 7261 6374 696f 6e20 7265 6775  interaction regu
+0000b9a0: 6c61 7269 7a61 7469 6f6e 2074 6572 6d20  larization term 
+0000b9b0: 666f 7220 616c 6c20 656e 636f 6465 7273  for all encoders
+0000b9c0: 2e0a 2020 2020 2020 2020 2020 2020 2a2a  ..            **
+0000b9d0: 6b77 6172 6773 3a20 4164 6469 7469 6f6e  kwargs: Addition
+0000b9e0: 616c 206b 6579 776f 7264 2061 7267 756d  al keyword argum
+0000b9f0: 656e 7473 2074 6f20 7061 7373 2074 6f20  ents to pass to 
+0000ba00: 7468 6520 6d6f 6465 6c2e 0a0a 2020 2020  the model...    
+0000ba10: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+0000ba20: 2020 2020 2020 2020 2054 7570 6c65 3a20           Tuple: 
+0000ba30: 5475 706c 6520 636f 6e74 6169 6e69 6e67  Tuple containing
+0000ba40: 2061 6c6c 2074 7261 696e 6564 206d 6f64   all trained mod
+0000ba50: 656c 732e 2053 6565 2073 7065 6369 6669  els. See specifi
+0000ba60: 6320 6d6f 6465 6c20 646f 6375 6d65 6e74  c model document
+0000ba70: 6174 696f 6e20 756e 6465 7220 6465 6570  ation under deep
+0000ba80: 6f66 2e6d 6f64 656c 7320 666f 7220 6465  of.models for de
+0000ba90: 7461 696c 732e 0a20 2020 2020 2020 20da  tails..        .
+0000baa0: 0e54 7261 696e 6564 5f6d 6f64 656c 73da  .Trained_models.
+0000bab0: 0f74 7261 696e 6564 5f77 6569 6768 7473  .trained_weights
+0000bac0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+0000bad0: 0005 0000 0013 0000 0073 3800 0000 6700  .........s8...g.
+0000bae0: 7c00 5d30 7d01 8800 7c01 7600 7204 8801  |.]0}...|.v.r...
+0000baf0: 7c01 7600 7204 6400 a000 8802 a101 7c01  |.v.r.d.......|.
+0000bb00: 7600 7204 6401 a000 8803 a101 7204 7c01  v.r.d.......r.|.
+0000bb10: 9102 7104 5300 2902 7a0b 656e 636f 6469  ..q.S.).z.encodi
+0000bb20: 6e67 3d7b 7d7a 046b 3d7b 7d29 0172 6d00  ng={}z.k={}).rm.
+0000bb30: 0000 2902 724b 0000 00da 0177 a904 72da  ..).rK.....w..r.
+0000bb40: 0100 0072 db01 0000 72dd 0100 0072 e101  ...r....r....r..
+0000bb50: 0000 7227 0000 0072 2800 0000 724d 0000  ..r'...r(...rM..
+0000bb60: 005b 0600 0073 0c00 0000 0602 0201 0801  .[...s..........
+0000bb70: 0801 0e01 0afb 7a3b 436f 6f72 6469 6e61  ......z;Coordina
+0000bb80: 7465 732e 6465 6570 5f75 6e73 7570 6572  tes.deep_unsuper
+0000bb90: 7669 7365 645f 656d 6265 6464 696e 672e  vised_embedding.
+0000bba0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
+0000bbb0: 6d70 3e72 0100 0000 291b 72d9 0100 0072  mp>r....).r....r
+0000bbc0: a001 0000 72da 0100 0072 db01 0000 72dc  ....r....r....r.
+0000bbd0: 0100 0072 dd01 0000 72de 0100 0072 df01  ...r....r....r..
+0000bbe0: 0000 72e0 0100 0072 e101 0000 72e2 0100  ..r....r....r...
+0000bbf0: 0072 e301 0000 72e4 0100 0072 e501 0000  .r....r....r....
+0000bc00: 72e6 0100 0072 e701 0000 72e8 0100 0072  r....r....r....r
+0000bc10: e901 0000 72ea 0100 0072 eb01 0000 72ec  ....r....r....r.
+0000bc20: 0100 0072 ed01 0000 72ee 0100 0072 ef01  ...r....r....r..
+0000bc30: 0000 72f0 0100 0072 f101 0000 72f2 0100  ..r....r....r...
+0000bc40: 007a 4f4e 6f20 7072 6574 7261 696e 6564  .zONo pretrained
+0000bc50: 206d 6f64 656c 2066 6f75 6e64 2066 6f72   model found for
+0000bc60: 2074 6865 2067 6976 656e 2070 6172 616d   the given param
+0000bc70: 6574 6572 732e 2050 6c65 6173 6520 7472  eters. Please tr
+0000bc80: 6169 6e20 6120 6d6f 6465 6c20 6669 7273  ain a model firs
+0000bc90: 742e 290d 721e 0000 0072 1f00 0000 7220  t.).r....r....r 
+0000bca0: 0000 0072 2400 0000 7231 0100 0072 5801  ...r$...r1...rX.
+0000bcb0: 0000 72a3 0000 0072 5b00 0000 7282 0000  ..r....r[...r...
+0000bcc0: 00da 0b6d 6f64 656c 5f75 7469 6c73 da17  ...model_utils..
+0000bcd0: 656d 6265 6464 696e 675f 6d6f 6465 6c5f  embedding_model_
+0000bce0: 6669 7474 696e 6772 c800 0000 7275 0100  fittingr....ru..
+0000bcf0: 0029 1f72 5700 0000 72d9 0100 0072 a001  .).rW...r....r..
+0000bd00: 0000 72da 0100 0072 db01 0000 72dc 0100  ..r....r....r...
+0000bd10: 0072 dd01 0000 72de 0100 0072 df01 0000  .r....r....r....
+0000bd20: 72e0 0100 0072 e101 0000 72e2 0100 0072  r....r....r....r
+0000bd30: e301 0000 72e4 0100 0072 e501 0000 72e6  ....r....r....r.
+0000bd40: 0100 0072 e701 0000 72e8 0100 0072 e901  ...r....r....r..
+0000bd50: 0000 72ea 0100 0072 eb01 0000 72ec 0100  ..r....r....r...
+0000bd60: 0072 ed01 0000 72ee 0100 0072 ef01 0000  .r....r....r....
+0000bd70: 72f0 0100 0072 f101 0000 72f2 0100 0072  r....r....r....r
+0000bd80: a101 0000 da0f 7072 6574 7261 696e 6564  ......pretrained
+0000bd90: 5f70 6174 6872 4600 0000 7227 0000 0072  _pathrF...r'...r
+0000bda0: f601 0000 7228 0000 00da 1b64 6565 705f  ....r(.....deep_
+0000bdb0: 756e 7375 7065 7276 6973 6564 5f65 6d62  unsupervised_emb
+0000bdc0: 6564 6469 6e67 0d06 0000 7376 0000 0000  edding....sv....
+0000bdd0: 4204 0106 0104 0104 0102 0102 fc04 0606  B...............
+0000bde0: 0102 0308 ff06 0210 0208 fe04 0702 f902  ................
+0000bdf0: fb04 1002 0108 0102 0102 0102 0102 0102  ................
+0000be00: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+0000be10: 0102 0102 0102 0106 0104 0104 0102 0102  ................
+0000be20: fc02 0602 0102 0102 0102 0102 0102 0102  ................
+0000be30: 0102 0102 0102 e004 2102 df0a 230c 0102  ........!...#...
+0000be40: 0102 ff0a 057a 2743 6f6f 7264 696e 6174  .....z'Coordinat
+0000be50: 6573 2e64 6565 705f 756e 7375 7065 7276  es.deep_unsuperv
+0000be60: 6973 6564 5f65 6d62 6564 6469 6e67 2908  ised_embedding).
+0000be70: 4646 7201 0000 0046 544e 4646 2905 7201  FFr....FTNFF).r.
+0000be80: 0000 004e 5446 4629 0546 7201 0000 004e  ...NTFF).Fr....N
+0000be90: 4646 2902 7201 0000 0072 5800 0000 2901  FF).r....rX...).
+0000bea0: 4629 034e 4e54 2902 4e54 2906 4e4e 4646  F).NNT).NT).NNFF
+0000beb0: 4e54 291a 4e72 d001 0000 72d1 0100 0072  NT).Nr....r....r
+0000bec0: d201 0000 72d3 0100 0072 d401 0000 5446  ....r....r....TF
+0000bed0: 72d5 0100 0072 ad00 0000 72bc 0100 0072  r....r....r....r
+0000bee0: d601 0000 72d7 0100 0072 bc01 0000 72bc  ....r....r....r.
+0000bef0: 0100 0072 2d00 0000 4646 5446 7201 0000  ...r-...FFTFr...
+0000bf00: 0072 d801 0000 72b1 0000 0072 ad00 0000  .r....r....r....
+0000bf10: 4672 ad00 0000 2927 7259 0000 0072 2a01  Fr....)'rY...r*.
+0000bf20: 0000 722b 0100 0072 2c01 0000 72d2 0000  ..r+...r,...r...
+0000bf30: 0072 a300 0000 72de 0000 0072 df00 0000  .r....r....r....
+0000bf40: 722e 0100 00da 076e 6461 7272 6179 7221  r......ndarrayr!
+0000bf50: 0100 0072 1400 0000 729d 0100 00da 0547  ...r....r......G
+0000bf60: 7261 7068 72b6 0000 0072 6a00 0000 726e  raphr....rj...rn
+0000bf70: 0000 0072 6f00 0000 722d 0100 0072 1300  ...ro...r-...r..
+0000bf80: 0000 da0a 7461 626c 655f 6469 6374 726c  ....table_dictrl
+0000bf90: 0100 0072 fa00 0000 7205 0100 0072 1801  ...r....r....r..
+0000bfa0: 0000 7279 0100 0072 2f01 0000 727a 0100  ..ry...r/...rz..
+0000bfb0: 0072 7e01 0000 7260 0100 0072 8400 0000  .r~...r`...r....
+0000bfc0: 7288 0100 0072 2501 0000 72af 0100 00da  r....r%...r.....
+0000bfd0: 0369 6e66 72cf 0100 0072 1500 0000 72c1  .infr....r....r.
+0000bfe0: 0000 0072 fa01 0000 7227 0000 0072 2700  ...r....r'...r'.
+0000bff0: 0000 7227 0000 0072 2800 0000 721b 0000  ..r'...r(...r...
+0000c000: 00db 0200 0073 6601 0000 0801 0412 0201  .....sf.........
+0000c010: 0801 0201 0201 0201 0201 02ea 0202 0201  ................
+0000c020: 0201 0201 0401 0201 0201 0201 0401 0201  ................
+0000c030: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+0000c040: 0201 0401 0201 02ea 0c47 0804 0806 0001  .........G......
+0000c050: 0001 0001 0001 0001 0001 0001 00f7 0202  ................
+0000c060: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+0000c070: 02f6 0c7f 002e 0001 0001 0001 0001 00fa  ................
+0000c080: 0202 0201 0201 0201 0201 0201 02f9 0c55  ...............U
+0000c090: 0001 0001 0001 0001 00fa 0202 0201 0201  ................
+0000c0a0: 0201 0201 0201 02f9 0c42 143a 1007 0201  .........B.:....
+0000c0b0: 0a04 0810 0804 0201 0a05 00ff 0201 06ff  ................
+0000c0c0: 0c2f 1216 0001 0001 0001 0001 0001 00f9  ./..............
+0000c0d0: 0202 0201 0201 0201 0201 0201 0202 02f7  ................
+0000c0e0: 0c7f 000d 0201 0201 0401 0201 0201 02f9  ................
+0000c0f0: 0202 0201 0201 0201 0201 0201 0201 02f8  ................
+0000c100: 0c77 0001 0001 0001 0001 0001 0001 0001  .w..............
+0000c110: 0001 0001 0001 0001 0001 0001 0001 0001  ................
+0000c120: 0001 0001 0001 0001 0001 0001 0001 0001  ................
+0000c130: 0001 0001 00e4 0202 1601 0401 0201 0201  ................
+0000c140: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+0000c150: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+0000c160: 0201 0201 0201 0201 0201 0201 0202 02e2  ................
+0000c170: 721b 0000 0063 0000 0000 0000 0000 0000  r....c..........
+0000c180: 0000 0000 0000 0e00 0000 0000 0000 735c  ..............s\
+0000c190: 0100 0065 005a 0164 005a 0264 015a 0364  ...e.Z.d.Z.d.Z.d
+0000c1a0: 0264 0265 0464 0367 0183 0164 0264 0264  .d.e.d.g...d.d.d
+0000c1b0: 0264 0264 0464 0466 0965 0565 0665 0665  .d.d.d.f.e.e.e.e
+0000c1c0: 076a 0865 0965 0665 0a6a 0b65 0c65 0d65  .j.e.e.e.j.e.e.e
+0000c1d0: 0c65 0e65 0565 0c66 0219 0064 059c 0b87  .e.e.e.f...d....
+0000c1e0: 0066 0164 0664 0784 0d5a 0f65 1065 1164  .f.d.d...Z.e.e.d
+0000c1f0: 089c 0264 0964 0a84 045a 1265 0d65 1164  ...d.d...Z.e.e.d
+0000c200: 0b9c 0264 0c64 0d84 045a 1365 076a 1464  ...d.d...Z.e.j.d
+0000c210: 0e9c 0164 0f64 1084 045a 1564 3065 0665  ...d.d...Z.d0e.e
+0000c220: 1665 0665 1765 1865 1866 0219 0064 129c  .e.e.e.e.f...d..
+0000c230: 0464 1364 1484 055a 1964 3165 1665 0665  .d.d...Z.d1e.e.e
+0000c240: 1765 1865 1866 0219 0064 169c 0364 1764  .e.e.f...d...d.d
+0000c250: 1884 055a 1a64 3265 1665 0665 1765 1865  ...Z.d2e.e.e.e.e
+0000c260: 1866 0219 0064 169c 0364 1964 1a84 055a  .f...d...d.d...Z
+0000c270: 1b64 3365 1665 1765 1865 1866 0219 0064  .d3e.e.e.e.f...d
+0000c280: 1b9c 0264 1c64 1d84 055a 1c64 3465 0665  ...d.d...Z.d4e.e
+0000c290: 1164 1e9c 0264 1f64 2084 055a 1d64 0464  .d...d.d ..Z.d.d
+0000c2a0: 219c 0164 2264 2384 025a 1e64 3565 1165  !..d"d#..Z.d5e.e
+0000c2b0: 1665 0464 259c 0364 2664 2784 055a 1f64  .e.d%..d&d'..Z.d
+0000c2c0: 3665 0665 1665 1665 0665 1865 1665 1665  6e.e.e.e.e.e.e.e
+0000c2d0: 0c65 0c65 1665 0d65 076a 1464 2d9c 0c64  .e.e.e.e.j.d-..d
+0000c2e0: 2e64 2f84 055a 2087 0004 005a 2153 0029  .d/..Z ....Z!S.)
+0000c2f0: 3772 db00 0000 7ae5 4d61 696e 2063 6c61  7r....z.Main cla
+0000c300: 7373 2066 6f72 2073 746f 7269 6e67 2061  ss for storing a
+0000c310: 2073 696e 676c 6520 6461 7461 7365 7420   single dataset 
+0000c320: 6173 2061 2064 6963 7469 6f6e 6172 7920  as a dictionary 
+0000c330: 7769 7468 2069 6e64 6976 6964 7561 6c73  with individuals
+0000c340: 2061 7320 6b65 7973 2061 6e64 2070 616e   as keys and pan
+0000c350: 6461 732e 4461 7461 4672 616d 6573 2061  das.DataFrames a
+0000c360: 7320 7661 6c75 6573 2e0a 0a20 2020 2049  s values...    I
+0000c370: 6e63 6c75 6465 7320 6d65 7468 6f64 7320  ncludes methods 
+0000c380: 666f 7220 6765 6e65 7261 7469 6e67 2074  for generating t
+0000c390: 7261 696e 696e 6720 616e 6420 7465 7374  raining and test
+0000c3a0: 696e 6720 6461 7461 7365 7473 2066 6f72  ing datasets for
+0000c3b0: 2074 6865 2073 7570 6572 7669 7365 6420   the supervised 
+0000c3c0: 616e 6420 756e 7375 7065 7276 6973 6564  and unsupervised
+0000c3d0: 206d 6f64 656c 732e 0a20 2020 204e 722d   models..    Nr-
+0000c3e0: 0000 0046 290b 7262 0100 0072 b000 0000  ...F).rb...r....
+0000c3f0: 7235 0000 0072 6000 0000 7234 0000 0072  r5...r`...r4...r
+0000c400: 4401 0000 7264 0000 0072 4501 0000 7239  D...rd...rE...r9
+0000c410: 0000 0072 4a01 0000 724b 0100 0063 0c00  ...rJ...rK...c..
+0000c420: 0000 0000 0000 0000 0000 0c00 0000 0300  ................
+0000c430: 0000 0300 0000 734c 0000 0074 0083 00a0  ......sL...t....
+0000c440: 017c 01a1 0101 007c 027c 005f 027c 067c  .|.....|.|._.|.|
+0000c450: 005f 037c 077c 005f 047c 087c 005f 057c  ._.|.|._.|.|._.|
+0000c460: 037c 005f 067c 047c 005f 077c 057c 005f  .|._.|.|._.|.|._
+0000c470: 087c 097c 005f 097c 0a7c 005f 0a7c 0b7c  .|.|._.|.|._.|.|
+0000c480: 005f 0b64 0153 0029 0261 f604 0000 5374  ._.d.S.).a....St
+0000c490: 6f72 6520 7369 6e67 6c65 2064 6174 6173  ore single datas
+0000c4a0: 6574 7320 6173 2064 6963 7469 6f6e 6172  ets as dictionar
+0000c4b0: 6965 7320 7769 7468 2069 6e64 6976 6964  ies with individ
+0000c4c0: 7561 6c73 2061 7320 6b65 7973 2061 6e64  uals as keys and
+0000c4d0: 2070 616e 6461 732e 4461 7461 4672 616d   pandas.DataFram
+0000c4e0: 6573 2061 7320 7661 6c75 6573 2e0a 0a20  es as values... 
+0000c4f0: 2020 2020 2020 2049 6e63 6c75 6465 7320         Includes 
+0000c500: 6d65 7468 6f64 7320 666f 7220 6765 6e65  methods for gene
+0000c510: 7261 7469 6e67 2074 7261 696e 696e 6720  rating training 
+0000c520: 616e 6420 7465 7374 696e 6720 6461 7461  and testing data
+0000c530: 7365 7473 2066 6f72 2074 6865 2061 7574  sets for the aut
+0000c540: 6f65 6e63 6f64 6572 732e 0a0a 2020 2020  oencoders...    
+0000c550: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+0000c560: 2020 2020 2020 7461 6273 2028 4469 6374        tabs (Dict
+0000c570: 293a 2044 6963 7469 6f6e 6172 7920 6f66  ): Dictionary of
+0000c580: 2070 616e 6461 732e 4461 7461 4672 616d   pandas.DataFram
+0000c590: 6573 2077 6974 6820 696e 6469 7669 6475  es with individu
+0000c5a0: 616c 2065 7870 6572 696d 656e 7473 2061  al experiments a
+0000c5b0: 7320 6b65 7973 2e0a 2020 2020 2020 2020  s keys..        
+0000c5c0: 2020 2020 7479 7020 2873 7472 293a 2054      typ (str): T
+0000c5d0: 7970 6520 6f66 2074 6865 2064 6174 6173  ype of the datas
+0000c5e0: 6574 2e20 4578 616d 706c 6573 2061 7265  et. Examples are
+0000c5f0: 2022 636f 6f72 6473 222c 2022 6469 7374   "coords", "dist
+0000c600: 7322 2c20 616e 6420 2261 6e67 6c65 7322  s", and "angles"
+0000c610: 2e20 466f 7220 6c6f 6767 696e 6720 7075  . For logging pu
+0000c620: 7270 6f73 6573 206f 6e6c 792e 0a20 2020  rposes only..   
+0000c630: 2020 2020 2020 2020 2061 7265 6e61 2028           arena (
+0000c640: 7374 7229 3a20 5479 7065 206f 6620 7468  str): Type of th
+0000c650: 6520 6172 656e 612e 204d 7573 7420 6265  e arena. Must be
+0000c660: 206f 6e65 206f 6620 2263 6972 6375 6c61   one of "circula
+0000c670: 722d 6175 746f 6465 7465 6374 222c 2022  r-autodetect", "
+0000c680: 6369 7263 756c 6172 2d6d 616e 7561 6c22  circular-manual"
+0000c690: 2c20 6f72 2022 706f 6c79 676f 6e2d 6d61  , or "polygon-ma
+0000c6a0: 6e75 616c 222e 2048 616e 646c 6564 2069  nual". Handled i
+0000c6b0: 6e74 6572 6e61 6c6c 792e 0a20 2020 2020  nternally..     
+0000c6c0: 2020 2020 2020 2061 7265 6e61 5f64 696d         arena_dim
+0000c6d0: 7320 286e 702e 6172 7261 7929 3a20 4469  s (np.array): Di
+0000c6e0: 6d65 6e73 696f 6e73 206f 6620 7468 6520  mensions of the 
+0000c6f0: 6172 656e 6120 696e 206d 6d2e 0a20 2020  arena in mm..   
+0000c700: 2020 2020 2020 2020 2061 6e69 6d61 6c5f           animal_
+0000c710: 6964 7320 286c 6973 7429 3a20 6c69 7374  ids (list): list
+0000c720: 206f 6620 616e 696d 616c 2069 6473 2e0a   of animal ids..
+0000c730: 2020 2020 2020 2020 2020 2020 6365 6e74              cent
+0000c740: 6572 2028 7374 7229 3a20 5479 7065 206f  er (str): Type o
+0000c750: 6620 7468 6520 6365 6e74 6572 2e20 4861  f the center. Ha
+0000c760: 6e64 6c65 6420 696e 7465 726e 616c 6c79  ndled internally
+0000c770: 2e0a 2020 2020 2020 2020 2020 2020 706f  ..            po
+0000c780: 6c61 7220 2862 6f6f 6c29 3a20 5768 6574  lar (bool): Whet
+0000c790: 6865 7220 7468 6520 6461 7461 7365 7420  her the dataset 
+0000c7a0: 6973 2069 6e20 706f 6c61 7220 636f 6f72  is in polar coor
+0000c7b0: 6469 6e61 7465 732e 2048 616e 646c 6564  dinates. Handled
+0000c7c0: 2069 6e74 6572 6e61 6c6c 792e 0a20 2020   internally..   
+0000c7d0: 2020 2020 2020 2020 2065 7870 5f63 6f6e           exp_con
+0000c7e0: 6469 7469 6f6e 7320 2864 6963 7429 3a20  ditions (dict): 
+0000c7f0: 6469 6374 696f 6e61 7279 2077 6974 6820  dictionary with 
+0000c800: 6578 7065 7269 6d65 6e74 2049 4473 2061  experiment IDs a
+0000c810: 7320 6b65 7973 2061 6e64 2065 7870 6572  s keys and exper
+0000c820: 696d 656e 7461 6c20 636f 6e64 6974 696f  imental conditio
+0000c830: 6e73 2061 7320 7661 6c75 6573 2e0a 2020  ns as values..  
+0000c840: 2020 2020 2020 2020 2020 7072 6f70 6167            propag
+0000c850: 6174 655f 6c61 6265 6c73 2028 626f 6f6c  ate_labels (bool
+0000c860: 293a 2057 6865 7468 6572 2074 6f20 7072  ): Whether to pr
+0000c870: 6f70 6167 6174 6520 7068 656e 6f74 7970  opagate phenotyp
+0000c880: 6963 206c 6162 656c 7320 6672 6f6d 2074  ic labels from t
+0000c890: 6865 206f 7269 6769 6e61 6c20 6578 7065  he original expe
+0000c8a0: 7269 6d65 6e74 7320 746f 2074 6865 2074  riments to the t
+0000c8b0: 7261 6e73 666f 726d 6564 2064 6174 6173  ransformed datas
+0000c8c0: 6574 2e0a 2020 2020 2020 2020 2020 2020  et..            
+0000c8d0: 7072 6f70 6167 6174 655f 616e 6e6f 7461  propagate_annota
+0000c8e0: 7469 6f6e 7320 2844 6963 7429 3a20 4469  tions (Dict): Di
+0000c8f0: 6374 696f 6e61 7279 206f 6620 616e 6e6f  ctionary of anno
+0000c900: 7461 7469 6f6e 7320 746f 2070 726f 7061  tations to propa
+0000c910: 6761 7465 2e20 4966 2070 726f 7669 6465  gate. If provide
+0000c920: 642c 2074 6865 2073 7570 6572 7669 7365  d, the supervise
+0000c930: 6420 616e 6e6f 7461 7469 6f6e 7320 6f66  d annotations of
+0000c940: 2074 6865 2069 6e64 6976 6964 7561 6c20   the individual 
+0000c950: 6578 7065 7269 6d65 6e74 7320 6172 6520  experiments are 
+0000c960: 7072 6f70 6167 6174 6564 2074 6f20 7468  propagated to th
+0000c970: 6520 6461 7461 7365 742e 0a0a 2020 2020  e dataset...    
+0000c980: 2020 2020 4e29 0cda 0573 7570 6572 726a      N)...superrj
+0000c990: 0000 00da 055f 7479 7065 da07 5f63 656e  ....._type.._cen
+0000c9a0: 7465 7272 4201 0000 da06 5f70 6f6c 6172  terrB....._polar
+0000c9b0: 7233 0100 0072 3501 0000 7232 0100 0072  r3...r5...r2...r
+0000c9c0: 3801 0000 da11 5f70 726f 7061 6761 7465  8....._propagate
+0000c9d0: 5f6c 6162 656c 73da 165f 7072 6f70 6167  _labels.._propag
+0000c9e0: 6174 655f 616e 6e6f 7461 7469 6f6e 7329  ate_annotations)
+0000c9f0: 0c72 5700 0000 7262 0100 0072 b000 0000  .rW...rb...r....
+0000ca00: 7235 0000 0072 6000 0000 7234 0000 0072  r5...r`...r4...r
+0000ca10: 4401 0000 7264 0000 0072 4501 0000 7239  D...rd...rE...r9
+0000ca20: 0000 0072 4a01 0000 724b 0100 00a9 01da  ...rJ...rK......
+0000ca30: 095f 5f63 6c61 7373 5f5f 7227 0000 0072  .__class__r'...r
+0000ca40: 2800 0000 726a 0000 0099 0600 0073 1600  (...rj.......s..
+0000ca50: 0000 001f 0c01 0601 0601 0601 0601 0601  ................
+0000ca60: 0601 0601 0601 0601 7a12 5461 626c 6544  ........z.TableD
+0000ca70: 6963 742e 5f5f 696e 6974 5f5f 2902 72f6  ict.__init__).r.
+0000ca80: 0000 0072 1a00 0000 6302 0000 0000 0000  ...r....c.......
+0000ca90: 0000 0000 0002 0000 0008 0000 0003 0000  ................
+0000caa0: 0073 5c00 0000 7400 6a01 a002 7c00 a101  .s\...t.j...|...
+0000cab0: 8901 7403 a004 8701 6601 6401 6402 8408  ..t.....f.d.d...
+0000cac0: 8800 4400 8301 a101 732c 4a00 6403 8301  ..D.....s,J.d...
+0000cad0: 8201 7405 8700 6601 6404 6405 8408 8801  ..t...f.d.d.....
+0000cae0: a006 a100 4400 8301 7c00 6a07 7c00 6a08  ....D...|.j.|.j.
+0000caf0: 7c00 6a09 7c00 6a0a 7c00 6a0b 6406 8d06  |.j.|.j.|.j.d...
+0000cb00: 5300 2907 616e 0100 0052 6574 7572 6e20  S.).an...Return 
+0000cb10: 6120 7375 6273 6574 206f 6620 7468 6520  a subset of the 
+0000cb20: 6f72 6967 696e 616c 2074 6162 6c65 5f64  original table_d
+0000cb30: 6963 7420 6f62 6a65 6374 2c20 636f 6e74  ict object, cont
+0000cb40: 6169 6e69 6e67 206f 6e6c 7920 7468 6520  aining only the 
+0000cb50: 7370 6563 6966 6965 6420 6b65 7973 2e0a  specified keys..
+0000cb60: 0a20 2020 2020 2020 2055 7365 6675 6c2c  .        Useful,
+0000cb70: 2066 6f72 2065 7861 6d70 6c65 2c20 746f   for example, to
+0000cb80: 2073 656c 6563 7420 6461 7461 2063 6f6d   select data com
+0000cb90: 696e 6720 6672 6f6d 2076 6964 656f 7320  ing from videos 
+0000cba0: 6f66 2061 2073 7065 6369 6669 6564 2063  of a specified c
+0000cbb0: 6f6e 6469 7469 6f6e 2e0a 0a20 2020 2020  ondition...     
+0000cbc0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+0000cbd0: 2020 2020 206b 6579 7320 286c 6973 7429       keys (list)
+0000cbe0: 3a20 4c69 7374 206f 6620 6b65 7973 2074  : List of keys t
+0000cbf0: 6f20 6b65 6570 2e0a 0a20 2020 2020 2020  o keep...       
+0000cc00: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+0000cc10: 2020 2020 2020 5461 626c 6544 6963 743a        TableDict:
+0000cc20: 2053 7562 7365 7420 6f66 2074 6865 206f   Subset of the o
+0000cc30: 7269 6769 6e61 6c20 7461 626c 655f 6469  riginal table_di
+0000cc40: 6374 206f 626a 6563 742c 2063 6f6e 7461  ct object, conta
+0000cc50: 696e 696e 6720 6f6e 6c79 2074 6865 2073  ining only the s
+0000cc60: 7065 6369 6669 6564 206b 6579 732e 0a20  pecified keys.. 
+0000cc70: 2020 2020 2020 2063 0100 0000 0000 0000         c........
+0000cc80: 0000 0000 0200 0000 0500 0000 1300 0000  ................
+0000cc90: 7318 0000 0067 007c 005d 107d 017c 0188  s....g.|.].}.|..
+0000cca0: 00a0 00a1 0076 0091 0271 0453 0072 2700  .....v...q.S.r'.
+0000ccb0: 0000 a901 72f6 0000 0029 0272 4b00 0000  ....r....).rK...
+0000ccc0: 72ed 0000 0029 01da 0574 6162 6c65 7227  r....)...tabler'
+0000ccd0: 0000 0072 2800 0000 724d 0000 00d0 0600  ...r(...rM......
+0000cce0: 0072 4e00 0000 7a2b 5461 626c 6544 6963  .rN...z+TableDic
+0000ccf0: 742e 6669 6c74 6572 5f76 6964 656f 732e  t.filter_videos.
+0000cd00: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
+0000cd10: 6d70 3e7a 1549 6e76 616c 6964 206b 6579  mp>z.Invalid key
+0000cd20: 7320 7365 6c65 6374 6564 6301 0000 0000  s selectedc.....
+0000cd30: 0000 0000 0000 0003 0000 0004 0000 0013  ................
+0000cd40: 0000 0073 1e00 0000 6900 7c00 5d16 5c02  ...s....i.|.].\.
+0000cd50: 7d01 7d02 7c01 8800 7600 7204 7c01 7c02  }.}.|...v.r.|.|.
+0000cd60: 9302 7104 5300 7227 0000 0072 2700 0000  ..q.S.r'...r'...
+0000cd70: a903 724b 0000 0072 ed00 0000 7229 0100  ..rK...r....r)..
+0000cd80: 0072 0702 0000 7227 0000 0072 2800 0000  .r....r'...r(...
+0000cd90: 7298 0000 00d3 0600 0072 4e00 0000 7a2b  r........rN...z+
+0000cda0: 5461 626c 6544 6963 742e 6669 6c74 6572  TableDict.filter
+0000cdb0: 5f76 6964 656f 732e 3c6c 6f63 616c 733e  _videos.<locals>
+0000cdc0: 2e3c 6469 6374 636f 6d70 3ea9 0472 6400  .<dictcomp>..rd.
+0000cdd0: 0000 724a 0100 0072 4b01 0000 7239 0000  ..rJ...rK...r9..
+0000cde0: 0029 0c72 8200 0000 7283 0000 0072 5301  .).r....r....rS.
+0000cdf0: 0000 72de 0000 0072 5800 0000 72db 0000  ..r....rX...r...
+0000ce00: 0072 cc00 0000 7200 0200 0072 4201 0000  .r....r....rB...
+0000ce10: 7203 0200 0072 0402 0000 7238 0100 0029  r....r....r8...)
+0000ce20: 0272 5700 0000 72f6 0000 0072 2700 0000  .rW...r....r'...
+0000ce30: 2902 72f6 0000 0072 0802 0000 7228 0000  ).r....r....r(..
+0000ce40: 00da 0d66 696c 7465 725f 7669 6465 6f73  ...filter_videos
+0000ce50: c406 0000 7314 0000 0000 0b0c 0120 0202  ....s........ ..
+0000ce60: 0114 0104 0104 0104 0104 0104 fa7a 1754  .............z.T
+0000ce70: 6162 6c65 4469 6374 2e66 696c 7465 725f  ableDict.filter_
+0000ce80: 7669 6465 6f73 2902 da0b 6578 705f 6669  videos)...exp_fi
+0000ce90: 6c74 6572 7372 1a00 0000 6302 0000 0000  ltersr....c.....
+0000cea0: 0000 0000 0000 0003 0000 000a 0000 0003  ................
+0000ceb0: 0000 0073 6c00 0000 7400 6a01 a002 8803  ...sl...t.j.....
+0000cec0: a101 7d02 7c01 a003 a100 4400 5d52 5c02  ..}.|.....D.]R\.
+0000ced0: 8900 8901 8700 8701 8703 6603 6401 6402  ..........f.d.d.
+0000cee0: 8408 7c02 a003 a100 4400 8301 8902 7404  ..|.....D.....t.
+0000cef0: 8802 8803 6a05 8803 6a06 8803 6a07 8803  ....j...j...j...
+0000cf00: 6a08 8702 6601 6403 6402 8408 8803 6a09  j...f.d.d.....j.
+0000cf10: a003 a100 4400 8301 6404 8d06 7d02 7114  ....D...d...}.q.
+0000cf20: 7c02 5300 2905 615c 0100 0052 6574 7572  |.S.).a\...Retur
+0000cf30: 6e20 6120 7375 6273 6574 206f 6620 7468  n a subset of th
+0000cf40: 6520 6f72 6967 696e 616c 2074 6162 6c65  e original table
+0000cf50: 5f64 6963 7420 6f62 6a65 6374 2c20 636f  _dict object, co
+0000cf60: 6e74 6169 6e69 6e67 206f 6e6c 7920 7669  ntaining only vi
+0000cf70: 6465 6f73 2062 656c 6f6e 6769 6e67 2074  deos belonging t
+0000cf80: 6f20 7468 6520 7370 6563 6966 6965 6420  o the specified 
+0000cf90: 6578 7065 7269 6d65 6e74 616c 2063 6f6e  experimental con
+0000cfa0: 6469 7469 6f6e 2e0a 0a20 2020 2020 2020  dition...       
+0000cfb0: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+0000cfc0: 2020 2065 7870 5f66 696c 7465 7273 2028     exp_filters (
+0000cfd0: 6469 6374 293a 2065 7870 6572 696d 656e  dict): experimen
+0000cfe0: 7461 6c20 636f 6e64 6974 696f 6e73 2061  tal conditions a
+0000cff0: 6e64 2076 616c 7565 7320 746f 2066 696c  nd values to fil
+0000d000: 7465 7220 6f6e 2e0a 0a20 2020 2020 2020  ter on...       
+0000d010: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+0000d020: 2020 2020 2020 5461 626c 6544 6963 743a        TableDict:
+0000d030: 2053 7562 7365 7420 6f66 2074 6865 206f   Subset of the o
+0000d040: 7269 6769 6e61 6c20 7461 626c 655f 6469  riginal table_di
+0000d050: 6374 206f 626a 6563 742c 2063 6f6e 7461  ct object, conta
+0000d060: 696e 696e 6720 6f6e 6c79 2074 6865 2073  ining only the s
+0000d070: 7065 6369 6669 6564 206b 6579 732e 0a20  pecified keys.. 
+0000d080: 2020 2020 2020 2063 0100 0000 0000 0000         c........
+0000d090: 0000 0000 0300 0000 0400 0000 1300 0000  ................
+0000d0a0: 732a 0000 0069 007c 005d 225c 027d 017d  s*...i.|.]"\.}.}
+0000d0b0: 0288 026a 007c 0119 0088 0019 006a 0188  ...j.|.......j..
+0000d0c0: 016b 0272 047c 017c 0293 0271 0453 0072  .k.r.|.|...q.S.r
+0000d0d0: 2700 0000 2902 7238 0100 0072 c900 0000  '...).r8...r....
+0000d0e0: 7209 0200 0029 03da 0d65 7870 5f63 6f6e  r....)...exp_con
+0000d0f0: 6469 7469 6f6e da09 6578 705f 7661 6c75  dition..exp_valu
+0000d100: 6572 5700 0000 7227 0000 0072 2800 0000  erW...r'...r(...
+0000d110: 7298 0000 00e8 0600 0073 0600 0000 0602  r........s......
+0000d120: 0601 14fe 7a2e 5461 626c 6544 6963 742e  ....z.TableDict.
+0000d130: 6669 6c74 6572 5f63 6f6e 6469 7469 6f6e  filter_condition
+0000d140: 2e3c 6c6f 6361 6c73 3e2e 3c64 6963 7463  .<locals>.<dictc
+0000d150: 6f6d 703e 6301 0000 0000 0000 0000 0000  omp>c...........
+0000d160: 0003 0000 0005 0000 0013 0000 0073 2200  .............s".
+0000d170: 0000 6900 7c00 5d1a 5c02 7d01 7d02 7c01  ..i.|.].\.}.}.|.
+0000d180: 8800 a000 a100 7600 7204 7c01 7c02 9302  ......v.r.|.|...
+0000d190: 7104 5300 7227 0000 0072 0702 0000 7209  q.S.r'...r....r.
+0000d1a0: 0200 0029 01da 0e66 696c 7465 7265 645f  ...)...filtered_
+0000d1b0: 7461 626c 6572 2700 0000 7228 0000 0072  tabler'...r(...r
+0000d1c0: 9800 0000 f306 0000 7306 0000 0006 0206  ........s.......
+0000d1d0: 010c fe72 0a02 0000 290a 7282 0000 0072  ...r....).r....r
+0000d1e0: 8300 0000 7253 0100 0072 cc00 0000 72db  ....rS...r....r.
+0000d1f0: 0000 0072 0002 0000 7242 0100 0072 0302  ...r....rB...r..
+0000d200: 0000 7204 0200 0072 3801 0000 2903 7257  ..r....r8...).rW
+0000d210: 0000 0072 0c02 0000 7208 0200 0072 2700  ...r....r....r'.
+0000d220: 0000 2904 720d 0200 0072 0e02 0000 720f  ..).r....r....r.
+0000d230: 0200 0072 5700 0000 7228 0000 00da 1066  ...rW...r(.....f
+0000d240: 696c 7465 725f 636f 6e64 6974 696f 6edb  ilter_condition.
+0000d250: 0600 0073 2000 0000 0009 0c02 1002 0e02  ...s ...........
+0000d260: 06fe 0605 0201 0201 0401 0401 0401 0401  ................
+0000d270: 0a02 08fe 04fa 080d 7a1a 5461 626c 6544  ........z.TableD
+0000d280: 6963 742e 6669 6c74 6572 5f63 6f6e 6469  ict.filter_condi
+0000d290: 7469 6f6e 2901 721a 0000 0063 0100 0000  tion).r....c....
+0000d2a0: 0000 0000 0000 0000 0300 0000 0500 0000  ................
+0000d2b0: 4300 0000 736c 0000 0064 017d 017c 006a  C...sl...d.}.|.j
+0000d2c0: 0072 3464 0264 0384 007c 00a0 01a1 0044  .r4d.d...|.....D
+0000d2d0: 0083 017d 0174 02a0 0364 0464 0584 007c  ...}.t...d.d...|
+0000d2e0: 01a0 04a1 0044 0083 01a1 017d 0164 0664  .....D.....}.d.d
+0000d2f0: 0384 007c 00a0 01a1 0044 0083 017d 0274  ...|.....D...}.t
+0000d300: 026a 0564 0764 0584 007c 02a0 04a1 0044  .j.d.d...|.....D
+0000d310: 0083 0164 0864 098d 026a 067d 027c 027c  ...d.d...j.}.|.|
+0000d320: 0166 0253 0029 0a7a 7c52 6574 7572 6e20  .f.S.).z|Return 
+0000d330: 6120 6e75 6d70 7920 6e64 6172 7261 7920  a numpy ndarray 
+0000d340: 6672 6f6d 2074 6865 2070 7265 7072 6f63  from the preproc
+0000d350: 6573 7369 6e67 206f 6620 7468 6520 7461  essing of the ta
+0000d360: 626c 655f 6469 6374 206f 626a 6563 742c  ble_dict object,
+0000d370: 2072 6561 6479 2066 6f72 2070 726f 6a65   ready for proje
+0000d380: 6374 696f 6e20 696e 746f 2061 206c 6f77  ction into a low
+0000d390: 6572 2064 696d 656e 7369 6f6e 616c 2073  er dimensional s
+0000d3a0: 7061 6365 2e4e 6301 0000 0000 0000 0000  pace.Nc.........
+0000d3b0: 0000 0003 0000 0005 0000 0053 0000 0073  ...........S...s
+0000d3c0: 1c00 0000 6900 7c00 5d14 5c02 7d01 7d02  ....i.|.].\.}.}.
+0000d3d0: 7c01 7c02 6a00 6400 1900 9302 7104 5300  |.|.j.d.....q.S.
+0000d3e0: a901 2902 7201 0000 0072 9501 0000 7291  ..).r....r....r.
+0000d3f0: 0000 00a9 0372 4b00 0000 72ed 0000 00da  .....rK...r.....
+0000d400: 0176 7227 0000 0072 2700 0000 7228 0000  .vr'...r'...r(..
+0000d410: 0072 9800 0000 0207 0000 724e 0000 007a  .r........rN...z
+0000d420: 3154 6162 6c65 4469 6374 2e5f 7072 6570  1TableDict._prep
+0000d430: 6172 655f 7072 6f6a 6563 7469 6f6e 2e3c  are_projection.<
+0000d440: 6c6f 6361 6c73 3e2e 3c64 6963 7463 6f6d  locals>.<dictcom
+0000d450: 703e 6301 0000 0000 0000 0000 0000 0002  p>c.............
+0000d460: 0000 0003 0000 0053 0000 0073 1000 0000  .......S...s....
+0000d470: 6700 7c00 5d08 7d01 7c01 9102 7104 5300  g.|.].}.|...q.S.
+0000d480: 7227 0000 0072 2700 0000 2902 724b 0000  r'...r'...).rK..
+0000d490: 0072 f900 0000 7227 0000 0072 2700 0000  .r....r'...r'...
+0000d4a0: 7228 0000 0072 4d00 0000 0307 0000 724e  r(...rM.......rN
+0000d4b0: 0000 007a 3154 6162 6c65 4469 6374 2e5f  ...z1TableDict._
+0000d4c0: 7072 6570 6172 655f 7072 6f6a 6563 7469  prepare_projecti
+0000d4d0: 6f6e 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  on.<locals>.<lis
+0000d4e0: 7463 6f6d 703e 6301 0000 0000 0000 0000  tcomp>c.........
+0000d4f0: 0000 0003 0000 0007 0000 0053 0000 0073  ...........S...s
+0000d500: 2000 0000 6900 7c00 5d18 5c02 7d01 7d02   ...i.|.].\.}.}.
+0000d510: 7c01 7400 6a01 7c02 6400 6401 8d02 9302  |.t.j.|.d.d.....
+0000d520: 7104 5300 2902 7201 0000 0072 ac00 0000  q.S.).r....r....
+0000d530: 2902 72de 0000 00da 046d 6561 6e72 1202  ).r......meanr..
+0000d540: 0000 7227 0000 0072 2700 0000 7228 0000  ..r'...r'...r(..
+0000d550: 0072 9800 0000 0507 0000 724e 0000 0063  .r........rN...c
+0000d560: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+0000d570: 0500 0000 5300 0000 7324 0000 0067 007c  ....S...s$...g.|
+0000d580: 005d 1c7d 0174 00a0 017c 01a1 0164 0064  .].}.t...|...d.d
+0000d590: 0085 0274 006a 0266 0219 0091 0271 0453  ...t.j.f.....q.S
+0000d5a0: 0072 2701 0000 2903 72de 0000 0072 df00  .r'...).r....r..
+0000d5b0: 0000 da07 6e65 7761 7869 7329 0272 4b00  ....newaxis).rK.
+0000d5c0: 0000 da03 6578 7072 2700 0000 7227 0000  ....expr'...r'..
+0000d5d0: 0072 2800 0000 724d 0000 0007 0700 0072  .r(...rM.......r
+0000d5e0: 4e00 0000 7232 0000 0072 ac00 0000 2907  N...r2...r....).
+0000d5f0: 7203 0200 0072 cc00 0000 72de 0000 0072  r....r....r....r
+0000d600: df00 0000 72c9 0000 0072 9b01 0000 72c2  ....r....r....r.
+0000d610: 0000 0029 0372 5700 0000 da06 6c61 6265  ...).rW.....labe
+0000d620: 6c73 da01 5872 2700 0000 7227 0000 0072  ls..Xr'...r'...r
+0000d630: 2800 0000 da13 5f70 7265 7061 7265 5f70  (....._prepare_p
+0000d640: 726f 6a65 6374 696f 6efc 0600 0073 1200  rojection....s..
+0000d650: 0000 0002 0403 0601 1201 1802 1201 0401  ................
+0000d660: 12ff 0804 7a1d 5461 626c 6544 6963 742e  ....z.TableDict.
+0000d670: 5f70 7265 7061 7265 5f70 726f 6a65 6374  _prepare_project
+0000d680: 696f 6e72 9300 0000 2904 da0f 7072 6f6a  ionr....)...proj
+0000d690: 6563 7469 6f6e 5f74 7970 6572 e101 0000  ection_typer....
+0000d6a0: da06 6b65 726e 656c 721a 0000 0063 0400  ..kernelr....c..
+0000d6b0: 0000 0000 0000 0000 0000 0600 0000 0400  ................
+0000d6c0: 0000 4300 0000 7370 0000 007c 00a0 00a1  ..C...sp...|....
+0000d6d0: 005c 027d 047d 057c 0164 016b 0272 2274  .\.}.}.|.d.k.r"t
+0000d6e0: 016a 027c 0264 028d 017d 016e 2a7c 0164  .j.|.d...}.n*|.d
+0000d6f0: 036b 0272 3874 037c 027c 0364 048d 027d  .k.r8t.|.|.d...}
+0000d700: 016e 147c 0164 056b 0272 4c74 046a 057c  .n.|.d.k.rLt.j.|
+0000d710: 0264 028d 017d 017c 01a0 067c 04a1 017d  .d...}.|...|...}
+0000d720: 047c 0564 0675 0172 687c 047c 057c 0166  .|.d.u.rh|.|.|.f
+0000d730: 0353 007c 047c 0166 0253 0029 0761 5602  .S.|.|.f.S.).aV.
+0000d740: 0000 5265 7475 726e 2061 2074 7261 696e  ..Return a train
+0000d750: 696e 6720 7365 7420 6765 6e65 7261 7465  ing set generate
+0000d760: 6420 6672 6f6d 2074 6865 2032 4420 6f72  d from the 2D or
+0000d770: 6967 696e 616c 2064 6174 6120 2874 696d  iginal data (tim
+0000d780: 6520 7820 6665 6174 7572 6573 2920 616e  e x features) an
+0000d790: 6420 6120 7370 6563 6966 6965 6420 7072  d a specified pr
+0000d7a0: 6f6a 6563 7469 6f6e 2074 6f20 616e 206e  ojection to an n
+0000d7b0: 5f63 6f6d 706f 6e65 6e74 7320 7370 6163  _components spac
+0000d7c0: 652e 0a0a 2020 2020 2020 2020 5468 6520  e...        The 
+0000d7d0: 7361 6d70 6c65 2070 6172 616d 6574 6572  sample parameter
+0000d7e0: 2061 6c6c 6f77 7320 7468 6520 7573 6572   allows the user
+0000d7f0: 2074 6f20 7261 6e64 6f6d 6c79 2070 6963   to randomly pic
+0000d800: 6b20 6120 7375 6273 6574 206f 6620 7468  k a subset of th
+0000d810: 6520 6461 7461 2066 6f72 2070 6572 666f  e data for perfo
+0000d820: 726d 616e 6365 206f 7220 7669 7375 616c  rmance or visual
+0000d830: 697a 6174 696f 6e20 7265 6173 6f6e 732e  ization reasons.
+0000d840: 2046 6f72 2069 6e74 6572 6e61 6c20 7573   For internal us
+0000d850: 6167 6520 6f6e 6c79 2e0a 0a20 2020 2020  age only...     
+0000d860: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+0000d870: 2020 2020 2070 726f 6a65 6374 696f 6e5f       projection_
+0000d880: 7479 7065 2028 7374 7229 3a20 5072 6f6a  type (str): Proj
+0000d890: 6563 7469 6f6e 2074 6f20 6265 2075 7365  ection to be use
+0000d8a0: 642e 0a20 2020 2020 2020 2020 2020 206e  d..            n
+0000d8b0: 5f63 6f6d 706f 6e65 6e74 7320 2869 6e74  _components (int
+0000d8c0: 293a 204e 756d 6265 7220 6f66 2063 6f6d  ): Number of com
+0000d8d0: 706f 6e65 6e74 7320 746f 2070 726f 6a65  ponents to proje
+0000d8e0: 6374 2074 6f2e 0a20 2020 2020 2020 2020  ct to..         
+0000d8f0: 2020 206b 6572 6e65 6c20 2873 7472 293a     kernel (str):
+0000d900: 204b 6572 6e65 6c20 746f 2062 6520 7573   Kernel to be us
+0000d910: 6564 2066 6f72 2074 6865 2072 616e 646f  ed for the rando
+0000d920: 6d20 616e 6420 5043 4120 616c 676f 7269  m and PCA algori
+0000d930: 7468 6d73 2e0a 0a20 2020 2020 2020 2052  thms...        R
+0000d940: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+0000d950: 2020 2020 7475 706c 653a 2054 7570 6c65      tuple: Tuple
+0000d960: 2063 6f6e 7461 696e 696e 6720 7072 6f6a   containing proj
+0000d970: 6563 7465 6420 6461 7461 2061 6e64 2070  ected data and p
+0000d980: 726f 6a65 6374 696f 6e20 7479 7065 2e0a  rojection type..
+0000d990: 2020 2020 2020 2020 da06 7261 6e64 6f6d          ..random
+0000d9a0: a901 72e1 0100 00da 0370 6361 a902 72e1  ..r......pca..r.
+0000d9b0: 0100 0072 1b02 0000 da04 756d 6170 4e29  ...r......umapN)
+0000d9c0: 0772 1902 0000 7207 0000 00da 1847 6175  .r....r......Gau
+0000d9d0: 7373 6961 6e52 616e 646f 6d50 726f 6a65  ssianRandomProje
+0000d9e0: 6374 696f 6e72 0800 0000 7220 0200 00da  ctionr....r ....
+0000d9f0: 0455 4d41 50da 0d66 6974 5f74 7261 6e73  .UMAP..fit_trans
+0000da00: 666f 726d 2906 7257 0000 0072 1a02 0000  form).rW...r....
+0000da10: 72e1 0100 0072 1b02 0000 7218 0200 0072  r....r....r....r
+0000da20: 1702 0000 7227 0000 0072 2700 0000 7228  ....r'...r'...r(
+0000da30: 0000 00da 0b5f 7072 6f6a 6563 7469 6f6e  ....._projection
+0000da40: 0c07 0000 731a 0000 0000 120c 0208 0104  ....s...........
+0000da50: 0102 ff08 0308 010e 0108 010c 020a 0208  ................
+0000da60: 010a 027a 1554 6162 6c65 4469 6374 2e5f  ...z.TableDict._
+0000da70: 7072 6f6a 6563 7469 6f6e 72d8 0100 0029  projectionr....)
+0000da80: 0372 e101 0000 721b 0200 0072 1a00 0000  .r....r....r....
+0000da90: 6303 0000 0000 0000 0000 0000 0003 0000  c...............
+0000daa0: 0005 0000 0043 0000 0073 1000 0000 7c00  .....C...s....|.
+0000dab0: 6a00 6401 7c01 7c02 6402 8d03 5300 2903  j.d.|.|.d...S.).
+0000dac0: 6117 0200 0052 6574 7572 6e20 6120 7472  a....Return a tr
+0000dad0: 6169 6e69 6e67 2073 6574 2067 656e 6572  aining set gener
+0000dae0: 6174 6564 2066 726f 6d20 7468 6520 3244  ated from the 2D
+0000daf0: 206f 7269 6769 6e61 6c20 6461 7461 2028   original data (
+0000db00: 7469 6d65 2078 2066 6561 7475 7265 7329  time x features)
+0000db10: 2061 6e64 2061 2072 616e 646f 6d20 7072   and a random pr
+0000db20: 6f6a 6563 7469 6f6e 2074 6f20 6120 6e5f  ojection to a n_
+0000db30: 636f 6d70 6f6e 656e 7473 2073 7061 6365  components space
+0000db40: 2e0a 0a20 2020 2020 2020 2054 6865 2073  ...        The s
+0000db50: 616d 706c 6520 7061 7261 6d65 7465 7220  ample parameter 
+0000db60: 616c 6c6f 7773 2074 6865 2075 7365 7220  allows the user 
+0000db70: 746f 2072 616e 646f 6d6c 7920 7069 636b  to randomly pick
+0000db80: 2061 2073 7562 7365 7420 6f66 2074 6865   a subset of the
+0000db90: 2064 6174 6120 666f 720a 2020 2020 2020   data for.      
+0000dba0: 2020 7065 7266 6f72 6d61 6e63 6520 6f72    performance or
+0000dbb0: 2076 6973 7561 6c69 7a61 7469 6f6e 2072   visualization r
+0000dbc0: 6561 736f 6e73 2e0a 0a20 2020 2020 2020  easons...       
+0000dbd0: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+0000dbe0: 2020 206e 5f63 6f6d 706f 6e65 6e74 7320     n_components 
+0000dbf0: 2869 6e74 293a 204e 756d 6265 7220 6f66  (int): Number of
+0000dc00: 2063 6f6d 706f 6e65 6e74 7320 746f 2070   components to p
+0000dc10: 726f 6a65 6374 2074 6f2e 2044 6566 6175  roject to. Defau
+0000dc20: 6c74 2069 7320 322e 0a20 2020 2020 2020  lt is 2..       
+0000dc30: 2020 2020 206b 6572 6e65 6c20 2873 7472       kernel (str
+0000dc40: 293a 204b 6572 6e65 6c20 746f 2062 6520  ): Kernel to be 
+0000dc50: 7573 6564 2066 6f72 2070 726f 6a65 6374  used for project
+0000dc60: 696f 6e73 2e20 4465 6661 756c 7473 2074  ions. Defaults t
+0000dc70: 6f20 6c69 6e65 6172 2e0a 0a20 2020 2020  o linear...     
+0000dc80: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+0000dc90: 2020 2020 2020 2020 7475 706c 653a 2054          tuple: T
+0000dca0: 7570 6c65 2063 6f6e 7461 696e 696e 6720  uple containing 
+0000dcb0: 7072 6f6a 6563 7465 6420 6461 7461 2061  projected data a
+0000dcc0: 6e64 2070 726f 6a65 6374 696f 6e20 7479  nd projection ty
+0000dcd0: 7065 2e0a 2020 2020 2020 2020 721c 0200  pe..        r...
+0000dce0: 0072 1f02 0000 a901 7224 0200 00a9 0372  .r......r$.....r
+0000dcf0: 5700 0000 72e1 0100 0072 1b02 0000 7227  W...r....r....r'
+0000dd00: 0000 0072 2700 0000 7228 0000 0072 0700  ...r'...r(...r..
+0000dd10: 0000 3007 0000 7302 0000 0000 0f7a 1b54  ..0...s......z.T
+0000dd20: 6162 6c65 4469 6374 2e72 616e 646f 6d5f  ableDict.random_
+0000dd30: 7072 6f6a 6563 7469 6f6e 6303 0000 0000  projectionc.....
+0000dd40: 0000 0000 0000 0003 0000 0005 0000 0043  ...............C
+0000dd50: 0000 0073 1000 0000 7c00 6a00 6401 7c01  ...s....|.j.d.|.
+0000dd60: 7c02 6402 8d03 5300 2903 6114 0200 0052  |.d...S.).a....R
+0000dd70: 6574 7572 6e20 6120 7472 6169 6e69 6e67  eturn a training
+0000dd80: 2073 6574 2067 656e 6572 6174 6564 2066   set generated f
+0000dd90: 726f 6d20 7468 6520 3244 206f 7269 6769  rom the 2D origi
+0000dda0: 6e61 6c20 6461 7461 2028 7469 6d65 2078  nal data (time x
+0000ddb0: 2066 6561 7475 7265 7329 2061 6e64 2061   features) and a
+0000ddc0: 2050 4341 2070 726f 6a65 6374 696f 6e20   PCA projection 
+0000ddd0: 746f 2061 206e 5f63 6f6d 706f 6e65 6e74  to a n_component
+0000dde0: 7320 7370 6163 652e 0a0a 2020 2020 2020  s space...      
+0000ddf0: 2020 5468 6520 7361 6d70 6c65 2070 6172    The sample par
+0000de00: 616d 6574 6572 2061 6c6c 6f77 7320 7468  ameter allows th
+0000de10: 6520 7573 6572 2074 6f20 7261 6e64 6f6d  e user to random
+0000de20: 6c79 2070 6963 6b20 6120 7375 6273 6574  ly pick a subset
+0000de30: 206f 6620 7468 6520 6461 7461 2066 6f72   of the data for
+0000de40: 0a20 2020 2020 2020 2070 6572 666f 726d  .        perform
+0000de50: 616e 6365 206f 7220 7669 7375 616c 697a  ance or visualiz
+0000de60: 6174 696f 6e20 7265 6173 6f6e 732e 0a0a  ation reasons...
+0000de70: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+0000de80: 2020 2020 2020 2020 2020 6e5f 636f 6d70            n_comp
+0000de90: 6f6e 656e 7473 2028 696e 7429 3a20 4e75  onents (int): Nu
+0000dea0: 6d62 6572 206f 6620 636f 6d70 6f6e 656e  mber of componen
+0000deb0: 7473 2074 6f20 7072 6f6a 6563 7420 746f  ts to project to
+0000dec0: 2e20 4465 6661 756c 7420 6973 2032 2e0a  . Default is 2..
+0000ded0: 2020 2020 2020 2020 2020 2020 6b65 726e              kern
+0000dee0: 656c 2028 7374 7229 3a20 4b65 726e 656c  el (str): Kernel
+0000def0: 2074 6f20 6265 2075 7365 6420 666f 7220   to be used for 
+0000df00: 7072 6f6a 6563 7469 6f6e 732e 2044 6566  projections. Def
+0000df10: 6175 6c74 7320 746f 206c 696e 6561 722e  aults to linear.
+0000df20: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+0000df30: 733a 0a20 2020 2020 2020 2020 2020 2074  s:.            t
+0000df40: 7570 6c65 3a20 5475 706c 6520 636f 6e74  uple: Tuple cont
+0000df50: 6169 6e69 6e67 2070 726f 6a65 6374 6564  aining projected
+0000df60: 2064 6174 6120 616e 6420 7072 6f6a 6563   data and projec
+0000df70: 7469 6f6e 2074 7970 652e 0a20 2020 2020  tion type..     
+0000df80: 2020 2072 1e02 0000 721f 0200 0072 2502     r....r....r%.
+0000df90: 0000 7226 0200 0072 2700 0000 7227 0000  ..r&...r'...r'..
+0000dfa0: 0072 2800 0000 721e 0200 0041 0700 0073  .r(...r....A...s
+0000dfb0: 0200 0000 000d 7a0d 5461 626c 6544 6963  ......z.TableDic
+0000dfc0: 742e 7063 6129 0272 e101 0000 721a 0000  t.pca).r....r...
+0000dfd0: 0063 0200 0000 0000 0000 0000 0000 0200  .c..............
+0000dfe0: 0000 0400 0000 4300 0000 730e 0000 007c  ......C...s....|
+0000dff0: 006a 0064 017c 0164 028d 0253 0029 0361  .j.d.|.d...S.).a
+0000e000: 1f02 0000 5265 7475 726e 2061 2074 7261  ....Return a tra
+0000e010: 696e 696e 6720 7365 7420 6765 6e65 7261  ining set genera
+0000e020: 7465 6420 6672 6f6d 2074 6865 2032 4420  ted from the 2D 
+0000e030: 6f72 6967 696e 616c 2064 6174 6120 2874  original data (t
+0000e040: 696d 6520 7820 6665 6174 7572 6573 2920  ime x features) 
+0000e050: 616e 6420 6120 5043 4120 7072 6f6a 6563  and a PCA projec
+0000e060: 7469 6f6e 2074 6f20 6120 6e5f 636f 6d70  tion to a n_comp
+0000e070: 6f6e 656e 7473 2073 7061 6365 2e0a 0a20  onents space... 
+0000e080: 2020 2020 2020 2054 6865 2073 616d 706c         The sampl
+0000e090: 6520 7061 7261 6d65 7465 7220 616c 6c6f  e parameter allo
+0000e0a0: 7773 2074 6865 2075 7365 7220 746f 2072  ws the user to r
+0000e0b0: 616e 646f 6d6c 7920 7069 636b 2061 2073  andomly pick a s
+0000e0c0: 7562 7365 7420 6f66 2074 6865 2064 6174  ubset of the dat
+0000e0d0: 6120 666f 720a 2020 2020 2020 2020 7065  a for.        pe
+0000e0e0: 7266 6f72 6d61 6e63 6520 6f72 2076 6973  rformance or vis
+0000e0f0: 7561 6c69 7a61 7469 6f6e 2072 6561 736f  ualization reaso
+0000e100: 6e73 2e0a 0a20 2020 2020 2020 2041 7267  ns...        Arg
+0000e110: 733a 0a20 2020 2020 2020 2020 2020 206e  s:.            n
+0000e120: 5f63 6f6d 706f 6e65 6e74 7320 2869 6e74  _components (int
+0000e130: 293a 204e 756d 6265 7220 6f66 2063 6f6d  ): Number of com
+0000e140: 706f 6e65 6e74 7320 746f 2070 726f 6a65  ponents to proje
+0000e150: 6374 2074 6f2e 2044 6566 6175 6c74 2069  ct to. Default i
+0000e160: 7320 322e 0a20 2020 2020 2020 2020 2020  s 2..           
+0000e170: 2070 6572 706c 6578 6974 7920 2869 6e74   perplexity (int
+0000e180: 293a 2050 6572 706c 6578 6974 7920 7061  ): Perplexity pa
+0000e190: 7261 6d65 7465 7220 666f 7220 7468 6520  rameter for the 
+0000e1a0: 742d 534e 4520 616c 676f 7269 7468 6d2e  t-SNE algorithm.
+0000e1b0: 2044 6566 6175 6c74 2069 7320 3330 2e0a   Default is 30..
+0000e1c0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+0000e1d0: 3a0a 2020 2020 2020 2020 2020 2020 7475  :.            tu
+0000e1e0: 706c 653a 2054 7570 6c65 2063 6f6e 7461  ple: Tuple conta
+0000e1f0: 696e 696e 6720 7072 6f6a 6563 7465 6420  ining projected 
+0000e200: 6461 7461 2061 6e64 2070 726f 6a65 6374  data and project
+0000e210: 696f 6e20 7479 7065 2e0a 0a20 2020 2020  ion type...     
+0000e220: 2020 2072 2002 0000 721d 0200 0072 2502     r ...r....r%.
+0000e230: 0000 2902 7257 0000 0072 e101 0000 7227  ..).rW...r....r'
+0000e240: 0000 0072 2700 0000 7228 0000 0072 2002  ...r'...r(...r .
+0000e250: 0000 5007 0000 7308 0000 0000 1104 0102  ..P...s.........
+0000e260: 0102 fe7a 0e54 6162 6c65 4469 6374 2e75  ...z.TableDict.u
+0000e270: 6d61 7029 0272 4901 0000 721a 0000 0063  map).rI...r....c
+0000e280: 0200 0000 0000 0000 0000 0000 0500 0000  ................
+0000e290: 0800 0000 0300 0000 736e 0000 007c 00a0  ........sn...|..
+0000e2a0: 00a1 007d 027c 02a0 01a1 0044 005d 3e5c  ...}.|.....D.]>\
+0000e2b0: 027d 037d 0474 026a 03a0 047c 046a 057c  .}.}.t.j...|.j.|
+0000e2c0: 01a1 0289 007c 046a 0664 0164 0185 0287  .....|.j.d.d....
+0000e2d0: 0066 0164 0264 0384 087c 046a 0544 0083  .f.d.d...|.j.D..
+0000e2e0: 0166 0219 007c 027c 033c 0071 1074 077c  .f...|.|.<.q.t.|
+0000e2f0: 027c 006a 087c 006a 097c 006a 0a7c 006a  .|.j.|.j.|.j.|.j
+0000e300: 0b7c 006a 0c64 048d 0653 0029 0561 7901  .|.j.d...S.).ay.
+0000e310: 0000 4669 6c74 6572 2061 2054 6162 6c65  ..Filter a Table
+0000e320: 4469 6374 206f 626a 6563 7420 746f 206b  Dict object to k
+0000e330: 6565 7020 6f6e 6c79 2074 686f 7365 2063  eep only those c
+0000e340: 6f6c 756d 6e73 2072 656c 6174 6564 2074  olumns related t
+0000e350: 6f20 7468 6520 7365 6c65 6374 6564 2069  o the selected i
+0000e360: 642e 0a0a 2020 2020 2020 2020 4c65 6176  d...        Leav
+0000e370: 6520 6c61 6265 6c73 2075 6e74 6f75 6368  e labels untouch
+0000e380: 6564 2069 6620 7072 6573 656e 742e 0a0a  ed if present...
+0000e390: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+0000e3a0: 2020 2020 2020 2020 2020 7365 6c65 6374            select
+0000e3b0: 6564 5f69 6420 2873 7472 293a 2073 656c  ed_id (str): sel
+0000e3c0: 6563 7420 6120 7369 6e67 6c65 2061 6e69  ect a single ani
+0000e3d0: 6d61 6c20 6f6e 206d 756c 7469 2061 6e69  mal on multi ani
+0000e3e0: 6d61 6c20 7365 7474 696e 6773 2e20 4465  mal settings. De
+0000e3f0: 6661 756c 7473 2074 6f20 4e6f 6e65 2028  faults to None (
+0000e400: 616c 6c20 616e 696d 616c 7320 6172 6520  all animals are 
+0000e410: 7072 6f63 6573 7365 6429 2e0a 0a20 2020  processed)...   
+0000e420: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
+0000e430: 2020 2020 2020 2020 2020 7461 626c 655f            table_
+0000e440: 6469 6374 3a20 4669 6c74 6572 6564 2054  dict: Filtered T
+0000e450: 6162 6c65 4469 6374 206f 626a 6563 742c  ableDict object,
+0000e460: 206b 6565 7069 6e67 206f 6e6c 7920 7468   keeping only th
+0000e470: 6520 7365 6c65 6374 6564 2061 6e69 6d61  e selected anima
+0000e480: 6c2e 0a20 2020 2020 2020 204e 6301 0000  l..        Nc...
+0000e490: 0000 0000 0000 0000 0002 0000 0004 0000  ................
+0000e4a0: 0013 0000 0073 1800 0000 6700 7c00 5d10  .....s....g.|.].
+0000e4b0: 7d01 7c01 8800 7600 7204 7c01 9102 7104  }.|...v.r.|...q.
+0000e4c0: 5300 7227 0000 0072 2700 0000 2902 724b  S.r'...r'...).rK
+0000e4d0: 0000 00da 0362 7061 a901 da0f 636f 6c75  .....bpa....colu
+0000e4e0: 6d6e 735f 746f 5f6b 6565 7072 2700 0000  mns_to_keepr'...
+0000e4f0: 7228 0000 0072 4d00 0000 7507 0000 724e  r(...rM...u...rN
+0000e500: 0000 007a 2754 6162 6c65 4469 6374 2e66  ...z'TableDict.f
+0000e510: 696c 7465 725f 6964 2e3c 6c6f 6361 6c73  ilter_id.<locals
+0000e520: 3e2e 3c6c 6973 7463 6f6d 703e 2905 72b0  >.<listcomp>).r.
+0000e530: 0000 0072 6400 0000 724a 0100 0072 4b01  ...rd...rJ...rK.
+0000e540: 0000 7239 0000 0029 0d72 cd00 0000 72cc  ..r9...).r....r.
+0000e550: 0000 0072 8200 0000 7283 0000 0072 0f01  ...r....r....r..
+0000e560: 0000 72b8 0000 0072 c400 0000 72db 0000  ..r....r....r...
+0000e570: 0072 0002 0000 7242 0100 0072 0302 0000  .r....rB...r....
+0000e580: 7204 0200 0072 3801 0000 2905 7257 0000  r....r8...).rW..
+0000e590: 0072 4901 0000 7262 0100 0072 e600 0000  .rI...rb...r....
+0000e5a0: 72f9 0000 0072 2700 0000 7228 0200 0072  r....r'...r(...r
+0000e5b0: 2800 0000 da09 6669 6c74 6572 5f69 6466  (.....filter_idf
+0000e5c0: 0700 0073 1c00 0000 000b 0801 1001 1001  ...s............
+0000e5d0: 0401 1aff 0a04 0201 0201 0401 0401 0401  ................
+0000e5e0: 0401 04fa 7a13 5461 626c 6544 6963 742e  ....z.TableDict.
+0000e5f0: 6669 6c74 6572 5f69 64a9 01da 0c69 676e  filter_id....ign
+0000e600: 6f72 655f 696e 6465 7863 0100 0000 0000  ore_indexc......
+0000e610: 0000 0100 0000 0d00 0000 0700 0000 0700  ................
+0000e620: 0000 7322 0100 0074 00a0 017c 00a1 0167  ..s"...t...|...g
+0000e630: 0174 027c 0283 0117 007d 0274 0374 0283  .t.|.....}.t.t..
+0000e640: 017d 037c 0244 005d 247d 047c 04a0 04a1  .}.|.D.]$}.|....
+0000e650: 0044 005d 165c 027d 057d 067c 037c 0519  .D.].\.}.}.|.|..
+0000e660: 00a0 057c 06a1 0101 0071 2c71 2074 067c  ...|.....q,q t.|
+0000e670: 006a 0767 0164 0164 0284 007c 0244 0083  .j.g.d.d...|.D..
+0000e680: 0117 0083 017d 0774 0887 0066 0164 0364  .....}.t...f.d.d
+0000e690: 0484 087c 03a0 04a1 0044 0083 0164 057c  ...|.....D...d.|
+0000e6a0: 006a 097c 077c 006a 0a64 068d 057d 087c  .j.|.|.j.d...}.|
+0000e6b0: 08a0 04a1 0044 005d 845c 027d 057d 0964  .....D.].\.}.}.d
+0000e6c0: 0764 0284 007c 096a 0b44 0083 017d 0a74  .d...|.j.D...}.t
+0000e6d0: 0c7c 0a83 0164 086b 0472 9074 0c7c 0a64  .|...d.k.r.t.|.d
+0000e6e0: 0819 0083 0164 096b 0272 cc7c 0a64 0819  .....d.k.r.|.d..
+0000e6f0: 006e 087c 0a64 0819 0067 017d 0b7c 096a  .n.|.d...g.}.|.j
+0000e700: 0d64 0a64 0a85 027c 0b66 0219 006a 0e64  .d.d...|.f...j.d
+0000e710: 0a64 0a85 0264 0866 0219 007d 0c7c 096a  .d...d.f...}.|.j
+0000e720: 0f7c 0a64 0964 0b8d 027c 087c 053c 007c  .|.d.d...|.|.<.|
+0000e730: 0c7c 087c 0519 0064 0c3c 0071 907c 006a  .|.|...d.<.q.|.j
+0000e740: 107c 085f 107c 0853 0029 0d61 ac01 0000  .|._.|.S.).a....
+0000e750: 5461 6b65 2061 206e 756d 6265 7220 6f66  Take a number of
+0000e760: 2074 6162 6c65 5f64 6963 7420 6f62 6a65   table_dict obje
+0000e770: 6374 7320 616e 6420 6d65 7267 6573 2074  cts and merges t
+0000e780: 6865 6d20 746f 2074 6865 2063 7572 7265  hem to the curre
+0000e790: 6e74 206f 6e65 2e0a 0a20 2020 2020 2020  nt one...       
+0000e7a0: 2052 6574 7572 6e73 2061 2074 6162 6c65   Returns a table
+0000e7b0: 5f64 6963 7420 6f62 6a65 6374 206f 6620  _dict object of 
+0000e7c0: 7479 7065 2027 6d65 7267 6564 272e 0a20  type 'merged'.. 
+0000e7d0: 2020 2020 2020 204f 6e6c 7920 616e 6e6f         Only anno
+0000e7e0: 7461 7469 6f6e 7320 6f66 2074 6865 2066  tations of the f
+0000e7f0: 6972 7374 2074 6162 6c65 5f64 6963 7420  irst table_dict 
+0000e800: 6f62 6a65 6374 2061 7265 206b 6570 742e  object are kept.
+0000e810: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+0000e820: 2020 2020 2020 2020 2020 2020 2a61 7267              *arg
+0000e830: 7320 2874 6162 6c65 5f64 6963 7429 3a20  s (table_dict): 
+0000e840: 7461 626c 655f 6469 6374 206f 626a 6563  table_dict objec
+0000e850: 7473 2074 6f20 6265 206d 6572 6765 642e  ts to be merged.
+0000e860: 0a20 2020 2020 2020 2020 2020 2069 676e  .            ign
+0000e870: 6f72 655f 696e 6465 7820 2862 6f6f 6c29  ore_index (bool)
+0000e880: 3a20 6967 6e6f 7265 2069 6e64 6578 2077  : ignore index w
+0000e890: 6865 6e20 6d65 7267 696e 672e 2044 6566  hen merging. Def
+0000e8a0: 6175 6c74 7320 746f 2046 616c 7365 2e0a  aults to False..
+0000e8b0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+0000e8c0: 3a0a 2020 2020 2020 2020 2020 2020 7461  :.            ta
+0000e8d0: 626c 655f 6469 6374 3a20 4d65 7267 6564  ble_dict: Merged
+0000e8e0: 2074 6162 6c65 5f64 6963 7420 6f62 6a65   table_dict obje
+0000e8f0: 6374 2e0a 2020 2020 2020 2020 6301 0000  ct..        c...
+0000e900: 0000 0000 0000 0000 0002 0000 0003 0000  ................
+0000e910: 0053 0000 0073 1200 0000 6700 7c00 5d0a  .S...s....g.|.].
+0000e920: 7d01 7c01 6a00 9102 7104 5300 7227 0000  }.|.j...q.S.r'..
+0000e930: 0029 0172 0302 0000 2902 724b 0000 00da  .).r....).rK....
+0000e940: 0774 6162 6469 6374 7227 0000 0072 2700  .tabdictr'...r'.
+0000e950: 0000 7228 0000 0072 4d00 0000 9507 0000  ..r(...rM.......
+0000e960: 724e 0000 007a 2354 6162 6c65 4469 6374  rN...z#TableDict
+0000e970: 2e6d 6572 6765 2e3c 6c6f 6361 6c73 3e2e  .merge.<locals>.
+0000e980: 3c6c 6973 7463 6f6d 703e 6301 0000 0000  <listcomp>c.....
+0000e990: 0000 0000 0000 0003 0000 0009 0000 0013  ................
+0000e9a0: 0000 0073 2400 0000 6900 7c00 5d1c 5c02  ...s$...i.|.].\.
+0000e9b0: 7d01 7d02 7c01 7400 6a01 7c02 6400 8800  }.}.|.t.j.|.d...
+0000e9c0: 6401 6402 8d04 9302 7104 5300 2903 7232  d.d.....q.S.).r2
+0000e9d0: 0000 00da 0569 6e6e 6572 2903 728f 0000  .....inner).r...
+0000e9e0: 0072 2c02 0000 7220 0000 0029 0272 bf00  .r,...r ...).r..
+0000e9f0: 0000 72d8 0000 0029 0372 4b00 0000 72e6  ..r....).rK...r.
+0000ea00: 0000 0072 f900 0000 722b 0200 0072 2700  ...r....r+...r'.
+0000ea10: 0000 7228 0000 0072 9800 0000 9907 0000  ..r(...r........
+0000ea20: 7304 0000 0006 0206 ff7a 2354 6162 6c65  s........z#Table
+0000ea30: 4469 6374 2e6d 6572 6765 2e3c 6c6f 6361  Dict.merge.<loca
+0000ea40: 6c73 3e2e 3c64 6963 7463 6f6d 703e da06  ls>.<dictcomp>..
+0000ea50: 6d65 7267 6564 2904 72b0 0000 0072 6400  merged).r....rd.
+0000ea60: 0000 724a 0100 0072 4b01 0000 6301 0000  ..rJ...rK...c...
+0000ea70: 0000 0000 0000 0000 0002 0000 0005 0000  ................
+0000ea80: 0053 0000 0073 1c00 0000 6700 7c00 5d14  .S...s....g.|.].
+0000ea90: 7d01 6400 7400 7c01 8301 7600 7204 7c01  }.d.t.|...v.r.|.
+0000eaa0: 9102 7104 5300 a901 7252 0100 0072 a200  ..q.S...rR...r..
+0000eab0: 0000 a902 724b 0000 00da 0363 6f6c 7227  ....rK.....colr'
+0000eac0: 0000 0072 2700 0000 7228 0000 0072 4d00  ...r'...r(...rM.
+0000ead0: 0000 a607 0000 724e 0000 0072 0100 0000  ......rN...r....
+0000eae0: 7232 0000 004e 72ac 0000 0072 5201 0000  r2...Nr....rR...
+0000eaf0: 2911 72cd 0000 0072 5301 0000 72b6 0000  ).r....rS...r...
+0000eb00: 0072 0200 0000 72cc 0000 0072 fe00 0000  .r....r....r....
+0000eb10: 725b 0100 0072 0302 0000 72db 0000 0072  r[...r....r....r
+0000eb20: 4201 0000 7204 0200 0072 b800 0000 725f  B...r....r....r_
+0000eb30: 0000 0072 c400 0000 7292 0000 0072 8800  ...r....r....r..
+0000eb40: 0000 7232 0100 0029 0d72 5700 0000 722c  ..r2...).rW...r,
+0000eb50: 0200 00da 0461 7267 73da 0b6d 6572 6765  .....args..merge
+0000eb60: 645f 6469 6374 722d 0200 0072 e600 0000  d_dictr-...r....
+0000eb70: 72f9 0000 0072 4a01 0000 da0d 6d65 7267  r....rJ.....merg
+0000eb80: 6564 5f74 6162 6c65 7372 5500 0000 da0a  ed_tablesrU.....
+0000eb90: 7068 656e 6f5f 636f 6c73 da09 7068 656e  pheno_cols..phen
+0000eba0: 6f5f 636f 6c72 1702 0000 7227 0000 0072  o_colr....r'...r
+0000ebb0: 2b02 0000 7228 0000 0072 9801 0000 8107  +...r(...r......
+0000ebc0: 0000 7336 0000 0000 0d14 0108 0108 0110  ..s6............
+0000ebd0: 0112 0202 0114 ff04 0402 010a 0206 fe04  ................
+0000ebe0: 0402 0104 0102 0104 f806 0c10 0210 010c  ................
+0000ebf0: 0320 ff02 0320 0212 010e 0308 027a 0f54  . ... .......z.T
+0000ec00: 6162 6c65 4469 6374 2e6d 6572 6765 7201  ableDict.merger.
+0000ec10: 0000 0029 03da 1263 7572 7265 6e74 5f74  ...)...current_t
+0000ec20: 6162 6c65 5f64 6963 74da 0b74 6573 745f  able_dict..test_
+0000ec30: 7669 6465 6f73 721a 0000 0063 0300 0000  videosr....c....
+0000ec40: 0000 0000 0000 0000 0c00 0000 0800 0000  ................
+0000ec50: 0300 0000 738c 0300 007c 01a0 00a1 0089  ....s....|......
+0000ec60: 0174 016a 0267 0074 0364 018d 027d 0374  .t.j.g.t.d...}.t
+0000ec70: 016a 0264 0264 0384 0088 0144 0083 0174  .j.d.d.....D...t
+0000ec80: 0464 018d 0289 017c 006a 0572 9a74 016a  .d.....|.j.r.t.j
+0000ec90: 0688 0164 0464 058d 027d 0474 0774 087c  ...d.d...}.t.t.|
+0000eca0: 0464 0664 0685 0264 0766 0219 0083 0183  .d.d...d.f......
+0000ecb0: 0144 005d 3c89 0074 016a 096a 0a87 0087  .D.]<..t.j.j....
+0000ecc0: 0166 0264 0864 0384 0874 0b74 0c88 0183  .f.d.d...t.t....
+0000ecd0: 0183 0144 0083 017c 0264 0964 0a8d 037d  ...D...|.d.d...}
+0000ece0: 0574 01a0 067c 037c 0567 02a1 017d 0371  .t...|.|.g...}.q
+0000ecf0: 5a6e 1a74 016a 096a 0a74 0b74 0c88 0183  Zn.t.j.j.t.t....
+0000ed00: 0183 017c 0264 0964 0a8d 037d 0374 01a0  ...|.d.d...}.t..
+0000ed10: 0267 00a1 0174 01a0 0267 00a1 0174 01a0  .g...t...g...t..
+0000ed20: 0267 00a1 0103 0002 007d 067d 077d 087c  .g.......}.}.}.|
+0000ed30: 0264 046b 0490 0172 467a 2874 01a0 0688  .d.k...rFz(t....
+0000ed40: 017c 0319 00a1 017d 0774 01a0 0674 016a  .|.....}.t...t.j
+0000ed50: 0d88 017c 0364 0464 058d 03a1 017d 0957  ...|.d.d.....}.W
+0000ed60: 006e 3a04 0074 0e90 0179 4201 0001 0001  .n:..t...yB.....
+0000ed70: 0074 016a 0267 0074 0364 018d 027d 0374  .t.j.g.t.d...}.t
+0000ed80: 01a0 0674 0888 0183 01a1 017d 0974 0fa0  ...t.......}.t..
+0000ed90: 1064 0ba1 0101 0059 006e 0230 006e 0e74  .d.....Y.n.0.n.t
+0000eda0: 01a0 0674 0888 0183 01a1 017d 097c 006a  ...t.......}.|.j
+0000edb0: 0590 0272 2874 1183 007d 0a7c 0964 0664  ...r(t...}.|.d.d
+0000edc0: 0685 0264 0664 0785 0266 0219 007c 0964  ...d.d...f...|.d
+0000edd0: 0664 0685 0264 0766 0219 0064 0664 0685  .d...d.f...d.d..
+0000ede0: 0274 016a 1266 0219 0002 007d 097d 067c  .t.j.f.....}.}.|
+0000edf0: 0aa0 137c 0664 0664 0685 0264 0466 0219  ...|.d.d...d.f..
+0000ee00: 00a1 017c 0664 0664 0685 0264 0466 023c  ...|.d.d...d.f.<
+0000ee10: 007a 5a7c 0764 0664 0685 0264 0664 0785  .zZ|.d.d...d.d..
+0000ee20: 0266 0219 007c 0764 0664 0685 0264 0766  .f...|.d.d...d.f
+0000ee30: 0219 0064 0664 0685 0274 016a 1266 0219  ...d.d...t.j.f..
+0000ee40: 0002 007d 077d 087c 0aa0 147c 0864 0664  ...}.}.|...|.d.d
+0000ee50: 0685 0264 0466 0219 00a1 017c 0864 0664  ...d.f.....|.d.d
+0000ee60: 0685 0264 0466 023c 0057 006e 1404 0074  ...d.f.<.W.n...t
+0000ee70: 1590 0279 2601 0001 0001 0059 006e 0230  ...y&......Y.n.0
+0000ee80: 007c 006a 1690 0372 6674 087c 006a 16a0  .|.j...rft.|.j..
+0000ee90: 00a1 0083 0164 0419 006a 1764 0c19 007d  .....d...j.d...}
+0000eea0: 0b7a 407c 0964 0664 0685 0264 067c 0b0b  .z@|.d.d...d.|..
+0000eeb0: 0085 0266 0219 0074 016a 067c 067c 0964  ...f...t.j.|.|.d
+0000eec0: 0664 0685 027c 0b0b 0064 0685 0266 0219  .d...|...d...f..
+0000eed0: 0067 0264 0c64 058d 0202 007d 097d 0657  .g.d.d.....}.}.W
+0000eee0: 006e 4204 0074 0e90 0279 ca01 0001 0001  .nB..t...y......
+0000eef0: 007c 0964 0664 0685 0264 067c 0b0b 0085  .|.d.d...d.|....
+0000ef00: 0266 0219 007c 0964 0664 0685 027c 0b0b  .f...|.d.d...|..
+0000ef10: 0064 0685 0266 0219 0002 007d 097d 0659  .d...f.....}.}.Y
+0000ef20: 006e 0230 007a 847a 3c7c 0764 0664 0685  .n.0.z.z<|.d.d..
+0000ef30: 0264 067c 0b0b 0085 0266 0219 0074 01a0  .d.|.....f...t..
+0000ef40: 067c 087c 0764 0664 0685 027c 0b0b 0064  .|.|.d.d...|...d
+0000ef50: 0685 0266 0219 0067 02a1 0102 007d 077d  ...f...g.....}.}
+0000ef60: 0857 006e 4204 0074 0e90 0379 4c01 0001  .W.nB..t...yL...
+0000ef70: 0001 007c 0764 0664 0685 0264 067c 0b0b  ...|.d.d...d.|..
+0000ef80: 0085 0266 0219 007c 0764 0664 0685 027c  ...f...|.d.d...|
+0000ef90: 0b0b 0064 0685 0266 0219 0002 007d 077d  ...d...f.....}.}
+0000efa0: 0859 006e 0230 0057 006e 1404 0074 1590  .Y.n.0.W.n...t..
+0000efb0: 0379 6401 0001 0001 0059 006e 0230 007c  .yd......Y.n.0.|
+0000efc0: 09a0 1874 19a1 017c 06a0 1874 19a1 017c  ...t...|...t...|
+0000efd0: 07a0 1874 19a1 017c 08a0 1874 19a1 017c  ...t...|...t...|
+0000efe0: 0366 0553 0029 0d61 d401 0000 4765 6e65  .f.S.).a....Gene
+0000eff0: 7261 7465 2074 7261 696e 696e 6720 616e  rate training an
+0000f000: 6420 7465 7374 2073 6574 7320 6173 206e  d test sets as n
+0000f010: 756d 7079 2e61 7272 6179 206f 626a 6563  umpy.array objec
+0000f020: 7473 2066 6f72 206d 6f64 656c 2074 7261  ts for model tra
+0000f030: 696e 696e 672e 0a0a 2020 2020 2020 2020  ining...        
+0000f040: 496e 7465 6e64 6564 2066 6f72 2069 6e74  Intended for int
+0000f050: 6572 6e61 6c20 7573 6167 6520 6f6e 6c79  ernal usage only
+0000f060: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
+0000f070: 0a20 2020 2020 2020 2020 2020 2063 7572  .            cur
+0000f080: 7265 6e74 5f74 6162 6c65 5f64 6963 7420  rent_table_dict 
+0000f090: 2874 6162 6c65 5f64 6963 7429 3a20 7461  (table_dict): ta
+0000f0a0: 626c 655f 6469 6374 206f 626a 6563 7420  ble_dict object 
+0000f0b0: 636f 6e74 6169 6e69 6e67 2074 6865 2064  containing the d
+0000f0c0: 6174 6120 746f 2062 6520 7573 6564 2066  ata to be used f
+0000f0d0: 6f72 2074 7261 696e 696e 672e 0a20 2020  or training..   
+0000f0e0: 2020 2020 2020 2020 2074 6573 745f 7669           test_vi
+0000f0f0: 6465 6f73 2028 696e 7429 3a20 4e75 6d62  deos (int): Numb
+0000f100: 6572 206f 6620 7669 6465 6f73 2074 6f20  er of videos to 
+0000f110: 6265 2075 7365 6420 666f 7220 7465 7374  be used for test
+0000f120: 696e 672e 2044 6566 6175 6c74 7320 746f  ing. Defaults to
+0000f130: 2030 2e0a 0a20 2020 2020 2020 2052 6574   0...        Ret
+0000f140: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
+0000f150: 2020 7475 706c 653a 2054 7570 6c65 2063    tuple: Tuple c
+0000f160: 6f6e 7461 696e 696e 6720 7472 6169 6e69  ontaining traini
+0000f170: 6e67 2064 6174 612c 2074 7261 696e 696e  ng data, trainin
+0000f180: 6720 6c61 6265 6c73 2028 6966 2061 6e79  g labels (if any
+0000f190: 292c 2074 6573 7420 6461 7461 2c20 616e  ), test data, an
+0000f1a0: 6420 7465 7374 206c 6162 656c 7320 2869  d test labels (i
+0000f1b0: 6620 616e 7929 2e0a 2020 2020 2020 2020  f any)..        
+0000f1c0: 7286 0000 0063 0100 0000 0000 0000 0000  r....c..........
+0000f1d0: 0000 0200 0000 0300 0000 5300 0000 7312  ..........S...s.
+0000f1e0: 0000 0067 007c 005d 0a7d 017c 016a 0091  ...g.|.].}.|.j..
+0000f1f0: 0271 0453 0072 2700 0000 2901 72c9 0000  .q.S.r'...).r...
+0000f200: 0029 0272 4b00 0000 7213 0200 0072 2700  .).rK...r....r'.
+0000f210: 0000 7227 0000 0072 2800 0000 724d 0000  ..r'...r(...rM..
+0000f220: 00ca 0700 0072 4e00 0000 7a2e 5461 626c  .....rN...z.Tabl
+0000f230: 6544 6963 742e 6765 745f 7472 6169 6e69  eDict.get_traini
+0000f240: 6e67 5f73 6574 2e3c 6c6f 6361 6c73 3e2e  ng_set.<locals>.
+0000f250: 3c6c 6973 7463 6f6d 703e 7201 0000 0072  <listcomp>r....r
+0000f260: ac00 0000 4e72 9501 0000 6301 0000 0000  ....Nr....c.....
+0000f270: 0000 0000 0000 0002 0000 0004 0000 0013  ................
+0000f280: 0000 0073 2000 0000 6700 7c00 5d18 7d01  ...s ...g.|.].}.
+0000f290: 8801 7c01 1900 6400 1900 8800 6b02 7204  ..|...d.....k.r.
+0000f2a0: 7c01 9102 7104 5300 7211 0200 0072 2700  |...q.S.r....r'.
+0000f2b0: 0000 724a 0000 00a9 02da 056c 6162 656c  ..rJ.......label
+0000f2c0: da08 7261 775f 6461 7461 7227 0000 0072  ..raw_datar'...r
+0000f2d0: 2800 0000 724d 0000 00d0 0700 0072 4e00  (...rM.......rN.
+0000f2e0: 0000 46a9 01da 0772 6570 6c61 6365 7a79  ..F....replacezy
+0000f2f0: 436f 756c 6420 6e6f 7420 6669 6e64 206d  Could not find m
+0000f300: 6f72 6520 7468 616e 206f 6e65 2073 616d  ore than one sam
+0000f310: 706c 6520 666f 7220 6174 206c 6561 7374  ple for at least
+0000f320: 206f 6e65 2063 6f6e 6469 7469 6f6e 2e20   one condition. 
+0000f330: 5061 7274 6974 696f 6e20 6265 7477 6565  Partition betwee
+0000f340: 6e20 7472 6169 6e69 6e67 2061 6e64 2074  n training and t
+0000f350: 6573 7420 7365 7420 7761 7320 6e6f 7420  est set was not 
+0000f360: 706f 7373 6962 6c65 2e72 3200 0000 291a  possible.r2...).
+0000f370: 72c9 0000 0072 de00 0000 72df 0000 0072  r....r....r....r
+0000f380: 2101 0000 da06 6f62 6a65 6374 7203 0200  !.....objectr...
+0000f390: 0072 9b01 0000 72b7 0000 0072 b600 0000  .r....r....r....
+0000f3a0: 721c 0200 00da 0663 686f 6963 6572 d000  r......choicer..
+0000f3b0: 0000 725f 0000 00da 0664 656c 6574 6572  ..r_.....deleter
+0000f3c0: 7501 0000 7213 0100 0072 1401 0000 720d  u...r....r....r.
+0000f3d0: 0000 0072 1502 0000 7223 0200 00da 0974  ...r....r#.....t
+0000f3e0: 7261 6e73 666f 726d 72c8 0000 0072 0402  ransformr....r..
+0000f3f0: 0000 72d5 0000 0072 d100 0000 72c1 0000  ..r....r....r...
+0000f400: 0029 0c72 5700 0000 7238 0200 0072 3902  .).rW...r8...r9.
+0000f410: 0000 da0a 7465 7374 5f69 6e64 6578 da0a  ....test_index..
+0000f420: 636f 6e63 6174 5f72 6177 da0b 6c61 6265  concat_raw..labe
+0000f430: 6c5f 696e 6465 78da 0779 5f74 7261 696e  l_index..y_train
+0000f440: da06 585f 7465 7374 da06 795f 7465 7374  ..X_test..y_test
+0000f450: da07 585f 7472 6169 6eda 026c 65da 076e  ..X_train..le..n
+0000f460: 5f61 6e6e 6f74 7227 0000 0072 3a02 0000  _annotr'...r:...
+0000f470: 7228 0000 00da 1067 6574 5f74 7261 696e  r(.....get_train
+0000f480: 696e 675f 7365 74b6 0700 0073 7600 0000  ing_set....sv...
+0000f490: 000e 0804 0e02 1801 0601 0e02 1c01 0601  ................
+0000f4a0: 1a01 0201 02fd 0605 1202 0601 0eff 0604  ................
+0000f4b0: 2201 0a01 0201 0e01 1a01 0e01 0e01 0e01  "...............
+0000f4c0: 0401 02ff 0c06 0e02 0801 0601 3401 2201  ............4.".
+0000f4d0: 0201 3401 2601 0e01 0602 0801 1802 0202  ..4.&...........
+0000f4e0: 1401 22fe 0a04 0e01 3402 0201 0202 1401  ..".....4.......
+0000f4f0: 1efe 0a04 0e01 3802 0e01 0603 0801 0801  ......8.........
+0000f500: 0801 0801 02fb 7a1a 5461 626c 6544 6963  ......z.TableDic
+0000f510: 742e 6765 745f 7472 6169 6e69 6e67 5f73  t.get_training_s
+0000f520: 6574 72d8 0000 00e9 1900 0000 7232 0000  etr.........r2..
+0000f530: 00da 0873 7461 6e64 6172 6472 d501 0000  ...standardr....
+0000f540: 290c da0a 6861 6e64 6c65 5f69 6473 da0b  )...handle_ids..
+0000f550: 7769 6e64 6f77 5f73 697a 65da 0b77 696e  window_size..win
+0000f560: 646f 775f 7374 6570 da05 7363 616c 65da  dow_step..scale.
+0000f570: 1170 7265 7472 6169 6e65 645f 7363 616c  .pretrained_scal
+0000f580: 6572 7239 0200 0072 8000 0000 da07 7368  err9...r......sh
+0000f590: 7566 666c 65da 1366 696c 7465 725f 6c6f  uffle..filter_lo
+0000f5a0: 775f 7661 7269 616e 6365 da16 696e 7465  w_variance..inte
+0000f5b0: 7270 6f6c 6174 655f 6e6f 726d 616c 697a  rpolate_normaliz
+0000f5c0: 6564 da12 7072 6563 6f6d 7075 7465 645f  ed..precomputed_
+0000f5d0: 6272 6561 6b73 721a 0000 0063 0d00 0000  breaksr....c....
+0000f5e0: 0000 0000 0000 0000 2200 0000 0d00 0000  ........".......
+0000f5f0: 0300 0000 7314 0700 0074 00a0 017c 00a1  ....s....t...|..
+0000f600: 017d 0d7c 0264 0176 0073 1a4a 0064 0283  .}.|.d.v.s.J.d..
+0000f610: 0182 017c 0a72 7e7c 0da0 02a1 0044 005d  ...|.r~|.....D.]
+0000f620: 565c 027d 0e7d 0f7c 0f6a 0364 0364 0385  V\.}.}.|.j.d.d..
+0000f630: 0274 0474 05a0 067c 0f6a 0764 0464 058d  .t.t...|.j.d.d..
+0000f640: 017c 0a6b 04a1 0164 0419 0083 0174 0474  .|.k...d.....t.t
+0000f650: 05a0 0664 0664 0784 007c 0f6a 0844 0083  ...d.d...|.j.D..
+0000f660: 01a1 0164 0419 0083 0117 0066 0219 007c  ...d.......f...|
+0000f670: 0d7c 0e3c 0071 267c 0590 0172 987c 0872  .|.<.q&|...r.|.r
+0000f680: 9074 0964 0883 0101 007c 0564 0976 0172  .t.d.....|.d.v.r
+0000f690: a074 0a64 0a83 0182 017c 0da0 02a1 0044  .t.d.....|.....D
+0000f6a0: 005d 425c 027d 0e7d 0f74 0b6a 0c6a 0d7c  .]B\.}.}.t.j.j.|
+0000f6b0: 007c 0f7c 0564 0364 0b8d 047d 1074 0e6a  .|.|.d.d...}.t.j
+0000f6c0: 0f7c 107c 0f6a 087c 0f6a 1064 0c8d 036a  .|.|.j.|.j.d...j
+0000f6d0: 1164 0d64 0e84 0064 0464 058d 027c 0d7c  .d.d...d.d...|.|
+0000f6e0: 0e3c 0071 a87c 0564 0f6b 0272 fc74 1283  .<.q.|.d.k.r.t..
+0000f6f0: 007d 116e 187c 0564 106b 0290 0172 0e74  .}.n.|.d.k...r.t
+0000f700: 1383 007d 116e 0674 1483 007d 117c 0664  ...}.n.t...}.|.d
+0000f710: 0375 0090 0172 5274 0ea0 1574 047c 0da0  .u...rRt...t.|..
+0000f720: 16a1 0083 01a1 017d 127c 11a0 177c 126a  .......}.|...|.j
+0000f730: 1864 0364 0385 027c 126a 1974 1a6b 0266  .d.d...|.j.t.k.f
+0000f740: 0219 006a 16a1 0101 006e 047c 067d 117c  ...j.....n.|.}.|
+0000f750: 0da0 02a1 0044 005d 365c 027d 0e7d 0f74  .....D.]6\.}.}.t
+0000f760: 0b6a 0c6a 0d7c 007c 0f7c 057c 1164 0b8d  .j.j.|.|.|.|.d..
+0000f770: 047d 1074 0e6a 0f7c 107c 0f6a 087c 0f6a  .}.t.j.|.|.j.|.j
+0000f780: 1064 0c8d 037c 0d7c 0e3c 0090 0171 5e6e  .d...|.|.<...q^n
+0000f790: 0464 037d 117c 0564 0f6b 0290 0272 c87c  .d.}.|.d.k...r.|
+0000f7a0: 0b90 0272 c874 00a0 017c 0da1 017d 137c  ...r.t...|...}.|
+0000f7b0: 13a0 02a1 0044 0090 015d 025c 027d 0e7d  .....D...].\.}.}
+0000f7c0: 0f74 00a0 017c 0f6a 16a1 017d 147a 2274  .t...|.j...}.z"t
+0000f7d0: 056a 1b7c 147c 147c 0b6b 043c 0074 056a  .j.|.|.|.k.<.t.j
+0000f7e0: 1b7c 147c 147c 0b0b 006b 003c 0057 006e  .|.|.|...k.<.W.n
+0000f7f0: 9e04 0074 1c90 0279 9401 0001 0001 0074  ...t...y.......t
+0000f800: 056a 1b7c 1474 056a 1d7c 1464 0364 0385  .j.|.t.j.|.d.d..
+0000f810: 0264 0364 1185 0266 0219 00a0 1e74 1aa1  .d.d...f.....t..
+0000f820: 017c 0b6b 0474 05a0 1f64 1267 0174 207c  .|.k.t...d.g.t |
+0000f830: 1483 0114 0067 01a1 016a 2164 1364 058d  .....g...j!d.d..
+0000f840: 033c 0074 056a 1b7c 1474 056a 1d7c 1464  .<.t.j.|.t.j.|.d
+0000f850: 0364 0385 0264 0364 1185 0266 0219 00a0  .d...d.d...f....
+0000f860: 1e74 1aa1 017c 0b0b 006b 0074 05a0 1f64  .t...|...k.t...d
+0000f870: 1267 0174 207c 1483 0114 0067 01a1 016a  .g.t |.....g...j
+0000f880: 2164 1364 058d 033c 0059 006e 0230 0074  !d.d...<.Y.n.0.t
+0000f890: 0e6a 0f7c 147c 0f6a 107c 0f6a 0864 148d  .j.|.|.j.|.j.d..
+0000f8a0: 03a0 1164 1564 0e84 00a1 016a 2264 1664  ...d.d.....j"d.d
+0000f8b0: 178d 017c 137c 0e3c 0090 0171 be7c 137d  ...|.|.<...q.|.}
+0000f8c0: 0d7c 00a0 237c 0d7c 07a1 025c 057d 157d  .|..#|.|...\.}.}
+0000f8d0: 167d 177d 1889 017c 0890 0272 ec74 0964  .}.}...|...r.t.d
+0000f8e0: 1883 0101 0074 0b6a 0c6a 247c 0d7c 1587  .....t.j.j$|.|..
+0000f8f0: 0166 0164 1964 0784 0874 2574 207c 0d83  .f.d.d...t%t |..
+0000f900: 0183 0144 0083 017c 017c 037c 047c 0c64  ...D...|.|.|.|.d
+0000f910: 1a8d 075c 027d 157d 197c 0864 136b 0490  ...\.}.}.|.d.k..
+0000f920: 0372 867c 0190 0372 8674 056a 267c 1564  .r.|...r.t.j&|.d
+0000f930: 046b 0364 1b64 058d 026a 2764 1364 058d  .k.d.d...j'd.d..
+0000f940: 017d 1a74 0964 1ca0 287c 1aa0 29a1 007c  .}.t.d..(|..)..|
+0000f950: 1aa0 2aa1 00a1 0283 0101 0074 0964 1da0  ..*........t.d..
+0000f960: 287c 1aa0 2ba1 00a1 0183 0101 0074 0964  (|..+........t.d
+0000f970: 1ea0 287c 1aa0 2ca1 00a1 0183 0101 007c  ..(|..,........|
+0000f980: 006a 2d90 0373 967c 006a 2e90 0372 f07c  .j-..s.|.j...r.|
+0000f990: 1964 0375 0090 0372 d674 0b6a 0c6a 247c  .d.u...r.t.j.j$|
+0000f9a0: 0d7c 1687 0166 0164 1f64 0784 0874 2574  .|...f.d.d...t%t
+0000f9b0: 207c 0d83 0183 0144 0083 0164 127c 037c   |.....D...d.|.|
+0000f9c0: 047c 0c64 1a8d 075c 027d 167d 1b6e 0e74  .|.d...\.}.}.n.t
+0000f9d0: 0b6a 0ca0 2f7c 167c 19a1 027d 167c 166a  .j../|.|...}.|.j
+0000f9e0: 2964 1364 058d 017d 167c 0790 0472 c874  )d.d...}.|...r.t
+0000f9f0: 2088 0183 0164 046b 0490 0472 c874 0b6a   ....d.k...r.t.j
+0000fa00: 0c6a 247c 0d7c 1788 017c 017c 037c 047c  .j$|.|...|.|.|.|
+0000fa10: 0c64 1a8d 075c 027d 177d 1c7c 006a 2d90  .d...\.}.}.|.j-.
+0000fa20: 0473 327c 006a 2e90 0472 8c7c 1c64 0375  .s2|.j...r.|.d.u
+0000fa30: 0090 0472 7274 0b6a 0c6a 247c 0d7c 1887  ...rrt.j.j$|.|..
+0000fa40: 0166 0164 2064 0784 0874 2574 207c 0d83  .f.d d...t%t |..
+0000fa50: 0183 0144 0083 0164 127c 037c 047c 0c64  ...D...d.|.|.|.d
+0000fa60: 1a8d 075c 027d 187d 1b6e 1a74 0b6a 0ca0  ...\.}.}.n.t.j..
+0000fa70: 2f7c 187c 1ca1 027d 187c 186a 2964 1364  /|.|...}.|.j)d.d
+0000fa80: 058d 017d 187c 0990 0472 c874 056a 306a  ...}.|...r.t.j0j
+0000fa90: 317c 176a 3264 0419 007c 176a 3264 0419  1|.j2d...|.j2d..
+0000faa0: 0064 1264 218d 037d 1d7c 177c 1d19 007d  .d.d!..}.|.|...}
+0000fab0: 177c 006a 2d90 0472 c87c 187c 1d19 007d  .|.j-..r.|.|...}
+0000fac0: 187c 0990 0572 0474 056a 306a 317c 156a  .|...r.t.j0j1|.j
+0000fad0: 3264 0419 007c 156a 3264 0419 0064 1264  2d...|.j2d...d.d
+0000fae0: 218d 037d 1e7c 157c 1e19 007d 157c 006a  !..}.|.|...}.|.j
+0000faf0: 2d90 0572 047c 167c 1e19 007d 1674 05a0  -..r.|.|...}.t..
+0000fb00: 1f7c 17a1 0174 05a0 1f7c 18a1 0102 007d  .|...t...|.....}
+0000fb10: 177d 187c 0790 0572 be7c 0190 0572 be74  .}.|...r.|...r.t
+0000fb20: 207c 176a 3283 0164 046b 0490 0572 be7c   |.j2..d.k...r.|
+0000fb30: 156a 3264 1319 007c 176a 3264 1319 006b  .j2d...|.j2d...k
+0000fb40: 0390 0572 be74 05a0 337c 156a 3264 1319  ...r.t..3|.j2d..
+0000fb50: 007c 176a 3264 1319 00a1 027d 1f7c 156a  .|.j2d.....}.|.j
+0000fb60: 3264 1319 007c 1f6b 0090 0572 9a74 056a  2d...|.k...r.t.j
+0000fb70: 347c 1564 2264 047c 1f7c 156a 3264 1319  4|.d"d.|.|.j2d..
+0000fb80: 0018 0066 0264 2266 0364 2364 248d 037d  ...f.d"f.d#d$..}
+0000fb90: 156e 2474 056a 347c 1764 2264 047c 1f7c  .n$t.j4|.d"d.|.|
+0000fba0: 176a 3264 1319 0018 0066 0264 2266 0364  .j2d.....f.d"f.d
+0000fbb0: 2364 248d 037d 177c 0890 0572 cc74 0964  #d$..}.|...r.t.d
+0000fbc0: 2583 0101 007c 166a 3264 266b 0390 0672  %....|.j2d&k...r
+0000fbd0: 0a7c 156a 3264 0419 007c 166a 3264 0419  .|.j2d...|.j2d..
+0000fbe0: 006b 0290 0673 0a4a 0064 27a0 287c 156a  .k...s.J.d'.(|.j
+0000fbf0: 3264 0419 007c 166a 3264 0419 00a1 0283  2d...|.j2d......
+0000fc00: 0182 017c 186a 3264 266b 0390 0672 347c  ...|.j2d&k...r4|
+0000fc10: 176a 3264 0419 007c 186a 3264 0419 006b  .j2d...|.j2d...k
+0000fc20: 0290 0673 344a 0064 2883 0182 0174 207c  ...s4J.d(....t |
+0000fc30: 006a 3583 0164 136b 0490 0772 047c 0264  .j5..d.k...r.|.d
+0000fc40: 296b 0290 0772 0467 0067 0002 007d 207d  )k...r.g.g...} }
+0000fc50: 217c 006a 3544 005d 8289 007c 20a0 1d7c  !|.j5D.]...| ..|
+0000fc60: 1564 0364 0385 0264 0364 0385 0274 05a0  .d.d...d.d...t..
+0000fc70: 0687 0066 0164 2a64 0784 0874 047c 0da0  ...f.d*d...t.|..
+0000fc80: 16a1 0083 0164 0419 006a 0844 0083 01a1  .....d...j.D....
+0000fc90: 0166 0319 00a1 0101 007c 21a0 1d7c 1764  .f.......|!..|.d
+0000fca0: 0364 0385 0264 0364 0385 0274 05a0 0687  .d...d.d...t....
+0000fcb0: 0066 0164 2b64 0784 0874 047c 0da0 16a1  .f.d+d...t.|....
+0000fcc0: 0083 0164 0419 006a 0844 0083 01a1 0166  ...d...j.D.....f
+0000fcd0: 0319 00a1 0101 0090 0671 5e74 05a0 3674  .........q^t..6t
+0000fce0: 05a0 377c 20a1 01a1 0174 05a0 3674 05a0  ..7| ....t..6t..
+0000fcf0: 377c 21a1 01a1 0102 007d 157d 177c 157c  7|!......}.}.|.|
+0000fd00: 167c 177c 1866 047c 1166 0253 0029 2c61  .|.|.f.|.f.S.),a
+0000fd10: 170c 0000 5072 6570 726f 6365 7373 2074  ....Preprocess t
+0000fd20: 6865 206c 6f61 6465 6420 6461 7461 7365  he loaded datase
+0000fd30: 7420 6265 666f 7265 2066 6565 6469 6e67  t before feeding
+0000fd40: 2074 6f20 756e 7375 7065 7276 6973 6564   to unsupervised
+0000fd50: 2065 6d62 6564 6469 6e67 206d 6f64 656c   embedding model
+0000fd60: 732e 0a0a 2020 2020 2020 2020 4361 7061  s...        Capa
+0000fd70: 626c 6520 6f66 2072 6574 7572 6e69 6e67  ble of returning
+0000fd80: 2074 7261 696e 696e 6720 616e 6420 7465   training and te
+0000fd90: 7374 2073 6574 7320 7265 6164 7920 666f  st sets ready fo
+0000fda0: 7220 6d6f 6465 6c20 7472 6169 6e69 6e67  r model training
+0000fdb0: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
+0000fdc0: 0a20 2020 2020 2020 2020 2020 2061 7574  .            aut
+0000fdd0: 6f6d 6174 6963 5f63 6861 6e67 6570 6f69  omatic_changepoi
+0000fde0: 6e74 7320 2873 7472 293a 2073 7065 6369  nts (str): speci
+0000fdf0: 6669 6573 2074 6865 2063 6861 6e67 6570  fies the changep
+0000fe00: 6f69 6e74 2064 6574 6563 7469 6f6e 206b  oint detection k
+0000fe10: 6572 6e65 6c20 746f 2075 7365 2074 6f20  ernel to use to 
+0000fe20: 7275 7074 7572 6520 7468 6520 6461 7461  rupture the data
+0000fe30: 2061 6372 6f73 7320 7469 6d65 2075 7369   across time usi
+0000fe40: 6e67 2050 656c 742e 2043 616e 2062 6520  ng Pelt. Can be 
+0000fe50: 7365 7420 746f 2022 7262 6622 2028 6465  set to "rbf" (de
+0000fe60: 6661 756c 7429 2c20 6f72 2022 6c69 6e65  fault), or "line
+0000fe70: 6172 222e 2049 6620 4661 6c73 652c 2066  ar". If False, f
+0000fe80: 6978 6564 2d6c 656e 6774 6820 7275 7074  ixed-length rupt
+0000fe90: 7572 6573 2061 7265 2061 7070 696c 6564  ures are appiled
+0000fea0: 2e0a 2020 2020 2020 2020 2020 2020 6861  ..            ha
+0000feb0: 6e64 6c65 5f69 6473 2028 7374 7229 3a20  ndle_ids (str): 
+0000fec0: 696e 6469 6361 7465 7320 7468 6520 6465  indicates the de
+0000fed0: 6661 756c 7420 6163 7469 6f6e 2074 6f20  fault action to 
+0000fee0: 6861 6e64 6c65 206d 756c 7469 706c 6520  handle multiple 
+0000fef0: 616e 696d 616c 7320 696e 2074 6865 2054  animals in the T
+0000ff00: 6162 6c65 4469 6374 206f 626a 6563 742e  ableDict object.
+0000ff10: 204d 7573 7420 6265 206f 6e65 206f 6620   Must be one of 
+0000ff20: 2263 6f6e 6361 7422 2028 626f 6479 2070  "concat" (body p
+0000ff30: 6172 7473 2066 726f 6d20 6469 6666 6572  arts from differ
+0000ff40: 656e 7420 616e 696d 616c 7320 6172 6520  ent animals are 
+0000ff50: 7472 6561 7465 6420 6173 2066 6561 7475  treated as featu
+0000ff60: 7265 7329 2061 6e64 2022 7370 6c69 7422  res) and "split"
+0000ff70: 2028 6469 6666 6572 656e 7420 736c 6964   (different slid
+0000ff80: 696e 6720 7769 6e64 6f77 7320 6172 6520  ing windows are 
+0000ff90: 6372 6561 7465 6420 666f 7220 6561 6368  created for each
+0000ffa0: 2061 6e69 6d61 6c29 2e0a 2020 2020 2020   animal)..      
+0000ffb0: 2020 2020 2020 7769 6e64 6f77 5f73 697a        window_siz
+0000ffc0: 6520 2869 6e74 293a 204d 696e 696d 756d  e (int): Minimum
+0000ffd0: 2073 697a 6520 6f66 2074 6865 2061 7070   size of the app
+0000ffe0: 6c69 6564 2072 7570 7475 7265 732e 2049  lied ruptures. I
+0000fff0: 6620 6175 746f 6d61 7469 635f 6368 616e  f automatic_chan
+00010000: 6765 706f 696e 7473 2069 7320 4661 6c73  gepoints is Fals
+00010010: 652c 2073 7065 6369 6669 6573 2074 6865  e, specifies the
+00010020: 2073 697a 6520 6f66 2074 6865 2073 6c69   size of the sli
+00010030: 6469 6e67 2077 696e 646f 7720 746f 2070  ding window to p
+00010040: 6173 7320 7468 726f 7567 6820 7468 6520  ass through the 
+00010050: 6461 7461 2074 6f20 6765 6e65 7261 7465  data to generate
+00010060: 2074 7261 696e 696e 6720 696e 7374 616e   training instan
+00010070: 6365 732e 0a20 2020 2020 2020 2020 2020  ces..           
+00010080: 2077 696e 646f 775f 7374 6570 2028 696e   window_step (in
+00010090: 7429 3a20 5370 6563 6966 6965 7320 7468  t): Specifies th
+000100a0: 6520 6d69 6e69 6d75 6d20 6a75 6d70 2066  e minimum jump f
+000100b0: 6f72 2074 6865 2072 7570 7475 7265 2061  or the rupture a
+000100c0: 6c67 6f72 6974 686d 732e 2049 6620 6175  lgorithms. If au
+000100d0: 746f 6d61 7469 635f 6368 616e 6765 706f  tomatic_changepo
+000100e0: 696e 7473 2069 7320 4661 6c73 652c 2073  ints is False, s
+000100f0: 7065 6369 6669 6573 2074 6865 2073 7465  pecifies the ste
+00010100: 7020 746f 2074 616b 6520 7768 656e 2073  p to take when s
+00010110: 6c69 6469 6e67 2074 6865 2061 666f 7265  liding the afore
+00010120: 6d65 6e74 696f 6e65 6420 7769 6e64 6f77  mentioned window
+00010130: 2e20 496e 2074 6869 7320 6361 7365 2c20  . In this case, 
+00010140: 6120 7661 6c75 6520 6f66 2031 2069 6e64  a value of 1 ind
+00010150: 6963 6174 6573 2061 2074 7275 6520 736c  icates a true sl
+00010160: 6964 696e 6720 7769 6e64 6f77 2c20 616e  iding window, an
+00010170: 6420 6120 7661 6c75 6520 6571 7561 6c20  d a value equal 
+00010180: 746f 2077 696e 646f 775f 7369 7a65 2073  to window_size s
+00010190: 706c 6974 7320 7468 6520 6461 7461 2069  plits the data i
+000101a0: 6e74 6f20 6e6f 6e2d 6f76 6572 6c61 7070  nto non-overlapp
+000101b0: 696e 6720 6368 756e 6b73 2e0a 2020 2020  ing chunks..    
+000101c0: 2020 2020 2020 2020 7363 616c 6520 2873          scale (s
+000101d0: 7472 293a 2044 6174 6120 7363 616c 696e  tr): Data scalin
+000101e0: 6720 6d65 7468 6f64 2e20 4d75 7374 2062  g method. Must b
+000101f0: 6520 6f6e 6520 6f66 2027 7374 616e 6461  e one of 'standa
+00010200: 7264 272c 2027 726f 6275 7374 2720 2864  rd', 'robust' (d
+00010210: 6566 6175 6c74 3b20 7265 636f 6d6d 656e  efault; recommen
+00010220: 6465 6429 2061 6e64 2027 6d69 6e6d 6178  ded) and 'minmax
+00010230: 272e 0a20 2020 2020 2020 2020 2020 2070  '..            p
+00010240: 7265 7472 6169 6e65 645f 7363 616c 6572  retrained_scaler
+00010250: 2028 416e 7929 3a20 5072 652d 6669 7420   (Any): Pre-fit 
+00010260: 676c 6f62 616c 2073 6361 6c65 722c 2074  global scaler, t
+00010270: 7261 696e 6564 206f 6e20 7468 6520 7768  rained on the wh
+00010280: 6f6c 6520 6461 7461 7365 742e 2055 7365  ole dataset. Use
+00010290: 6675 6c20 746f 2070 726f 6365 7373 2073  ful to process s
+000102a0: 696e 676c 6520 7669 6465 6f73 2e0a 2020  ingle videos..  
+000102b0: 2020 2020 2020 2020 2020 7465 7374 5f76            test_v
+000102c0: 6964 656f 7320 2869 6e74 293a 204e 756d  ideos (int): Num
+000102d0: 6265 7220 6f66 2076 6964 656f 7320 746f  ber of videos to
+000102e0: 2075 7365 2066 6f72 2074 6573 7469 6e67   use for testing
+000102f0: 2e20 4966 2030 2c20 6e6f 2074 6573 7420  . If 0, no test 
+00010300: 7365 7420 6973 2067 656e 6572 6174 6564  set is generated
+00010310: 2e0a 2020 2020 2020 2020 2020 2020 7665  ..            ve
+00010320: 7262 6f73 6520 2869 6e74 293a 2056 6572  rbose (int): Ver
+00010330: 626f 7369 7479 206c 6576 656c 2e20 3020  bosity level. 0 
+00010340: 2864 6566 6175 6c74 2920 6973 2073 696c  (default) is sil
+00010350: 656e 742c 2031 2070 7269 6e74 7320 7072  ent, 1 prints pr
+00010360: 6f67 7265 7373 2c20 3220 7072 696e 7473  ogress, 2 prints
+00010370: 2064 6562 7567 2069 6e66 6f72 6d61 7469   debug informati
+00010380: 6f6e 2e0a 2020 2020 2020 2020 2020 2020  on..            
+00010390: 7368 7566 666c 6520 2862 6f6f 6c29 3a20  shuffle (bool): 
+000103a0: 5768 6574 6865 7220 746f 2073 6875 6666  Whether to shuff
+000103b0: 6c65 2074 6865 2064 6174 6120 6265 666f  le the data befo
+000103c0: 7265 2070 7265 7072 6f63 6573 7369 6e67  re preprocessing
+000103d0: 2e20 4465 6661 756c 7473 2074 6f20 4661  . Defaults to Fa
+000103e0: 6c73 652e 0a20 2020 2020 2020 2020 2020  lse..           
+000103f0: 2066 696c 7465 725f 6c6f 775f 7661 7269   filter_low_vari
+00010400: 616e 6365 2028 666c 6f61 7429 3a20 7265  ance (float): re
+00010410: 6d6f 7665 2066 6561 7475 7265 7320 7769  move features wi
+00010420: 7468 2076 6172 6961 6e63 6520 6c6f 7765  th variance lowe
+00010430: 7220 7468 616e 2074 6865 2073 7065 6369  r than the speci
+00010440: 6669 6564 2074 6872 6573 686f 6c64 2e20  fied threshold. 
+00010450: 5573 6566 756c 2074 6f20 6765 7420 7269  Useful to get ri
+00010460: 6420 6f66 2074 6865 2078 2061 7869 7320  d of the x axis 
+00010470: 6f66 2074 6865 2062 6f64 7920 7061 7274  of the body part
+00010480: 2075 7365 6420 666f 7220 616c 6967 6e6d   used for alignm
+00010490: 656e 7420 2877 6869 6368 2077 6f75 6c64  ent (which would
+000104a0: 2069 6e74 726f 6475 6365 206e 6f69 7365   introduce noise
+000104b0: 2061 6674 6572 2073 7461 6e64 6172 6469   after standardi
+000104c0: 7a61 7469 6f6e 292e 0a20 2020 2020 2020  zation)..       
+000104d0: 2020 2020 2069 6e74 6572 706f 6c61 7465       interpolate
+000104e0: 5f6e 6f72 6d61 6c69 7a65 6428 696e 7429  _normalized(int)
+000104f0: 3a20 6966 206e 6f74 2030 2c20 6974 2073  : if not 0, it s
+00010500: 7065 6369 6669 6573 2074 6865 206e 756d  pecifies the num
+00010510: 6265 7220 6f66 2073 7461 6e64 6172 6420  ber of standard 
+00010520: 6465 7669 6174 696f 6e73 2062 6579 6f6e  deviations beyon
+00010530: 6420 7768 6963 6820 7661 6c75 6573 2077  d which values w
+00010540: 696c 6c20 6265 2069 6e74 6572 706f 6c61  ill be interpola
+00010550: 7465 6420 6166 7465 7220 6e6f 726d 616c  ted after normal
+00010560: 697a 6174 696f 6e2e 204f 6e6c 7920 7573  ization. Only us
+00010570: 6564 2069 6620 7363 616c 6520 6973 2073  ed if scale is s
+00010580: 6574 2074 6f20 2273 7461 6e64 6172 6422  et to "standard"
+00010590: 2e0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
+000105a0: 6563 6f6d 7075 7465 645f 6272 6561 6b73  ecomputed_breaks
+000105b0: 2028 6469 6374 293a 2049 6620 7072 6f76   (dict): If prov
+000105c0: 6964 6564 2c20 6368 616e 6765 706f 696e  ided, changepoin
+000105d0: 7420 6465 7465 6374 696f 6e20 6973 2070  t detection is p
+000105e0: 7265 7665 6e74 6564 2c20 616e 6420 7072  revented, and pr
+000105f0: 6f76 6964 6564 2062 7265 616b 7320 6172  ovided breaks ar
+00010600: 6520 7573 6564 2069 6e73 7465 6164 2e0a  e used instead..
+00010610: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00010620: 3a0a 2020 2020 2020 2020 2020 2020 585f  :.            X_
+00010630: 7472 6169 6e20 286e 702e 6e64 6172 7261  train (np.ndarra
+00010640: 7929 3a20 3344 2064 6174 6173 6574 2077  y): 3D dataset w
+00010650: 6974 6820 7368 6170 6520 2869 6e73 7461  ith shape (insta
+00010660: 6e63 6573 2c20 736c 6964 696e 675f 7769  nces, sliding_wi
+00010670: 6e64 6f77 5f73 697a 652c 2066 6561 7475  ndow_size, featu
+00010680: 7265 7329 2067 656e 6572 6174 6564 2066  res) generated f
+00010690: 726f 6d20 616c 6c20 7472 6169 6e69 6e67  rom all training
+000106a0: 2076 6964 656f 732e 0a20 2020 2020 2020   videos..       
+000106b0: 2020 2020 2079 5f74 7261 696e 2028 6e70       y_train (np
+000106c0: 2e6e 6461 7272 6179 293a 2033 4420 6461  .ndarray): 3D da
+000106d0: 7461 7365 7420 7769 7468 2073 6861 7065  taset with shape
+000106e0: 2028 696e 7374 616e 6365 732c 2073 6c69   (instances, sli
+000106f0: 6469 6e67 5f77 696e 646f 775f 7369 7a65  ding_window_size
+00010700: 2c20 6c61 6265 6c73 2920 6765 6e65 7261  , labels) genera
+00010710: 7465 6420 6672 6f6d 2061 6c6c 2074 7261  ted from all tra
+00010720: 696e 696e 6720 7669 6465 6f73 2e20 4e6f  ining videos. No
+00010730: 7465 2074 6861 7420 6e6f 206c 6162 656c  te that no label
+00010740: 7320 6172 6520 7573 6520 6279 2064 6566  s are use by def
+00010750: 6175 6c74 2069 6e20 7468 6520 6675 6c6c  ault in the full
+00010760: 7920 756e 7375 7065 7276 6973 6564 2070  y unsupervised p
+00010770: 6970 656c 696e 6520 2869 6e20 7768 6963  ipeline (in whic
+00010780: 6820 6361 7365 2074 6869 7320 6973 2061  h case this is a
+00010790: 6e20 656d 7074 7920 6172 7261 7929 2e0a  n empty array)..
+000107a0: 2020 2020 2020 2020 2020 2020 585f 7465              X_te
+000107b0: 7374 2028 6e70 2e6e 6461 7272 6179 293a  st (np.ndarray):
+000107c0: 2033 4420 6461 7461 7365 7420 7769 7468   3D dataset with
+000107d0: 2073 6861 7065 2028 696e 7374 616e 6365   shape (instance
+000107e0: 732c 2073 6c69 6469 6e67 5f77 696e 646f  s, sliding_windo
+000107f0: 775f 7369 7a65 2c20 6665 6174 7572 6573  w_size, features
+00010800: 2920 6765 6e65 7261 7465 6420 6672 6f6d  ) generated from
+00010810: 2061 6c6c 2074 6573 7420 7669 6465 6f73   all test videos
+00010820: 2028 3020 6279 2064 6566 6175 6c74 292e   (0 by default).
+00010830: 0a20 2020 2020 2020 2020 2020 2079 5f74  .            y_t
+00010840: 6573 7420 286e 702e 6e64 6172 7261 7929  est (np.ndarray)
+00010850: 3a20 3344 2064 6174 6173 6574 2077 6974  : 3D dataset wit
+00010860: 6820 7368 6170 6520 2869 6e73 7461 6e63  h shape (instanc
+00010870: 6573 2c20 736c 6964 696e 675f 7769 6e64  es, sliding_wind
+00010880: 6f77 5f73 697a 652c 206c 6162 656c 7329  ow_size, labels)
+00010890: 2067 656e 6572 6174 6564 2066 726f 6d20   generated from 
+000108a0: 616c 6c20 7465 7374 2076 6964 656f 732e  all test videos.
+000108b0: 204e 6f74 6520 7468 6174 206e 6f20 6c61   Note that no la
+000108c0: 6265 6c73 2061 7265 2075 7365 2062 7920  bels are use by 
+000108d0: 6465 6661 756c 7420 696e 2074 6865 2066  default in the f
+000108e0: 756c 6c79 2075 6e73 7570 6572 7669 7365  ully unsupervise
+000108f0: 6420 7069 7065 6c69 6e65 2028 696e 2077  d pipeline (in w
+00010900: 6869 6368 2063 6173 6520 7468 6973 2069  hich case this i
+00010910: 7320 616e 2065 6d70 7479 2061 7272 6179  s an empty array
+00010920: 292e 0a20 2020 2020 2020 2029 0272 d800  )..        ).r..
+00010930: 0000 7223 0000 007a 5668 616e 646c 6520  ..r#...zVhandle 
+00010940: 4944 7320 7368 6f75 6c64 2062 6520 6f6e  IDs should be on
+00010950: 6520 6f66 2027 636f 6e63 6174 272c 2061  e of 'concat', a
+00010960: 6e64 2027 7370 6c69 7427 2e20 5365 6520  nd 'split'. See 
+00010970: 646f 6375 6d65 6e74 6174 696f 6e20 666f  documentation fo
+00010980: 7220 6d6f 7265 2064 6574 6169 6c73 2e4e  r more details.N
+00010990: 7201 0000 0072 ac00 0000 6301 0000 0000  r....r....c.....
+000109a0: 0000 0000 0000 0002 0000 0005 0000 0053  ...............S
+000109b0: 0000 0073 1800 0000 6700 7c00 5d10 7d01  ...s....g.|.].}.
+000109c0: 6400 7400 7c01 8301 7600 9102 7104 5300  d.t.|...v...q.S.
+000109d0: 7230 0200 0072 a200 0000 7231 0200 0072  r0...r....r1...r
+000109e0: 2700 0000 7227 0000 0072 2800 0000 724d  '...r'...r(...rM
+000109f0: 0000 004b 0800 0072 4e00 0000 7a28 5461  ...K...rN...z(Ta
+00010a00: 626c 6544 6963 742e 7072 6570 726f 6365  bleDict.preproce
+00010a10: 7373 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  ss.<locals>.<lis
+00010a20: 7463 6f6d 703e 7a0f 5363 616c 696e 6720  tcomp>z.Scaling 
+00010a30: 6461 7461 2e2e 2e29 03da 0672 6f62 7573  data...)...robus
+00010a40: 7472 4e02 0000 da06 6d69 6e6d 6178 7a38  trN.....minmaxz8
+00010a50: 496e 7661 6c69 6420 7363 616c 6572 2e20  Invalid scaler. 
+00010a60: 5365 6c65 6374 206f 6e65 206f 6620 7374  Select one of st
+00010a70: 616e 6461 7264 2c20 6d69 6e6d 6178 206f  andard, minmax o
+00010a80: 7220 726f 6275 7374 2904 7226 0000 00da  r robust).r&....
+00010a90: 0d66 6561 7475 7265 5f61 7272 6179 7252  .feature_arrayrR
+00010aa0: 0200 0072 ad01 0000 2902 72b8 0000 0072  ...r....).r....r
+00010ab0: ca00 0000 6301 0000 0000 0000 0000 0000  ....c...........
+00010ac0: 0001 0000 0004 0000 0053 0000 0073 0e00  .........S...s..
+00010ad0: 0000 7400 6a01 7c00 6401 6402 8d02 5300  ..t.j.|.d.d...S.
+00010ae0: a903 4eda 0669 676e 6f72 6529 01da 0665  ..N..ignore)...e
+00010af0: 7272 6f72 73a9 0272 bf00 0000 da0a 746f  rrors..r......to
+00010b00: 5f6e 756d 6572 6963 7208 0100 0072 2700  _numericr....r'.
+00010b10: 0000 7227 0000 0072 2800 0000 72a5 0000  ..r'...r(...r...
+00010b20: 0065 0800 0072 4e00 0000 7a26 5461 626c  .e...rN...z&Tabl
+00010b30: 6544 6963 742e 7072 6570 726f 6365 7373  eDict.preprocess
+00010b40: 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d 6264  .<locals>.<lambd
+00010b50: 613e 724e 0200 0072 5902 0000 7295 0100  a>rN...rY...r...
+00010b60: 0046 7232 0000 0072 0e01 0000 6301 0000  .Fr2...r....c...
+00010b70: 0000 0000 0000 0000 0001 0000 0004 0000  ................
+00010b80: 0053 0000 0073 0e00 0000 7400 6a01 7c00  .S...s....t.j.|.
+00010b90: 6401 6402 8d02 5300 725b 0200 0072 5e02  d.d...S.r[...r^.
+00010ba0: 0000 7208 0100 0072 2700 0000 7227 0000  ..r....r'...r'..
+00010bb0: 0072 2800 0000 72a5 0000 00a6 0800 0072  .r(...r........r
+00010bc0: 4e00 0000 da04 626f 7468 2901 da0f 6c69  N.....both)...li
+00010bd0: 6d69 745f 6469 7265 6374 696f 6e7a 1742  mit_directionz.B
+00010be0: 7265 616b 696e 6720 7469 6d65 2073 6572  reaking time ser
+00010bf0: 6965 732e 2e2e 6301 0000 0000 0000 0000  ies...c.........
+00010c00: 0000 0002 0000 0004 0000 0013 0000 0073  ...............s
+00010c10: 1800 0000 6700 7c00 5d10 7d01 7c01 8800  ....g.|.].}.|...
+00010c20: 7601 7204 7c01 9102 7104 5300 7227 0000  v.r.|...q.S.r'..
+00010c30: 0072 2700 0000 724a 0000 00a9 0172 4302  .r'...rJ.....rC.
+00010c40: 0000 7227 0000 0072 2800 0000 724d 0000  ..r'...r(...rM..
+00010c50: 00b8 0800 0072 4e00 0000 2907 72fd 0100  .....rN...).r...
+00010c60: 00da 0a74 6f5f 7275 7074 7572 65da 0f72  ...to_rupture..r
+00010c70: 7570 7475 7265 5f69 6e64 6963 6573 da16  upture_indices..
+00010c80: 6175 746f 6d61 7469 635f 6368 616e 6765  automatic_change
+00010c90: 706f 696e 7473 7250 0200 0072 5102 0000  pointsrP...rQ...
+00010ca0: 7257 0200 0072 9300 0000 7a32 6176 6572  rW...r....z2aver
+00010cb0: 6167 6520 7275 7074 7572 6520 6c65 6e67  age rupture leng
+00010cc0: 7468 3a20 7b7d 2c20 7374 616e 6461 7264  th: {}, standard
+00010cd0: 2064 6576 6961 7469 6f6e 3a20 7b7d 7a1a   deviation: {}z.
+00010ce0: 6d69 6e69 6d75 6d20 7275 7074 7572 6520  minimum rupture 
+00010cf0: 6c65 6e67 7468 3a20 7b7d 7a1a 6d61 7869  length: {}z.maxi
+00010d00: 6d75 6d20 7275 7074 7572 6520 6c65 6e67  mum rupture leng
+00010d10: 7468 3a20 7b7d 6301 0000 0000 0000 0000  th: {}c.........
+00010d20: 0000 0002 0000 0004 0000 0013 0000 0073  ...............s
+00010d30: 1800 0000 6700 7c00 5d10 7d01 7c01 8800  ....g.|.].}.|...
+00010d40: 7601 7204 7c01 9102 7104 5300 7227 0000  v.r.|...q.S.r'..
+00010d50: 0072 2700 0000 724a 0000 0072 6202 0000  .r'...rJ...rb...
+00010d60: 7227 0000 0072 2800 0000 724d 0000 00d0  r'...r(...rM....
+00010d70: 0800 0073 0200 0000 0601 6301 0000 0000  ...s......c.....
+00010d80: 0000 0000 0000 0002 0000 0004 0000 0013  ................
+00010d90: 0000 0073 1800 0000 6700 7c00 5d10 7d01  ...s....g.|.].}.
+00010da0: 7c01 8800 7600 7204 7c01 9102 7104 5300  |...v.r.|...q.S.
+00010db0: 7227 0000 0072 2700 0000 724a 0000 0072  r'...r'...rJ...r
+00010dc0: 6202 0000 7227 0000 0072 2800 0000 724d  b...r'...r(...rM
+00010dd0: 0000 00f0 0800 0073 0200 0000 0601 723d  .......s......r=
+00010de0: 0200 0029 0272 0100 0000 7201 0000 0072  ...).r....r....r
+00010df0: ad00 0000 2901 da0f 636f 6e73 7461 6e74  ....)...constant
+00010e00: 5f76 616c 7565 7372 2001 0000 72ef 0000  _valuesr ...r...
+00010e10: 007a 3c74 7261 696e 696e 6720 7365 7420  .z<training set 
+00010e20: 287b 7d29 2061 6e64 206c 6162 656c 7320  ({}) and labels 
+00010e30: 287b 7d29 2064 6f20 6e6f 7420 6861 7665  ({}) do not have
+00010e40: 2074 6865 2073 616d 6520 7368 6170 657a   the same shapez
+00010e50: 3274 7261 696e 696e 6720 7365 7420 616e  2training set an
+00010e60: 6420 6c61 6265 6c73 2064 6f20 6e6f 7420  d labels do not 
+00010e70: 6861 7665 2074 6865 2073 616d 6520 7368  have the same sh
+00010e80: 6170 6572 2300 0000 6301 0000 0000 0000  aper#...c.......
+00010e90: 0000 0000 0002 0000 0005 0000 0013 0000  ................
+00010ea0: 0073 2600 0000 6700 7c00 5d1e 7d01 7400  .s&...g.|.].}.t.
+00010eb0: a001 7c01 6701 a101 a002 a100 6400 1900  ..|.g.......d...
+00010ec0: a003 8800 a101 9102 7104 5300 72ef 0000  ........q.S.r...
+00010ed0: 00a9 0472 de00 0000 72df 0000 00da 0766  ...r....r......f
+00010ee0: 6c61 7474 656e 7249 0000 0072 4a00 0000  lattenrI...rJ...
+00010ef0: 7209 0100 0072 2700 0000 7228 0000 0072  r....r'...r(...r
+00010f00: 4d00 0000 3d09 0000 7304 0000 0006 0202  M...=...s.......
+00010f10: ff63 0100 0000 0000 0000 0000 0000 0200  .c..............
+00010f20: 0000 0500 0000 1300 0000 7326 0000 0067  ..........s&...g
+00010f30: 007c 005d 1e7d 0174 00a0 017c 0167 01a1  .|.].}.t...|.g..
+00010f40: 01a0 02a1 0064 0019 00a0 0388 00a1 0191  .....d..........
+00010f50: 0271 0453 0072 ef00 0000 7267 0200 0072  .q.S.r....rg...r
+00010f60: 4a00 0000 7209 0100 0072 2700 0000 7228  J...r....r'...r(
+00010f70: 0000 0072 4d00 0000 4909 0000 7304 0000  ...rM...I...s...
+00010f80: 0006 0202 ff29 3872 cd00 0000 7253 0100  .....)8r....rS..
+00010f90: 0072 cc00 0000 7292 0000 0072 b600 0000  .r....r....r....
+00010fa0: 72de 0000 00da 0577 6865 7265 da03 7661  r......where..va
+00010fb0: 7272 b800 0000 7281 0000 0072 7501 0000  rr....r....ru...
+00010fc0: 7282 0000 0072 8300 0000 da0b 7363 616c  r....r......scal
+00010fd0: 655f 7461 626c 6572 bf00 0000 72dc 0000  e_tabler....r...
+00010fe0: 0072 ca00 0000 7210 0100 0072 0b00 0000  .r....r....r....
+00010ff0: 720a 0000 0072 0c00 0000 72d8 0000 0072  r....r....r....r
+00011000: c900 0000 da03 6669 7472 c400 0000 da06  ......fitr......
+00011010: 6474 7970 6573 72c1 0000 00da 036e 616e  dtypesr......nan
+00011020: da09 5479 7065 4572 726f 7272 fe00 0000  ..TypeErrorr....
+00011030: 72d1 0000 0072 df00 0000 725f 0000 0072  r....r....r_...r
+00011040: c200 0000 da0b 696e 7465 7270 6f6c 6174  ......interpolat
+00011050: 6572 4c02 0000 da16 7275 7074 7572 655f  erL.....rupture_
+00011060: 7065 725f 6578 7065 7269 6d65 6e74 72d0  per_experimentr.
+00011070: 0000 0072 5800 0000 da03 7375 6d72 6d00  ...rX.....sumrm.
+00011080: 0000 7214 0200 00da 0373 7464 da03 6d69  ..r......std..mi
+00011090: 6eda 036d 6178 7203 0200 0072 0402 0000  n..maxr....r....
+000110a0: da16 7370 6c69 745f 7769 7468 5f62 7265  ..split_with_bre
+000110b0: 616b 706f 696e 7473 721c 0200 0072 4002  akpointsr....r@.
+000110c0: 0000 72d5 0000 00da 076d 6178 696d 756d  ..r......maximum
+000110d0: da03 7061 6472 3201 0000 da07 7371 7565  ..padr2.....sque
+000110e0: 657a 6572 9b01 0000 2922 7257 0000 0072  ezer....)"rW...r
+000110f0: 6502 0000 724f 0200 0072 5002 0000 7251  e...rO...rP...rQ
+00011100: 0200 0072 5202 0000 7253 0200 0072 3902  ...rR...rS...r9.
+00011110: 0000 7280 0000 0072 5402 0000 7255 0200  ..r....rT...rU..
+00011120: 0072 5602 0000 7257 0200 00da 0a74 6162  .rV...rW.....tab
+00011130: 6c65 5f74 656d 7072 e600 0000 7255 0000  le_tempr....rU..
+00011140: 00da 0b63 7572 7265 6e74 5f74 6162 72ad  ...current_tabr.
+00011150: 0100 00da 0b63 6f6e 6361 745f 6461 7461  .....concat_data
+00011160: da0e 746f 5f69 6e74 6572 706f 6c61 7465  ..to_interpolate
+00011170: da07 6375 725f 7461 6272 4902 0000 7246  ..cur_tabrI...rF
+00011180: 0200 0072 4702 0000 7248 0200 00da 0c74  ...rG...rH.....t
+00011190: 7261 696e 5f62 7265 616b 73da 0b72 7074  rain_breaks..rpt
+000111a0: 5f6c 656e 6774 6873 728d 0000 00da 0b74  _lengthsr......t
+000111b0: 6573 745f 6272 6561 6b73 da0c 7368 7566  est_breaks..shuf
+000111c0: 666c 655f 7465 7374 da0d 7368 7566 666c  fle_test..shuffl
+000111d0: 655f 7472 6169 6eda 0d6d 6178 5f73 6571  e_train..max_seq
+000111e0: 6c65 6e67 7468 da0d 585f 7472 6169 6e5f  length..X_train_
+000111f0: 7370 6c69 74da 0c58 5f74 6573 745f 7370  split..X_test_sp
+00011200: 6c69 7472 2700 0000 2902 7297 0000 0072  litr'...).r....r
+00011210: 4302 0000 7228 0000 0072 9001 0000 1408  C...r(...r......
+00011220: 0000 73cc 0100 0000 290a 020a 0302 fd04  ..s.....).......
+00011230: 0504 0310 0104 0106 011c 011c ff02 ff02  ................
+00011240: ff0a 0606 0104 0108 0208 0102 0102 ff04  ................
+00011250: 0510 0206 0102 0102 0102 0102 fc06 0704  ................
+00011260: 0102 0104 0104 fd06 0408 fc0c 0708 0108  ................
+00011270: 010a 0108 0206 020a 0112 0104 0118 ff06  ................
+00011280: 0404 0210 0206 0102 0102 0102 0102 fc06  ................
+00011290: 0704 010a ff10 0504 0210 030a 0112 010c  ................
+000112a0: 0202 010e 0114 030e 0804 fa02 0104 011c  ................
+000112b0: 0116 0102 fd04 ff02 0d04 fa02 0104 011e  ................
+000112c0: 0116 0102 fd04 ff08 0914 0106 ff04 0202  ................
+000112d0: fe04 ff0a 0604 0304 0104 ff0e 0406 0108  ................
+000112e0: 0306 0102 0102 0118 0102 0102 0102 0102  ................
+000112f0: f90a 0b10 011a 0102 0104 010c ff02 ff04  ................
+00011300: 0512 0112 0210 020a 0106 0102 0102 010a  ................
+00011310: 010a ff04 0302 0102 0102 0102 f70c 0d0e  ................
+00011320: 020c 0214 0306 0102 0102 0102 0102 0102  ................
+00011330: 0102 0102 f90a 0a10 010a 0106 0102 0102  ................
+00011340: 010a 010a ff04 0302 0102 0102 0102 f70c  ................
+00011350: 0c0e 010c 0206 0106 0112 ff06 0308 0208  ................
+00011360: 0108 0206 0106 0112 ff06 0308 0208 0108  ................
+00011370: 0216 0502 ff04 0202 fe04 030c fd04 0412  ................
+00011380: fc04 0618 0110 0104 0102 0116 0102 fd08  ................
+00011390: 0604 0102 0116 0102 fd06 0606 0108 020c  ................
+000113a0: 0212 ff06 0204 0110 ff02 fe04 050c 0212  ................
+000113b0: ff06 0202 fe04 051a 010a 010a 0104 0102  ................
+000113c0: 0106 0106 0104 010a 0210 fe04 ff02 fe02  ................
+000113d0: ff02 ff04 0c04 0102 0106 0106 0104 010a  ................
+000113e0: 0210 fe04 ff02 fe02 ff02 ff08 0d12 0108  ................
+000113f0: ff08 047a 1454 6162 6c65 4469 6374 2e70  ...z.TableDict.p
+00011400: 7265 7072 6f63 6573 7329 0272 9300 0000  reprocess).r....
+00011410: 4e29 0272 9300 0000 72d8 0100 0029 0272  N).r....r....).r
+00011420: 9300 0000 72d8 0100 0029 0172 9300 0000  ....r....).r....
+00011430: 2901 4e29 0172 0100 0000 290c 4672 d800  ).N).r....).Fr..
+00011440: 0000 724d 0200 0072 3200 0000 724e 0200  ..rM...r2...rN..
+00011450: 004e 7201 0000 0072 0100 0000 4646 72d5  .Nr....r....FFr.
+00011460: 0100 004e 2922 7259 0000 0072 2a01 0000  ...N)"rY...r*...
+00011470: 722b 0100 0072 2c01 0000 72d2 0000 0072  r+...r,...r....r
+00011480: 1300 0000 72a3 0000 0072 de00 0000 72df  ....r....r....r.
+00011490: 0000 0072 1400 0000 729d 0100 0072 fc01  ...r....r....r..
+000114a0: 0000 722d 0100 0072 2e01 0000 7212 0000  ..r-...r....r...
+000114b0: 0072 6a00 0000 72b6 0000 0072 fd01 0000  .rj...r....r....
+000114c0: 720b 0200 0072 1002 0000 72fb 0100 0072  r....r....r....r
+000114d0: 1902 0000 7221 0100 0072 1500 0000 7210  ....r!...r....r.
+000114e0: 0000 0072 2402 0000 7207 0000 0072 1e02  ...r$...r....r..
+000114f0: 0000 7220 0200 0072 2a02 0000 7298 0100  ..r ...r*...r...
+00011500: 0072 4c02 0000 7290 0100 00da 0d5f 5f63  .rL...r......__c
+00011510: 6c61 7373 6365 6c6c 5f5f 7227 0000 0072  lasscell__r'...r
+00011520: 2700 0000 7205 0200 0072 2800 0000 72db  '...r....r(...r.
+00011530: 0000 0093 0600 0073 9c00 0000 0801 0409  .......s........
+00011540: 0201 0201 0801 0201 0201 0201 0201 0201  ................
+00011550: 02f4 0202 0201 0201 0201 0401 0201 0201  ................
+00011560: 0401 0201 0201 0201 0af4 102b 1017 1021  ...........+...!
+00011570: 1013 0001 00fc 0202 0201 0201 0201 0afb  ................
+00011580: 0c25 00ff 0201 0401 0afe 0c11 1c11 00fe  .%..............
+00011590: 0202 0201 0afd 0c16 121b 0e36 00ff 0201  ...........6....
+000115a0: 0401 02fe 0c60 0001 0001 0001 0001 0001  .....`..........
+000115b0: 0001 0001 0001 0001 0001 0001 00f3 0203  ................
+000115c0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+000115d0: 0201 0201 0201 04f2 72db 0000 00da 085f  ........r......_
+000115e0: 5f6d 6169 6e5f 5fda 0132 da14 5446 5f43  _main__..2..TF_C
+000115f0: 5050 5f4d 494e 5f4c 4f47 5f4c 4556 454c  PP_MIN_LOG_LEVEL
+00011600: 2944 722c 0100 00da 0b63 6f6c 6c65 6374  )Dr,.....collect
+00011610: 696f 6e73 7202 0000 00da 0764 6966 666c  ionsr......diffl
+00011620: 6962 7203 0000 00da 0d70 6b67 5f72 6573  ibr......pkg_res
+00011630: 6f75 7263 6573 7204 0000 00da 1073 6861  ourcesr......sha
+00011640: 7065 6c79 2e67 656f 6d65 7472 7972 0500  pely.geometryr..
+00011650: 0000 7276 0000 0072 0600 0000 da07 736b  ..rv...r......sk
+00011660: 6c65 6172 6e72 0700 0000 da15 736b 6c65  learnr......skle
+00011670: 6172 6e2e 6465 636f 6d70 6f73 6974 696f  arn.decompositio
+00011680: 6e72 0800 0000 da10 736b 6c65 6172 6e2e  nr......sklearn.
+00011690: 6d61 6e69 666f 6c64 7209 0000 00da 1573  manifoldr......s
+000116a0: 6b6c 6561 726e 2e70 7265 7072 6f63 6573  klearn.preproces
+000116b0: 7369 6e67 720a 0000 0072 0b00 0000 720c  singr....r....r.
+000116c0: 0000 0072 0d00 0000 720e 0000 0072 0f00  ...r....r....r..
+000116d0: 0000 da06 7479 7069 6e67 7210 0000 0072  ....typingr....r
+000116e0: 1100 0000 7212 0000 0072 1300 0000 7214  ....r....r....r.
+000116f0: 0000 0072 1500 0000 72cd 0000 00da 0864  ...r....r......d
+00011700: 6174 6574 696d 65da 046d 6174 68da 116d  atetime..math..m
+00011710: 6174 706c 6f74 6c69 622e 7079 706c 6f74  atplotlib.pyplot
+00011720: da06 7079 706c 6f74 da03 706c 74da 086e  ..pyplot..plt..n
+00011730: 6574 776f 726b 7872 9d01 0000 da05 6e75  etworkxr......nu
+00011740: 6d70 7972 de00 0000 721e 0000 00da 0670  mpyr....r......p
+00011750: 616e 6461 7372 bf00 0000 7221 0000 0072  andasr....r!...r
+00011760: 2301 0000 72c6 0000 00da 0a74 656e 736f  #...r......tenso
+00011770: 7266 6c6f 77da 0274 6672 2002 0000 7213  rflow..tfr ...r.
+00011780: 0100 00da 1264 6565 706f 662e 6d6f 6465  .....deepof.mode
+00011790: 6c5f 7574 696c 7372 8200 0000 da0d 6465  l_utilsr......de
+000117a0: 6570 6f66 2e6d 6f64 656c 73da 1764 6565  epof.models..dee
+000117b0: 706f 662e 616e 6e6f 7461 7469 6f6e 5f75  pof.annotation_u
+000117c0: 7469 6c73 da0c 6465 6570 6f66 2e75 7469  tils..deepof.uti
+000117d0: 6c73 da0e 6465 6570 6f66 2e76 6973 7561  ls..deepof.visua
+000117e0: 6c73 da07 7072 6f6a 6563 7472 2600 0000  ls..projectr&...
+000117f0: 72fd 0100 0072 a300 0000 7229 0000 0072  r....r....r)...r
+00011800: 2a00 0000 721b 0000 0072 2e01 0000 72db  *...r....r....r.
+00011810: 0000 0072 5900 0000 da07 656e 7669 726f  ...rY.....enviro
+00011820: 6e72 2700 0000 7227 0000 0072 2700 0000  nr'...r'...r'...
+00011830: 7228 0000 00da 083c 6d6f 6475 6c65 3e01  r(.....<module>.
+00011840: 0000 0073 7600 0000 0410 0c01 0c01 0c01  ...sv...........
+00011850: 0c01 0c01 0c01 0c01 0c01 1806 0c01 0c01  ................
+00011860: 1401 1801 0801 0801 0801 0c01 0801 0801  ................
+00011870: 0801 0801 0801 0801 0801 0801 0801 0801  ................
+00011880: 0802 0801 0801 0801 0801 0803 0a01 0a01  ................
+00011890: 0a06 1013 0e7f 007f 007f 007f 007f 000b  ................
+000118a0: 0e7f 007f 007f 007f 007f 007f 007f 003f  ...............?
+000118b0: 107f 007f 007f 007f 007f 004a 0a02       ...........J..
```

### Comparing `deepof-0.5.0/deepof/__pycache__/deepof_train_embeddings.cpython-39.pyc` & `deepof-0.5.1/deepof/__pycache__/deepof_train_embeddings.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepof-0.5.0/deepof/__pycache__/hypermodels.cpython-36.pyc` & `deepof-0.5.1/deepof/__pycache__/hypermodels.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `deepof-0.5.0/deepof/__pycache__/hypermodels.cpython-39.pyc` & `deepof-0.5.1/deepof/__pycache__/hypermodels.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepof-0.5.0/deepof/__pycache__/model_utils.cpython-36.pyc` & `deepof-0.5.1/deepof/__pycache__/model_utils.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `deepof-0.5.0/deepof/__pycache__/model_utils.cpython-39.pyc` & `deepof-0.5.1/deepof/__pycache__/model_utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepof-0.5.0/deepof/__pycache__/models.cpython-36.pyc` & `deepof-0.5.1/deepof/__pycache__/models.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `deepof-0.5.0/deepof/__pycache__/models.cpython-39.pyc` & `deepof-0.5.1/deepof/__pycache__/models.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepof-0.5.0/deepof/__pycache__/pose_utils.cpython-39.pyc` & `deepof-0.5.1/deepof/__pycache__/pose_utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepof-0.5.0/deepof/__pycache__/post_hoc.cpython-39.pyc` & `deepof-0.5.1/deepof/__pycache__/post_hoc.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepof-0.5.0/deepof/__pycache__/preprocess.cpython-36.pyc` & `deepof-0.5.1/deepof/__pycache__/preprocess.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `deepof-0.5.0/deepof/__pycache__/utils.cpython-36.pyc` & `deepof-0.5.1/deepof/__pycache__/utils.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `deepof-0.5.0/deepof/__pycache__/utils.cpython-39.pyc` & `deepof-0.5.1/deepof/__pycache__/utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepof-0.5.0/deepof/__pycache__/visuals.cpython-36.pyc` & `deepof-0.5.1/deepof/__pycache__/visuals.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `deepof-0.5.0/deepof/__pycache__/visuals.cpython-39.pyc` & `deepof-0.5.1/deepof/__pycache__/visuals.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepof-0.5.0/deepof/annotation_utils.py` & `deepof-0.5.1/deepof/annotation_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -592,15 +592,19 @@
         "Center",
         "Spine_2",
         "Left_fhip",
         "Right_fhip",
         "Left_bhip",
         "Right_bhip",
     ]
-    main_body = [body_part for body_part in main_body if body_part in coords.columns]
+    main_body = [
+        body_part
+        for body_part in main_body
+        if any(body_part in col[0] for col in coords.columns)
+    ]
 
     def onebyone_contact(interactors: List, bparts: List):
         """Return a smooth boolean array with 1to1 contacts between two mice."""
         nonlocal raw_coords, animal_ids, params, arena_abs, arena_params
 
         try:
             left = interactors[0] + bparts[0]
@@ -651,15 +655,20 @@
             "Right_ear",
             "Left_fhip",
             "Right_fhip",
             "Left_bhip",
             "Right_bhip",
             "Tail_base",
         ]
-        bparts = [bpart for bpart in bparts if bpart in ovr_speeds.columns]
+        bparts = [
+            bpart
+            for bpart in bparts
+            if bpart
+            if any(bpart in col for col in ovr_speeds.columns)
+        ]
         array = ovr_speeds[[_id + ucond + bpart for bpart in bparts]]
         avg_speed = np.nanmedian(array[1:], axis=1)
         return np.insert(avg_speed, 0, np.nan, axis=0)
 
     # Get all animal ID combinations
     animal_pairs = list(combinations(animal_ids, 2))
```

### Comparing `deepof-0.5.0/deepof/data.py` & `deepof-0.5.1/deepof/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 """
 # @author lucasmiranda42
 # encoding: utf-8
 # module deepof
 
 
 from collections import defaultdict
+from difflib import get_close_matches
 from pkg_resources import resource_filename
 from shapely.geometry import Polygon
 from shutil import rmtree
 from sklearn import random_projection
 from sklearn.decomposition import KernelPCA
 from sklearn.manifold import TSNE
 from sklearn.preprocessing import (
@@ -1475,28 +1476,36 @@
                     self, animal_id=_id, include_angles=False
                 )
                 for _id in self._animal_ids
             }
 
         # noinspection PyTypeChecker
         for key in tqdm(self._tables.keys()):
+
             # Remove indices and add at the very end, to avoid conflicts if
             # frame_rate is specified in project
             tag_index = raw_coords[key].index
+
             supervised_tags = deepof.annotation_utils.supervised_tagging(
                 self,
                 raw_coords=raw_coords,
                 coords=coords,
                 dists=dists,
                 full_features=features_dict,
                 speeds=speeds,
-                video=[vid for vid in self._videos if key][0],
+                video=get_close_matches(
+                    key,
+                    [vid for vid in self._videos if vid.startswith(key)],
+                    cutoff=0.1,
+                    n=1,
+                )[0],
                 trained_model_path=self._trained_model_path,
                 params=params,
             )
+
             supervised_tags.index = tag_index
             tag_dict[key] = supervised_tags
 
         if propagate_labels:  # pragma: no cover
             for key, tab in tag_dict.items():
                 tab["pheno"] = self._exp_conditions[key]
```

### Comparing `deepof-0.5.0/deepof/deepof_train_embeddings.py` & `deepof-0.5.1/deepof/deepof_train_embeddings.py`

 * *Files identical despite different names*

### Comparing `deepof-0.5.0/deepof/hypermodels.py` & `deepof-0.5.1/deepof/hypermodels.py`

 * *Files identical despite different names*

### Comparing `deepof-0.5.0/deepof/model_utils.py` & `deepof-0.5.1/deepof/model_utils.py`

 * *Files identical despite different names*

### Comparing `deepof-0.5.0/deepof/models.py` & `deepof-0.5.1/deepof/models.py`

 * *Files identical despite different names*

### Comparing `deepof-0.5.0/deepof/post_hoc.py` & `deepof-0.5.1/deepof/post_hoc.py`

 * *Files identical despite different names*

### Comparing `deepof-0.5.0/deepof/trained_models/deepof_supervised/deepof_supervised_huddle_estimator.pkl` & `deepof-0.5.1/deepof/trained_models/deepof_supervised/deepof_supervised_huddle_estimator.pkl`

 * *Files identical despite different names*

### Comparing `deepof-0.5.0/deepof/utils.py` & `deepof-0.5.1/deepof/utils.py`

 * *Files identical despite different names*

### Comparing `deepof-0.5.0/deepof/visuals.py` & `deepof-0.5.1/deepof/visuals.py`

 * *Files identical despite different names*

### Comparing `deepof-0.5.0/deepof.egg-info/PKG-INFO` & `deepof-0.5.1/deepof.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepof
-Version: 0.5.0
+Version: 0.5.1
 Summary: A suite for postprocessing time-series extracted from videos of freely moving rodents using DeepLabCut
 Home-page: https://gitlab.mpcdf.mpg.de/lucasmir/deepof/
 Author: Lucas Miranda
 Author-email: lucas_miranda@psych.mpg.de
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -12,15 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Pipeline](https://gitlab.mpcdf.mpg.de/lucasmir/deepof/badges/master/pipeline.svg)](https://gitlab.mpcdf.mpg.de/lucasmir/deepof/-/pipelines)
 [![Coverage](https://gitlab.mpcdf.mpg.de/lucasmir/deepof/badges/master/coverage.svg)](https://coverage.readthedocs.io/en/coverage-5.3/)
 [![Documentation Status](https://readthedocs.org/projects/deepof/badge/?version=latest)](https://deepof.readthedocs.io/en/latest)
 [![CodeFactor](https://www.codefactor.io/repository/github/lucasmiranda42/deepof/badge)](https://www.codefactor.io/repository/github/lucasmiranda42/deepof)
-[![Version](https://img.shields.io/badge/release-v0.5.0-informational)](https://pypi.org/project/deepof/)
+[![Version](https://img.shields.io/badge/release-v0.5.1-informational)](https://pypi.org/project/deepof/)
 [![MLFPM](https://img.shields.io/badge/funding-MLFPM-informational)](https://mlfpm.eu/)
 [![Black](https://img.shields.io/badge/code%20style-black-black)](https://github.com/psf/black)
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.05394/status.svg)](https://doi.org/10.21105/joss.05394)
 
 <br>
 
 <div align="center">
@@ -155,14 +155,31 @@
     volume = {8},
     url = {https://joss.theoj.org/papers/10.21105/joss.05394},
     doi = {10.21105/JOSS.05394},
     issn = {2475-9066}
 }
 ```
 
+```bibtex
+@article{DeepOF:NCOMMS,
+  doi = {10.1038/s41467-023-40040-3},
+  url = {https://doi.org/10.1038/s41467-023-40040-3},
+  year = {2023},
+  month = jul,
+  publisher = {Springer Science and Business Media {LLC}},
+  volume = {14},
+  number = {1},
+  author = {Joeri Bordes and Lucas Miranda and Maya Reinhardt and Sowmya Narayan and Jakob Hartmann and Emily L. Newman and Lea Maria Brix and Lotte van Doeselaar and Clara Engelhardt and Larissa Dillmann and Shiladitya Mitra and Kerry J. Ressler and Benno P\"{u}tz and Felix Agakov and Bertram M\"{u}ller-Myhsok and Mathias V. Schmidt},
+  title = {Automatically annotated motion tracking identifies a distinct social behavioral profile following chronic social defeat stress},
+  journal = {Nature Communications}
+}
+```
+
+All data and code used to generate the results in the NCOMMS paper are available [here](https://datashare.mpcdf.mpg.de/s/3ETwBe1CKk09c9x) (password: *DeepOF2023*).
+
 ---
 ### Issues
 
 If you encounter any problems while using this package, please open an issue in the [issue tracker](https://github.com/mlfpm/deepof/issues).
 
 ---
 ### Contributions
```

### Comparing `deepof-0.5.0/deepof.egg-info/SOURCES.txt` & `deepof-0.5.1/deepof.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepof-0.5.0/deepof.egg-info/requires.txt` & `deepof-0.5.1/deepof.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `deepof-0.5.0/requirements.txt` & `deepof-0.5.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `deepof-0.5.0/setup.py` & `deepof-0.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r") as fp:
     install_requires = [pkg.replace("\n", "") for pkg in fp]
 
 setuptools.setup(
     name="deepof",
-    version="0.5.0",
+    version="0.5.1",
     author="Lucas Miranda",
     author_email="lucas_miranda@psych.mpg.de",
     description="A suite for postprocessing time-series extracted from videos of freely moving rodents using DeepLabCut",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.mpcdf.mpg.de/lucasmir/deepof/",
     packages=setuptools.find_packages(
```

