# Comparing `tmp/torp-0.0.0.tar.gz` & `tmp/torp-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torp-0.0.0.tar", last modified: Tue Jul 18 05:06:06 2023, max compression
+gzip compressed data, was "torp-0.0.3.tar", last modified: Tue Jul 18 22:44:03 2023, max compression
```

## Comparing `torp-0.0.0.tar` & `torp-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 sathya    (1000) sathya    (1000)        0 2023-07-18 05:06:06.785776 torp-0.0.0/
--rw-rw-r--   0 sathya    (1000) sathya    (1000)     1068 2023-07-18 04:39:01.000000 torp-0.0.0/LICENSE.txt
--rw-rw-r--   0 sathya    (1000) sathya    (1000)       74 2023-07-18 05:06:06.785776 torp-0.0.0/PKG-INFO
--rw-rw-r--   0 sathya    (1000) sathya    (1000)     1905 2023-07-18 05:00:57.000000 torp-0.0.0/README.md
--rw-rw-r--   0 sathya    (1000) sathya    (1000)       79 2023-07-18 05:06:06.785776 torp-0.0.0/setup.cfg
--rw-rw-r--   0 sathya    (1000) sathya    (1000)      996 2023-07-18 05:04:46.000000 torp-0.0.0/setup.py
-drwxrwxr-x   0 sathya    (1000) sathya    (1000)        0 2023-07-18 05:06:06.785776 torp-0.0.0/torp/
--rw-rw-r--   0 sathya    (1000) sathya    (1000)       21 2023-07-18 04:38:20.000000 torp-0.0.0/torp/__init__.py
--rw-rw-r--   0 sathya    (1000) sathya    (1000)    14081 2023-07-17 22:23:26.000000 torp-0.0.0/torp/helper.py
-drwxrwxr-x   0 sathya    (1000) sathya    (1000)        0 2023-07-18 05:06:06.785776 torp-0.0.0/torp.egg-info/
--rw-rw-r--   0 sathya    (1000) sathya    (1000)       74 2023-07-18 05:06:06.000000 torp-0.0.0/torp.egg-info/PKG-INFO
--rw-rw-r--   0 sathya    (1000) sathya    (1000)      184 2023-07-18 05:06:06.000000 torp-0.0.0/torp.egg-info/SOURCES.txt
--rw-rw-r--   0 sathya    (1000) sathya    (1000)        1 2023-07-18 05:06:06.000000 torp-0.0.0/torp.egg-info/dependency_links.txt
--rw-rw-r--   0 sathya    (1000) sathya    (1000)        5 2023-07-18 05:06:06.000000 torp-0.0.0/torp.egg-info/top_level.txt
+drwxrwxr-x   0 sathya    (1000) sathya    (1000)        0 2023-07-18 22:44:03.808649 torp-0.0.3/
+-rw-rw-r--   0 sathya    (1000) sathya    (1000)     1068 2023-07-18 04:39:01.000000 torp-0.0.3/LICENSE.txt
+-rw-rw-r--   0 sathya    (1000) sathya    (1000)       74 2023-07-18 22:44:03.808649 torp-0.0.3/PKG-INFO
+-rw-rw-r--   0 sathya    (1000) sathya    (1000)     1905 2023-07-18 05:00:57.000000 torp-0.0.3/README.md
+-rw-rw-r--   0 sathya    (1000) sathya    (1000)       79 2023-07-18 22:44:03.808649 torp-0.0.3/setup.cfg
+-rw-rw-r--   0 sathya    (1000) sathya    (1000)     1012 2023-07-18 22:44:01.000000 torp-0.0.3/setup.py
+drwxrwxr-x   0 sathya    (1000) sathya    (1000)        0 2023-07-18 22:44:03.808649 torp-0.0.3/torp/
+-rw-rw-r--   0 sathya    (1000) sathya    (1000)      411 2023-07-18 22:29:22.000000 torp-0.0.3/torp/__init__.py
+-rw-rw-r--   0 sathya    (1000) sathya    (1000)    14081 2023-07-17 22:23:26.000000 torp-0.0.3/torp/helper.py
+drwxrwxr-x   0 sathya    (1000) sathya    (1000)        0 2023-07-18 22:44:03.808649 torp-0.0.3/torp.egg-info/
+-rw-rw-r--   0 sathya    (1000) sathya    (1000)       74 2023-07-18 22:44:03.000000 torp-0.0.3/torp.egg-info/PKG-INFO
+-rw-rw-r--   0 sathya    (1000) sathya    (1000)      184 2023-07-18 22:44:03.000000 torp-0.0.3/torp.egg-info/SOURCES.txt
+-rw-rw-r--   0 sathya    (1000) sathya    (1000)        1 2023-07-18 22:44:03.000000 torp-0.0.3/torp.egg-info/dependency_links.txt
+-rw-rw-r--   0 sathya    (1000) sathya    (1000)        5 2023-07-18 22:44:03.000000 torp-0.0.3/torp.egg-info/top_level.txt
```

### Comparing `torp-0.0.0/LICENSE.txt` & `torp-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `torp-0.0.0/README.md` & `torp-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `torp-0.0.0/setup.py` & `torp-0.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 
 setup_args = dict(
     name='Torch Helper',
-    version='0.0.6',
+    version='0.0.3',
     description='TORch helpeR',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n',
     license='MIT',
     packages=find_packages(),
     author='Sathyaprakash Narayanan',
     author_email='snaray17@ucsc.edu',
@@ -26,8 +26,8 @@
     requirement_path = lib_folder + './requirements.txt'
     install_requires = []
 
     if os.path.isfile(requirement_path):
         with open(requirement_path) as f:
             install_requires = f.read().splitlines()
     print(install_requires)
-    setup(name="torp", install_requires=install_requires)
+    setup(name="torp", version='0.0.3',install_requires=install_requires)
```

### Comparing `torp-0.0.0/torp/helper.py` & `torp-0.0.3/torp/helper.py`

 * *Files identical despite different names*

