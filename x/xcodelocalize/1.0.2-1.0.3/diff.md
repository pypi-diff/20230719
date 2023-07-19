# Comparing `tmp/xcodelocalize-1.0.2.tar.gz` & `tmp/xcodelocalize-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcodelocalize-1.0.2.tar", max compression
+gzip compressed data, was "xcodelocalize-1.0.3.tar", max compression
```

## Comparing `xcodelocalize-1.0.2.tar` & `xcodelocalize-1.0.3.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1068 2023-02-04 04:42:01.815868 xcodelocalize-1.0.2/LICENSE
--rw-r--r--   0        0        0     3307 2023-02-22 22:01:01.463363 xcodelocalize-1.0.2/README.md
--rw-r--r--   0        0        0      744 2023-02-22 22:05:05.639564 xcodelocalize-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      795 2023-02-22 21:52:15.193396 xcodelocalize-1.0.2/src/xcodelocalize/Settings.py
--rw-r--r--   0        0        0     2047 2023-02-22 21:57:23.927386 xcodelocalize-1.0.2/src/xcodelocalize/Strings.py
--rw-r--r--   0        0        0      703 2023-02-04 04:42:01.815868 xcodelocalize-1.0.2/src/xcodelocalize/Translator.py
--rw-r--r--   0        0        0        0 2023-02-04 04:42:01.815868 xcodelocalize-1.0.2/src/xcodelocalize/__init__.py
--rw-r--r--   0        0        0       28 2023-02-04 04:42:01.815868 xcodelocalize-1.0.2/src/xcodelocalize/__main__.py
--rw-r--r--   0        0        0     5836 2023-02-22 22:04:38.625917 xcodelocalize-1.0.2/src/xcodelocalize/main.py
--rw-r--r--   0        0        0     4319 1970-01-01 00:00:00.000000 xcodelocalize-1.0.2/setup.py
--rw-r--r--   0        0        0     4172 1970-01-01 00:00:00.000000 xcodelocalize-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-19 14:09:46.068356 xcodelocalize-1.0.3/LICENSE
+-rw-r--r--   0        0        0     3307 2023-07-19 14:09:46.068356 xcodelocalize-1.0.3/README.md
+-rw-r--r--   0        0        0      744 2023-07-19 14:10:05.692673 xcodelocalize-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      795 2023-07-19 14:09:46.068356 xcodelocalize-1.0.3/src/xcodelocalize/Settings.py
+-rw-r--r--   0        0        0     2048 2023-07-19 14:09:46.072356 xcodelocalize-1.0.3/src/xcodelocalize/Strings.py
+-rw-r--r--   0        0        0      703 2023-07-19 14:09:46.072356 xcodelocalize-1.0.3/src/xcodelocalize/Translator.py
+-rw-r--r--   0        0        0        0 2023-07-19 14:09:46.072356 xcodelocalize-1.0.3/src/xcodelocalize/__init__.py
+-rw-r--r--   0        0        0       28 2023-07-19 14:09:46.072356 xcodelocalize-1.0.3/src/xcodelocalize/__main__.py
+-rw-r--r--   0        0        0     5836 2023-07-19 14:09:46.072356 xcodelocalize-1.0.3/src/xcodelocalize/main.py
+-rw-r--r--   0        0        0     4172 1970-01-01 00:00:00.000000 xcodelocalize-1.0.3/PKG-INFO
```

### Comparing `xcodelocalize-1.0.2/LICENSE` & `xcodelocalize-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xcodelocalize-1.0.2/README.md` & `xcodelocalize-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `xcodelocalize-1.0.2/pyproject.toml` & `xcodelocalize-1.0.3/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "xcodelocalize"
-version = "1.0.2"
+version = "1.0.3"
 description = "Tool for automatic search and localization of .strings files"
 authors = ["MarkParker5 <markparker.it@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://pypi.org/project/xcodelocalize/"
 repository = "https://github.com/MarkParker5/XCodeLocalize"
-documentation = "https://github.com/MarkParker5/XCodeLocalize/blob/main/readme.md"
+documentation = "https://github.com/MarkParker5/XCodeLocalize/blob/main/README.md"
 keywords = ["xcode", "localize", "strings", "localization", "ios"]
 
 [tool.poetry.scripts]
 xcodelocalize = "xcodelocalize.main:run"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `xcodelocalize-1.0.2/src/xcodelocalize/Settings.py` & `xcodelocalize-1.0.3/src/xcodelocalize/Settings.py`

 * *Files identical despite different names*

### Comparing `xcodelocalize-1.0.2/src/xcodelocalize/Strings.py` & `xcodelocalize-1.0.3/src/xcodelocalize/Strings.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         else:
             return f'<StringsFile []>'
 
     def read(self):
         with open(self.path, 'r') as f:
             file = f.read().replace('%@', '_ARG_')
 
-            pattern = re.compile(r'(\/\*(?P<comment>[\s\S]*?)\*\/)?[\s]+"(?P<key>[^"]+)"\s?=\s?"(?P<value>[^"]+)";')
+            pattern = re.compile(r'(\/\*(?P<comment>[\s\S]*?)\*\/)?[\s]*"(?P<key>[^"]+)"\s?=\s?"(?P<value>[^"]+)";')
 
             for match in pattern.finditer(file):
                 groups = match.groupdict()
 
                 if not all([groups.get('value'), groups.get('key')]):
                     continue
 
@@ -68,8 +68,8 @@
             for string in sorted(self.strings.values(), key = lambda s: s.key):
                 comment = f'/* {string.comment} */\n' if string.comment else ''
                 value = string.value.replace('"', '”')
                 f.write(
                     f'\n{comment}"{string.key}" = "{value}";\n' \
                         .replace('_ARG_', '%@') \
                         .replace('$ {','${')
-                )
+                )
```

### Comparing `xcodelocalize-1.0.2/src/xcodelocalize/Translator.py` & `xcodelocalize-1.0.3/src/xcodelocalize/Translator.py`

 * *Files identical despite different names*

### Comparing `xcodelocalize-1.0.2/src/xcodelocalize/main.py` & `xcodelocalize-1.0.3/src/xcodelocalize/main.py`

 * *Files identical despite different names*

### Comparing `xcodelocalize-1.0.2/PKG-INFO` & `xcodelocalize-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: xcodelocalize
-Version: 1.0.2
+Version: 1.0.3
 Summary: Tool for automatic search and localization of .strings files
 Home-page: https://pypi.org/project/xcodelocalize/
 License: MIT
 Keywords: xcode,localize,strings,localization,ios
 Author: MarkParker5
 Author-email: markparker.it@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: mtranslate (>=1.8,<2.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
-Project-URL: Documentation, https://github.com/MarkParker5/XCodeLocalize/blob/main/readme.md
+Project-URL: Documentation, https://github.com/MarkParker5/XCodeLocalize/blob/main/README.md
 Project-URL: Repository, https://github.com/MarkParker5/XCodeLocalize
 Description-Content-Type: text/markdown
 
 # XCodeLocalize
 
 ## Requirments
```

