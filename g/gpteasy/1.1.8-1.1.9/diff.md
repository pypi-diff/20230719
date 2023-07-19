# Comparing `tmp/gpteasy-1.1.8.tar.gz` & `tmp/gpteasy-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpteasy-1.1.8.tar", last modified: Tue Jul 18 14:51:38 2023, max compression
+gzip compressed data, was "gpteasy-1.1.9.tar", last modified: Tue Jul 18 19:18:58 2023, max compression
```

## Comparing `gpteasy-1.1.8.tar` & `gpteasy-1.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-07-18 14:51:38.015084 gpteasy-1.1.8/
--rw-r--r--   0 hp         (501) staff       (20)     1211 2020-11-28 21:10:12.000000 gpteasy-1.1.8/LICENSE
--rw-r--r--   0 hp         (501) staff       (20)     5188 2023-07-18 14:51:38.014769 gpteasy-1.1.8/PKG-INFO
--rw-r--r--   0 hp         (501) staff       (20)     3335 2023-07-18 14:51:30.000000 gpteasy-1.1.8/README.md
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-07-18 14:51:38.011625 gpteasy-1.1.8/gpteasy/
--rw-r--r--   0 hp         (501) staff       (20)      118 2023-06-16 09:28:57.000000 gpteasy-1.1.8/gpteasy/__init__.py
--rw-r--r--   0 hp         (501) staff       (20)     5420 2023-07-07 12:58:10.000000 gpteasy-1.1.8/gpteasy/commands.py
--rw-r--r--   0 hp         (501) staff       (20)      572 2023-06-16 09:08:00.000000 gpteasy-1.1.8/gpteasy/display.py
--rw-r--r--   0 hp         (501) staff       (20)    15090 2023-07-18 14:48:16.000000 gpteasy-1.1.8/gpteasy/gpt.py
--rw-r--r--   0 hp         (501) staff       (20)     1193 2023-06-17 13:35:36.000000 gpteasy-1.1.8/gpteasy/repl.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-07-18 14:51:38.014165 gpteasy-1.1.8/gpteasy.egg-info/
--rw-r--r--   0 hp         (501) staff       (20)     5188 2023-07-18 14:51:37.000000 gpteasy-1.1.8/gpteasy.egg-info/PKG-INFO
--rw-r--r--   0 hp         (501) staff       (20)      276 2023-07-18 14:51:38.000000 gpteasy-1.1.8/gpteasy.egg-info/SOURCES.txt
--rw-r--r--   0 hp         (501) staff       (20)        1 2023-07-18 14:51:37.000000 gpteasy-1.1.8/gpteasy.egg-info/dependency_links.txt
--rw-r--r--   0 hp         (501) staff       (20)      105 2023-07-18 14:51:38.000000 gpteasy-1.1.8/gpteasy.egg-info/requires.txt
--rw-r--r--   0 hp         (501) staff       (20)        8 2023-07-18 14:51:38.000000 gpteasy-1.1.8/gpteasy.egg-info/top_level.txt
--rw-r--r--   0 hp         (501) staff       (20)     1146 2023-07-18 14:51:30.000000 gpteasy-1.1.8/pyproject.toml
--rw-r--r--   0 hp         (501) staff       (20)       38 2023-07-18 14:51:38.015164 gpteasy-1.1.8/setup.cfg
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-07-18 19:18:58.845140 gpteasy-1.1.9/
+-rw-r--r--   0 hp         (501) staff       (20)     1211 2020-11-28 21:10:12.000000 gpteasy-1.1.9/LICENSE
+-rw-r--r--   0 hp         (501) staff       (20)     5188 2023-07-18 19:18:58.844680 gpteasy-1.1.9/PKG-INFO
+-rw-r--r--   0 hp         (501) staff       (20)     3335 2023-07-18 19:18:50.000000 gpteasy-1.1.9/README.md
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-07-18 19:18:58.840957 gpteasy-1.1.9/gpteasy/
+-rw-r--r--   0 hp         (501) staff       (20)      118 2023-06-16 09:28:57.000000 gpteasy-1.1.9/gpteasy/__init__.py
+-rw-r--r--   0 hp         (501) staff       (20)     5420 2023-07-07 12:58:10.000000 gpteasy-1.1.9/gpteasy/commands.py
+-rw-r--r--   0 hp         (501) staff       (20)      572 2023-06-16 09:08:00.000000 gpteasy-1.1.9/gpteasy/display.py
+-rw-r--r--   0 hp         (501) staff       (20)    15617 2023-07-18 19:18:24.000000 gpteasy-1.1.9/gpteasy/gpt.py
+-rw-r--r--   0 hp         (501) staff       (20)     1193 2023-06-17 13:35:36.000000 gpteasy-1.1.9/gpteasy/repl.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-07-18 19:18:58.844179 gpteasy-1.1.9/gpteasy.egg-info/
+-rw-r--r--   0 hp         (501) staff       (20)     5188 2023-07-18 19:18:58.000000 gpteasy-1.1.9/gpteasy.egg-info/PKG-INFO
+-rw-r--r--   0 hp         (501) staff       (20)      276 2023-07-18 19:18:58.000000 gpteasy-1.1.9/gpteasy.egg-info/SOURCES.txt
+-rw-r--r--   0 hp         (501) staff       (20)        1 2023-07-18 19:18:58.000000 gpteasy-1.1.9/gpteasy.egg-info/dependency_links.txt
+-rw-r--r--   0 hp         (501) staff       (20)      105 2023-07-18 19:18:58.000000 gpteasy-1.1.9/gpteasy.egg-info/requires.txt
+-rw-r--r--   0 hp         (501) staff       (20)        8 2023-07-18 19:18:58.000000 gpteasy-1.1.9/gpteasy.egg-info/top_level.txt
+-rw-r--r--   0 hp         (501) staff       (20)     1146 2023-07-18 19:18:50.000000 gpteasy-1.1.9/pyproject.toml
+-rw-r--r--   0 hp         (501) staff       (20)       38 2023-07-18 19:18:58.845291 gpteasy-1.1.9/setup.cfg
```

### Comparing `gpteasy-1.1.8/LICENSE` & `gpteasy-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gpteasy-1.1.8/PKG-INFO` & `gpteasy-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpteasy
-Version: 1.1.8
+Version: 1.1.9
 Summary: Makes working with OpenAi's GPT API super easy
 Author-email: HP Harmsen <hp@harmsen.nl>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -38,15 +38,15 @@
 License-File: LICENSE
 
 # GPT Easy
 
 Package to make working with the OpenAI GPT API in Python super easy.
 
 Author: Hans-Peter Harmsen (hp@harmsen.nl) \
-Current version: 1.1.8
+Current version: 1.1.9
 
 ## Installation
 1. Install the package:
 ~~~~bash
 python -m pip install gpteasy
 ~~~~
 2. Create an OpenAI acccount [here](https://platform.openai.com/))
```

### Comparing `gpteasy-1.1.8/README.md` & `gpteasy-1.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # GPT Easy
 
 Package to make working with the OpenAI GPT API in Python super easy.
 
 Author: Hans-Peter Harmsen (hp@harmsen.nl) \
-Current version: 1.1.8
+Current version: 1.1.9
 
 ## Installation
 1. Install the package:
 ~~~~bash
 python -m pip install gpteasy
 ~~~~
 2. Create an OpenAI acccount [here](https://platform.openai.com/))
```

### Comparing `gpteasy-1.1.8/gpteasy/commands.py` & `gpteasy-1.1.9/gpteasy/commands.py`

 * *Files identical despite different names*

### Comparing `gpteasy-1.1.8/gpteasy/display.py` & `gpteasy-1.1.9/gpteasy/display.py`

 * *Files identical despite different names*

### Comparing `gpteasy-1.1.8/gpteasy/gpt.py` & `gpteasy-1.1.9/gpteasy/gpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -309,14 +309,29 @@
             print_message(message)
 
     def file_input(self, filename):
         with open(filename, "r") as f:
             prompt = f.read()
         self.chat(prompt)
 
+    def dumps(self) -> str:
+        dict = {}
+        for key, value in self.__dict__.items():
+            if value is not None:
+                try:
+                    json.dumps(value)
+                    dict[key] = value
+                except ValueError:
+                    match key:
+                        case 'save_dir':
+                            dict[key] = str(value)
+                        case 'messages':
+                            dict[key] = [message.to_dict() for message in value]
+        return json.dumps(dict)
+
 
 class Message:
     """ Handles the completion as returned by GPT """
     def __init__(self, role=None, text_or_completion=None, function_name=None, function_content=None):
         self.role = role
         if isinstance(text_or_completion, str):
             self.text = text_or_completion
@@ -355,13 +370,12 @@
         if self.function_name:
             res += f' function_name: {self.function_name}'
         if self.function_content:
             res += f' function_content: {self.function_content}'
         return res
 
     def to_dict(self):
-        dict = {}
+        dictionary = {}
         for key, value in self.__dict__.items():
-            if value != None:
-                json.dumps(value)
-                dict[key] = value
-        return dict
+            if value is not None:
+                dictionary[key] = value
+        return dictionary
```

### Comparing `gpteasy-1.1.8/gpteasy/repl.py` & `gpteasy-1.1.9/gpteasy/repl.py`

 * *Files identical despite different names*

### Comparing `gpteasy-1.1.8/gpteasy.egg-info/PKG-INFO` & `gpteasy-1.1.9/gpteasy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpteasy
-Version: 1.1.8
+Version: 1.1.9
 Summary: Makes working with OpenAi's GPT API super easy
 Author-email: HP Harmsen <hp@harmsen.nl>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -38,15 +38,15 @@
 License-File: LICENSE
 
 # GPT Easy
 
 Package to make working with the OpenAI GPT API in Python super easy.
 
 Author: Hans-Peter Harmsen (hp@harmsen.nl) \
-Current version: 1.1.8
+Current version: 1.1.9
 
 ## Installation
 1. Install the package:
 ~~~~bash
 python -m pip install gpteasy
 ~~~~
 2. Create an OpenAI acccount [here](https://platform.openai.com/))
```

### Comparing `gpteasy-1.1.8/pyproject.toml` & `gpteasy-1.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gpteasy"
-version = "1.1.8"
+version = "1.1.9"
 description = "Makes working with OpenAi's GPT API super easy"
 readme = "README.md"
 authors = [{ name = "HP Harmsen", email = "hp@harmsen.nl" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

