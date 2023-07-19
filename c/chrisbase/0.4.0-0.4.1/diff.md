# Comparing `tmp/chrisbase-0.4.0.tar.gz` & `tmp/chrisbase-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chrisbase-0.4.0.tar", last modified: Sun Jul  9 15:13:02 2023, max compression
+gzip compressed data, was "chrisbase-0.4.1.tar", last modified: Wed Jul 19 09:23:56 2023, max compression
```

## Comparing `chrisbase-0.4.0.tar` & `chrisbase-0.4.1.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 15:13:02.541626 chrisbase-0.4.0/
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     1066 2023-07-08 17:51:01.000000 chrisbase-0.4.0/LICENSE
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)      816 2023-07-09 15:13:02.541626 chrisbase-0.4.0/PKG-INFO
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)      286 2023-07-08 17:51:01.000000 chrisbase-0.4.0/README.md
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)       81 2023-07-08 17:51:01.000000 chrisbase-0.4.0/pyproject.toml
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)      961 2023-07-09 15:13:02.541626 chrisbase-0.4.0/setup.cfg
-drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 15:13:02.541626 chrisbase-0.4.0/src/
-drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 15:13:02.541626 chrisbase-0.4.0/src/chrisbase/
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)        0 2023-07-08 17:51:01.000000 chrisbase-0.4.0/src/chrisbase/__init__.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)      151 2023-07-08 17:51:01.000000 chrisbase-0.4.0/src/chrisbase/cli.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)    24356 2023-07-08 17:51:01.000000 chrisbase-0.4.0/src/chrisbase/io.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     2170 2023-07-08 17:51:01.000000 chrisbase-0.4.0/src/chrisbase/morp.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     1059 2023-07-08 17:51:01.000000 chrisbase-0.4.0/src/chrisbase/time.py
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)     5122 2023-07-08 17:51:01.000000 chrisbase-0.4.0/src/chrisbase/util.py
-drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 15:13:02.541626 chrisbase-0.4.0/src/chrisbase.egg-info/
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)      816 2023-07-09 15:13:02.000000 chrisbase-0.4.0/src/chrisbase.egg-info/PKG-INFO
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)      431 2023-07-09 15:13:02.000000 chrisbase-0.4.0/src/chrisbase.egg-info/SOURCES.txt
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)        1 2023-07-09 15:13:02.000000 chrisbase-0.4.0/src/chrisbase.egg-info/dependency_links.txt
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)       48 2023-07-09 15:13:02.000000 chrisbase-0.4.0/src/chrisbase.egg-info/entry_points.txt
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)      143 2023-07-09 15:13:02.000000 chrisbase-0.4.0/src/chrisbase.egg-info/requires.txt
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)       10 2023-07-09 15:13:02.000000 chrisbase-0.4.0/src/chrisbase.egg-info/top_level.txt
--rw-r--r--   0 chrisjihee (1000016) users    (1000001)        1 2023-07-09 15:13:02.000000 chrisbase-0.4.0/src/chrisbase.egg-info/zip-safe
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-19 09:23:56.288288 chrisbase-0.4.1/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1066 2023-07-19 08:43:11.000000 chrisbase-0.4.1/LICENSE
+-rw-rw-r--   0 chris     (1000) chris     (1000)      816 2023-07-19 09:23:56.288288 chrisbase-0.4.1/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      286 2023-07-19 08:43:11.000000 chrisbase-0.4.1/README.md
+-rw-rw-r--   0 chris     (1000) chris     (1000)       81 2023-07-19 08:43:11.000000 chrisbase-0.4.1/pyproject.toml
+-rw-rw-r--   0 chris     (1000) chris     (1000)      990 2023-07-19 09:23:56.288288 chrisbase-0.4.1/setup.cfg
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-19 09:23:56.288288 chrisbase-0.4.1/src/
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-19 09:23:56.288288 chrisbase-0.4.1/src/chrisbase/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-07-19 08:43:11.000000 chrisbase-0.4.1/src/chrisbase/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      151 2023-07-19 08:43:11.000000 chrisbase-0.4.1/src/chrisbase/cli.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    24356 2023-07-19 08:43:11.000000 chrisbase-0.4.1/src/chrisbase/io.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2170 2023-07-19 08:43:11.000000 chrisbase-0.4.1/src/chrisbase/morp.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1279 2023-07-19 09:18:46.000000 chrisbase-0.4.1/src/chrisbase/net.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1059 2023-07-19 08:43:11.000000 chrisbase-0.4.1/src/chrisbase/time.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     5122 2023-07-19 08:43:11.000000 chrisbase-0.4.1/src/chrisbase/util.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-07-19 09:23:56.288288 chrisbase-0.4.1/src/chrisbase.egg-info/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      816 2023-07-19 09:23:56.000000 chrisbase-0.4.1/src/chrisbase.egg-info/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      452 2023-07-19 09:23:56.000000 chrisbase-0.4.1/src/chrisbase.egg-info/SOURCES.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-07-19 09:23:56.000000 chrisbase-0.4.1/src/chrisbase.egg-info/dependency_links.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)       48 2023-07-19 09:23:56.000000 chrisbase-0.4.1/src/chrisbase.egg-info/entry_points.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)      169 2023-07-19 09:23:56.000000 chrisbase-0.4.1/src/chrisbase.egg-info/requires.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)       10 2023-07-19 09:23:56.000000 chrisbase-0.4.1/src/chrisbase.egg-info/top_level.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-07-19 09:23:56.000000 chrisbase-0.4.1/src/chrisbase.egg-info/zip-safe
```

### Comparing `chrisbase-0.4.0/LICENSE` & `chrisbase-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chrisbase-0.4.0/PKG-INFO` & `chrisbase-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chrisbase
-Version: 0.4.0
+Version: 0.4.1
 Summary: A base tool for python programming.
 Home-page: https://github.com/chrisjihee/chrisbase
 Author: Jihee Ryu
 Author-email: chrisjihee@naver.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `chrisbase-0.4.0/setup.cfg` & `chrisbase-0.4.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = chrisbase
-version = 0.4.0
+version = 0.4.1
 author = Jihee Ryu
 author_email = chrisjihee@naver.com
 url = https://github.com/chrisjihee/chrisbase
 description = A base tool for python programming.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
@@ -33,14 +33,17 @@
 	matplotlib
 	sqlalchemy
 	dataclasses
 	dataclasses-json
 	scikit-learn
 	seqeval
 	openpyxl
+	netifaces
+	ipaddress
+	httpx
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 * = README.md
```

### Comparing `chrisbase-0.4.0/src/chrisbase/io.py` & `chrisbase-0.4.1/src/chrisbase/io.py`

 * *Files identical despite different names*

### Comparing `chrisbase-0.4.0/src/chrisbase/morp.py` & `chrisbase-0.4.1/src/chrisbase/morp.py`

 * *Files identical despite different names*

### Comparing `chrisbase-0.4.0/src/chrisbase/time.py` & `chrisbase-0.4.1/src/chrisbase/time.py`

 * *Files identical despite different names*

### Comparing `chrisbase-0.4.0/src/chrisbase/util.py` & `chrisbase-0.4.1/src/chrisbase/util.py`

 * *Files identical despite different names*

### Comparing `chrisbase-0.4.0/src/chrisbase.egg-info/PKG-INFO` & `chrisbase-0.4.1/src/chrisbase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chrisbase
-Version: 0.4.0
+Version: 0.4.1
 Summary: A base tool for python programming.
 Home-page: https://github.com/chrisjihee/chrisbase
 Author: Jihee Ryu
 Author-email: chrisjihee@naver.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

