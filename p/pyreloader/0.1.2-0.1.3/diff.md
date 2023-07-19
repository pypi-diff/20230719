# Comparing `tmp/pyreloader-0.1.2.tar.gz` & `tmp/pyreloader-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyreloader-0.1.2.tar", last modified: Wed Jul 19 07:54:22 2023, max compression
+gzip compressed data, was "pyreloader-0.1.3.tar", last modified: Wed Jul 19 12:43:40 2023, max compression
```

## Comparing `pyreloader-0.1.2.tar` & `pyreloader-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 d067954    (501) staff       (20)        0 2023-07-19 07:54:22.239943 pyreloader-0.1.2/
--rw-r--r--   0 d067954    (501) staff       (20)     1077 2023-07-19 07:05:20.000000 pyreloader-0.1.2/LICENSE.txt
--rw-r--r--   0 d067954    (501) staff       (20)      663 2023-07-19 07:54:22.239653 pyreloader-0.1.2/PKG-INFO
--rw-r--r--   0 d067954    (501) staff       (20)      212 2023-07-19 07:53:23.000000 pyreloader-0.1.2/README.md
--rw-r--r--   0 d067954    (501) staff       (20)       98 2023-07-19 07:38:13.000000 pyreloader-0.1.2/pyproject.toml
-drwxr-xr-x   0 d067954    (501) staff       (20)        0 2023-07-19 07:54:22.238732 pyreloader-0.1.2/pyreloader.egg-info/
--rw-r--r--   0 d067954    (501) staff       (20)      663 2023-07-19 07:54:22.000000 pyreloader-0.1.2/pyreloader.egg-info/PKG-INFO
--rw-r--r--   0 d067954    (501) staff       (20)      218 2023-07-19 07:54:22.000000 pyreloader-0.1.2/pyreloader.egg-info/SOURCES.txt
--rw-r--r--   0 d067954    (501) staff       (20)        1 2023-07-19 07:54:22.000000 pyreloader-0.1.2/pyreloader.egg-info/dependency_links.txt
--rw-r--r--   0 d067954    (501) staff       (20)       47 2023-07-19 07:54:22.000000 pyreloader-0.1.2/pyreloader.egg-info/entry_points.txt
--rw-r--r--   0 d067954    (501) staff       (20)       11 2023-07-19 07:54:22.000000 pyreloader-0.1.2/pyreloader.egg-info/top_level.txt
--rw-r--r--   0 d067954    (501) staff       (20)       38 2023-07-19 07:54:22.239991 pyreloader-0.1.2/setup.cfg
--rw-r--r--   0 d067954    (501) staff       (20)      820 2023-07-19 07:54:01.000000 pyreloader-0.1.2/setup.py
+drwxr-xr-x   0 d067954    (501) staff       (20)        0 2023-07-19 12:43:40.549269 pyreloader-0.1.3/
+-rw-r--r--   0 d067954    (501) staff       (20)     1077 2023-07-19 07:05:20.000000 pyreloader-0.1.3/LICENSE.txt
+-rw-r--r--   0 d067954    (501) staff       (20)      663 2023-07-19 12:43:40.549041 pyreloader-0.1.3/PKG-INFO
+-rw-r--r--   0 d067954    (501) staff       (20)      212 2023-07-19 07:53:23.000000 pyreloader-0.1.3/README.md
+-rw-r--r--   0 d067954    (501) staff       (20)       98 2023-07-19 07:38:13.000000 pyreloader-0.1.3/pyproject.toml
+drwxr-xr-x   0 d067954    (501) staff       (20)        0 2023-07-19 12:43:40.548564 pyreloader-0.1.3/pyreloader.egg-info/
+-rw-r--r--   0 d067954    (501) staff       (20)      663 2023-07-19 12:43:40.000000 pyreloader-0.1.3/pyreloader.egg-info/PKG-INFO
+-rw-r--r--   0 d067954    (501) staff       (20)      232 2023-07-19 12:43:40.000000 pyreloader-0.1.3/pyreloader.egg-info/SOURCES.txt
+-rw-r--r--   0 d067954    (501) staff       (20)        1 2023-07-19 12:43:40.000000 pyreloader-0.1.3/pyreloader.egg-info/dependency_links.txt
+-rw-r--r--   0 d067954    (501) staff       (20)       47 2023-07-19 12:43:40.000000 pyreloader-0.1.3/pyreloader.egg-info/entry_points.txt
+-rw-r--r--   0 d067954    (501) staff       (20)       11 2023-07-19 12:43:40.000000 pyreloader-0.1.3/pyreloader.egg-info/top_level.txt
+-rw-r--r--   0 d067954    (501) staff       (20)     1345 2023-07-19 06:50:14.000000 pyreloader-0.1.3/pyreloader.py
+-rw-r--r--   0 d067954    (501) staff       (20)       38 2023-07-19 12:43:40.549308 pyreloader-0.1.3/setup.cfg
+-rw-r--r--   0 d067954    (501) staff       (20)      820 2023-07-19 12:43:10.000000 pyreloader-0.1.3/setup.py
```

### Comparing `pyreloader-0.1.2/LICENSE.txt` & `pyreloader-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyreloader-0.1.2/PKG-INFO` & `pyreloader-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreloader
-Version: 0.1.2
+Version: 0.1.3
 Summary: Reload a python program on kill signal.
 Home-page: https://github.com/chuan137/pyreloader
 Author: Chuan Miao
 Author-email: chuan137@gmail.com
 License: MIT
 Keywords: reload server
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyreloader-0.1.2/pyreloader.egg-info/PKG-INFO` & `pyreloader-0.1.3/pyreloader.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreloader
-Version: 0.1.2
+Version: 0.1.3
 Summary: Reload a python program on kill signal.
 Home-page: https://github.com/chuan137/pyreloader
 Author: Chuan Miao
 Author-email: chuan137@gmail.com
 License: MIT
 Keywords: reload server
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyreloader-0.1.2/setup.py` & `pyreloader-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name = "pyreloader",
-    version = "0.1.2",
+    version = "0.1.3",
     author = "Chuan Miao",
     author_email = "chuan137@gmail.com",
     description = ("Reload a python program on kill signal."),
     license = "MIT",
     keywords = "reload server",
     url = "https://github.com/chuan137/pyreloader",
     py_modules=['pyreloader'],
```

