# Comparing `tmp/khmernormalizer-0.0.1.tar.gz` & `tmp/khmernormalizer-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "khmernormalizer-0.0.1.tar", last modified: Wed Jul 19 08:53:38 2023, max compression
+gzip compressed data, was "khmernormalizer-0.0.2.tar", last modified: Wed Jul 19 09:17:31 2023, max compression
```

## Comparing `khmernormalizer-0.0.1.tar` & `khmernormalizer-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2023-07-19 08:53:38.112855 khmernormalizer-0.0.1/
--rw-r--r--   0 seanghay   (501) staff       (20)     1066 2023-07-19 08:53:38.112576 khmernormalizer-0.0.1/PKG-INFO
--rw-r--r--   0 seanghay   (501) staff       (20)      582 2023-07-19 08:48:01.000000 khmernormalizer-0.0.1/README.md
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2023-07-19 08:53:38.109855 khmernormalizer-0.0.1/khmernormalizer/
--rw-r--r--   0 seanghay   (501) staff       (20)       52 2023-07-19 05:09:47.000000 khmernormalizer-0.0.1/khmernormalizer/__init__.py
--rw-r--r--   0 seanghay   (501) staff       (20)    12453 2023-07-19 08:39:10.000000 khmernormalizer-0.0.1/khmernormalizer/mappings.py
--rw-r--r--   0 seanghay   (501) staff       (20)     1861 2023-07-19 08:39:10.000000 khmernormalizer-0.0.1/khmernormalizer/normalizer.py
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2023-07-19 08:53:38.112138 khmernormalizer-0.0.1/khmernormalizer.egg-info/
--rw-r--r--   0 seanghay   (501) staff       (20)     1066 2023-07-19 08:53:38.000000 khmernormalizer-0.0.1/khmernormalizer.egg-info/PKG-INFO
--rw-r--r--   0 seanghay   (501) staff       (20)      298 2023-07-19 08:53:38.000000 khmernormalizer-0.0.1/khmernormalizer.egg-info/SOURCES.txt
--rw-r--r--   0 seanghay   (501) staff       (20)        1 2023-07-19 08:53:38.000000 khmernormalizer-0.0.1/khmernormalizer.egg-info/dependency_links.txt
--rw-r--r--   0 seanghay   (501) staff       (20)       31 2023-07-19 08:53:38.000000 khmernormalizer-0.0.1/khmernormalizer.egg-info/requires.txt
--rw-r--r--   0 seanghay   (501) staff       (20)       16 2023-07-19 08:53:38.000000 khmernormalizer-0.0.1/khmernormalizer.egg-info/top_level.txt
--rw-r--r--   0 seanghay   (501) staff       (20)       38 2023-07-19 08:53:38.112949 khmernormalizer-0.0.1/setup.cfg
--rw-r--r--   0 seanghay   (501) staff       (20)      892 2023-07-19 08:53:22.000000 khmernormalizer-0.0.1/setup.py
+drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2023-07-19 09:17:31.859027 khmernormalizer-0.0.2/
+-rw-r--r--   0 seanghay   (501) staff       (20)     1065 2023-07-19 08:59:08.000000 khmernormalizer-0.0.2/LICENSE
+-rw-r--r--   0 seanghay   (501) staff       (20)     1157 2023-07-19 09:17:31.858750 khmernormalizer-0.0.2/PKG-INFO
+-rw-r--r--   0 seanghay   (501) staff       (20)      652 2023-07-19 08:56:16.000000 khmernormalizer-0.0.2/README.md
+drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2023-07-19 09:17:31.856448 khmernormalizer-0.0.2/khmernormalizer/
+-rw-r--r--   0 seanghay   (501) staff       (20)      101 2023-07-19 09:08:02.000000 khmernormalizer-0.0.2/khmernormalizer/__init__.py
+-rw-r--r--   0 seanghay   (501) staff       (20)    12453 2023-07-19 08:39:10.000000 khmernormalizer-0.0.2/khmernormalizer/mappings.py
+-rw-r--r--   0 seanghay   (501) staff       (20)     1862 2023-07-19 09:08:52.000000 khmernormalizer-0.0.2/khmernormalizer/normalizer.py
+drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2023-07-19 09:17:31.858363 khmernormalizer-0.0.2/khmernormalizer.egg-info/
+-rw-r--r--   0 seanghay   (501) staff       (20)     1157 2023-07-19 09:17:31.000000 khmernormalizer-0.0.2/khmernormalizer.egg-info/PKG-INFO
+-rw-r--r--   0 seanghay   (501) staff       (20)      306 2023-07-19 09:17:31.000000 khmernormalizer-0.0.2/khmernormalizer.egg-info/SOURCES.txt
+-rw-r--r--   0 seanghay   (501) staff       (20)        1 2023-07-19 09:17:31.000000 khmernormalizer-0.0.2/khmernormalizer.egg-info/dependency_links.txt
+-rw-r--r--   0 seanghay   (501) staff       (20)       31 2023-07-19 09:17:31.000000 khmernormalizer-0.0.2/khmernormalizer.egg-info/requires.txt
+-rw-r--r--   0 seanghay   (501) staff       (20)       16 2023-07-19 09:17:31.000000 khmernormalizer-0.0.2/khmernormalizer.egg-info/top_level.txt
+-rw-r--r--   0 seanghay   (501) staff       (20)       38 2023-07-19 09:17:31.859108 khmernormalizer-0.0.2/setup.cfg
+-rw-r--r--   0 seanghay   (501) staff       (20)      891 2023-07-19 09:12:15.000000 khmernormalizer-0.0.2/setup.py
```

### Comparing `khmernormalizer-0.0.1/PKG-INFO` & `khmernormalizer-0.0.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: khmernormalizer
-Version: 0.0.1
+Version: 0.0.2
 Summary: A missing toolkit for Khmer Natural Language Processing.
-Home-page: https://github.com/seanghay/khmer-normalizer
+Home-page: https://github.com/seanghay/khmernormalizer
 Author: Seanghay Yath
 Author-email: seanghay.dev@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
-Requires-Python: >=3.5
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
-### Khmer Normalizer 
+## Khmer Normalizer 
 
 A missing toolkit for **Khmer Natural Language Processing**.
 
 - Character Reordering
 - Duplicate Whitespaces
 - Remove zero width space
 - Remove emojis
@@ -24,14 +25,22 @@
 - Fix Unicode issues
 - Fix Khmer trailing vowels
 - URL Replacements
 - Unicode Normalization (NFKC)
 - Quotes symbols normalization
 - Remove repeated punctuations
 
+### Installation
+
+```shell
+pip install khmernormalizer
+```
+
+### Usage
+
 ```python
 from khmernormalizer import normalize
 
 text = "hello, world សួស្តី​ពិភពលោក !!!! 🇰🇭"
 result = normalize(text)
 # -> "hello, world សួស្តី​ពិភពលោក!"
 ```
```

### Comparing `khmernormalizer-0.0.1/README.md` & `khmernormalizer-0.0.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-### Khmer Normalizer 
+## Khmer Normalizer 
 
 A missing toolkit for **Khmer Natural Language Processing**.
 
 - Character Reordering
 - Duplicate Whitespaces
 - Remove zero width space
 - Remove emojis
@@ -10,14 +10,22 @@
 - Fix Unicode issues
 - Fix Khmer trailing vowels
 - URL Replacements
 - Unicode Normalization (NFKC)
 - Quotes symbols normalization
 - Remove repeated punctuations
 
+### Installation
+
+```shell
+pip install khmernormalizer
+```
+
+### Usage
+
 ```python
 from khmernormalizer import normalize
 
 text = "hello, world សួស្តី​ពិភពលោក !!!! 🇰🇭"
 result = normalize(text)
 # -> "hello, world សួស្តី​ពិភពលោក!"
 ```
```

### Comparing `khmernormalizer-0.0.1/khmernormalizer/mappings.py` & `khmernormalizer-0.0.2/khmernormalizer/mappings.py`

 * *Files identical despite different names*

### Comparing `khmernormalizer-0.0.1/khmernormalizer/normalizer.py` & `khmernormalizer-0.0.2/khmernormalizer/normalizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 # adapted from https://github.com/csebuetnlp/normalizer/blob/main/normalizer/const.py
 from ftfy import fix_text, TextFixerConfig
 from emoji import replace_emoji
 from khmernormalizer import mappings
+
 import re
 import unicodedata
 
 def fix_quotes(text):
     text = mappings.SINGLE_QUOTE_REGEX.sub("'", text)
     text = mappings.DOUBLE_QUOTE_REGEX.sub('"', text)
     return text
```

### Comparing `khmernormalizer-0.0.1/khmernormalizer.egg-info/PKG-INFO` & `khmernormalizer-0.0.2/khmernormalizer.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: khmernormalizer
-Version: 0.0.1
+Version: 0.0.2
 Summary: A missing toolkit for Khmer Natural Language Processing.
-Home-page: https://github.com/seanghay/khmer-normalizer
+Home-page: https://github.com/seanghay/khmernormalizer
 Author: Seanghay Yath
 Author-email: seanghay.dev@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
-Requires-Python: >=3.5
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
-### Khmer Normalizer 
+## Khmer Normalizer 
 
 A missing toolkit for **Khmer Natural Language Processing**.
 
 - Character Reordering
 - Duplicate Whitespaces
 - Remove zero width space
 - Remove emojis
@@ -24,14 +25,22 @@
 - Fix Unicode issues
 - Fix Khmer trailing vowels
 - URL Replacements
 - Unicode Normalization (NFKC)
 - Quotes symbols normalization
 - Remove repeated punctuations
 
+### Installation
+
+```shell
+pip install khmernormalizer
+```
+
+### Usage
+
 ```python
 from khmernormalizer import normalize
 
 text = "hello, world សួស្តី​ពិភពលោក !!!! 🇰🇭"
 result = normalize(text)
 # -> "hello, world សួស្តី​ពិភពលោក!"
 ```
```

### Comparing `khmernormalizer-0.0.1/setup.py` & `khmernormalizer-0.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     
 setuptools.setup(
   name="khmernormalizer",
   version=khmernormalizer.__version__,
   description="A missing toolkit for Khmer Natural Language Processing.",
   long_description=readme_md,
   long_description_content_type="text/markdown",
-  url="https://github.com/seanghay/khmer-normalizer",
+  url="https://github.com/seanghay/khmernormalizer",
   author="Seanghay Yath",
   author_email="seanghay.dev@gmail.com",
   packages=["khmernormalizer"],
   package_dir={"khmernormalizer": "khmernormalizer"}, 
   classifiers=[
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
@@ -24,9 +24,9 @@
   install_requires=[
     "regex",
     "emoji==2.6.0",
     "ftfy==6.1.1"
   ],
   package_data={'': ["*"]},
   include_package_data=True,
-  python_requires='>=3.5'
+  python_requires='>=3.7'
 )
```

