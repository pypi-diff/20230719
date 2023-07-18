# Comparing `tmp/khoj_assistant-0.8.3.dev42.tar.gz` & `tmp/khoj_assistant-0.8.3.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Tue Jul 18 23:43:17 2023, max compression
+gzip compressed data, last modified: Thu Jul 13 05:22:49 2023, max compression
```

## Comparing `khoj_assistant-0.8.3.dev42.tar` & `khoj_assistant-0.8.3.dev8.tar`

### file list

```diff
@@ -1,82 +1,81 @@
--rw-r--r--   0        0        0        0 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/__init__.py
--rw-r--r--   0        0        0    13939 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/configure.py
--rw-r--r--   0        0        0     5316 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/main.py
--rw-r--r--   0        0        0        0 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/interface/desktop/__init__.py
--rw-r--r--   0        0        0     2355 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/interface/desktop/main_window.py
--rw-r--r--   0        0        0     1397 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/interface/desktop/system_tray.py
--rw-r--r--   0        0        0      582 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/interface/web/404.html
--rw-r--r--   0        0        0     5144 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/interface/web/base_config.html
--rw-r--r--   0        0        0      657 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/interface/web/base_processor_integration.html
--rw-r--r--   0        0        0    18018 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/interface/web/chat.html
--rw-r--r--   0        0        0    19687 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/interface/web/config.html
--rw-r--r--   0        0        0     7089 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/interface/web/content_type_github_input.html
--rw-r--r--   0        0        0     7322 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/interface/web/content_type_input.html
--rw-r--r--   0        0        0     3560 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/interface/web/content_type_notion_input.html
--rw-r--r--   0        0        0    18924 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/interface/web/index.html
--rw-r--r--   0        0        0      402 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/interface/web/khoj.webmanifest
--rw-r--r--   0        0        0      418 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/interface/web/khoj_chat.webmanifest
--rw-r--r--   0        0        0     3660 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/interface/web/processor_conversation_input.html
--rw-r--r--   0        0        0     2433 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/interface/web/assets/khoj.css
--rw-r--r--   0        0        0   275822 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/interface/web/assets/markdown-it.min.js
--rw-r--r--   0        0        0    58643 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/interface/web/assets/org.min.js
--rw-r--r--   0        0        0    73572 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/interface/web/assets/pico.min.css
--rw-r--r--   0        0        0    51584 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/interface/web/assets/icons/chat.svg
--rw-r--r--   0        0        0      549 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/interface/web/assets/icons/confirm-icon.svg
--rw-r--r--   0        0        0   205167 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/interface/web/assets/icons/favicon-128x128.ico
--rw-r--r--   0        0        0    12518 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/interface/web/assets/icons/favicon-128x128.png
--rw-r--r--   0        0        0    31531 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/interface/web/assets/icons/favicon.icns
--rw-r--r--   0        0        0      964 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/interface/web/assets/icons/github.svg
--rw-r--r--   0        0        0    13011 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
--rw-r--r--   0        0        0  1301428 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
--rw-r--r--   0        0        0     4031 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/interface/web/assets/icons/logotype.svg
--rw-r--r--   0        0        0      283 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/interface/web/assets/icons/markdown.svg
--rw-r--r--   0        0        0     1578 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/interface/web/assets/icons/notion.svg
--rw-r--r--   0        0        0     7946 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/interface/web/assets/icons/org.svg
--rw-r--r--   0        0        0     2504 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/interface/web/assets/icons/pdf.svg
--rw-r--r--   0        0        0     1877 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/interface/web/assets/icons/question-mark-icon.svg
--rw-r--r--   0        0        0        0 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/processor/__init__.py
--rw-r--r--   0        0        0     4788 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/processor/text_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/processor/conversation/__init__.py
--rw-r--r--   0        0        0     4824 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/processor/conversation/gpt.py
--rw-r--r--   0        0        0     3991 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/processor/conversation/prompts.py
--rw-r--r--   0        0        0     8304 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/processor/conversation/utils.py
--rw-r--r--   0        0        0        0 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/processor/github/__init__.py
--rw-r--r--   0        0        0    13274 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/processor/github/github_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/processor/jsonl/__init__.py
--rw-r--r--   0        0        0     3578 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/processor/jsonl/jsonl_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/processor/markdown/__init__.py
--rw-r--r--   0        0        0     7156 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/processor/markdown/markdown_to_jsonl.py
--rw-r--r--   0        0        0     9578 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/processor/notion/notion_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/processor/org_mode/__init__.py
--rw-r--r--   0        0        0     7190 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/processor/org_mode/org_to_jsonl.py
--rw-r--r--   0        0        0    16881 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/processor/org_mode/orgnode.py
--rw-r--r--   0        0        0        0 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/processor/pdf/__init__.py
--rw-r--r--   0        0        0     5099 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/processor/pdf/pdf_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/routers/__init__.py
--rw-r--r--   0        0        0    23782 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/routers/api.py
--rw-r--r--   0        0        0      167 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/routers/api_beta.py
--rw-r--r--   0        0        0     3657 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/routers/helpers.py
--rw-r--r--   0        0        0     6674 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/routers/web_client.py
--rw-r--r--   0        0        0        0 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/search_filter/__init__.py
--rw-r--r--   0        0        0      539 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/search_filter/base_filter.py
--rw-r--r--   0        0        0     7566 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/search_filter/date_filter.py
--rw-r--r--   0        0        0     2844 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/search_filter/file_filter.py
--rw-r--r--   0        0        0     3770 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/search_filter/word_filter.py
--rw-r--r--   0        0        0        0 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/search_type/__init__.py
--rw-r--r--   0        0        0    11434 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/search_type/image_search.py
--rw-r--r--   0        0        0    11134 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/search_type/text_search.py
--rw-r--r--   0        0        0        0 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/utils/__init__.py
--rw-r--r--   0        0        0     2619 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/utils/cli.py
--rw-r--r--   0        0        0     2303 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/utils/config.py
--rw-r--r--   0        0        0     2710 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/utils/constants.py
--rw-r--r--   0        0        0     6937 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/utils/helpers.py
--rw-r--r--   0        0        0     1233 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/utils/jsonl.py
--rw-r--r--   0        0        0     2463 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/utils/models.py
--rw-r--r--   0        0        0     4393 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/utils/rawconfig.py
--rw-r--r--   0        0        0     1113 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/utils/state.py
--rw-r--r--   0        0        0     1486 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/src/khoj/utils/yaml.py
--rw-r--r--   0        0        0      523 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/.gitignore
--rw-r--r--   0        0        0    32472 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/LICENSE
--rw-r--r--   0        0        0    24858 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/README.md
--rw-r--r--   0        0        0     2794 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/pyproject.toml
--rw-r--r--   0        0        0    27225 2023-07-18 23:43:17.000000 khoj_assistant-0.8.3.dev42/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/__init__.py
+-rw-r--r--   0        0        0    11626 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/configure.py
+-rw-r--r--   0        0        0     5515 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/main.py
+-rw-r--r--   0        0        0        0 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/desktop/__init__.py
+-rw-r--r--   0        0        0     2049 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/desktop/main_window.py
+-rw-r--r--   0        0        0     1395 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/desktop/system_tray.py
+-rw-r--r--   0        0        0      582 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/404.html
+-rw-r--r--   0        0        0     4897 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/base_config.html
+-rw-r--r--   0        0        0      657 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/base_processor_integration.html
+-rw-r--r--   0        0        0    18018 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/chat.html
+-rw-r--r--   0        0        0    16252 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/config.html
+-rw-r--r--   0        0        0     6930 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/content_type_github_input.html
+-rw-r--r--   0        0        0     7322 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/content_type_input.html
+-rw-r--r--   0        0        0     3401 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/content_type_notion_input.html
+-rw-r--r--   0        0        0    18924 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/index.html
+-rw-r--r--   0        0        0      402 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/khoj.webmanifest
+-rw-r--r--   0        0        0      418 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/khoj_chat.webmanifest
+-rw-r--r--   0        0        0     3660 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/processor_conversation_input.html
+-rw-r--r--   0        0        0     2433 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/khoj.css
+-rw-r--r--   0        0        0   275822 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/markdown-it.min.js
+-rw-r--r--   0        0        0    58643 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/org.min.js
+-rw-r--r--   0        0        0    73572 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/pico.min.css
+-rw-r--r--   0        0        0    51584 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/chat.svg
+-rw-r--r--   0        0        0      549 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/confirm-icon.svg
+-rw-r--r--   0        0        0   205167 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/favicon-128x128.ico
+-rw-r--r--   0        0        0    12518 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/favicon-128x128.png
+-rw-r--r--   0        0        0    31531 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/favicon.icns
+-rw-r--r--   0        0        0      964 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/github.svg
+-rw-r--r--   0        0        0    13011 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
+-rw-r--r--   0        0        0  1301428 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
+-rw-r--r--   0        0        0     4031 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/logotype.svg
+-rw-r--r--   0        0        0      283 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/markdown.svg
+-rw-r--r--   0        0        0     1578 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/notion.svg
+-rw-r--r--   0        0        0     7946 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/org.svg
+-rw-r--r--   0        0        0     2504 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/pdf.svg
+-rw-r--r--   0        0        0        0 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/processor/__init__.py
+-rw-r--r--   0        0        0     4455 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/processor/text_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/processor/conversation/__init__.py
+-rw-r--r--   0        0        0     4824 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/processor/conversation/gpt.py
+-rw-r--r--   0        0        0     3991 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/processor/conversation/prompts.py
+-rw-r--r--   0        0        0     8304 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/processor/conversation/utils.py
+-rw-r--r--   0        0        0        0 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/processor/github/__init__.py
+-rw-r--r--   0        0        0    13517 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/processor/github/github_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/processor/jsonl/__init__.py
+-rw-r--r--   0        0        0     3937 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/processor/jsonl/jsonl_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/processor/markdown/__init__.py
+-rw-r--r--   0        0        0     7454 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/processor/markdown/markdown_to_jsonl.py
+-rw-r--r--   0        0        0     9295 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/processor/notion/notion_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/processor/org_mode/__init__.py
+-rw-r--r--   0        0        0     7259 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/processor/org_mode/org_to_jsonl.py
+-rw-r--r--   0        0        0    16881 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/processor/org_mode/orgnode.py
+-rw-r--r--   0        0        0        0 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/processor/pdf/__init__.py
+-rw-r--r--   0        0        0     5397 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/processor/pdf/pdf_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/routers/__init__.py
+-rw-r--r--   0        0        0    20526 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/routers/api.py
+-rw-r--r--   0        0        0      167 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/routers/api_beta.py
+-rw-r--r--   0        0        0     2895 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/routers/helpers.py
+-rw-r--r--   0        0        0     5524 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/routers/web_client.py
+-rw-r--r--   0        0        0        0 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/search_filter/__init__.py
+-rw-r--r--   0        0        0      539 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/search_filter/base_filter.py
+-rw-r--r--   0        0        0     7566 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/search_filter/date_filter.py
+-rw-r--r--   0        0        0     2844 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/search_filter/file_filter.py
+-rw-r--r--   0        0        0     3770 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/search_filter/word_filter.py
+-rw-r--r--   0        0        0        0 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/search_type/__init__.py
+-rw-r--r--   0        0        0    11381 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/search_type/image_search.py
+-rw-r--r--   0        0        0    11237 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/search_type/text_search.py
+-rw-r--r--   0        0        0        0 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/utils/__init__.py
+-rw-r--r--   0        0        0     2042 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/utils/cli.py
+-rw-r--r--   0        0        0     2571 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/utils/config.py
+-rw-r--r--   0        0        0     2710 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/utils/constants.py
+-rw-r--r--   0        0        0     6889 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/utils/helpers.py
+-rw-r--r--   0        0        0     1607 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/utils/jsonl.py
+-rw-r--r--   0        0        0     2463 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/utils/models.py
+-rw-r--r--   0        0        0     4338 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/utils/rawconfig.py
+-rw-r--r--   0        0        0     1066 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/utils/state.py
+-rw-r--r--   0        0        0     1486 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/src/khoj/utils/yaml.py
+-rw-r--r--   0        0        0      523 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/.gitignore
+-rw-r--r--   0        0        0    32472 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/LICENSE
+-rw-r--r--   0        0        0    24858 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/README.md
+-rw-r--r--   0        0        0     2792 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/pyproject.toml
+-rw-r--r--   0        0        0    27222 2023-07-13 05:22:49.000000 khoj_assistant-0.8.3.dev8/PKG-INFO
```

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/configure.py` & `khoj_assistant-0.8.3.dev8/src/khoj/configure.py`

 * *Files 23% similar despite different names*

```diff
@@ -16,88 +16,48 @@
 from khoj.processor.markdown.markdown_to_jsonl import MarkdownToJsonl
 from khoj.processor.org_mode.org_to_jsonl import OrgToJsonl
 from khoj.processor.pdf.pdf_to_jsonl import PdfToJsonl
 from khoj.processor.github.github_to_jsonl import GithubToJsonl
 from khoj.processor.notion.notion_to_jsonl import NotionToJsonl
 from khoj.search_type import image_search, text_search
 from khoj.utils import constants, state
-from khoj.utils.config import (
-    ContentIndex,
-    SearchType,
-    SearchModels,
-    ProcessorConfigModel,
-    ConversationProcessorConfigModel,
-)
+from khoj.utils.config import SearchType, SearchModels, ProcessorConfigModel, ConversationProcessorConfigModel
 from khoj.utils.helpers import LRU, resolve_absolute_path, merge_dicts
-from khoj.utils.rawconfig import FullConfig, ProcessorConfig, SearchConfig, ContentConfig
+from khoj.utils.rawconfig import FullConfig, ProcessorConfig
 from khoj.search_filter.date_filter import DateFilter
 from khoj.search_filter.word_filter import WordFilter
 from khoj.search_filter.file_filter import FileFilter
 
 
 logger = logging.getLogger(__name__)
 
 
-def initialize_server(
-    config: Optional[FullConfig], regenerate: bool, type: Optional[SearchType] = None, required=False
-):
-    if config is None and required:
-        logger.error(
-            f"🚨 Exiting as Khoj is not configured.\nConfigure it via http://localhost:42110/config or by editing {state.config_file}."
-        )
-        sys.exit(1)
-    elif config is None:
-        logger.warning(
-            f"🚨 Khoj is not configured.\nConfigure it via http://localhost:42110/config, plugins or by editing {state.config_file}."
-        )
-        return None
-
-    try:
-        configure_server(config, regenerate, type)
-    except Exception as e:
-        logger.error(f"🚨 Failed to configure server on app load: {e}", exc_info=True)
-
-
-def configure_server(config: FullConfig, regenerate: bool, search_type: Optional[SearchType] = None):
-    # Update Config
-    state.config = config
+def configure_server(args, required=False):
+    if args.config is None:
+        if required:
+            logger.error(
+                f"Exiting as Khoj is not configured.\nConfigure it via http://localhost:42110/config or by editing {state.config_file}."
+            )
+            sys.exit(1)
+        else:
+            logger.warning(
+                f"Khoj is not configured.\nConfigure it via http://localhost:42110/config, plugins or by editing {state.config_file}."
+            )
+            return
+    else:
+        state.config = args.config
 
     # Initialize Processor from Config
-    try:
-        state.config_lock.acquire()
-        state.processor_config = configure_processor(state.config.processor)
-    except Exception as e:
-        logger.error(f"🚨 Failed to configure processor")
-        raise e
-    finally:
-        state.config_lock.release()
+    state.processor_config = configure_processor(args.config.processor)
 
-    # Initialize Search Models from Config
-    try:
-        state.config_lock.acquire()
-        state.SearchType = configure_search_types(state.config)
-        state.search_models = configure_search(state.search_models, state.config.search_type)
-    except Exception as e:
-        logger.error(f"🚨 Failed to configure search models")
-        raise e
-    finally:
-        state.config_lock.release()
-
-    # Initialize Content from Config
-    if state.search_models:
-        try:
-            state.config_lock.acquire()
-            state.content_index = configure_content(
-                state.content_index, state.config.content_type, state.search_models, regenerate, search_type
-            )
-        except Exception as e:
-            logger.error(f"🚨 Failed to index content")
-            raise e
-        finally:
-            state.config_lock.release()
+    # Initialize the search type and model from Config
+    state.search_index_lock.acquire()
+    state.SearchType = configure_search_types(state.config)
+    state.model = configure_search(state.model, state.config, args.regenerate)
+    state.search_index_lock.release()
 
 
 def configure_routes(app):
     # Import APIs here to setup search types before while configuring server
     from khoj.routers.api import api
     from khoj.routers.api_beta import api_beta
     from khoj.routers.web_client import web_client
@@ -108,166 +68,137 @@
     app.include_router(web_client)
 
 
 if not state.demo:
 
     @schedule.repeat(schedule.every(61).minutes)
     def update_search_index():
-        try:
-            state.config_lock.acquire()
-            state.content_index = configure_content(
-                state.content_index, state.config.content_type, state.search_models, regenerate=False
-            )
-            logger.info("📬 Content index updated via Scheduler")
-        except Exception as e:
-            logger.error(f"🚨 Error updating content index via Scheduler: {e}")
-        finally:
-            state.config_lock.release()
+        state.search_index_lock.acquire()
+        state.model = configure_search(state.model, state.config, regenerate=False)
+        state.search_index_lock.release()
+        logger.info("📬 Search index updated via Scheduler")
 
 
 def configure_search_types(config: FullConfig):
     # Extract core search types
     core_search_types = {e.name: e.value for e in SearchType}
     # Extract configured plugin search types
     plugin_search_types = {}
     if config.content_type and config.content_type.plugins:
         plugin_search_types = {plugin_type: plugin_type for plugin_type in config.content_type.plugins.keys()}
 
     # Dynamically generate search type enum by merging core search types with configured plugin search types
     return Enum("SearchType", merge_dicts(core_search_types, plugin_search_types))
 
 
-def configure_search(search_models: SearchModels, search_config: Optional[SearchConfig]) -> Optional[SearchModels]:
-    # Run Validation Checks
-    if search_config is None:
-        logger.warning("🚨 No Search configuration available.")
-        return None
-    if search_models is None:
-        search_models = SearchModels()
-
-    # Initialize Search Models
-    if search_config.asymmetric:
-        logger.info("🔍 📜 Setting up text search model")
-        search_models.text_search = text_search.initialize_model(search_config.asymmetric)
-
-    if search_config.image:
-        logger.info("🔍 🌄 Setting up image search model")
-        search_models.image_search = image_search.initialize_model(search_config.image)
-
-    return search_models
-
-
-def configure_content(
-    content_index: Optional[ContentIndex],
-    content_config: Optional[ContentConfig],
-    search_models: SearchModels,
-    regenerate: bool,
-    t: Optional[state.SearchType] = None,
-) -> Optional[ContentIndex]:
-    # Run Validation Checks
-    if content_config is None:
-        logger.warning("🚨 No Content configuration available.")
-        return None
-    if content_index is None:
-        content_index = ContentIndex()
+def configure_search(model: SearchModels, config: FullConfig, regenerate: bool, t: Optional[state.SearchType] = None):
+    if config is None or config.content_type is None or config.search_type is None:
+        logger.warning("🚨 No Content or Search type is configured.")
+        return
+
+    if model is None:
+        model = SearchModels()
 
     try:
         # Initialize Org Notes Search
-        if (t == state.SearchType.Org or t == None) and content_config.org and search_models.text_search:
+        if (t == state.SearchType.Org or t == None) and config.content_type.org and config.search_type.asymmetric:
             logger.info("🦄 Setting up search for orgmode notes")
             # Extract Entries, Generate Notes Embeddings
-            content_index.org = text_search.setup(
+            model.org_search = text_search.setup(
                 OrgToJsonl,
-                content_config.org,
-                search_models.text_search.bi_encoder,
+                config.content_type.org,
+                search_config=config.search_type.asymmetric,
                 regenerate=regenerate,
                 filters=[DateFilter(), WordFilter(), FileFilter()],
             )
 
         # Initialize Markdown Search
-        if (t == state.SearchType.Markdown or t == None) and content_config.markdown and search_models.text_search:
+        if (
+            (t == state.SearchType.Markdown or t == None)
+            and config.content_type.markdown
+            and config.search_type.asymmetric
+        ):
             logger.info("💎 Setting up search for markdown notes")
             # Extract Entries, Generate Markdown Embeddings
-            content_index.markdown = text_search.setup(
+            model.markdown_search = text_search.setup(
                 MarkdownToJsonl,
-                content_config.markdown,
-                search_models.text_search.bi_encoder,
+                config.content_type.markdown,
+                search_config=config.search_type.asymmetric,
                 regenerate=regenerate,
                 filters=[DateFilter(), WordFilter(), FileFilter()],
             )
 
         # Initialize PDF Search
-        if (t == state.SearchType.Pdf or t == None) and content_config.pdf and search_models.text_search:
+        if (t == state.SearchType.Pdf or t == None) and config.content_type.pdf and config.search_type.asymmetric:
             logger.info("🖨️ Setting up search for pdf")
             # Extract Entries, Generate PDF Embeddings
-            content_index.pdf = text_search.setup(
+            model.pdf_search = text_search.setup(
                 PdfToJsonl,
-                content_config.pdf,
-                search_models.text_search.bi_encoder,
+                config.content_type.pdf,
+                search_config=config.search_type.asymmetric,
                 regenerate=regenerate,
                 filters=[DateFilter(), WordFilter(), FileFilter()],
             )
 
         # Initialize Image Search
-        if (t == state.SearchType.Image or t == None) and content_config.image and search_models.image_search:
+        if (t == state.SearchType.Image or t == None) and config.content_type.image and config.search_type.image:
             logger.info("🌄 Setting up search for images")
             # Extract Entries, Generate Image Embeddings
-            content_index.image = image_search.setup(
-                content_config.image, search_models.image_search.image_encoder, regenerate=regenerate
+            model.image_search = image_search.setup(
+                config.content_type.image, search_config=config.search_type.image, regenerate=regenerate
             )
 
-        if (t == state.SearchType.Github or t == None) and content_config.github and search_models.text_search:
+        if (t == state.SearchType.Github or t == None) and config.content_type.github and config.search_type.asymmetric:
             logger.info("🐙 Setting up search for github")
             # Extract Entries, Generate Github Embeddings
-            content_index.github = text_search.setup(
+            model.github_search = text_search.setup(
                 GithubToJsonl,
-                content_config.github,
-                search_models.text_search.bi_encoder,
+                config.content_type.github,
+                search_config=config.search_type.asymmetric,
                 regenerate=regenerate,
                 filters=[DateFilter(), WordFilter(), FileFilter()],
             )
 
         # Initialize External Plugin Search
-        if (t == None or t in state.SearchType) and content_config.plugins and search_models.text_search:
+        if (t == None or t in state.SearchType) and config.content_type.plugins:
             logger.info("🔌 Setting up search for plugins")
-            content_index.plugins = {}
-            for plugin_type, plugin_config in content_config.plugins.items():
-                content_index.plugins[plugin_type] = text_search.setup(
+            model.plugin_search = {}
+            for plugin_type, plugin_config in config.content_type.plugins.items():
+                model.plugin_search[plugin_type] = text_search.setup(
                     JsonlToJsonl,
                     plugin_config,
-                    search_models.text_search.bi_encoder,
+                    search_config=config.search_type.asymmetric,
                     regenerate=regenerate,
                     filters=[DateFilter(), WordFilter(), FileFilter()],
                 )
 
         # Initialize Notion Search
-        if (t == None or t in state.SearchType) and content_config.notion and search_models.text_search:
+        if (t == None or t in state.SearchType) and config.content_type.notion:
             logger.info("🔌 Setting up search for notion")
-            content_index.notion = text_search.setup(
+            model.notion_search = text_search.setup(
                 NotionToJsonl,
-                content_config.notion,
-                search_models.text_search.bi_encoder,
+                config.content_type.notion,
+                search_config=config.search_type.asymmetric,
                 regenerate=regenerate,
                 filters=[DateFilter(), WordFilter(), FileFilter()],
             )
 
     except Exception as e:
-        logger.error(f"🚨 Failed to setup search: {e}", exc_info=True)
+        logger.error("🚨 Failed to setup search")
         raise e
 
     # Invalidate Query Cache
     state.query_cache = LRU()
 
-    return content_index
+    return model
 
 
-def configure_processor(processor_config: Optional[ProcessorConfig]):
+def configure_processor(processor_config: ProcessorConfig):
     if not processor_config:
-        logger.warning("🚨 No Processor configuration available.")
-        return None
+        return
 
     processor = ProcessorConfigModel()
 
     # Initialize Conversation Processor
     if processor_config.conversation:
         logger.info("💬 Setting up conversation processor")
         processor.conversation = configure_conversation_processor(processor_config.conversation)
```

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/main.py` & `khoj_assistant-0.8.3.dev8/src/khoj/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,21 +17,26 @@
 # Ignore non-actionable warnings
 warnings.filterwarnings("ignore", message=r"snapshot_download.py has been made private", category=FutureWarning)
 warnings.filterwarnings("ignore", message=r"legacy way to download files from the HF hub,", category=FutureWarning)
 
 # External Packages
 import uvicorn
 from fastapi import FastAPI
+from PyQt6 import QtWidgets
+from PyQt6.QtCore import QThread, QTimer
 from rich.logging import RichHandler
 import schedule
 
 # Internal Packages
-from khoj.configure import configure_routes, initialize_server
+from khoj.configure import configure_routes, configure_server
 from khoj.utils import state
 from khoj.utils.cli import cli
+from khoj.interface.desktop.main_window import MainWindow
+from khoj.interface.desktop.system_tray import create_system_tray
+
 
 # Initialize the Application Server
 app = FastAPI()
 
 # Setup Logger
 rich_handler = RichHandler(rich_tracebacks=True)
 rich_handler.setFormatter(fmt=logging.Formatter(fmt="%(message)s", datefmt="[%X]"))
@@ -66,40 +71,35 @@
     logger.info("🌘 Starting Khoj")
 
     if not args.gui:
         # Setup task scheduler
         poll_task_scheduler()
 
         # Start Server
-        initialize_server(args.config, args.regenerate, required=False)
+        configure_server(args, required=False)
         configure_routes(app)
         start_server(app, host=args.host, port=args.port, socket=args.socket)
     else:
-        from PySide6 import QtWidgets
-        from PySide6.QtCore import QThread, QTimer
-        from khoj.interface.desktop.main_window import MainWindow, ServerThread
-        from khoj.interface.desktop.system_tray import create_system_tray
-
         # Setup GUI
         gui = QtWidgets.QApplication([])
         main_window = MainWindow(args.host, args.port)
 
         # System tray is only available on Windows, MacOS.
         # On Linux (Gnome) the System tray is not supported.
         # Since only the Main Window is available
         # Quitting it should quit the application
         if system() in ["Windows", "Darwin"]:
             gui.setQuitOnLastWindowClosed(False)
             tray = create_system_tray(gui, main_window)
             tray.show()
 
         # Setup Server
-        initialize_server(args.config, args.regenerate, required=False)
+        configure_server(args, required=False)
         configure_routes(app)
-        server = ServerThread(start_server_func=lambda: start_server(app, host=args.host, port=args.port))
+        server = ServerThread(app, args.host, args.port, args.socket)
 
         url = f"http://{args.host}:{args.port}"
         logger.info(f"🌗 Khoj is running at {url}")
         try:
             startup_url = url if args.config else f"{url}/config"
             webbrowser.open(startup_url)
         except:
@@ -132,16 +132,14 @@
             except:
                 pass
 
         gui.exec()
 
 
 def sigint_handler(*args):
-    from PySide6 import QtWidgets
-
     QtWidgets.QApplication.quit()
 
 
 def set_state(args):
     state.config_file = args.config_file
     state.config = args.config
     state.verbose = args.verbose
@@ -162,14 +160,29 @@
 def poll_task_scheduler():
     timer_thread = threading.Timer(60.0, poll_task_scheduler)
     timer_thread.daemon = True
     timer_thread.start()
     schedule.run_pending()
 
 
+class ServerThread(QThread):
+    def __init__(self, app, host=None, port=None, socket=None):
+        super(ServerThread, self).__init__()
+        self.app = app
+        self.host = host
+        self.port = port
+        self.socket = socket
+
+    def __del__(self):
+        self.wait()
+
+    def run(self):
+        start_server(self.app, self.host, self.port, self.socket)
+
+
 def run_gui():
     sys.argv += ["--gui"]
     run()
 
 
 if __name__ == "__main__":
     run_gui()
```

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/interface/desktop/main_window.py` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/desktop/main_window.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,16 @@
 # Standard Packages
 import webbrowser
 
 # External Packages
-from PySide6 import QtGui, QtWidgets
-from PySide6.QtCore import Qt
+from PyQt6 import QtGui, QtWidgets
+from PyQt6.QtCore import Qt
 
 # Internal Packages
 from khoj.utils import constants
-from PySide6.QtCore import QThread
-
-
-class ServerThread(QThread):
-    def __init__(self, start_server_func):
-        super(ServerThread, self).__init__()
-        self.start_server_func = start_server_func
-
-    def __del__(self):
-        self.wait()
-
-    def run(self):
-        self.start_server_func()
 
 
 class MainWindow(QtWidgets.QMainWindow):
     """Create Window to Navigate users to the web UI"""
 
     def __init__(self, host: str, port: int):
         super(MainWindow, self).__init__()
```

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/interface/desktop/system_tray.py` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/desktop/system_tray.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Standard Packages
 import webbrowser
 
 # External Packages
-from PySide6 import QtGui, QtWidgets
+from PyQt6 import QtGui, QtWidgets
 
 # Internal Packages
 from khoj.utils import constants, state
 from khoj.interface.desktop.main_window import MainWindow
 
 
 def create_system_tray(gui: QtWidgets.QApplication, main_window: MainWindow):
```

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/interface/web/404.html` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/404.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/interface/web/base_config.html` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/base_config.html`

 * *Files 6% similar despite different names*

```diff
@@ -47,18 +47,14 @@
             div.filler {
                 display: none;
             }
 
             body.khoj-configure {
                 padding: 0;
             }
-
-            div.section {
-                padding: 12px;
-            }
         }
 
         img.khoj-logo {
             max-width: none!important;
         }
         div.khoj-header-wrapper{
             display: grid;
@@ -69,19 +65,14 @@
             grid-auto-flow: row;
             gap: 32px;
         }
         .section {
             display: grid;
             justify-self: center;
         }
-
-        div.instructions {
-            font-size: large;
-        }
-
         .section-title {
             margin: 0;
             padding: 0 0 16px 0;
             font-size: 32;
             font-weight: normal;
         }
         .section-cards {
@@ -167,19 +158,14 @@
             text-align: left;
         }
 
         img.configured-icon {
             max-width: 16px;
         }
 
-        div.finalize-actions {
-            grid-auto-flow: column;
-            grid-gap: 24px;
-        }
-
         @media screen and (max-width: 600px) {
             .section-cards {
                 grid-template-columns: 1fr;
             }
         }
     </style>
 </html>
```

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/interface/web/base_processor_integration.html` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/base_processor_integration.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/interface/web/chat.html` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/chat.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/interface/web/config.html` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/config.html`

 * *Files 19% similar despite different names*

```diff
@@ -7,19 +7,15 @@
         <div class="section-cards">
             <div class="card">
                 <div class="card-title-row">
                     <img class="card-icon" src="/static/assets/icons/github.svg" alt="Github">
                     <h3 class="card-title">
                         Github
                         {% if current_config.content_type.github %}
-                            {% if current_model_state.github == False %}
-                                <img id="misconfigured-icon-github" class="configured-icon" src="/static/assets/icons/question-mark-icon.svg" alt="Not Configured" title="Embeddings have not been generated yet for this content type. Either the configuration is invalid, or you just need to click Configure.">
-                            {% else %}
-                                <img id="configured-icon-github" class="configured-icon" src="/static/assets/icons/confirm-icon.svg" alt="Configured">
-                            {% endif %}
+                            <img id="configured-icon-github" class="configured-icon" src="/static/assets/icons/confirm-icon.svg" alt="Configured">
                         {% endif %}
                     </h3>
                 </div>
                 <div class="card-description-row">
                 <p class="card-description">Set repositories for Khoj to index</p>
                 </div>
                 <div class="card-action-row">
@@ -42,19 +38,15 @@
             </div>
             <div class="card">
                 <div class="card-title-row">
                     <img class="card-icon" src="/static/assets/icons/notion.svg" alt="Notion">
                     <h3 class="card-title">
                         Notion
                         {% if current_config.content_type.notion %}
-                            {% if current_model_state.notion == False %}
-                                <img id="misconfigured-icon-notion" class="configured-icon" src="/static/assets/icons/question-mark-icon.svg" alt="Not Configured" title="Embeddings have not been generated yet for this content type. Either the configuration is invalid, or you just need to click Configure.">
-                            {% else %}
-                                <img id="configured-icon-notion" class="configured-icon" src="/static/assets/icons/confirm-icon.svg" alt="Configured">
-                            {% endif %}
+                            <img id="configured-icon-notion" class="configured-icon" src="/static/assets/icons/confirm-icon.svg" alt="Configured">
                         {% endif %}
                     </h3>
                 </div>
                 <div class="card-description-row">
                     <p class="card-description">Configure your settings from Notion</p>
                 </div>
                 <div class="card-action-row">
@@ -77,19 +69,15 @@
             </div>
             <div class="card">
                 <div class="card-title-row">
                     <img class="card-icon" src="/static/assets/icons/markdown.svg" alt="markdown">
                     <h3 class="card-title">
                         Markdown
                         {% if current_config.content_type.markdown %}
-                            {% if current_model_state.markdown == False%}
-                                <img id="misconfigured-icon-markdown" class="configured-icon" src="/static/assets/icons/question-mark-icon.svg" alt="Not Configured" title="Embeddings have not been generated yet for this content type. Either the configuration is invalid, or you just need to click Configure.">
-                            {% else %}
-                                <img id="configured-icon-markdown" class="configured-icon" src="/static/assets/icons/confirm-icon.svg" alt="Configured">
-                            {% endif %}
+                            <img id="configured-icon-markdown" class="configured-icon" src="/static/assets/icons/confirm-icon.svg" alt="Configured">
                         {% endif %}
                     </h3>
                 </div>
                 <div class="card-description-row">
                     <p class="card-description">Set markdown files for Khoj to index</p>
                 </div>
                 <div class="card-action-row">
@@ -112,19 +100,15 @@
             </div>
             <div class="card">
                 <div class="card-title-row">
                     <img class="card-icon" src="/static/assets/icons/org.svg" alt="org">
                     <h3 class="card-title">
                         Org
                         {% if current_config.content_type.org %}
-                            {% if current_model_state.org == False %}
-                                <img id="misconfigured-icon-org" class="configured-icon" src="/static/assets/icons/question-mark-icon.svg" alt="Not Configured" title="Embeddings have not been generated yet for this content type. Either the configuration is invalid, or you just need to click Configure.">
-                            {% else %}
-                                <img id="configured-icon-org" class="configured-icon" src="/static/assets/icons/confirm-icon.svg" alt="Configured">
-                            {% endif %}
+                            <img id="configured-icon-org" class="configured-icon" src="/static/assets/icons/confirm-icon.svg" alt="Configured">
                         {% endif %}
                     </h3>
                 </div>
                 <div class="card-description-row">
                 <p class="card-description">Set org files for Khoj to index</p>
                 </div>
                 <div class="card-action-row">
@@ -147,19 +131,15 @@
             </div>
             <div class="card">
                 <div class="card-title-row">
                     <img class="card-icon" src="/static/assets/icons/pdf.svg" alt="PDF">
                     <h3 class="card-title">
                         PDF
                         {% if current_config.content_type.pdf %}
-                            {% if current_model_state.pdf == False %}
-                                <img id="misconfigured-icon-pdf" class="configured-icon" src="/static/assets/icons/question-mark-icon.svg" alt="Not Configured" title="Embeddings have not been generated yet for this content type. Either the configuration is invalid, or you need to click Configure.">
-                            {% else %}
-                                <img id="configured-icon-pdf" class="configured-icon" src="/static/assets/icons/confirm-icon.svg" alt="Configured">
-                            {% endif %}
+                            <img id="configured-icon-pdf" class="configured-icon" src="/static/assets/icons/confirm-icon.svg" alt="Configured">
                         {% endif %}
                     </h3>
                 </div>
                 <div class="card-description-row">
                 <p class="card-description">Set PDF files for Khoj to index</p>
                 </div>
                 <div class="card-action-row">
@@ -187,20 +167,16 @@
         <div class="section-cards">
             <div class="card">
                 <div class="card-title-row">
                     <img class="card-icon" src="/static/assets/icons/chat.svg" alt="Chat">
                     <h3 class="card-title">
                         Chat
                         {% if current_config.processor and current_config.processor.conversation %}
-                            {% if current_model_state.conversation == False %}
-                                <img id="misconfigured-icon-conversation-processor" class="configured-icon" src="/static/assets/icons/question-mark-icon.svg" alt="Not Configured" title="Embeddings have not been generated yet for this content type. Either the configuration is invalid, or you just need to click Configure.">
-                            {% else %}
-                                <img id="configured-icon-conversation-processor" class="configured-icon" src="/static/assets/icons/confirm-icon.svg" alt="Configured">
-                            {% endif %}
-                        {% endif %}
+                            <img id="configured-icon-conversation-processor" class="configured-icon" src="/static/assets/icons/confirm-icon.svg" alt="Configured">
+                         {% endif %}
                     </h3>
                 </div>
                 <div class="card-description-row">
                 <p class="card-description">Setup Khoj Chat with OpenAI</p>
                 </div>
                 <div class="card-action-row">
                     <a class="card-button" href="/config/processor/conversation">
@@ -224,16 +200,14 @@
     </div>
     <div class="section">
         <div id="results-count" title="Number of items to show in search and use for chat response">
             <label for="results-count-slider">Results Count: <span id="results-count-value">5</span></label>
             <input type="range" id="results-count-slider" name="results-count-slider" min="1" max="10" step="1" value="5">
         </div>
         <div id="status" style="display: none;"></div>
-    </div>
-    <div class="section finalize-actions">
         <button id="configure" type="submit" title="Update index with the latest changes">⚙️ Configure</button>
         <button id="reinitialize" type="submit" title="Regenerate index from scratch">🔄 Reinitialize</button>
     </div>
 </div>
 <script>
     function clearContentType(content_type) {
         const csrfToken = document.cookie.split('; ').find(row => row.startsWith('csrftoken'))?.split('=')[1];
@@ -247,22 +221,15 @@
         .then(response => response.json())
         .then(data => {
             if (data.status == "ok") {
                 var contentTypeClearButton = document.getElementById("clear-" + content_type);
                 contentTypeClearButton.style.display = "none";
 
                 var configuredIcon = document.getElementById("configured-icon-" + content_type);
-                if (configuredIcon) {
-                    configuredIcon.style.display = "none";
-                }
-
-                var misconfiguredIcon = document.getElementById("misconfigured-icon-" + content_type);
-                if (misconfiguredIcon) {
-                    misconfiguredIcon.style.display = "none";
-                }
+                configuredIcon.style.display = "none";
             }
         })
     };
 
     function clearConversationProcessor() {
         const csrfToken = document.cookie.split('; ').find(row => row.startsWith('csrftoken'))?.split('=')[1];
         fetch('/api/delete/config/data/processor/conversation', {
@@ -275,23 +242,15 @@
         .then(response => response.json())
         .then(data => {
             if (data.status == "ok") {
                 var conversationClearButton = document.getElementById("clear-conversation");
                 conversationClearButton.style.display = "none";
 
                 var configuredIcon = document.getElementById("configured-icon-conversation-processor");
-                if (configuredIcon) {
-                    configuredIcon.style.display = "none";
-                }
-
-                var misconfiguredIcon = document.getElementById("misconfigured-icon-conversation-processor");
-
-                if (misconfiguredIcon) {
-                    misconfiguredIcon.style.display = "none";
-                }
+                configuredIcon.style.display = "none";
             }
         })
     };
 
     var configure = document.getElementById("configure");
     configure.addEventListener("click", function(event) {
         event.preventDefault();
@@ -329,22 +288,22 @@
         })
         .then(response => response.json())
         .then(data => {
             console.log('Success:', data);
             if (data.detail != null) {
                 throw new Error(data.detail);
             }
-            document.getElementById("status").innerHTML = emoji + " " + successText;
+            document.getElementById("status").innerHTML = emoji + successText;
             document.getElementById("status").style.display = "block";
             button.disabled = false;
             button.innerHTML = '✅ Done!';
         })
         .catch((error) => {
             console.error('Error:', error);
-            document.getElementById("status").innerHTML = emoji + " " + errorText
+            document.getElementById("status").innerHTML = emoji + errorText
             document.getElementById("status").style.display = "block";
             button.disabled = false;
             button.innerHTML = '⚠️ Unsuccessful';
         });
     }
 
     // Setup the results count slider
```

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/interface/web/content_type_github_input.html` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/content_type_github_input.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 {% extends "base_config.html" %}
 {% block content %}
 <div class="page">
     <div class="section">
         <h2 class="section-title">
             <img class="card-icon" src="/static/assets/icons/github.svg" alt="Github">
             <span class="card-title-text">Github</span>
-            <div class="instructions">
-                <a href="https://github.com/khoj-ai/khoj/wiki/Setup-Github-integration">ⓘ Help</a>
-            </div>
         </h2>
         <form>
             <table>
                 <tr>
                     <td>
                         <label for="pat-token">Personal Access Token</label>
                     </td>
```

#### html2text {}

```diff
@@ -1,10 +1,9 @@
 {% extends "base_config.html" %} {% block content %}
-[Github] Github
-â_Help
+***** [Github] Github *****
 Personal Access Token [{{ current_config['pat_token'] }}]
 *** Repositories ***
 {% for repo in current_config['repos'] %}
 Repository Owner [{{ repo.owner }}    ] Repository Name [{{ repo.name}}      ]
 Repository Branch [{{ repo.branch }}   ] Remove Repository
 {% endfor %}
 Add Repository
```

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/interface/web/content_type_input.html` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/content_type_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/interface/web/content_type_notion_input.html` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/content_type_notion_input.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 {% extends "base_config.html" %}
 {% block content %}
 <div class="page">
     <div class="section">
         <h2 class="section-title">
             <img class="card-icon" src="/static/assets/icons/notion.svg" alt="Notion">
             <span class="card-title-text">Notion</span>
-            <div class="instructions">
-                <a href="https://github.com/khoj-ai/khoj/wiki/Setup-Notion-Integration">ⓘ Help</a>
-            </div>
         </h2>
         <form>
             <table>
                 <tr>
                     <td>
                         <label for="token">Token</label>
                     </td>
```

#### html2text {}

```diff
@@ -1,8 +1,7 @@
 {% extends "base_config.html" %} {% block content %}
-[Notion] Notion
-â_Help
+***** [Notion] Notion *****
 Token [{{ current_config['token'] }}]
 Compressed JSONL (Output) [{{ current_config['compressed_jsonl'] }}]
 Embeddings File (Output)  [{{ current_config['embeddings_file'] }}]
 Save
  {% endblock %}
```

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/interface/web/index.html` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/index.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/interface/web/processor_conversation_input.html` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/processor_conversation_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/interface/web/assets/khoj.css` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/khoj.css`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/interface/web/assets/markdown-it.min.js` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/markdown-it.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/interface/web/assets/org.min.js` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/org.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/interface/web/assets/pico.min.css` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/pico.min.css`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/interface/web/assets/icons/chat.svg` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/chat.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/interface/web/assets/icons/confirm-icon.svg` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/confirm-icon.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/interface/web/assets/icons/favicon-128x128.ico` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/favicon-128x128.ico`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/interface/web/assets/icons/favicon-128x128.png` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/interface/web/assets/icons/favicon.icns` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/favicon.icns`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/interface/web/assets/icons/github.svg` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/github.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/interface/web/assets/icons/logotype.svg` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/logotype.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/interface/web/assets/icons/notion.svg` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/notion.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/interface/web/assets/icons/org.svg` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/org.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/interface/web/assets/icons/pdf.svg` & `khoj_assistant-0.8.3.dev8/src/khoj/interface/web/assets/icons/pdf.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/processor/text_to_jsonl.py` & `khoj_assistant-0.8.3.dev8/src/khoj/processor/text_to_jsonl.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 class TextToJsonl(ABC):
     def __init__(self, config: TextConfigBase):
         self.config = config
 
     @abstractmethod
-    def process(self, previous_entries: List[Entry] = []) -> List[Tuple[int, Entry]]:
+    def process(self, previous_entries: List[Entry] = None) -> List[Tuple[int, Entry]]:
         ...
 
     @staticmethod
     def hash_func(key: str) -> Callable:
         return lambda entry: hashlib.md5(bytes(getattr(entry, key), encoding="utf-8")).hexdigest()
 
     @staticmethod
@@ -74,31 +74,24 @@
             hash_to_previous_entries = dict(zip(previous_entry_hashes, previous_entries))
 
             # All entries that did not exist in the previous set are to be added
             new_entry_hashes = set(current_entry_hashes) - set(previous_entry_hashes)
             # All entries that exist in both current and previous sets are kept
             existing_entry_hashes = set(current_entry_hashes) & set(previous_entry_hashes)
 
-            # load new entries in the order in which they are processed for a stable sort
-            new_entries = [
-                (current_entry_hashes.index(entry_hash), hash_to_current_entries[entry_hash])
-                for entry_hash in new_entry_hashes
-            ]
-            new_entries_sorted = sorted(new_entries, key=lambda e: e[0])
             # Mark new entries with -1 id to flag for later embeddings generation
-            new_entries_sorted = [(-1, entry[1]) for entry in new_entries_sorted]
-
+            new_entries = [(-1, hash_to_current_entries[entry_hash]) for entry_hash in new_entry_hashes]
             # Set id of existing entries to their previous ids to reuse their existing encoded embeddings
             existing_entries = [
                 (previous_entry_hashes.index(entry_hash), hash_to_previous_entries[entry_hash])
                 for entry_hash in existing_entry_hashes
             ]
-            existing_entries_sorted = sorted(existing_entries, key=lambda e: e[0])
 
-            entries_with_ids = existing_entries_sorted + new_entries_sorted
+            existing_entries_sorted = sorted(existing_entries, key=lambda e: e[0])
+            entries_with_ids = existing_entries_sorted + new_entries
 
         return entries_with_ids
 
     @staticmethod
     def convert_text_maps_to_jsonl(entries: List[Entry]) -> str:
         # Convert each entry to JSON and write to JSONL file
         return "".join([f"{entry.to_json()}\n" for entry in entries])
```

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/processor/conversation/gpt.py` & `khoj_assistant-0.8.3.dev8/src/khoj/processor/conversation/gpt.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/processor/conversation/prompts.py` & `khoj_assistant-0.8.3.dev8/src/khoj/processor/conversation/prompts.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/processor/conversation/utils.py` & `khoj_assistant-0.8.3.dev8/src/khoj/processor/conversation/utils.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/processor/github/github_to_jsonl.py` & `khoj_assistant-0.8.3.dev8/src/khoj/processor/github/github_to_jsonl.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 
 # Internal Packages
 from khoj.utils.helpers import timer
 from khoj.utils.rawconfig import Entry, GithubContentConfig, GithubRepoConfig
 from khoj.processor.markdown.markdown_to_jsonl import MarkdownToJsonl
 from khoj.processor.org_mode.org_to_jsonl import OrgToJsonl
 from khoj.processor.text_to_jsonl import TextToJsonl
-from khoj.utils.jsonl import compress_jsonl_data
+from khoj.utils.jsonl import dump_jsonl, compress_jsonl_data
 from khoj.utils.rawconfig import Entry
+from khoj.utils import state
 
 
 logger = logging.getLogger(__name__)
 
 
 class GithubToJsonl(TextToJsonl):
     def __init__(self, config: GithubContentConfig):
@@ -33,15 +34,15 @@
             wait_time = int(response.headers.get("X-RateLimit-Reset")) - int(time.time())
             logger.info(f"Github Rate limit reached. Waiting for {wait_time} seconds")
             time.sleep(wait_time)
             return func(*args, **kwargs)
         else:
             return
 
-    def process(self, previous_entries=[]):
+    def process(self, previous_entries=None):
         current_entries = []
         for repo in self.config.repos:
             current_entries += self.process_repo(repo)
 
         return self.update_entries_with_ids(current_entries, previous_entries)
 
     def process_repo(self, repo: GithubRepoConfig):
@@ -93,15 +94,18 @@
 
         with timer("Write github entries to JSONL file", logger):
             # Process Each Entry from All Notes Files
             entries = list(map(lambda entry: entry[1], entries_with_ids))
             jsonl_data = MarkdownToJsonl.convert_markdown_maps_to_jsonl(entries)
 
             # Compress JSONL formatted Data
-            compress_jsonl_data(jsonl_data, self.config.compressed_jsonl)
+            if self.config.compressed_jsonl.suffix == ".gz":
+                compress_jsonl_data(jsonl_data, self.config.compressed_jsonl)
+            elif self.config.compressed_jsonl.suffix == ".jsonl":
+                dump_jsonl(jsonl_data, self.config.compressed_jsonl)
 
         return entries_with_ids
 
     def get_files(self, repo_url: str, repo: GithubRepoConfig):
         # Get the contents of the repository
         repo_content_url = f"{repo_url}/git/trees/{repo.branch}"
         headers = {"Authorization": f"token {self.config.pat_token}"}
```

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/processor/jsonl/jsonl_to_jsonl.py` & `khoj_assistant-0.8.3.dev8/src/khoj/processor/jsonl/jsonl_to_jsonl.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 import logging
 from pathlib import Path
 from typing import List
 
 # Internal Packages
 from khoj.processor.text_to_jsonl import TextToJsonl
 from khoj.utils.helpers import get_absolute_path, timer
-from khoj.utils.jsonl import load_jsonl, compress_jsonl_data
+from khoj.utils.jsonl import load_jsonl, dump_jsonl, compress_jsonl_data
 from khoj.utils.rawconfig import Entry
 
 
 logger = logging.getLogger(__name__)
 
 
 class JsonlToJsonl(TextToJsonl):
     # Define Functions
-    def process(self, previous_entries=[]):
+    def process(self, previous_entries=None):
         # Extract required fields from config
         input_jsonl_files, input_jsonl_filter, output_file = (
             self.config.input_files,
             self.config.input_filter,
             self.config.compressed_jsonl,
         )
 
@@ -34,25 +34,34 @@
 
         # Split entries by max tokens supported by model
         with timer("Split entries by max token size supported by model", logger):
             current_entries = self.split_entries_by_max_tokens(current_entries, max_tokens=256)
 
         # Identify, mark and merge any new entries with previous entries
         with timer("Identify new or updated entries", logger):
-            entries_with_ids = TextToJsonl.mark_entries_for_update(
-                current_entries, previous_entries, key="compiled", logger=logger
-            )
+            if not previous_entries:
+                entries_with_ids = list(enumerate(current_entries))
+            else:
+                entries_with_ids = TextToJsonl.mark_entries_for_update(
+                    current_entries,
+                    previous_entries,
+                    key="compiled",
+                    logger=logger,
+                )
 
         with timer("Write entries to JSONL file", logger):
             # Process Each Entry from All Notes Files
             entries = list(map(lambda entry: entry[1], entries_with_ids))
             jsonl_data = JsonlToJsonl.convert_entries_to_jsonl(entries)
 
             # Compress JSONL formatted Data
-            compress_jsonl_data(jsonl_data, output_file)
+            if output_file.suffix == ".gz":
+                compress_jsonl_data(jsonl_data, output_file)
+            elif output_file.suffix == ".jsonl":
+                dump_jsonl(jsonl_data, output_file)
 
         return entries_with_ids
 
     @staticmethod
     def get_jsonl_files(jsonl_files=None, jsonl_file_filters=None):
         "Get all jsonl files to process"
         absolute_jsonl_files, filtered_jsonl_files = set(), set()
```

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/processor/markdown/markdown_to_jsonl.py` & `khoj_assistant-0.8.3.dev8/src/khoj/processor/markdown/markdown_to_jsonl.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 from pathlib import Path
 from typing import List
 
 # Internal Packages
 from khoj.processor.text_to_jsonl import TextToJsonl
 from khoj.utils.helpers import get_absolute_path, is_none_or_empty, timer
 from khoj.utils.constants import empty_escape_sequences
-from khoj.utils.jsonl import compress_jsonl_data
+from khoj.utils.jsonl import dump_jsonl, compress_jsonl_data
 from khoj.utils.rawconfig import Entry, TextContentConfig
 
 
 logger = logging.getLogger(__name__)
 
 
 class MarkdownToJsonl(TextToJsonl):
     def __init__(self, config: TextContentConfig):
         super().__init__(config)
         self.config = config
 
     # Define Functions
-    def process(self, previous_entries=[]):
+    def process(self, previous_entries=None):
         # Extract required fields from config
         markdown_files, markdown_file_filter, output_file = (
             self.config.input_files,
             self.config.input_filter,
             self.config.compressed_jsonl,
         )
 
@@ -47,25 +47,31 @@
 
         # Split entries by max tokens supported by model
         with timer("Split entries by max token size supported by model", logger):
             current_entries = self.split_entries_by_max_tokens(current_entries, max_tokens=256)
 
         # Identify, mark and merge any new entries with previous entries
         with timer("Identify new or updated entries", logger):
-            entries_with_ids = TextToJsonl.mark_entries_for_update(
-                current_entries, previous_entries, key="compiled", logger=logger
-            )
+            if not previous_entries:
+                entries_with_ids = list(enumerate(current_entries))
+            else:
+                entries_with_ids = TextToJsonl.mark_entries_for_update(
+                    current_entries, previous_entries, key="compiled", logger=logger
+                )
 
         with timer("Write markdown entries to JSONL file", logger):
             # Process Each Entry from All Notes Files
             entries = list(map(lambda entry: entry[1], entries_with_ids))
             jsonl_data = MarkdownToJsonl.convert_markdown_maps_to_jsonl(entries)
 
             # Compress JSONL formatted Data
-            compress_jsonl_data(jsonl_data, output_file)
+            if output_file.suffix == ".gz":
+                compress_jsonl_data(jsonl_data, output_file)
+            elif output_file.suffix == ".jsonl":
+                dump_jsonl(jsonl_data, output_file)
 
         return entries_with_ids
 
     @staticmethod
     def get_markdown_files(markdown_files=None, markdown_file_filters=None):
         "Get Markdown files to process"
         absolute_markdown_files, filtered_markdown_files = set(), set()
```

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/processor/notion/notion_to_jsonl.py` & `khoj_assistant-0.8.3.dev8/src/khoj/processor/notion/notion_to_jsonl.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # External Packages
 import requests
 
 # Internal Packages
 from khoj.utils.helpers import timer
 from khoj.utils.rawconfig import Entry, NotionContentConfig
 from khoj.processor.text_to_jsonl import TextToJsonl
-from khoj.utils.jsonl import compress_jsonl_data
+from khoj.utils.jsonl import dump_jsonl, compress_jsonl_data
 from khoj.utils.rawconfig import Entry
 
 from enum import Enum
 
 
 logger = logging.getLogger(__name__)
 
@@ -74,33 +74,31 @@
             NotionBlockType.TO_DO.value,
             NotionBlockType.TOGGLE.value,
             NotionBlockType.CHILD_PAGE.value,
             NotionBlockType.BOOKMARK.value,
             NotionBlockType.DIVIDER.value,
         ]
 
-        self.body_params = {"page_size": 100}
-
-    def process(self, previous_entries=[]):
+    def process(self, previous_entries=None):
         current_entries = []
 
         # Get all pages
         with timer("Getting all pages via search endpoint", logger=logger):
             responses = []
 
             while True:
                 result = self.session.post(
                     "https://api.notion.com/v1/search",
-                    json=self.body_params,
+                    json={"page_size": 100},
                 ).json()
                 responses.append(result)
                 if result["has_more"] == False:
                     break
                 else:
-                    self.body_params.update({"start_cursor": result["next_cursor"]})
+                    self.session.params = {"start_cursor": responses[-1]["next_cursor"]}
 
         for response in responses:
             with timer("Processing response", logger=logger):
                 pages_or_databases = response["results"]
 
                 # Get all pages content
                 for p_or_d in pages_or_databases:
@@ -172,16 +170,15 @@
                 )
         return current_entries
 
     def process_heading(self, heading):
         return f"\n<b>{heading}</b>\n"
 
     def process_nested_children(self, children, raw_content, block_type=None):
-        results = children["results"] if children.get("results") else []
-        for child in results:
+        for child in children["results"]:
             child_type = child.get("type")
             if child_type == None:
                 continue
             child_data = child[child_type]
             if child_data.get("rich_text") and len(child_data["rich_text"]) > 0:
                 for text in child_data["rich_text"]:
                     raw_content += self.process_text(text, block_type)
@@ -198,19 +195,15 @@
             return f"<a href='{text['href']}'>{text['plain_text']}</a>"
         raw_text = text["plain_text"]
         if text_type in self.display_block_block_types or block_type in self.display_block_block_types:
             return f"\n{raw_text}\n"
         return raw_text
 
     def get_block_children(self, block_id):
-        try:
-            return self.session.get(f"https://api.notion.com/v1/blocks/{block_id}/children").json()
-        except Exception as e:
-            logger.error(f"Error getting children for block {block_id}: {e}")
-            return {}
+        return self.session.get(f"https://api.notion.com/v1/blocks/{block_id}/children").json()
 
     def get_page(self, page_id):
         return self.session.get(f"https://api.notion.com/v1/pages/{page_id}").json()
 
     def get_page_children(self, page_id):
         return self.session.get(f"https://api.notion.com/v1/blocks/{page_id}/children").json()
 
@@ -218,38 +211,33 @@
         try:
             page = self.get_page(page_id)
             content = self.get_page_children(page_id)
         except Exception as e:
             logger.error(f"Error getting page {page_id}: {e}")
             return None, None
         properties = page["properties"]
-        title_field = "title"
-        if "Title" in properties:
-            title_field = "Title"
-        elif "Name" in properties:
-            title_field = "Name"
-        elif "Page" in properties:
-            title_field = "Page"
-        elif "Event" in properties:
-            title_field = "Event"
-        elif title_field not in properties:
-            logger.error(f"Page {page_id} does not have a title field")
-            return None, None
+        title_field = "Title" if "Title" in properties else "title"
         title = page["properties"][title_field]["title"][0]["text"]["content"]
         return title, content
 
     def update_entries_with_ids(self, current_entries, previous_entries):
         # Identify, mark and merge any new entries with previous entries
         with timer("Identify new or updated entries", logger):
-            entries_with_ids = TextToJsonl.mark_entries_for_update(
-                current_entries, previous_entries, key="compiled", logger=logger
-            )
+            if not previous_entries:
+                entries_with_ids = list(enumerate(current_entries))
+            else:
+                entries_with_ids = TextToJsonl.mark_entries_for_update(
+                    current_entries, previous_entries, key="compiled", logger=logger
+                )
 
         with timer("Write Notion entries to JSONL file", logger):
             # Process Each Entry from all Notion entries
             entries = list(map(lambda entry: entry[1], entries_with_ids))
             jsonl_data = TextToJsonl.convert_text_maps_to_jsonl(entries)
 
             # Compress JSONL formatted Data
-            compress_jsonl_data(jsonl_data, self.config.compressed_jsonl)
+            if self.config.compressed_jsonl.suffix == ".gz":
+                compress_jsonl_data(jsonl_data, self.config.compressed_jsonl)
+            elif self.config.compressed_jsonl.suffix == ".jsonl":
+                dump_jsonl(jsonl_data, self.config.compressed_jsonl)
 
         return entries_with_ids
```

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/processor/org_mode/org_to_jsonl.py` & `khoj_assistant-0.8.3.dev8/src/khoj/processor/org_mode/org_to_jsonl.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 from pathlib import Path
 from typing import Iterable, List
 
 # Internal Packages
 from khoj.processor.org_mode import orgnode
 from khoj.processor.text_to_jsonl import TextToJsonl
 from khoj.utils.helpers import get_absolute_path, is_none_or_empty, timer
-from khoj.utils.jsonl import compress_jsonl_data
+from khoj.utils.jsonl import dump_jsonl, compress_jsonl_data
 from khoj.utils.rawconfig import Entry, TextContentConfig
 from khoj.utils import state
 
 
 logger = logging.getLogger(__name__)
 
 
 class OrgToJsonl(TextToJsonl):
     def __init__(self, config: TextContentConfig):
         super().__init__(config)
         self.config = config
 
     # Define Functions
-    def process(self, previous_entries: List[Entry] = []):
+    def process(self, previous_entries: List[Entry] = None):
         # Extract required fields from config
         org_files, org_file_filter, output_file = (
             self.config.input_files,
             self.config.input_filter,
             self.config.compressed_jsonl,
         )
         index_heading_entries = self.config.index_heading_entries
@@ -47,26 +47,31 @@
         with timer("Convert OrgNodes into list of entries", logger):
             current_entries = self.convert_org_nodes_to_entries(entry_nodes, file_to_entries, index_heading_entries)
 
         with timer("Split entries by max token size supported by model", logger):
             current_entries = self.split_entries_by_max_tokens(current_entries, max_tokens=256)
 
         # Identify, mark and merge any new entries with previous entries
-        with timer("Identify new or updated entries", logger):
+        if not previous_entries:
+            entries_with_ids = list(enumerate(current_entries))
+        else:
             entries_with_ids = TextToJsonl.mark_entries_for_update(
                 current_entries, previous_entries, key="compiled", logger=logger
             )
 
         # Process Each Entry from All Notes Files
         with timer("Write org entries to JSONL file", logger):
             entries = map(lambda entry: entry[1], entries_with_ids)
             jsonl_data = self.convert_org_entries_to_jsonl(entries)
 
             # Compress JSONL formatted Data
-            compress_jsonl_data(jsonl_data, output_file)
+            if output_file.suffix == ".gz":
+                compress_jsonl_data(jsonl_data, output_file)
+            elif output_file.suffix == ".jsonl":
+                dump_jsonl(jsonl_data, output_file)
 
         return entries_with_ids
 
     @staticmethod
     def get_org_files(org_files=None, org_file_filters=None):
         "Get Org files to process"
         absolute_org_files, filtered_org_files = set(), set()
@@ -116,21 +121,17 @@
         "Convert Org-Mode nodes into list of Entry objects"
         entries: List[Entry] = []
         for parsed_entry in parsed_entries:
             if not parsed_entry.hasBody and not index_heading_entries:
                 # Ignore title notes i.e notes with just headings and empty body
                 continue
 
-            todo_str = f"{parsed_entry.todo} " if parsed_entry.todo else ""
             # Prepend filename as top heading to entry
             filename = Path(entry_to_file_map[parsed_entry]).stem
-            if parsed_entry.heading:
-                heading = f"* {filename}\n** {todo_str}{parsed_entry.heading}."
-            else:
-                heading = f"* {filename}."
+            heading = f"* {filename}\n** {parsed_entry.heading}." if parsed_entry.heading else f"* {filename}."
 
             compiled = heading
             if state.verbose > 2:
                 logger.debug(f"Title: {parsed_entry.heading}")
 
             if parsed_entry.tags:
                 tags_str = " ".join(parsed_entry.tags)
```

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/processor/org_mode/orgnode.py` & `khoj_assistant-0.8.3.dev8/src/khoj/processor/org_mode/orgnode.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/processor/pdf/pdf_to_jsonl.py` & `khoj_assistant-0.8.3.dev8/src/khoj/processor/pdf/pdf_to_jsonl.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 
 # External Packages
 from langchain.document_loaders import PyPDFLoader
 
 # Internal Packages
 from khoj.processor.text_to_jsonl import TextToJsonl
 from khoj.utils.helpers import get_absolute_path, is_none_or_empty, timer
-from khoj.utils.jsonl import compress_jsonl_data
+from khoj.utils.jsonl import dump_jsonl, compress_jsonl_data
 from khoj.utils.rawconfig import Entry
 
 
 logger = logging.getLogger(__name__)
 
 
 class PdfToJsonl(TextToJsonl):
     # Define Functions
-    def process(self, previous_entries=[]):
+    def process(self, previous_entries=None):
         # Extract required fields from config
         pdf_files, pdf_file_filter, output_file = (
             self.config.input_files,
             self.config.input_filter,
             self.config.compressed_jsonl,
         )
 
@@ -41,25 +41,31 @@
 
         # Split entries by max tokens supported by model
         with timer("Split entries by max token size supported by model", logger):
             current_entries = self.split_entries_by_max_tokens(current_entries, max_tokens=256)
 
         # Identify, mark and merge any new entries with previous entries
         with timer("Identify new or updated entries", logger):
-            entries_with_ids = TextToJsonl.mark_entries_for_update(
-                current_entries, previous_entries, key="compiled", logger=logger
-            )
+            if not previous_entries:
+                entries_with_ids = list(enumerate(current_entries))
+            else:
+                entries_with_ids = TextToJsonl.mark_entries_for_update(
+                    current_entries, previous_entries, key="compiled", logger=logger
+                )
 
         with timer("Write PDF entries to JSONL file", logger):
             # Process Each Entry from All Notes Files
             entries = list(map(lambda entry: entry[1], entries_with_ids))
             jsonl_data = PdfToJsonl.convert_pdf_maps_to_jsonl(entries)
 
             # Compress JSONL formatted Data
-            compress_jsonl_data(jsonl_data, output_file)
+            if output_file.suffix == ".gz":
+                compress_jsonl_data(jsonl_data, output_file)
+            elif output_file.suffix == ".jsonl":
+                dump_jsonl(jsonl_data, output_file)
 
         return entries_with_ids
 
     @staticmethod
     def get_pdf_files(pdf_files=None, pdf_file_filters=None):
         "Get PDF files to process"
         absolute_pdf_files, filtered_pdf_files = set(), set()
```

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/routers/api.py` & `khoj_assistant-0.8.3.dev8/src/khoj/routers/api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # Standard Packages
 import concurrent.futures
 import math
 import time
 import yaml
 import logging
 import json
-from typing import Iterable, List, Optional, Union
+from typing import List, Optional, Union
 
 # External Packages
 from fastapi import APIRouter, HTTPException, Header, Request
 from sentence_transformers import util
 
 # Internal Packages
-from khoj.configure import configure_processor, configure_server
+from khoj.configure import configure_processor, configure_search
 from khoj.search_type import image_search, text_search
 from khoj.search_filter.date_filter import DateFilter
 from khoj.search_filter.file_filter import FileFilter
 from khoj.search_filter.word_filter import WordFilter
 from khoj.utils.config import TextSearchModel
-from khoj.utils.helpers import timer
+from khoj.utils.helpers import log_telemetry, timer
 from khoj.utils.rawconfig import (
     ContentConfig,
     FullConfig,
     ProcessorConfig,
     SearchConfig,
     SearchResponse,
     TextContentConfig,
@@ -30,15 +30,15 @@
     GithubContentConfig,
     NotionContentConfig,
 )
 from khoj.utils.state import SearchType
 from khoj.utils import state, constants
 from khoj.utils.yaml import save_config_to_file_updated_state
 from fastapi.responses import StreamingResponse, Response
-from khoj.routers.helpers import perform_chat_checks, generate_chat_response, update_telemetry_state
+from khoj.routers.helpers import perform_chat_checks, generate_chat_response
 from khoj.processor.conversation.gpt import extract_questions
 from fastapi.requests import Request
 
 
 # Initialize Router
 api = APIRouter()
 logger = logging.getLogger(__name__)
@@ -52,210 +52,112 @@
             state.config.search_type = SearchConfig.parse_obj(constants.default_config["search-type"])
 
     @api.get("/config/data", response_model=FullConfig)
     def get_config_data():
         return state.config
 
     @api.post("/config/data")
-    async def set_config_data(
-        request: Request,
-        updated_config: FullConfig,
-        client: Optional[str] = None,
-    ):
+    async def set_config_data(updated_config: FullConfig):
         state.config = updated_config
         with open(state.config_file, "w") as outfile:
             yaml.dump(yaml.safe_load(state.config.json(by_alias=True)), outfile)
             outfile.close()
-
-        configuration_update_metadata = dict()
-
-        if state.config.content_type is not None:
-            configuration_update_metadata["github"] = state.config.content_type.github is not None
-            configuration_update_metadata["notion"] = state.config.content_type.notion is not None
-            configuration_update_metadata["org"] = state.config.content_type.org is not None
-            configuration_update_metadata["pdf"] = state.config.content_type.pdf is not None
-            configuration_update_metadata["markdown"] = state.config.content_type.markdown is not None
-            configuration_update_metadata["plugins"] = state.config.content_type.plugins is not None
-
-        if state.config.processor is not None:
-            configuration_update_metadata["conversation_processor"] = state.config.processor.conversation is not None
-
-        update_telemetry_state(
-            request=request,
-            telemetry_type="api",
-            api="set_config",
-            client=client,
-            metadata=configuration_update_metadata,
-        )
         return state.config
 
     @api.post("/config/data/content_type/github", status_code=200)
-    async def set_content_config_github_data(
-        request: Request,
-        updated_config: Union[GithubContentConfig, None],
-        client: Optional[str] = None,
-    ):
+    async def set_content_config_github_data(updated_config: Union[GithubContentConfig, None]):
         _initialize_config()
 
         if not state.config.content_type:
             state.config.content_type = ContentConfig(**{"github": updated_config})
         else:
             state.config.content_type.github = updated_config
 
-        update_telemetry_state(
-            request=request,
-            telemetry_type="api",
-            api="set_content_config",
-            client=client,
-            metadata={"content_type": "github"},
-        )
-
         try:
             save_config_to_file_updated_state()
             return {"status": "ok"}
         except Exception as e:
             return {"status": "error", "message": str(e)}
 
     @api.post("/config/data/content_type/notion", status_code=200)
-    async def set_content_config_notion_data(
-        request: Request,
-        updated_config: Union[NotionContentConfig, None],
-        client: Optional[str] = None,
-    ):
+    async def set_content_config_notion_data(updated_config: Union[NotionContentConfig, None]):
         _initialize_config()
 
         if not state.config.content_type:
             state.config.content_type = ContentConfig(**{"notion": updated_config})
         else:
             state.config.content_type.notion = updated_config
 
-        update_telemetry_state(
-            request=request,
-            telemetry_type="api",
-            api="set_content_config",
-            client=client,
-            metadata={"content_type": "notion"},
-        )
-
         try:
             save_config_to_file_updated_state()
             return {"status": "ok"}
         except Exception as e:
             return {"status": "error", "message": str(e)}
 
     @api.post("/delete/config/data/content_type/{content_type}", status_code=200)
-    async def remove_content_config_data(
-        request: Request,
-        content_type: str,
-        client: Optional[str] = None,
-    ):
+    async def remove_content_config_data(content_type: str):
         if not state.config or not state.config.content_type:
             return {"status": "ok"}
 
-        update_telemetry_state(
-            request=request,
-            telemetry_type="api",
-            api="delete_content_config",
-            client=client,
-            metadata={"content_type": content_type},
-        )
-
         if state.config.content_type:
             state.config.content_type[content_type] = None
 
         if content_type == "github":
-            state.content_index.github = None
+            state.model.github_search = None
         elif content_type == "notion":
-            state.content_index.notion = None
+            state.model.notion_search = None
         elif content_type == "plugins":
-            state.content_index.plugins = None
+            state.model.plugin_search = None
         elif content_type == "pdf":
-            state.content_index.pdf = None
+            state.model.pdf_search = None
         elif content_type == "markdown":
-            state.content_index.markdown = None
+            state.model.markdown_search = None
         elif content_type == "org":
-            state.content_index.org = None
+            state.model.org_search = None
 
         try:
             save_config_to_file_updated_state()
             return {"status": "ok"}
         except Exception as e:
             return {"status": "error", "message": str(e)}
 
     @api.post("/delete/config/data/processor/conversation", status_code=200)
-    async def remove_processor_conversation_config_data(
-        request: Request,
-        client: Optional[str] = None,
-    ):
+    async def remove_processor_conversation_config_data():
         if not state.config or not state.config.processor or not state.config.processor.conversation:
             return {"status": "ok"}
 
         state.config.processor.conversation = None
 
-        update_telemetry_state(
-            request=request,
-            telemetry_type="api",
-            api="delete_processor_config",
-            client=client,
-            metadata={"processor_type": "conversation"},
-        )
-
         try:
             save_config_to_file_updated_state()
             return {"status": "ok"}
         except Exception as e:
             return {"status": "error", "message": str(e)}
 
     @api.post("/config/data/content_type/{content_type}", status_code=200)
-    async def set_content_config_data(
-        request: Request,
-        content_type: str,
-        updated_config: Union[TextContentConfig, None],
-        client: Optional[str] = None,
-    ):
+    async def set_content_config_data(content_type: str, updated_config: Union[TextContentConfig, None]):
         _initialize_config()
 
         if not state.config.content_type:
             state.config.content_type = ContentConfig(**{content_type: updated_config})
         else:
             state.config.content_type[content_type] = updated_config
 
-        update_telemetry_state(
-            request=request,
-            telemetry_type="api",
-            api="set_content_config",
-            client=client,
-            metadata={"content_type": content_type},
-        )
-
         try:
             save_config_to_file_updated_state()
             return {"status": "ok"}
         except Exception as e:
             return {"status": "error", "message": str(e)}
 
     @api.post("/config/data/processor/conversation", status_code=200)
-    async def set_processor_conversation_config_data(
-        request: Request,
-        updated_config: Union[ConversationProcessorConfig, None],
-        client: Optional[str] = None,
-    ):
+    async def set_processor_conversation_config_data(updated_config: Union[ConversationProcessorConfig, None]):
         _initialize_config()
 
         state.config.processor = ProcessorConfig(conversation=updated_config)
         state.processor_config = configure_processor(state.config.processor)
-
-        update_telemetry_state(
-            request=request,
-            telemetry_type="api",
-            api="set_content_config",
-            client=client,
-            metadata={"processor_type": "conversation"},
-        )
-
         try:
             save_config_to_file_updated_state()
             return {"status": "ok"}
         except Exception as e:
             return {"status": "error", "message": str(e)}
 
 
@@ -276,15 +178,15 @@
 
     configured_content_types = state.config.content_type.dict(exclude_none=True)
     return [
         search_type.value
         for search_type in SearchType
         if (
             search_type.value in configured_content_types
-            and getattr(state.content_index, search_type.value) is not None
+            and getattr(state.model, f"{search_type.value}_search") is not None
         )
         or ("plugins" in configured_content_types and search_type.name in configured_content_types["plugins"])
         or search_type == SearchType.All
     ]
 
 
 @api.get("/search", response_model=List[SearchResponse])
@@ -304,15 +206,15 @@
     start_time = time.time()
 
     # Run validation checks
     results: List[SearchResponse] = []
     if q is None or q == "":
         logger.warning(f"No query param (q) passed in API call to initiate search")
         return results
-    if not state.search_models or not any(state.search_models.__dict__.values()):
+    if not state.model or not any(state.model.__dict__.values()):
         logger.warning(f"No search models loaded. Configure a search model before initiating search")
         return results
 
     # initialize variables
     user_query = q.strip()
     results_count = n or 5
     score_threshold = score_threshold if score_threshold is not None else -math.inf
@@ -328,163 +230,134 @@
     defiltered_query = user_query
     for filter in [DateFilter(), WordFilter(), FileFilter()]:
         defiltered_query = filter.defilter(user_query)
 
     encoded_asymmetric_query = None
     if t == SearchType.All or t != SearchType.Image:
         text_search_models: List[TextSearchModel] = [
-            model for model in state.search_models.__dict__.values() if isinstance(model, TextSearchModel)
+            model for model in state.model.__dict__.values() if isinstance(model, TextSearchModel)
         ]
         if text_search_models:
             with timer("Encoding query took", logger=logger):
                 encoded_asymmetric_query = util.normalize_embeddings(
                     text_search_models[0].bi_encoder.encode(
                         [defiltered_query],
                         convert_to_tensor=True,
                         device=state.device,
                     )
                 )
 
     with concurrent.futures.ThreadPoolExecutor() as executor:
-        if (t == SearchType.Org or t == SearchType.All) and state.content_index.org and state.search_models.text_search:
+        if (t == SearchType.Org or t == SearchType.All) and state.model.org_search:
             # query org-mode notes
             search_futures += [
                 executor.submit(
                     text_search.query,
                     user_query,
-                    state.search_models.text_search,
-                    state.content_index.org,
+                    state.model.org_search,
                     question_embedding=encoded_asymmetric_query,
                     rank_results=r or False,
                     score_threshold=score_threshold,
                     dedupe=dedupe or True,
                 )
             ]
 
-        if (
-            (t == SearchType.Markdown or t == SearchType.All)
-            and state.content_index.markdown
-            and state.search_models.text_search
-        ):
+        if (t == SearchType.Markdown or t == SearchType.All) and state.model.markdown_search:
             # query markdown notes
             search_futures += [
                 executor.submit(
                     text_search.query,
                     user_query,
-                    state.search_models.text_search,
-                    state.content_index.markdown,
+                    state.model.markdown_search,
                     question_embedding=encoded_asymmetric_query,
                     rank_results=r or False,
                     score_threshold=score_threshold,
                     dedupe=dedupe or True,
                 )
             ]
 
-        if (
-            (t == SearchType.Github or t == SearchType.All)
-            and state.content_index.github
-            and state.search_models.text_search
-        ):
+        if (t == SearchType.Github or t == SearchType.All) and state.model.github_search:
             # query github issues
             search_futures += [
                 executor.submit(
                     text_search.query,
                     user_query,
-                    state.search_models.text_search,
-                    state.content_index.github,
+                    state.model.github_search,
                     question_embedding=encoded_asymmetric_query,
                     rank_results=r or False,
                     score_threshold=score_threshold,
                     dedupe=dedupe or True,
                 )
             ]
 
-        if (t == SearchType.Pdf or t == SearchType.All) and state.content_index.pdf and state.search_models.text_search:
+        if (t == SearchType.Pdf or t == SearchType.All) and state.model.pdf_search:
             # query pdf files
             search_futures += [
                 executor.submit(
                     text_search.query,
                     user_query,
-                    state.search_models.text_search,
-                    state.content_index.pdf,
+                    state.model.pdf_search,
                     question_embedding=encoded_asymmetric_query,
                     rank_results=r or False,
                     score_threshold=score_threshold,
                     dedupe=dedupe or True,
                 )
             ]
 
-        if (t == SearchType.Image) and state.content_index.image and state.search_models.image_search:
+        if (t == SearchType.Image) and state.model.image_search:
             # query images
             search_futures += [
                 executor.submit(
                     image_search.query,
                     user_query,
                     results_count,
-                    state.search_models.image_search,
-                    state.content_index.image,
+                    state.model.image_search,
                     score_threshold=score_threshold,
                 )
             ]
 
-        if (
-            (t == SearchType.All or t in SearchType)
-            and state.content_index.plugins
-            and state.search_models.plugin_search
-        ):
+        if (t == SearchType.All or t in SearchType) and state.model.plugin_search:
             # query specified plugin type
-            # Get plugin content, search model for specified search type, or the first one if none specified
-            plugin_search = state.search_models.plugin_search.get(t.value) or next(
-                iter(state.search_models.plugin_search.values())
-            )
-            plugin_content = state.content_index.plugins.get(t.value) or next(
-                iter(state.content_index.plugins.values())
-            )
             search_futures += [
                 executor.submit(
                     text_search.query,
                     user_query,
-                    plugin_search,
-                    plugin_content,
+                    # Get plugin search model for specified search type, or the first one if none specified
+                    state.model.plugin_search.get(t.value) or next(iter(state.model.plugin_search.values())),
                     question_embedding=encoded_asymmetric_query,
                     rank_results=r or False,
                     score_threshold=score_threshold,
                     dedupe=dedupe or True,
                 )
             ]
 
-        if (
-            (t == SearchType.Notion or t == SearchType.All)
-            and state.content_index.notion
-            and state.search_models.text_search
-        ):
+        if (t == SearchType.Notion or t == SearchType.All) and state.model.notion_search:
             # query notion pages
             search_futures += [
                 executor.submit(
                     text_search.query,
                     user_query,
-                    state.search_models.text_search,
-                    state.content_index.notion,
+                    state.model.notion_search,
                     question_embedding=encoded_asymmetric_query,
                     rank_results=r or False,
                     score_threshold=score_threshold,
                     dedupe=dedupe or True,
                 )
             ]
 
         # Query across each requested content types in parallel
         with timer("Query took", logger):
             for search_future in concurrent.futures.as_completed(search_futures):
-                if t == SearchType.Image and state.content_index.image:
+                if t == SearchType.Image:
                     hits = await search_future.result()
                     output_directory = constants.web_directory / "images"
                     # Collate results
                     results += image_search.collate_results(
                         hits,
-                        image_names=state.content_index.image.image_names,
+                        image_names=state.model.image_search.image_names,
                         output_directory=output_directory,
                         image_files_url="/static/images",
                         count=results_count,
                     )
                 else:
                     hits, entries = await search_future.result()
                     # Collate results
@@ -492,24 +365,28 @@
 
             # Sort results across all content types and take top results
             results = sorted(results, key=lambda x: float(x.score), reverse=True)[:results_count]
 
     # Cache results
     state.query_cache[query_cache_key] = results
 
-    update_telemetry_state(
-        request=request,
-        telemetry_type="api",
-        api="search",
-        client=client,
-        user_agent=user_agent,
-        referer=referer,
-        host=host,
-    )
-
+    user_state = {
+        "client_host": request.client.host if request.client else "unknown",
+        "user_agent": user_agent or "unknown",
+        "referer": referer or "unknown",
+        "host": host or "unknown",
+    }
+
+    # Only log telemetry if query is new and not a continuation of previous query
+    if state.previous_query is None or state.previous_query not in user_query:
+        state.telemetry += [
+            log_telemetry(
+                telemetry_type="api", api="search", client=client, app_config=state.config.app, properties=user_state
+            )
+        ]
     state.previous_query = user_query
 
     end_time = time.time()
     logger.debug(f"🔍 Search took: {end_time - start_time:.3f} seconds")
 
     return results
 
@@ -520,44 +397,50 @@
     t: Optional[SearchType] = None,
     force: Optional[bool] = False,
     client: Optional[str] = None,
     user_agent: Optional[str] = Header(None),
     referer: Optional[str] = Header(None),
     host: Optional[str] = Header(None),
 ):
-    if not state.config:
-        error_msg = f"🚨 Khoj is not configured.\nConfigure it via http://localhost:42110/config, plugins or by editing {state.config_file}."
-        logger.warning(error_msg)
-        raise HTTPException(status_code=500, detail=error_msg)
     try:
-        configure_server(state.config, regenerate=force or False, search_type=t)
-    except Exception as e:
-        error_msg = f"🚨 Failed to update server via API: {e}"
-        logger.error(error_msg, exc_info=True)
-        raise HTTPException(status_code=500, detail=error_msg)
+        state.search_index_lock.acquire()
+        try:
+            state.model = configure_search(state.model, state.config, regenerate=force or False, t=t)
+        except Exception as e:
+            logger.error(e)
+            raise HTTPException(status_code=500, detail=str(e))
+        finally:
+            state.search_index_lock.release()
+    except ValueError as e:
+        logger.error(e)
+        raise HTTPException(status_code=500, detail=str(e))
     else:
-        components = []
-        if state.search_models:
-            components.append("Search models")
-        if state.content_index:
-            components.append("Content index")
-        if state.processor_config:
-            components.append("Conversation processor")
-        components_msg = ", ".join(components)
-        logger.info(f"📬 {components_msg} updated via API")
-
-    update_telemetry_state(
-        request=request,
-        telemetry_type="api",
-        api="update",
-        client=client,
-        user_agent=user_agent,
-        referer=referer,
-        host=host,
-    )
+        logger.info("📬 Search index updated via API")
+
+    try:
+        if state.config and state.config.processor:
+            state.processor_config = configure_processor(state.config.processor)
+    except ValueError as e:
+        logger.error(e)
+        raise HTTPException(status_code=500, detail=str(e))
+    else:
+        logger.info("📬 Processor reconfigured via API")
+
+    user_state = {
+        "client_host": request.client.host if request.client else None,
+        "user_agent": user_agent or "unknown",
+        "referer": referer or "unknown",
+        "host": host or "unknown",
+    }
+
+    state.telemetry += [
+        log_telemetry(
+            telemetry_type="api", api="update", client=client, app_config=state.config.app, properties=user_state
+        )
+    ]
 
     return {"status": "ok", "message": "khoj reloaded"}
 
 
 @api.get("/chat/history")
 def chat_history(
     request: Request,
@@ -567,23 +450,26 @@
     host: Optional[str] = Header(None),
 ):
     perform_chat_checks()
 
     # Load Conversation History
     meta_log = state.processor_config.conversation.meta_log
 
-    update_telemetry_state(
-        request=request,
-        telemetry_type="api",
-        api="chat",
-        client=client,
-        user_agent=user_agent,
-        referer=referer,
-        host=host,
-    )
+    user_state = {
+        "client_host": request.client.host if request.client else None,
+        "user_agent": user_agent or "unknown",
+        "referer": referer or "unknown",
+        "host": host or "unknown",
+    }
+
+    state.telemetry += [
+        log_telemetry(
+            telemetry_type="api", api="chat", client=client, app_config=state.config.app, properties=user_state
+        )
+    ]
 
     return {"status": "ok", "response": meta_log.get("chat", [])}
 
 
 @api.get("/chat", response_class=Response)
 async def chat(
     request: Request,
@@ -619,23 +505,26 @@
         except StopIteration:
             break
 
     actual_response = aggregated_gpt_response.split("### compiled references:")[0]
 
     response_obj = {"response": actual_response, "context": compiled_references}
 
-    update_telemetry_state(
-        request=request,
-        telemetry_type="api",
-        api="chat",
-        client=client,
-        user_agent=user_agent,
-        referer=referer,
-        host=host,
-    )
+    user_state = {
+        "client_host": request.client.host if request.client else None,
+        "user_agent": user_agent or "unknown",
+        "referer": referer or "unknown",
+        "host": host or "unknown",
+    }
+
+    state.telemetry += [
+        log_telemetry(
+            telemetry_type="api", api="chat", client=client, app_config=state.config.app, properties=user_state
+        )
+    ]
 
     return Response(content=json.dumps(response_obj), media_type="application/json", status_code=200)
 
 
 async def extract_references_and_questions(
     request: Request,
     q: str,
```

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/routers/helpers.py` & `khoj_assistant-0.8.3.dev8/src/khoj/routers/helpers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,15 @@
+from fastapi import HTTPException
 import logging
 from datetime import datetime
 from functools import partial
-from typing import List, Optional
-
-from fastapi import HTTPException, Request
+from typing import List
 
 from khoj.utils import state
-from khoj.utils.helpers import timer, log_telemetry
+from khoj.utils.helpers import timer
 from khoj.processor.conversation.gpt import converse
 from khoj.processor.conversation.utils import message_to_log, reciprocal_conversation_to_chatml
 
 
 logger = logging.getLogger(__name__)
 
 
@@ -21,41 +20,14 @@
         or state.processor_config.conversation.openai_api_key is None
     ):
         raise HTTPException(
             status_code=500, detail="Set your OpenAI API key via Khoj settings and restart it to use Khoj Chat."
         )
 
 
-def update_telemetry_state(
-    request: Request,
-    telemetry_type: str,
-    api: str,
-    client: Optional[str] = None,
-    user_agent: Optional[str] = None,
-    referer: Optional[str] = None,
-    host: Optional[str] = None,
-    metadata: Optional[dict] = None,
-):
-    user_state = {
-        "client_host": request.client.host if request.client else None,
-        "user_agent": user_agent or "unknown",
-        "referer": referer or "unknown",
-        "host": host or "unknown",
-    }
-
-    if metadata:
-        user_state.update(metadata)
-
-    state.telemetry += [
-        log_telemetry(
-            telemetry_type=telemetry_type, api=api, client=client, app_config=state.config.app, properties=user_state
-        )
-    ]
-
-
 def generate_chat_response(
     q: str,
     meta_log: dict,
     compiled_references: List[str] = [],
     inferred_queries: List[str] = [],
 ):
     def _save_to_conversation_log(
```

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/routers/web_client.py` & `khoj_assistant-0.8.3.dev8/src/khoj/routers/web_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -35,52 +35,15 @@
     def config_page(request: Request):
         default_full_config = FullConfig(
             content_type=None,
             search_type=None,
             processor=None,
         )
         current_config = state.config or json.loads(default_full_config.json())
-
-        successfully_configured = {
-            "pdf": False,
-            "markdown": False,
-            "org": False,
-            "image": False,
-            "github": False,
-            "notion": False,
-            "conversation": False,
-        }
-
-        if state.content_index:
-            successfully_configured.update(
-                {
-                    "pdf": state.content_index.pdf is not None,
-                    "markdown": state.content_index.markdown is not None,
-                    "org": state.content_index.org is not None,
-                    "image": state.content_index.image is not None,
-                    "github": state.content_index.github is not None,
-                    "notion": state.content_index.notion is not None,
-                }
-            )
-
-        if state.processor_config:
-            successfully_configured.update(
-                {
-                    "conversation": state.processor_config.conversation is not None,
-                }
-            )
-
-        return templates.TemplateResponse(
-            "config.html",
-            context={
-                "request": request,
-                "current_config": current_config,
-                "current_model_state": successfully_configured,
-            },
-        )
+        return templates.TemplateResponse("config.html", context={"request": request, "current_config": current_config})
 
     @web_client.get("/config/content_type/github", response_class=HTMLResponse)
     def github_config_page(request: Request):
         default_copy = constants.default_config.copy()
         default_github = default_copy["content-type"]["github"]  # type: ignore
 
         default_config = TextContentConfig(
```

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/search_filter/base_filter.py` & `khoj_assistant-0.8.3.dev8/src/khoj/search_filter/base_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/search_filter/date_filter.py` & `khoj_assistant-0.8.3.dev8/src/khoj/search_filter/date_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/search_filter/file_filter.py` & `khoj_assistant-0.8.3.dev8/src/khoj/search_filter/file_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/search_filter/word_filter.py` & `khoj_assistant-0.8.3.dev8/src/khoj/search_filter/word_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/search_type/image_search.py` & `khoj_assistant-0.8.3.dev8/src/khoj/search_type/image_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,20 +8,18 @@
 from typing import List
 
 # External Packages
 from sentence_transformers import SentenceTransformer, util
 from PIL import Image
 from tqdm import trange
 import torch
-from khoj.utils import state
 
 # Internal Packages
 from khoj.utils.helpers import get_absolute_path, get_from_dict, resolve_absolute_path, load_model, timer
-from khoj.utils.config import ImageContent, ImageSearchModel
-from khoj.utils.models import BaseEncoder
+from khoj.utils.config import ImageSearchModel
 from khoj.utils.rawconfig import ImageContentConfig, ImageSearchConfig, SearchResponse
 
 
 # Create Logger
 logger = logging.getLogger(__name__)
 
 
@@ -38,15 +36,15 @@
     # Load the CLIP model
     encoder = load_model(
         model_dir=search_config.model_directory,
         model_name=search_config.encoder,
         model_type=search_config.encoder_type or SentenceTransformer,
     )
 
-    return ImageSearchModel(encoder)
+    return encoder
 
 
 def extract_entries(image_directories):
     image_names = []
     for image_directory in image_directories:
         image_directory = resolve_absolute_path(image_directory, strict=True)
         image_names.extend(list(image_directory.glob("*.jpg")))
@@ -141,46 +139,44 @@
         image_processed_metadata += ". " + ", ".join(image_metadata_subjects)
 
     logger.debug(f"{image_name}:\t{image_processed_metadata}")
 
     return image_processed_metadata
 
 
-async def query(
-    raw_query, count, search_model: ImageSearchModel, content: ImageContent, score_threshold: float = -math.inf
-):
+async def query(raw_query, count, model: ImageSearchModel, score_threshold: float = -math.inf):
     # Set query to image content if query is of form file:/path/to/file.png
     if raw_query.startswith("file:") and pathlib.Path(raw_query[5:]).is_file():
         query_imagepath = resolve_absolute_path(pathlib.Path(raw_query[5:]), strict=True)
         query = copy.deepcopy(Image.open(query_imagepath))
         query.thumbnail((640, query.height))  # scale down image for faster processing
         logger.info(f"🔎 Find Images by Image: {query_imagepath}")
     else:
         # Truncate words in query to stay below max_tokens supported by ML model
         max_words = 20
         query = " ".join(raw_query.split()[:max_words])
         logger.info(f"🔎 Find Images by Text: {query}")
 
     # Now we encode the query (which can either be an image or a text string)
     with timer("Query Encode Time", logger):
-        query_embedding = search_model.image_encoder.encode([query], convert_to_tensor=True, show_progress_bar=False)
+        query_embedding = model.image_encoder.encode([query], convert_to_tensor=True, show_progress_bar=False)
 
     # Compute top_k ranked images based on cosine-similarity b/w query and all image embeddings.
     with timer("Search Time", logger):
         image_hits = {
             result["corpus_id"]: {"image_score": result["score"], "score": result["score"]}
-            for result in util.semantic_search(query_embedding, content.image_embeddings, top_k=count)[0]
+            for result in util.semantic_search(query_embedding, model.image_embeddings, top_k=count)[0]
         }
 
     # Compute top_k ranked images based on cosine-similarity b/w query and all image metadata embeddings.
-    if content.image_metadata_embeddings:
+    if model.image_metadata_embeddings:
         with timer("Metadata Search Time", logger):
             metadata_hits = {
                 result["corpus_id"]: result["score"]
-                for result in util.semantic_search(query_embedding, content.image_metadata_embeddings, top_k=count)[0]
+                for result in util.semantic_search(query_embedding, model.image_metadata_embeddings, top_k=count)[0]
             }
 
         # Sum metadata, image scores of the highest ranked images
         for corpus_id, score in metadata_hits.items():
             scaling_factor = 0.33
             if "corpus_id" in image_hits:
                 image_hits[corpus_id].update(
@@ -239,15 +235,18 @@
                 }
             )
         ]
 
     return results
 
 
-def setup(config: ImageContentConfig, encoder: BaseEncoder, regenerate: bool) -> ImageContent:
+def setup(config: ImageContentConfig, search_config: ImageSearchConfig, regenerate: bool) -> ImageSearchModel:
+    # Initialize Model
+    encoder = initialize_model(search_config)
+
     # Extract Entries
     absolute_image_files, filtered_image_files = set(), set()
     if config.input_directories:
         image_directories = [resolve_absolute_path(directory, strict=True) for directory in config.input_directories]
         absolute_image_files = set(extract_entries(image_directories))
     if config.input_filter:
         filtered_image_files = {
@@ -265,8 +264,8 @@
         encoder,
         embeddings_file,
         batch_size=config.batch_size,
         regenerate=regenerate,
         use_xmp_metadata=config.use_xmp_metadata,
     )
 
-    return ImageContent(all_image_files, image_embeddings, image_metadata_embeddings)
+    return ImageSearchModel(all_image_files, image_embeddings, image_metadata_embeddings, encoder)
```

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/search_type/text_search.py` & `khoj_assistant-0.8.3.dev8/src/khoj/search_type/text_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,27 +9,30 @@
 from sentence_transformers import SentenceTransformer, CrossEncoder, util
 from khoj.processor.text_to_jsonl import TextToJsonl
 from khoj.search_filter.base_filter import BaseFilter
 
 # Internal Packages
 from khoj.utils import state
 from khoj.utils.helpers import get_absolute_path, is_none_or_empty, resolve_absolute_path, load_model, timer
-from khoj.utils.config import TextContent, TextSearchModel
+from khoj.utils.config import TextSearchModel
 from khoj.utils.models import BaseEncoder
 from khoj.utils.rawconfig import SearchResponse, TextSearchConfig, TextConfigBase, Entry
 from khoj.utils.jsonl import load_jsonl
 
 
 logger = logging.getLogger(__name__)
 
 
 def initialize_model(search_config: TextSearchConfig):
     "Initialize model for semantic search on text"
     torch.set_num_threads(4)
 
+    # Number of entries we want to retrieve with the bi-encoder
+    top_k = 15
+
     # If model directory is configured
     if search_config.model_directory:
         # Convert model directory to absolute path
         search_config.model_directory = resolve_absolute_path(search_config.model_directory)
         # Create model directory if it doesn't exist
         search_config.model_directory.parent.mkdir(parents=True, exist_ok=True)
 
@@ -45,106 +48,101 @@
     cross_encoder = load_model(
         model_dir=search_config.model_directory,
         model_name=search_config.cross_encoder,
         model_type=CrossEncoder,
         device=f"{state.device}",
     )
 
-    return TextSearchModel(bi_encoder, cross_encoder)
+    return bi_encoder, cross_encoder, top_k
 
 
 def extract_entries(jsonl_file) -> List[Entry]:
     "Load entries from compressed jsonl"
     return list(map(Entry.from_dict, load_jsonl(jsonl_file)))
 
 
 def compute_embeddings(
-    entries_with_ids: List[Tuple[int, Entry]],
-    bi_encoder: BaseEncoder,
-    embeddings_file: Path,
-    regenerate=False,
-    normalize=True,
+    entries_with_ids: List[Tuple[int, Entry]], bi_encoder: BaseEncoder, embeddings_file: Path, regenerate=False
 ):
     "Compute (and Save) Embeddings or Load Pre-Computed Embeddings"
-    new_embeddings = torch.tensor([], device=state.device)
-    existing_embeddings = torch.tensor([], device=state.device)
-    create_index_msg = ""
+    new_entries = []
     # Load pre-computed embeddings from file if exists and update them if required
     if embeddings_file.exists() and not regenerate:
-        corpus_embeddings: torch.Tensor = torch.load(get_absolute_path(embeddings_file), map_location=state.device)
+        corpus_embeddings = torch.load(get_absolute_path(embeddings_file), map_location=state.device)
         logger.debug(f"Loaded {len(corpus_embeddings)} text embeddings from {embeddings_file}")
-    else:
-        corpus_embeddings = torch.tensor([], device=state.device)
-        create_index_msg = " Creating index from scratch."
 
-    # Encode any new entries in the corpus and update corpus embeddings
-    new_entries = [entry.compiled for id, entry in entries_with_ids if id == -1]
-    if new_entries:
-        logger.info(f"📩 Indexing {len(new_entries)} text entries.{create_index_msg}")
-        new_embeddings = bi_encoder.encode(
+        # Encode any new entries in the corpus and update corpus embeddings
+        new_entries = [entry.compiled for id, entry in entries_with_ids if id == -1]
+        if new_entries:
+            logger.info(f"📩 Indexing {len(new_entries)} text entries.")
+            new_embeddings = bi_encoder.encode(
+                new_entries, convert_to_tensor=True, device=state.device, show_progress_bar=True
+            )
+            existing_entry_ids = [id for id, _ in entries_with_ids if id != -1]
+            if existing_entry_ids:
+                existing_embeddings = torch.index_select(
+                    corpus_embeddings, 0, torch.tensor(existing_entry_ids, device=state.device)
+                )
+            else:
+                existing_embeddings = torch.tensor([], device=state.device)
+            corpus_embeddings = torch.cat([existing_embeddings, new_embeddings], dim=0)
+    # Else compute the corpus embeddings from scratch
+    else:
+        new_entries = [entry.compiled for _, entry in entries_with_ids]
+        logger.info(f"📩 Indexing {len(new_entries)} text entries. Creating index from scratch.")
+        corpus_embeddings = bi_encoder.encode(
             new_entries, convert_to_tensor=True, device=state.device, show_progress_bar=True
         )
 
-    # Extract existing embeddings from previous corpus embeddings
-    existing_entry_ids = [id for id, _ in entries_with_ids if id != -1]
-    if existing_entry_ids:
-        existing_embeddings = torch.index_select(
-            corpus_embeddings, 0, torch.tensor(existing_entry_ids, device=state.device)
-        )
-
-    # Set corpus embeddings to merger of existing and new embeddings
-    corpus_embeddings = torch.cat([existing_embeddings, new_embeddings], dim=0)
-    if normalize:
-        # Normalize embeddings for faster lookup via dot product when querying
-        corpus_embeddings = util.normalize_embeddings(corpus_embeddings)
-
     # Save regenerated or updated embeddings to file
-    torch.save(corpus_embeddings, embeddings_file)
-    logger.info(f"📩 Saved computed text embeddings to {embeddings_file}")
+    if new_entries:
+        corpus_embeddings = util.normalize_embeddings(corpus_embeddings)
+        torch.save(corpus_embeddings, embeddings_file)
+        logger.info(f"📩 Saved computed text embeddings to {embeddings_file}")
 
     return corpus_embeddings
 
 
 async def query(
     raw_query: str,
-    search_model: TextSearchModel,
-    content: TextContent,
+    model: TextSearchModel,
     question_embedding: Union[torch.Tensor, None] = None,
     rank_results: bool = False,
     score_threshold: float = -math.inf,
     dedupe: bool = True,
 ) -> Tuple[List[dict], List[Entry]]:
     "Search for entries that answer the query"
-    query, entries, corpus_embeddings = raw_query, content.entries, content.corpus_embeddings
+    query, entries, corpus_embeddings = raw_query, model.entries, model.corpus_embeddings
 
     # Filter query, entries and embeddings before semantic search
-    query, entries, corpus_embeddings = apply_filters(query, entries, corpus_embeddings, content.filters)
+    query, entries, corpus_embeddings = apply_filters(query, entries, corpus_embeddings, model.filters)
 
     # If no entries left after filtering, return empty results
     if entries is None or len(entries) == 0:
         return [], []
     # If query only had filters it'll be empty now. So short-circuit and return results.
     if query.strip() == "":
         hits = [{"corpus_id": id, "score": 1.0} for id, _ in enumerate(entries)]
         return hits, entries
 
     # Encode the query using the bi-encoder
     if question_embedding is None:
         with timer("Query Encode Time", logger, state.device):
-            question_embedding = search_model.bi_encoder.encode([query], convert_to_tensor=True, device=state.device)
+            question_embedding = model.bi_encoder.encode([query], convert_to_tensor=True, device=state.device)
             question_embedding = util.normalize_embeddings(question_embedding)
 
     # Find relevant entries for the query
-    top_k = min(len(entries), search_model.top_k or 10)  # top_k hits can't be more than the total entries in corpus
     with timer("Search Time", logger, state.device):
-        hits = util.semantic_search(question_embedding, corpus_embeddings, top_k, score_function=util.dot_score)[0]
+        hits = util.semantic_search(
+            question_embedding, corpus_embeddings, top_k=model.top_k, score_function=util.dot_score
+        )[0]
 
     # Score all retrieved entries using the cross-encoder
-    if rank_results and search_model.cross_encoder:
-        hits = cross_encoder_score(search_model.cross_encoder, query, entries, hits)
+    if rank_results:
+        hits = cross_encoder_score(model.cross_encoder, query, entries, hits)
 
     # Filter results by score threshold
     hits = [hit for hit in hits if hit.get("cross-score", hit.get("score")) >= score_threshold]
 
     # Order results by cross-encoder score followed by bi-encoder score
     hits = sort_results(rank_results, hits)
 
@@ -171,42 +169,45 @@
         for hit in hits[0:count]
     ]
 
 
 def setup(
     text_to_jsonl: Type[TextToJsonl],
     config: TextConfigBase,
-    bi_encoder: BaseEncoder,
+    search_config: TextSearchConfig,
     regenerate: bool,
     filters: List[BaseFilter] = [],
-    normalize: bool = True,
-) -> TextContent:
+) -> TextSearchModel:
+    # Initialize Model
+    bi_encoder, cross_encoder, top_k = initialize_model(search_config)
+
     # Map notes in text files to (compressed) JSONL formatted file
     config.compressed_jsonl = resolve_absolute_path(config.compressed_jsonl)
-    previous_entries = []
-    if config.compressed_jsonl.exists() and not regenerate:
-        previous_entries = extract_entries(config.compressed_jsonl)
-    entries_with_indices = text_to_jsonl(config).process(previous_entries)
+    previous_entries = (
+        extract_entries(config.compressed_jsonl) if config.compressed_jsonl.exists() and not regenerate else None
+    )
+    entries_with_indices = text_to_jsonl(config).process(previous_entries or [])
 
     # Extract Updated Entries
     entries = extract_entries(config.compressed_jsonl)
     if is_none_or_empty(entries):
         config_params = ", ".join([f"{key}={value}" for key, value in config.dict().items()])
         raise ValueError(f"No valid entries found in specified files: {config_params}")
+    top_k = min(len(entries), top_k)  # top_k hits can't be more than the total entries in corpus
 
     # Compute or Load Embeddings
     config.embeddings_file = resolve_absolute_path(config.embeddings_file)
     corpus_embeddings = compute_embeddings(
-        entries_with_indices, bi_encoder, config.embeddings_file, regenerate=regenerate, normalize=normalize
+        entries_with_indices, bi_encoder, config.embeddings_file, regenerate=regenerate
     )
 
     for filter in filters:
         filter.load(entries, regenerate=regenerate)
 
-    return TextContent(entries, corpus_embeddings, filters)
+    return TextSearchModel(entries, corpus_embeddings, bi_encoder, cross_encoder, filters, top_k)
 
 
 def apply_filters(
     query: str, entries: List[Entry], corpus_embeddings: torch.Tensor, filters: List[BaseFilter]
 ) -> Tuple[str, List[Entry], torch.Tensor]:
     """Filter query, entries and embeddings before semantic search"""
```

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/utils/cli.py` & `khoj_assistant-0.8.3.dev8/src/khoj/utils/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Standard Packages
 import argparse
 import pathlib
 from importlib.metadata import version
 
 # Internal Packages
 from khoj.utils.helpers import resolve_absolute_path
-from khoj.utils.yaml import load_config_from_file, parse_config_from_file, save_config_to_file
+from khoj.utils.yaml import parse_config_from_file
 
 
 def cli(args=None):
     # Setup Argument Parser for the Commandline Interface
     parser = argparse.ArgumentParser(description="Start Khoj; An AI personal assistant for your Digital Brain")
     parser.add_argument(
         "--config-file", "-c", default="~/.khoj/khoj.yml", type=pathlib.Path, help="YAML file to configure Khoj"
@@ -30,38 +30,21 @@
         help="Path to UNIX socket for server. Use to run server behind reverse proxy. Default: /tmp/uvicorn.sock",
     )
     parser.add_argument("--version", "-V", action="store_true", help="Print the installed Khoj version and exit")
     parser.add_argument("--demo", action="store_true", default=False, help="Run Khoj in demo mode")
 
     args = parser.parse_args(args)
 
-    args.version_no = version("khoj-assistant")
     if args.version:
         # Show version of khoj installed and exit
-        print(args.version_no)
+        print(version("khoj-assistant"))
         exit(0)
 
     # Normalize config_file path to absolute path
     args.config_file = resolve_absolute_path(args.config_file)
 
     if not args.config_file.exists():
         args.config = None
     else:
-        args = migrate_config(args)
         args.config = parse_config_from_file(args.config_file)
 
     return args
-
-
-def migrate_config(args):
-    raw_config = load_config_from_file(args.config_file)
-
-    # Add version to khoj config schema
-    if "version" not in raw_config:
-        raw_config["version"] = args.version_no
-        save_config_to_file(raw_config, args.config_file)
-
-        # regenerate khoj index on first start of this version
-        # this should refresh index and apply index corruption fixes from #325
-        args.regenerate = True
-
-    return args
```

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/utils/constants.py` & `khoj_assistant-0.8.3.dev8/src/khoj/utils/constants.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/utils/helpers.py` & `khoj_assistant-0.8.3.dev8/src/khoj/utils/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 # Internal Packages
 from khoj.utils import constants
 
 
 if TYPE_CHECKING:
     # External Packages
-    from sentence_transformers import SentenceTransformer, CrossEncoder
+    from sentence_transformers import CrossEncoder
 
     # Internal Packages
     from khoj.utils.models import BaseEncoder
     from khoj.utils.rawconfig import AppConfig
 
 
 def is_none_or_empty(item):
@@ -60,17 +60,15 @@
         if key not in priority_dict:
             merged_dict[key] = default_dict[key]
         elif isinstance(priority_dict[key], dict) and isinstance(default_dict[key], dict):
             merged_dict[key] = merge_dicts(priority_dict[key], default_dict[key])
     return merged_dict
 
 
-def load_model(
-    model_name: str, model_type, model_dir=None, device: str = None
-) -> Union[BaseEncoder, SentenceTransformer, CrossEncoder]:
+def load_model(model_name: str, model_type, model_dir=None, device: str = None) -> Union[BaseEncoder, CrossEncoder]:
     "Load model from disk or huggingface"
     # Construct model path
     logger = logging.getLogger(__name__)
     model_path = path.join(model_dir, model_name.replace("/", "_")) if model_dir is not None else None
 
     # Load model from model_path if it exists there
     model_type_class = get_class_by_name(model_type) if isinstance(model_type, str) else model_type
```

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/utils/jsonl.py` & `khoj_assistant-0.8.3.dev8/src/khoj/utils/jsonl.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     # Initialize Variables
     data = []
     jsonl_file = None
 
     # Open JSONL file
     if input_path.suffix == ".gz":
         jsonl_file = gzip.open(get_absolute_path(input_path), "rt", encoding="utf-8")
-    else:
+    elif input_path.suffix == ".jsonl":
         jsonl_file = open(get_absolute_path(input_path), "r", encoding="utf-8")
 
     # Read JSONL file
     for line in jsonl_file:
         data.append(json.loads(line.strip(empty_escape_sequences)))
 
     # Close JSONL file
@@ -32,14 +32,25 @@
 
     # Log JSONL entries loaded
     logger.debug(f"Loaded {len(data)} records from {input_path}")
 
     return data
 
 
+def dump_jsonl(jsonl_data, output_path):
+    "Write List of JSON objects to JSON line file"
+    # Create output directory, if it doesn't exist
+    output_path.parent.mkdir(parents=True, exist_ok=True)
+
+    with open(output_path, "w", encoding="utf-8") as f:
+        f.write(jsonl_data)
+
+    logger.debug(f"Wrote jsonl data to {output_path}")
+
+
 def compress_jsonl_data(jsonl_data, output_path):
     # Create output directory, if it doesn't exist
     output_path.parent.mkdir(parents=True, exist_ok=True)
 
     with gzip.open(output_path, "wt", encoding="utf-8") as gzip_file:
         gzip_file.write(jsonl_data)
```

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/utils/models.py` & `khoj_assistant-0.8.3.dev8/src/khoj/utils/models.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/utils/rawconfig.py` & `khoj_assistant-0.8.3.dev8/src/khoj/utils/rawconfig.py`

 * *Files 4% similar despite different names*

```diff
@@ -115,19 +115,18 @@
 
 
 class AppConfig(ConfigBase):
     should_log_telemetry: bool
 
 
 class FullConfig(ConfigBase):
-    content_type: Optional[ContentConfig] = None
-    search_type: Optional[SearchConfig] = None
-    processor: Optional[ProcessorConfig] = None
+    content_type: Optional[ContentConfig]
+    search_type: Optional[SearchConfig]
+    processor: Optional[ProcessorConfig]
     app: Optional[AppConfig] = AppConfig(should_log_telemetry=True)
-    version: Optional[str] = None
 
 
 class SearchResponse(ConfigBase):
     entry: str
     score: str
     additional: Optional[dict]
```

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/utils/state.py` & `khoj_assistant-0.8.3.dev8/src/khoj/utils/state.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,30 +5,29 @@
 
 # External Packages
 import torch
 from pathlib import Path
 
 # Internal Packages
 from khoj.utils import config as utils_config
-from khoj.utils.config import ContentIndex, SearchModels, ProcessorConfigModel
+from khoj.utils.config import SearchModels, ProcessorConfigModel
 from khoj.utils.helpers import LRU
 from khoj.utils.rawconfig import FullConfig
 
 # Application Global State
 config = FullConfig()
-search_models = SearchModels()
-content_index = ContentIndex()
+model = SearchModels()
 processor_config = ProcessorConfigModel()
 config_file: Path = None
 verbose: int = 0
 host: str = None
 port: int = None
 cli_args: List[str] = None
 query_cache = LRU()
-config_lock = threading.Lock()
+search_index_lock = threading.Lock()
 SearchType = utils_config.SearchType
 telemetry: List[Dict[str, str]] = []
 previous_query: str = None
 demo: bool = False
 
 if torch.cuda.is_available():
     # Use CUDA GPU
```

### Comparing `khoj_assistant-0.8.3.dev42/src/khoj/utils/yaml.py` & `khoj_assistant-0.8.3.dev8/src/khoj/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev42/.gitignore` & `khoj_assistant-0.8.3.dev8/.gitignore`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev42/LICENSE` & `khoj_assistant-0.8.3.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev42/README.md` & `khoj_assistant-0.8.3.dev8/README.md`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev42/pyproject.toml` & `khoj_assistant-0.8.3.dev8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     "fastapi == 0.77.1",
     "jinja2 == 3.1.2",
     "openai >= 0.27.0",
     "tiktoken >= 0.3.0",
     "tenacity >= 8.2.2",
     "pillow == 9.3.0",
     "pydantic >= 1.10.10",
-    "pyside6 >= 6.5.1",
+    "pyqt6 == 6.3.1",
     "pyyaml == 6.0",
     "rich >= 13.3.1",
     "schedule == 1.1.0",
     "sentence-transformers == 2.2.2",
     "torch >= 2.0.1",
     "uvicorn == 0.17.6",
     "aiohttp == 3.8.4",
```

### Comparing `khoj_assistant-0.8.3.dev42/PKG-INFO` & `khoj_assistant-0.8.3.dev8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khoj-assistant
-Version: 0.8.3.dev42
+Version: 0.8.3.dev8
 Summary: An AI personal assistant for your Digital Brain
 Project-URL: Homepage, https://github.com/khoj-ai/khoj#readme
 Project-URL: Issues, https://github.com/khoj-ai/khoj/issues
 Project-URL: Discussions, https://github.com/khoj-ai/khoj/discussions
 Project-URL: Releases, https://github.com/khoj-ai/khoj/releases
 Author: Debanjum Singh Solanky, Saba Imran
 License-Expression: GPL-3.0-or-later
@@ -30,15 +30,15 @@
 Requires-Dist: fastapi==0.77.1
 Requires-Dist: jinja2==3.1.2
 Requires-Dist: langchain>=0.0.187
 Requires-Dist: openai>=0.27.0
 Requires-Dist: pillow==9.3.0
 Requires-Dist: pydantic>=1.10.10
 Requires-Dist: pypdf>=3.9.0
-Requires-Dist: pyside6>=6.5.1
+Requires-Dist: pyqt6==6.3.1
 Requires-Dist: pyyaml==6.0
 Requires-Dist: requests>=2.26.0
 Requires-Dist: rich>=13.3.1
 Requires-Dist: schedule==1.1.0
 Requires-Dist: sentence-transformers==2.2.2
 Requires-Dist: tenacity>=8.2.2
 Requires-Dist: tiktoken>=0.3.0
```

