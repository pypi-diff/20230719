# Comparing `tmp/VDBpy-0.1.3.tar.gz` & `tmp/VDBpy-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VDBpy-0.1.3.tar", last modified: Wed Jul 19 09:41:57 2023, max compression
+gzip compressed data, was "VDBpy-0.1.4.tar", last modified: Wed Jul 19 09:58:11 2023, max compression
```

## Comparing `VDBpy-0.1.3.tar` & `VDBpy-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 09:41:57.027624 VDBpy-0.1.3/
--rw-rw-rw-   0        0        0      605 2023-07-19 09:41:57.027624 VDBpy-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      115 2023-07-18 16:04:07.000000 VDBpy-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-19 09:41:57.003852 VDBpy-0.1.3/VDBpy/
--rw-rw-rw-   0        0        0        0 2023-07-18 15:19:32.000000 VDBpy-0.1.3/VDBpy/__init__.py
--rw-rw-rw-   0        0        0     1323 2023-07-19 09:40:17.000000 VDBpy-0.1.3/VDBpy/indexing.py
--rw-rw-rw-   0        0        0      179 2023-07-19 09:41:06.000000 VDBpy-0.1.3/VDBpy/query.py
--rw-rw-rw-   0        0        0     1108 2023-07-19 09:41:03.000000 VDBpy-0.1.3/VDBpy/similarity.py
-drwxrwxrwx   0        0        0        0 2023-07-19 09:41:57.023888 VDBpy-0.1.3/VDBpy.egg-info/
--rw-rw-rw-   0        0        0      605 2023-07-19 09:41:56.000000 VDBpy-0.1.3/VDBpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2023-07-19 09:41:56.000000 VDBpy-0.1.3/VDBpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 09:41:56.000000 VDBpy-0.1.3/VDBpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-19 09:41:56.000000 VDBpy-0.1.3/VDBpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-19 09:41:57.032076 VDBpy-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      675 2023-07-19 09:41:33.000000 VDBpy-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 09:58:11.894189 VDBpy-0.1.4/
+-rw-rw-rw-   0        0        0     1513 2023-07-19 09:58:11.894189 VDBpy-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      982 2023-07-19 09:56:16.000000 VDBpy-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-19 09:58:11.852361 VDBpy-0.1.4/VDBpy/
+-rw-rw-rw-   0        0        0        0 2023-07-18 15:19:32.000000 VDBpy-0.1.4/VDBpy/__init__.py
+-rw-rw-rw-   0        0        0     1323 2023-07-19 09:40:17.000000 VDBpy-0.1.4/VDBpy/indexing.py
+-rw-rw-rw-   0        0        0      179 2023-07-19 09:41:06.000000 VDBpy-0.1.4/VDBpy/query.py
+-rw-rw-rw-   0        0        0     1108 2023-07-19 09:41:03.000000 VDBpy-0.1.4/VDBpy/similarity.py
+drwxrwxrwx   0        0        0        0 2023-07-19 09:58:11.894189 VDBpy-0.1.4/VDBpy.egg-info/
+-rw-rw-rw-   0        0        0     1513 2023-07-19 09:58:11.000000 VDBpy-0.1.4/VDBpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      205 2023-07-19 09:58:11.000000 VDBpy-0.1.4/VDBpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 09:58:11.000000 VDBpy-0.1.4/VDBpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-19 09:58:11.000000 VDBpy-0.1.4/VDBpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-19 09:58:11.894189 VDBpy-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      675 2023-07-19 09:57:53.000000 VDBpy-0.1.4/setup.py
```

### Comparing `VDBpy-0.1.3/VDBpy/indexing.py` & `VDBpy-0.1.4/VDBpy/indexing.py`

 * *Files identical despite different names*

### Comparing `VDBpy-0.1.3/VDBpy/similarity.py` & `VDBpy-0.1.4/VDBpy/similarity.py`

 * *Files identical despite different names*

### Comparing `VDBpy-0.1.3/setup.py` & `VDBpy-0.1.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='VDBpy',
-    version='0.1.3',
+    version='0.1.4',
     packages=find_packages(),
     description='A simple vector database allows difference search methods (consine similarity and euclidean distance ect.)',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Justin He',
     author_email='justin.he814@gmail.com',
     url='https://github.com/Ateee329/VDBpy',
```

