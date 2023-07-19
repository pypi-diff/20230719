# Comparing `tmp/OneOnOne-0.6891.tar.gz` & `tmp/OneOnOne-0.6892.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OneOnOne-0.6891.tar", last modified: Wed Jul 19 11:25:21 2023, max compression
+gzip compressed data, was "OneOnOne-0.6892.tar", last modified: Wed Jul 19 11:54:34 2023, max compression
```

## Comparing `OneOnOne-0.6891.tar` & `OneOnOne-0.6892.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-19 11:25:21.698964 OneOnOne-0.6891/
--rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.6891/LICENSE
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-19 11:25:21.692276 OneOnOne-0.6891/OneOnOne/
--rw-r--r--   0 sohinib    (501) staff       (20)    36229 2023-07-19 11:25:05.000000 OneOnOne-0.6891/OneOnOne/__init__.py
--rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.6891/OneOnOne/classes.py
--rw-r--r--   0 sohinib    (501) staff       (20)    14768 2023-07-15 09:46:38.000000 OneOnOne-0.6891/OneOnOne/classification.py
--rw-r--r--   0 sohinib    (501) staff       (20)     1868 2023-07-12 19:25:09.000000 OneOnOne-0.6891/OneOnOne/contextdecider.py
--rw-r--r--   0 sohinib    (501) staff       (20)        0 2023-07-10 11:03:09.000000 OneOnOne-0.6891/OneOnOne/questionanswer.py
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-19 11:25:21.697360 OneOnOne-0.6891/OneOnOne.egg-info/
--rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-19 11:25:21.000000 OneOnOne-0.6891/OneOnOne.egg-info/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)      307 2023-07-19 11:25:21.000000 OneOnOne-0.6891/OneOnOne.egg-info/SOURCES.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-19 11:25:21.000000 OneOnOne-0.6891/OneOnOne.egg-info/dependency_links.txt
--rw-r--r--   0 sohinib    (501) staff       (20)      120 2023-07-19 11:25:21.000000 OneOnOne-0.6891/OneOnOne.egg-info/requires.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-19 11:25:21.000000 OneOnOne-0.6891/OneOnOne.egg-info/top_level.txt
--rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-19 11:25:21.698335 OneOnOne-0.6891/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)     1606 2023-07-12 20:09:33.000000 OneOnOne-0.6891/README.md
--rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-19 11:25:21.699193 OneOnOne-0.6891/setup.cfg
--rw-r--r--   0 sohinib    (501) staff       (20)     1918 2023-07-19 11:25:13.000000 OneOnOne-0.6891/setup.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-19 11:54:34.134430 OneOnOne-0.6892/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.6892/LICENSE
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-19 11:54:34.132128 OneOnOne-0.6892/OneOnOne/
+-rw-r--r--   0 sohinib    (501) staff       (20)    36428 2023-07-19 11:53:52.000000 OneOnOne-0.6892/OneOnOne/__init__.py
+-rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.6892/OneOnOne/classes.py
+-rw-r--r--   0 sohinib    (501) staff       (20)    14768 2023-07-15 09:46:38.000000 OneOnOne-0.6892/OneOnOne/classification.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     1868 2023-07-12 19:25:09.000000 OneOnOne-0.6892/OneOnOne/contextdecider.py
+-rw-r--r--   0 sohinib    (501) staff       (20)        0 2023-07-10 11:03:09.000000 OneOnOne-0.6892/OneOnOne/questionanswer.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-19 11:54:34.133676 OneOnOne-0.6892/OneOnOne.egg-info/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-19 11:54:34.000000 OneOnOne-0.6892/OneOnOne.egg-info/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)      307 2023-07-19 11:54:34.000000 OneOnOne-0.6892/OneOnOne.egg-info/SOURCES.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-19 11:54:34.000000 OneOnOne-0.6892/OneOnOne.egg-info/dependency_links.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)      120 2023-07-19 11:54:34.000000 OneOnOne-0.6892/OneOnOne.egg-info/requires.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-19 11:54:34.000000 OneOnOne-0.6892/OneOnOne.egg-info/top_level.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-19 11:54:34.134076 OneOnOne-0.6892/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)     1606 2023-07-12 20:09:33.000000 OneOnOne-0.6892/README.md
+-rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-19 11:54:34.134533 OneOnOne-0.6892/setup.cfg
+-rw-r--r--   0 sohinib    (501) staff       (20)     1919 2023-07-19 11:54:13.000000 OneOnOne-0.6892/setup.py
```

### Comparing `OneOnOne-0.6891/LICENSE` & `OneOnOne-0.6892/LICENSE`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6891/OneOnOne/__init__.py` & `OneOnOne-0.6892/OneOnOne/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 class PretrainedModel:
     def __init__(self, model_type="resnet50", dataset="cifar10", samplingtype="none"):
 
         self.model_type=model_type
         self.dataset=dataset
         self.samplingtype=samplingtype
 
-        self.map={"resnet50_cifar10_none":"1aP0TlpzOU9orokpQ1mKoOYyFCL_LgDRs"}
+        self.map={"resnet50_cifar10_none":"1tRc7uBW4AqfijKosZLKon_7Cxyl0iMvN","resnet50_cifar10_leastconfidence":"1fSJYo5VOppTkgWb-Fu2Sf_JL4s9JUmoK","resnet50_cifar10_mixed":"","resnet50_cifar10_margin":"","efficientnetb6_cifar10_none":"","efficientnetb6_tinyimagenet_none":""}
 
         if self.dataset=="tinyimagenet":
             self.model_type="efficientnetb6"
             self.samplingtype="none"
 
         self.model_name=f'{self.model_type}_{self.dataset}_{self.samplingtype}'
```

### Comparing `OneOnOne-0.6891/OneOnOne/classes.py` & `OneOnOne-0.6892/OneOnOne/classes.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6891/OneOnOne/classification.py` & `OneOnOne-0.6892/OneOnOne/classification.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6891/OneOnOne/contextdecider.py` & `OneOnOne-0.6892/OneOnOne/contextdecider.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6891/OneOnOne.egg-info/PKG-INFO` & `OneOnOne-0.6892/OneOnOne.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.6891
+Version: 0.6892
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OneOnOne-0.6891/PKG-INFO` & `OneOnOne-0.6892/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.6891
+Version: 0.6892
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OneOnOne-0.6891/README.md` & `OneOnOne-0.6892/README.md`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6891/setup.py` & `OneOnOne-0.6892/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from setuptools import setup, find_packages
 
-VERSION=0.6891
+VERSION=0.6892
+
 
 DESCRIPTION="A package for pre-trained image classification and context-decider for question-answering chatbots."
 LONG_DESCRIPTION="Your one-stop destination to utilize image-classification models with just one line of code. A library meant to simplify your life by providing you with pre-trained models like ResNet50, EfficientNetVB6, VGG19, etc. You can simply opt for training your own models from scratch by just tweaking a few values. If you want to try popular active-learning sampling methods on image classification, no need to worry! This library has got you covered. Along with that for simple-bridging and basic into NLP, we have context-deciders, HTML parsers and simple chatbot object classes, to create an interface similar to Google Lens. You input an image or item that you are curious about and you can ask one-on-one questions from the chatbot. This is made possible by using the tiny imagenet dataset. This library is being actively updated and new features are being added frequently. New datasets and pre-trained models will be updated soon. Feel free to share your feedback! I would really appreciate it!"
 CLASSIFIERS=[
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Education',
     'License :: OSI Approved :: MIT License',
```

