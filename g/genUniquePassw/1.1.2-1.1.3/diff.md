# Comparing `tmp/genUniquePassw-1.1.2.tar.gz` & `tmp/genUniquePassw-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genUniquePassw-1.1.2.tar", last modified: Wed Jul 19 03:13:14 2023, max compression
+gzip compressed data, was "genUniquePassw-1.1.3.tar", last modified: Wed Jul 19 03:36:03 2023, max compression
```

## Comparing `genUniquePassw-1.1.2.tar` & `genUniquePassw-1.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-19 03:13:14.271932 genUniquePassw-1.1.2/
--rw-rw-r--   0 user      (1000) user      (1000)      733 2023-07-19 03:13:14.271932 genUniquePassw-1.1.2/PKG-INFO
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-19 03:13:14.271932 genUniquePassw-1.1.2/genUniquePassw.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)      733 2023-07-19 03:13:14.000000 genUniquePassw-1.1.2/genUniquePassw.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      209 2023-07-19 03:13:14.000000 genUniquePassw-1.1.2/genUniquePassw.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-19 03:13:14.000000 genUniquePassw-1.1.2/genUniquePassw.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        8 2023-07-19 03:13:14.000000 genUniquePassw-1.1.2/genUniquePassw.egg-info/top_level.txt
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-19 03:13:14.271932 genUniquePassw-1.1.2/package/
--rw-rw-r--   0 user      (1000) user      (1000)       69 2023-07-19 03:12:18.000000 genUniquePassw-1.1.2/package/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1280 2023-07-18 10:39:31.000000 genUniquePassw-1.1.2/package/generate_password.py
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-19 03:13:14.271932 genUniquePassw-1.1.2/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1525 2023-07-19 03:13:05.000000 genUniquePassw-1.1.2/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-19 03:36:03.270137 genUniquePassw-1.1.3/
+-rw-rw-r--   0 user      (1000) user      (1000)      733 2023-07-19 03:36:03.270137 genUniquePassw-1.1.3/PKG-INFO
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-19 03:36:03.270137 genUniquePassw-1.1.3/genUniquePassw.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)      733 2023-07-19 03:36:03.000000 genUniquePassw-1.1.3/genUniquePassw.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      209 2023-07-19 03:36:03.000000 genUniquePassw-1.1.3/genUniquePassw.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-19 03:36:03.000000 genUniquePassw-1.1.3/genUniquePassw.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        8 2023-07-19 03:36:03.000000 genUniquePassw-1.1.3/genUniquePassw.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-19 03:36:03.270137 genUniquePassw-1.1.3/package/
+-rw-rw-r--   0 user      (1000) user      (1000)       17 2023-07-19 03:35:35.000000 genUniquePassw-1.1.3/package/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      916 2023-07-19 03:31:40.000000 genUniquePassw-1.1.3/package/generate_password.py
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-19 03:36:03.270137 genUniquePassw-1.1.3/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1525 2023-07-19 03:35:54.000000 genUniquePassw-1.1.3/setup.py
```

### Comparing `genUniquePassw-1.1.2/PKG-INFO` & `genUniquePassw-1.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genUniquePassw
-Version: 1.1.2
+Version: 1.1.3
 Summary: Python package to generate random passwords of maximum length 12, avoiding names present in specified files.
 Home-page: https://github.com/kanchann23/genUniquePassw
 Author: kanchan
 Author-email: kanchanbora321@gmail.com
 License: MIT
 Keywords: security,password
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `genUniquePassw-1.1.2/genUniquePassw.egg-info/PKG-INFO` & `genUniquePassw-1.1.3/genUniquePassw.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genUniquePassw
-Version: 1.1.2
+Version: 1.1.3
 Summary: Python package to generate random passwords of maximum length 12, avoiding names present in specified files.
 Home-page: https://github.com/kanchann23/genUniquePassw
 Author: kanchan
 Author-email: kanchanbora321@gmail.com
 License: MIT
 Keywords: security,password
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `genUniquePassw-1.1.2/setup.py` & `genUniquePassw-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='genUniquePassw',       # Replace with the name of your package
-    version='1.1.2',                # Replace with the version number of your package
+    version='1.1.3',                # Replace with the version number of your package
     author='kanchan',             # Replace with the author's name
     author_email='kanchanbora321@gmail.com',  # Replace with the author's email
     description='Python package to generate random passwords of maximum length 12, avoiding names present in specified files.',
     long_description='generate password',  # Use README.md content or plain text
     long_description_content_type='text/plain',  # Specify the type of long description (text/plain, text/markdown, etc.)
     url='https://github.com/kanchann23/genUniquePassw',  # Replace with the URL of your package's repository
     license='MIT',                  # Replace with the license type of your package
```

