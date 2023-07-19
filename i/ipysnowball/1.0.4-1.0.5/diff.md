# Comparing `tmp/ipysnowball-1.0.4.tar.gz` & `tmp/ipysnowball-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipysnowball-1.0.4.tar", last modified: Wed Jul 19 10:07:33 2023, max compression
+gzip compressed data, was "ipysnowball-1.0.5.tar", last modified: Wed Jul 19 13:55:23 2023, max compression
```

## Comparing `ipysnowball-1.0.4.tar` & `ipysnowball-1.0.5.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 issa       (501) staff       (20)        0 2023-07-19 10:07:33.467707 ipysnowball-1.0.4/
--rw-r--r--   0 issa       (501) staff       (20)    11357 2023-06-06 08:57:00.000000 ipysnowball-1.0.4/LICENSE
--rw-r--r--   0 issa       (501) staff       (20)     2779 2023-07-19 10:07:33.466317 ipysnowball-1.0.4/PKG-INFO
--rw-r--r--   0 issa       (501) staff       (20)    70376 2023-07-19 09:56:20.000000 ipysnowball-1.0.4/README.md
-drwxr-xr-x   0 issa       (501) staff       (20)        0 2023-07-19 10:07:33.436895 ipysnowball-1.0.4/ipysnowball.egg-info/
--rw-r--r--   0 issa       (501) staff       (20)     2779 2023-07-19 10:07:33.000000 ipysnowball-1.0.4/ipysnowball.egg-info/PKG-INFO
--rw-r--r--   0 issa       (501) staff       (20)      580 2023-07-19 10:07:33.000000 ipysnowball-1.0.4/ipysnowball.egg-info/SOURCES.txt
--rw-r--r--   0 issa       (501) staff       (20)        1 2023-07-19 10:07:33.000000 ipysnowball-1.0.4/ipysnowball.egg-info/dependency_links.txt
--rw-r--r--   0 issa       (501) staff       (20)       40 2023-07-19 10:07:33.000000 ipysnowball-1.0.4/ipysnowball.egg-info/requires.txt
--rw-r--r--   0 issa       (501) staff       (20)       17 2023-07-19 10:07:33.000000 ipysnowball-1.0.4/ipysnowball.egg-info/top_level.txt
-drwxr-xr-x   0 issa       (501) staff       (20)        0 2023-07-19 10:07:33.460496 ipysnowball-1.0.4/pysnowball/
--rw-r--r--   0 issa       (501) staff       (20)     1323 2023-07-19 08:08:16.000000 ipysnowball-1.0.4/pysnowball/__init__.py
--rw-r--r--   0 issa       (501) staff       (20)     5133 2023-07-19 09:47:00.000000 ipysnowball-1.0.4/pysnowball/api_ref.py
--rw-r--r--   0 issa       (501) staff       (20)      260 2023-06-06 08:57:00.000000 ipysnowball-1.0.4/pysnowball/bond.py
--rw-r--r--   0 issa       (501) staff       (20)      826 2023-06-06 08:57:00.000000 ipysnowball-1.0.4/pysnowball/capital.py
--rw-r--r--   0 issa       (501) staff       (20)       72 2023-06-06 08:57:00.000000 ipysnowball-1.0.4/pysnowball/cons.py
--rw-r--r--   0 issa       (501) staff       (20)      381 2023-06-06 08:57:00.000000 ipysnowball-1.0.4/pysnowball/cube.py
--rw-r--r--   0 issa       (501) staff       (20)     1338 2023-06-06 08:57:00.000000 ipysnowball-1.0.4/pysnowball/f10.py
--rw-r--r--   0 issa       (501) staff       (20)     1209 2023-06-06 08:57:00.000000 ipysnowball-1.0.4/pysnowball/finance.py
--rw-r--r--   0 issa       (501) staff       (20)     1045 2023-06-06 08:57:00.000000 ipysnowball-1.0.4/pysnowball/fund.py
--rw-r--r--   0 issa       (501) staff       (20)     2737 2023-06-06 08:57:00.000000 ipysnowball-1.0.4/pysnowball/hkex.py
--rw-r--r--   0 issa       (501) staff       (20)     1272 2023-06-06 08:57:00.000000 ipysnowball-1.0.4/pysnowball/index.py
--rw-r--r--   0 issa       (501) staff       (20)      516 2023-06-06 09:07:03.000000 ipysnowball-1.0.4/pysnowball/realtime.py
--rw-r--r--   0 issa       (501) staff       (20)      311 2023-06-06 08:57:00.000000 ipysnowball-1.0.4/pysnowball/report.py
--rw-r--r--   0 issa       (501) staff       (20)      419 2023-07-19 10:01:28.000000 ipysnowball-1.0.4/pysnowball/scan.py
--rw-r--r--   0 issa       (501) staff       (20)      302 2023-06-06 08:57:00.000000 ipysnowball-1.0.4/pysnowball/token.py
--rw-r--r--   0 issa       (501) staff       (20)      222 2023-06-06 08:57:00.000000 ipysnowball-1.0.4/pysnowball/user.py
--rw-r--r--   0 issa       (501) staff       (20)     4276 2023-07-19 10:07:15.000000 ipysnowball-1.0.4/pysnowball/utls.py
--rw-r--r--   0 issa       (501) staff       (20)       38 2023-07-19 10:07:33.467929 ipysnowball-1.0.4/setup.cfg
--rw-r--r--   0 issa       (501) staff       (20)     3253 2023-07-19 10:07:21.000000 ipysnowball-1.0.4/setup.py
-drwxr-xr-x   0 issa       (501) staff       (20)        0 2023-07-19 10:07:33.464483 ipysnowball-1.0.4/tests/
--rw-r--r--   0 issa       (501) staff       (20)        0 2023-06-06 08:57:00.000000 ipysnowball-1.0.4/tests/__init__.py
--rw-r--r--   0 issa       (501) staff       (20)     1178 2023-06-06 08:57:00.000000 ipysnowball-1.0.4/tests/test_fund.py
+drwxr-xr-x   0 issa       (501) staff       (20)        0 2023-07-19 13:55:23.109001 ipysnowball-1.0.5/
+-rw-r--r--   0 issa       (501) staff       (20)    11357 2023-06-06 08:57:00.000000 ipysnowball-1.0.5/LICENSE
+-rw-r--r--   0 issa       (501) staff       (20)     2779 2023-07-19 13:55:23.093800 ipysnowball-1.0.5/PKG-INFO
+-rw-r--r--   0 issa       (501) staff       (20)    70376 2023-07-19 09:56:20.000000 ipysnowball-1.0.5/README.md
+drwxr-xr-x   0 issa       (501) staff       (20)        0 2023-07-19 13:55:22.987819 ipysnowball-1.0.5/ipysnowball.egg-info/
+-rw-r--r--   0 issa       (501) staff       (20)     2779 2023-07-19 13:55:22.000000 ipysnowball-1.0.5/ipysnowball.egg-info/PKG-INFO
+-rw-r--r--   0 issa       (501) staff       (20)      599 2023-07-19 13:55:22.000000 ipysnowball-1.0.5/ipysnowball.egg-info/SOURCES.txt
+-rw-r--r--   0 issa       (501) staff       (20)        1 2023-07-19 13:55:22.000000 ipysnowball-1.0.5/ipysnowball.egg-info/dependency_links.txt
+-rw-r--r--   0 issa       (501) staff       (20)       40 2023-07-19 13:55:22.000000 ipysnowball-1.0.5/ipysnowball.egg-info/requires.txt
+-rw-r--r--   0 issa       (501) staff       (20)       17 2023-07-19 13:55:22.000000 ipysnowball-1.0.5/ipysnowball.egg-info/top_level.txt
+drwxr-xr-x   0 issa       (501) staff       (20)        0 2023-07-19 13:55:23.080479 ipysnowball-1.0.5/pysnowball/
+-rw-r--r--   0 issa       (501) staff       (20)     1323 2023-07-19 08:08:16.000000 ipysnowball-1.0.5/pysnowball/__init__.py
+-rw-r--r--   0 issa       (501) staff       (20)     5133 2023-07-19 09:47:00.000000 ipysnowball-1.0.5/pysnowball/api_ref.py
+-rw-r--r--   0 issa       (501) staff       (20)      260 2023-06-06 08:57:00.000000 ipysnowball-1.0.5/pysnowball/bond.py
+-rw-r--r--   0 issa       (501) staff       (20)      826 2023-06-06 08:57:00.000000 ipysnowball-1.0.5/pysnowball/capital.py
+-rw-r--r--   0 issa       (501) staff       (20)       72 2023-06-06 08:57:00.000000 ipysnowball-1.0.5/pysnowball/cons.py
+-rw-r--r--   0 issa       (501) staff       (20)      381 2023-06-06 08:57:00.000000 ipysnowball-1.0.5/pysnowball/cube.py
+-rw-r--r--   0 issa       (501) staff       (20)     1338 2023-06-06 08:57:00.000000 ipysnowball-1.0.5/pysnowball/f10.py
+-rw-r--r--   0 issa       (501) staff       (20)     1209 2023-06-06 08:57:00.000000 ipysnowball-1.0.5/pysnowball/finance.py
+-rw-r--r--   0 issa       (501) staff       (20)     1045 2023-06-06 08:57:00.000000 ipysnowball-1.0.5/pysnowball/fund.py
+-rw-r--r--   0 issa       (501) staff       (20)     2737 2023-06-06 08:57:00.000000 ipysnowball-1.0.5/pysnowball/hkex.py
+-rw-r--r--   0 issa       (501) staff       (20)     1272 2023-06-06 08:57:00.000000 ipysnowball-1.0.5/pysnowball/index.py
+-rw-r--r--   0 issa       (501) staff       (20)      516 2023-06-06 09:07:03.000000 ipysnowball-1.0.5/pysnowball/realtime.py
+-rw-r--r--   0 issa       (501) staff       (20)      311 2023-06-06 08:57:00.000000 ipysnowball-1.0.5/pysnowball/report.py
+-rw-r--r--   0 issa       (501) staff       (20)      405 2023-07-19 13:53:53.000000 ipysnowball-1.0.5/pysnowball/scan.py
+-rw-r--r--   0 issa       (501) staff       (20)      302 2023-06-06 08:57:00.000000 ipysnowball-1.0.5/pysnowball/token.py
+-rw-r--r--   0 issa       (501) staff       (20)      222 2023-06-06 08:57:00.000000 ipysnowball-1.0.5/pysnowball/user.py
+-rw-r--r--   0 issa       (501) staff       (20)     4284 2023-07-19 13:53:32.000000 ipysnowball-1.0.5/pysnowball/utls.py
+-rw-r--r--   0 issa       (501) staff       (20)       38 2023-07-19 13:55:23.109367 ipysnowball-1.0.5/setup.cfg
+-rw-r--r--   0 issa       (501) staff       (20)     3253 2023-07-19 13:54:30.000000 ipysnowball-1.0.5/setup.py
+drwxr-xr-x   0 issa       (501) staff       (20)        0 2023-07-19 13:55:23.089903 ipysnowball-1.0.5/tests/
+-rw-r--r--   0 issa       (501) staff       (20)        0 2023-06-06 08:57:00.000000 ipysnowball-1.0.5/tests/__init__.py
+-rw-r--r--   0 issa       (501) staff       (20)     1178 2023-06-06 08:57:00.000000 ipysnowball-1.0.5/tests/test_fund.py
+-rw-r--r--   0 issa       (501) staff       (20)      425 2023-07-19 13:54:24.000000 ipysnowball-1.0.5/tests/test_scan.py
```

### Comparing `ipysnowball-1.0.4/LICENSE` & `ipysnowball-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ipysnowball-1.0.4/PKG-INFO` & `ipysnowball-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipysnowball
-Version: 1.0.4
+Version: 1.0.5
 Summary: 原版雪球Python API pysnowball 的修改
 Home-page: https://github.com/issaTan/pysnowball
 Author: IssaTan
 Author-email: tanxinhao.1990@gmail.com
 Keywords: Financial Data,XueQiu,Snow Ball,雪球,Python Api
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ipysnowball-1.0.4/README.md` & `ipysnowball-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ipysnowball-1.0.4/ipysnowball.egg-info/PKG-INFO` & `ipysnowball-1.0.5/ipysnowball.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipysnowball
-Version: 1.0.4
+Version: 1.0.5
 Summary: 原版雪球Python API pysnowball 的修改
 Home-page: https://github.com/issaTan/pysnowball
 Author: IssaTan
 Author-email: tanxinhao.1990@gmail.com
 Keywords: Financial Data,XueQiu,Snow Ball,雪球,Python Api
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ipysnowball-1.0.4/ipysnowball.egg-info/SOURCES.txt` & `ipysnowball-1.0.5/ipysnowball.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,8 +20,9 @@
 pysnowball/realtime.py
 pysnowball/report.py
 pysnowball/scan.py
 pysnowball/token.py
 pysnowball/user.py
 pysnowball/utls.py
 tests/__init__.py
-tests/test_fund.py
+tests/test_fund.py
+tests/test_scan.py
```

### Comparing `ipysnowball-1.0.4/pysnowball/__init__.py` & `ipysnowball-1.0.5/pysnowball/__init__.py`

 * *Files identical despite different names*

### Comparing `ipysnowball-1.0.4/pysnowball/api_ref.py` & `ipysnowball-1.0.5/pysnowball/api_ref.py`

 * *Files identical despite different names*

### Comparing `ipysnowball-1.0.4/pysnowball/capital.py` & `ipysnowball-1.0.5/pysnowball/capital.py`

 * *Files identical despite different names*

### Comparing `ipysnowball-1.0.4/pysnowball/f10.py` & `ipysnowball-1.0.5/pysnowball/f10.py`

 * *Files identical despite different names*

### Comparing `ipysnowball-1.0.4/pysnowball/finance.py` & `ipysnowball-1.0.5/pysnowball/finance.py`

 * *Files identical despite different names*

### Comparing `ipysnowball-1.0.4/pysnowball/fund.py` & `ipysnowball-1.0.5/pysnowball/fund.py`

 * *Files identical despite different names*

### Comparing `ipysnowball-1.0.4/pysnowball/hkex.py` & `ipysnowball-1.0.5/pysnowball/hkex.py`

 * *Files identical despite different names*

### Comparing `ipysnowball-1.0.4/pysnowball/index.py` & `ipysnowball-1.0.5/pysnowball/index.py`

 * *Files identical despite different names*

### Comparing `ipysnowball-1.0.4/pysnowball/realtime.py` & `ipysnowball-1.0.5/pysnowball/realtime.py`

 * *Files identical despite different names*

### Comparing `ipysnowball-1.0.4/pysnowball/utls.py` & `ipysnowball-1.0.5/pysnowball/utls.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,18 +12,18 @@
                'User-Agent': 'Xueqiu iPhone 11.8',
                'Accept-Language': 'zh-Hans-CN;q=1, ja-JP;q=0.9',
                'Accept-Encoding': 'br, gzip, deflate',
                'Connection': 'keep-alive'}
 
     response = requests.get(url, headers=HEADERS)
 
-    print(url)
-    print(HEADERS)
-    print(response)
-    print(response.content)
+    # print(url)
+    # print(HEADERS)
+    # print(response)
+    # print(response.content)
 
     if response.status_code != 200:
         raise Exception(response.content)
 
     return json.loads(response.content)
```

### Comparing `ipysnowball-1.0.4/setup.py` & `ipysnowball-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         'requests >= 2.18.4',
         'beautifulsoup4 >= 4.10.0'
     ]
     return reqs
 
 setuptools.setup(
     name="ipysnowball",
-    version="1.0.4",
+    version="1.0.5",
     author="IssaTan",
     author_email="tanxinhao.1990@gmail.com",
     description="原版雪球Python API pysnowball 的修改",
     long_description=long_desc,
     long_description_content_type="text/markdown",
     url="https://github.com/issaTan/pysnowball",
     packages=setuptools.find_packages(),
```

### Comparing `ipysnowball-1.0.4/tests/test_fund.py` & `ipysnowball-1.0.5/tests/test_fund.py`

 * *Files identical despite different names*

