# Comparing `tmp/nonebot_plugin_dall-e-0.2.tar.gz` & `tmp/nonebot_plugin_dall-e-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_dall-e-0.2.tar", last modified: Wed Jul 19 01:30:58 2023, max compression
+gzip compressed data, was "nonebot_plugin_dall-e-0.3.tar", last modified: Wed Jul 19 01:50:45 2023, max compression
```

## Comparing `nonebot_plugin_dall-e-0.2.tar` & `nonebot_plugin_dall-e-0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 01:30:58.095930 nonebot_plugin_dall-e-0.2/
--rw-rw-rw-   0        0        0    11558 2023-07-18 15:29:46.000000 nonebot_plugin_dall-e-0.2/LICENSE
--rw-rw-rw-   0        0        0      367 2023-07-19 01:30:58.095930 nonebot_plugin_dall-e-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2487 2023-07-18 15:09:46.000000 nonebot_plugin_dall-e-0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-19 01:30:58.083205 nonebot_plugin_dall-e-0.2/nonebot_plugin_dall-e/
--rw-rw-rw-   0        0        0     5609 2023-07-18 14:47:40.000000 nonebot_plugin_dall-e-0.2/nonebot_plugin_dall-e/__init__.py
--rw-rw-rw-   0        0        0     3733 2023-07-18 14:47:40.000000 nonebot_plugin_dall-e-0.2/nonebot_plugin_dall-e/openai.py
--rw-rw-rw-   0        0        0     2733 2023-07-18 14:58:37.000000 nonebot_plugin_dall-e-0.2/nonebot_plugin_dall-e/tools.py
-drwxrwxrwx   0        0        0        0 2023-07-19 01:30:58.095930 nonebot_plugin_dall-e-0.2/nonebot_plugin_dall_e.egg-info/
--rw-rw-rw-   0        0        0      367 2023-07-19 01:30:58.000000 nonebot_plugin_dall-e-0.2/nonebot_plugin_dall_e.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      347 2023-07-19 01:30:58.000000 nonebot_plugin_dall-e-0.2/nonebot_plugin_dall_e.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 01:30:58.000000 nonebot_plugin_dall-e-0.2/nonebot_plugin_dall_e.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-07-19 01:30:58.000000 nonebot_plugin_dall-e-0.2/nonebot_plugin_dall_e.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-07-19 01:30:58.000000 nonebot_plugin_dall-e-0.2/nonebot_plugin_dall_e.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-19 01:30:58.095930 nonebot_plugin_dall-e-0.2/setup.cfg
--rw-rw-rw-   0        0        0      759 2023-07-19 01:29:41.000000 nonebot_plugin_dall-e-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 01:50:45.687287 nonebot_plugin_dall-e-0.3/
+-rw-rw-rw-   0        0        0    11558 2023-07-18 15:29:46.000000 nonebot_plugin_dall-e-0.3/LICENSE
+-rw-rw-rw-   0        0        0      367 2023-07-19 01:50:45.687287 nonebot_plugin_dall-e-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2487 2023-07-18 15:09:46.000000 nonebot_plugin_dall-e-0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-19 01:50:45.687287 nonebot_plugin_dall-e-0.3/nonebot_plugin_dall-e/
+-rw-rw-rw-   0        0        0     6031 2023-07-19 01:49:22.000000 nonebot_plugin_dall-e-0.3/nonebot_plugin_dall-e/__init__.py
+-rw-rw-rw-   0        0        0     3733 2023-07-18 14:47:40.000000 nonebot_plugin_dall-e-0.3/nonebot_plugin_dall-e/openai.py
+-rw-rw-rw-   0        0        0     2733 2023-07-18 14:58:37.000000 nonebot_plugin_dall-e-0.3/nonebot_plugin_dall-e/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-19 01:50:45.687287 nonebot_plugin_dall-e-0.3/nonebot_plugin_dall_e.egg-info/
+-rw-rw-rw-   0        0        0      367 2023-07-19 01:50:45.000000 nonebot_plugin_dall-e-0.3/nonebot_plugin_dall_e.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      347 2023-07-19 01:50:45.000000 nonebot_plugin_dall-e-0.3/nonebot_plugin_dall_e.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 01:50:45.000000 nonebot_plugin_dall-e-0.3/nonebot_plugin_dall_e.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-07-19 01:50:45.000000 nonebot_plugin_dall-e-0.3/nonebot_plugin_dall_e.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-19 01:50:45.000000 nonebot_plugin_dall-e-0.3/nonebot_plugin_dall_e.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-19 01:50:45.687287 nonebot_plugin_dall-e-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      759 2023-07-19 01:49:22.000000 nonebot_plugin_dall-e-0.3/setup.py
```

### Comparing `nonebot_plugin_dall-e-0.2/LICENSE` & `nonebot_plugin_dall-e-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_dall-e-0.2/README.md` & `nonebot_plugin_dall-e-0.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_dall-e-0.2/nonebot_plugin_dall-e/__init__.py` & `nonebot_plugin_dall-e-0.3/nonebot_plugin_dall-e/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,34 @@
 from nonebot import get_driver, on_command
 from nonebot.adapters.onebot.v11 import Message, MessageEvent, PrivateMessageEvent, MessageSegment, GroupMessageEvent
 from nonebot.adapters.onebot.v11.helpers import ImageURLs
 from nonebot.params import CommandArg
 from nonebot.rule import to_me
 from enum import Enum
+from nonebot.plugin import PluginMetadata
 import threading
 from typing import Optional
 from nonebot.permission import SUPERUSER
 from .openai import DALLEKeyManager
 from .tools import *
 
+__version__ = "0.3"
+__plugin_meta__ = PluginMetadata(
+    name="DALL-E绘图",
+    description='使用DALL·E绘图',
+    type="application",
+    usage='',
+    homepage="https://github.com/Rockytkg/nonebot_plugin_dall-e",
+    supported_adapters={"~onebot.v11"},
+    extra={
+        "version": __version__,
+        "author": "Agnes4m <2696916846@qq.com>",
+    },
+)
+
 superusers = get_driver().config.superusers
 usageCountPerMinuteKey = get_driver().config.usageCountPerMinuteKey
 
 
 class Size(Enum):
     SMALL = '256x256'
     MEDIUM = '512x512'
```

### Comparing `nonebot_plugin_dall-e-0.2/nonebot_plugin_dall-e/openai.py` & `nonebot_plugin_dall-e-0.3/nonebot_plugin_dall-e/openai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_dall-e-0.2/nonebot_plugin_dall-e/tools.py` & `nonebot_plugin_dall-e-0.3/nonebot_plugin_dall-e/tools.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_dall-e-0.2/setup.py` & `nonebot_plugin_dall-e-0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="nonebot_plugin_dall-e",
-    version="0.2",
+    version="0.3",
     packages=find_packages(),
     install_requires=["nonebot2", "openai", "pillow", "aiohttp", "nonebot-adapter-onebot"],
 
     author="Join-liu",
     author_email="2696916846@qq.com",
     description="""
     A nonebot2 plugin that uses a key pool and key polling technology to manage API calls effectively.
```

