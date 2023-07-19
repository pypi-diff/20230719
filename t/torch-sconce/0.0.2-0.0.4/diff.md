# Comparing `tmp/torch-sconce-0.0.2.tar.gz` & `tmp/torch-sconce-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch-sconce-0.0.2.tar", last modified: Wed Jul 19 05:12:08 2023, max compression
+gzip compressed data, was "torch-sconce-0.0.4.tar", last modified: Wed Jul 19 05:16:26 2023, max compression
```

## Comparing `torch-sconce-0.0.2.tar` & `torch-sconce-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 sathya    (1000) sathya    (1000)        0 2023-07-19 05:12:08.086715 torch-sconce-0.0.2/
--rw-rw-r--   0 sathya    (1000) sathya    (1000)     1068 2023-07-18 04:39:01.000000 torch-sconce-0.0.2/LICENSE.txt
--rw-rw-r--   0 sathya    (1000) sathya    (1000)     4339 2023-07-19 05:12:08.086715 torch-sconce-0.0.2/PKG-INFO
--rw-rw-r--   0 sathya    (1000) sathya    (1000)     3924 2023-07-19 04:38:17.000000 torch-sconce-0.0.2/README.md
--rw-rw-r--   0 sathya    (1000) sathya    (1000)       79 2023-07-19 05:12:08.086715 torch-sconce-0.0.2/setup.cfg
--rw-rw-r--   0 sathya    (1000) sathya    (1000)     1052 2023-07-19 05:12:05.000000 torch-sconce-0.0.2/setup.py
-drwxrwxr-x   0 sathya    (1000) sathya    (1000)        0 2023-07-19 05:12:08.086715 torch-sconce-0.0.2/torch-sconce/
--rw-rw-r--   0 sathya    (1000) sathya    (1000)       48 2023-07-19 04:12:17.000000 torch-sconce-0.0.2/torch-sconce/__init__.py
--rw-rw-r--   0 sathya    (1000) sathya    (1000)     5927 2023-07-19 03:01:54.000000 torch-sconce-0.0.2/torch-sconce/sconce.py
-drwxrwxr-x   0 sathya    (1000) sathya    (1000)        0 2023-07-19 05:12:08.086715 torch-sconce-0.0.2/torch_sconce.egg-info/
--rw-rw-r--   0 sathya    (1000) sathya    (1000)     4339 2023-07-19 05:12:08.000000 torch-sconce-0.0.2/torch_sconce.egg-info/PKG-INFO
--rw-rw-r--   0 sathya    (1000) sathya    (1000)      232 2023-07-19 05:12:08.000000 torch-sconce-0.0.2/torch_sconce.egg-info/SOURCES.txt
--rw-rw-r--   0 sathya    (1000) sathya    (1000)        1 2023-07-19 05:12:08.000000 torch-sconce-0.0.2/torch_sconce.egg-info/dependency_links.txt
--rw-rw-r--   0 sathya    (1000) sathya    (1000)       13 2023-07-19 05:12:08.000000 torch-sconce-0.0.2/torch_sconce.egg-info/top_level.txt
+drwxrwxr-x   0 sathya    (1000) sathya    (1000)        0 2023-07-19 05:16:26.112980 torch-sconce-0.0.4/
+-rw-rw-r--   0 sathya    (1000) sathya    (1000)     1068 2023-07-18 04:39:01.000000 torch-sconce-0.0.4/LICENSE.txt
+-rw-rw-r--   0 sathya    (1000) sathya    (1000)     4352 2023-07-19 05:16:26.112980 torch-sconce-0.0.4/PKG-INFO
+-rw-rw-r--   0 sathya    (1000) sathya    (1000)     3924 2023-07-19 04:38:17.000000 torch-sconce-0.0.4/README.md
+-rw-rw-r--   0 sathya    (1000) sathya    (1000)       79 2023-07-19 05:16:26.112980 torch-sconce-0.0.4/setup.cfg
+-rw-rw-r--   0 sathya    (1000) sathya    (1000)     1065 2023-07-19 05:15:19.000000 torch-sconce-0.0.4/setup.py
+drwxrwxr-x   0 sathya    (1000) sathya    (1000)        0 2023-07-19 05:16:26.112980 torch-sconce-0.0.4/torch-sconce/
+-rw-rw-r--   0 sathya    (1000) sathya    (1000)       48 2023-07-19 04:12:17.000000 torch-sconce-0.0.4/torch-sconce/__init__.py
+-rw-rw-r--   0 sathya    (1000) sathya    (1000)     5927 2023-07-19 03:01:54.000000 torch-sconce-0.0.4/torch-sconce/sconce.py
+drwxrwxr-x   0 sathya    (1000) sathya    (1000)        0 2023-07-19 05:16:26.112980 torch-sconce-0.0.4/torch_sconce.egg-info/
+-rw-rw-r--   0 sathya    (1000) sathya    (1000)     4352 2023-07-19 05:16:26.000000 torch-sconce-0.0.4/torch_sconce.egg-info/PKG-INFO
+-rw-rw-r--   0 sathya    (1000) sathya    (1000)      232 2023-07-19 05:16:26.000000 torch-sconce-0.0.4/torch_sconce.egg-info/SOURCES.txt
+-rw-rw-r--   0 sathya    (1000) sathya    (1000)        1 2023-07-19 05:16:26.000000 torch-sconce-0.0.4/torch_sconce.egg-info/dependency_links.txt
+-rw-rw-r--   0 sathya    (1000) sathya    (1000)       13 2023-07-19 05:16:26.000000 torch-sconce-0.0.4/torch_sconce.egg-info/top_level.txt
```

### Comparing `torch-sconce-0.0.2/LICENSE.txt` & `torch-sconce-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `torch-sconce-0.0.2/PKG-INFO` & `torch-sconce-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: torch-sconce
-Version: 0.0.2
-Summary: sconce: torch helper
+Version: 0.0.4
+Summary: torch-sconce: torch helper
 Home-page: https://github.com/satabios/sconce
-Download-URL: https://pypi.org/project/sonce/
+Download-URL: https://pypi.org/project/torch-sconce/
 Author: Sathyaprakash Narayanan
 Author-email: snaray17@ucsc.edu
 License: MIT
 Keywords: Development Pipeline,Deployment Pipeline,Torch,Pruning,Compression,Model Pruning
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `torch-sconce-0.0.2/README.md` & `torch-sconce-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `torch-sconce-0.0.2/setup.py` & `torch-sconce-0.0.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 
 setup_args = dict(
     name='torch-sconce',
-    version='0.0.2',
-    description='sconce: torch helper',
+    version='0.0.4',
+    description='torch-sconce: torch helper',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n',
     license='MIT',
     packages=find_packages(),
     author='Sathyaprakash Narayanan',
     author_email='snaray17@ucsc.edu',
     keywords=['Development Pipeline','Deployment Pipeline','Torch','Pruning', 'Compression', 'Model Pruning'],
     url='https://github.com/satabios/sconce',
-    download_url='https://pypi.org/project/sonce/'
+    download_url='https://pypi.org/project/torch-sconce/'
 )
 
 if __name__ == '__main__':
     lib_folder = os.path.dirname(os.path.realpath(__file__))
     requirement_path = lib_folder + './requirements.txt'
     install_requires = []
```

### Comparing `torch-sconce-0.0.2/torch-sconce/sconce.py` & `torch-sconce-0.0.4/torch-sconce/sconce.py`

 * *Files identical despite different names*

### Comparing `torch-sconce-0.0.2/torch_sconce.egg-info/PKG-INFO` & `torch-sconce-0.0.4/torch_sconce.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: torch-sconce
-Version: 0.0.2
-Summary: sconce: torch helper
+Version: 0.0.4
+Summary: torch-sconce: torch helper
 Home-page: https://github.com/satabios/sconce
-Download-URL: https://pypi.org/project/sonce/
+Download-URL: https://pypi.org/project/torch-sconce/
 Author: Sathyaprakash Narayanan
 Author-email: snaray17@ucsc.edu
 License: MIT
 Keywords: Development Pipeline,Deployment Pipeline,Torch,Pruning,Compression,Model Pruning
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

