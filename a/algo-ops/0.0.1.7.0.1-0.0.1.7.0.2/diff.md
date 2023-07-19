# Comparing `tmp/algo-ops-0.0.1.7.0.1.tar.gz` & `tmp/algo-ops-0.0.1.7.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "algo-ops-0.0.1.7.0.1.tar", last modified: Mon Apr 17 04:37:14 2023, max compression
+gzip compressed data, was "algo-ops-0.0.1.7.0.2.tar", last modified: Wed Jul 19 06:31:15 2023, max compression
```

## Comparing `algo-ops-0.0.1.7.0.1.tar` & `algo-ops-0.0.1.7.0.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-17 04:37:14.028335 algo-ops-0.0.1.7.0.1/
--rw-r--r--   0 tandonp    (501) staff       (20)     1071 2022-03-24 04:58:29.000000 algo-ops-0.0.1.7.0.1/LICENSE
--rw-r--r--   0 tandonp    (501) staff       (20)       24 2022-03-21 02:23:19.000000 algo-ops-0.0.1.7.0.1/MANIFEST.in
--rw-r--r--   0 tandonp    (501) staff       (20)     2536 2023-04-17 04:37:14.028164 algo-ops-0.0.1.7.0.1/PKG-INFO
--rw-r--r--   0 tandonp    (501) staff       (20)     2083 2022-06-03 05:15:50.000000 algo-ops-0.0.1.7.0.1/README.md
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-17 04:37:14.023827 algo-ops-0.0.1.7.0.1/algo_ops/
--rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-09 07:46:32.000000 algo-ops-0.0.1.7.0.1/algo_ops/__init__.py
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-17 04:37:14.025261 algo-ops-0.0.1.7.0.1/algo_ops/dependency/
--rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-13 23:06:19.000000 algo-ops-0.0.1.7.0.1/algo_ops/dependency/__init__.py
--rw-r--r--   0 tandonp    (501) staff       (20)     2460 2023-03-19 19:09:30.000000 algo-ops-0.0.1.7.0.1/algo_ops/dependency/sys_util.py
--rw-r--r--   0 tandonp    (501) staff       (20)     5315 2023-03-19 19:10:06.000000 algo-ops-0.0.1.7.0.1/algo_ops/dependency/tester_util.py
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-17 04:37:14.026341 algo-ops-0.0.1.7.0.1/algo_ops/ops/
--rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-13 23:06:19.000000 algo-ops-0.0.1.7.0.1/algo_ops/ops/__init__.py
--rw-r--r--   0 tandonp    (501) staff       (20)     5703 2023-04-17 04:32:50.000000 algo-ops-0.0.1.7.0.1/algo_ops/ops/cv.py
--rw-r--r--   0 tandonp    (501) staff       (20)     7026 2023-03-19 19:09:12.000000 algo-ops-0.0.1.7.0.1/algo_ops/ops/op.py
--rw-r--r--   0 tandonp    (501) staff       (20)       19 2022-06-08 03:22:52.000000 algo-ops-0.0.1.7.0.1/algo_ops/ops/settings.py
--rw-r--r--   0 tandonp    (501) staff       (20)     2213 2022-06-08 03:22:52.000000 algo-ops-0.0.1.7.0.1/algo_ops/ops/text.py
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-17 04:37:14.026693 algo-ops-0.0.1.7.0.1/algo_ops/paraloop/
--rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-02-28 05:34:12.000000 algo-ops-0.0.1.7.0.1/algo_ops/paraloop/__init__.py
--rw-r--r--   0 tandonp    (501) staff       (20)     1911 2023-04-15 23:53:29.000000 algo-ops-0.0.1.7.0.1/algo_ops/paraloop/paraloop.py
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-17 04:37:14.026950 algo-ops-0.0.1.7.0.1/algo_ops/pickleable_object/
--rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-09 07:46:32.000000 algo-ops-0.0.1.7.0.1/algo_ops/pickleable_object/__init__.py
--rw-r--r--   0 tandonp    (501) staff       (20)      760 2023-03-19 19:11:09.000000 algo-ops-0.0.1.7.0.1/algo_ops/pickleable_object/pickleable_object.py
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-17 04:37:14.027590 algo-ops-0.0.1.7.0.1/algo_ops/pipeline/
--rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-13 23:06:19.000000 algo-ops-0.0.1.7.0.1/algo_ops/pipeline/__init__.py
--rw-r--r--   0 tandonp    (501) staff       (20)     3396 2023-03-19 19:11:29.000000 algo-ops-0.0.1.7.0.1/algo_ops/pipeline/cv_pipeline.py
--rw-r--r--   0 tandonp    (501) staff       (20)     7637 2023-03-19 19:13:35.000000 algo-ops-0.0.1.7.0.1/algo_ops/pipeline/pipeline.py
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-17 04:37:14.027947 algo-ops-0.0.1.7.0.1/algo_ops/plot/
--rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-13 23:06:19.000000 algo-ops-0.0.1.7.0.1/algo_ops/plot/__init__.py
--rw-r--r--   0 tandonp    (501) staff       (20)     2080 2023-03-19 19:14:03.000000 algo-ops-0.0.1.7.0.1/algo_ops/plot/plot.py
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-17 04:37:14.024609 algo-ops-0.0.1.7.0.1/algo_ops.egg-info/
--rw-r--r--   0 tandonp    (501) staff       (20)     2536 2023-04-17 04:37:13.000000 algo-ops-0.0.1.7.0.1/algo_ops.egg-info/PKG-INFO
--rw-r--r--   0 tandonp    (501) staff       (20)      746 2023-04-17 04:37:13.000000 algo-ops-0.0.1.7.0.1/algo_ops.egg-info/SOURCES.txt
--rw-r--r--   0 tandonp    (501) staff       (20)        1 2023-04-17 04:37:13.000000 algo-ops-0.0.1.7.0.1/algo_ops.egg-info/dependency_links.txt
--rw-r--r--   0 tandonp    (501) staff       (20)       75 2023-04-17 04:37:13.000000 algo-ops-0.0.1.7.0.1/algo_ops.egg-info/requires.txt
--rw-r--r--   0 tandonp    (501) staff       (20)        9 2023-04-17 04:37:13.000000 algo-ops-0.0.1.7.0.1/algo_ops.egg-info/top_level.txt
--rw-r--r--   0 tandonp    (501) staff       (20)      195 2023-03-19 19:54:12.000000 algo-ops-0.0.1.7.0.1/pyproject.toml
--rw-r--r--   0 tandonp    (501) staff       (20)       74 2023-03-18 06:13:49.000000 algo-ops-0.0.1.7.0.1/requirements.txt
--rw-r--r--   0 tandonp    (501) staff       (20)       38 2023-04-17 04:37:14.028380 algo-ops-0.0.1.7.0.1/setup.cfg
--rw-r--r--   0 tandonp    (501) staff       (20)      791 2023-04-17 04:37:02.000000 algo-ops-0.0.1.7.0.1/setup.py
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-07-19 06:31:15.560046 algo-ops-0.0.1.7.0.2/
+-rw-r--r--   0 tandonp    (501) staff       (20)     1071 2022-03-24 04:58:29.000000 algo-ops-0.0.1.7.0.2/LICENSE
+-rw-r--r--   0 tandonp    (501) staff       (20)       24 2022-03-21 02:23:19.000000 algo-ops-0.0.1.7.0.2/MANIFEST.in
+-rw-r--r--   0 tandonp    (501) staff       (20)     2537 2023-07-19 06:31:15.559880 algo-ops-0.0.1.7.0.2/PKG-INFO
+-rw-r--r--   0 tandonp    (501) staff       (20)     2083 2022-06-03 05:15:50.000000 algo-ops-0.0.1.7.0.2/README.md
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-07-19 06:31:15.556429 algo-ops-0.0.1.7.0.2/algo_ops/
+-rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-09 07:46:32.000000 algo-ops-0.0.1.7.0.2/algo_ops/__init__.py
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-07-19 06:31:15.557526 algo-ops-0.0.1.7.0.2/algo_ops/dependency/
+-rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-13 23:06:19.000000 algo-ops-0.0.1.7.0.2/algo_ops/dependency/__init__.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     2460 2023-03-19 19:09:30.000000 algo-ops-0.0.1.7.0.2/algo_ops/dependency/sys_util.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     5315 2023-03-19 19:10:06.000000 algo-ops-0.0.1.7.0.2/algo_ops/dependency/tester_util.py
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-07-19 06:31:15.558179 algo-ops-0.0.1.7.0.2/algo_ops/ops/
+-rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-13 23:06:19.000000 algo-ops-0.0.1.7.0.2/algo_ops/ops/__init__.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     5703 2023-04-17 04:32:50.000000 algo-ops-0.0.1.7.0.2/algo_ops/ops/cv.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     7026 2023-03-19 19:09:12.000000 algo-ops-0.0.1.7.0.2/algo_ops/ops/op.py
+-rw-r--r--   0 tandonp    (501) staff       (20)       19 2022-06-08 03:22:52.000000 algo-ops-0.0.1.7.0.2/algo_ops/ops/settings.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     2213 2022-06-08 03:22:52.000000 algo-ops-0.0.1.7.0.2/algo_ops/ops/text.py
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-07-19 06:31:15.558662 algo-ops-0.0.1.7.0.2/algo_ops/paraloop/
+-rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-02-28 05:34:12.000000 algo-ops-0.0.1.7.0.2/algo_ops/paraloop/__init__.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     1911 2023-04-15 23:53:29.000000 algo-ops-0.0.1.7.0.2/algo_ops/paraloop/paraloop.py
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-07-19 06:31:15.558965 algo-ops-0.0.1.7.0.2/algo_ops/pickleable_object/
+-rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-09 07:46:32.000000 algo-ops-0.0.1.7.0.2/algo_ops/pickleable_object/__init__.py
+-rw-r--r--   0 tandonp    (501) staff       (20)      760 2023-03-19 19:11:09.000000 algo-ops-0.0.1.7.0.2/algo_ops/pickleable_object/pickleable_object.py
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-07-19 06:31:15.559386 algo-ops-0.0.1.7.0.2/algo_ops/pipeline/
+-rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-13 23:06:19.000000 algo-ops-0.0.1.7.0.2/algo_ops/pipeline/__init__.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     3396 2023-03-19 19:11:29.000000 algo-ops-0.0.1.7.0.2/algo_ops/pipeline/cv_pipeline.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     7637 2023-03-19 19:13:35.000000 algo-ops-0.0.1.7.0.2/algo_ops/pipeline/pipeline.py
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-07-19 06:31:15.559670 algo-ops-0.0.1.7.0.2/algo_ops/plot/
+-rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-03-13 23:06:19.000000 algo-ops-0.0.1.7.0.2/algo_ops/plot/__init__.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     2080 2023-03-19 19:14:03.000000 algo-ops-0.0.1.7.0.2/algo_ops/plot/plot.py
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-07-19 06:31:15.557144 algo-ops-0.0.1.7.0.2/algo_ops.egg-info/
+-rw-r--r--   0 tandonp    (501) staff       (20)     2537 2023-07-19 06:31:15.000000 algo-ops-0.0.1.7.0.2/algo_ops.egg-info/PKG-INFO
+-rw-r--r--   0 tandonp    (501) staff       (20)      746 2023-07-19 06:31:15.000000 algo-ops-0.0.1.7.0.2/algo_ops.egg-info/SOURCES.txt
+-rw-r--r--   0 tandonp    (501) staff       (20)        1 2023-07-19 06:31:15.000000 algo-ops-0.0.1.7.0.2/algo_ops.egg-info/dependency_links.txt
+-rw-r--r--   0 tandonp    (501) staff       (20)       75 2023-07-19 06:31:15.000000 algo-ops-0.0.1.7.0.2/algo_ops.egg-info/requires.txt
+-rw-r--r--   0 tandonp    (501) staff       (20)        9 2023-07-19 06:31:15.000000 algo-ops-0.0.1.7.0.2/algo_ops.egg-info/top_level.txt
+-rw-r--r--   0 tandonp    (501) staff       (20)      195 2023-03-19 19:54:12.000000 algo-ops-0.0.1.7.0.2/pyproject.toml
+-rw-r--r--   0 tandonp    (501) staff       (20)       74 2023-03-18 06:13:49.000000 algo-ops-0.0.1.7.0.2/requirements.txt
+-rw-r--r--   0 tandonp    (501) staff       (20)       38 2023-07-19 06:31:15.560101 algo-ops-0.0.1.7.0.2/setup.cfg
+-rw-r--r--   0 tandonp    (501) staff       (20)      792 2023-07-19 06:31:11.000000 algo-ops-0.0.1.7.0.2/setup.py
```

### Comparing `algo-ops-0.0.1.7.0.1/LICENSE` & `algo-ops-0.0.1.7.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `algo-ops-0.0.1.7.0.1/PKG-INFO` & `algo-ops-0.0.1.7.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: algo-ops
-Version: 0.0.1.7.0.1
+Version: 0.0.1.7.0.2
 Summary: Algo-Ops Algorithm Prototyping Framework
 Home-page: https://github.com/prateekt/algo-ops
 Author: Prateek Tandon
 Author-email: prateek1.tandon@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9.7
+Requires-Python: >=3.11.4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Algo-Ops
 
 Pipeline Infrastructure for Prototyping and Deploying Algorithms
```

### Comparing `algo-ops-0.0.1.7.0.1/README.md` & `algo-ops-0.0.1.7.0.2/README.md`

 * *Files identical despite different names*

### Comparing `algo-ops-0.0.1.7.0.1/algo_ops/dependency/sys_util.py` & `algo-ops-0.0.1.7.0.2/algo_ops/dependency/sys_util.py`

 * *Files identical despite different names*

### Comparing `algo-ops-0.0.1.7.0.1/algo_ops/dependency/tester_util.py` & `algo-ops-0.0.1.7.0.2/algo_ops/dependency/tester_util.py`

 * *Files identical despite different names*

### Comparing `algo-ops-0.0.1.7.0.1/algo_ops/ops/cv.py` & `algo-ops-0.0.1.7.0.2/algo_ops/ops/cv.py`

 * *Files identical despite different names*

### Comparing `algo-ops-0.0.1.7.0.1/algo_ops/ops/op.py` & `algo-ops-0.0.1.7.0.2/algo_ops/ops/op.py`

 * *Files identical despite different names*

### Comparing `algo-ops-0.0.1.7.0.1/algo_ops/ops/text.py` & `algo-ops-0.0.1.7.0.2/algo_ops/ops/text.py`

 * *Files identical despite different names*

### Comparing `algo-ops-0.0.1.7.0.1/algo_ops/paraloop/paraloop.py` & `algo-ops-0.0.1.7.0.2/algo_ops/paraloop/paraloop.py`

 * *Files identical despite different names*

### Comparing `algo-ops-0.0.1.7.0.1/algo_ops/pickleable_object/pickleable_object.py` & `algo-ops-0.0.1.7.0.2/algo_ops/pickleable_object/pickleable_object.py`

 * *Files identical despite different names*

### Comparing `algo-ops-0.0.1.7.0.1/algo_ops/pipeline/cv_pipeline.py` & `algo-ops-0.0.1.7.0.2/algo_ops/pipeline/cv_pipeline.py`

 * *Files identical despite different names*

### Comparing `algo-ops-0.0.1.7.0.1/algo_ops/pipeline/pipeline.py` & `algo-ops-0.0.1.7.0.2/algo_ops/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `algo-ops-0.0.1.7.0.1/algo_ops/plot/plot.py` & `algo-ops-0.0.1.7.0.2/algo_ops/plot/plot.py`

 * *Files identical despite different names*

### Comparing `algo-ops-0.0.1.7.0.1/algo_ops.egg-info/PKG-INFO` & `algo-ops-0.0.1.7.0.2/algo_ops.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: algo-ops
-Version: 0.0.1.7.0.1
+Version: 0.0.1.7.0.2
 Summary: Algo-Ops Algorithm Prototyping Framework
 Home-page: https://github.com/prateekt/algo-ops
 Author: Prateek Tandon
 Author-email: prateek1.tandon@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9.7
+Requires-Python: >=3.11.4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Algo-Ops
 
 Pipeline Infrastructure for Prototyping and Deploying Algorithms
```

### Comparing `algo-ops-0.0.1.7.0.1/algo_ops.egg-info/SOURCES.txt` & `algo-ops-0.0.1.7.0.2/algo_ops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `algo-ops-0.0.1.7.0.1/setup.py` & `algo-ops-0.0.1.7.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 with open("requirements.txt") as f:
     required = f.read().splitlines()
 
 setuptools.setup(
     name="algo-ops",
-    version="0.0.1.7.0.1",
+    version="0.0.1.7.0.2",
     author="Prateek Tandon",
     author_email="prateek1.tandon@gmail.com",
     description="Algo-Ops Algorithm Prototyping Framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/prateekt/algo-ops",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires=">=3.9.7",
+    python_requires=">=3.11.4",
     install_requires=required,
 )
```

