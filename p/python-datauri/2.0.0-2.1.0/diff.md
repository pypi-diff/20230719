# Comparing `tmp/python-datauri-2.0.0.tar.gz` & `tmp/python-datauri-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-datauri-2.0.0.tar", last modified: Fri May 26 20:05:17 2023, max compression
+gzip compressed data, was "python-datauri-2.1.0.tar", last modified: Wed Jul 19 15:55:28 2023, max compression
```

## Comparing `python-datauri-2.0.0.tar` & `python-datauri-2.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 flavio.curella   (502) staff       (20)        0 2023-05-26 20:05:17.679940 python-datauri-2.0.0/
--rw-r--r--   0 flavio.curella   (502) staff       (20)     1211 2020-07-31 14:49:13.000000 python-datauri-2.0.0/LICENSE
--rw-r--r--   0 flavio.curella   (502) staff       (20)      231 2023-05-26 15:55:57.000000 python-datauri-2.0.0/MANIFEST.in
--rw-r--r--   0 flavio.curella   (502) staff       (20)     2766 2023-05-26 20:05:17.680105 python-datauri-2.0.0/PKG-INFO
--rw-r--r--   0 flavio.curella   (502) staff       (20)     2022 2023-05-26 20:00:44.000000 python-datauri-2.0.0/README.rst
-drwxr-xr-x   0 flavio.curella   (502) staff       (20)        0 2023-05-26 20:05:17.674701 python-datauri-2.0.0/datauri/
--rw-r--r--   0 flavio.curella   (502) staff       (20)     5420 2023-05-26 18:22:14.000000 python-datauri-2.0.0/datauri/__init__.py
--rw-r--r--   0 flavio.curella   (502) staff       (20)      134 2020-07-31 14:49:13.000000 python-datauri-2.0.0/datauri/exceptions.py
--rw-r--r--   0 flavio.curella   (502) staff       (20)        0 2023-05-26 15:53:10.000000 python-datauri-2.0.0/datauri/py.typed
--rw-r--r--   0 flavio.curella   (502) staff       (20)      296 2023-05-26 15:52:20.000000 python-datauri-2.0.0/mypy.ini
-drwxr-xr-x   0 flavio.curella   (502) staff       (20)        0 2023-05-26 20:05:17.676861 python-datauri-2.0.0/python_datauri.egg-info/
--rw-r--r--   0 flavio.curella   (502) staff       (20)     2766 2023-05-26 20:05:17.000000 python-datauri-2.0.0/python_datauri.egg-info/PKG-INFO
--rw-r--r--   0 flavio.curella   (502) staff       (20)      462 2023-05-26 20:05:17.000000 python-datauri-2.0.0/python_datauri.egg-info/SOURCES.txt
--rw-r--r--   0 flavio.curella   (502) staff       (20)        1 2023-05-26 20:05:17.000000 python-datauri-2.0.0/python_datauri.egg-info/dependency_links.txt
--rw-r--r--   0 flavio.curella   (502) staff       (20)       18 2023-05-26 20:05:17.000000 python-datauri-2.0.0/python_datauri.egg-info/requires.txt
--rw-r--r--   0 flavio.curella   (502) staff       (20)       14 2023-05-26 20:05:17.000000 python-datauri-2.0.0/python_datauri.egg-info/top_level.txt
--rw-r--r--   0 flavio.curella   (502) staff       (20)      197 2023-05-26 20:05:17.681019 python-datauri-2.0.0/setup.cfg
--rw-r--r--   0 flavio.curella   (502) staff       (20)     1247 2023-05-26 20:04:51.000000 python-datauri-2.0.0/setup.py
-drwxr-xr-x   0 flavio.curella   (502) staff       (20)        0 2023-05-26 20:05:17.678132 python-datauri-2.0.0/tests/
--rw-r--r--   0 flavio.curella   (502) staff       (20)        0 2020-07-31 14:49:13.000000 python-datauri-2.0.0/tests/__init__.py
-drwxr-xr-x   0 flavio.curella   (502) staff       (20)        0 2023-05-26 20:05:17.679544 python-datauri-2.0.0/tests/assets/
--rw-r--r--   0 flavio.curella   (502) staff       (20)       19 2020-07-31 14:49:13.000000 python-datauri-2.0.0/tests/assets/test_file.txt
--rw-r--r--   0 flavio.curella   (502) staff       (20)       19 2020-07-31 14:49:13.000000 python-datauri-2.0.0/tests/assets/test_file_ebcdic.txt
--rw-r--r--   0 flavio.curella   (502) staff       (20)     3324 2020-07-31 14:49:13.000000 python-datauri-2.0.0/tests/assets/test_long_file.txt
--rw-r--r--   0 flavio.curella   (502) staff       (20)     5549 2023-05-26 19:56:28.000000 python-datauri-2.0.0/tests/test_parsing.py
--rw-r--r--   0 flavio.curella   (502) staff       (20)      561 2023-05-26 20:03:31.000000 python-datauri-2.0.0/tests/test_pydantic.py
+drwxr-xr-x   0 flavio.curella   (502) staff       (20)        0 2023-07-19 15:55:28.544588 python-datauri-2.1.0/
+-rw-r--r--   0 flavio.curella   (502) staff       (20)     1211 2020-07-31 14:49:13.000000 python-datauri-2.1.0/LICENSE
+-rw-r--r--   0 flavio.curella   (502) staff       (20)      231 2023-05-26 15:55:57.000000 python-datauri-2.1.0/MANIFEST.in
+-rw-r--r--   0 flavio.curella   (502) staff       (20)     3323 2023-07-19 15:55:28.544836 python-datauri-2.1.0/PKG-INFO
+-rw-r--r--   0 flavio.curella   (502) staff       (20)     2579 2023-07-19 15:52:28.000000 python-datauri-2.1.0/README.rst
+drwxr-xr-x   0 flavio.curella   (502) staff       (20)        0 2023-07-19 15:55:28.536380 python-datauri-2.1.0/datauri/
+-rw-r--r--   0 flavio.curella   (502) staff       (20)     5493 2023-07-19 15:51:43.000000 python-datauri-2.1.0/datauri/__init__.py
+-rw-r--r--   0 flavio.curella   (502) staff       (20)      134 2020-07-31 14:49:13.000000 python-datauri-2.1.0/datauri/exceptions.py
+-rw-r--r--   0 flavio.curella   (502) staff       (20)        0 2023-05-26 15:53:10.000000 python-datauri-2.1.0/datauri/py.typed
+-rw-r--r--   0 flavio.curella   (502) staff       (20)      296 2023-05-26 15:52:20.000000 python-datauri-2.1.0/mypy.ini
+drwxr-xr-x   0 flavio.curella   (502) staff       (20)        0 2023-07-19 15:55:28.539815 python-datauri-2.1.0/python_datauri.egg-info/
+-rw-r--r--   0 flavio.curella   (502) staff       (20)     3323 2023-07-19 15:55:28.000000 python-datauri-2.1.0/python_datauri.egg-info/PKG-INFO
+-rw-r--r--   0 flavio.curella   (502) staff       (20)      462 2023-07-19 15:55:28.000000 python-datauri-2.1.0/python_datauri.egg-info/SOURCES.txt
+-rw-r--r--   0 flavio.curella   (502) staff       (20)        1 2023-07-19 15:55:28.000000 python-datauri-2.1.0/python_datauri.egg-info/dependency_links.txt
+-rw-r--r--   0 flavio.curella   (502) staff       (20)       18 2023-07-19 15:55:28.000000 python-datauri-2.1.0/python_datauri.egg-info/requires.txt
+-rw-r--r--   0 flavio.curella   (502) staff       (20)       14 2023-07-19 15:55:28.000000 python-datauri-2.1.0/python_datauri.egg-info/top_level.txt
+-rw-r--r--   0 flavio.curella   (502) staff       (20)      197 2023-07-19 15:55:28.545974 python-datauri-2.1.0/setup.cfg
+-rw-r--r--   0 flavio.curella   (502) staff       (20)     1247 2023-07-19 15:55:12.000000 python-datauri-2.1.0/setup.py
+drwxr-xr-x   0 flavio.curella   (502) staff       (20)        0 2023-07-19 15:55:28.542029 python-datauri-2.1.0/tests/
+-rw-r--r--   0 flavio.curella   (502) staff       (20)        0 2020-07-31 14:49:13.000000 python-datauri-2.1.0/tests/__init__.py
+drwxr-xr-x   0 flavio.curella   (502) staff       (20)        0 2023-07-19 15:55:28.544023 python-datauri-2.1.0/tests/assets/
+-rw-r--r--   0 flavio.curella   (502) staff       (20)       19 2020-07-31 14:49:13.000000 python-datauri-2.1.0/tests/assets/test_file.txt
+-rw-r--r--   0 flavio.curella   (502) staff       (20)       19 2020-07-31 14:49:13.000000 python-datauri-2.1.0/tests/assets/test_file_ebcdic.txt
+-rw-r--r--   0 flavio.curella   (502) staff       (20)     3324 2020-07-31 14:49:13.000000 python-datauri-2.1.0/tests/assets/test_long_file.txt
+-rw-r--r--   0 flavio.curella   (502) staff       (20)     5549 2023-05-26 19:56:28.000000 python-datauri-2.1.0/tests/test_parsing.py
+-rw-r--r--   0 flavio.curella   (502) staff       (20)      596 2023-05-26 20:10:51.000000 python-datauri-2.1.0/tests/test_pydantic.py
```

### Comparing `python-datauri-2.0.0/LICENSE` & `python-datauri-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-datauri-2.0.0/PKG-INFO` & `python-datauri-2.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-datauri
-Version: 2.0.0
+Version: 2.1.0
 Summary: A li'l class for data URI manipulation in Python
 Home-page: https://github.com/fcurella/python-datauri/
 Maintainer: Flavio Curella
 Maintainer-email: flavio.curella@gmail.com
 License: Unlicense
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -82,14 +82,42 @@
   >>> from datauri import DataURI
   >>> png_uri = DataURI.from_file('somefile.png')
   >>> png_uri.mimetype
   'image/png'
   >>> png_uri.data
   b'\x89PNG\r\n...'
 
+
+Serializing
+-----------
+
+`DataURI` is a subclass of `str`, so you can just use `str()` to print it out:
+
+.. code-block:: python
+
+  >>> from datauri import DataURI
+  >>> png_uri = DataURI.from_file('somefile.png')
+  >>> str(png_uri)
+  'data:image/jpeg;base64,/9j/4AAQSkZJRgABAQAASABIA...'
+ 
+Pydantic Support
+----------------
+
+You can use `DataURI` as a type for `Pydantic` v1:
+
+.. code-block:: python
+
+  from datauri import DataURI
+  from datauri import DataURI
+  from pydantic import BaseModel
+
+
+  class ProfilePicture(BaseModel):
+    image_data: DataURI
+
 License
 -------
 
 This code is released under the `Unlicense <http://unlicense.org/>`_.
 
 Credits
 -------
```

### Comparing `python-datauri-2.0.0/README.rst` & `python-datauri-2.1.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -62,14 +62,42 @@
   >>> from datauri import DataURI
   >>> png_uri = DataURI.from_file('somefile.png')
   >>> png_uri.mimetype
   'image/png'
   >>> png_uri.data
   b'\x89PNG\r\n...'
 
+
+Serializing
+-----------
+
+`DataURI` is a subclass of `str`, so you can just use `str()` to print it out:
+
+.. code-block:: python
+
+  >>> from datauri import DataURI
+  >>> png_uri = DataURI.from_file('somefile.png')
+  >>> str(png_uri)
+  'data:image/jpeg;base64,/9j/4AAQSkZJRgABAQAASABIA...'
+ 
+Pydantic Support
+----------------
+
+You can use `DataURI` as a type for `Pydantic` v1:
+
+.. code-block:: python
+
+  from datauri import DataURI
+  from datauri import DataURI
+  from pydantic import BaseModel
+
+
+  class ProfilePicture(BaseModel):
+    image_data: DataURI
+
 License
 -------
 
 This code is released under the `Unlicense <http://unlicense.org/>`_.
 
 Credits
 -------
```

### Comparing `python-datauri-2.0.0/datauri/__init__.py` & `python-datauri-2.1.0/datauri/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,16 +67,18 @@
 
     @classmethod
     def from_file(
         cls,
         filename: str,
         charset: Optional[str] = None,
         base64: Optional[bool] = True,
+        mimetype: Optional[str] = None,
     ) -> Self:
-        mimetype, _ = mimetypes.guess_type(filename, strict=False)
+        if mimetype is None:
+            mimetype, _ = mimetypes.guess_type(filename, strict=False)
         with open(filename, "rb") as fp:
             data = fp.read()
 
         return cls.make(mimetype, charset, base64, data)
 
     def __new__(cls, *args: Any, **kwargs: Any) -> Self:
         uri = super(DataURI, cls).__new__(cls, *args, **kwargs)
```

### Comparing `python-datauri-2.0.0/python_datauri.egg-info/PKG-INFO` & `python-datauri-2.1.0/python_datauri.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-datauri
-Version: 2.0.0
+Version: 2.1.0
 Summary: A li'l class for data URI manipulation in Python
 Home-page: https://github.com/fcurella/python-datauri/
 Maintainer: Flavio Curella
 Maintainer-email: flavio.curella@gmail.com
 License: Unlicense
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -82,14 +82,42 @@
   >>> from datauri import DataURI
   >>> png_uri = DataURI.from_file('somefile.png')
   >>> png_uri.mimetype
   'image/png'
   >>> png_uri.data
   b'\x89PNG\r\n...'
 
+
+Serializing
+-----------
+
+`DataURI` is a subclass of `str`, so you can just use `str()` to print it out:
+
+.. code-block:: python
+
+  >>> from datauri import DataURI
+  >>> png_uri = DataURI.from_file('somefile.png')
+  >>> str(png_uri)
+  'data:image/jpeg;base64,/9j/4AAQSkZJRgABAQAASABIA...'
+ 
+Pydantic Support
+----------------
+
+You can use `DataURI` as a type for `Pydantic` v1:
+
+.. code-block:: python
+
+  from datauri import DataURI
+  from datauri import DataURI
+  from pydantic import BaseModel
+
+
+  class ProfilePicture(BaseModel):
+    image_data: DataURI
+
 License
 -------
 
 This code is released under the `Unlicense <http://unlicense.org/>`_.
 
 Credits
 -------
```

### Comparing `python-datauri-2.0.0/setup.py` & `python-datauri-2.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 from setuptools import find_packages, setup
 
-VERSION = "2.0.0"
+VERSION = "2.1.0"
 
 
 def read(fname):
     try:
         with open(os.path.join(os.path.dirname(__file__), fname)) as fh:
             return fh.read()
     except IOError:
```

### Comparing `python-datauri-2.0.0/tests/assets/test_long_file.txt` & `python-datauri-2.1.0/tests/assets/test_long_file.txt`

 * *Files identical despite different names*

### Comparing `python-datauri-2.0.0/tests/test_parsing.py` & `python-datauri-2.1.0/tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `python-datauri-2.0.0/tests/test_pydantic.py` & `python-datauri-2.1.0/tests/test_pydantic.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,9 +8,13 @@
 def test_pydantic():
     class Model(pydantic.BaseModel):
         content: DataURI
 
     t = "data:text/plain;charset=utf-8;base64,VGhlIHF1aWNrIGJyb3duIGZveCBqdW1wZWQgb3ZlciB0aGUgbGF6eSBkb2cu"
     instance = Model(content=t)
     assert isinstance(instance.content, DataURI)
-    assert instance.json() == '{"content": "data:text/plain;charset=utf-8;base64,VGhlIHF1aWNrIGJyb3duIGZveCBqdW1wZWQgb3ZlciB0aGUgbGF6eSBkb2cu"}'
+    assert (
+        instance.json()
+        == '{"content": "data:text/plain;charset=utf-8;base64,VGhlIHF1aWNrIGJyb3duIGZveCBqdW1wZWQgb3ZlciB0'
+        'aGUgbGF6eSBkb2cu"}'
+    )
     assert instance.dict() == {"content": DataURI(t)}
```

