# Comparing `tmp/open_interpreter-0.0.231.tar.gz` & `tmp/open_interpreter-0.0.232.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_interpreter-0.0.231.tar", max compression
+gzip compressed data, was "open_interpreter-0.0.232.tar", max compression
```

## Comparing `open_interpreter-0.0.231.tar` & `open_interpreter-0.0.232.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.231/LICENSE
--rw-r--r--   0        0        0     5627 2023-07-18 19:30:20.415609 open_interpreter-0.0.231/README.md
--rw-r--r--   0        0        0      135 2023-07-14 08:44:08.027686 open_interpreter-0.0.231/interpreter/__init__.py
--rw-r--r--   0        0        0     5903 2023-07-19 02:14:04.928691 open_interpreter-0.0.231/interpreter/exec.py
--rw-r--r--   0        0        0     7046 2023-07-19 04:34:31.280710 open_interpreter-0.0.231/interpreter/interpreter.py
--rw-r--r--   0        0        0     3665 2023-07-19 04:08:44.789294 open_interpreter-0.0.231/interpreter/json_utils.py
--rw-r--r--   0        0        0     3526 2023-07-19 02:26:22.378280 open_interpreter-0.0.231/interpreter/openai_utils.py
--rw-r--r--   0        0        0     2279 2023-07-19 05:03:34.928002 open_interpreter-0.0.231/interpreter/system_message.txt
--rw-r--r--   0        0        0     3062 2023-07-19 04:30:14.739747 open_interpreter-0.0.231/interpreter/system_message_experimental.txt
--rw-r--r--   0        0        0     3322 2023-07-19 00:31:12.448238 open_interpreter-0.0.231/interpreter/view.py
--rw-r--r--   0        0        0      542 2023-07-19 05:04:51.013033 open_interpreter-0.0.231/pyproject.toml
--rw-r--r--   0        0        0     6208 1970-01-01 00:00:00.000000 open_interpreter-0.0.231/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.232/LICENSE
+-rw-r--r--   0        0        0     5627 2023-07-18 19:30:20.415609 open_interpreter-0.0.232/README.md
+-rw-r--r--   0        0        0      135 2023-07-14 08:44:08.027686 open_interpreter-0.0.232/interpreter/__init__.py
+-rw-r--r--   0        0        0     5903 2023-07-19 02:14:04.928691 open_interpreter-0.0.232/interpreter/exec.py
+-rw-r--r--   0        0        0     6848 2023-07-19 06:28:40.373577 open_interpreter-0.0.232/interpreter/interpreter.py
+-rw-r--r--   0        0        0     3665 2023-07-19 04:08:44.789294 open_interpreter-0.0.232/interpreter/json_utils.py
+-rw-r--r--   0        0        0     3526 2023-07-19 02:26:22.378280 open_interpreter-0.0.232/interpreter/openai_utils.py
+-rw-r--r--   0        0        0     2279 2023-07-19 05:03:34.928002 open_interpreter-0.0.232/interpreter/system_message.txt
+-rw-r--r--   0        0        0     3062 2023-07-19 06:29:05.530210 open_interpreter-0.0.232/interpreter/system_message_scratch_sheet.txt
+-rw-r--r--   0        0        0     3322 2023-07-19 00:31:12.448238 open_interpreter-0.0.232/interpreter/view.py
+-rw-r--r--   0        0        0      542 2023-07-19 06:45:51.237796 open_interpreter-0.0.232/pyproject.toml
+-rw-r--r--   0        0        0     6208 1970-01-01 00:00:00.000000 open_interpreter-0.0.232/PKG-INFO
```

### Comparing `open_interpreter-0.0.231/LICENSE` & `open_interpreter-0.0.232/LICENSE`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.231/README.md` & `open_interpreter-0.0.232/README.md`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.231/interpreter/exec.py` & `open_interpreter-0.0.232/interpreter/exec.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.231/interpreter/interpreter.py` & `open_interpreter-0.0.232/interpreter/interpreter.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,23 +22,20 @@
 }]
 
 # Locate system_message.txt using the absolute path
 # for the directory where this file is located ("here"):
 here = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(here, 'system_message.txt'), 'r') as f:
     system_message = f.read().strip()
-with open(os.path.join(here, 'experimental_system_message.txt'), 'r') as f:
-    experimental_system_message = f.read().strip()
 
 class Interpreter:
     def __init__(self):
         self.messages = []
         self._logs = []
         self.system_message = system_message
-        self.experimental_system_message = experimental_system_message
         self.temperature = 0.2
         self.api_key = None
         self.max_output_chars = 2000
 
     def reset(self):
         self.messages = []
         self._logs = []
```

### Comparing `open_interpreter-0.0.231/interpreter/json_utils.py` & `open_interpreter-0.0.232/interpreter/json_utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.231/interpreter/openai_utils.py` & `open_interpreter-0.0.232/interpreter/openai_utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.231/interpreter/system_message.txt` & `open_interpreter-0.0.232/interpreter/system_message.txt`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.231/interpreter/system_message_experimental.txt` & `open_interpreter-0.0.232/interpreter/system_message_scratch_sheet.txt`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.231/interpreter/view.py` & `open_interpreter-0.0.232/interpreter/view.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.231/pyproject.toml` & `open_interpreter-0.0.232/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "open-interpreter"
 packages = [
     {include = "interpreter"}
 ]
-version = "0.0.231"
+version = "0.0.232"
 description = "Ask GPT-4 to run code locally."
 authors = ["Killian Lucas <killian@drinkwater.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 openai = "^0.27.8"
```

### Comparing `open_interpreter-0.0.231/PKG-INFO` & `open_interpreter-0.0.232/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-interpreter
-Version: 0.0.231
+Version: 0.0.232
 Summary: Ask GPT-4 to run code locally.
 Author: Killian Lucas
 Author-email: killian@drinkwater.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: open-interpreter Version: 0.0.231 Summary: Ask GPT-
+Metadata-Version: 2.1 Name: open-interpreter Version: 0.0.232 Summary: Ask GPT-
 4 to run code locally. Author: Killian Lucas Author-email:
 killian@drinkwater.ai Requires-Python: >=3.10,<4.0 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: astor
 (>=0.8.1,<0.9.0) Requires-Dist: ipython (>=8.14.0,<9.0.0) Requires-Dist: openai
 (>=0.27.8,<0.28.0) Requires-Dist: rich (>=13.4.2,<14.0.0) Requires-Dist:
 tiktoken (>=0.4.0,<0.5.0) Description-Content-Type: text/markdown # Open
```

