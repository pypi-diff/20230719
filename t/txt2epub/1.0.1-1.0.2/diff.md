# Comparing `tmp/txt2epub-1.0.1.tar.gz` & `tmp/txt2epub-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "txt2epub-1.0.1.tar", last modified: Wed Jul 19 15:45:09 2023, max compression
+gzip compressed data, was "txt2epub-1.0.2.tar", last modified: Wed Jul 19 16:02:05 2023, max compression
```

## Comparing `txt2epub-1.0.1.tar` & `txt2epub-1.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    18092 2023-07-19 14:27:40.732574 txt2epub-1.0.1/LICENSE
--rw-r--r--   0        0        0      274 2023-07-19 15:39:52.348107 txt2epub-1.0.1/README.md
--rw-r--r--   0        0        0      885 2023-07-19 15:45:09.836562 txt2epub-1.0.1/pyproject.toml
--rwxr-xr-x   0        0        0       97 2023-07-19 15:44:43.356412 txt2epub-1.0.1/txt2epub/__init__.py
--rwxr-xr-x   0        0        0     1419 2023-07-19 15:31:46.188789 txt2epub-1.0.1/txt2epub/__main__.py
--rwxr-xr-x   0        0        0     2387 2023-07-19 15:36:07.583530 txt2epub-1.0.1/txt2epub/txt2epub.py
--rwxr-xr-x   0        0        0     4037 2023-07-19 15:35:47.456753 txt2epub-1.0.1/txt2epub/txt2epub_gui.py
--rw-r--r--   0        0        0      924 1970-01-01 00:00:00.000000 txt2epub-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    18092 2023-07-19 14:27:40.732574 txt2epub-1.0.2/LICENSE
+-rw-r--r--   0        0        0      274 2023-07-19 15:39:52.348107 txt2epub-1.0.2/README.md
+-rw-r--r--   0        0        0      885 2023-07-19 16:02:05.942384 txt2epub-1.0.2/pyproject.toml
+-rwxr-xr-x   0        0        0       97 2023-07-19 16:01:36.392214 txt2epub-1.0.2/txt2epub/__init__.py
+-rwxr-xr-x   0        0        0     1419 2023-07-19 15:31:46.188789 txt2epub-1.0.2/txt2epub/__main__.py
+-rwxr-xr-x   0        0        0     2518 2023-07-19 16:00:20.205108 txt2epub-1.0.2/txt2epub/txt2epub.py
+-rwxr-xr-x   0        0        0     4256 2023-07-19 16:01:11.718738 txt2epub-1.0.2/txt2epub/txt2epub_gui.py
+-rw-r--r--   0        0        0      924 1970-01-01 00:00:00.000000 txt2epub-1.0.2/PKG-INFO
```

### Comparing `txt2epub-1.0.1/LICENSE` & `txt2epub-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `txt2epub-1.0.1/pyproject.toml` & `txt2epub-1.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ]
 dependencies = [
     "langdetect>=1.0.0",
     "ebooklib>=0.18",
     "PyQt6>=6.5.0",
 ]
 dynamic = []
-version = "1.0.1"
+version = "1.0.2"
 
 [project.license]
 text = "GPL-2.0-only"
 
 [project.urls]
 homepage = "https://github.com/k4yt3x/txt2epub/"
```

### Comparing `txt2epub-1.0.1/txt2epub/__main__.py` & `txt2epub-1.0.2/txt2epub/__main__.py`

 * *Files identical despite different names*

### Comparing `txt2epub-1.0.1/txt2epub/txt2epub.py` & `txt2epub-1.0.2/txt2epub/txt2epub.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,18 @@
     def create_epub(self, input_file: pathlib.Path, output_file: pathlib.Path = None):
         # get the book title from the file name
         book_title = self.book_title or input_file.stem
 
         # read text from file
         with input_file.open("r", encoding="utf-8") as txt_file:
             text = txt_file.read()
-            book_language = self.book_language or langdetect.detect(text)
+            try:
+                book_language = self.book_language or langdetect.detect(text)
+            except langdetect.lang_detect_exception.LangDetectException:
+                book_language = "en"
 
         # split text into chapters
         chapters = text.split("\n\n\n")
 
         # create new EPUB book
         book = epub.EpubBook()
```

### Comparing `txt2epub-1.0.1/txt2epub/txt2epub_gui.py` & `txt2epub-1.0.2/txt2epub/txt2epub_gui.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,20 +73,24 @@
     def select_file(self):
         file_path, _ = QFileDialog.getOpenFileName(
             self, "Select a text file", "", "Text Files (*.txt);;All Files (*)"
         )
         self.on_select(file_path)
 
     def on_select(self, file: str):
-        if file is not None:
+        file_path = pathlib.Path(file)
+        if file is not None and file_path.is_file():
             self.file_path = pathlib.Path(file)
             self.title_input.setText(self.file_path.stem)
             with self.file_path.open("r", encoding="utf-8") as txt_file:
                 text = txt_file.read()
-                self.language_input.setText(langdetect.detect(text))
+                try:
+                    self.language_input.setText(langdetect.detect(text))
+                except langdetect.lang_detect_exception.LangDetectException:
+                    self.language_input.setText("en")
             self.label.setText(f"Selected file: {self.file_path.name}")
 
     def generate_epub(self):
         if self.file_path:
             try:
                 creator = Txt2Epub(
                     book_title=self.title_input.text() or "Default Title",
```

### Comparing `txt2epub-1.0.1/PKG-INFO` & `txt2epub-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: txt2epub
-Version: 1.0.1
+Version: 1.0.2
 Summary: A simple TXT to ePub converter
 Keywords: ebook
 Home-page: https://github.com/k4yt3x/txt2epub/
 Author-Email: K4YT3X <i@k4yt3x.com>
 License: GPL-2.0-only
 Classifier: Environment :: Console
 Classifier: Environment :: X11 Applications :: Qt
```

