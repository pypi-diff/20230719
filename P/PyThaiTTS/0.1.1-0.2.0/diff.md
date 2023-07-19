# Comparing `tmp/PyThaiTTS-0.1.1.tar.gz` & `tmp/PyThaiTTS-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyThaiTTS-0.1.1.tar", last modified: Sat Aug 27 16:59:38 2022, max compression
+gzip compressed data, was "PyThaiTTS-0.2.0.tar", last modified: Wed Jul 19 08:22:07 2023, max compression
```

## Comparing `PyThaiTTS-0.1.1.tar` & `PyThaiTTS-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 16:59:38.377478 PyThaiTTS-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-08-27 16:59:28.000000 PyThaiTTS-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1671 2022-08-27 16:59:38.377478 PyThaiTTS-0.1.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 16:59:38.373478 PyThaiTTS-0.1.1/PyThaiTTS.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1671 2022-08-27 16:59:38.000000 PyThaiTTS-0.1.1/PyThaiTTS.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      315 2022-08-27 16:59:38.000000 PyThaiTTS-0.1.1/PyThaiTTS.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-27 16:59:38.000000 PyThaiTTS-0.1.1/PyThaiTTS.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-27 16:59:38.000000 PyThaiTTS-0.1.1/PyThaiTTS.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-08-27 16:59:38.000000 PyThaiTTS-0.1.1/PyThaiTTS.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-08-27 16:59:38.000000 PyThaiTTS-0.1.1/PyThaiTTS.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      594 2022-08-27 16:59:28.000000 PyThaiTTS-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 16:59:38.373478 PyThaiTTS-0.1.1/pythaitts/
--rw-r--r--   0 runner    (1001) docker     (121)     1974 2022-08-27 16:59:28.000000 PyThaiTTS-0.1.1/pythaitts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 16:59:38.377478 PyThaiTTS-0.1.1/pythaitts/pretrained/
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-08-27 16:59:28.000000 PyThaiTTS-0.1.1/pythaitts/pretrained/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4524 2022-08-27 16:59:28.000000 PyThaiTTS-0.1.1/pythaitts/pretrained/khanomtan_tts.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-27 16:59:38.377478 PyThaiTTS-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1616 2022-08-27 16:59:28.000000 PyThaiTTS-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 08:22:07.596397 PyThaiTTS-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-07-19 08:21:56.000000 PyThaiTTS-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1671 2023-07-19 08:22:07.596397 PyThaiTTS-0.2.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 08:22:07.596397 PyThaiTTS-0.2.0/PyThaiTTS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1671 2023-07-19 08:22:07.000000 PyThaiTTS-0.2.0/PyThaiTTS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      355 2023-07-19 08:22:07.000000 PyThaiTTS-0.2.0/PyThaiTTS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-19 08:22:07.000000 PyThaiTTS-0.2.0/PyThaiTTS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-19 08:22:07.000000 PyThaiTTS-0.2.0/PyThaiTTS.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-07-19 08:22:07.000000 PyThaiTTS-0.2.0/PyThaiTTS.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-19 08:22:07.000000 PyThaiTTS-0.2.0/PyThaiTTS.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      594 2023-07-19 08:21:56.000000 PyThaiTTS-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 08:22:07.596397 PyThaiTTS-0.2.0/pythaitts/
+-rw-r--r--   0 runner    (1001) docker     (122)     2597 2023-07-19 08:21:56.000000 PyThaiTTS-0.2.0/pythaitts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 08:22:07.596397 PyThaiTTS-0.2.0/pythaitts/pretrained/
+-rw-r--r--   0 runner    (1001) docker     (122)      197 2023-07-19 08:21:56.000000 PyThaiTTS-0.2.0/pythaitts/pretrained/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4524 2023-07-19 08:21:56.000000 PyThaiTTS-0.2.0/pythaitts/pretrained/khanomtan_tts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1972 2023-07-19 08:21:56.000000 PyThaiTTS-0.2.0/pythaitts/pretrained/lunarlist_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-19 08:22:07.596397 PyThaiTTS-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1616 2023-07-19 08:21:56.000000 PyThaiTTS-0.2.0/setup.py
```

### Comparing `PyThaiTTS-0.1.1/LICENSE` & `PyThaiTTS-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyThaiTTS-0.1.1/PKG-INFO` & `PyThaiTTS-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyThaiTTS
-Version: 0.1.1
+Version: 0.2.0
 Summary: Open Source Thai Text-to-speech library in Python
 Home-page: https://github.com/pythainlp/pythaitts
 Author: Wannaphong
 Author-email: wannaphong@yahoo.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://github.com/pythainlp/pythaitts
 Project-URL: Source, https://github.com/pythainlp/pythaitts
```

### Comparing `PyThaiTTS-0.1.1/PyThaiTTS.egg-info/PKG-INFO` & `PyThaiTTS-0.2.0/PyThaiTTS.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyThaiTTS
-Version: 0.1.1
+Version: 0.2.0
 Summary: Open Source Thai Text-to-speech library in Python
 Home-page: https://github.com/pythainlp/pythaitts
 Author: Wannaphong
 Author-email: wannaphong@yahoo.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://github.com/pythainlp/pythaitts
 Project-URL: Source, https://github.com/pythainlp/pythaitts
```

### Comparing `PyThaiTTS-0.1.1/README.md` & `PyThaiTTS-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `PyThaiTTS-0.1.1/pythaitts/__init__.py` & `PyThaiTTS-0.2.0/pythaitts/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,47 @@
 # -*- coding: utf-8 -*-
 """
 PyThaiTTS
 """
-__version__ = "0.1.1"
+__version__ = "0.2.0"
 
 
 class TTS:
-    def __init__(self, pretrained="khanomtan", mode="last_checkpoint", version="1.0") -> None:
+    def __init__(self, pretrained="khanomtan", mode="last_checkpoint", version="1.0", device:str="cpu") -> None:
         """
-        :param str pretrained: TTS pretrained (khanomtan)
+        :param str pretrained: TTS pretrained (khanomtan, lunarlist)
         :param str mode: pretrained mode
         :param str version: model version (default is 1.0 or 1.1)
 
         **Options for mode**
             * *last_checkpoint* (default) - last checkpoint of model
             * *best_model* - Best model (best loss)
         
         You can see more about khanomtan tts at `https://github.com/wannaphong/KhanomTan-TTS-v1.0 <https://github.com/wannaphong/KhanomTan-TTS-v1.0>`_
         and `https://github.com/wannaphong/KhanomTan-TTS-v1.1 <https://github.com/wannaphong/KhanomTan-TTS-v1.1>`_
+        
+        For lunarlist tts model, you must to install nemo before use the model by pip install nemo_toolkit['tts'].
+        You can see more about lunarlist tts at `https://link.medium.com/OpPjQis6wBb <https://link.medium.com/OpPjQis6wBb>`_
+        
         """
         self.pretrained = pretrained
         self.mode = mode
+        self.device = device
         self.load_pretrained(version=version)
 
     def load_pretrained(self,version):
         """
         Load pretrined
         """
         if self.pretrained == "khanomtan":
             from pythaitts.pretrained import KhanomTan
             self.model = KhanomTan(mode=self.mode, version=version)
+        elif self.pretrained == "lunarlist":
+            from pythaitts.pretrained import LunarlistModel
+            self.model = LunarlistModel(mode=self.mode, device=self.device)
         else:
             raise NotImplemented(
                 "PyThaiTTS doesn't support %s pretrained." % self.pretrained
             )
 
     def tts(self, text: str, speaker_idx: str = "Linda", language_idx: str = "th-th", return_type: str = "file", filename: str = None):
         """
@@ -41,14 +49,16 @@
 
         :param str text: text
         :param str speaker_idx: speaker (default is Linda)
         :param str language_idx: language (default is th-th)
         :param str return_type: return type (default is file)
         :param str filename: path filename for save wav file if return_type is file.
         """
+        if self.pretrained == "lunarlist":
+            return self.model(text=text,return_type=return_type,filename=filename)
         return self.model(
             text=text,
             speaker_idx=speaker_idx,
             language_idx=language_idx,
             return_type=return_type,
             filename=filename
         )
```

### Comparing `PyThaiTTS-0.1.1/pythaitts/pretrained/khanomtan_tts.py` & `PyThaiTTS-0.2.0/pythaitts/pretrained/khanomtan_tts.py`

 * *Files identical despite different names*

### Comparing `PyThaiTTS-0.1.1/setup.py` & `PyThaiTTS-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     readme = f.read()
 
 with open("requirements.txt","r",encoding="utf-8-sig") as f:
     requirements = [i.strip() for i in f.readlines()]
 
 setup(
     name="PyThaiTTS",
-    version="0.1.1",
+    version="0.2.0",
     description="Open Source Thai Text-to-speech library in Python",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Wannaphong",
     author_email="wannaphong@yahoo.com",
     url="https://github.com/pythainlp/pythaitts",
     packages=find_packages(),
```

