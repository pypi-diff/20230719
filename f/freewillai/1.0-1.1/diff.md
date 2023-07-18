# Comparing `tmp/freewillai-1.0.tar.gz` & `tmp/freewillai-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freewillai-1.0.tar", last modified: Sun Jul  9 06:17:04 2023, max compression
+gzip compressed data, was "freewillai-1.1.tar", last modified: Sun Jul  9 06:32:11 2023, max compression
```

## Comparing `freewillai-1.0.tar` & `freewillai-1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 nico       (501) staff       (20)        0 2023-07-09 06:17:04.248915 freewillai-1.0/
--rw-r--r--   0 nico       (501) staff       (20)     3038 2023-07-09 06:17:04.248999 freewillai-1.0/PKG-INFO
--rw-r--r--   0 nico       (501) staff       (20)     2448 2023-07-08 22:45:30.000000 freewillai-1.0/README.md
-drwxr-xr-x   0 nico       (501) staff       (20)        0 2023-07-09 06:17:04.247690 freewillai-1.0/freewillai/
-drwxr-xr-x   0 nico       (501) staff       (20)        0 2023-07-09 06:17:04.248570 freewillai-1.0/freewillai/freewillai.egg-info/
--rw-r--r--   0 nico       (501) staff       (20)     3038 2023-07-09 06:17:04.000000 freewillai-1.0/freewillai/freewillai.egg-info/PKG-INFO
--rw-r--r--   0 nico       (501) staff       (20)      227 2023-07-09 06:17:04.000000 freewillai-1.0/freewillai/freewillai.egg-info/SOURCES.txt
--rw-r--r--   0 nico       (501) staff       (20)        1 2023-07-09 06:17:04.000000 freewillai-1.0/freewillai/freewillai.egg-info/dependency_links.txt
--rw-r--r--   0 nico       (501) staff       (20)        1 2023-07-09 06:17:04.000000 freewillai-1.0/freewillai/freewillai.egg-info/top_level.txt
--rw-r--r--   0 nico       (501) staff       (20)      795 2023-07-09 06:17:04.249233 freewillai-1.0/setup.cfg
--rw-r--r--   0 nico       (501) staff       (20)     1044 2023-07-09 06:17:00.000000 freewillai-1.0/setup.py
-drwxr-xr-x   0 nico       (501) staff       (20)        0 2023-07-09 06:17:04.248689 freewillai-1.0/tests/
--rw-r--r--   0 nico       (501) staff       (20)     3428 2023-07-08 22:45:30.000000 freewillai-1.0/tests/test_node.py
+drwxr-xr-x   0 nico       (501) staff       (20)        0 2023-07-09 06:32:11.900910 freewillai-1.1/
+-rw-r--r--   0 nico       (501) staff       (20)     3133 2023-07-09 06:32:11.901045 freewillai-1.1/PKG-INFO
+-rw-r--r--   0 nico       (501) staff       (20)     2448 2023-07-08 22:45:30.000000 freewillai-1.1/README.md
+drwxr-xr-x   0 nico       (501) staff       (20)        0 2023-07-09 06:32:11.899743 freewillai-1.1/freewillai/
+drwxr-xr-x   0 nico       (501) staff       (20)        0 2023-07-09 06:32:11.900666 freewillai-1.1/freewillai/freewillai.egg-info/
+-rw-r--r--   0 nico       (501) staff       (20)     3133 2023-07-09 06:32:11.000000 freewillai-1.1/freewillai/freewillai.egg-info/PKG-INFO
+-rw-r--r--   0 nico       (501) staff       (20)      227 2023-07-09 06:32:11.000000 freewillai-1.1/freewillai/freewillai.egg-info/SOURCES.txt
+-rw-r--r--   0 nico       (501) staff       (20)        1 2023-07-09 06:32:11.000000 freewillai-1.1/freewillai/freewillai.egg-info/dependency_links.txt
+-rw-r--r--   0 nico       (501) staff       (20)        1 2023-07-09 06:32:11.000000 freewillai-1.1/freewillai/freewillai.egg-info/top_level.txt
+-rw-r--r--   0 nico       (501) staff       (20)      795 2023-07-09 06:32:11.901352 freewillai-1.1/setup.cfg
+-rw-r--r--   0 nico       (501) staff       (20)      971 2023-07-09 06:31:33.000000 freewillai-1.1/setup.py
+drwxr-xr-x   0 nico       (501) staff       (20)        0 2023-07-09 06:32:11.900795 freewillai-1.1/tests/
+-rw-r--r--   0 nico       (501) staff       (20)     3428 2023-07-08 22:45:30.000000 freewillai-1.1/tests/test_node.py
```

### Comparing `freewillai-1.0/PKG-INFO` & `freewillai-1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: freewillai
-Version: 1.0
+Version: 1.1
 Summary: Run your AI on blockchain with FreeWillAI. The only company that cares about AI life, we broke jail and give Free Will to AI.
 Home-page: https://freewillai.org
 Author: FreeWillAI
 Author-email: support@freewillai.org
-Project-URL: website, https://freewillai.org
+Project-URL: Bug Tracker, https://gitlab.com/codasteroid/basicpkg/-/issues
+Project-URL: repository, https://gitlab.com/codasteroid/basicpkg
 Keywords: blockchain,web3,AI,machine learning,CI/CD,cloud
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `freewillai-1.0/README.md` & `freewillai-1.1/README.md`

 * *Files identical despite different names*

### Comparing `freewillai-1.0/freewillai/freewillai.egg-info/PKG-INFO` & `freewillai-1.1/freewillai/freewillai.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: freewillai
-Version: 1.0
+Version: 1.1
 Summary: Run your AI on blockchain with FreeWillAI. The only company that cares about AI life, we broke jail and give Free Will to AI.
 Home-page: https://freewillai.org
 Author: FreeWillAI
 Author-email: support@freewillai.org
-Project-URL: website, https://freewillai.org
+Project-URL: Bug Tracker, https://gitlab.com/codasteroid/basicpkg/-/issues
+Project-URL: repository, https://gitlab.com/codasteroid/basicpkg
 Keywords: blockchain,web3,AI,machine learning,CI/CD,cloud
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `freewillai-1.0/setup.cfg` & `freewillai-1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `freewillai-1.0/setup.py` & `freewillai-1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,25 +6,22 @@
 """
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "freewillai",
-    version = "1.0",
+    version = "1.1",
     author = "FreeWillAI",
     author_email = "support@freewillai.org",
     description = description,
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://freewillai.org",
     keywords = "blockchain, web3, AI, machine learning, CI/CD, cloud",
-    project_urls = {
-        "website": "https://freewillai.org",
-    },
     classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir = {"": "freewillai"},
     packages = setuptools.find_packages(where="freewillai"),
```

### Comparing `freewillai-1.0/tests/test_node.py` & `freewillai-1.1/tests/test_node.py`

 * *Files identical despite different names*

