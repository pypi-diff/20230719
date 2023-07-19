# Comparing `tmp/ImgTextClipboard-python-0.1.2.tar.gz` & `tmp/ImgTextClipboard-python-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ImgTextClipboard-python-0.1.2.tar", last modified: Wed Jul 19 07:22:52 2023, max compression
+gzip compressed data, was "ImgTextClipboard-python-0.1.3.tar", last modified: Wed Jul 19 07:26:12 2023, max compression
```

## Comparing `ImgTextClipboard-python-0.1.2.tar` & `ImgTextClipboard-python-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 07:22:52.589585 ImgTextClipboard-python-0.1.2/
-drwxrwxrwx   0        0        0        0 2023-07-19 07:22:52.587592 ImgTextClipboard-python-0.1.2/ImgTextClipboard/
--rw-rw-rw-   0        0        0     1176 2023-07-19 06:16:06.000000 ImgTextClipboard-python-0.1.2/ImgTextClipboard/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-19 07:22:52.589585 ImgTextClipboard-python-0.1.2/ImgTextClipboard_python.egg-info/
--rw-rw-rw-   0        0        0      587 2023-07-19 07:22:52.000000 ImgTextClipboard-python-0.1.2/ImgTextClipboard_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-07-19 07:22:52.000000 ImgTextClipboard-python-0.1.2/ImgTextClipboard_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 07:22:52.000000 ImgTextClipboard-python-0.1.2/ImgTextClipboard_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-07-19 07:22:52.000000 ImgTextClipboard-python-0.1.2/ImgTextClipboard_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-19 07:22:52.000000 ImgTextClipboard-python-0.1.2/ImgTextClipboard_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      587 2023-07-19 07:22:52.589585 ImgTextClipboard-python-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-19 06:28:29.000000 ImgTextClipboard-python-0.1.2/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-19 07:22:52.589585 ImgTextClipboard-python-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      999 2023-07-19 07:22:32.000000 ImgTextClipboard-python-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 07:26:12.395902 ImgTextClipboard-python-0.1.3/
+drwxrwxrwx   0        0        0        0 2023-07-19 07:26:12.393910 ImgTextClipboard-python-0.1.3/ImgTextClipboard/
+-rw-rw-rw-   0        0        0     1176 2023-07-19 06:16:06.000000 ImgTextClipboard-python-0.1.3/ImgTextClipboard/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 07:26:12.395902 ImgTextClipboard-python-0.1.3/ImgTextClipboard_python.egg-info/
+-rw-rw-rw-   0        0        0      587 2023-07-19 07:26:12.000000 ImgTextClipboard-python-0.1.3/ImgTextClipboard_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-07-19 07:26:12.000000 ImgTextClipboard-python-0.1.3/ImgTextClipboard_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 07:26:12.000000 ImgTextClipboard-python-0.1.3/ImgTextClipboard_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-07-19 07:26:12.000000 ImgTextClipboard-python-0.1.3/ImgTextClipboard_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-19 07:26:12.000000 ImgTextClipboard-python-0.1.3/ImgTextClipboard_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      587 2023-07-19 07:26:12.395902 ImgTextClipboard-python-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-19 06:28:29.000000 ImgTextClipboard-python-0.1.3/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-19 07:26:12.395902 ImgTextClipboard-python-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1027 2023-07-19 07:26:05.000000 ImgTextClipboard-python-0.1.3/setup.py
```

### Comparing `ImgTextClipboard-python-0.1.2/ImgTextClipboard/__init__.py` & `ImgTextClipboard-python-0.1.3/ImgTextClipboard/__init__.py`

 * *Files identical despite different names*

### Comparing `ImgTextClipboard-python-0.1.2/ImgTextClipboard_python.egg-info/PKG-INFO` & `ImgTextClipboard-python-0.1.3/ImgTextClipboard_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ImgTextClipboard-python
-Version: 0.1.2
+Version: 0.1.3
 Summary: Convenient to operate clipboard related images by oneself
 Home-page: https://github.com/LanluZ/ImgTextClipboard-python
 Author: LanluZ
 Keywords: image,copy,paste,windows,clipboard
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ImgTextClipboard-python-0.1.2/PKG-INFO` & `ImgTextClipboard-python-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ImgTextClipboard-python
-Version: 0.1.2
+Version: 0.1.3
 Summary: Convenient to operate clipboard related images by oneself
 Home-page: https://github.com/LanluZ/ImgTextClipboard-python
 Author: LanluZ
 Keywords: image,copy,paste,windows,clipboard
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ImgTextClipboard-python-0.1.2/setup.py` & `ImgTextClipboard-python-0.1.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import setuptools
 
 setuptools.setup(
     name="ImgTextClipboard-python",  # 库的名字
-    version='0.1.2',  # 库的版本号，后续更新的时候只需要改版本号就行
+    version='0.1.3',  # 库的版本号，后续更新的时候只需要改版本号就行
     author="LanluZ",  # 你的你的名字
     description="Convenient to operate clipboard related images by oneself",  # 介绍
     long_description_content_type="text/markdown",
     url='https://github.com/LanluZ/ImgTextClipboard-python',
     packages=setuptools.find_packages(),
     install_requires=[
         "pywin32>=306",
         "Pillow>=10.0.0",
         "image>=1.5.33",
+        "pyperclip>=1.8.2"
     ],
     keywords=['image', 'copy', 'paste', 'windows', 'clipboard'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
```

