# Comparing `tmp/eef-data-0.50.tar.gz` & `tmp/eef-data-0.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eef-data-0.50.tar", last modified: Tue Jul 18 23:42:10 2023, max compression
+gzip compressed data, was "eef-data-0.51.tar", last modified: Wed Jul 19 00:03:25 2023, max compression
```

## Comparing `eef-data-0.50.tar` & `eef-data-0.51.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-18 23:42:10.863881 eef-data-0.50/
--rw-rw-r--   0 linux     (1000) linux     (1000)     1073 2023-05-04 23:15:45.000000 eef-data-0.50/LICENSE
--rw-rw-r--   0 linux     (1000) linux     (1000)    62814 2023-07-18 23:42:10.863881 eef-data-0.50/PKG-INFO
--rw-rw-r--   0 linux     (1000) linux     (1000)    64622 2023-07-18 23:21:55.000000 eef-data-0.50/README.md
-drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-18 23:42:10.863881 eef-data-0.50/eef_data.egg-info/
--rw-rw-r--   0 linux     (1000) linux     (1000)    62814 2023-07-18 23:42:10.000000 eef-data-0.50/eef_data.egg-info/PKG-INFO
--rw-rw-r--   0 linux     (1000) linux     (1000)      328 2023-07-18 23:42:10.000000 eef-data-0.50/eef_data.egg-info/SOURCES.txt
--rw-rw-r--   0 linux     (1000) linux     (1000)        1 2023-07-18 23:42:10.000000 eef-data-0.50/eef_data.egg-info/dependency_links.txt
--rw-rw-r--   0 linux     (1000) linux     (1000)       47 2023-07-18 23:42:10.000000 eef-data-0.50/eef_data.egg-info/entry_points.txt
--rw-rw-r--   0 linux     (1000) linux     (1000)       78 2023-07-18 23:42:10.000000 eef-data-0.50/eef_data.egg-info/requires.txt
--rw-rw-r--   0 linux     (1000) linux     (1000)        8 2023-07-18 23:42:10.000000 eef-data-0.50/eef_data.egg-info/top_level.txt
-drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-18 23:42:10.863881 eef-data-0.50/eefdata/
--rw-rw-r--   0 linux     (1000) linux     (1000)        0 2023-03-17 12:41:41.000000 eef-data-0.50/eefdata/__init__.py
--rw-rw-r--   0 linux     (1000) linux     (1000)   165254 2023-07-18 23:16:25.000000 eef-data-0.50/eefdata/app.py
-drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-18 23:42:10.863881 eef-data-0.50/eefdata/src/
--rw-rw-r--   0 linux     (1000) linux     (1000)        0 2023-03-17 12:41:42.000000 eef-data-0.50/eefdata/src/__init__.py
--rw-rw-r--   0 linux     (1000) linux     (1000)   151479 2023-07-18 18:50:53.000000 eef-data-0.50/eefdata/src/attributeIDs.py
--rw-rw-r--   0 linux     (1000) linux     (1000)   263004 2023-07-18 23:21:18.000000 eef-data-0.50/eefdata/src/funcs.py
--rw-rw-r--   0 linux     (1000) linux     (1000)       38 2023-07-18 23:42:10.863881 eef-data-0.50/setup.cfg
--rw-rw-r--   0 linux     (1000) linux     (1000)      693 2023-07-18 23:40:53.000000 eef-data-0.50/setup.py
+drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-19 00:03:25.972187 eef-data-0.51/
+-rw-rw-r--   0 linux     (1000) linux     (1000)     1073 2023-05-04 23:15:45.000000 eef-data-0.51/LICENSE
+-rw-rw-r--   0 linux     (1000) linux     (1000)       25 2023-07-19 00:02:37.000000 eef-data-0.51/MANIFEST.in
+-rw-rw-r--   0 linux     (1000) linux     (1000)    62840 2023-07-19 00:03:25.972187 eef-data-0.51/PKG-INFO
+-rw-rw-r--   0 linux     (1000) linux     (1000)    64622 2023-07-18 23:21:55.000000 eef-data-0.51/README.md
+-rwxrwxrwx   0 linux     (1000) linux     (1000)    62627 2023-07-18 23:33:52.000000 eef-data-0.51/README_package.md
+drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-19 00:03:25.972187 eef-data-0.51/eef_data.egg-info/
+-rw-rw-r--   0 linux     (1000) linux     (1000)    62840 2023-07-19 00:03:25.000000 eef-data-0.51/eef_data.egg-info/PKG-INFO
+-rw-rw-r--   0 linux     (1000) linux     (1000)      358 2023-07-19 00:03:25.000000 eef-data-0.51/eef_data.egg-info/SOURCES.txt
+-rw-rw-r--   0 linux     (1000) linux     (1000)        1 2023-07-19 00:03:25.000000 eef-data-0.51/eef_data.egg-info/dependency_links.txt
+-rw-rw-r--   0 linux     (1000) linux     (1000)       47 2023-07-19 00:03:25.000000 eef-data-0.51/eef_data.egg-info/entry_points.txt
+-rw-rw-r--   0 linux     (1000) linux     (1000)       78 2023-07-19 00:03:25.000000 eef-data-0.51/eef_data.egg-info/requires.txt
+-rw-rw-r--   0 linux     (1000) linux     (1000)        8 2023-07-19 00:03:25.000000 eef-data-0.51/eef_data.egg-info/top_level.txt
+drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-19 00:03:25.972187 eef-data-0.51/eefdata/
+-rw-rw-r--   0 linux     (1000) linux     (1000)        0 2023-03-17 12:41:41.000000 eef-data-0.51/eefdata/__init__.py
+-rw-rw-r--   0 linux     (1000) linux     (1000)   165254 2023-07-18 23:16:25.000000 eef-data-0.51/eefdata/app.py
+drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-19 00:03:25.972187 eef-data-0.51/eefdata/src/
+-rw-rw-r--   0 linux     (1000) linux     (1000)        0 2023-03-17 12:41:42.000000 eef-data-0.51/eefdata/src/__init__.py
+-rw-rw-r--   0 linux     (1000) linux     (1000)   151479 2023-07-18 18:50:53.000000 eef-data-0.51/eefdata/src/attributeIDs.py
+-rw-rw-r--   0 linux     (1000) linux     (1000)   263004 2023-07-18 23:21:18.000000 eef-data-0.51/eefdata/src/funcs.py
+-rw-rw-r--   0 linux     (1000) linux     (1000)       38 2023-07-19 00:03:25.972187 eef-data-0.51/setup.cfg
+-rw-rw-r--   0 linux     (1000) linux     (1000)      771 2023-07-19 00:03:24.000000 eef-data-0.51/setup.py
```

### Comparing `eef-data-0.50/LICENSE` & `eef-data-0.51/LICENSE`

 * *Files identical despite different names*

### Comparing `eef-data-0.50/PKG-INFO` & `eef-data-0.51/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: eef-data
-Version: 0.50
+Version: 0.51
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
+Requires-Python: >=3.10.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 [<img alt="" src="https://img.shields.io/pypi/v/eef-data?label=PyPI%20Package" />](https://pypi.org/project/eef-data/)
 
 <h1 align="center">
```

### Comparing `eef-data-0.50/README.md` & `eef-data-0.51/README.md`

 * *Files identical despite different names*

### Comparing `eef-data-0.50/eef_data.egg-info/PKG-INFO` & `eef-data-0.51/README_package.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: eef-data
-Version: 0.50
-Summary: UNKNOWN
-Home-page: UNKNOWN
-License: UNKNOWN
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 
 [<img alt="" src="https://img.shields.io/pypi/v/eef-data?label=PyPI%20Package" />](https://pypi.org/project/eef-data/)
 
 <h1 align="center">
 
 EEF Datafile Extractor
 
@@ -887,9 +877,8 @@
 | `Intervention Setting`                      | `raw`  | `int_setting_raw`    |
 | `Intervention Setting (ht)`                 | `ht`   | `int_setting_ht`     |
 | `Intervention Setting (info)`               | `info` | `int_setting_info`   |
 </details>
 
 ## License
 
-Distributed under the MIT License. See LICENSE for more information.
-
+Distributed under the MIT License. See LICENSE for more information.
```

### Comparing `eef-data-0.50/eefdata/app.py` & `eef-data-0.51/eefdata/app.py`

 * *Files identical despite different names*

### Comparing `eef-data-0.50/eefdata/src/attributeIDs.py` & `eef-data-0.51/eefdata/src/attributeIDs.py`

 * *Files identical despite different names*

### Comparing `eef-data-0.50/eefdata/src/funcs.py` & `eef-data-0.51/eefdata/src/funcs.py`

 * *Files identical despite different names*

### Comparing `eef-data-0.50/setup.py` & `eef-data-0.51/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 
 # Read the contents of your README file
 with open('README_package.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='eef-data',
-    version='0.50',  # Remember to increment the version number
+    version='0.51',  # Remember to increment the version number
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'numpy==1.22.0',
         'pandas==1.5.0',
         'prompt_toolkit==3.0.30',
         'rich==12.4.4',
         'toolz==0.11.2'
     ],
+    python_requires='>=3.10.6',
     long_description=long_description,
+    package_data={'': ['README_package.md']},
     long_description_content_type='text/markdown',
     entry_points={
         'console_scripts': [
             'eef-data=eefdata.app:main',
         ],
     },
 )
```

