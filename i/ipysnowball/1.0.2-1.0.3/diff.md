# Comparing `tmp/ipysnowball-1.0.2.tar.gz` & `tmp/ipysnowball-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipysnowball-1.0.2.tar", last modified: Wed Jul 19 09:56:58 2023, max compression
+gzip compressed data, was "ipysnowball-1.0.3.tar", last modified: Wed Jul 19 10:01:57 2023, max compression
```

## Comparing `ipysnowball-1.0.2.tar` & `ipysnowball-1.0.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 issa       (501) staff       (20)        0 2023-07-19 09:56:58.981643 ipysnowball-1.0.2/
--rw-r--r--   0 issa       (501) staff       (20)    11357 2023-06-06 08:57:00.000000 ipysnowball-1.0.2/LICENSE
--rw-r--r--   0 issa       (501) staff       (20)     2779 2023-07-19 09:56:58.980543 ipysnowball-1.0.2/PKG-INFO
--rw-r--r--   0 issa       (501) staff       (20)    70376 2023-07-19 09:56:20.000000 ipysnowball-1.0.2/README.md
-drwxr-xr-x   0 issa       (501) staff       (20)        0 2023-07-19 09:56:58.953870 ipysnowball-1.0.2/ipysnowball.egg-info/
--rw-r--r--   0 issa       (501) staff       (20)     2779 2023-07-19 09:56:58.000000 ipysnowball-1.0.2/ipysnowball.egg-info/PKG-INFO
--rw-r--r--   0 issa       (501) staff       (20)      580 2023-07-19 09:56:58.000000 ipysnowball-1.0.2/ipysnowball.egg-info/SOURCES.txt
--rw-r--r--   0 issa       (501) staff       (20)        1 2023-07-19 09:56:58.000000 ipysnowball-1.0.2/ipysnowball.egg-info/dependency_links.txt
--rw-r--r--   0 issa       (501) staff       (20)       40 2023-07-19 09:56:58.000000 ipysnowball-1.0.2/ipysnowball.egg-info/requires.txt
--rw-r--r--   0 issa       (501) staff       (20)       17 2023-07-19 09:56:58.000000 ipysnowball-1.0.2/ipysnowball.egg-info/top_level.txt
-drwxr-xr-x   0 issa       (501) staff       (20)        0 2023-07-19 09:56:58.977030 ipysnowball-1.0.2/pysnowball/
--rw-r--r--   0 issa       (501) staff       (20)     1323 2023-07-19 08:08:16.000000 ipysnowball-1.0.2/pysnowball/__init__.py
--rw-r--r--   0 issa       (501) staff       (20)     5133 2023-07-19 09:47:00.000000 ipysnowball-1.0.2/pysnowball/api_ref.py
--rw-r--r--   0 issa       (501) staff       (20)      260 2023-06-06 08:57:00.000000 ipysnowball-1.0.2/pysnowball/bond.py
--rw-r--r--   0 issa       (501) staff       (20)      826 2023-06-06 08:57:00.000000 ipysnowball-1.0.2/pysnowball/capital.py
--rw-r--r--   0 issa       (501) staff       (20)       72 2023-06-06 08:57:00.000000 ipysnowball-1.0.2/pysnowball/cons.py
--rw-r--r--   0 issa       (501) staff       (20)      381 2023-06-06 08:57:00.000000 ipysnowball-1.0.2/pysnowball/cube.py
--rw-r--r--   0 issa       (501) staff       (20)     1338 2023-06-06 08:57:00.000000 ipysnowball-1.0.2/pysnowball/f10.py
--rw-r--r--   0 issa       (501) staff       (20)     1209 2023-06-06 08:57:00.000000 ipysnowball-1.0.2/pysnowball/finance.py
--rw-r--r--   0 issa       (501) staff       (20)     1045 2023-06-06 08:57:00.000000 ipysnowball-1.0.2/pysnowball/fund.py
--rw-r--r--   0 issa       (501) staff       (20)     2737 2023-06-06 08:57:00.000000 ipysnowball-1.0.2/pysnowball/hkex.py
--rw-r--r--   0 issa       (501) staff       (20)     1272 2023-06-06 08:57:00.000000 ipysnowball-1.0.2/pysnowball/index.py
--rw-r--r--   0 issa       (501) staff       (20)      516 2023-06-06 09:07:03.000000 ipysnowball-1.0.2/pysnowball/realtime.py
--rw-r--r--   0 issa       (501) staff       (20)      311 2023-06-06 08:57:00.000000 ipysnowball-1.0.2/pysnowball/report.py
--rw-r--r--   0 issa       (501) staff       (20)      419 2023-07-19 09:53:21.000000 ipysnowball-1.0.2/pysnowball/scan.py
--rw-r--r--   0 issa       (501) staff       (20)      302 2023-06-06 08:57:00.000000 ipysnowball-1.0.2/pysnowball/token.py
--rw-r--r--   0 issa       (501) staff       (20)      222 2023-06-06 08:57:00.000000 ipysnowball-1.0.2/pysnowball/user.py
--rw-r--r--   0 issa       (501) staff       (20)     4284 2023-06-06 08:57:00.000000 ipysnowball-1.0.2/pysnowball/utls.py
--rw-r--r--   0 issa       (501) staff       (20)       38 2023-07-19 09:56:58.981878 ipysnowball-1.0.2/setup.cfg
--rw-r--r--   0 issa       (501) staff       (20)     3253 2023-07-19 09:55:18.000000 ipysnowball-1.0.2/setup.py
-drwxr-xr-x   0 issa       (501) staff       (20)        0 2023-07-19 09:56:58.979059 ipysnowball-1.0.2/tests/
--rw-r--r--   0 issa       (501) staff       (20)        0 2023-06-06 08:57:00.000000 ipysnowball-1.0.2/tests/__init__.py
--rw-r--r--   0 issa       (501) staff       (20)     1178 2023-06-06 08:57:00.000000 ipysnowball-1.0.2/tests/test_fund.py
+drwxr-xr-x   0 issa       (501) staff       (20)        0 2023-07-19 10:01:57.267482 ipysnowball-1.0.3/
+-rw-r--r--   0 issa       (501) staff       (20)    11357 2023-06-06 08:57:00.000000 ipysnowball-1.0.3/LICENSE
+-rw-r--r--   0 issa       (501) staff       (20)     2779 2023-07-19 10:01:57.266348 ipysnowball-1.0.3/PKG-INFO
+-rw-r--r--   0 issa       (501) staff       (20)    70376 2023-07-19 09:56:20.000000 ipysnowball-1.0.3/README.md
+drwxr-xr-x   0 issa       (501) staff       (20)        0 2023-07-19 10:01:57.209426 ipysnowball-1.0.3/ipysnowball.egg-info/
+-rw-r--r--   0 issa       (501) staff       (20)     2779 2023-07-19 10:01:57.000000 ipysnowball-1.0.3/ipysnowball.egg-info/PKG-INFO
+-rw-r--r--   0 issa       (501) staff       (20)      580 2023-07-19 10:01:57.000000 ipysnowball-1.0.3/ipysnowball.egg-info/SOURCES.txt
+-rw-r--r--   0 issa       (501) staff       (20)        1 2023-07-19 10:01:57.000000 ipysnowball-1.0.3/ipysnowball.egg-info/dependency_links.txt
+-rw-r--r--   0 issa       (501) staff       (20)       40 2023-07-19 10:01:57.000000 ipysnowball-1.0.3/ipysnowball.egg-info/requires.txt
+-rw-r--r--   0 issa       (501) staff       (20)       17 2023-07-19 10:01:57.000000 ipysnowball-1.0.3/ipysnowball.egg-info/top_level.txt
+drwxr-xr-x   0 issa       (501) staff       (20)        0 2023-07-19 10:01:57.263534 ipysnowball-1.0.3/pysnowball/
+-rw-r--r--   0 issa       (501) staff       (20)     1323 2023-07-19 08:08:16.000000 ipysnowball-1.0.3/pysnowball/__init__.py
+-rw-r--r--   0 issa       (501) staff       (20)     5133 2023-07-19 09:47:00.000000 ipysnowball-1.0.3/pysnowball/api_ref.py
+-rw-r--r--   0 issa       (501) staff       (20)      260 2023-06-06 08:57:00.000000 ipysnowball-1.0.3/pysnowball/bond.py
+-rw-r--r--   0 issa       (501) staff       (20)      826 2023-06-06 08:57:00.000000 ipysnowball-1.0.3/pysnowball/capital.py
+-rw-r--r--   0 issa       (501) staff       (20)       72 2023-06-06 08:57:00.000000 ipysnowball-1.0.3/pysnowball/cons.py
+-rw-r--r--   0 issa       (501) staff       (20)      381 2023-06-06 08:57:00.000000 ipysnowball-1.0.3/pysnowball/cube.py
+-rw-r--r--   0 issa       (501) staff       (20)     1338 2023-06-06 08:57:00.000000 ipysnowball-1.0.3/pysnowball/f10.py
+-rw-r--r--   0 issa       (501) staff       (20)     1209 2023-06-06 08:57:00.000000 ipysnowball-1.0.3/pysnowball/finance.py
+-rw-r--r--   0 issa       (501) staff       (20)     1045 2023-06-06 08:57:00.000000 ipysnowball-1.0.3/pysnowball/fund.py
+-rw-r--r--   0 issa       (501) staff       (20)     2737 2023-06-06 08:57:00.000000 ipysnowball-1.0.3/pysnowball/hkex.py
+-rw-r--r--   0 issa       (501) staff       (20)     1272 2023-06-06 08:57:00.000000 ipysnowball-1.0.3/pysnowball/index.py
+-rw-r--r--   0 issa       (501) staff       (20)      516 2023-06-06 09:07:03.000000 ipysnowball-1.0.3/pysnowball/realtime.py
+-rw-r--r--   0 issa       (501) staff       (20)      311 2023-06-06 08:57:00.000000 ipysnowball-1.0.3/pysnowball/report.py
+-rw-r--r--   0 issa       (501) staff       (20)      419 2023-07-19 10:01:28.000000 ipysnowball-1.0.3/pysnowball/scan.py
+-rw-r--r--   0 issa       (501) staff       (20)      302 2023-06-06 08:57:00.000000 ipysnowball-1.0.3/pysnowball/token.py
+-rw-r--r--   0 issa       (501) staff       (20)      222 2023-06-06 08:57:00.000000 ipysnowball-1.0.3/pysnowball/user.py
+-rw-r--r--   0 issa       (501) staff       (20)     4280 2023-07-19 10:01:31.000000 ipysnowball-1.0.3/pysnowball/utls.py
+-rw-r--r--   0 issa       (501) staff       (20)       38 2023-07-19 10:01:57.267736 ipysnowball-1.0.3/setup.cfg
+-rw-r--r--   0 issa       (501) staff       (20)     3253 2023-07-19 10:01:36.000000 ipysnowball-1.0.3/setup.py
+drwxr-xr-x   0 issa       (501) staff       (20)        0 2023-07-19 10:01:57.265242 ipysnowball-1.0.3/tests/
+-rw-r--r--   0 issa       (501) staff       (20)        0 2023-06-06 08:57:00.000000 ipysnowball-1.0.3/tests/__init__.py
+-rw-r--r--   0 issa       (501) staff       (20)     1178 2023-06-06 08:57:00.000000 ipysnowball-1.0.3/tests/test_fund.py
```

### Comparing `ipysnowball-1.0.2/LICENSE` & `ipysnowball-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ipysnowball-1.0.2/PKG-INFO` & `ipysnowball-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipysnowball
-Version: 1.0.2
+Version: 1.0.3
 Summary: 原版雪球Python API pysnowball 的修改
 Home-page: https://github.com/issaTan/pysnowball
 Author: IssaTan
 Author-email: tanxinhao.1990@gmail.com
 Keywords: Financial Data,XueQiu,Snow Ball,雪球,Python Api
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ipysnowball-1.0.2/README.md` & `ipysnowball-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ipysnowball-1.0.2/ipysnowball.egg-info/PKG-INFO` & `ipysnowball-1.0.3/ipysnowball.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipysnowball
-Version: 1.0.2
+Version: 1.0.3
 Summary: 原版雪球Python API pysnowball 的修改
 Home-page: https://github.com/issaTan/pysnowball
 Author: IssaTan
 Author-email: tanxinhao.1990@gmail.com
 Keywords: Financial Data,XueQiu,Snow Ball,雪球,Python Api
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ipysnowball-1.0.2/ipysnowball.egg-info/SOURCES.txt` & `ipysnowball-1.0.3/ipysnowball.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ipysnowball-1.0.2/pysnowball/__init__.py` & `ipysnowball-1.0.3/pysnowball/__init__.py`

 * *Files identical despite different names*

### Comparing `ipysnowball-1.0.2/pysnowball/api_ref.py` & `ipysnowball-1.0.3/pysnowball/api_ref.py`

 * *Files identical despite different names*

### Comparing `ipysnowball-1.0.2/pysnowball/capital.py` & `ipysnowball-1.0.3/pysnowball/capital.py`

 * *Files identical despite different names*

### Comparing `ipysnowball-1.0.2/pysnowball/f10.py` & `ipysnowball-1.0.3/pysnowball/f10.py`

 * *Files identical despite different names*

### Comparing `ipysnowball-1.0.2/pysnowball/finance.py` & `ipysnowball-1.0.3/pysnowball/finance.py`

 * *Files identical despite different names*

### Comparing `ipysnowball-1.0.2/pysnowball/fund.py` & `ipysnowball-1.0.3/pysnowball/fund.py`

 * *Files identical despite different names*

### Comparing `ipysnowball-1.0.2/pysnowball/hkex.py` & `ipysnowball-1.0.3/pysnowball/hkex.py`

 * *Files identical despite different names*

### Comparing `ipysnowball-1.0.2/pysnowball/index.py` & `ipysnowball-1.0.3/pysnowball/index.py`

 * *Files identical despite different names*

### Comparing `ipysnowball-1.0.2/pysnowball/realtime.py` & `ipysnowball-1.0.3/pysnowball/realtime.py`

 * *Files identical despite different names*

### Comparing `ipysnowball-1.0.2/pysnowball/utls.py` & `ipysnowball-1.0.3/pysnowball/utls.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,17 +12,17 @@
                'User-Agent': 'Xueqiu iPhone 11.8',
                'Accept-Language': 'zh-Hans-CN;q=1, ja-JP;q=0.9',
                'Accept-Encoding': 'br, gzip, deflate',
                'Connection': 'keep-alive'}
 
     response = requests.get(url, headers=HEADERS)
 
-    # print(url)
+    print(url)
     # print(HEADERS)
-    # print(response)
+    print(response)
     # print(response.content)
 
     if response.status_code != 200:
         raise Exception(response.content)
 
     return json.loads(response.content)
```

### Comparing `ipysnowball-1.0.2/setup.py` & `ipysnowball-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         'requests >= 2.18.4',
         'beautifulsoup4 >= 4.10.0'
     ]
     return reqs
 
 setuptools.setup(
     name="ipysnowball",
-    version="1.0.2",
+    version="1.0.3",
     author="IssaTan",
     author_email="tanxinhao.1990@gmail.com",
     description="原版雪球Python API pysnowball 的修改",
     long_description=long_desc,
     long_description_content_type="text/markdown",
     url="https://github.com/issaTan/pysnowball",
     packages=setuptools.find_packages(),
```

### Comparing `ipysnowball-1.0.2/tests/test_fund.py` & `ipysnowball-1.0.3/tests/test_fund.py`

 * *Files identical despite different names*

