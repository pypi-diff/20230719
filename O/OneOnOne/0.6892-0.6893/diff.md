# Comparing `tmp/OneOnOne-0.6892.tar.gz` & `tmp/OneOnOne-0.6893.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OneOnOne-0.6892.tar", last modified: Wed Jul 19 11:54:34 2023, max compression
+gzip compressed data, was "OneOnOne-0.6893.tar", last modified: Wed Jul 19 12:05:07 2023, max compression
```

## Comparing `OneOnOne-0.6892.tar` & `OneOnOne-0.6893.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-19 11:54:34.134430 OneOnOne-0.6892/
--rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.6892/LICENSE
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-19 11:54:34.132128 OneOnOne-0.6892/OneOnOne/
--rw-r--r--   0 sohinib    (501) staff       (20)    36428 2023-07-19 11:53:52.000000 OneOnOne-0.6892/OneOnOne/__init__.py
--rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.6892/OneOnOne/classes.py
--rw-r--r--   0 sohinib    (501) staff       (20)    14768 2023-07-15 09:46:38.000000 OneOnOne-0.6892/OneOnOne/classification.py
--rw-r--r--   0 sohinib    (501) staff       (20)     1868 2023-07-12 19:25:09.000000 OneOnOne-0.6892/OneOnOne/contextdecider.py
--rw-r--r--   0 sohinib    (501) staff       (20)        0 2023-07-10 11:03:09.000000 OneOnOne-0.6892/OneOnOne/questionanswer.py
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-19 11:54:34.133676 OneOnOne-0.6892/OneOnOne.egg-info/
--rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-19 11:54:34.000000 OneOnOne-0.6892/OneOnOne.egg-info/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)      307 2023-07-19 11:54:34.000000 OneOnOne-0.6892/OneOnOne.egg-info/SOURCES.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-19 11:54:34.000000 OneOnOne-0.6892/OneOnOne.egg-info/dependency_links.txt
--rw-r--r--   0 sohinib    (501) staff       (20)      120 2023-07-19 11:54:34.000000 OneOnOne-0.6892/OneOnOne.egg-info/requires.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-19 11:54:34.000000 OneOnOne-0.6892/OneOnOne.egg-info/top_level.txt
--rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-19 11:54:34.134076 OneOnOne-0.6892/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)     1606 2023-07-12 20:09:33.000000 OneOnOne-0.6892/README.md
--rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-19 11:54:34.134533 OneOnOne-0.6892/setup.cfg
--rw-r--r--   0 sohinib    (501) staff       (20)     1919 2023-07-19 11:54:13.000000 OneOnOne-0.6892/setup.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-19 12:05:07.435499 OneOnOne-0.6893/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.6893/LICENSE
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-19 12:05:07.430675 OneOnOne-0.6893/OneOnOne/
+-rw-r--r--   0 sohinib    (501) staff       (20)    36452 2023-07-19 11:59:58.000000 OneOnOne-0.6893/OneOnOne/__init__.py
+-rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.6893/OneOnOne/classes.py
+-rw-r--r--   0 sohinib    (501) staff       (20)    14768 2023-07-15 09:46:38.000000 OneOnOne-0.6893/OneOnOne/classification.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     1868 2023-07-12 19:25:09.000000 OneOnOne-0.6893/OneOnOne/contextdecider.py
+-rw-r--r--   0 sohinib    (501) staff       (20)        0 2023-07-10 11:03:09.000000 OneOnOne-0.6893/OneOnOne/questionanswer.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-19 12:05:07.434494 OneOnOne-0.6893/OneOnOne.egg-info/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-19 12:05:07.000000 OneOnOne-0.6893/OneOnOne.egg-info/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)      307 2023-07-19 12:05:07.000000 OneOnOne-0.6893/OneOnOne.egg-info/SOURCES.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-19 12:05:07.000000 OneOnOne-0.6893/OneOnOne.egg-info/dependency_links.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)      120 2023-07-19 12:05:07.000000 OneOnOne-0.6893/OneOnOne.egg-info/requires.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-19 12:05:07.000000 OneOnOne-0.6893/OneOnOne.egg-info/top_level.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-19 12:05:07.435042 OneOnOne-0.6893/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)     1606 2023-07-12 20:09:33.000000 OneOnOne-0.6893/README.md
+-rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-19 12:05:07.435717 OneOnOne-0.6893/setup.cfg
+-rw-r--r--   0 sohinib    (501) staff       (20)     1919 2023-07-19 12:04:43.000000 OneOnOne-0.6893/setup.py
```

### Comparing `OneOnOne-0.6892/LICENSE` & `OneOnOne-0.6893/LICENSE`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6892/OneOnOne/__init__.py` & `OneOnOne-0.6893/OneOnOne/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         except:
             os.system(f"!gdown --id {self.map[self.model_name]}")
 
 
         for file in os.listdir(os.getcwd()):
             if file.endswith(f"{self.model_name}.zip"):
                 zip_file = ZipFile(file)
-                zip_file.extractall(self.path)
+                zip_file.extractall(os.getcwd() + f'/models_to_load/')
             else:
                 print("not found")
 
         self.model=load_model(self.path)
         self.model.summary()
```

### Comparing `OneOnOne-0.6892/OneOnOne/classes.py` & `OneOnOne-0.6893/OneOnOne/classes.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6892/OneOnOne/classification.py` & `OneOnOne-0.6893/OneOnOne/classification.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6892/OneOnOne/contextdecider.py` & `OneOnOne-0.6893/OneOnOne/contextdecider.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6892/OneOnOne.egg-info/PKG-INFO` & `OneOnOne-0.6893/OneOnOne.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.6892
+Version: 0.6893
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OneOnOne-0.6892/PKG-INFO` & `OneOnOne-0.6893/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.6892
+Version: 0.6893
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OneOnOne-0.6892/README.md` & `OneOnOne-0.6893/README.md`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6892/setup.py` & `OneOnOne-0.6893/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION=0.6892
+VERSION=0.6893
 
 
 DESCRIPTION="A package for pre-trained image classification and context-decider for question-answering chatbots."
 LONG_DESCRIPTION="Your one-stop destination to utilize image-classification models with just one line of code. A library meant to simplify your life by providing you with pre-trained models like ResNet50, EfficientNetVB6, VGG19, etc. You can simply opt for training your own models from scratch by just tweaking a few values. If you want to try popular active-learning sampling methods on image classification, no need to worry! This library has got you covered. Along with that for simple-bridging and basic into NLP, we have context-deciders, HTML parsers and simple chatbot object classes, to create an interface similar to Google Lens. You input an image or item that you are curious about and you can ask one-on-one questions from the chatbot. This is made possible by using the tiny imagenet dataset. This library is being actively updated and new features are being added frequently. New datasets and pre-trained models will be updated soon. Feel free to share your feedback! I would really appreciate it!"
 CLASSIFIERS=[
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Education',
```

