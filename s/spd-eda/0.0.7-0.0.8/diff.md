# Comparing `tmp/spd_eda-0.0.7.tar.gz` & `tmp/spd_eda-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spd_eda-0.0.7.tar", last modified: Mon Oct 24 19:57:41 2022, max compression
+gzip compressed data, was "spd_eda-0.0.8.tar", last modified: Wed Jul 19 13:47:20 2023, max compression
```

## Comparing `spd_eda-0.0.7.tar` & `spd_eda-0.0.8.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2022-10-24 19:57:41.795756 spd_eda-0.0.7/
--rw-rw-rw-   0        0        0        0 2022-09-08 20:28:11.000000 spd_eda-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     9679 2022-10-24 19:57:41.794757 spd_eda-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     9316 2022-10-20 20:56:07.000000 spd_eda-0.0.7/README.md
--rw-rw-rw-   0        0        0      660 2022-10-24 19:57:23.000000 spd_eda-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-10-24 19:57:41.795756 spd_eda-0.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-10-24 19:57:41.707866 spd_eda-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2022-10-24 19:57:41.718864 spd_eda-0.0.7/src/spd_eda/
--rw-rw-rw-   0        0        0      647 2022-09-14 15:46:48.000000 spd_eda-0.0.7/src/spd_eda/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-24 19:57:41.741871 spd_eda-0.0.7/src/spd_eda/athena_tools/
--rw-rw-rw-   0        0        0        0 2022-09-12 18:57:01.000000 spd_eda-0.0.7/src/spd_eda/athena_tools/__init__.py
--rw-rw-rw-   0        0        0     6643 2022-09-12 19:03:47.000000 spd_eda-0.0.7/src/spd_eda/athena_tools/athena_column.py
--rw-rw-rw-   0        0        0     9407 2022-09-13 16:49:56.000000 spd_eda-0.0.7/src/spd_eda/athena_tools/athena_table.py
--rw-rw-rw-   0        0        0      380 2022-09-12 19:03:47.000000 spd_eda-0.0.7/src/spd_eda/athena_tools/utils.py
-drwxrwxrwx   0        0        0        0 2022-10-24 19:57:41.746866 spd_eda-0.0.7/src/spd_eda/eda_tools/
--rw-rw-rw-   0        0        0        0 2022-09-08 18:55:20.000000 spd_eda-0.0.7/src/spd_eda/eda_tools/__init__.py
--rw-rw-rw-   0        0        0     9224 2022-10-24 15:15:09.000000 spd_eda-0.0.7/src/spd_eda/eda_tools/eda.py
-drwxrwxrwx   0        0        0        0 2022-10-24 19:57:41.751866 spd_eda-0.0.7/src/spd_eda/excel_tools/
--rw-rw-rw-   0        0        0        0 2022-09-08 19:22:51.000000 spd_eda-0.0.7/src/spd_eda/excel_tools/__init__.py
--rw-rw-rw-   0        0        0     7411 2022-10-24 16:58:22.000000 spd_eda-0.0.7/src/spd_eda/excel_tools/excel_output.py
-drwxrwxrwx   0        0        0        0 2022-10-24 19:57:41.780338 spd_eda-0.0.7/src/spd_eda/pa/
--rw-rw-rw-   0        0        0        0 2022-09-09 17:04:23.000000 spd_eda-0.0.7/src/spd_eda/pa/__init__.py
--rw-rw-rw-   0        0        0    38969 2022-09-15 14:49:00.000000 spd_eda-0.0.7/src/spd_eda/pa/analysis.py
--rw-rw-rw-   0        0        0     1993 2022-09-26 15:12:59.000000 spd_eda-0.0.7/src/spd_eda/pa/analysis_summary.py
--rw-rw-rw-   0        0        0     1218 2022-09-15 14:49:00.000000 spd_eda-0.0.7/src/spd_eda/pa/config.py
--rw-rw-rw-   0        0        0      241 2022-09-09 17:05:24.000000 spd_eda-0.0.7/src/spd_eda/pa/connection.py
--rw-rw-rw-   0        0        0     5615 2022-09-09 17:34:27.000000 spd_eda-0.0.7/src/spd_eda/pa/datasource.py
--rw-rw-rw-   0        0        0     3225 2022-09-09 17:34:27.000000 spd_eda-0.0.7/src/spd_eda/pa/dataview.py
--rw-rw-rw-   0        0        0    18925 2022-09-13 14:22:51.000000 spd_eda-0.0.7/src/spd_eda/pa/dataview_eda.py
--rw-rw-rw-   0        0        0    17580 2022-09-15 14:49:00.000000 spd_eda-0.0.7/src/spd_eda/pa/pa_stats.py
--rw-rw-rw-   0        0        0     5041 2022-09-14 15:46:48.000000 spd_eda-0.0.7/src/spd_eda/pa/plinko.py
-drwxrwxrwx   0        0        0        0 2022-10-24 19:57:41.790764 spd_eda-0.0.7/src/spd_eda/sql_tools/
--rw-rw-rw-   0        0        0        0 2022-09-12 19:35:04.000000 spd_eda-0.0.7/src/spd_eda/sql_tools/__init__.py
--rw-rw-rw-   0        0        0      241 2022-09-12 19:47:52.000000 spd_eda-0.0.7/src/spd_eda/sql_tools/connection.py
--rw-rw-rw-   0        0        0     4858 2022-09-12 20:38:00.000000 spd_eda-0.0.7/src/spd_eda/sql_tools/sql_table.py
--rw-rw-rw-   0        0        0      253 2022-09-12 19:53:22.000000 spd_eda-0.0.7/src/spd_eda/sql_tools/utils.py
-drwxrwxrwx   0        0        0        0 2022-10-24 19:57:41.730870 spd_eda-0.0.7/src/spd_eda.egg-info/
--rw-rw-rw-   0        0        0     9679 2022-10-24 19:57:41.000000 spd_eda-0.0.7/src/spd_eda.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      941 2022-10-24 19:57:41.000000 spd_eda-0.0.7/src/spd_eda.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-24 19:57:41.000000 spd_eda-0.0.7/src/spd_eda.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2022-10-24 19:57:41.000000 spd_eda-0.0.7/src/spd_eda.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-10-24 19:57:41.000000 spd_eda-0.0.7/src/spd_eda.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-19 13:47:20.072083 spd_eda-0.0.8/
+-rw-rw-rw-   0        0        0        0 2022-09-08 20:28:11.000000 spd_eda-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     9679 2023-07-19 13:47:20.070793 spd_eda-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     9316 2022-10-20 20:56:07.000000 spd_eda-0.0.8/README.md
+-rw-rw-rw-   0        0        0      661 2023-07-19 13:46:59.000000 spd_eda-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-19 13:47:20.073083 spd_eda-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-19 13:47:19.934114 spd_eda-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-07-19 13:47:19.956081 spd_eda-0.0.8/src/spd_eda/
+-rw-rw-rw-   0        0        0      647 2022-09-14 15:46:48.000000 spd_eda-0.0.8/src/spd_eda/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 13:47:19.990081 spd_eda-0.0.8/src/spd_eda/athena_tools/
+-rw-rw-rw-   0        0        0        0 2022-09-12 18:57:01.000000 spd_eda-0.0.8/src/spd_eda/athena_tools/__init__.py
+-rw-rw-rw-   0        0        0     6643 2022-09-12 19:03:47.000000 spd_eda-0.0.8/src/spd_eda/athena_tools/athena_column.py
+-rw-rw-rw-   0        0        0     9407 2022-09-13 16:49:56.000000 spd_eda-0.0.8/src/spd_eda/athena_tools/athena_table.py
+-rw-rw-rw-   0        0        0      380 2022-09-12 19:03:47.000000 spd_eda-0.0.8/src/spd_eda/athena_tools/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-19 13:47:19.997084 spd_eda-0.0.8/src/spd_eda/eda_tools/
+-rw-rw-rw-   0        0        0        0 2022-09-08 18:55:20.000000 spd_eda-0.0.8/src/spd_eda/eda_tools/__init__.py
+-rw-rw-rw-   0        0        0     9394 2023-02-01 17:37:20.000000 spd_eda-0.0.8/src/spd_eda/eda_tools/eda.py
+drwxrwxrwx   0        0        0        0 2023-07-19 13:47:20.006080 spd_eda-0.0.8/src/spd_eda/excel_tools/
+-rw-rw-rw-   0        0        0        0 2022-09-08 19:22:51.000000 spd_eda-0.0.8/src/spd_eda/excel_tools/__init__.py
+-rw-rw-rw-   0        0        0     7411 2022-10-24 16:58:22.000000 spd_eda-0.0.8/src/spd_eda/excel_tools/excel_output.py
+drwxrwxrwx   0        0        0        0 2023-07-19 13:47:20.050082 spd_eda-0.0.8/src/spd_eda/pa/
+-rw-rw-rw-   0        0        0        0 2022-09-09 17:04:23.000000 spd_eda-0.0.8/src/spd_eda/pa/__init__.py
+-rw-rw-rw-   0        0        0    38969 2022-09-15 14:49:00.000000 spd_eda-0.0.8/src/spd_eda/pa/analysis.py
+-rw-rw-rw-   0        0        0     1993 2022-09-26 15:12:59.000000 spd_eda-0.0.8/src/spd_eda/pa/analysis_summary.py
+-rw-rw-rw-   0        0        0     1218 2022-09-15 14:49:00.000000 spd_eda-0.0.8/src/spd_eda/pa/config.py
+-rw-rw-rw-   0        0        0      241 2022-09-09 17:05:24.000000 spd_eda-0.0.8/src/spd_eda/pa/connection.py
+-rw-rw-rw-   0        0        0     5615 2022-09-09 17:34:27.000000 spd_eda-0.0.8/src/spd_eda/pa/datasource.py
+-rw-rw-rw-   0        0        0     3225 2022-09-09 17:34:27.000000 spd_eda-0.0.8/src/spd_eda/pa/dataview.py
+-rw-rw-rw-   0        0        0    18925 2022-09-13 14:22:51.000000 spd_eda-0.0.8/src/spd_eda/pa/dataview_eda.py
+-rw-rw-rw-   0        0        0    17580 2022-09-15 14:49:00.000000 spd_eda-0.0.8/src/spd_eda/pa/pa_stats.py
+-rw-rw-rw-   0        0        0     5041 2022-09-14 15:46:48.000000 spd_eda-0.0.8/src/spd_eda/pa/plinko.py
+drwxrwxrwx   0        0        0        0 2023-07-19 13:47:20.065089 spd_eda-0.0.8/src/spd_eda/sql_tools/
+-rw-rw-rw-   0        0        0        0 2022-09-12 19:35:04.000000 spd_eda-0.0.8/src/spd_eda/sql_tools/__init__.py
+-rw-rw-rw-   0        0        0      241 2022-09-12 19:47:52.000000 spd_eda-0.0.8/src/spd_eda/sql_tools/connection.py
+-rw-rw-rw-   0        0        0     4858 2022-09-12 20:38:00.000000 spd_eda-0.0.8/src/spd_eda/sql_tools/sql_table.py
+-rw-rw-rw-   0        0        0      253 2022-09-12 19:53:22.000000 spd_eda-0.0.8/src/spd_eda/sql_tools/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-19 13:47:19.974080 spd_eda-0.0.8/src/spd_eda.egg-info/
+-rw-rw-rw-   0        0        0     9679 2023-07-19 13:47:19.000000 spd_eda-0.0.8/src/spd_eda.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      941 2023-07-19 13:47:19.000000 spd_eda-0.0.8/src/spd_eda.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 13:47:19.000000 spd_eda-0.0.8/src/spd_eda.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       96 2023-07-19 13:47:19.000000 spd_eda-0.0.8/src/spd_eda.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-19 13:47:19.000000 spd_eda-0.0.8/src/spd_eda.egg-info/top_level.txt
```

### Comparing `spd_eda-0.0.7/PKG-INFO` & `spd_eda-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spd_eda
-Version: 0.0.7
+Version: 0.0.8
 Summary: initial testing
 Author-email: sdooley <author@example.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `spd_eda-0.0.7/README.md` & `spd_eda-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `spd_eda-0.0.7/pyproject.toml` & `spd_eda-0.0.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b70 726f 6a65 6374 5d0d 0a6e 616d 6520  [project]..name 
 00000010: 3d20 2273 7064 5f65 6461 220d 0a76 6572  = "spd_eda"..ver
-00000020: 7369 6f6e 203d 2022 302e 302e 3722 0d0a  sion = "0.0.7"..
+00000020: 7369 6f6e 203d 2022 302e 302e 3822 0d0a  sion = "0.0.8"..
 00000030: 6175 7468 6f72 7320 3d20 5b0d 0a20 207b  authors = [..  {
 00000040: 206e 616d 653d 2273 646f 6f6c 6579 222c   name="sdooley",
 00000050: 2065 6d61 696c 3d22 6175 7468 6f72 4065   email="author@e
 00000060: 7861 6d70 6c65 2e63 6f6d 2220 7d2c 0d0a  xample.com" },..
 00000070: 5d0d 0a64 6573 6372 6970 7469 6f6e 203d  ]..description =
 00000080: 2022 696e 6974 6961 6c20 7465 7374 696e   "initial testin
 00000090: 6722 0d0a 7265 6164 6d65 203d 2022 5245  g"..readme = "RE
@@ -20,23 +20,23 @@
 00000130: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
 00000140: 4d49 5420 4c69 6365 6e73 6522 2c0d 0a20  MIT License",.. 
 00000150: 2020 2022 4f70 6572 6174 696e 6720 5379     "Operating Sy
 00000160: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
 00000170: 656e 6465 6e74 222c 0d0a 5d0d 0a64 6570  endent",..]..dep
 00000180: 656e 6465 6e63 6965 7320 3d20 5b0d 0a20  endencies = [.. 
 00000190: 2020 2022 7061 6e64 6173 3e3d 312e 342e     "pandas>=1.4.
-000001a0: 2a22 2c0d 0a20 2020 2022 786c 7378 7772  *",..    "xlsxwr
-000001b0: 6974 6572 3e3d 332e 302e 2a22 2c0d 0a20  iter>=3.0.*",.. 
+000001a0: 3422 2c0d 0a20 2020 2022 786c 7378 7772  4",..    "xlsxwr
+000001b0: 6974 6572 3e3d 332e 302e 3322 2c0d 0a20  iter>=3.0.3",.. 
 000001c0: 2020 2022 7079 6f64 6263 3e3d 342e 302e     "pyodbc>=4.0.
-000001d0: 2a22 2c0d 0a20 2020 2022 7365 6162 6f72  *",..    "seabor
-000001e0: 6e3e 3d30 2e31 322e 2a22 2c0d 0a20 2020  n>=0.12.*",..   
-000001f0: 2022 7363 6970 793e 3d31 2e39 2e2a 222c   "scipy>=1.9.*",
-00000200: 0d0a 2020 2020 2261 7773 7772 616e 676c  ..    "awswrangl
-00000210: 6572 3e3d 322e 3136 2e2a 220d 0a20 2020  er>=2.16.*"..   
-00000220: 205d 0d0a 0d0a 5b62 7569 6c64 2d73 7973   ]....[build-sys
-00000230: 7465 6d5d 0d0a 7265 7175 6972 6573 203d  tem]..requires =
-00000240: 205b 0d0a 2020 2020 2273 6574 7570 746f   [..    "setupto
-00000250: 6f6c 733e 3d34 3222 2c0d 0a20 2020 2022  ols>=42",..    "
-00000260: 7768 6565 6c22 0d0a 5d0d 0a62 7569 6c64  wheel"..]..build
-00000270: 2d62 6163 6b65 6e64 3d22 7365 7475 7074  -backend="setupt
-00000280: 6f6f 6c73 2e62 7569 6c64 5f6d 6574 6122  ools.build_meta"
-00000290: 0d0a 0d0a                                ....
+000001d0: 3334 222c 0d0a 2020 2020 2273 6561 626f  34",..    "seabo
+000001e0: 726e 3e3d 302e 3132 2e30 222c 0d0a 2020  rn>=0.12.0",..  
+000001f0: 2020 2273 6369 7079 3e3d 312e 392e 3122    "scipy>=1.9.1"
+00000200: 2c0d 0a20 2020 2022 6177 7377 7261 6e67  ,..    "awswrang
+00000210: 6c65 723e 3d32 2e31 362e 3122 0d0a 2020  ler>=2.16.1"..  
+00000220: 2020 5d0d 0a0d 0a5b 6275 696c 642d 7379    ]....[build-sy
+00000230: 7374 656d 5d0d 0a72 6571 7569 7265 7320  stem]..requires 
+00000240: 3d20 5b0d 0a20 2020 2022 7365 7475 7074  = [..    "setupt
+00000250: 6f6f 6c73 3e3d 3432 222c 0d0a 2020 2020  ools>=42",..    
+00000260: 2277 6865 656c 220d 0a5d 0d0a 6275 696c  "wheel"..]..buil
+00000270: 642d 6261 636b 656e 643d 2273 6574 7570  d-backend="setup
+00000280: 746f 6f6c 732e 6275 696c 645f 6d65 7461  tools.build_meta
+00000290: 220d 0a0d 0a                             "....
```

### Comparing `spd_eda-0.0.7/src/spd_eda/__init__.py` & `spd_eda-0.0.8/src/spd_eda/__init__.py`

 * *Files identical despite different names*

### Comparing `spd_eda-0.0.7/src/spd_eda/athena_tools/athena_column.py` & `spd_eda-0.0.8/src/spd_eda/athena_tools/athena_column.py`

 * *Files identical despite different names*

### Comparing `spd_eda-0.0.7/src/spd_eda/athena_tools/athena_table.py` & `spd_eda-0.0.8/src/spd_eda/athena_tools/athena_table.py`

 * *Files identical despite different names*

### Comparing `spd_eda-0.0.7/src/spd_eda/eda_tools/eda.py` & `spd_eda-0.0.8/src/spd_eda/eda_tools/eda.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 def create_categorical_series_no_missing(s, null_replacement='Missing-Values'):
     new_series = s.fillna(null_replacement).copy()
     new_series.name = f"{s.name}_clean"
     return new_series
 
 
 def calculate_cramers_v_value(contingency_table):
+    # TODO: Guard against blowing up when variables have no one-way stats (i.e. 100% missing values)
     if len(contingency_table) == 1:
         return 0.0
     else:
         try:
             (chi2_stat, p_val, df, expected) = scs.chi2_contingency(contingency_table.values)
         except ValueError:
             return -1
@@ -162,14 +163,15 @@
         weight_sse = (one_way_df[weight_col] * ((one_way_df[metric_col] - book_totals[metric_col]) ** 2)).sum()
         signal = ((weight_sse / book_totals[weight_col]) ** 0.5) / book_totals[metric_col]
         return signal
 
     def _get_series_for_signal_metric(self, metric_col, weight_col):
         signal_metric_dict = {}
         for col in self.df.columns.tolist():
+            print(f"_get_series_for_signal_metric for col: {col}")
             col_one_way_df = self.var_info_dict[col]['one_way']
             signal_metric_dict[col] = self._calculate_signal(col_one_way_df, metric_col, weight_col)
 
         signal_metric_series = pd.Series(signal_metric_dict)
         signal_metric_series.name = f"signal_{metric_col}"
 
         return signal_metric_series
```

### Comparing `spd_eda-0.0.7/src/spd_eda/excel_tools/excel_output.py` & `spd_eda-0.0.8/src/spd_eda/excel_tools/excel_output.py`

 * *Files identical despite different names*

### Comparing `spd_eda-0.0.7/src/spd_eda/pa/analysis.py` & `spd_eda-0.0.8/src/spd_eda/pa/analysis.py`

 * *Files identical despite different names*

### Comparing `spd_eda-0.0.7/src/spd_eda/pa/analysis_summary.py` & `spd_eda-0.0.8/src/spd_eda/pa/analysis_summary.py`

 * *Files identical despite different names*

### Comparing `spd_eda-0.0.7/src/spd_eda/pa/config.py` & `spd_eda-0.0.8/src/spd_eda/pa/config.py`

 * *Files identical despite different names*

### Comparing `spd_eda-0.0.7/src/spd_eda/pa/datasource.py` & `spd_eda-0.0.8/src/spd_eda/pa/datasource.py`

 * *Files identical despite different names*

### Comparing `spd_eda-0.0.7/src/spd_eda/pa/dataview.py` & `spd_eda-0.0.8/src/spd_eda/pa/dataview.py`

 * *Files identical despite different names*

### Comparing `spd_eda-0.0.7/src/spd_eda/pa/dataview_eda.py` & `spd_eda-0.0.8/src/spd_eda/pa/dataview_eda.py`

 * *Files identical despite different names*

### Comparing `spd_eda-0.0.7/src/spd_eda/pa/pa_stats.py` & `spd_eda-0.0.8/src/spd_eda/pa/pa_stats.py`

 * *Files identical despite different names*

### Comparing `spd_eda-0.0.7/src/spd_eda/pa/plinko.py` & `spd_eda-0.0.8/src/spd_eda/pa/plinko.py`

 * *Files identical despite different names*

### Comparing `spd_eda-0.0.7/src/spd_eda/sql_tools/sql_table.py` & `spd_eda-0.0.8/src/spd_eda/sql_tools/sql_table.py`

 * *Files identical despite different names*

### Comparing `spd_eda-0.0.7/src/spd_eda.egg-info/PKG-INFO` & `spd_eda-0.0.8/src/spd_eda.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spd-eda
-Version: 0.0.7
+Version: 0.0.8
 Summary: initial testing
 Author-email: sdooley <author@example.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `spd_eda-0.0.7/src/spd_eda.egg-info/SOURCES.txt` & `spd_eda-0.0.8/src/spd_eda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

