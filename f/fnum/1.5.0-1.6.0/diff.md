# Comparing `tmp/fnum-1.5.0-py3-none-any.whl.zip` & `tmp/fnum-1.6.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 6859 bytes, number of entries: 12
--rw-r--r--  2.0 unx      626 b- defN 23-Jul-11 03:55 fnum/__init__.py
--rw-r--r--  2.0 unx       29 b- defN 23-Jul-11 03:55 fnum/__main__.py
--rw-r--r--  2.0 unx     7196 b- defN 23-Jul-11 03:55 fnum/_orchestrator.py
--rw-r--r--  2.0 unx     2464 b- defN 23-Jul-11 03:55 fnum/cli.py
--rw-r--r--  2.0 unx       41 b- defN 23-Jul-11 03:55 fnum/exceptions.py
--rw-r--r--  2.0 unx     2116 b- defN 23-Jul-11 03:55 fnum/metadata.py
--rw-r--r--  2.0 unx     1069 b- defN 23-Jul-11 03:55 fnum-1.5.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1038 b- defN 23-Jul-11 03:55 fnum-1.5.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-11 03:55 fnum-1.5.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       38 b- defN 23-Jul-11 03:55 fnum-1.5.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 23-Jul-11 03:55 fnum-1.5.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      897 b- defN 23-Jul-11 03:55 fnum-1.5.0.dist-info/RECORD
-12 files, 15611 bytes uncompressed, 5367 bytes compressed:  65.6%
+Zip file size: 7037 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      626 b- defN 23-Jul-19 03:52 fnum/__init__.py
+-rw-r--r--  2.0 unx       29 b- defN 23-Jul-19 03:52 fnum/__main__.py
+-rw-r--r--  2.0 unx     7650 b- defN 23-Jul-19 03:52 fnum/_orchestrator.py
+-rw-r--r--  2.0 unx     2568 b- defN 23-Jul-19 03:52 fnum/cli.py
+-rw-r--r--  2.0 unx       41 b- defN 23-Jul-19 03:52 fnum/exceptions.py
+-rw-r--r--  2.0 unx     2116 b- defN 23-Jul-19 03:52 fnum/metadata.py
+-rw-r--r--  2.0 unx     1069 b- defN 23-Jul-19 03:52 fnum-1.6.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1038 b- defN 23-Jul-19 03:52 fnum-1.6.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-19 03:52 fnum-1.6.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       38 b- defN 23-Jul-19 03:52 fnum-1.6.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 23-Jul-19 03:52 fnum-1.6.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      897 b- defN 23-Jul-19 03:52 fnum-1.6.0.dist-info/RECORD
+12 files, 16169 bytes uncompressed, 5545 bytes compressed:  65.7%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: fnum/exceptions.py
 Comment: 
 
 Filename: fnum/metadata.py
 Comment: 
 
-Filename: fnum-1.5.0.dist-info/LICENSE
+Filename: fnum-1.6.0.dist-info/LICENSE
 Comment: 
 
-Filename: fnum-1.5.0.dist-info/METADATA
+Filename: fnum-1.6.0.dist-info/METADATA
 Comment: 
 
-Filename: fnum-1.5.0.dist-info/WHEEL
+Filename: fnum-1.6.0.dist-info/WHEEL
 Comment: 
 
-Filename: fnum-1.5.0.dist-info/entry_points.txt
+Filename: fnum-1.6.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: fnum-1.5.0.dist-info/top_level.txt
+Filename: fnum-1.6.0.dist-info/top_level.txt
 Comment: 
 
-Filename: fnum-1.5.0.dist-info/RECORD
+Filename: fnum-1.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fnum/__init__.py

```diff
@@ -1,14 +1,14 @@
 import logging
 
 from ._orchestrator import _NumberOrchestrator
 from .metadata import FnumMetadata, FnumMax
 
 
-__version__ = "1.5.0"
+__version__ = "1.6.0"
 
 _log = logging.getLogger(__name__)
 
 
 def number_files(
     dirpath, suffixes, write_metadata=False, write_max=False, include_imeta=False
 ):
```

## fnum/_orchestrator.py

```diff
@@ -1,7 +1,8 @@
+import logging
 from pathlib import Path
 from imeta import ImageMetadata
 
 from .exceptions import FnumException
 from .metadata import FnumMetadata
 
 
@@ -85,16 +86,21 @@
     regen_meta = False
 
     ordered_ranges = None
     ordered_files = None
     unordered_ranges = None
     unordered_files = None
     new_files = None
+    removed_files = None
+
+    log = None
 
     def __init__(self, dirpath, suffixes, write_metadata, write_max, include_imeta):
+        self.log = logging.getLogger(__name__)
+
         self.dirpath = Path(dirpath)
         self.suffixes = suffixes
         self.write_metadata = write_metadata
         self.write_max = write_max
         self.include_imeta = include_imeta
 
         try:
@@ -105,16 +111,19 @@
                 self.regen_meta = True
 
     def numpath(self, suffix):
         return self.dirpath / (str(self.num) + suffix)
 
     def move_file(self, filepath):
         newpath = self.numpath(filepath.suffix)
+        self.log.debug(f"Renaming {filepath.name} to {newpath.name}")
         if newpath.exists():
-            raise FnumException(f"Can't override existing file {newpath.name}")
+            raise FnumException(
+                f"Can't override existing file {newpath.name} while renaming {filepath.name}"
+            )
 
         if self.metadata:
             try:
                 order_index = self.metadata.order.index(filepath.name)
                 self.metadata.order[order_index] = newpath.name
             except ValueError:
                 self.metadata.order.append(newpath.name)
@@ -154,14 +163,16 @@
 
     def find_movable(self):
         self.ordered_ranges = NumRanges()
         self.ordered_files = {}
         self.unordered_ranges = NumRanges()
         self.unordered_files = {}
         self.new_files = []
+        self.removed_files = []
+        self.log.debug(f"Numbering will start from {self.num}")
 
         # Find files in metadata file's order
         if self.metadata:
             for name in self.metadata.order:
                 filepath = self.dirpath / name
                 if filepath.exists():
                     try:
@@ -169,24 +180,16 @@
                         if num >= self.num:
                             self.ordered_ranges += num
                             self.ordered_files[num] = filepath
                     except ValueError:
                         self.new_files.append(filepath)
                     continue
 
-                try:
-                    self.metadata.order.remove(name)
-                except ValueError:
-                    pass
-                try:
-                    original_index = tuple(self.metadata.originals.values()).index(name)
-                    original_key = tuple(self.metadata.originals.keys())[original_index]
-                    del self.metadata.originals[original_key]
-                except ValueError:
-                    pass
+                self.log.debug(f"Missing {name}, removing from metadata")
+                self.removed_files.append(name)
 
         for filepath in self.dirpath.iterdir():
             if not filepath.is_file() or filepath.suffix not in self.suffixes:
                 continue
 
             try:
                 num = int(filepath.stem)
@@ -207,12 +210,24 @@
         for filepath in self.new_files:
             self.move_file(filepath)
 
     def maybe_write_metadata(self):
         if not self.metadata:
             return
 
+        for name in self.removed_files:
+            try:
+                self.metadata.order.remove(name)
+            except ValueError:
+                pass
+            try:
+                original_index = tuple(self.metadata.originals.values()).index(name)
+                original_key = tuple(self.metadata.originals.keys())[original_index]
+                del self.metadata.originals[original_key]
+            except ValueError:
+                pass
+
         self.metadata.max = self.num - 1
         if self.write_max:
             self.metadata.get_max().to_file(self.dirpath)
         if self.write_metadata:
             self.metadata.to_file(self.dirpath)
```

## fnum/cli.py

```diff
@@ -48,21 +48,26 @@
 @click.option(
     "--include-imeta/--no-include-imeta",
     default=False,
     help="""
 Also rename image metadata files generated by imeta.
     """,
 )
+@click.option(
+    "-v",
+    "--verbose",
+    count=True,
+)
 def cli(**kwargs):
     dirpath = kwargs["dirpath"]
     if "/" in kwargs["suffixes"]:
         click.echo("Suffixes contains a '/', did you mean ','?", err=True)
     suffixes = kwargs["suffixes"].split(",")
 
-    _log.setLevel(logging.INFO)
+    _log.setLevel(logging.DEBUG if kwargs["verbose"] > 0 else logging.INFO)
     handler = logging.StreamHandler(io.StringIO())
     handler.setFormatter(_ClickFormatter())
     _log.addHandler(handler)
 
     try:
         try:
             number_files(
```

## Comparing `fnum-1.5.0.dist-info/LICENSE` & `fnum-1.6.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fnum-1.5.0.dist-info/METADATA` & `fnum-1.6.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnum
-Version: 1.5.0
+Version: 1.6.0
 Summary: Renames files in a directory using sequential integers
 Author-email: Matt Wisniewski <healthycrowd@mattw.life>
 License: MIT
 Project-URL: homepage, https://github.com/healthycrowd/fnum
 Keywords: fnum,cli,utility,file,rename,sequential,order
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

