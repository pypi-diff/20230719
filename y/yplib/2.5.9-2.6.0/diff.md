# Comparing `tmp/yplib-2.5.9.tar.gz` & `tmp/yplib-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-2.5.9.tar", last modified: Mon Jul 17 02:23:25 2023, max compression
+gzip compressed data, was "dist\yplib-2.6.0.tar", last modified: Tue Jul 18 23:52:26 2023, max compression
```

## Comparing `yplib-2.5.9.tar` & `yplib-2.6.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 02:23:25.950173 yplib-2.5.9/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.5.9/LICENSE
--rw-rw-rw-   0        0        0      352 2023-07-17 02:23:25.949970 yplib-2.5.9/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.5.9/README.md
--rw-rw-rw-   0        0        0       42 2023-07-17 02:23:25.950529 yplib-2.5.9/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-07-17 02:23:06.000000 yplib-2.5.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:23:25.933169 yplib-2.5.9/yplib/
--rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.5.9/yplib/__init__.py
--rw-rw-rw-   0        0        0    10012 2023-07-10 07:39:00.000000 yplib-2.5.9/yplib/chart.py
--rw-rw-rw-   0        0        0     8406 2023-07-13 00:33:38.000000 yplib-2.5.9/yplib/chart_html.py
--rw-rw-rw-   0        0        0     1534 2023-07-10 07:30:11.000000 yplib-2.5.9/yplib/db.py
--rw-rw-rw-   0        0        0     5292 2023-07-17 02:22:22.000000 yplib-2.5.9/yplib/file.py
--rw-rw-rw-   0        0        0     6117 2023-07-11 01:16:49.000000 yplib-2.5.9/yplib/http_util.py
--rw-rw-rw-   0        0        0    33959 2023-07-17 00:29:59.000000 yplib-2.5.9/yplib/index.py
--rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.5.9/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.5.9/yplib/mail_html.py
--rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.5.9/yplib/markdown.py
--rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.5.9/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2023-07-17 02:23:25.949348 yplib-2.5.9/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-07-17 02:23:25.000000 yplib-2.5.9/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-07-17 02:23:25.000000 yplib-2.5.9/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 02:23:25.000000 yplib-2.5.9/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-17 02:23:25.000000 yplib-2.5.9/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 23:52:26.823415 yplib-2.6.0/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.6.0/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-07-18 23:52:26.823415 yplib-2.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.6.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-18 23:52:26.823415 yplib-2.6.0/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-07-18 23:50:50.000000 yplib-2.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 23:52:26.820291 yplib-2.6.0/yplib/
+-rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.6.0/yplib/__init__.py
+-rw-rw-rw-   0        0        0    10012 2023-07-10 07:39:00.000000 yplib-2.6.0/yplib/chart.py
+-rw-rw-rw-   0        0        0     8406 2023-07-13 00:33:38.000000 yplib-2.6.0/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     1534 2023-07-10 07:30:11.000000 yplib-2.6.0/yplib/db.py
+-rw-rw-rw-   0        0        0     5292 2023-07-17 02:22:22.000000 yplib-2.6.0/yplib/file.py
+-rw-rw-rw-   0        0        0     6117 2023-07-11 01:16:49.000000 yplib-2.6.0/yplib/http_util.py
+-rw-rw-rw-   0        0        0    33979 2023-07-18 09:01:03.000000 yplib-2.6.0/yplib/index.py
+-rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.6.0/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.6.0/yplib/mail_html.py
+-rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.6.0/yplib/markdown.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.6.0/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2023-07-18 23:52:26.821769 yplib-2.6.0/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-07-18 23:52:26.000000 yplib-2.6.0/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-07-18 23:52:26.000000 yplib-2.6.0/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 23:52:26.000000 yplib-2.6.0/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-18 23:52:26.000000 yplib-2.6.0/yplib.egg-info/top_level.txt
```

### Comparing `yplib-2.5.9/LICENSE` & `yplib-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-2.5.9/setup.py` & `yplib-2.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="2.5.9",
+  version="2.6.0",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-2.5.9/yplib/__init__.py` & `yplib-2.6.0/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-2.5.9/yplib/chart.py` & `yplib-2.6.0/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-2.5.9/yplib/chart_html.py` & `yplib-2.6.0/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.5.9/yplib/db.py` & `yplib-2.6.0/yplib/db.py`

 * *Files identical despite different names*

### Comparing `yplib-2.5.9/yplib/file.py` & `yplib-2.6.0/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-2.5.9/yplib/http_util.py` & `yplib-2.6.0/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-2.5.9/yplib/index.py` & `yplib-2.6.0/yplib/index.py`

 * *Files 0% similar despite different names*

```diff
@@ -375,15 +375,15 @@
     file_name = datetime.today().strftime('%Y%m%d_%H%M') if file_name is None else file_name
     return to_txt(data_list=data_list, file_name=file_name, file_path='txt', fixed_name=True)
 
 
 # 转化成字符串
 def to_str(data):
     if can_use_json(data):
-        s = json.dumps(data)
+        s = json.dumps(data, ensure_ascii=False)
     else:
         s = str(data)
     return s
 
 
 # 匹配字符串
 # 可以参考 正则表达式的操作, 可以使用 chatgpt 帮忙写出这段代码
```

### Comparing `yplib-2.5.9/yplib/mail.py` & `yplib-2.6.0/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-2.5.9/yplib/mail_html.py` & `yplib-2.6.0/yplib/mail_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.5.9/yplib/markdown.py` & `yplib-2.6.0/yplib/markdown.py`

 * *Files identical despite different names*

