# Comparing `tmp/mcqq-tool-0.0.8.tar.gz` & `tmp/mcqq-tool-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcqq-tool-0.0.8.tar", last modified: Mon Jul  3 03:49:39 2023, max compression
+gzip compressed data, was "mcqq-tool-0.0.9.tar", last modified: Wed Jul 19 13:29:36 2023, max compression
```

## Comparing `mcqq-tool-0.0.8.tar` & `mcqq-tool-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:49:39.384939 mcqq-tool-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-03 03:49:28.000000 mcqq-tool-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-03 03:49:39.384939 mcqq-tool-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-03 03:49:28.000000 mcqq-tool-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:49:39.384939 mcqq-tool-0.0.8/mcqq_tool/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-03 03:49:28.000000 mcqq-tool-0.0.8/mcqq_tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-07-03 03:49:28.000000 mcqq-tool-0.0.8/mcqq_tool/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-07-03 03:49:28.000000 mcqq-tool-0.0.8/mcqq_tool/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:49:39.384939 mcqq-tool-0.0.8/mcqq_tool/model/
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-03 03:49:28.000000 mcqq-tool-0.0.8/mcqq_tool/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-03 03:49:28.000000 mcqq-tool-0.0.8/mcqq_tool/model/basemodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-03 03:49:28.000000 mcqq-tool-0.0.8/mcqq_tool/model/minecraft.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 03:49:28.000000 mcqq-tool-0.0.8/mcqq_tool/model/model_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-03 03:49:28.000000 mcqq-tool-0.0.8/mcqq_tool/model/spigot.py
--rw-r--r--   0 runner    (1001) docker     (123)    12814 2023-07-03 03:49:28.000000 mcqq-tool-0.0.8/mcqq_tool/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:49:39.384939 mcqq-tool-0.0.8/mcqq_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-03 03:49:39.000000 mcqq-tool-0.0.8/mcqq_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-03 03:49:39.000000 mcqq-tool-0.0.8/mcqq_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 03:49:39.000000 mcqq-tool-0.0.8/mcqq_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-03 03:49:39.000000 mcqq-tool-0.0.8/mcqq_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-03 03:49:39.000000 mcqq-tool-0.0.8/mcqq_tool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 03:49:39.384939 mcqq-tool-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-03 03:49:28.000000 mcqq-tool-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:29:36.315772 mcqq-tool-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-19 13:29:25.000000 mcqq-tool-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-19 13:29:36.315772 mcqq-tool-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-19 13:29:25.000000 mcqq-tool-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:29:36.311771 mcqq-tool-0.0.9/mcqq_tool/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-19 13:29:25.000000 mcqq-tool-0.0.9/mcqq_tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-07-19 13:29:25.000000 mcqq-tool-0.0.9/mcqq_tool/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-07-19 13:29:25.000000 mcqq-tool-0.0.9/mcqq_tool/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:29:36.311771 mcqq-tool-0.0.9/mcqq_tool/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-19 13:29:25.000000 mcqq-tool-0.0.9/mcqq_tool/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-19 13:29:25.000000 mcqq-tool-0.0.9/mcqq_tool/model/basemodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-19 13:29:25.000000 mcqq-tool-0.0.9/mcqq_tool/model/minecraft.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 13:29:25.000000 mcqq-tool-0.0.9/mcqq_tool/model/model_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-19 13:29:25.000000 mcqq-tool-0.0.9/mcqq_tool/model/spigot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12814 2023-07-19 13:29:25.000000 mcqq-tool-0.0.9/mcqq_tool/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:29:36.311771 mcqq-tool-0.0.9/mcqq_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-19 13:29:36.000000 mcqq-tool-0.0.9/mcqq_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-19 13:29:36.000000 mcqq-tool-0.0.9/mcqq_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 13:29:36.000000 mcqq-tool-0.0.9/mcqq_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-19 13:29:36.000000 mcqq-tool-0.0.9/mcqq_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-19 13:29:36.000000 mcqq-tool-0.0.9/mcqq_tool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 13:29:36.315772 mcqq-tool-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-19 13:29:25.000000 mcqq-tool-0.0.9/setup.py
```

### Comparing `mcqq-tool-0.0.8/LICENSE` & `mcqq-tool-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mcqq-tool-0.0.8/PKG-INFO` & `mcqq-tool-0.0.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcqq-tool
-Version: 0.0.8
+Version: 0.0.9
 Summary: MC_QQ 工具包
 Home-page: https://github.com/17TheWord/mcqq-tool
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mcqq-tool-0.0.8/mcqq_tool/common.py` & `mcqq-tool-0.0.9/mcqq_tool/common.py`

 * *Files identical despite different names*

### Comparing `mcqq-tool-0.0.8/mcqq_tool/config.py` & `mcqq-tool-0.0.9/mcqq_tool/config.py`

 * *Files identical despite different names*

### Comparing `mcqq-tool-0.0.8/mcqq_tool/model/__init__.py` & `mcqq-tool-0.0.9/mcqq_tool/model/__init__.py`

 * *Files identical despite different names*

### Comparing `mcqq-tool-0.0.8/mcqq_tool/model/basemodel.py` & `mcqq-tool-0.0.9/mcqq_tool/model/basemodel.py`

 * *Files identical despite different names*

### Comparing `mcqq-tool-0.0.8/mcqq_tool/model/minecraft.py` & `mcqq-tool-0.0.9/mcqq_tool/model/minecraft.py`

 * *Files identical despite different names*

### Comparing `mcqq-tool-0.0.8/mcqq_tool/model/spigot.py` & `mcqq-tool-0.0.9/mcqq_tool/model/spigot.py`

 * *Files identical despite different names*

### Comparing `mcqq-tool-0.0.8/mcqq_tool/utils.py` & `mcqq-tool-0.0.9/mcqq_tool/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,15 +232,15 @@
     """
     # 获取昵称
     member_nickname = await get_member_nickname(bot, event, event.user_id)
 
     # 初始化日志消息
     text_msg = member_nickname + " 说："
 
-    command_msg = "tellraw @p "
+    command_msg = "tellraw @a "
 
     message_list = [
         {"text": "[MC_QQ] ", "color": "yellow"},
     ]
     if plugin_config.mc_qq_send_group_name:
         if isinstance(event, GroupMessageEvent):
             message_list.append(
```

### Comparing `mcqq-tool-0.0.8/mcqq_tool.egg-info/PKG-INFO` & `mcqq-tool-0.0.9/mcqq_tool.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcqq-tool
-Version: 0.0.8
+Version: 0.0.9
 Summary: MC_QQ 工具包
 Home-page: https://github.com/17TheWord/mcqq-tool
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mcqq-tool-0.0.8/setup.py` & `mcqq-tool-0.0.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="mcqq-tool",
-    version="0.0.8",
+    version="0.0.9",
     author="17TheWord",
     author_email="17theword@gmail.com",
     description="MC_QQ 工具包",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/17TheWord/mcqq-tool",
     packages=setuptools.find_packages(),
```

