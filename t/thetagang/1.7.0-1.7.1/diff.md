# Comparing `tmp/thetagang-1.7.0.tar.gz` & `tmp/thetagang-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thetagang-1.7.0.tar", max compression
+gzip compressed data, was "thetagang-1.7.1.tar", max compression
```

## Comparing `thetagang-1.7.0.tar` & `thetagang-1.7.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    34523 2023-07-19 14:10:31.881745 thetagang-1.7.0/LICENSE
--rw-r--r--   0        0        0    14617 2023-07-19 14:10:31.881745 thetagang-1.7.0/README.md
--rw-r--r--   0        0        0     1660 2023-07-19 14:10:31.881745 thetagang-1.7.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-19 14:10:31.889746 thetagang-1.7.0/thetagang/__init__.py
--rw-r--r--   0        0        0     9120 2023-07-19 14:10:31.889746 thetagang-1.7.0/thetagang/config.py
--rw-r--r--   0        0        0     1396 2023-07-19 14:10:31.889746 thetagang-1.7.0/thetagang/config_defaults.py
--rw-r--r--   0        0        0     1461 2023-07-19 14:10:31.889746 thetagang-1.7.0/thetagang/dict_merge.py
--rw-r--r--   0        0        0       59 2023-07-19 14:10:31.889746 thetagang-1.7.0/thetagang/entry.py
--rw-r--r--   0        0        0     1091 2023-07-19 14:10:31.889746 thetagang-1.7.0/thetagang/fmt.py
--rw-r--r--   0        0        0     1022 2023-07-19 14:10:31.889746 thetagang-1.7.0/thetagang/main.py
--rw-r--r--   0        0        0      377 2023-07-19 14:10:31.889746 thetagang-1.7.0/thetagang/options.py
--rw-r--r--   0        0        0    79453 2023-07-19 14:10:31.889746 thetagang-1.7.0/thetagang/portfolio_manager.py
--rw-r--r--   0        0        0     3951 2023-07-19 14:10:31.889746 thetagang-1.7.0/thetagang/test_util.py
--rwxr-xr-x   0        0        0     8433 2023-07-19 14:10:31.889746 thetagang-1.7.0/thetagang/thetagang.py
--rw-r--r--   0        0        0     5820 2023-07-19 14:10:31.889746 thetagang-1.7.0/thetagang/util.py
--rw-r--r--   0        0        0    15877 1970-01-01 00:00:00.000000 thetagang-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-07-19 15:05:25.867614 thetagang-1.7.1/LICENSE
+-rw-r--r--   0        0        0    14617 2023-07-19 15:05:25.867614 thetagang-1.7.1/README.md
+-rw-r--r--   0        0        0     1660 2023-07-19 15:05:25.867614 thetagang-1.7.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-19 15:05:25.871614 thetagang-1.7.1/thetagang/__init__.py
+-rw-r--r--   0        0        0     9120 2023-07-19 15:05:25.871614 thetagang-1.7.1/thetagang/config.py
+-rw-r--r--   0        0        0     1396 2023-07-19 15:05:25.871614 thetagang-1.7.1/thetagang/config_defaults.py
+-rw-r--r--   0        0        0     1461 2023-07-19 15:05:25.871614 thetagang-1.7.1/thetagang/dict_merge.py
+-rw-r--r--   0        0        0       59 2023-07-19 15:05:25.871614 thetagang-1.7.1/thetagang/entry.py
+-rw-r--r--   0        0        0     1091 2023-07-19 15:05:25.871614 thetagang-1.7.1/thetagang/fmt.py
+-rw-r--r--   0        0        0     1022 2023-07-19 15:05:25.871614 thetagang-1.7.1/thetagang/main.py
+-rw-r--r--   0        0        0      377 2023-07-19 15:05:25.871614 thetagang-1.7.1/thetagang/options.py
+-rw-r--r--   0        0        0    79453 2023-07-19 15:05:25.875614 thetagang-1.7.1/thetagang/portfolio_manager.py
+-rw-r--r--   0        0        0     3951 2023-07-19 15:05:25.875614 thetagang-1.7.1/thetagang/test_util.py
+-rwxr-xr-x   0        0        0     8433 2023-07-19 15:05:25.875614 thetagang-1.7.1/thetagang/thetagang.py
+-rw-r--r--   0        0        0     5820 2023-07-19 15:05:25.875614 thetagang-1.7.1/thetagang/util.py
+-rw-r--r--   0        0        0    15877 1970-01-01 00:00:00.000000 thetagang-1.7.1/PKG-INFO
```

### Comparing `thetagang-1.7.0/LICENSE` & `thetagang-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `thetagang-1.7.0/README.md` & `thetagang-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `thetagang-1.7.0/pyproject.toml` & `thetagang-1.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 description = "ThetaGang is an IBKR bot for getting money"
 documentation = "https://github.com/brndnmtthws/thetagang/blob/master/README.md"
 homepage = "https://github.com/brndnmtthws/thetagang"
 license = "AGPL-3.0-only"
 name = "thetagang"
 readme = "README.md"
 repository = "https://github.com/brndnmtthws/thetagang.git"
-version = "1.7.0"
+version = "1.7.1"
 
 [tool.poetry.dependencies]
 click = "^8.1.3"
 click-log = "^0.4.0"
 ib_insync = "^0.9.86"
 python = ">=3.9,<4.0"
 python-dateutil = "^2.8.1"
```

### Comparing `thetagang-1.7.0/thetagang/config.py` & `thetagang-1.7.1/thetagang/config.py`

 * *Files identical despite different names*

### Comparing `thetagang-1.7.0/thetagang/config_defaults.py` & `thetagang-1.7.1/thetagang/config_defaults.py`

 * *Files identical despite different names*

### Comparing `thetagang-1.7.0/thetagang/dict_merge.py` & `thetagang-1.7.1/thetagang/dict_merge.py`

 * *Files identical despite different names*

### Comparing `thetagang-1.7.0/thetagang/fmt.py` & `thetagang-1.7.1/thetagang/fmt.py`

 * *Files identical despite different names*

### Comparing `thetagang-1.7.0/thetagang/main.py` & `thetagang-1.7.1/thetagang/main.py`

 * *Files identical despite different names*

### Comparing `thetagang-1.7.0/thetagang/portfolio_manager.py` & `thetagang-1.7.1/thetagang/portfolio_manager.py`

 * *Files identical despite different names*

### Comparing `thetagang-1.7.0/thetagang/test_util.py` & `thetagang-1.7.1/thetagang/test_util.py`

 * *Files identical despite different names*

### Comparing `thetagang-1.7.0/thetagang/thetagang.py` & `thetagang-1.7.1/thetagang/thetagang.py`

 * *Files identical despite different names*

### Comparing `thetagang-1.7.0/thetagang/util.py` & `thetagang-1.7.1/thetagang/util.py`

 * *Files identical despite different names*

### Comparing `thetagang-1.7.0/PKG-INFO` & `thetagang-1.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thetagang
-Version: 1.7.0
+Version: 1.7.1
 Summary: ThetaGang is an IBKR bot for getting money
 Home-page: https://github.com/brndnmtthws/thetagang
 License: AGPL-3.0-only
 Author: Brenden Matthews
 Author-email: brenden@brndn.io
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

