# Comparing `tmp/ifsFractals-1.0.3.tar.gz` & `tmp/ifsFractals-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ifsFractals-1.0.3.tar", last modified: Sun Apr 11 07:21:24 2021, max compression
+gzip compressed data, was "ifsFractals-1.0.4.tar", last modified: Wed Jul 19 11:53:04 2023, max compression
```

## Comparing `ifsFractals-1.0.3.tar` & `ifsFractals-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 peterfrancis   (501) staff       (20)        0 2021-04-11 07:21:24.000000 ifsFractals-1.0.3/
--rw-r--r--   0 peterfrancis   (501) staff       (20)     1070 2019-09-07 01:05:57.000000 ifsFractals-1.0.3/LICENSE
--rw-r--r--   0 peterfrancis   (501) staff       (20)      601 2021-04-11 07:21:24.000000 ifsFractals-1.0.3/PKG-INFO
--rw-r--r--   0 peterfrancis   (501) staff       (20)     1025 2019-12-03 04:58:04.000000 ifsFractals-1.0.3/README.md
-drwxr-xr-x   0 peterfrancis   (501) staff       (20)        0 2021-04-11 07:21:24.000000 ifsFractals-1.0.3/ifsFractals/
--rw-r--r--   0 peterfrancis   (501) staff       (20)     9117 2021-04-11 06:44:59.000000 ifsFractals-1.0.3/ifsFractals/__init__.py
-drwxr-xr-x   0 peterfrancis   (501) staff       (20)        0 2021-04-11 07:21:24.000000 ifsFractals-1.0.3/ifsFractals.egg-info/
--rw-r--r--   0 peterfrancis   (501) staff       (20)      601 2021-04-11 07:21:24.000000 ifsFractals-1.0.3/ifsFractals.egg-info/PKG-INFO
--rw-r--r--   0 peterfrancis   (501) staff       (20)      234 2021-04-11 07:21:24.000000 ifsFractals-1.0.3/ifsFractals.egg-info/SOURCES.txt
--rw-r--r--   0 peterfrancis   (501) staff       (20)        1 2021-04-11 07:21:24.000000 ifsFractals-1.0.3/ifsFractals.egg-info/dependency_links.txt
--rw-r--r--   0 peterfrancis   (501) staff       (20)       40 2021-04-11 07:21:24.000000 ifsFractals-1.0.3/ifsFractals.egg-info/requires.txt
--rw-r--r--   0 peterfrancis   (501) staff       (20)       12 2021-04-11 07:21:24.000000 ifsFractals-1.0.3/ifsFractals.egg-info/top_level.txt
--rw-r--r--   0 peterfrancis   (501) staff       (20)       74 2021-04-11 07:21:24.000000 ifsFractals-1.0.3/setup.cfg
--rw-r--r--   0 peterfrancis   (501) staff       (20)      800 2021-04-11 07:21:02.000000 ifsFractals-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:53:04.455982 ifsFractals-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-19 11:52:51.000000 ifsFractals-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-19 11:53:04.455982 ifsFractals-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-19 11:52:51.000000 ifsFractals-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:53:04.455982 ifsFractals-1.0.4/ifsFractals/
+-rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-07-19 11:52:51.000000 ifsFractals-1.0.4/ifsFractals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:53:04.455982 ifsFractals-1.0.4/ifsFractals.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-19 11:53:04.000000 ifsFractals-1.0.4/ifsFractals.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-19 11:53:04.000000 ifsFractals-1.0.4/ifsFractals.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 11:53:04.000000 ifsFractals-1.0.4/ifsFractals.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-19 11:53:04.000000 ifsFractals-1.0.4/ifsFractals.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-19 11:53:04.000000 ifsFractals-1.0.4/ifsFractals.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-19 11:53:04.455982 ifsFractals-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-19 11:52:51.000000 ifsFractals-1.0.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ifsFractals-1.0.3/LICENSE` & `ifsFractals-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ifsFractals-1.0.3/ifsFractals/__init__.py` & `ifsFractals-1.0.4/ifsFractals/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,29 +19,29 @@
 
 from IPython.core.display import display, HTML
 from IPython.display import IFrame
 
 
 
 ## Built-In Transformations
-def Scale(s):
+def Scale(s:float):
     return np.array([[s, 0, 0],[0, s, 0],[0, 0, 1]], dtype=np.float64)
-def Translate(a, b):
+def Translate(a:float, b:float):
     return np.array([[1, 0, a],[0, 1, b],[0, 0, 1]], dtype=np.float64)
-def Rotate(theta):
+def Rotate(theta:float):
     return np.array([[np.cos(theta), -np.sin(theta), 0],[np.sin(theta), np.cos(theta), 0],[0, 0, 1]], dtype=np.float64)
-def ShearX(t):
+def ShearX(t:float):
     return np.array([[1, t, 0],[0,1, 0],[0, 0, 1]], dtype=np.float64)
-def ShearY(t):
+def ShearY(t:float):
     return np.array([[1, 0, 0],[t,1, 0],[0, 0, 1]], dtype=np.float64)
-def ScaleX(s):
+def ScaleX(s:float):
     return np.array([[s, 0, 0],[0, 1, 0],[0, 0, 1]], dtype=np.float64)
-def ScaleY(s):
+def ScaleY(s:float):
     return np.array([[1, 0, 0],[0, s, 0],[0, 0, 1]], dtype=np.float64)
-def ScaleXY(s, t):
+def ScaleXY(s:float, t:float):
     return np.array([[s, 0, 0],[0,t, 0],[0, 0, 1]], dtype=np.float64)
 
 
 
 
 
 
@@ -255,19 +255,22 @@
 
     def display(self):
         # https://stackoverflow.com/a/26649884
         plt.imshow(np.asarray(self.pic))
 
     def export(self):
         for T in self.transformations:
-            print(T.tolist())
+            return {
+                'transformations': T.tolist(),
+                'weights': T.weights
+            }
 
     def link(self):
         matrices = [(np.round(T * 1000) / 1000).tolist() for T in self.transformations]
-        link = 'https://ifs-fractals.herokuapp.com/playground/t='
+        link = 'https://ifs-fractals.peterefrancis.com/playground/t='
         for m in matrices:
             link += f'M({m[0][0]},{m[0][1]},{m[1][0]},{m[1][1]},{m[0][2]},{m[1][2]})&'
         return link[:-1] + "/w=" + ",".join([str(el) for el in self.weights])
 
     def link_web(self):
         display(HTML("<a href='" + self.link() + "' target='_blank '>Click me to open in IFS Fractals</a>"))
```

### Comparing `ifsFractals-1.0.3/setup.py` & `ifsFractals-1.0.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup
 from os import path
 
 setup(
     name="ifsFractals",
     packages=["ifsFractals"],
-    version="1.0.3",
+    version="1.0.4",
     author="Peter Francis",
-    author_email="franpe02@gettysburg.edu",
-    description="For Generating Fast IFS Fractals",
+    author_email="peter.e.francis@stonybrook.edu",
+    description="For Fast Generation of IFS Fractals",
     long_description="""
     # ifsFractals
 
     A python module for fast Iterated Function System Fractal generation
 
     See the [GitHub Repo](https://github.com/PeterEFrancis/ifsFractals-py) for more information.
     """,
```

