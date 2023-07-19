# Comparing `tmp/discohooker-0.0.0b1.tar.gz` & `tmp/discohooker-0.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discohooker-0.0.0b1.tar", last modified: Wed Jul 19 15:15:35 2023, max compression
+gzip compressed data, was "discohooker-0.0.0b2.tar", last modified: Wed Jul 19 15:31:52 2023, max compression
```

## Comparing `discohooker-0.0.0b1.tar` & `discohooker-0.0.0b2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-19 15:15:35.859805 discohooker-0.0.0b1/
--rw-r--r--   0 runner    (1000) runner    (1000)     1066 2023-07-17 08:42:29.000000 discohooker-0.0.0b1/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     1113 2023-07-19 15:15:35.859805 discohooker-0.0.0b1/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      647 2023-07-19 15:15:07.000000 discohooker-0.0.0b1/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-19 15:15:35.855805 discohooker-0.0.0b1/discohooker/
--rw-r--r--   0 runner    (1000) runner    (1000)       92 2023-07-19 13:55:35.000000 discohooker-0.0.0b1/discohooker/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3695 2023-07-19 14:18:21.000000 discohooker-0.0.0b1/discohooker/embed.py
--rw-r--r--   0 runner    (1000) runner    (1000)      278 2023-07-19 15:15:06.000000 discohooker-0.0.0b1/discohooker/errors.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4844 2023-07-19 15:15:06.000000 discohooker-0.0.0b1/discohooker/webhook.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-19 15:15:35.859805 discohooker-0.0.0b1/discohooker.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1113 2023-07-19 15:15:35.000000 discohooker-0.0.0b1/discohooker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      305 2023-07-19 15:15:35.000000 discohooker-0.0.0b1/discohooker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-19 15:15:35.000000 discohooker-0.0.0b1/discohooker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       23 2023-07-19 15:15:35.000000 discohooker-0.0.0b1/discohooker.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       12 2023-07-19 15:15:35.000000 discohooker-0.0.0b1/discohooker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      472 2023-07-15 08:52:33.000000 discohooker-0.0.0b1/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-19 15:15:35.859805 discohooker-0.0.0b1/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      714 2023-07-19 14:03:39.000000 discohooker-0.0.0b1/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-19 15:31:52.923751 discohooker-0.0.0b2/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1066 2023-07-17 08:42:29.000000 discohooker-0.0.0b2/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     1113 2023-07-19 15:31:52.919751 discohooker-0.0.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      647 2023-07-19 15:15:07.000000 discohooker-0.0.0b2/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-19 15:31:52.915751 discohooker-0.0.0b2/discohooker/
+-rw-r--r--   0 runner    (1000) runner    (1000)       92 2023-07-19 13:55:35.000000 discohooker-0.0.0b2/discohooker/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3693 2023-07-19 15:29:36.000000 discohooker-0.0.0b2/discohooker/embed.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      278 2023-07-19 15:15:06.000000 discohooker-0.0.0b2/discohooker/errors.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4844 2023-07-19 15:15:06.000000 discohooker-0.0.0b2/discohooker/webhook.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-19 15:31:52.919751 discohooker-0.0.0b2/discohooker.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1113 2023-07-19 15:31:52.000000 discohooker-0.0.0b2/discohooker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      305 2023-07-19 15:31:52.000000 discohooker-0.0.0b2/discohooker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-19 15:31:52.000000 discohooker-0.0.0b2/discohooker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       23 2023-07-19 15:31:52.000000 discohooker-0.0.0b2/discohooker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       12 2023-07-19 15:31:52.000000 discohooker-0.0.0b2/discohooker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      472 2023-07-15 08:52:33.000000 discohooker-0.0.0b2/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-19 15:31:52.923751 discohooker-0.0.0b2/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      714 2023-07-19 15:30:53.000000 discohooker-0.0.0b2/setup.py
```

### Comparing `discohooker-0.0.0b1/LICENSE` & `discohooker-0.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `discohooker-0.0.0b1/PKG-INFO` & `discohooker-0.0.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discohooker
-Version: 0.0.0b1
+Version: 0.0.0b2
 Summary: A easy PyPI to send Discord Webhook!
 Home-page: https://replit.com/@MAX110331/discohooker
 Author: MaxPython110331
 Author-email: max.gamil110331@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `discohooker-0.0.0b1/README.md` & `discohooker-0.0.0b2/README.md`

 * *Files identical despite different names*

### Comparing `discohooker-0.0.0b1/discohooker/embed.py` & `discohooker-0.0.0b2/discohooker/embed.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import .errors import Errors
+from .errors import Errors
 import random
 from datetime import datetime
 
 
 class EmbedField:
     def __init__(self, name: str=None, value: str=None, inline: bool=True):
         self.name=name
@@ -31,15 +31,15 @@
         
 
 
 class Embed:
     def __init__(self, title: str=None, description: str=None, colour: str=0xffffff, url: str=None, fields: list[EmbedField]=[], timestamp: datetime.datetime=None):
         self.title=title
         self.description=description
-        sepf.colour=colour
+        self.colour=colour
         if not url.startswith("https://") and url != None:
             raise Errors.URLError("This is not URL! Please check and change your URL!")
         self.url=url
         self.fields=fields
         self.timestamp=timestamp
         self._image={}
         self._thumbnail={}
```

### Comparing `discohooker-0.0.0b1/discohooker/webhook.py` & `discohooker-0.0.0b2/discohooker/webhook.py`

 * *Files identical despite different names*

### Comparing `discohooker-0.0.0b1/discohooker.egg-info/PKG-INFO` & `discohooker-0.0.0b2/discohooker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discohooker
-Version: 0.0.0b1
+Version: 0.0.0b2
 Summary: A easy PyPI to send Discord Webhook!
 Home-page: https://replit.com/@MAX110331/discohooker
 Author: MaxPython110331
 Author-email: max.gamil110331@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `discohooker-0.0.0b1/setup.py` & `discohooker-0.0.0b2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="discohooker",
-    version="0.0.0b1",
+    version="0.0.0b2",
     author="MaxPython110331",
     author_email="max.gamil110331@gmail.com",
     description="A easy PyPI to send Discord Webhook!",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://replit.com/@MAX110331/discohooker",
```

