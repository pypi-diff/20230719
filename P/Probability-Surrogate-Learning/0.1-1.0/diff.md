# Comparing `tmp/Probability-Surrogate-Learning-0.1.tar.gz` & `tmp/Probability-Surrogate-Learning-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Probability-Surrogate-Learning-0.1.tar", last modified: Tue Jul 18 22:40:43 2023, max compression
+gzip compressed data, was "Probability-Surrogate-Learning-1.0.tar", last modified: Tue Jul 18 22:44:45 2023, max compression
```

## Comparing `Probability-Surrogate-Learning-0.1.tar` & `Probability-Surrogate-Learning-1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 liwenlin   (501) staff       (20)        0 2023-07-18 22:40:43.989112 Probability-Surrogate-Learning-0.1/
-drwxr-xr-x   0 liwenlin   (501) staff       (20)        0 2023-07-18 22:40:43.986386 Probability-Surrogate-Learning-0.1/Data-Generator/
--rw-r--r--   0 liwenlin   (501) staff       (20)        0 2023-07-16 09:38:25.000000 Probability-Surrogate-Learning-0.1/Data-Generator/__init__.py
-drwxr-xr-x   0 liwenlin   (501) staff       (20)        0 2023-07-18 22:40:43.987275 Probability-Surrogate-Learning-0.1/Data-Generator/data/
--rw-r--r--   0 liwenlin   (501) staff       (20)        0 2023-07-16 09:38:25.000000 Probability-Surrogate-Learning-0.1/Data-Generator/data/__init__.py
--rw-r--r--   0 liwenlin   (501) staff       (20)    20533 2023-07-16 09:38:30.000000 Probability-Surrogate-Learning-0.1/Data-Generator/data/pde_solvers.py
--rw-r--r--   0 liwenlin   (501) staff       (20)    12807 2023-07-16 09:38:30.000000 Probability-Surrogate-Learning-0.1/Data-Generator/data/rawdata.py
--rw-r--r--   0 liwenlin   (501) staff       (20)     2328 2023-07-16 09:38:30.000000 Probability-Surrogate-Learning-0.1/Data-Generator/generate.py
-drwxr-xr-x   0 liwenlin   (501) staff       (20)        0 2023-07-18 22:40:43.988136 Probability-Surrogate-Learning-0.1/Data-Generator/infras/
--rw-r--r--   0 liwenlin   (501) staff       (20)        0 2023-07-16 09:38:30.000000 Probability-Surrogate-Learning-0.1/Data-Generator/infras/__init__.py
--rw-r--r--   0 liwenlin   (501) staff       (20)     4388 2023-07-16 09:38:30.000000 Probability-Surrogate-Learning-0.1/Data-Generator/infras/configs.py
--rw-r--r--   0 liwenlin   (501) staff       (20)     5432 2023-07-16 09:38:30.000000 Probability-Surrogate-Learning-0.1/Data-Generator/infras/misc.py
--rw-r--r--   0 liwenlin   (501) staff       (20)     4574 2023-07-16 09:38:30.000000 Probability-Surrogate-Learning-0.1/Data-Generator/infras/randutils.py
--rw-r--r--   0 liwenlin   (501) staff       (20)     6679 2023-07-16 09:38:30.000000 Probability-Surrogate-Learning-0.1/Data-Generator/infras/utils.py
--rw-r--r--   0 liwenlin   (501) staff       (20)     1066 2023-07-16 09:38:33.000000 Probability-Surrogate-Learning-0.1/LICENSE.md
--rw-r--r--   0 liwenlin   (501) staff       (20)     8067 2023-07-18 22:40:43.988930 Probability-Surrogate-Learning-0.1/PKG-INFO
-drwxr-xr-x   0 liwenlin   (501) staff       (20)        0 2023-07-18 22:40:43.988735 Probability-Surrogate-Learning-0.1/Probability_Surrogate_Learning.egg-info/
--rw-r--r--   0 liwenlin   (501) staff       (20)     8067 2023-07-18 22:40:43.000000 Probability-Surrogate-Learning-0.1/Probability_Surrogate_Learning.egg-info/PKG-INFO
--rw-r--r--   0 liwenlin   (501) staff       (20)      560 2023-07-18 22:40:43.000000 Probability-Surrogate-Learning-0.1/Probability_Surrogate_Learning.egg-info/SOURCES.txt
--rw-r--r--   0 liwenlin   (501) staff       (20)        1 2023-07-18 22:40:43.000000 Probability-Surrogate-Learning-0.1/Probability_Surrogate_Learning.egg-info/dependency_links.txt
--rw-r--r--   0 liwenlin   (501) staff       (20)       15 2023-07-18 22:40:43.000000 Probability-Surrogate-Learning-0.1/Probability_Surrogate_Learning.egg-info/top_level.txt
--rw-r--r--   0 liwenlin   (501) staff       (20)     7525 2023-07-18 21:11:45.000000 Probability-Surrogate-Learning-0.1/README.md
--rw-r--r--   0 liwenlin   (501) staff       (20)       38 2023-07-18 22:40:43.989186 Probability-Surrogate-Learning-0.1/setup.cfg
--rw-r--r--   0 liwenlin   (501) staff       (20)      710 2023-07-18 22:36:24.000000 Probability-Surrogate-Learning-0.1/setup.py
+drwxr-xr-x   0 liwenlin   (501) staff       (20)        0 2023-07-18 22:44:45.325955 Probability-Surrogate-Learning-1.0/
+drwxr-xr-x   0 liwenlin   (501) staff       (20)        0 2023-07-18 22:44:45.322842 Probability-Surrogate-Learning-1.0/Data-Generator/
+-rw-r--r--   0 liwenlin   (501) staff       (20)        0 2023-07-16 09:38:25.000000 Probability-Surrogate-Learning-1.0/Data-Generator/__init__.py
+drwxr-xr-x   0 liwenlin   (501) staff       (20)        0 2023-07-18 22:44:45.323785 Probability-Surrogate-Learning-1.0/Data-Generator/data/
+-rw-r--r--   0 liwenlin   (501) staff       (20)        0 2023-07-16 09:38:25.000000 Probability-Surrogate-Learning-1.0/Data-Generator/data/__init__.py
+-rw-r--r--   0 liwenlin   (501) staff       (20)    20533 2023-07-16 09:38:30.000000 Probability-Surrogate-Learning-1.0/Data-Generator/data/pde_solvers.py
+-rw-r--r--   0 liwenlin   (501) staff       (20)    12807 2023-07-16 09:38:30.000000 Probability-Surrogate-Learning-1.0/Data-Generator/data/rawdata.py
+-rw-r--r--   0 liwenlin   (501) staff       (20)     2328 2023-07-16 09:38:30.000000 Probability-Surrogate-Learning-1.0/Data-Generator/generate.py
+drwxr-xr-x   0 liwenlin   (501) staff       (20)        0 2023-07-18 22:44:45.324922 Probability-Surrogate-Learning-1.0/Data-Generator/infras/
+-rw-r--r--   0 liwenlin   (501) staff       (20)        0 2023-07-16 09:38:30.000000 Probability-Surrogate-Learning-1.0/Data-Generator/infras/__init__.py
+-rw-r--r--   0 liwenlin   (501) staff       (20)     4388 2023-07-16 09:38:30.000000 Probability-Surrogate-Learning-1.0/Data-Generator/infras/configs.py
+-rw-r--r--   0 liwenlin   (501) staff       (20)     5432 2023-07-16 09:38:30.000000 Probability-Surrogate-Learning-1.0/Data-Generator/infras/misc.py
+-rw-r--r--   0 liwenlin   (501) staff       (20)     4574 2023-07-16 09:38:30.000000 Probability-Surrogate-Learning-1.0/Data-Generator/infras/randutils.py
+-rw-r--r--   0 liwenlin   (501) staff       (20)     6679 2023-07-16 09:38:30.000000 Probability-Surrogate-Learning-1.0/Data-Generator/infras/utils.py
+-rw-r--r--   0 liwenlin   (501) staff       (20)     1066 2023-07-16 09:38:33.000000 Probability-Surrogate-Learning-1.0/LICENSE.md
+-rw-r--r--   0 liwenlin   (501) staff       (20)     8184 2023-07-18 22:44:45.325810 Probability-Surrogate-Learning-1.0/PKG-INFO
+drwxr-xr-x   0 liwenlin   (501) staff       (20)        0 2023-07-18 22:44:45.325574 Probability-Surrogate-Learning-1.0/Probability_Surrogate_Learning.egg-info/
+-rw-r--r--   0 liwenlin   (501) staff       (20)     8184 2023-07-18 22:44:45.000000 Probability-Surrogate-Learning-1.0/Probability_Surrogate_Learning.egg-info/PKG-INFO
+-rw-r--r--   0 liwenlin   (501) staff       (20)      560 2023-07-18 22:44:45.000000 Probability-Surrogate-Learning-1.0/Probability_Surrogate_Learning.egg-info/SOURCES.txt
+-rw-r--r--   0 liwenlin   (501) staff       (20)        1 2023-07-18 22:44:45.000000 Probability-Surrogate-Learning-1.0/Probability_Surrogate_Learning.egg-info/dependency_links.txt
+-rw-r--r--   0 liwenlin   (501) staff       (20)       15 2023-07-18 22:44:45.000000 Probability-Surrogate-Learning-1.0/Probability_Surrogate_Learning.egg-info/top_level.txt
+-rw-r--r--   0 liwenlin   (501) staff       (20)     7642 2023-07-18 22:43:06.000000 Probability-Surrogate-Learning-1.0/README.md
+-rw-r--r--   0 liwenlin   (501) staff       (20)       38 2023-07-18 22:44:45.326004 Probability-Surrogate-Learning-1.0/setup.cfg
+-rw-r--r--   0 liwenlin   (501) staff       (20)      710 2023-07-18 22:44:37.000000 Probability-Surrogate-Learning-1.0/setup.py
```

### Comparing `Probability-Surrogate-Learning-0.1/Data-Generator/data/pde_solvers.py` & `Probability-Surrogate-Learning-1.0/Data-Generator/data/pde_solvers.py`

 * *Files identical despite different names*

### Comparing `Probability-Surrogate-Learning-0.1/Data-Generator/data/rawdata.py` & `Probability-Surrogate-Learning-1.0/Data-Generator/data/rawdata.py`

 * *Files identical despite different names*

### Comparing `Probability-Surrogate-Learning-0.1/Data-Generator/generate.py` & `Probability-Surrogate-Learning-1.0/Data-Generator/generate.py`

 * *Files identical despite different names*

### Comparing `Probability-Surrogate-Learning-0.1/Data-Generator/infras/configs.py` & `Probability-Surrogate-Learning-1.0/Data-Generator/infras/configs.py`

 * *Files identical despite different names*

### Comparing `Probability-Surrogate-Learning-0.1/Data-Generator/infras/misc.py` & `Probability-Surrogate-Learning-1.0/Data-Generator/infras/misc.py`

 * *Files identical despite different names*

### Comparing `Probability-Surrogate-Learning-0.1/Data-Generator/infras/randutils.py` & `Probability-Surrogate-Learning-1.0/Data-Generator/infras/randutils.py`

 * *Files identical despite different names*

### Comparing `Probability-Surrogate-Learning-0.1/Data-Generator/infras/utils.py` & `Probability-Surrogate-Learning-1.0/Data-Generator/infras/utils.py`

 * *Files identical despite different names*

### Comparing `Probability-Surrogate-Learning-0.1/LICENSE.md` & `Probability-Surrogate-Learning-1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Probability-Surrogate-Learning-0.1/PKG-INFO` & `Probability-Surrogate-Learning-1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 Metadata-Version: 2.1
 Name: Probability-Surrogate-Learning
-Version: 0.1
+Version: 1.0
 Summary: This is a comprehensive machine learning library, specifically tailored for surrogate learning and active learning.
 Home-page: https://github.com/liwenlin664477/Probability-Surrogate-Learning
 Author: Wenlin Li
 Author-email: u1327012@example.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Probability-Surrogate-Learning
 This is a comprehensive machine learning library, specifically tailored for surrogate learning and active learning. Our objective is to provide a robust platform that empowers researchers and developers to seamlessly implement and experiment with these advanced machine learning techniques.
 
+You can directly install our library by running:
+```commandline
+pip install Probability-Surrogate-Learning==0.1
+```
+
 ---
 ## Active Learning Techniques
 ### [Deep Multi-fidelity Active Learning (DMFAL)](https://arxiv.org/abs/2012.00901)
 
 To run the code:
 ```commandline
 cd Active-Learning/Deep-Multi-fidelity-Active-Learning
```

### Comparing `Probability-Surrogate-Learning-0.1/Probability_Surrogate_Learning.egg-info/PKG-INFO` & `Probability-Surrogate-Learning-1.0/Probability_Surrogate_Learning.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 Metadata-Version: 2.1
 Name: Probability-Surrogate-Learning
-Version: 0.1
+Version: 1.0
 Summary: This is a comprehensive machine learning library, specifically tailored for surrogate learning and active learning.
 Home-page: https://github.com/liwenlin664477/Probability-Surrogate-Learning
 Author: Wenlin Li
 Author-email: u1327012@example.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Probability-Surrogate-Learning
 This is a comprehensive machine learning library, specifically tailored for surrogate learning and active learning. Our objective is to provide a robust platform that empowers researchers and developers to seamlessly implement and experiment with these advanced machine learning techniques.
 
+You can directly install our library by running:
+```commandline
+pip install Probability-Surrogate-Learning==0.1
+```
+
 ---
 ## Active Learning Techniques
 ### [Deep Multi-fidelity Active Learning (DMFAL)](https://arxiv.org/abs/2012.00901)
 
 To run the code:
 ```commandline
 cd Active-Learning/Deep-Multi-fidelity-Active-Learning
```

### Comparing `Probability-Surrogate-Learning-0.1/Probability_Surrogate_Learning.egg-info/SOURCES.txt` & `Probability-Surrogate-Learning-1.0/Probability_Surrogate_Learning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Probability-Surrogate-Learning-0.1/README.md` & `Probability-Surrogate-Learning-1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 # Probability-Surrogate-Learning
 This is a comprehensive machine learning library, specifically tailored for surrogate learning and active learning. Our objective is to provide a robust platform that empowers researchers and developers to seamlessly implement and experiment with these advanced machine learning techniques.
 
+You can directly install our library by running:
+```commandline
+pip install Probability-Surrogate-Learning==0.1
+```
+
 ---
 ## Active Learning Techniques
 ### [Deep Multi-fidelity Active Learning (DMFAL)](https://arxiv.org/abs/2012.00901)
 
 To run the code:
 ```commandline
 cd Active-Learning/Deep-Multi-fidelity-Active-Learning
```

### Comparing `Probability-Surrogate-Learning-0.1/setup.py` & `Probability-Surrogate-Learning-1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Probability-Surrogate-Learning",
-    version="0.1",
+    version="1.0",
     packages=find_packages(),
     author="Wenlin Li",
     author_email="u1327012@example.com",
     description="This is a comprehensive machine learning library, "
                 "specifically tailored for surrogate learning and active learning.",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
```

