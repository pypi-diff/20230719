# Comparing `tmp/mayfpayapi-1.4.6.tar.gz` & `tmp/mayfpayapi-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mayfpayapi-1.4.6.tar", last modified: Fri Jun 30 16:15:17 2023, max compression
+gzip compressed data, was "mayfpayapi-1.5.1.tar", last modified: Wed Jul 19 07:11:08 2023, max compression
```

## Comparing `mayfpayapi-1.4.6.tar` & `mayfpayapi-1.5.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 dimamayfeed   (502) staff       (20)        0 2023-06-30 16:15:17.697151 mayfpayapi-1.4.6/
--rw-r--r--   0 dimamayfeed   (502) staff       (20)      642 2023-06-30 16:15:17.696961 mayfpayapi-1.4.6/PKG-INFO
--rw-r--r--   0 dimamayfeed   (502) staff       (20)        0 2023-06-30 09:26:33.000000 mayfpayapi-1.4.6/README.md
-drwxr-xr-x   0 dimamayfeed   (502) staff       (20)        0 2023-06-30 16:15:17.695463 mayfpayapi-1.4.6/mayfpayapi/
--rw-r--r--   0 dimamayfeed   (502) staff       (20)       25 2023-06-30 14:21:04.000000 mayfpayapi-1.4.6/mayfpayapi/__init__.py
--rw-r--r--   0 dimamayfeed   (502) staff       (20)     4279 2023-06-30 16:14:57.000000 mayfpayapi-1.4.6/mayfpayapi/mayfpayapi.py
-drwxr-xr-x   0 dimamayfeed   (502) staff       (20)        0 2023-06-30 16:15:17.696669 mayfpayapi-1.4.6/mayfpayapi.egg-info/
--rw-r--r--   0 dimamayfeed   (502) staff       (20)      642 2023-06-30 16:15:17.000000 mayfpayapi-1.4.6/mayfpayapi.egg-info/PKG-INFO
--rw-r--r--   0 dimamayfeed   (502) staff       (20)      235 2023-06-30 16:15:17.000000 mayfpayapi-1.4.6/mayfpayapi.egg-info/SOURCES.txt
--rw-r--r--   0 dimamayfeed   (502) staff       (20)        1 2023-06-30 16:15:17.000000 mayfpayapi-1.4.6/mayfpayapi.egg-info/dependency_links.txt
--rw-r--r--   0 dimamayfeed   (502) staff       (20)        9 2023-06-30 16:15:17.000000 mayfpayapi-1.4.6/mayfpayapi.egg-info/requires.txt
--rw-r--r--   0 dimamayfeed   (502) staff       (20)       11 2023-06-30 16:15:17.000000 mayfpayapi-1.4.6/mayfpayapi.egg-info/top_level.txt
--rw-r--r--   0 dimamayfeed   (502) staff       (20)       38 2023-06-30 16:15:17.697216 mayfpayapi-1.4.6/setup.cfg
--rw-r--r--   0 dimamayfeed   (502) staff       (20)      979 2023-06-30 16:15:03.000000 mayfpayapi-1.4.6/setup.py
+drwxr-xr-x   0 dimamayfeed   (502) staff       (20)        0 2023-07-19 07:11:08.720821 mayfpayapi-1.5.1/
+-rw-r--r--   0 dimamayfeed   (502) staff       (20)     1794 2023-07-19 07:11:08.720634 mayfpayapi-1.5.1/PKG-INFO
+-rw-r--r--   0 dimamayfeed   (502) staff       (20)     1241 2023-07-19 07:07:33.000000 mayfpayapi-1.5.1/README.md
+drwxr-xr-x   0 dimamayfeed   (502) staff       (20)        0 2023-07-19 07:11:08.719176 mayfpayapi-1.5.1/mayfpayapi/
+-rw-r--r--   0 dimamayfeed   (502) staff       (20)       26 2023-04-10 18:23:23.000000 mayfpayapi-1.5.1/mayfpayapi/__init__.py
+-rw-r--r--   0 dimamayfeed   (502) staff       (20)     2646 2023-07-19 07:06:17.000000 mayfpayapi-1.5.1/mayfpayapi/mayfpayapi.py
+drwxr-xr-x   0 dimamayfeed   (502) staff       (20)        0 2023-07-19 07:11:08.720363 mayfpayapi-1.5.1/mayfpayapi.egg-info/
+-rw-r--r--   0 dimamayfeed   (502) staff       (20)     1794 2023-07-19 07:11:08.000000 mayfpayapi-1.5.1/mayfpayapi.egg-info/PKG-INFO
+-rw-r--r--   0 dimamayfeed   (502) staff       (20)      235 2023-07-19 07:11:08.000000 mayfpayapi-1.5.1/mayfpayapi.egg-info/SOURCES.txt
+-rw-r--r--   0 dimamayfeed   (502) staff       (20)        1 2023-07-19 07:11:08.000000 mayfpayapi-1.5.1/mayfpayapi.egg-info/dependency_links.txt
+-rw-r--r--   0 dimamayfeed   (502) staff       (20)        9 2023-07-19 07:11:08.000000 mayfpayapi-1.5.1/mayfpayapi.egg-info/requires.txt
+-rw-r--r--   0 dimamayfeed   (502) staff       (20)       11 2023-07-19 07:11:08.000000 mayfpayapi-1.5.1/mayfpayapi.egg-info/top_level.txt
+-rw-r--r--   0 dimamayfeed   (502) staff       (20)       38 2023-07-19 07:11:08.720900 mayfpayapi-1.5.1/setup.cfg
+-rw-r--r--   0 dimamayfeed   (502) staff       (20)      892 2023-07-19 07:08:49.000000 mayfpayapi-1.5.1/setup.py
```

### Comparing `mayfpayapi-1.4.6/setup.py` & `mayfpayapi-1.5.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='mayfpayapi',
-    version='1.4.6',
-    author='MayfPay.top',
+    version='1.5.1',
+    author='MayfPay',
     author_email='support@mayfpay.top',
-    description='MayfPayApi is a Python library for interacting with the MayfPay payment system API.',
-    long_description=long_description,
-    long_description_content_type='text/markdown',
+    description='MayfPayApi is a Python library for interacting with the MayfPay payment system API. It provides methods for retrieving kassa balances, creating and checking invoices.',
     url='https://github.com/MAYFPAY/MayfPayApi',
     packages=find_packages(),
-    classifiers=[
-        'Programming Language :: Python :: 3',
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: OS Independent',
-    ],
+    py_modules=['mayfpayapi'],
     project_urls={
         'Source': 'https://github.com/MAYFPAY/MayfPayApi',
         'Documentation': 'https://mayfpay.top/docs',
         'Bug Reports': 'https://github.com/MAYFPAY/MayfPayApi/issues',
     },
-    python_requires='>=3.6',
+    long_description=long_description,
+    long_description_content_type="text/markdown",
     install_requires=[
         'requests',
     ],
 )
```

