# Comparing `tmp/nonebot_plugin_spark_gpt-1.2.0.tar.gz` & `tmp/nonebot_plugin_spark_gpt-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_spark_gpt-1.2.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_spark_gpt-1.2.1.tar", max compression
```

## Comparing `nonebot_plugin_spark_gpt-1.2.0.tar` & `nonebot_plugin_spark_gpt-1.2.1.tar`

### file list

```diff
@@ -1,86 +1,120 @@
--rw-r--r--   0        0        0      219 2023-07-11 09:53:31.539890 nonebot_plugin_spark_gpt-1.2.0/nonebot/adapters/discord/__init__.py
--rw-r--r--   0        0        0    17261 2023-07-11 09:53:31.540890 nonebot_plugin_spark_gpt-1.2.0/nonebot/adapters/discord/adapter.py
--rw-r--r--   0        0        0      138 2023-07-11 09:53:31.541890 nonebot_plugin_spark_gpt-1.2.0/nonebot/adapters/discord/api/__init__.py
--rw-r--r--   0        0        0       27 2023-07-11 09:53:31.542890 nonebot_plugin_spark_gpt-1.2.0/nonebot/adapters/discord/api/client.py
--rw-r--r--   0        0        0    51932 2023-07-11 09:53:31.542890 nonebot_plugin_spark_gpt-1.2.0/nonebot/adapters/discord/api/client.pyi
--rw-r--r--   0        0        0    98693 2023-07-11 09:53:31.543890 nonebot_plugin_spark_gpt-1.2.0/nonebot/adapters/discord/api/handle.py
--rw-r--r--   0        0        0   115238 2023-07-11 09:53:31.544890 nonebot_plugin_spark_gpt-1.2.0/nonebot/adapters/discord/api/model.py
--rw-r--r--   0        0        0     1482 2023-07-11 09:53:31.544890 nonebot_plugin_spark_gpt-1.2.0/nonebot/adapters/discord/api/request.py
--rw-r--r--   0        0        0    34839 2023-07-11 09:53:31.544890 nonebot_plugin_spark_gpt-1.2.0/nonebot/adapters/discord/api/types.py
--rw-r--r--   0        0        0     2441 2023-07-11 09:53:31.545890 nonebot_plugin_spark_gpt-1.2.0/nonebot/adapters/discord/api/utils.py
--rw-r--r--   0        0        0     7255 2023-07-11 09:53:31.545890 nonebot_plugin_spark_gpt-1.2.0/nonebot/adapters/discord/bot.py
--rw-r--r--   0        0        0     2192 2023-07-11 09:53:31.546890 nonebot_plugin_spark_gpt-1.2.0/nonebot/adapters/discord/config.py
--rw-r--r--   0        0        0    28334 2023-07-11 09:53:31.546890 nonebot_plugin_spark_gpt-1.2.0/nonebot/adapters/discord/event.py
--rw-r--r--   0        0        0     2076 2023-07-11 09:53:31.546890 nonebot_plugin_spark_gpt-1.2.0/nonebot/adapters/discord/exception.py
--rw-r--r--   0        0        0    13603 2023-07-11 09:53:31.547890 nonebot_plugin_spark_gpt-1.2.0/nonebot/adapters/discord/message.py
--rw-r--r--   0        0        0     2874 2023-07-11 09:53:31.547890 nonebot_plugin_spark_gpt-1.2.0/nonebot/adapters/discord/payload.py
--rw-r--r--   0        0        0     1946 2023-07-11 09:53:31.547890 nonebot_plugin_spark_gpt-1.2.0/nonebot/adapters/discord/typing.py
--rw-r--r--   0        0        0      626 2023-07-11 09:53:31.548892 nonebot_plugin_spark_gpt-1.2.0/nonebot/adapters/discord/utils.py
--rw-r--r--   0        0        0      836 2023-07-18 04:47:31.258172 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/__init__.py
--rw-r--r--   0        0        0     4008 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/chatbot/bard.py
--rw-r--r--   0        0        0     9680 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/chatbot/chatgpt_web.py
--rw-r--r--   0        0        0     9032 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/chatbot/claude_ai.py
--rw-r--r--   0        0        0     3976 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/chatbot/load_config.py
--rw-r--r--   0        0        0     6760 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/chatbot/newbing.py
--rw-r--r--   0        0        0     6153 2023-07-18 14:14:01.907658 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/chatbot/poe.py
--rw-r--r--   0        0        0     7619 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/chatbot/slack_claude.py
--rw-r--r--   0        0        0     8129 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/chatbot/spark_desk.py
--rw-r--r--   0        0        0     7435 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/chatbot/sydneybing.py
--rw-r--r--   0        0        0     6802 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/chatbot/tongyiqianwen.py
--rw-r--r--   0        0        0        0 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/__init__.py
--rw-r--r--   0        0        0    17078 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/BingImageCreator.py
--rw-r--r--   0        0        0    11565 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/chathub.py
--rw-r--r--   0        0        0     2057 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/constants.py
--rw-r--r--   0        0        0     4460 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/conversation.py
--rw-r--r--   0        0        0     1256 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/conversation_style.py
--rw-r--r--   0        0        0     7856 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/EdgeGPT.py
--rw-r--r--   0        0        0    14237 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/EdgeUtils.py
--rw-r--r--   0        0        0       46 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/exceptions.py
--rw-r--r--   0        0        0      267 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/ImageGen.py
--rw-r--r--   0        0        0     2247 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/locale.py
--rw-r--r--   0        0        0     7512 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/main.py
--rw-r--r--   0        0        0     5792 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/request.py
--rw-r--r--   0        0        0      955 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/utilities.py
--rw-r--r--   0        0        0       83 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/chatbot/utils/SydneyGPT/__init__.py
--rw-r--r--   0        0        0     1454 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/chatbot/utils/SydneyGPT/conversation_style.py
--rw-r--r--   0        0        0      127 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/chatbot/utils/SydneyGPT/main.py
--rw-r--r--   0        0        0     5878 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/chatbot/utils/SydneyGPT/SydneyGPT.py
--rw-r--r--   0        0        0      719 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/chatbot/utils/SydneyGPT/SydneyGPTUtils.py
--rw-r--r--   0        0        0        0 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/common/__init__.py
--rw-r--r--   0        0        0     5559 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/common/config.py
--rw-r--r--   0        0        0     1694 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/common/load_config.py
--rw-r--r--   0        0        0     4951 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/common/mytypes.py
--rw-r--r--   0        0        0     4583 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/common/prefix_data.py
--rw-r--r--   0        0        0    30736 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/common/prompt_data.py
--rw-r--r--   0        0        0     9955 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/common/user_data.py
--rw-r--r--   0        0        0    14446 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/common/web/app.py
--rw-r--r--   0        0        0      547 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/common/web/data/spark_gpt/common/config.json
--rw-r--r--   0        0        0        0 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/common/web/templates/__init__.py
--rw-r--r--   0        0        0     4730 2023-07-18 14:23:03.984592 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/common/web/templates/config.html
--rw-r--r--   0        0        0     2246 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/common/web/templates/index.html
--rw-r--r--   0        0        0    10215 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/common/web/templates/prefix.html
--rw-r--r--   0        0        0    10211 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/common/web/templates/prompt.html
--rw-r--r--   0        0        0       23 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/platforms/__init__.py
--rw-r--r--   0        0        0       51 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/platforms/nonebot/__init__.py
--rw-r--r--   0        0        0    17861 2023-07-18 05:09:10.149494 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/platforms/nonebot/bot_main.py
--rw-r--r--   0        0        0    26033 2023-07-18 04:44:52.814514 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/platforms/nonebot/config_main.py
--rw-r--r--   0        0        0        0 2023-07-18 04:29:07.301197 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/platforms/nonebot/HelpMsg.jpeg
--rw-r--r--   0        0        0        0 2023-07-18 05:06:33.089620 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/platforms/nonebot/PrefixMsg.jpeg
--rw-r--r--   0        0        0  2236062 2023-07-18 05:06:33.086620 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/platforms/nonebot/PromptMsg.jpeg
--rw-r--r--   0        0        0   763987 2023-07-18 05:06:33.081637 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/platforms/nonebot/SourceMsg.jpeg
--rw-r--r--   0        0        0   602183 2023-07-18 04:29:07.301197 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/platforms/nonebot/SuperMsg.jpeg
--rw-r--r--   0        0        0     2275 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/platforms/nonebot/userlinks.py
--rw-r--r--   0        0        0    15735 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/platforms/nonebot/utils.py
--rw-r--r--   0        0        0     6458 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/platforms/temp_bots.py
--rw-r--r--   0        0        0     2031 2023-07-18 14:15:26.312443 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/utils/render.py
--rw-r--r--   0        0        0  1458204 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/utils/templates/katex/katex.min.b64_fonts.css
--rw-r--r--   0        0        0   270288 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/utils/templates/katex/katex.min.js
--rw-r--r--   0        0        0     1290 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/utils/templates/katex/mathtex-script-type.min.js
--rw-r--r--   0        0        0    19652 2023-07-18 14:07:51.094876 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/utils/templates/markdown.css
--rw-r--r--   0        0        0     1259 2023-07-18 14:07:25.504474 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/utils/templates/markdown.html
--rw-r--r--   0        0        0     4963 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/utils/templates/pygments-default.css
--rw-r--r--   0        0        0      125 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/utils/templates/text.css
--rw-r--r--   0        0        0     1113 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/utils/utils.py
--rw-r--r--   0        0        0     1005 2023-07-18 07:42:13.353393 nonebot_plugin_spark_gpt-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     8456 2023-07-18 07:21:07.799511 nonebot_plugin_spark_gpt-1.2.0/README.md
--rw-r--r--   0        0        0     9665 1970-01-01 00:00:00.000000 nonebot_plugin_spark_gpt-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      219 2023-07-11 09:53:31.539890 nonebot_plugin_spark_gpt-1.2.1/nonebot/adapters/discord/__init__.py
+-rw-r--r--   0        0        0    17261 2023-07-11 09:53:31.540890 nonebot_plugin_spark_gpt-1.2.1/nonebot/adapters/discord/adapter.py
+-rw-r--r--   0        0        0      138 2023-07-11 09:53:31.541890 nonebot_plugin_spark_gpt-1.2.1/nonebot/adapters/discord/api/__init__.py
+-rw-r--r--   0        0        0       27 2023-07-11 09:53:31.542890 nonebot_plugin_spark_gpt-1.2.1/nonebot/adapters/discord/api/client.py
+-rw-r--r--   0        0        0    51932 2023-07-11 09:53:31.542890 nonebot_plugin_spark_gpt-1.2.1/nonebot/adapters/discord/api/client.pyi
+-rw-r--r--   0        0        0    98693 2023-07-11 09:53:31.543890 nonebot_plugin_spark_gpt-1.2.1/nonebot/adapters/discord/api/handle.py
+-rw-r--r--   0        0        0   115238 2023-07-11 09:53:31.544890 nonebot_plugin_spark_gpt-1.2.1/nonebot/adapters/discord/api/model.py
+-rw-r--r--   0        0        0     1482 2023-07-11 09:53:31.544890 nonebot_plugin_spark_gpt-1.2.1/nonebot/adapters/discord/api/request.py
+-rw-r--r--   0        0        0    34839 2023-07-11 09:53:31.544890 nonebot_plugin_spark_gpt-1.2.1/nonebot/adapters/discord/api/types.py
+-rw-r--r--   0        0        0     2441 2023-07-11 09:53:31.545890 nonebot_plugin_spark_gpt-1.2.1/nonebot/adapters/discord/api/utils.py
+-rw-r--r--   0        0        0     7255 2023-07-11 09:53:31.545890 nonebot_plugin_spark_gpt-1.2.1/nonebot/adapters/discord/bot.py
+-rw-r--r--   0        0        0     2192 2023-07-11 09:53:31.546890 nonebot_plugin_spark_gpt-1.2.1/nonebot/adapters/discord/config.py
+-rw-r--r--   0        0        0    28334 2023-07-11 09:53:31.546890 nonebot_plugin_spark_gpt-1.2.1/nonebot/adapters/discord/event.py
+-rw-r--r--   0        0        0     2076 2023-07-11 09:53:31.546890 nonebot_plugin_spark_gpt-1.2.1/nonebot/adapters/discord/exception.py
+-rw-r--r--   0        0        0    13603 2023-07-11 09:53:31.547890 nonebot_plugin_spark_gpt-1.2.1/nonebot/adapters/discord/message.py
+-rw-r--r--   0        0        0     2874 2023-07-11 09:53:31.547890 nonebot_plugin_spark_gpt-1.2.1/nonebot/adapters/discord/payload.py
+-rw-r--r--   0        0        0     1946 2023-07-11 09:53:31.547890 nonebot_plugin_spark_gpt-1.2.1/nonebot/adapters/discord/typing.py
+-rw-r--r--   0        0        0      626 2023-07-11 09:53:31.548892 nonebot_plugin_spark_gpt-1.2.1/nonebot/adapters/discord/utils.py
+-rw-r--r--   0        0        0      836 2023-07-18 04:47:31.258172 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-19 08:14:04.493611 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/__init__.py
+-rw-r--r--   0        0        0     4008 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/bard.py
+-rw-r--r--   0        0        0     9680 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/chatgpt_web.py
+-rw-r--r--   0        0        0     9032 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/claude_ai.py
+-rw-r--r--   0        0        0     4541 2023-07-19 08:52:31.757677 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/load_config.py
+-rw-r--r--   0        0        0     6760 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/newbing.py
+-rw-r--r--   0        0        0     8434 2023-07-19 09:50:18.910215 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/poe.py
+-rw-r--r--   0        0        0     7619 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/slack_claude.py
+-rw-r--r--   0        0        0     8129 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/spark_desk.py
+-rw-r--r--   0        0        0     7435 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/sydneybing.py
+-rw-r--r--   0        0        0     6802 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/tongyiqianwen.py
+-rw-r--r--   0        0        0        0 2023-07-19 08:14:04.488610 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-19 08:51:03.240242 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/__init__.py
+-rw-r--r--   0        0        0    17586 2023-07-19 08:50:59.147722 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/BingImageCreator.py
+-rw-r--r--   0        0        0    11837 2023-07-19 08:51:01.064843 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/chathub.py
+-rw-r--r--   0        0        0     2107 2023-07-19 08:51:04.982654 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/constants.py
+-rw-r--r--   0        0        0     4582 2023-07-19 08:51:08.212221 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/conversation.py
+-rw-r--r--   0        0        0     1312 2023-07-19 08:51:06.614074 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/conversation_style.py
+-rw-r--r--   0        0        0     8088 2023-07-19 08:51:10.504420 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/EdgeGPT.py
+-rw-r--r--   0        0        0    14626 2023-07-19 08:50:55.647270 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/EdgeUtils.py
+-rw-r--r--   0        0        0       48 2023-07-19 08:50:53.449019 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/exceptions.py
+-rw-r--r--   0        0        0      278 2023-07-19 08:50:48.240509 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/ImageGen.py
+-rw-r--r--   0        0        0     2332 2023-07-19 08:50:51.738573 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/locale.py
+-rw-r--r--   0        0        0     7757 2023-07-19 08:50:44.460438 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/main.py
+-rw-r--r--   0        0        0     5948 2023-07-19 08:50:50.007184 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/request.py
+-rw-r--r--   0        0        0      992 2023-07-19 08:51:13.314721 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/utilities.py
+-rw-r--r--   0        0        0    25186 2023-07-19 14:24:28.880037 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/poe.py
+-rw-r--r--   0        0        0        0 2023-07-19 06:18:30.467959 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/poe_graphql/__init__.py
+-rw-r--r--   0        0        0     1145 2023-07-19 06:18:30.461961 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/poe_graphql/AddHumanMessageMutation.graphql
+-rw-r--r--   0        0        0      536 2023-07-19 06:18:30.461961 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/poe_graphql/AddMessageBreakMutation.graphql
+-rw-r--r--   0        0        0      187 2023-07-19 06:18:30.461961 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/poe_graphql/AutoSubscriptionMutation.graphql
+-rw-r--r--   0        0        0      105 2023-07-19 06:18:30.461961 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/poe_graphql/BioFragment.graphql
+-rw-r--r--   0        0        0       78 2023-07-19 06:18:30.462960 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/poe_graphql/ChatAddedSubscription.graphql
+-rw-r--r--   0        0        0      106 2023-07-19 06:18:30.462960 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/poe_graphql/ChatFragment.graphql
+-rw-r--r--   0        0        0    12084 2023-07-19 06:18:30.462960 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/poe_graphql/ChatListPaginationQuery.graphql
+-rw-r--r--   0        0        0      712 2023-07-19 06:18:30.462960 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/poe_graphql/ChatPaginationQuery.graphql
+-rw-r--r--   0        0        0      162 2023-07-19 06:18:30.462960 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/poe_graphql/ChatViewQuery.graphql
+-rw-r--r--   0        0        0      167 2023-07-19 06:18:30.463987 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/poe_graphql/DeleteHumanMessagesMutation.graphql
+-rw-r--r--   0        0        0      129 2023-07-19 06:18:30.463987 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/poe_graphql/DeleteMessageMutation.graphql
+-rw-r--r--   0        0        0      154 2023-07-19 06:18:30.463987 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/poe_graphql/DeleteUserMessagesMutation.graphql
+-rw-r--r--   0        0        0     1148 2023-07-19 06:18:30.463987 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/poe_graphql/ExploreBotsListPaginationQuery.graphql
+-rw-r--r--   0        0        0      111 2023-07-19 06:18:30.463987 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/poe_graphql/HandleFragment.graphql
+-rw-r--r--   0        0        0      319 2023-07-19 06:18:30.464960 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/poe_graphql/LoginWithVerificationCodeMutation.graphql
+-rw-r--r--   0        0        0     1985 2023-07-19 06:18:30.464960 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/poe_graphql/MessageAddedSubscription.graphql
+-rw-r--r--   0        0        0      141 2023-07-19 06:18:30.464960 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/poe_graphql/MessageDeletedSubscription.graphql
+-rw-r--r--   0        0        0      207 2023-07-19 06:18:30.464960 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/poe_graphql/MessageFragment.graphql
+-rw-r--r--   0        0        0      152 2023-07-19 06:18:30.464960 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/poe_graphql/MessageRemoveVoteMutation.graphql
+-rw-r--r--   0        0        0      223 2023-07-19 06:18:30.465959 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/poe_graphql/MessageSetVoteMutation.graphql
+-rw-r--r--   0        0        0     1832 2023-07-19 06:18:30.465959 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/poe_graphql/PoeBotCreateMutation.graphql
+-rw-r--r--   0        0        0      968 2023-07-19 06:18:30.465959 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/poe_graphql/PoeBotEditMutation.graphql
+-rw-r--r--   0        0        0      963 2023-07-19 06:18:30.465959 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/poe_graphql/SendMessageMutation.graphql
+-rw-r--r--   0        0        0      275 2023-07-19 06:18:30.465959 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/poe_graphql/SendVerificationCodeForLoginMutation.graphql
+-rw-r--r--   0        0        0      222 2023-07-19 06:18:30.465959 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/poe_graphql/ShareMessagesMutation.graphql
+-rw-r--r--   0        0        0      321 2023-07-19 06:18:30.466959 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/poe_graphql/SignupWithVerificationCodeMutation.graphql
+-rw-r--r--   0        0        0      166 2023-07-19 06:18:30.466959 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/poe_graphql/StaleChatUpdateMutation.graphql
+-rw-r--r--   0        0        0      170 2023-07-19 06:18:30.466959 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/poe_graphql/SubscriptionsMutation.graphql
+-rw-r--r--   0        0        0       98 2023-07-19 06:18:30.466959 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/poe_graphql/SummarizePlainPostQuery.graphql
+-rw-r--r--   0        0        0      150 2023-07-19 06:18:30.466959 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/poe_graphql/SummarizeQuotePostQuery.graphql
+-rw-r--r--   0        0        0      183 2023-07-19 06:18:30.466959 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/poe_graphql/SummarizeSharePostQuery.graphql
+-rw-r--r--   0        0        0      382 2023-07-19 06:18:30.467959 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/poe_graphql/UserSnippetFragment.graphql
+-rw-r--r--   0        0        0      421 2023-07-19 06:18:30.467959 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/poe_graphql/ViewerInfoQuery.graphql
+-rw-r--r--   0        0        0     1068 2023-07-19 06:18:30.467959 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/poe_graphql/ViewerStateFragment.graphql
+-rw-r--r--   0        0        0      700 2023-07-19 06:18:30.467959 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/poe_graphql/ViewerStateUpdatedSubscription.graphql
+-rw-r--r--   0        0        0       83 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/SydneyGPT/__init__.py
+-rw-r--r--   0        0        0     1454 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/SydneyGPT/conversation_style.py
+-rw-r--r--   0        0        0      127 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/SydneyGPT/main.py
+-rw-r--r--   0        0        0     5878 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/SydneyGPT/SydneyGPT.py
+-rw-r--r--   0        0        0      719 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/SydneyGPT/SydneyGPTUtils.py
+-rw-r--r--   0        0        0        0 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/common/__init__.py
+-rw-r--r--   0        0        0     5657 2023-07-19 08:44:30.873672 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/common/config.py
+-rw-r--r--   0        0        0     1694 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/common/load_config.py
+-rw-r--r--   0        0        0     4998 2023-07-19 08:26:34.686822 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/common/mytypes.py
+-rw-r--r--   0        0        0     4583 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/common/prefix_data.py
+-rw-r--r--   0        0        0    30736 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/common/prompt_data.py
+-rw-r--r--   0        0        0     9955 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/common/user_data.py
+-rw-r--r--   0        0        0    14709 2023-07-19 08:44:30.885588 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/common/web/app.py
+-rw-r--r--   0        0        0      547 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/common/web/data/spark_gpt/common/config.json
+-rw-r--r--   0        0        0        0 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/common/web/templates/__init__.py
+-rw-r--r--   0        0        0     4730 2023-07-18 14:23:03.984592 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/common/web/templates/config.html
+-rw-r--r--   0        0        0     2246 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/common/web/templates/index.html
+-rw-r--r--   0        0        0    10215 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/common/web/templates/prefix.html
+-rw-r--r--   0        0        0    10211 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/common/web/templates/prompt.html
+-rw-r--r--   0        0        0       23 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/platforms/__init__.py
+-rw-r--r--   0        0        0       51 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/platforms/nonebot/__init__.py
+-rw-r--r--   0        0        0    17861 2023-07-18 05:09:10.149494 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/platforms/nonebot/bot_main.py
+-rw-r--r--   0        0        0    26033 2023-07-18 04:44:52.814514 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/platforms/nonebot/config_main.py
+-rw-r--r--   0        0        0     2275 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/platforms/nonebot/userlinks.py
+-rw-r--r--   0        0        0    15735 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/platforms/nonebot/utils.py
+-rw-r--r--   0        0        0     6523 2023-07-19 09:05:38.201293 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/platforms/temp_bots.py
+-rw-r--r--   0        0        0     2092 2023-07-19 11:14:09.912607 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/utils/render.py
+-rw-r--r--   0        0        0  1458204 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/utils/templates/katex/katex.min.b64_fonts.css
+-rw-r--r--   0        0        0   270288 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/utils/templates/katex/katex.min.js
+-rw-r--r--   0        0        0     1290 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/utils/templates/katex/mathtex-script-type.min.js
+-rw-r--r--   0        0        0    19652 2023-07-18 14:07:51.094876 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/utils/templates/markdown.css
+-rw-r--r--   0        0        0     1259 2023-07-19 08:47:11.045440 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/utils/templates/markdown.html
+-rw-r--r--   0        0        0     4963 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/utils/templates/pygments-default.css
+-rw-r--r--   0        0        0      125 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/utils/templates/text.css
+-rw-r--r--   0        0        0     1113 1979-12-31 16:00:00.000000 nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/utils/utils.py
+-rw-r--r--   0        0        0     1005 2023-07-19 08:47:39.497772 nonebot_plugin_spark_gpt-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     8456 2023-07-19 08:46:50.874546 nonebot_plugin_spark_gpt-1.2.1/README.md
+-rw-r--r--   0        0        0     9665 1970-01-01 00:00:00.000000 nonebot_plugin_spark_gpt-1.2.1/PKG-INFO
```

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot/adapters/discord/adapter.py` & `nonebot_plugin_spark_gpt-1.2.1/nonebot/adapters/discord/adapter.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot/adapters/discord/api/client.pyi` & `nonebot_plugin_spark_gpt-1.2.1/nonebot/adapters/discord/api/client.pyi`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot/adapters/discord/api/handle.py` & `nonebot_plugin_spark_gpt-1.2.1/nonebot/adapters/discord/api/handle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot/adapters/discord/api/model.py` & `nonebot_plugin_spark_gpt-1.2.1/nonebot/adapters/discord/api/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot/adapters/discord/api/request.py` & `nonebot_plugin_spark_gpt-1.2.1/nonebot/adapters/discord/api/request.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot/adapters/discord/api/types.py` & `nonebot_plugin_spark_gpt-1.2.1/nonebot/adapters/discord/api/types.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot/adapters/discord/api/utils.py` & `nonebot_plugin_spark_gpt-1.2.1/nonebot/adapters/discord/api/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot/adapters/discord/bot.py` & `nonebot_plugin_spark_gpt-1.2.1/nonebot/adapters/discord/bot.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot/adapters/discord/config.py` & `nonebot_plugin_spark_gpt-1.2.1/nonebot/adapters/discord/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot/adapters/discord/event.py` & `nonebot_plugin_spark_gpt-1.2.1/nonebot/adapters/discord/event.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot/adapters/discord/exception.py` & `nonebot_plugin_spark_gpt-1.2.1/nonebot/adapters/discord/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot/adapters/discord/message.py` & `nonebot_plugin_spark_gpt-1.2.1/nonebot/adapters/discord/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot/adapters/discord/payload.py` & `nonebot_plugin_spark_gpt-1.2.1/nonebot/adapters/discord/payload.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot/adapters/discord/typing.py` & `nonebot_plugin_spark_gpt-1.2.1/nonebot/adapters/discord/typing.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot/adapters/discord/utils.py` & `nonebot_plugin_spark_gpt-1.2.1/nonebot/adapters/discord/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/__init__.py` & `nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/chatbot/bard.py` & `nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/bard.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/chatbot/chatgpt_web.py` & `nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/chatgpt_web.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/chatbot/claude_ai.py` & `nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/claude_ai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/chatbot/load_config.py` & `nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/load_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,24 +15,32 @@
     from .newbing import ABLE as NEWBING_ABLE
     from .poe import ABLE as POE_ABLE
     from .slack_claude import ABLE as SLACKCLAUDE_ABLE
     from .claude_ai import ABLE as CLAUDE_AI_ABLE
     from .bard import ABLE as BARD_ABLE
     from .spark_desk import ABLE as SPARKDESK_ABLE
     from .tongyiqianwen import ABLE as TongYiQianWen_ABLE
-
+    from .poe import SUBSCRIBE_ABLE as POE_SUBSCRIBE_ABLE
     able_dict = {
         "poe chatgpt": {
             "able": POE_ABLE,
             "des": "poe网站的chatgpt,支持预设最长约2000字,支持前缀但字数不宜过多",
         },
         "poe claude": {
             "able": POE_ABLE,
             "des": "poe网站的claude,支持预设最长约2000字,支持前缀但字数不宜过多",
         },
+        "poe chatgpt4": {
+            "able": POE_SUBSCRIBE_ABLE,
+            "des": "poe网站的chatgpt4,仅限已定阅用户使用,仅限白名单用户对话使用,支持预设最长约2000字,支持前缀但字数不宜过多",
+        },
+        "poe claude-2-100k": {
+            "able": POE_SUBSCRIBE_ABLE,
+            "des": "poe网站的claude-2-100k,仅限已定阅用户使用,仅限白名单用户对话使用,支持预设最长约2000字,支持前缀但字数不宜过多",
+        },
         "chatgpt web": {
             "able": CHATGPTWEB_ABLE,
             "des": "openai官网的chatgpt网页版,支持预设最长约5400字,支持前缀但字数不宜过多",
         },
         "claude ai": {
             "able": CLAUDE_AI_ABLE,
             "des": "claude官网的claude网页版,支持超极长的预设,有内容安全审查,支持前缀字数也很长",
```

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/chatbot/newbing.py` & `nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/newbing.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/chatbot/poe.py` & `nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/poe.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,75 +1,115 @@
 import asyncio
 import uuid
 
 from nonebot.log import logger
 from nonebot.utils import run_sync
 
-import poe
+from .utils import poe
 from ..common.config import config
 from ..common.mytypes import CommonUserInfo, BotData, BotInfo
 from ..common.user_data import common_users
 
 COOKIE = ""
 PROXY = ""
 ABLE = True
+SUBSCRIBE_ABLE = True
 CLIENT = None
+WHITE_LIST = ""
 
 
 def load_config():
-    global COOKIE, PROXY, ABLE
+    global COOKIE, PROXY, ABLE, SUBSCRIBE_ABLE, WHITE_LIST
     ABLE = True
+    SUBSCRIBE_ABLE = True
     try:
         PROXY = config.get_config(source="Poe配置", config_name="proxy")
     except Exception as e:
         logger.info(f"加载Poe配置时warn:{str(e)},如果你已经配置了分流或全局代理,请无视此warn")
 
     try:
         COOKIE = config.get_config(source="Poe配置", config_name="cookie")
     except Exception as e:
         ABLE = False
+        SUBSCRIBE_ABLE = False
         logger.warning(f"加载Poe配置时warn:{str(e)},无法使用Poe")
 
+    try:
+        subscrid = config.get_config(source="Poe配置", config_name="subscribed")
+        if subscrid != "True":
+            SUBSCRIBE_ABLE = False
+            logger.warning(f"加载Poe配置时info:poe设定为未订阅,无法使用poe的订阅功能")
+    except Exception as e:
+        SUBSCRIBE_ABLE = False
+        logger.warning(f"加载Poe配置时info:poe设定为未订阅,无法使用poe的订阅功能")
+    try:
+        WHITE_LIST += config.get_config(source="Poe配置", config_name="whitelist")
+    except Exception as e:
+        logger.warning(f"加载Poe配置时warn:{str(e)},订阅功能白名单用户无法正常获取")
+
 
 load_config()
 
 
 class Poe_Bot:
     def __init__(
-            self, common_userinfo: CommonUserInfo, bot_info: BotInfo, bot_data: BotData
+            self, common_userinfo: CommonUserInfo, bot_info: BotInfo, bot_data: BotData,
     ):
         self.lock = asyncio.Lock()
         self.nickname = bot_info.nickname
         self.common_userinfo = common_userinfo
         self.botdata = bot_data
         self.source = bot_data.source
 
         if self.source == "poe claude":
             self.base_model = "a2"
-        else:
+        elif self.source == "poe chatgpt":
             self.base_model = "chinchilla"
+        elif self.source == "poe chatgpt4":
+            if not SUBSCRIBE_ABLE:
+                raise Exception("Poe账户未订阅,无法使用订阅功能")
+            if self.common_userinfo.user_id not in WHITE_LIST:
+                raise Exception("你不在poe订阅功能白名单内,无法使用订阅功能")
+            self.base_model = "beaver"
+        else:
+            if not SUBSCRIBE_ABLE:
+                raise Exception("Poe账户未订阅,无法使用订阅功能")
+            if self.common_userinfo.user_id not in WHITE_LIST:
+                raise Exception("你不在poe订阅功能白名单内,无法使用订阅功能")
+            self.base_model = "a2_2"
+
         if not COOKIE:
             raise Exception("Poe的配置cookie没有填写,无法使用")
 
     def __hash__(self) -> int:
         return hash((self.common_userinfo.user_id, self.nickname))
 
     async def ask(self, question: str):
+        if self.botdata.source == "poe chatgpt4" or self.botdata.source == "poe claude-2-100k":
+            if not SUBSCRIBE_ABLE:
+                raise Exception("Poe账户未订阅,无法使用订阅功能")
+            if not self.common_userinfo.user_id in WHITE_LIST:
+                raise Exception("你不在poe订阅功能白名单内,无法使用订阅功能")
         if self.botdata.prefix:
             question += self.botdata.prefix + "\n" + question
         if not self.botdata.handle:
             await self.refresh()
         try:
             answer = await self.chat(question)
 
             return answer
         except Exception as e:
             raise e
 
     async def refresh(self):
+        if self.botdata.source == "poe chatgpt4" or self.botdata.source == "poe claude-2-100k":
+            if not SUBSCRIBE_ABLE:
+                raise Exception("Poe账户未订阅,无法使用订阅功能")
+            if self.common_userinfo.user_id not in WHITE_LIST:
+                raise Exception("你不在poe订阅功能白名单内,无法使用订阅功能")
         if not self.botdata.handle:
             try:
                 await self.new_bot()
                 await self.chat(self.botdata.prompt)
             except Exception as e:
                 raise e
         else:
```

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/chatbot/slack_claude.py` & `nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/slack_claude.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/chatbot/spark_desk.py` & `nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/spark_desk.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/chatbot/sydneybing.py` & `nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/sydneybing.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/chatbot/tongyiqianwen.py` & `nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/tongyiqianwen.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/constants.py` & `nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/constants.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-import random
-import uuid
-
-DELIMITER = "\x1e"
-
-# Generate random IP between range 13.104.0.0/14
-FORWARDED_IP = f"1.0.0.{random.randint(0, 255)}"
-
-HEADERS = {
-    "accept": "application/json",
-    "accept-language": "en-US,en;q=0.9",
-    "content-type": "application/json",
-    "sec-ch-ua": '"Not_A Brand";v="99", Microsoft Edge";v="110", "Chromium";v="110"',
-    "sec-ch-ua-arch": '"x86"',
-    "sec-ch-ua-bitness": '"64"',
-    "sec-ch-ua-full-version": '"109.0.1518.78"',
-    "sec-ch-ua-full-version-list": '"Chromium";v="110.0.5481.192", "Not A(Brand";v="24.0.0.0", "Microsoft Edge";v="110.0.1587.69"',
-    "sec-ch-ua-mobile": "?0",
-    "sec-ch-ua-model": "",
-    "sec-ch-ua-platform": '"Windows"',
-    "sec-ch-ua-platform-version": '"15.0.0"',
-    "sec-fetch-dest": "empty",
-    "sec-fetch-mode": "cors",
-    "sec-fetch-site": "same-origin",
-    "x-ms-client-request-id": str(uuid.uuid4()),
-    "x-ms-useragent": "azsdk-js-api-client-factory/1.0.0-beta.1 core-rest-pipeline/1.10.0 OS/Win32",
-    "Referer": "https://www.bing.com/search?q=Bing+AI&showconv=1&FORM=hpcodx",
-    "Referrer-Policy": "origin-when-cross-origin",
-    "x-forwarded-for": FORWARDED_IP,
-}
-
-HEADERS_INIT_CONVER = {
-    "authority": "www.bing.com",
-    "accept": "application/json",
-    "accept-language": "en-US,en;q=0.9",
-    "cache-control": "max-age=0",
-    "sec-ch-ua": '"Chromium";v="110", "Not A(Brand";v="24", "Microsoft Edge";v="110"',
-    "sec-ch-ua-arch": '"x86"',
-    "sec-ch-ua-bitness": '"64"',
-    "sec-ch-ua-full-version": '"110.0.1587.69"',
-    "sec-ch-ua-full-version-list": '"Chromium";v="110.0.5481.192", "Not A(Brand";v="24.0.0.0", "Microsoft Edge";v="110.0.1587.69"',
-    "sec-ch-ua-mobile": "?0",
-    "sec-ch-ua-model": '""',
-    "sec-ch-ua-platform": '"Windows"',
-    "sec-ch-ua-platform-version": '"15.0.0"',
-    "upgrade-insecure-requests": "1",
-    "user-agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36 Edg/112.0.1722.46",
-    "x-edge-shopping-flag": "1",
-    "x-forwarded-for": FORWARDED_IP,
-}
+import random
+import uuid
+
+DELIMITER = "\x1e"
+
+# Generate random IP between range 13.104.0.0/14
+FORWARDED_IP = f"1.0.0.{random.randint(0, 255)}"
+
+HEADERS = {
+    "accept": "application/json",
+    "accept-language": "en-US,en;q=0.9",
+    "content-type": "application/json",
+    "sec-ch-ua": '"Not_A Brand";v="99", Microsoft Edge";v="110", "Chromium";v="110"',
+    "sec-ch-ua-arch": '"x86"',
+    "sec-ch-ua-bitness": '"64"',
+    "sec-ch-ua-full-version": '"109.0.1518.78"',
+    "sec-ch-ua-full-version-list": '"Chromium";v="110.0.5481.192", "Not A(Brand";v="24.0.0.0", "Microsoft Edge";v="110.0.1587.69"',
+    "sec-ch-ua-mobile": "?0",
+    "sec-ch-ua-model": "",
+    "sec-ch-ua-platform": '"Windows"',
+    "sec-ch-ua-platform-version": '"15.0.0"',
+    "sec-fetch-dest": "empty",
+    "sec-fetch-mode": "cors",
+    "sec-fetch-site": "same-origin",
+    "x-ms-client-request-id": str(uuid.uuid4()),
+    "x-ms-useragent": "azsdk-js-api-client-factory/1.0.0-beta.1 core-rest-pipeline/1.10.0 OS/Win32",
+    "Referer": "https://www.bing.com/search?q=Bing+AI&showconv=1&FORM=hpcodx",
+    "Referrer-Policy": "origin-when-cross-origin",
+    "x-forwarded-for": FORWARDED_IP,
+}
+
+HEADERS_INIT_CONVER = {
+    "authority": "www.bing.com",
+    "accept": "application/json",
+    "accept-language": "en-US,en;q=0.9",
+    "cache-control": "max-age=0",
+    "sec-ch-ua": '"Chromium";v="110", "Not A(Brand";v="24", "Microsoft Edge";v="110"',
+    "sec-ch-ua-arch": '"x86"',
+    "sec-ch-ua-bitness": '"64"',
+    "sec-ch-ua-full-version": '"110.0.1587.69"',
+    "sec-ch-ua-full-version-list": '"Chromium";v="110.0.5481.192", "Not A(Brand";v="24.0.0.0", "Microsoft Edge";v="110.0.1587.69"',
+    "sec-ch-ua-mobile": "?0",
+    "sec-ch-ua-model": '""',
+    "sec-ch-ua-platform": '"Windows"',
+    "sec-ch-ua-platform-version": '"15.0.0"',
+    "upgrade-insecure-requests": "1",
+    "user-agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36 Edg/112.0.1722.46",
+    "x-edge-shopping-flag": "1",
+    "x-forwarded-for": FORWARDED_IP,
+}
```

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/conversation.py` & `nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/conversation.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,122 +1,122 @@
-import json
-import os
-from typing import List
-from typing import Union
-
-import httpx
-
-from .constants import HEADERS_INIT_CONVER
-from .exceptions import NotAllowedToAccess
-
-
-class Conversation:
-    def __init__(
-            self,
-            proxy: Union[str, None] = None,
-            async_mode: bool = False,
-            cookies: Union[List[dict], None] = None,
-    ) -> None:
-        if async_mode:
-            return
-        self.struct: dict = {
-            "conversationId": None,
-            "clientId": None,
-            "conversationSignature": None,
-            "result": {"value": "Success", "message": None},
-        }
-        self.proxy = proxy
-        proxy = (
-                proxy
-                or os.environ.get("all_proxy")
-                or os.environ.get("ALL_PROXY")
-                or os.environ.get("https_proxy")
-                or os.environ.get("HTTPS_PROXY")
-                or None
-        )
-        if proxy is not None and proxy.startswith("socks5h://"):
-            proxy = "socks5://" + proxy[len("socks5h://"):]
-        self.session = httpx.Client(
-            proxies=proxy,
-            timeout=900,
-            headers=HEADERS_INIT_CONVER,
-        )
-        if cookies:
-            for cookie in cookies:
-                self.session.cookies.set(cookie["name"], cookie["value"])
-        # Send GET request
-        response = self.session.get(
-            url=os.environ.get("BING_PROXY_URL")
-                or "https://edgeservices.bing.com/edgesvc/turing/conversation/create",
-        )
-        if response.status_code != 200:
-            print(f"Status code: {response.status_code}")
-            print(response.text)
-            print(response.url)
-            raise Exception("Authentication failed")
-        try:
-            self.struct = response.json()
-        except (json.decoder.JSONDecodeError, NotAllowedToAccess) as exc:
-            raise Exception(
-                "Authentication failed. You have not been accepted into the beta.",
-            ) from exc
-        if self.struct["result"]["value"] == "UnauthorizedRequest":
-            raise NotAllowedToAccess(self.struct["result"]["message"])
-
-    @staticmethod
-    async def create(
-            proxy: Union[str, None] = None,
-            cookies: Union[List[dict], None] = None,
-    ) -> "Conversation":
-        self = Conversation(async_mode=True)
-        self.struct = {
-            "conversationId": None,
-            "clientId": None,
-            "conversationSignature": None,
-            "result": {"value": "Success", "message": None},
-        }
-        self.proxy = proxy
-        proxy = (
-                proxy
-                or os.environ.get("all_proxy")
-                or os.environ.get("ALL_PROXY")
-                or os.environ.get("https_proxy")
-                or os.environ.get("HTTPS_PROXY")
-                or None
-        )
-        if proxy is not None and proxy.startswith("socks5h://"):
-            proxy = "socks5://" + proxy[len("socks5h://"):]
-        transport = httpx.AsyncHTTPTransport(retries=900)
-        # Convert cookie format to httpx format
-        formatted_cookies = None
-        if cookies:
-            formatted_cookies = httpx.Cookies()
-            for cookie in cookies:
-                formatted_cookies.set(cookie["name"], cookie["value"])
-        async with httpx.AsyncClient(
-                proxies=proxy,
-                timeout=30,
-                headers=HEADERS_INIT_CONVER,
-                transport=transport,
-                cookies=formatted_cookies,
-        ) as client:
-            # Send GET request
-            response = await client.get(
-                url=os.environ.get("BING_PROXY_URL")
-                    or "https://www.bing.com/turing/conversation/create",
-                follow_redirects=True,
-            )
-        if response.status_code != 200:
-            print(f"Status code: {response.status_code}")
-            print(response.text)
-            print(response.url)
-            raise Exception("Authentication failed")
-        try:
-            self.struct = response.json()
-        except (json.decoder.JSONDecodeError, NotAllowedToAccess) as exc:
-            print(response.text)
-            raise Exception(
-                "Authentication failed. You have not been accepted into the beta.",
-            ) from exc
-        if self.struct["result"]["value"] == "UnauthorizedRequest":
-            raise NotAllowedToAccess(self.struct["result"]["message"])
-        return self
+import json
+import os
+from typing import List
+from typing import Union
+
+import httpx
+
+from .constants import HEADERS_INIT_CONVER
+from .exceptions import NotAllowedToAccess
+
+
+class Conversation:
+    def __init__(
+            self,
+            proxy: Union[str, None] = None,
+            async_mode: bool = False,
+            cookies: Union[List[dict], None] = None,
+    ) -> None:
+        if async_mode:
+            return
+        self.struct: dict = {
+            "conversationId": None,
+            "clientId": None,
+            "conversationSignature": None,
+            "result": {"value": "Success", "message": None},
+        }
+        self.proxy = proxy
+        proxy = (
+                proxy
+                or os.environ.get("all_proxy")
+                or os.environ.get("ALL_PROXY")
+                or os.environ.get("https_proxy")
+                or os.environ.get("HTTPS_PROXY")
+                or None
+        )
+        if proxy is not None and proxy.startswith("socks5h://"):
+            proxy = "socks5://" + proxy[len("socks5h://"):]
+        self.session = httpx.Client(
+            proxies=proxy,
+            timeout=900,
+            headers=HEADERS_INIT_CONVER,
+        )
+        if cookies:
+            for cookie in cookies:
+                self.session.cookies.set(cookie["name"], cookie["value"])
+        # Send GET request
+        response = self.session.get(
+            url=os.environ.get("BING_PROXY_URL")
+                or "https://edgeservices.bing.com/edgesvc/turing/conversation/create",
+        )
+        if response.status_code != 200:
+            print(f"Status code: {response.status_code}")
+            print(response.text)
+            print(response.url)
+            raise Exception("Authentication failed")
+        try:
+            self.struct = response.json()
+        except (json.decoder.JSONDecodeError, NotAllowedToAccess) as exc:
+            raise Exception(
+                "Authentication failed. You have not been accepted into the beta.",
+            ) from exc
+        if self.struct["result"]["value"] == "UnauthorizedRequest":
+            raise NotAllowedToAccess(self.struct["result"]["message"])
+
+    @staticmethod
+    async def create(
+            proxy: Union[str, None] = None,
+            cookies: Union[List[dict], None] = None,
+    ) -> "Conversation":
+        self = Conversation(async_mode=True)
+        self.struct = {
+            "conversationId": None,
+            "clientId": None,
+            "conversationSignature": None,
+            "result": {"value": "Success", "message": None},
+        }
+        self.proxy = proxy
+        proxy = (
+                proxy
+                or os.environ.get("all_proxy")
+                or os.environ.get("ALL_PROXY")
+                or os.environ.get("https_proxy")
+                or os.environ.get("HTTPS_PROXY")
+                or None
+        )
+        if proxy is not None and proxy.startswith("socks5h://"):
+            proxy = "socks5://" + proxy[len("socks5h://"):]
+        transport = httpx.AsyncHTTPTransport(retries=900)
+        # Convert cookie format to httpx format
+        formatted_cookies = None
+        if cookies:
+            formatted_cookies = httpx.Cookies()
+            for cookie in cookies:
+                formatted_cookies.set(cookie["name"], cookie["value"])
+        async with httpx.AsyncClient(
+                proxies=proxy,
+                timeout=30,
+                headers=HEADERS_INIT_CONVER,
+                transport=transport,
+                cookies=formatted_cookies,
+        ) as client:
+            # Send GET request
+            response = await client.get(
+                url=os.environ.get("BING_PROXY_URL")
+                    or "https://www.bing.com/turing/conversation/create",
+                follow_redirects=True,
+            )
+        if response.status_code != 200:
+            print(f"Status code: {response.status_code}")
+            print(response.text)
+            print(response.url)
+            raise Exception("Authentication failed")
+        try:
+            self.struct = response.json()
+        except (json.decoder.JSONDecodeError, NotAllowedToAccess) as exc:
+            print(response.text)
+            raise Exception(
+                "Authentication failed. You have not been accepted into the beta.",
+            ) from exc
+        if self.struct["result"]["value"] == "UnauthorizedRequest":
+            raise NotAllowedToAccess(self.struct["result"]["message"])
+        return self
```

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/EdgeUtils.py` & `nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/EdgeUtils.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,389 +1,389 @@
-import asyncio
-import contextlib
-import json
-import re
-from pathlib import Path
-
-from log2d import Log
-
-from .EdgeGPT import Chatbot, ConversationStyle
-from .ImageGen import ImageGen
-
-Log("BingChat")
-log = Log.BingChat.debug  # shortcut to create a log entry
-
-
-class Cookie:
-    """
-    Convenience class for Bing Cookie files, data, and configuration. This Class
-    is updated dynamically by the Query class to allow cycling through >1
-    cookie/credentials file e.g. when daily request limits (current 200 per
-    account per day) are exceeded.
-    """
-
-    current_file_index = 0
-    dir_path = Path.home().resolve() / "bing_cookies"
-    current_file_path = dir_path  # Avoid Path errors when no cookie file used
-    search_pattern = "bing_cookies_*.json"
-    ignore_files = set()
-    request_count = {}
-    supplied_files = set()
-    rotate_cookies = True
-
-    @classmethod
-    def files(cls: type) -> list[Path]:
-        """
-        Return a sorted list of all cookie files matching .search_pattern in
-        cls.dir_path, plus any supplied files, minus any ignored files.
-        """
-        all_files = set(Path(cls.dir_path).glob(cls.search_pattern))
-        if hasattr(cls, "supplied_files"):
-            supplied_files = {x for x in cls.supplied_files if x.is_file()}
-            all_files.update(supplied_files)
-        return sorted(all_files - cls.ignore_files)
-
-    @classmethod
-    def import_data(cls: type) -> None:
-        """
-        Read the active cookie file and populate the following attributes:
-
-          .current_file_path
-          .current_data
-          .image_token
-        """
-        if not cls.files():
-            log("No files in Cookie.dir_path")
-            return
-        try:
-            cls.current_file_path = cls.files()[cls.current_file_index]
-        except IndexError:
-            log(f"Invalid file index [{cls.current_file_index}]")
-            log("Files in Cookie.dir_path:")
-            for file in cls.files():
-                log(f"{file}")
-            return
-        log(f"Importing cookies from: {cls.current_file_path.name}")
-        with open(cls.current_file_path, encoding="utf-8") as file:
-            cls.current_data = json.load(file)
-        cls.image_token = [
-            x for x in cls.current_data if x.get("name").startswith("_U")
-        ]
-        cls.image_token = cls.image_token[0].get("value")
-
-    @classmethod
-    def import_next(cls: type, discard: bool = False) -> None:
-        """
-        Cycle through to the next cookies file then import it.
-
-        discard (bool): True -Mark the previous file to be ignored for the remainder of the current session.  Otherwise cycle through all available
-        cookie files (sharing the workload and 'resting' when not in use).
-        """
-        if not hasattr(cls, "current_file_path"):
-            cls.import_data()
-            return
-        with contextlib.suppress(AttributeError):
-            # Will fail on first instantiation because no current_file_path
-            if discard:
-                cls.ignore_files.add(cls.current_file_path)
-            else:
-                Cookie.current_file_index += 1
-        if Cookie.current_file_index >= len(cls.files()):
-            Cookie.current_file_index = 0
-        Cookie.import_data()
-
-
-class Query:
-    """
-    A convenience class that wraps around EdgeGPT.Chatbot to encapsulate input,
-    config, and output all together.  Relies on Cookie class for authentication
-    unless ignore_cookies=True
-    """
-
-    index = []
-    image_dir_path = Path.cwd().resolve() / "bing_images"
-
-    def __init__(
-            self,
-            prompt: str,
-            style: ConversationStyle = "precise",
-            content_type: str = "text",
-            cookie_files: set[Path] = None,
-            ignore_cookies: bool = False,
-            echo: bool = True,
-            echo_prompt: bool = False,
-            locale: str = "en-GB",
-            simplify_response: bool = True,
-    ) -> None:
-        """
-        Arguments:
-
-        prompt: Text to enter into Bing Chat
-        style: creative, balanced, or precise
-        content_type: "text" for Bing Chat; "image" for Dall-e
-        ignore_cookies (bool): Ignore cookie data altogether
-        echo: Print something to confirm request made
-        echo_prompt: Print confirmation of the evaluated prompt
-        simplify_response: True -> single simplified prompt/response exchange
-        cookie_files: iterable of Paths or strings of cookie files (json)
-
-        Files in Cookie.dir_path will also be used if they exist.  This defaults
-        to the current working directory, so set Cookie.dir_path before
-        creating a Query if your cookie files are elsewhere.
-        """
-        self.__class__.index += [self]
-        self.prompt = prompt
-        self.locale = locale
-        self.simplify_response = simplify_response
-        self.ignore_cookies = ignore_cookies
-        if not ignore_cookies:
-            if cookie_files:
-                # Convert singular argument to an iterable:
-                if isinstance(cookie_files, (str, Path)):
-                    cookie_files = {cookie_files}
-                # Check all elements exist and are Paths:
-                cookie_files = {
-                    Path(x).resolve()
-                    for x in cookie_files
-                    if isinstance(x, (str, Path)) and x
-                }
-                Cookie.supplied_files = cookie_files
-            files = Cookie.files()  # includes .supplied_files
-            if Cookie.rotate_cookies:
-                Cookie.import_next()
-            else:
-                Cookie.import_data()
-        if content_type == "text":
-            self.style = style
-            self.log_and_send_query(echo, echo_prompt)
-        if content_type == "image":
-            self.create_image()
-
-    def log_and_send_query(self, echo: bool, echo_prompt: bool) -> None:
-        self.response = asyncio.run(self.send_to_bing(echo, echo_prompt))
-        if not hasattr(Cookie, "current_data"):
-            name = "<no_cookies>"
-        else:
-            name = Cookie.current_file_path.name
-        if not Cookie.request_count.get(name):
-            Cookie.request_count[name] = 1
-        else:
-            Cookie.request_count[name] += 1
-
-    def create_image(self) -> None:
-        image_generator = ImageGen(Cookie.image_token)
-        image_generator.save_images(
-            image_generator.get_images(self.prompt),
-            output_dir=self.__class__.image_dir_path,
-        )
-
-    async def send_to_bing(self, echo: bool = True, echo_prompt: bool = False) -> str:
-        """Creat, submit, then close a Chatbot instance.  Return the response"""
-        retries = len(Cookie.files()) or 1
-        while retries:
-            if not hasattr(Cookie, "current_data"):
-                bot = await Chatbot.create()
-            else:
-                bot = await Chatbot.create(cookies=Cookie.current_data)
-            if echo_prompt:
-                log(f"{self.prompt=}")
-            if echo:
-                log("Waiting for response...")
-            if self.style.lower() not in "creative balanced precise".split():
-                self.style = "precise"
-            try:
-                return await bot.ask(
-                    prompt=self.prompt,
-                    conversation_style=getattr(ConversationStyle, self.style),
-                    simplify_response=self.simplify_response,
-                    locale=self.locale,
-                )
-            except Exception as ex:
-                log(
-                    f"Exception: [{Cookie.current_file_path.name} may have exceeded the daily limit]\n{ex}",
-                )
-                Cookie.import_next(discard=True)
-                retries -= 1
-            finally:
-                await bot.close()
-        return None
-
-    @property
-    def output(self) -> str:
-        """The response from a completed Chatbot request"""
-        if not self.simplify_response:
-            return [
-                x.get("text") or x.get("hiddenText")
-                for x in self.response["item"]["messages"]
-                if x["author"] == "bot"
-            ]
-        try:
-            return self.response["text"]
-        except TypeError as te:
-            raise TypeError(
-                f"{te}\n(No response received - probably rate throttled...)"
-            ) from te
-
-    @property
-    def sources(self) -> list[list[dict]]:
-        """The source names and details parsed from a completed Chatbot request"""
-        if self.simplify_response:
-            return self.response["sources_text"]
-        return [
-            x.get("sourceAttributions") or []
-            for x in self.response["item"]["messages"]
-            if x["author"] == "bot"
-        ]
-
-    @property
-    def sources_dict(self) -> dict[int, str]:
-        """The source names and details as a dictionary"""
-        if self.simplify_response:
-            text = self.response["sources_text"]
-            sources = enumerate(re.findall(r"\((http.*?)\)", text))
-            return {index + 1: value for index, value in sources}
-        all_sources = []
-        name = "providerDisplayName"
-        url = "seeMoreUrl"
-        for sources in self.sources:
-            if not sources:
-                continue
-            data = {
-                index + 1: source[url]
-                for index, source in enumerate(sources)
-                if name in source and url in source
-            }
-            all_sources += [data]
-        return all_sources
-
-    @property
-    def code_block_formats(self) -> list[str]:
-        """
-        Extract a list of programming languages/formats used in code blocks
-        """
-        regex = r"``` *(\b\w+\b\+*) *"
-        if self.simplify_response:
-            return re.findall(regex, self.output)
-        return re.findall(regex, "\n".join(self.output))
-
-    @property
-    def code_blocks(self) -> list[str]:
-        """
-        Return a list of code blocks (```) or snippets (`) as strings.
-
-        If the response contains a mix of snippets and code blocks, return the
-        code blocks only.
-
-        This method is not suitable if the main text response includes either of
-        the delimiters but not as part of an actual snippet or code block.
-
-        For example:
-        'In Markdown, the back-tick (`) is used to denote a code snippet'
-
-        """
-
-        final_blocks = []
-        if isinstance(self.output, str):  # I.e. simplify_response is True
-            separator = "```" if "```" in self.output else "`"
-            code_blocks = self.output.split(separator)[1:-1:2]
-            if separator == "`":
-                return code_blocks
-        else:
-            code_blocks = []
-            for response in self.output:
-                separator = "```" if "```" in response else "`"
-                code_blocks.extend(response.split(separator)[1:-1:2])
-            code_blocks = [x for x in code_blocks if x]
-        # Remove language name if present:
-        for block in code_blocks:
-            lines = block.splitlines()
-            code = lines[1:] if re.match(" *\\w+ *", lines[0]) else lines
-            final_blocks += ["\n".join(code).removeprefix(separator)]
-        return [x for x in final_blocks if x]
-
-    @property
-    def code(self) -> str:
-        """
-        Extract and join any snippets of code or formatted data in the response
-        """
-        return "\n\n".join(self.code_blocks)
-
-    @property
-    def suggestions(self) -> list[str]:
-        """Follow-on questions suggested by the Chatbot"""
-        if self.simplify_response:
-            return self.response["suggestions"]
-        try:
-            return [
-                x["text"]
-                for x in self.response["item"]["messages"][1]["suggestedResponses"]
-            ]
-        except KeyError:
-            return None
-
-    def __repr__(self) -> str:
-        return f"<EdgeGPT.Query: {self.prompt}>"
-
-    def __str__(self) -> str:
-        return self.output if self.simplify_response else "\n\n".join(self.output)
-
-
-class ImageQuery(Query):
-    def __init__(self, prompt: str, **kwargs) -> None:
-        kwargs["content_type"] = "image"
-        super().__init__(prompt, **kwargs)
-
-    def __repr__(self) -> str:
-        return f"<EdgeGPT.ImageQuery: {self.prompt}>"
-
-
-def test_cookie_rotation() -> None:
-    for i in range(1, 50):
-        q = Query(
-            f"What is {i} in Roman numerals?  Give the answer in JSON",
-            style="precise",
-        )
-        log(f"{i}: {Cookie.current_file_path.name}")
-        log(q.code)
-        log(f"Cookie count: {Cookie.request_count.get(Cookie.current_file_path.name)}")
-
-
-def test_features() -> Query:
-    try:
-        q = Query(
-            f"What is {i} in Roman numerals?  Give the answer in JSON", style="precise"
-        )
-        log(f"{i}: {Cookie.current_file_path.name}")
-        print(f"{Cookie.current_file_index=}")
-        print(f"{Cookie.current_file_path=}")
-        print(f"{Cookie.current_data=}")
-        print(f"{Cookie.dir_path=}")
-        print(f"{Cookie.search_pattern=}")
-        print(f"{Cookie.files()=}")
-        print(f"{Cookie.image_token=}")
-        print(f"{Cookie.import_next(discard=True)=}")
-        print(f"{Cookie.rotate_cookies=}")
-        print(f"{Cookie.files()=}")
-        print(f"{Cookie.ignore_files=}")
-        print(f"{Cookie.supplied_files=}")
-        print(
-            f"{Cookie.request_count=}")  # Keeps a tally of requests made in using each cookie file during this session
-        print(f"{q=}")
-        print(f"{q.prompt=}")
-        print(f"{q.ignore_cookies=}")
-        print(f"{q.style=}")
-        print(f"{q.simplify_response=}")
-        print(f"{q.locale=}")
-        print(f"{q.output=}")
-        print(q)
-        print(f"{q.sources=}")
-        print(f"{q.sources_dict=}")
-        print(f"{q.suggestions=}")
-        print(f"{q.code=}")  # All code as a single string
-        print(f"{q.code_blocks=}")  # Individual code blocks
-        print(f"{q.code_block_formats=}")  # The language/format of each code block (if given)
-        print(f"{Query.index=}")  # Keeps an index of Query objects created
-        print(f"{Query.image_dir_path=}")
-    except Exception as E:
-        raise Exception(E) from E
-    finally:
-        return q
+import asyncio
+import contextlib
+import json
+import re
+from pathlib import Path
+
+from log2d import Log
+
+from .EdgeGPT import Chatbot, ConversationStyle
+from .ImageGen import ImageGen
+
+Log("BingChat")
+log = Log.BingChat.debug  # shortcut to create a log entry
+
+
+class Cookie:
+    """
+    Convenience class for Bing Cookie files, data, and configuration. This Class
+    is updated dynamically by the Query class to allow cycling through >1
+    cookie/credentials file e.g. when daily request limits (current 200 per
+    account per day) are exceeded.
+    """
+
+    current_file_index = 0
+    dir_path = Path.home().resolve() / "bing_cookies"
+    current_file_path = dir_path  # Avoid Path errors when no cookie file used
+    search_pattern = "bing_cookies_*.json"
+    ignore_files = set()
+    request_count = {}
+    supplied_files = set()
+    rotate_cookies = True
+
+    @classmethod
+    def files(cls: type) -> list[Path]:
+        """
+        Return a sorted list of all cookie files matching .search_pattern in
+        cls.dir_path, plus any supplied files, minus any ignored files.
+        """
+        all_files = set(Path(cls.dir_path).glob(cls.search_pattern))
+        if hasattr(cls, "supplied_files"):
+            supplied_files = {x for x in cls.supplied_files if x.is_file()}
+            all_files.update(supplied_files)
+        return sorted(all_files - cls.ignore_files)
+
+    @classmethod
+    def import_data(cls: type) -> None:
+        """
+        Read the active cookie file and populate the following attributes:
+
+          .current_file_path
+          .current_data
+          .image_token
+        """
+        if not cls.files():
+            log("No files in Cookie.dir_path")
+            return
+        try:
+            cls.current_file_path = cls.files()[cls.current_file_index]
+        except IndexError:
+            log(f"Invalid file index [{cls.current_file_index}]")
+            log("Files in Cookie.dir_path:")
+            for file in cls.files():
+                log(f"{file}")
+            return
+        log(f"Importing cookies from: {cls.current_file_path.name}")
+        with open(cls.current_file_path, encoding="utf-8") as file:
+            cls.current_data = json.load(file)
+        cls.image_token = [
+            x for x in cls.current_data if x.get("name").startswith("_U")
+        ]
+        cls.image_token = cls.image_token[0].get("value")
+
+    @classmethod
+    def import_next(cls: type, discard: bool = False) -> None:
+        """
+        Cycle through to the next cookies file then import it.
+
+        discard (bool): True -Mark the previous file to be ignored for the remainder of the current session.  Otherwise cycle through all available
+        cookie files (sharing the workload and 'resting' when not in use).
+        """
+        if not hasattr(cls, "current_file_path"):
+            cls.import_data()
+            return
+        with contextlib.suppress(AttributeError):
+            # Will fail on first instantiation because no current_file_path
+            if discard:
+                cls.ignore_files.add(cls.current_file_path)
+            else:
+                Cookie.current_file_index += 1
+        if Cookie.current_file_index >= len(cls.files()):
+            Cookie.current_file_index = 0
+        Cookie.import_data()
+
+
+class Query:
+    """
+    A convenience class that wraps around EdgeGPT.Chatbot to encapsulate input,
+    config, and output all together.  Relies on Cookie class for authentication
+    unless ignore_cookies=True
+    """
+
+    index = []
+    image_dir_path = Path.cwd().resolve() / "bing_images"
+
+    def __init__(
+            self,
+            prompt: str,
+            style: ConversationStyle = "precise",
+            content_type: str = "text",
+            cookie_files: set[Path] = None,
+            ignore_cookies: bool = False,
+            echo: bool = True,
+            echo_prompt: bool = False,
+            locale: str = "en-GB",
+            simplify_response: bool = True,
+    ) -> None:
+        """
+        Arguments:
+
+        prompt: Text to enter into Bing Chat
+        style: creative, balanced, or precise
+        content_type: "text" for Bing Chat; "image" for Dall-e
+        ignore_cookies (bool): Ignore cookie data altogether
+        echo: Print something to confirm request made
+        echo_prompt: Print confirmation of the evaluated prompt
+        simplify_response: True -> single simplified prompt/response exchange
+        cookie_files: iterable of Paths or strings of cookie files (json)
+
+        Files in Cookie.dir_path will also be used if they exist.  This defaults
+        to the current working directory, so set Cookie.dir_path before
+        creating a Query if your cookie files are elsewhere.
+        """
+        self.__class__.index += [self]
+        self.prompt = prompt
+        self.locale = locale
+        self.simplify_response = simplify_response
+        self.ignore_cookies = ignore_cookies
+        if not ignore_cookies:
+            if cookie_files:
+                # Convert singular argument to an iterable:
+                if isinstance(cookie_files, (str, Path)):
+                    cookie_files = {cookie_files}
+                # Check all elements exist and are Paths:
+                cookie_files = {
+                    Path(x).resolve()
+                    for x in cookie_files
+                    if isinstance(x, (str, Path)) and x
+                }
+                Cookie.supplied_files = cookie_files
+            files = Cookie.files()  # includes .supplied_files
+            if Cookie.rotate_cookies:
+                Cookie.import_next()
+            else:
+                Cookie.import_data()
+        if content_type == "text":
+            self.style = style
+            self.log_and_send_query(echo, echo_prompt)
+        if content_type == "image":
+            self.create_image()
+
+    def log_and_send_query(self, echo: bool, echo_prompt: bool) -> None:
+        self.response = asyncio.run(self.send_to_bing(echo, echo_prompt))
+        if not hasattr(Cookie, "current_data"):
+            name = "<no_cookies>"
+        else:
+            name = Cookie.current_file_path.name
+        if not Cookie.request_count.get(name):
+            Cookie.request_count[name] = 1
+        else:
+            Cookie.request_count[name] += 1
+
+    def create_image(self) -> None:
+        image_generator = ImageGen(Cookie.image_token)
+        image_generator.save_images(
+            image_generator.get_images(self.prompt),
+            output_dir=self.__class__.image_dir_path,
+        )
+
+    async def send_to_bing(self, echo: bool = True, echo_prompt: bool = False) -> str:
+        """Creat, submit, then close a Chatbot instance.  Return the response"""
+        retries = len(Cookie.files()) or 1
+        while retries:
+            if not hasattr(Cookie, "current_data"):
+                bot = await Chatbot.create()
+            else:
+                bot = await Chatbot.create(cookies=Cookie.current_data)
+            if echo_prompt:
+                log(f"{self.prompt=}")
+            if echo:
+                log("Waiting for response...")
+            if self.style.lower() not in "creative balanced precise".split():
+                self.style = "precise"
+            try:
+                return await bot.ask(
+                    prompt=self.prompt,
+                    conversation_style=getattr(ConversationStyle, self.style),
+                    simplify_response=self.simplify_response,
+                    locale=self.locale,
+                )
+            except Exception as ex:
+                log(
+                    f"Exception: [{Cookie.current_file_path.name} may have exceeded the daily limit]\n{ex}",
+                )
+                Cookie.import_next(discard=True)
+                retries -= 1
+            finally:
+                await bot.close()
+        return None
+
+    @property
+    def output(self) -> str:
+        """The response from a completed Chatbot request"""
+        if not self.simplify_response:
+            return [
+                x.get("text") or x.get("hiddenText")
+                for x in self.response["item"]["messages"]
+                if x["author"] == "bot"
+            ]
+        try:
+            return self.response["text"]
+        except TypeError as te:
+            raise TypeError(
+                f"{te}\n(No response received - probably rate throttled...)"
+            ) from te
+
+    @property
+    def sources(self) -> list[list[dict]]:
+        """The source names and details parsed from a completed Chatbot request"""
+        if self.simplify_response:
+            return self.response["sources_text"]
+        return [
+            x.get("sourceAttributions") or []
+            for x in self.response["item"]["messages"]
+            if x["author"] == "bot"
+        ]
+
+    @property
+    def sources_dict(self) -> dict[int, str]:
+        """The source names and details as a dictionary"""
+        if self.simplify_response:
+            text = self.response["sources_text"]
+            sources = enumerate(re.findall(r"\((http.*?)\)", text))
+            return {index + 1: value for index, value in sources}
+        all_sources = []
+        name = "providerDisplayName"
+        url = "seeMoreUrl"
+        for sources in self.sources:
+            if not sources:
+                continue
+            data = {
+                index + 1: source[url]
+                for index, source in enumerate(sources)
+                if name in source and url in source
+            }
+            all_sources += [data]
+        return all_sources
+
+    @property
+    def code_block_formats(self) -> list[str]:
+        """
+        Extract a list of programming languages/formats used in code blocks
+        """
+        regex = r"``` *(\b\w+\b\+*) *"
+        if self.simplify_response:
+            return re.findall(regex, self.output)
+        return re.findall(regex, "\n".join(self.output))
+
+    @property
+    def code_blocks(self) -> list[str]:
+        """
+        Return a list of code blocks (```) or snippets (`) as strings.
+
+        If the response contains a mix of snippets and code blocks, return the
+        code blocks only.
+
+        This method is not suitable if the main text response includes either of
+        the delimiters but not as part of an actual snippet or code block.
+
+        For example:
+        'In Markdown, the back-tick (`) is used to denote a code snippet'
+
+        """
+
+        final_blocks = []
+        if isinstance(self.output, str):  # I.e. simplify_response is True
+            separator = "```" if "```" in self.output else "`"
+            code_blocks = self.output.split(separator)[1:-1:2]
+            if separator == "`":
+                return code_blocks
+        else:
+            code_blocks = []
+            for response in self.output:
+                separator = "```" if "```" in response else "`"
+                code_blocks.extend(response.split(separator)[1:-1:2])
+            code_blocks = [x for x in code_blocks if x]
+        # Remove language name if present:
+        for block in code_blocks:
+            lines = block.splitlines()
+            code = lines[1:] if re.match(" *\\w+ *", lines[0]) else lines
+            final_blocks += ["\n".join(code).removeprefix(separator)]
+        return [x for x in final_blocks if x]
+
+    @property
+    def code(self) -> str:
+        """
+        Extract and join any snippets of code or formatted data in the response
+        """
+        return "\n\n".join(self.code_blocks)
+
+    @property
+    def suggestions(self) -> list[str]:
+        """Follow-on questions suggested by the Chatbot"""
+        if self.simplify_response:
+            return self.response["suggestions"]
+        try:
+            return [
+                x["text"]
+                for x in self.response["item"]["messages"][1]["suggestedResponses"]
+            ]
+        except KeyError:
+            return None
+
+    def __repr__(self) -> str:
+        return f"<EdgeGPT.Query: {self.prompt}>"
+
+    def __str__(self) -> str:
+        return self.output if self.simplify_response else "\n\n".join(self.output)
+
+
+class ImageQuery(Query):
+    def __init__(self, prompt: str, **kwargs) -> None:
+        kwargs["content_type"] = "image"
+        super().__init__(prompt, **kwargs)
+
+    def __repr__(self) -> str:
+        return f"<EdgeGPT.ImageQuery: {self.prompt}>"
+
+
+def test_cookie_rotation() -> None:
+    for i in range(1, 50):
+        q = Query(
+            f"What is {i} in Roman numerals?  Give the answer in JSON",
+            style="precise",
+        )
+        log(f"{i}: {Cookie.current_file_path.name}")
+        log(q.code)
+        log(f"Cookie count: {Cookie.request_count.get(Cookie.current_file_path.name)}")
+
+
+def test_features() -> Query:
+    try:
+        q = Query(
+            f"What is {i} in Roman numerals?  Give the answer in JSON", style="precise"
+        )
+        log(f"{i}: {Cookie.current_file_path.name}")
+        print(f"{Cookie.current_file_index=}")
+        print(f"{Cookie.current_file_path=}")
+        print(f"{Cookie.current_data=}")
+        print(f"{Cookie.dir_path=}")
+        print(f"{Cookie.search_pattern=}")
+        print(f"{Cookie.files()=}")
+        print(f"{Cookie.image_token=}")
+        print(f"{Cookie.import_next(discard=True)=}")
+        print(f"{Cookie.rotate_cookies=}")
+        print(f"{Cookie.files()=}")
+        print(f"{Cookie.ignore_files=}")
+        print(f"{Cookie.supplied_files=}")
+        print(
+            f"{Cookie.request_count=}")  # Keeps a tally of requests made in using each cookie file during this session
+        print(f"{q=}")
+        print(f"{q.prompt=}")
+        print(f"{q.ignore_cookies=}")
+        print(f"{q.style=}")
+        print(f"{q.simplify_response=}")
+        print(f"{q.locale=}")
+        print(f"{q.output=}")
+        print(q)
+        print(f"{q.sources=}")
+        print(f"{q.sources_dict=}")
+        print(f"{q.suggestions=}")
+        print(f"{q.code=}")  # All code as a single string
+        print(f"{q.code_blocks=}")  # Individual code blocks
+        print(f"{q.code_block_formats=}")  # The language/format of each code block (if given)
+        print(f"{Query.index=}")  # Keeps an index of Query objects created
+        print(f"{Query.image_dir_path=}")
+    except Exception as E:
+        raise Exception(E) from E
+    finally:
+        return q
```

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/chatbot/utils/SydneyGPT/conversation_style.py` & `nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/SydneyGPT/conversation_style.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/chatbot/utils/SydneyGPT/SydneyGPT.py` & `nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/SydneyGPT/SydneyGPT.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/chatbot/utils/SydneyGPT/SydneyGPTUtils.py` & `nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/chatbot/utils/SydneyGPT/SydneyGPTUtils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/common/config.py` & `nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/common/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,14 +40,15 @@
         "claude_id",
         "slack_user_token",
         "XSRF_TOKEN",
         "pic_width",
         "public_command",
         "private_command",
         "wait_msg_able",
+        "subscribed"
     ],
 )
 
 
 class Config(BaseModel):
     path: Path = Field(None, description="配置文件的存储路径")
     config: dict = Field(None, description="配置文件的内容")
@@ -59,15 +60,15 @@
         self.config = {
             "总控配置": {
                 "superusers": "[]",
                 "pic_able": "Auto",
                 "url_able": "True",
                 "wait_msg_able": "True",
                 "num_limit": "500",
-                "pic_width": "1800",
+                "pic_width": "700",
                 "private_command": "/",
                 "public_command": ".",
             },
             "Newbing配置": {
                 "cookie": "",
                 "proxy": "",
                 "wss_link": "wss://sydney.bing.com/sydney/ChatHub",
@@ -92,14 +93,16 @@
                 "cookie": "",
                 "organization_uuid": "",
                 "proxy": "",
             },
             "Poe配置": {
                 "cookie": "",
                 "proxy": "",
+                "subscribed": "False",
+                "whitelist": "[""]"
             },
             "Bard配置": {
                 "__Secure-1PSID": "",
                 "proxy": "",
             },
             "通义千问配置": {
                 "cookie": "",
```

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/common/load_config.py` & `nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/common/load_config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/common/mytypes.py` & `nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/common/mytypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 from pydantic import BaseModel
 
 PLATFORM = Literal["OneBot V11", "Telegram", "Kaiheila", "Discord"]
 SOURCE = Literal[
     "poe chatgpt",
     "poe claude",
+    "poe chatgpt4",
+    "poe claude-2-100k",
     "chatgpt web",
     "slack claude",
     "claude ai",
     "spark desk",
     "bing",
     "sydneybing",
     "bard",
```

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/common/prefix_data.py` & `nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/common/prefix_data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/common/prompt_data.py` & `nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/common/prompt_data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/common/user_data.py` & `nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/common/user_data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/common/web/app.py` & `nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/common/web/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,16 @@
             "cookie": "获取方式为打开https://claude.ai和开发者工具中的网络,和claude进行对话,并在append_message的请求中获取请求头中的cookie",
             "organization_uuid": "获取方式为登陆后打开https://claude.ai/api/organizations,并复制uuid一项的值,填写在此处",
             "proxy": "访问POE官网时使用的代理链接,请按照协议://地址:端口的格式填写",
         },
         "Poe配置": {
             "cookie": "获取方式为打开https://poe.com/,登录后F12打开开发者工具,在应用程序->cookie中复制p-b项的值,如l_recO0QgugqEyfgMbBc-g%3D%3D",
             "proxy": "访问POE官网时使用的代理链接,请按照协议://地址:端口的格式填写",
+            "whitelist": "允许使用gpt4和claude2 100k的用户的列表,注意填写的是通用用户id,不是qq号或某平台id",
+            "subscribed": "账号是否为订阅账户,只有订阅账户才可使用gpt4 和 claude2 100k,否则将报错"
         },
         "Bard配置": {
             "__Secure-1PSID": "获取方式:打开Bard网页,打开开发者工具中的应用程序,选择其中的cookie,并且复制其中的__Secure-1PSID一项的值复制到这里",
             "proxy": "访问Bard官网时使用的代理链接,请按照协议://地址:端口的格式填写",
         },
         "通义千问配置": {
             "cookie": "获取方法为打开通义千问聊天界面,F12打开开发者工具的网络界面,提取其中的heartbeat请求的cookie的值",
```

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/common/web/data/spark_gpt/common/config.json` & `nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/common/web/data/spark_gpt/common/config.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/common/web/templates/config.html` & `nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/common/web/templates/config.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/common/web/templates/index.html` & `nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/common/web/templates/index.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/common/web/templates/prefix.html` & `nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/common/web/templates/prefix.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/common/web/templates/prompt.html` & `nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/common/web/templates/prompt.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/platforms/nonebot/bot_main.py` & `nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/platforms/nonebot/bot_main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/platforms/nonebot/config_main.py` & `nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/platforms/nonebot/config_main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/platforms/nonebot/userlinks.py` & `nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/platforms/nonebot/userlinks.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/platforms/nonebot/utils.py` & `nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/platforms/nonebot/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/platforms/temp_bots.py` & `nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/platforms/temp_bots.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,16 @@
     "bing": Newbing_Bot,
     "sydneybing": SydneyBing_Bot,
     "chatgpt web": ChatGPT_web_Bot,
     "slack claude": Slack_Claude_Bot,
     "claude ai": Claude_Bot,
     "poe chatgpt": Poe_Bot,
     "poe claude": Poe_Bot,
+    "poe claude-2-100k": Poe_Bot,
+    "poe chatgpt4": Poe_Bot,
     "bard": Bard_Bot,
     "通义千问": TongYiQianWen_Bot,
 }
 
 GET_HANDLERS = {
     OB11_Bot: lambda event: str(event.reply.message_id),
     TG_Bot: lambda event: str(event.reply_to_message.message_id + event.from_.id),
```

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/utils/render.py` & `nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/utils/render.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from pathlib import Path
 
 import aiofiles
 import markdown
-from nonebot import require
 from jinja2 import Environment, FileSystemLoader
+from nonebot import require
 
 require("nonebot_plugin_htmlrender")
 from nonebot_plugin_htmlrender import html_to_pic
 
 require("nonebot_plugin_templates")
 from nonebot_plugin_templates.templates_render import Font_Path
 
-
 TEMPLATES_PATH = Path(__file__).parent / "templates"
 env = Environment(
     extensions=["jinja2.ext.loopcontrols"],
     loader=FileSystemLoader(str(TEMPLATES_PATH)),
     enable_async=True,
 )
 text_template = env.get_template("markdown.html")
@@ -27,14 +26,16 @@
 
 
 async def read_tpl(path: str) -> str:
     return await read_file(f"{TEMPLATES_PATH}/{path}")
 
 
 async def md_to_pic(md: str, width: int = 600, font_path: str = Font_Path):
+    if md.count("```") % 2 == 1:
+        md += "  \n```"
     md = markdown.markdown(
         md,
         extensions=[
             "pymdownx.tasklist",
             "tables",
             "fenced_code",
             "codehilite",
@@ -55,13 +56,13 @@
             f"<script defer>{mathtex_js}</script>"
         )
 
     css = await read_tpl("markdown.css") + await read_tpl("pygments-default.css")
     html = await text_template.render_async(
         md=md, font_path=font_path, css=css, extra=extra
     )
-    with open(Path() / "temp.html", "w") as f:
-        f.write(html)
+    # with open(Path() / "temp.html", "w") as f:
+    #     f.write(html)
     return await html_to_pic(
         html=html,
         viewport={"width": width, "height": 10},
     )
```

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/utils/templates/katex/katex.min.b64_fonts.css` & `nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/utils/templates/katex/katex.min.b64_fonts.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/utils/templates/katex/katex.min.js` & `nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/utils/templates/katex/katex.min.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/utils/templates/katex/mathtex-script-type.min.js` & `nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/utils/templates/katex/mathtex-script-type.min.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/utils/templates/markdown.css` & `nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/utils/templates/markdown.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/utils/templates/markdown.html` & `nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/utils/templates/markdown.html`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
                 font-family: "Custom Font";
                 padding: 8px !important;
             }
         }
 
         .markdown-body::after {
             font-family: "Custom Font";
-            content: "Spark GPT 1.2.0";
+            content: "Spark GPT 1.2.1";
             font-size: 10px !important;
             font-weight: bold;
             color: black;
         }
     </style>
 </head>
```

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/utils/templates/pygments-default.css` & `nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/utils/templates/pygments-default.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.0/nonebot_plugin_spark_gpt/utils/utils.py` & `nonebot_plugin_spark_gpt-1.2.1/nonebot_plugin_spark_gpt/utils/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.0/pyproject.toml` & `nonebot_plugin_spark_gpt-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_spark_gpt"
-version = "1.2.0"
+version = "1.2.1"
 description = "Spark-GPT,将多种来源的gpt接入qq,TG,Kook,Discord及更多平台,提供webui进行实时配置热更新,效率高超,使用便捷,管理完善,功能强大"
 authors = ["canxin121 <1969730106@qq.com>"]
 readme = "README.md"
 packages = [{ include = "nonebot_plugin_spark_gpt"},{ include = "nonebot"}]
 
 [tool.poetry.dependencies]
 nonebot-adapter-onebot = "^2.2.1"
```

### Comparing `nonebot_plugin_spark_gpt-1.2.0/README.md` & `nonebot_plugin_spark_gpt-1.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     <img src="https://img.shields.io/badge/OneBot-v11-black?style=social&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEAAAABABAMAAABYR2ztAAAAIVBMVEUAAAAAAAADAwMHBwceHh4UFBQNDQ0ZGRkoKCgvLy8iIiLWSdWYAAAAAXRSTlMAQObYZgAAAQVJREFUSMftlM0RgjAQhV+0ATYK6i1Xb+iMd0qgBEqgBEuwBOxU2QDKsjvojQPvkJ/ZL5sXkgWrFirK4MibYUdE3OR2nEpuKz1/q8CdNxNQgthZCXYVLjyoDQftaKuniHHWRnPh2GCUetR2/9HsMAXyUT4/3UHwtQT2AggSCGKeSAsFnxBIOuAggdh3AKTL7pDuCyABcMb0aQP7aM4AnAbc/wHwA5D2wDHTTe56gIIOUA/4YYV2e1sg713PXdZJAuncdZMAGkAukU9OAn40O849+0ornPwT93rphWF0mgAbauUrEOthlX8Zu7P5A6kZyKCJy75hhw1Mgr9RAUvX7A3csGqZegEdniCx30c3agAAAABJRU5ErkJggg==" alt="onebot">
     <a href="https://github.com/canxin121/nonebot_poe_chat/releases/">
     <img src="https://img.shields.io/github/last-commit/canxin121/Spark-GPT" alt="github">
     </a>
 </p>
 <div align="left">
 
-## 最新版本号1.1.9
+## 最新版本号1.2.1
 # 详细教程-> [![残心文档库](source/doc.png)](https://canxin121.github.io/docs/docs/Spark_GPT.html)  
   
 ---
 # 介绍部分
 
 ## 功能特性
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
                 [https://socialify.git.ci/canxin121/Spark-GPT/
 image?font=Raleway&forks=1&issues=1&language=1&logo=https%3A%2F%2Fcanxin121.github.io%2Fdocs%2Flogo.png&name=1&owner=1&pattern=Charlie%20Brown&pulls=1&stargazers=1&theme=Auto]
                          ****** Spark-GPTä»åº ******
                                    Spark-GPT
                             [pypi] [python] [pypi]
                                [onebot]_[github]
-## ææ°çæ¬å·1.1.9 # è¯¦ç»æç¨-> [![æ®å¿ææ¡£åº](source/doc.png)]
+## ææ°çæ¬å·1.2.1 # è¯¦ç»æç¨-> [![æ®å¿ææ¡£åº](source/doc.png)]
 (https://canxin121.github.io/docs/docs/Spark_GPT.html) --- # ä»ç»é¨å ##
 åè½ç¹æ§ - æ±èä¼å¤æ¥æºçgpt(poe
 (chatgpt+claude),chatgptç½é¡µç,Newbing,slack
 claude,è®¯é£æç«,éä¹åé®),æ¯æå¤å¹³å°(tg,kook( åå¼é»å¦),qq
 (gocq),discord)ä½¿ç¨ä¸ä¸åå¹³å°ç¨æ·æ°æ®ç»å®äºé -
 æ¯æäººæ ¼é¢è®¾ååç¼ç³»ç»,æ¯ææè½¬å¾æè½¬é¾æ¥,æ¯ææ¯ä¸ªç¨æ·åå»ºä¸åæ¥æºä¸åäººæ ¼çbot,åæ¶æ¯æå¬ç¨å±åçbot
 -
```

### Comparing `nonebot_plugin_spark_gpt-1.2.0/PKG-INFO` & `nonebot_plugin_spark_gpt-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-spark-gpt
-Version: 1.2.0
+Version: 1.2.1
 Summary: Spark-GPT,将多种来源的gpt接入qq,TG,Kook,Discord及更多平台,提供webui进行实时配置热更新,效率高超,使用便捷,管理完善,功能强大
 Author: canxin121
 Author-email: 1969730106@qq.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -47,15 +47,15 @@
     <img src="https://img.shields.io/badge/OneBot-v11-black?style=social&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEAAAABABAMAAABYR2ztAAAAIVBMVEUAAAAAAAADAwMHBwceHh4UFBQNDQ0ZGRkoKCgvLy8iIiLWSdWYAAAAAXRSTlMAQObYZgAAAQVJREFUSMftlM0RgjAQhV+0ATYK6i1Xb+iMd0qgBEqgBEuwBOxU2QDKsjvojQPvkJ/ZL5sXkgWrFirK4MibYUdE3OR2nEpuKz1/q8CdNxNQgthZCXYVLjyoDQftaKuniHHWRnPh2GCUetR2/9HsMAXyUT4/3UHwtQT2AggSCGKeSAsFnxBIOuAggdh3AKTL7pDuCyABcMb0aQP7aM4AnAbc/wHwA5D2wDHTTe56gIIOUA/4YYV2e1sg713PXdZJAuncdZMAGkAukU9OAn40O849+0ornPwT93rphWF0mgAbauUrEOthlX8Zu7P5A6kZyKCJy75hhw1Mgr9RAUvX7A3csGqZegEdniCx30c3agAAAABJRU5ErkJggg==" alt="onebot">
     <a href="https://github.com/canxin121/nonebot_poe_chat/releases/">
     <img src="https://img.shields.io/github/last-commit/canxin121/Spark-GPT" alt="github">
     </a>
 </p>
 <div align="left">
 
-## 最新版本号1.1.9
+## 最新版本号1.2.1
 # 详细教程-> [![残心文档库](source/doc.png)](https://canxin121.github.io/docs/docs/Spark_GPT.html)  
   
 ---
 # 介绍部分
 
 ## 功能特性
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-spark-gpt Version: 1.2.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-spark-gpt Version: 1.2.1 Summary:
 Spark-
 GPT,å°å¤ç§æ¥æºçgptæ¥å¥qq,TG,Kook,Discordåæ´å¤å¹³å°,æä¾webuiè¿è¡å®æ¶éç½®ç­æ´æ°,æçé«è¶,ä½¿ç¨ä¾¿æ·,ç®¡çå®å,åè½å¼ºå¤§
 Author: canxin121 Author-email: 1969730106@qq.com Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Sydneygpt (==0.11.8) Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: bardapi (>=0.1.24,<0.2.0) Requires-Dist: bidict
@@ -18,15 +18,15 @@
 uvicorn (>=0.22.0,<0.23.0) Description-Content-Type: text/markdown
                 [https://socialify.git.ci/canxin121/Spark-GPT/
 image?font=Raleway&forks=1&issues=1&language=1&logo=https%3A%2F%2Fcanxin121.github.io%2Fdocs%2Flogo.png&name=1&owner=1&pattern=Charlie%20Brown&pulls=1&stargazers=1&theme=Auto]
                          ****** Spark-GPTä»åº ******
                                    Spark-GPT
                             [pypi] [python] [pypi]
                                [onebot]_[github]
-## ææ°çæ¬å·1.1.9 # è¯¦ç»æç¨-> [![æ®å¿ææ¡£åº](source/doc.png)]
+## ææ°çæ¬å·1.2.1 # è¯¦ç»æç¨-> [![æ®å¿ææ¡£åº](source/doc.png)]
 (https://canxin121.github.io/docs/docs/Spark_GPT.html) --- # ä»ç»é¨å ##
 åè½ç¹æ§ - æ±èä¼å¤æ¥æºçgpt(poe
 (chatgpt+claude),chatgptç½é¡µç,Newbing,slack
 claude,è®¯é£æç«,éä¹åé®),æ¯æå¤å¹³å°(tg,kook( åå¼é»å¦),qq
 (gocq),discord)ä½¿ç¨ä¸ä¸åå¹³å°ç¨æ·æ°æ®ç»å®äºé -
 æ¯æäººæ ¼é¢è®¾ååç¼ç³»ç»,æ¯ææè½¬å¾æè½¬é¾æ¥,æ¯ææ¯ä¸ªç¨æ·åå»ºä¸åæ¥æºä¸åäººæ ¼çbot,åæ¶æ¯æå¬ç¨å±åçbot
 -
```

