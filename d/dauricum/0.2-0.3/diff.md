# Comparing `tmp/dauricum-0.2.tar.gz` & `tmp/dauricum-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dauricum-0.2.tar", last modified: Fri Jul  7 16:53:05 2023, max compression
+gzip compressed data, was "dauricum-0.3.tar", last modified: Wed Jul 19 15:08:27 2023, max compression
```

## Comparing `dauricum-0.2.tar` & `dauricum-0.3.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 16:53:05.657614 dauricum-0.2/
--rw-rw-rw-   0        0        0     1668 2023-07-07 16:53:05.657614 dauricum-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1144 2023-07-07 16:46:05.000000 dauricum-0.2/README.md
--rw-rw-rw-   0        0        0      535 2023-07-07 16:52:38.000000 dauricum-0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-07 16:53:05.658613 dauricum-0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-07 16:53:05.637115 dauricum-0.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-07 16:53:05.643622 dauricum-0.2/src/dauricum/
--rw-rw-rw-   0        0        0     3317 2023-07-07 16:52:29.000000 dauricum-0.2/src/dauricum/__init__.py
--rw-rw-rw-   0        0        0     3218 2023-07-07 15:48:41.000000 dauricum-0.2/src/dauricum/__main__.py
--rw-rw-rw-   0        0        0     1046 2023-07-07 15:13:01.000000 dauricum-0.2/src/dauricum/logger.py
-drwxrwxrwx   0        0        0        0 2023-07-07 16:53:05.656615 dauricum-0.2/src/dauricum/transformers/
--rw-rw-rw-   0        0        0     5359 2023-07-07 15:09:19.000000 dauricum-0.2/src/dauricum/transformers/ControlFlowTransformer.py
--rw-rw-rw-   0        0        0      313 2023-07-06 20:06:24.000000 dauricum-0.2/src/dauricum/transformers/IfStatementTransformer.py
--rw-rw-rw-   0        0        0     6058 2023-07-07 15:50:07.000000 dauricum-0.2/src/dauricum/transformers/InOutlineTransformer.py
--rw-rw-rw-   0        0        0    18409 2023-07-07 15:31:39.000000 dauricum-0.2/src/dauricum/transformers/MBAExprTransformer.py
--rw-rw-rw-   0        0        0     1849 2023-07-07 13:21:14.000000 dauricum-0.2/src/dauricum/transformers/MemoryTransformer.py
--rw-rw-rw-   0        0        0     5165 2023-07-07 15:09:52.000000 dauricum-0.2/src/dauricum/transformers/TryCatchTransformer.py
--rw-rw-rw-   0        0        0     3728 2023-07-07 15:11:46.000000 dauricum-0.2/src/dauricum/transformers/TryNormalizerTransformer.py
--rw-rw-rw-   0        0        0        0 2023-07-07 13:55:08.000000 dauricum-0.2/src/dauricum/transformers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 16:53:05.647620 dauricum-0.2/src/dauricum.egg-info/
--rw-rw-rw-   0        0        0     1668 2023-07-07 16:53:05.000000 dauricum-0.2/src/dauricum.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      631 2023-07-07 16:53:05.000000 dauricum-0.2/src/dauricum.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 16:53:05.000000 dauricum-0.2/src/dauricum.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-07 16:53:05.000000 dauricum-0.2/src/dauricum.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-19 15:08:27.526213 dauricum-0.3/
+-rw-rw-rw-   0        0        0     1669 2023-07-19 15:08:27.526213 dauricum-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1145 2023-07-07 16:58:20.000000 dauricum-0.3/README.md
+-rw-rw-rw-   0        0        0      535 2023-07-19 15:07:34.000000 dauricum-0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-19 15:08:27.526213 dauricum-0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-19 15:08:27.497231 dauricum-0.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-19 15:08:27.503226 dauricum-0.3/src/dauricum/
+-rw-rw-rw-   0        0        0     3314 2023-07-19 15:07:49.000000 dauricum-0.3/src/dauricum/__init__.py
+-rw-rw-rw-   0        0        0     4071 2023-07-19 15:03:19.000000 dauricum-0.3/src/dauricum/__main__.py
+-rw-rw-rw-   0        0        0     1046 2023-07-07 15:13:01.000000 dauricum-0.3/src/dauricum/logger.py
+drwxrwxrwx   0        0        0        0 2023-07-19 15:08:27.524212 dauricum-0.3/src/dauricum/transformers/
+-rw-rw-rw-   0        0        0     5359 2023-07-07 15:09:19.000000 dauricum-0.3/src/dauricum/transformers/ControlFlowTransformer.py
+-rw-rw-rw-   0        0        0     6058 2023-07-07 15:50:07.000000 dauricum-0.3/src/dauricum/transformers/InOutlineTransformer.py
+-rw-rw-rw-   0        0        0    18409 2023-07-07 15:31:39.000000 dauricum-0.3/src/dauricum/transformers/MBAExprTransformer.py
+-rw-rw-rw-   0        0        0     1849 2023-07-07 13:21:14.000000 dauricum-0.3/src/dauricum/transformers/MemoryTransformer.py
+-rw-rw-rw-   0        0        0     2684 2023-07-16 09:22:58.000000 dauricum-0.3/src/dauricum/transformers/OpaqueTransformer.py
+-rw-rw-rw-   0        0        0    15070 2023-07-19 14:53:26.000000 dauricum-0.3/src/dauricum/transformers/RenamerTransformer.py
+-rw-rw-rw-   0        0        0     5165 2023-07-07 15:09:52.000000 dauricum-0.3/src/dauricum/transformers/TryCatchTransformer.py
+-rw-rw-rw-   0        0        0     3728 2023-07-07 15:11:46.000000 dauricum-0.3/src/dauricum/transformers/TryNormalizerTransformer.py
+-rw-rw-rw-   0        0        0        0 2023-07-07 13:55:08.000000 dauricum-0.3/src/dauricum/transformers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 15:08:27.509221 dauricum-0.3/src/dauricum.egg-info/
+-rw-rw-rw-   0        0        0     1669 2023-07-19 15:08:27.000000 dauricum-0.3/src/dauricum.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      674 2023-07-19 15:08:27.000000 dauricum-0.3/src/dauricum.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 15:08:27.000000 dauricum-0.3/src/dauricum.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-19 15:08:27.000000 dauricum-0.3/src/dauricum.egg-info/top_level.txt
```

### Comparing `dauricum-0.2/PKG-INFO` & `dauricum-0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: dauricum
-Version: 0.2
+Version: 0.3
 Summary: Python 3.10+ obfuscator with many obfuscation methods.
 Author-email: nighty1337 <mg938436@gmail.com>
 Project-URL: Homepage, https://github.com/Maxdsdsdsd/dauricum
 Project-URL: Bug Tracker, https://github.com/Maxdsdsdsd/dauricum/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
-<h1 align="center">daricum</h1>
+<h1 align="center">dauricum</h1>
 
 ![Commits](https://img.shields.io/github/commit-activity/m/Maxdsdsdsd/dauricum)
 ![Stars](https://img.shields.io/github/stars/Maxdsdsdsd/dauricum)
 
 *A work-in-progress Python 3.10+ obfuscator with many obfuscation methods.*
  
  This obfuscator is built on ast. Inspired by [jargonaut](https://github.com/mad-cat-lon/jargonaut/tree/master).
```

### Comparing `dauricum-0.2/README.md` & `dauricum-0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<h1 align="center">daricum</h1>
+<h1 align="center">dauricum</h1>
 
 ![Commits](https://img.shields.io/github/commit-activity/m/Maxdsdsdsd/dauricum)
 ![Stars](https://img.shields.io/github/stars/Maxdsdsdsd/dauricum)
 
 *A work-in-progress Python 3.10+ obfuscator with many obfuscation methods.*
  
  This obfuscator is built on ast. Inspired by [jargonaut](https://github.com/mad-cat-lon/jargonaut/tree/master).
```

### Comparing `dauricum-0.2/pyproject.toml` & `dauricum-0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dauricum"
-version = "0.2"
+version = "0.3"
 authors = [
   { name="nighty1337", email="mg938436@gmail.com" },
 ]
 description = "Python 3.10+ obfuscator with many obfuscation methods."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `dauricum-0.2/src/dauricum/__init__.py` & `dauricum-0.3/src/dauricum/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,27 +2,29 @@
 
 dauricum.
 
 Python 3.10+ obfuscator with many obfuscation methods.
 
 """
 
-__version__ = "0.2"
+__version__ = "0.3"
 __author__ = 'nighty1337'
 __credits__ = 'POP_JUMP_FORWARD_IF_FALSE'
 
 import ast
 
 from io import TextIOWrapper
 from dauricum.transformers import TryCatchTransformer
 from dauricum.transformers import TryNormalizerTransformer
 from dauricum.transformers import MemoryTransformer
 from dauricum.transformers import InOutlineTransformer
 from dauricum.transformers import ControlFlowTransformer
 from dauricum.transformers import MBAExprTransformer
+from dauricum.transformers import OpaqueTransformer
+from dauricum.transformers import RenamerTransformer
 from dauricum.logger import Logger
 
 class ObfuscatorSettings():
     def __init__(self):
         self.transformers = []
         self.logger_enabled = True
     def addTransformer(self, transformer):
@@ -69,30 +71,38 @@
         
         Try Normalizer Transformer
         
         @param iterations - Iterations (Default - 5)
         
         """
         self.addTransformer(TryNormalizerTransformer.TryNormalizierTransformer(iterations))
+    def Opaque(self, iterations: int):
+        """ 
+        
+        Opaque Transformer
+        
+        """
+        self.addTransformer(OpaqueTransformer.OpaqueTransformer(iterations))
+    def Renamer(self, mode: int):
+        """ 
+        
+        Renamer Transformer
+        
+        """
+        self.addTransformer(RenamerTransformer.RenamerTransformer(mode))
 
 class Obfuscator:
     def obfuscate(input_file: TextIOWrapper, out_file: TextIOWrapper, settings: ObfuscatorSettings):
         Logger.init(settings.logger_enabled)
         Logger.logger.name = __class__.__name__
         
         Logger.logger.info(f"Obfuscating \"{input_file.name}\" ")
         
         tree = ast.parse(input_file.read())
         
         for transformer in settings.transformers:
             transformer.setTree(tree)
+            Logger.logger.name = transformer.__class__.__name__
             
             tree = transformer.proceed()
         
-        # tree = MBAExprTransformer.MBAExprTransformer(tree, True).proceed()
-        # tree = InOutlineTransformer.InOutlineTransformer(tree).proceed()
-        # tree = ControlFlowTransformer.ControlFlowTransformer(tree).proceed()
-        # tree = TryCatchTransformer.TryCatchTransformer(tree, True, 3).proceed() # Default - 1; Medium - 3; Hard - 5
-        # tree = TryNormalizerTransformer.TryNormalizierTransformer(tree, 5).proceed() # Default - 5
-        #tree = MemoryTransformer.MemoryTransformer(tree).proceed() # Unused currently
-        
         out_file.write(ast.unparse(tree))
```

### Comparing `dauricum-0.2/src/dauricum/__main__.py` & `dauricum-0.3/src/dauricum/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -70,34 +70,62 @@
     )
     parser.add_argument(
         "--try-normalizer-iter",
         type=int,
         default=1,
         help="Count of ... in one try-catch block"
     )
+    parser.add_argument(
+        "--opaque",
+        action='store_true',
+        help="Enables Opaque Tranformer"
+    )
+    parser.add_argument(
+        "--opaque-iter",
+        type=int,
+        default=1,
+        help="Count of iterations"
+    )
+    parser.add_argument(
+        "--rename",
+        action='store_true',
+        help="Enables Renamer Tranformer"
+    )
+    parser.add_argument(
+        "--rename-mode",
+        type=int,
+        default=0,
+        help="Change Renamer mode (0 - random sequence of 32 characters, 1 - random misleading word, 2 - random sequence of 64 characters, 3 - random word of misleading characters)"
+    )
     
     args = parser.parse_args()
     return args
 
 def main():
     args = handle_args()
     
     if (args.input == None or args.output == None):
         raise ValueError("Input or Output file is not specified!")
     
-    input, output = open(args.input, "r"), open(args.output, "w")
+    input, output = open(args.input, "r", encoding="utf-8"), open(args.output, "w", encoding="utf-8")
     
     settings = ObfuscatorSettings()
     settings.setLoggerEnabled(args.logging)
     
     if (args.mba_expression):
         settings.MBAExpression(args.mba_expression_mode)
         
+    if (args.rename):
+        settings.Renamer(args.rename_mode)
+        
     if (args.in_outline):
         settings.InOutline()
+    
+    if (args.opaque):
+        settings.Opaque(args.opaque_iter)
         
     if (args.control_flow):
         settings.ControlFlow()
     
     if (args.try_catch):
         settings.TryCatch(args.try_catch_mode, args.try_catch_iter)
```

### Comparing `dauricum-0.2/src/dauricum/logger.py` & `dauricum-0.3/src/dauricum/logger.py`

 * *Files identical despite different names*

### Comparing `dauricum-0.2/src/dauricum/transformers/ControlFlowTransformer.py` & `dauricum-0.3/src/dauricum/transformers/ControlFlowTransformer.py`

 * *Files identical despite different names*

### Comparing `dauricum-0.2/src/dauricum/transformers/InOutlineTransformer.py` & `dauricum-0.3/src/dauricum/transformers/InOutlineTransformer.py`

 * *Files identical despite different names*

### Comparing `dauricum-0.2/src/dauricum/transformers/MBAExprTransformer.py` & `dauricum-0.3/src/dauricum/transformers/MBAExprTransformer.py`

 * *Files identical despite different names*

### Comparing `dauricum-0.2/src/dauricum/transformers/MemoryTransformer.py` & `dauricum-0.3/src/dauricum/transformers/MemoryTransformer.py`

 * *Files identical despite different names*

### Comparing `dauricum-0.2/src/dauricum/transformers/TryCatchTransformer.py` & `dauricum-0.3/src/dauricum/transformers/TryCatchTransformer.py`

 * *Files identical despite different names*

### Comparing `dauricum-0.2/src/dauricum/transformers/TryNormalizerTransformer.py` & `dauricum-0.3/src/dauricum/transformers/TryNormalizerTransformer.py`

 * *Files identical despite different names*

### Comparing `dauricum-0.2/src/dauricum.egg-info/PKG-INFO` & `dauricum-0.3/src/dauricum.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: dauricum
-Version: 0.2
+Version: 0.3
 Summary: Python 3.10+ obfuscator with many obfuscation methods.
 Author-email: nighty1337 <mg938436@gmail.com>
 Project-URL: Homepage, https://github.com/Maxdsdsdsd/dauricum
 Project-URL: Bug Tracker, https://github.com/Maxdsdsdsd/dauricum/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
-<h1 align="center">daricum</h1>
+<h1 align="center">dauricum</h1>
 
 ![Commits](https://img.shields.io/github/commit-activity/m/Maxdsdsdsd/dauricum)
 ![Stars](https://img.shields.io/github/stars/Maxdsdsdsd/dauricum)
 
 *A work-in-progress Python 3.10+ obfuscator with many obfuscation methods.*
  
  This obfuscator is built on ast. Inspired by [jargonaut](https://github.com/mad-cat-lon/jargonaut/tree/master).
```

### Comparing `dauricum-0.2/src/dauricum.egg-info/SOURCES.txt` & `dauricum-0.3/src/dauricum.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 src/dauricum/__main__.py
 src/dauricum/logger.py
 src/dauricum.egg-info/PKG-INFO
 src/dauricum.egg-info/SOURCES.txt
 src/dauricum.egg-info/dependency_links.txt
 src/dauricum.egg-info/top_level.txt
 src/dauricum/transformers/ControlFlowTransformer.py
-src/dauricum/transformers/IfStatementTransformer.py
 src/dauricum/transformers/InOutlineTransformer.py
 src/dauricum/transformers/MBAExprTransformer.py
 src/dauricum/transformers/MemoryTransformer.py
+src/dauricum/transformers/OpaqueTransformer.py
+src/dauricum/transformers/RenamerTransformer.py
 src/dauricum/transformers/TryCatchTransformer.py
 src/dauricum/transformers/TryNormalizerTransformer.py
 src/dauricum/transformers/__init__.py
```

