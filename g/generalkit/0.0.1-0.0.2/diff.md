# Comparing `tmp/generalkit-0.0.1.tar.gz` & `tmp/generalkit-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generalkit-0.0.1.tar", last modified: Mon Jul 17 08:44:56 2023, max compression
+gzip compressed data, was "generalkit-0.0.2.tar", last modified: Wed Jul 19 07:58:04 2023, max compression
```

## Comparing `generalkit-0.0.1.tar` & `generalkit-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 08:44:56.014795 generalkit-0.0.1/
--rw-rw-rw-   0        0        0      430 2023-07-17 08:44:56.014795 generalkit-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-17 08:02:28.000000 generalkit-0.0.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-17 08:44:56.010103 generalkit-0.0.1/generalkit.egg-info/
--rw-rw-rw-   0        0        0      430 2023-07-17 08:44:55.000000 generalkit-0.0.1/generalkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2023-07-17 08:44:55.000000 generalkit-0.0.1/generalkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 08:44:55.000000 generalkit-0.0.1/generalkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-07-17 08:44:55.000000 generalkit-0.0.1/generalkit.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-17 08:44:56.012801 generalkit-0.0.1/kit/
--rw-rw-rw-   0        0        0        0 2023-07-17 07:58:41.000000 generalkit-0.0.1/kit/__init__.py
--rw-rw-rw-   0        0        0     3599 2023-07-13 09:13:43.000000 generalkit-0.0.1/kit/file_utils.py
--rw-rw-rw-   0        0        0     4224 2023-07-13 09:44:55.000000 generalkit-0.0.1/kit/stream.py
--rw-rw-rw-   0        0        0       42 2023-07-17 08:44:56.014795 generalkit-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      957 2023-07-17 08:44:49.000000 generalkit-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 07:58:04.152510 generalkit-0.0.2/
+-rw-rw-rw-   0        0        0      430 2023-07-19 07:58:04.151547 generalkit-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      125 2023-07-17 09:09:33.000000 generalkit-0.0.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-19 07:58:04.145535 generalkit-0.0.2/generalkit.egg-info/
+-rw-rw-rw-   0        0        0      430 2023-07-19 07:58:04.000000 generalkit-0.0.2/generalkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-07-19 07:58:04.000000 generalkit-0.0.2/generalkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 07:58:04.000000 generalkit-0.0.2/generalkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-07-19 07:58:04.000000 generalkit-0.0.2/generalkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-19 07:58:04.000000 generalkit-0.0.2/generalkit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-19 07:58:04.150545 generalkit-0.0.2/kit/
+-rw-rw-rw-   0        0        0        0 2023-07-17 07:58:41.000000 generalkit-0.0.2/kit/__init__.py
+-rw-rw-rw-   0        0        0     3599 2023-07-13 09:13:43.000000 generalkit-0.0.2/kit/file_utils.py
+-rw-rw-rw-   0        0        0     3197 2023-07-19 07:56:39.000000 generalkit-0.0.2/kit/media.py
+-rw-rw-rw-   0        0        0     4224 2023-07-13 09:44:55.000000 generalkit-0.0.2/kit/stream.py
+-rw-rw-rw-   0        0        0       42 2023-07-19 07:58:04.152510 generalkit-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      990 2023-07-19 07:58:00.000000 generalkit-0.0.2/setup.py
```

### Comparing `generalkit-0.0.1/kit/file_utils.py` & `generalkit-0.0.2/kit/file_utils.py`

 * *Files identical despite different names*

### Comparing `generalkit-0.0.1/kit/stream.py` & `generalkit-0.0.2/kit/stream.py`

 * *Files identical despite different names*

### Comparing `generalkit-0.0.1/setup.py` & `generalkit-0.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 # these things are needed for the README.rst show on pypi (if you dont need delete it)
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.rst"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 # you need to change all these
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'easy tool kit'
 
 setup(
     name="generalkit",
     version=VERSION,
     author="wade",
     author_email="wade.xiao.x@gmail.com",
     description=DESCRIPTION,
     packages=find_packages(),
     license='MIT',
     install_requires=[
-
+        'ffmpy','pydub','moviepy'
     ],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

