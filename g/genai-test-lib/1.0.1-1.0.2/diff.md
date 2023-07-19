# Comparing `tmp/genai_test_lib-1.0.1.tar.gz` & `tmp/genai_test_lib-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genai_test_lib-1.0.1.tar", last modified: Tue Jul 18 12:23:16 2023, max compression
+gzip compressed data, was "genai_test_lib-1.0.2.tar", last modified: Wed Jul 19 14:02:45 2023, max compression
```

## Comparing `genai_test_lib-1.0.1.tar` & `genai_test_lib-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxr-xr-x   0 atul       (501) staff       (20)        0 2023-07-18 12:23:16.824647 genai_test_lib-1.0.1/
--rw-r--r--   0 atul       (501) staff       (20)      188 2023-07-18 12:23:16.824480 genai_test_lib-1.0.1/PKG-INFO
-drwxr-xr-x   0 atul       (501) staff       (20)        0 2023-07-18 12:23:16.822472 genai_test_lib-1.0.1/genai_test_lib/
--rw-r--r--   0 atul       (501) staff       (20)        0 2023-07-18 12:20:19.000000 genai_test_lib-1.0.1/genai_test_lib/__init__.py
-drwxr-xr-x   0 atul       (501) staff       (20)        0 2023-07-18 12:23:16.824110 genai_test_lib-1.0.1/genai_test_lib/text_comparision/
--rw-r--r--   0 atul       (501) staff       (20)        0 2023-07-18 12:20:19.000000 genai_test_lib-1.0.1/genai_test_lib/text_comparision/__init__.py
--rw-r--r--   0 atul       (501) staff       (20)      594 2023-07-18 08:00:17.000000 genai_test_lib-1.0.1/genai_test_lib/text_comparision/output_parser.py
--rw-r--r--   0 atul       (501) staff       (20)     2189 2023-07-18 12:22:52.000000 genai_test_lib-1.0.1/genai_test_lib/text_comparision/text_compare.py
-drwxr-xr-x   0 atul       (501) staff       (20)        0 2023-07-18 12:23:16.823411 genai_test_lib-1.0.1/genai_test_lib.egg-info/
--rw-r--r--   0 atul       (501) staff       (20)      188 2023-07-18 12:23:16.000000 genai_test_lib-1.0.1/genai_test_lib.egg-info/PKG-INFO
--rw-r--r--   0 atul       (501) staff       (20)      402 2023-07-18 12:23:16.000000 genai_test_lib-1.0.1/genai_test_lib.egg-info/SOURCES.txt
--rw-r--r--   0 atul       (501) staff       (20)        1 2023-07-18 12:23:16.000000 genai_test_lib-1.0.1/genai_test_lib.egg-info/dependency_links.txt
--rw-r--r--   0 atul       (501) staff       (20)        1 2023-07-18 12:23:16.000000 genai_test_lib-1.0.1/genai_test_lib.egg-info/not-zip-safe
--rw-r--r--   0 atul       (501) staff       (20)       17 2023-07-18 12:23:16.000000 genai_test_lib-1.0.1/genai_test_lib.egg-info/requires.txt
--rw-r--r--   0 atul       (501) staff       (20)       15 2023-07-18 12:23:16.000000 genai_test_lib-1.0.1/genai_test_lib.egg-info/top_level.txt
--rw-r--r--   0 atul       (501) staff       (20)       38 2023-07-18 12:23:16.824713 genai_test_lib-1.0.1/setup.cfg
--rw-r--r--   0 atul       (501) staff       (20)      238 2023-07-18 12:21:31.000000 genai_test_lib-1.0.1/setup.py
+drwxr-xr-x   0 atul       (501) staff       (20)        0 2023-07-19 14:02:45.416931 genai_test_lib-1.0.2/
+-rw-r--r--   0 atul       (501) staff       (20)     1065 2023-07-11 03:33:05.000000 genai_test_lib-1.0.2/LICENSE
+-rw-r--r--   0 atul       (501) staff       (20)       80 2023-07-19 14:02:45.416743 genai_test_lib-1.0.2/PKG-INFO
+drwxr-xr-x   0 atul       (501) staff       (20)        0 2023-07-19 14:02:45.414569 genai_test_lib-1.0.2/genai_test_lib/
+-rw-r--r--   0 atul       (501) staff       (20)        0 2023-07-18 12:20:19.000000 genai_test_lib-1.0.2/genai_test_lib/__init__.py
+drwxr-xr-x   0 atul       (501) staff       (20)        0 2023-07-19 14:02:45.415782 genai_test_lib-1.0.2/genai_test_lib/generate_qna/
+-rw-r--r--   0 atul       (501) staff       (20)        0 2023-07-18 13:31:53.000000 genai_test_lib-1.0.2/genai_test_lib/generate_qna/__init__.py
+-rw-r--r--   0 atul       (501) staff       (20)     5768 2023-07-19 14:01:49.000000 genai_test_lib-1.0.2/genai_test_lib/generate_qna/retrive_qna.py
+drwxr-xr-x   0 atul       (501) staff       (20)        0 2023-07-19 14:02:45.416438 genai_test_lib-1.0.2/genai_test_lib/text_comparision/
+-rw-r--r--   0 atul       (501) staff       (20)        0 2023-07-18 12:20:19.000000 genai_test_lib-1.0.2/genai_test_lib/text_comparision/__init__.py
+-rw-r--r--   0 atul       (501) staff       (20)      594 2023-07-18 08:00:17.000000 genai_test_lib-1.0.2/genai_test_lib/text_comparision/output_parser.py
+-rw-r--r--   0 atul       (501) staff       (20)     2189 2023-07-19 07:39:47.000000 genai_test_lib-1.0.2/genai_test_lib/text_comparision/text_compare.py
+drwxr-xr-x   0 atul       (501) staff       (20)        0 2023-07-19 14:02:45.415503 genai_test_lib-1.0.2/genai_test_lib.egg-info/
+-rw-r--r--   0 atul       (501) staff       (20)       80 2023-07-19 14:02:45.000000 genai_test_lib-1.0.2/genai_test_lib.egg-info/PKG-INFO
+-rw-r--r--   0 atul       (501) staff       (20)      493 2023-07-19 14:02:45.000000 genai_test_lib-1.0.2/genai_test_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 atul       (501) staff       (20)        1 2023-07-19 14:02:45.000000 genai_test_lib-1.0.2/genai_test_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 atul       (501) staff       (20)        1 2023-07-19 14:02:45.000000 genai_test_lib-1.0.2/genai_test_lib.egg-info/not-zip-safe
+-rw-r--r--   0 atul       (501) staff       (20)       17 2023-07-19 14:02:45.000000 genai_test_lib-1.0.2/genai_test_lib.egg-info/requires.txt
+-rw-r--r--   0 atul       (501) staff       (20)       15 2023-07-19 14:02:45.000000 genai_test_lib-1.0.2/genai_test_lib.egg-info/top_level.txt
+-rw-r--r--   0 atul       (501) staff       (20)       38 2023-07-19 14:02:45.416978 genai_test_lib-1.0.2/setup.cfg
+-rw-r--r--   0 atul       (501) staff       (20)      238 2023-07-19 14:02:32.000000 genai_test_lib-1.0.2/setup.py
```

### Comparing `genai_test_lib-1.0.1/genai_test_lib/text_comparision/output_parser.py` & `genai_test_lib-1.0.2/genai_test_lib/text_comparision/output_parser.py`

 * *Files identical despite different names*

### Comparing `genai_test_lib-1.0.1/genai_test_lib/text_comparision/text_compare.py` & `genai_test_lib-1.0.2/genai_test_lib/text_comparision/text_compare.py`

 * *Files identical despite different names*

