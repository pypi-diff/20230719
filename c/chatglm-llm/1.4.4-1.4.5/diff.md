# Comparing `tmp/chatglm-llm-1.4.4.tar.gz` & `tmp/chatglm-llm-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatglm-llm-1.4.4.tar", last modified: Tue Jul  4 07:13:05 2023, max compression
+gzip compressed data, was "chatglm-llm-1.4.5.tar", last modified: Wed Jul 19 07:05:39 2023, max compression
```

## Comparing `chatglm-llm-1.4.4.tar` & `chatglm-llm-1.4.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-07-04 07:13:05.594086 chatglm-llm-1.4.4/
--rw-r--r--   0 mroy       (501) staff       (20)       36 2023-05-10 01:48:15.000000 chatglm-llm-1.4.4/MANIFEST.in
--rw-r--r--   0 mroy       (501) staff       (20)      212 2023-07-04 07:13:05.593963 chatglm-llm-1.4.4/PKG-INFO
--rw-r--r--   0 mroy       (501) staff       (20)     1887 2023-05-04 01:08:28.000000 chatglm-llm-1.4.4/README.md
-drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-07-04 07:13:05.592478 chatglm-llm-1.4.4/chatglm_llm.egg-info/
--rw-r--r--   0 mroy       (501) staff       (20)      212 2023-07-04 07:13:05.000000 chatglm-llm-1.4.4/chatglm_llm.egg-info/PKG-INFO
--rw-r--r--   0 mroy       (501) staff       (20)      540 2023-07-04 07:13:05.000000 chatglm-llm-1.4.4/chatglm_llm.egg-info/SOURCES.txt
--rw-r--r--   0 mroy       (501) staff       (20)        1 2023-07-04 07:13:05.000000 chatglm-llm-1.4.4/chatglm_llm.egg-info/dependency_links.txt
--rw-r--r--   0 mroy       (501) staff       (20)       53 2023-07-04 07:13:05.000000 chatglm-llm-1.4.4/chatglm_llm.egg-info/entry_points.txt
--rw-r--r--   0 mroy       (501) staff       (20)        1 2023-05-04 01:12:10.000000 chatglm-llm-1.4.4/chatglm_llm.egg-info/not-zip-safe
--rw-r--r--   0 mroy       (501) staff       (20)      266 2023-07-04 07:13:05.000000 chatglm-llm-1.4.4/chatglm_llm.egg-info/requires.txt
--rw-r--r--   0 mroy       (501) staff       (20)       12 2023-07-04 07:13:05.000000 chatglm-llm-1.4.4/chatglm_llm.egg-info/top_level.txt
-drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-07-04 07:13:05.593361 chatglm-llm-1.4.4/chatglm_src/
--rw-r--r--   0 mroy       (501) staff       (20)      755 2023-06-16 02:41:40.000000 chatglm-llm-1.4.4/chatglm_src/__init__.py
--rw-r--r--   0 mroy       (501) staff       (20)     4201 2023-05-13 02:36:58.000000 chatglm-llm-1.4.4/chatglm_src/callbacks.py
-drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-07-04 07:13:05.593650 chatglm-llm-1.4.4/chatglm_src/chains/
--rw-r--r--   0 mroy       (501) staff       (20)       69 2023-05-10 01:48:15.000000 chatglm-llm-1.4.4/chatglm_src/chains/__init__.py
--rw-r--r--   0 mroy       (501) staff       (20)     4402 2023-05-11 09:17:21.000000 chatglm-llm-1.4.4/chatglm_src/chains/local_qa.py
--rw-r--r--   0 mroy       (501) staff       (20)     2272 2023-06-28 08:26:21.000000 chatglm-llm-1.4.4/chatglm_src/chatglm_utils.py
--rw-r--r--   0 mroy       (501) staff       (20)     2785 2023-07-04 07:10:48.000000 chatglm-llm-1.4.4/chatglm_src/cluster_and_smi.py
--rw-r--r--   0 mroy       (501) staff       (20)      537 2023-05-30 04:20:56.000000 chatglm-llm-1.4.4/chatglm_src/cmd.py
--rw-r--r--   0 mroy       (501) staff       (20)     3235 2023-07-04 07:11:23.000000 chatglm-llm-1.4.4/chatglm_src/embeding.py
--rw-r--r--   0 mroy       (501) staff       (20)    41882 2023-07-04 07:12:19.000000 chatglm-llm-1.4.4/chatglm_src/llm.py
-drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-07-04 07:13:05.593795 chatglm-llm-1.4.4/chatglm_src/loader/
--rw-r--r--   0 mroy       (501) staff       (20)     1403 2023-05-11 01:28:05.000000 chatglm-llm-1.4.4/chatglm_src/loader/__init__.py
--rw-r--r--   0 mroy       (501) staff       (20)       38 2023-07-04 07:13:05.594127 chatglm-llm-1.4.4/setup.cfg
--rw-r--r--   0 mroy       (501) staff       (20)     1078 2023-07-04 07:12:38.000000 chatglm-llm-1.4.4/setup.py
+drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-07-19 07:05:39.880321 chatglm-llm-1.4.5/
+-rw-r--r--   0 mroy       (501) staff       (20)       36 2023-05-10 01:48:15.000000 chatglm-llm-1.4.5/MANIFEST.in
+-rw-r--r--   0 mroy       (501) staff       (20)      212 2023-07-19 07:05:39.880211 chatglm-llm-1.4.5/PKG-INFO
+-rw-r--r--   0 mroy       (501) staff       (20)     1887 2023-05-04 01:08:28.000000 chatglm-llm-1.4.5/README.md
+drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-07-19 07:05:39.878947 chatglm-llm-1.4.5/chatglm_llm.egg-info/
+-rw-r--r--   0 mroy       (501) staff       (20)      212 2023-07-19 07:05:39.000000 chatglm-llm-1.4.5/chatglm_llm.egg-info/PKG-INFO
+-rw-r--r--   0 mroy       (501) staff       (20)      540 2023-07-19 07:05:39.000000 chatglm-llm-1.4.5/chatglm_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 mroy       (501) staff       (20)        1 2023-07-19 07:05:39.000000 chatglm-llm-1.4.5/chatglm_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 mroy       (501) staff       (20)       53 2023-07-19 07:05:39.000000 chatglm-llm-1.4.5/chatglm_llm.egg-info/entry_points.txt
+-rw-r--r--   0 mroy       (501) staff       (20)        1 2023-05-04 01:12:10.000000 chatglm-llm-1.4.5/chatglm_llm.egg-info/not-zip-safe
+-rw-r--r--   0 mroy       (501) staff       (20)      276 2023-07-19 07:05:39.000000 chatglm-llm-1.4.5/chatglm_llm.egg-info/requires.txt
+-rw-r--r--   0 mroy       (501) staff       (20)       12 2023-07-19 07:05:39.000000 chatglm-llm-1.4.5/chatglm_llm.egg-info/top_level.txt
+drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-07-19 07:05:39.879689 chatglm-llm-1.4.5/chatglm_src/
+-rw-r--r--   0 mroy       (501) staff       (20)      755 2023-06-16 02:41:40.000000 chatglm-llm-1.4.5/chatglm_src/__init__.py
+-rw-r--r--   0 mroy       (501) staff       (20)     4201 2023-05-13 02:36:58.000000 chatglm-llm-1.4.5/chatglm_src/callbacks.py
+drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-07-19 07:05:39.879944 chatglm-llm-1.4.5/chatglm_src/chains/
+-rw-r--r--   0 mroy       (501) staff       (20)       69 2023-05-10 01:48:15.000000 chatglm-llm-1.4.5/chatglm_src/chains/__init__.py
+-rw-r--r--   0 mroy       (501) staff       (20)     4402 2023-05-11 09:17:21.000000 chatglm-llm-1.4.5/chatglm_src/chains/local_qa.py
+-rw-r--r--   0 mroy       (501) staff       (20)     2272 2023-06-28 08:26:21.000000 chatglm-llm-1.4.5/chatglm_src/chatglm_utils.py
+-rw-r--r--   0 mroy       (501) staff       (20)     2876 2023-07-19 07:04:40.000000 chatglm-llm-1.4.5/chatglm_src/cluster_and_smi.py
+-rw-r--r--   0 mroy       (501) staff       (20)      537 2023-05-30 04:20:56.000000 chatglm-llm-1.4.5/chatglm_src/cmd.py
+-rw-r--r--   0 mroy       (501) staff       (20)     3235 2023-07-04 07:11:23.000000 chatglm-llm-1.4.5/chatglm_src/embeding.py
+-rw-r--r--   0 mroy       (501) staff       (20)    41882 2023-07-04 07:12:19.000000 chatglm-llm-1.4.5/chatglm_src/llm.py
+drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-07-19 07:05:39.880050 chatglm-llm-1.4.5/chatglm_src/loader/
+-rw-r--r--   0 mroy       (501) staff       (20)     1403 2023-05-11 01:28:05.000000 chatglm-llm-1.4.5/chatglm_src/loader/__init__.py
+-rw-r--r--   0 mroy       (501) staff       (20)       38 2023-07-19 07:05:39.880360 chatglm-llm-1.4.5/setup.cfg
+-rw-r--r--   0 mroy       (501) staff       (20)     1103 2023-07-19 07:05:00.000000 chatglm-llm-1.4.5/setup.py
```

### Comparing `chatglm-llm-1.4.4/README.md` & `chatglm-llm-1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.4.4/chatglm_llm.egg-info/SOURCES.txt` & `chatglm-llm-1.4.5/chatglm_llm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.4.4/chatglm_src/__init__.py` & `chatglm-llm-1.4.5/chatglm_src/__init__.py`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.4.4/chatglm_src/callbacks.py` & `chatglm-llm-1.4.5/chatglm_src/callbacks.py`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.4.4/chatglm_src/chains/local_qa.py` & `chatglm-llm-1.4.5/chatglm_src/chains/local_qa.py`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.4.4/chatglm_src/chatglm_utils.py` & `chatglm-llm-1.4.5/chatglm_src/chatglm_utils.py`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.4.4/chatglm_src/cluster_and_smi.py` & `chatglm-llm-1.4.5/chatglm_src/cluster_and_smi.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from websocket import create_connection
 import datetime
 import time
 from hashlib import md5
 import json
 from termcolor import colored
 import tqdm
+import termcolor
 
 
 def cluster(data, n_clusters=2,eps=0.5,min_samples=3, method='kmeans'):
     
     if method == 'kmeans':
         kmeans = KMeans(n_clusters=n_clusters, random_state=0, n_init='auto').fit(data)
         return kmeans.labels_
@@ -63,20 +64,20 @@
     })
     msg = send_and_recv(data, ws)
     return msg
 
 
 def send_and_recv(data, ws):
     try:
-        for i in tqdm.tqdm(range(0, len(data), 1024*102), desc="sending data"):
+        for i in tqdm.tqdm(range(0, len(data), 1024*102), desc=termcolor.colored(" + sending data","cyan")):
             ws.send(data[i:i+1024*102])
         ws.send("[STOP]")
         message = ""
         total = int(ws.recv())
-        bar = tqdm.tqdm(desc="receiving data", total=total)
+        bar = tqdm.tqdm(desc=termcolor.colored(" + receiving data","cyan", attrs=["bold"]), total=total)
         while 1:
             res = ws.recv()
             message += res
             bar.update(len(res))
             if message.endswith("[STOP]"):
                 message = message[:-6]
                 break
```

### Comparing `chatglm-llm-1.4.4/chatglm_src/cmd.py` & `chatglm-llm-1.4.5/chatglm_src/cmd.py`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.4.4/chatglm_src/embeding.py` & `chatglm-llm-1.4.5/chatglm_src/embeding.py`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.4.4/chatglm_src/llm.py` & `chatglm-llm-1.4.5/chatglm_src/llm.py`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.4.4/chatglm_src/loader/__init__.py` & `chatglm-llm-1.4.5/chatglm_src/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.4.4/setup.py` & `chatglm-llm-1.4.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 
 setup(name='chatglm-llm',
-    version='1.4.4',
+    version='1.4.5',
     description='chatglm llm',
     url='https://github.com/xxx',
     author='auth',
     author_email='xxx@gmail.com',
     license='MIT',
     include_package_data=True,
     zip_safe=False,
@@ -20,14 +20,15 @@
             "fschat==0.2.2",
             "cpm_kernels",
             "mdtex2html",
             "sentencepiece",
             "accelerate",
             "scikit-learn",
             'torch',    
+            'termcolor',
             'transformers',
         ],
     },
     install_requires=[
         'requests',
         'termcolor',
         'tqdm',
```

