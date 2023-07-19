# Comparing `tmp/toRST-0.0.1.tar.gz` & `tmp/toRST-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toRST-0.0.1.tar", last modified: Tue Jul 18 20:25:56 2023, max compression
+gzip compressed data, was "toRST-0.0.2.tar", last modified: Wed Jul 19 01:19:18 2023, max compression
```

## Comparing `toRST-0.0.1.tar` & `toRST-0.0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-18 20:25:56.227449 toRST-0.0.1/
--rw-r--r--   0 jreyno     (501) staff       (20)     1085 2023-07-18 19:42:12.000000 toRST-0.0.1/LICENSE
--rw-r--r--   0 jreyno     (501) staff       (20)     1755 2023-07-18 20:25:56.227496 toRST-0.0.1/PKG-INFO
--rw-r--r--   0 jreyno     (501) staff       (20)      534 2023-07-18 19:55:00.000000 toRST-0.0.1/README.md
-drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-18 20:25:56.224684 toRST-0.0.1/csv2rst/
--rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.0.1/csv2rst/__init__.py
--rw-r--r--   0 jreyno     (501) staff       (20)      488 2023-07-18 16:07:34.000000 toRST-0.0.1/csv2rst/csv2rst.py
-drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-18 20:25:56.225470 toRST-0.0.1/funcs/
--rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.0.1/funcs/__init__.py
--rw-r--r--   0 jreyno     (501) staff       (20)     1179 2023-07-18 16:07:34.000000 toRST-0.0.1/funcs/command.py
--rw-r--r--   0 jreyno     (501) staff       (20)       76 2023-07-18 16:07:34.000000 toRST-0.0.1/funcs/funcs.py
-drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-18 20:25:56.225719 toRST-0.0.1/json2rst/
--rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.0.1/json2rst/__init__.py
--rw-r--r--   0 jreyno     (501) staff       (20)      385 2023-07-18 16:07:34.000000 toRST-0.0.1/json2rst/json2rst.py
--rw-r--r--   0 jreyno     (501) staff       (20)      103 2023-07-18 19:59:51.000000 toRST-0.0.1/pyproject.toml
--rw-r--r--   0 jreyno     (501) staff       (20)      678 2023-07-18 20:25:56.227717 toRST-0.0.1/setup.cfg
--rw-r--r--   0 jreyno     (501) staff       (20)      673 2023-07-18 20:19:19.000000 toRST-0.0.1/setup.py
-drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-18 20:25:56.225890 toRST-0.0.1/tests/
--rw-r--r--   0 jreyno     (501) staff       (20)      790 2023-07-18 16:07:34.000000 toRST-0.0.1/tests/test_toRST_toRST.py
-drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-18 20:25:56.226498 toRST-0.0.1/toRST/
--rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.0.1/toRST/__init__.py
--rw-r--r--   0 jreyno     (501) staff       (20)     2663 2023-07-18 20:10:44.000000 toRST-0.0.1/toRST/toRST.py
--rw-r--r--   0 jreyno     (501) staff       (20)      356 2023-07-18 19:42:12.000000 toRST-0.0.1/toRST/write.py
-drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-18 20:25:56.227326 toRST-0.0.1/toRST.egg-info/
--rw-r--r--   0 jreyno     (501) staff       (20)     1755 2023-07-18 20:25:56.000000 toRST-0.0.1/toRST.egg-info/PKG-INFO
--rw-r--r--   0 jreyno     (501) staff       (20)      404 2023-07-18 20:25:56.000000 toRST-0.0.1/toRST.egg-info/SOURCES.txt
--rw-r--r--   0 jreyno     (501) staff       (20)        1 2023-07-18 20:25:56.000000 toRST-0.0.1/toRST.egg-info/dependency_links.txt
--rw-r--r--   0 jreyno     (501) staff       (20)       44 2023-07-18 20:25:56.000000 toRST-0.0.1/toRST.egg-info/entry_points.txt
--rw-r--r--   0 jreyno     (501) staff       (20)       29 2023-07-18 20:25:56.000000 toRST-0.0.1/toRST.egg-info/top_level.txt
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-19 01:19:18.471189 toRST-0.0.2/
+-rw-r--r--   0 jreyno     (501) staff       (20)     1085 2023-07-18 19:42:12.000000 toRST-0.0.2/LICENSE
+-rw-r--r--   0 jreyno     (501) staff       (20)     1755 2023-07-19 01:19:18.471239 toRST-0.0.2/PKG-INFO
+-rw-r--r--   0 jreyno     (501) staff       (20)     1022 2023-07-19 00:45:51.000000 toRST-0.0.2/README.md
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-19 01:19:18.468325 toRST-0.0.2/csv2rst/
+-rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.0.2/csv2rst/__init__.py
+-rw-r--r--   0 jreyno     (501) staff       (20)      488 2023-07-18 16:07:34.000000 toRST-0.0.2/csv2rst/csv2rst.py
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-19 01:19:18.469151 toRST-0.0.2/funcs/
+-rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.0.2/funcs/__init__.py
+-rw-r--r--   0 jreyno     (501) staff       (20)     1179 2023-07-18 16:07:34.000000 toRST-0.0.2/funcs/command.py
+-rw-r--r--   0 jreyno     (501) staff       (20)       76 2023-07-18 16:07:34.000000 toRST-0.0.2/funcs/funcs.py
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-19 01:19:18.469519 toRST-0.0.2/json2rst/
+-rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.0.2/json2rst/__init__.py
+-rw-r--r--   0 jreyno     (501) staff       (20)      385 2023-07-18 16:07:34.000000 toRST-0.0.2/json2rst/json2rst.py
+-rw-r--r--   0 jreyno     (501) staff       (20)      103 2023-07-18 20:40:47.000000 toRST-0.0.2/pyproject.toml
+-rw-r--r--   0 jreyno     (501) staff       (20)      678 2023-07-19 01:19:18.471484 toRST-0.0.2/setup.cfg
+-rw-r--r--   0 jreyno     (501) staff       (20)      673 2023-07-19 01:14:05.000000 toRST-0.0.2/setup.py
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-19 01:19:18.469670 toRST-0.0.2/tests/
+-rw-r--r--   0 jreyno     (501) staff       (20)      790 2023-07-18 16:07:34.000000 toRST-0.0.2/tests/test_toRST_toRST.py
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-19 01:19:18.470213 toRST-0.0.2/toRST/
+-rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.0.2/toRST/__init__.py
+-rw-r--r--   0 jreyno     (501) staff       (20)     2994 2023-07-19 01:13:36.000000 toRST-0.0.2/toRST/toRST.py
+-rw-r--r--   0 jreyno     (501) staff       (20)      374 2023-07-19 00:58:12.000000 toRST-0.0.2/toRST/write.py
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-19 01:19:18.471071 toRST-0.0.2/toRST.egg-info/
+-rw-r--r--   0 jreyno     (501) staff       (20)     1755 2023-07-19 01:19:18.000000 toRST-0.0.2/toRST.egg-info/PKG-INFO
+-rw-r--r--   0 jreyno     (501) staff       (20)      404 2023-07-19 01:19:18.000000 toRST-0.0.2/toRST.egg-info/SOURCES.txt
+-rw-r--r--   0 jreyno     (501) staff       (20)        1 2023-07-19 01:19:18.000000 toRST-0.0.2/toRST.egg-info/dependency_links.txt
+-rw-r--r--   0 jreyno     (501) staff       (20)       44 2023-07-19 01:19:18.000000 toRST-0.0.2/toRST.egg-info/entry_points.txt
+-rw-r--r--   0 jreyno     (501) staff       (20)       29 2023-07-19 01:19:18.000000 toRST-0.0.2/toRST.egg-info/top_level.txt
```

### Comparing `toRST-0.0.1/LICENSE` & `toRST-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `toRST-0.0.1/PKG-INFO` & `toRST-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toRST
-Version: 0.0.1
+Version: 0.0.2
 Summary: Command line tool for converting CSV and JSON files into reStructuredText Tables.
 Home-page: https://github.com/jrey999/toRST
 Author: John Reynolds
 Author-email: reynoldsjohngreg@gmail.com
 License: The MIT License (MIT)
         Copyright © 2023 John Reynolds
```

### Comparing `toRST-0.0.1/funcs/command.py` & `toRST-0.0.2/funcs/command.py`

 * *Files identical despite different names*

### Comparing `toRST-0.0.1/setup.cfg` & `toRST-0.0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = torst
-version = 0.0.1
+version = 0.0.2
 author = John Reynolds
 author_email = reynoldsjohngreg@gmail.com
 description = Convert various data formats to reStructuredText tables.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jrey999/toRST
 project_urls =
```

### Comparing `toRST-0.0.1/setup.py` & `toRST-0.0.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Command line tool for converting CSV and JSON files into reStructuredText Tables.
 """.strip()
 
 with open('LICENSE') as f:
     license = f.read()
 setup(
     name='toRST',
-    version='0.0.1',
+    version='0.0.2',
     description='Command line tool for converting CSV and JSON files into reStructuredText Tables.',
     long_description=readme,
     author='John Reynolds',
     author_email='reynoldsjohngreg@gmail.com',
     url='https://github.com/jrey999/toRST',
     license=license,
     packages=find_packages(exclude=('tests',)),
```

### Comparing `toRST-0.0.1/tests/test_toRST_toRST.py` & `toRST-0.0.2/tests/test_toRST_toRST.py`

 * *Files identical despite different names*

### Comparing `toRST-0.0.1/toRST/toRST.py` & `toRST-0.0.2/toRST/toRST.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,31 +52,35 @@
 
         :returns: Dict with page formatting metadata
         :rtype: dict[str, int or str]
         """
         return {
             "num_columns": len(self.headers),
             "page_wdith": sum(self.column_widths.values()),
-            "new_line": "".join(["+" + column_width * "=" for column_width in self.column_widths.values()]) + "+"
+            "header": "".join(["+" + column_width * "=" for column_width in self.column_widths.values()]) + "+",
+            "new_line": "".join(["+" + column_width * "-" for column_width in self.column_widths.values()]) + "+"
         }
     
     def build_table(self) -> list[str]:
         
         """
         Construct the reST grid table.
 
         This iterates through the data rows, building each line 
         of the table with proper column widths and formatting.
 
         :returns: A list of table lines
         :rtype: list[str]
         """
-        table = []
-        for row in self.data:
+        table = [
+            self.page_info["header"],
+            "|" + ("|".join([str(cell) + " " * (self.column_widths[index] - len(str(cell))) for index, cell in enumerate(self.data[0])])) + "|",
+            self.page_info["header"]
+            ]
+        for row in self.data[1:]:
             
-            table += [self.page_info["new_line"]]
             rst_row=""
             for index, cell in enumerate(row):
                 column_width = self.column_widths[index]
                 rst_row += "|" + (str(cell) + " " * (column_width - len(str(cell))))
-            table += [rst_row + "|"]
+            table += [rst_row + "|"] + [self.page_info["new_line"]]
         return table + [self.page_info["new_line"]]
```

### Comparing `toRST-0.0.1/toRST.egg-info/PKG-INFO` & `toRST-0.0.2/toRST.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toRST
-Version: 0.0.1
+Version: 0.0.2
 Summary: Command line tool for converting CSV and JSON files into reStructuredText Tables.
 Home-page: https://github.com/jrey999/toRST
 Author: John Reynolds
 Author-email: reynoldsjohngreg@gmail.com
 License: The MIT License (MIT)
         Copyright © 2023 John Reynolds
```

