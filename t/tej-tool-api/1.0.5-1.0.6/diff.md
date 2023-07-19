# Comparing `tmp/tej-tool-api-1.0.5.tar.gz` & `tmp/tej-tool-api-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tej-tool-api-1.0.5.tar", last modified: Wed Jul 19 01:22:21 2023, max compression
+gzip compressed data, was "tej-tool-api-1.0.6.tar", last modified: Wed Jul 19 01:23:24 2023, max compression
```

## Comparing `tej-tool-api-1.0.5.tar` & `tej-tool-api-1.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 01:22:21.904130 tej-tool-api-1.0.5/
--rw-rw-rw-   0        0        0     5566 2023-07-19 01:22:21.904130 tej-tool-api-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     5156 2023-07-19 01:21:55.000000 tej-tool-api-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-19 01:22:21.888506 tej-tool-api-1.0.5/TejTOolAPI/
--rw-rw-rw-   0        0        0      197 2023-05-19 07:13:38.000000 tej-tool-api-1.0.5/TejTOolAPI/Error.py
--rw-rw-rw-   0        0        0    17814 2023-07-19 01:08:13.000000 tej-tool-api-1.0.5/TejTOolAPI/Map_Dask_API.py
--rw-rw-rw-   0        0        0    11001 2023-07-19 01:08:13.000000 tej-tool-api-1.0.5/TejTOolAPI/TejToolAPI.py
--rw-rw-rw-   0        0        0      582 2023-07-10 09:13:18.000000 tej-tool-api-1.0.5/TejTOolAPI/__init__.py
--rw-rw-rw-   0        0        0     2329 2023-07-10 09:13:18.000000 tej-tool-api-1.0.5/TejTOolAPI/exchange_calendar.py
--rw-rw-rw-   0        0        0     1488 2023-07-12 03:01:58.000000 tej-tool-api-1.0.5/TejTOolAPI/parameters.py
-drwxrwxrwx   0        0        0        0 2023-07-19 01:22:21.872880 tej-tool-api-1.0.5/TejTOolAPI/tables/
--rw-rw-rw-   0        0        0    38860 2023-07-10 09:13:18.000000 tej-tool-api-1.0.5/TejTOolAPI/tables/columns_group.xlsx
--rw-rw-rw-   0        0        0   137941 2023-05-19 07:13:38.000000 tej-tool-api-1.0.5/TejTOolAPI/tables/mktboard.csv
--rw-rw-rw-   0        0        0       42 2023-07-19 01:22:21.904130 tej-tool-api-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1490 2023-07-19 01:22:17.000000 tej-tool-api-1.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-19 01:22:21.888506 tej-tool-api-1.0.5/tej_tool_api.egg-info/
--rw-rw-rw-   0        0        0     5566 2023-07-19 01:22:21.000000 tej-tool-api-1.0.5/tej_tool_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      417 2023-07-19 01:22:21.000000 tej-tool-api-1.0.5/tej_tool_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 01:22:21.000000 tej-tool-api-1.0.5/tej_tool_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-07-19 01:22:21.000000 tej-tool-api-1.0.5/tej_tool_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-07-19 01:22:21.000000 tej-tool-api-1.0.5/tej_tool_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-19 01:23:24.381233 tej-tool-api-1.0.6/
+-rw-rw-rw-   0        0        0     5568 2023-07-19 01:23:24.381233 tej-tool-api-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     5158 2023-07-19 01:23:01.000000 tej-tool-api-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-19 01:23:24.365580 tej-tool-api-1.0.6/TejTOolAPI/
+-rw-rw-rw-   0        0        0      197 2023-05-19 07:13:38.000000 tej-tool-api-1.0.6/TejTOolAPI/Error.py
+-rw-rw-rw-   0        0        0    17814 2023-07-19 01:08:13.000000 tej-tool-api-1.0.6/TejTOolAPI/Map_Dask_API.py
+-rw-rw-rw-   0        0        0    11001 2023-07-19 01:08:13.000000 tej-tool-api-1.0.6/TejTOolAPI/TejToolAPI.py
+-rw-rw-rw-   0        0        0      582 2023-07-10 09:13:18.000000 tej-tool-api-1.0.6/TejTOolAPI/__init__.py
+-rw-rw-rw-   0        0        0     2329 2023-07-10 09:13:18.000000 tej-tool-api-1.0.6/TejTOolAPI/exchange_calendar.py
+-rw-rw-rw-   0        0        0     1488 2023-07-12 03:01:58.000000 tej-tool-api-1.0.6/TejTOolAPI/parameters.py
+drwxrwxrwx   0        0        0        0 2023-07-19 01:23:24.349971 tej-tool-api-1.0.6/TejTOolAPI/tables/
+-rw-rw-rw-   0        0        0    38860 2023-07-10 09:13:18.000000 tej-tool-api-1.0.6/TejTOolAPI/tables/columns_group.xlsx
+-rw-rw-rw-   0        0        0   137941 2023-05-19 07:13:38.000000 tej-tool-api-1.0.6/TejTOolAPI/tables/mktboard.csv
+-rw-rw-rw-   0        0        0       42 2023-07-19 01:23:24.381233 tej-tool-api-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1490 2023-07-19 01:23:21.000000 tej-tool-api-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 01:23:24.365580 tej-tool-api-1.0.6/tej_tool_api.egg-info/
+-rw-rw-rw-   0        0        0     5568 2023-07-19 01:23:24.000000 tej-tool-api-1.0.6/tej_tool_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      417 2023-07-19 01:23:24.000000 tej-tool-api-1.0.6/tej_tool_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 01:23:24.000000 tej-tool-api-1.0.6/tej_tool_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-07-19 01:23:24.000000 tej-tool-api-1.0.6/tej_tool_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-19 01:23:24.000000 tej-tool-api-1.0.6/tej_tool_api.egg-info/top_level.txt
```

### Comparing `tej-tool-api-1.0.5/PKG-INFO` & `tej-tool-api-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tej-tool-api
-Version: 1.0.5
+Version: 1.0.6
 Summary: Package to fetch a large quantity of data from tejapi.
 Home-page: https://api.tej.com.tw
 Author: tej
 Author-email: tej@tej.com.tw
 Maintainer: tej api Development Team
 Maintainer-email: tej@tej.com
 License: MIT
@@ -106,14 +106,15 @@
 
 | COLUMNS | TABLE_NAMES | 
 |---------|-----------------|
 | r404    | fin_self_acc    |
 | r404    | fin_auditor    |
 
 <br>
+
 **參數:**
 
 
 
 | Parameters | Is Required | Data Type | Descriptions |
 |------------|-------------|-----------|--------------|
 | columns    | Required    | list      | 欄位代碼，可參考[TEJAPI_量化投資資料庫](http://10.10.10.66/datatables.html?db=TWN&t=%E5%8F%B0%E7%81%A3%E8%B3%87%E6%96%99%E5%BA%AB#G%E9%87%8F%E5%8C%96%E6%8A%95%E8%B3%87) |
```

### Comparing `tej-tool-api-1.0.5/README.md` & `tej-tool-api-1.0.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -92,14 +92,15 @@
 
 | COLUMNS | TABLE_NAMES | 
 |---------|-----------------|
 | r404    | fin_self_acc    |
 | r404    | fin_auditor    |
 
 <br>
+
 **參數:**
 
 
 
 | Parameters | Is Required | Data Type | Descriptions |
 |------------|-------------|-----------|--------------|
 | columns    | Required    | list      | 欄位代碼，可參考[TEJAPI_量化投資資料庫](http://10.10.10.66/datatables.html?db=TWN&t=%E5%8F%B0%E7%81%A3%E8%B3%87%E6%96%99%E5%BA%AB#G%E9%87%8F%E5%8C%96%E6%8A%95%E8%B3%87) |
```

### Comparing `tej-tool-api-1.0.5/TejTOolAPI/Map_Dask_API.py` & `tej-tool-api-1.0.6/TejTOolAPI/Map_Dask_API.py`

 * *Files identical despite different names*

### Comparing `tej-tool-api-1.0.5/TejTOolAPI/TejToolAPI.py` & `tej-tool-api-1.0.6/TejTOolAPI/TejToolAPI.py`

 * *Files identical despite different names*

### Comparing `tej-tool-api-1.0.5/TejTOolAPI/__init__.py` & `tej-tool-api-1.0.6/TejTOolAPI/__init__.py`

 * *Files identical despite different names*

### Comparing `tej-tool-api-1.0.5/TejTOolAPI/exchange_calendar.py` & `tej-tool-api-1.0.6/TejTOolAPI/exchange_calendar.py`

 * *Files identical despite different names*

### Comparing `tej-tool-api-1.0.5/TejTOolAPI/parameters.py` & `tej-tool-api-1.0.6/TejTOolAPI/parameters.py`

 * *Files identical despite different names*

### Comparing `tej-tool-api-1.0.5/TejTOolAPI/tables/columns_group.xlsx` & `tej-tool-api-1.0.6/TejTOolAPI/tables/columns_group.xlsx`

 * *Files identical despite different names*

### Comparing `tej-tool-api-1.0.5/TejTOolAPI/tables/mktboard.csv` & `tej-tool-api-1.0.6/TejTOolAPI/tables/mktboard.csv`

 * *Files identical despite different names*

### Comparing `tej-tool-api-1.0.5/setup.py` & `tej-tool-api-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 long_description = (this_directionary/"README.md").read_text(encoding='utf-8')
 setup(
     name='tej-tool-api',
     description='Package to fetch a large quantity of data from tejapi.',
     keywords=['tej', 'big data', 'data', 'financial', 'economic','stock','TEJ',],
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.0.5',
+    version='1.0.6',
     author='tej',
     author_email='tej@tej.com.tw',
     maintainer='tej api Development Team',
     maintainer_email='tej@tej.com',
     url='https://api.tej.com.tw',
     license='MIT',
     install_requires=install_requires,
```

### Comparing `tej-tool-api-1.0.5/tej_tool_api.egg-info/PKG-INFO` & `tej-tool-api-1.0.6/tej_tool_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tej-tool-api
-Version: 1.0.5
+Version: 1.0.6
 Summary: Package to fetch a large quantity of data from tejapi.
 Home-page: https://api.tej.com.tw
 Author: tej
 Author-email: tej@tej.com.tw
 Maintainer: tej api Development Team
 Maintainer-email: tej@tej.com
 License: MIT
@@ -106,14 +106,15 @@
 
 | COLUMNS | TABLE_NAMES | 
 |---------|-----------------|
 | r404    | fin_self_acc    |
 | r404    | fin_auditor    |
 
 <br>
+
 **參數:**
 
 
 
 | Parameters | Is Required | Data Type | Descriptions |
 |------------|-------------|-----------|--------------|
 | columns    | Required    | list      | 欄位代碼，可參考[TEJAPI_量化投資資料庫](http://10.10.10.66/datatables.html?db=TWN&t=%E5%8F%B0%E7%81%A3%E8%B3%87%E6%96%99%E5%BA%AB#G%E9%87%8F%E5%8C%96%E6%8A%95%E8%B3%87) |
```

