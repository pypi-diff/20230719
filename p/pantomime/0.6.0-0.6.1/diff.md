# Comparing `tmp/pantomime-0.6.0.tar.gz` & `tmp/pantomime-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pantomime-0.6.0.tar", last modified: Mon Feb  6 08:19:52 2023, max compression
+gzip compressed data, was "pantomime-0.6.1.tar", last modified: Wed Jul 19 12:40:23 2023, max compression
```

## Comparing `pantomime-0.6.0.tar` & `pantomime-0.6.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 08:19:52.268595 pantomime-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-02-06 08:19:34.000000 pantomime-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-02-06 08:19:34.000000 pantomime-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-02-06 08:19:52.268595 pantomime-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-02-06 08:19:34.000000 pantomime-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 08:19:52.264595 pantomime-0.6.0/pantomime/
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-02-06 08:19:34.000000 pantomime-0.6.0/pantomime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-02-06 08:19:34.000000 pantomime-0.6.0/pantomime/filename.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-02-06 08:19:34.000000 pantomime-0.6.0/pantomime/mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-02-06 08:19:34.000000 pantomime-0.6.0/pantomime/mime.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-02-06 08:19:34.000000 pantomime-0.6.0/pantomime/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 08:19:34.000000 pantomime-0.6.0/pantomime/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-02-06 08:19:34.000000 pantomime-0.6.0/pantomime/types.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-06 08:19:34.000000 pantomime-0.6.0/pantomime/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 08:19:52.268595 pantomime-0.6.0/pantomime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-02-06 08:19:52.000000 pantomime-0.6.0/pantomime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-02-06 08:19:52.000000 pantomime-0.6.0/pantomime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-06 08:19:52.000000 pantomime-0.6.0/pantomime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-06 08:19:52.000000 pantomime-0.6.0/pantomime.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-06 08:19:46.000000 pantomime-0.6.0/pantomime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-02-06 08:19:52.000000 pantomime-0.6.0/pantomime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-06 08:19:52.000000 pantomime-0.6.0/pantomime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-06 08:19:52.268595 pantomime-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-02-06 08:19:34.000000 pantomime-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 08:19:52.268595 pantomime-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 08:19:34.000000 pantomime-0.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-02-06 08:19:34.000000 pantomime-0.6.0/tests/test_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-02-06 08:19:34.000000 pantomime-0.6.0/tests/test_filename.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-02-06 08:19:34.000000 pantomime-0.6.0/tests/test_mime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:40:23.903046 pantomime-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-19 12:40:04.000000 pantomime-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-19 12:40:04.000000 pantomime-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-19 12:40:23.903046 pantomime-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-19 12:40:04.000000 pantomime-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:40:23.903046 pantomime-0.6.1/pantomime/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-19 12:40:04.000000 pantomime-0.6.1/pantomime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-19 12:40:04.000000 pantomime-0.6.1/pantomime/filename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-19 12:40:04.000000 pantomime-0.6.1/pantomime/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-19 12:40:04.000000 pantomime-0.6.1/pantomime/mime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-19 12:40:04.000000 pantomime-0.6.1/pantomime/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:40:04.000000 pantomime-0.6.1/pantomime/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-07-19 12:40:04.000000 pantomime-0.6.1/pantomime/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-19 12:40:04.000000 pantomime-0.6.1/pantomime/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:40:23.903046 pantomime-0.6.1/pantomime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-19 12:40:23.000000 pantomime-0.6.1/pantomime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-19 12:40:23.000000 pantomime-0.6.1/pantomime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 12:40:23.000000 pantomime-0.6.1/pantomime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 12:40:23.000000 pantomime-0.6.1/pantomime.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 12:40:08.000000 pantomime-0.6.1/pantomime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-19 12:40:23.000000 pantomime-0.6.1/pantomime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-19 12:40:23.000000 pantomime-0.6.1/pantomime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-19 12:40:23.907046 pantomime-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-19 12:40:04.000000 pantomime-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:40:23.903046 pantomime-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:40:04.000000 pantomime-0.6.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-19 12:40:04.000000 pantomime-0.6.1/tests/test_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-19 12:40:04.000000 pantomime-0.6.1/tests/test_filename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-19 12:40:04.000000 pantomime-0.6.1/tests/test_mime.py
```

### Comparing `pantomime-0.6.0/LICENSE` & `pantomime-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pantomime-0.6.0/PKG-INFO` & `pantomime-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pantomime
-Version: 0.6.0
+Version: 0.6.1
 Summary: MIME type normalisation and labels.
 Home-page: http://github.com/alephdata/pantomime
 Author: Journalism Development Network, Inc.
 Author-email: data@occrp.org
 License: MIT
 Keywords: mime mimetypes file types
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pantomime-0.6.0/README.md` & `pantomime-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `pantomime-0.6.0/pantomime/filename.py` & `pantomime-0.6.1/pantomime/filename.py`

 * *Files identical despite different names*

### Comparing `pantomime-0.6.0/pantomime/mappings.py` & `pantomime-0.6.1/pantomime/mappings.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Dict
 from pantomime.types import DEFAULT, PLAIN, DIRECTORY
-from pantomime.types import EXCEL, PDF, CSV, RTF, PSD, WORD
+from pantomime.types import EXCEL, PDF, CSV, RTF, PSD, WORD, XML
 from pantomime.types import RAR, ZIP, GZIP, TIFF, JPEG
 
 REPLACE: Dict[str, str] = {
     "x-unknown/unknown": DEFAULT,
     "unknown/unknown": DEFAULT,
     "x-unknown/octet-stream": DEFAULT,
     "application/x-unknown": DEFAULT,
@@ -14,14 +14,16 @@
     "x-unknown/stream": DEFAULT,
     "application/binary": DEFAULT,
     # Invalid
     "image/*": DEFAULT,
     "*/*": DEFAULT,
     # CSV
     "application/csv": CSV,
+    # XML
+    "text/xml": XML,
     # Plain
     "plain/text": PLAIN,
     "text/text": PLAIN,
     # Rich text
     "application/rtf": RTF,
     "file/rtf": RTF,
     "text/richtext": RTF,
```

### Comparing `pantomime-0.6.0/pantomime/mime.py` & `pantomime-0.6.1/pantomime/mime.py`

 * *Files identical despite different names*

### Comparing `pantomime-0.6.0/pantomime/parse.py` & `pantomime-0.6.1/pantomime/parse.py`

 * *Files identical despite different names*

### Comparing `pantomime-0.6.0/pantomime/types.py` & `pantomime-0.6.1/pantomime/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 EXCEL = "application/vnd.ms-excel"
 XLS = EXCEL
 XLSX = "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet"
 WORD = "application/vnd.ms-word"
 DOCX = "application/vnd.openxmlformats-officedocument.wordprocessing"
 CSV = "text/csv"
 RTF = "text/rtf"
-XML = "text/xml"
+XML = "application/xml"
 PSD = "image/vnd.adobe.photoshop"
 RAR = "application/rar"
 ZIP = "application/zip"
 GZIP = "application/gzip"
 RFC822 = "message/rfc822"
 HTML = "text/html"
 JPEG = "image/jpeg"
```

### Comparing `pantomime-0.6.0/pantomime.egg-info/PKG-INFO` & `pantomime-0.6.1/pantomime.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pantomime
-Version: 0.6.0
+Version: 0.6.1
 Summary: MIME type normalisation and labels.
 Home-page: http://github.com/alephdata/pantomime
 Author: Journalism Development Network, Inc.
 Author-email: data@occrp.org
 License: MIT
 Keywords: mime mimetypes file types
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pantomime-0.6.0/pantomime.egg-info/SOURCES.txt` & `pantomime-0.6.1/pantomime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pantomime-0.6.0/setup.py` & `pantomime-0.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md") as f:
     long_description = f.read()
 
 
 setup(
     name="pantomime",
-    version="0.6.0",
+    version="0.6.1",
     description="MIME type normalisation and labels.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
```

### Comparing `pantomime-0.6.0/tests/test_extension.py` & `pantomime-0.6.1/tests/test_extension.py`

 * *Files identical despite different names*

### Comparing `pantomime-0.6.0/tests/test_filename.py` & `pantomime-0.6.1/tests/test_filename.py`

 * *Files identical despite different names*

### Comparing `pantomime-0.6.0/tests/test_mime.py` & `pantomime-0.6.1/tests/test_mime.py`

 * *Files identical despite different names*

