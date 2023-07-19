# Comparing `tmp/markdown_toc_creator-0.0.1.tar.gz` & `tmp/markdown_toc_creator-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown_toc_creator-0.0.1.tar", last modified: Wed Jul 19 09:36:19 2023, max compression
+gzip compressed data, was "markdown_toc_creator-0.0.2.tar", last modified: Wed Jul 19 09:55:04 2023, max compression
```

## Comparing `markdown_toc_creator-0.0.1.tar` & `markdown_toc_creator-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:36:19.563776 markdown_toc_creator-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-19 09:36:08.000000 markdown_toc_creator-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-19 09:36:19.563776 markdown_toc_creator-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-19 09:36:08.000000 markdown_toc_creator-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:36:19.563776 markdown_toc_creator-0.0.1/markdown_toc_creator/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-19 09:36:08.000000 markdown_toc_creator-0.0.1/markdown_toc_creator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-07-19 09:36:08.000000 markdown_toc_creator-0.0.1/markdown_toc_creator/create_toc.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-19 09:36:08.000000 markdown_toc_creator-0.0.1/markdown_toc_creator/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-07-19 09:36:08.000000 markdown_toc_creator-0.0.1/markdown_toc_creator/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-19 09:36:08.000000 markdown_toc_creator-0.0.1/markdown_toc_creator/toc_entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:36:19.563776 markdown_toc_creator-0.0.1/markdown_toc_creator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-19 09:36:19.000000 markdown_toc_creator-0.0.1/markdown_toc_creator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-19 09:36:19.000000 markdown_toc_creator-0.0.1/markdown_toc_creator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 09:36:19.000000 markdown_toc_creator-0.0.1/markdown_toc_creator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-19 09:36:19.000000 markdown_toc_creator-0.0.1/markdown_toc_creator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-19 09:36:19.000000 markdown_toc_creator-0.0.1/markdown_toc_creator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-19 09:36:19.000000 markdown_toc_creator-0.0.1/markdown_toc_creator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-19 09:36:19.563776 markdown_toc_creator-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-19 09:36:08.000000 markdown_toc_creator-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:36:19.563776 markdown_toc_creator-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-19 09:36:08.000000 markdown_toc_creator-0.0.1/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:55:04.585655 markdown_toc_creator-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-19 09:54:50.000000 markdown_toc_creator-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-19 09:55:04.585655 markdown_toc_creator-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-19 09:54:50.000000 markdown_toc_creator-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:55:04.585655 markdown_toc_creator-0.0.2/markdown_toc_creator/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-19 09:54:50.000000 markdown_toc_creator-0.0.2/markdown_toc_creator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-07-19 09:54:50.000000 markdown_toc_creator-0.0.2/markdown_toc_creator/create_toc.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-19 09:54:50.000000 markdown_toc_creator-0.0.2/markdown_toc_creator/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-07-19 09:54:50.000000 markdown_toc_creator-0.0.2/markdown_toc_creator/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-19 09:54:50.000000 markdown_toc_creator-0.0.2/markdown_toc_creator/toc_entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:55:04.585655 markdown_toc_creator-0.0.2/markdown_toc_creator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-19 09:55:04.000000 markdown_toc_creator-0.0.2/markdown_toc_creator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-19 09:55:04.000000 markdown_toc_creator-0.0.2/markdown_toc_creator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 09:55:04.000000 markdown_toc_creator-0.0.2/markdown_toc_creator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-19 09:55:04.000000 markdown_toc_creator-0.0.2/markdown_toc_creator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-19 09:55:04.000000 markdown_toc_creator-0.0.2/markdown_toc_creator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-19 09:55:04.000000 markdown_toc_creator-0.0.2/markdown_toc_creator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-19 09:55:04.585655 markdown_toc_creator-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-19 09:54:50.000000 markdown_toc_creator-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:55:04.585655 markdown_toc_creator-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-07-19 09:54:50.000000 markdown_toc_creator-0.0.2/tests/test_main.py
```

### Comparing `markdown_toc_creator-0.0.1/LICENSE` & `markdown_toc_creator-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `markdown_toc_creator-0.0.1/PKG-INFO` & `markdown_toc_creator-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdown_toc_creator
-Version: 0.0.1
+Version: 0.0.2
 Summary: Create table of contents for markdown files
 Home-page: https://github.com/jsh9/markdown-toc-creator
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
```

### Comparing `markdown_toc_creator-0.0.1/README.md` & `markdown_toc_creator-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `markdown_toc_creator-0.0.1/markdown_toc_creator/create_toc.py` & `markdown_toc_creator-0.0.2/markdown_toc_creator/create_toc.py`

 * *Files identical despite different names*

### Comparing `markdown_toc_creator-0.0.1/markdown_toc_creator/main.py` & `markdown_toc_creator-0.0.2/markdown_toc_creator/main.py`

 * *Files identical despite different names*

### Comparing `markdown_toc_creator-0.0.1/markdown_toc_creator/toc_entry.py` & `markdown_toc_creator-0.0.2/markdown_toc_creator/toc_entry.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,17 +13,20 @@
             style: str,
     ) -> None:
         self.displayText = displayText
         self.indent = indent
         self.style = style
         self.anchorLinkText: str = self._calcAnchorLinkText()
 
+    def render(self) -> str:
+        text = self.removePoundChar(self.displayText)
+        return self.indent + f'- [{text}]({self.anchorLinkText})'
+
     def _calcAnchorLinkText(self) -> str:
-        # remove '#' characters from the start of the header
-        text = re.sub(r'^#+\s', '', self.displayText)
+        text = self.removePoundChar(self.displayText)
 
         # remove HTML tags
         soup = BeautifulSoup(text, 'html.parser')
         text = soup.get_text()
 
         if self.style == 'gitlab':
             # remove emojis represented as :emoji_name:
@@ -37,16 +40,18 @@
 
         # check last character
         anchorLink = anchorLink[:-1] if anchorLink[-1] == '-' else anchorLink
 
         # prepend '#' to create a URL anchor
         return '#' + anchorLink
 
-    def render(self) -> str:
-        return self.indent + f'- [{self.displayText}]({self.anchorLinkText})'
+    @classmethod
+    def removePoundChar(cls, string: str) -> str:
+        # remove '#' characters from the start of the header
+        return re.sub(r'^#+\s', '', string)
 
 
 def deduplicateAnchorLinkText(tocEntries: List[TocEntry]) -> None:
     allAnchorLinkTexts: List[str] = [_.anchorLinkText for _ in tocEntries]
 
     seen: Set[str] = set()
     duplicated: Set[str] = set()
```

### Comparing `markdown_toc_creator-0.0.1/markdown_toc_creator.egg-info/PKG-INFO` & `markdown_toc_creator-0.0.2/markdown_toc_creator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdown-toc-creator
-Version: 0.0.1
+Version: 0.0.2
 Summary: Create table of contents for markdown files
 Home-page: https://github.com/jsh9/markdown-toc-creator
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
```

### Comparing `markdown_toc_creator-0.0.1/setup.cfg` & `markdown_toc_creator-0.0.2/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = markdown_toc_creator
-version = 0.0.1
+version = 0.0.2
 description = Create table of contents for markdown files
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jsh9/markdown-toc-creator
 license = MIT
 license_file = LICENSE
 classifiers =
```

### Comparing `markdown_toc_creator-0.0.1/tests/test_main.py` & `markdown_toc_creator-0.0.2/tests/test_main.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,28 +18,28 @@
         skip_first_n_lines=3,
         quiet=False,
         in_place=False,
         style=style,
     )
     expected = {
         'github': [
-            '- [# This header has spaces in it](#this-header-has-spaces-in-it)',
-            '  - [## This header has a :thumbsup: in it](#this-header-has-a-thumbsup-in-it)',
-            '- [# This header has Unicode in it: 中文](#this-header-has-unicode-in-it-中文)',
-            '  - [## This header has spaces in it](#this-header-has-spaces-in-it-1)',
-            '    - [### This header has spaces in it](#this-header-has-spaces-in-it-2)',
-            '  - [## This header has 3.5 in it (and parentheses)](#this-header-has-35-in-it-and-parentheses)',
-            "    - [### What day is today? I don't know.](#what-day-is-today-i-dont-know)",
-            '  - [## This header has     consecutive spaces in it](#this-header-has-----consecutive-spaces-in-it)',
+            '- [This header has spaces in it](#this-header-has-spaces-in-it)',
+            '  - [This header has a :thumbsup: in it](#this-header-has-a-thumbsup-in-it)',
+            '- [This header has Unicode in it: 中文](#this-header-has-unicode-in-it-中文)',
+            '  - [This header has spaces in it](#this-header-has-spaces-in-it-1)',
+            '    - [This header has spaces in it](#this-header-has-spaces-in-it-2)',
+            '  - [This header has 3.5 in it (and parentheses)](#this-header-has-35-in-it-and-parentheses)',
+            "    - [What day is today? I don't know.](#what-day-is-today-i-dont-know)",
+            '  - [This header has     consecutive spaces in it](#this-header-has-----consecutive-spaces-in-it)',
         ],
         'gitlab': [
-            '- [# This header has spaces in it](#this-header-has-spaces-in-it)',
-            '  - [## This header has a :thumbsup: in it](#this-header-has-a-in-it)',
-            '- [# This header has Unicode in it: 中文](#this-header-has-unicode-in-it-中文)',
-            '  - [## This header has spaces in it](#this-header-has-spaces-in-it-1)',
-            '    - [### This header has spaces in it](#this-header-has-spaces-in-it-2)',
-            '  - [## This header has 3.5 in it (and parentheses)](#this-header-has-35-in-it-and-parentheses)',
-            "    - [### What day is today? I don't know.](#what-day-is-today-i-dont-know)",
-            '  - [## This header has     consecutive spaces in it](#this-header-has-consecutive-spaces-in-it)',
+            '- [This header has spaces in it](#this-header-has-spaces-in-it)',
+            '  - [This header has a :thumbsup: in it](#this-header-has-a-in-it)',
+            '- [This header has Unicode in it: 中文](#this-header-has-unicode-in-it-中文)',
+            '  - [This header has spaces in it](#this-header-has-spaces-in-it-1)',
+            '    - [This header has spaces in it](#this-header-has-spaces-in-it-2)',
+            '  - [This header has 3.5 in it (and parentheses)](#this-header-has-35-in-it-and-parentheses)',
+            "    - [What day is today? I don't know.](#what-day-is-today-i-dont-know)",
+            '  - [This header has     consecutive spaces in it](#this-header-has-consecutive-spaces-in-it)',
         ],
     }
     assert tocLines == expected[style]
```

