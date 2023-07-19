# Comparing `tmp/image_file_validator-0.0.4-py3-none-any.whl.zip` & `tmp/image_file_validator-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3289 bytes, number of entries: 7
+Zip file size: 3254 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-19 07:09 image_file_validator/__init__.py
 -rw-rw-rw-  2.0 fat      763 b- defN 23-Jul-19 09:33 image_file_validator/image_file_validator.py
--rw-rw-rw-  2.0 fat     1065 b- defN 23-Jul-19 09:46 image_file_validator-0.0.4.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     1326 b- defN 23-Jul-19 09:46 image_file_validator-0.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-19 09:46 image_file_validator-0.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       21 b- defN 23-Jul-19 09:45 image_file_validator-0.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      641 b- defN 23-Jul-19 09:46 image_file_validator-0.0.4.dist-info/RECORD
-7 files, 3908 bytes uncompressed, 2127 bytes compressed:  45.6%
+-rw-rw-rw-  2.0 fat     1065 b- defN 23-Jul-19 09:51 image_file_validator-0.0.5.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     1232 b- defN 23-Jul-19 09:51 image_file_validator-0.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-19 09:51 image_file_validator-0.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       21 b- defN 23-Jul-19 09:50 image_file_validator-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      641 b- defN 23-Jul-19 09:51 image_file_validator-0.0.5.dist-info/RECORD
+7 files, 3814 bytes uncompressed, 2092 bytes compressed:  45.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: image_file_validator/__init__.py
 Comment: 
 
 Filename: image_file_validator/image_file_validator.py
 Comment: 
 
-Filename: image_file_validator-0.0.4.dist-info/LICENSE.txt
+Filename: image_file_validator-0.0.5.dist-info/LICENSE.txt
 Comment: 
 
-Filename: image_file_validator-0.0.4.dist-info/METADATA
+Filename: image_file_validator-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: image_file_validator-0.0.4.dist-info/WHEEL
+Filename: image_file_validator-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: image_file_validator-0.0.4.dist-info/top_level.txt
+Filename: image_file_validator-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: image_file_validator-0.0.4.dist-info/RECORD
+Filename: image_file_validator-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `image_file_validator-0.0.4.dist-info/LICENSE.txt` & `image_file_validator-0.0.5.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `image_file_validator-0.0.4.dist-info/METADATA` & `image_file_validator-0.0.5.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-file-validator
-Version: 0.0.4
+Version: 0.0.5
 Summary: A simple pluggable image file validator for all type of python applications
 Home-page: https://github.com/Zeecoworld/image-file-validator
 Author: Isaac Yakubu
 Author-email: engrisaac1234@gmail.com
 License: MIT
 Keywords: image-validate,image,image file validation
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,25 +18,23 @@
 
 This is a simple pluggable python library that validate image file and size useful for all 
 type of python applications.
 
 
 ####How to use the packages
 
-import os 
-import magic 
 
-imagecheck = ImageValidator("./hello.txt",2014)
-check_for_image_mime = imagecheck.check_file_size("./hello.txt",2014)
-check_for_image_size = imagecheck.check_file_mime_type("./hello.txt")
+from image_file_validator.image_file_validator import check_file_type
+
+check_for_image_size = check_file_type("./hello.png")
 
 
 # PIP PACKAGE DEPENDECIES
 
-pip install python-magic (pick your desired os)
+pip install filetype (pick your desired os)
 
 
 ### KINDLY MAKE PR for UPGRADE....
```

## Comparing `image_file_validator-0.0.4.dist-info/RECORD` & `image_file_validator-0.0.5.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 image_file_validator/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 image_file_validator/image_file_validator.py,sha256=JtvQCTVZsQbR2zQ9CLvGl96IyiXm8X5fx2jM27CcwH4,763
-image_file_validator-0.0.4.dist-info/LICENSE.txt,sha256=xOsvVkDlkKtVxzDzaycmKXDWsgC9d151PB4hrwnDLt0,1065
-image_file_validator-0.0.4.dist-info/METADATA,sha256=8PyVT_bTaSqT3waSCQXQqyo2aQmDrJFhFF341z4dQ1k,1326
-image_file_validator-0.0.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-image_file_validator-0.0.4.dist-info/top_level.txt,sha256=vaE80yHhZ8-tFA1R8CvDIU4TJf41GcoJ5Sic3gWNrHo,21
-image_file_validator-0.0.4.dist-info/RECORD,,
+image_file_validator-0.0.5.dist-info/LICENSE.txt,sha256=xOsvVkDlkKtVxzDzaycmKXDWsgC9d151PB4hrwnDLt0,1065
+image_file_validator-0.0.5.dist-info/METADATA,sha256=tAUJVXHhMHqVDzDYGbVmlJJseeUNi0ZGzDEwIQZy8lw,1232
+image_file_validator-0.0.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+image_file_validator-0.0.5.dist-info/top_level.txt,sha256=vaE80yHhZ8-tFA1R8CvDIU4TJf41GcoJ5Sic3gWNrHo,21
+image_file_validator-0.0.5.dist-info/RECORD,,
```

