# Comparing `tmp/convosense_utilities-1.0.0.tar.gz` & `tmp/convosense_utilities-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "convosense_utilities-1.0.0.tar", last modified: Wed Jul 19 09:17:03 2023, max compression
+gzip compressed data, was "convosense_utilities-1.0.1.tar", last modified: Wed Jul 19 09:55:46 2023, max compression
```

## Comparing `convosense_utilities-1.0.0.tar` & `convosense_utilities-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 09:17:03.374754 convosense_utilities-1.0.0/
--rw-rw-rw-   0        0        0    11556 2023-07-17 20:22:30.000000 convosense_utilities-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     6715 2023-07-19 09:17:03.369717 convosense_utilities-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     6036 2023-07-19 03:17:36.000000 convosense_utilities-1.0.0/README.md
--rw-rw-rw-   0        0        0      745 2023-07-19 09:08:59.000000 convosense_utilities-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-19 09:17:03.376720 convosense_utilities-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-19 09:17:03.258731 convosense_utilities-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-19 09:17:03.314754 convosense_utilities-1.0.0/src/convosense_utilities/
--rw-rw-rw-   0        0        0        0 2023-07-17 19:36:15.000000 convosense_utilities-1.0.0/src/convosense_utilities/__init__.py
--rw-rw-rw-   0        0        0     5063 2023-07-19 01:36:23.000000 convosense_utilities-1.0.0/src/convosense_utilities/email_signature_remover.py
-drwxrwxrwx   0        0        0        0 2023-07-19 09:17:03.367734 convosense_utilities-1.0.0/src/convosense_utilities.egg-info/
--rw-rw-rw-   0        0        0     6715 2023-07-19 09:17:03.000000 convosense_utilities-1.0.0/src/convosense_utilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2023-07-19 09:17:03.000000 convosense_utilities-1.0.0/src/convosense_utilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 09:17:03.000000 convosense_utilities-1.0.0/src/convosense_utilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-07-19 09:17:03.000000 convosense_utilities-1.0.0/src/convosense_utilities.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-07-19 09:17:03.000000 convosense_utilities-1.0.0/src/convosense_utilities.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-19 09:55:46.265807 convosense_utilities-1.0.1/
+-rw-rw-rw-   0        0        0    11556 2023-07-17 20:22:30.000000 convosense_utilities-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     6715 2023-07-19 09:55:46.264807 convosense_utilities-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6036 2023-07-19 03:17:36.000000 convosense_utilities-1.0.1/README.md
+-rw-rw-rw-   0        0        0      736 2023-07-19 09:55:19.000000 convosense_utilities-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-19 09:55:46.266814 convosense_utilities-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-19 09:55:46.156816 convosense_utilities-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-19 09:55:46.178810 convosense_utilities-1.0.1/src/convosense_utilities/
+-rw-rw-rw-   0        0        0        0 2023-07-17 19:36:15.000000 convosense_utilities-1.0.1/src/convosense_utilities/__init__.py
+-rw-rw-rw-   0        0        0     5063 2023-07-19 01:36:23.000000 convosense_utilities-1.0.1/src/convosense_utilities/email_signature_remover.py
+drwxrwxrwx   0        0        0        0 2023-07-19 09:55:46.263808 convosense_utilities-1.0.1/src/convosense_utilities.egg-info/
+-rw-rw-rw-   0        0        0     6715 2023-07-19 09:55:46.000000 convosense_utilities-1.0.1/src/convosense_utilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2023-07-19 09:55:46.000000 convosense_utilities-1.0.1/src/convosense_utilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 09:55:46.000000 convosense_utilities-1.0.1/src/convosense_utilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-07-19 09:55:46.000000 convosense_utilities-1.0.1/src/convosense_utilities.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-07-19 09:55:46.000000 convosense_utilities-1.0.1/src/convosense_utilities.egg-info/top_level.txt
```

### Comparing `convosense_utilities-1.0.0/LICENSE` & `convosense_utilities-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `convosense_utilities-1.0.0/PKG-INFO` & `convosense_utilities-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convosense_utilities
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package to extract the email body out of the email text, by removing signature, in order to get accurate sentiment results.
 Author-email: Swapnil Bonde <swapnilbonde94@gmail.com>
 Project-URL: GitHub repo, https://github.com/convosense/email_signature_remover
 Project-URL: Bug Tracker, https://github.com/convosense/email_signature_remover/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `convosense_utilities-1.0.0/README.md` & `convosense_utilities-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `convosense_utilities-1.0.0/pyproject.toml` & `convosense_utilities-1.0.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "convosense_utilities"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Swapnil Bonde", email="swapnilbonde94@gmail.com" }
 ]
 description = "A package to extract the email body out of the email text, by removing signature, in order to get accurate sentiment results."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -12,14 +12,13 @@
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
   "email_reply_parser",
   "nltk",
-  "spacy",
-  "re"
+  "spacy"
 ]
 
 [project.urls]
 "GitHub repo" = "https://github.com/convosense/email_signature_remover"
 "Bug Tracker" = "https://github.com/convosense/email_signature_remover/issues"
```

### Comparing `convosense_utilities-1.0.0/src/convosense_utilities/email_signature_remover.py` & `convosense_utilities-1.0.1/src/convosense_utilities/email_signature_remover.py`

 * *Files identical despite different names*

### Comparing `convosense_utilities-1.0.0/src/convosense_utilities.egg-info/PKG-INFO` & `convosense_utilities-1.0.1/src/convosense_utilities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convosense-utilities
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package to extract the email body out of the email text, by removing signature, in order to get accurate sentiment results.
 Author-email: Swapnil Bonde <swapnilbonde94@gmail.com>
 Project-URL: GitHub repo, https://github.com/convosense/email_signature_remover
 Project-URL: Bug Tracker, https://github.com/convosense/email_signature_remover/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

