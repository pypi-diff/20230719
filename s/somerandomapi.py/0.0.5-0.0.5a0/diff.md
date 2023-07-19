# Comparing `tmp/somerandomapi.py-0.0.5.tar.gz` & `tmp/somerandomapi.py-0.0.5a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "somerandomapi.py-0.0.5.tar", last modified: Wed Jul 19 15:11:18 2023, max compression
+gzip compressed data, was "somerandomapi.py-0.0.5a0.tar", last modified: Wed Jul 19 14:59:05 2023, max compression
```

## Comparing `somerandomapi.py-0.0.5.tar` & `somerandomapi.py-0.0.5a0.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:11:18.372500 somerandomapi.py-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    16724 2023-07-19 15:11:10.000000 somerandomapi.py-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21232 2023-07-19 15:11:18.372500 somerandomapi.py-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-19 15:11:10.000000 somerandomapi.py-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-07-19 15:11:10.000000 somerandomapi.py-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 15:11:18.372500 somerandomapi.py-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:11:18.368500 somerandomapi.py-0.0.5/somerandomapi/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-19 15:11:10.000000 somerandomapi.py-0.0.5/somerandomapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:11:18.368500 somerandomapi.py-0.0.5/somerandomapi/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-19 15:11:10.000000 somerandomapi.py-0.0.5/somerandomapi/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-07-19 15:11:10.000000 somerandomapi.py-0.0.5/somerandomapi/clients/animal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-07-19 15:11:10.000000 somerandomapi.py-0.0.5/somerandomapi/clients/animu.py
--rw-r--r--   0 runner    (1001) docker     (123)    16826 2023-07-19 15:11:10.000000 somerandomapi.py-0.0.5/somerandomapi/clients/canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-07-19 15:11:10.000000 somerandomapi.py-0.0.5/somerandomapi/clients/chatbot.py
--rw-r--r--   0 runner    (1001) docker     (123)    13656 2023-07-19 15:11:10.000000 somerandomapi.py-0.0.5/somerandomapi/clients/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-07-19 15:11:10.000000 somerandomapi.py-0.0.5/somerandomapi/clients/pokemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-07-19 15:11:10.000000 somerandomapi.py-0.0.5/somerandomapi/clients/premium.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-07-19 15:11:10.000000 somerandomapi.py-0.0.5/somerandomapi/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-07-19 15:11:10.000000 somerandomapi.py-0.0.5/somerandomapi/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:11:18.372500 somerandomapi.py-0.0.5/somerandomapi/internals/
--rw-r--r--   0 runner    (1001) docker     (123)    17262 2023-07-19 15:11:10.000000 somerandomapi.py-0.0.5/somerandomapi/internals/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-07-19 15:11:10.000000 somerandomapi.py-0.0.5/somerandomapi/internals/http.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:11:18.372500 somerandomapi.py-0.0.5/somerandomapi/models/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-19 15:11:10.000000 somerandomapi.py-0.0.5/somerandomapi/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-07-19 15:11:10.000000 somerandomapi.py-0.0.5/somerandomapi/models/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-19 15:11:10.000000 somerandomapi.py-0.0.5/somerandomapi/models/animal_fact.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-19 15:11:10.000000 somerandomapi.py-0.0.5/somerandomapi/models/animu_quote.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-19 15:11:10.000000 somerandomapi.py-0.0.5/somerandomapi/models/chatbot.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-19 15:11:10.000000 somerandomapi.py-0.0.5/somerandomapi/models/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-19 15:11:10.000000 somerandomapi.py-0.0.5/somerandomapi/models/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-07-19 15:11:10.000000 somerandomapi.py-0.0.5/somerandomapi/models/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-19 15:11:10.000000 somerandomapi.py-0.0.5/somerandomapi/models/lyrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-19 15:11:10.000000 somerandomapi.py-0.0.5/somerandomapi/models/namecard.py
--rw-r--r--   0 runner    (1001) docker     (123)    13535 2023-07-19 15:11:10.000000 somerandomapi.py-0.0.5/somerandomapi/models/pokemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-07-19 15:11:10.000000 somerandomapi.py-0.0.5/somerandomapi/models/rankcard.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-19 15:11:10.000000 somerandomapi.py-0.0.5/somerandomapi/models/rgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-19 15:11:10.000000 somerandomapi.py-0.0.5/somerandomapi/models/tweet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:11:18.372500 somerandomapi.py-0.0.5/somerandomapi/models/welcome/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-19 15:11:10.000000 somerandomapi.py-0.0.5/somerandomapi/models/welcome/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-19 15:11:10.000000 somerandomapi.py-0.0.5/somerandomapi/models/welcome/free.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-19 15:11:10.000000 somerandomapi.py-0.0.5/somerandomapi/models/welcome/premium.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-19 15:11:10.000000 somerandomapi.py-0.0.5/somerandomapi/models/youtube_comment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:11:18.372500 somerandomapi.py-0.0.5/somerandomapi/types/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-19 15:11:10.000000 somerandomapi.py-0.0.5/somerandomapi/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-19 15:11:10.000000 somerandomapi.py-0.0.5/somerandomapi/types/animal.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-19 15:11:10.000000 somerandomapi.py-0.0.5/somerandomapi/types/animu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:11:18.372500 somerandomapi.py-0.0.5/somerandomapi/types/canvas/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-19 15:11:10.000000 somerandomapi.py-0.0.5/somerandomapi/types/canvas/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-19 15:11:10.000000 somerandomapi.py-0.0.5/somerandomapi/types/canvas/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-19 15:11:10.000000 somerandomapi.py-0.0.5/somerandomapi/types/canvas/overlay.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-19 15:11:10.000000 somerandomapi.py-0.0.5/somerandomapi/types/chatbot.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-19 15:11:10.000000 somerandomapi.py-0.0.5/somerandomapi/types/facts.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-19 15:11:10.000000 somerandomapi.py-0.0.5/somerandomapi/types/http.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-19 15:11:10.000000 somerandomapi.py-0.0.5/somerandomapi/types/img.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-19 15:11:10.000000 somerandomapi.py-0.0.5/somerandomapi/types/others.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-19 15:11:10.000000 somerandomapi.py-0.0.5/somerandomapi/types/pokemon.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-19 15:11:10.000000 somerandomapi.py-0.0.5/somerandomapi/types/premium.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-19 15:11:10.000000 somerandomapi.py-0.0.5/somerandomapi/types/welcome.py
--rw-r--r--   0 runner    (1001) docker     (123)     9167 2023-07-19 15:11:10.000000 somerandomapi.py-0.0.5/somerandomapi/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:11:18.368500 somerandomapi.py-0.0.5/somerandomapi.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21232 2023-07-19 15:11:18.000000 somerandomapi.py-0.0.5/somerandomapi.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-19 15:11:18.000000 somerandomapi.py-0.0.5/somerandomapi.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 15:11:18.000000 somerandomapi.py-0.0.5/somerandomapi.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-19 15:11:18.000000 somerandomapi.py-0.0.5/somerandomapi.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-19 15:11:18.000000 somerandomapi.py-0.0.5/somerandomapi.py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:59:05.809629 somerandomapi.py-0.0.5a0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16724 2023-07-19 14:58:56.000000 somerandomapi.py-0.0.5a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21234 2023-07-19 14:59:05.809629 somerandomapi.py-0.0.5a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-19 14:58:56.000000 somerandomapi.py-0.0.5a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-07-19 14:58:56.000000 somerandomapi.py-0.0.5a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 14:59:05.809629 somerandomapi.py-0.0.5a0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:59:05.801629 somerandomapi.py-0.0.5a0/somerandomapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-19 14:58:56.000000 somerandomapi.py-0.0.5a0/somerandomapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:59:05.805629 somerandomapi.py-0.0.5a0/somerandomapi/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-19 14:58:56.000000 somerandomapi.py-0.0.5a0/somerandomapi/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-07-19 14:58:56.000000 somerandomapi.py-0.0.5a0/somerandomapi/clients/animal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-07-19 14:58:56.000000 somerandomapi.py-0.0.5a0/somerandomapi/clients/animu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16826 2023-07-19 14:58:56.000000 somerandomapi.py-0.0.5a0/somerandomapi/clients/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-07-19 14:58:56.000000 somerandomapi.py-0.0.5a0/somerandomapi/clients/chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13656 2023-07-19 14:58:56.000000 somerandomapi.py-0.0.5a0/somerandomapi/clients/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-07-19 14:58:56.000000 somerandomapi.py-0.0.5a0/somerandomapi/clients/pokemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-07-19 14:58:56.000000 somerandomapi.py-0.0.5a0/somerandomapi/clients/premium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-07-19 14:58:56.000000 somerandomapi.py-0.0.5a0/somerandomapi/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-07-19 14:58:56.000000 somerandomapi.py-0.0.5a0/somerandomapi/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:59:05.805629 somerandomapi.py-0.0.5a0/somerandomapi/internals/
+-rw-r--r--   0 runner    (1001) docker     (123)    17262 2023-07-19 14:58:56.000000 somerandomapi.py-0.0.5a0/somerandomapi/internals/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-07-19 14:58:56.000000 somerandomapi.py-0.0.5a0/somerandomapi/internals/http.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:59:05.805629 somerandomapi.py-0.0.5a0/somerandomapi/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-19 14:58:56.000000 somerandomapi.py-0.0.5a0/somerandomapi/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-07-19 14:58:56.000000 somerandomapi.py-0.0.5a0/somerandomapi/models/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-19 14:58:56.000000 somerandomapi.py-0.0.5a0/somerandomapi/models/animal_fact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-19 14:58:56.000000 somerandomapi.py-0.0.5a0/somerandomapi/models/animu_quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-19 14:58:56.000000 somerandomapi.py-0.0.5a0/somerandomapi/models/chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-19 14:58:56.000000 somerandomapi.py-0.0.5a0/somerandomapi/models/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-19 14:58:56.000000 somerandomapi.py-0.0.5a0/somerandomapi/models/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-07-19 14:58:56.000000 somerandomapi.py-0.0.5a0/somerandomapi/models/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-19 14:58:56.000000 somerandomapi.py-0.0.5a0/somerandomapi/models/lyrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-19 14:58:56.000000 somerandomapi.py-0.0.5a0/somerandomapi/models/namecard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13535 2023-07-19 14:58:56.000000 somerandomapi.py-0.0.5a0/somerandomapi/models/pokemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-07-19 14:58:56.000000 somerandomapi.py-0.0.5a0/somerandomapi/models/rankcard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-19 14:58:56.000000 somerandomapi.py-0.0.5a0/somerandomapi/models/rgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-19 14:58:56.000000 somerandomapi.py-0.0.5a0/somerandomapi/models/tweet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:59:05.805629 somerandomapi.py-0.0.5a0/somerandomapi/models/welcome/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-19 14:58:56.000000 somerandomapi.py-0.0.5a0/somerandomapi/models/welcome/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-19 14:58:56.000000 somerandomapi.py-0.0.5a0/somerandomapi/models/welcome/free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-19 14:58:56.000000 somerandomapi.py-0.0.5a0/somerandomapi/models/welcome/premium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-19 14:58:56.000000 somerandomapi.py-0.0.5a0/somerandomapi/models/youtube_comment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:59:05.809629 somerandomapi.py-0.0.5a0/somerandomapi/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-19 14:58:56.000000 somerandomapi.py-0.0.5a0/somerandomapi/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-19 14:58:56.000000 somerandomapi.py-0.0.5a0/somerandomapi/types/animal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-19 14:58:56.000000 somerandomapi.py-0.0.5a0/somerandomapi/types/animu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:59:05.809629 somerandomapi.py-0.0.5a0/somerandomapi/types/canvas/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-19 14:58:56.000000 somerandomapi.py-0.0.5a0/somerandomapi/types/canvas/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-19 14:58:56.000000 somerandomapi.py-0.0.5a0/somerandomapi/types/canvas/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-19 14:58:56.000000 somerandomapi.py-0.0.5a0/somerandomapi/types/canvas/overlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-19 14:58:56.000000 somerandomapi.py-0.0.5a0/somerandomapi/types/chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-19 14:58:56.000000 somerandomapi.py-0.0.5a0/somerandomapi/types/facts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-19 14:58:56.000000 somerandomapi.py-0.0.5a0/somerandomapi/types/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-19 14:58:56.000000 somerandomapi.py-0.0.5a0/somerandomapi/types/img.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-19 14:58:56.000000 somerandomapi.py-0.0.5a0/somerandomapi/types/others.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-19 14:58:56.000000 somerandomapi.py-0.0.5a0/somerandomapi/types/pokemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-19 14:58:56.000000 somerandomapi.py-0.0.5a0/somerandomapi/types/premium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-19 14:58:56.000000 somerandomapi.py-0.0.5a0/somerandomapi/types/welcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9167 2023-07-19 14:58:56.000000 somerandomapi.py-0.0.5a0/somerandomapi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:59:05.801629 somerandomapi.py-0.0.5a0/somerandomapi.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21234 2023-07-19 14:59:05.000000 somerandomapi.py-0.0.5a0/somerandomapi.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-19 14:59:05.000000 somerandomapi.py-0.0.5a0/somerandomapi.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 14:59:05.000000 somerandomapi.py-0.0.5a0/somerandomapi.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-19 14:59:05.000000 somerandomapi.py-0.0.5a0/somerandomapi.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-19 14:59:05.000000 somerandomapi.py-0.0.5a0/somerandomapi.py.egg-info/top_level.txt
```

### Comparing `somerandomapi.py-0.0.5/LICENSE` & `somerandomapi.py-0.0.5a0/LICENSE`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.5/PKG-INFO` & `somerandomapi.py-0.0.5a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: somerandomapi.py
-Version: 0.0.5
+Version: 0.0.5a0
 Summary: A maintained wrapper for the somerandomapi API.
 Author: Soheab_
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
```

### Comparing `somerandomapi.py-0.0.5/pyproject.toml` & `somerandomapi.py-0.0.5a0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.5/somerandomapi/clients/__init__.py` & `somerandomapi.py-0.0.5a0/somerandomapi/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.5/somerandomapi/clients/animal.py` & `somerandomapi.py-0.0.5a0/somerandomapi/clients/animal.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.5/somerandomapi/clients/animu.py` & `somerandomapi.py-0.0.5a0/somerandomapi/clients/animu.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.5/somerandomapi/clients/canvas.py` & `somerandomapi.py-0.0.5a0/somerandomapi/clients/canvas.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.5/somerandomapi/clients/chatbot.py` & `somerandomapi.py-0.0.5a0/somerandomapi/clients/chatbot.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.5/somerandomapi/clients/client.py` & `somerandomapi.py-0.0.5a0/somerandomapi/clients/client.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.5/somerandomapi/clients/pokemon.py` & `somerandomapi.py-0.0.5a0/somerandomapi/clients/pokemon.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.5/somerandomapi/clients/premium.py` & `somerandomapi.py-0.0.5a0/somerandomapi/clients/premium.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.5/somerandomapi/enums.py` & `somerandomapi.py-0.0.5a0/somerandomapi/enums.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.5/somerandomapi/errors.py` & `somerandomapi.py-0.0.5a0/somerandomapi/errors.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.5/somerandomapi/internals/endpoints.py` & `somerandomapi.py-0.0.5a0/somerandomapi/internals/endpoints.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.5/somerandomapi/internals/http.py` & `somerandomapi.py-0.0.5a0/somerandomapi/internals/http.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.5/somerandomapi/models/abc.py` & `somerandomapi.py-0.0.5a0/somerandomapi/models/abc.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.5/somerandomapi/models/dictionary.py` & `somerandomapi.py-0.0.5a0/somerandomapi/models/dictionary.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.5/somerandomapi/models/encoding.py` & `somerandomapi.py-0.0.5a0/somerandomapi/models/encoding.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.5/somerandomapi/models/image.py` & `somerandomapi.py-0.0.5a0/somerandomapi/models/image.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.5/somerandomapi/models/lyrics.py` & `somerandomapi.py-0.0.5a0/somerandomapi/models/lyrics.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.5/somerandomapi/models/namecard.py` & `somerandomapi.py-0.0.5a0/somerandomapi/models/namecard.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.5/somerandomapi/models/pokemon.py` & `somerandomapi.py-0.0.5a0/somerandomapi/models/pokemon.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.5/somerandomapi/models/rankcard.py` & `somerandomapi.py-0.0.5a0/somerandomapi/models/rankcard.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.5/somerandomapi/models/rgb.py` & `somerandomapi.py-0.0.5a0/somerandomapi/models/rgb.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.5/somerandomapi/models/tweet.py` & `somerandomapi.py-0.0.5a0/somerandomapi/models/tweet.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.5/somerandomapi/models/welcome/free.py` & `somerandomapi.py-0.0.5a0/somerandomapi/models/welcome/free.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.5/somerandomapi/models/welcome/premium.py` & `somerandomapi.py-0.0.5a0/somerandomapi/models/welcome/premium.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.5/somerandomapi/models/youtube_comment.py` & `somerandomapi.py-0.0.5a0/somerandomapi/models/youtube_comment.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.5/somerandomapi/types/pokemon.py` & `somerandomapi.py-0.0.5a0/somerandomapi/types/pokemon.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.5/somerandomapi/utils.py` & `somerandomapi.py-0.0.5a0/somerandomapi/utils.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.5/somerandomapi.py.egg-info/PKG-INFO` & `somerandomapi.py-0.0.5a0/somerandomapi.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: somerandomapi.py
-Version: 0.0.5
+Version: 0.0.5a0
 Summary: A maintained wrapper for the somerandomapi API.
 Author: Soheab_
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
```

### Comparing `somerandomapi.py-0.0.5/somerandomapi.py.egg-info/SOURCES.txt` & `somerandomapi.py-0.0.5a0/somerandomapi.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

