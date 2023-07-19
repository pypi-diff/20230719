# Comparing `tmp/tair-1.3.4.tar.gz` & `tmp/tair-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tair-1.3.4.tar", last modified: Tue May 30 11:01:38 2023, max compression
+gzip compressed data, was "tair-1.3.5.tar", last modified: Wed Jul 19 09:27:01 2023, max compression
```

## Comparing `tair-1.3.4.tar` & `tair-1.3.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 yangbodong   (502) staff       (20)        0 2023-05-30 11:01:38.163755 tair-1.3.4/
--rw-r--r--   0 yangbodong   (502) staff       (20)     1064 2022-07-27 06:08:53.000000 tair-1.3.4/LICENSE
--rw-r--r--   0 yangbodong   (502) staff       (20)     4659 2023-05-30 11:01:38.163536 tair-1.3.4/PKG-INFO
--rw-r--r--   0 yangbodong   (502) staff       (20)     4378 2023-05-06 06:15:53.000000 tair-1.3.4/README.md
--rw-r--r--   0 yangbodong   (502) staff       (20)       38 2023-05-30 11:01:38.163815 tair-1.3.4/setup.cfg
--rwxr-xr-x   0 yangbodong   (502) staff       (20)      488 2023-05-30 11:00:40.000000 tair-1.3.4/setup.py
-drwxr-xr-x   0 yangbodong   (502) staff       (20)        0 2023-05-30 11:01:38.135491 tair-1.3.4/tair/
--rw-r--r--   0 yangbodong   (502) staff       (20)     1557 2023-02-17 07:55:24.000000 tair-1.3.4/tair/__init__.py
-drwxr-xr-x   0 yangbodong   (502) staff       (20)        0 2023-05-30 11:01:38.156460 tair-1.3.4/tair/asyncio/
--rw-r--r--   0 yangbodong   (502) staff       (20)     1412 2022-08-16 03:42:18.000000 tair-1.3.4/tair/asyncio/__init__.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     3293 2023-01-05 06:47:04.000000 tair-1.3.4/tair/asyncio/client.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     1639 2023-01-05 07:08:21.000000 tair-1.3.4/tair/asyncio/cluster.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     1005 2023-01-05 06:47:04.000000 tair-1.3.4/tair/asyncio/pipeline.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     3308 2022-08-16 03:42:18.000000 tair-1.3.4/tair/client.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     1866 2022-08-16 03:42:18.000000 tair-1.3.4/tair/cluster.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     5361 2023-02-17 07:55:24.000000 tair-1.3.4/tair/commands.py
--rw-r--r--   0 yangbodong   (502) staff       (20)      334 2022-07-27 06:08:53.000000 tair-1.3.4/tair/exceptions.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     1184 2022-08-16 03:42:18.000000 tair-1.3.4/tair/pipeline.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     1582 2022-08-16 03:42:18.000000 tair-1.3.4/tair/tairbloom.py
--rw-r--r--   0 yangbodong   (502) staff       (20)    11976 2022-09-01 08:46:46.000000 tair-1.3.4/tair/taircpc.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     3156 2022-08-25 09:35:31.000000 tair-1.3.4/tair/tairdoc.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     5190 2022-08-25 09:35:31.000000 tair-1.3.4/tair/tairgis.py
--rw-r--r--   0 yangbodong   (502) staff       (20)    14354 2022-08-25 09:35:31.000000 tair-1.3.4/tair/tairhash.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     4944 2022-08-16 03:42:18.000000 tair-1.3.4/tair/tairroaring.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     6759 2023-04-10 02:26:45.000000 tair-1.3.4/tair/tairsearch.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     9196 2023-01-05 06:47:04.000000 tair-1.3.4/tair/tairstring.py
--rw-r--r--   0 yangbodong   (502) staff       (20)    13708 2022-09-01 08:46:46.000000 tair-1.3.4/tair/tairts.py
--rw-r--r--   0 yangbodong   (502) staff       (20)    14123 2023-04-28 05:48:28.000000 tair-1.3.4/tair/tairvector.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     7377 2022-08-16 03:42:18.000000 tair-1.3.4/tair/tairzset.py
--rw-r--r--   0 yangbodong   (502) staff       (20)      259 2022-08-16 03:42:18.000000 tair-1.3.4/tair/typing.py
-drwxr-xr-x   0 yangbodong   (502) staff       (20)        0 2023-05-30 11:01:38.154450 tair-1.3.4/tair.egg-info/
--rw-r--r--   0 yangbodong   (502) staff       (20)     4659 2023-05-30 11:01:38.000000 tair-1.3.4/tair.egg-info/PKG-INFO
--rw-r--r--   0 yangbodong   (502) staff       (20)      874 2023-05-30 11:01:38.000000 tair-1.3.4/tair.egg-info/SOURCES.txt
--rw-r--r--   0 yangbodong   (502) staff       (20)        1 2023-05-30 11:01:38.000000 tair-1.3.4/tair.egg-info/dependency_links.txt
--rw-r--r--   0 yangbodong   (502) staff       (20)       13 2023-05-30 11:01:38.000000 tair-1.3.4/tair.egg-info/requires.txt
--rw-r--r--   0 yangbodong   (502) staff       (20)        5 2023-05-30 11:01:38.000000 tair-1.3.4/tair.egg-info/top_level.txt
-drwxr-xr-x   0 yangbodong   (502) staff       (20)        0 2023-05-30 11:01:38.163135 tair-1.3.4/tests/
--rw-r--r--   0 yangbodong   (502) staff       (20)     2256 2023-01-05 07:58:42.000000 tair-1.3.4/tests/test_from_url.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     2223 2023-01-05 06:47:04.000000 tair-1.3.4/tests/test_pipeline.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     2484 2022-08-16 03:42:18.000000 tair-1.3.4/tests/test_tairbloom.py
--rw-r--r--   0 yangbodong   (502) staff       (20)    24057 2022-09-01 08:46:46.000000 tair-1.3.4/tests/test_taircpc.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     4708 2022-08-25 09:35:31.000000 tair-1.3.4/tests/test_tairdoc.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     8533 2022-08-25 09:35:31.000000 tair-1.3.4/tests/test_tairgis.py
--rw-r--r--   0 yangbodong   (502) staff       (20)    41035 2022-08-16 03:42:18.000000 tair-1.3.4/tests/test_tairhash.py
--rw-r--r--   0 yangbodong   (502) staff       (20)     9432 2022-08-16 03:42:18.000000 tair-1.3.4/tests/test_tairroaring.py
--rw-r--r--   0 yangbodong   (502) staff       (20)    18793 2023-04-10 02:26:45.000000 tair-1.3.4/tests/test_tairsearch.py
--rw-r--r--   0 yangbodong   (502) staff       (20)    19152 2022-08-16 03:42:18.000000 tair-1.3.4/tests/test_tairstring.py
--rw-r--r--   0 yangbodong   (502) staff       (20)    13908 2022-09-01 08:46:46.000000 tair-1.3.4/tests/test_tairts.py
--rw-r--r--   0 yangbodong   (502) staff       (20)    16155 2023-04-28 05:48:28.000000 tair-1.3.4/tests/test_tairvector.py
--rw-r--r--   0 yangbodong   (502) staff       (20)    23955 2022-08-16 03:42:18.000000 tair-1.3.4/tests/test_tairzset.py
+drwxr-xr-x   0 yangbodong   (502) staff       (20)        0 2023-07-19 09:27:01.606902 tair-1.3.5/
+-rw-r--r--   0 yangbodong   (502) staff       (20)     1064 2022-07-27 06:08:53.000000 tair-1.3.5/LICENSE
+-rw-r--r--   0 yangbodong   (502) staff       (20)     4569 2023-07-19 09:27:01.606374 tair-1.3.5/PKG-INFO
+-rw-r--r--   0 yangbodong   (502) staff       (20)     4288 2023-07-19 08:57:03.000000 tair-1.3.5/README.md
+-rw-r--r--   0 yangbodong   (502) staff       (20)       38 2023-07-19 09:27:01.607028 tair-1.3.5/setup.cfg
+-rwxr-xr-x   0 yangbodong   (502) staff       (20)      488 2023-07-19 09:24:03.000000 tair-1.3.5/setup.py
+drwxr-xr-x   0 yangbodong   (502) staff       (20)        0 2023-07-19 09:27:01.594006 tair-1.3.5/tair/
+-rw-r--r--   0 yangbodong   (502) staff       (20)     1557 2023-02-17 07:55:24.000000 tair-1.3.5/tair/__init__.py
+drwxr-xr-x   0 yangbodong   (502) staff       (20)        0 2023-07-19 09:27:01.598028 tair-1.3.5/tair/asyncio/
+-rw-r--r--   0 yangbodong   (502) staff       (20)     1412 2022-08-16 03:42:18.000000 tair-1.3.5/tair/asyncio/__init__.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     3293 2023-01-05 06:47:04.000000 tair-1.3.5/tair/asyncio/client.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     1639 2023-01-05 07:08:21.000000 tair-1.3.5/tair/asyncio/cluster.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     1005 2023-01-05 06:47:04.000000 tair-1.3.5/tair/asyncio/pipeline.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     3308 2022-08-16 03:42:18.000000 tair-1.3.5/tair/client.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     1866 2022-08-16 03:42:18.000000 tair-1.3.5/tair/cluster.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     5361 2023-02-17 07:55:24.000000 tair-1.3.5/tair/commands.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)      334 2022-07-27 06:08:53.000000 tair-1.3.5/tair/exceptions.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     1184 2022-08-16 03:42:18.000000 tair-1.3.5/tair/pipeline.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     1582 2022-08-16 03:42:18.000000 tair-1.3.5/tair/tairbloom.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)    11976 2022-09-01 08:46:46.000000 tair-1.3.5/tair/taircpc.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     3156 2022-08-25 09:35:31.000000 tair-1.3.5/tair/tairdoc.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     5190 2022-08-25 09:35:31.000000 tair-1.3.5/tair/tairgis.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)    14354 2022-08-25 09:35:31.000000 tair-1.3.5/tair/tairhash.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     4944 2022-08-16 03:42:18.000000 tair-1.3.5/tair/tairroaring.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     6759 2023-04-10 02:26:45.000000 tair-1.3.5/tair/tairsearch.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     9196 2023-01-05 06:47:04.000000 tair-1.3.5/tair/tairstring.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)    13708 2022-09-01 08:46:46.000000 tair-1.3.5/tair/tairts.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)    18561 2023-07-19 08:58:48.000000 tair-1.3.5/tair/tairvector.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     7377 2022-08-16 03:42:18.000000 tair-1.3.5/tair/tairzset.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)      259 2022-08-16 03:42:18.000000 tair-1.3.5/tair/typing.py
+drwxr-xr-x   0 yangbodong   (502) staff       (20)        0 2023-07-19 09:27:01.595496 tair-1.3.5/tair.egg-info/
+-rw-r--r--   0 yangbodong   (502) staff       (20)     4569 2023-07-19 09:27:01.000000 tair-1.3.5/tair.egg-info/PKG-INFO
+-rw-r--r--   0 yangbodong   (502) staff       (20)      874 2023-07-19 09:27:01.000000 tair-1.3.5/tair.egg-info/SOURCES.txt
+-rw-r--r--   0 yangbodong   (502) staff       (20)        1 2023-07-19 09:27:01.000000 tair-1.3.5/tair.egg-info/dependency_links.txt
+-rw-r--r--   0 yangbodong   (502) staff       (20)       13 2023-07-19 09:27:01.000000 tair-1.3.5/tair.egg-info/requires.txt
+-rw-r--r--   0 yangbodong   (502) staff       (20)        5 2023-07-19 09:27:01.000000 tair-1.3.5/tair.egg-info/top_level.txt
+drwxr-xr-x   0 yangbodong   (502) staff       (20)        0 2023-07-19 09:27:01.605825 tair-1.3.5/tests/
+-rw-r--r--   0 yangbodong   (502) staff       (20)     2256 2023-01-05 07:58:42.000000 tair-1.3.5/tests/test_from_url.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     2223 2023-01-05 06:47:04.000000 tair-1.3.5/tests/test_pipeline.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     2484 2022-08-16 03:42:18.000000 tair-1.3.5/tests/test_tairbloom.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)    24057 2022-09-01 08:46:46.000000 tair-1.3.5/tests/test_taircpc.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     4708 2022-08-25 09:35:31.000000 tair-1.3.5/tests/test_tairdoc.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     8533 2022-08-25 09:35:31.000000 tair-1.3.5/tests/test_tairgis.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)    41035 2022-08-16 03:42:18.000000 tair-1.3.5/tests/test_tairhash.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)     9432 2022-08-16 03:42:18.000000 tair-1.3.5/tests/test_tairroaring.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)    18793 2023-04-10 02:26:45.000000 tair-1.3.5/tests/test_tairsearch.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)    19152 2022-08-16 03:42:18.000000 tair-1.3.5/tests/test_tairstring.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)    13908 2022-09-01 08:46:46.000000 tair-1.3.5/tests/test_tairts.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)    24876 2023-07-19 08:58:48.000000 tair-1.3.5/tests/test_tairvector.py
+-rw-r--r--   0 yangbodong   (502) staff       (20)    23955 2022-08-16 03:42:18.000000 tair-1.3.5/tests/test_tairzset.py
```

### Comparing `tair-1.3.4/LICENSE` & `tair-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tair-1.3.4/PKG-INFO` & `tair-1.3.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tair
-Version: 1.3.4
+Version: 1.3.5
 Summary: Python client for Tair
 Home-page: https://github.com/alibaba/tair-py
 Author: Vincil Lau
 Author-email: vincillau@outlook.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -21,22 +21,22 @@
 English | [简体中文](https://github.com/alibaba/tair-py/blob/main/README.zh_CN.md)
 
 tair-py is a Python client of [Tair](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/apsaradb-for-redis-enhanced-edition-overview) based on [redis-py](https://github.com/redis/redis-py). The following modules of Tair are supported.
 
 - [TairString](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairstring-commands), is a string that contains a version number. ([Open sourced](https://github.com/alibaba/TairString))
 - [TairHash](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairhash-commands), is a hash that allows you to specify the expiration time and version number of a field. ([Open sourced](https://github.com/alibaba/TairHash))
 - [TairZset](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairzset-commands), allows you to sort data of the double type based on multiple dimensions. ([Open sourced](https://github.com/alibaba/TairZset))
-- [TairBloom](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairbloom-commands), is a Bloom filter that supports dynamic scaling. (Coming soon)
-- [TairRoaring](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairroaring-commands), is a more efficient and balanced type of compressed bitmaps recognized by the industry. (Coming soon)
-- [TairSearch](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairsearch-command), is a full-text search module developed in-house based on Redis modules. (Coming soon)
-- [TairDoc](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairdoc-commands), to perform create, read, update, and delete (CRUD) operations on JSON data. (Coming soon)
+- [TairBloom](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairbloom-commands), is a Bloom filter that supports dynamic scaling. 
+- [TairRoaring](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairroaring-commands), is a more efficient and balanced type of compressed bitmaps recognized by the industry. 
+- [TairSearch](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairsearch-command), is a full-text search module developed in-house based on Redis modules. 
+- [TairDoc](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairdoc-commands), to perform create, read, update, and delete (CRUD) operations on JSON data. 
 - [TairGis](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairgis-commands), allowing you to query points, linestrings, and polygons. ([Open Sourced](https://github.com/tair-opensource/TairGis))
-- [TairTs](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairts-commands), is a time series data structure that is developed on top of Redis modules.  (Coming soon)
-- [TairCpc](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/taircpc-commands), is a data structure developed based on the compressed probability counting (CPC) sketch. (Coming soon)
-- [TairVector](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairvector),  is a self-developed data structure that provides high-performance real-time storage and retrieval of vectors. (Coming soon)
+- [TairTs](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairts-commands), is a time series data structure that is developed on top of Redis modules.
+- [TairCpc](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/taircpc-commands), is a data structure developed based on the compressed probability counting (CPC) sketch. 
+- [TairVector](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairvector), is a vector search data structure, offering simplicity, flexibility, real-time performance, and high efficiency.  
 
 ## Install
 
 Install from pip:
 
 ```shell
 pip install tair
```

### Comparing `tair-1.3.4/README.md` & `tair-1.3.5/tair.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: tair
+Version: 1.3.5
+Summary: Python client for Tair
+Home-page: https://github.com/alibaba/tair-py
+Author: Vincil Lau
+Author-email: vincillau@outlook.com
+License: MIT
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # tair-py
 
 [![Test](https://github.com/alibaba/tair-py/actions/workflows/test.yml/badge.svg)](https://github.com/alibaba/tair-py/actions/workflows/test.yml)
 [![Format](https://github.com/alibaba/tair-py/actions/workflows/format.yml/badge.svg)](https://github.com/alibaba/tair-py/actions/workflows/format.yml)
 [![Coverage](https://github.com/alibaba/tair-py/actions/workflows/coverage.yml/badge.svg)](https://github.com/alibaba/tair-py/actions/workflows/coverage.yml)
 [![MIT licensed](https://img.shields.io/badge/license-MIT-blue.svg)](./LICENSE)
 [![pypi](https://badge.fury.io/py/tair.svg)](https://pypi.org/project/tair/)
@@ -9,22 +21,22 @@
 English | [简体中文](https://github.com/alibaba/tair-py/blob/main/README.zh_CN.md)
 
 tair-py is a Python client of [Tair](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/apsaradb-for-redis-enhanced-edition-overview) based on [redis-py](https://github.com/redis/redis-py). The following modules of Tair are supported.
 
 - [TairString](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairstring-commands), is a string that contains a version number. ([Open sourced](https://github.com/alibaba/TairString))
 - [TairHash](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairhash-commands), is a hash that allows you to specify the expiration time and version number of a field. ([Open sourced](https://github.com/alibaba/TairHash))
 - [TairZset](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairzset-commands), allows you to sort data of the double type based on multiple dimensions. ([Open sourced](https://github.com/alibaba/TairZset))
-- [TairBloom](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairbloom-commands), is a Bloom filter that supports dynamic scaling. (Coming soon)
-- [TairRoaring](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairroaring-commands), is a more efficient and balanced type of compressed bitmaps recognized by the industry. (Coming soon)
-- [TairSearch](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairsearch-command), is a full-text search module developed in-house based on Redis modules. (Coming soon)
-- [TairDoc](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairdoc-commands), to perform create, read, update, and delete (CRUD) operations on JSON data. (Coming soon)
+- [TairBloom](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairbloom-commands), is a Bloom filter that supports dynamic scaling. 
+- [TairRoaring](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairroaring-commands), is a more efficient and balanced type of compressed bitmaps recognized by the industry. 
+- [TairSearch](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairsearch-command), is a full-text search module developed in-house based on Redis modules. 
+- [TairDoc](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairdoc-commands), to perform create, read, update, and delete (CRUD) operations on JSON data. 
 - [TairGis](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairgis-commands), allowing you to query points, linestrings, and polygons. ([Open Sourced](https://github.com/tair-opensource/TairGis))
-- [TairTs](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairts-commands), is a time series data structure that is developed on top of Redis modules.  (Coming soon)
-- [TairCpc](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/taircpc-commands), is a data structure developed based on the compressed probability counting (CPC) sketch. (Coming soon)
-- [TairVector](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairvector),  is a self-developed data structure that provides high-performance real-time storage and retrieval of vectors. (Coming soon)
+- [TairTs](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairts-commands), is a time series data structure that is developed on top of Redis modules.
+- [TairCpc](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/taircpc-commands), is a data structure developed based on the compressed probability counting (CPC) sketch. 
+- [TairVector](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairvector), is a vector search data structure, offering simplicity, flexibility, real-time performance, and high efficiency.  
 
 ## Install
 
 Install from pip:
 
 ```shell
 pip install tair
@@ -77,8 +89,8 @@
 ## Tair All SDK
 
 | language | GitHub |
 |----------|---|
 | Java     |https://github.com/alibaba/alibabacloud-tairjedis-sdk|
 | Python   |https://github.com/alibaba/tair-py|
 | Go       |https://github.com/alibaba/tair-go|
-| .Net     |https://github.com/alibaba/AlibabaCloud.TairSDK|
+| .Net     |https://github.com/alibaba/AlibabaCloud.TairSDK|
```

### Comparing `tair-1.3.4/tair/__init__.py` & `tair-1.3.5/tair/__init__.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.4/tair/asyncio/__init__.py` & `tair-1.3.5/tair/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.4/tair/asyncio/client.py` & `tair-1.3.5/tair/asyncio/client.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.4/tair/asyncio/cluster.py` & `tair-1.3.5/tair/asyncio/cluster.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.4/tair/asyncio/pipeline.py` & `tair-1.3.5/tair/asyncio/pipeline.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.4/tair/client.py` & `tair-1.3.5/tair/client.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.4/tair/cluster.py` & `tair-1.3.5/tair/cluster.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.4/tair/commands.py` & `tair-1.3.5/tair/commands.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.4/tair/pipeline.py` & `tair-1.3.5/tair/pipeline.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.4/tair/tairbloom.py` & `tair-1.3.5/tair/tairbloom.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.4/tair/taircpc.py` & `tair-1.3.5/tair/taircpc.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.4/tair/tairdoc.py` & `tair-1.3.5/tair/tairdoc.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.4/tair/tairgis.py` & `tair-1.3.5/tair/tairgis.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.4/tair/tairhash.py` & `tair-1.3.5/tair/tairhash.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.4/tair/tairroaring.py` & `tair-1.3.5/tair/tairroaring.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.4/tair/tairsearch.py` & `tair-1.3.5/tair/tairsearch.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.4/tair/tairstring.py` & `tair-1.3.5/tair/tairstring.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.4/tair/tairts.py` & `tair-1.3.5/tair/tairts.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.4/tair/tairvector.py` & `tair-1.3.5/tair/tairvector.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+from concurrent.futures import ThreadPoolExecutor
 from functools import partial, reduce
-from typing import Dict, List, Sequence, Tuple, Union, Optional
+from typing import Dict, List, Sequence, Tuple, Union, Optional, Iterable
 
 from redis.client import pairs_to_dict
 from redis.utils import str_if_bytes
 
 
 VectorType = Sequence[Union[int, float]]
 
 
 class DistanceMetric:
     Euclidean = "L2"  # an alias to L2
     L2 = "L2"
     InnerProduct = "IP"
     Jaccard = "JACCARD"
+    Cosine = "COSINE"
 
 
 class IndexType:
     HNSW = "HNSW"
     FLAT = "FLAT"
 
 
@@ -302,47 +304,93 @@
 
     def tvs_hmget(self, index: str, key: str, *args):
         """
         get specified attributes of a data entry, use attribute key "VECTOR" to get vector value
         """
         return self.execute_command(self.HMGET_CMD, index, key, *args)
 
-    # def tvs_hmget(self, index: str, key: str,fields: Iterable[str]):
-    #     return self.execute_command(self.HMGET_CMD, index,key, *fields)
-
-    def tvs_scan(self, index: str, pattern: Optional[str] = None, batch: int = 10):
+    def tvs_scan(
+        self,
+        index: str,
+        pattern: Optional[str] = None,
+        batch: int = 10,
+        filter_str: Optional[str] = None,
+        vector: Optional[VectorType] = None,
+        max_dist: Optional[float] = None,
+    ):
         """
         scan all data entries in an index
         """
         args = ([] if pattern is None else ["MATCH", pattern]) + ["COUNT", batch]
+        if filter_str is not None:
+            args.append("FILTER")
+            args.append(filter_str)
+        if vector is not None and max_dist is not None:
+            args.append("VECTOR")
+            args.append(self.encode_vector(vector))
+            args.append("MAX_DIST")
+            args.append(max_dist)
+        elif vector is None and max_dist is None:
+            pass
+        else:
+            raise ValueError("missing vector or max_dist")
 
         def get_batch(c):
             return self.execute_command(self.SCAN_CMD, index, c, *args)
 
         return TairVectorScanResult(self, get_batch)
 
+    def _tvs_scan(
+        self,
+        index: str,
+        cursor: int = 0,
+        count: Optional[int] = None,
+        pattern: Optional[str] = None,
+        filter_str: Optional[str] = None,
+        vector: Union[VectorType, bytes, None] = None,
+        max_dist: Optional[float] = None,
+    ):
+        args = [] if pattern is None else ["MATCH", pattern]
+        if count is not None:
+            args += ("COUNT", count)
+        if filter_str is not None:
+            args.append("FILTER")
+            args.append(filter_str)
+        if vector is not None and max_dist is not None:
+            args.append("VECTOR")
+            args.append(
+                vector if isinstance(vector, bytes) else self.encode_vector(vector)
+            )
+            args.append("MAX_DIST")
+            args.append(max_dist)
+        elif vector is None and max_dist is None:
+            pass
+        else:
+            raise ValueError("missing vector or max_dist")
+        return self.execute_command(self.SCAN_CMD, index, cursor, *args)
+
     SEARCH_CMD = "TVS.KNNSEARCH"
     MSEARCH_CMD = "TVS.MKNNSEARCH"
     MINDEXKNNSEARCH_CMD = "TVS.MINDEXKNNSEARCH"
     MINDEXMKNNSEARCH_CMD = "TVS.MINDEXMKNNSEARCH"
 
     def tvs_knnsearch(
         self,
         index: str,
         k: int,
-        vector: Union[VectorType, str],
+        vector: Union[VectorType, str, bytes],
         is_binary: bool = False,
         filter_str: Optional[str] = None,
         **kwargs
     ):
         """
         search for the top @k approximate nearest neighbors of @vector in an index
         """
         params = reduce(lambda x, y: x + y, kwargs.items(), ())
-        if not isinstance(vector, str):
+        if (not isinstance(vector, str)) and (not isinstance(vector, bytes)):
             vector = TairVectorCommands.encode_vector(vector, is_binary)
         if filter_str is None:
             return self.execute_command(self.SEARCH_CMD, index, k, vector, *params)
         return self.execute_command(
             self.SEARCH_CMD, index, k, vector, filter_str, *params
         )
 
@@ -381,24 +429,24 @@
             *params
         )
 
     def tvs_mindexknnsearch(
         self,
         index: Sequence[str],
         k: int,
-        vector: Union[VectorType, str],
+        vector: Union[VectorType, str, bytes],
         is_binary: bool = False,
         filter_str: Optional[str] = None,
         **kwargs
     ):
         """
         search for the top @k approximate nearest neighbors of @vector in indexs
         """
         params = reduce(lambda x, y: x + y, kwargs.items(), ())
-        if not isinstance(vector, str):
+        if (not isinstance(vector, str)) and (not isinstance(vector, bytes)):
             vector = TairVectorCommands.encode_vector(vector, is_binary)
         if filter_str is None:
             return self.execute_command(
                 self.MINDEXKNNSEARCH_CMD, len(index), *index, k, vector, *params
             )
         return self.execute_command(
             self.MINDEXKNNSEARCH_CMD, len(index), *index, k, vector, filter_str, *params
@@ -437,14 +485,105 @@
             k,
             len(encoded_vectors),
             *encoded_vectors,
             filter_str,
             *params
         )
 
+    GETDISTANCE_CMD = "TVS.GETDISTANCE"
+
+    def _tvs_getdistance(
+        self,
+        index_name: str,
+        vector: VectorType,
+        keys: Iterable[str],
+        top_n: Optional[int] = None,
+        max_dist: Optional[float] = None,
+        filter_str: Optional[str] = None,
+    ):
+        """
+        low level interface for TVS.GETDISTANCE
+        """
+        args = list(keys)
+        if top_n is not None:
+            args += ("TOPN", top_n)
+        if max_dist is not None:
+            args += ("MAX_DIST", max_dist)
+        if filter_str is not None:
+            args += ("FILTER", filter_str)
+
+        if (not isinstance(vector, str)) and (not isinstance(vector, bytes)):
+            vector_str = self.encode_vector(vector)
+        else:
+            vector_str = vector
+        return self.execute_command(
+            self.GETDISTANCE_CMD, index_name, vector_str, len(keys), *args
+        )
+
+    def tvs_getdistance(
+        self,
+        index_name: str,
+        vector: Union[VectorType, str, bytes],
+        keys: Iterable[str],
+        batch_size: int = 100000,
+        parallelism: int = 1,
+        top_n: Optional[int] = None,
+        max_dist: Optional[float] = None,
+        filter_str: Optional[str] = None,
+    ):
+        """
+        wrapped interface for TVS.GETDISTANCE
+        """
+        import heapq
+        import itertools
+
+        if (not isinstance(vector, str)) and (not isinstance(vector, bytes)):
+            vector_str = self.encode_vector(vector)
+        else:
+            vector_str = vector
+
+        k = len(keys)
+        if top_n is not None:
+            k = min(k, top_n)
+
+        args = ["TOPN", k]
+        if max_dist is not None:
+            args += ("MAX_DIST", max_dist)
+        if filter_str is not None:
+            args += ("FILTER", filter_str)
+
+        def process_batch(batch):
+            return self.execute_command(
+                self.GETDISTANCE_CMD,
+                index_name,
+                vector_str,
+                len(batch),
+                *(batch + args)
+            )
+
+        with ThreadPoolExecutor(max_workers=parallelism) as executor:
+            batches = [
+                keys[i : i + batch_size] for i in range(0, len(keys), batch_size)
+            ]
+
+            futures = [executor.submit(process_batch, batch) for batch in batches]
+
+            queue = []
+            for f in futures:
+                result = f.result()
+                queue = heapq.merge(
+                    queue,
+                    [
+                        (float(result[i + 1]), result[i])
+                        for i in range(0, len(result), 2)
+                    ],
+                )
+            queue = itertools.islice(queue, k)
+            return [(key, score) for score, key in queue]
+
 
 def parse_tvs_get_index_result(resp) -> Union[Dict, None]:
     if len(resp) == 0:
         return None
     return pairs_to_dict(resp, decode_keys=True, decode_string_values=True)
```

### Comparing `tair-1.3.4/tair/tairzset.py` & `tair-1.3.5/tair/tairzset.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.4/tair.egg-info/PKG-INFO` & `tair-1.3.5/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: tair
-Version: 1.3.4
-Summary: Python client for Tair
-Home-page: https://github.com/alibaba/tair-py
-Author: Vincil Lau
-Author-email: vincillau@outlook.com
-License: MIT
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # tair-py
 
 [![Test](https://github.com/alibaba/tair-py/actions/workflows/test.yml/badge.svg)](https://github.com/alibaba/tair-py/actions/workflows/test.yml)
 [![Format](https://github.com/alibaba/tair-py/actions/workflows/format.yml/badge.svg)](https://github.com/alibaba/tair-py/actions/workflows/format.yml)
 [![Coverage](https://github.com/alibaba/tair-py/actions/workflows/coverage.yml/badge.svg)](https://github.com/alibaba/tair-py/actions/workflows/coverage.yml)
 [![MIT licensed](https://img.shields.io/badge/license-MIT-blue.svg)](./LICENSE)
 [![pypi](https://badge.fury.io/py/tair.svg)](https://pypi.org/project/tair/)
@@ -21,22 +9,22 @@
 English | [简体中文](https://github.com/alibaba/tair-py/blob/main/README.zh_CN.md)
 
 tair-py is a Python client of [Tair](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/apsaradb-for-redis-enhanced-edition-overview) based on [redis-py](https://github.com/redis/redis-py). The following modules of Tair are supported.
 
 - [TairString](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairstring-commands), is a string that contains a version number. ([Open sourced](https://github.com/alibaba/TairString))
 - [TairHash](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairhash-commands), is a hash that allows you to specify the expiration time and version number of a field. ([Open sourced](https://github.com/alibaba/TairHash))
 - [TairZset](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairzset-commands), allows you to sort data of the double type based on multiple dimensions. ([Open sourced](https://github.com/alibaba/TairZset))
-- [TairBloom](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairbloom-commands), is a Bloom filter that supports dynamic scaling. (Coming soon)
-- [TairRoaring](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairroaring-commands), is a more efficient and balanced type of compressed bitmaps recognized by the industry. (Coming soon)
-- [TairSearch](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairsearch-command), is a full-text search module developed in-house based on Redis modules. (Coming soon)
-- [TairDoc](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairdoc-commands), to perform create, read, update, and delete (CRUD) operations on JSON data. (Coming soon)
+- [TairBloom](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairbloom-commands), is a Bloom filter that supports dynamic scaling. 
+- [TairRoaring](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairroaring-commands), is a more efficient and balanced type of compressed bitmaps recognized by the industry. 
+- [TairSearch](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairsearch-command), is a full-text search module developed in-house based on Redis modules. 
+- [TairDoc](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairdoc-commands), to perform create, read, update, and delete (CRUD) operations on JSON data. 
 - [TairGis](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairgis-commands), allowing you to query points, linestrings, and polygons. ([Open Sourced](https://github.com/tair-opensource/TairGis))
-- [TairTs](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairts-commands), is a time series data structure that is developed on top of Redis modules.  (Coming soon)
-- [TairCpc](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/taircpc-commands), is a data structure developed based on the compressed probability counting (CPC) sketch. (Coming soon)
-- [TairVector](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairvector),  is a self-developed data structure that provides high-performance real-time storage and retrieval of vectors. (Coming soon)
+- [TairTs](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairts-commands), is a time series data structure that is developed on top of Redis modules.
+- [TairCpc](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/taircpc-commands), is a data structure developed based on the compressed probability counting (CPC) sketch. 
+- [TairVector](https://www.alibabacloud.com/help/en/apsaradb-for-redis/latest/tairvector), is a vector search data structure, offering simplicity, flexibility, real-time performance, and high efficiency.  
 
 ## Install
 
 Install from pip:
 
 ```shell
 pip install tair
@@ -89,8 +77,8 @@
 ## Tair All SDK
 
 | language | GitHub |
 |----------|---|
 | Java     |https://github.com/alibaba/alibabacloud-tairjedis-sdk|
 | Python   |https://github.com/alibaba/tair-py|
 | Go       |https://github.com/alibaba/tair-go|
-| .Net     |https://github.com/alibaba/AlibabaCloud.TairSDK|
+| .Net     |https://github.com/alibaba/AlibabaCloud.TairSDK|
```

### Comparing `tair-1.3.4/tair.egg-info/SOURCES.txt` & `tair-1.3.5/tair.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tair-1.3.4/tests/test_from_url.py` & `tair-1.3.5/tests/test_from_url.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.4/tests/test_pipeline.py` & `tair-1.3.5/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.4/tests/test_tairbloom.py` & `tair-1.3.5/tests/test_tairbloom.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.4/tests/test_taircpc.py` & `tair-1.3.5/tests/test_taircpc.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.4/tests/test_tairdoc.py` & `tair-1.3.5/tests/test_tairdoc.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.4/tests/test_tairgis.py` & `tair-1.3.5/tests/test_tairgis.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.4/tests/test_tairhash.py` & `tair-1.3.5/tests/test_tairhash.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.4/tests/test_tairroaring.py` & `tair-1.3.5/tests/test_tairroaring.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.4/tests/test_tairsearch.py` & `tair-1.3.5/tests/test_tairsearch.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.4/tests/test_tairstring.py` & `tair-1.3.5/tests/test_tairstring.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.4/tests/test_tairts.py` & `tair-1.3.5/tests/test_tairts.py`

 * *Files identical despite different names*

### Comparing `tair-1.3.4/tests/test_tairvector.py` & `tair-1.3.5/tests/test_tairvector.py`

 * *Files 23% similar despite different names*

```diff
@@ -50,15 +50,14 @@
     def test_0_delete_all_indices(self):
         # get all indices
         indices = []
         result = client.tvs_scan_index()
         for index in result.iter():
             indices.append(index)
 
-        print("deleting indices:", indices)
         # deleting all indices
         for index in indices:
             try:
                 ret = client.tvs_del_index(index)
                 self.assertEqual(ret, 1)
             except:
                 self.logger.error("delete index [%s] failed" % index)
@@ -67,17 +66,14 @@
         indices = []
         result = client.tvs_scan_index()
         for index in result.iter():
             indices.append(index)
         self.assertEqual(indices, [])
 
     def test_1_delete_noexist_index(self):
-        print(
-            "deleting no-exist index",
-        )
         ret = client.tvs_del_index("test")
         self.assertFalse(ret, 0)
 
     def test_2_get_nonexist_index(self):
         self.assertIsNone(client.tvs_get_index("test"))
 
     def test_3_create_index(self):
@@ -285,21 +281,14 @@
         self.assertEqual(len(result), len(batch))
         for r in result:
             d = 0.0
             for _, v in r:
                 self.assertGreaterEqual(v, d)
                 d = v
 
-    # todo
-    def test_5_search_with_filters(self):
-        pass
-
-    def test_6_msearch_with_filters(self):
-        pass
-
     def test_7_mindexknnsearch(self):
         indexs = ["test", "test2"]
         for q in queries:
             result = client.tvs_mindexknnsearch(indexs, self.top_k, vector=q)
             self.assertEqual(self.top_k, len(result))
             d = 0.0
             for k, v in result:
@@ -336,15 +325,14 @@
         with self.assertRaises(ValueError):
             index = TairVectorIndex(client, "test")
 
     def test_1_create_index(self):
         # create a new index
         index = TairVectorIndex(client, "test", dim=dim, **self.index_params)
         self.assertIsNotNone(index)
-        print(index)
 
         # get an existing index
         index2 = TairVectorIndex(client, "test")
         self.assertEqual(str(index), str(index2))
 
     def test_2_create_duplicate_index(self):
         with self.assertRaises(redis.exceptions.ResponseError):
@@ -481,10 +469,236 @@
             self.assertAlmostEqual(s, jaccard(q, test_bin_vectors[int(k)]))
 
     def test_9_cleanup(self):
         ret = client.tvs_del_index("test_bin")
         self.assertEqual(ret, 1)
 
 
+filter_test_data = [
+    {"vector": "[7,3]", "name": "Aaron", "age": "12"},  # dist 58
+    {"vector": "[9,2]", "name": "Bob", "age": "33"},  # dist 85
+    {"vector": "[6,6]", "name": "Charlie", "age": "29"},  # dist 72
+    {"vector": "[3,5]", "name": "Daniel", "age": "23"},  # dist 34
+    {"vector": "[3,7]", "name": "Eason", "age": "22"},  # dist 58
+    {"vector": "[3,6]", "name": "Fabian", "age": "35"},  # dist 45
+    {"vector": "[5,2]", "name": "George", "age": "12"},  # dist 29
+    {"vector": "[8,9]", "name": "Henry", "age": "30"},  # dist 145
+    {"vector": "[5,5]", "name": "Ivan", "age": "16"},  # dist 50
+    {"vector": "[2,7]", "name": "James", "age": "12"},  # dist 53
+]
+
+
+class ScanTest(unittest.TestCase):
+    index_name = "scan_test"
+
+    def test_0_create(self):
+        ret = client.tvs_create_index(
+            self.index_name,
+            2,
+            distance_type=DistanceMetric.L2,
+        )
+        self.assertTrue(ret)
+        for i, d in enumerate(filter_test_data):
+            ret = client.tvs_hset(self.index_name, str(i), **d)
+            self.assertEqual(ret, 3)
+
+    def test_1_basic_scan(self):
+        result = [r for r in client.tvs_scan(self.index_name, "*")]
+        result = sorted(result)
+        self.assertListEqual(result, [str(i).encode() for i in range(0, 10)])
+
+        result = [r for r in client.tvs_scan(self.index_name, "a*")]
+        self.assertEqual(len(result), 0)
+
+    def test_2_scan_with_filter(self):
+        result = [r for r in client.tvs_scan(self.index_name, filter_str="age>30")]
+        result = sorted(result)
+        self.assertListEqual(result, [b"1", b"5"])
+
+        result = [r for r in client.tvs_scan(self.index_name, filter_str='name>"H"')]
+        result = sorted(result)
+        self.assertListEqual(result, [b"7", b"8", b"9"])
+
+        result = [
+            r for r in client.tvs_scan(self.index_name, filter_str='name=="Henry"')
+        ]
+        self.assertListEqual(result, [b"7"])
+
+    def test_3_scan_with_max_distance(self):
+        with self.assertRaises(ValueError):
+            client.tvs_scan(self.index_name, max_dist=50)
+        with self.assertRaises(ValueError):
+            client.tvs_scan(self.index_name, vector=[0, 0])
+        result = [
+            r for r in client.tvs_scan(self.index_name, vector=[0, 0], max_dist=50)
+        ]
+        result = sorted(result)
+        self.assertListEqual(result, [b"3", b"5", b"6"])
+
+    def test_4_scan_with_both(self):
+        result = [
+            r
+            for r in client.tvs_scan(
+                self.index_name, vector=[0, 0], max_dist=50, filter_str="age<30"
+            )
+        ]
+        result = sorted(result)
+        self.assertListEqual(result, [b"3", b"6"])
+
+    def test_9_cleanup(self):
+        ret = client.tvs_del_index(self.index_name)
+        self.assertEqual(ret, 1)
+
+
+class SearchWithFilterTest(unittest.TestCase):
+    index_name = "filter_test"
+
+    def test_0_create(self):
+        ret = client.tvs_create_index(
+            self.index_name,
+            2,
+            distance_type=DistanceMetric.L2,
+        )
+        self.assertTrue(ret)
+        for i, d in enumerate(filter_test_data):
+            ret = client.tvs_hset(self.index_name, str(i), **d)
+            self.assertEqual(ret, 3)
+
+    def test_1_knnsearch(self):
+        result = client.tvs_knnsearch(self.index_name, 5, vector=[0, 0])
+        self.assertListEqual([t[0] for t in result], [b"6", b"3", b"5", b"8", b"9"])
+        result = client.tvs_knnsearch(self.index_name, 5, vector=[0, 0], MAX_DIST=50)
+        self.assertListEqual([t[0] for t in result], [b"6", b"3", b"5", b"8"])
+        result = client.tvs_knnsearch(
+            self.index_name, 5, vector=[0, 0], filter_str="age<20"
+        )
+        self.assertListEqual([t[0] for t in result], [b"6", b"8", b"9", b"0"])
+        result = client.tvs_knnsearch(
+            self.index_name, 5, vector=[0, 0], MAX_DIST=50, filter_str="age<20"
+        )
+        self.assertListEqual([t[0] for t in result], [b"6", b"8"])
+
+    def test_2_mknnsearch(self):
+        result = client.tvs_mknnsearch(self.index_name, 5, [[0, 0]])
+        self.assertListEqual([t[0] for t in result[0]], [b"6", b"3", b"5", b"8", b"9"])
+        result = client.tvs_mknnsearch(self.index_name, 5, [[0, 0]], MAX_DIST=50)
+        self.assertListEqual([t[0] for t in result[0]], [b"6", b"3", b"5", b"8"])
+        result = client.tvs_mknnsearch(
+            self.index_name, 5, [[0, 0]], filter_str="age<20"
+        )
+        self.assertListEqual([t[0] for t in result[0]], [b"6", b"8", b"9", b"0"])
+        result = client.tvs_mknnsearch(
+            self.index_name, 5, [[0, 0]], MAX_DIST=50, filter_str="age<20"
+        )
+        self.assertListEqual([t[0] for t in result[0]], [b"6", b"8"])
+
+    def test_3_mindexknnsearch(self):
+        result = client.tvs_mindexknnsearch([self.index_name], 5, vector=[0, 0])
+        self.assertListEqual([t[0] for t in result], [b"6", b"3", b"5", b"8", b"9"])
+        result = client.tvs_mindexknnsearch(
+            [self.index_name], 5, vector=[0, 0], MAX_DIST=50
+        )
+        self.assertListEqual([t[0] for t in result], [b"6", b"3", b"5", b"8"])
+        result = client.tvs_mindexknnsearch(
+            [self.index_name], 5, vector=[0, 0], filter_str="age<20"
+        )
+        self.assertListEqual([t[0] for t in result], [b"6", b"8", b"9", b"0"])
+        result = client.tvs_mindexknnsearch(
+            [self.index_name], 5, vector=[0, 0], MAX_DIST=50, filter_str="age<20"
+        )
+        self.assertListEqual([t[0] for t in result], [b"6", b"8"])
+
+    def test_4_mindexmknnsearch(self):
+        result = client.tvs_mindexmknnsearch([self.index_name], 5, [[0, 0]])
+        self.assertListEqual([t[0] for t in result[0]], [b"6", b"3", b"5", b"8", b"9"])
+        result = client.tvs_mindexmknnsearch(
+            [self.index_name], 5, [[0, 0]], MAX_DIST=50
+        )
+        self.assertListEqual([t[0] for t in result[0]], [b"6", b"3", b"5", b"8"])
+        result = client.tvs_mindexmknnsearch(
+            [self.index_name], 5, [[0, 0]], filter_str="age<20"
+        )
+        self.assertListEqual([t[0] for t in result[0]], [b"6", b"8", b"9", b"0"])
+        result = client.tvs_mindexmknnsearch(
+            [self.index_name], 5, [[0, 0]], MAX_DIST=50, filter_str="age<20"
+        )
+        self.assertListEqual([t[0] for t in result[0]], [b"6", b"8"])
+
+    def test_9_cleanup(self):
+        ret = client.tvs_del_index(self.index_name)
+        self.assertEqual(ret, 1)
+
+
+class GetDistanceTest(unittest.TestCase):
+    index_name = "getdistance_test"
+
+    def test_0_create(self):
+        vectors = [[random() for _ in range(dim)] for _ in range(1000)]
+        ret = client.tvs_create_index(
+            self.index_name,
+            dim,
+            distance_type=DistanceMetric.L2,
+        )
+        self.assertTrue(ret)
+        for i, v in enumerate(vectors):
+            ret = client.tvs_hset(self.index_name, str(i), v, attr=i)
+            self.assertEqual(ret, 2)
+
+    def test_1_getdistance(self):
+        query = [random() for _ in range(dim)]
+        keys = [str(i) for i in range(1000)]
+
+        # test low level interface
+        results = client._tvs_getdistance(self.index_name, query, keys, top_n=10)
+        self.assertEqual(20, len(results))
+        for i in range(0, len(results) - 2, 2):
+            self.assertTrue(float(results[i + 1]) <= float(results[i + 3]))
+
+        # test wrapped interface
+        results = client.tvs_getdistance(
+            self.index_name, query, keys, batch_size=100, top_n=10
+        )
+        self.assertEqual(10, len(results))
+        for i in range(len(results) - 1):
+            self.assertTrue(results[i][1] <= results[i + 1][1])
+
+    def test_2_getdistance_with_max_dist(self):
+        query = [random() for _ in range(dim)]
+        keys = [str(i) for i in range(1000)]
+
+        results = client.tvs_getdistance(
+            self.index_name, query, keys, batch_size=100, top_n=10, max_dist=3.0
+        )
+        self.assertGreater(len(results), 0)
+        self.assertGreaterEqual(10, len(results))
+        for i in range(len(results) - 1):
+            self.assertTrue(results[i][1] <= results[i + 1][1])
+        for _, score in results:
+            self.assertGreater(3.0, score)
+
+    def test_3_getdistance_with_filter(self):
+        query = [random() for _ in range(dim)]
+        keys = [str(i) for i in range(1000)]
+
+        results = client.tvs_getdistance(
+            self.index_name,
+            query,
+            keys,
+            batch_size=100,
+            top_n=10,
+            filter_str="attr<500",
+        )
+        self.assertGreater(len(results), 0)
+        self.assertGreaterEqual(10, len(results))
+        for i in range(len(results) - 1):
+            self.assertTrue(results[i][1] <= results[i + 1][1])
+        for key, _ in results:
+            self.assertLess(int(key), 500)
+
+    def test_9_cleanup(self):
+        ret = client.tvs_del_index(self.index_name)
+        self.assertEqual(ret, 1)
+
+
 if __name__ == "__main__":
     unittest.main()
     client.close()
```

### Comparing `tair-1.3.4/tests/test_tairzset.py` & `tair-1.3.5/tests/test_tairzset.py`

 * *Files identical despite different names*

