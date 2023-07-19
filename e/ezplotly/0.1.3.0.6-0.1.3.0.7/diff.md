# Comparing `tmp/ezplotly-0.1.3.0.6.tar.gz` & `tmp/ezplotly-0.1.3.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezplotly-0.1.3.0.6.tar", last modified: Sun Apr  2 20:23:19 2023, max compression
+gzip compressed data, was "ezplotly-0.1.3.0.7.tar", last modified: Wed Jul 19 06:40:44 2023, max compression
```

## Comparing `ezplotly-0.1.3.0.6.tar` & `ezplotly-0.1.3.0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-02 20:23:19.391949 ezplotly-0.1.3.0.6/
--rw-r--r--   0 tandonp    (501) staff       (20)     1073 2022-03-26 01:28:59.000000 ezplotly-0.1.3.0.6/LICENSE.txt
--rw-r--r--   0 tandonp    (501) staff       (20)       24 2022-03-26 01:28:59.000000 ezplotly-0.1.3.0.6/MANIFEST.in
--rw-r--r--   0 tandonp    (501) staff       (20)     2200 2023-04-02 20:23:19.391800 ezplotly-0.1.3.0.6/PKG-INFO
--rw-r--r--   0 tandonp    (501) staff       (20)     1726 2022-06-03 04:18:36.000000 ezplotly-0.1.3.0.6/README.md
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-02 20:23:19.390320 ezplotly-0.1.3.0.6/ezplotly/
--rw-r--r--   0 tandonp    (501) staff       (20)       24 2022-03-26 01:28:59.000000 ezplotly-0.1.3.0.6/ezplotly/__init__.py
--rw-r--r--   0 tandonp    (501) staff       (20)    41486 2023-03-18 05:34:37.000000 ezplotly-0.1.3.0.6/ezplotly/ezplotly.py
--rw-r--r--   0 tandonp    (501) staff       (20)      960 2023-04-01 23:18:30.000000 ezplotly-0.1.3.0.6/ezplotly/settings.py
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-02 20:23:19.391031 ezplotly-0.1.3.0.6/ezplotly.egg-info/
--rw-r--r--   0 tandonp    (501) staff       (20)     2200 2023-04-02 20:23:19.000000 ezplotly-0.1.3.0.6/ezplotly.egg-info/PKG-INFO
--rw-r--r--   0 tandonp    (501) staff       (20)      389 2023-04-02 20:23:19.000000 ezplotly-0.1.3.0.6/ezplotly.egg-info/SOURCES.txt
--rw-r--r--   0 tandonp    (501) staff       (20)        1 2023-04-02 20:23:19.000000 ezplotly-0.1.3.0.6/ezplotly.egg-info/dependency_links.txt
--rw-r--r--   0 tandonp    (501) staff       (20)       81 2023-04-02 20:23:19.000000 ezplotly-0.1.3.0.6/ezplotly.egg-info/requires.txt
--rw-r--r--   0 tandonp    (501) staff       (20)       30 2023-04-02 20:23:19.000000 ezplotly-0.1.3.0.6/ezplotly.egg-info/top_level.txt
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-02 20:23:19.391307 ezplotly-0.1.3.0.6/ezplotly_bio/
--rw-r--r--   0 tandonp    (501) staff       (20)       28 2022-03-26 01:28:59.000000 ezplotly-0.1.3.0.6/ezplotly_bio/__init__.py
--rw-r--r--   0 tandonp    (501) staff       (20)    30234 2023-03-18 05:34:37.000000 ezplotly-0.1.3.0.6/ezplotly_bio/ezplotly_bio.py
--rw-r--r--   0 tandonp    (501) staff       (20)      193 2023-04-01 23:18:30.000000 ezplotly-0.1.3.0.6/pyproject.toml
--rw-r--r--   0 tandonp    (501) staff       (20)       80 2022-06-07 09:37:11.000000 ezplotly-0.1.3.0.6/requirements.txt
--rw-r--r--   0 tandonp    (501) staff       (20)       38 2023-04-02 20:23:19.391996 ezplotly-0.1.3.0.6/setup.cfg
--rw-r--r--   0 tandonp    (501) staff       (20)      789 2023-04-02 20:22:02.000000 ezplotly-0.1.3.0.6/setup.py
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-02 20:23:19.391604 ezplotly-0.1.3.0.6/yayrocs/
--rw-r--r--   0 tandonp    (501) staff       (20)       23 2022-03-26 01:28:59.000000 ezplotly-0.1.3.0.6/yayrocs/__init__.py
--rw-r--r--   0 tandonp    (501) staff       (20)     6561 2022-03-26 01:28:59.000000 ezplotly-0.1.3.0.6/yayrocs/yayrocs.py
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-07-19 06:40:44.880792 ezplotly-0.1.3.0.7/
+-rw-r--r--   0 tandonp    (501) staff       (20)     1073 2022-03-26 01:28:59.000000 ezplotly-0.1.3.0.7/LICENSE.txt
+-rw-r--r--   0 tandonp    (501) staff       (20)       24 2022-03-26 01:28:59.000000 ezplotly-0.1.3.0.7/MANIFEST.in
+-rw-r--r--   0 tandonp    (501) staff       (20)     2203 2023-07-19 06:40:44.880549 ezplotly-0.1.3.0.7/PKG-INFO
+-rw-r--r--   0 tandonp    (501) staff       (20)     1726 2022-06-03 04:18:36.000000 ezplotly-0.1.3.0.7/README.md
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-07-19 06:40:44.878978 ezplotly-0.1.3.0.7/ezplotly/
+-rw-r--r--   0 tandonp    (501) staff       (20)       24 2022-03-26 01:28:59.000000 ezplotly-0.1.3.0.7/ezplotly/__init__.py
+-rw-r--r--   0 tandonp    (501) staff       (20)    41486 2023-03-18 05:34:37.000000 ezplotly-0.1.3.0.7/ezplotly/ezplotly.py
+-rw-r--r--   0 tandonp    (501) staff       (20)      960 2023-04-01 23:18:30.000000 ezplotly-0.1.3.0.7/ezplotly/settings.py
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-07-19 06:40:44.879738 ezplotly-0.1.3.0.7/ezplotly.egg-info/
+-rw-r--r--   0 tandonp    (501) staff       (20)     2203 2023-07-19 06:40:44.000000 ezplotly-0.1.3.0.7/ezplotly.egg-info/PKG-INFO
+-rw-r--r--   0 tandonp    (501) staff       (20)      389 2023-07-19 06:40:44.000000 ezplotly-0.1.3.0.7/ezplotly.egg-info/SOURCES.txt
+-rw-r--r--   0 tandonp    (501) staff       (20)        1 2023-07-19 06:40:44.000000 ezplotly-0.1.3.0.7/ezplotly.egg-info/dependency_links.txt
+-rw-r--r--   0 tandonp    (501) staff       (20)       81 2023-07-19 06:40:44.000000 ezplotly-0.1.3.0.7/ezplotly.egg-info/requires.txt
+-rw-r--r--   0 tandonp    (501) staff       (20)       30 2023-07-19 06:40:44.000000 ezplotly-0.1.3.0.7/ezplotly.egg-info/top_level.txt
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-07-19 06:40:44.880014 ezplotly-0.1.3.0.7/ezplotly_bio/
+-rw-r--r--   0 tandonp    (501) staff       (20)       28 2022-03-26 01:28:59.000000 ezplotly-0.1.3.0.7/ezplotly_bio/__init__.py
+-rw-r--r--   0 tandonp    (501) staff       (20)    30234 2023-03-18 05:34:37.000000 ezplotly-0.1.3.0.7/ezplotly_bio/ezplotly_bio.py
+-rw-r--r--   0 tandonp    (501) staff       (20)      193 2023-04-01 23:18:30.000000 ezplotly-0.1.3.0.7/pyproject.toml
+-rw-r--r--   0 tandonp    (501) staff       (20)       80 2022-06-07 09:37:11.000000 ezplotly-0.1.3.0.7/requirements.txt
+-rw-r--r--   0 tandonp    (501) staff       (20)       38 2023-07-19 06:40:44.880840 ezplotly-0.1.3.0.7/setup.cfg
+-rw-r--r--   0 tandonp    (501) staff       (20)      792 2023-07-19 06:39:57.000000 ezplotly-0.1.3.0.7/setup.py
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-07-19 06:40:44.880366 ezplotly-0.1.3.0.7/yayrocs/
+-rw-r--r--   0 tandonp    (501) staff       (20)       23 2022-03-26 01:28:59.000000 ezplotly-0.1.3.0.7/yayrocs/__init__.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     6561 2022-03-26 01:28:59.000000 ezplotly-0.1.3.0.7/yayrocs/yayrocs.py
```

### Comparing `ezplotly-0.1.3.0.6/LICENSE.txt` & `ezplotly-0.1.3.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ezplotly-0.1.3.0.6/PKG-INFO` & `ezplotly-0.1.3.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: ezplotly
-Version: 0.1.3.0.6
+Version: 0.1.3.0.7
 Summary: An easy wrapper for making Plotly plots in Jupyter notebooks
 Home-page: https://github.com/prateekt/ezplotly
 Author: Prateek Tandon
 Author-email: prateek1.tandon@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.11.4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # EZPlotly and EZPlotly_bio For Jupyter Notebooks
 Introducing EZPlotly: An easy, intuitive wrapper for making Plotly plots in Jupyter notebooks
 
 Plotly offers interactive plots, as opposed to the static plots that most other python visualization tools provide. However, Plotly syntax can be challenging to write, whereas the other libraries are a lot easier to plot with. EZPlotly helps bridge the gap. EZPlotly makes plotting with Plotly simpler and more matplotlib or matlab-like for experienced users of those toolsets.
```

### Comparing `ezplotly-0.1.3.0.6/README.md` & `ezplotly-0.1.3.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ezplotly-0.1.3.0.6/ezplotly/ezplotly.py` & `ezplotly-0.1.3.0.7/ezplotly/ezplotly.py`

 * *Files identical despite different names*

### Comparing `ezplotly-0.1.3.0.6/ezplotly/settings.py` & `ezplotly-0.1.3.0.7/ezplotly/settings.py`

 * *Files identical despite different names*

### Comparing `ezplotly-0.1.3.0.6/ezplotly.egg-info/PKG-INFO` & `ezplotly-0.1.3.0.7/ezplotly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: ezplotly
-Version: 0.1.3.0.6
+Version: 0.1.3.0.7
 Summary: An easy wrapper for making Plotly plots in Jupyter notebooks
 Home-page: https://github.com/prateekt/ezplotly
 Author: Prateek Tandon
 Author-email: prateek1.tandon@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.11.4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # EZPlotly and EZPlotly_bio For Jupyter Notebooks
 Introducing EZPlotly: An easy, intuitive wrapper for making Plotly plots in Jupyter notebooks
 
 Plotly offers interactive plots, as opposed to the static plots that most other python visualization tools provide. However, Plotly syntax can be challenging to write, whereas the other libraries are a lot easier to plot with. EZPlotly helps bridge the gap. EZPlotly makes plotting with Plotly simpler and more matplotlib or matlab-like for experienced users of those toolsets.
```

### Comparing `ezplotly-0.1.3.0.6/ezplotly_bio/ezplotly_bio.py` & `ezplotly-0.1.3.0.7/ezplotly_bio/ezplotly_bio.py`

 * *Files identical despite different names*

### Comparing `ezplotly-0.1.3.0.6/setup.py` & `ezplotly-0.1.3.0.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 with open("requirements.txt") as f:
     required = f.read().splitlines()
 
 setuptools.setup(
     name="ezplotly",
-    version="0.1.3.0.6",
+    version="0.1.3.0.7",
     author="Prateek Tandon",
     author_email="prateek1.tandon@gmail.com",
     description="An easy wrapper for making Plotly plots in Jupyter notebooks",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/prateekt/ezplotly",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires=">=3.6",
+    python_requires=">=3.11.4",
     install_requires=required,
 )
```

### Comparing `ezplotly-0.1.3.0.6/yayrocs/yayrocs.py` & `ezplotly-0.1.3.0.7/yayrocs/yayrocs.py`

 * *Files identical despite different names*

