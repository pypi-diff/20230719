# Comparing `tmp/herta_villa_sdk-0.6.0.tar.gz` & `tmp/herta_villa_sdk-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "herta_villa_sdk-0.6.0.tar", last modified: Mon Jul 17 10:53:00 2023, max compression
+gzip compressed data, was "herta_villa_sdk-0.6.1.tar", last modified: Wed Jul 19 02:30:29 2023, max compression
```

## Comparing `herta_villa_sdk-0.6.0.tar` & `herta_villa_sdk-0.6.1.tar`

### file list

```diff
@@ -1,34 +1,41 @@
--rw-r--r--   0        0        0     1068 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/LICENSE
--rw-r--r--   0        0        0     4420 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/README.md
--rw-r--r--   0        0        0      668 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/__init__.py
--rw-r--r--   0        0        0        0 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/apis/__init__.py
--rw-r--r--   0        0        0      782 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/apis/auth.py
--rw-r--r--   0        0        0     1739 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/apis/base.py
--rw-r--r--   0        0        0      520 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/apis/emoticon.py
--rw-r--r--   0        0        0      611 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/apis/img.py
--rw-r--r--   0        0        0     2174 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/apis/member.py
--rw-r--r--   0        0        0     2710 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/apis/message.py
--rw-r--r--   0        0        0     4422 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/apis/role.py
--rw-r--r--   0        0        0     4190 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/apis/room.py
--rw-r--r--   0        0        0      645 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/apis/villa.py
--rw-r--r--   0        0        0     7869 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/bot.py
--rw-r--r--   0        0        0     5398 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/event.py
--rw-r--r--   0        0        0     1060 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/exception.py
--rw-r--r--   0        0        0     1481 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/match.py
--rw-r--r--   0        0        0      353 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/message/__init__.py
--rw-r--r--   0        0        0     3799 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/message/chain.py
--rw-r--r--   0        0        0     1414 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/message/image.py
--rw-r--r--   0        0        0      927 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/message/post.py
--rw-r--r--   0        0        0     6289 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/message/text.py
--rw-r--r--   0        0        0      442 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/message/types.py
--rw-r--r--   0        0        0     6280 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/model.py
--rw-r--r--   0        0        0      970 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/server/__init__.py
--rw-r--r--   0        0        0     1383 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/server/aiohttp.py
--rw-r--r--   0        0        0     1653 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/server/fastapi.py
--rw-r--r--   0        0        0     3081 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/server/internal.py
--rw-r--r--   0        0        0      564 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/typing.py
--rw-r--r--   0        0        0      563 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/utils.py
--rw-r--r--   0        0        0       58 2023-07-17 10:52:21.357138 herta_villa_sdk-0.6.0/hertavilla/version.py
--rw-r--r--   0        0        0     2278 2023-07-17 10:53:00.129792 herta_villa_sdk-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      528 2023-07-17 10:52:21.361139 herta_villa_sdk-0.6.0/tests/test_utils.py
--rw-r--r--   0        0        0     5202 1970-01-01 00:00:00.000000 herta_villa_sdk-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-07-17 10:30:29.148597 herta_villa_sdk-0.6.1/LICENSE
+-rw-r--r--   0        0        0     4624 2023-07-19 02:26:51.304211 herta_villa_sdk-0.6.1/README.md
+-rw-r--r--   0        0        0      694 2023-07-17 10:30:29.148597 herta_villa_sdk-0.6.1/hertavilla/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-11 03:47:58.704094 herta_villa_sdk-0.6.1/hertavilla/apis/__init__.py
+-rw-r--r--   0        0        0      808 2023-07-11 03:47:58.704094 herta_villa_sdk-0.6.1/hertavilla/apis/auth.py
+-rw-r--r--   0        0        0     1804 2023-07-17 11:11:09.233220 herta_villa_sdk-0.6.1/hertavilla/apis/base.py
+-rw-r--r--   0        0        0      541 2023-07-11 03:47:58.719717 herta_villa_sdk-0.6.1/hertavilla/apis/emoticon.py
+-rw-r--r--   0        0        0      636 2023-07-17 10:30:29.148597 herta_villa_sdk-0.6.1/hertavilla/apis/img.py
+-rw-r--r--   0        0        0     2248 2023-07-11 03:47:58.719825 herta_villa_sdk-0.6.1/hertavilla/apis/member.py
+-rw-r--r--   0        0        0     2809 2023-07-11 03:47:58.719825 herta_villa_sdk-0.6.1/hertavilla/apis/message.py
+-rw-r--r--   0        0        0     4571 2023-07-11 03:47:58.720329 herta_villa_sdk-0.6.1/hertavilla/apis/role.py
+-rw-r--r--   0        0        0     4355 2023-07-11 03:47:58.720329 herta_villa_sdk-0.6.1/hertavilla/apis/room.py
+-rw-r--r--   0        0        0      671 2023-07-11 03:47:58.720329 herta_villa_sdk-0.6.1/hertavilla/apis/villa.py
+-rw-r--r--   0        0        0     8156 2023-07-17 11:11:09.233220 herta_villa_sdk-0.6.1/hertavilla/bot.py
+-rw-r--r--   0        0        0     5631 2023-07-11 03:47:58.720329 herta_villa_sdk-0.6.1/hertavilla/event.py
+-rw-r--r--   0        0        0     1108 2023-07-17 11:11:09.233220 herta_villa_sdk-0.6.1/hertavilla/exception.py
+-rw-r--r--   0        0        0     1537 2023-06-23 08:30:51.896265 herta_villa_sdk-0.6.1/hertavilla/match.py
+-rw-r--r--   0        0        0      366 2023-06-21 17:10:20.989824 herta_villa_sdk-0.6.1/hertavilla/message/__init__.py
+-rw-r--r--   0        0        0     3917 2023-07-07 08:04:43.463528 herta_villa_sdk-0.6.1/hertavilla/message/chain.py
+-rw-r--r--   0        0        0     1472 2023-07-07 08:04:43.463528 herta_villa_sdk-0.6.1/hertavilla/message/image.py
+-rw-r--r--   0        0        0      969 2023-07-07 08:04:43.463528 herta_villa_sdk-0.6.1/hertavilla/message/post.py
+-rw-r--r--   0        0        0     6519 2023-07-07 08:04:43.463528 herta_villa_sdk-0.6.1/hertavilla/message/text.py
+-rw-r--r--   0        0        0      469 2023-07-07 08:04:43.463528 herta_villa_sdk-0.6.1/hertavilla/message/types.py
+-rw-r--r--   0        0        0     6566 2023-07-11 03:47:58.720329 herta_villa_sdk-0.6.1/hertavilla/model.py
+-rw-r--r--   0        0        0      967 2023-07-19 02:26:51.304211 herta_villa_sdk-0.6.1/hertavilla/server/__init__.py
+-rw-r--r--   0        0        0      817 2023-07-19 02:26:51.304211 herta_villa_sdk-0.6.1/hertavilla/server/_lifespan.py
+-rw-r--r--   0        0        0     2047 2023-07-19 02:26:51.304211 herta_villa_sdk-0.6.1/hertavilla/server/aiohttp.py
+-rw-r--r--   0        0        0     2427 2023-07-19 02:26:51.304211 herta_villa_sdk-0.6.1/hertavilla/server/fastapi.py
+-rw-r--r--   0        0        0     3448 2023-07-19 02:26:51.304211 herta_villa_sdk-0.6.1/hertavilla/server/internal.py
+-rw-r--r--   0        0        0      583 2023-07-07 08:04:43.463528 herta_villa_sdk-0.6.1/hertavilla/typing.py
+-rw-r--r--   0        0        0      587 2023-07-07 08:04:43.463528 herta_villa_sdk-0.6.1/hertavilla/utils.py
+-rw-r--r--   0        0        0       61 2023-07-19 02:29:50.966622 herta_villa_sdk-0.6.1/hertavilla/version.py
+-rw-r--r--   0        0        0     2292 2023-07-19 02:30:29.013481 herta_villa_sdk-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0       39 2023-06-23 15:08:40.334591 herta_villa_sdk-0.6.1/tests/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2023-06-23 15:08:40.334591 herta_villa_sdk-0.6.1/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      310 2023-06-23 15:08:40.334591 herta_villa_sdk-0.6.1/tests/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2023-06-23 15:10:48.533369 herta_villa_sdk-0.6.1/tests/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0       77 2023-06-25 10:19:28.031034 herta_villa_sdk-0.6.1/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2023-06-25 10:19:28.031034 herta_villa_sdk-0.6.1/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      554 2023-07-07 08:04:43.463528 herta_villa_sdk-0.6.1/tests/test_utils.py
+-rw-r--r--   0        0        0     5279 1970-01-01 00:00:00.000000 herta_villa_sdk-0.6.1/PKG-INFO
```

### Comparing `herta_villa_sdk-0.6.0/LICENSE` & `herta_villa_sdk-0.6.1/LICENSE`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Herta-villa
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
+Copyright (c) 2023 Herta-villa
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

### Comparing `herta_villa_sdk-0.6.0/README.md` & `herta_villa_sdk-0.6.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,125 +1,127 @@
-# Herta-villa-SDK
-
-[![license](https://img.shields.io/github/license/Herta-villa/Herta-villa-SDK)](https://github.com/Herta-villa/Herta-villa-SDK/blob/master/LICENSE)
-[![pypi](https://img.shields.io/pypi/v/herta-villa-sdk)](https://pypi.python.org/pypi/herta-villa-sdk)
-![python version](https://img.shields.io/badge/Python-3.8+-green)
-[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
-
-大别野「黑塔」Python SDK
-
-## 特性
-
-- 多种服务器后端（内置 `aiohttp` 和 `fastapi` 后端），完整异步支持
-- 完整类型注解支持
-- ...
-
-## 安装
-
-```shell
-pip install herta-villa-sdk
-```
-
-FastAPI 后端支持:
-
-```shell
-pip install herta-villa-sdk[fastapi]
-```
-
-## 快速开始
-
-你需要拥有一个[大别野](https://dby.miyoushe.com/chat)机器人。可前往大别野[「机器人开发者社区」](https://dby.miyoushe.com/chat/463/20020)（`OpenVilla`）申请。
-
-```python
-from hertavilla import MessageChain, SendMessageEvent, VillaBot, run
-
-
-PUB_KEY = """-----BEGIN PUBLIC KEY-----
-aaa
-bbb
-ccc
------END PUBLIC KEY-----
-"""  # 开放平台 pub_key
-# 需要注意 `-----BEGIN PUBLIC KEY-----` 前没有换行符
-#  `-----END PUBLIC KEY-----` 后有一个换行符
-# 目前从网页端复制下来的时候会为一串 pub_key，需要将空格转为换行
-
-bot = VillaBot(
-    "bot_id",  # 这里填写 bot_id
-    "bot_secret",  # 这里填写 secret
-    "/",  # bot 回调 endpoint
-    PUB_KEY,  # 开放平台提供的 pub_key
-)
-
-
-@bot.startswith("/")  # 注册一个消息匹配器，匹配前缀为 / 的消息
-async def _(event: SendMessageEvent, bot: VillaBot):
-    message = event.message
-    if str(message[1]) == "/hello":
-        chain = MessageChain()
-        chain.append("world")
-        await bot.send(event.villa_id, event.room_id, chain)
-
-
-run(bot)  # 运行 bot
-```
-
-可以向你的 bot 发送 `@Bot /hello`，bot 会回复 `world`。
-
-## 示例
-
-详见 [examples](./examples/) 文件夹
-
-## 支持的 API
-
-- [x] 鉴权
-  - [x] 校验用户机器人访问凭证 `/checkMemberBotAccessToken`
-- [x] 大别野
-  - [x] 获取大别野信息 `/getVilla`
-- [x] 用户
-  - [x] 获取用户信息 `/getMember`
-  - [x] 获取大别野成员列表 `/getVillaMembers`
-  - [x] 踢出大别野用户 `/deleteVillaMember`
-- [x] 消息
-  - [x] 置顶消息 `/pinMessage`
-  - [x] 撤回消息 `/recallMessage`
-  - [x] 发送消息 `/sendMessage`
-- [x] 房间
-  - [x] 创建分组 `/createGroup`
-  - [x] 编辑分组 `/editGroup`
-  - [x] 删除分组 `/deleteGroup`
-  - [x] 获取分组列表 `/getGroupList`
-  - [x] 编辑房间 `/editRoom`
-  - [x] 删除房间 `/deleteRoom`
-  - [x] 获取房间信息 `/getRoom`
-  - [x] 获取房间列表信息 `/getVillaGroupRoomList`
-- [x] 身份组
-  - [x] 向身份组操作用户 `/operateMemberToRole`
-  - [x] 创建身份组 `/createMemberRole`
-  - [x] 编辑身份组 `/editMemberRole`
-  - [x] 删除身份组 `/deleteMemberRole`
-  - [x] 获取身份组 `/getMemberRoleInfo`
-  - [x] 获取大别野下所有身份组 `/getVillaMemberRoles`
-- [x] 表态表情
-  - [x] 获取全量表情 `/getAllEmoticons`
-- [ ] 审核 `/audit`
-
-## 支持的事件
-
-- [x] [JoinVilla](https://webstatic.mihoyo.com/vila/bot/doc/callback.html###JoinVilla) 有新用户加入大别野
-- [x] [SendMessage](https://webstatic.mihoyo.com/vila/bot/doc/callback.html###SendMessage) 用户@机器人发送消息
-- [x] [CreateRobot](https://webstatic.mihoyo.com/vila/bot/doc/callback.html###CreateRobot) 大别野添加机器人实例
-- [x] [DeleteRobot](https://webstatic.mihoyo.com/vila/bot/doc/callback.html###DeleteRobot) 大别野删除机器人实例
-- [x] [AddQuickEmoticon](https://webstatic.mihoyo.com/vila/bot/doc/callback.html#AddQuickEmoticon) 用户使用表情回复消息表态
-- [ ] [AuditCallback](https://webstatic.mihoyo.com/vila/bot/doc/callback.html#AuditCallback) 审核结果回调
-
-## Bug 反馈及建议
-
-大别野 Bot 和 Herta SDK 均处于开发状态中，如遇到问题或有相关建议可通过 [Issue](https://github.com/Herta-villa/Herta-villa-SDK/issues/new) 提出，感谢支持！
-
-## 相关项目
-
-- [CMHopeSunshine/villa-py](https://github.com/CMHopeSunshine/villa-py) 米游社大别野 Bot Python SDK（非官方）
-
-## 交流
-
-- 前往大别野[「斩尽芜杂」](https://dby.miyoushe.com/chat/1785/25317)（`aaUeZqd`）
+# Herta-villa-SDK
+
+[![license](https://img.shields.io/github/license/Herta-villa/Herta-villa-SDK)](https://github.com/Herta-villa/Herta-villa-SDK/blob/master/LICENSE)
+[![pypi](https://img.shields.io/pypi/v/herta-villa-sdk)](https://pypi.python.org/pypi/herta-villa-sdk)
+![python version](https://img.shields.io/badge/Python-3.8+-green)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+
+大别野「黑塔」Python SDK
+
+## 特性
+
+- 多种服务器后端（内置 `aiohttp` 和 `fastapi` 后端），完整异步支持
+- 完整类型注解支持
+- ...
+
+## 安装
+
+```shell
+pip install herta-villa-sdk
+```
+
+FastAPI 后端支持:
+
+```shell
+pip install herta-villa-sdk[fastapi]
+```
+
+## 快速开始
+
+你需要拥有一个[大别野](https://dby.miyoushe.com/chat)机器人。可前往大别野[「机器人开发者社区」](https://dby.miyoushe.com/chat/463/20020)（`OpenVilla`）申请。
+
+```python
+from hertavilla import MessageChain, SendMessageEvent, VillaBot, run
+from hertavilla.server import init_backend
+
+
+PUB_KEY = """-----BEGIN PUBLIC KEY-----
+aaa
+bbb
+ccc
+-----END PUBLIC KEY-----
+"""  # 开放平台 pub_key
+# 需要注意 `-----BEGIN PUBLIC KEY-----` 前没有换行符
+#  `-----END PUBLIC KEY-----` 后有一个换行符
+# 目前从网页端复制下来的时候会为一串 pub_key，需要将空格转为换行
+
+bot = VillaBot(
+    "bot_id",  # 这里填写 bot_id
+    "bot_secret",  # 这里填写 secret
+    "/",  # bot 回调 endpoint
+    PUB_KEY,  # 开放平台提供的 pub_key
+)
+
+
+@bot.startswith("/")  # 注册一个消息匹配器，匹配前缀为 / 的消息
+async def _(event: SendMessageEvent, bot: VillaBot):
+    message = event.message
+    if str(message[1]) == "/hello":
+        chain = MessageChain()
+        chain.append("world")
+        await bot.send(event.villa_id, event.room_id, chain)
+
+
+init_backend()  # 初始化后端
+run(bot)  # 运行 bot
+```
+
+可以向你的 bot 发送 `@Bot /hello`，bot 会回复 `world`。
+
+## 示例
+
+详见 [examples](./examples/) 文件夹
+
+## 支持的 API
+
+- [x] 鉴权
+  - [x] 校验用户机器人访问凭证 `/checkMemberBotAccessToken`
+- [x] 大别野
+  - [x] 获取大别野信息 `/getVilla`
+- [x] 用户
+  - [x] 获取用户信息 `/getMember`
+  - [x] 获取大别野成员列表 `/getVillaMembers`
+  - [x] 踢出大别野用户 `/deleteVillaMember`
+- [x] 消息
+  - [x] 置顶消息 `/pinMessage`
+  - [x] 撤回消息 `/recallMessage`
+  - [x] 发送消息 `/sendMessage`
+- [x] 房间
+  - [x] 创建分组 `/createGroup`
+  - [x] 编辑分组 `/editGroup`
+  - [x] 删除分组 `/deleteGroup`
+  - [x] 获取分组列表 `/getGroupList`
+  - [x] 编辑房间 `/editRoom`
+  - [x] 删除房间 `/deleteRoom`
+  - [x] 获取房间信息 `/getRoom`
+  - [x] 获取房间列表信息 `/getVillaGroupRoomList`
+- [x] 身份组
+  - [x] 向身份组操作用户 `/operateMemberToRole`
+  - [x] 创建身份组 `/createMemberRole`
+  - [x] 编辑身份组 `/editMemberRole`
+  - [x] 删除身份组 `/deleteMemberRole`
+  - [x] 获取身份组 `/getMemberRoleInfo`
+  - [x] 获取大别野下所有身份组 `/getVillaMemberRoles`
+- [x] 表态表情
+  - [x] 获取全量表情 `/getAllEmoticons`
+- [ ] 审核 `/audit`
+
+## 支持的事件
+
+- [x] [JoinVilla](https://webstatic.mihoyo.com/vila/bot/doc/callback.html###JoinVilla) 有新用户加入大别野
+- [x] [SendMessage](https://webstatic.mihoyo.com/vila/bot/doc/callback.html###SendMessage) 用户@机器人发送消息
+- [x] [CreateRobot](https://webstatic.mihoyo.com/vila/bot/doc/callback.html###CreateRobot) 大别野添加机器人实例
+- [x] [DeleteRobot](https://webstatic.mihoyo.com/vila/bot/doc/callback.html###DeleteRobot) 大别野删除机器人实例
+- [x] [AddQuickEmoticon](https://webstatic.mihoyo.com/vila/bot/doc/callback.html#AddQuickEmoticon) 用户使用表情回复消息表态
+- [ ] [AuditCallback](https://webstatic.mihoyo.com/vila/bot/doc/callback.html#AuditCallback) 审核结果回调
+
+## Bug 反馈及建议
+
+大别野 Bot 和 Herta SDK 均处于开发状态中，如遇到问题或有相关建议可通过 [Issue](https://github.com/Herta-villa/Herta-villa-SDK/issues/new) 提出，感谢支持！
+
+## 相关项目
+
+- [CMHopeSunshine/villa-py](https://github.com/CMHopeSunshine/villa-py) 米游社大别野 Bot Python SDK（非官方）
+
+## 交流
+
+- 前往大别野[「斩尽芜杂」](https://dby.miyoushe.com/chat/1785/25317)（`aaUeZqd`）
```

### Comparing `herta_villa_sdk-0.6.0/hertavilla/apis/emoticon.py` & `herta_villa_sdk-0.6.1/hertavilla/apis/emoticon.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from __future__ import annotations
-
-from typing import List
-
-from hertavilla.apis.base import _BaseAPIMixin
-from hertavilla.model import Emoticon
-
-from pydantic import parse_obj_as
-
-
-class EmoticonAPIMixin(_BaseAPIMixin):
-    async def get_all_emoticon(self) -> list[Emoticon]:
-        """获取全量表情
-
-        Returns:
-            list[Emoticon]: 表情列表
-        """
-        return parse_obj_as(
-            List[Emoticon],
-            (await self.base_request("/getAllEmoticons", "GET"))["list"],
-        )
+from __future__ import annotations
+
+from typing import List
+
+from hertavilla.apis.base import _BaseAPIMixin
+from hertavilla.model import Emoticon
+
+from pydantic import parse_obj_as
+
+
+class EmoticonAPIMixin(_BaseAPIMixin):
+    async def get_all_emoticon(self) -> list[Emoticon]:
+        """获取全量表情
+
+        Returns:
+            list[Emoticon]: 表情列表
+        """
+        return parse_obj_as(
+            List[Emoticon],
+            (await self.base_request("/getAllEmoticons", "GET"))["list"],
+        )
```

### Comparing `herta_villa_sdk-0.6.0/hertavilla/apis/member.py` & `herta_villa_sdk-0.6.1/hertavilla/apis/member.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-from __future__ import annotations
-
-from typing import List
-
-from hertavilla.apis.base import _BaseAPIMixin
-from hertavilla.model import Member
-
-from pydantic import parse_obj_as
-
-
-class MemberAPIMixin(_BaseAPIMixin):
-    async def get_member(self, villa_id: int, uid: int) -> Member:
-        """获取用户信息
-
-        Args:
-            villa_id (int): 大别野 id
-            uid (int): 用户 id
-
-        Returns:
-            Member: 用户详情
-        """
-        return Member.parse_obj(
-            (
-                await self.base_request(
-                    "/getMember",
-                    "GET",
-                    villa_id,
-                    params={"uid": uid},
-                )
-            )["member"],
-        )
-
-    async def get_villa_members(
-        self,
-        villa_id: int,
-        offset_str: str = "0",
-        size: int = 10,
-    ) -> tuple[list[Member], str]:
-        """获取大别野成员列表。
-        当 offset_str 为空时，返回第一页的成员列表信息；
-        当使用本次请求返回值中的`下一页的偏移量起始位置`作为下次请求中的 offset_str 时，会返回下一页的成员列表。
-
-        Args:
-            villa_id (int): 大别野 id
-            offset_str (str, optional): 起始位置偏移量. Defaults to "0".
-            size (int, optional): 分页大小. Defaults to 10.
-
-        Returns:
-            tuple[list[Member], str]: 用户信息列表与下一页的偏移量起始位置
-        """  # noqa: E501
-        data = await self.base_request(
-            "/getVillaMembers",
-            "GET",
-            villa_id,
-            params={"offset_str": offset_str, "size": size},
-        )
-        return (
-            parse_obj_as(List[Member], data["list"]),
-            data["next_offset_str"],
-        )
-
-    async def delete_villa_member(self, villa_id: int, uid: int) -> None:
-        """踢出大别野用户
-
-        Args:
-            villa_id (int): 大别野 id
-            uid (int): 用户 id
-        """
-        await self.base_request(
-            "/deleteVillaMember",
-            "POST",
-            villa_id,
-            data={"uid": uid},
-        )
+from __future__ import annotations
+
+from typing import List
+
+from hertavilla.apis.base import _BaseAPIMixin
+from hertavilla.model import Member
+
+from pydantic import parse_obj_as
+
+
+class MemberAPIMixin(_BaseAPIMixin):
+    async def get_member(self, villa_id: int, uid: int) -> Member:
+        """获取用户信息
+
+        Args:
+            villa_id (int): 大别野 id
+            uid (int): 用户 id
+
+        Returns:
+            Member: 用户详情
+        """
+        return Member.parse_obj(
+            (
+                await self.base_request(
+                    "/getMember",
+                    "GET",
+                    villa_id,
+                    params={"uid": uid},
+                )
+            )["member"],
+        )
+
+    async def get_villa_members(
+        self,
+        villa_id: int,
+        offset_str: str = "0",
+        size: int = 10,
+    ) -> tuple[list[Member], str]:
+        """获取大别野成员列表。
+        当 offset_str 为空时，返回第一页的成员列表信息；
+        当使用本次请求返回值中的`下一页的偏移量起始位置`作为下次请求中的 offset_str 时，会返回下一页的成员列表。
+
+        Args:
+            villa_id (int): 大别野 id
+            offset_str (str, optional): 起始位置偏移量. Defaults to "0".
+            size (int, optional): 分页大小. Defaults to 10.
+
+        Returns:
+            tuple[list[Member], str]: 用户信息列表与下一页的偏移量起始位置
+        """  # noqa: E501
+        data = await self.base_request(
+            "/getVillaMembers",
+            "GET",
+            villa_id,
+            params={"offset_str": offset_str, "size": size},
+        )
+        return (
+            parse_obj_as(List[Member], data["list"]),
+            data["next_offset_str"],
+        )
+
+    async def delete_villa_member(self, villa_id: int, uid: int) -> None:
+        """踢出大别野用户
+
+        Args:
+            villa_id (int): 大别野 id
+            uid (int): 用户 id
+        """
+        await self.base_request(
+            "/deleteVillaMember",
+            "POST",
+            villa_id,
+            data={"uid": uid},
+        )
```

### Comparing `herta_villa_sdk-0.6.0/hertavilla/apis/villa.py` & `herta_villa_sdk-0.6.1/hertavilla/apis/villa.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from __future__ import annotations
-
-from hertavilla.apis.base import _BaseAPIMixin
-from hertavilla.model import Villa
-
-
-class VillaAPIMixin(_BaseAPIMixin):
-    async def get_villa(self, villa_id: int) -> Villa:
-        """获取大别野信息
-
-        Args:
-            villa_id (int): 大别野 id
-
-        Returns:
-            Villa: 大别野信息
-        """
-        return Villa.parse_obj(
-            (
-                await self.base_request(
-                    "/getVilla",
-                    "GET",
-                    villa_id,
-                    params={"villa_id": villa_id},
-                )
-            )["villa"],
-        )
+from __future__ import annotations
+
+from hertavilla.apis.base import _BaseAPIMixin
+from hertavilla.model import Villa
+
+
+class VillaAPIMixin(_BaseAPIMixin):
+    async def get_villa(self, villa_id: int) -> Villa:
+        """获取大别野信息
+
+        Args:
+            villa_id (int): 大别野 id
+
+        Returns:
+            Villa: 大别野信息
+        """
+        return Villa.parse_obj(
+            (
+                await self.base_request(
+                    "/getVilla",
+                    "GET",
+                    villa_id,
+                    params={"villa_id": villa_id},
+                )
+            )["villa"],
+        )
```

### Comparing `herta_villa_sdk-0.6.0/hertavilla/bot.py` & `herta_villa_sdk-0.6.1/hertavilla/bot.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,287 +1,287 @@
-from __future__ import annotations
-
-import asyncio
-import base64
-from dataclasses import dataclass
-import logging
-import re
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Callable,
-    Coroutine,
-    Generic,
-    NamedTuple,
-    TypeVar,
-)
-import urllib.parse
-
-from hertavilla.apis.auth import AuthAPIMixin
-from hertavilla.apis.img import ImgAPIMixin
-from hertavilla.apis.member import MemberAPIMixin
-from hertavilla.apis.message import MessageAPIMixin
-from hertavilla.apis.role import RoleAPIMixin
-from hertavilla.apis.room import RoomAPIMixin
-from hertavilla.apis.villa import VillaAPIMixin
-from hertavilla.match import Endswith, Keywords, Match, Regex, Startswith
-
-import rsa
-
-if TYPE_CHECKING:
-    from hertavilla.event import Command, Event, SendMessageEvent, Template
-    from hertavilla.message import MessageChain
-
-
-TE = TypeVar("TE", bound="Event")
-
-MessageHandlerFunc = Callable[
-    ["SendMessageEvent", "VillaBot"],
-    Coroutine[Any, Any, None],
-]
-
-logger = logging.getLogger("hertavilla.bot")
-
-
-@dataclass
-class Handler(Generic[TE]):
-    event: type[TE]
-    func: Callable[[TE, VillaBot], Coroutine[Any, Any, None]]
-
-    def __call__(self, *args: Any, **kwargs: Any) -> Any:
-        return self.func(*args, **kwargs)
-
-    def __eq__(self, __value: Event) -> bool:
-        return isinstance(__value, self.event)
-
-
-class MessageHandler(NamedTuple):
-    match: Match
-    func: Callable[["SendMessageEvent", VillaBot], Coroutine[Any, Any, None]]
-
-    def __call__(self, *args: Any, **kwargs: Any) -> Any:
-        return self.func(*args, **kwargs)
-
-    def check(self, chain: MessageChain) -> bool:
-        return self.match.check(chain)
-
-
-class VillaBot(
-    AuthAPIMixin,
-    MemberAPIMixin,
-    MessageAPIMixin,
-    RoomAPIMixin,
-    VillaAPIMixin,
-    RoleAPIMixin,
-    ImgAPIMixin,
-):
-    def __init__(
-        self,
-        bot_id: str,
-        secret: str,
-        callback_endpoint: str,
-        pub_key: str,
-        bot_info: "Template" | None = None,
-    ) -> None:
-        from hertavilla.event import SendMessageEvent
-
-        super().__init__(bot_id, secret, pub_key)
-        self.rsa_pub_key = rsa.PublicKey.load_pkcs1_openssl_pem(
-            pub_key.encode(),
-        )
-        self._bot_info = bot_info
-        self.callback_endpoint = callback_endpoint
-        self.handlers: list[Handler] = []
-        self.message_handlers: list[MessageHandler] = []
-        self.register_handler(SendMessageEvent, self.message_handler)
-
-    @property
-    def bot_info(self) -> "Template":
-        assert (
-            self._bot_info is not None
-        ), f"No bot info, maybe bot {self.bot_id} not connected"
-        return self._bot_info
-
-    @bot_info.setter
-    def bot_info(self, value: "Template") -> None:
-        self._bot_info = value
-
-    @property
-    def name(self) -> str:
-        """Bot 昵称"""
-        return self.bot_info.name
-
-    @property
-    def avatar(self) -> str:
-        """Bot 头像地址"""
-        return self.bot_info.icon
-
-    @property
-    def commands(self) -> list["Command"]:
-        """Bot 预设命令列表"""
-        return self.bot_info.commands
-
-    @property
-    def description(self) -> str:
-        """Bot 介绍"""
-        return self.bot_info.desc
-
-    def __repr__(self) -> str:
-        return f"<VillaBot id={self.bot_id!r}>"
-
-    def __eq__(self, __value: str | VillaBot) -> bool:
-        if isinstance(__value, VillaBot):
-            return (
-                self.bot_id == __value.bot_id and self.secret == __value.secret
-            )
-        return self.bot_id == __value
-
-    def __hash__(self) -> int:
-        return hash(self.bot_id)
-
-    def verify(
-        self,
-        sign: str,
-        body: str,
-    ) -> bool:
-        sign_ = base64.b64decode(sign)
-        sign_msg = urllib.parse.urlencode(
-            {"body": body, "secret": self.secret},
-        ).encode()
-        try:
-            rsa.verify(sign_msg, sign_, self.rsa_pub_key)
-        except rsa.VerificationError:
-            return False
-        else:
-            return True
-
-    async def send(
-        self,
-        villa_id: int,
-        room_id: int,
-        chain: "MessageChain",
-    ) -> str:
-        """通用发送消息方法
-
-        Args:
-            villa_id (int): 大别野 id
-            room_id (int): 房间 id
-            chain (MessageChain): 消息链
-
-        Returns:
-            str: bot_msg_id 机器人所发送消息的唯一标识符
-        """
-        return await self.send_message(
-            villa_id,
-            room_id,
-            *(await chain.to_content_json(self)),
-        )
-
-    # event handle
-
-    def register_handler(
-        self,
-        event: type[TE],
-        func: Callable[[TE, VillaBot], Coroutine[Any, Any, None]],
-    ):
-        self.handlers.append(Handler[TE](event, func))
-        logger.info(f"Registered the handler {func} for {event.__name__}")
-        return func
-
-    def listen(
-        self,
-        event: type[TE],
-    ) -> Callable[
-        [Callable[[TE, VillaBot], Coroutine[Any, Any, None]]],
-        Callable[[TE, VillaBot], Coroutine[Any, Any, None]],
-    ]:
-        def wrapper(
-            func: Callable[[TE, VillaBot], Coroutine[Any, Any, None]],
-        ) -> Callable[[TE, VillaBot], Coroutine[Any, Any, None]]:
-            self.register_handler(event, func)
-            return func
-
-        return wrapper
-
-    async def handle_event(self, event: Event) -> None:
-        handlers = filter(lambda x: x == event, self.handlers)
-        logger.info(f"Handling event {event.__class__.__name__}")
-        try:
-            await asyncio.gather(
-                *[handler(event, self) for handler in handlers],
-            )
-        except Exception:
-            logger.exception("Raised exceptions while handling event.")
-
-    # message handle
-    @staticmethod
-    async def message_handler(event: "SendMessageEvent", bot: "VillaBot"):
-        handlers = filter(
-            lambda x: x.check(event.message),
-            bot.message_handlers,
-        )
-        await asyncio.gather(*[handler(event, bot) for handler in handlers])
-
-    def register_msg_handler(self, match: Match, func: MessageHandlerFunc):
-        self.message_handlers.append(MessageHandler(match, func))
-        logger.info(f"Registered the handler {func} with {match}")
-        return func
-
-    def match(
-        self,
-        match: Match,
-    ) -> Callable[[MessageHandlerFunc], MessageHandlerFunc]:
-        def wrapper(
-            func: MessageHandlerFunc,
-        ) -> MessageHandlerFunc:
-            self.register_msg_handler(match, func)
-            return func
-
-        return wrapper
-
-    def regex(
-        self,
-        pattern: str | re.Pattern,
-    ) -> Callable[[MessageHandlerFunc], MessageHandlerFunc]:
-        def wrapper(
-            func: MessageHandlerFunc,
-        ) -> MessageHandlerFunc:
-            self.register_msg_handler(Regex(pattern), func)
-            return func
-
-        return wrapper
-
-    def startswith(
-        self,
-        prefix: str,
-    ) -> Callable[[MessageHandlerFunc], MessageHandlerFunc]:
-        def wrapper(
-            func: MessageHandlerFunc,
-        ) -> MessageHandlerFunc:
-            self.register_msg_handler(Startswith(prefix), func)
-            return func
-
-        return wrapper
-
-    def endswith(
-        self,
-        suffix: str,
-    ) -> Callable[[MessageHandlerFunc], MessageHandlerFunc]:
-        def wrapper(
-            func: MessageHandlerFunc,
-        ) -> MessageHandlerFunc:
-            self.register_msg_handler(Endswith(suffix), func)
-            return func
-
-        return wrapper
-
-    def keyword(
-        self,
-        *keywords: str,
-    ) -> Callable[[MessageHandlerFunc], MessageHandlerFunc]:
-        def wrapper(
-            func: MessageHandlerFunc,
-        ) -> MessageHandlerFunc:
-            self.register_msg_handler(Keywords(*keywords), func)
-            return func
-
-        return wrapper
+from __future__ import annotations
+
+import asyncio
+import base64
+from dataclasses import dataclass
+import logging
+import re
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Coroutine,
+    Generic,
+    NamedTuple,
+    TypeVar,
+)
+import urllib.parse
+
+from hertavilla.apis.auth import AuthAPIMixin
+from hertavilla.apis.img import ImgAPIMixin
+from hertavilla.apis.member import MemberAPIMixin
+from hertavilla.apis.message import MessageAPIMixin
+from hertavilla.apis.role import RoleAPIMixin
+from hertavilla.apis.room import RoomAPIMixin
+from hertavilla.apis.villa import VillaAPIMixin
+from hertavilla.match import Endswith, Keywords, Match, Regex, Startswith
+
+import rsa
+
+if TYPE_CHECKING:
+    from hertavilla.event import Command, Event, SendMessageEvent, Template
+    from hertavilla.message import MessageChain
+
+
+TE = TypeVar("TE", bound="Event")
+
+MessageHandlerFunc = Callable[
+    ["SendMessageEvent", "VillaBot"],
+    Coroutine[Any, Any, None],
+]
+
+logger = logging.getLogger("hertavilla.bot")
+
+
+@dataclass
+class Handler(Generic[TE]):
+    event: type[TE]
+    func: Callable[[TE, VillaBot], Coroutine[Any, Any, None]]
+
+    def __call__(self, *args: Any, **kwargs: Any) -> Any:
+        return self.func(*args, **kwargs)
+
+    def __eq__(self, __value: Event) -> bool:
+        return isinstance(__value, self.event)
+
+
+class MessageHandler(NamedTuple):
+    match: Match
+    func: Callable[["SendMessageEvent", VillaBot], Coroutine[Any, Any, None]]
+
+    def __call__(self, *args: Any, **kwargs: Any) -> Any:
+        return self.func(*args, **kwargs)
+
+    def check(self, chain: MessageChain) -> bool:
+        return self.match.check(chain)
+
+
+class VillaBot(
+    AuthAPIMixin,
+    MemberAPIMixin,
+    MessageAPIMixin,
+    RoomAPIMixin,
+    VillaAPIMixin,
+    RoleAPIMixin,
+    ImgAPIMixin,
+):
+    def __init__(
+        self,
+        bot_id: str,
+        secret: str,
+        callback_endpoint: str,
+        pub_key: str,
+        bot_info: "Template" | None = None,
+    ) -> None:
+        from hertavilla.event import SendMessageEvent
+
+        super().__init__(bot_id, secret, pub_key)
+        self.rsa_pub_key = rsa.PublicKey.load_pkcs1_openssl_pem(
+            pub_key.encode(),
+        )
+        self._bot_info = bot_info
+        self.callback_endpoint = callback_endpoint
+        self.handlers: list[Handler] = []
+        self.message_handlers: list[MessageHandler] = []
+        self.register_handler(SendMessageEvent, self.message_handler)
+
+    @property
+    def bot_info(self) -> "Template":
+        assert (
+            self._bot_info is not None
+        ), f"No bot info, maybe bot {self.bot_id} not connected"
+        return self._bot_info
+
+    @bot_info.setter
+    def bot_info(self, value: "Template") -> None:
+        self._bot_info = value
+
+    @property
+    def name(self) -> str:
+        """Bot 昵称"""
+        return self.bot_info.name
+
+    @property
+    def avatar(self) -> str:
+        """Bot 头像地址"""
+        return self.bot_info.icon
+
+    @property
+    def commands(self) -> list["Command"]:
+        """Bot 预设命令列表"""
+        return self.bot_info.commands
+
+    @property
+    def description(self) -> str:
+        """Bot 介绍"""
+        return self.bot_info.desc
+
+    def __repr__(self) -> str:
+        return f"<VillaBot id={self.bot_id!r}>"
+
+    def __eq__(self, __value: str | VillaBot) -> bool:
+        if isinstance(__value, VillaBot):
+            return (
+                self.bot_id == __value.bot_id and self.secret == __value.secret
+            )
+        return self.bot_id == __value
+
+    def __hash__(self) -> int:
+        return hash(self.bot_id)
+
+    def verify(
+        self,
+        sign: str,
+        body: str,
+    ) -> bool:
+        sign_ = base64.b64decode(sign)
+        sign_msg = urllib.parse.urlencode(
+            {"body": body, "secret": self.secret},
+        ).encode()
+        try:
+            rsa.verify(sign_msg, sign_, self.rsa_pub_key)
+        except rsa.VerificationError:
+            return False
+        else:
+            return True
+
+    async def send(
+        self,
+        villa_id: int,
+        room_id: int,
+        chain: "MessageChain",
+    ) -> str:
+        """通用发送消息方法
+
+        Args:
+            villa_id (int): 大别野 id
+            room_id (int): 房间 id
+            chain (MessageChain): 消息链
+
+        Returns:
+            str: bot_msg_id 机器人所发送消息的唯一标识符
+        """
+        return await self.send_message(
+            villa_id,
+            room_id,
+            *(await chain.to_content_json(self)),
+        )
+
+    # event handle
+
+    def register_handler(
+        self,
+        event: type[TE],
+        func: Callable[[TE, VillaBot], Coroutine[Any, Any, None]],
+    ):
+        self.handlers.append(Handler[TE](event, func))
+        logger.info(f"Registered the handler {func} for {event.__name__}")
+        return func
+
+    def listen(
+        self,
+        event: type[TE],
+    ) -> Callable[
+        [Callable[[TE, VillaBot], Coroutine[Any, Any, None]]],
+        Callable[[TE, VillaBot], Coroutine[Any, Any, None]],
+    ]:
+        def wrapper(
+            func: Callable[[TE, VillaBot], Coroutine[Any, Any, None]],
+        ) -> Callable[[TE, VillaBot], Coroutine[Any, Any, None]]:
+            self.register_handler(event, func)
+            return func
+
+        return wrapper
+
+    async def handle_event(self, event: Event) -> None:
+        handlers = filter(lambda x: x == event, self.handlers)
+        logger.info(f"Handling event {event.__class__.__name__}")
+        try:
+            await asyncio.gather(
+                *[handler(event, self) for handler in handlers],
+            )
+        except Exception:
+            logger.exception("Raised exceptions while handling event.")
+
+    # message handle
+    @staticmethod
+    async def message_handler(event: "SendMessageEvent", bot: "VillaBot"):
+        handlers = filter(
+            lambda x: x.check(event.message),
+            bot.message_handlers,
+        )
+        await asyncio.gather(*[handler(event, bot) for handler in handlers])
+
+    def register_msg_handler(self, match: Match, func: MessageHandlerFunc):
+        self.message_handlers.append(MessageHandler(match, func))
+        logger.info(f"Registered the handler {func} with {match}")
+        return func
+
+    def match(
+        self,
+        match: Match,
+    ) -> Callable[[MessageHandlerFunc], MessageHandlerFunc]:
+        def wrapper(
+            func: MessageHandlerFunc,
+        ) -> MessageHandlerFunc:
+            self.register_msg_handler(match, func)
+            return func
+
+        return wrapper
+
+    def regex(
+        self,
+        pattern: str | re.Pattern,
+    ) -> Callable[[MessageHandlerFunc], MessageHandlerFunc]:
+        def wrapper(
+            func: MessageHandlerFunc,
+        ) -> MessageHandlerFunc:
+            self.register_msg_handler(Regex(pattern), func)
+            return func
+
+        return wrapper
+
+    def startswith(
+        self,
+        prefix: str,
+    ) -> Callable[[MessageHandlerFunc], MessageHandlerFunc]:
+        def wrapper(
+            func: MessageHandlerFunc,
+        ) -> MessageHandlerFunc:
+            self.register_msg_handler(Startswith(prefix), func)
+            return func
+
+        return wrapper
+
+    def endswith(
+        self,
+        suffix: str,
+    ) -> Callable[[MessageHandlerFunc], MessageHandlerFunc]:
+        def wrapper(
+            func: MessageHandlerFunc,
+        ) -> MessageHandlerFunc:
+            self.register_msg_handler(Endswith(suffix), func)
+            return func
+
+        return wrapper
+
+    def keyword(
+        self,
+        *keywords: str,
+    ) -> Callable[[MessageHandlerFunc], MessageHandlerFunc]:
+        def wrapper(
+            func: MessageHandlerFunc,
+        ) -> MessageHandlerFunc:
+            self.register_msg_handler(Keywords(*keywords), func)
+            return func
+
+        return wrapper
```

### Comparing `herta_villa_sdk-0.6.0/hertavilla/exception.py` & `herta_villa_sdk-0.6.1/hertavilla/exception.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-from __future__ import annotations
-
-from typing import Any
-
-
-class PubkeyNoneWarning(Warning):
-    ...
-
-
-class SDKException(Exception):
-    ...
-
-
-class HTTPStatusError(SDKException):
-    def __init__(
-        self,
-        /,
-        status: int,
-    ) -> None:
-        self.status = status
-
-    def __repr__(self) -> str:
-        return "<HTTPStatusError status={self.status}"
-
-
-class _ExceptionWithRetcode(SDKException):
-    def __init__(self, /, retcode: int, message: str) -> None:
-        self.retcode = retcode
-        self.message = message
-
-    def to_dict(self):
-        return {"retcode": self.retcode, "message": self.message}
-
-
-class CallingApiException(_ExceptionWithRetcode):
-    def __repr__(self) -> str:
-        return (
-            "<CallingApiException "
-            f"retcode={self.retcode}, message={self.message!r}>"
-        )
-
-    def __str__(self) -> str:
-        return repr(self)
-
-
-def raise_exception(payload: dict[str, Any]):
-    if payload["retcode"] != 0:
-        raise CallingApiException(payload["retcode"], payload["message"])
+from __future__ import annotations
+
+from typing import Any
+
+
+class PubkeyNoneWarning(Warning):
+    ...
+
+
+class SDKException(Exception):
+    ...
+
+
+class HTTPStatusError(SDKException):
+    def __init__(
+        self,
+        /,
+        status: int,
+    ) -> None:
+        self.status = status
+
+    def __repr__(self) -> str:
+        return "<HTTPStatusError status={self.status}"
+
+
+class _ExceptionWithRetcode(SDKException):
+    def __init__(self, /, retcode: int, message: str) -> None:
+        self.retcode = retcode
+        self.message = message
+
+    def to_dict(self):
+        return {"retcode": self.retcode, "message": self.message}
+
+
+class CallingApiException(_ExceptionWithRetcode):
+    def __repr__(self) -> str:
+        return (
+            "<CallingApiException "
+            f"retcode={self.retcode}, message={self.message!r}>"
+        )
+
+    def __str__(self) -> str:
+        return repr(self)
+
+
+def raise_exception(payload: dict[str, Any]):
+    if payload["retcode"] != 0:
+        raise CallingApiException(payload["retcode"], payload["message"])
```

### Comparing `herta_villa_sdk-0.6.0/hertavilla/match.py` & `herta_villa_sdk-0.6.1/hertavilla/match.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-from __future__ import annotations
-
-import abc
-import re
-
-from hertavilla.message.chain import MessageChain
-
-
-class Match(abc.ABC):
-    @abc.abstractmethod
-    def check(self, chain: MessageChain) -> bool:
-        raise NotImplementedError
-
-
-class Regex(Match):
-    def __init__(self, pattern: str | re.Pattern) -> None:
-        if isinstance(pattern, str):
-            pattern = re.compile(pattern)
-        self.pattern = pattern
-
-    def __repr__(self) -> str:
-        return f"<Match:Regex pattern={self.pattern!r}>"
-
-    def check(self, chain: MessageChain) -> bool:
-        return re.match(self.pattern, chain.plaintext) is not None
-
-
-class Startswith(Match):
-    def __init__(self, prefix: str) -> None:
-        self.prefix = prefix
-
-    def check(self, chain: MessageChain) -> bool:
-        return chain.plaintext.startswith(self.prefix)
-
-    def __repr__(self) -> str:
-        return f"<Match:Startswith prefix={self.prefix!r}>"
-
-
-class Endswith(Match):
-    def __init__(self, suffix: str) -> None:
-        self.suffix = suffix
-
-    def check(self, chain: MessageChain) -> bool:
-        return chain.plaintext.endswith(self.suffix)
-
-    def __repr__(self) -> str:
-        return f"<Match:Endswith suffix={self.suffix!r}>"
-
-
-class Keywords(Regex):
-    def __init__(self, *keywords: str) -> None:
-        self.keywords = keywords
-        self.pattern = re.compile("|".join(keywords))
-
-    def __repr__(self) -> str:
-        return f"<Match:Keywords words={self.keywords!r}>"
+from __future__ import annotations
+
+import abc
+import re
+
+from hertavilla.message.chain import MessageChain
+
+
+class Match(abc.ABC):
+    @abc.abstractmethod
+    def check(self, chain: MessageChain) -> bool:
+        raise NotImplementedError
+
+
+class Regex(Match):
+    def __init__(self, pattern: str | re.Pattern) -> None:
+        if isinstance(pattern, str):
+            pattern = re.compile(pattern)
+        self.pattern = pattern
+
+    def __repr__(self) -> str:
+        return f"<Match:Regex pattern={self.pattern!r}>"
+
+    def check(self, chain: MessageChain) -> bool:
+        return re.match(self.pattern, chain.plaintext) is not None
+
+
+class Startswith(Match):
+    def __init__(self, prefix: str) -> None:
+        self.prefix = prefix
+
+    def check(self, chain: MessageChain) -> bool:
+        return chain.plaintext.startswith(self.prefix)
+
+    def __repr__(self) -> str:
+        return f"<Match:Startswith prefix={self.prefix!r}>"
+
+
+class Endswith(Match):
+    def __init__(self, suffix: str) -> None:
+        self.suffix = suffix
+
+    def check(self, chain: MessageChain) -> bool:
+        return chain.plaintext.endswith(self.suffix)
+
+    def __repr__(self) -> str:
+        return f"<Match:Endswith suffix={self.suffix!r}>"
+
+
+class Keywords(Regex):
+    def __init__(self, *keywords: str) -> None:
+        self.keywords = keywords
+        self.pattern = re.compile("|".join(keywords))
+
+    def __repr__(self) -> str:
+        return f"<Match:Keywords words={self.keywords!r}>"
```

### Comparing `herta_villa_sdk-0.6.0/hertavilla/message/post.py` & `herta_villa_sdk-0.6.1/hertavilla/message/post.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-from __future__ import annotations
-
-from typing import TYPE_CHECKING
-
-from hertavilla.message.types import (
-    MsgContent,
-    MsgContentInfo,
-    _Segment,
-)
-
-if TYPE_CHECKING:
-    from hertavilla.bot import VillaBot
-
-
-# MsgContentInfo for post
-class PostMsgContentInfo(MsgContentInfo):
-    content: PostMsgContent
-
-
-# Segment for post
-
-
-class Post(_Segment):
-    def __init__(self, post_id: str) -> None:
-        self.post_id = post_id
-
-    async def get_text(self, _: VillaBot) -> str:
-        # TODO: 帖子名
-        # 米游社的 API 可以获取到，但是需要 DS
-        # 感觉加到这里有点臃肿了
-        #
-        # https://bbs-api.miyoushe.com/post/wapi/semPosts?gids=6&post_id={}
-        return "[帖子]"
-
-
-# MsgContent for post
-class PostMsgContent(MsgContent):
-    post_id: str
-
-
-def post_to_content(post: Post) -> PostMsgContentInfo:
-    return {"content": PostMsgContent(post_id=post.post_id)}
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
+from hertavilla.message.types import (
+    MsgContent,
+    MsgContentInfo,
+    _Segment,
+)
+
+if TYPE_CHECKING:
+    from hertavilla.bot import VillaBot
+
+
+# MsgContentInfo for post
+class PostMsgContentInfo(MsgContentInfo):
+    content: PostMsgContent
+
+
+# Segment for post
+
+
+class Post(_Segment):
+    def __init__(self, post_id: str) -> None:
+        self.post_id = post_id
+
+    async def get_text(self, _: VillaBot) -> str:
+        # TODO: 帖子名
+        # 米游社的 API 可以获取到，但是需要 DS
+        # 感觉加到这里有点臃肿了
+        #
+        # https://bbs-api.miyoushe.com/post/wapi/semPosts?gids=6&post_id={}
+        return "[帖子]"
+
+
+# MsgContent for post
+class PostMsgContent(MsgContent):
+    post_id: str
+
+
+def post_to_content(post: Post) -> PostMsgContentInfo:
+    return {"content": PostMsgContent(post_id=post.post_id)}
```

### Comparing `herta_villa_sdk-0.6.0/hertavilla/server/__init__.py` & `herta_villa_sdk-0.6.1/hertavilla/server/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,39 @@
-from __future__ import annotations
-
-from typing import Any
-
-from hertavilla.bot import VillaBot
-from hertavilla.server.aiohttp import AIOHTTPBackend
-from hertavilla.server.internal import BaseBackend
-
-DEFAULT_BACKEND = AIOHTTPBackend
-_backend: BaseBackend | None = None
-
-
-def run(
-    *bots_: VillaBot,
-    host: str = "0.0.0.0",
-    port: int = 8080,
-    backend_class: type[BaseBackend] = DEFAULT_BACKEND,
-    **kwargs: Any,
-):
-    global _backend  # noqa: PLW0603
-    if _backend is None:
-        _backend = backend_class(host, port, **kwargs)
-    _backend.run(*bots_)
-
-
-def init_backend(backend: BaseBackend) -> None:
-    global _backend  # noqa: PLW0603
-    if _backend is not None:
-        raise RuntimeError(  # noqa: TRY003
-            "Backend has already been initialized",
-        )
-    _backend = backend
-
-
-def get_backend() -> BaseBackend:
-    if _backend is None:
-        raise RuntimeError("Backend isn't initialized")  # noqa: TRY003
-    return _backend
+from __future__ import annotations
+
+from typing import Any
+
+from hertavilla.bot import VillaBot
+from hertavilla.server.aiohttp import AIOHTTPBackend
+from hertavilla.server.internal import BaseBackend
+
+DEFAULT_BACKEND = AIOHTTPBackend
+_backend: BaseBackend | None = None
+
+
+def run(
+    *bots_: VillaBot,
+    host: str = "0.0.0.0",
+    port: int = 8080,
+    **kwargs: Any,
+):
+    backend = get_backend()
+    backend.run(*bots_, host=host, port=port, **kwargs)
+
+
+def init_backend(
+    backend_class: type[BaseBackend] = DEFAULT_BACKEND,
+    host: str = "0.0.0.0",
+    port: int = 8080,
+) -> None:
+    global _backend  # noqa: PLW0603
+    if _backend is not None:
+        raise RuntimeError(
+            "Backend has already been initialized",
+        )
+    _backend = backend_class(host, port)
+
+
+def get_backend() -> BaseBackend:
+    if _backend is None:
+        raise RuntimeError("Backend isn't initialized")
+    return _backend
```

### Comparing `herta_villa_sdk-0.6.0/hertavilla/server/internal.py` & `herta_villa_sdk-0.6.1/hertavilla/server/internal.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,105 +1,115 @@
-from __future__ import annotations
-
-import abc
-import asyncio
-from dataclasses import dataclass
-import json
-import logging
-from typing import Any, Callable, Sequence
-
-from hertavilla.bot import VillaBot
-from hertavilla.event import parse_event
-
-background_tasks = set()
-
-
-@dataclass
-class ResponseData:
-    status_code: int = 200
-    retcode: int = 0
-    message: str = ""
-
-
-INVALID_EVENT = ResponseData(400, -1, "event body is invalid")
-VERIFY_FAILED = ResponseData(401, -2, "verify failed")
-NO_BOT = ResponseData(404, 1, "no bot with this id")
-
-
-class BaseBackend(abc.ABC):
-    def __init__(self, host: str = "0.0.0.0", port: int = 8080, **kwargs: Any):
-        self.host = host
-        self.port = port
-        self.backend_extra_config = kwargs
-        self.bots: dict[str, VillaBot] = {}
-        self.logger = logging.getLogger(
-            f"hertavilla.backend.{self.name.lower()}",
-        )
-
-    @abc.abstractproperty
-    def name(self) -> str:
-        raise NotImplementedError
-
-    @abc.abstractproperty
-    def app(self) -> Any:
-        raise NotImplementedError
-
-    @abc.abstractmethod
-    def run(
-        self,
-        *bots_: VillaBot,
-        host: str | None = None,
-        port: int | None = None,
-    ):
-        ...
-
-    def _register_bots(
-        self,
-        bots: Sequence[VillaBot],
-        add_router_callback: Callable[[str], Any],
-    ) -> None:
-        for bot in bots:
-            self.bots[bot.bot_id] = bot
-            endpoint = bot.callback_endpoint
-            add_router_callback(endpoint)
-            self.logger.info(
-                f"Register endpoint {endpoint} for bot {bot.bot_id}",
-            )
-
-    async def _run_handles(
-        self,
-        sign: str | None,
-        body: str,
-    ) -> ResponseData:
-        payload = json.loads(body)
-        if not (event_payload := payload.get("event")):
-            self.logger.warning("Event is invalid")
-            return INVALID_EVENT
-        try:
-            event = parse_event(event_payload)
-        except ValueError:
-            self.logger.warning("Event is invalid")
-            return INVALID_EVENT
-
-        if bot := self.bots.get(event.robot.template.id):
-            if sign is None or not bot.verify(sign, body):
-                logging.warn("Event verify check is failed. Reject handling.")
-                return VERIFY_FAILED
-
-            self.logger.info(
-                (
-                    f"[RECV] {event.__class__.__name__} "
-                    f"on bot {event.robot.template.name}"
-                    f"({event.robot.template.id}) "
-                    f"in villa {event.robot.villa_id}"
-                ),
-            )
-            if bot._bot_info is None:  # noqa: SLF001
-                bot.bot_info = event.robot.template
-            task = asyncio.create_task(bot.handle_event(event))
-            background_tasks.add(task)
-            task.add_done_callback(background_tasks.discard)
-            return ResponseData()
-        self.logger.warning(
-            f"Received event but no bot with id {event.robot.template.id}",
-        )
-        return NO_BOT
+from __future__ import annotations
+
+import abc
+import asyncio
+from dataclasses import dataclass
+import json
+import logging
+from typing import Any, Callable, Sequence
+
+from hertavilla.bot import VillaBot
+from hertavilla.event import parse_event
+
+from ._lifespan import L_FUNC
+
+background_tasks = set()
+
+
+@dataclass
+class ResponseData:
+    status_code: int = 200
+    retcode: int = 0
+    message: str = ""
+
+
+INVALID_EVENT = ResponseData(400, -1, "event body is invalid")
+VERIFY_FAILED = ResponseData(401, -2, "verify failed")
+NO_BOT = ResponseData(404, 1, "no bot with this id")
+
+
+class BaseBackend(abc.ABC):
+    def __init__(self, host: str = "0.0.0.0", port: int = 8080, **kwargs: Any):
+        self.host = host
+        self.port = port
+        self.backend_extra_config = kwargs
+        self.bots: dict[str, VillaBot] = {}
+        self.logger = logging.getLogger(
+            f"hertavilla.backend.{self.name.lower()}",
+        )
+
+    @abc.abstractproperty
+    def name(self) -> str:
+        raise NotImplementedError
+
+    @abc.abstractproperty
+    def app(self) -> Any:
+        raise NotImplementedError
+
+    @abc.abstractmethod
+    def run(
+        self,
+        *bots_: VillaBot,
+        host: str | None = None,
+        port: int | None = None,
+    ):
+        raise NotImplementedError
+
+    @abc.abstractmethod
+    def on_startup(self, func: L_FUNC):
+        raise NotImplementedError
+
+    @abc.abstractmethod
+    def on_shutdown(self, func: L_FUNC):
+        raise NotImplementedError
+
+    def _register_bots(
+        self,
+        bots: Sequence[VillaBot],
+        add_router_callback: Callable[[str], Any],
+    ) -> None:
+        for bot in bots:
+            self.bots[bot.bot_id] = bot
+            endpoint = bot.callback_endpoint
+            add_router_callback(endpoint)
+            self.logger.info(
+                f"Register endpoint {endpoint} for bot {bot.bot_id}",
+            )
+
+    async def _run_handles(
+        self,
+        sign: str | None,
+        body: str,
+    ) -> ResponseData:
+        payload = json.loads(body)
+        if not (event_payload := payload.get("event")):
+            self.logger.warning("Event is invalid")
+            return INVALID_EVENT
+        try:
+            event = parse_event(event_payload)
+        except ValueError:
+            self.logger.warning("Event is invalid")
+            return INVALID_EVENT
+
+        if bot := self.bots.get(event.robot.template.id):
+            if sign is None or not bot.verify(sign, body):
+                logging.warn("Event verify check is failed. Reject handling.")
+                return VERIFY_FAILED
+
+            self.logger.info(
+                (
+                    f"[RECV] {event.__class__.__name__} "
+                    f"on bot {event.robot.template.name}"
+                    f"({event.robot.template.id}) "
+                    f"in villa {event.robot.villa_id}"
+                ),
+            )
+            if bot._bot_info is None:  # noqa: SLF001
+                bot.bot_info = event.robot.template
+            task = asyncio.create_task(bot.handle_event(event))
+            background_tasks.add(task)
+            task.add_done_callback(background_tasks.discard)
+            return ResponseData()
+        self.logger.warning(
+            f"Received event but no bot with id {event.robot.template.id}",
+        )
+        return NO_BOT
```

### Comparing `herta_villa_sdk-0.6.0/hertavilla/typing.py` & `herta_villa_sdk-0.6.1/hertavilla/typing.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from __future__ import annotations
-
-import sys
-
-# Because of pydantic's exception
-# Herta SDK provides this `TypedDict`
-# Import it by this:
-# from hertavilla.typing import TypedDict
-
-# Pydantic exception:
-#   TypeError: You should use `typing_extensions.TypedDict`
-#   instead of `typing.TypedDict` with Python < 3.9.2.
-#   Without it, there is no way to differentiate
-#   required and optional fields when subclassed.
-
-if sys.version_info >= (3, 9, 2):
-    from typing import TypedDict as TypedDict
-else:
-    from typing_extensions import TypedDict as TypedDict
+from __future__ import annotations
+
+import sys
+
+# Because of pydantic's exception
+# Herta SDK provides this `TypedDict`
+# Import it by this:
+# from hertavilla.typing import TypedDict
+
+# Pydantic exception:
+#   TypeError: You should use `typing_extensions.TypedDict`
+#   instead of `typing.TypedDict` with Python < 3.9.2.
+#   Without it, there is no way to differentiate
+#   required and optional fields when subclassed.
+
+if sys.version_info >= (3, 9, 2):
+    from typing import TypedDict as TypedDict
+else:
+    from typing_extensions import TypedDict as TypedDict
```

### Comparing `herta_villa_sdk-0.6.0/hertavilla/utils.py` & `herta_villa_sdk-0.6.1/hertavilla/utils.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from __future__ import annotations
-
-import json
-
-
-class MsgEncoder(json.JSONEncoder):
-    def default(self, obj):
-        from hertavilla.message.types import MsgContent
-
-        if isinstance(obj, MsgContent):
-            data = obj.dict()
-            for k in data.copy().keys():
-                if k.startswith("_"):
-                    data.pop(k)
-            return data
-        return json.JSONEncoder.default(self, obj)
-
-
-def _c(text: str) -> int:
-    return (len(text.encode("utf-16")) // 2) - 1
-
-
-def _rc(length: int) -> int:
-    return (length + 1) * 2
+from __future__ import annotations
+
+import json
+
+
+class MsgEncoder(json.JSONEncoder):
+    def default(self, obj):
+        from hertavilla.message.types import MsgContent
+
+        if isinstance(obj, MsgContent):
+            data = obj.dict()
+            for k in data.copy().keys():
+                if k.startswith("_"):
+                    data.pop(k)
+            return data
+        return json.JSONEncoder.default(self, obj)
+
+
+def _c(text: str) -> int:
+    return (len(text.encode("utf-16")) // 2) - 1
+
+
+def _rc(length: int) -> int:
+    return (length + 1) * 2
```

### Comparing `herta_villa_sdk-0.6.0/pyproject.toml` & `herta_villa_sdk-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 keywords = [
     "mihoyo",
     "miyoushe",
     "bot",
     "villa",
 ]
 dynamic = []
-version = "0.6.0"
+version = "0.6.1"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/Herta-villa/Herta-villa-SDK"
 Documentation = "https://github.com/Herta-villa/Herta-villa-SDK"
@@ -83,14 +83,15 @@
     "COM",
     "A",
     "B",
     "ASYNC",
 ]
 ignore = [
     "PLR0913",
+    "TRY003",
 ]
 allowed-confusables = [
     "，",
     "。",
     "（",
     "）",
     "；",
```

### Comparing `herta_villa_sdk-0.6.0/PKG-INFO` & `herta_villa_sdk-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: herta-villa-sdk
-Version: 0.6.0
+Version: 0.6.1
 Summary: 大别野「黑塔」Python SDK
 Keywords: mihoyo miyoushe bot villa
 Author-Email: MingxuanGame <MingxuanGame@outlook.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Herta-villa/Herta-villa-SDK
 Project-URL: Documentation, https://github.com/Herta-villa/Herta-villa-SDK
 Project-URL: Repository, https://github.com/Herta-villa/Herta-villa-SDK
@@ -47,14 +47,15 @@
 
 ## 快速开始
 
 你需要拥有一个[大别野](https://dby.miyoushe.com/chat)机器人。可前往大别野[「机器人开发者社区」](https://dby.miyoushe.com/chat/463/20020)（`OpenVilla`）申请。
 
 ```python
 from hertavilla import MessageChain, SendMessageEvent, VillaBot, run
+from hertavilla.server import init_backend
 
 
 PUB_KEY = """-----BEGIN PUBLIC KEY-----
 aaa
 bbb
 ccc
 -----END PUBLIC KEY-----
@@ -76,14 +77,15 @@
     message = event.message
     if str(message[1]) == "/hello":
         chain = MessageChain()
         chain.append("world")
         await bot.send(event.villa_id, event.room_id, chain)
 
 
+init_backend()  # 初始化后端
 run(bot)  # 运行 bot
 ```
 
 可以向你的 bot 发送 `@Bot /hello`，bot 会回复 `world`。
 
 ## 示例
```

