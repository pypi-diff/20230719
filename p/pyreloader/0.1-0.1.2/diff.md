# Comparing `tmp/pyreloader-0.1.tar.gz` & `tmp/pyreloader-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyreloader-0.1.tar", last modified: Wed Jul 19 07:37:22 2023, max compression
+gzip compressed data, was "pyreloader-0.1.2.tar", last modified: Wed Jul 19 07:54:22 2023, max compression
```

## Comparing `pyreloader-0.1.tar` & `pyreloader-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 d067954    (501) staff       (20)        0 2023-07-19 07:37:22.597413 pyreloader-0.1/
--rw-r--r--   0 d067954    (501) staff       (20)     1077 2023-07-19 07:05:20.000000 pyreloader-0.1/LICENSE.txt
--rw-r--r--   0 d067954    (501) staff       (20)      647 2023-07-19 07:37:22.597027 pyreloader-0.1/PKG-INFO
--rw-r--r--   0 d067954    (501) staff       (20)      206 2023-07-19 07:05:20.000000 pyreloader-0.1/README.md
--rw-r--r--   0 d067954    (501) staff       (20)       98 2023-07-19 07:27:54.000000 pyreloader-0.1/pyproject.toml
-drwxr-xr-x   0 d067954    (501) staff       (20)        0 2023-07-19 07:37:22.592488 pyreloader-0.1/pyreloader.egg-info/
--rw-r--r--   0 d067954    (501) staff       (20)      647 2023-07-19 07:37:22.000000 pyreloader-0.1/pyreloader.egg-info/PKG-INFO
--rw-r--r--   0 d067954    (501) staff       (20)      218 2023-07-19 07:37:22.000000 pyreloader-0.1/pyreloader.egg-info/SOURCES.txt
--rw-r--r--   0 d067954    (501) staff       (20)        1 2023-07-19 07:37:22.000000 pyreloader-0.1/pyreloader.egg-info/dependency_links.txt
--rw-r--r--   0 d067954    (501) staff       (20)       47 2023-07-19 07:37:22.000000 pyreloader-0.1/pyreloader.egg-info/entry_points.txt
--rw-r--r--   0 d067954    (501) staff       (20)       11 2023-07-19 07:37:22.000000 pyreloader-0.1/pyreloader.egg-info/top_level.txt
--rw-r--r--   0 d067954    (501) staff       (20)       38 2023-07-19 07:37:22.597508 pyreloader-0.1/setup.cfg
--rw-r--r--   0 d067954    (501) staff       (20)      810 2023-07-19 07:35:32.000000 pyreloader-0.1/setup.py
+drwxr-xr-x   0 d067954    (501) staff       (20)        0 2023-07-19 07:54:22.239943 pyreloader-0.1.2/
+-rw-r--r--   0 d067954    (501) staff       (20)     1077 2023-07-19 07:05:20.000000 pyreloader-0.1.2/LICENSE.txt
+-rw-r--r--   0 d067954    (501) staff       (20)      663 2023-07-19 07:54:22.239653 pyreloader-0.1.2/PKG-INFO
+-rw-r--r--   0 d067954    (501) staff       (20)      212 2023-07-19 07:53:23.000000 pyreloader-0.1.2/README.md
+-rw-r--r--   0 d067954    (501) staff       (20)       98 2023-07-19 07:38:13.000000 pyreloader-0.1.2/pyproject.toml
+drwxr-xr-x   0 d067954    (501) staff       (20)        0 2023-07-19 07:54:22.238732 pyreloader-0.1.2/pyreloader.egg-info/
+-rw-r--r--   0 d067954    (501) staff       (20)      663 2023-07-19 07:54:22.000000 pyreloader-0.1.2/pyreloader.egg-info/PKG-INFO
+-rw-r--r--   0 d067954    (501) staff       (20)      218 2023-07-19 07:54:22.000000 pyreloader-0.1.2/pyreloader.egg-info/SOURCES.txt
+-rw-r--r--   0 d067954    (501) staff       (20)        1 2023-07-19 07:54:22.000000 pyreloader-0.1.2/pyreloader.egg-info/dependency_links.txt
+-rw-r--r--   0 d067954    (501) staff       (20)       47 2023-07-19 07:54:22.000000 pyreloader-0.1.2/pyreloader.egg-info/entry_points.txt
+-rw-r--r--   0 d067954    (501) staff       (20)       11 2023-07-19 07:54:22.000000 pyreloader-0.1.2/pyreloader.egg-info/top_level.txt
+-rw-r--r--   0 d067954    (501) staff       (20)       38 2023-07-19 07:54:22.239991 pyreloader-0.1.2/setup.cfg
+-rw-r--r--   0 d067954    (501) staff       (20)      820 2023-07-19 07:54:01.000000 pyreloader-0.1.2/setup.py
```

### Comparing `pyreloader-0.1/LICENSE.txt` & `pyreloader-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyreloader-0.1/PKG-INFO` & `pyreloader-0.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: pyreloader
-Version: 0.1
-Summary: Reload a program on signal HUP.
+Version: 0.1.2
+Summary: Reload a python program on kill signal.
 Home-page: https://github.com/chuan137/pyreloader
 Author: Chuan Miao
 Author-email: chuan137@gmail.com
 License: MIT
 Keywords: reload server
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# Reloader
+# PyReloader
 
 Start given python script and reloads on signal SIGHUP.
 
 Installation:
 
-pip install reloader
+pip install pyreloader
 
 Usage:
 
-Start program: `reloader ./server.py`
+Start program: `pyreloader ./server.py`
 
 Reload program: `kill -HUP <pid of parent process>`
```

### Comparing `pyreloader-0.1/pyreloader.egg-info/PKG-INFO` & `pyreloader-0.1.2/pyreloader.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: pyreloader
-Version: 0.1
-Summary: Reload a program on signal HUP.
+Version: 0.1.2
+Summary: Reload a python program on kill signal.
 Home-page: https://github.com/chuan137/pyreloader
 Author: Chuan Miao
 Author-email: chuan137@gmail.com
 License: MIT
 Keywords: reload server
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# Reloader
+# PyReloader
 
 Start given python script and reloads on signal SIGHUP.
 
 Installation:
 
-pip install reloader
+pip install pyreloader
 
 Usage:
 
-Start program: `reloader ./server.py`
+Start program: `pyreloader ./server.py`
 
 Reload program: `kill -HUP <pid of parent process>`
```

### Comparing `pyreloader-0.1/setup.py` & `pyreloader-0.1.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 from setuptools import setup
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name = "pyreloader",
-    version = "0.1",
+    version = "0.1.2",
     author = "Chuan Miao",
     author_email = "chuan137@gmail.com",
-    description = ("Reload a program on signal HUP."),
+    description = ("Reload a python program on kill signal."),
     license = "MIT",
     keywords = "reload server",
     url = "https://github.com/chuan137/pyreloader",
     py_modules=['pyreloader'],
     long_description_content_type="text/markdown",
     long_description=read('README.md'),
     classifiers=[
```

