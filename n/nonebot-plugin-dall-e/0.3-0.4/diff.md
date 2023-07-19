# Comparing `tmp/nonebot_plugin_dall-e-0.3.tar.gz` & `tmp/nonebot_plugin_dall-e-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_dall-e-0.3.tar", last modified: Wed Jul 19 01:50:45 2023, max compression
+gzip compressed data, was "nonebot_plugin_dall-e-0.4.tar", last modified: Wed Jul 19 02:13:36 2023, max compression
```

## Comparing `nonebot_plugin_dall-e-0.3.tar` & `nonebot_plugin_dall-e-0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 01:50:45.687287 nonebot_plugin_dall-e-0.3/
--rw-rw-rw-   0        0        0    11558 2023-07-18 15:29:46.000000 nonebot_plugin_dall-e-0.3/LICENSE
--rw-rw-rw-   0        0        0      367 2023-07-19 01:50:45.687287 nonebot_plugin_dall-e-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2487 2023-07-18 15:09:46.000000 nonebot_plugin_dall-e-0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-19 01:50:45.687287 nonebot_plugin_dall-e-0.3/nonebot_plugin_dall-e/
--rw-rw-rw-   0        0        0     6031 2023-07-19 01:49:22.000000 nonebot_plugin_dall-e-0.3/nonebot_plugin_dall-e/__init__.py
--rw-rw-rw-   0        0        0     3733 2023-07-18 14:47:40.000000 nonebot_plugin_dall-e-0.3/nonebot_plugin_dall-e/openai.py
--rw-rw-rw-   0        0        0     2733 2023-07-18 14:58:37.000000 nonebot_plugin_dall-e-0.3/nonebot_plugin_dall-e/tools.py
-drwxrwxrwx   0        0        0        0 2023-07-19 01:50:45.687287 nonebot_plugin_dall-e-0.3/nonebot_plugin_dall_e.egg-info/
--rw-rw-rw-   0        0        0      367 2023-07-19 01:50:45.000000 nonebot_plugin_dall-e-0.3/nonebot_plugin_dall_e.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      347 2023-07-19 01:50:45.000000 nonebot_plugin_dall-e-0.3/nonebot_plugin_dall_e.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 01:50:45.000000 nonebot_plugin_dall-e-0.3/nonebot_plugin_dall_e.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-07-19 01:50:45.000000 nonebot_plugin_dall-e-0.3/nonebot_plugin_dall_e.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-07-19 01:50:45.000000 nonebot_plugin_dall-e-0.3/nonebot_plugin_dall_e.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-19 01:50:45.687287 nonebot_plugin_dall-e-0.3/setup.cfg
--rw-rw-rw-   0        0        0      759 2023-07-19 01:49:22.000000 nonebot_plugin_dall-e-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 02:13:36.211638 nonebot_plugin_dall-e-0.4/
+-rw-rw-rw-   0        0        0    11558 2023-07-18 15:29:46.000000 nonebot_plugin_dall-e-0.4/LICENSE
+-rw-rw-rw-   0        0        0      367 2023-07-19 02:13:36.211638 nonebot_plugin_dall-e-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2487 2023-07-18 15:09:46.000000 nonebot_plugin_dall-e-0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-19 02:13:36.205415 nonebot_plugin_dall-e-0.4/nonebot_plugin_dall-e/
+-rw-rw-rw-   0        0        0     6031 2023-07-19 02:10:23.000000 nonebot_plugin_dall-e-0.4/nonebot_plugin_dall-e/__init__.py
+-rw-rw-rw-   0        0        0     3865 2023-07-19 01:58:14.000000 nonebot_plugin_dall-e-0.4/nonebot_plugin_dall-e/openai.py
+-rw-rw-rw-   0        0        0     2774 2023-07-19 01:59:32.000000 nonebot_plugin_dall-e-0.4/nonebot_plugin_dall-e/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-19 02:13:36.210323 nonebot_plugin_dall-e-0.4/nonebot_plugin_dall_e.egg-info/
+-rw-rw-rw-   0        0        0      367 2023-07-19 02:13:36.000000 nonebot_plugin_dall-e-0.4/nonebot_plugin_dall_e.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      347 2023-07-19 02:13:36.000000 nonebot_plugin_dall-e-0.4/nonebot_plugin_dall_e.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 02:13:36.000000 nonebot_plugin_dall-e-0.4/nonebot_plugin_dall_e.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-07-19 02:13:36.000000 nonebot_plugin_dall-e-0.4/nonebot_plugin_dall_e.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-19 02:13:36.000000 nonebot_plugin_dall-e-0.4/nonebot_plugin_dall_e.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-19 02:13:36.212700 nonebot_plugin_dall-e-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      759 2023-07-19 02:10:23.000000 nonebot_plugin_dall-e-0.4/setup.py
```

### Comparing `nonebot_plugin_dall-e-0.3/LICENSE` & `nonebot_plugin_dall-e-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_dall-e-0.3/README.md` & `nonebot_plugin_dall-e-0.4/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_dall-e-0.3/nonebot_plugin_dall-e/__init__.py` & `nonebot_plugin_dall-e-0.4/nonebot_plugin_dall-e/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,30 +7,30 @@
 from nonebot.plugin import PluginMetadata
 import threading
 from typing import Optional
 from nonebot.permission import SUPERUSER
 from .openai import DALLEKeyManager
 from .tools import *
 
-__version__ = "0.3"
+__version__ = "0.4"
 __plugin_meta__ = PluginMetadata(
     name="DALL-E绘图",
     description='使用DALL·E绘图',
     type="application",
     usage='',
     homepage="https://github.com/Rockytkg/nonebot_plugin_dall-e",
     supported_adapters={"~onebot.v11"},
     extra={
         "version": __version__,
         "author": "Agnes4m <2696916846@qq.com>",
     },
 )
 
 superusers = get_driver().config.superusers
-usageCountPerMinuteKey = get_driver().config.usageCountPerMinuteKey
+usageCountPerMinuteKey = get_driver().config.usagecountperminutekey
 
 
 class Size(Enum):
     SMALL = '256x256'
     MEDIUM = '512x512'
     LARGE = '1024x1024'
```

### Comparing `nonebot_plugin_dall-e-0.3/nonebot_plugin_dall-e/openai.py` & `nonebot_plugin_dall-e-0.4/nonebot_plugin_dall-e/openai.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,16 +17,21 @@
         # 为每个key创建一个长度为3的队列，用于存储使用时间
         self.key_usage = {key: deque(maxlen=usage_count_per_minute_key) for key in keys}
         # 创建一个条件变量，用于等待key的释放
         self.condition = asyncio.Condition()
 
     @staticmethod
     def read_keys_from_file():
-        # 从文件中读取key
-        key_file = Path() / "data" / "openai_key.txt"
+        # 生成文件路径
+        key_file = Path("data") / "openai_key.txt"
+
+        # 检查文件是否存在，如果不存在则创建文件
+        if not key_file.exists():
+            key_file.touch()
+
         with open(key_file, 'r', encoding="utf8") as f:
             keys = [line.strip() for line in f.readlines()]
         return keys
 
     async def get_key(self):
         # 循环直到获取一个可用的key
         while True:
```

### Comparing `nonebot_plugin_dall-e-0.3/nonebot_plugin_dall-e/tools.py` & `nonebot_plugin_dall-e-0.4/nonebot_plugin_dall-e/tools.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from pathlib import Path
-import codecs
 from nonebot.log import logger
 from io import BytesIO
 import aiohttp
 
 
 class DFAFilter:
     def __init__(self):
         self.keyword_chains = {}
         self.delimit = '\x00'
         self.load_keywords()
 
     def load_keywords(self):
-        file_name = str(Path() / "data" / "违禁词.txt")
-        with codecs.open(file_name, 'r', encoding='utf8') as f:
-            for line in f:
+        file_path = Path("data") / "违禁词.txt"
+
+        if not file_path.exists():
+            file_path.touch()
+
+        with open(file_path, 'r', encoding='utf8') as file:
+            for line in file:
                 stripped_line = line.strip()
-                if stripped_line != '':
+                if stripped_line:
                     self.add(stripped_line)
 
     def add(self, keyword):
         keyword = keyword.lower()
         chars = keyword.strip()
         if not chars:
             return
```

### Comparing `nonebot_plugin_dall-e-0.3/setup.py` & `nonebot_plugin_dall-e-0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="nonebot_plugin_dall-e",
-    version="0.3",
+    version="0.4",
     packages=find_packages(),
     install_requires=["nonebot2", "openai", "pillow", "aiohttp", "nonebot-adapter-onebot"],
 
     author="Join-liu",
     author_email="2696916846@qq.com",
     description="""
     A nonebot2 plugin that uses a key pool and key polling technology to manage API calls effectively.
```

