# Comparing `tmp/qingxun-openapi-python-sdk-0.2.0.tar.gz` & `tmp/qingxun-openapi-python-sdk-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\qingxun-openapi-python-sdk-0.2.0.tar", last modified: Wed Jul 19 09:36:00 2023, max compression
+gzip compressed data, was "dist\qingxun-openapi-python-sdk-1.0.tar", last modified: Sun Apr 23 08:32:37 2023, max compression
```

## Comparing `qingxun-openapi-python-sdk-0.2.0.tar` & `qingxun-openapi-python-sdk-1.0.tar`

### file list

```diff
@@ -1,22 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 09:36:00.000000 qingxun-openapi-python-sdk-0.2.0/
--rw-rw-rw-   0        0        0       97 2023-07-19 09:36:00.000000 qingxun-openapi-python-sdk-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     6439 2023-07-19 09:18:45.000000 qingxun-openapi-python-sdk-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-19 09:36:00.000000 qingxun-openapi-python-sdk-0.2.0/TranslateApi/
--rw-rw-rw-   0        0        0      970 2023-07-19 09:34:41.000000 qingxun-openapi-python-sdk-0.2.0/TranslateApi/account.py
--rw-rw-rw-   0        0        0     2119 2023-07-19 09:34:41.000000 qingxun-openapi-python-sdk-0.2.0/TranslateApi/audio_trans.py
--rw-rw-rw-   0        0        0      886 2023-07-19 09:34:41.000000 qingxun-openapi-python-sdk-0.2.0/TranslateApi/dict_search.py
--rw-rw-rw-   0        0        0     1364 2023-07-19 09:34:41.000000 qingxun-openapi-python-sdk-0.2.0/TranslateApi/doc_convert.py
--rw-rw-rw-   0        0        0     6413 2023-07-19 09:34:41.000000 qingxun-openapi-python-sdk-0.2.0/TranslateApi/document_translation.py
--rw-rw-rw-   0        0        0     2813 2023-07-19 09:34:41.000000 qingxun-openapi-python-sdk-0.2.0/TranslateApi/image_trans.py
--rw-rw-rw-   0        0        0     1303 2023-07-19 09:34:41.000000 qingxun-openapi-python-sdk-0.2.0/TranslateApi/ocr.py
--rw-rw-rw-   0        0        0      592 2023-07-19 03:18:50.000000 qingxun-openapi-python-sdk-0.2.0/TranslateApi/preproccess.py
--rw-rw-rw-   0        0        0      934 2023-07-19 09:34:50.000000 qingxun-openapi-python-sdk-0.2.0/TranslateApi/text_trans.py
--rw-rw-rw-   0        0        0     3749 2023-07-19 09:34:41.000000 qingxun-openapi-python-sdk-0.2.0/TranslateApi/voice_trans.py
-drwxrwxrwx   0        0        0        0 2023-07-19 09:36:00.000000 qingxun-openapi-python-sdk-0.2.0/qingxun_openapi_python_sdk.egg-info/
--rw-rw-rw-   0        0        0       97 2023-07-19 09:36:00.000000 qingxun-openapi-python-sdk-0.2.0/qingxun_openapi_python_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      543 2023-07-19 09:36:00.000000 qingxun-openapi-python-sdk-0.2.0/qingxun_openapi_python_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 09:36:00.000000 qingxun-openapi-python-sdk-0.2.0/qingxun_openapi_python_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-07-19 09:36:00.000000 qingxun-openapi-python-sdk-0.2.0/qingxun_openapi_python_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-19 09:36:00.000000 qingxun-openapi-python-sdk-0.2.0/qingxun_openapi_python_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-19 09:36:00.000000 qingxun-openapi-python-sdk-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      298 2023-07-19 09:35:56.000000 qingxun-openapi-python-sdk-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 08:32:37.000000 qingxun-openapi-python-sdk-1.0/
+-rw-rw-rw-   0        0        0        0 2023-03-24 06:09:13.000000 qingxun-openapi-python-sdk-1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      227 2023-04-23 08:32:37.000000 qingxun-openapi-python-sdk-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-03-24 06:08:00.000000 qingxun-openapi-python-sdk-1.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-23 08:32:37.000000 qingxun-openapi-python-sdk-1.0/qingxun_openapi_python_sdk.egg-info/
+-rw-rw-rw-   0        0        0      227 2023-04-23 08:32:37.000000 qingxun-openapi-python-sdk-1.0/qingxun_openapi_python_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2023-04-23 08:32:37.000000 qingxun-openapi-python-sdk-1.0/qingxun_openapi_python_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 08:32:37.000000 qingxun-openapi-python-sdk-1.0/qingxun_openapi_python_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-23 08:32:37.000000 qingxun-openapi-python-sdk-1.0/qingxun_openapi_python_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 08:32:37.000000 qingxun-openapi-python-sdk-1.0/qingxunsdk/
+drwxrwxrwx   0        0        0        0 2023-04-23 08:32:37.000000 qingxun-openapi-python-sdk-1.0/qingxunsdk/TranslateApi/
+-rw-rw-rw-   0        0        0        0 2023-03-24 03:49:28.000000 qingxun-openapi-python-sdk-1.0/qingxunsdk/TranslateApi/__init__.py
+-rw-rw-rw-   0        0        0    18213 2023-04-20 07:17:35.000000 qingxun-openapi-python-sdk-1.0/qingxunsdk/TranslateApi/qxkjApi.py
+-rw-rw-rw-   0        0        0        0 2023-03-24 06:19:23.000000 qingxun-openapi-python-sdk-1.0/qingxunsdk/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-04-23 08:32:37.000000 qingxun-openapi-python-sdk-1.0/setup.cfg
+-rw-rw-rw-   0        0        0      504 2023-04-23 08:08:51.000000 qingxun-openapi-python-sdk-1.0/setup.py
```

