# Comparing `tmp/pigeonsai-0.0.16.tar.gz` & `tmp/pigeonsai-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pigeonsai-0.0.16.tar", last modified: Thu Jun 29 20:56:41 2023, max compression
+gzip compressed data, was "pigeonsai-0.0.17.tar", last modified: Wed Jul 19 04:57:53 2023, max compression
```

## Comparing `pigeonsai-0.0.16.tar` & `pigeonsai-0.0.17.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-29 20:56:41.470142 pigeonsai-0.0.16/
--rw-r--r--   0 ariaattar   (501) staff       (20)     2922 2023-06-29 20:56:41.469952 pigeonsai-0.0.16/PKG-INFO
--rw-r--r--   0 ariaattar   (501) staff       (20)     1508 2023-06-03 00:14:17.000000 pigeonsai-0.0.16/README.md
--rw-r--r--   0 ariaattar   (501) staff       (20)       38 2023-06-29 20:56:41.470195 pigeonsai-0.0.16/setup.cfg
--rw-r--r--   0 ariaattar   (501) staff       (20)     2065 2023-06-29 20:56:01.000000 pigeonsai-0.0.16/setup.py
-drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-29 20:56:41.467481 pigeonsai-0.0.16/src/
-drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-29 20:56:41.468276 pigeonsai-0.0.16/src/pigeonsai/
--rw-r--r--   0 ariaattar   (501) staff       (20)       50 2023-06-15 18:46:00.000000 pigeonsai-0.0.16/src/pigeonsai/__init__.py
--rw-r--r--   0 ariaattar   (501) staff       (20)     6310 2023-06-29 20:55:48.000000 pigeonsai-0.0.16/src/pigeonsai/pigeonsdb.py
-drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-29 20:56:41.469278 pigeonsai-0.0.16/src/pigeonsai.egg-info/
--rw-r--r--   0 ariaattar   (501) staff       (20)     2922 2023-06-29 20:56:41.000000 pigeonsai-0.0.16/src/pigeonsai.egg-info/PKG-INFO
--rw-r--r--   0 ariaattar   (501) staff       (20)      279 2023-06-29 20:56:41.000000 pigeonsai-0.0.16/src/pigeonsai.egg-info/SOURCES.txt
--rw-r--r--   0 ariaattar   (501) staff       (20)        1 2023-06-29 20:56:41.000000 pigeonsai-0.0.16/src/pigeonsai.egg-info/dependency_links.txt
--rw-r--r--   0 ariaattar   (501) staff       (20)       77 2023-06-29 20:56:41.000000 pigeonsai-0.0.16/src/pigeonsai.egg-info/requires.txt
--rw-r--r--   0 ariaattar   (501) staff       (20)       10 2023-06-29 20:56:41.000000 pigeonsai-0.0.16/src/pigeonsai.egg-info/top_level.txt
-drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-29 20:56:41.469495 pigeonsai-0.0.16/tests/
--rw-r--r--   0 ariaattar   (501) staff       (20)      609 2023-06-02 23:54:25.000000 pigeonsai-0.0.16/tests/test_pigeonsdb.py
+drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-07-19 04:57:53.644374 pigeonsai-0.0.17/
+-rw-r--r--   0 ariaattar   (501) staff       (20)     2922 2023-07-19 04:57:53.644226 pigeonsai-0.0.17/PKG-INFO
+-rw-r--r--   0 ariaattar   (501) staff       (20)     1508 2023-06-03 00:14:17.000000 pigeonsai-0.0.17/README.md
+-rw-r--r--   0 ariaattar   (501) staff       (20)       38 2023-07-19 04:57:53.644420 pigeonsai-0.0.17/setup.cfg
+-rw-r--r--   0 ariaattar   (501) staff       (20)     2065 2023-07-19 04:57:36.000000 pigeonsai-0.0.17/setup.py
+drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-07-19 04:57:53.640925 pigeonsai-0.0.17/src/
+drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-07-19 04:57:53.642153 pigeonsai-0.0.17/src/pigeonsai/
+-rw-r--r--   0 ariaattar   (501) staff       (20)       50 2023-06-15 18:46:00.000000 pigeonsai-0.0.17/src/pigeonsai/__init__.py
+-rw-r--r--   0 ariaattar   (501) staff       (20)     7826 2023-07-19 04:56:41.000000 pigeonsai-0.0.17/src/pigeonsai/pigeonsdb.py
+-rw-r--r--   0 ariaattar   (501) staff       (20)      710 2023-07-19 03:40:55.000000 pigeonsai-0.0.17/src/pigeonsai/utils.py
+drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-07-19 04:57:53.643825 pigeonsai-0.0.17/src/pigeonsai.egg-info/
+-rw-r--r--   0 ariaattar   (501) staff       (20)     2922 2023-07-19 04:57:53.000000 pigeonsai-0.0.17/src/pigeonsai.egg-info/PKG-INFO
+-rw-r--r--   0 ariaattar   (501) staff       (20)      302 2023-07-19 04:57:53.000000 pigeonsai-0.0.17/src/pigeonsai.egg-info/SOURCES.txt
+-rw-r--r--   0 ariaattar   (501) staff       (20)        1 2023-07-19 04:57:53.000000 pigeonsai-0.0.17/src/pigeonsai.egg-info/dependency_links.txt
+-rw-r--r--   0 ariaattar   (501) staff       (20)       90 2023-07-19 04:57:53.000000 pigeonsai-0.0.17/src/pigeonsai.egg-info/requires.txt
+-rw-r--r--   0 ariaattar   (501) staff       (20)       10 2023-07-19 04:57:53.000000 pigeonsai-0.0.17/src/pigeonsai.egg-info/top_level.txt
+drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-07-19 04:57:53.643964 pigeonsai-0.0.17/tests/
+-rw-r--r--   0 ariaattar   (501) staff       (20)      609 2023-06-02 23:54:25.000000 pigeonsai-0.0.17/tests/test_pigeonsdb.py
```

### Comparing `pigeonsai-0.0.16/PKG-INFO` & `pigeonsai-0.0.17/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pigeonsai
-Version: 0.0.16
+Version: 0.0.17
 Summary: PigeonAI client and SDK
 Home-page: https://www.pigeonsai.com/
 Author: PigeonsAI Inc.
 Author-email: info@pigeonsai.com
 License: Proprietary License
 Project-URL: Homepage, https://www.pigeonsai.com
 Project-URL: Documentation, https://pigeonsai.com/docs
```

### Comparing `pigeonsai-0.0.16/README.md` & `pigeonsai-0.0.17/README.md`

 * *Files identical despite different names*

### Comparing `pigeonsai-0.0.16/setup.py` & `pigeonsai-0.0.17/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 long_desc = """
 PigeonsAI is an ecosystem to build production ready machine learning applications.
 """
 
 setup(
     name="pigeonsai",
-    version="0.0.16",
+    version="0.0.17",
     description="PigeonAI client and SDK",
     license="Proprietary License",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     url="https://www.pigeonsai.com/",
     project_urls={
         "Homepage": "https://www.pigeonsai.com",
```

### Comparing `pigeonsai-0.0.16/src/pigeonsai.egg-info/PKG-INFO` & `pigeonsai-0.0.17/src/pigeonsai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pigeonsai
-Version: 0.0.16
+Version: 0.0.17
 Summary: PigeonAI client and SDK
 Home-page: https://www.pigeonsai.com/
 Author: PigeonsAI Inc.
 Author-email: info@pigeonsai.com
 License: Proprietary License
 Project-URL: Homepage, https://www.pigeonsai.com
 Project-URL: Documentation, https://pigeonsai.com/docs
```

### Comparing `pigeonsai-0.0.16/tests/test_pigeonsdb.py` & `pigeonsai-0.0.17/tests/test_pigeonsdb.py`

 * *Files identical despite different names*

