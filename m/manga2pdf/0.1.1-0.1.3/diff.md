# Comparing `tmp/manga2pdf-0.1.1.tar.gz` & `tmp/manga2pdf-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manga2pdf-0.1.1.tar", last modified: Tue Apr 25 05:46:46 2023, max compression
+gzip compressed data, was "manga2pdf-0.1.3.tar", last modified: Wed Jul 19 12:01:01 2023, max compression
```

## Comparing `manga2pdf-0.1.1.tar` & `manga2pdf-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 shun       (501) staff       (20)        0 2023-04-25 05:46:46.726258 manga2pdf-0.1.1/
--rw-r--r--   0 shun       (501) staff       (20)     1063 2023-03-12 05:13:58.000000 manga2pdf-0.1.1/LICENSE
--rw-r--r--   0 shun       (501) staff       (20)     5913 2023-04-25 05:46:46.726152 manga2pdf-0.1.1/PKG-INFO
--rw-r--r--   0 shun       (501) staff       (20)     5369 2023-04-15 20:09:50.000000 manga2pdf-0.1.1/README.md
--rw-r--r--   0 shun       (501) staff       (20)       38 2023-04-25 05:46:46.726286 manga2pdf-0.1.1/setup.cfg
--rw-r--r--   0 shun       (501) staff       (20)     1065 2023-04-22 06:44:25.000000 manga2pdf-0.1.1/setup.py
-drwxr-xr-x   0 shun       (501) staff       (20)        0 2023-04-25 05:46:46.725430 manga2pdf-0.1.1/src/
-drwxr-xr-x   0 shun       (501) staff       (20)        0 2023-04-25 05:46:46.726022 manga2pdf-0.1.1/src/manga2pdf.egg-info/
--rw-r--r--   0 shun       (501) staff       (20)     5913 2023-04-25 05:46:46.000000 manga2pdf-0.1.1/src/manga2pdf.egg-info/PKG-INFO
--rw-r--r--   0 shun       (501) staff       (20)      288 2023-04-25 05:46:46.000000 manga2pdf-0.1.1/src/manga2pdf.egg-info/SOURCES.txt
--rw-r--r--   0 shun       (501) staff       (20)        1 2023-04-25 05:46:46.000000 manga2pdf-0.1.1/src/manga2pdf.egg-info/dependency_links.txt
--rw-r--r--   0 shun       (501) staff       (20)       45 2023-04-25 05:46:46.000000 manga2pdf-0.1.1/src/manga2pdf.egg-info/entry_points.txt
--rw-r--r--   0 shun       (501) staff       (20)       52 2023-04-25 05:46:46.000000 manga2pdf-0.1.1/src/manga2pdf.egg-info/requires.txt
--rw-r--r--   0 shun       (501) staff       (20)       24 2023-04-25 05:46:46.000000 manga2pdf-0.1.1/src/manga2pdf.egg-info/top_level.txt
--rw-r--r--   0 shun       (501) staff       (20)    17683 2023-04-15 20:21:17.000000 manga2pdf-0.1.1/src/manga2pdf.py
--rw-r--r--   0 shun       (501) staff       (20)    18189 2023-04-15 20:21:57.000000 manga2pdf-0.1.1/src/manga2pdf_gui.py
+drwxr-xr-x   0 shun       (501) staff       (20)        0 2023-07-19 12:01:01.024741 manga2pdf-0.1.3/
+-rw-r--r--   0 shun       (501) staff       (20)     1063 2023-03-12 05:13:58.000000 manga2pdf-0.1.3/LICENSE
+-rw-r--r--   0 shun       (501) staff       (20)     6167 2023-07-19 12:01:01.024643 manga2pdf-0.1.3/PKG-INFO
+-rw-r--r--   0 shun       (501) staff       (20)     5623 2023-05-03 09:26:06.000000 manga2pdf-0.1.3/README.md
+-rw-r--r--   0 shun       (501) staff       (20)       38 2023-07-19 12:01:01.024778 manga2pdf-0.1.3/setup.cfg
+-rw-r--r--   0 shun       (501) staff       (20)     1065 2023-07-19 09:51:27.000000 manga2pdf-0.1.3/setup.py
+drwxr-xr-x   0 shun       (501) staff       (20)        0 2023-07-19 12:01:01.023934 manga2pdf-0.1.3/src/
+drwxr-xr-x   0 shun       (501) staff       (20)        0 2023-07-19 12:01:01.024519 manga2pdf-0.1.3/src/manga2pdf.egg-info/
+-rw-r--r--   0 shun       (501) staff       (20)     6167 2023-07-19 12:01:01.000000 manga2pdf-0.1.3/src/manga2pdf.egg-info/PKG-INFO
+-rw-r--r--   0 shun       (501) staff       (20)      288 2023-07-19 12:01:01.000000 manga2pdf-0.1.3/src/manga2pdf.egg-info/SOURCES.txt
+-rw-r--r--   0 shun       (501) staff       (20)        1 2023-07-19 12:01:01.000000 manga2pdf-0.1.3/src/manga2pdf.egg-info/dependency_links.txt
+-rw-r--r--   0 shun       (501) staff       (20)       45 2023-07-19 12:01:01.000000 manga2pdf-0.1.3/src/manga2pdf.egg-info/entry_points.txt
+-rw-r--r--   0 shun       (501) staff       (20)       52 2023-07-19 12:01:01.000000 manga2pdf-0.1.3/src/manga2pdf.egg-info/requires.txt
+-rw-r--r--   0 shun       (501) staff       (20)       24 2023-07-19 12:01:01.000000 manga2pdf-0.1.3/src/manga2pdf.egg-info/top_level.txt
+-rw-r--r--   0 shun       (501) staff       (20)    18928 2023-07-19 09:51:11.000000 manga2pdf-0.1.3/src/manga2pdf.py
+-rw-r--r--   0 shun       (501) staff       (20)    18123 2023-07-19 11:42:46.000000 manga2pdf-0.1.3/src/manga2pdf_gui.py
```

### Comparing `manga2pdf-0.1.1/LICENSE` & `manga2pdf-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `manga2pdf-0.1.1/PKG-INFO` & `manga2pdf-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manga2pdf
-Version: 0.1.1
+Version: 0.1.3
 Summary: Convert manga/comic files(zip, epub, etc.) or directory containing image files (jpg, png, etc.) to PDF.
 Home-page: https://github.com/mashu3/manga2pdf
 Author: mashu3
 License: MIT
 Keywords: manga comic pdf converter
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
@@ -31,22 +31,29 @@
 
 ## Usage
 This script can take input in the form of `zip`, `cbz`, `rar`, `cbr`, `epub` files or directories containing images (`jpg`, `jpeg`, `png`, `gif`, `bmp`) of manga or comic pages.
 
 The program can be executed from the command line with the following options:
 - The `input_path` argument represents the path to the input file. To execute the Python script correctly, specify the `input_path` argument as the path to the input file containing manga or comic images in any of the supported formats, such as `zip`, `cbz`, `rar`, `cbr`, `epub`, or a directory containing images in formats such as `jpg`, `jpeg`, `png`, `gif`, or `bmp`.
 - The `output_path` argument is the path to the output PDF file. To use the script, simply run the Python script with the path to the input file or directory as the argument. If the `--output` option is not specified, the output file name will be automatically generated based on the name of the input file or directory.
-- The `pagelayout` argument is the page layout of the PDF file. The `pagelayout` parameter can take in the following values:
+- The `pagelayout` parameter can take in the following values:
     - `SinglePage` -> Single page display
     - `OneColumn` -> Enable scrolling
     - `TwoPageLeft` -> Spread view
     - `TwoColumnLeft` -> Spread view with scrolling
     - (default) `TwoPageRight` -> Separate Cover, Spread View
     - `TwoColumnRight` -> Separate Cover, Scrolling Spread View
-- The `direction` argument is the reading direction of the PDF file. The `direction` parameter can take in the following values:
+- The `pagemode` parameter can take in the following values:
+    - (default) `UseNone` -> Neither document outline nor thumbnail images visible
+    - `UseOutlines` -> Document outline visible
+    - `UseThumbs` -> Thumbnail images visible
+    - `FullScreen` -> Full-screen mode
+    - `UseOC` -> Optional content group panel visible
+    - `UseAttachments` -> Attachments panel visible
+- The `direction` parameter can take in the following values:
     - `L2R` -> Left Binding
     - (default) `R2L` -> Right Binding
 
 By default, the page layout is set to `TwoPageRight` and the reading direction to `R2L`, which are suitable for Japanese manga.
 
 The `-j` or `--jpeg` option converts images to JPEG format before including them in the output PDF file, resulting in a smaller file size. Similarly, the `-g` or `--grayscale` option can be used to convert images to grayscale and reduce the size of the resulting PDF file. The program outputs the converted image in the specified format and compresses the PDF file accordingly.
```

### Comparing `manga2pdf-0.1.1/README.md` & `manga2pdf-0.1.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -16,22 +16,29 @@
 
 ## Usage
 This script can take input in the form of `zip`, `cbz`, `rar`, `cbr`, `epub` files or directories containing images (`jpg`, `jpeg`, `png`, `gif`, `bmp`) of manga or comic pages.
 
 The program can be executed from the command line with the following options:
 - The `input_path` argument represents the path to the input file. To execute the Python script correctly, specify the `input_path` argument as the path to the input file containing manga or comic images in any of the supported formats, such as `zip`, `cbz`, `rar`, `cbr`, `epub`, or a directory containing images in formats such as `jpg`, `jpeg`, `png`, `gif`, or `bmp`.
 - The `output_path` argument is the path to the output PDF file. To use the script, simply run the Python script with the path to the input file or directory as the argument. If the `--output` option is not specified, the output file name will be automatically generated based on the name of the input file or directory.
-- The `pagelayout` argument is the page layout of the PDF file. The `pagelayout` parameter can take in the following values:
+- The `pagelayout` parameter can take in the following values:
     - `SinglePage` -> Single page display
     - `OneColumn` -> Enable scrolling
     - `TwoPageLeft` -> Spread view
     - `TwoColumnLeft` -> Spread view with scrolling
     - (default) `TwoPageRight` -> Separate Cover, Spread View
     - `TwoColumnRight` -> Separate Cover, Scrolling Spread View
-- The `direction` argument is the reading direction of the PDF file. The `direction` parameter can take in the following values:
+- The `pagemode` parameter can take in the following values:
+    - (default) `UseNone` -> Neither document outline nor thumbnail images visible
+    - `UseOutlines` -> Document outline visible
+    - `UseThumbs` -> Thumbnail images visible
+    - `FullScreen` -> Full-screen mode
+    - `UseOC` -> Optional content group panel visible
+    - `UseAttachments` -> Attachments panel visible
+- The `direction` parameter can take in the following values:
     - `L2R` -> Left Binding
     - (default) `R2L` -> Right Binding
 
 By default, the page layout is set to `TwoPageRight` and the reading direction to `R2L`, which are suitable for Japanese manga.
 
 The `-j` or `--jpeg` option converts images to JPEG format before including them in the output PDF file, resulting in a smaller file size. Similarly, the `-g` or `--grayscale` option can be used to convert images to grayscale and reduce the size of the resulting PDF file. The program outputs the converted image in the specified format and compresses the PDF file accordingly.
```

### Comparing `manga2pdf-0.1.1/setup.py` & `manga2pdf-0.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.1.1"
+VERSION = "0.1.3"
 
 INSTALL_REQUIRES = (
     "numpy",
     "img2pdf",
     "Pillow",
     "pikepdf",
     "rarfile",
```

### Comparing `manga2pdf-0.1.1/src/manga2pdf.egg-info/PKG-INFO` & `manga2pdf-0.1.3/src/manga2pdf.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manga2pdf
-Version: 0.1.1
+Version: 0.1.3
 Summary: Convert manga/comic files(zip, epub, etc.) or directory containing image files (jpg, png, etc.) to PDF.
 Home-page: https://github.com/mashu3/manga2pdf
 Author: mashu3
 License: MIT
 Keywords: manga comic pdf converter
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
@@ -31,22 +31,29 @@
 
 ## Usage
 This script can take input in the form of `zip`, `cbz`, `rar`, `cbr`, `epub` files or directories containing images (`jpg`, `jpeg`, `png`, `gif`, `bmp`) of manga or comic pages.
 
 The program can be executed from the command line with the following options:
 - The `input_path` argument represents the path to the input file. To execute the Python script correctly, specify the `input_path` argument as the path to the input file containing manga or comic images in any of the supported formats, such as `zip`, `cbz`, `rar`, `cbr`, `epub`, or a directory containing images in formats such as `jpg`, `jpeg`, `png`, `gif`, or `bmp`.
 - The `output_path` argument is the path to the output PDF file. To use the script, simply run the Python script with the path to the input file or directory as the argument. If the `--output` option is not specified, the output file name will be automatically generated based on the name of the input file or directory.
-- The `pagelayout` argument is the page layout of the PDF file. The `pagelayout` parameter can take in the following values:
+- The `pagelayout` parameter can take in the following values:
     - `SinglePage` -> Single page display
     - `OneColumn` -> Enable scrolling
     - `TwoPageLeft` -> Spread view
     - `TwoColumnLeft` -> Spread view with scrolling
     - (default) `TwoPageRight` -> Separate Cover, Spread View
     - `TwoColumnRight` -> Separate Cover, Scrolling Spread View
-- The `direction` argument is the reading direction of the PDF file. The `direction` parameter can take in the following values:
+- The `pagemode` parameter can take in the following values:
+    - (default) `UseNone` -> Neither document outline nor thumbnail images visible
+    - `UseOutlines` -> Document outline visible
+    - `UseThumbs` -> Thumbnail images visible
+    - `FullScreen` -> Full-screen mode
+    - `UseOC` -> Optional content group panel visible
+    - `UseAttachments` -> Attachments panel visible
+- The `direction` parameter can take in the following values:
     - `L2R` -> Left Binding
     - (default) `R2L` -> Right Binding
 
 By default, the page layout is set to `TwoPageRight` and the reading direction to `R2L`, which are suitable for Japanese manga.
 
 The `-j` or `--jpeg` option converts images to JPEG format before including them in the output PDF file, resulting in a smaller file size. Similarly, the `-g` or `--grayscale` option can be used to convert images to grayscale and reduce the size of the resulting PDF file. The program outputs the converted image in the specified format and compresses the PDF file accordingly.
```

### Comparing `manga2pdf-0.1.1/src/manga2pdf.py` & `manga2pdf-0.1.3/src/manga2pdf.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,18 +19,19 @@
 from bs4 import BeautifulSoup
 
 warnings.filterwarnings('ignore', category=UserWarning)
 from bs4 import XMLParsedAsHTMLWarning
 warnings.filterwarnings('ignore', category=XMLParsedAsHTMLWarning)
 
 class MangaPdfConverter():   
-    def __init__(self, input_path: str, output_path: str, pagelayout:str, direction:str):
+    def __init__(self, input_path: str, output_path: str, pagelayout:str, pagemode:str, direction:str):
         self.input_path = input_path
         self.output_path = output_path
         self.pagelayout = pagelayout
+        self.pagemode = pagemode
         self.direction = direction
         self.convert_to_grayscale = False
         self.convert_to_jpeg = False
     def set_convert_to_jpeg(self, flag):
         self.convert_to_jpeg = flag
     def set_convert_to_grayscale(self, flag):
         self.convert_to_grayscale = flag
@@ -147,20 +148,36 @@
                 img = img.convert('RGB')
             img.save(img_output_path, 'PNG')
         return img_output_path, img_file_path
         
     # Function to extract the contents of an EPUB file
     def extract_epub_contents(self, epub):
         contents = epub.namelist()
+        ncx_names = []
+        opf_names = []
         for item in contents:
             extension = item.split('.')[-1].lower()
             if extension == 'ncx':
-                ncx_name = item
+                ncx_names.append(item)
             if extension == 'opf':
-                opf_name = item
+                opf_names.append(item)
+        flag = False
+        for ncx in ncx_names:
+            if 'standard' in ncx:
+                ncx_name = ncx
+                flag = True
+        if not flag:
+            ncx_name = ncx_names[0]
+        flag = False
+        for opf in opf_names:
+            if 'standard' in opf:
+                opf_name = opf
+                flag = True
+        if not flag:
+            opf_name = opf_names[0]
         page_names = []
         with epub.open(opf_name) as opf:
             content_opf = opf.read().decode()
             opf_soup = BeautifulSoup(content_opf, 'xml')
             for item in opf_soup.find_all('item', {'media-type': 'image/jpeg'}):
                 page_names.append(os.path.join(os.path.dirname(opf_name), item.get('href').replace('/', os.sep)).replace(os.sep, '/'))
             for item in opf_soup.find_all('item', {'media-type': 'image/png'}):
@@ -279,14 +296,18 @@
                     pdf_index.append(pikepdf.OutlineItem(index[0], index[1]))
                 with pdf.open_outline() as outline:
                     outline.root.extend(pdf_index)
             if self.pagelayout is not None:
                 if not hasattr(pdf.Root, 'PageLayout') \
                 or pdf.Root.PageLayout != '/' + self.pagelayout:
                     pdf.Root.PageLayout = pikepdf.Name('/' + self.pagelayout)
+            if self.pagemode is not None:
+                if not hasattr(pdf.Root, 'PageMode') \
+                or pdf.Root.PageMode != '/' + self.pagemodet:
+                    pdf.Root.PageMode = pikepdf.Name('/' + self.pagemode)
             if self.direction is not None:
                 if not hasattr(pdf.Root, 'ViewerPreferences'):
                     pdf.Root.ViewerPreferences = pikepdf.Dictionary()
                 if not hasattr(pdf.Root.ViewerPreferences, 'Direction') \
                     or pdf.Root.ViewerPreferences.Direction != '/' + self.direction:
                         pdf.Root.ViewerPreferences.Direction = pikepdf.Name('/' + self.direction)
             if self.output_path is None:
@@ -313,23 +334,32 @@
     parser = argparse.ArgumentParser(description='This program converts manga/comic files(zip, epub, etc.) or directory containing image files (jpg, png, etc.) to PDF', formatter_class=HelpFormatter)
     parser.add_argument('input_path', nargs='?', metavar='input_path', type=str,
                         help='input file path or directory path')
     parser.add_argument('-o', '--output', dest='output_path', type=str, default=None,
                         help='''\
 path to the output PDF file. 
 If not specified, the output file name is generated from the input file or directory name.''')
-    parser.add_argument('-p', '--pagelayout', type=str, default='TwoPageRight', 
+    parser.add_argument('-l', '--pagelayout', type=str, default='TwoPageRight', 
                         choices=['SinglePage', 'OneColumn', 'TwoColumnLeft', 'TwoColumnRight', 'TwoPageLeft', 'TwoPageRight'],
                         help='''\
 SinglePage -> Single page display
 OneColumn -> Enable scrolling
 TwoPageLeft -> Spread view
 TwoColumnLeft -> Spread view with scrolling
 (default) TwoPageRight -> Separate Cover, Spread View
 TwoColumnRight -> Separate Cover, Scrolling Spread View''')
+    parser.add_argument('-m', '--pagemode', type=str, default='UseNone', 
+                        choices=['UseOutlines', 'UseThumbs', 'FullScreen', 'UseOC', 'UseAttachments'],
+                        help='''\
+(default)UseNone -> Neither document outline nor thumbnail images visible
+UseOutlines -> Document outline visible
+UseThumbs -> Thumbnail images visible
+FullScreen -> Full-screen mode
+UseOC -> Optional content group panel visible
+UseAttachments -> Attachments panel visible''')
     parser.add_argument('-d', '--direction', type=str, default='R2L', choices=['L2R', 'R2L'],
                         help='''\
 L2R -> Left Binding
 (default)R2L -> Right Binding''')
     parser.add_argument('-j', '--jpeg', action='store_true', help='Convert images to JPEG')
     parser.add_argument('-g', '--grayscale', action='store_true', help='Convert images to grayscale')
     parser.add_argument('-gui', action='store_true', help='Launch GUI')
@@ -352,15 +382,15 @@
             if not args.output_path.endswith('.pdf'):
                 print('Error: The output file must be an PDF file.')
                 sys.exit(1)
         if args.grayscale and args.jpeg:
             print('Error: Cannot specify both --grayscale and --jpeg options.')
             sys.exit(1)
         
-        converter = MangaPdfConverter(args.input_path, args.output_path, args.pagelayout, args.direction)
+        converter = MangaPdfConverter(args.input_path, args.output_path, args.pagelayout, args.pagemode, args.direction)
         if args.jpeg:
             converter.set_convert_to_jpeg(True)
         elif args.grayscale:
             converter.set_convert_to_grayscale(True)
         converter.convert()
 
 if __name__ == '__main__':
```

### Comparing `manga2pdf-0.1.1/src/manga2pdf_gui.py` & `manga2pdf-0.1.3/src/manga2pdf_gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -266,15 +266,15 @@
         
         # Determine the conversion options
         convert_to_jpeg = self.conversion_var.get() == "jpeg"
         convert_to_grayscale = self.conversion_var.get() == "grayscale"
 
         # Call MangaPdfConverter with the appropriate arguments
         try:
-            converter = MangaPdfConverter(input_path=input_path, output_path=output_path, pagelayout=self.pagelayout_var.get(), direction=self.direction_var.get())
+            converter = MangaPdfConverter(input_path=input_path, output_path=output_path, pagelayout=self.pagelayout_var.get(), pagemode='UseNone', direction=self.direction_var.get())
 
             # Ask user if they want to convert
             confirm_text = {"en": "Are you sure you want to convert?", "ja": "変換処理を開始しますか？"}
             answer = messagebox.askyesno("Confirm Conversion", confirm_text[self.language], parent=self.master)
 
             if not answer:
                 cancele_text = {"en": "Conversion canceled.", "ja": "変換処理を中止しました"}
@@ -331,17 +331,14 @@
                 complete_success_text = {"en": "Conversion complete!", "ja": "変換処理が完了しました！"}
                 messagebox.showinfo("Success", complete_success_text[self.language], parent=self.master)
             else:
                 complete_error_text = {"en": "Conversion failed", "ja": "変換処理に失敗しました"}
                 messagebox.showerror("Error", complete_error_text[self.language], parent=self.master)
 
         except Exception as e:
-            # Close process window when done
-            processing_window.destroy()
-
             complete_error_text = {"en": "Conversion failed", "ja": "エラーで変換処理に失敗しました"}
             messagebox.showerror(title="Error", message=f"{complete_error_text[self.language]}\n{str(e)}", parent=self.master)
 
             # Re-enable main window
             self.master.deiconify()
 
 def launch_gui():
```

