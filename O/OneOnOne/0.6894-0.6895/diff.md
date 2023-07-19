# Comparing `tmp/OneOnOne-0.6894.tar.gz` & `tmp/OneOnOne-0.6895.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OneOnOne-0.6894.tar", last modified: Wed Jul 19 12:42:00 2023, max compression
+gzip compressed data, was "OneOnOne-0.6895.tar", last modified: Wed Jul 19 12:45:32 2023, max compression
```

## Comparing `OneOnOne-0.6894.tar` & `OneOnOne-0.6895.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-19 12:42:00.083147 OneOnOne-0.6894/
--rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.6894/LICENSE
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-19 12:42:00.080558 OneOnOne-0.6894/OneOnOne/
--rw-r--r--   0 sohinib    (501) staff       (20)    37788 2023-07-19 12:41:40.000000 OneOnOne-0.6894/OneOnOne/__init__.py
--rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.6894/OneOnOne/classes.py
--rw-r--r--   0 sohinib    (501) staff       (20)    14768 2023-07-15 09:46:38.000000 OneOnOne-0.6894/OneOnOne/classification.py
--rw-r--r--   0 sohinib    (501) staff       (20)     1868 2023-07-12 19:25:09.000000 OneOnOne-0.6894/OneOnOne/contextdecider.py
--rw-r--r--   0 sohinib    (501) staff       (20)        0 2023-07-10 11:03:09.000000 OneOnOne-0.6894/OneOnOne/questionanswer.py
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-19 12:42:00.082269 OneOnOne-0.6894/OneOnOne.egg-info/
--rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-19 12:41:59.000000 OneOnOne-0.6894/OneOnOne.egg-info/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)      307 2023-07-19 12:42:00.000000 OneOnOne-0.6894/OneOnOne.egg-info/SOURCES.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-19 12:41:59.000000 OneOnOne-0.6894/OneOnOne.egg-info/dependency_links.txt
--rw-r--r--   0 sohinib    (501) staff       (20)      120 2023-07-19 12:41:59.000000 OneOnOne-0.6894/OneOnOne.egg-info/requires.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-19 12:41:59.000000 OneOnOne-0.6894/OneOnOne.egg-info/top_level.txt
--rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-19 12:42:00.082723 OneOnOne-0.6894/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)     1606 2023-07-12 20:09:33.000000 OneOnOne-0.6894/README.md
--rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-19 12:42:00.083271 OneOnOne-0.6894/setup.cfg
--rw-r--r--   0 sohinib    (501) staff       (20)     1919 2023-07-19 12:41:51.000000 OneOnOne-0.6894/setup.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-19 12:45:32.750360 OneOnOne-0.6895/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.6895/LICENSE
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-19 12:45:32.743457 OneOnOne-0.6895/OneOnOne/
+-rw-r--r--   0 sohinib    (501) staff       (20)    37802 2023-07-19 12:45:04.000000 OneOnOne-0.6895/OneOnOne/__init__.py
+-rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.6895/OneOnOne/classes.py
+-rw-r--r--   0 sohinib    (501) staff       (20)    14768 2023-07-15 09:46:38.000000 OneOnOne-0.6895/OneOnOne/classification.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     1868 2023-07-12 19:25:09.000000 OneOnOne-0.6895/OneOnOne/contextdecider.py
+-rw-r--r--   0 sohinib    (501) staff       (20)        0 2023-07-10 11:03:09.000000 OneOnOne-0.6895/OneOnOne/questionanswer.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-19 12:45:32.748529 OneOnOne-0.6895/OneOnOne.egg-info/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-19 12:45:32.000000 OneOnOne-0.6895/OneOnOne.egg-info/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)      307 2023-07-19 12:45:32.000000 OneOnOne-0.6895/OneOnOne.egg-info/SOURCES.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-19 12:45:32.000000 OneOnOne-0.6895/OneOnOne.egg-info/dependency_links.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)      120 2023-07-19 12:45:32.000000 OneOnOne-0.6895/OneOnOne.egg-info/requires.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-19 12:45:32.000000 OneOnOne-0.6895/OneOnOne.egg-info/top_level.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-19 12:45:32.749571 OneOnOne-0.6895/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)     1606 2023-07-12 20:09:33.000000 OneOnOne-0.6895/README.md
+-rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-19 12:45:32.750689 OneOnOne-0.6895/setup.cfg
+-rw-r--r--   0 sohinib    (501) staff       (20)     1919 2023-07-19 12:45:26.000000 OneOnOne-0.6895/setup.py
```

### Comparing `OneOnOne-0.6894/LICENSE` & `OneOnOne-0.6895/LICENSE`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6894/OneOnOne/__init__.py` & `OneOnOne-0.6895/OneOnOne/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -325,14 +325,15 @@
             train_filenames = train_it.filenames
             val_filenames = val_it.filenames
             number_of_val_samples = len(val_filenames)
             number_of_train_samples = len(train_filenames)
             # class_mode='categorical',
             print(number_of_train_samples)
             print(number_of_val_samples)
+        else:
             if self.dataset == "cifar10":
                 classes = ['airplane', 'automobile', 'bird', 'cat', 'deer', 'dog', 'frog', 'horse', 'ship', 'truck']
                 num_classes = len(classes)
                 (training_images, training_labels), (
                     validation_images, validation_labels) = tf.keras.datasets.cifar10.load_data()
 
                 train_X = self.preprocess_image_input(training_images)
```

### Comparing `OneOnOne-0.6894/OneOnOne/classes.py` & `OneOnOne-0.6895/OneOnOne/classes.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6894/OneOnOne/classification.py` & `OneOnOne-0.6895/OneOnOne/classification.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6894/OneOnOne/contextdecider.py` & `OneOnOne-0.6895/OneOnOne/contextdecider.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6894/OneOnOne.egg-info/PKG-INFO` & `OneOnOne-0.6895/OneOnOne.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.6894
+Version: 0.6895
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OneOnOne-0.6894/PKG-INFO` & `OneOnOne-0.6895/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.6894
+Version: 0.6895
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OneOnOne-0.6894/README.md` & `OneOnOne-0.6895/README.md`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6894/setup.py` & `OneOnOne-0.6895/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION=0.6894
+VERSION=0.6895
 
 
 DESCRIPTION="A package for pre-trained image classification and context-decider for question-answering chatbots."
 LONG_DESCRIPTION="Your one-stop destination to utilize image-classification models with just one line of code. A library meant to simplify your life by providing you with pre-trained models like ResNet50, EfficientNetVB6, VGG19, etc. You can simply opt for training your own models from scratch by just tweaking a few values. If you want to try popular active-learning sampling methods on image classification, no need to worry! This library has got you covered. Along with that for simple-bridging and basic into NLP, we have context-deciders, HTML parsers and simple chatbot object classes, to create an interface similar to Google Lens. You input an image or item that you are curious about and you can ask one-on-one questions from the chatbot. This is made possible by using the tiny imagenet dataset. This library is being actively updated and new features are being added frequently. New datasets and pre-trained models will be updated soon. Feel free to share your feedback! I would really appreciate it!"
 CLASSIFIERS=[
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Education',
```

