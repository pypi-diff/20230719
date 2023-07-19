# Comparing `tmp/finance-scrapers-0.0.3.tar.gz` & `tmp/finance-scrapers-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finance-scrapers-0.0.3.tar", last modified: Fri Jul 14 18:02:52 2023, max compression
+gzip compressed data, was "finance-scrapers-0.0.4.tar", last modified: Wed Jul 19 03:53:31 2023, max compression
```

## Comparing `finance-scrapers-0.0.3.tar` & `finance-scrapers-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:02:52.038704 finance-scrapers-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-14 18:02:38.000000 finance-scrapers-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-14 18:02:52.038704 finance-scrapers-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-14 18:02:38.000000 finance-scrapers-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:02:52.034704 finance-scrapers-0.0.3/finance_scrapers/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-14 18:02:38.000000 finance-scrapers-0.0.3/finance_scrapers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-07-14 18:02:38.000000 finance-scrapers-0.0.3/finance_scrapers/stock_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-07-14 18:02:38.000000 finance-scrapers-0.0.3/finance_scrapers/yahoo_finance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:02:52.038704 finance-scrapers-0.0.3/finance_scrapers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-14 18:02:52.000000 finance-scrapers-0.0.3/finance_scrapers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-14 18:02:52.000000 finance-scrapers-0.0.3/finance_scrapers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 18:02:52.000000 finance-scrapers-0.0.3/finance_scrapers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-14 18:02:52.000000 finance-scrapers-0.0.3/finance_scrapers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 18:02:52.000000 finance-scrapers-0.0.3/finance_scrapers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-14 18:02:38.000000 finance-scrapers-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-14 18:02:52.038704 finance-scrapers-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-19 03:53:31.077796 finance-scrapers-0.0.4/
+-rw-rw-rw-   0        0        0     1089 2023-07-14 03:22:40.000000 finance-scrapers-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     2147 2023-07-19 03:53:31.078796 finance-scrapers-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1582 2023-07-19 03:40:29.000000 finance-scrapers-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-19 03:53:31.073789 finance-scrapers-0.0.4/finance_scrapers/
+-rw-rw-rw-   0        0        0      158 2023-07-19 03:47:19.000000 finance-scrapers-0.0.4/finance_scrapers/__init__.py
+-rw-rw-rw-   0        0        0     3728 2023-07-19 03:15:42.000000 finance-scrapers-0.0.4/finance_scrapers/downloader.py
+-rw-rw-rw-   0        0        0     3403 2023-07-14 17:55:28.000000 finance-scrapers-0.0.4/finance_scrapers/stock_info.py
+-rw-rw-rw-   0        0        0    11034 2023-07-19 03:47:34.000000 finance-scrapers-0.0.4/finance_scrapers/yahoo_finance.py
+drwxrwxrwx   0        0        0        0 2023-07-19 03:53:31.077796 finance-scrapers-0.0.4/finance_scrapers.egg-info/
+-rw-rw-rw-   0        0        0     2147 2023-07-19 03:53:31.000000 finance-scrapers-0.0.4/finance_scrapers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      366 2023-07-19 03:53:31.000000 finance-scrapers-0.0.4/finance_scrapers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 03:53:31.000000 finance-scrapers-0.0.4/finance_scrapers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       92 2023-07-19 03:53:31.000000 finance-scrapers-0.0.4/finance_scrapers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-19 03:53:31.000000 finance-scrapers-0.0.4/finance_scrapers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       91 2023-07-14 03:22:40.000000 finance-scrapers-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      766 2023-07-19 03:53:31.078796 finance-scrapers-0.0.4/setup.cfg
```

### Comparing `finance-scrapers-0.0.3/LICENSE` & `finance-scrapers-0.0.4/LICENSE`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Mandy Cyber
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Mandy Cyber
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `finance-scrapers-0.0.3/finance_scrapers/stock_info.py` & `finance-scrapers-0.0.4/finance_scrapers/stock_info.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-from enum import Enum
-
-class StockInfo(Enum):
-    """
-    Represents all the XPATH positions of information available about a stock
-    """
-
-    INFO_1 = {
-        "name_loc": """//*[@id="quote-summary"]/div[1]/table/tbody/tr[1]/td[1]/span""", 
-        "info_loc": """//*[@id="quote-summary"]/div[1]/table/tbody/tr[1]/td[2]"""
-        }
-    
-    INFO_2 = {
-        "name_loc": """//*[@id="quote-summary"]/div[1]/table/tbody/tr[2]/td[1]/span""", 
-        "info_loc": """//*[@id="quote-summary"]/div[1]/table/tbody/tr[2]/td[2]"""
-        }
-    
-    INFO_3 = {
-        "name_loc": """//*[@id="quote-summary"]/div[1]/table/tbody/tr[3]/td[1]/span""", 
-        "info_loc": """//*[@id="quote-summary"]/div[1]/table/tbody/tr[3]/td[2]"""
-        }
-    
-    INFO_4 = {
-        "name_loc": """//*[@id="quote-summary"]/div[1]/table/tbody/tr[4]/td[1]/span""", 
-        "info_loc": """//*[@id="quote-summary"]/div[1]/table/tbody/tr[4]/td[2]"""
-        }
-    
-    INFO_5 = {
-        "name_loc": """//*[@id="quote-summary"]/div[1]/table/tbody/tr[5]/td[1]/span""", 
-        "info_loc": """//*[@id="quote-summary"]/div[1]/table/tbody/tr[5]/td[2]"""
-        }
-    
-    INFO_6 = {
-        "name_loc": """//*[@id="quote-summary"]/div[1]/table/tbody/tr[6]/td[1]/span""", 
-        "info_loc": """//*[@id="quote-summary"]/div[1]/table/tbody/tr[6]/td[2]"""
-        }
-
-    INFO_7 = {
-        "name_loc": """//*[@id="quote-summary"]/div[1]/table/tbody/tr[7]/td[1]/span""", 
-        "info_loc": """//*[@id="quote-summary"]/div[1]/table/tbody/tr[7]/td[2]"""
-        }
-
-    INFO_8 = {
-        "name_loc": """//*[@id="quote-summary"]/div[1]/table/tbody/tr[8]/td[1]/span""", 
-        "info_loc": """//*[@id="quote-summary"]/div[1]/table/tbody/tr[8]/td[2]"""
-        }
-
-    INFO_9 = {
-        "name_loc": """//*[@id="quote-summary"]/div[2]/table/tbody/tr[1]/td[1]/span""", 
-        "info_loc": """//*[@id="quote-summary"]/div[2]/table/tbody/tr[1]/td[2]"""
-        }
-
-    INFO_10 = {
-        "name_loc": """//*[@id="quote-summary"]/div[2]/table/tbody/tr[3]/td[1]/span""", 
-        "info_loc": """//*[@id="quote-summary"]/div[2]/table/tbody/tr[2]/td[2]"""
-        }
-
-    INFO_11 = {
-        "name_loc": """//*[@id="quote-summary"]/div[2]/table/tbody/tr[3]/td[1]/span""", 
-        "info_loc": """//*[@id="quote-summary"]/div[2]/table/tbody/tr[3]/td[2]"""
-        }
-
-    INFO_12 = {
-        "name_loc": """//*[@id="quote-summary"]/div[2]/table/tbody/tr[4]/td[1]/span""", 
-        "info_loc": """//*[@id="quote-summary"]/div[2]/table/tbody/tr[4]/td[2]"""
-        }
-
-    INFO_13 = {
-        "name_loc": """//*[@id="quote-summary"]/div[2]/table/tbody/tr[5]/td[1]/span""", 
-        "info_loc": """//*[@id="quote-summary"]/div[2]/table/tbody/tr[5]/td[2]"""
-        }
-
-    INFO_14 = {
-        "name_loc": """//*[@id="quote-summary"]/div[2]/table/tbody/tr[6]/td[1]/span""", 
-        "info_loc": """//*[@id="quote-summary"]/div[2]/table/tbody/tr[6]/td[2]"""
-        }
-
-    INFO_15 = {
-        "name_loc": """//*[@id="quote-summary"]/div[1]/table/tbody/tr[7]/td[1]/span""", 
-        "info_loc": """//*[@id="quote-summary"]/div[2]/table/tbody/tr[7]/td[2]"""
-        }
-
-    INFO_16 = {
-        "name_loc": """//*[@id="quote-summary"]/div[1]/table/tbody/tr[8]/td[1]/span""", 
-        "info_loc": """//*[@id="quote-summary"]/div[2]/table/tbody/tr[8]/td[2]"""
+from enum import Enum
+
+class StockInfo(Enum):
+    """
+    Represents all the XPATH positions of information available about a stock
+    """
+
+    INFO_1 = {
+        "name_loc": """//*[@id="quote-summary"]/div[1]/table/tbody/tr[1]/td[1]/span""", 
+        "info_loc": """//*[@id="quote-summary"]/div[1]/table/tbody/tr[1]/td[2]"""
+        }
+    
+    INFO_2 = {
+        "name_loc": """//*[@id="quote-summary"]/div[1]/table/tbody/tr[2]/td[1]/span""", 
+        "info_loc": """//*[@id="quote-summary"]/div[1]/table/tbody/tr[2]/td[2]"""
+        }
+    
+    INFO_3 = {
+        "name_loc": """//*[@id="quote-summary"]/div[1]/table/tbody/tr[3]/td[1]/span""", 
+        "info_loc": """//*[@id="quote-summary"]/div[1]/table/tbody/tr[3]/td[2]"""
+        }
+    
+    INFO_4 = {
+        "name_loc": """//*[@id="quote-summary"]/div[1]/table/tbody/tr[4]/td[1]/span""", 
+        "info_loc": """//*[@id="quote-summary"]/div[1]/table/tbody/tr[4]/td[2]"""
+        }
+    
+    INFO_5 = {
+        "name_loc": """//*[@id="quote-summary"]/div[1]/table/tbody/tr[5]/td[1]/span""", 
+        "info_loc": """//*[@id="quote-summary"]/div[1]/table/tbody/tr[5]/td[2]"""
+        }
+    
+    INFO_6 = {
+        "name_loc": """//*[@id="quote-summary"]/div[1]/table/tbody/tr[6]/td[1]/span""", 
+        "info_loc": """//*[@id="quote-summary"]/div[1]/table/tbody/tr[6]/td[2]"""
+        }
+
+    INFO_7 = {
+        "name_loc": """//*[@id="quote-summary"]/div[1]/table/tbody/tr[7]/td[1]/span""", 
+        "info_loc": """//*[@id="quote-summary"]/div[1]/table/tbody/tr[7]/td[2]"""
+        }
+
+    INFO_8 = {
+        "name_loc": """//*[@id="quote-summary"]/div[1]/table/tbody/tr[8]/td[1]/span""", 
+        "info_loc": """//*[@id="quote-summary"]/div[1]/table/tbody/tr[8]/td[2]"""
+        }
+
+    INFO_9 = {
+        "name_loc": """//*[@id="quote-summary"]/div[2]/table/tbody/tr[1]/td[1]/span""", 
+        "info_loc": """//*[@id="quote-summary"]/div[2]/table/tbody/tr[1]/td[2]"""
+        }
+
+    INFO_10 = {
+        "name_loc": """//*[@id="quote-summary"]/div[2]/table/tbody/tr[3]/td[1]/span""", 
+        "info_loc": """//*[@id="quote-summary"]/div[2]/table/tbody/tr[2]/td[2]"""
+        }
+
+    INFO_11 = {
+        "name_loc": """//*[@id="quote-summary"]/div[2]/table/tbody/tr[3]/td[1]/span""", 
+        "info_loc": """//*[@id="quote-summary"]/div[2]/table/tbody/tr[3]/td[2]"""
+        }
+
+    INFO_12 = {
+        "name_loc": """//*[@id="quote-summary"]/div[2]/table/tbody/tr[4]/td[1]/span""", 
+        "info_loc": """//*[@id="quote-summary"]/div[2]/table/tbody/tr[4]/td[2]"""
+        }
+
+    INFO_13 = {
+        "name_loc": """//*[@id="quote-summary"]/div[2]/table/tbody/tr[5]/td[1]/span""", 
+        "info_loc": """//*[@id="quote-summary"]/div[2]/table/tbody/tr[5]/td[2]"""
+        }
+
+    INFO_14 = {
+        "name_loc": """//*[@id="quote-summary"]/div[2]/table/tbody/tr[6]/td[1]/span""", 
+        "info_loc": """//*[@id="quote-summary"]/div[2]/table/tbody/tr[6]/td[2]"""
+        }
+
+    INFO_15 = {
+        "name_loc": """//*[@id="quote-summary"]/div[1]/table/tbody/tr[7]/td[1]/span""", 
+        "info_loc": """//*[@id="quote-summary"]/div[2]/table/tbody/tr[7]/td[2]"""
+        }
+
+    INFO_16 = {
+        "name_loc": """//*[@id="quote-summary"]/div[1]/table/tbody/tr[8]/td[1]/span""", 
+        "info_loc": """//*[@id="quote-summary"]/div[2]/table/tbody/tr[8]/td[2]"""
         }
```

