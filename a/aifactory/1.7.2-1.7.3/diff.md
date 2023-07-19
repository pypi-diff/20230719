# Comparing `tmp/aifactory-1.7.2.tar.gz` & `tmp/aifactory-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aifactory-1.7.2.tar", last modified: Sun Jul 16 03:49:57 2023, max compression
+gzip compressed data, was "aifactory-1.7.3.tar", last modified: Wed Jul 19 08:29:14 2023, max compression
```

## Comparing `aifactory-1.7.2.tar` & `aifactory-1.7.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-07-16 03:49:57.018251 aifactory-1.7.2/
--rw-r--r--   0 kyj        (501) staff       (20)      228 2023-07-16 03:49:57.018100 aifactory-1.7.2/PKG-INFO
-drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-07-16 03:49:57.017124 aifactory-1.7.2/aifactory/
--rw-r--r--   0 kyj        (501) staff       (20)        0 2023-05-10 03:11:14.000000 aifactory-1.7.2/aifactory/__init__.py
--rw-r--r--   0 kyj        (501) staff       (20)     3743 2023-05-10 03:11:14.000000 aifactory-1.7.2/aifactory/api.py
--rw-r--r--   0 kyj        (501) staff       (20)     3710 2023-05-10 03:11:14.000000 aifactory-1.7.2/aifactory/demo.py
--rw-r--r--   0 kyj        (501) staff       (20)    14314 2023-05-10 03:11:14.000000 aifactory-1.7.2/aifactory/grade.py
--rw-r--r--   0 kyj        (501) staff       (20)     5966 2023-05-10 03:11:14.000000 aifactory-1.7.2/aifactory/make_zip.py
--rw-r--r--   0 kyj        (501) staff       (20)     7466 2023-07-16 03:49:36.000000 aifactory-1.7.2/aifactory/score.py
--rw-r--r--   0 kyj        (501) staff       (20)       50 2023-05-10 03:11:14.000000 aifactory-1.7.2/aifactory/train.py
-drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-07-16 03:49:57.017895 aifactory-1.7.2/aifactory.egg-info/
--rw-r--r--   0 kyj        (501) staff       (20)      228 2023-07-16 03:49:56.000000 aifactory-1.7.2/aifactory.egg-info/PKG-INFO
--rw-r--r--   0 kyj        (501) staff       (20)      308 2023-07-16 03:49:56.000000 aifactory-1.7.2/aifactory.egg-info/SOURCES.txt
--rw-r--r--   0 kyj        (501) staff       (20)        1 2023-07-16 03:49:56.000000 aifactory-1.7.2/aifactory.egg-info/dependency_links.txt
--rw-r--r--   0 kyj        (501) staff       (20)       41 2023-07-16 03:49:56.000000 aifactory-1.7.2/aifactory.egg-info/requires.txt
--rw-r--r--   0 kyj        (501) staff       (20)       17 2023-07-16 03:49:56.000000 aifactory-1.7.2/aifactory.egg-info/top_level.txt
--rw-r--r--   0 kyj        (501) staff       (20)       38 2023-07-16 03:49:57.018303 aifactory-1.7.2/setup.cfg
--rw-r--r--   0 kyj        (501) staff       (20)      430 2023-07-16 03:48:59.000000 aifactory-1.7.2/setup.py
+drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-07-19 08:29:14.576268 aifactory-1.7.3/
+-rw-r--r--   0 kyj        (501) staff       (20)      228 2023-07-19 08:29:14.576099 aifactory-1.7.3/PKG-INFO
+drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-07-19 08:29:14.574999 aifactory-1.7.3/aifactory/
+-rw-r--r--   0 kyj        (501) staff       (20)        0 2023-05-10 03:11:14.000000 aifactory-1.7.3/aifactory/__init__.py
+-rw-r--r--   0 kyj        (501) staff       (20)     3743 2023-05-10 03:11:14.000000 aifactory-1.7.3/aifactory/api.py
+-rw-r--r--   0 kyj        (501) staff       (20)     3710 2023-05-10 03:11:14.000000 aifactory-1.7.3/aifactory/demo.py
+-rw-r--r--   0 kyj        (501) staff       (20)    14314 2023-05-10 03:11:14.000000 aifactory-1.7.3/aifactory/grade.py
+-rw-r--r--   0 kyj        (501) staff       (20)     5966 2023-05-10 03:11:14.000000 aifactory-1.7.3/aifactory/make_zip.py
+-rw-r--r--   0 kyj        (501) staff       (20)     7503 2023-07-19 08:14:00.000000 aifactory-1.7.3/aifactory/score.py
+-rw-r--r--   0 kyj        (501) staff       (20)       50 2023-05-10 03:11:14.000000 aifactory-1.7.3/aifactory/train.py
+drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-07-19 08:29:14.575881 aifactory-1.7.3/aifactory.egg-info/
+-rw-r--r--   0 kyj        (501) staff       (20)      228 2023-07-19 08:29:14.000000 aifactory-1.7.3/aifactory.egg-info/PKG-INFO
+-rw-r--r--   0 kyj        (501) staff       (20)      308 2023-07-19 08:29:14.000000 aifactory-1.7.3/aifactory.egg-info/SOURCES.txt
+-rw-r--r--   0 kyj        (501) staff       (20)        1 2023-07-19 08:29:14.000000 aifactory-1.7.3/aifactory.egg-info/dependency_links.txt
+-rw-r--r--   0 kyj        (501) staff       (20)       41 2023-07-19 08:29:14.000000 aifactory-1.7.3/aifactory.egg-info/requires.txt
+-rw-r--r--   0 kyj        (501) staff       (20)       17 2023-07-19 08:29:14.000000 aifactory-1.7.3/aifactory.egg-info/top_level.txt
+-rw-r--r--   0 kyj        (501) staff       (20)       38 2023-07-19 08:29:14.576327 aifactory-1.7.3/setup.cfg
+-rw-r--r--   0 kyj        (501) staff       (20)      430 2023-07-19 08:29:11.000000 aifactory-1.7.3/setup.py
```

### Comparing `aifactory-1.7.2/aifactory/api.py` & `aifactory-1.7.3/aifactory/api.py`

 * *Files identical despite different names*

### Comparing `aifactory-1.7.2/aifactory/demo.py` & `aifactory-1.7.3/aifactory/demo.py`

 * *Files identical despite different names*

### Comparing `aifactory-1.7.2/aifactory/grade.py` & `aifactory-1.7.3/aifactory/grade.py`

 * *Files identical despite different names*

### Comparing `aifactory-1.7.2/aifactory/make_zip.py` & `aifactory-1.7.3/aifactory/make_zip.py`

 * *Files identical despite different names*

### Comparing `aifactory-1.7.2/aifactory/score.py` & `aifactory-1.7.3/aifactory/score.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,17 +102,18 @@
     main_name = ipynbname.name()
   except Exception as e:
     main_name = "task.py"
 
   print("file : {0}".format(main_name))
   make_zip(main_name)
   
-  with open('./aif.zip', 'rb') as f:
-    data = f.read()
+  # with open('./aif.zip', 'rb') as f:
+  #   data = f.read()
 
+  file = open('./aif.zip', 'rb')
   try:        
     submitData = {"key" : key, "modelname" : model_name, "requestID": "0", "fileName": "0"}    
     res = requests.post(bridgeUrl + "/submit", json=submitData)
     if res.status_code != 200:
       print("중계서버 오류")
       return 
     
@@ -150,15 +151,15 @@
         return
     else :
       print("파일 전송 오류")       
       return
     res = requests.put(
       signedUrl,
       headers={'Content-Type': "application/octet-stream"},
-      data=data
+      data=file
     ) 
 
     if res.status_code != 200 :
       print("파일 전송 오류")       
       return 
     
     submitData = {"key" : key, "modelname" : model_name, "requestID": requestID, "fileName": fileName}
```

